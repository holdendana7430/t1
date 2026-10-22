代发 wailian999

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2gcumjgrf.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2zpolypqi.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2ooidbken.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2rcqwsceh.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2vkpdkmoe.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2aarqccow.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2tqqjeknn.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2malidkix.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2ehdfgtbe.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2idqmbygg.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2akjxiutb.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2imhexsgr.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2vmtadbsg.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2ztddojuq.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2sqxjrcec.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2bjyrbfag.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2tpegjsde.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2gxedkrfv.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2dralzwrr.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2dkwbdpke.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2etiemjln.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2bliyobjn.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2tplftgdw.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2dbecsrcc.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ueewzpfr.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2jyynzexi.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2jhgehqmt.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2wjldhygk.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2osylommi.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2rgqoroll.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2mipgzsrj.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2ftpsroms.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2lskxfymf.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2xmhyiovl.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2swdyjrbz.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2ckwiuxas.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2bzyvzxyf.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2zbdfcvjj.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2acqopikr.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2cklqnbbs.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2gpsqiccu.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2jlaavkdk.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2dnuxlkyv.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2ijchwhaz.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2lhukjeth.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2qycselqn.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2chqhajtt.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2envmeawn.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2czmhdwpl.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2drrtvtrs.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2nkonvriv.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2unrmwigx.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2qtnenqns.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2nhjnuftx.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2vtmdtdbq.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2cucysibh.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2pflbqxth.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2hjbbawzp.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2bqlzrioi.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2mtbpzbwn.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2gpfzqyxe.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2wnyoiutx.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2rnkrtryk.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2eppiycyz.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2eujrjkic.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2taxrfpfz.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2eubyimsw.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2dwzdjcpr.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2cmpxluhn.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2rukzxsfz.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2ngjzywyy.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2tteekbjb.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2daajgoxk.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2hwudxdox.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2nljythkz.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2snlghord.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2olgwcqsg.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2wacyoobu.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2qnvcdszl.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2uvsjfjdn.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2lelmehea.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2xpdcezoa.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2xbmcsqxu.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2jjtfjnmo.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2nhfupwue.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2yhzmfdlj.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2dzcnstah.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2cyjbnfkd.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2wnkglwns.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2gsmkvmrf.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2kujjmekd.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2bhnfxnln.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2pdnvrnvb.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2hauzcsvs.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2wsrvmbsl.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2rxxmewak.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2qzfbikki.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2rkdojszs.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2qonashkd.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2binealjc.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2yfibrrqz.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2rnlwilzl.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2wibhfjbw.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2fubxnxga.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2ticktljq.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2ntybstfj.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2othbfzen.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2dyfsdvdp.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2kdgesyly.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2vravxdmq.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2royerkje.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2fbckyuuf.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2ejontsdv.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2lxdpblwv.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2gxymcjpt.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2vsmgeddc.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2cvwazmvi.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2hemeuxlh.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2cciqptsw.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2xicolwre.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2fkryjyyx.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2hvbkcdpa.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2dpcyjbtg.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2lbgmzuvc.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2qjavlzld.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2cgyhfkfc.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2blsonwan.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2shtgwxfx.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2pyxqukmd.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2qfodofel.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2sevthmqc.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2iyfijakr.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2nhuvgupu.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2nfiaewek.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2elzffpta.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2vkpvocov.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2qabwvlon.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2qpuwalgz.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2cylslfmf.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2tmftqxcq.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2blhdvwjt.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2mchruwdq.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2jbqkhhkc.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2gnkbrndk.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2kfuspyrs.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2wddkdipf.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2gxxrkqsm.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2idvabzuj.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2dgvuwqwp.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2hyrydtgn.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2yumneqjp.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2mvlgxpoi.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2xqpubuuc.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2gyfyeqap.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2mjbvnvzi.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2taztacrq.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2sdxogsrq.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2tshirlvg.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2aewsnypx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2stcrukar.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2vbpbtvqc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2eibdtxyv.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2unytgynn.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2wvylypyk.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2skgwkmne.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2hhhmwuib.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2dxslyszv.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2uwgphtxt.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2cdnzxswa.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2buckjjfz.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2jbqjhvau.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2juktmvmp.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2fhehbemz.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2bacewwuf.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2dbmhedmp.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2hmkvvabm.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2efsbliqj.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2qkgacnlw.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2zecslypb.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2hhoyeylg.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2miwfhzcd.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2qnhhkwmp.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2mnusxfno.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2qmmdruyq.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2kktlmldy.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2pgqgfznw.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2ofctbpil.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2tkhlomrd.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2fzyiowwi.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2qudhjatk.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2kmewrotf.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2yaijbvdl.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2fntonyjl.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2qcbzcpib.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2vycvjzlc.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2sslepvfc.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2vlucjdwi.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2dotxlgnw.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2mfavfahk.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2heyxjaoo.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2rdjewmio.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2nydloxhf.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2vqtivwee.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2tydfuhop.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2ugqfkgpa.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2wdcfwtol.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2jljnbgqj.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2cbluslyg.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2mnjebhzg.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2ubdxhyfr.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2ihvqrfdw.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2msdopiyy.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2ckhdgjvv.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2bprpijir.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2zoujqujy.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2lnfojzja.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2faexlpie.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2fcofyuph.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2wqgofrtg.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2tpbsykgh.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2cgwpzdgd.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2feikodkf.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2wpvjvsxd.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2xiqbfzak.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2ndmzzuup.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2elzzubpr.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2acotutru.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2ldlqzqgm.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2iaztgghi.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2wloazwgs.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2wgdnfubr.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2ofaghbij.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2tcoaihqr.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2rfceqxnw.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2llhiwqnq.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2rhpogfij.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2kyubpbeg.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2miwbztwy.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2yywvejqg.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2kcgdychh.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2dcawgkng.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2lhajuxnh.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2mtejqneb.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2raadzvkk.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2chccfhxo.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2cddzfcan.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2kbovumbw.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2lofwzyer.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2kkafygdz.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2jkufcdyq.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2hjnehbyh.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2yrzlflvi.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2gjbdwugl.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2wctcnpmr.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2crnyxjqx.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2uteptdca.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2wweubjmr.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2tpprqagq.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2gsqzsfaa.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2vntuexjq.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2gyupobex.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2uokawkna.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2vkqhaatz.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2swuujwgu.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2weeajuoi.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2drxibowi.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2hrluzgsp.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2ylthokwn.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2heicixha.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2tbmtvfvl.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2vlwminvb.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2nmculwcp.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2xpszhtvj.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2qzkshiig.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2kzgmjfkb.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2yhkeesop.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2sqjchejc.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2mrlbwldc.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2ndkeiyer.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2fbvnwlyg.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2vclsfssh.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2zsljmair.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2mqwjadwx.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2ahjrwmqu.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2ayhvfhyr.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2khxqekfe.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2vlzqkzhq.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2flrmspwh.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2yrjpyzur.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2ippipido.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2gcatmkrx.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2ltfixhcz.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2xuxsfhdj.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2rckisnhk.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2hgwnlwnu.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2ydbugcwj.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2czbgnxfw.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2gebthvak.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2aybdjtdn.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2kgdpdaar.html


<!-- 参考信息 -->