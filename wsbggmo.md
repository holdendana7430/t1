代发 wailian999

);
来源：http://mobile.fanxiaobao.xyz/Article/details/glscfhmwc.sHtML

[Q03] 增加列
来源：http://wap.fanxiaobao.xyz/Article/details/gxfvcojmo.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://m.share.fanxiaobao.xyz/Article/details/gxrmvaojo.sHtML

[Q04] 修改列类型
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsoqtluye.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://3g.fanxiaobao.xyz/Article/details/gqrmrtixr.sHtML

[Q05] 重命名列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxikuqfxn.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://m.share.fanxiaobao.xyz/Article/details/gwbbbhyvf.sHtML

[Q06] 删除列
来源：http://3g.fanxiaobao.xyz/Article/details/gehvuadwr.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://wap.fanxiaobao.xyz/Article/details/gjmplzwpw.sHtML

[Q07] 删除表
来源：http://blog.fanxiaobao.xyz/Article/details/gjabaditg.sHtML

DROP TABLE IF EXISTS orders;
来源：http://3g.fanxiaobao.xyz/Article/details/ggxnxesnj.sHtML

[Q08] 创建普通索引
来源：http://read.share.fanxiaobao.xyz/Article/details/ghcbzdaad.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://mobile.fanxiaobao.xyz/Article/details/gehaxxbvy.sHtML

[Q09] 创建唯一索引
来源：http://mobile.fanxiaobao.xyz/Article/details/godgqqivz.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://read.share.fanxiaobao.xyz/Article/details/gaoswplau.sHtML

[Q10] 插入单行
来源：http://wap.fanxiaobao.xyz/Article/details/gnlsnygtd.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wap.fanxiaobao.xyz/Article/details/gskcdvgtl.sHtML

[Q11] 一次插入多行
来源：http://www.share.fanxiaobao.xyz/Article/details/ghcsrinxc.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcjlujslr.sHtML

[Q12] 插入后取自增 ID
来源：http://www.blog.fanxiaobao.xyz/Article/details/genevmddr.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://read.share.fanxiaobao.xyz/Article/details/gptxmobfb.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mobile.fanxiaobao.xyz/Article/details/gjmhequbt.sHtML

[Q13] 忽略重复插入
来源：http://mobile.fanxiaobao.xyz/Article/details/gnashaogr.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mobile.fanxiaobao.xyz/Article/details/gxcgvncuw.sHtML

[Q14] 存在则更新（upsert）
来源：http://m.share.fanxiaobao.xyz/Article/details/guvuzpbaq.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://m.share.fanxiaobao.xyz/Article/details/gmvdblgoo.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mobile.fanxiaobao.xyz/Article/details/ggkhpolrl.sHtML

[Q15] 查询全部
来源：http://3g.fanxiaobao.xyz/Article/details/ghpwbjjfm.sHtML

SELECT * FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/guyydrntb.sHtML

[Q16] 查询指定列
来源：http://www.share.fanxiaobao.xyz/Article/details/gsgrjovjv.sHtML

SELECT id, name FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gsrxubxgy.sHtML

[Q17] 条件查询
来源：http://m.share.fanxiaobao.xyz/Article/details/gqqbatuwy.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gdfrvtzkx.sHtML

[Q18] 模糊匹配
来源：http://read.share.fanxiaobao.xyz/Article/details/geewddsiq.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://baike.fanxiaobao.xyz/Article/details/gddwfmacj.sHtML

[Q19] 范围查询
来源：http://baike.fanxiaobao.xyz/Article/details/gjbwwupdn.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://blog.fanxiaobao.xyz/Article/details/glcmsohde.sHtML

[Q20] IN 列表
来源：http://3g.fanxiaobao.xyz/Article/details/glihaphej.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://m.share.fanxiaobao.xyz/Article/details/grfnrygwj.sHtML

[Q21] 空值判断
来源：http://blog.fanxiaobao.xyz/Article/details/gwkpezrwy.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://3g.fanxiaobao.xyz/Article/details/ghhjzpiie.sHtML

[Q22] 排序
来源：http://m.share.fanxiaobao.xyz/Article/details/gipsaqqee.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mobile.fanxiaobao.xyz/Article/details/gikudkkgr.sHtML

[Q23] 分页
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvbolipkc.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wap.fanxiaobao.xyz/Article/details/gyrmngryo.sHtML

[Q24] 去重
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghxtkgkpe.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdhnkrhmj.sHtML

[Q25] 只取前 N 条
来源：http://m.share.fanxiaobao.xyz/Article/details/gvcryeoyy.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfdqsfmew.sHtML

[Q26] 计数
来源：http://3g.fanxiaobao.xyz/Article/details/gwtjjypit.sHtML

SELECT COUNT(*) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/ggtzlhmdj.sHtML

[Q27] 条件计数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkivalkgg.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/glaulqdeo.sHtML

[Q28] 求和与平均
来源：http://wap.fanxiaobao.xyz/Article/details/gmautdvst.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wap.fanxiaobao.xyz/Article/details/grmlyqgjm.sHtML

[Q29] 最大最小值
来源：http://m.share.fanxiaobao.xyz/Article/details/givkkdknb.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gpinbtpxg.sHtML

[Q30] 分组统计
来源：http://wap.fanxiaobao.xyz/Article/details/ghytgqghu.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.fanxiaobao.xyz/Article/details/gediwxdbq.sHtML

[Q31] 分组后过滤
来源：http://m.share.fanxiaobao.xyz/Article/details/gskzticsi.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://baike.fanxiaobao.xyz/Article/details/gfezznpdf.sHtML

[Q32] 分组拼接字符串
来源：http://baike.fanxiaobao.xyz/Article/details/gmdofesay.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wap.fanxiaobao.xyz/Article/details/gapyhyogs.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://blog.fanxiaobao.xyz/Article/details/gcystwvbm.sHtML

[Q33] 多列分组
来源：http://read.share.fanxiaobao.xyz/Article/details/gsnefjfgj.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://baike.fanxiaobao.xyz/Article/details/ggmajqhbq.sHtML

[Q34] 每组取第一条
来源：http://m.share.fanxiaobao.xyz/Article/details/guhczbeke.sHtML

SELECT * FROM (
来源：http://m.share.fanxiaobao.xyz/Article/details/gmzzlfycq.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://read.share.fanxiaobao.xyz/Article/details/ggnttdpia.sHtML

) t WHERE rn = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/gkxrrsnhy.sHtML

[Q35] 内连接
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gatdbvcss.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://blog.fanxiaobao.xyz/Article/details/gmdbyvomw.sHtML

[Q36] 左连接
来源：http://m.share.fanxiaobao.xyz/Article/details/gyxlvrppp.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvvutqtal.sHtML

[Q37] 右连接
来源：http://3g.fanxiaobao.xyz/Article/details/gnqgckbak.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://baike.fanxiaobao.xyz/Article/details/gkvgmhnuv.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.fanxiaobao.xyz/Article/details/gbcobqbxk.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://blog.fanxiaobao.xyz/Article/details/gypiacfxv.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.fanxiaobao.xyz/Article/details/gujlljbny.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://wap.fanxiaobao.xyz/Article/details/gacjgcrjj.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.fanxiaobao.xyz/Article/details/goytuwibc.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://baike.fanxiaobao.xyz/Article/details/gjnrlqyrq.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wap.fanxiaobao.xyz/Article/details/gkwfccnyk.sHtML

[Q41] 多表连接
来源：http://read.share.fanxiaobao.xyz/Article/details/gvyoimifk.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://m.share.fanxiaobao.xyz/Article/details/gsyxmlhtl.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghgntbjre.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.fanxiaobao.xyz/Article/details/gtsdzvvsz.sHtML

[Q42] 连接条件附加过滤
来源：http://wap.fanxiaobao.xyz/Article/details/grbxicvqc.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.fanxiaobao.xyz/Article/details/guqxfwxdc.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mobile.fanxiaobao.xyz/Article/details/gvuyxogsf.sHtML

[Q43] 标量子查询
来源：http://3g.fanxiaobao.xyz/Article/details/gyylwmtci.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.fanxiaobao.xyz/Article/details/gpstmtkgs.sHtML

[Q44] IN 子查询
来源：http://mobile.fanxiaobao.xyz/Article/details/gqihvuvne.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://baike.fanxiaobao.xyz/Article/details/gfdjbcdlf.sHtML

[Q45] EXISTS 判断存在
来源：http://www.share.fanxiaobao.xyz/Article/details/gvwjewcnl.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.fanxiaobao.xyz/Article/details/guoevokzu.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://wap.fanxiaobao.xyz/Article/details/gmdffkikt.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.fanxiaobao.xyz/Article/details/goznboezb.sHtML

[Q47] 与平均值比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdrryxltq.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mobile.fanxiaobao.xyz/Article/details/gdgqegmof.sHtML

[Q48] CTE 公用表表达式
来源：http://read.share.fanxiaobao.xyz/Article/details/gxruhiwet.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.fanxiaobao.xyz/Article/details/geeyqydov.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdyjoolvb.sHtML

[Q49] 更新单行
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzdeygotg.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://3g.fanxiaobao.xyz/Article/details/gvjiopuqh.sHtML

[Q50] 批量更新
来源：http://wap.fanxiaobao.xyz/Article/details/gldqzgoiz.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.blog.fanxiaobao.xyz/Article/details/grwtbszch.sHtML

[Q51] 用子查询更新
来源：http://mobile.fanxiaobao.xyz/Article/details/getbatapy.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/gcaulvzho.sHtML

[Q52] 删除指定行
来源：http://read.share.fanxiaobao.xyz/Article/details/gxmodxcjc.sHtML

DELETE FROM users WHERE id = 10;
来源：http://blog.fanxiaobao.xyz/Article/details/gvoezpnfz.sHtML

[Q53] 按条件删除
来源：http://read.share.fanxiaobao.xyz/Article/details/gmberchxn.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.fanxiaobao.xyz/Article/details/gggeceehi.sHtML

[Q54] 清空表
来源：http://3g.fanxiaobao.xyz/Article/details/gsplcaymi.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.fanxiaobao.xyz/Article/details/gvuymmvsh.sHtML

[Q55] 排名（并列占位）
来源：http://wap.fanxiaobao.xyz/Article/details/gfpkfzqil.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://blog.fanxiaobao.xyz/Article/details/gunjnjtfy.sHtML

[Q56] 密集排名（并列不占位）
来源：http://read.share.fanxiaobao.xyz/Article/details/ggehbhxou.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.fanxiaobao.xyz/Article/details/gmehuxcnm.sHtML

[Q57] 行号
来源：http://wap.fanxiaobao.xyz/Article/details/gobflkyvz.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/ghgtiumzv.sHtML

[Q58] 累计求和
来源：http://read.share.fanxiaobao.xyz/Article/details/gqvdfumst.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/gdavfhfxh.sHtML

[Q59] 分组内累计
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsfrpxltt.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/gpvndxaob.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.fanxiaobao.xyz/Article/details/gqisiozjo.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.fanxiaobao.xyz/Article/details/gipqfmjbe.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/glgndyyob.sHtML

[Q61] 移动平均
来源：http://m.share.fanxiaobao.xyz/Article/details/ghqowfgux.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghlvtuhke.sHtML

[Q62] 分组占比
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggdeohabw.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://baike.fanxiaobao.xyz/Article/details/ghgslsaiw.sHtML

[Q63] 开启事务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqacnhvry.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjjweuarn.sHtML

[Q64] 提交事务
来源：http://mobile.fanxiaobao.xyz/Article/details/giwzppatw.sHtML

COMMIT;
来源：http://blog.fanxiaobao.xyz/Article/details/guvvwzmux.sHtML

[Q65] 回滚事务
来源：http://read.share.fanxiaobao.xyz/Article/details/guzxohofp.sHtML

ROLLBACK;
来源：http://blog.fanxiaobao.xyz/Article/details/gwrcbcfxl.sHtML

[Q66] 行锁查询
来源：http://baike.fanxiaobao.xyz/Article/details/gzfpmttvd.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mobile.fanxiaobao.xyz/Article/details/grjygfezk.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzvsuxpvk.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.fanxiaobao.xyz/Article/details/grielvufm.sHtML

[Q68] 保存点
来源：http://baike.fanxiaobao.xyz/Article/details/gubygbvwl.sHtML

SAVEPOINT sp1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjpfqvdpa.sHtML

ROLLBACK TO sp1;
来源：http://m.share.fanxiaobao.xyz/Article/details/grplgyoeb.sHtML

[Q69] 查看执行计划
来源：http://read.share.fanxiaobao.xyz/Article/details/geltzevbw.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.fanxiaobao.xyz/Article/details/gnpndywlx.sHtML

[Q70] 更新统计信息
来源：http://m.share.fanxiaobao.xyz/Article/details/gtpkilhpq.sHtML

ANALYZE TABLE users;
来源：http://baike.fanxiaobao.xyz/Article/details/gkbqygqbr.sHtML

[Q71] 查看建表语句
来源：http://blog.fanxiaobao.xyz/Article/details/grdcabpme.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://m.share.fanxiaobao.xyz/Article/details/gkdovjojw.sHtML

[Q72] 查看索引
来源：http://m.share.fanxiaobao.xyz/Article/details/gypegpmwb.sHtML

SHOW INDEX FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gxzqapkeb.sHtML

[Q73] 查看表状态
来源：http://read.share.fanxiaobao.xyz/Article/details/gjplzsahg.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbhnhnelr.sHtML

[Q74] 强制使用索引
来源：http://baike.fanxiaobao.xyz/Article/details/gxlikyacm.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.fanxiaobao.xyz/Article/details/gnsuxpdgj.sHtML

[Q75] 日期格式化
来源：http://3g.fanxiaobao.xyz/Article/details/gjjgwnzkk.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/gasdlrdvk.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.fanxiaobao.xyz/Article/details/gfflkrivd.sHtML

[Q76] 按天统计
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtfboqayv.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.fanxiaobao.xyz/Article/details/gmterszgn.sHtML

[Q77] 时间加减
来源：http://blog.fanxiaobao.xyz/Article/details/gvsprntfm.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.fanxiaobao.xyz/Article/details/galuysusu.sHtML

[Q78] 当前时间
来源：http://read.share.fanxiaobao.xyz/Article/details/gyworweav.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.fanxiaobao.xyz/Article/details/gxyfvecbi.sHtML

[Q79] 字符串拼接
来源：http://wap.fanxiaobao.xyz/Article/details/gjheuqnji.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.fanxiaobao.xyz/Article/details/grozmzboy.sHtML

[Q80] 字符串截取
来源：http://m.share.fanxiaobao.xyz/Article/details/giwyjjjlq.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gflfxvvid.sHtML

[Q81] 字符串替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gheuxtpno.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gynhdolaq.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.fanxiaobao.xyz/Article/details/geahxubqz.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gvwrvctci.sHtML

[Q83] 大小写转换
来源：http://wap.fanxiaobao.xyz/Article/details/gozcmvmhy.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/grpwdvyqe.sHtML

[Q84] 去除首尾空格
来源：http://3g.fanxiaobao.xyz/Article/details/geqnsidhd.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gwtlsscen.sHtML

[Q85] 数值取整
来源：http://mobile.fanxiaobao.xyz/Article/details/gswgjkwjr.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.fanxiaobao.xyz/Article/details/geucrdskg.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtnxcyqci.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wap.fanxiaobao.xyz/Article/details/gpnlskjhr.sHtML

[Q87] JSON 字段做条件
来源：http://blog.fanxiaobao.xyz/Article/details/gnkogmxle.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.fanxiaobao.xyz/Article/details/gyibqzltx.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.fanxiaobao.xyz/Article/details/gmsknbsrx.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gprnfmpsy.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gfgxyqgff.sHtML

[Q89] 判断表是否存在
来源：http://www.share.fanxiaobao.xyz/Article/details/ggqxcbznn.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.fanxiaobao.xyz/Article/details/gxpabeovk.sHtML

[Q90] 生成序号列
来源：http://read.share.fanxiaobao.xyz/Article/details/gwjuwppeo.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.fanxiaobao.xyz/Article/details/gkwvfimve.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glweucvsh.sHtML

R. Bash 专题
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzldsvqgd.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gcyurmqkm.sHtML

[R01] shebang 与严格模式
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkjgjlzxg.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glhnfcaac.sHtML

set -euo pipefail
来源：http://www.share.fanxiaobao.xyz/Article/details/gzhfotbng.sHtML

[R02] 变量赋值与使用
来源：http://blog.fanxiaobao.xyz/Article/details/gbrorwrwx.sHtML

name="Tom"; echo "$name"
来源：http://read.share.fanxiaobao.xyz/Article/details/glejprsig.sHtML

[R03] 只读变量
来源：http://wap.fanxiaobao.xyz/Article/details/gnuwodrvu.sHtML

readonly PI=3.14
来源：http://blog.fanxiaobao.xyz/Article/details/gkojyrpma.sHtML

[R04] 位置参数
来源：http://read.share.fanxiaobao.xyz/Article/details/guagabdvs.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.fanxiaobao.xyz/Article/details/gyfuhuwla.sHtML

[R05] 参数默认值
来源：http://read.share.fanxiaobao.xyz/Article/details/gpsfbommt.sHtML

name="${1:-default}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gngflccqs.sHtML

[R06] 判断命令是否存在
来源：http://www.share.fanxiaobao.xyz/Article/details/gknphwczt.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcfatrfah.sHtML

[R07] if 判断文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gehgrkdcp.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/gimtyvopj.sHtML

[R08] 数值比较
来源：http://3g.fanxiaobao.xyz/Article/details/gnihlnsjy.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/gauksgjfl.sHtML

[R09] 字符串比较
来源：http://m.share.fanxiaobao.xyz/Article/details/gjhxbvmxv.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.fanxiaobao.xyz/Article/details/gdtxdebto.sHtML

[R10] 正则匹配
来源：http://www.blog.fanxiaobao.xyz/Article/details/gutpaaail.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.fanxiaobao.xyz/Article/details/gbupypedg.sHtML

[R11] case 多分支
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjvuackmu.sHtML

case "$1" in
来源：http://www.share.fanxiaobao.xyz/Article/details/gzwihyfcv.sHtML

start) echo "启动" ;;
来源：http://www.share.fanxiaobao.xyz/Article/details/gvphelqot.sHtML

stop)  echo "停止" ;;
来源：http://m.share.fanxiaobao.xyz/Article/details/giklioain.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.fanxiaobao.xyz/Article/details/gxsfamppb.sHtML

esac
来源：http://read.share.fanxiaobao.xyz/Article/details/gyalktcfz.sHtML

[R12] for 遍历文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gtwfqjqne.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/ghobughmn.sHtML

[R13] for 计数循环
来源：http://www.share.fanxiaobao.xyz/Article/details/gyeharupx.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/grlpoyywe.sHtML

[R14] C 风格 for
来源：http://www.share.fanxiaobao.xyz/Article/details/gwekfapjm.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gtzngzcxg.sHtML

[R15] while 逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/grunskpml.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gffmnnznc.sHtML

[R16] until 等待条件
来源：http://blog.fanxiaobao.xyz/Article/details/gsydsmdyv.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.fanxiaobao.xyz/Article/details/gdbpvimcl.sHtML

[R17] 数组定义与取值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpsszcaen.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.fanxiaobao.xyz/Article/details/gojashabl.sHtML

[R18] 遍历数组
来源：http://m.share.fanxiaobao.xyz/Article/details/gvzlgjohg.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gzsrsilrr.sHtML

[R19] 数组长度
来源：http://baike.fanxiaobao.xyz/Article/details/ghdqqhxpb.sHtML

echo "${#arr[@]}"
来源：http://baike.fanxiaobao.xyz/Article/details/gpqcyqhyf.sHtML

[R20] 关联数组（字典）
来源：http://3g.fanxiaobao.xyz/Article/details/gbswfgxkn.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.fanxiaobao.xyz/Article/details/glihntxch.sHtML

[R21] 字符串长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gcbtwvput.sHtML

echo "${#s}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggrnffztw.sHtML

[R22] 截取子串
来源：http://blog.fanxiaobao.xyz/Article/details/gtahzqbsd.sHtML

echo "${s:0:5}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gmsgotbju.sHtML

[R23] 字符串替换
来源：http://3g.fanxiaobao.xyz/Article/details/gumlkgwbp.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gunhspikw.sHtML

[R24] 大小写转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/goawnnosi.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.fanxiaobao.xyz/Article/details/goctksyiw.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.fanxiaobao.xyz/Article/details/gvofvdppj.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.fanxiaobao.xyz/Article/details/gyqxfufrq.sHtML

[R26] 命令替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gssgwlnhn.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.fanxiaobao.xyz/Article/details/giyrycjbf.sHtML

[R27] 算术展开
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goffqnfeh.sHtML

echo $((1 + 2 * 3))
来源：http://wap.fanxiaobao.xyz/Article/details/gepqxzooh.sHtML

[R28] 浮点运算
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkmtpxtdd.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjnsuflvd.sHtML

[R29] 定义函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdmpakkdp.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gmdnecuqc.sHtML

[R30] 函数返回状态码
来源：http://3g.fanxiaobao.xyz/Article/details/gjecmunno.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.fanxiaobao.xyz/Article/details/gpasnumjz.sHtML

[R31] 局部变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gszlphmab.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gpzhuvsij.sHtML

[R32] 参数个数校验
来源：http://m.share.fanxiaobao.xyz/Article/details/gvjzspurp.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gujdlzham.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.fanxiaobao.xyz/Article/details/gwxkrjuko.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.fanxiaobao.xyz/Article/details/gnmugzavt.sHtML

[R34] 退出时清理
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkzwaldoo.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.fanxiaobao.xyz/Article/details/getmhxcpq.sHtML

[R35] 后台执行并等待
来源：http://read.share.fanxiaobao.xyz/Article/details/gkapcyats.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqfqutoyo.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guzlyobbe.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.fanxiaobao.xyz/Article/details/gdjgaptwa.sHtML

[R37] 把输出赋给变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gtrxhfbpk.sHtML

files=$(ls -1)
来源：http://blog.fanxiaobao.xyz/Article/details/gkgheelsl.sHtML

[R38] 管道串联
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxyjjgoku.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.fanxiaobao.xyz/Article/details/gqbphxahp.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.fanxiaobao.xyz/Article/details/gervflftq.sHtML

cmd > out.log 2>&1
来源：http://www.share.fanxiaobao.xyz/Article/details/gdpavruxx.sHtML

[R40] 追加写日志
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxdudvqan.sHtML

echo "log" >> out.log
来源：http://blog.fanxiaobao.xyz/Article/details/ggtttquug.sHtML

[R41] 丢弃输出
来源：http://3g.fanxiaobao.xyz/Article/details/gfvmqybcj.sHtML

cmd >/dev/null 2>&1
来源：http://wap.fanxiaobao.xyz/Article/details/gwlyxsmna.sHtML

[R42] 输入重定向
来源：http://www.blog.fanxiaobao.xyz/Article/details/glieikodq.sHtML

wc -l < a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gdonezmhk.sHtML

[R43] 按名字查找文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gyegeycbi.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geyaauytv.sHtML

[R44] 按修改时间查找
来源：http://baike.fanxiaobao.xyz/Article/details/gcxdnfpcx.sHtML

find . -mtime -7 -type f
来源：http://baike.fanxiaobao.xyz/Article/details/gabncntzb.sHtML

[R45] 批量删除
来源：http://read.share.fanxiaobao.xyz/Article/details/gelzobjmb.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.fanxiaobao.xyz/Article/details/goqjflmec.sHtML

[R46] 递归替换文件内容
来源：http://read.share.fanxiaobao.xyz/Article/details/gcfwbnxpv.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnuxtwxuv.sHtML

[R47] sed 单行替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gqrtlroty.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gqxdwuxin.sHtML

[R48] awk 取指定列
来源：http://www.blog.fanxiaobao.xyz/Article/details/glisyvobq.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gyofdbmgd.sHtML

[R49] awk 带条件
来源：http://wap.fanxiaobao.xyz/Article/details/gwgbabsla.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.fanxiaobao.xyz/Article/details/gnkiuxunv.sHtML

[R50] awk 求和
来源：http://read.share.fanxiaobao.xyz/Article/details/gnvtimquw.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkyqfcbct.sHtML

[R51] 排序去重取前几
来源：http://www.blog.fanxiaobao.xyz/Article/details/gndnqetsu.sHtML


<!-- 参考信息 -->