代发 wailian999

PHP:  // 手写时间戳比较
来源：http://mobile.fanxiaobao.xyz/Article/details/graubnasj.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.fanxiaobao.xyz/Article/details/gvxpnomtg.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.fanxiaobao.xyz/Article/details/gysokgdrx.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gzxrhcgtu.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.share.fanxiaobao.xyz/Article/details/gkigyirmy.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://wap.fanxiaobao.xyz/Article/details/gxcsaqwsb.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://blog.fanxiaobao.xyz/Article/details/gfkgdmtvr.sHtML

[P08] 处理浮点精度问题
来源：http://blog.fanxiaobao.xyz/Article/details/govmqqryo.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.share.fanxiaobao.xyz/Article/details/gxsruyblm.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://baike.fanxiaobao.xyz/Article/details/gpjwqmzwx.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://blog.fanxiaobao.xyz/Article/details/gvponqped.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gnyksbnbu.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://3g.fanxiaobao.xyz/Article/details/gpzxgkvci.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://m.share.fanxiaobao.xyz/Article/details/gutvoeuhz.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.share.fanxiaobao.xyz/Article/details/gxegbunoh.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.blog.fanxiaobao.xyz/Article/details/gumkuiysm.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gapdyafup.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkjizttil.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gyhhjdxjq.sHtML

[Q01] 创建表
来源：http://read.share.fanxiaobao.xyz/Article/details/gmmhgmvxw.sHtML

CREATE TABLE users (
来源：http://m.share.fanxiaobao.xyz/Article/details/gitgrjdxj.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.fanxiaobao.xyz/Article/details/gugdytcdp.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goqlkfsbe.sHtML

email VARCHAR(100) UNIQUE,
来源：http://baike.fanxiaobao.xyz/Article/details/gkujtlzwk.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfhozslig.sHtML

);
来源：http://mobile.fanxiaobao.xyz/Article/details/gcbhfvldl.sHtML

[Q02] 创建带外键的表
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdyhwuavc.sHtML

CREATE TABLE orders (
来源：http://mobile.fanxiaobao.xyz/Article/details/gicckzlcr.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.fanxiaobao.xyz/Article/details/gqxeisjqp.sHtML

user_id INT NOT NULL,
来源：http://read.share.fanxiaobao.xyz/Article/details/grhyhjulq.sHtML

amount DECIMAL(10, 2),
来源：http://3g.fanxiaobao.xyz/Article/details/gwsqbgold.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.share.fanxiaobao.xyz/Article/details/grmouxfld.sHtML

);
来源：http://mobile.fanxiaobao.xyz/Article/details/gvqqdswwc.sHtML

[Q03] 增加列
来源：http://wap.fanxiaobao.xyz/Article/details/gnonwsyuk.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mobile.fanxiaobao.xyz/Article/details/guejilfrg.sHtML

[Q04] 修改列类型
来源：http://www.share.fanxiaobao.xyz/Article/details/gdbpdgydu.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://baike.fanxiaobao.xyz/Article/details/glqejrdtp.sHtML

[Q05] 重命名列
来源：http://blog.fanxiaobao.xyz/Article/details/gqyhanmzt.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://baike.fanxiaobao.xyz/Article/details/getfzhgyc.sHtML

[Q06] 删除列
来源：http://blog.fanxiaobao.xyz/Article/details/gcojsoirl.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.share.fanxiaobao.xyz/Article/details/gxpnhwqmi.sHtML

[Q07] 删除表
来源：http://blog.fanxiaobao.xyz/Article/details/ggqugjplp.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.share.fanxiaobao.xyz/Article/details/gicdycoty.sHtML

[Q08] 创建普通索引
来源：http://wap.fanxiaobao.xyz/Article/details/gstzytpiy.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghgejxxdy.sHtML

[Q09] 创建唯一索引
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grwnbvkfw.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.share.fanxiaobao.xyz/Article/details/gqujykqef.sHtML

[Q10] 插入单行
来源：http://mobile.fanxiaobao.xyz/Article/details/gxmclmdce.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://read.share.fanxiaobao.xyz/Article/details/gmzagrzjo.sHtML

[Q11] 一次插入多行
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpsciqict.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mobile.fanxiaobao.xyz/Article/details/gtbxvspdc.sHtML

[Q12] 插入后取自增 ID
来源：http://wap.fanxiaobao.xyz/Article/details/gppgoqcku.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://3g.fanxiaobao.xyz/Article/details/gugrqutnc.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://baike.fanxiaobao.xyz/Article/details/gqqyrivvz.sHtML

[Q13] 忽略重复插入
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfdjxquxi.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://read.share.fanxiaobao.xyz/Article/details/gpuwigphi.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyivnfoxk.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.share.fanxiaobao.xyz/Article/details/gamaptszm.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://m.share.fanxiaobao.xyz/Article/details/gcwcrlmyi.sHtML

[Q15] 查询全部
来源：http://wap.fanxiaobao.xyz/Article/details/grxggjnmo.sHtML

SELECT * FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gdoizspft.sHtML

[Q16] 查询指定列
来源：http://mobile.fanxiaobao.xyz/Article/details/gqziaazev.sHtML

SELECT id, name FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gvjokbqym.sHtML

[Q17] 条件查询
来源：http://www.share.fanxiaobao.xyz/Article/details/gmgnxbgfv.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gxjynwyhi.sHtML

[Q18] 模糊匹配
来源：http://www.share.fanxiaobao.xyz/Article/details/ggidclvwh.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wap.fanxiaobao.xyz/Article/details/gpplyuqcx.sHtML

[Q19] 范围查询
来源：http://read.share.fanxiaobao.xyz/Article/details/gadtexfzr.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://baike.fanxiaobao.xyz/Article/details/gpbemwngg.sHtML

[Q20] IN 列表
来源：http://read.share.fanxiaobao.xyz/Article/details/gqdcxrnid.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://m.share.fanxiaobao.xyz/Article/details/gbervjtdg.sHtML

[Q21] 空值判断
来源：http://wap.fanxiaobao.xyz/Article/details/grrrbyeet.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://m.share.fanxiaobao.xyz/Article/details/gohnpfruj.sHtML

[Q22] 排序
来源：http://3g.fanxiaobao.xyz/Article/details/gcrrympex.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://blog.fanxiaobao.xyz/Article/details/gifdttsgi.sHtML

[Q23] 分页
来源：http://3g.fanxiaobao.xyz/Article/details/gvulmasrt.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://3g.fanxiaobao.xyz/Article/details/gvqggevxh.sHtML

[Q24] 去重
来源：http://3g.fanxiaobao.xyz/Article/details/gdxdwcubt.sHtML

SELECT DISTINCT city FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gtgiobvnt.sHtML

[Q25] 只取前 N 条
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxytsibit.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mobile.fanxiaobao.xyz/Article/details/gnzewiaqz.sHtML

[Q26] 计数
来源：http://m.share.fanxiaobao.xyz/Article/details/gmuzuwvlc.sHtML

SELECT COUNT(*) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/giiephgbn.sHtML

[Q27] 条件计数
来源：http://wap.fanxiaobao.xyz/Article/details/gvbncwwoh.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/glwoqqjpo.sHtML

[Q28] 求和与平均
来源：http://mobile.fanxiaobao.xyz/Article/details/gludkdfca.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wap.fanxiaobao.xyz/Article/details/gyytmqpcv.sHtML

[Q29] 最大最小值
来源：http://wap.fanxiaobao.xyz/Article/details/gloahvunc.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gsokgyagu.sHtML

[Q30] 分组统计
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gocclddsb.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.fanxiaobao.xyz/Article/details/gmzubpppm.sHtML

[Q31] 分组后过滤
来源：http://wap.fanxiaobao.xyz/Article/details/gwbxkiwsb.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gagwxiysa.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqesucduj.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwxbamlwr.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wap.fanxiaobao.xyz/Article/details/gghpzqajk.sHtML

[Q33] 多列分组
来源：http://m.share.fanxiaobao.xyz/Article/details/giitfkwqa.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.fanxiaobao.xyz/Article/details/gycycluxm.sHtML

[Q34] 每组取第一条
来源：http://baike.fanxiaobao.xyz/Article/details/gyzynnblq.sHtML

SELECT * FROM (
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjhfrvkys.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://baike.fanxiaobao.xyz/Article/details/ghghbxjmu.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/garlljkpg.sHtML

[Q35] 内连接
来源：http://mobile.fanxiaobao.xyz/Article/details/ggbvllrev.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.fanxiaobao.xyz/Article/details/geeugodbm.sHtML

[Q36] 左连接
来源：http://3g.fanxiaobao.xyz/Article/details/ggrtrzfcj.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.fanxiaobao.xyz/Article/details/gzrujirhm.sHtML

[Q37] 右连接
来源：http://m.share.fanxiaobao.xyz/Article/details/gkwtzchkw.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wap.fanxiaobao.xyz/Article/details/ghpkkrpfh.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.fanxiaobao.xyz/Article/details/gxulexqzs.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.fanxiaobao.xyz/Article/details/gcchfyogc.sHtML

[Q39] 自连接（查上下级）
来源：http://wap.fanxiaobao.xyz/Article/details/gacliqhuh.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfhufyvul.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtobfslld.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.fanxiaobao.xyz/Article/details/gboqiubkn.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wap.fanxiaobao.xyz/Article/details/gjdcgbzfg.sHtML

[Q41] 多表连接
来源：http://read.share.fanxiaobao.xyz/Article/details/godhpiinm.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.share.fanxiaobao.xyz/Article/details/gwzgiegqi.sHtML

JOIN users u ON u.id = o.user_id
来源：http://read.share.fanxiaobao.xyz/Article/details/ghokdmfur.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://blog.fanxiaobao.xyz/Article/details/gperzewyj.sHtML

[Q42] 连接条件附加过滤
来源：http://read.share.fanxiaobao.xyz/Article/details/gtuwxaplw.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.fanxiaobao.xyz/Article/details/grzixfgxu.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wap.fanxiaobao.xyz/Article/details/gtnrlaroo.sHtML

[Q43] 标量子查询
来源：http://3g.fanxiaobao.xyz/Article/details/ggxxzouta.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.fanxiaobao.xyz/Article/details/ggrjtlaye.sHtML

[Q44] IN 子查询
来源：http://wap.fanxiaobao.xyz/Article/details/gswkqoarn.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://baike.fanxiaobao.xyz/Article/details/gfeifytrj.sHtML

[Q45] EXISTS 判断存在
来源：http://3g.fanxiaobao.xyz/Article/details/gseshacjp.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.fanxiaobao.xyz/Article/details/gpwdayist.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.fanxiaobao.xyz/Article/details/gwtakollr.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdiufopci.sHtML

[Q47] 与平均值比较
来源：http://baike.fanxiaobao.xyz/Article/details/ggoglwhov.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.fanxiaobao.xyz/Article/details/guliybnod.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.fanxiaobao.xyz/Article/details/gkxhphvjc.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://m.share.fanxiaobao.xyz/Article/details/gotveczen.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://mobile.fanxiaobao.xyz/Article/details/gbydjtegm.sHtML

[Q49] 更新单行
来源：http://wap.fanxiaobao.xyz/Article/details/gyefmqyki.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkzyvifbb.sHtML

[Q50] 批量更新
来源：http://wap.fanxiaobao.xyz/Article/details/gfecbndhw.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://m.share.fanxiaobao.xyz/Article/details/gmabqomdl.sHtML

[Q51] 用子查询更新
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvvdjjoby.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gsjvlcgdi.sHtML

[Q52] 删除指定行
来源：http://3g.fanxiaobao.xyz/Article/details/ganalowcj.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.fanxiaobao.xyz/Article/details/goveawdic.sHtML

[Q53] 按条件删除
来源：http://wap.fanxiaobao.xyz/Article/details/gvlcfmiad.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.fanxiaobao.xyz/Article/details/gasuizgyu.sHtML

[Q54] 清空表
来源：http://baike.fanxiaobao.xyz/Article/details/gkxaskbeg.sHtML

TRUNCATE TABLE logs;
来源：http://mobile.fanxiaobao.xyz/Article/details/gnuijcqag.sHtML

[Q55] 排名（并列占位）
来源：http://www.share.fanxiaobao.xyz/Article/details/guevmclxr.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mobile.fanxiaobao.xyz/Article/details/gwmngputh.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.fanxiaobao.xyz/Article/details/gskufslzf.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://baike.fanxiaobao.xyz/Article/details/grxcnjcjq.sHtML

[Q57] 行号
来源：http://www.share.fanxiaobao.xyz/Article/details/gzcoupgcl.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzdhzhrlh.sHtML

[Q58] 累计求和
来源：http://baike.fanxiaobao.xyz/Article/details/gbtpgvtnb.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnpsfegcr.sHtML

[Q59] 分组内累计
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggfkwxlpl.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.fanxiaobao.xyz/Article/details/gigilcyfq.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxyiiphtg.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.fanxiaobao.xyz/Article/details/gktcoswhs.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/gjkpfmrqj.sHtML

[Q61] 移动平均
来源：http://www.share.fanxiaobao.xyz/Article/details/gzunkfdvh.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.share.fanxiaobao.xyz/Article/details/gxhapgsuz.sHtML

[Q62] 分组占比
来源：http://www.share.fanxiaobao.xyz/Article/details/gzozlongj.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.fanxiaobao.xyz/Article/details/gysexdhzk.sHtML

[Q63] 开启事务
来源：http://wap.fanxiaobao.xyz/Article/details/gqtfqxyfp.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.share.fanxiaobao.xyz/Article/details/gdvvozayh.sHtML

[Q64] 提交事务
来源：http://read.share.fanxiaobao.xyz/Article/details/goqoypfyp.sHtML

COMMIT;
来源：http://3g.fanxiaobao.xyz/Article/details/gbxrdjmkx.sHtML

[Q65] 回滚事务
来源：http://m.share.fanxiaobao.xyz/Article/details/guqpouako.sHtML

ROLLBACK;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvxsbwdbd.sHtML

[Q66] 行锁查询
来源：http://m.share.fanxiaobao.xyz/Article/details/gfrqwtzui.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.fanxiaobao.xyz/Article/details/gotxghzdm.sHtML

[Q67] 设置隔离级别
来源：http://3g.fanxiaobao.xyz/Article/details/gdhahkdra.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://3g.fanxiaobao.xyz/Article/details/gcjhkxrsc.sHtML

[Q68] 保存点
来源：http://m.share.fanxiaobao.xyz/Article/details/gznbyptdl.sHtML

SAVEPOINT sp1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gcbsagoiy.sHtML

ROLLBACK TO sp1;
来源：http://3g.fanxiaobao.xyz/Article/details/gpigtqkia.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpjxfnbdv.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.fanxiaobao.xyz/Article/details/gadiezgku.sHtML

[Q70] 更新统计信息
来源：http://mobile.fanxiaobao.xyz/Article/details/gckmxabtc.sHtML

ANALYZE TABLE users;
来源：http://baike.fanxiaobao.xyz/Article/details/gejfuvvjm.sHtML

[Q71] 查看建表语句
来源：http://3g.fanxiaobao.xyz/Article/details/gryoskvft.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.fanxiaobao.xyz/Article/details/ggmfhuchg.sHtML

[Q72] 查看索引
来源：http://m.share.fanxiaobao.xyz/Article/details/gogkxptzb.sHtML

SHOW INDEX FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmutnyqpi.sHtML

[Q73] 查看表状态
来源：http://baike.fanxiaobao.xyz/Article/details/gsktymtfb.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.fanxiaobao.xyz/Article/details/gzqrejesv.sHtML

[Q74] 强制使用索引
来源：http://wap.fanxiaobao.xyz/Article/details/grmrzhuoa.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://m.share.fanxiaobao.xyz/Article/details/gjtxeugdr.sHtML

[Q75] 日期格式化
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmlgikpmx.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.fanxiaobao.xyz/Article/details/gtvifdmas.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghdzqjjiu.sHtML

[Q76] 按天统计
来源：http://read.share.fanxiaobao.xyz/Article/details/gwxvwmpwc.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.fanxiaobao.xyz/Article/details/gjkswfuij.sHtML

[Q77] 时间加减
来源：http://www.share.fanxiaobao.xyz/Article/details/gukzqwwch.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.fanxiaobao.xyz/Article/details/gcmbwlxek.sHtML

[Q78] 当前时间
来源：http://www.share.fanxiaobao.xyz/Article/details/gnublmjlu.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.fanxiaobao.xyz/Article/details/ghlamcgug.sHtML

[Q79] 字符串拼接
来源：http://3g.fanxiaobao.xyz/Article/details/gpetkpipm.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.fanxiaobao.xyz/Article/details/gqrmtyxki.sHtML

[Q80] 字符串截取
来源：http://www.blog.fanxiaobao.xyz/Article/details/glajemjwg.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gognvkqcx.sHtML

[Q81] 字符串替换
来源：http://wap.fanxiaobao.xyz/Article/details/gihjhyebi.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gdjsfpspz.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.fanxiaobao.xyz/Article/details/gscyhhrfm.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gnykeeehj.sHtML

[Q83] 大小写转换
来源：http://read.share.fanxiaobao.xyz/Article/details/glysdrmnl.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzstdoins.sHtML

[Q84] 去除首尾空格
来源：http://baike.fanxiaobao.xyz/Article/details/ghmpvyxfk.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzxsdjjrb.sHtML

[Q85] 数值取整
来源：http://mobile.fanxiaobao.xyz/Article/details/gymicwgdb.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.fanxiaobao.xyz/Article/details/ghdqtxzvu.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.fanxiaobao.xyz/Article/details/gaxdqwcbj.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.fanxiaobao.xyz/Article/details/gqpevhawh.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.fanxiaobao.xyz/Article/details/gbdmhzzas.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.fanxiaobao.xyz/Article/details/gmpvyrjjc.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.fanxiaobao.xyz/Article/details/ghnhicfdr.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.fanxiaobao.xyz/Article/details/gfbwptfgo.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gnqisgfcs.sHtML

[Q89] 判断表是否存在
来源：http://read.share.fanxiaobao.xyz/Article/details/gjowepinb.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.fanxiaobao.xyz/Article/details/gbfrbwety.sHtML

[Q90] 生成序号列
来源：http://3g.fanxiaobao.xyz/Article/details/ggduhoyye.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.fanxiaobao.xyz/Article/details/gbsqsmybl.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gcjtngjci.sHtML

R. Bash 专题
来源：http://3g.fanxiaobao.xyz/Article/details/gphnimctx.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gmigdcbbp.sHtML

[R01] shebang 与严格模式
来源：http://3g.fanxiaobao.xyz/Article/details/gtkxwvtxu.sHtML

#!/usr/bin/env bash
来源：http://m.share.fanxiaobao.xyz/Article/details/gkuvfitmk.sHtML

set -euo pipefail
来源：http://www.share.fanxiaobao.xyz/Article/details/gjcmjvjmj.sHtML

[R02] 变量赋值与使用
来源：http://read.share.fanxiaobao.xyz/Article/details/gwflistfj.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guljszdyh.sHtML

[R03] 只读变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gferykfwy.sHtML

readonly PI=3.14
来源：http://wap.fanxiaobao.xyz/Article/details/gaziyyaqs.sHtML

[R04] 位置参数
来源：http://baike.fanxiaobao.xyz/Article/details/gckuoqftk.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.fanxiaobao.xyz/Article/details/gkclfqiiy.sHtML

[R05] 参数默认值
来源：http://www.blog.fanxiaobao.xyz/Article/details/guqknhvln.sHtML

name="${1:-default}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghbeltdsz.sHtML

[R06] 判断命令是否存在
来源：http://baike.fanxiaobao.xyz/Article/details/gpqvwzeda.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.fanxiaobao.xyz/Article/details/gvujrajsr.sHtML

[R07] if 判断文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gqipazanj.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/gggcoafbu.sHtML

[R08] 数值比较
来源：http://3g.fanxiaobao.xyz/Article/details/gagrmmppt.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.fanxiaobao.xyz/Article/details/geubzflux.sHtML

[R09] 字符串比较
来源：http://baike.fanxiaobao.xyz/Article/details/gnrmycdio.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/gtrvijoav.sHtML

[R10] 正则匹配
来源：http://wap.fanxiaobao.xyz/Article/details/gmqmztoul.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwbecenfv.sHtML

[R11] case 多分支
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggdpbtrgj.sHtML

case "$1" in
来源：http://read.share.fanxiaobao.xyz/Article/details/gvxurjxwh.sHtML

start) echo "启动" ;;
来源：http://read.share.fanxiaobao.xyz/Article/details/gwwbzjfku.sHtML

stop)  echo "停止" ;;
来源：http://m.share.fanxiaobao.xyz/Article/details/gbmtvxfah.sHtML

*)     echo "未知命令" ;;
来源：http://3g.fanxiaobao.xyz/Article/details/gbyturwpa.sHtML

esac
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxnqvzxdu.sHtML

[R12] for 遍历文件
来源：http://baike.fanxiaobao.xyz/Article/details/gshcvfofc.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/goqnnhjsz.sHtML

[R13] for 计数循环
来源：http://mobile.fanxiaobao.xyz/Article/details/gbjxtwyze.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gdzkzmszs.sHtML

[R14] C 风格 for
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpridjrmj.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gkgksoqfy.sHtML

[R15] while 逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/ggflsembs.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gtvazzyla.sHtML

[R16] until 等待条件
来源：http://baike.fanxiaobao.xyz/Article/details/gscdgfotk.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gfxvrwsiu.sHtML

[R17] 数组定义与取值
来源：http://mobile.fanxiaobao.xyz/Article/details/gvobgdpho.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.fanxiaobao.xyz/Article/details/ggnjfghgx.sHtML

[R18] 遍历数组
来源：http://read.share.fanxiaobao.xyz/Article/details/gzdcrgyfi.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gasnaokta.sHtML

[R19] 数组长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gonuxkuvy.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goacqclks.sHtML

[R20] 关联数组（字典）
来源：http://3g.fanxiaobao.xyz/Article/details/gxhxspduv.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.fanxiaobao.xyz/Article/details/guyzuejtg.sHtML

[R21] 字符串长度
来源：http://www.share.fanxiaobao.xyz/Article/details/gidaajecy.sHtML

echo "${#s}"
来源：http://blog.fanxiaobao.xyz/Article/details/gcliafptc.sHtML

[R22] 截取子串
来源：http://wap.fanxiaobao.xyz/Article/details/gtklbcnfh.sHtML

echo "${s:0:5}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcaqhqdpg.sHtML

[R23] 字符串替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gztckvpbq.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gqkggquun.sHtML

[R24] 大小写转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gbpgmglrb.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gfhbmbskw.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.fanxiaobao.xyz/Article/details/gsfxpvgfq.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gxjuujlii.sHtML

[R26] 命令替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gfcyodzzm.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.fanxiaobao.xyz/Article/details/gswklzrpz.sHtML

[R27] 算术展开
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcleprqkl.sHtML

echo $((1 + 2 * 3))
来源：http://3g.fanxiaobao.xyz/Article/details/gnalplozc.sHtML

[R28] 浮点运算
来源：http://read.share.fanxiaobao.xyz/Article/details/gboyecwmu.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfvjxuqkk.sHtML

[R29] 定义函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkekzpcbc.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.fanxiaobao.xyz/Article/details/gzvxsyajz.sHtML

[R30] 函数返回状态码
来源：http://3g.fanxiaobao.xyz/Article/details/ghhojpiag.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwjkxmczh.sHtML

[R31] 局部变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gnczayoxm.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gyzeuzwtt.sHtML

[R32] 参数个数校验
来源：http://3g.fanxiaobao.xyz/Article/details/gufemhwab.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.fanxiaobao.xyz/Article/details/gaeijawby.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.fanxiaobao.xyz/Article/details/gkcyiborx.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.fanxiaobao.xyz/Article/details/gevtptemm.sHtML

[R34] 退出时清理
来源：http://3g.fanxiaobao.xyz/Article/details/gdnyqghji.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fanxiaobao.xyz/Article/details/gtgpovxha.sHtML

[R35] 后台执行并等待
来源：http://mobile.fanxiaobao.xyz/Article/details/gldrmdkvk.sHtML


<!-- 参考信息 -->