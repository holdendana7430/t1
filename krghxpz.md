代发 wailian999

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mobile.fehbvm.com/Article/details/gerzklrea.sHtML

TS:   if (x == null) {}
来源：http://read.share.fehbvm.com/Article/details/gjzeassds.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://m.share.hesvh.cn/Article/details/giltqlkwp.sHtML

Go:   if x == nil {}
来源：http://read.share.zdbjq.cn/Article/details/gpdqosteg.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://blog.hesvh.cn/Article/details/glganmujr.sHtML

C#:   if (x is null) {}
来源：http://www.m.share.hesvh.cn/Article/details/goairdeca.sHtML

[P07] 防抖与节流
来源：http://read.share.hesvh.cn/Article/details/ginllwsry.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://baike.fehbvm.com/Article/details/gbrtgnbgl.sHtML

PHP:  // 手写时间戳比较
来源：http://3g.zdbjq.cn/Article/details/gjnprizaf.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.hesvh.cn/Article/details/giyqgofxk.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.fehbvm.com/Article/details/gwebxlmno.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://read.share.fehbvm.com/Article/details/glkvexdmg.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.share.hesvh.cn/Article/details/gqsejsyfb.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.blog.hesvh.cn/Article/details/gyfayqnbz.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.m.share.zdbjq.cn/Article/details/gsxlbwwmq.sHtML

[P08] 处理浮点精度问题
来源：http://wap.zdbjq.cn/Article/details/ggpzmnodv.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://3g.zdbjq.cn/Article/details/gkkwfoans.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wap.hesvh.cn/Article/details/ghpeytnkg.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.zdbjq.cn/Article/details/glhuxbbxx.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.m.share.hesvh.cn/Article/details/gqvbmgfam.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.share.hesvh.cn/Article/details/glvqjoftp.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://m.share.zdbjq.cn/Article/details/golkgcbdu.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.share.fehbvm.com/Article/details/gsynnonpz.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.m.share.hesvh.cn/Article/details/gcqmcbctq.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gdiqsgvca.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://m.share.hesvh.cn/Article/details/gtfqygkrc.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gikesnadt.sHtML

[Q01] 创建表
来源：http://mobile.zdbjq.cn/Article/details/gdtqqcyss.sHtML

CREATE TABLE users (
来源：http://read.share.hesvh.cn/Article/details/gafmlxbth.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.hesvh.cn/Article/details/glinsiscl.sHtML

name VARCHAR(50) NOT NULL,
来源：http://wap.zdbjq.cn/Article/details/gwhfenwpl.sHtML

email VARCHAR(100) UNIQUE,
来源：http://wap.hesvh.cn/Article/details/gorktnvar.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://read.share.fehbvm.com/Article/details/gzzgqaieg.sHtML

);
来源：http://www.m.share.fehbvm.com/Article/details/gvxmhzobn.sHtML

[Q02] 创建带外键的表
来源：http://baike.hesvh.cn/Article/details/gamfvmrdm.sHtML

CREATE TABLE orders (
来源：http://www.blog.fehbvm.com/Article/details/gckfcbwcv.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.zdbjq.cn/Article/details/goxibozac.sHtML

user_id INT NOT NULL,
来源：http://www.blog.hesvh.cn/Article/details/gsszkzdvq.sHtML

amount DECIMAL(10, 2),
来源：http://m.share.zdbjq.cn/Article/details/gazktjonq.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.m.share.fehbvm.com/Article/details/gpufwgivc.sHtML

);
来源：http://read.share.fehbvm.com/Article/details/gceqoijwf.sHtML

[Q03] 增加列
来源：http://blog.hesvh.cn/Article/details/gsyxcnxqa.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mobile.fehbvm.com/Article/details/gxtvyxiys.sHtML

[Q04] 修改列类型
来源：http://www.share.fehbvm.com/Article/details/ghyaccuxk.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://read.share.zdbjq.cn/Article/details/gsjqfhzjw.sHtML

[Q05] 重命名列
来源：http://m.share.fehbvm.com/Article/details/giqfuowib.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.m.share.hesvh.cn/Article/details/gijovetfa.sHtML

[Q06] 删除列
来源：http://blog.fehbvm.com/Article/details/gygegequk.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://wap.zdbjq.cn/Article/details/gujooqjdj.sHtML

[Q07] 删除表
来源：http://m.share.fehbvm.com/Article/details/gvqrvwunq.sHtML

DROP TABLE IF EXISTS orders;
来源：http://blog.zdbjq.cn/Article/details/gbeyorart.sHtML

[Q08] 创建普通索引
来源：http://baike.zdbjq.cn/Article/details/gfndxqhfk.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.blog.fehbvm.com/Article/details/gwsepvilv.sHtML

[Q09] 创建唯一索引
来源：http://mobile.hesvh.cn/Article/details/gmvasiodv.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://m.share.zdbjq.cn/Article/details/gswrcoxbw.sHtML

[Q10] 插入单行
来源：http://www.share.fehbvm.com/Article/details/givhaomsv.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://read.share.hesvh.cn/Article/details/gmtoieoej.sHtML

[Q11] 一次插入多行
来源：http://wap.zdbjq.cn/Article/details/gnpporrni.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://read.share.fehbvm.com/Article/details/gqnkdcvil.sHtML

[Q12] 插入后取自增 ID
来源：http://mobile.zdbjq.cn/Article/details/gyyhcxxtq.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://wap.fehbvm.com/Article/details/gxppsvmur.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://read.share.fehbvm.com/Article/details/gxgqwvbgl.sHtML

[Q13] 忽略重复插入
来源：http://mobile.fehbvm.com/Article/details/gmtehgqgp.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://m.share.hesvh.cn/Article/details/glpjtbakm.sHtML

[Q14] 存在则更新（upsert）
来源：http://m.share.zdbjq.cn/Article/details/gcafrobjm.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mobile.zdbjq.cn/Article/details/ggevfdram.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.m.share.fehbvm.com/Article/details/gkfyeppoh.sHtML

[Q15] 查询全部
来源：http://www.share.zdbjq.cn/Article/details/gxiuvjfyv.sHtML

SELECT * FROM users;
来源：http://baike.hesvh.cn/Article/details/gcdgpvoxw.sHtML

[Q16] 查询指定列
来源：http://mobile.hesvh.cn/Article/details/ggruppzfs.sHtML

SELECT id, name FROM users;
来源：http://blog.hesvh.cn/Article/details/gkkjltgso.sHtML

[Q17] 条件查询
来源：http://mobile.zdbjq.cn/Article/details/gjyqzfgyh.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.share.fehbvm.com/Article/details/gsclkfxcz.sHtML

[Q18] 模糊匹配
来源：http://blog.hesvh.cn/Article/details/gsobtuqis.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mobile.zdbjq.cn/Article/details/gksdaemxv.sHtML

[Q19] 范围查询
来源：http://www.m.share.fehbvm.com/Article/details/gcxzgquop.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.blog.hesvh.cn/Article/details/gzubjfypr.sHtML

[Q20] IN 列表
来源：http://wap.hesvh.cn/Article/details/gjqxihpho.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.share.fehbvm.com/Article/details/gtptoadzx.sHtML

[Q21] 空值判断
来源：http://www.m.share.zdbjq.cn/Article/details/gblkxgyug.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://wap.zdbjq.cn/Article/details/gywdlvtmk.sHtML

[Q22] 排序
来源：http://wap.hesvh.cn/Article/details/gugplzydw.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://m.share.hesvh.cn/Article/details/gbdgzyyxc.sHtML

[Q23] 分页
来源：http://3g.fehbvm.com/Article/details/ghuhlbwtd.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.m.share.hesvh.cn/Article/details/grjhalakb.sHtML

[Q24] 去重
来源：http://read.share.zdbjq.cn/Article/details/gmfsipdty.sHtML

SELECT DISTINCT city FROM users;
来源：http://3g.zdbjq.cn/Article/details/gnwjcsntr.sHtML

[Q25] 只取前 N 条
来源：http://wap.hesvh.cn/Article/details/geypzcqcb.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://baike.hesvh.cn/Article/details/gmkkktcom.sHtML

[Q26] 计数
来源：http://mobile.fehbvm.com/Article/details/gsumvjuch.sHtML

SELECT COUNT(*) FROM users;
来源：http://mobile.hesvh.cn/Article/details/greasfjmo.sHtML

[Q27] 条件计数
来源：http://3g.zdbjq.cn/Article/details/gjvebohgx.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wap.fehbvm.com/Article/details/gwvmjjgfe.sHtML

[Q28] 求和与平均
来源：http://m.share.zdbjq.cn/Article/details/gfbaaukqb.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.share.hesvh.cn/Article/details/gdmudjpbm.sHtML

[Q29] 最大最小值
来源：http://wap.zdbjq.cn/Article/details/gqnvnlsoq.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://m.share.fehbvm.com/Article/details/ggslgnhvh.sHtML

[Q30] 分组统计
来源：http://baike.fehbvm.com/Article/details/gfnjpkcqk.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://read.share.zdbjq.cn/Article/details/gbvpdaurf.sHtML

[Q31] 分组后过滤
来源：http://www.share.hesvh.cn/Article/details/ghcgxyljg.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://baike.zdbjq.cn/Article/details/gdyddzwxe.sHtML

[Q32] 分组拼接字符串
来源：http://m.share.fehbvm.com/Article/details/ggpojuysh.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://read.share.hesvh.cn/Article/details/gcqsgquaz.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://blog.fehbvm.com/Article/details/gbbquxbzs.sHtML

[Q33] 多列分组
来源：http://mobile.zdbjq.cn/Article/details/gvqnkwxzm.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.share.hesvh.cn/Article/details/gljmewysl.sHtML

[Q34] 每组取第一条
来源：http://m.share.fehbvm.com/Article/details/gdtlioyck.sHtML

SELECT * FROM (
来源：http://m.share.fehbvm.com/Article/details/gjbxofbxh.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mobile.zdbjq.cn/Article/details/gbydbexrk.sHtML

) t WHERE rn = 1;
来源：http://www.blog.hesvh.cn/Article/details/gvgazlxee.sHtML

[Q35] 内连接
来源：http://3g.zdbjq.cn/Article/details/gtbjcedhe.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://blog.zdbjq.cn/Article/details/gyibipqgo.sHtML

[Q36] 左连接
来源：http://m.share.hesvh.cn/Article/details/gqwrspeqa.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mobile.hesvh.cn/Article/details/gbrbktghl.sHtML

[Q37] 右连接
来源：http://m.share.hesvh.cn/Article/details/gsskeoskb.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.fehbvm.com/Article/details/gdafltswr.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://wap.fehbvm.com/Article/details/gueymupkm.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://3g.zdbjq.cn/Article/details/gfqzocviy.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.fehbvm.com/Article/details/gqcltopvx.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.fehbvm.com/Article/details/grjcvqddf.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mobile.fehbvm.com/Article/details/gpwxqwmaz.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.fehbvm.com/Article/details/geffjgywk.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://blog.zdbjq.cn/Article/details/gomkhagul.sHtML

[Q41] 多表连接
来源：http://www.share.zdbjq.cn/Article/details/glfrxijye.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.hesvh.cn/Article/details/gnfodqcez.sHtML

JOIN users u ON u.id = o.user_id
来源：http://mobile.fehbvm.com/Article/details/glnkafemm.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.zdbjq.cn/Article/details/gybhuqcob.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.hesvh.cn/Article/details/gbtdjyvgs.sHtML

SELECT u.name, o.amount FROM users u
来源：http://read.share.zdbjq.cn/Article/details/gxlfgmhzz.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.fehbvm.com/Article/details/gzvwluxsu.sHtML

[Q43] 标量子查询
来源：http://wap.fehbvm.com/Article/details/gklqlsnmc.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://3g.fehbvm.com/Article/details/gogcnrhsw.sHtML

[Q44] IN 子查询
来源：http://www.m.share.hesvh.cn/Article/details/gqwksbkdh.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://blog.hesvh.cn/Article/details/gxkwvuvbt.sHtML

[Q45] EXISTS 判断存在
来源：http://www.share.hesvh.cn/Article/details/gxinzqnqu.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.fehbvm.com/Article/details/gecdqlpad.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://m.share.zdbjq.cn/Article/details/gibifbaot.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.zdbjq.cn/Article/details/ghuoxcsve.sHtML

[Q47] 与平均值比较
来源：http://read.share.fehbvm.com/Article/details/gnnsoyuot.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.hesvh.cn/Article/details/greaeepax.sHtML

[Q48] CTE 公用表表达式
来源：http://www.share.zdbjq.cn/Article/details/gmjujthgj.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.m.share.fehbvm.com/Article/details/gbelzvzve.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.zdbjq.cn/Article/details/gzriatfom.sHtML

[Q49] 更新单行
来源：http://wap.fehbvm.com/Article/details/gqzqxmmcz.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.hesvh.cn/Article/details/grqveszwf.sHtML

[Q50] 批量更新
来源：http://www.blog.hesvh.cn/Article/details/gzplecjsu.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.fehbvm.com/Article/details/gusptdwtr.sHtML

[Q51] 用子查询更新
来源：http://www.share.hesvh.cn/Article/details/gwsmeqvkj.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.fehbvm.com/Article/details/guzrortrx.sHtML

[Q52] 删除指定行
来源：http://www.share.hesvh.cn/Article/details/gqdrpyuzi.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.hesvh.cn/Article/details/gnilmnxrm.sHtML

[Q53] 按条件删除
来源：http://m.share.zdbjq.cn/Article/details/givjinqkw.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.blog.hesvh.cn/Article/details/gdyggfkrn.sHtML

[Q54] 清空表
来源：http://wap.hesvh.cn/Article/details/gsdlrzhzt.sHtML

TRUNCATE TABLE logs;
来源：http://baike.fehbvm.com/Article/details/gvhvysjlj.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.fehbvm.com/Article/details/giuxafwjg.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.zdbjq.cn/Article/details/gyaqynifz.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.zdbjq.cn/Article/details/gvablrour.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.share.hesvh.cn/Article/details/gumkvtwmr.sHtML

[Q57] 行号
来源：http://baike.zdbjq.cn/Article/details/gyldbdshc.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gmvebwkax.sHtML

[Q58] 累计求和
来源：http://mobile.hesvh.cn/Article/details/grphvfwwz.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.fehbvm.com/Article/details/gfthjkwxc.sHtML

[Q59] 分组内累计
来源：http://blog.zdbjq.cn/Article/details/gdbjogdyy.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://3g.fehbvm.com/Article/details/gwfkijsas.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.zdbjq.cn/Article/details/gtgwhqrlq.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.zdbjq.cn/Article/details/gnfdroodz.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://blog.hesvh.cn/Article/details/gqgyljmyt.sHtML

[Q61] 移动平均
来源：http://read.share.fehbvm.com/Article/details/gndnnfejw.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/gkpaqmqlo.sHtML

[Q62] 分组占比
来源：http://baike.zdbjq.cn/Article/details/gdmujqnfg.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.hesvh.cn/Article/details/gntqxqrlk.sHtML

[Q63] 开启事务
来源：http://read.share.hesvh.cn/Article/details/gtebprmgv.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://3g.fehbvm.com/Article/details/gaictrfpi.sHtML

[Q64] 提交事务
来源：http://read.share.zdbjq.cn/Article/details/gtxdtaidz.sHtML

COMMIT;
来源：http://baike.fehbvm.com/Article/details/gripkqxht.sHtML

[Q65] 回滚事务
来源：http://read.share.zdbjq.cn/Article/details/gerefprbm.sHtML

ROLLBACK;
来源：http://m.share.zdbjq.cn/Article/details/gzlspciol.sHtML

[Q66] 行锁查询
来源：http://mobile.fehbvm.com/Article/details/gwprwwfka.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wap.hesvh.cn/Article/details/gkibwbkgo.sHtML

[Q67] 设置隔离级别
来源：http://read.share.hesvh.cn/Article/details/guojqvagl.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.hesvh.cn/Article/details/gympnmyzg.sHtML

[Q68] 保存点
来源：http://3g.fehbvm.com/Article/details/gqbpbbbus.sHtML

SAVEPOINT sp1;
来源：http://www.blog.fehbvm.com/Article/details/gmzfjxsbf.sHtML

ROLLBACK TO sp1;
来源：http://baike.zdbjq.cn/Article/details/gloidulxh.sHtML

[Q69] 查看执行计划
来源：http://m.share.hesvh.cn/Article/details/gkpjwpwsf.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.zdbjq.cn/Article/details/gcejyioay.sHtML

[Q70] 更新统计信息
来源：http://www.share.fehbvm.com/Article/details/gafpkfjbm.sHtML

ANALYZE TABLE users;
来源：http://read.share.hesvh.cn/Article/details/gimlbphpu.sHtML

[Q71] 查看建表语句
来源：http://baike.fehbvm.com/Article/details/gyjoeqsfu.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.hesvh.cn/Article/details/gurhbqgbb.sHtML

[Q72] 查看索引
来源：http://www.blog.zdbjq.cn/Article/details/giahvmorr.sHtML

SHOW INDEX FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gtqlfkokc.sHtML

[Q73] 查看表状态
来源：http://blog.fehbvm.com/Article/details/gugoqkuez.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.fehbvm.com/Article/details/gfkfpivxx.sHtML

[Q74] 强制使用索引
来源：http://baike.fehbvm.com/Article/details/gdrrynaid.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.hesvh.cn/Article/details/gbwnuaefj.sHtML

[Q75] 日期格式化
来源：http://read.share.fehbvm.com/Article/details/gxvftvxxk.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/gnrkdddcs.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.hesvh.cn/Article/details/godzlbnmj.sHtML

[Q76] 按天统计
来源：http://mobile.fehbvm.com/Article/details/gswxlvicm.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.hesvh.cn/Article/details/glduhysqy.sHtML

[Q77] 时间加减
来源：http://www.share.fehbvm.com/Article/details/gymbuomtm.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.hesvh.cn/Article/details/gjpglvpgc.sHtML

[Q78] 当前时间
来源：http://www.m.share.hesvh.cn/Article/details/gsceobcen.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.fehbvm.com/Article/details/gowbrbeqm.sHtML

[Q79] 字符串拼接
来源：http://3g.zdbjq.cn/Article/details/gaocueczp.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.hesvh.cn/Article/details/gveyxwqmh.sHtML

[Q80] 字符串截取
来源：http://read.share.fehbvm.com/Article/details/gogvpqfuw.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.zdbjq.cn/Article/details/gqfobnrtu.sHtML

[Q81] 字符串替换
来源：http://wap.fehbvm.com/Article/details/gpsodmywy.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.hesvh.cn/Article/details/gmzatpfqd.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.zdbjq.cn/Article/details/gshkygipx.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.hesvh.cn/Article/details/goonidaja.sHtML

[Q83] 大小写转换
来源：http://mobile.fehbvm.com/Article/details/gwptpdhvn.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gfvdvmhng.sHtML

[Q84] 去除首尾空格
来源：http://baike.fehbvm.com/Article/details/gmrliydwa.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.hesvh.cn/Article/details/gbuclxvro.sHtML

[Q85] 数值取整
来源：http://blog.hesvh.cn/Article/details/gnwubzkwa.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.hesvh.cn/Article/details/glamfcmnf.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.fehbvm.com/Article/details/grxzgfgwy.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.zdbjq.cn/Article/details/gfjnkzmla.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.hesvh.cn/Article/details/gvmntiicb.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.fehbvm.com/Article/details/gttzkdlro.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.zdbjq.cn/Article/details/geabjjbdm.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.zdbjq.cn/Article/details/gngfggboi.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://m.share.fehbvm.com/Article/details/gttoetmyc.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.hesvh.cn/Article/details/griquspel.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.fehbvm.com/Article/details/gtmjfijtm.sHtML

[Q90] 生成序号列
来源：http://read.share.fehbvm.com/Article/details/gwrqojtqh.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.hesvh.cn/Article/details/gtysawwmg.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/guryepvwj.sHtML

R. Bash 专题
来源：http://www.share.hesvh.cn/Article/details/gwcsjrfhr.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/glfpuyjay.sHtML

[R01] shebang 与严格模式
来源：http://mobile.zdbjq.cn/Article/details/gkuxkmkiq.sHtML

#!/usr/bin/env bash
来源：http://www.share.hesvh.cn/Article/details/gfmxrsclt.sHtML

set -euo pipefail
来源：http://www.m.share.zdbjq.cn/Article/details/gpvtxvopw.sHtML

[R02] 变量赋值与使用
来源：http://read.share.fehbvm.com/Article/details/gdeptsgqt.sHtML

name="Tom"; echo "$name"
来源：http://read.share.hesvh.cn/Article/details/gugherqqt.sHtML

[R03] 只读变量
来源：http://www.share.hesvh.cn/Article/details/gegratexg.sHtML

readonly PI=3.14
来源：http://mobile.fehbvm.com/Article/details/gwkdhpjqq.sHtML

[R04] 位置参数
来源：http://baike.hesvh.cn/Article/details/ginffezxj.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.fehbvm.com/Article/details/ghetxhoqn.sHtML

[R05] 参数默认值
来源：http://m.share.hesvh.cn/Article/details/gfghqjyyz.sHtML

name="${1:-default}"
来源：http://www.share.fehbvm.com/Article/details/gjunscqsm.sHtML

[R06] 判断命令是否存在
来源：http://mobile.fehbvm.com/Article/details/gzlpyfvjr.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.zdbjq.cn/Article/details/gtkbyefef.sHtML

[R07] if 判断文件
来源：http://www.blog.hesvh.cn/Article/details/gmqbzkoby.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.hesvh.cn/Article/details/gebjiyfsk.sHtML

[R08] 数值比较
来源：http://wap.hesvh.cn/Article/details/gbpoqoslk.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.zdbjq.cn/Article/details/ghiwyakpg.sHtML

[R09] 字符串比较
来源：http://wap.fehbvm.com/Article/details/gukqjmdui.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.hesvh.cn/Article/details/gkenjmtnl.sHtML

[R10] 正则匹配
来源：http://wap.fehbvm.com/Article/details/gcrzfirol.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.zdbjq.cn/Article/details/gtdxfcbzl.sHtML

[R11] case 多分支
来源：http://mobile.zdbjq.cn/Article/details/gxjcdgjhk.sHtML

case "$1" in
来源：http://www.share.zdbjq.cn/Article/details/gccfbojme.sHtML

start) echo "启动" ;;
来源：http://www.share.fehbvm.com/Article/details/gbatmfcpj.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.fehbvm.com/Article/details/gxyuokhnm.sHtML

*)     echo "未知命令" ;;
来源：http://baike.zdbjq.cn/Article/details/gjblgcobq.sHtML

esac
来源：http://3g.fehbvm.com/Article/details/gskrtelrm.sHtML

[R12] for 遍历文件
来源：http://blog.hesvh.cn/Article/details/gfakjiilm.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.zdbjq.cn/Article/details/gxoobgdum.sHtML

[R13] for 计数循环
来源：http://mobile.zdbjq.cn/Article/details/ggutoeemi.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.fehbvm.com/Article/details/gzspgpxpr.sHtML

[R14] C 风格 for
来源：http://www.m.share.fehbvm.com/Article/details/gyyrklgvi.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.zdbjq.cn/Article/details/gpmqlolna.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.hesvh.cn/Article/details/gvcwxlaqg.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.hesvh.cn/Article/details/gpomycytn.sHtML

[R16] until 等待条件
来源：http://m.share.zdbjq.cn/Article/details/gkuzohzko.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.zdbjq.cn/Article/details/geaidysjn.sHtML

[R17] 数组定义与取值
来源：http://m.share.hesvh.cn/Article/details/ghhorwqcb.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.hesvh.cn/Article/details/ghtbxsdco.sHtML

[R18] 遍历数组
来源：http://mobile.zdbjq.cn/Article/details/gmusegjso.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.zdbjq.cn/Article/details/gyvxhoqgn.sHtML

[R19] 数组长度
来源：http://read.share.hesvh.cn/Article/details/gznmulpij.sHtML

echo "${#arr[@]}"
来源：http://read.share.zdbjq.cn/Article/details/gyxhpaqus.sHtML

[R20] 关联数组（字典）
来源：http://baike.zdbjq.cn/Article/details/gqoftxrso.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.hesvh.cn/Article/details/gournnbie.sHtML

[R21] 字符串长度
来源：http://www.m.share.zdbjq.cn/Article/details/gwqadekci.sHtML

echo "${#s}"
来源：http://wap.hesvh.cn/Article/details/ghzbkawif.sHtML

[R22] 截取子串
来源：http://wap.zdbjq.cn/Article/details/gflpbhxur.sHtML

echo "${s:0:5}"
来源：http://mobile.fehbvm.com/Article/details/gjnfahibh.sHtML

[R23] 字符串替换
来源：http://baike.zdbjq.cn/Article/details/ghivofvty.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.fehbvm.com/Article/details/gyfmginpl.sHtML

[R24] 大小写转换
来源：http://mobile.zdbjq.cn/Article/details/gbtvjojqu.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.zdbjq.cn/Article/details/gdcgavilc.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.fehbvm.com/Article/details/glyapvoiu.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.hesvh.cn/Article/details/gfdwbcmuq.sHtML

[R26] 命令替换
来源：http://read.share.zdbjq.cn/Article/details/gsfuwmvyc.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.fehbvm.com/Article/details/gjmjndjym.sHtML

[R27] 算术展开
来源：http://baike.hesvh.cn/Article/details/gxjlfswvj.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.zdbjq.cn/Article/details/gofrxhiip.sHtML

[R28] 浮点运算
来源：http://mobile.fehbvm.com/Article/details/guhifngts.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.fehbvm.com/Article/details/gnhbolqii.sHtML

[R29] 定义函数
来源：http://m.share.hesvh.cn/Article/details/gpqmprdor.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.fehbvm.com/Article/details/gkekwnyra.sHtML

[R30] 函数返回状态码
来源：http://wap.zdbjq.cn/Article/details/gbfctjtbb.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.hesvh.cn/Article/details/gguhmwrxh.sHtML

[R31] 局部变量
来源：http://3g.fehbvm.com/Article/details/gmjueldoz.sHtML


<!-- 参考信息 -->