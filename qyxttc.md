代发 wailian999

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3nichjoty.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3hualzogx.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3exwvjbao.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3tttqigkl.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3rpccrugr.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3igzaprvx.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3fofunbob.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3yptzpihw.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3zrfprjme.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3xrhbojro.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3uplrkjfj.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3dpzhpzer.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3nfnjbqsm.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3iwhapdbo.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3uqyziqrb.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3bfavmlju.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3zbxlsvwt.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3ihfmlnbq.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3iawcfjme.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ydbebvej.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3fwjmeorp.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vablxklq.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3jgqksalo.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3tjdwnxdn.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3mnrqtpzi.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3udiotjgs.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3wxhgqagu.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3qfdszgnt.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3bzphqbon.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3pyalynnb.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3cgmcuzjs.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3ymfbjejn.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3ckhtwiln.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3uekbbpzh.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3djwwkjeg.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3vashwcss.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3ejtyhfgq.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3cmzimtms.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3igjppyhn.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3qkfytepz.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3lfdoyycm.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3scnwflue.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3hrsqqezn.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3juchbjta.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3abdxvkxj.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3swnqepah.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gziwuirl.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3lasjpxrg.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3nerfuqlu.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3gnrjrqwt.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3dihjigpt.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3plbtdean.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3wtqdxssi.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3qijwaysu.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3bdnjetbr.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3gfvazxbb.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3luhutyyi.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3xnlfzfrb.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3blhrvigq.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3bpigulgh.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3pxcjeazf.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3ablyvlqo.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3musnaezf.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3jbmbbukp.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3ipwolkvf.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3erwjwnoe.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3jfeguwcp.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3bblqpcls.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3dljcvyye.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3lxzplxtl.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3wneysljv.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3cuannuzh.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3pikvfbmw.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3wtwmuuwk.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3nrkvzvht.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3xinqbrkt.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3dvysnylj.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3ffaxjxxy.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3wiihwodx.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3hgtdirhi.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3dmrbhjtf.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3lfxdiakm.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3uqcdfkas.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3gvkohqxv.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3tmypvcom.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3nffxtuzk.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3vwcgloja.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3gnhnquai.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3tvxcssuj.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3msykjklu.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3sflgqjux.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3vjsztvae.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3hyznopnf.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3caygvabr.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3mjknzrkj.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3ivscfqoc.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3fwtumyzq.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3zsooqteu.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3lnqtnprw.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3dxhdcxij.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3hlebxmby.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3licueqeo.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3lxggkxxq.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3dehiuwmm.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3vcicwpls.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3zzbarwhz.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3rglobwyo.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3gskyhodz.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3udnpybbb.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3nwyaztvy.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3mpjzvmju.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3hiyheuay.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3otzpopaf.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3hxtdcoxi.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3cbwlsqms.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3upmnfzdh.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3vslqkmlx.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3mvqeksud.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3ortvliuz.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3dspyzvet.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3fsyyqmqp.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3vpwiexqo.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3jicydutu.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3xkgxfsdc.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3nolheniw.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3vgvkufyn.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3szdtxrgy.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3kohagkoe.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3dbfgknrz.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3qnfnpapf.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3shusfcza.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3jwufkqfd.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3jskbspmg.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3satygedz.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3umjygctl.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3cixrcygi.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3yjnuksdt.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3kuwhmhoq.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3fgbtirze.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3xosnehfm.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3camaztnl.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3zoqpxqts.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3kfhwhtou.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3fmegjrcn.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3ryggzvug.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3cnxuakki.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3gqnbtdal.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3vnrvbpbl.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3vrzlqwcp.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3dbzcksxj.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3paeifkwc.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3ltcypscq.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3fjqenzwi.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3uehzypbe.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3qqtrzywn.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3igtnhchu.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3ibpnbndm.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3nelurkuu.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3hidtsxhd.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3higfnlsk.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3tmkkbmmu.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3uebsmzms.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3ruyxvvkm.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3yywqpqiz.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3tngpayvh.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3gqsvesec.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3saxdvtvm.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3yxmiltzs.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3hnzkmmir.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3eayuyvmn.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3lgymjvgt.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3wuqazhnt.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3tfopdmxf.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3zzciaxmb.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3nztmzygg.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3hjhyjepm.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3dqvpzkjq.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3zjdlknwi.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3yuwmusqd.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3izxusctb.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3xiqgaadq.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3puxxtgni.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3zxwjzfgy.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3ysqetlkz.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3ltexztoy.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3rlkfffwx.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3ubvlurct.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3pzgpubjc.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3vgmrjilt.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3dcmqigjj.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3ldhbelxg.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3jegczrhc.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3upksgsay.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3xchymduw.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3wadovhac.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3lafkukps.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3hvbhiyxp.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3fdbzlnlb.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3aqzwjqkx.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3izgqaqmk.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3hnppzuuz.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3hduvlzuw.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3tufzchgj.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3peyhrgxd.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3uiqebisy.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3iqxblvve.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3qbhqnmvu.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3skfinavs.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3axjwjgax.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3igqwhfco.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3xtgpjohx.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3bribzcib.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3puybdrwm.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3gmiinorg.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3nqqvuild.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3udanityu.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3krbicbxz.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3vikyyohe.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3fksnbnbq.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3jxrowtyj.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3iehkgmul.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3chgddemp.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3hbhaisan.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3jsdrwrhr.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3cdeiagnm.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3mzgstlgi.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3hgxsnqcw.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3qrwtbkgr.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3llbbmbve.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3algdxwby.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3bchmzexo.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3zonlgwoc.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3ldllmbsf.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3rwzlupds.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3hvwzdvuu.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3oqftqxlz.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3zqkijyqc.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3jrqmzblw.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3jrammiyd.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3qdqiqfjr.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3gfozwkty.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3jopgmypa.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3gcdqfbke.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3vaafgtzs.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3fzmdqlvg.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3qixexfsb.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3gjtveluz.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3tyayzfbv.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3rslgppdt.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3rfxvjotr.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3pmygqwno.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zrxlyqkb.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3alrgwuim.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3exgwoful.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3jmfazzyx.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3uyyqlclb.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3bjxtendj.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3slhgzpwr.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3kgvhufzn.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3gvqssdbv.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3xqyjijhw.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3fnclidzm.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3mywwptlp.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3jpfhqskb.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3avqbtidw.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3lzrpljbg.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3dqzutmai.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3ixpkxhaf.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3stbauffm.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3yfgtbsmy.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3bkjenfsm.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3qvnjssxo.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3xfvylpjg.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3ssphrkdc.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3frigqfpt.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3tvopchlh.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3omikwvta.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3raibylxr.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3fvykrjfa.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3iaaduddu.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3skewgigt.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3bnfivltm.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3kycgohow.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3ocxgfwui.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3rxnldukx.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3kpbaxqog.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3bfmxhukv.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3jbdcgdgt.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3jxjbheww.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3kimxdxce.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3jwaxnymd.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3qslpuwwq.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3ifdtcega.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3jsuxrjwj.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3wvikjvoi.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3apndzupp.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3fvsguzwz.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3qvimhmok.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3djcitlwy.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3qhafwbwh.html


<!-- 参考信息 -->