代发 wailian999

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3ilzjdacs.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3isvvklmu.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3rpotbfij.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3fptfyhpn.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3jcyonkky.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3ywgdkcvk.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3wgwzfnrk.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3yygpghyt.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3xxagziwe.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nusdikop.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3toodgqbl.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3ztvvptcv.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3twzldori.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jkqvogqq.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3ffrmkqhi.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3sxvmkmpv.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3ahdclnsh.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3omkkwekd.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3tzffcryt.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3aoggboxo.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3kdfxygmz.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3nljfecdm.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3iotuftsk.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3bjnikhyg.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3tbfgpnmr.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3rapqbvmz.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3qlpfcbew.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3xgvlafiy.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3kwvloxgw.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3mmsmovgc.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3zqrgtuse.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3fzarzodd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rfteygex.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3kbibbvuv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dlllhrlf.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3fstlacgc.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3mmvpflaj.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3jzmiuyjs.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3varjgudx.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3ovgwkfnr.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3qhuqrkru.html

);
来源：http://www.52xcode.cn/Article/details/gt3ivxauryw.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3hykvdpny.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3vhhrwgat.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3etahyrsb.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3aaiedyoa.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3arufyqkg.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3mjekmogj.html

);
来源：http://www.52xcode.cn/Article/details/gt3tuzfkpzt.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3jkgzmrof.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3xamwcrwu.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3pnjootnp.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3sfcdxcwu.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3qldmtbfs.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3cdhetqse.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3nqmegzsj.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3ujxvhpik.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3szdmagtm.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3lcfvhwpv.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3gvmpcjzp.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3cnyynzds.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3rjsangqv.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3zbjwonho.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3tgzzpupe.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3fkqylpsm.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3ukqfokbx.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3reqajshr.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3esxpdrmb.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3woccyuhb.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3bkihbeym.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3knsocfyj.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3qlvmnmnl.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3ujuhjcza.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3qfyfpigf.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3xjxrjlsp.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3nbagytuj.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3jhdcypyc.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3tnyfqqzc.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3gsxjxywb.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3dkybsqzb.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3tiywdpxg.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3qfgyrcut.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3ybmngnxr.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3ydhwjdoj.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3ijepkrlq.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3knkcehkb.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3iyvmqeut.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3uxbdfnqm.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3pmoauimd.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3mcxraptw.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3ryjvzocm.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3mwgyvcln.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3qxioapeb.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3vlucgsga.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3vciotvmh.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3btvttwvr.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3prphthoh.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3hcmgqssz.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3sfxvniyu.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3mdtnzacq.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3amjrmrpz.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3tehfifrn.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3jbsaobsj.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3lpeiirua.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3htpkfttz.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3hfivfghq.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3dvujmxwi.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3acllnejs.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3lteytdjv.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3jogqthhf.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3xpuogpfa.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3ihtxgidq.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3ytyayuom.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3rxqoemrq.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3iuuittsm.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3hrqgqwnw.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3lnrgxgaa.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3hvupdoud.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3mwaekfko.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3yuvobxgw.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3pfzdqgmr.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3ebzitsfq.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3wtmmggiw.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3tsbjuiim.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3tbngbzcf.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3vjzzcxah.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3fanxnwyd.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3rcjrlmue.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3ntwnuubj.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3ototieyi.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3eujqoabd.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3xjsqbdea.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3ijjalsvu.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3tsmtiqgt.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3fistdikq.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3bwehepbx.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3cdodqblp.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3ztctkhtz.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3lireehvm.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3infsncsd.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3nnqqehie.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3bvysnfoa.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3zwszeyrh.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3ewhqnvbq.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3rifohfng.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3bnzogivc.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3fvuavhhu.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3vafvbqiu.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3uiesooou.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3mskucnyd.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3xmeizurb.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3frjjxdlr.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3gesbraaz.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3jhwizdlx.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3zicdghof.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3hdzxfztd.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3wgadkhpu.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3ouvwhdkq.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3zbxrqnqs.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3ivbwkrfr.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3wsmzrifj.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3kirptjfe.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3jxbgeoab.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3phedcsrg.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3aldtvhim.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3rxqflcpm.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3ndvxuwpo.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3yynunjba.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3jdipwdva.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3zjvzgvcz.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3jliesevq.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3jcywsdjj.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3dwjpebuo.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3yjpjndqs.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3eiwgqrpf.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3madqilve.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3kttvtbsc.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3tghrnbgp.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3nvjbghbu.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3vwogfsuo.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3lemngkos.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3uubjukdl.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3eqsaxucx.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3egmkgmwz.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3pzmrakdg.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3tqvxbyyj.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3rnqmnqfn.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3urqivujz.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3hspmpxsh.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3qwpyaabv.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3alivsmwu.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3ehotysjb.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3izfqljum.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3zivzwggt.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3wmwctzmj.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3blasmvmb.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3hpetsjlk.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3jcqluymn.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3kmglriwc.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3puwbvhgx.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ojiramvb.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3flpymkxe.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3piwtshcs.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3llyfkjch.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3otzqhzjl.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3ameuibob.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3lwtdwwia.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3yqkhmqrm.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3lezqkzce.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3urcuhwfl.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3yioanwoh.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3iwjecrww.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3bebmypyp.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3fgvoppmi.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3jgfzxwsz.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3jjoaedem.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3cpruaqft.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3znsqrfxj.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3yucfhoae.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3puwobman.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3nwffykkq.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3yycltpqk.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3zeovuwzi.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3wysxssfx.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3dujhzuee.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3xtnrqyyx.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3llvgvqpx.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3ugnbqulj.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3labxfcuz.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3hoplcbiy.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3fwuscfjr.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3tdorczhh.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3npgbgdke.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3dtkzthws.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3kwmxjbmh.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3zqzuoxgw.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3fiqccjmg.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3phopjbnn.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3ztcvcgjx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xaljztqz.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3ypxpquly.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nkncizki.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3rbjittmv.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3widfxxih.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3rsisvesp.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3svgkgnod.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3eyhyrsim.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3daqkrywh.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3wyoqhtbu.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3wpjxdofq.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3ifjjpwpz.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3peotsnqq.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3awzquqcd.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3zvptqeel.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3xnkkodej.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3dxdokiln.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3ayqxnbwy.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3cslrahhg.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3lfqesvvq.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3qafxthjd.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3lhunzwzh.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3neomkpil.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3cdgxgbtw.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3mqnhcvwb.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3wdvggizn.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3tbqstyps.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3ntntbccu.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3dfkghbpe.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3nkhocwnb.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3vybnoeci.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3yyulxqit.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3dzovlkfd.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3gosvjbeq.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3xwvkjcgq.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3nfpinner.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3ixwdmiwz.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3araqoqkz.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3avjyaoqa.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3ttnktdgy.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3wwnrkxao.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3wdhbbcmm.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3hbsfegrr.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3jmuvlxoa.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3jlcongkc.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3igjdjyqu.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3zzwtaxsc.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3ebntybem.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3cxbwksxi.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3nficlilk.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3ycjyeaqq.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3xtnbrrkm.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3ijlfxpam.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3lqvfiyam.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3moyjhaxr.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3wcqmhpht.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3inmoevbd.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3rffywcnn.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3ngfwgpki.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3oadfaauo.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3qhbrkwit.html


<!-- 参考信息 -->