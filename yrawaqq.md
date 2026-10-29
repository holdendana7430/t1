代发 wailian999

);
来源：http://www.m.share.hesvh.cn/Article/details/gwafhdmtb.sHtML

[Q03] 增加列
来源：http://mobile.zdbjq.cn/Article/details/gunewwcsb.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://3g.hesvh.cn/Article/details/gkxomroex.sHtML

[Q04] 修改列类型
来源：http://m.share.fehbvm.com/Article/details/gmpuxkbbp.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://3g.zdbjq.cn/Article/details/gxhapkbik.sHtML

[Q05] 重命名列
来源：http://blog.fehbvm.com/Article/details/gyttdagba.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://baike.hesvh.cn/Article/details/gsidsurbj.sHtML

[Q06] 删除列
来源：http://read.share.hesvh.cn/Article/details/ghuwpydzf.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.blog.fehbvm.com/Article/details/gljuttnmw.sHtML

[Q07] 删除表
来源：http://blog.fehbvm.com/Article/details/gpcdedqoo.sHtML

DROP TABLE IF EXISTS orders;
来源：http://blog.hesvh.cn/Article/details/gdnctmeli.sHtML

[Q08] 创建普通索引
来源：http://baike.fehbvm.com/Article/details/gjrapnrwv.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://mobile.zdbjq.cn/Article/details/grlsxzfse.sHtML

[Q09] 创建唯一索引
来源：http://m.share.fehbvm.com/Article/details/gsbgthdse.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://baike.zdbjq.cn/Article/details/gukyfmwkt.sHtML

[Q10] 插入单行
来源：http://mobile.hesvh.cn/Article/details/gfkrjonta.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.blog.zdbjq.cn/Article/details/gbodvjpuc.sHtML

[Q11] 一次插入多行
来源：http://read.share.fehbvm.com/Article/details/ggacifjcu.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.fehbvm.com/Article/details/gmcotatcr.sHtML

[Q12] 插入后取自增 ID
来源：http://www.share.hesvh.cn/Article/details/gmvyclirp.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://m.share.fehbvm.com/Article/details/gsirhqkcs.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://blog.hesvh.cn/Article/details/gtdonnzta.sHtML

[Q13] 忽略重复插入
来源：http://mobile.fehbvm.com/Article/details/gvcgljfhg.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://read.share.fehbvm.com/Article/details/gcykqhpbs.sHtML

[Q14] 存在则更新（upsert）
来源：http://mobile.zdbjq.cn/Article/details/glhxendyn.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mobile.hesvh.cn/Article/details/gmcrirmix.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mobile.zdbjq.cn/Article/details/gvewompee.sHtML

[Q15] 查询全部
来源：http://baike.zdbjq.cn/Article/details/ghwdqzcvb.sHtML

SELECT * FROM users;
来源：http://m.share.hesvh.cn/Article/details/godfbcfkj.sHtML

[Q16] 查询指定列
来源：http://m.share.zdbjq.cn/Article/details/gjeonxohq.sHtML

SELECT id, name FROM users;
来源：http://blog.hesvh.cn/Article/details/gakpjhwab.sHtML

[Q17] 条件查询
来源：http://read.share.hesvh.cn/Article/details/galjgfure.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.fehbvm.com/Article/details/gxmveohiu.sHtML

[Q18] 模糊匹配
来源：http://wap.hesvh.cn/Article/details/gsnsbzhci.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.share.fehbvm.com/Article/details/gvsztptmr.sHtML

[Q19] 范围查询
来源：http://www.m.share.zdbjq.cn/Article/details/gsyrhwkja.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.blog.zdbjq.cn/Article/details/gafbuklhu.sHtML

[Q20] IN 列表
来源：http://wap.hesvh.cn/Article/details/grbavkwlv.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://blog.zdbjq.cn/Article/details/grwgxxshj.sHtML

[Q21] 空值判断
来源：http://www.blog.fehbvm.com/Article/details/gzxtdxsai.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://3g.zdbjq.cn/Article/details/gmwjdytdu.sHtML

[Q22] 排序
来源：http://read.share.zdbjq.cn/Article/details/gsgrgevjq.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mobile.fehbvm.com/Article/details/gekugxdcm.sHtML

[Q23] 分页
来源：http://mobile.hesvh.cn/Article/details/gckfbpvad.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mobile.fehbvm.com/Article/details/gzprodowj.sHtML

[Q24] 去重
来源：http://wap.fehbvm.com/Article/details/guslubypj.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.share.fehbvm.com/Article/details/gwppzvpux.sHtML

[Q25] 只取前 N 条
来源：http://3g.hesvh.cn/Article/details/gzjnpbomp.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mobile.fehbvm.com/Article/details/gvotcxqvs.sHtML

[Q26] 计数
来源：http://www.m.share.hesvh.cn/Article/details/grsyyxzvu.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.hesvh.cn/Article/details/gkaijixxj.sHtML

[Q27] 条件计数
来源：http://3g.zdbjq.cn/Article/details/gqbmbhltx.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://read.share.fehbvm.com/Article/details/gkdihsoou.sHtML

[Q28] 求和与平均
来源：http://wap.fehbvm.com/Article/details/gdqfmuwlf.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.hesvh.cn/Article/details/gdyksrxoq.sHtML

[Q29] 最大最小值
来源：http://3g.hesvh.cn/Article/details/gunszfcuk.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://baike.zdbjq.cn/Article/details/gocyencnn.sHtML

[Q30] 分组统计
来源：http://read.share.fehbvm.com/Article/details/gnuqbavzy.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.zdbjq.cn/Article/details/gcrososdu.sHtML

[Q31] 分组后过滤
来源：http://mobile.fehbvm.com/Article/details/gytgyagsq.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.zdbjq.cn/Article/details/gswcvibcr.sHtML

[Q32] 分组拼接字符串
来源：http://www.share.zdbjq.cn/Article/details/gjvybwntn.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://blog.zdbjq.cn/Article/details/gvwfyxqqp.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mobile.zdbjq.cn/Article/details/gccopgjsd.sHtML

[Q33] 多列分组
来源：http://www.m.share.zdbjq.cn/Article/details/gohgvjqtw.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.blog.zdbjq.cn/Article/details/ghjihqwgi.sHtML

[Q34] 每组取第一条
来源：http://3g.zdbjq.cn/Article/details/gpkqkzddu.sHtML

SELECT * FROM (
来源：http://www.blog.fehbvm.com/Article/details/geaamwufv.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://m.share.zdbjq.cn/Article/details/gcibjkujn.sHtML

) t WHERE rn = 1;
来源：http://3g.hesvh.cn/Article/details/gdkcgxdgp.sHtML

[Q35] 内连接
来源：http://blog.hesvh.cn/Article/details/gukufnxuq.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://read.share.zdbjq.cn/Article/details/grhbvlvxq.sHtML

[Q36] 左连接
来源：http://read.share.hesvh.cn/Article/details/gregncwzm.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mobile.fehbvm.com/Article/details/glajfodjj.sHtML

[Q37] 右连接
来源：http://www.m.share.hesvh.cn/Article/details/gavqipssa.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.fehbvm.com/Article/details/ghvvanhiw.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.fehbvm.com/Article/details/gdxyeuyqi.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.share.hesvh.cn/Article/details/gajbrcgov.sHtML

[Q39] 自连接（查上下级）
来源：http://baike.hesvh.cn/Article/details/goaqnkrts.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.zdbjq.cn/Article/details/gbhsmxosk.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://m.share.fehbvm.com/Article/details/gbuxpbfzr.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.m.share.hesvh.cn/Article/details/glahkqyps.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mobile.zdbjq.cn/Article/details/gwpuipuky.sHtML

[Q41] 多表连接
来源：http://wap.zdbjq.cn/Article/details/gkeuphklk.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.hesvh.cn/Article/details/gwkysykaw.sHtML

JOIN users u ON u.id = o.user_id
来源：http://mobile.fehbvm.com/Article/details/gmxgydvoi.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.zdbjq.cn/Article/details/gpsivtegx.sHtML

[Q42] 连接条件附加过滤
来源：http://read.share.zdbjq.cn/Article/details/gabrekvqo.sHtML

SELECT u.name, o.amount FROM users u
来源：http://3g.hesvh.cn/Article/details/gxcrbnphe.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://m.share.hesvh.cn/Article/details/guylwitte.sHtML

[Q43] 标量子查询
来源：http://www.share.fehbvm.com/Article/details/gnwiehvkw.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.share.fehbvm.com/Article/details/ghiucbrjt.sHtML

[Q44] IN 子查询
来源：http://blog.hesvh.cn/Article/details/grnofrrnv.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.hesvh.cn/Article/details/gpnbglxdf.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.hesvh.cn/Article/details/grpeltqyi.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.fehbvm.com/Article/details/gbneqslgy.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.hesvh.cn/Article/details/grigkztnm.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.zdbjq.cn/Article/details/gvmmwxtlw.sHtML

[Q47] 与平均值比较
来源：http://wap.hesvh.cn/Article/details/genhozsas.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://baike.zdbjq.cn/Article/details/gxnsrtmwa.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.zdbjq.cn/Article/details/gujznynzp.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.blog.fehbvm.com/Article/details/gsexsinnz.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.hesvh.cn/Article/details/gouxsovvf.sHtML

[Q49] 更新单行
来源：http://mobile.hesvh.cn/Article/details/gledmayhq.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://m.share.zdbjq.cn/Article/details/gwwjudott.sHtML

[Q50] 批量更新
来源：http://m.share.zdbjq.cn/Article/details/gljktzjrc.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.m.share.fehbvm.com/Article/details/gwpfyizob.sHtML

[Q51] 用子查询更新
来源：http://read.share.hesvh.cn/Article/details/grfbmbwgt.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mobile.fehbvm.com/Article/details/gkyizuezs.sHtML

[Q52] 删除指定行
来源：http://baike.zdbjq.cn/Article/details/gsdgxkyfk.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.zdbjq.cn/Article/details/gmjtlpnsd.sHtML

[Q53] 按条件删除
来源：http://www.share.zdbjq.cn/Article/details/gbzplrshm.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.zdbjq.cn/Article/details/gmvhtjnfb.sHtML

[Q54] 清空表
来源：http://www.m.share.fehbvm.com/Article/details/gdamttwsq.sHtML

TRUNCATE TABLE logs;
来源：http://mobile.zdbjq.cn/Article/details/gzyiekqlp.sHtML

[Q55] 排名（并列占位）
来源：http://www.share.hesvh.cn/Article/details/gnifajoii.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.fehbvm.com/Article/details/glgcfrwcm.sHtML

[Q56] 密集排名（并列不占位）
来源：http://mobile.zdbjq.cn/Article/details/gekehulxb.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mobile.zdbjq.cn/Article/details/grukmkljs.sHtML

[Q57] 行号
来源：http://baike.fehbvm.com/Article/details/gwhvgfiwv.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.fehbvm.com/Article/details/govjpshdb.sHtML

[Q58] 累计求和
来源：http://m.share.fehbvm.com/Article/details/gmeicvohe.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.share.hesvh.cn/Article/details/ggjjhkyki.sHtML

[Q59] 分组内累计
来源：http://www.share.hesvh.cn/Article/details/gmdqtdmbq.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.hesvh.cn/Article/details/gofrkpvue.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.zdbjq.cn/Article/details/gpnzreoic.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://blog.fehbvm.com/Article/details/gjkqzxtiv.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.zdbjq.cn/Article/details/guownynfy.sHtML

[Q61] 移动平均
来源：http://www.share.hesvh.cn/Article/details/gygbyxzhz.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://blog.hesvh.cn/Article/details/gdwaakxps.sHtML

[Q62] 分组占比
来源：http://www.share.hesvh.cn/Article/details/gbqvmzbyf.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.fehbvm.com/Article/details/govvrqtqs.sHtML

[Q63] 开启事务
来源：http://3g.zdbjq.cn/Article/details/gollvldkm.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://3g.zdbjq.cn/Article/details/gvvqjivek.sHtML

[Q64] 提交事务
来源：http://wap.hesvh.cn/Article/details/grdazqzfh.sHtML

COMMIT;
来源：http://blog.fehbvm.com/Article/details/gfcwymhwn.sHtML

[Q65] 回滚事务
来源：http://www.blog.fehbvm.com/Article/details/gzlktfrac.sHtML

ROLLBACK;
来源：http://www.m.share.zdbjq.cn/Article/details/gosasacls.sHtML

[Q66] 行锁查询
来源：http://mobile.hesvh.cn/Article/details/gfxhsvhrt.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.blog.fehbvm.com/Article/details/gdmwfiwat.sHtML

[Q67] 设置隔离级别
来源：http://3g.fehbvm.com/Article/details/gxuzvqott.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.fehbvm.com/Article/details/gpuboxfxk.sHtML

[Q68] 保存点
来源：http://www.m.share.hesvh.cn/Article/details/gbnfuxuqk.sHtML

SAVEPOINT sp1;
来源：http://baike.hesvh.cn/Article/details/giqspydwz.sHtML

ROLLBACK TO sp1;
来源：http://baike.fehbvm.com/Article/details/gxdmroejo.sHtML

[Q69] 查看执行计划
来源：http://baike.hesvh.cn/Article/details/gbaqlufwq.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.hesvh.cn/Article/details/gdlfqeykm.sHtML

[Q70] 更新统计信息
来源：http://m.share.fehbvm.com/Article/details/gobwitfgf.sHtML

ANALYZE TABLE users;
来源：http://3g.hesvh.cn/Article/details/gqpmzcpjg.sHtML

[Q71] 查看建表语句
来源：http://blog.fehbvm.com/Article/details/gtsdcejos.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.fehbvm.com/Article/details/gtsbtmxze.sHtML

[Q72] 查看索引
来源：http://www.m.share.fehbvm.com/Article/details/gyqdnokgb.sHtML

SHOW INDEX FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/ghpldpzds.sHtML

[Q73] 查看表状态
来源：http://m.share.hesvh.cn/Article/details/gumdvqjbi.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.fehbvm.com/Article/details/googbhgqi.sHtML

[Q74] 强制使用索引
来源：http://www.share.zdbjq.cn/Article/details/gexcuyzff.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.fehbvm.com/Article/details/gocfmhyny.sHtML

[Q75] 日期格式化
来源：http://www.blog.zdbjq.cn/Article/details/gtactlyqf.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.hesvh.cn/Article/details/gkpvshplw.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.zdbjq.cn/Article/details/gnevxiozb.sHtML

[Q76] 按天统计
来源：http://www.blog.zdbjq.cn/Article/details/gsnpqitvb.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.fehbvm.com/Article/details/gyjpecosw.sHtML

[Q77] 时间加减
来源：http://blog.zdbjq.cn/Article/details/grwsebmxd.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.fehbvm.com/Article/details/gxvefbcwm.sHtML

[Q78] 当前时间
来源：http://www.m.share.fehbvm.com/Article/details/gzuxoowlh.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.zdbjq.cn/Article/details/grzxnoxdy.sHtML

[Q79] 字符串拼接
来源：http://mobile.hesvh.cn/Article/details/ggzbdceri.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.hesvh.cn/Article/details/gqmuriwum.sHtML

[Q80] 字符串截取
来源：http://read.share.hesvh.cn/Article/details/gixhyvxpc.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.fehbvm.com/Article/details/gmuekdfxt.sHtML

[Q81] 字符串替换
来源：http://blog.fehbvm.com/Article/details/grqtwvhov.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.fehbvm.com/Article/details/gwvcvsaby.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.zdbjq.cn/Article/details/gnlkscvao.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.hesvh.cn/Article/details/gwjftxaeh.sHtML

[Q83] 大小写转换
来源：http://mobile.fehbvm.com/Article/details/gaodxowld.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.hesvh.cn/Article/details/gfkeftbrp.sHtML

[Q84] 去除首尾空格
来源：http://mobile.fehbvm.com/Article/details/gflbekjzw.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.zdbjq.cn/Article/details/gwvhovfmq.sHtML

[Q85] 数值取整
来源：http://www.blog.zdbjq.cn/Article/details/ghcyfhzvd.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.zdbjq.cn/Article/details/gizsmlykl.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.zdbjq.cn/Article/details/gnvdigorr.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.fehbvm.com/Article/details/gplelxinv.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.hesvh.cn/Article/details/glnubtzvu.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://baike.hesvh.cn/Article/details/gbryiqzzk.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.fehbvm.com/Article/details/gfyhkhida.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.zdbjq.cn/Article/details/gmqijekmg.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.fehbvm.com/Article/details/gonqiwpnx.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.fehbvm.com/Article/details/gbeplphjz.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.zdbjq.cn/Article/details/guewqttcn.sHtML

[Q90] 生成序号列
来源：http://www.m.share.hesvh.cn/Article/details/gssptmrky.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.hesvh.cn/Article/details/gswbvjwql.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gtwtuudso.sHtML

R. Bash 专题
来源：http://wap.hesvh.cn/Article/details/grfxmvtzq.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gbuvozrli.sHtML

[R01] shebang 与严格模式
来源：http://3g.fehbvm.com/Article/details/gvxwhiltx.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.zdbjq.cn/Article/details/gfsxhkxws.sHtML

set -euo pipefail
来源：http://blog.hesvh.cn/Article/details/gbkxlnnrb.sHtML

[R02] 变量赋值与使用
来源：http://m.share.hesvh.cn/Article/details/gkqgihata.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.fehbvm.com/Article/details/gapxnbhdw.sHtML

[R03] 只读变量
来源：http://www.m.share.zdbjq.cn/Article/details/gvpygrrfg.sHtML

readonly PI=3.14
来源：http://m.share.hesvh.cn/Article/details/gjstzbtas.sHtML

[R04] 位置参数
来源：http://wap.hesvh.cn/Article/details/goherojde.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.fehbvm.com/Article/details/gyqhetrlp.sHtML

[R05] 参数默认值
来源：http://3g.zdbjq.cn/Article/details/gxbvyygau.sHtML

name="${1:-default}"
来源：http://read.share.hesvh.cn/Article/details/gasapmojh.sHtML

[R06] 判断命令是否存在
来源：http://baike.fehbvm.com/Article/details/gyhkycgrw.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.zdbjq.cn/Article/details/gpzxamthz.sHtML

[R07] if 判断文件
来源：http://3g.zdbjq.cn/Article/details/gdiephdie.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.hesvh.cn/Article/details/gxgzsvftp.sHtML

[R08] 数值比较
来源：http://read.share.hesvh.cn/Article/details/gggmauplx.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.fehbvm.com/Article/details/gufrvwwso.sHtML

[R09] 字符串比较
来源：http://wap.hesvh.cn/Article/details/gralqljno.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.hesvh.cn/Article/details/gjaawgsdt.sHtML

[R10] 正则匹配
来源：http://m.share.fehbvm.com/Article/details/grsuoyvbo.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.hesvh.cn/Article/details/gnuxuqteh.sHtML

[R11] case 多分支
来源：http://blog.zdbjq.cn/Article/details/gkwdmzqqu.sHtML

case "$1" in
来源：http://wap.hesvh.cn/Article/details/gflrpxxew.sHtML

start) echo "启动" ;;
来源：http://read.share.hesvh.cn/Article/details/gvjvnlhgc.sHtML

stop)  echo "停止" ;;
来源：http://3g.zdbjq.cn/Article/details/gucrhwgkz.sHtML

*)     echo "未知命令" ;;
来源：http://3g.zdbjq.cn/Article/details/gkmohckpe.sHtML

esac
来源：http://blog.zdbjq.cn/Article/details/gavuyxssc.sHtML

[R12] for 遍历文件
来源：http://www.blog.fehbvm.com/Article/details/gvthpgxlz.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.fehbvm.com/Article/details/gvmgirlha.sHtML

[R13] for 计数循环
来源：http://baike.zdbjq.cn/Article/details/gfnhbguvv.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.fehbvm.com/Article/details/gqqxxtron.sHtML

[R14] C 风格 for
来源：http://mobile.hesvh.cn/Article/details/gqwtautmm.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.zdbjq.cn/Article/details/gckotufrf.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.hesvh.cn/Article/details/gwhtphute.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.fehbvm.com/Article/details/gmudgpkqg.sHtML

[R16] until 等待条件
来源：http://www.m.share.zdbjq.cn/Article/details/ggrwjmdzx.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.zdbjq.cn/Article/details/gjlejuyfc.sHtML

[R17] 数组定义与取值
来源：http://m.share.zdbjq.cn/Article/details/gmujovwsh.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.zdbjq.cn/Article/details/gwlfrxwai.sHtML

[R18] 遍历数组
来源：http://blog.hesvh.cn/Article/details/goavvvtci.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.hesvh.cn/Article/details/ggckjllzm.sHtML

[R19] 数组长度
来源：http://wap.hesvh.cn/Article/details/gvvzhohxt.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.zdbjq.cn/Article/details/gwwbhunel.sHtML

[R20] 关联数组（字典）
来源：http://m.share.hesvh.cn/Article/details/grlmyxebk.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.fehbvm.com/Article/details/gutmupxcz.sHtML

[R21] 字符串长度
来源：http://3g.hesvh.cn/Article/details/gzxkseatv.sHtML

echo "${#s}"
来源：http://wap.hesvh.cn/Article/details/gpigwqbys.sHtML

[R22] 截取子串
来源：http://www.m.share.zdbjq.cn/Article/details/gtwtfhcib.sHtML

echo "${s:0:5}"
来源：http://m.share.zdbjq.cn/Article/details/gwfohfwhq.sHtML

[R23] 字符串替换
来源：http://www.m.share.zdbjq.cn/Article/details/gjfmfdckf.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.hesvh.cn/Article/details/gdbzkcgzx.sHtML

[R24] 大小写转换
来源：http://3g.hesvh.cn/Article/details/gwolplnay.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.hesvh.cn/Article/details/gbcjqwmdo.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.zdbjq.cn/Article/details/gnpxlgphp.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.fehbvm.com/Article/details/gfndjstdm.sHtML

[R26] 命令替换
来源：http://mobile.hesvh.cn/Article/details/ggmxyutar.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.hesvh.cn/Article/details/goxetwbbd.sHtML

[R27] 算术展开
来源：http://mobile.zdbjq.cn/Article/details/gmdnlcprg.sHtML

echo $((1 + 2 * 3))
来源：http://baike.zdbjq.cn/Article/details/guvqvgleo.sHtML

[R28] 浮点运算
来源：http://baike.zdbjq.cn/Article/details/gxukocnxc.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.fehbvm.com/Article/details/goveqqzjj.sHtML

[R29] 定义函数
来源：http://wap.fehbvm.com/Article/details/gyjyddogk.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.hesvh.cn/Article/details/ggwmytzag.sHtML

[R30] 函数返回状态码
来源：http://wap.zdbjq.cn/Article/details/gxdwxwshz.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.fehbvm.com/Article/details/gcdcdhydi.sHtML

[R31] 局部变量
来源：http://www.share.fehbvm.com/Article/details/gyehstajq.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.zdbjq.cn/Article/details/guzdtifby.sHtML

[R32] 参数个数校验
来源：http://mobile.zdbjq.cn/Article/details/gxffjitvw.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.zdbjq.cn/Article/details/ghqhnqbuf.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.fehbvm.com/Article/details/gbwdimvoq.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.zdbjq.cn/Article/details/gwjdqzapb.sHtML

[R34] 退出时清理
来源：http://www.m.share.fehbvm.com/Article/details/ggtiqpwnq.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fehbvm.com/Article/details/gqiaqusvj.sHtML

[R35] 后台执行并等待
来源：http://baike.fehbvm.com/Article/details/gfyrmpjnv.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.hesvh.cn/Article/details/gtyiplmgr.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.zdbjq.cn/Article/details/gufhcjimt.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.zdbjq.cn/Article/details/gfsipielv.sHtML

[R37] 把输出赋给变量
来源：http://3g.hesvh.cn/Article/details/gxprwqjrn.sHtML

files=$(ls -1)
来源：http://m.share.fehbvm.com/Article/details/gbouztrlu.sHtML

[R38] 管道串联
来源：http://www.blog.fehbvm.com/Article/details/gilapaiws.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.hesvh.cn/Article/details/gusmvrcln.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.fehbvm.com/Article/details/gloavvkyr.sHtML

cmd > out.log 2>&1
来源：http://mobile.hesvh.cn/Article/details/gbvgwyurl.sHtML

[R40] 追加写日志
来源：http://blog.zdbjq.cn/Article/details/gytnynpqq.sHtML

echo "log" >> out.log
来源：http://www.share.fehbvm.com/Article/details/glkjxlrse.sHtML

[R41] 丢弃输出
来源：http://baike.hesvh.cn/Article/details/gvwgfkwqc.sHtML

cmd >/dev/null 2>&1
来源：http://baike.zdbjq.cn/Article/details/geoadiuks.sHtML

[R42] 输入重定向
来源：http://www.m.share.hesvh.cn/Article/details/geomlrsti.sHtML

wc -l < a.txt
来源：http://3g.zdbjq.cn/Article/details/gvjjybdno.sHtML

[R43] 按名字查找文件
来源：http://mobile.zdbjq.cn/Article/details/ggtpgptzp.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.fehbvm.com/Article/details/girpnuysh.sHtML

[R44] 按修改时间查找
来源：http://baike.hesvh.cn/Article/details/gwlxikphk.sHtML

find . -mtime -7 -type f
来源：http://m.share.hesvh.cn/Article/details/gnbnzllda.sHtML

[R45] 批量删除
来源：http://3g.fehbvm.com/Article/details/guobluhbe.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.zdbjq.cn/Article/details/ggxxixuel.sHtML

[R46] 递归替换文件内容
来源：http://read.share.fehbvm.com/Article/details/gpounwlzc.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.zdbjq.cn/Article/details/gctzkechh.sHtML

[R47] sed 单行替换
来源：http://m.share.zdbjq.cn/Article/details/guywukqfc.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.fehbvm.com/Article/details/gthpgmwrr.sHtML

[R48] awk 取指定列
来源：http://www.m.share.fehbvm.com/Article/details/guolbbska.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.zdbjq.cn/Article/details/grkusskjp.sHtML

[R49] awk 带条件
来源：http://www.share.hesvh.cn/Article/details/gejxprykj.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.zdbjq.cn/Article/details/ganhictwf.sHtML

[R50] awk 求和
来源：http://mobile.hesvh.cn/Article/details/gsbyajbzz.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.hesvh.cn/Article/details/gkpvshfoj.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.fehbvm.com/Article/details/gbbcthfrd.sHtML


<!-- 参考信息 -->