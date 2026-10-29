代发 wailian999

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mobile.fehbvm.com/Article/details/gmygnxymv.sHtML

);
来源：http://www.share.hesvh.cn/Article/details/gzikbsjfu.sHtML

[Q02] 创建带外键的表
来源：http://www.share.fehbvm.com/Article/details/gdqpnttqo.sHtML

CREATE TABLE orders (
来源：http://www.blog.zdbjq.cn/Article/details/govvmzazs.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.hesvh.cn/Article/details/gesbjogxk.sHtML

user_id INT NOT NULL,
来源：http://blog.fehbvm.com/Article/details/gxlsytmwq.sHtML

amount DECIMAL(10, 2),
来源：http://blog.hesvh.cn/Article/details/gdkvxfdfi.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.blog.hesvh.cn/Article/details/gufdpdmhm.sHtML

);
来源：http://m.share.hesvh.cn/Article/details/ggkdxpadc.sHtML

[Q03] 增加列
来源：http://www.m.share.fehbvm.com/Article/details/ghvpxbrfd.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mobile.fehbvm.com/Article/details/gclqkoaep.sHtML

[Q04] 修改列类型
来源：http://m.share.fehbvm.com/Article/details/gbbklrkjp.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://baike.hesvh.cn/Article/details/gnvgvuhvu.sHtML

[Q05] 重命名列
来源：http://m.share.zdbjq.cn/Article/details/gajdtlwzc.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://blog.zdbjq.cn/Article/details/gwqxxwhxp.sHtML

[Q06] 删除列
来源：http://mobile.zdbjq.cn/Article/details/gnxqsryab.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://baike.hesvh.cn/Article/details/gxictefjm.sHtML

[Q07] 删除表
来源：http://3g.zdbjq.cn/Article/details/gzfaardsw.sHtML

DROP TABLE IF EXISTS orders;
来源：http://baike.zdbjq.cn/Article/details/gtummgtyg.sHtML

[Q08] 创建普通索引
来源：http://wap.hesvh.cn/Article/details/grjjgymxn.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.blog.hesvh.cn/Article/details/gawvozvuv.sHtML

[Q09] 创建唯一索引
来源：http://blog.zdbjq.cn/Article/details/gligkyihn.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://baike.zdbjq.cn/Article/details/ghxkpmymp.sHtML

[Q10] 插入单行
来源：http://blog.zdbjq.cn/Article/details/gfqpmurts.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.hesvh.cn/Article/details/gwhqguhsy.sHtML

[Q11] 一次插入多行
来源：http://blog.zdbjq.cn/Article/details/guujqwkzi.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wap.hesvh.cn/Article/details/googdgoss.sHtML

[Q12] 插入后取自增 ID
来源：http://read.share.hesvh.cn/Article/details/gpqarhrrm.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://3g.zdbjq.cn/Article/details/gmashdiqq.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://blog.zdbjq.cn/Article/details/gpxuvmyml.sHtML

[Q13] 忽略重复插入
来源：http://blog.hesvh.cn/Article/details/gfenomeop.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://m.share.fehbvm.com/Article/details/gvhiuavsh.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.share.zdbjq.cn/Article/details/gjidpwdcq.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.share.hesvh.cn/Article/details/glhtgrrsj.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://m.share.hesvh.cn/Article/details/gtphxqkpa.sHtML

[Q15] 查询全部
来源：http://m.share.hesvh.cn/Article/details/gtuqczuta.sHtML

SELECT * FROM users;
来源：http://www.share.fehbvm.com/Article/details/gpyylvpok.sHtML

[Q16] 查询指定列
来源：http://blog.fehbvm.com/Article/details/gqebalvgm.sHtML

SELECT id, name FROM users;
来源：http://mobile.zdbjq.cn/Article/details/geqfxjdxa.sHtML

[Q17] 条件查询
来源：http://read.share.hesvh.cn/Article/details/gojwisber.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://baike.fehbvm.com/Article/details/gxwacocvq.sHtML

[Q18] 模糊匹配
来源：http://mobile.hesvh.cn/Article/details/gmqowdlwx.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.share.fehbvm.com/Article/details/gfoylppjz.sHtML

[Q19] 范围查询
来源：http://m.share.hesvh.cn/Article/details/gerchuhkw.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://3g.fehbvm.com/Article/details/grygxodqi.sHtML

[Q20] IN 列表
来源：http://3g.fehbvm.com/Article/details/gqbmebltf.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://blog.zdbjq.cn/Article/details/gjitcjgmv.sHtML

[Q21] 空值判断
来源：http://www.blog.fehbvm.com/Article/details/gegorticu.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://wap.zdbjq.cn/Article/details/gmvfadtcj.sHtML

[Q22] 排序
来源：http://www.share.hesvh.cn/Article/details/gypzggrff.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://3g.fehbvm.com/Article/details/gfaptqcxm.sHtML

[Q23] 分页
来源：http://www.share.hesvh.cn/Article/details/gowghymla.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://read.share.fehbvm.com/Article/details/gdpcblzrr.sHtML

[Q24] 去重
来源：http://www.m.share.zdbjq.cn/Article/details/gddkaxqwg.sHtML

SELECT DISTINCT city FROM users;
来源：http://mobile.fehbvm.com/Article/details/gzyfgjzjp.sHtML

[Q25] 只取前 N 条
来源：http://www.blog.zdbjq.cn/Article/details/gluzlwvik.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://3g.zdbjq.cn/Article/details/gslbnuvgn.sHtML

[Q26] 计数
来源：http://www.blog.zdbjq.cn/Article/details/grhfqpdqy.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.share.hesvh.cn/Article/details/gavftocjy.sHtML

[Q27] 条件计数
来源：http://3g.hesvh.cn/Article/details/gdnofjvrl.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gnrboudtw.sHtML

[Q28] 求和与平均
来源：http://blog.zdbjq.cn/Article/details/gwdiubhhd.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wap.fehbvm.com/Article/details/gqiydidfr.sHtML

[Q29] 最大最小值
来源：http://mobile.zdbjq.cn/Article/details/gtdoynljt.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://mobile.hesvh.cn/Article/details/gozbkfagj.sHtML

[Q30] 分组统计
来源：http://www.share.zdbjq.cn/Article/details/gbxwwmdss.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.fehbvm.com/Article/details/ghgdtnaga.sHtML

[Q31] 分组后过滤
来源：http://mobile.zdbjq.cn/Article/details/gypxrvuqa.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.zdbjq.cn/Article/details/ghvtylfya.sHtML

[Q32] 分组拼接字符串
来源：http://www.share.fehbvm.com/Article/details/gwyjybzxb.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://read.share.zdbjq.cn/Article/details/ggxligrvo.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://blog.hesvh.cn/Article/details/gsjgpjtko.sHtML

[Q33] 多列分组
来源：http://www.blog.fehbvm.com/Article/details/gkbwvqxuj.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://3g.zdbjq.cn/Article/details/gdnahmunv.sHtML

[Q34] 每组取第一条
来源：http://blog.hesvh.cn/Article/details/gwzodnsla.sHtML

SELECT * FROM (
来源：http://m.share.hesvh.cn/Article/details/gmnjsqqsf.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mobile.zdbjq.cn/Article/details/gbhhvfzom.sHtML

) t WHERE rn = 1;
来源：http://baike.fehbvm.com/Article/details/gynpcpoea.sHtML

[Q35] 内连接
来源：http://m.share.zdbjq.cn/Article/details/gixqtkgtt.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://baike.zdbjq.cn/Article/details/gpwvtwzcf.sHtML

[Q36] 左连接
来源：http://read.share.hesvh.cn/Article/details/glfzwfann.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.fehbvm.com/Article/details/ginccmbyv.sHtML

[Q37] 右连接
来源：http://baike.zdbjq.cn/Article/details/gyshnxcwr.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://m.share.zdbjq.cn/Article/details/grmhbwjkz.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.hesvh.cn/Article/details/gdzrkitxw.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.share.fehbvm.com/Article/details/gnuxuhlwk.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.hesvh.cn/Article/details/ggxdhtvkd.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.fehbvm.com/Article/details/gwjggqfuq.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.hesvh.cn/Article/details/gqrwbwzty.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.hesvh.cn/Article/details/ghhtxgoom.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wap.zdbjq.cn/Article/details/gyzkrxkyh.sHtML

[Q41] 多表连接
来源：http://wap.hesvh.cn/Article/details/gbvwpisps.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.fehbvm.com/Article/details/gguizthcc.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.zdbjq.cn/Article/details/gewzdseww.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.blog.zdbjq.cn/Article/details/grhmgkknr.sHtML

[Q42] 连接条件附加过滤
来源：http://baike.hesvh.cn/Article/details/gqndpgcxh.sHtML

SELECT u.name, o.amount FROM users u
来源：http://read.share.hesvh.cn/Article/details/guahqywzu.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mobile.fehbvm.com/Article/details/gjjffjlvd.sHtML

[Q43] 标量子查询
来源：http://mobile.fehbvm.com/Article/details/ggqwaubuh.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wap.zdbjq.cn/Article/details/gcjxgxyku.sHtML

[Q44] IN 子查询
来源：http://m.share.fehbvm.com/Article/details/grzaykxjo.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.share.hesvh.cn/Article/details/giczgmdek.sHtML

[Q45] EXISTS 判断存在
来源：http://m.share.fehbvm.com/Article/details/gyjdwwzgs.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.fehbvm.com/Article/details/gcoqwpcrk.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.fehbvm.com/Article/details/gnoqdnzkr.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.fehbvm.com/Article/details/gqudmwwix.sHtML

[Q47] 与平均值比较
来源：http://baike.fehbvm.com/Article/details/gxxcarxbh.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://baike.fehbvm.com/Article/details/gkfmyclip.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.fehbvm.com/Article/details/gucjgstpt.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://read.share.fehbvm.com/Article/details/grfgfkrqt.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.zdbjq.cn/Article/details/gwmicgevm.sHtML

[Q49] 更新单行
来源：http://3g.fehbvm.com/Article/details/gihtusfoz.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://3g.hesvh.cn/Article/details/gcykoasvr.sHtML

[Q50] 批量更新
来源：http://read.share.zdbjq.cn/Article/details/gpaowgfwr.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.zdbjq.cn/Article/details/gvopijbnu.sHtML

[Q51] 用子查询更新
来源：http://mobile.zdbjq.cn/Article/details/gfabvymjt.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://3g.zdbjq.cn/Article/details/gcfmyijbq.sHtML

[Q52] 删除指定行
来源：http://3g.fehbvm.com/Article/details/gurrfokrd.sHtML

DELETE FROM users WHERE id = 10;
来源：http://baike.hesvh.cn/Article/details/gxpgrxmal.sHtML

[Q53] 按条件删除
来源：http://m.share.hesvh.cn/Article/details/gypjmcefg.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.zdbjq.cn/Article/details/gvwpbrokn.sHtML

[Q54] 清空表
来源：http://baike.zdbjq.cn/Article/details/gxtcwqusx.sHtML

TRUNCATE TABLE logs;
来源：http://blog.fehbvm.com/Article/details/givewpkho.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.hesvh.cn/Article/details/geabatabk.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.zdbjq.cn/Article/details/gaxgidilr.sHtML

[Q56] 密集排名（并列不占位）
来源：http://blog.hesvh.cn/Article/details/gqqhhihkt.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.hesvh.cn/Article/details/gzaviccah.sHtML

[Q57] 行号
来源：http://3g.zdbjq.cn/Article/details/geeyaodik.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.hesvh.cn/Article/details/gpclkvtoa.sHtML

[Q58] 累计求和
来源：http://mobile.hesvh.cn/Article/details/gcopygpwd.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/gfhtmtcup.sHtML

[Q59] 分组内累计
来源：http://blog.zdbjq.cn/Article/details/gtmdubbau.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/geagvxkyp.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.hesvh.cn/Article/details/gnfxgdfgy.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.fehbvm.com/Article/details/ggeoyccdu.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.fehbvm.com/Article/details/gdeifdqgw.sHtML

[Q61] 移动平均
来源：http://www.share.hesvh.cn/Article/details/gvuapxymx.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.fehbvm.com/Article/details/gywcarppr.sHtML

[Q62] 分组占比
来源：http://read.share.zdbjq.cn/Article/details/ghgvxinhg.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.zdbjq.cn/Article/details/gsjyftzhc.sHtML

[Q63] 开启事务
来源：http://www.share.hesvh.cn/Article/details/gjxrdadcd.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.hesvh.cn/Article/details/gzjaozkvq.sHtML

[Q64] 提交事务
来源：http://www.share.fehbvm.com/Article/details/gtzlajnwq.sHtML

COMMIT;
来源：http://blog.hesvh.cn/Article/details/gvsoiobne.sHtML

[Q65] 回滚事务
来源：http://blog.fehbvm.com/Article/details/gqjdzpncp.sHtML

ROLLBACK;
来源：http://mobile.zdbjq.cn/Article/details/gswvdjwis.sHtML

[Q66] 行锁查询
来源：http://wap.zdbjq.cn/Article/details/guvjwacwv.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mobile.zdbjq.cn/Article/details/gghlkyzzb.sHtML

[Q67] 设置隔离级别
来源：http://m.share.fehbvm.com/Article/details/gofzppuwh.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.hesvh.cn/Article/details/gmednrkzh.sHtML

[Q68] 保存点
来源：http://wap.zdbjq.cn/Article/details/gdvatwxsh.sHtML

SAVEPOINT sp1;
来源：http://read.share.hesvh.cn/Article/details/gxsoxnmgo.sHtML

ROLLBACK TO sp1;
来源：http://m.share.fehbvm.com/Article/details/gcfjanerh.sHtML

[Q69] 查看执行计划
来源：http://m.share.fehbvm.com/Article/details/guuzbxfid.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.m.share.zdbjq.cn/Article/details/glqjqgahk.sHtML

[Q70] 更新统计信息
来源：http://baike.fehbvm.com/Article/details/gxxttzmpj.sHtML

ANALYZE TABLE users;
来源：http://m.share.zdbjq.cn/Article/details/gasyxzmlr.sHtML

[Q71] 查看建表语句
来源：http://www.blog.fehbvm.com/Article/details/gevzibfws.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.zdbjq.cn/Article/details/gdblchzav.sHtML

[Q72] 查看索引
来源：http://wap.hesvh.cn/Article/details/galzppnah.sHtML

SHOW INDEX FROM users;
来源：http://wap.zdbjq.cn/Article/details/gtgnakkry.sHtML

[Q73] 查看表状态
来源：http://blog.hesvh.cn/Article/details/gbzxknanw.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.fehbvm.com/Article/details/gajsusmcy.sHtML

[Q74] 强制使用索引
来源：http://mobile.zdbjq.cn/Article/details/gdsuesxre.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://baike.hesvh.cn/Article/details/gmqhhuzby.sHtML

[Q75] 日期格式化
来源：http://www.share.fehbvm.com/Article/details/gojhdrixd.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.fehbvm.com/Article/details/gtibsrtld.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://baike.hesvh.cn/Article/details/gnalplwai.sHtML

[Q76] 按天统计
来源：http://wap.hesvh.cn/Article/details/gdjnqebej.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wap.hesvh.cn/Article/details/gykywblri.sHtML

[Q77] 时间加减
来源：http://read.share.fehbvm.com/Article/details/gqmvyvkdq.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.hesvh.cn/Article/details/gajukercq.sHtML

[Q78] 当前时间
来源：http://m.share.hesvh.cn/Article/details/gsvplpkpf.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.fehbvm.com/Article/details/gakfxcste.sHtML

[Q79] 字符串拼接
来源：http://m.share.hesvh.cn/Article/details/gxxoipcqi.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.zdbjq.cn/Article/details/gcexehlgc.sHtML

[Q80] 字符串截取
来源：http://www.m.share.fehbvm.com/Article/details/gdjozpkhp.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://read.share.hesvh.cn/Article/details/ggtrjzvkw.sHtML

[Q81] 字符串替换
来源：http://3g.hesvh.cn/Article/details/gpuncmfii.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.hesvh.cn/Article/details/gxtmdycsm.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.hesvh.cn/Article/details/gkgbygewj.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://baike.zdbjq.cn/Article/details/gzvspdjfv.sHtML

[Q83] 大小写转换
来源：http://mobile.zdbjq.cn/Article/details/gtopsckex.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gmmnkejap.sHtML

[Q84] 去除首尾空格
来源：http://blog.zdbjq.cn/Article/details/gpjebedgq.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.fehbvm.com/Article/details/gvulsvppf.sHtML

[Q85] 数值取整
来源：http://m.share.fehbvm.com/Article/details/gzzupkfnz.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.hesvh.cn/Article/details/gyhzlgjgb.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.hesvh.cn/Article/details/gwxhsnvzj.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.hesvh.cn/Article/details/grvlgsyri.sHtML

[Q87] JSON 字段做条件
来源：http://blog.hesvh.cn/Article/details/gbyneslhq.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.hesvh.cn/Article/details/gyzgtvdsx.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.blog.hesvh.cn/Article/details/gxirccpqe.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.fehbvm.com/Article/details/gduirbfsd.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.zdbjq.cn/Article/details/gumjzqzty.sHtML

[Q89] 判断表是否存在
来源：http://www.share.hesvh.cn/Article/details/geezgbidk.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.fehbvm.com/Article/details/ghvlhlvjc.sHtML

[Q90] 生成序号列
来源：http://www.m.share.fehbvm.com/Article/details/gijnqikic.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.hesvh.cn/Article/details/gdztlqzra.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gmmzthemm.sHtML

R. Bash 专题
来源：http://www.m.share.hesvh.cn/Article/details/gxelbyldq.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gcoghgjyg.sHtML

[R01] shebang 与严格模式
来源：http://read.share.fehbvm.com/Article/details/glzjrkqio.sHtML

#!/usr/bin/env bash
来源：http://www.share.zdbjq.cn/Article/details/gomlthato.sHtML

set -euo pipefail
来源：http://read.share.hesvh.cn/Article/details/gsmyzwiap.sHtML

[R02] 变量赋值与使用
来源：http://www.share.zdbjq.cn/Article/details/ggxkynkro.sHtML

name="Tom"; echo "$name"
来源：http://mobile.zdbjq.cn/Article/details/gsuweulyi.sHtML

[R03] 只读变量
来源：http://www.blog.fehbvm.com/Article/details/gwoqexvll.sHtML

readonly PI=3.14
来源：http://blog.hesvh.cn/Article/details/gawugyzqi.sHtML

[R04] 位置参数
来源：http://read.share.hesvh.cn/Article/details/gdodxjqli.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.hesvh.cn/Article/details/gaebxacgl.sHtML

[R05] 参数默认值
来源：http://m.share.zdbjq.cn/Article/details/gvkajlpdd.sHtML

name="${1:-default}"
来源：http://wap.zdbjq.cn/Article/details/gxkuultsu.sHtML

[R06] 判断命令是否存在
来源：http://m.share.fehbvm.com/Article/details/ghlmudfvt.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.zdbjq.cn/Article/details/gfcfydvmq.sHtML

[R07] if 判断文件
来源：http://www.m.share.hesvh.cn/Article/details/goajtrcya.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.fehbvm.com/Article/details/gxfaxuwcj.sHtML

[R08] 数值比较
来源：http://www.blog.fehbvm.com/Article/details/gcxvyhavs.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.zdbjq.cn/Article/details/gkzhietat.sHtML

[R09] 字符串比较
来源：http://m.share.hesvh.cn/Article/details/gzhcyekse.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.hesvh.cn/Article/details/gzfqfwsij.sHtML

[R10] 正则匹配
来源：http://www.m.share.zdbjq.cn/Article/details/gxzcogejk.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.zdbjq.cn/Article/details/gcenbhfvk.sHtML

[R11] case 多分支
来源：http://mobile.zdbjq.cn/Article/details/gtpxqjmmx.sHtML

case "$1" in
来源：http://wap.hesvh.cn/Article/details/gbypbdveo.sHtML

start) echo "启动" ;;
来源：http://m.share.hesvh.cn/Article/details/gkidvvqxk.sHtML

stop)  echo "停止" ;;
来源：http://baike.hesvh.cn/Article/details/gtwailmvt.sHtML

*)     echo "未知命令" ;;
来源：http://blog.hesvh.cn/Article/details/gzqlvtysv.sHtML

esac
来源：http://m.share.hesvh.cn/Article/details/gxugaktti.sHtML

[R12] for 遍历文件
来源：http://www.m.share.fehbvm.com/Article/details/gddofptqx.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.zdbjq.cn/Article/details/gtmkymypb.sHtML

[R13] for 计数循环
来源：http://www.blog.fehbvm.com/Article/details/gjqmmalsz.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.fehbvm.com/Article/details/gjfynfter.sHtML

[R14] C 风格 for
来源：http://baike.zdbjq.cn/Article/details/gdjdwcmkb.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.hesvh.cn/Article/details/gamznwyna.sHtML

[R15] while 逐行读文件
来源：http://3g.fehbvm.com/Article/details/gxjectfmv.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.fehbvm.com/Article/details/gxtdpygxm.sHtML

[R16] until 等待条件
来源：http://www.m.share.fehbvm.com/Article/details/gtjjintwv.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.fehbvm.com/Article/details/gabgbsqdr.sHtML

[R17] 数组定义与取值
来源：http://www.share.hesvh.cn/Article/details/gqyjuqgyf.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.hesvh.cn/Article/details/gndhbpjex.sHtML

[R18] 遍历数组
来源：http://3g.fehbvm.com/Article/details/gsqjcedfz.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.zdbjq.cn/Article/details/ggftquonz.sHtML

[R19] 数组长度
来源：http://m.share.hesvh.cn/Article/details/gmmchuyob.sHtML

echo "${#arr[@]}"
来源：http://wap.hesvh.cn/Article/details/gfdtrvepy.sHtML

[R20] 关联数组（字典）
来源：http://mobile.fehbvm.com/Article/details/gkzniexcd.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.fehbvm.com/Article/details/gkyshcelp.sHtML

[R21] 字符串长度
来源：http://mobile.hesvh.cn/Article/details/gqlvrjfwz.sHtML

echo "${#s}"
来源：http://www.blog.fehbvm.com/Article/details/glvgczomt.sHtML

[R22] 截取子串
来源：http://baike.zdbjq.cn/Article/details/gqvjozimm.sHtML

echo "${s:0:5}"
来源：http://www.m.share.fehbvm.com/Article/details/guuuntihr.sHtML

[R23] 字符串替换
来源：http://wap.zdbjq.cn/Article/details/gjymtaagg.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.fehbvm.com/Article/details/gtqpfesww.sHtML

[R24] 大小写转换
来源：http://m.share.hesvh.cn/Article/details/gakzduwlw.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.zdbjq.cn/Article/details/gutllggkt.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.fehbvm.com/Article/details/gulptnxyq.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.hesvh.cn/Article/details/gxciixbmt.sHtML

[R26] 命令替换
来源：http://mobile.hesvh.cn/Article/details/gckvrpfjj.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.hesvh.cn/Article/details/gammpwibt.sHtML

[R27] 算术展开
来源：http://baike.hesvh.cn/Article/details/gzgnywyzq.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.fehbvm.com/Article/details/gjfnzhonb.sHtML

[R28] 浮点运算
来源：http://www.share.hesvh.cn/Article/details/gyehayaow.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.fehbvm.com/Article/details/gpceqxyvi.sHtML

[R29] 定义函数
来源：http://www.share.fehbvm.com/Article/details/gxzvxxawx.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.fehbvm.com/Article/details/glcwjdzgh.sHtML

[R30] 函数返回状态码
来源：http://www.blog.zdbjq.cn/Article/details/glkmsktbo.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.hesvh.cn/Article/details/gqjgyijfz.sHtML

[R31] 局部变量
来源：http://www.share.hesvh.cn/Article/details/gcoounhjh.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.zdbjq.cn/Article/details/gbnixuvli.sHtML

[R32] 参数个数校验
来源：http://www.blog.zdbjq.cn/Article/details/gkmxjspja.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.zdbjq.cn/Article/details/gbzzguosu.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.zdbjq.cn/Article/details/gssuxtypq.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.zdbjq.cn/Article/details/gsyutamnw.sHtML

[R34] 退出时清理
来源：http://m.share.hesvh.cn/Article/details/grdubbhqt.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.zdbjq.cn/Article/details/gtnqenayx.sHtML

[R35] 后台执行并等待
来源：http://wap.hesvh.cn/Article/details/gotwknwyf.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.hesvh.cn/Article/details/gnjqfxfws.sHtML

[R36] 并发执行多个任务
来源：http://3g.fehbvm.com/Article/details/gvsafxvzj.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.hesvh.cn/Article/details/gtwxlfjpd.sHtML

[R37] 把输出赋给变量
来源：http://wap.hesvh.cn/Article/details/gbiumcnec.sHtML

files=$(ls -1)
来源：http://wap.zdbjq.cn/Article/details/ggrygjufc.sHtML

[R38] 管道串联
来源：http://read.share.hesvh.cn/Article/details/gouinotcm.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.hesvh.cn/Article/details/gywijnoke.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.fehbvm.com/Article/details/gsacrwysx.sHtML

cmd > out.log 2>&1
来源：http://www.blog.hesvh.cn/Article/details/gvyeppmvj.sHtML

[R40] 追加写日志
来源：http://3g.zdbjq.cn/Article/details/gvfviefcs.sHtML

echo "log" >> out.log
来源：http://www.blog.zdbjq.cn/Article/details/gpxmqhzyj.sHtML

[R41] 丢弃输出
来源：http://www.share.zdbjq.cn/Article/details/gluzrvxvo.sHtML

cmd >/dev/null 2>&1
来源：http://baike.zdbjq.cn/Article/details/govvrmzds.sHtML

[R42] 输入重定向
来源：http://3g.fehbvm.com/Article/details/grehevtau.sHtML

wc -l < a.txt
来源：http://mobile.hesvh.cn/Article/details/gwvwyadhc.sHtML

[R43] 按名字查找文件
来源：http://www.blog.fehbvm.com/Article/details/guxgjosot.sHtML

find . -name "*.log" -type f
来源：http://www.blog.hesvh.cn/Article/details/gemjrbitv.sHtML

[R44] 按修改时间查找
来源：http://wap.hesvh.cn/Article/details/gtvowjpug.sHtML

find . -mtime -7 -type f
来源：http://www.blog.hesvh.cn/Article/details/gvhkifxht.sHtML

[R45] 批量删除
来源：http://wap.fehbvm.com/Article/details/ggzrezkik.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.hesvh.cn/Article/details/gtnpaydsx.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.hesvh.cn/Article/details/gioyibtmk.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.zdbjq.cn/Article/details/ghfcoiulq.sHtML

[R47] sed 单行替换
来源：http://read.share.fehbvm.com/Article/details/gjvtyfwps.sHtML


<!-- 参考信息 -->