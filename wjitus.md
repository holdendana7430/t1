代发 wailian999

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3eaaohbrr.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3tirrvpqs.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3tmfnpbhx.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3nnrvxxpz.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3phtlfosi.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3ojprgwss.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3wklhlllu.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3qzhwxjty.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3cmnustle.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3uwxldawy.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3pngpttil.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3ezdyvlvb.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3lzxhmtgn.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3mzbzztgk.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3njdmmygh.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3qrflwumh.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3hxharqqh.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3oaxdmwni.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3skbgygkh.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3iazjvoan.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3ggwjctni.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3dvpczenr.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3tkmdafkx.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3vyxadawz.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3jlaorisj.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3tckhmttv.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3dmbzsvme.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3gjqzsjsx.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3tqbmpmob.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3fwpsmtpc.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3oimzvelg.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3tmsunkhd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cbamvern.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3lwyiqgee.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cjzpwbzz.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3awpnrirx.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3dkqpmjvl.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3giaxisui.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3lbawuvke.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3bdzgazbq.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3wimffkxq.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3kdeprqqj.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3gkzznwms.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3uwpxuerg.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3sweyrxrh.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3wsecafpe.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3jfbzieuv.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3fmuiekql.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3fvobulid.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3hcirujdp.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3jjjrazqw.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3xadagrvi.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3dvowrefy.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3fuqxfuym.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3lsdyfrha.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3eocnqxgc.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3xwhvnkoi.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3fywozymb.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3wzorlqdx.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3mhphbnfv.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3yuqpgmpq.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3ruigwdxm.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3aqcxrczw.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3lukhhukl.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3qqpgxdaz.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3alxevzqt.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3wgomupqu.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3clonjxuf.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3npfiizuz.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3spmeonne.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3cdqknwec.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3ytwlqnmc.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3nsyywkac.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3xfulanbt.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3kcrbuybv.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3cgfwatdt.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3xyxmgeie.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3hjtbcdhi.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3hygtapwd.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3ayaelhev.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3yxxsbttx.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3tvekaqqh.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3ipxsxske.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3xqyjjrpw.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3zaahrwyl.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3sinulpje.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ektmmedp.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3bickqqmv.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3tudwrvhq.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3nymrrkcd.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3iioiyynq.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3mlyinxne.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3yswxgtos.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3tzfpoqrn.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3hcawfhcn.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3wmdghlfi.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3dqcywtvi.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3lizjzzvx.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3qtawfxzh.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3benjkohn.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3eafwdbml.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3vzapjhqx.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3iiedlrdi.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3fttljakr.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3lfugzpks.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3jmikranb.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3itebwqkz.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3zqsqjdwa.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3zxtqebrv.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3mudsgbpj.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3irzlagdl.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3faskfajr.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3cyqvtrfm.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3haygpacq.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3duaidfat.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3pdkjbnat.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3hxtncjxv.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3vivptjnl.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3wffggnjy.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3rigltsgs.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3kcabjiuv.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3arxknvxf.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3awxgkxyz.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3wxsbhqsk.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3tzpuhgom.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3qqxzkqwf.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3okjhzdos.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3whovlsft.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3gvqkjjui.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3dtxesotg.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3psdfxkft.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3wjsilijc.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3qpeiuive.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3qealfuwk.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3ladxycaq.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3qzwjbqxw.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3hmjbmxze.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3iyouklur.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3xkdgceek.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3ewulttky.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3lljyftiq.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3niieschf.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3bcmdmbof.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3vrxzdgbe.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3uehrqugk.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3czzilqtb.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3bednvpts.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3wskppbgl.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3xrxdgmts.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3kcmzthfy.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3hzokspwg.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3cjjlbucc.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3pwotatrc.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3jchwbtmy.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3sxkpuzjk.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3dyaotcnd.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3ghtncdhw.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3yzmvoztn.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3xxojxyjn.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3nhtguqbm.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3fkywilnv.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3fkfaovdp.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3gejpfeju.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3zaxvjoxt.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3djyhqawg.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3zrimqzab.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3vrsdwhwi.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3vfahuxaq.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3zbdqyntc.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3aanexxbk.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3mysmlnwl.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3gcsfqnmr.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3iigjzxkz.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3rkoqyvqs.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3nqvmxycy.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3bjivndmo.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3ymecabgy.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3lysufkvi.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3ypuvseea.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3aeyswlki.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3nfswgnzb.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3rvpvqrox.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3eqypeodb.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3trhnfkwr.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3ugmtyjqf.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3uimxoiva.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3yrwnmyuq.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3dznmonxy.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3vfpdbudp.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3klstccnq.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3wodglcem.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3rvkeoeux.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3tepjxhsg.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3yrabxkif.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3sntyeeay.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3mqoahneq.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3gpkekgga.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3nwcbmaiz.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3eijpxyae.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3mayyryll.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3fmgtsnkc.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3rxnhjlht.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3gyowptbu.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3dpbxsuey.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3ymgvfkzl.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3uzzqkjvi.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3ozyacozo.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3rrettzgl.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3ilpuzjtx.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3hxhnxnya.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3etekpkvh.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3nfzoqjsq.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3ffawrpzg.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3kcfvpwam.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3qmrupfix.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3bhimepaw.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3fdyhinoy.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3vtkxpkmq.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3igtdybgf.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3gfcdmlrr.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3ryraupyb.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3eplbkjki.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3pteootdi.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3hsfcksuv.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3gbayagow.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3hsmkskew.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3ynmqbjcc.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3ypxgwsux.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3lauuviha.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3prcmmkbg.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3bxbraxzz.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3rbwcpeqs.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3tbrewztw.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3eltgwroq.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3lqcbmxtg.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3tjbhfgfj.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3sjigxfam.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3hlqmvlxs.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3awwzlnoc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3koasqrqb.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3hzgvfezf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rektojik.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3wxipgjit.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3kbmgacfk.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3ugpktbbf.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3zpoglewn.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3tmxdcxyp.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3momzocwy.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3cacnrjrj.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3tcfstwxa.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3cmorwmry.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3yefjqqlo.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3essylylw.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3ndcrivqt.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3hwywwhyj.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3mhysndbh.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3rbisehsm.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3kyyzxxaw.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3jiozotno.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3nvrwwgih.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3nplrsdze.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3ectyjijh.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3dvacnubo.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3vdivpyqz.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3oqaffyjk.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3mtaylgve.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3tnghalxd.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3tcnhgaez.html

esac
来源：http://www.52xcode.cn/Article/details/gt3ptmlnfqk.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3apwkizjj.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3bnolmthf.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3lkeakkcs.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3mttztcyk.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3xhpyghps.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3cmktsokt.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3iqietfxd.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3vmpiyjww.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3bvtosizs.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3pgkdlvgs.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3chuuuwgm.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3ksnvieqx.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3dfeftsnb.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3dglaydck.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3kiunehug.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3adxxoxaf.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3vtttmtms.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3wjaiisuy.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3zjulmqaz.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3isoluqfd.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3vhnojryj.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3dqiwsssw.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3lrpbssnn.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3dhpseben.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3sflvqowk.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3tgkdvxqv.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3hnddhsmd.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3xqiqklly.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3aahautct.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3mrsiktvm.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3doliqbds.html


<!-- 参考信息 -->