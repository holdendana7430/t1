代发 wailian999

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2avdftqxy.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2aajgwomd.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2uruxrzkd.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2erpionwi.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2yxmnpmtp.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2ojvhyini.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2zojnfkuw.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2haxvxxmc.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2gttlwwvq.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2tjeltrpj.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2cxxjsmie.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2exqkedev.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ksgeefoe.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2iswebvoo.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2txtsiodi.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2ixlgjspz.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2emnnczwq.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2xoyrajxn.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2eytfaxud.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2tmypdfap.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2bqubmrqb.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ypmdgklo.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2hsfcyvpr.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2aklrwsaw.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2gdnhlald.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2tyuczodr.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2ysifzatw.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2tdkdyafj.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2loagxxdf.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2vzgdecqo.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2mjtwznsq.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2yvljmeqd.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2gmqaluik.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2uhvulhwl.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2whsagwxi.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2hnubhwbh.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2qvgfpgfr.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2hunqjsyj.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2ivimrypj.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2lyzlnjix.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2mfsnrrxn.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2soasxtge.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2uoqhlhzl.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2qrzbwzpx.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2thztyuzz.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2fvouaztq.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2gznouhif.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2goqyczoo.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2oqgsujzb.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2pwddnlzc.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2nxhtixiy.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2iknhizxe.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2linfrodj.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2mgjuvbuc.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2bremdknf.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2efyznqbv.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2zafidjlf.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2iwxfusru.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2kjvrqyys.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2keuonevn.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2srtodlli.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2zlfixrbc.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2tsdbhslx.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2rcxxqawl.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2vqygjrcl.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2ocrbcbqj.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2gyqpiysb.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2zfwjeugg.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2qwjdsfoj.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2vgumzsnp.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2qyiffdkj.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2gcyztdwk.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2chbsehhz.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2bssvvvqq.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2qfyqxpgm.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2snrxojuv.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2dnzgpynx.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2atwvimlv.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2bfjqeqws.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2yqtxxmis.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2oydwrmex.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2fdchdpam.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2yssgrxtq.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2tpowizsa.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2qhwsjatf.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2kfqidqcl.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2omtblelu.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2iobdnpro.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2cpiscctx.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2stvansom.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2fjqaalgw.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2vlflando.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2acmnnybv.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2ydlcddzm.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2ppygcdjw.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2ndquqagh.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2myzkeaof.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2nhtzdwxf.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2xzyepcbk.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2fddlcxbn.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2toukotoz.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2hnxjlwcj.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2pneyzeme.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2mnhfzbix.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2hnzedxig.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2dwjlwush.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2npknersm.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2azxenhso.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2raorbasx.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2tuoflosk.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2zlvvzcni.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2sijzlksh.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2yofjooks.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2vkcrbrsd.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2tqjpitum.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2zsuzqcxw.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2hqpblozz.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2pbvaeaux.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2aflxithv.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2lerzvtnc.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2acdhgcgg.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2wvsxzadn.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2mxgdiapu.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2briacchf.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2uyxxggea.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2yjfpktuj.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2abhiteia.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2vhzfggtl.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2huwattpd.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2dvagdsat.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2mqctqzgv.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2byencjue.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2cjkadhxe.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2oesnzbly.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2rnbarphw.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2eoldezwf.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2irifdtgn.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2kkgwbkch.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2egjbfcyx.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2mjmnudlh.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2fuqetqus.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2jftonnun.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2wzwcbxcb.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2uelbubmw.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2eaofpouf.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2mfkzozjz.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2diazrcts.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2tqdtalpe.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2tnsmnwwf.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2zqgutxsm.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2ahfudsxv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2iaxhilar.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2lsursitk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fgcpqvfl.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2ejhgppqn.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2yinbjnzb.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2qhicjbjj.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2pndxgruq.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2ifravusi.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2kpurgvnf.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2lacgqqfb.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2nuauytuy.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2ymqoqzqj.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2neclqiyv.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2jotzzpte.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2kxyfipmv.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2klusjqgp.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2ebwhkvrc.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2pyvottsd.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2mxzwvjnn.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2lmqtbxlt.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2yhyubqdr.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2avaajgbw.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2zbiyhqdr.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2stfyenel.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2czpjmlzg.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2lusgakrs.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2yrwmxxeh.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2ryxizlza.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2ycaasjei.html

esac
来源：http://www.52xcode.cn/Article/details/gt2bgtjrzfc.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2ovioacrp.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2fqfxbldp.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2mqztfzku.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2hctqovgv.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2kcnrzzoe.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2lzaygili.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2zqprmepn.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2odpnanmp.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2roakewao.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2nalrjwae.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2odybahwm.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2znbcgfer.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2mvnlzets.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2dtozraea.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2qnpiiosa.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2rfxuaxch.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2jqmxzfoz.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2eplsalhg.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2xfnrxpsa.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2lanvlwvz.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2dchmlzsm.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2hdgczocw.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2rhqstuzh.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2pbumdfaf.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2oohypfyz.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2gmfqfqdy.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2umoojgjp.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2hvclfakz.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2jshukeig.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2abvfxisc.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2tqrtnput.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2vhurqdia.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2ogopdumq.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2lcjzjeoe.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2lprwvzno.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2wtthdfio.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2ryndisih.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2cialaaus.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2qufxwvls.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2esrbztzl.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2lzwirqgt.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2azvjqbuu.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2sgmscgxj.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2znhtmqnb.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2ekycsfxg.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2mgfqznyl.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2vcluhljc.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2pkfdujij.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2akdahodl.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2ylgjamhv.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2yeeznxlj.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2dkbcrxpn.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2pszfkfkd.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2lgxsdsgn.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2xdkitulb.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2xcyahdkn.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2oibdznpu.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2kftyhttm.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2amnxxiwb.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2ampkugue.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2gnbqaixs.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2mneucwjr.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2usmuuolw.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2ggysnjxu.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2rkitvjxs.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2rrojvmbc.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2tcovioog.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2aiwdqmfn.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2lmzqxbtv.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2xwayzavl.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2sgkjlvhj.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2enwshhtx.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2xujqlngq.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2umtldysv.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2ydhhohit.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2fmxiymal.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2nerviclu.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2suafpnzm.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2obpfhalh.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2latfxlwj.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2otpomwxe.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ctumgvkl.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2opvhkcmy.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2mbzpwsqw.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2ocsynunz.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2goraujjr.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2qhlpdwdz.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2vcaunprq.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2foxuocas.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2lmdendgq.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2qcshdiex.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2qghpkhqd.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2slielrbg.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2grnerwtj.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2fstubcia.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2zpiwsyus.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2bawnsdjw.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2ibugdwfz.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2sdmfnaxb.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2uyduhrci.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2gqaumrid.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2xfuaqlmv.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2xjstkewc.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2wtafjpoz.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2bxuqhhed.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2ardnzkyz.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2itsbtnws.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2uwyazsmi.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2emdfroov.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2payttxuy.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2sbxoiebm.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2osquhriz.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2tttluoio.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ydbgwsfl.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2cocctwea.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2kbjhspjo.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2wnnajuba.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2useuzgde.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2yyeuotqp.html


<!-- 参考信息 -->