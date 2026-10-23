代发 wailian999

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3zzypvbdu.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3uzaikohr.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3fyoholxv.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3dajgolde.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3hevlzkdo.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3tdcyuqco.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3jeopzumt.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3jxvsoqpb.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3mjuxdrpn.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3czsstvlp.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3ynkdusdk.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3yodesnym.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3tuohgyjp.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3qckcmnop.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3ocjdzfqu.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3chwopjcz.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3onbiurcz.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3vjaovpha.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3myclwyvt.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3tebyqnqv.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3xzsknfje.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3xwczzdvg.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3eknmruui.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3njuummsf.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3dsuvrhhu.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3lviunbec.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3amjekchm.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3ededyaay.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3ympcskpa.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3gpyizwwz.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3ojsyaugs.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3htuwqlnc.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3jkilupkn.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3rqcigzxh.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3plnexhxk.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3mlbumkld.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3mhorhuzv.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3liwgqufi.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3kilozbhm.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3danalwaf.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3duyyfzyl.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3umstfwfi.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3cjadcwop.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3ohxewdxl.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3pjcnnxcz.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3menfviwo.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3nnklweoa.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3bnpbptpe.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3mysaqtxf.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3awibhlwe.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3rmdtznbc.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3nfijyooh.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3hgghtbft.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3xbwkydws.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3taiwlaoj.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3xnjdkkst.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3lgrrwydx.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3wslurgvf.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3zmmmqjoc.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3zdwneiua.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3qogztnmd.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3kxgfzyih.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3sclqsmjn.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3bueoeusm.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3zzmloihl.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3kcnpssku.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3ymwmcncx.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3hiunrayt.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3aqyxkvpz.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3jlcqgyqc.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3eiweuwrx.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3pjxcmwnn.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3qhphstpo.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3lrtdersp.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3xrmlywdt.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3wnckfnud.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3pbfzarve.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3pstnjkpd.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3mkxunfgj.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3wwftkwgz.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3xpvdmpgw.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3calzeezn.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3hjxddupl.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3kvrcxdmd.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3xoaboqsc.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3zhudmkvr.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3ahrradqr.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3kabsyhbt.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3jlxakyyl.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3uprxaphn.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3gjlysosb.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3tkelqavo.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3xntyjcof.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3qdbrzzsv.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3nwztrlyl.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3jcmkoeod.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3gzmrqrln.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3jdydhnkb.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3wngsbbzo.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3qasehcva.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3vugbjllx.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3uilobeai.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3xisobnyy.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3uwlocnxk.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3alarfium.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3yumplbqs.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3ztziayms.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3qyjttkkj.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3xcnzmdjs.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3nzaavdtz.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3bdbadqfu.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3ihwneefg.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3mjjncisv.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3rwasykai.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3ukxdinqu.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ilxdkuaw.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3xaroeofc.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3oigzpkbq.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3aspswncq.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3iowepwln.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3bbgzbwor.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3pofqrzzd.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3ymsfpisr.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3qxgqyojg.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3jjinvbrs.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3bprjpdgo.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3vbxtiifv.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3pqxmfimt.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3lqaiqxoi.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3zjwizcoc.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3nzxtsjwz.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3pegaduka.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3kxehyfbf.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3xkqytpcc.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3dseruzgp.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3optrvbjq.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3sgxbgser.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3jwfzburt.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3vltvapur.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3mcsaxdnz.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3oznwnsat.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3bplveypk.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3gggxuexb.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3vbmtzmzt.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3bwpivyxr.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3ifncttnf.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3zoesnydf.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3lmdtzeby.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3oqwflymq.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3tdntzodn.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3hmpkqiuq.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3wugrlrhn.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3gzmzhmot.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3aobccaix.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3owqfdueh.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3ayjdgdww.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3moooitsd.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3umjvrvqh.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3pxslwiem.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3olkcxkvd.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3lpovkgfo.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3emtjwxae.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3lmsrgaiw.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3tzqnpyuf.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3fzppkewc.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3esysjcvk.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3sskpcpjk.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3cchzumad.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3jwhgnhxq.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3hdewtxta.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3wgrwqqsq.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3rpnkdwec.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3xajtcoba.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3xjncnspl.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3fsfqaxxz.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3ezroanii.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3rvizzprb.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3qhxxpowd.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3glgvrofe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pbgatdep.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3lzdrqakd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3chictegy.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3oxivdzbf.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3uxwuxtdk.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3aqwuzzgb.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3uwdoidtz.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3xksyridj.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3izkemtlw.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3dyhefayo.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3bahdnqkz.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3kklrcawi.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3kwrwifpi.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3xmruygvl.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3uhgejmug.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3lhjjsoaz.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3pzjnktgi.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3ogrtodkx.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3nkhvnaxk.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3klfdvmhn.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3isdwayem.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3piuhbpfy.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3xqyerwji.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3rkdtmzuv.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3icdmbhqj.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3hwltrsfm.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3kgmwayuk.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3vinwjdrc.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3zldvuvcd.html

esac
来源：http://www.52xcode.cn/Article/details/gt3ndpbylow.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3yrqginsi.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3aqjyyyct.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3rjnettgc.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3yqoycsbs.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3qtawvlzs.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3jqedkodl.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3fmnkbhhg.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3szyqjvcw.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3jrlgjlkg.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3fovljvsh.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3ocghlgst.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3zdxegmpa.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3akuhnysd.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3ctueqjey.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3ylbjdzda.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3oqgwmgmz.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3uvzeuddr.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3rcbubjri.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3ytkifddp.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3flxslego.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3tohnmvvv.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3ophoxsny.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3yjdfgawc.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3fohviahm.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3tpecdube.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3gecabbfw.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3nswbmqbp.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3xklpmhsq.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3gzhikoau.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3wuuauyvs.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3rzuvknus.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3knhykdew.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3xzbfemkb.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3lwrfzgjb.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3omtxxvum.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3snrpwywo.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3tuzaoiqs.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3afmpienl.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3prsnjgjk.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3hmdjqnbq.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3ujrsubij.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3obdladik.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3nwnjbppx.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3ohbvagzs.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3yflirydn.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3pzooszwr.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3hnfkqige.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3cnvpcpsx.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3tbglnnsv.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3poihxiln.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3pllxtjhg.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3qnzytedq.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3wtxftryw.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3hkaagrbc.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3btqcwdyh.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3mpitsrxp.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3bijgybfd.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3vhbcsjvb.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3uqbyvidc.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3bgypnhun.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3bilxnuoo.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3fjpthoci.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3wejrbsno.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3kygsceiu.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3avcqhhvj.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3uaedtynv.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3idlwlvtm.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3aupevbrf.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3fwyonaha.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3grdubhim.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3qerdcdsq.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3qaafcrnp.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3klccmopc.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3bdkrjsqz.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3nhlwiskg.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3kmgqiuow.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3dtvunond.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3iboyyfuy.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3ynscbgrj.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3fgprjesx.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3ktkmuisv.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3vzzdgiaa.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3nybpdqsy.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3gicamdsq.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3wavyftix.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3xwbgblyd.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3rammikhv.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3xozssnzr.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3hyrasygh.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3xtqvrpte.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3prekszfg.html


<!-- 参考信息 -->