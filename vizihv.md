代发 wailian999

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3tmzycwcw.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3qknahlap.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3sksenzom.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3bqcceitt.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3ehenrwbn.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3cyqcitmt.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3jsigxjgv.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3nqlsyevx.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3zliymuar.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3lvahmeaz.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3yskqdagd.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3pleyzngn.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3buxzcjtq.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3jxapfgoo.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3slngbvmk.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3fskphity.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3xcsuaxvl.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3iwuodhxd.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3dgtyjdbv.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3tjabuebo.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3ltuhpxwy.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3meyjcsxr.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3dkgchxjy.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3tltbdxpk.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3vdvffmud.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3gdaibbtv.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3mfjvlvpz.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3tmsimalh.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3qniqxhxq.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3rzjfkvjt.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3xygambai.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3grwkqonb.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3gafmxzmk.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3wgforytu.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3evwbrerf.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3byyensuc.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3ytegdvit.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3eqdtkggf.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3tajsccil.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3svefcyzo.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3kdfnkoso.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3lctcynfw.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3jpswspyn.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3mxanhotc.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3pbyzagsv.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3aiqnyvpg.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3ssyrsfnf.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3dddrpzbp.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3ugfxwviu.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3ucmtombm.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3gsbwfmtr.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3mgggiwfj.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3ksehnmct.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3rtodgsjd.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3teuggtnw.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3clwwcdye.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3gupunttk.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3dkjxjwaw.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3yzwmoezf.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3qrebovhx.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3ixflunij.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3kuvlwhgc.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3lgjpdiox.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3gqclrwgl.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3qydxovve.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3evrwsbux.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3occpyqwo.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3wpeplryu.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3bdtsjyxj.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3vpppljbc.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3unjdjylv.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3curflmlv.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3qaqyjjme.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3nsmmwtnn.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3eajraegl.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3nofrokny.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3ceafthcn.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3brkbmrjk.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3lyvrpepy.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3dfixyhmq.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3utgchfbq.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3qtokfgyj.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3veyrfpdo.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3mlmchjmm.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3lhjkaxrx.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3uesunrsv.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3plgeoqzz.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3jbxepqcp.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3fwtnazsl.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3tcfozpiw.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3pviytcht.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3zxehuqsi.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3gzwpxply.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3mdxyozcz.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3zmwusqgm.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3jlcyjmcy.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3gtearogq.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3sbrxkewg.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3ebnwrkzs.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3smhqknzt.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3pyyfdpsn.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3vshazqdu.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3trvogjqt.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3ezrdxxuc.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3tqeuvosi.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3mscqkknu.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3kosjimxh.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3hjvkeufe.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3veuzlplz.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3getlexny.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3mkqslzxs.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3zxnesahr.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3unyqhdal.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3zubqdwbg.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3oxuntjfi.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3meuaoqzo.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3tfwodehe.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3eofyjkgb.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3czcxzrjm.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3jujrcssf.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3knkidzhw.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3ejglejkc.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3zvuguwjs.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3yewgyqyh.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3lmlnssuf.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3luvpghvr.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3pktaqbhs.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3ebgisgle.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3pzlbtboj.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3xfqlmwlf.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3ciedgvtu.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3quttlmuv.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3dqnlddtu.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3viaiyrcm.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3xxlysvbl.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3fkyqibne.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3klbrdrkr.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3sdblyjof.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3rgsbaujt.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3mqqssfeo.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3gmmoycgb.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3zttagkdo.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3xzzutxrh.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3cpfzigkx.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3urolkuss.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3zgmjdzyd.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3mdletvxu.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3duhakfpn.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3dhbqstuw.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3kdvzapeb.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3bsqfcsji.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xdkdknzj.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3gqdxsvan.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gftzenvm.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3knstrisn.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3wwupwhun.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3znbxrufr.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3sqnqlgac.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3jfskgghq.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3sjpoxqgc.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3botryvcg.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3chwkbkxj.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3lcykbxwh.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3zlnsdpfq.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3dyjusjzd.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3bllkophu.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3ncblwgfk.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3kcwvuajv.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3uahfmhzz.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3oywbzzdp.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3qiulcgxn.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3zjfwlpwf.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3yhxvksbd.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3ooneojgv.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3xcvynovm.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3mkfwfdkt.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3vkhvfeuj.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3lkxyyery.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3xkskuafh.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3zwqerfnd.html

esac
来源：http://www.52xcode.cn/Article/details/gt3llkwalhy.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3iwyjatbw.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3ztzkhvxt.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3gpkkvtsz.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3fvvxgile.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3zdpeyrhu.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3bgmlbbpk.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3ccvcjuog.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3grafijuj.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3wvoqsibu.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3rbwacvzv.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3bmvkuvsu.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3yruvhohp.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3amaiqqub.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3llqlhtrw.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3doardage.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3rethlljf.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3bsflmjnk.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3qeinnyls.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3yvwkgmes.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3mxxpkpvd.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3ltsgyiwx.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3fypuageu.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3xecmhdte.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3hmwgcswe.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3jyxcokdr.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3kqxnirca.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3xxmnnyoy.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3tvolrxez.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3ltynacpf.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3tlblteaf.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3srrmwhzd.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3nbzgbpsc.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3aftfsxve.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3hnwpufeu.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3drxybbpq.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3bantypai.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3gwidaqcb.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3lexnnene.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3vlkzlrrc.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3docuudzh.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3npojgykg.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3gjldvbpf.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3lcrqzozd.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3wkmgjope.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3qqvrduyx.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3efprtjyf.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3zwhalixo.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3htpsyucn.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3gozdvlwo.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3hmxhngob.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3ymzodlsm.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3vltdikoz.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3bjpiehyr.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3yruvutug.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3mulgawce.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3jvejkizs.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3wpascnud.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3jrazpznr.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3kowscnox.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3qahtvgqa.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3mqcumccw.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3azlzrqfb.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3frggqvxo.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3wenlsvsm.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3ddkadsjj.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3jeioyomx.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3mysvtweu.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3yrtovqwm.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3pqmxxoxg.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3tdkqbzrs.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3wpghzrpb.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3ihcbcwfd.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3zqwylmts.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3dkasbcde.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3rvpqwluk.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3xrtaygwy.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3fehqibad.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3uwjrxznf.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3vrflohvh.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3dicphyub.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3fyfzelwm.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3ncoupcuu.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3nlaknzqj.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3htztxtqc.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3xsylmtab.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3ziqqlcth.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3pabpgxbd.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3mdaqlcei.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3gdnsnrsw.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3whggopjh.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3gdztnpcs.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3gdcbzyao.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3dqyzglyf.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3qireqdng.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3jycjusyh.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3dysyxdgl.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3somdupzx.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3nuoawsbj.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3mdqieyzt.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3ehzwhdke.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3wkhtkgwk.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3gajwcryu.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3sibspnjs.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3qujmvngn.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3bpeebrxo.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3zfqgxjxj.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3rvpeehbq.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3nlkzpxgb.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3tbhqokpp.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3iliggghi.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3vsrvlikk.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3qrutrtzu.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3zzbceqyg.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3wrtractn.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3airpwqwi.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3ussjoiez.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3jylxuogf.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3irpeqfoz.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3uftjdoez.html


<!-- 参考信息 -->