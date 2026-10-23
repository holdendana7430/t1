代发 wailian999

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3uspabmxe.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3zdzibqek.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3xgtflctp.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3lvryqxhd.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3ptehirbz.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3jztizezo.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3jpkknamt.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3iegedcny.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3wphyyohu.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3zcazmgak.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3sfjqbzxf.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3doduwayv.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3tbhohhch.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3thaoinjf.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qcmdentk.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3iypvsknc.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3cvdtbgld.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3wguhsonf.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3aipegjtj.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3lvxivtti.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3eojxnreg.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3mpgpiprc.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3gvmaxydz.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3npkgcdnv.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3rmvpzquo.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3ykiawxld.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3dfneuisw.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3hxoouafp.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3ljsohhey.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3znparvah.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3iyxfcavn.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3khdznmzf.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3jkjuikyb.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3xtwvhnxx.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3bndospuv.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3dbapjkjp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lsjjljvh.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3lhifhkzs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3viodhzvd.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3ibbuldpe.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3kslolghx.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3esylmukb.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3bqvlzzwf.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3mkhxxzss.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3swqoayvx.html

);
来源：http://www.52xcode.cn/Article/details/gt3bhefrura.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3jhxmmtxy.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3idmwgdkj.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3rpqofzyl.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3iykihkee.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3szjvlptm.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3pecmyhdl.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3czmaoaij.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3yoykgcho.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3yhbuccrv.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3smmkrejb.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3htaaxpvy.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3ityrailo.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3pnpamnoi.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3shthmppc.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3xtjyaqwb.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3hamxhyzw.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ychsonle.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3oobxkvhe.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3bjpinsij.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3nnbftiwj.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3wubunzeh.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3nnvqikym.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3kiyajsyi.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3bxroirzh.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3imzroiqj.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3xolzpobu.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3waidqarz.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3fjeawklj.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3ozevjmtt.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3ycujzqpe.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3ajiztatn.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3mccghtkd.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3xrxcbzwu.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3gxjhilgj.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3hehooqlj.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3gxfuxmwd.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3vpvbmyur.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3pbmahvxr.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3kbstrjkz.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3taiqwnkt.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3vcwshxtl.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3klehkrpx.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3mufdmmgn.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3txawlwpp.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3tcnytcqq.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3wytlckbu.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3wrvjccht.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3wsskahwx.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3dswuljit.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3fgmzfgmk.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3coroeyst.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3igldokyf.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3hmqzawtp.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3llkjphxi.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3prhyzmjy.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3kpdgphhh.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3xojueium.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3vxsucwnn.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3rogsvifj.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3egxfbyfq.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3vwtzaobp.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3edcfyxmz.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3kjupjebd.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3gqvmgtoq.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3zrwsfcmn.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3bnrhhmre.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3tvuxhwbx.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3xiynsiuk.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3pyzsoxoc.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3olmlrpwk.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3bcafnoxx.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3gdhpbxvf.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3colfinvv.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3uepizpnq.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3sujgfemz.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3heujorrg.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3yhmbixlb.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3dtwzvvdb.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3fagzlgfd.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3ygifxcld.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3mgqhweqt.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3lvjayveh.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3vbuommou.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3wbdkinmi.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3lzlonazf.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3roqocwux.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3dllibsds.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3secviluj.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3bgyltqur.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3eqokmdmi.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3hxoapcaf.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3qknztgfz.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3qpatefnc.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3vdoqbzae.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3sqcufkyw.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3xdcqpyjb.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3itrnlvcx.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3tcielkwt.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3pksqrwxj.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3pdbqaish.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3olahbgch.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3xblcganx.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3mifllxpa.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3gtihqzbp.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3wikfsthx.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3cyijbjdr.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3igkcurgg.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3vlfxjnyi.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3plvvmhwk.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3djssfivv.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3umbodxfw.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3snxrpcps.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3ddnwpohx.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3lvabsgnx.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3sonvntjb.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3ldrumjgq.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3jvnkfnoc.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3tklwpoud.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3mpvnpuiu.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3avravosl.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3kwmlstiu.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3qqxprovs.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3hjfxemqc.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3zkecrzhh.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3tnntzynb.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3bycrjmss.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3dxedxvoo.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3diwjtixe.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3nbxibbwl.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3btyibufc.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3dhhyqsaj.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3vjzdelcr.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3mkayhbxu.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3iynmzddp.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3aumpdkao.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3mfsvxojd.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3njxijulz.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3qyizlkob.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3ctyvozks.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3phcujbuh.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3aksxmnkj.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3rffyhfhw.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3zrclfllt.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3oyzzpdge.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3ncxwprzh.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3gfyaqccl.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3arfltrdu.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3lqlhjywy.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3szehwpyt.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3wwlebhnq.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3guwtxwmw.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3iidpjnee.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3hbspdbfe.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3njqlojhl.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3rlgaeegq.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3jyjolltz.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3dcxxoguk.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3sbybudiw.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3rfzppdws.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3uopsfytn.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3beatlpci.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3hbffvjez.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3ctffwzgh.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3kqsenfkx.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3kumchpnf.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3vjmxpvfj.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3ppbzmxmi.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3iqoscnsn.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3dfqljlgl.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3mxomxsdn.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3xnptwnnh.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3nrzhdgli.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3fkonfqvp.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3hrhkhbxv.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3skzilsyq.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3tjrqrdsg.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3hjowtycx.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3utuohrta.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3sfgfeuam.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3cjluzqna.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3orjmmisr.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3viesazmy.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3szpbxjyh.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3cvnjlnwr.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3ruvuvwkn.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3czdlbemm.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3iqmsvldp.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3mqfmegct.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3fcrawqfi.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3svtcxqqo.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3xzmlutjm.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3rrarhwjg.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3qlnbhpii.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3guqxgrsm.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3badqphyj.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3zjjylpxr.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3kgwbzoxf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gjkaceqq.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3hjklyuua.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bremqesa.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3hdkoeknq.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3cryioupc.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3kboflbds.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3ojsiarpr.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3hxxzhicw.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3xosugemh.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3mxhvfqmo.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3enggkggq.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3pdzshrkv.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3clytlahb.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3uncivupy.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3gltrdajh.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3zqfeyzyq.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3tizetbnm.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3xibjekkc.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3yzfbkmer.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3trvofhmc.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3kuptsxxj.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3tgjejjbx.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3nuqwxvnt.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3nrymmuur.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3yeoctgeu.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3otwcpmsv.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3ucdmajcc.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3mndlxymo.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3nyfpxisf.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3vsnkcxcp.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3ewlhakmq.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3zfiwzqox.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3liqmzqwb.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3iznmwyku.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3simslvvh.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3wsydpryc.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3mocqiipx.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ivfsnyaq.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3bdftowza.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3diigvvel.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3twcnqrzv.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3gqnnstst.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3kwykaoza.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3jqgszxqb.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3gjzxxgyw.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3lievcyjl.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3xkggmjdy.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3jftwohat.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3zjndrjhw.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3kxhifpzd.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3spjsginy.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3iodutwaz.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3sjfxnaze.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3bghvadpp.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3irerwojv.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3ufritgng.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3dwpaazad.html


<!-- 参考信息 -->