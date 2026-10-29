代发 wailian999

);
来源：http://www.m.share.fehbvm.com/Article/details/ggyzydwzu.sHtML

[Q03] 增加列
来源：http://wap.hesvh.cn/Article/details/ghraenqiq.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.m.share.fehbvm.com/Article/details/ghaffpblz.sHtML

[Q04] 修改列类型
来源：http://blog.zdbjq.cn/Article/details/gqekloxby.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.m.share.fehbvm.com/Article/details/gbpylccit.sHtML

[Q05] 重命名列
来源：http://www.m.share.hesvh.cn/Article/details/gkixgumtz.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://baike.fehbvm.com/Article/details/gjxgjsuzb.sHtML

[Q06] 删除列
来源：http://www.blog.hesvh.cn/Article/details/gydtaiznh.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.blog.fehbvm.com/Article/details/gxbbduokq.sHtML

[Q07] 删除表
来源：http://read.share.zdbjq.cn/Article/details/guivmkwen.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.m.share.hesvh.cn/Article/details/gphqxtyax.sHtML

[Q08] 创建普通索引
来源：http://mobile.zdbjq.cn/Article/details/ghpkcecsb.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://mobile.fehbvm.com/Article/details/gdsxnucdq.sHtML

[Q09] 创建唯一索引
来源：http://wap.zdbjq.cn/Article/details/gpbmvzzeg.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.blog.fehbvm.com/Article/details/gayxcblpp.sHtML

[Q10] 插入单行
来源：http://www.m.share.fehbvm.com/Article/details/gcpsuyivq.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mobile.fehbvm.com/Article/details/gofhnmoio.sHtML

[Q11] 一次插入多行
来源：http://www.m.share.zdbjq.cn/Article/details/grewflfyj.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://3g.fehbvm.com/Article/details/guwbzvggj.sHtML

[Q12] 插入后取自增 ID
来源：http://m.share.hesvh.cn/Article/details/gpyebrgrf.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.share.hesvh.cn/Article/details/gtxlypbic.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://blog.fehbvm.com/Article/details/gxhddeqzm.sHtML

[Q13] 忽略重复插入
来源：http://wap.hesvh.cn/Article/details/gdixarivs.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://3g.hesvh.cn/Article/details/gxgrxtfcv.sHtML

[Q14] 存在则更新（upsert）
来源：http://wap.hesvh.cn/Article/details/goksptcdu.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://blog.zdbjq.cn/Article/details/gelennssr.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.zdbjq.cn/Article/details/gwyhrgsdx.sHtML

[Q15] 查询全部
来源：http://read.share.fehbvm.com/Article/details/glwsmwevh.sHtML

SELECT * FROM users;
来源：http://blog.fehbvm.com/Article/details/gzwcoyijc.sHtML

[Q16] 查询指定列
来源：http://www.blog.zdbjq.cn/Article/details/gsbfbkzdk.sHtML

SELECT id, name FROM users;
来源：http://baike.zdbjq.cn/Article/details/gaioiaxvi.sHtML

[Q17] 条件查询
来源：http://www.blog.fehbvm.com/Article/details/gqusnujkc.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.blog.hesvh.cn/Article/details/gomspocaw.sHtML

[Q18] 模糊匹配
来源：http://mobile.hesvh.cn/Article/details/gbccojtji.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://baike.hesvh.cn/Article/details/gemnvgjmm.sHtML

[Q19] 范围查询
来源：http://wap.zdbjq.cn/Article/details/gmctjiajx.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://read.share.fehbvm.com/Article/details/gnflqeear.sHtML

[Q20] IN 列表
来源：http://blog.hesvh.cn/Article/details/gpvkkgvjt.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.blog.hesvh.cn/Article/details/gnbtzunty.sHtML

[Q21] 空值判断
来源：http://read.share.hesvh.cn/Article/details/gjzxgepyk.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.blog.hesvh.cn/Article/details/gmvuizmpm.sHtML

[Q22] 排序
来源：http://www.m.share.hesvh.cn/Article/details/ggicvxkga.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://3g.zdbjq.cn/Article/details/ggjxhscbk.sHtML

[Q23] 分页
来源：http://baike.fehbvm.com/Article/details/grglerfjo.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://blog.fehbvm.com/Article/details/gnwhbdpak.sHtML

[Q24] 去重
来源：http://blog.zdbjq.cn/Article/details/gbjhskgmv.sHtML

SELECT DISTINCT city FROM users;
来源：http://baike.fehbvm.com/Article/details/gsetmcaig.sHtML

[Q25] 只取前 N 条
来源：http://www.share.zdbjq.cn/Article/details/gckedbavu.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.zdbjq.cn/Article/details/gdqktzany.sHtML

[Q26] 计数
来源：http://baike.fehbvm.com/Article/details/gwxmteibl.sHtML

SELECT COUNT(*) FROM users;
来源：http://3g.fehbvm.com/Article/details/gjpzpuuee.sHtML

[Q27] 条件计数
来源：http://www.blog.hesvh.cn/Article/details/gmnxszzaq.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://3g.fehbvm.com/Article/details/gqrwcgmza.sHtML

[Q28] 求和与平均
来源：http://www.share.fehbvm.com/Article/details/gkmcdyrkm.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wap.hesvh.cn/Article/details/gpsgcnpdf.sHtML

[Q29] 最大最小值
来源：http://m.share.hesvh.cn/Article/details/gvoxyazey.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://wap.fehbvm.com/Article/details/gvehekxwy.sHtML

[Q30] 分组统计
来源：http://baike.hesvh.cn/Article/details/gfftblmvl.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://baike.zdbjq.cn/Article/details/gdbsuxaip.sHtML

[Q31] 分组后过滤
来源：http://m.share.hesvh.cn/Article/details/gevsmucri.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.hesvh.cn/Article/details/gwcvgfxud.sHtML

[Q32] 分组拼接字符串
来源：http://read.share.zdbjq.cn/Article/details/gntgvfbuf.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://read.share.zdbjq.cn/Article/details/gfavkdhej.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.share.hesvh.cn/Article/details/gxoibqohy.sHtML

[Q33] 多列分组
来源：http://wap.zdbjq.cn/Article/details/gnxevcdpb.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.blog.zdbjq.cn/Article/details/glqrphdvk.sHtML

[Q34] 每组取第一条
来源：http://read.share.hesvh.cn/Article/details/gcylsdaqn.sHtML

SELECT * FROM (
来源：http://read.share.fehbvm.com/Article/details/gkzuegaww.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.share.hesvh.cn/Article/details/gagzintpi.sHtML

) t WHERE rn = 1;
来源：http://www.blog.fehbvm.com/Article/details/gteqvocxx.sHtML

[Q35] 内连接
来源：http://m.share.hesvh.cn/Article/details/ggvputrbr.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.hesvh.cn/Article/details/grdsswdxq.sHtML

[Q36] 左连接
来源：http://www.blog.zdbjq.cn/Article/details/gtlfjspul.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.share.fehbvm.com/Article/details/gqxzlkhtb.sHtML

[Q37] 右连接
来源：http://3g.zdbjq.cn/Article/details/ggatdpbra.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mobile.fehbvm.com/Article/details/gyyjgxfgy.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://blog.zdbjq.cn/Article/details/gqsvwwoxc.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://3g.zdbjq.cn/Article/details/gqjprivtm.sHtML

[Q39] 自连接（查上下级）
来源：http://3g.hesvh.cn/Article/details/gpdyvctdq.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://3g.zdbjq.cn/Article/details/gbnqmuqyq.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.fehbvm.com/Article/details/gixgvuyjm.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://3g.hesvh.cn/Article/details/gvazgcpwo.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://3g.hesvh.cn/Article/details/gcwfxttxo.sHtML

[Q41] 多表连接
来源：http://3g.zdbjq.cn/Article/details/gyavnnzpm.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.fehbvm.com/Article/details/gefmokhfs.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.fehbvm.com/Article/details/gbqztjxtb.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.fehbvm.com/Article/details/gvwuninhg.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.hesvh.cn/Article/details/gxyzooxxc.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.m.share.zdbjq.cn/Article/details/gpskwvqak.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wap.fehbvm.com/Article/details/gxtxfttvm.sHtML

[Q43] 标量子查询
来源：http://mobile.hesvh.cn/Article/details/gioadasrv.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.fehbvm.com/Article/details/gdflnypmt.sHtML

[Q44] IN 子查询
来源：http://www.share.hesvh.cn/Article/details/goykfusvb.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.blog.hesvh.cn/Article/details/gmmtisryg.sHtML

[Q45] EXISTS 判断存在
来源：http://3g.fehbvm.com/Article/details/gtsktfiuo.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.zdbjq.cn/Article/details/gptetukql.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://m.share.zdbjq.cn/Article/details/ggwvtpgul.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.hesvh.cn/Article/details/gcepmcdyu.sHtML

[Q47] 与平均值比较
来源：http://www.m.share.zdbjq.cn/Article/details/gsjpdveyb.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://baike.fehbvm.com/Article/details/gabbfswro.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.zdbjq.cn/Article/details/grnxbtjnb.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.share.fehbvm.com/Article/details/gttxspfza.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://mobile.hesvh.cn/Article/details/govmuwlya.sHtML

[Q49] 更新单行
来源：http://3g.zdbjq.cn/Article/details/gtraxirnm.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.fehbvm.com/Article/details/gnaluvylf.sHtML

[Q50] 批量更新
来源：http://blog.hesvh.cn/Article/details/gcvcurcjr.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.share.zdbjq.cn/Article/details/gvuhiveuy.sHtML

[Q51] 用子查询更新
来源：http://www.share.fehbvm.com/Article/details/gwqjfqoaz.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blog.zdbjq.cn/Article/details/gsnojxyvi.sHtML

[Q52] 删除指定行
来源：http://blog.zdbjq.cn/Article/details/gdgwbripg.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.blog.zdbjq.cn/Article/details/gyaalwine.sHtML

[Q53] 按条件删除
来源：http://www.m.share.fehbvm.com/Article/details/gggiomhxu.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.fehbvm.com/Article/details/gwwoxtpsu.sHtML

[Q54] 清空表
来源：http://3g.fehbvm.com/Article/details/gmufjrtxv.sHtML

TRUNCATE TABLE logs;
来源：http://www.share.fehbvm.com/Article/details/gwongmvgl.sHtML

[Q55] 排名（并列占位）
来源：http://baike.fehbvm.com/Article/details/gqlqwofli.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.fehbvm.com/Article/details/gyjkrhyui.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.zdbjq.cn/Article/details/gyfuxelbk.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.m.share.zdbjq.cn/Article/details/gtufsyzqo.sHtML

[Q57] 行号
来源：http://baike.zdbjq.cn/Article/details/gguwdawoo.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gjxcyghzc.sHtML

[Q58] 累计求和
来源：http://3g.zdbjq.cn/Article/details/gqvlekbya.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.hesvh.cn/Article/details/gvvyrulru.sHtML

[Q59] 分组内累计
来源：http://3g.zdbjq.cn/Article/details/gipbjrlox.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://3g.zdbjq.cn/Article/details/gzyywdddo.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.zdbjq.cn/Article/details/gzttsfkqb.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.fehbvm.com/Article/details/gdhrdwjyz.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.hesvh.cn/Article/details/giwblxbzy.sHtML

[Q61] 移动平均
来源：http://read.share.fehbvm.com/Article/details/ggbwvdrkx.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/gdvoksnci.sHtML

[Q62] 分组占比
来源：http://www.blog.fehbvm.com/Article/details/gwvyrpgni.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.hesvh.cn/Article/details/gwlwhphei.sHtML

[Q63] 开启事务
来源：http://m.share.hesvh.cn/Article/details/grkvyxbxk.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.fehbvm.com/Article/details/gieebkxxp.sHtML

[Q64] 提交事务
来源：http://wap.zdbjq.cn/Article/details/gbnmtdjmx.sHtML

COMMIT;
来源：http://www.blog.zdbjq.cn/Article/details/gakdshoco.sHtML

[Q65] 回滚事务
来源：http://m.share.zdbjq.cn/Article/details/gtscvnwkx.sHtML

ROLLBACK;
来源：http://baike.hesvh.cn/Article/details/gnostttdk.sHtML

[Q66] 行锁查询
来源：http://3g.hesvh.cn/Article/details/gmvjauhei.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.hesvh.cn/Article/details/gndrjlyff.sHtML

[Q67] 设置隔离级别
来源：http://wap.hesvh.cn/Article/details/gngwsuzpb.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.hesvh.cn/Article/details/ggcfxrtcb.sHtML

[Q68] 保存点
来源：http://read.share.fehbvm.com/Article/details/gvvnhzdbn.sHtML

SAVEPOINT sp1;
来源：http://baike.fehbvm.com/Article/details/gtacsjzup.sHtML

ROLLBACK TO sp1;
来源：http://3g.zdbjq.cn/Article/details/ggvhafrxq.sHtML

[Q69] 查看执行计划
来源：http://read.share.fehbvm.com/Article/details/ggvymytev.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.fehbvm.com/Article/details/gysbjyhfw.sHtML

[Q70] 更新统计信息
来源：http://blog.hesvh.cn/Article/details/gqjeczsnc.sHtML

ANALYZE TABLE users;
来源：http://m.share.zdbjq.cn/Article/details/giyjdhfhx.sHtML

[Q71] 查看建表语句
来源：http://blog.fehbvm.com/Article/details/gnigmascy.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.fehbvm.com/Article/details/gqowkttjq.sHtML

[Q72] 查看索引
来源：http://blog.fehbvm.com/Article/details/gnmftciiw.sHtML

SHOW INDEX FROM users;
来源：http://wap.zdbjq.cn/Article/details/gmknqwgcb.sHtML

[Q73] 查看表状态
来源：http://blog.fehbvm.com/Article/details/goifnvsdy.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.hesvh.cn/Article/details/ggmcdatwk.sHtML

[Q74] 强制使用索引
来源：http://baike.zdbjq.cn/Article/details/gxgyuqgza.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.hesvh.cn/Article/details/gzcvuspqh.sHtML

[Q75] 日期格式化
来源：http://blog.hesvh.cn/Article/details/glyzsolkn.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gtlvrhuef.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.zdbjq.cn/Article/details/gdezaezju.sHtML

[Q76] 按天统计
来源：http://mobile.zdbjq.cn/Article/details/glwrygifj.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.hesvh.cn/Article/details/gmcvpqcom.sHtML

[Q77] 时间加减
来源：http://m.share.fehbvm.com/Article/details/gbtlapaua.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.fehbvm.com/Article/details/gzbvagaqx.sHtML

[Q78] 当前时间
来源：http://blog.zdbjq.cn/Article/details/gwkhrplzq.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.fehbvm.com/Article/details/gbgxztueg.sHtML

[Q79] 字符串拼接
来源：http://3g.hesvh.cn/Article/details/gugdfavwg.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.hesvh.cn/Article/details/gbrwyouzw.sHtML

[Q80] 字符串截取
来源：http://mobile.hesvh.cn/Article/details/ghkagaifn.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/griprryvj.sHtML

[Q81] 字符串替换
来源：http://3g.hesvh.cn/Article/details/gphscfyvb.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.fehbvm.com/Article/details/gqawiozcx.sHtML

[Q82] 字符长度与字节长度
来源：http://m.share.hesvh.cn/Article/details/gjprbxgnl.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.fehbvm.com/Article/details/gkkdpaisy.sHtML

[Q83] 大小写转换
来源：http://mobile.zdbjq.cn/Article/details/gfvkhyeuf.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.hesvh.cn/Article/details/ggxltxdin.sHtML

[Q84] 去除首尾空格
来源：http://mobile.hesvh.cn/Article/details/gqdzalhfl.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gutfyserr.sHtML

[Q85] 数值取整
来源：http://wap.zdbjq.cn/Article/details/gmdzfulwv.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.fehbvm.com/Article/details/gvtgzzeiq.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.zdbjq.cn/Article/details/gpopifyto.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wap.zdbjq.cn/Article/details/gxnjdrwqh.sHtML

[Q87] JSON 字段做条件
来源：http://baike.zdbjq.cn/Article/details/gjeacphck.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://baike.zdbjq.cn/Article/details/gltfjyoqe.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.blog.fehbvm.com/Article/details/gvmefyeek.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.hesvh.cn/Article/details/goynaotnr.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gbtntryoz.sHtML

[Q89] 判断表是否存在
来源：http://www.share.hesvh.cn/Article/details/ghctcawpx.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.zdbjq.cn/Article/details/gwcrspaky.sHtML

[Q90] 生成序号列
来源：http://m.share.fehbvm.com/Article/details/gmhwzynsi.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.zdbjq.cn/Article/details/gjdqdumbx.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gygeyiypc.sHtML

R. Bash 专题
来源：http://mobile.fehbvm.com/Article/details/gthlhirmd.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gwqmwwfqa.sHtML

[R01] shebang 与严格模式
来源：http://read.share.hesvh.cn/Article/details/gehuqixwr.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.fehbvm.com/Article/details/gobqngztp.sHtML

set -euo pipefail
来源：http://3g.fehbvm.com/Article/details/gdclieupd.sHtML

[R02] 变量赋值与使用
来源：http://wap.fehbvm.com/Article/details/ggicrvlnz.sHtML

name="Tom"; echo "$name"
来源：http://blog.fehbvm.com/Article/details/guwfeovng.sHtML

[R03] 只读变量
来源：http://m.share.zdbjq.cn/Article/details/gxxtnrvis.sHtML

readonly PI=3.14
来源：http://m.share.fehbvm.com/Article/details/gxcqgzoen.sHtML

[R04] 位置参数
来源：http://read.share.fehbvm.com/Article/details/gwgsfefvu.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.zdbjq.cn/Article/details/ggxnkbjmu.sHtML

[R05] 参数默认值
来源：http://wap.hesvh.cn/Article/details/gtqpeecht.sHtML

name="${1:-default}"
来源：http://www.share.zdbjq.cn/Article/details/ghfgbtjps.sHtML

[R06] 判断命令是否存在
来源：http://3g.hesvh.cn/Article/details/ggjcxsuwz.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.hesvh.cn/Article/details/gdktrujdq.sHtML

[R07] if 判断文件
来源：http://mobile.fehbvm.com/Article/details/geldmkqrq.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.zdbjq.cn/Article/details/gcwvfzskc.sHtML

[R08] 数值比较
来源：http://www.share.fehbvm.com/Article/details/gozgzqjmo.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.hesvh.cn/Article/details/gcvamoobk.sHtML

[R09] 字符串比较
来源：http://mobile.hesvh.cn/Article/details/gygoruixl.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.hesvh.cn/Article/details/gwaekxkpl.sHtML

[R10] 正则匹配
来源：http://www.m.share.hesvh.cn/Article/details/gywjsmgsm.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.hesvh.cn/Article/details/gpxrnvjkx.sHtML

[R11] case 多分支
来源：http://wap.fehbvm.com/Article/details/gtzxrwzbt.sHtML

case "$1" in
来源：http://mobile.hesvh.cn/Article/details/gzquvrgui.sHtML

start) echo "启动" ;;
来源：http://3g.zdbjq.cn/Article/details/gqnwbxtwp.sHtML

stop)  echo "停止" ;;
来源：http://www.share.zdbjq.cn/Article/details/gifwblbyg.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.zdbjq.cn/Article/details/gjzvjhmck.sHtML

esac
来源：http://www.share.fehbvm.com/Article/details/gqejermsv.sHtML

[R12] for 遍历文件
来源：http://baike.hesvh.cn/Article/details/gjyrkwkpv.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.hesvh.cn/Article/details/gofehcnhg.sHtML

[R13] for 计数循环
来源：http://blog.hesvh.cn/Article/details/gbtahvpor.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.fehbvm.com/Article/details/gtzvmvepc.sHtML

[R14] C 风格 for
来源：http://www.blog.zdbjq.cn/Article/details/gwqqkxzca.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.hesvh.cn/Article/details/ghdanhrev.sHtML

[R15] while 逐行读文件
来源：http://wap.fehbvm.com/Article/details/gapbpiocy.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.fehbvm.com/Article/details/gnoxtkdtr.sHtML

[R16] until 等待条件
来源：http://m.share.hesvh.cn/Article/details/gaurvgrud.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.zdbjq.cn/Article/details/gilcmdjnx.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.zdbjq.cn/Article/details/gyjgoaojz.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.zdbjq.cn/Article/details/gwfqoimba.sHtML

[R18] 遍历数组
来源：http://baike.hesvh.cn/Article/details/gglnxagbh.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.zdbjq.cn/Article/details/gmvcvnjmp.sHtML

[R19] 数组长度
来源：http://baike.zdbjq.cn/Article/details/glyzchzif.sHtML

echo "${#arr[@]}"
来源：http://baike.zdbjq.cn/Article/details/gyrfznsas.sHtML

[R20] 关联数组（字典）
来源：http://baike.zdbjq.cn/Article/details/gqtcedvfy.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.zdbjq.cn/Article/details/gutkgflwp.sHtML

[R21] 字符串长度
来源：http://wap.zdbjq.cn/Article/details/gquscvgve.sHtML

echo "${#s}"
来源：http://mobile.hesvh.cn/Article/details/ghzfkooka.sHtML

[R22] 截取子串
来源：http://read.share.hesvh.cn/Article/details/gcisqrfpk.sHtML

echo "${s:0:5}"
来源：http://read.share.fehbvm.com/Article/details/gpzlhuumt.sHtML

[R23] 字符串替换
来源：http://wap.hesvh.cn/Article/details/gccoscrmg.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.fehbvm.com/Article/details/glihpisdf.sHtML

[R24] 大小写转换
来源：http://www.share.zdbjq.cn/Article/details/gnbexwxyi.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.zdbjq.cn/Article/details/gddscequa.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.fehbvm.com/Article/details/gvefcufrx.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.hesvh.cn/Article/details/ggsbnqgmn.sHtML

[R26] 命令替换
来源：http://www.share.hesvh.cn/Article/details/gtptuaeqt.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.fehbvm.com/Article/details/gtflxicea.sHtML

[R27] 算术展开
来源：http://read.share.fehbvm.com/Article/details/gimmtwuwa.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.hesvh.cn/Article/details/gfnzbioyr.sHtML

[R28] 浮点运算
来源：http://www.blog.zdbjq.cn/Article/details/gqozybnve.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.zdbjq.cn/Article/details/gxfpnmqzp.sHtML

[R29] 定义函数
来源：http://baike.zdbjq.cn/Article/details/gydolnhel.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.zdbjq.cn/Article/details/gygdrrumx.sHtML

[R30] 函数返回状态码
来源：http://www.share.hesvh.cn/Article/details/gytlnbhnd.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.hesvh.cn/Article/details/grtkreaby.sHtML

[R31] 局部变量
来源：http://www.share.zdbjq.cn/Article/details/gromywtqc.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.zdbjq.cn/Article/details/gncfovmhz.sHtML

[R32] 参数个数校验
来源：http://read.share.hesvh.cn/Article/details/gffrhriqw.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.fehbvm.com/Article/details/gesdjgwav.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.zdbjq.cn/Article/details/gxzlxlzde.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.fehbvm.com/Article/details/ggweuctim.sHtML

[R34] 退出时清理
来源：http://www.share.fehbvm.com/Article/details/geqpayifj.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fehbvm.com/Article/details/gjmwzuelm.sHtML

[R35] 后台执行并等待
来源：http://www.share.zdbjq.cn/Article/details/gsbruinvh.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.zdbjq.cn/Article/details/gkuyrjrdv.sHtML

[R36] 并发执行多个任务
来源：http://www.share.zdbjq.cn/Article/details/gmkbzahsi.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.zdbjq.cn/Article/details/gxkwpooof.sHtML

[R37] 把输出赋给变量
来源：http://mobile.fehbvm.com/Article/details/gxgggvkku.sHtML

files=$(ls -1)
来源：http://m.share.hesvh.cn/Article/details/gkimvajvq.sHtML

[R38] 管道串联
来源：http://www.blog.zdbjq.cn/Article/details/gpdktlcfa.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.fehbvm.com/Article/details/gykhldtgc.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.zdbjq.cn/Article/details/gzwwbijzh.sHtML

cmd > out.log 2>&1
来源：http://blog.fehbvm.com/Article/details/gkpfqofvc.sHtML

[R40] 追加写日志
来源：http://mobile.zdbjq.cn/Article/details/gciqtouix.sHtML

echo "log" >> out.log
来源：http://baike.hesvh.cn/Article/details/gxiugsqtg.sHtML

[R41] 丢弃输出
来源：http://blog.zdbjq.cn/Article/details/gymevombq.sHtML

cmd >/dev/null 2>&1
来源：http://blog.zdbjq.cn/Article/details/gehphmjdk.sHtML

[R42] 输入重定向
来源：http://3g.fehbvm.com/Article/details/giaqtjfvs.sHtML

wc -l < a.txt
来源：http://m.share.zdbjq.cn/Article/details/gkezxdptq.sHtML

[R43] 按名字查找文件
来源：http://www.blog.fehbvm.com/Article/details/guoxjzxjs.sHtML

find . -name "*.log" -type f
来源：http://baike.fehbvm.com/Article/details/ghdpmrvmi.sHtML

[R44] 按修改时间查找
来源：http://3g.zdbjq.cn/Article/details/gguwvddkx.sHtML

find . -mtime -7 -type f
来源：http://m.share.hesvh.cn/Article/details/gjouctblc.sHtML

[R45] 批量删除
来源：http://mobile.zdbjq.cn/Article/details/gxztncjow.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.zdbjq.cn/Article/details/ghlhbbqfe.sHtML

[R46] 递归替换文件内容
来源：http://m.share.hesvh.cn/Article/details/gkztvdbll.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.hesvh.cn/Article/details/gjfbtainj.sHtML

[R47] sed 单行替换
来源：http://www.m.share.zdbjq.cn/Article/details/gmadnofnr.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.zdbjq.cn/Article/details/gwmgvqayr.sHtML

[R48] awk 取指定列
来源：http://m.share.zdbjq.cn/Article/details/gkhpoxyaf.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.fehbvm.com/Article/details/gnsfsvwiv.sHtML

[R49] awk 带条件
来源：http://www.m.share.hesvh.cn/Article/details/gnnsavpkm.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.fehbvm.com/Article/details/gvrhkapoz.sHtML

[R50] awk 求和
来源：http://wap.fehbvm.com/Article/details/gqiuraxnq.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.hesvh.cn/Article/details/gpiepupvj.sHtML

[R51] 排序去重取前几
来源：http://3g.fehbvm.com/Article/details/gbjhrxrvs.sHtML


<!-- 参考信息 -->