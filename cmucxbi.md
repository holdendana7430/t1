代发 wailian999

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hy.shxzukj.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://bw.newstarts.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://bf.9csxet.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ii.colortex.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://nb.huanxung.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://rf.huanxung.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://gl.szxytkj.cn

[P04] 求长度
来源：http://yd.huanxung.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://qr.haigaiapp.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://xk.szxytkj.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mr.muxihuayi.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ry.nszjky.cn

Java: list.size();  map.size();  s.length()
来源：http://dh.haigaiapp.cn

Go:   len(arr);  len(m)
来源：http://nm.jctech888.com.cn

Ruby: x.length;  x.size
来源：http://aa.yuexingan06.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://cj.asd995.cn

[P05] 判断两个对象内容是否相等
来源：http://ji.wgjwhj.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://ui.chemitech.net.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://cr.huanxung.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://cg.haigaiapp.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ur.yuntaijiaju.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://di.hahajie.cn

Go:   reflect.DeepEqual(a, b)
来源：http://wh.9csxet.cn

Ruby: a == b
来源：http://yh.szxytkj.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://og.szsharing.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hn.wgjwhj.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://gj.521024.cn

PHP:  if (empty($x)) {}
来源：http://ch.jianghongdianzi.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://uc.szsharing.cn

TS:   if (x == null) {}
来源：http://us.huixiangedu.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://fn.nicolike.cn

Go:   if x == nil {}
来源：http://ub.muxihuayi.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://lt.asd995.cn

C#:   if (x is null) {}
来源：http://qm.chemitech.net.cn

[P07] 防抖与节流
来源：http://en.shxzukj.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://of.wgjwhj.cn

PHP:  // 手写时间戳比较
来源：http://hc.panjiajie.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://sz.muxihuayi.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xz.colortex.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://so.jctech888.com.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://nw.521024.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://pu.jianghongdianzi.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://vb.yuexingan06.cn

[P08] 处理浮点精度问题
来源：http://jg.panjiajie.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://sv.bjjhwx.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://az.szxytkj.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://tx.huixiangedu.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wx.muxihuayi.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://sf.nszjky.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://vd.colortex.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://tb.521024.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://gg.shxzskj.cn

================================================================================
来源：http://ic.bjjhwx.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://jx.shxzukj.cn

================================================================================
来源：http://to.panjiajie.cn

[Q01] 创建表
来源：http://td.colortex.cn

CREATE TABLE users (
来源：http://vl.muxihuayi.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mj.muxihuayi.cn

name VARCHAR(50) NOT NULL,
来源：http://na.muxihuayi.cn

email VARCHAR(100) UNIQUE,
来源：http://gj.hnjuh.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://le.colortex.cn

);
来源：http://vm.gzmigu.cn

[Q02] 创建带外键的表
来源：http://br.jianghongdianzi.cn

CREATE TABLE orders (
来源：http://oj.shtwfgs.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://kd.shtwfgs.cn

user_id INT NOT NULL,
来源：http://yd.panjiajie.cn

amount DECIMAL(10, 2),
来源：http://ss.huanxung.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://pu.huanxung.cn

);
来源：http://wd.9csxet.cn

[Q03] 增加列
来源：http://wc.shxzukj.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://oh.colortex.cn

[Q04] 修改列类型
来源：http://ht.panjiajie.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://nc.yuntaijiaju.cn

[Q05] 重命名列
来源：http://kk.lnxyls.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://dp.bookmarksfly.cn

[Q06] 删除列
来源：http://wp.gzmigu.cn

ALTER TABLE users DROP COLUMN age;
来源：http://qa.jctech888.com.cn

[Q07] 删除表
来源：http://co.asd995.cn

DROP TABLE IF EXISTS orders;
来源：http://ko.nicolike.cn

[Q08] 创建普通索引
来源：http://lr.bjjhwx.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://fy.colortex.cn

[Q09] 创建唯一索引
来源：http://np.wgjwhj.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mp.newstarts.cn

[Q10] 插入单行
来源：http://dh.asd995.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://dp.huixinmuqiang.cn

[Q11] 一次插入多行
来源：http://vq.hnjuh.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://qz.haigaiapp.cn

[Q12] 插入后取自增 ID
来源：http://qn.wgjwhj.cn

INSERT INTO users (name) VALUES ('C');
来源：http://cv.huanxung.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ja.colortex.cn

[Q13] 忽略重复插入
来源：http://py.gzmigu.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://gj.jctech888.com.cn

[Q14] 存在则更新（upsert）
来源：http://jw.szsharing.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://tm.shxzskj.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://lq.szxytkj.cn

[Q15] 查询全部
来源：http://jl.szxytkj.cn

SELECT * FROM users;
来源：http://th.huixiangedu.cn

[Q16] 查询指定列
来源：http://bc.jctech888.com.cn

SELECT id, name FROM users;
来源：http://rz.gzmigu.cn

[Q17] 条件查询
来源：http://xs.hnjuh.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ka.huanxung.cn

[Q18] 模糊匹配
来源：http://cf.huanxung.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://fr.panjiajie.cn

[Q19] 范围查询
来源：http://oc.hnjuh.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://bv.wgjwhj.cn

[Q20] IN 列表
来源：http://eu.shxzukj.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ju.asd995.cn

[Q21] 空值判断
来源：http://re.lnxyls.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://le.huixinmuqiang.cn

[Q22] 排序
来源：http://ip.muxihuayi.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://es.newstarts.cn

[Q23] 分页
来源：http://sh.yuntaijiaju.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ea.szsharing.cn

[Q24] 去重
来源：http://xn.hnjuh.cn

SELECT DISTINCT city FROM users;
来源：http://mj.huixinmuqiang.cn

[Q25] 只取前 N 条
来源：http://ko.huixinmuqiang.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://xv.huixiangedu.cn

[Q26] 计数
来源：http://mc.muxihuayi.cn

SELECT COUNT(*) FROM users;
来源：http://wd.panjiajie.cn

[Q27] 条件计数
来源：http://vl.asd995.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://vn.yuexingan06.cn

[Q28] 求和与平均
来源：http://yt.9csxet.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://gc.muxihuayi.cn

[Q29] 最大最小值
来源：http://fp.nicolike.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://rv.chemitech.net.cn

[Q30] 分组统计
来源：http://cy.huanxung.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wh.bjjhwx.cn

[Q31] 分组后过滤
来源：http://fs.colortex.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ti.huixinmuqiang.cn

[Q32] 分组拼接字符串
来源：http://yb.shxzukj.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wu.hnjuh.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://km.yuexingan06.cn

[Q33] 多列分组
来源：http://oj.panjiajie.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://gk.haigaiapp.cn

[Q34] 每组取第一条
来源：http://ji.muxihuayi.cn

SELECT * FROM (
来源：http://yo.asd995.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ee.jianghongdianzi.cn

) t WHERE rn = 1;
来源：http://wz.shxzukj.cn

[Q35] 内连接
来源：http://tu.muxihuayi.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ca.lnxyls.cn

[Q36] 左连接
来源：http://tm.colortex.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://yk.nszjky.cn

[Q37] 右连接
来源：http://ld.jctech888.com.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://is.521024.cn

[Q38] 全外连接（PostgreSQL）
来源：http://yu.lnxyls.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://rl.huixiangedu.cn

[Q39] 自连接（查上下级）
来源：http://ce.hnjuh.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://ca.szsharing.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://rd.nicolike.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://gv.panjiajie.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://vl.jianghongdianzi.cn

[Q41] 多表连接
来源：http://zn.hahajie.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://gz.hahajie.cn

JOIN users u ON u.id = o.user_id
来源：http://yb.haigaiapp.cn

JOIN products p ON p.id = o.product_id;
来源：http://xm.521024.cn

[Q42] 连接条件附加过滤
来源：http://uj.szsharing.cn

SELECT u.name, o.amount FROM users u
来源：http://yo.huixiangedu.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ki.nicolike.cn

[Q43] 标量子查询
来源：http://cr.szsharing.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://at.haigaiapp.cn

[Q44] IN 子查询
来源：http://un.wgjwhj.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://is.yuexingan06.cn

[Q45] EXISTS 判断存在
来源：http://yn.shtwfgs.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://pg.yuexingan06.cn

[Q46] NOT EXISTS 判断不存在
来源：http://eu.521024.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://lm.jctech888.com.cn

[Q47] 与平均值比较
来源：http://yd.nicolike.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ef.yuexingan06.cn

[Q48] CTE 公用表表达式
来源：http://ze.huanxung.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://so.wgjwhj.cn

SELECT * FROM t WHERE c > 5;
来源：http://om.haigaiapp.cn

[Q49] 更新单行
来源：http://vg.nicolike.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://xf.szxytkj.cn

[Q50] 批量更新
来源：http://un.yuntaijiaju.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://yz.nszjky.cn

[Q51] 用子查询更新
来源：http://ky.9csxet.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://zs.chemitech.net.cn

[Q52] 删除指定行
来源：http://bz.bjjhwx.cn

DELETE FROM users WHERE id = 10;
来源：http://vk.wgjwhj.cn

[Q53] 按条件删除
来源：http://jd.huixinmuqiang.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://xr.bjjhwx.cn

[Q54] 清空表
来源：http://si.szsharing.cn

TRUNCATE TABLE logs;
来源：http://ej.colortex.cn

[Q55] 排名（并列占位）
来源：http://ns.szxytkj.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mr.huixinmuqiang.cn

[Q56] 密集排名（并列不占位）
来源：http://lt.haigaiapp.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://oc.jianghongdianzi.cn

[Q57] 行号
来源：http://mw.huixiangedu.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wh.chemitech.net.cn

[Q58] 累计求和
来源：http://ma.shtwfgs.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://gp.colortex.cn

[Q59] 分组内累计
来源：http://ra.shxzukj.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://id.wgjwhj.cn

[Q60] 取上一行 / 下一行
来源：http://mx.shxzukj.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ez.colortex.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://cr.gzmigu.cn

[Q61] 移动平均
来源：http://bs.hnjuh.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://iy.wgjwhj.cn

[Q62] 分组占比
来源：http://id.hahajie.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ta.panjiajie.cn

[Q63] 开启事务
来源：http://fw.chemitech.net.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://wi.yuntaijiaju.cn

[Q64] 提交事务
来源：http://te.jianghongdianzi.cn

COMMIT;
来源：http://jv.gzmigu.cn

[Q65] 回滚事务
来源：http://yf.hnjuh.cn

ROLLBACK;
来源：http://ar.bookmarksfly.cn

[Q66] 行锁查询
来源：http://gr.shtwfgs.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ic.haigaiapp.cn

[Q67] 设置隔离级别
来源：http://iu.shxzskj.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://kr.hahajie.cn

[Q68] 保存点
来源：http://nz.nicolike.cn

SAVEPOINT sp1;
来源：http://bp.yuntaijiaju.cn

ROLLBACK TO sp1;
来源：http://ll.hnjuh.cn

[Q69] 查看执行计划
来源：http://qt.asd995.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://so.asd995.cn

[Q70] 更新统计信息
来源：http://uf.muxihuayi.cn

ANALYZE TABLE users;
来源：http://vp.szsharing.cn

[Q71] 查看建表语句
来源：http://fx.panjiajie.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mi.nszjky.cn

[Q72] 查看索引
来源：http://el.szsharing.cn

SHOW INDEX FROM users;
来源：http://nv.muxihuayi.cn

[Q73] 查看表状态
来源：http://br.hnjuh.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://wp.lnxyls.cn

[Q74] 强制使用索引
来源：http://no.huanxung.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://vx.hahajie.cn

[Q75] 日期格式化
来源：http://ky.nicolike.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://lu.panjiajie.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://au.hahajie.cn

[Q76] 按天统计
来源：http://rl.9csxet.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://jz.wgjwhj.cn

[Q77] 时间加减
来源：http://re.bookmarksfly.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://yd.huixiangedu.cn

[Q78] 当前时间
来源：http://uy.lnxyls.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://xe.szxytkj.cn

[Q79] 字符串拼接
来源：http://ul.9csxet.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://gr.jctech888.com.cn

[Q80] 字符串截取
来源：http://be.newstarts.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://az.shtwfgs.cn

[Q81] 字符串替换
来源：http://iw.521024.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://bz.9csxet.cn

[Q82] 字符长度与字节长度
来源：http://kr.shxzskj.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://bx.bjjhwx.cn

[Q83] 大小写转换
来源：http://fp.huixiangedu.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://fv.lnxyls.cn

[Q84] 去除首尾空格
来源：http://up.9csxet.cn

SELECT TRIM(name) FROM users;
来源：http://ns.hnjuh.cn

[Q85] 数值取整
来源：http://vy.nicolike.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://cn.szxytkj.cn

[Q86] 读取 JSON 字段
来源：http://ss.bjjhwx.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ee.muxihuayi.cn

[Q87] JSON 字段做条件
来源：http://hu.521024.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ut.gzmigu.cn

[Q88] 行转列（条件聚合）
来源：http://dg.shxzskj.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://qj.jianghongdianzi.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://us.hnjuh.cn

[Q89] 判断表是否存在
来源：http://vm.shxzskj.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://pe.panjiajie.cn

[Q90] 生成序号列
来源：http://kb.colortex.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://rr.hnjuh.cn

================================================================================
来源：http://vu.jctech888.com.cn

R. Bash 专题
来源：http://dc.hnjuh.cn

================================================================================
来源：http://xq.nszjky.cn

[R01] shebang 与严格模式
来源：http://kj.huanxung.cn

#!/usr/bin/env bash
来源：http://jb.panjiajie.cn

set -euo pipefail
来源：http://ws.huixinmuqiang.cn

[R02] 变量赋值与使用
来源：http://pv.shxzukj.cn

name="Tom"; echo "$name"
来源：http://jz.gzmigu.cn

[R03] 只读变量
来源：http://wk.wgjwhj.cn

readonly PI=3.14
来源：http://bt.hnjuh.cn

[R04] 位置参数
来源：http://cr.hahajie.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ug.bjjhwx.cn

[R05] 参数默认值
来源：http://ns.jianghongdianzi.cn

name="${1:-default}"
来源：http://qb.huixinmuqiang.cn

[R06] 判断命令是否存在
来源：http://yl.lnxyls.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wn.hahajie.cn

[R07] if 判断文件
来源：http://hm.gzmigu.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://fp.521024.cn

[R08] 数值比较
来源：http://ur.wgjwhj.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://sa.bjjhwx.cn

[R09] 字符串比较
来源：http://zj.chemitech.net.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://tb.haigaiapp.cn

[R10] 正则匹配
来源：http://zo.wgjwhj.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ev.9csxet.cn

[R11] case 多分支
来源：http://xx.wgjwhj.cn

case "$1" in
来源：http://nh.shtwfgs.cn

start) echo "启动" ;;
来源：http://ci.shtwfgs.cn

stop)  echo "停止" ;;
来源：http://zf.haigaiapp.cn

*)     echo "未知命令" ;;
来源：http://of.huixinmuqiang.cn

esac
来源：http://gp.huanxung.cn

[R12] for 遍历文件
来源：http://jc.shxzskj.cn

for f in *.txt; do echo "$f"; done
来源：http://xe.bookmarksfly.cn

[R13] for 计数循环
来源：http://pt.asd995.cn

for i in {1..10}; do echo "$i"; done
来源：http://gu.bookmarksfly.cn

[R14] C 风格 for
来源：http://wm.huixiangedu.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://za.haigaiapp.cn

[R15] while 逐行读文件
来源：http://oi.huixinmuqiang.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ef.shxzukj.cn

[R16] until 等待条件
来源：http://hc.jianghongdianzi.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://vy.shxzskj.cn

[R17] 数组定义与取值
来源：http://hg.yuexingan06.cn


<!-- 参考信息 -->