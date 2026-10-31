代发 wailian999

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wt.bookmarksfly.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://jh.muxihuayi.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://vp.yuntaijiaju.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ms.shxzukj.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://yt.nszjky.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://np.szsharing.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ng.szsharing.cn

[P04] 求长度
来源：http://iv.szsharing.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://eh.hahajie.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ar.panjiajie.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://yq.nicolike.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://vm.panjiajie.cn

Java: list.size();  map.size();  s.length()
来源：http://wc.szsharing.cn

Go:   len(arr);  len(m)
来源：http://lg.asd995.cn

Ruby: x.length;  x.size
来源：http://hp.hnjuh.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://ws.huixinmuqiang.cn

[P05] 判断两个对象内容是否相等
来源：http://rt.521024.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://hl.wgjwhj.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ij.asd995.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://jy.haigaiapp.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ft.colortex.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://xs.jianghongdianzi.cn

Go:   reflect.DeepEqual(a, b)
来源：http://cx.lnxyls.cn

Ruby: a == b
来源：http://ii.521024.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://bb.hahajie.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://an.shxzskj.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://cz.haigaiapp.cn

PHP:  if (empty($x)) {}
来源：http://vw.bookmarksfly.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ck.newstarts.cn

TS:   if (x == null) {}
来源：http://pn.asd995.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://jp.shxzukj.cn

Go:   if x == nil {}
来源：http://yl.muxihuayi.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://bs.yuntaijiaju.cn

C#:   if (x is null) {}
来源：http://mt.asd995.cn

[P07] 防抖与节流
来源：http://vy.chemitech.net.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://bd.szxytkj.cn

PHP:  // 手写时间戳比较
来源：http://tq.nicolike.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qw.muxihuayi.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://bu.yuntaijiaju.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://bv.gzmigu.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://bc.lnxyls.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://oe.bookmarksfly.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://fh.colortex.cn

[P08] 处理浮点精度问题
来源：http://es.9csxet.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://cm.bookmarksfly.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ag.nszjky.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://fv.szxytkj.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://uc.asd995.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://zi.huixiangedu.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://yt.huixiangedu.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://yw.gzmigu.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://tb.panjiajie.cn

================================================================================
来源：http://dq.bjjhwx.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ek.nicolike.cn

================================================================================
来源：http://tl.521024.cn

[Q01] 创建表
来源：http://ui.shxzukj.cn

CREATE TABLE users (
来源：http://lc.9csxet.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://lz.chemitech.net.cn

name VARCHAR(50) NOT NULL,
来源：http://px.jctech888.com.cn

email VARCHAR(100) UNIQUE,
来源：http://eh.9csxet.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ds.huanxung.cn

);
来源：http://ou.asd995.cn

[Q02] 创建带外键的表
来源：http://ks.newstarts.cn

CREATE TABLE orders (
来源：http://wd.9csxet.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://rt.bjjhwx.cn

user_id INT NOT NULL,
来源：http://sv.bookmarksfly.cn

amount DECIMAL(10, 2),
来源：http://cr.shxzukj.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://yh.yuexingan06.cn

);
来源：http://qm.shtwfgs.cn

[Q03] 增加列
来源：http://ij.nszjky.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://px.hahajie.cn

[Q04] 修改列类型
来源：http://ry.jianghongdianzi.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://si.huanxung.cn

[Q05] 重命名列
来源：http://sr.huanxung.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://fv.panjiajie.cn

[Q06] 删除列
来源：http://jg.jctech888.com.cn

ALTER TABLE users DROP COLUMN age;
来源：http://yf.huixinmuqiang.cn

[Q07] 删除表
来源：http://lu.szsharing.cn

DROP TABLE IF EXISTS orders;
来源：http://fq.9csxet.cn

[Q08] 创建普通索引
来源：http://ft.jctech888.com.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://za.muxihuayi.cn

[Q09] 创建唯一索引
来源：http://gy.shtwfgs.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hy.lnxyls.cn

[Q10] 插入单行
来源：http://og.szsharing.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://zq.hahajie.cn

[Q11] 一次插入多行
来源：http://zu.shxzskj.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://dv.newstarts.cn

[Q12] 插入后取自增 ID
来源：http://bg.muxihuayi.cn

INSERT INTO users (name) VALUES ('C');
来源：http://ae.huanxung.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://lw.yuntaijiaju.cn

[Q13] 忽略重复插入
来源：http://tg.asd995.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ib.muxihuayi.cn

[Q14] 存在则更新（upsert）
来源：http://ki.lnxyls.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wj.haigaiapp.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ll.colortex.cn

[Q15] 查询全部
来源：http://cq.hnjuh.cn

SELECT * FROM users;
来源：http://lz.9csxet.cn

[Q16] 查询指定列
来源：http://dq.9csxet.cn

SELECT id, name FROM users;
来源：http://hb.nicolike.cn

[Q17] 条件查询
来源：http://pu.asd995.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://zq.521024.cn

[Q18] 模糊匹配
来源：http://jm.muxihuayi.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://pp.huixiangedu.cn

[Q19] 范围查询
来源：http://kb.huanxung.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://po.shxzskj.cn

[Q20] IN 列表
来源：http://zb.haigaiapp.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ok.wgjwhj.cn

[Q21] 空值判断
来源：http://zy.yuntaijiaju.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://tx.nicolike.cn

[Q22] 排序
来源：http://us.muxihuayi.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://kp.asd995.cn

[Q23] 分页
来源：http://ww.muxihuayi.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://nx.bookmarksfly.cn

[Q24] 去重
来源：http://sv.jianghongdianzi.cn

SELECT DISTINCT city FROM users;
来源：http://he.9csxet.cn

[Q25] 只取前 N 条
来源：http://ae.asd995.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://la.9csxet.cn

[Q26] 计数
来源：http://zu.hahajie.cn

SELECT COUNT(*) FROM users;
来源：http://iz.asd995.cn

[Q27] 条件计数
来源：http://rm.shxzskj.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://kj.szsharing.cn

[Q28] 求和与平均
来源：http://xd.muxihuayi.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://pd.nszjky.cn

[Q29] 最大最小值
来源：http://au.shxzskj.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://jl.yuntaijiaju.cn

[Q30] 分组统计
来源：http://kt.hahajie.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ke.jianghongdianzi.cn

[Q31] 分组后过滤
来源：http://jq.szxytkj.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hb.huanxung.cn

[Q32] 分组拼接字符串
来源：http://ax.yuntaijiaju.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://pf.yuntaijiaju.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ga.9csxet.cn

[Q33] 多列分组
来源：http://dr.huixinmuqiang.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://yp.521024.cn

[Q34] 每组取第一条
来源：http://jc.shxzukj.cn

SELECT * FROM (
来源：http://fr.haigaiapp.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://bq.muxihuayi.cn

) t WHERE rn = 1;
来源：http://py.nicolike.cn

[Q35] 内连接
来源：http://bv.yuexingan06.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://qx.shxzskj.cn

[Q36] 左连接
来源：http://xx.jctech888.com.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ye.szxytkj.cn

[Q37] 右连接
来源：http://cm.yuexingan06.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://bj.hnjuh.cn

[Q38] 全外连接（PostgreSQL）
来源：http://vb.gzmigu.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ta.szxytkj.cn

[Q39] 自连接（查上下级）
来源：http://sw.szxytkj.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://gg.shxzukj.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://km.jianghongdianzi.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://yd.jctech888.com.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://lc.jianghongdianzi.cn

[Q41] 多表连接
来源：http://jd.521024.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://vv.jianghongdianzi.cn

JOIN users u ON u.id = o.user_id
来源：http://aq.huanxung.cn

JOIN products p ON p.id = o.product_id;
来源：http://xa.huixinmuqiang.cn

[Q42] 连接条件附加过滤
来源：http://pq.nicolike.cn

SELECT u.name, o.amount FROM users u
来源：http://ij.chemitech.net.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://il.9csxet.cn

[Q43] 标量子查询
来源：http://ke.huanxung.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://iu.shxzukj.cn

[Q44] IN 子查询
来源：http://hc.9csxet.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://jv.lnxyls.cn

[Q45] EXISTS 判断存在
来源：http://jd.hnjuh.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://fs.yuntaijiaju.cn

[Q46] NOT EXISTS 判断不存在
来源：http://xb.chemitech.net.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://td.haigaiapp.cn

[Q47] 与平均值比较
来源：http://tz.szxytkj.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://da.521024.cn

[Q48] CTE 公用表表达式
来源：http://zn.chemitech.net.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://sj.bookmarksfly.cn

SELECT * FROM t WHERE c > 5;
来源：http://yg.521024.cn

[Q49] 更新单行
来源：http://se.newstarts.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://fd.bookmarksfly.cn

[Q50] 批量更新
来源：http://ih.asd995.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://rx.bjjhwx.cn

[Q51] 用子查询更新
来源：http://be.shtwfgs.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://xw.chemitech.net.cn

[Q52] 删除指定行
来源：http://bn.huixinmuqiang.cn

DELETE FROM users WHERE id = 10;
来源：http://sz.shxzskj.cn

[Q53] 按条件删除
来源：http://kf.yuntaijiaju.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mn.huanxung.cn

[Q54] 清空表
来源：http://fz.jianghongdianzi.cn

TRUNCATE TABLE logs;
来源：http://uy.9csxet.cn

[Q55] 排名（并列占位）
来源：http://de.yuntaijiaju.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://lv.jctech888.com.cn

[Q56] 密集排名（并列不占位）
来源：http://jn.shxzukj.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ms.9csxet.cn

[Q57] 行号
来源：http://lj.521024.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://iq.jctech888.com.cn

[Q58] 累计求和
来源：http://dh.wgjwhj.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://dn.huixiangedu.cn

[Q59] 分组内累计
来源：http://on.muxihuayi.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://gf.haigaiapp.cn

[Q60] 取上一行 / 下一行
来源：http://ca.hnjuh.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://re.bjjhwx.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://sh.lnxyls.cn

[Q61] 移动平均
来源：http://pf.nicolike.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://tz.shtwfgs.cn

[Q62] 分组占比
来源：http://df.panjiajie.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://yo.huanxung.cn

[Q63] 开启事务
来源：http://hb.haigaiapp.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://td.haigaiapp.cn

[Q64] 提交事务
来源：http://ne.shxzukj.cn

COMMIT;
来源：http://rb.huanxung.cn

[Q65] 回滚事务
来源：http://as.bookmarksfly.cn

ROLLBACK;
来源：http://ho.newstarts.cn

[Q66] 行锁查询
来源：http://tk.jctech888.com.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ub.colortex.cn

[Q67] 设置隔离级别
来源：http://gj.shxzukj.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ve.bookmarksfly.cn

[Q68] 保存点
来源：http://us.hnjuh.cn

SAVEPOINT sp1;
来源：http://px.chemitech.net.cn

ROLLBACK TO sp1;
来源：http://zn.hnjuh.cn

[Q69] 查看执行计划
来源：http://wl.jctech888.com.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://na.colortex.cn

[Q70] 更新统计信息
来源：http://lh.huixinmuqiang.cn

ANALYZE TABLE users;
来源：http://au.bjjhwx.cn

[Q71] 查看建表语句
来源：http://iu.bookmarksfly.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://js.nszjky.cn

[Q72] 查看索引
来源：http://cc.hahajie.cn

SHOW INDEX FROM users;
来源：http://wd.lnxyls.cn

[Q73] 查看表状态
来源：http://md.chemitech.net.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://tw.bjjhwx.cn

[Q74] 强制使用索引
来源：http://ce.szxytkj.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mr.szsharing.cn

[Q75] 日期格式化
来源：http://cw.huixiangedu.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://na.colortex.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ko.bookmarksfly.cn

[Q76] 按天统计
来源：http://db.newstarts.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://tx.shxzskj.cn

[Q77] 时间加减
来源：http://yq.nszjky.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://io.shtwfgs.cn

[Q78] 当前时间
来源：http://by.yuntaijiaju.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://se.asd995.cn

[Q79] 字符串拼接
来源：http://ok.bookmarksfly.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://bl.shxzskj.cn

[Q80] 字符串截取
来源：http://wf.huixinmuqiang.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://dp.panjiajie.cn

[Q81] 字符串替换
来源：http://lr.chemitech.net.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://pp.shxzskj.cn

[Q82] 字符长度与字节长度
来源：http://kv.asd995.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://db.colortex.cn

[Q83] 大小写转换
来源：http://oa.szxytkj.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://xk.newstarts.cn

[Q84] 去除首尾空格
来源：http://ao.szsharing.cn

SELECT TRIM(name) FROM users;
来源：http://bm.asd995.cn

[Q85] 数值取整
来源：http://ci.gzmigu.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://uj.nszjky.cn

[Q86] 读取 JSON 字段
来源：http://lz.bookmarksfly.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://xt.szxytkj.cn

[Q87] JSON 字段做条件
来源：http://wg.shtwfgs.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://gv.jctech888.com.cn

[Q88] 行转列（条件聚合）
来源：http://vx.9csxet.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://qv.yuexingan06.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hi.jianghongdianzi.cn

[Q89] 判断表是否存在
来源：http://hq.bookmarksfly.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mo.bookmarksfly.cn

[Q90] 生成序号列
来源：http://hq.szxytkj.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wx.szsharing.cn

================================================================================
来源：http://mg.muxihuayi.cn

R. Bash 专题
来源：http://vz.lnxyls.cn

================================================================================
来源：http://iq.asd995.cn

[R01] shebang 与严格模式
来源：http://mm.lnxyls.cn

#!/usr/bin/env bash
来源：http://jt.bookmarksfly.cn

set -euo pipefail
来源：http://dz.lnxyls.cn

[R02] 变量赋值与使用
来源：http://pj.jianghongdianzi.cn

name="Tom"; echo "$name"
来源：http://ay.huanxung.cn

[R03] 只读变量
来源：http://dk.jctech888.com.cn

readonly PI=3.14
来源：http://ij.huixiangedu.cn

[R04] 位置参数
来源：http://sz.huixinmuqiang.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://lt.muxihuayi.cn

[R05] 参数默认值
来源：http://tc.yuntaijiaju.cn

name="${1:-default}"
来源：http://vq.panjiajie.cn

[R06] 判断命令是否存在
来源：http://sc.haigaiapp.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://rj.muxihuayi.cn

[R07] if 判断文件
来源：http://th.wgjwhj.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://rd.gzmigu.cn

[R08] 数值比较
来源：http://xy.yuexingan06.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://ti.hnjuh.cn

[R09] 字符串比较
来源：http://wt.shxzskj.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://if.muxihuayi.cn

[R10] 正则匹配
来源：http://ji.panjiajie.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://xj.yuntaijiaju.cn

[R11] case 多分支
来源：http://xr.gzmigu.cn

case "$1" in
来源：http://vc.bjjhwx.cn

start) echo "启动" ;;
来源：http://if.haigaiapp.cn

stop)  echo "停止" ;;
来源：http://zj.9csxet.cn

*)     echo "未知命令" ;;
来源：http://ot.shxzukj.cn

esac
来源：http://ng.hahajie.cn

[R12] for 遍历文件
来源：http://pb.shxzukj.cn

for f in *.txt; do echo "$f"; done
来源：http://uk.jianghongdianzi.cn

[R13] for 计数循环
来源：http://ww.huanxung.cn

for i in {1..10}; do echo "$i"; done
来源：http://oa.szxytkj.cn

[R14] C 风格 for
来源：http://rp.lnxyls.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://eh.yuntaijiaju.cn

[R15] while 逐行读文件
来源：http://as.wgjwhj.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ez.nicolike.cn

[R16] until 等待条件
来源：http://fs.bjjhwx.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://zw.gzmigu.cn

[R17] 数组定义与取值
来源：http://ff.szsharing.cn


<!-- 参考信息 -->