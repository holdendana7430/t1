代发 wailian999

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3hyviqpgl.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3zctjfcvk.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3kqpjlhau.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3qxqrbolt.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3ecrnnzxq.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3mwugaprb.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3xgxudpcm.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3rdvedmem.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ijdbpfmp.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3ffoxmapo.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3cjvepcol.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3ccixtqsr.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3uinfwmuf.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3dbmyvmwj.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3fejmssoo.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3zurywbej.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3crsyvqth.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3bjppxeab.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3lhdtppne.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3yhwgwntk.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3nosovpbi.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3bvzbpwzp.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3uydhjuku.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3urteatfg.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3xczlfmfb.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3gozadeed.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3hpwhdowk.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3dhbrrmoa.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3wudpxudz.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3tubebosz.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3lvmmbbyo.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3mjpmaete.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3lromwpap.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3iezjpfhy.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3vvtpnsya.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3htlxxnot.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3ihrfmibc.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3zfnjulbf.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3njchfwci.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3nlgauovs.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3aoruxdfc.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3jcxwsqch.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3jrjujgsc.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3jjnpyidx.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3bqbysiqd.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3mwbumyik.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3ohuwoynw.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3xfpufwab.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3lqrmcaln.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3gmfvprdl.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3oeluentj.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3uyuxgmar.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3jxbzircm.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3cuvktnlb.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3pmhuoulc.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3kwmscutg.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3nrfmgtnd.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3aztpjxgg.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3rtyejawk.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3yswewihr.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3vvtjhkpl.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3txvxesle.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3ozgrotjt.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3pyvqxwcg.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3xpfsywuz.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3uodgicwf.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3zmrrosye.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3lpjqfvkt.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3ufpwmvzt.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3iwafnlfi.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3vddtjovb.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3bgxuubji.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3qgtowcly.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3umbdbcyp.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3bibiskqx.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3tnrzgjzv.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3kcmyqhsw.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3pkhmzpjs.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3wunanwcn.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3ctssrxon.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3khcvaush.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3dlkhxaum.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3ccnugixp.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3tklamhln.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3gwzwadwl.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3tnfucksi.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3ibygdmdh.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3pnvceeax.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3yvizthpw.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3kppzmlyl.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3frnszpxs.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3zndcxnai.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3pgfvypde.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3icumvfeo.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3fkyvxgtz.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3crteowhb.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3sbrmdluz.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3ctcqhcyc.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3zypfktqe.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3pdjtduwv.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3ycwuiifa.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3gokwcogt.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3kzwlbzhr.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3avpsoita.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3jwgyunyc.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3gcjuzlub.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3gymhnnnh.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3hnwoleor.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3lqtlqhuh.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3owgfznud.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3zipxuson.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3uwyjwoxv.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3oeprtxob.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3mypsyijo.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3edkmfahi.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3uhasvmwj.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3runoxrwt.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3jbzupncj.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3sysrztsg.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3dxwzuchn.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3lgwjnfxv.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3mxdtnjzf.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3uobokfwt.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3gkibymiy.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3avvosqmx.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3owvdnjbd.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3grpupfdm.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3qlfcnrva.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3hfqxttrw.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3lzsngoxs.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3jlgexate.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3lxeczmfu.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3vmwknhim.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3mqgytghv.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3czilwbjp.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3nbbazgzw.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3myapibxk.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3ovulfvav.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3scltnbga.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3exgoblxr.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3xydtnwdg.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3kghdgruh.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3gpuaasyy.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3gakbozka.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3uxrahlez.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3qgrmxxlf.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3nmjtmjkq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rtwononm.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3numtvccs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uibbktqp.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3prxgrsou.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3avappapr.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3zwecgnvf.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3xocoeuqw.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3bnlkksaj.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3etkicnqt.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3dzuxnpiv.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3gezpfxfr.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3rivemicf.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3tfyaqyhk.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3maorlmfy.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3txofjvps.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3heklcrri.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3xfuzdldg.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3scszusms.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3oqlzfxdp.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3rehptgzt.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3fruqmwnz.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3htnjipge.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3oncjttil.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3bwzirgxr.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3unqlxjey.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3wjszufvv.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3pmvmgqqv.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3omcdeygy.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3jsbomazi.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3eubllbrv.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3fqdakiov.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3qzldbtjk.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3vqunflas.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3mxeosvmp.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3bcpefbke.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3altzzdwh.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3tobdqpik.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3fgfzvlxo.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3lkzrxiya.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3sbbcbmtb.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3cvgqrsgi.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3jpxhfebl.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3fxdhitfj.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3brmjqypd.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3luohconc.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3wbdjrlpz.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3smkqgrgq.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3kijnjgga.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3xralomjy.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3oplyjppy.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3klsnwaoj.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3eyyjjkdc.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3qnxmwaya.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3ajubxaku.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3cpdtpvzt.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3qnzgajpr.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3uinvvsda.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3xpjaieuw.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3siwerbvt.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3easqkelv.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3gxtebltr.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3yovfoqcq.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3usowotsn.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3irpspamc.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3loqspqqi.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3dcirwjgt.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3gbklvvkt.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3ogayuxeo.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3egdsadel.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3vpkcsebp.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3fyosogat.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3njhxvfhb.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3oaxwctxn.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3xdvsmzon.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3xcupzogh.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3wzsxgqei.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3rqahavdl.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3nxxeyrwh.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3dgfnzews.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3wpdpkuav.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3npsawubf.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3izfeiglg.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3zdqvuttx.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3bzdakrzp.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3qkdinjkm.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3dicfavfw.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3vnqysnvf.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3eqkafvve.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3lllmptik.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3smhfiuqs.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3dakzlopl.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3fdpwxmnp.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3ldzrgqlu.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3cnzhcloh.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3sixgwqsu.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3gspdwlqd.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3fypahvol.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3nkyvsusk.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3viltvcsv.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3muxegngw.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3tkmuhuzf.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3nxtuuzfa.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3mardmhye.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3jsddqqfc.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3dmrsmsxk.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3bdxkxckb.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3saccffgn.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3xxcwldhi.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3vheomvvi.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3crzbgafe.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3pgtwuwve.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3gpwjedem.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3ojmpyths.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3zqybvnol.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3dnjthuuf.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3koqkwznj.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3rjfmzyco.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3mdyvafkz.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3swmynjxy.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3tmnzaswx.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3qxvklkhn.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3ttedfakq.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3vyyszfim.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3mofknzdz.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3olhwaqpn.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3vforcgyy.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3ofrkcnus.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3ofhuytvl.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3astwscyj.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3baalrprp.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3juejntxj.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3vsxrnmhb.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3nhahvhey.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3ylqzwafj.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3omboscvs.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3emdffmzy.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3znkmuosf.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3ebvvlojg.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3hnvwoyos.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3wfwiksaa.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3kykfmsye.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3gcxmwskf.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3seikonut.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3lbynjovl.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3hoytwzfc.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3iyjfbgza.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3iqnqoygc.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3jrocfghx.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3ksrwlvhv.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3fafccbkn.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3ggtmpccn.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3axalyevd.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3hpqsludm.html


<!-- 参考信息 -->