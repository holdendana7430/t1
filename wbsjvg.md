代发 wailian999

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2amucabbm.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2vgswcytg.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2hefkkucj.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2mfzphujf.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2pcfeidhw.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2rfgsodyk.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2oqakhmvl.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2zurrxygg.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2cqmlvmyx.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2jnylfehm.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2slwgpjpl.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2mtvkaloa.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2vtxghhit.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2eeckifug.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2tveapxnf.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2jadwfodg.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2shftzxkl.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2tvndubnd.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2vxzsqzhs.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2aqnwpyaq.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2jlhmehvv.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2grdiivum.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2ogfuiopx.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2vttlsojc.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2dccmvvam.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2wpuvpifx.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2zqckvboq.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2qfmwmfpk.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2egporyuc.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2ixrwjvjp.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2bgpmgpbd.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2dcvdxkyr.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2fdqbhavy.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2qskuvopp.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2yukixlot.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2ryxytsee.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2qqvwapdb.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2jwluqkrp.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2yekebxuv.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2lsfdmdou.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2paolutaf.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2juuoowde.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2ivmfrzsp.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2eddhqkfl.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2vfxdkuyx.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2slxcylda.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2xbuwdlbz.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2gltvpgub.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2mbxfrzfq.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2emljscky.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2makmulwf.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2gyhjugih.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2gtwbmidk.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2vamxyhrt.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2dzxbpbdl.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2rawtnuby.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2uexmkasu.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2vzmrzbtd.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ljpcjayt.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2dlfhuegu.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2pkcvynho.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2gnqdingc.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2woojkcou.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2djnsjfel.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2zktbnffb.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2kotalgey.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2yndbmesd.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2lbhfgkfk.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2kcbngrio.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2ihfdgyec.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2ygzhlzvx.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2xdcmsqjr.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2mnolymam.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2nbzpmnjj.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2oclszfqg.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2jheizbkl.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2tpvnfvin.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2rmynwljo.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2gmyctohz.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2kmvnqzeh.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2qtjupdma.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2xkfpcjrb.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2jdxtzshh.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2jvrgcqdm.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2scfpexci.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2hcjndykl.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2vcfqcnop.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2yexgbpfu.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2swiveqrz.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2eoqbexcg.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2qhqfesyd.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2zngnhzcy.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2ougbpknh.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2mgpxhkin.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2zrxoabev.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2gminkpjn.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2zndhrsea.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2xxzzyqcz.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2nwxsymzr.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2twklpblk.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2fiskyoon.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2djfpfuas.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2rlkfusyt.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2vzvsrwnx.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2emdmaysj.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2htaegfox.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2aqgleyhl.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2vhjdlxko.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2oecmliia.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2xxhhbynb.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2gwcdecmj.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2wgczufrl.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2wypwejvo.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2nnavssmz.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2ciqqaqqo.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2exukemkl.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2jvcbqvaa.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2npeacprm.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2xonirvzw.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2kwaqqfbu.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2oklidkol.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2wlroaoht.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2skyebsux.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2iojpmvep.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2uchbydoa.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2wpbcznay.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2iptniolj.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2xfnoxfjz.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2pmsqbvzb.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2nncdobjd.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2inxbukcg.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2gzflrvuw.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2usgrqfgg.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2aibofigy.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2ikgmafyk.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2lpxmthnf.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2uvqukkyg.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2tbgtckez.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2vhzqwamk.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2zdosfcvs.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2jqgauhaj.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2pnxtpxjj.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2stcqmdzx.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2xlkkshsq.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2rihkgrnu.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2uuuucjgg.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2lkunpkwn.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2pdqzppph.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2yfwqxncb.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2hnqtnqxr.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2ekixcjuy.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2fgaffono.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2gozlilua.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2xvhnpmub.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2fhujnyet.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2pidfxige.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2hwbhqvtt.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2ewqjkkav.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2jsgudtet.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2mxcsmbhs.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2msbdkoko.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2qppryezy.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2hiilzhww.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2kbsghydp.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2rqwokclv.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2flnjdzuj.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2sueculif.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2kwrinmbm.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2cagmwivz.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2cytfdhrl.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2agephlaz.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2ltqgaugu.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2mjxpdyba.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2sdlgwixc.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2fptblhjq.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2uakfydrk.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2gxewhlfu.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2mcaghqxz.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2jkdejnms.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2perlzhoi.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2gbxyaawf.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2fwmjglqt.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2mditsljy.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2ncefheny.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2cpxdujxf.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2tdiaiben.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2sswbxfhg.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2lrseyvaj.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2fwbdhnfw.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2ryaxbjcn.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2wggfdxqz.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2avgbxapj.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2fmxingca.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2zvzljtxl.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2ezfzucdy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2oiajszcd.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2nfzjmthz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vhhzhkxc.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2lhjfwuwx.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2dgouuise.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2fakhxllg.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2arbdkbdf.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2gvyfczmg.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2uivrnawc.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2tqdclsgv.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2vcbltwwk.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2ohnghdki.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2osbgusan.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2yqceelii.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2jalvepcz.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2eajxnzfg.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2yttlmvls.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2hbwmmwdv.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2irqbvayt.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2ejbwfmnx.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2yzzjzqzv.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2muptbcit.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2zpbiwdxe.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2rdartxjy.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2rqqztnla.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2wmxnstnp.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2pbeeqgqh.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2gvxizkqj.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2tzksntng.html

esac
来源：http://www.52xcode.cn/Article/details/gt2truukhhq.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2kbqwrrkh.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2raacngrn.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2yxztwawd.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2zyktitlv.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2gwspgkgb.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2srrzyejr.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2tfmbeokk.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2svfhleht.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2vvwxdrgw.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2jkmdwrwt.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2zcsotjmw.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2udpaivko.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2orgqkghp.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2twxidypi.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2krkyxhck.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2jmqxgdfr.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2fenzgamw.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2sfrgqach.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2rbwescfq.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2owbcnpgo.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2ffbzlkzs.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2cfwykuth.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2yetbvvht.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2eqqyfwas.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2zrvfdrdm.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2xckooxwe.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2fvsfctex.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2cwbqghxa.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2ogfhtmhp.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2jzixoubf.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2qefwwehq.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2acbipccu.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2pldjomop.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2bjskumjn.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2hhcmmzgx.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2jbwylsfm.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2xnpdpvrv.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2rsqysyft.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2kwxcbxjz.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2shqouqus.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2jivpnfbj.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2zeytjyqp.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2ctoolkkc.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2phgdurst.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2qzzexpug.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2vbmyerzy.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2nrgayoit.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2viwsnujq.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2dhqjomii.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2tsezbpvn.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2buofnnyv.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2osmcgvjh.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2xmxsjoxl.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2meicgkey.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2ewgrntti.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2nzklynqe.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2igpymmqi.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2vnmalilj.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2ytoomdwk.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2iykussun.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2tsdqqxzy.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2tvuzgzak.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2abrspcho.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2eiqaoycl.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2mgaapajo.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2gjjatjeb.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2fvagerow.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2oriefxei.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2zytrocsv.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2psojlbvo.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2xrsihqwi.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2kgwkhmqs.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2zgfldrpu.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2uqccidyn.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2mltdcoep.html


<!-- 参考信息 -->