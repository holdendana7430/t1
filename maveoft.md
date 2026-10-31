代发 wailian999

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://do.haigaiapp.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://xq.szsharing.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ia.shtwfgs.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://cw.haigaiapp.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://sd.panjiajie.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://lu.haigaiapp.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://em.jctech888.com.cn

[P04] 求长度
来源：http://fk.wgjwhj.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://uj.gzmigu.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://nm.lnxyls.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://on.9csxet.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://xy.521024.cn

Java: list.size();  map.size();  s.length()
来源：http://uq.gzmigu.cn

Go:   len(arr);  len(m)
来源：http://ev.shxzskj.cn

Ruby: x.length;  x.size
来源：http://nf.huanxung.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://ev.colortex.cn

[P05] 判断两个对象内容是否相等
来源：http://of.jctech888.com.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://tb.jctech888.com.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ht.huixiangedu.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://fr.panjiajie.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://nl.chemitech.net.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://nx.wgjwhj.cn

Go:   reflect.DeepEqual(a, b)
来源：http://bf.hahajie.cn

Ruby: a == b
来源：http://de.chemitech.net.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://uq.haigaiapp.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://uq.lnxyls.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ac.szxytkj.cn

PHP:  if (empty($x)) {}
来源：http://bq.bjjhwx.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://df.huixinmuqiang.cn

TS:   if (x == null) {}
来源：http://ef.haigaiapp.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://ru.newstarts.cn

Go:   if x == nil {}
来源：http://ux.521024.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://on.shxzukj.cn

C#:   if (x is null) {}
来源：http://le.muxihuayi.cn

[P07] 防抖与节流
来源：http://rf.shxzukj.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hq.chemitech.net.cn

PHP:  // 手写时间戳比较
来源：http://mu.hahajie.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ms.wgjwhj.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ro.newstarts.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://bx.huanxung.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://yo.shxzskj.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://gw.yuexingan06.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://jn.newstarts.cn

[P08] 处理浮点精度问题
来源：http://wq.huixinmuqiang.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ib.yuexingan06.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://qi.bjjhwx.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://zz.panjiajie.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://rr.szxytkj.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://lu.huanxung.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ua.gzmigu.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://qr.newstarts.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hg.haigaiapp.cn

================================================================================
来源：http://vt.szsharing.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://uz.hnjuh.cn

================================================================================
来源：http://ma.nicolike.cn

[Q01] 创建表
来源：http://nz.jianghongdianzi.cn

CREATE TABLE users (
来源：http://aj.panjiajie.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://qs.hnjuh.cn

name VARCHAR(50) NOT NULL,
来源：http://kw.jctech888.com.cn

email VARCHAR(100) UNIQUE,
来源：http://fr.lnxyls.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ub.jianghongdianzi.cn

);
来源：http://br.9csxet.cn

[Q02] 创建带外键的表
来源：http://jb.yuntaijiaju.cn

CREATE TABLE orders (
来源：http://tq.lnxyls.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://tg.colortex.cn

user_id INT NOT NULL,
来源：http://hq.huixiangedu.cn

amount DECIMAL(10, 2),
来源：http://bj.newstarts.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://jn.yuexingan06.cn

);
来源：http://xa.haigaiapp.cn

[Q03] 增加列
来源：http://fg.chemitech.net.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ye.shxzskj.cn

[Q04] 修改列类型
来源：http://ip.shtwfgs.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://qh.jctech888.com.cn

[Q05] 重命名列
来源：http://cn.muxihuayi.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://iz.szxytkj.cn

[Q06] 删除列
来源：http://un.shtwfgs.cn

ALTER TABLE users DROP COLUMN age;
来源：http://ng.muxihuayi.cn

[Q07] 删除表
来源：http://be.nicolike.cn

DROP TABLE IF EXISTS orders;
来源：http://es.szsharing.cn

[Q08] 创建普通索引
来源：http://zw.nszjky.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://sw.gzmigu.cn

[Q09] 创建唯一索引
来源：http://kt.colortex.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://py.jctech888.com.cn

[Q10] 插入单行
来源：http://ra.wgjwhj.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://fo.wgjwhj.cn

[Q11] 一次插入多行
来源：http://rw.chemitech.net.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://zs.huixinmuqiang.cn

[Q12] 插入后取自增 ID
来源：http://la.jctech888.com.cn

INSERT INTO users (name) VALUES ('C');
来源：http://qx.yuexingan06.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://bh.yuntaijiaju.cn

[Q13] 忽略重复插入
来源：http://js.chemitech.net.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://vk.haigaiapp.cn

[Q14] 存在则更新（upsert）
来源：http://fc.gzmigu.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wn.szsharing.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://iz.jianghongdianzi.cn

[Q15] 查询全部
来源：http://zr.9csxet.cn

SELECT * FROM users;
来源：http://zn.jianghongdianzi.cn

[Q16] 查询指定列
来源：http://wj.shxzskj.cn

SELECT id, name FROM users;
来源：http://ck.szsharing.cn

[Q17] 条件查询
来源：http://ra.hahajie.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ao.hnjuh.cn

[Q18] 模糊匹配
来源：http://no.bookmarksfly.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://si.9csxet.cn

[Q19] 范围查询
来源：http://xm.shtwfgs.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://qe.nicolike.cn

[Q20] IN 列表
来源：http://nq.huixiangedu.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://kr.wgjwhj.cn

[Q21] 空值判断
来源：http://dw.muxihuayi.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://kf.nszjky.cn

[Q22] 排序
来源：http://nr.panjiajie.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://gy.nicolike.cn

[Q23] 分页
来源：http://on.hnjuh.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ey.9csxet.cn

[Q24] 去重
来源：http://nr.bjjhwx.cn

SELECT DISTINCT city FROM users;
来源：http://cj.hahajie.cn

[Q25] 只取前 N 条
来源：http://yo.jctech888.com.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://fi.szsharing.cn

[Q26] 计数
来源：http://cz.lnxyls.cn

SELECT COUNT(*) FROM users;
来源：http://hn.yuexingan06.cn

[Q27] 条件计数
来源：http://vu.yuntaijiaju.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://qk.wgjwhj.cn

[Q28] 求和与平均
来源：http://ot.gzmigu.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://io.haigaiapp.cn

[Q29] 最大最小值
来源：http://zh.lnxyls.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://kt.shtwfgs.cn

[Q30] 分组统计
来源：http://ts.huixinmuqiang.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://tt.shtwfgs.cn

[Q31] 分组后过滤
来源：http://zt.shxzskj.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://xe.hahajie.cn

[Q32] 分组拼接字符串
来源：http://tw.colortex.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mj.gzmigu.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://vu.asd995.cn

[Q33] 多列分组
来源：http://yf.panjiajie.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wr.newstarts.cn

[Q34] 每组取第一条
来源：http://gu.huanxung.cn

SELECT * FROM (
来源：http://hp.bookmarksfly.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ef.huixinmuqiang.cn

) t WHERE rn = 1;
来源：http://qi.bookmarksfly.cn

[Q35] 内连接
来源：http://ug.huixiangedu.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://cl.gzmigu.cn

[Q36] 左连接
来源：http://hw.lnxyls.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hp.nicolike.cn

[Q37] 右连接
来源：http://xc.shxzukj.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://qh.shxzskj.cn

[Q38] 全外连接（PostgreSQL）
来源：http://si.huixiangedu.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://jm.jctech888.com.cn

[Q39] 自连接（查上下级）
来源：http://fw.bjjhwx.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://lt.hahajie.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://iq.szxytkj.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://iu.muxihuayi.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://gp.szsharing.cn

[Q41] 多表连接
来源：http://oi.bjjhwx.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://fx.jctech888.com.cn

JOIN users u ON u.id = o.user_id
来源：http://qt.colortex.cn

JOIN products p ON p.id = o.product_id;
来源：http://tc.huanxung.cn

[Q42] 连接条件附加过滤
来源：http://sw.colortex.cn

SELECT u.name, o.amount FROM users u
来源：http://bf.shxzskj.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://vx.hahajie.cn

[Q43] 标量子查询
来源：http://cq.huanxung.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://qf.lnxyls.cn

[Q44] IN 子查询
来源：http://yy.521024.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ap.huanxung.cn

[Q45] EXISTS 判断存在
来源：http://ig.nszjky.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://lh.lnxyls.cn

[Q46] NOT EXISTS 判断不存在
来源：http://zs.szsharing.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://uy.newstarts.cn

[Q47] 与平均值比较
来源：http://fw.shxzukj.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://fq.gzmigu.cn

[Q48] CTE 公用表表达式
来源：http://aa.hahajie.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wa.hnjuh.cn

SELECT * FROM t WHERE c > 5;
来源：http://ih.shxzukj.cn

[Q49] 更新单行
来源：http://uv.shtwfgs.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://lv.chemitech.net.cn

[Q50] 批量更新
来源：http://ib.shxzukj.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://st.panjiajie.cn

[Q51] 用子查询更新
来源：http://sk.asd995.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://gz.panjiajie.cn

[Q52] 删除指定行
来源：http://qz.asd995.cn

DELETE FROM users WHERE id = 10;
来源：http://ae.haigaiapp.cn

[Q53] 按条件删除
来源：http://ji.huixinmuqiang.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://sq.lnxyls.cn

[Q54] 清空表
来源：http://vq.asd995.cn

TRUNCATE TABLE logs;
来源：http://ug.hnjuh.cn

[Q55] 排名（并列占位）
来源：http://pp.asd995.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://xi.hnjuh.cn

[Q56] 密集排名（并列不占位）
来源：http://jt.yuexingan06.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://qe.9csxet.cn

[Q57] 行号
来源：http://ei.yuntaijiaju.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://at.bookmarksfly.cn

[Q58] 累计求和
来源：http://we.hahajie.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://de.hnjuh.cn

[Q59] 分组内累计
来源：http://vl.muxihuayi.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ms.9csxet.cn

[Q60] 取上一行 / 下一行
来源：http://im.bookmarksfly.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wc.huanxung.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://gp.muxihuayi.cn

[Q61] 移动平均
来源：http://eb.yuntaijiaju.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://rh.szsharing.cn

[Q62] 分组占比
来源：http://po.huixinmuqiang.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://oy.shtwfgs.cn

[Q63] 开启事务
来源：http://ht.nszjky.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://at.muxihuayi.cn

[Q64] 提交事务
来源：http://ny.bjjhwx.cn

COMMIT;
来源：http://yl.gzmigu.cn

[Q65] 回滚事务
来源：http://ls.muxihuayi.cn

ROLLBACK;
来源：http://de.haigaiapp.cn

[Q66] 行锁查询
来源：http://qn.yuexingan06.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ey.521024.cn

[Q67] 设置隔离级别
来源：http://zx.chemitech.net.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://gm.wgjwhj.cn

[Q68] 保存点
来源：http://da.wgjwhj.cn

SAVEPOINT sp1;
来源：http://go.bjjhwx.cn

ROLLBACK TO sp1;
来源：http://jl.9csxet.cn

[Q69] 查看执行计划
来源：http://kl.colortex.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://cr.nicolike.cn

[Q70] 更新统计信息
来源：http://zv.huixinmuqiang.cn

ANALYZE TABLE users;
来源：http://cj.muxihuayi.cn

[Q71] 查看建表语句
来源：http://yp.nszjky.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://yf.hahajie.cn

[Q72] 查看索引
来源：http://qn.huanxung.cn

SHOW INDEX FROM users;
来源：http://yk.chemitech.net.cn

[Q73] 查看表状态
来源：http://jl.gzmigu.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://rg.panjiajie.cn

[Q74] 强制使用索引
来源：http://cb.panjiajie.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ea.jctech888.com.cn

[Q75] 日期格式化
来源：http://bh.lnxyls.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://vj.haigaiapp.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mm.shtwfgs.cn

[Q76] 按天统计
来源：http://jr.9csxet.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ca.newstarts.cn

[Q77] 时间加减
来源：http://az.asd995.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://vs.shxzukj.cn

[Q78] 当前时间
来源：http://pu.asd995.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://se.szxytkj.cn

[Q79] 字符串拼接
来源：http://mh.jianghongdianzi.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://sw.shxzskj.cn

[Q80] 字符串截取
来源：http://zs.shxzukj.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://xu.bookmarksfly.cn

[Q81] 字符串替换
来源：http://rn.asd995.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://lk.bjjhwx.cn

[Q82] 字符长度与字节长度
来源：http://gc.jianghongdianzi.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://jj.hnjuh.cn

[Q83] 大小写转换
来源：http://jc.haigaiapp.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ib.szsharing.cn

[Q84] 去除首尾空格
来源：http://ut.colortex.cn

SELECT TRIM(name) FROM users;
来源：http://ys.szsharing.cn

[Q85] 数值取整
来源：http://yl.huixiangedu.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://bu.shxzukj.cn

[Q86] 读取 JSON 字段
来源：http://me.shtwfgs.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ec.bjjhwx.cn

[Q87] JSON 字段做条件
来源：http://ip.jctech888.com.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ex.shxzukj.cn

[Q88] 行转列（条件聚合）
来源：http://fk.hahajie.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://qe.haigaiapp.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://kg.521024.cn

[Q89] 判断表是否存在
来源：http://qf.nicolike.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://bh.yuntaijiaju.cn

[Q90] 生成序号列
来源：http://md.9csxet.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://qo.jctech888.com.cn

================================================================================
来源：http://se.huixiangedu.cn

R. Bash 专题
来源：http://lx.nicolike.cn

================================================================================
来源：http://kl.shxzskj.cn

[R01] shebang 与严格模式
来源：http://kg.jianghongdianzi.cn

#!/usr/bin/env bash
来源：http://ch.bjjhwx.cn

set -euo pipefail
来源：http://uw.jianghongdianzi.cn

[R02] 变量赋值与使用
来源：http://dr.shtwfgs.cn

name="Tom"; echo "$name"
来源：http://ru.wgjwhj.cn

[R03] 只读变量
来源：http://oh.hahajie.cn

readonly PI=3.14
来源：http://hi.wgjwhj.cn

[R04] 位置参数
来源：http://si.chemitech.net.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://jm.wgjwhj.cn

[R05] 参数默认值
来源：http://jo.bjjhwx.cn

name="${1:-default}"
来源：http://pv.bjjhwx.cn

[R06] 判断命令是否存在
来源：http://tp.hahajie.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://gh.yuexingan06.cn

[R07] if 判断文件
来源：http://dv.shxzukj.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://zd.szsharing.cn

[R08] 数值比较
来源：http://pz.hnjuh.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://mz.colortex.cn

[R09] 字符串比较
来源：http://nt.colortex.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://qp.huixiangedu.cn

[R10] 正则匹配
来源：http://fg.hnjuh.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://gq.shtwfgs.cn

[R11] case 多分支
来源：http://rt.521024.cn

case "$1" in
来源：http://bm.szsharing.cn

start) echo "启动" ;;
来源：http://in.chemitech.net.cn

stop)  echo "停止" ;;
来源：http://tk.bjjhwx.cn

*)     echo "未知命令" ;;
来源：http://vv.huixinmuqiang.cn

esac
来源：http://ll.panjiajie.cn

[R12] for 遍历文件
来源：http://gz.huanxung.cn

for f in *.txt; do echo "$f"; done
来源：http://da.colortex.cn

[R13] for 计数循环
来源：http://gn.szsharing.cn

for i in {1..10}; do echo "$i"; done
来源：http://xm.huanxung.cn

[R14] C 风格 for
来源：http://dn.szsharing.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://br.huixinmuqiang.cn

[R15] while 逐行读文件
来源：http://js.hahajie.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://sn.chemitech.net.cn

[R16] until 等待条件
来源：http://co.shxzukj.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ja.jianghongdianzi.cn

[R17] 数组定义与取值
来源：http://di.9csxet.cn


<!-- 参考信息 -->