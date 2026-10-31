代发 wailian999

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.panjiajie.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://co.chemitech.net.cn

[P03] 生成短随机字符串
来源：http://kn.muxihuayi.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://jp.shxzskj.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://nj.bjjhwx.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://kh.bjjhwx.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ad.hahajie.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://fj.jianghongdianzi.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://tr.hahajie.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://hd.huanxung.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ng.panjiajie.cn

[P04] 求长度
来源：http://do.nszjky.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://bg.huanxung.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ys.lnxyls.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://af.muxihuayi.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://dt.chemitech.net.cn

Java: list.size();  map.size();  s.length()
来源：http://xr.huixiangedu.cn

Go:   len(arr);  len(m)
来源：http://hb.muxihuayi.cn

Ruby: x.length;  x.size
来源：http://za.yuntaijiaju.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://bc.521024.cn

[P05] 判断两个对象内容是否相等
来源：http://bn.521024.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://gj.hnjuh.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://tj.colortex.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mu.nszjky.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://sx.hahajie.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://dn.wgjwhj.cn

Go:   reflect.DeepEqual(a, b)
来源：http://ve.bjjhwx.cn

Ruby: a == b
来源：http://nu.521024.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://bm.huixiangedu.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://dm.521024.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://qf.asd995.cn

PHP:  if (empty($x)) {}
来源：http://xw.wgjwhj.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://lk.nszjky.cn

TS:   if (x == null) {}
来源：http://az.huixinmuqiang.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://ja.shxzskj.cn

Go:   if x == nil {}
来源：http://ey.nicolike.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://el.nszjky.cn

C#:   if (x is null) {}
来源：http://wv.nszjky.cn

[P07] 防抖与节流
来源：http://kp.jianghongdianzi.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://cb.haigaiapp.cn

PHP:  // 手写时间戳比较
来源：http://si.panjiajie.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://bu.bjjhwx.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qp.nicolike.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://zw.shxzskj.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mj.jctech888.com.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://qf.szxytkj.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://xx.wgjwhj.cn

[P08] 处理浮点精度问题
来源：http://dr.bookmarksfly.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://yz.muxihuayi.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://tv.jianghongdianzi.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://kl.shxzskj.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://xm.bookmarksfly.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://lp.asd995.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://vc.panjiajie.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://kf.newstarts.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://lc.hnjuh.cn

================================================================================
来源：http://ng.yuexingan06.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://kc.muxihuayi.cn

================================================================================
来源：http://hs.haigaiapp.cn

[Q01] 创建表
来源：http://pa.newstarts.cn

CREATE TABLE users (
来源：http://wu.bjjhwx.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://vz.wgjwhj.cn

name VARCHAR(50) NOT NULL,
来源：http://ww.panjiajie.cn

email VARCHAR(100) UNIQUE,
来源：http://bs.9csxet.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://kv.lnxyls.cn

);
来源：http://cc.chemitech.net.cn

[Q02] 创建带外键的表
来源：http://nj.lnxyls.cn

CREATE TABLE orders (
来源：http://cs.szxytkj.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ss.lnxyls.cn

user_id INT NOT NULL,
来源：http://ba.haigaiapp.cn

amount DECIMAL(10, 2),
来源：http://uo.bookmarksfly.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://kk.huixiangedu.cn

);
来源：http://nm.hnjuh.cn

[Q03] 增加列
来源：http://ge.shtwfgs.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ub.gzmigu.cn

[Q04] 修改列类型
来源：http://on.newstarts.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://tp.jianghongdianzi.cn

[Q05] 重命名列
来源：http://ub.9csxet.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://qj.bookmarksfly.cn

[Q06] 删除列
来源：http://ax.haigaiapp.cn

ALTER TABLE users DROP COLUMN age;
来源：http://ri.lnxyls.cn

[Q07] 删除表
来源：http://ia.huixiangedu.cn

DROP TABLE IF EXISTS orders;
来源：http://yy.nszjky.cn

[Q08] 创建普通索引
来源：http://bg.colortex.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://jq.yuexingan06.cn

[Q09] 创建唯一索引
来源：http://gn.shxzskj.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://fq.asd995.cn

[Q10] 插入单行
来源：http://yb.yuexingan06.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hk.asd995.cn

[Q11] 一次插入多行
来源：http://fu.colortex.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://zh.shxzukj.cn

[Q12] 插入后取自增 ID
来源：http://by.colortex.cn

INSERT INTO users (name) VALUES ('C');
来源：http://ah.newstarts.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://cc.jctech888.com.cn

[Q13] 忽略重复插入
来源：http://jx.muxihuayi.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://og.colortex.cn

[Q14] 存在则更新（upsert）
来源：http://jz.shxzskj.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hf.chemitech.net.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://kq.chemitech.net.cn

[Q15] 查询全部
来源：http://bx.9csxet.cn

SELECT * FROM users;
来源：http://qr.muxihuayi.cn

[Q16] 查询指定列
来源：http://yv.muxihuayi.cn

SELECT id, name FROM users;
来源：http://eg.shxzskj.cn

[Q17] 条件查询
来源：http://uj.huanxung.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ci.shxzukj.cn

[Q18] 模糊匹配
来源：http://vz.huixiangedu.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://uj.szxytkj.cn

[Q19] 范围查询
来源：http://nf.haigaiapp.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://bq.bookmarksfly.cn

[Q20] IN 列表
来源：http://bd.szsharing.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://nq.hahajie.cn

[Q21] 空值判断
来源：http://qu.jctech888.com.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://gd.521024.cn

[Q22] 排序
来源：http://uu.nicolike.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://je.9csxet.cn

[Q23] 分页
来源：http://ih.jctech888.com.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://nn.521024.cn

[Q24] 去重
来源：http://io.yuexingan06.cn

SELECT DISTINCT city FROM users;
来源：http://km.lnxyls.cn

[Q25] 只取前 N 条
来源：http://kf.huixiangedu.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://du.panjiajie.cn

[Q26] 计数
来源：http://fu.521024.cn

SELECT COUNT(*) FROM users;
来源：http://ol.szxytkj.cn

[Q27] 条件计数
来源：http://om.newstarts.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://bb.nszjky.cn

[Q28] 求和与平均
来源：http://md.panjiajie.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hx.haigaiapp.cn

[Q29] 最大最小值
来源：http://qa.szsharing.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://sw.wgjwhj.cn

[Q30] 分组统计
来源：http://vt.bjjhwx.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ky.huixiangedu.cn

[Q31] 分组后过滤
来源：http://gj.hahajie.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://oh.lnxyls.cn

[Q32] 分组拼接字符串
来源：http://xm.lnxyls.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://oo.haigaiapp.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://fq.muxihuayi.cn

[Q33] 多列分组
来源：http://xt.muxihuayi.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://rx.panjiajie.cn

[Q34] 每组取第一条
来源：http://tk.nszjky.cn

SELECT * FROM (
来源：http://fk.asd995.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://pa.nicolike.cn

) t WHERE rn = 1;
来源：http://hb.huanxung.cn

[Q35] 内连接
来源：http://mq.shtwfgs.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ge.nszjky.cn

[Q36] 左连接
来源：http://cb.haigaiapp.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://sc.nszjky.cn

[Q37] 右连接
来源：http://yl.jctech888.com.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://gs.newstarts.cn

[Q38] 全外连接（PostgreSQL）
来源：http://yo.huixiangedu.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://px.shtwfgs.cn

[Q39] 自连接（查上下级）
来源：http://wr.yuexingan06.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://ys.yuntaijiaju.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ho.chemitech.net.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://uk.shxzskj.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://pc.gzmigu.cn

[Q41] 多表连接
来源：http://vc.9csxet.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://ek.hnjuh.cn

JOIN users u ON u.id = o.user_id
来源：http://hl.shxzskj.cn

JOIN products p ON p.id = o.product_id;
来源：http://av.wgjwhj.cn

[Q42] 连接条件附加过滤
来源：http://ek.huixinmuqiang.cn

SELECT u.name, o.amount FROM users u
来源：http://zu.panjiajie.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://gl.lnxyls.cn

[Q43] 标量子查询
来源：http://fn.colortex.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://fz.panjiajie.cn

[Q44] IN 子查询
来源：http://zk.bookmarksfly.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://md.newstarts.cn

[Q45] EXISTS 判断存在
来源：http://bj.panjiajie.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://um.bookmarksfly.cn

[Q46] NOT EXISTS 判断不存在
来源：http://at.9csxet.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://zl.yuexingan06.cn

[Q47] 与平均值比较
来源：http://qm.panjiajie.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://qf.haigaiapp.cn

[Q48] CTE 公用表表达式
来源：http://sx.9csxet.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://jm.521024.cn

SELECT * FROM t WHERE c > 5;
来源：http://sg.muxihuayi.cn

[Q49] 更新单行
来源：http://qe.muxihuayi.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://db.szsharing.cn

[Q50] 批量更新
来源：http://nv.newstarts.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://xj.shxzskj.cn

[Q51] 用子查询更新
来源：http://rz.hnjuh.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://lo.yuexingan06.cn

[Q52] 删除指定行
来源：http://yn.hahajie.cn

DELETE FROM users WHERE id = 10;
来源：http://ya.colortex.cn

[Q53] 按条件删除
来源：http://zb.nszjky.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ae.yuexingan06.cn

[Q54] 清空表
来源：http://ab.hahajie.cn

TRUNCATE TABLE logs;
来源：http://ce.shxzskj.cn

[Q55] 排名（并列占位）
来源：http://so.haigaiapp.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://pt.bookmarksfly.cn

[Q56] 密集排名（并列不占位）
来源：http://ad.shxzskj.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://or.huixinmuqiang.cn

[Q57] 行号
来源：http://th.huixinmuqiang.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ba.jctech888.com.cn

[Q58] 累计求和
来源：http://op.haigaiapp.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://lc.huixinmuqiang.cn

[Q59] 分组内累计
来源：http://cc.wgjwhj.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ha.wgjwhj.cn

[Q60] 取上一行 / 下一行
来源：http://vc.shtwfgs.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://da.huanxung.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://vj.wgjwhj.cn

[Q61] 移动平均
来源：http://kk.colortex.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://db.colortex.cn

[Q62] 分组占比
来源：http://bp.yuexingan06.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://os.colortex.cn

[Q63] 开启事务
来源：http://yo.muxihuayi.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://xt.gzmigu.cn

[Q64] 提交事务
来源：http://sf.hnjuh.cn

COMMIT;
来源：http://lp.huixinmuqiang.cn

[Q65] 回滚事务
来源：http://rj.wgjwhj.cn

ROLLBACK;
来源：http://vu.nicolike.cn

[Q66] 行锁查询
来源：http://wd.lnxyls.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mn.hahajie.cn

[Q67] 设置隔离级别
来源：http://lo.jctech888.com.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://yv.yuntaijiaju.cn

[Q68] 保存点
来源：http://qb.chemitech.net.cn

SAVEPOINT sp1;
来源：http://fx.bjjhwx.cn

ROLLBACK TO sp1;
来源：http://kf.shtwfgs.cn

[Q69] 查看执行计划
来源：http://pe.hahajie.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://px.szsharing.cn

[Q70] 更新统计信息
来源：http://by.nicolike.cn

ANALYZE TABLE users;
来源：http://qs.nicolike.cn

[Q71] 查看建表语句
来源：http://yu.szxytkj.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://go.9csxet.cn

[Q72] 查看索引
来源：http://sn.yuntaijiaju.cn

SHOW INDEX FROM users;
来源：http://ba.shxzukj.cn

[Q73] 查看表状态
来源：http://id.bjjhwx.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://ra.shtwfgs.cn

[Q74] 强制使用索引
来源：http://vh.chemitech.net.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mb.nicolike.cn

[Q75] 日期格式化
来源：http://vb.bookmarksfly.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wy.huixiangedu.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://xj.bjjhwx.cn

[Q76] 按天统计
来源：http://bw.521024.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wq.huanxung.cn

[Q77] 时间加减
来源：http://mv.bookmarksfly.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ni.haigaiapp.cn

[Q78] 当前时间
来源：http://gg.hahajie.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://aa.asd995.cn

[Q79] 字符串拼接
来源：http://hh.yuntaijiaju.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wm.shtwfgs.cn

[Q80] 字符串截取
来源：http://di.huixiangedu.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://re.panjiajie.cn

[Q81] 字符串替换
来源：http://fy.panjiajie.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://sf.jctech888.com.cn

[Q82] 字符长度与字节长度
来源：http://ec.hnjuh.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://nf.yuexingan06.cn

[Q83] 大小写转换
来源：http://et.huanxung.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://my.shtwfgs.cn

[Q84] 去除首尾空格
来源：http://wj.hnjuh.cn

SELECT TRIM(name) FROM users;
来源：http://xs.9csxet.cn

[Q85] 数值取整
来源：http://pp.panjiajie.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://xi.bjjhwx.cn

[Q86] 读取 JSON 字段
来源：http://bw.shxzskj.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://cb.muxihuayi.cn

[Q87] JSON 字段做条件
来源：http://hk.521024.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ir.panjiajie.cn

[Q88] 行转列（条件聚合）
来源：http://ek.wgjwhj.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://iu.newstarts.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://xs.szsharing.cn

[Q89] 判断表是否存在
来源：http://xe.lnxyls.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://je.hnjuh.cn

[Q90] 生成序号列
来源：http://bm.shxzskj.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://bl.jianghongdianzi.cn

================================================================================
来源：http://sg.wgjwhj.cn

R. Bash 专题
来源：http://wf.huixinmuqiang.cn

================================================================================
来源：http://aa.yuexingan06.cn

[R01] shebang 与严格模式
来源：http://mn.yuntaijiaju.cn

#!/usr/bin/env bash
来源：http://le.521024.cn

set -euo pipefail
来源：http://am.colortex.cn

[R02] 变量赋值与使用
来源：http://et.huixiangedu.cn

name="Tom"; echo "$name"
来源：http://fg.9csxet.cn

[R03] 只读变量
来源：http://qx.jctech888.com.cn

readonly PI=3.14
来源：http://px.jctech888.com.cn

[R04] 位置参数
来源：http://mg.haigaiapp.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://to.haigaiapp.cn

[R05] 参数默认值
来源：http://yc.szsharing.cn

name="${1:-default}"
来源：http://fq.shxzukj.cn

[R06] 判断命令是否存在
来源：http://po.shxzskj.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://od.asd995.cn

[R07] if 判断文件
来源：http://ct.szsharing.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hl.muxihuayi.cn

[R08] 数值比较
来源：http://sd.521024.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://vh.asd995.cn

[R09] 字符串比较
来源：http://zs.9csxet.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ga.szxytkj.cn

[R10] 正则匹配
来源：http://cc.muxihuayi.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://jv.bookmarksfly.cn

[R11] case 多分支
来源：http://yw.panjiajie.cn

case "$1" in
来源：http://sg.shxzskj.cn

start) echo "启动" ;;
来源：http://yg.jctech888.com.cn

stop)  echo "停止" ;;
来源：http://fx.nicolike.cn

*)     echo "未知命令" ;;
来源：http://oz.asd995.cn

esac
来源：http://wo.bookmarksfly.cn

[R12] for 遍历文件
来源：http://wh.chemitech.net.cn

for f in *.txt; do echo "$f"; done
来源：http://kq.panjiajie.cn

[R13] for 计数循环
来源：http://rs.shtwfgs.cn

for i in {1..10}; do echo "$i"; done
来源：http://iw.lnxyls.cn

[R14] C 风格 for
来源：http://eh.szsharing.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://rm.huixinmuqiang.cn

[R15] while 逐行读文件
来源：http://oe.yuntaijiaju.cn


<!-- 参考信息 -->