代发 wailian999

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ih.szxytkj.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://na.wgjwhj.cn

[P03] 生成短随机字符串
来源：http://dp.jianghongdianzi.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://bu.chemitech.net.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://dq.lnxyls.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://qr.jctech888.com.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hk.nszjky.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://lb.shtwfgs.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ca.shxzukj.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://us.lnxyls.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://lq.hnjuh.cn

[P04] 求长度
来源：http://mr.lnxyls.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://zs.panjiajie.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://rl.nicolike.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://pw.bjjhwx.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hw.9csxet.cn

Java: list.size();  map.size();  s.length()
来源：http://em.wgjwhj.cn

Go:   len(arr);  len(m)
来源：http://uv.shtwfgs.cn

Ruby: x.length;  x.size
来源：http://to.hnjuh.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://bg.muxihuayi.cn

[P05] 判断两个对象内容是否相等
来源：http://wj.shxzskj.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://zi.shxzukj.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://yi.szxytkj.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://qh.gzmigu.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://gz.shxzukj.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://xy.shxzskj.cn

Go:   reflect.DeepEqual(a, b)
来源：http://pp.huanxung.cn

Ruby: a == b
来源：http://mf.colortex.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://gp.shtwfgs.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://sc.9csxet.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://yx.huanxung.cn

PHP:  if (empty($x)) {}
来源：http://cy.bjjhwx.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://gx.panjiajie.cn

TS:   if (x == null) {}
来源：http://rv.521024.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://um.huanxung.cn

Go:   if x == nil {}
来源：http://bq.newstarts.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://kk.yuntaijiaju.cn

C#:   if (x is null) {}
来源：http://ky.huanxung.cn

[P07] 防抖与节流
来源：http://of.yuntaijiaju.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://az.lnxyls.cn

PHP:  // 手写时间戳比较
来源：http://pk.asd995.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://cl.asd995.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://gi.newstarts.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://il.jianghongdianzi.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://li.hnjuh.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://lk.yuexingan06.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://td.yuexingan06.cn

[P08] 处理浮点精度问题
来源：http://dr.shxzskj.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://jb.jianghongdianzi.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://le.hahajie.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://pm.521024.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://fu.bjjhwx.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://xn.nszjky.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://di.szxytkj.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ho.huixinmuqiang.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://jc.shxzukj.cn

================================================================================
来源：http://dk.jianghongdianzi.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wf.shtwfgs.cn

================================================================================
来源：http://jo.haigaiapp.cn

[Q01] 创建表
来源：http://sz.colortex.cn

CREATE TABLE users (
来源：http://hd.9csxet.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://uk.jctech888.com.cn

name VARCHAR(50) NOT NULL,
来源：http://lv.521024.cn

email VARCHAR(100) UNIQUE,
来源：http://yy.521024.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://te.jctech888.com.cn

);
来源：http://ot.shxzskj.cn

[Q02] 创建带外键的表
来源：http://ao.panjiajie.cn

CREATE TABLE orders (
来源：http://vx.yuexingan06.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://xd.haigaiapp.cn

user_id INT NOT NULL,
来源：http://td.shxzukj.cn

amount DECIMAL(10, 2),
来源：http://mp.gzmigu.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mi.colortex.cn

);
来源：http://bk.yuntaijiaju.cn

[Q03] 增加列
来源：http://mp.panjiajie.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://zu.9csxet.cn

[Q04] 修改列类型
来源：http://as.chemitech.net.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://iq.shxzukj.cn

[Q05] 重命名列
来源：http://oy.panjiajie.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://gw.szsharing.cn

[Q06] 删除列
来源：http://ln.bookmarksfly.cn

ALTER TABLE users DROP COLUMN age;
来源：http://lu.shxzukj.cn

[Q07] 删除表
来源：http://vg.bookmarksfly.cn

DROP TABLE IF EXISTS orders;
来源：http://ra.szxytkj.cn

[Q08] 创建普通索引
来源：http://at.huixinmuqiang.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://xs.muxihuayi.cn

[Q09] 创建唯一索引
来源：http://aq.huixiangedu.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://vq.huixiangedu.cn

[Q10] 插入单行
来源：http://kb.shtwfgs.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://zj.haigaiapp.cn

[Q11] 一次插入多行
来源：http://hd.muxihuayi.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://xl.yuntaijiaju.cn

[Q12] 插入后取自增 ID
来源：http://ia.shxzskj.cn

INSERT INTO users (name) VALUES ('C');
来源：http://aw.panjiajie.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://kw.asd995.cn

[Q13] 忽略重复插入
来源：http://fs.yuexingan06.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hr.9csxet.cn

[Q14] 存在则更新（upsert）
来源：http://ho.jianghongdianzi.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://eh.szsharing.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://bq.jctech888.com.cn

[Q15] 查询全部
来源：http://kt.panjiajie.cn

SELECT * FROM users;
来源：http://nx.huanxung.cn

[Q16] 查询指定列
来源：http://zo.panjiajie.cn

SELECT id, name FROM users;
来源：http://uj.hnjuh.cn

[Q17] 条件查询
来源：http://qu.huixiangedu.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://kn.jctech888.com.cn

[Q18] 模糊匹配
来源：http://sr.muxihuayi.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://xs.asd995.cn

[Q19] 范围查询
来源：http://nd.panjiajie.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://pc.bjjhwx.cn

[Q20] IN 列表
来源：http://ju.9csxet.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://vd.newstarts.cn

[Q21] 空值判断
来源：http://uh.shxzukj.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://lt.wgjwhj.cn

[Q22] 排序
来源：http://jb.huixiangedu.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://pq.jctech888.com.cn

[Q23] 分页
来源：http://ja.huixinmuqiang.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ds.hahajie.cn

[Q24] 去重
来源：http://gv.yuntaijiaju.cn

SELECT DISTINCT city FROM users;
来源：http://rr.szsharing.cn

[Q25] 只取前 N 条
来源：http://tr.yuntaijiaju.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ys.jianghongdianzi.cn

[Q26] 计数
来源：http://qs.hahajie.cn

SELECT COUNT(*) FROM users;
来源：http://lk.szsharing.cn

[Q27] 条件计数
来源：http://gw.nszjky.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://yt.haigaiapp.cn

[Q28] 求和与平均
来源：http://mj.muxihuayi.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://vh.hahajie.cn

[Q29] 最大最小值
来源：http://tk.nszjky.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://kc.newstarts.cn

[Q30] 分组统计
来源：http://gj.jianghongdianzi.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://cm.bjjhwx.cn

[Q31] 分组后过滤
来源：http://ss.nszjky.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://tm.colortex.cn

[Q32] 分组拼接字符串
来源：http://bu.shxzukj.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://rt.521024.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://qw.hnjuh.cn

[Q33] 多列分组
来源：http://nl.szsharing.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ws.huanxung.cn

[Q34] 每组取第一条
来源：http://ej.newstarts.cn

SELECT * FROM (
来源：http://oh.asd995.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hq.jianghongdianzi.cn

) t WHERE rn = 1;
来源：http://al.hahajie.cn

[Q35] 内连接
来源：http://nz.nicolike.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ns.hahajie.cn

[Q36] 左连接
来源：http://pr.haigaiapp.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://vm.nicolike.cn

[Q37] 右连接
来源：http://br.hahajie.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://od.huanxung.cn

[Q38] 全外连接（PostgreSQL）
来源：http://rw.wgjwhj.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://jv.wgjwhj.cn

[Q39] 自连接（查上下级）
来源：http://tr.colortex.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://ke.521024.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://er.muxihuayi.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://mt.bjjhwx.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://qo.huixiangedu.cn

[Q41] 多表连接
来源：http://yg.hahajie.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://gt.hnjuh.cn

JOIN users u ON u.id = o.user_id
来源：http://ax.muxihuayi.cn

JOIN products p ON p.id = o.product_id;
来源：http://to.jctech888.com.cn

[Q42] 连接条件附加过滤
来源：http://yh.bjjhwx.cn

SELECT u.name, o.amount FROM users u
来源：http://ur.shtwfgs.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://go.bjjhwx.cn

[Q43] 标量子查询
来源：http://lk.521024.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://fi.colortex.cn

[Q44] IN 子查询
来源：http://uj.shtwfgs.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://md.haigaiapp.cn

[Q45] EXISTS 判断存在
来源：http://mf.shxzukj.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://cb.yuexingan06.cn

[Q46] NOT EXISTS 判断不存在
来源：http://vn.nszjky.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://kw.chemitech.net.cn

[Q47] 与平均值比较
来源：http://kj.bjjhwx.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://te.shxzukj.cn

[Q48] CTE 公用表表达式
来源：http://ue.shxzukj.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://yn.hahajie.cn

SELECT * FROM t WHERE c > 5;
来源：http://xo.asd995.cn

[Q49] 更新单行
来源：http://bw.nszjky.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://uk.shxzukj.cn

[Q50] 批量更新
来源：http://qa.shtwfgs.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://pl.hnjuh.cn

[Q51] 用子查询更新
来源：http://ka.521024.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://vk.huixinmuqiang.cn

[Q52] 删除指定行
来源：http://ng.nicolike.cn

DELETE FROM users WHERE id = 10;
来源：http://nx.colortex.cn

[Q53] 按条件删除
来源：http://re.asd995.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://gb.shtwfgs.cn

[Q54] 清空表
来源：http://lv.newstarts.cn

TRUNCATE TABLE logs;
来源：http://lw.huixinmuqiang.cn

[Q55] 排名（并列占位）
来源：http://mr.chemitech.net.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ey.chemitech.net.cn

[Q56] 密集排名（并列不占位）
来源：http://uy.nicolike.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hx.nszjky.cn

[Q57] 行号
来源：http://be.haigaiapp.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://my.huixinmuqiang.cn

[Q58] 累计求和
来源：http://sz.muxihuayi.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://md.wgjwhj.cn

[Q59] 分组内累计
来源：http://ew.huixiangedu.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://qp.bjjhwx.cn

[Q60] 取上一行 / 下一行
来源：http://qb.bookmarksfly.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ch.colortex.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://qv.szxytkj.cn

[Q61] 移动平均
来源：http://pu.nicolike.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://kv.lnxyls.cn

[Q62] 分组占比
来源：http://vf.chemitech.net.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://fv.szsharing.cn

[Q63] 开启事务
来源：http://hf.9csxet.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://az.panjiajie.cn

[Q64] 提交事务
来源：http://ew.bookmarksfly.cn

COMMIT;
来源：http://xt.shtwfgs.cn

[Q65] 回滚事务
来源：http://zs.nszjky.cn

ROLLBACK;
来源：http://xf.jianghongdianzi.cn

[Q66] 行锁查询
来源：http://xt.asd995.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://qo.lnxyls.cn

[Q67] 设置隔离级别
来源：http://os.yuexingan06.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://qi.szsharing.cn

[Q68] 保存点
来源：http://fn.muxihuayi.cn

SAVEPOINT sp1;
来源：http://ec.huanxung.cn

ROLLBACK TO sp1;
来源：http://yo.huanxung.cn

[Q69] 查看执行计划
来源：http://yk.asd995.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://cv.huixinmuqiang.cn

[Q70] 更新统计信息
来源：http://lr.shxzskj.cn

ANALYZE TABLE users;
来源：http://jn.muxihuayi.cn

[Q71] 查看建表语句
来源：http://ph.newstarts.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://uu.wgjwhj.cn

[Q72] 查看索引
来源：http://js.nszjky.cn

SHOW INDEX FROM users;
来源：http://ko.jctech888.com.cn

[Q73] 查看表状态
来源：http://xc.muxihuayi.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://ad.muxihuayi.cn

[Q74] 强制使用索引
来源：http://om.bookmarksfly.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ro.9csxet.cn

[Q75] 日期格式化
来源：http://mh.jianghongdianzi.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://uo.yuntaijiaju.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://sx.shxzskj.cn

[Q76] 按天统计
来源：http://bl.nszjky.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://fi.szxytkj.cn

[Q77] 时间加减
来源：http://iy.lnxyls.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ud.nicolike.cn

[Q78] 当前时间
来源：http://zf.szsharing.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mo.shxzukj.cn

[Q79] 字符串拼接
来源：http://zj.asd995.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ow.hnjuh.cn

[Q80] 字符串截取
来源：http://ek.nicolike.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://zu.shtwfgs.cn

[Q81] 字符串替换
来源：http://id.haigaiapp.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://fq.panjiajie.cn

[Q82] 字符长度与字节长度
来源：http://fy.panjiajie.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ch.chemitech.net.cn

[Q83] 大小写转换
来源：http://tx.panjiajie.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://dg.szsharing.cn

[Q84] 去除首尾空格
来源：http://ch.jianghongdianzi.cn

SELECT TRIM(name) FROM users;
来源：http://gy.lnxyls.cn

[Q85] 数值取整
来源：http://uu.lnxyls.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://je.bjjhwx.cn

[Q86] 读取 JSON 字段
来源：http://vt.asd995.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://bc.bookmarksfly.cn

[Q87] JSON 字段做条件
来源：http://gm.huanxung.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://fq.haigaiapp.cn

[Q88] 行转列（条件聚合）
来源：http://mv.chemitech.net.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://pi.jianghongdianzi.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ke.newstarts.cn

[Q89] 判断表是否存在
来源：http://yf.newstarts.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ec.panjiajie.cn

[Q90] 生成序号列
来源：http://tk.shxzukj.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ar.521024.cn

================================================================================
来源：http://gs.szsharing.cn

R. Bash 专题
来源：http://ef.bjjhwx.cn

================================================================================
来源：http://br.chemitech.net.cn

[R01] shebang 与严格模式
来源：http://nj.yuntaijiaju.cn

#!/usr/bin/env bash
来源：http://lf.huixinmuqiang.cn

set -euo pipefail
来源：http://op.shxzskj.cn

[R02] 变量赋值与使用
来源：http://ok.yuntaijiaju.cn

name="Tom"; echo "$name"
来源：http://li.nicolike.cn

[R03] 只读变量
来源：http://uh.wgjwhj.cn

readonly PI=3.14
来源：http://ky.521024.cn

[R04] 位置参数
来源：http://ze.haigaiapp.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://iw.bjjhwx.cn

[R05] 参数默认值
来源：http://kp.nicolike.cn

name="${1:-default}"
来源：http://vs.huixinmuqiang.cn

[R06] 判断命令是否存在
来源：http://lf.nicolike.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hb.bookmarksfly.cn

[R07] if 判断文件
来源：http://ph.gzmigu.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ib.yuexingan06.cn

[R08] 数值比较
来源：http://ea.jctech888.com.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://lv.9csxet.cn

[R09] 字符串比较
来源：http://pm.wgjwhj.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://dc.jianghongdianzi.cn

[R10] 正则匹配
来源：http://ot.huixinmuqiang.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ow.bjjhwx.cn

[R11] case 多分支
来源：http://vv.huixiangedu.cn

case "$1" in
来源：http://oi.panjiajie.cn

start) echo "启动" ;;
来源：http://jr.asd995.cn

stop)  echo "停止" ;;
来源：http://yn.yuntaijiaju.cn

*)     echo "未知命令" ;;
来源：http://wr.9csxet.cn

esac
来源：http://wc.521024.cn

[R12] for 遍历文件
来源：http://yz.asd995.cn

for f in *.txt; do echo "$f"; done
来源：http://jx.hahajie.cn

[R13] for 计数循环
来源：http://du.nicolike.cn

for i in {1..10}; do echo "$i"; done
来源：http://js.szsharing.cn

[R14] C 风格 for
来源：http://jg.szxytkj.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://uo.gzmigu.cn

[R15] while 逐行读文件
来源：http://jk.haigaiapp.cn


<!-- 参考信息 -->