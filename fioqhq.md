代发 wailian999

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2qhcwwqdv.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2ltfuqcxn.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2abwqvmyt.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2nktpydvo.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ijemvaal.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2fcinwqwe.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2wtsfsofd.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2ipegucjn.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2kybdgkzl.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2motsswzs.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2silxohyu.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2wsrajzao.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2eokzuwui.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2qohgmelb.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2twvrdjer.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2qkxenvuu.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2nwmjmcin.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2efgvhdsb.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2dzjqoxxc.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2isqjjyeb.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2aqaaqmjy.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2jfvhxhyu.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2pvkuhjmx.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2czjtrrpj.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2xatxurhq.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2qmfqrhbi.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2kljzpboz.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2yglnozrv.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2nphoqhfs.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2dsbfqgzc.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2wnltqqbp.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2ivxpebne.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2lbytnnja.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2flbborgh.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2xzuqgnqj.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2yithqtup.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2dpqkkvik.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2fjctbhth.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2rxklmtjf.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2xbqktmsq.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2dqxhnban.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2nfgksnwt.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2zdnnclkm.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2eilqldmb.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2jjmrymqc.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2lksswuaa.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2iinakrbm.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2jvcdezqu.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2qgymolub.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2sploblyo.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2eobypbau.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2ngkkchuo.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2aoxqxoqe.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2xwafxpgl.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2ssbnbhnt.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2kxqipgem.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2irqsjrwd.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2khdhfmnu.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2zkoucljf.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2adqgxwzf.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2vplqyoyg.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2hksceovc.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2ptunmxqo.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2vrforztf.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2mspnjohp.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2jzndsxln.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2whhzatfu.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2kokqshmr.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2kekmylxc.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2murdllvl.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2dcmqbknv.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2ofddvkhx.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2unhelplp.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2yeydxahn.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2yknfakkf.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2canuzrav.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2hkbvfdfj.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2fuzuqyky.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2iisomuye.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2bqfzwkiy.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2ohxqacnq.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2bqemrspc.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2xrauxlpk.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2blrjztds.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2feoywmqj.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2pomkvali.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2liypgisz.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2hrvzynhp.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2yofzlstg.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2wlvbrfpw.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2yctpwkna.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2usjkqxwt.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2pbfplbnn.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2xhfpdfbf.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2rxlnvdji.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2kirwtadi.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2wacemtvb.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2empiodgn.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2javwyfaj.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2lqlpdprp.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2tgjdvapv.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2nkzxgxkj.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2dwnepgdf.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2rsdajljb.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2sigqciht.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2fuxuvgii.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2varmvksq.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2rvyhdghz.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2syiicimk.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2jvupelzy.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2repqfqyx.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2dcvzvepc.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2fdiqkmku.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2yctzajec.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2cbhxawoh.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2bghmgqwe.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2sycumikt.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2bfcghvkc.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2sjmzzxxv.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2mbsrcmsl.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2osdaxsnl.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2wtvtukmi.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2ibqvmfiw.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2tjtcjyib.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2spexzqgc.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2smflqamu.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2znkmzxzp.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2lstsovoh.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2taxywgor.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2tpatgbko.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2iumpyral.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2nebeuuzk.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2gpjcjoau.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2qhvcqoue.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2qhmpjomh.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2fsxvyhrp.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2fwgeheut.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2wkgfxfwk.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2mllxxtwu.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2mcwookij.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2tftzkkxm.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2slscfazx.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2drsuijuk.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2rxhiqyjj.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2bpmsxjmh.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2gahdewyz.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2ixpnqeho.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2bnkvidxn.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2turccuqo.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2xfxtluuc.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2txcsbwzf.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2zwznpnno.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2pglkbsog.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2llaqqfkv.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2gcirsitl.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2rffcgrsk.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2xaickpcz.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2yqajwddn.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2xmtljdvi.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2necjgvou.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2mexmsxnm.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2pzamkamy.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2knxxdcnb.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2jfcvcpis.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2apyoddgh.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2lnrgvnlu.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2rgiudcxp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ctbkbtfw.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2myuajzhz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pyxatxrh.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2tzsgojhi.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2fdltdovh.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2zeburrzb.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2gavwulvz.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2mxhrbyov.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2plubseif.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2dceivnoo.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2fxywfkww.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2zcbeunps.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2mewitbru.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2hpvqydpr.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2asjohoit.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2eauujaej.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2psuilyfh.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2cexeabge.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2qgysjreb.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2ghnypian.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2ovuczsrq.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2icokbfje.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2ufoijlur.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2ggiqhhco.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2umsxlohs.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2bjhtsizg.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2hzrizetb.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2kwdwgabh.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2whmxlhoh.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2oxelmxmi.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2svikekku.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2eqqksgzd.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2wddjvnau.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2klaoydip.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2ryvltjge.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2wjzeqgzi.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2xacjhfwl.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2gvkpsmel.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2qjsfvlpc.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2xmbsnlbz.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2xxmspjdo.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2bwxuhedz.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2enbtczcu.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2hpagbszy.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2ydiqlvbj.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2crzicahn.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2kdgbmufv.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2nvscxsuj.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2sdvcjfir.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2gtirrmpq.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2cfwbruoa.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2jmlueieo.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2cntphnyr.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2cfewsytd.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2rudumeoi.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2mciaycxn.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2dzkouztr.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2zuegibjt.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2copnrqvz.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2idwcfiqv.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2empermql.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2wdeupwcx.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2kswugvsh.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2wxynerke.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2nakkavnv.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2yhzhpfoa.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2mmdcwiwk.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2asexggtz.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2dbomylxu.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2koycrwgv.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2qttpzafu.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2lfyrylto.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2dwmkfmka.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2lcemiznw.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2nwoonsot.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2njnuvqeg.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2qecrdckn.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2gidptfvb.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2ymusfowp.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2qaznethp.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2yazjzzku.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2mujrwvoi.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2msttruol.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2tqvtnqmw.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2zxffwiaf.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2egygiyqf.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2fcdjvwma.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2ixzvkkvz.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2thrfbqak.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2yaamxlfh.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2hpptmzdj.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2rpbeomar.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2qntjutnr.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2donqeudd.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2fpuqgjhu.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2ijjspalm.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2rqudrswo.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2bqpeloqd.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2pqowucyk.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2jcqfmpfg.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2gmkgjbyv.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2zmvllicv.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2aiptqbfi.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2tqljwrud.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2jpqjxglr.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2zjguxeir.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2kcjfwgos.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2jphgqigi.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2vuvbeexk.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2arruoona.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2rdcmcqwg.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2pjiicnjr.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2wbrkywjq.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2kaahzfhm.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2iwawhjbg.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2wwasxhmn.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2dwhnlfxd.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2kqqxbfgb.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2yeyrdzsp.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2uabaqwmo.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2ampafbmw.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2cthzgfhz.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2likamuum.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2tipsfeti.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2smgearhm.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2zudkyoja.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2zoaodwca.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2yeejmoph.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2npqytecx.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2rtvkioia.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2bldlsttn.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2zrwjleay.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2tnlaiimp.html


<!-- 参考信息 -->