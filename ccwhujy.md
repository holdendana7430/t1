代发 wailian999

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://yi.gzmigu.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://vz.gzmigu.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ax.newstarts.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://zi.asd995.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hy.nicolike.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://cb.bookmarksfly.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://fo.hahajie.cn

[P04] 求长度
来源：http://rw.yuntaijiaju.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://kc.asd995.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ae.hnjuh.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://iq.huixiangedu.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://xg.jianghongdianzi.cn

Java: list.size();  map.size();  s.length()
来源：http://xl.szxytkj.cn

Go:   len(arr);  len(m)
来源：http://cl.nszjky.cn

Ruby: x.length;  x.size
来源：http://cj.bookmarksfly.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://sq.haigaiapp.cn

[P05] 判断两个对象内容是否相等
来源：http://uc.lnxyls.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://hj.asd995.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://gn.jianghongdianzi.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://fw.muxihuayi.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://vp.521024.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://gu.huanxung.cn

Go:   reflect.DeepEqual(a, b)
来源：http://ij.hnjuh.cn

Ruby: a == b
来源：http://xe.chemitech.net.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ph.shxzskj.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://vn.hahajie.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://xz.jianghongdianzi.cn

PHP:  if (empty($x)) {}
来源：http://ty.bookmarksfly.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://cc.huanxung.cn

TS:   if (x == null) {}
来源：http://jl.lnxyls.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://so.szsharing.cn

Go:   if x == nil {}
来源：http://vp.muxihuayi.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ov.chemitech.net.cn

C#:   if (x is null) {}
来源：http://pn.muxihuayi.cn

[P07] 防抖与节流
来源：http://sv.panjiajie.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ar.chemitech.net.cn

PHP:  // 手写时间戳比较
来源：http://zg.gzmigu.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ce.hahajie.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ah.haigaiapp.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://kq.huanxung.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://xk.9csxet.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://qz.szsharing.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://nr.chemitech.net.cn

[P08] 处理浮点精度问题
来源：http://yd.panjiajie.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ps.szsharing.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://od.szxytkj.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://sm.wgjwhj.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://dz.bookmarksfly.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://jv.bookmarksfly.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://xj.bookmarksfly.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ak.newstarts.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://bx.huixiangedu.cn

================================================================================
来源：http://ss.hnjuh.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://yw.yuexingan06.cn

================================================================================
来源：http://sm.nicolike.cn

[Q01] 创建表
来源：http://ga.szsharing.cn

CREATE TABLE users (
来源：http://zb.huanxung.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://se.huanxung.cn

name VARCHAR(50) NOT NULL,
来源：http://vx.9csxet.cn

email VARCHAR(100) UNIQUE,
来源：http://ip.wgjwhj.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://kh.521024.cn

);
来源：http://gz.shxzskj.cn

[Q02] 创建带外键的表
来源：http://rn.huixinmuqiang.cn

CREATE TABLE orders (
来源：http://cs.colortex.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ns.chemitech.net.cn

user_id INT NOT NULL,
来源：http://fw.wgjwhj.cn

amount DECIMAL(10, 2),
来源：http://qq.bjjhwx.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://dx.muxihuayi.cn

);
来源：http://oo.shxzukj.cn

[Q03] 增加列
来源：http://iw.lnxyls.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://tx.panjiajie.cn

[Q04] 修改列类型
来源：http://rz.jianghongdianzi.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://oq.yuntaijiaju.cn

[Q05] 重命名列
来源：http://tq.huixiangedu.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://lv.yuexingan06.cn

[Q06] 删除列
来源：http://zf.bjjhwx.cn

ALTER TABLE users DROP COLUMN age;
来源：http://pj.jianghongdianzi.cn

[Q07] 删除表
来源：http://co.yuntaijiaju.cn

DROP TABLE IF EXISTS orders;
来源：http://lj.panjiajie.cn

[Q08] 创建普通索引
来源：http://ao.jctech888.com.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://xb.wgjwhj.cn

[Q09] 创建唯一索引
来源：http://ss.muxihuayi.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://vs.szsharing.cn

[Q10] 插入单行
来源：http://lo.521024.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://oq.jianghongdianzi.cn

[Q11] 一次插入多行
来源：http://hp.chemitech.net.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://vl.yuexingan06.cn

[Q12] 插入后取自增 ID
来源：http://sg.jctech888.com.cn

INSERT INTO users (name) VALUES ('C');
来源：http://bb.szsharing.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://zd.huixinmuqiang.cn

[Q13] 忽略重复插入
来源：http://me.wgjwhj.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://uh.huixiangedu.cn

[Q14] 存在则更新（upsert）
来源：http://yh.nszjky.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ti.bookmarksfly.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://zy.huixiangedu.cn

[Q15] 查询全部
来源：http://dw.newstarts.cn

SELECT * FROM users;
来源：http://cf.hahajie.cn

[Q16] 查询指定列
来源：http://vx.huixiangedu.cn

SELECT id, name FROM users;
来源：http://uu.gzmigu.cn

[Q17] 条件查询
来源：http://rj.jctech888.com.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ux.hnjuh.cn

[Q18] 模糊匹配
来源：http://os.asd995.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://lo.lnxyls.cn

[Q19] 范围查询
来源：http://jc.jianghongdianzi.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://vr.wgjwhj.cn

[Q20] IN 列表
来源：http://tb.newstarts.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://jm.chemitech.net.cn

[Q21] 空值判断
来源：http://at.9csxet.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://ey.jianghongdianzi.cn

[Q22] 排序
来源：http://sz.hahajie.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://lu.hahajie.cn

[Q23] 分页
来源：http://lu.gzmigu.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://df.hnjuh.cn

[Q24] 去重
来源：http://ak.chemitech.net.cn

SELECT DISTINCT city FROM users;
来源：http://hd.hahajie.cn

[Q25] 只取前 N 条
来源：http://yf.bjjhwx.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://xz.lnxyls.cn

[Q26] 计数
来源：http://gs.bjjhwx.cn

SELECT COUNT(*) FROM users;
来源：http://gh.panjiajie.cn

[Q27] 条件计数
来源：http://jo.huixiangedu.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://pz.jianghongdianzi.cn

[Q28] 求和与平均
来源：http://xe.jianghongdianzi.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://rk.jianghongdianzi.cn

[Q29] 最大最小值
来源：http://jx.panjiajie.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://pr.shtwfgs.cn

[Q30] 分组统计
来源：http://px.nicolike.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://uw.bookmarksfly.cn

[Q31] 分组后过滤
来源：http://ct.shtwfgs.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://my.szsharing.cn

[Q32] 分组拼接字符串
来源：http://ej.nicolike.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://bk.hahajie.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://jl.jctech888.com.cn

[Q33] 多列分组
来源：http://sn.521024.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mp.shxzskj.cn

[Q34] 每组取第一条
来源：http://fu.asd995.cn

SELECT * FROM (
来源：http://cz.haigaiapp.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://lj.jctech888.com.cn

) t WHERE rn = 1;
来源：http://wr.bjjhwx.cn

[Q35] 内连接
来源：http://tr.panjiajie.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://br.huixiangedu.cn

[Q36] 左连接
来源：http://sh.huanxung.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://dy.newstarts.cn

[Q37] 右连接
来源：http://ai.jianghongdianzi.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://jx.huanxung.cn

[Q38] 全外连接（PostgreSQL）
来源：http://gp.wgjwhj.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://si.wgjwhj.cn

[Q39] 自连接（查上下级）
来源：http://zr.hahajie.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://be.bjjhwx.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://fp.huixiangedu.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://pz.chemitech.net.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ha.wgjwhj.cn

[Q41] 多表连接
来源：http://xo.haigaiapp.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://ho.bjjhwx.cn

JOIN users u ON u.id = o.user_id
来源：http://gd.shtwfgs.cn

JOIN products p ON p.id = o.product_id;
来源：http://gz.shtwfgs.cn

[Q42] 连接条件附加过滤
来源：http://rp.lnxyls.cn

SELECT u.name, o.amount FROM users u
来源：http://dt.huanxung.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://xt.521024.cn

[Q43] 标量子查询
来源：http://uh.bookmarksfly.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://yz.shxzukj.cn

[Q44] IN 子查询
来源：http://wm.muxihuayi.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://nr.muxihuayi.cn

[Q45] EXISTS 判断存在
来源：http://lo.gzmigu.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://lp.huixiangedu.cn

[Q46] NOT EXISTS 判断不存在
来源：http://mk.9csxet.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wv.gzmigu.cn

[Q47] 与平均值比较
来源：http://qt.bjjhwx.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://lh.wgjwhj.cn

[Q48] CTE 公用表表达式
来源：http://up.muxihuayi.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://lw.jianghongdianzi.cn

SELECT * FROM t WHERE c > 5;
来源：http://kx.9csxet.cn

[Q49] 更新单行
来源：http://gt.shxzukj.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ut.hnjuh.cn

[Q50] 批量更新
来源：http://tl.bjjhwx.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://zc.chemitech.net.cn

[Q51] 用子查询更新
来源：http://bl.yuexingan06.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://au.huixiangedu.cn

[Q52] 删除指定行
来源：http://hp.bjjhwx.cn

DELETE FROM users WHERE id = 10;
来源：http://tq.bookmarksfly.cn

[Q53] 按条件删除
来源：http://go.hnjuh.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://gf.szxytkj.cn

[Q54] 清空表
来源：http://lj.lnxyls.cn

TRUNCATE TABLE logs;
来源：http://vt.jianghongdianzi.cn

[Q55] 排名（并列占位）
来源：http://bs.shtwfgs.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://xj.bookmarksfly.cn

[Q56] 密集排名（并列不占位）
来源：http://yl.yuexingan06.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ts.nicolike.cn

[Q57] 行号
来源：http://hu.bookmarksfly.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ln.jianghongdianzi.cn

[Q58] 累计求和
来源：http://xc.hnjuh.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ra.bjjhwx.cn

[Q59] 分组内累计
来源：http://yu.9csxet.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://cw.huixinmuqiang.cn

[Q60] 取上一行 / 下一行
来源：http://hd.szsharing.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://yq.lnxyls.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hg.lnxyls.cn

[Q61] 移动平均
来源：http://iy.521024.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://jr.asd995.cn

[Q62] 分组占比
来源：http://fv.yuexingan06.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://zh.newstarts.cn

[Q63] 开启事务
来源：http://wp.bjjhwx.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://ot.lnxyls.cn

[Q64] 提交事务
来源：http://qe.shtwfgs.cn

COMMIT;
来源：http://xa.lnxyls.cn

[Q65] 回滚事务
来源：http://yk.shxzukj.cn

ROLLBACK;
来源：http://uh.shxzskj.cn

[Q66] 行锁查询
来源：http://ha.jctech888.com.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.newstarts.cn

[Q67] 设置隔离级别
来源：http://ny.9csxet.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://fu.jctech888.com.cn

[Q68] 保存点
来源：http://io.haigaiapp.cn

SAVEPOINT sp1;
来源：http://ju.colortex.cn

ROLLBACK TO sp1;
来源：http://qs.panjiajie.cn

[Q69] 查看执行计划
来源：http://wq.huanxung.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mv.haigaiapp.cn

[Q70] 更新统计信息
来源：http://xk.bjjhwx.cn

ANALYZE TABLE users;
来源：http://vc.bookmarksfly.cn

[Q71] 查看建表语句
来源：http://dy.newstarts.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hr.colortex.cn

[Q72] 查看索引
来源：http://ei.shxzskj.cn

SHOW INDEX FROM users;
来源：http://fh.asd995.cn

[Q73] 查看表状态
来源：http://nb.szsharing.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://lk.huixinmuqiang.cn

[Q74] 强制使用索引
来源：http://yn.jianghongdianzi.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://if.shxzskj.cn

[Q75] 日期格式化
来源：http://jn.521024.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://du.shtwfgs.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://vo.szxytkj.cn

[Q76] 按天统计
来源：http://pv.huixiangedu.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ac.colortex.cn

[Q77] 时间加减
来源：http://yf.9csxet.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://db.newstarts.cn

[Q78] 当前时间
来源：http://ad.asd995.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://rm.bookmarksfly.cn

[Q79] 字符串拼接
来源：http://pw.szxytkj.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://jj.lnxyls.cn

[Q80] 字符串截取
来源：http://sk.wgjwhj.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ic.wgjwhj.cn

[Q81] 字符串替换
来源：http://ik.gzmigu.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://te.jctech888.com.cn

[Q82] 字符长度与字节长度
来源：http://dl.shxzskj.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://py.huixiangedu.cn

[Q83] 大小写转换
来源：http://uj.newstarts.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ul.szxytkj.cn

[Q84] 去除首尾空格
来源：http://wu.nszjky.cn

SELECT TRIM(name) FROM users;
来源：http://ms.colortex.cn

[Q85] 数值取整
来源：http://if.bjjhwx.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wr.shtwfgs.cn

[Q86] 读取 JSON 字段
来源：http://hc.hahajie.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ke.wgjwhj.cn

[Q87] JSON 字段做条件
来源：http://xl.jianghongdianzi.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://gd.jianghongdianzi.cn

[Q88] 行转列（条件聚合）
来源：http://ng.hnjuh.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://if.shxzukj.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://tx.jctech888.com.cn

[Q89] 判断表是否存在
来源：http://lu.shxzukj.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://br.asd995.cn

[Q90] 生成序号列
来源：http://tf.huanxung.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://gc.huixiangedu.cn

================================================================================
来源：http://fb.huanxung.cn

R. Bash 专题
来源：http://mg.szxytkj.cn

================================================================================
来源：http://ti.szsharing.cn

[R01] shebang 与严格模式
来源：http://zb.521024.cn

#!/usr/bin/env bash
来源：http://he.shxzukj.cn

set -euo pipefail
来源：http://sl.szsharing.cn

[R02] 变量赋值与使用
来源：http://uw.jctech888.com.cn

name="Tom"; echo "$name"
来源：http://fh.yuntaijiaju.cn

[R03] 只读变量
来源：http://jq.colortex.cn

readonly PI=3.14
来源：http://qd.shxzskj.cn

[R04] 位置参数
来源：http://gy.wgjwhj.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://uo.bookmarksfly.cn

[R05] 参数默认值
来源：http://ka.jianghongdianzi.cn

name="${1:-default}"
来源：http://wq.chemitech.net.cn

[R06] 判断命令是否存在
来源：http://ue.huixinmuqiang.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://sq.shtwfgs.cn

[R07] if 判断文件
来源：http://dm.nicolike.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://to.colortex.cn

[R08] 数值比较
来源：http://ty.hnjuh.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://bk.colortex.cn

[R09] 字符串比较
来源：http://rq.panjiajie.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://uo.jianghongdianzi.cn

[R10] 正则匹配
来源：http://sm.bjjhwx.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wc.newstarts.cn

[R11] case 多分支
来源：http://fy.hnjuh.cn

case "$1" in
来源：http://dh.huixiangedu.cn

start) echo "启动" ;;
来源：http://qx.yuntaijiaju.cn

stop)  echo "停止" ;;
来源：http://sf.shxzukj.cn

*)     echo "未知命令" ;;
来源：http://ku.szxytkj.cn

esac
来源：http://ae.yuntaijiaju.cn

[R12] for 遍历文件
来源：http://tv.bookmarksfly.cn

for f in *.txt; do echo "$f"; done
来源：http://fj.huixiangedu.cn

[R13] for 计数循环
来源：http://je.huixiangedu.cn

for i in {1..10}; do echo "$i"; done
来源：http://ax.gzmigu.cn

[R14] C 风格 for
来源：http://av.szsharing.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://le.panjiajie.cn

[R15] while 逐行读文件
来源：http://vf.shtwfgs.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://kx.wgjwhj.cn

[R16] until 等待条件
来源：http://zd.chemitech.net.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://yg.haigaiapp.cn

[R17] 数组定义与取值
来源：http://mg.nszjky.cn


<!-- 参考信息 -->