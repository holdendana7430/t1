代发 wailian999

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3bcerowsz.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3bbhbkzxm.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3vpdyljtp.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3myoionve.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3qefrmqah.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3zwfeexro.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ctrhgybi.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3mexhgrhx.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3stcgwugl.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3ncmoxpfx.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3vzjqrhlg.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3rqqmfqtk.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3hdxnyrhm.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3uonkbobu.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3gfnnydvj.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3wonegzct.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3bogeozbg.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3kunafolr.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3yugdvgbg.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3sxhwsbed.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3ljhseynj.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3mpvbtukf.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3yirxhwak.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3iltqepwq.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3weqignip.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3vxuvdxwk.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3zhervvrl.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3twvpcpov.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3omtimyit.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3cjmmnymc.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3isdhhlri.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3yrcwcgdu.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3wbjuzdkk.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3tepwzekp.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3szwiqjuw.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3wfshucqg.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3bgxlljae.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3vhngsmti.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3cquwyqbb.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3wvcalwph.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3gdfrmctr.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3hmvwzdpn.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3ygxtowgl.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3bbbgmcfz.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3rzukphab.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3gpdxzwry.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3oxsbvewd.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3rlntugue.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3jlaytxsv.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3xlrsqjuq.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3ewufltmd.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3rxbdjsdi.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3lahubncj.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3windxufw.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3bmgixqzj.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3iioyojjd.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3jhgljlbp.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3mpovluxf.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3dkqleqcn.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3bjqpleun.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3portoisf.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3jyerubpy.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3yzpdhbtd.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3uoxovqye.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3jyqttnwk.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3dktyarpb.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3eoqsiilc.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3nnvwosqw.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3clxnlqkm.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3igqtcckf.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3uvmctsgb.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3pubeyfze.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3slpxcwob.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3ysjdzixc.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3zhgxmzxv.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3wmnfkgqa.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3syxtnckm.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3vnuzylsf.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3gkiylicl.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3oqkzatew.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3subvcyes.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3ozbwpdqg.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3nimlbxih.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3engwpwki.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3etxnmujh.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3dzbjmsmu.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3lacdwsga.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3phoozodj.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3atlcimva.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3nvhcjplh.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3bvfxeniw.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3cqzdaxqo.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3smpitdbd.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3obfwpchd.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3ahcwplnk.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3ntcarpoj.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3nwhjvaex.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3myqgekmt.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3qgfiqmyp.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3esjvvtmz.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3hszerraf.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3mpbfzfwc.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3kapyoauc.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3plgvqxvd.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3punqiluh.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3lyitoafp.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3amfbmuae.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3njiqripq.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3ykateovo.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3gppnznmi.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3viqcfgie.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3itjknabs.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3wpwzkxfk.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3lbzbyewl.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3tzehydub.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3xgciobma.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3xmczmcsp.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3jhpnigbq.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3meajcqyi.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3pqxcgncg.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3qmjdtvha.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3kjecncok.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3zmfgtvys.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3ylmyqyfb.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3djhmmvzk.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3zjtqmyja.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3eehtsthu.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3rdetosoy.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3yueztjrz.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3djzvlvix.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3lkpnglgc.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3qhlzmipg.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3laukfidx.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3oubblzgy.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3ousuvbtk.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3nfbjklbl.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3zbhwqdaw.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3djjwloud.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3bruldsop.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3xdevfofl.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3pppzqpok.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3fogkqgmy.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3dpqezqwb.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3bddlakvi.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3rlpskjxs.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3mghbcpht.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3vsghtfro.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3erxhzeiq.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3uefiepkf.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3fqxmzyjs.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3hwusfuop.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3mlqygmot.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3qhtnzpmo.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3srtefxce.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3aqdlvcua.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3cumcpfqd.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3ejebrjuo.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3qvsmcjze.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3bqymffdr.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3mtowolob.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3cqmlwakx.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3dtujiziz.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3cabjuini.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3lzmqhusa.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3rhkzthpb.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3jxreurct.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3kalrwdfl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xcceqhse.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3jkpqfuyt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3inhdtxiq.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3vziavuqm.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3isgdbhfy.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3yozzycjm.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3rvqwftxh.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3znkhoury.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3tumhvmmb.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3vtujqahe.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3fipblxfl.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3qlmqppwk.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3jnhhkded.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3nwmlkxxo.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3qlaknxmr.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3bneycqbd.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3kelwkqjm.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3uygzdxzp.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3sizfhapw.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3wqspatuc.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3smhjpqoo.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3lfgfzgtt.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3pxtftbsz.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3wocuqghg.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3drppzhuo.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3tbrzfavl.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3vtqttowi.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3gvsmhcrm.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3uokxwbvg.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3bywubiap.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3rgtsxjms.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3yebldizl.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3qqhlysyj.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3eaujuxei.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3xijfwcux.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3tuduaqju.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3oretawlv.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3stalnhah.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3ayoggbfz.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3uctrqywn.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3ixaiokns.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3bmqvtlsu.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3bcxxmrjg.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3dkeweuzv.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3hxrelzzv.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3tvnlqxjv.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3uramwvwo.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3vyyzrfqw.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3zskbvilo.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3zepjlajk.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3fkcaiqwf.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3zntgdhpc.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3kxtbdbqg.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3brvcydwh.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3rndxuqwd.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3sttudedr.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3gbjpsoee.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3mwiqdudm.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3pyqtyboh.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3mipysbvl.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3wodhmbbf.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3fqutbezh.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3moeyerdg.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3ewekqkyz.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3xadbprff.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3svhgrspl.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3nvirahfa.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3ewjpzhow.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3delzfaht.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3hjdddown.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3ldedqnpx.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3swbefvjz.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3smirlrzj.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3oluagzzi.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3ftbwejdw.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3aorsrakm.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3uvwgkoxn.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3hmsobhxy.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3llvvinlg.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3mgdvvqry.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3kczqtzsl.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3szeigtih.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3agqohuhy.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3ykhccapd.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3lodqnxkp.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3oatwmfrq.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3mplraxoq.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3rxfknhqv.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3tlotaovk.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3okgqomfc.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3fsxhxxmp.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3mtuqfxgs.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3fibwxiis.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3ylginfku.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3yiehfmem.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3nayauqyh.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3xgpijidi.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3njsxpcbo.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3coefjyjn.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3lhcvwdsm.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3pzgxtedz.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3ubvqqwne.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3qfedpnyv.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3oividmvz.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3ppdzfidi.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3hwmiekae.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3mcdizzph.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3biikmgaa.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3atpxdrza.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3spnlewxs.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3qxuomcia.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3vghcwfzu.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3zijqyvdn.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3ravbiimx.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3zolvdmxh.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3tntqdoel.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3docpgneh.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3llxcpmvc.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3cjxscvry.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3prrolfvz.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3vasmpdho.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3daojevcj.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3yvhcmmof.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3ocblqlse.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3zpjrcfel.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3bridwkpr.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3tllalziq.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3ueairnos.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3txnsamrv.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3ramrrjig.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3wkdvnlnr.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3gjqdwuca.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3zajkhrrf.html


<!-- 参考信息 -->