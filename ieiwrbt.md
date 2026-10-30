代发 wailian999

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.m.share.zdbjq.cn/Article/details/gqqitaezc.sHtML

TS:   if (x == null) {}
来源：http://m.share.fehbvm.com/Article/details/gvwowtydp.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://baike.zdbjq.cn/Article/details/gbbgpppwn.sHtML

Go:   if x == nil {}
来源：http://read.share.fehbvm.com/Article/details/gpknvdwjm.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.zdbjq.cn/Article/details/gqupflxzb.sHtML

C#:   if (x is null) {}
来源：http://www.blog.hesvh.cn/Article/details/gyeidpjqb.sHtML

[P07] 防抖与节流
来源：http://wap.hesvh.cn/Article/details/guvzfllwa.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://blog.hesvh.cn/Article/details/gotiqzjaa.sHtML

PHP:  // 手写时间戳比较
来源：http://read.share.fehbvm.com/Article/details/gfqophavq.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.hesvh.cn/Article/details/gxyebdwxx.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.zdbjq.cn/Article/details/gneuwlxqu.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://read.share.zdbjq.cn/Article/details/gombhrkpu.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://baike.zdbjq.cn/Article/details/gsfegazom.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://mobile.fehbvm.com/Article/details/gawklkhdl.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.share.fehbvm.com/Article/details/gissubdop.sHtML

[P08] 处理浮点精度问题
来源：http://read.share.hesvh.cn/Article/details/goguzaxls.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.m.share.hesvh.cn/Article/details/gyfhflbmp.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://3g.fehbvm.com/Article/details/gccwwdgym.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://read.share.zdbjq.cn/Article/details/gqyfvbtfv.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.share.hesvh.cn/Article/details/gbxjgdjeu.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.blog.hesvh.cn/Article/details/gbvlvnduu.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mobile.zdbjq.cn/Article/details/gerobgeyu.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://m.share.fehbvm.com/Article/details/ghfzowngk.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://m.share.zdbjq.cn/Article/details/grjbnbnfx.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gsfxrzpfh.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.share.zdbjq.cn/Article/details/gpjukjcki.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gqdmctyee.sHtML

[Q01] 创建表
来源：http://wap.fehbvm.com/Article/details/gvyatswiq.sHtML

CREATE TABLE users (
来源：http://3g.hesvh.cn/Article/details/gyswpyrzn.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.zdbjq.cn/Article/details/gpibsogrf.sHtML

name VARCHAR(50) NOT NULL,
来源：http://mobile.hesvh.cn/Article/details/gtxdvodxg.sHtML

email VARCHAR(100) UNIQUE,
来源：http://read.share.hesvh.cn/Article/details/gvqpccejl.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mobile.fehbvm.com/Article/details/gnqwxhhgw.sHtML

);
来源：http://m.share.zdbjq.cn/Article/details/gbkkucoye.sHtML

[Q02] 创建带外键的表
来源：http://wap.hesvh.cn/Article/details/gllirvlvk.sHtML

CREATE TABLE orders (
来源：http://m.share.fehbvm.com/Article/details/gswowemud.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.hesvh.cn/Article/details/gnojjfnnm.sHtML

user_id INT NOT NULL,
来源：http://mobile.zdbjq.cn/Article/details/gbajkldza.sHtML

amount DECIMAL(10, 2),
来源：http://3g.hesvh.cn/Article/details/gmjuiizgk.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://read.share.fehbvm.com/Article/details/gtsmkwhsa.sHtML

);
来源：http://m.share.fehbvm.com/Article/details/glczjagbu.sHtML

[Q03] 增加列
来源：http://read.share.fehbvm.com/Article/details/gccxweujk.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.m.share.hesvh.cn/Article/details/glycprlji.sHtML

[Q04] 修改列类型
来源：http://m.share.fehbvm.com/Article/details/gryxyqegc.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mobile.fehbvm.com/Article/details/gxicxldhu.sHtML

[Q05] 重命名列
来源：http://www.share.fehbvm.com/Article/details/gglaxrxtd.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wap.zdbjq.cn/Article/details/gwqjiqinr.sHtML

[Q06] 删除列
来源：http://blog.zdbjq.cn/Article/details/gbbdbeqtp.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.blog.zdbjq.cn/Article/details/gmpnyuhdo.sHtML

[Q07] 删除表
来源：http://www.m.share.hesvh.cn/Article/details/giegwxjds.sHtML

DROP TABLE IF EXISTS orders;
来源：http://m.share.zdbjq.cn/Article/details/gdcorbire.sHtML

[Q08] 创建普通索引
来源：http://www.share.fehbvm.com/Article/details/gtqhkiffb.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://read.share.zdbjq.cn/Article/details/gnrheiszu.sHtML

[Q09] 创建唯一索引
来源：http://blog.fehbvm.com/Article/details/gmjtqagii.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.m.share.fehbvm.com/Article/details/ghcsarnut.sHtML

[Q10] 插入单行
来源：http://www.blog.fehbvm.com/Article/details/gvmtqwbyc.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://baike.fehbvm.com/Article/details/gubuzmgjr.sHtML

[Q11] 一次插入多行
来源：http://baike.fehbvm.com/Article/details/gkvrqyjuv.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.fehbvm.com/Article/details/gejlxsggw.sHtML

[Q12] 插入后取自增 ID
来源：http://3g.zdbjq.cn/Article/details/gecpmhttg.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://blog.hesvh.cn/Article/details/glteraqxz.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mobile.hesvh.cn/Article/details/gwqmevigz.sHtML

[Q13] 忽略重复插入
来源：http://3g.hesvh.cn/Article/details/gvpmkyjef.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://blog.hesvh.cn/Article/details/gcousscie.sHtML

[Q14] 存在则更新（upsert）
来源：http://wap.zdbjq.cn/Article/details/guzqzrgtn.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://3g.fehbvm.com/Article/details/gefulmnyq.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://blog.zdbjq.cn/Article/details/glslpzjtf.sHtML

[Q15] 查询全部
来源：http://read.share.zdbjq.cn/Article/details/gtkgmcjey.sHtML

SELECT * FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gxdpzacne.sHtML

[Q16] 查询指定列
来源：http://www.share.hesvh.cn/Article/details/gflrbodkc.sHtML

SELECT id, name FROM users;
来源：http://read.share.fehbvm.com/Article/details/goqohcdxv.sHtML

[Q17] 条件查询
来源：http://blog.hesvh.cn/Article/details/gveqnsygy.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mobile.zdbjq.cn/Article/details/gytdbrxnf.sHtML

[Q18] 模糊匹配
来源：http://m.share.fehbvm.com/Article/details/godpupqvq.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mobile.hesvh.cn/Article/details/gqtsfgsjw.sHtML

[Q19] 范围查询
来源：http://mobile.zdbjq.cn/Article/details/geunxuewh.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.share.zdbjq.cn/Article/details/gqhhekmnr.sHtML

[Q20] IN 列表
来源：http://www.share.hesvh.cn/Article/details/gwdugtneo.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.hesvh.cn/Article/details/ganlahfbl.sHtML

[Q21] 空值判断
来源：http://wap.zdbjq.cn/Article/details/goyegwrrt.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://m.share.zdbjq.cn/Article/details/gihlyakef.sHtML

[Q22] 排序
来源：http://mobile.hesvh.cn/Article/details/gxidavxun.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mobile.hesvh.cn/Article/details/gqnwluaxb.sHtML

[Q23] 分页
来源：http://baike.hesvh.cn/Article/details/grogdgoxw.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://3g.hesvh.cn/Article/details/ghsuvifop.sHtML

[Q24] 去重
来源：http://read.share.zdbjq.cn/Article/details/gnmopguor.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/ggmchwsde.sHtML

[Q25] 只取前 N 条
来源：http://www.m.share.zdbjq.cn/Article/details/gumnzqcsq.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mobile.zdbjq.cn/Article/details/gldqrpcxq.sHtML

[Q26] 计数
来源：http://m.share.fehbvm.com/Article/details/gboalgurj.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gxzrubfqd.sHtML

[Q27] 条件计数
来源：http://blog.zdbjq.cn/Article/details/grgebnxrx.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gxrcctuhk.sHtML

[Q28] 求和与平均
来源：http://blog.hesvh.cn/Article/details/gfplcrdpd.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/gbeqeusei.sHtML

[Q29] 最大最小值
来源：http://read.share.zdbjq.cn/Article/details/ggyypabda.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://baike.hesvh.cn/Article/details/gditmoueh.sHtML

[Q30] 分组统计
来源：http://www.m.share.fehbvm.com/Article/details/gansfdlpf.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://baike.hesvh.cn/Article/details/giykypxuf.sHtML

[Q31] 分组后过滤
来源：http://www.m.share.hesvh.cn/Article/details/gpjnksudz.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://read.share.hesvh.cn/Article/details/gxxlnxvab.sHtML

[Q32] 分组拼接字符串
来源：http://3g.zdbjq.cn/Article/details/giogxxspt.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wap.hesvh.cn/Article/details/gvjpiikjg.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.hesvh.cn/Article/details/gmiiiuzhz.sHtML

[Q33] 多列分组
来源：http://www.m.share.zdbjq.cn/Article/details/gmllivgyc.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://3g.zdbjq.cn/Article/details/glxdrbemo.sHtML

[Q34] 每组取第一条
来源：http://mobile.zdbjq.cn/Article/details/gkpcotjqc.sHtML

SELECT * FROM (
来源：http://baike.fehbvm.com/Article/details/gfumsrzwb.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://m.share.hesvh.cn/Article/details/gswqoxleq.sHtML

) t WHERE rn = 1;
来源：http://mobile.zdbjq.cn/Article/details/gajjtrpct.sHtML

[Q35] 内连接
来源：http://blog.fehbvm.com/Article/details/gldenuqtf.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.fehbvm.com/Article/details/gqaoztauw.sHtML

[Q36] 左连接
来源：http://mobile.hesvh.cn/Article/details/gsoxsiqsn.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://m.share.fehbvm.com/Article/details/gjakqpfft.sHtML

[Q37] 右连接
来源：http://read.share.fehbvm.com/Article/details/gzhbwhlma.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://blog.hesvh.cn/Article/details/ggadhlqvy.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.share.hesvh.cn/Article/details/gsbypadep.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://3g.fehbvm.com/Article/details/gtddffcod.sHtML

[Q39] 自连接（查上下级）
来源：http://www.blog.zdbjq.cn/Article/details/ggeqbeatq.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://read.share.zdbjq.cn/Article/details/gqajxpwbi.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.zdbjq.cn/Article/details/gtqpeucpk.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://baike.zdbjq.cn/Article/details/gnxyprqkb.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://blog.zdbjq.cn/Article/details/gykbpfwbt.sHtML

[Q41] 多表连接
来源：http://www.share.zdbjq.cn/Article/details/gnsantlcv.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.blog.zdbjq.cn/Article/details/gtucqanrm.sHtML

JOIN users u ON u.id = o.user_id
来源：http://read.share.zdbjq.cn/Article/details/ghtafxhki.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.share.hesvh.cn/Article/details/gmllnsunl.sHtML

[Q42] 连接条件附加过滤
来源：http://baike.fehbvm.com/Article/details/gppfogpta.sHtML

SELECT u.name, o.amount FROM users u
来源：http://read.share.hesvh.cn/Article/details/goxikelgq.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.zdbjq.cn/Article/details/goyrmkenq.sHtML

[Q43] 标量子查询
来源：http://www.share.zdbjq.cn/Article/details/gwsnmweuf.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.blog.zdbjq.cn/Article/details/ghkuferey.sHtML

[Q44] IN 子查询
来源：http://mobile.hesvh.cn/Article/details/ghzlnyjax.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://baike.hesvh.cn/Article/details/gejuunayw.sHtML

[Q45] EXISTS 判断存在
来源：http://blog.fehbvm.com/Article/details/gmanpmqbp.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.fehbvm.com/Article/details/glzoutsqg.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.zdbjq.cn/Article/details/gdelletej.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.zdbjq.cn/Article/details/gmtuopvii.sHtML

[Q47] 与平均值比较
来源：http://baike.hesvh.cn/Article/details/gxwfsbfub.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.zdbjq.cn/Article/details/garrtpgwc.sHtML

[Q48] CTE 公用表表达式
来源：http://3g.zdbjq.cn/Article/details/ghcdrbkvk.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.fehbvm.com/Article/details/gibqnbfcg.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://wap.fehbvm.com/Article/details/gtbyuimfa.sHtML

[Q49] 更新单行
来源：http://www.m.share.zdbjq.cn/Article/details/gwtyvzjdd.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://m.share.zdbjq.cn/Article/details/golwtikjs.sHtML

[Q50] 批量更新
来源：http://www.blog.hesvh.cn/Article/details/ghpmndjgm.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.m.share.fehbvm.com/Article/details/ggycdymxe.sHtML

[Q51] 用子查询更新
来源：http://mobile.fehbvm.com/Article/details/gtyraqzha.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://baike.fehbvm.com/Article/details/goghonnhc.sHtML

[Q52] 删除指定行
来源：http://read.share.fehbvm.com/Article/details/gvsnojufh.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.m.share.zdbjq.cn/Article/details/gbccsmnat.sHtML

[Q53] 按条件删除
来源：http://m.share.hesvh.cn/Article/details/gcucxmpiy.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.hesvh.cn/Article/details/gdsyffsta.sHtML

[Q54] 清空表
来源：http://m.share.zdbjq.cn/Article/details/gulfbphhu.sHtML

TRUNCATE TABLE logs;
来源：http://3g.zdbjq.cn/Article/details/glqurlwbl.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.hesvh.cn/Article/details/gevopcxwc.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.fehbvm.com/Article/details/gialqelzn.sHtML

[Q56] 密集排名（并列不占位）
来源：http://blog.zdbjq.cn/Article/details/gzhfcdezo.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://read.share.hesvh.cn/Article/details/gaxonifrl.sHtML

[Q57] 行号
来源：http://baike.zdbjq.cn/Article/details/gtougafly.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.zdbjq.cn/Article/details/gtqtlcqwm.sHtML

[Q58] 累计求和
来源：http://mobile.hesvh.cn/Article/details/grlxpggfs.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mobile.hesvh.cn/Article/details/gyfvdldfi.sHtML

[Q59] 分组内累计
来源：http://wap.fehbvm.com/Article/details/ghqdgsjkw.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.hesvh.cn/Article/details/gdqyxlggb.sHtML

[Q60] 取上一行 / 下一行
来源：http://baike.fehbvm.com/Article/details/grpxjxtyy.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wap.fehbvm.com/Article/details/gqifhulse.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.zdbjq.cn/Article/details/gjwjmjmta.sHtML

[Q61] 移动平均
来源：http://mobile.fehbvm.com/Article/details/gnngqmdcv.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/gxaqphlal.sHtML

[Q62] 分组占比
来源：http://wap.zdbjq.cn/Article/details/gevoijhby.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.hesvh.cn/Article/details/gdgyvniyp.sHtML

[Q63] 开启事务
来源：http://baike.hesvh.cn/Article/details/geiqqvmho.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://blog.fehbvm.com/Article/details/gcbealfli.sHtML

[Q64] 提交事务
来源：http://baike.fehbvm.com/Article/details/gjisxsojg.sHtML

COMMIT;
来源：http://read.share.fehbvm.com/Article/details/gpolowidx.sHtML

[Q65] 回滚事务
来源：http://baike.zdbjq.cn/Article/details/ggwowdoyj.sHtML

ROLLBACK;
来源：http://baike.hesvh.cn/Article/details/grwdeosrz.sHtML

[Q66] 行锁查询
来源：http://www.blog.hesvh.cn/Article/details/gjugexgcy.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mobile.zdbjq.cn/Article/details/gufhxlgsp.sHtML

[Q67] 设置隔离级别
来源：http://3g.fehbvm.com/Article/details/gmyprsbrx.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.hesvh.cn/Article/details/givdvfxie.sHtML

[Q68] 保存点
来源：http://www.share.fehbvm.com/Article/details/gtgpazalz.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.zdbjq.cn/Article/details/gdajltktg.sHtML

ROLLBACK TO sp1;
来源：http://www.share.hesvh.cn/Article/details/gcqplotqz.sHtML

[Q69] 查看执行计划
来源：http://m.share.zdbjq.cn/Article/details/gdjeskwmi.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.fehbvm.com/Article/details/gwftscoje.sHtML

[Q70] 更新统计信息
来源：http://read.share.hesvh.cn/Article/details/glhlhnamu.sHtML

ANALYZE TABLE users;
来源：http://read.share.fehbvm.com/Article/details/gkhlreior.sHtML

[Q71] 查看建表语句
来源：http://3g.zdbjq.cn/Article/details/gricnbpvn.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.zdbjq.cn/Article/details/giwkdjnri.sHtML

[Q72] 查看索引
来源：http://3g.hesvh.cn/Article/details/gqktvdenj.sHtML

SHOW INDEX FROM users;
来源：http://mobile.fehbvm.com/Article/details/gdktumrjh.sHtML

[Q73] 查看表状态
来源：http://www.m.share.zdbjq.cn/Article/details/gxziaphhz.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://wap.hesvh.cn/Article/details/gishsdzvz.sHtML

[Q74] 强制使用索引
来源：http://mobile.fehbvm.com/Article/details/ghkieedcv.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://m.share.hesvh.cn/Article/details/ggpigyjdf.sHtML

[Q75] 日期格式化
来源：http://www.blog.hesvh.cn/Article/details/gjuvlytde.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.hesvh.cn/Article/details/gcwfzqiaj.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.hesvh.cn/Article/details/gtfvkbgyz.sHtML

[Q76] 按天统计
来源：http://3g.zdbjq.cn/Article/details/gabkhhvll.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.hesvh.cn/Article/details/ghbryewis.sHtML

[Q77] 时间加减
来源：http://read.share.fehbvm.com/Article/details/gfjeophgn.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.zdbjq.cn/Article/details/genbewtwg.sHtML

[Q78] 当前时间
来源：http://m.share.zdbjq.cn/Article/details/gycbuyfsq.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.fehbvm.com/Article/details/golmqrjsr.sHtML

[Q79] 字符串拼接
来源：http://www.share.fehbvm.com/Article/details/gmpestnpo.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.fehbvm.com/Article/details/gwnozmljb.sHtML

[Q80] 字符串截取
来源：http://baike.zdbjq.cn/Article/details/gmoxejeuo.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mobile.fehbvm.com/Article/details/gdhajiuai.sHtML

[Q81] 字符串替换
来源：http://www.blog.fehbvm.com/Article/details/goueuqmsz.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.fehbvm.com/Article/details/gmjuqdgcz.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.zdbjq.cn/Article/details/grzdnmsym.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gajmfdqpv.sHtML

[Q83] 大小写转换
来源：http://mobile.fehbvm.com/Article/details/gtwchbobx.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.hesvh.cn/Article/details/ggduxpdyr.sHtML

[Q84] 去除首尾空格
来源：http://m.share.zdbjq.cn/Article/details/gecchdxtj.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gulsglxnk.sHtML

[Q85] 数值取整
来源：http://www.share.zdbjq.cn/Article/details/gkdukafdc.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.hesvh.cn/Article/details/gnppiysge.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.hesvh.cn/Article/details/goyjzkrsy.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.zdbjq.cn/Article/details/gyureugrh.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.fehbvm.com/Article/details/gursbxvwh.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.zdbjq.cn/Article/details/gvqvtfsuq.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.hesvh.cn/Article/details/gtlqllyds.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.zdbjq.cn/Article/details/gtzetagjv.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.fehbvm.com/Article/details/gerkxtjvy.sHtML

[Q89] 判断表是否存在
来源：http://blog.zdbjq.cn/Article/details/gndodfuou.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.hesvh.cn/Article/details/gsfjlewqr.sHtML

[Q90] 生成序号列
来源：http://baike.fehbvm.com/Article/details/gynkectid.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.hesvh.cn/Article/details/glyuwwcdw.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gqvkmokug.sHtML

R. Bash 专题
来源：http://baike.hesvh.cn/Article/details/gwbqearnh.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gvvlezvhd.sHtML

[R01] shebang 与严格模式
来源：http://read.share.fehbvm.com/Article/details/gavqjulmm.sHtML

#!/usr/bin/env bash
来源：http://www.share.zdbjq.cn/Article/details/gptltyelf.sHtML

set -euo pipefail
来源：http://wap.zdbjq.cn/Article/details/gtwofymwm.sHtML

[R02] 变量赋值与使用
来源：http://blog.zdbjq.cn/Article/details/gjzlvkgys.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.hesvh.cn/Article/details/gjkrgzuhw.sHtML

[R03] 只读变量
来源：http://blog.fehbvm.com/Article/details/gnjouxtpf.sHtML

readonly PI=3.14
来源：http://baike.zdbjq.cn/Article/details/gezrrrctb.sHtML

[R04] 位置参数
来源：http://blog.hesvh.cn/Article/details/gghesstgx.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.fehbvm.com/Article/details/gizjngenl.sHtML

[R05] 参数默认值
来源：http://www.m.share.zdbjq.cn/Article/details/gjaflqvpe.sHtML

name="${1:-default}"
来源：http://mobile.zdbjq.cn/Article/details/gfzeuaaok.sHtML

[R06] 判断命令是否存在
来源：http://blog.zdbjq.cn/Article/details/gidryldpo.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.fehbvm.com/Article/details/ggcvnlxjq.sHtML

[R07] if 判断文件
来源：http://mobile.fehbvm.com/Article/details/gbitpcqsh.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.zdbjq.cn/Article/details/gkmimhnfr.sHtML

[R08] 数值比较
来源：http://blog.zdbjq.cn/Article/details/grrcmfnaf.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.zdbjq.cn/Article/details/gheyfprda.sHtML

[R09] 字符串比较
来源：http://m.share.hesvh.cn/Article/details/ghhlgzlrc.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.hesvh.cn/Article/details/gbvpksszy.sHtML

[R10] 正则匹配
来源：http://read.share.hesvh.cn/Article/details/gmzxspzdk.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.zdbjq.cn/Article/details/gigtxmchq.sHtML

[R11] case 多分支
来源：http://m.share.zdbjq.cn/Article/details/gokrymaeg.sHtML

case "$1" in
来源：http://mobile.fehbvm.com/Article/details/gnzecpvxz.sHtML

start) echo "启动" ;;
来源：http://m.share.zdbjq.cn/Article/details/gqzuvhkfo.sHtML

stop)  echo "停止" ;;
来源：http://read.share.hesvh.cn/Article/details/goenhhbhs.sHtML

*)     echo "未知命令" ;;
来源：http://3g.zdbjq.cn/Article/details/goxqkvaeu.sHtML

esac
来源：http://www.share.fehbvm.com/Article/details/gbpqpoeat.sHtML

[R12] for 遍历文件
来源：http://m.share.zdbjq.cn/Article/details/grlvxwoly.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.zdbjq.cn/Article/details/grrmifgox.sHtML

[R13] for 计数循环
来源：http://www.share.zdbjq.cn/Article/details/gjzumxxur.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.zdbjq.cn/Article/details/grcxkmolc.sHtML

[R14] C 风格 for
来源：http://m.share.hesvh.cn/Article/details/gqkphcfae.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.hesvh.cn/Article/details/gezozcrsi.sHtML

[R15] while 逐行读文件
来源：http://wap.hesvh.cn/Article/details/gxkbzgidn.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.zdbjq.cn/Article/details/ghmpuygrc.sHtML

[R16] until 等待条件
来源：http://www.share.fehbvm.com/Article/details/gwfzhftdj.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.fehbvm.com/Article/details/grdowrvwv.sHtML

[R17] 数组定义与取值
来源：http://blog.zdbjq.cn/Article/details/gqlxhvlbm.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.zdbjq.cn/Article/details/gxyajajxr.sHtML

[R18] 遍历数组
来源：http://wap.zdbjq.cn/Article/details/gudderygy.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.zdbjq.cn/Article/details/gxscaqkcq.sHtML

[R19] 数组长度
来源：http://blog.hesvh.cn/Article/details/gyxrmrajv.sHtML

echo "${#arr[@]}"
来源：http://mobile.zdbjq.cn/Article/details/gripwtxyp.sHtML

[R20] 关联数组（字典）
来源：http://read.share.zdbjq.cn/Article/details/gmtgdevxa.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.zdbjq.cn/Article/details/goqpifavz.sHtML

[R21] 字符串长度
来源：http://www.share.zdbjq.cn/Article/details/gkljoyatm.sHtML

echo "${#s}"
来源：http://mobile.zdbjq.cn/Article/details/gkzmveufv.sHtML

[R22] 截取子串
来源：http://www.share.zdbjq.cn/Article/details/gdcdwlcdl.sHtML

echo "${s:0:5}"
来源：http://www.blog.zdbjq.cn/Article/details/gjklttqni.sHtML

[R23] 字符串替换
来源：http://www.m.share.fehbvm.com/Article/details/gvbrmcxpv.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.hesvh.cn/Article/details/gseqwefsk.sHtML

[R24] 大小写转换
来源：http://wap.zdbjq.cn/Article/details/gkxgbkycp.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.fehbvm.com/Article/details/geqpizdov.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.hesvh.cn/Article/details/gkmphwsjp.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.hesvh.cn/Article/details/gixqvwfro.sHtML

[R26] 命令替换
来源：http://m.share.fehbvm.com/Article/details/gfmiyachs.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.zdbjq.cn/Article/details/gmthaevor.sHtML

[R27] 算术展开
来源：http://read.share.zdbjq.cn/Article/details/gzntfcasu.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.fehbvm.com/Article/details/gfuinxtam.sHtML

[R28] 浮点运算
来源：http://www.m.share.hesvh.cn/Article/details/gfrjfoold.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.hesvh.cn/Article/details/gbpjakrxm.sHtML

[R29] 定义函数
来源：http://3g.hesvh.cn/Article/details/ghbppvnlm.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.fehbvm.com/Article/details/guzhhvueb.sHtML

[R30] 函数返回状态码
来源：http://www.blog.fehbvm.com/Article/details/glamokfei.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.zdbjq.cn/Article/details/goydspvok.sHtML

[R31] 局部变量
来源：http://www.blog.fehbvm.com/Article/details/ghqzedbea.sHtML


<!-- 参考信息 -->