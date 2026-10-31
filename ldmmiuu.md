代发 wailian999

Ruby: Digest::SHA256.hexdigest(s)
来源：http://yh.chemitech.net.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://zo.bjjhwx.cn

[P03] 生成短随机字符串
来源：http://fg.shtwfgs.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://dm.wgjwhj.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://se.newstarts.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://yh.nicolike.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://zq.szsharing.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ut.lnxyls.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://po.nszjky.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://uz.haigaiapp.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://cn.hnjuh.cn

[P04] 求长度
来源：http://xg.bookmarksfly.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://km.newstarts.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://jw.lnxyls.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://jw.yuexingan06.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://nd.shxzskj.cn

Java: list.size();  map.size();  s.length()
来源：http://jf.panjiajie.cn

Go:   len(arr);  len(m)
来源：http://rp.newstarts.cn

Ruby: x.length;  x.size
来源：http://km.panjiajie.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://vn.chemitech.net.cn

[P05] 判断两个对象内容是否相等
来源：http://lo.muxihuayi.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://gc.bjjhwx.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ov.wgjwhj.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://th.hnjuh.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://rl.521024.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://tc.muxihuayi.cn

Go:   reflect.DeepEqual(a, b)
来源：http://lm.panjiajie.cn

Ruby: a == b
来源：http://vy.jctech888.com.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mm.gzmigu.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://qv.yuntaijiaju.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://zu.lnxyls.cn

PHP:  if (empty($x)) {}
来源：http://gg.asd995.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://pb.chemitech.net.cn

TS:   if (x == null) {}
来源：http://fj.521024.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://fm.bookmarksfly.cn

Go:   if x == nil {}
来源：http://qx.bookmarksfly.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ot.hahajie.cn

C#:   if (x is null) {}
来源：http://yw.huanxung.cn

[P07] 防抖与节流
来源：http://mb.521024.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://fx.wgjwhj.cn

PHP:  // 手写时间戳比较
来源：http://kd.bjjhwx.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://os.9csxet.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://oq.shxzukj.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://pd.jctech888.com.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://pe.newstarts.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://oz.haigaiapp.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://yz.lnxyls.cn

[P08] 处理浮点精度问题
来源：http://ka.shtwfgs.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://jc.yuexingan06.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://nq.wgjwhj.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://gp.wgjwhj.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ge.muxihuayi.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://px.yuntaijiaju.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://bq.nicolike.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://lv.jctech888.com.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ga.huanxung.cn

================================================================================
来源：http://xd.panjiajie.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://it.newstarts.cn

================================================================================
来源：http://pd.gzmigu.cn

[Q01] 创建表
来源：http://rr.bjjhwx.cn

CREATE TABLE users (
来源：http://fg.lnxyls.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://yg.asd995.cn

name VARCHAR(50) NOT NULL,
来源：http://wb.jianghongdianzi.cn

email VARCHAR(100) UNIQUE,
来源：http://jo.bjjhwx.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ku.lnxyls.cn

);
来源：http://at.lnxyls.cn

[Q02] 创建带外键的表
来源：http://kb.asd995.cn

CREATE TABLE orders (
来源：http://mq.hahajie.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://xl.haigaiapp.cn

user_id INT NOT NULL,
来源：http://nt.nicolike.cn

amount DECIMAL(10, 2),
来源：http://xc.521024.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ew.shtwfgs.cn

);
来源：http://sa.szxytkj.cn

[Q03] 增加列
来源：http://gk.lnxyls.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://tc.jianghongdianzi.cn

[Q04] 修改列类型
来源：http://am.newstarts.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://up.colortex.cn

[Q05] 重命名列
来源：http://os.shxzukj.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://xb.nicolike.cn

[Q06] 删除列
来源：http://kq.bookmarksfly.cn

ALTER TABLE users DROP COLUMN age;
来源：http://ws.muxihuayi.cn

[Q07] 删除表
来源：http://wc.huanxung.cn

DROP TABLE IF EXISTS orders;
来源：http://cn.newstarts.cn

[Q08] 创建普通索引
来源：http://wm.newstarts.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://cd.shtwfgs.cn

[Q09] 创建唯一索引
来源：http://vr.panjiajie.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://rt.lnxyls.cn

[Q10] 插入单行
来源：http://yu.nicolike.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://nb.hahajie.cn

[Q11] 一次插入多行
来源：http://tw.jianghongdianzi.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ln.shtwfgs.cn

[Q12] 插入后取自增 ID
来源：http://hh.jianghongdianzi.cn

INSERT INTO users (name) VALUES ('C');
来源：http://bv.jianghongdianzi.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ge.9csxet.cn

[Q13] 忽略重复插入
来源：http://ia.nszjky.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mn.hahajie.cn

[Q14] 存在则更新（upsert）
来源：http://aa.bjjhwx.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://zg.shxzukj.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ad.szxytkj.cn

[Q15] 查询全部
来源：http://bi.colortex.cn

SELECT * FROM users;
来源：http://ce.asd995.cn

[Q16] 查询指定列
来源：http://wz.newstarts.cn

SELECT id, name FROM users;
来源：http://ov.chemitech.net.cn

[Q17] 条件查询
来源：http://mh.jianghongdianzi.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://zk.muxihuayi.cn

[Q18] 模糊匹配
来源：http://tw.bjjhwx.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://de.asd995.cn

[Q19] 范围查询
来源：http://pq.nszjky.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://sh.jianghongdianzi.cn

[Q20] IN 列表
来源：http://vg.huixinmuqiang.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://kf.gzmigu.cn

[Q21] 空值判断
来源：http://jx.shtwfgs.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://zq.huanxung.cn

[Q22] 排序
来源：http://qc.gzmigu.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://oc.shtwfgs.cn

[Q23] 分页
来源：http://ws.asd995.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://tk.huanxung.cn

[Q24] 去重
来源：http://zh.huixinmuqiang.cn

SELECT DISTINCT city FROM users;
来源：http://wu.lnxyls.cn

[Q25] 只取前 N 条
来源：http://hg.huanxung.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ov.9csxet.cn

[Q26] 计数
来源：http://pc.hnjuh.cn

SELECT COUNT(*) FROM users;
来源：http://jl.chemitech.net.cn

[Q27] 条件计数
来源：http://sm.bookmarksfly.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://xn.haigaiapp.cn

[Q28] 求和与平均
来源：http://xl.newstarts.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://bf.szsharing.cn

[Q29] 最大最小值
来源：http://es.szxytkj.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://mx.bjjhwx.cn

[Q30] 分组统计
来源：http://ue.hnjuh.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ye.yuntaijiaju.cn

[Q31] 分组后过滤
来源：http://vv.lnxyls.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://nq.huixinmuqiang.cn

[Q32] 分组拼接字符串
来源：http://eh.hnjuh.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://lf.shxzskj.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://lu.muxihuayi.cn

[Q33] 多列分组
来源：http://yn.jianghongdianzi.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wt.bookmarksfly.cn

[Q34] 每组取第一条
来源：http://ti.huanxung.cn

SELECT * FROM (
来源：http://rh.nicolike.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://rs.asd995.cn

) t WHERE rn = 1;
来源：http://ag.huanxung.cn

[Q35] 内连接
来源：http://pz.chemitech.net.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://te.lnxyls.cn

[Q36] 左连接
来源：http://hn.lnxyls.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://tp.nszjky.cn

[Q37] 右连接
来源：http://ds.lnxyls.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://bf.hnjuh.cn

[Q38] 全外连接（PostgreSQL）
来源：http://be.huixinmuqiang.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://kx.jctech888.com.cn

[Q39] 自连接（查上下级）
来源：http://vs.nszjky.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://lz.chemitech.net.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://st.huixinmuqiang.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://ls.wgjwhj.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://uo.shxzskj.cn

[Q41] 多表连接
来源：http://mo.shxzskj.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://jp.gzmigu.cn

JOIN users u ON u.id = o.user_id
来源：http://xk.shtwfgs.cn

JOIN products p ON p.id = o.product_id;
来源：http://od.shxzskj.cn

[Q42] 连接条件附加过滤
来源：http://ds.lnxyls.cn

SELECT u.name, o.amount FROM users u
来源：http://ty.jianghongdianzi.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://th.jianghongdianzi.cn

[Q43] 标量子查询
来源：http://le.bookmarksfly.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://xp.shxzskj.cn

[Q44] IN 子查询
来源：http://ql.huixinmuqiang.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ve.bjjhwx.cn

[Q45] EXISTS 判断存在
来源：http://rw.huixiangedu.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://xb.bookmarksfly.cn

[Q46] NOT EXISTS 判断不存在
来源：http://ox.jctech888.com.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ez.521024.cn

[Q47] 与平均值比较
来源：http://fv.haigaiapp.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://oz.newstarts.cn

[Q48] CTE 公用表表达式
来源：http://fq.panjiajie.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ey.szsharing.cn

SELECT * FROM t WHERE c > 5;
来源：http://bs.yuexingan06.cn

[Q49] 更新单行
来源：http://aq.huixiangedu.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://sy.bookmarksfly.cn

[Q50] 批量更新
来源：http://hk.wgjwhj.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://nj.shxzskj.cn

[Q51] 用子查询更新
来源：http://yr.yuntaijiaju.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wq.9csxet.cn

[Q52] 删除指定行
来源：http://am.9csxet.cn

DELETE FROM users WHERE id = 10;
来源：http://wo.panjiajie.cn

[Q53] 按条件删除
来源：http://az.szsharing.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://op.asd995.cn

[Q54] 清空表
来源：http://qo.colortex.cn

TRUNCATE TABLE logs;
来源：http://nq.9csxet.cn

[Q55] 排名（并列占位）
来源：http://dw.yuntaijiaju.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://rc.huixiangedu.cn

[Q56] 密集排名（并列不占位）
来源：http://ug.521024.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ra.muxihuayi.cn

[Q57] 行号
来源：http://mk.szxytkj.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://lk.hnjuh.cn

[Q58] 累计求和
来源：http://sn.yuexingan06.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://tg.chemitech.net.cn

[Q59] 分组内累计
来源：http://qr.szsharing.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ih.lnxyls.cn

[Q60] 取上一行 / 下一行
来源：http://ii.colortex.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://jz.muxihuayi.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://be.jianghongdianzi.cn

[Q61] 移动平均
来源：http://xi.yuexingan06.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://xe.bookmarksfly.cn

[Q62] 分组占比
来源：http://io.huanxung.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://dm.huixinmuqiang.cn

[Q63] 开启事务
来源：http://tc.hnjuh.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://ma.szxytkj.cn

[Q64] 提交事务
来源：http://jn.gzmigu.cn

COMMIT;
来源：http://kn.lnxyls.cn

[Q65] 回滚事务
来源：http://hs.bjjhwx.cn

ROLLBACK;
来源：http://so.jctech888.com.cn

[Q66] 行锁查询
来源：http://iz.521024.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://vn.shtwfgs.cn

[Q67] 设置隔离级别
来源：http://lq.chemitech.net.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://cm.gzmigu.cn

[Q68] 保存点
来源：http://jd.asd995.cn

SAVEPOINT sp1;
来源：http://le.jctech888.com.cn

ROLLBACK TO sp1;
来源：http://fr.lnxyls.cn

[Q69] 查看执行计划
来源：http://ss.wgjwhj.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://jl.jianghongdianzi.cn

[Q70] 更新统计信息
来源：http://lr.shtwfgs.cn

ANALYZE TABLE users;
来源：http://xf.haigaiapp.cn

[Q71] 查看建表语句
来源：http://kt.szsharing.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://av.newstarts.cn

[Q72] 查看索引
来源：http://wo.521024.cn

SHOW INDEX FROM users;
来源：http://lr.szxytkj.cn

[Q73] 查看表状态
来源：http://ej.shxzukj.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://qu.lnxyls.cn

[Q74] 强制使用索引
来源：http://bs.yuexingan06.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://zh.szxytkj.cn

[Q75] 日期格式化
来源：http://pn.shxzukj.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://cq.shtwfgs.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://fa.colortex.cn

[Q76] 按天统计
来源：http://cf.nszjky.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://zr.lnxyls.cn

[Q77] 时间加减
来源：http://bn.newstarts.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ds.szsharing.cn

[Q78] 当前时间
来源：http://dz.huanxung.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://vp.yuexingan06.cn

[Q79] 字符串拼接
来源：http://kz.nszjky.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ee.bookmarksfly.cn

[Q80] 字符串截取
来源：http://zr.hnjuh.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://xv.nicolike.cn

[Q81] 字符串替换
来源：http://rl.hnjuh.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://oy.szsharing.cn

[Q82] 字符长度与字节长度
来源：http://an.colortex.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://pf.shxzskj.cn

[Q83] 大小写转换
来源：http://pg.szxytkj.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://gj.gzmigu.cn

[Q84] 去除首尾空格
来源：http://pm.szxytkj.cn

SELECT TRIM(name) FROM users;
来源：http://qo.jctech888.com.cn

[Q85] 数值取整
来源：http://on.jctech888.com.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://pf.nicolike.cn

[Q86] 读取 JSON 字段
来源：http://zo.jctech888.com.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ek.panjiajie.cn

[Q87] JSON 字段做条件
来源：http://bx.bjjhwx.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ht.wgjwhj.cn

[Q88] 行转列（条件聚合）
来源：http://oy.muxihuayi.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://io.nszjky.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://my.newstarts.cn

[Q89] 判断表是否存在
来源：http://wm.hahajie.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://es.huanxung.cn

[Q90] 生成序号列
来源：http://ym.jianghongdianzi.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://dx.szsharing.cn

================================================================================
来源：http://lf.muxihuayi.cn

R. Bash 专题
来源：http://li.huanxung.cn

================================================================================
来源：http://zy.haigaiapp.cn

[R01] shebang 与严格模式
来源：http://zk.521024.cn

#!/usr/bin/env bash
来源：http://fm.newstarts.cn

set -euo pipefail
来源：http://lt.jctech888.com.cn

[R02] 变量赋值与使用
来源：http://zk.hahajie.cn

name="Tom"; echo "$name"
来源：http://kb.huanxung.cn

[R03] 只读变量
来源：http://lk.521024.cn

readonly PI=3.14
来源：http://mk.muxihuayi.cn

[R04] 位置参数
来源：http://ed.chemitech.net.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hr.colortex.cn

[R05] 参数默认值
来源：http://or.huixiangedu.cn

name="${1:-default}"
来源：http://mt.colortex.cn

[R06] 判断命令是否存在
来源：http://sm.asd995.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://op.haigaiapp.cn

[R07] if 判断文件
来源：http://px.szsharing.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://iy.szxytkj.cn

[R08] 数值比较
来源：http://xl.haigaiapp.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://sf.haigaiapp.cn

[R09] 字符串比较
来源：http://mx.shxzskj.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ms.colortex.cn

[R10] 正则匹配
来源：http://xs.panjiajie.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://cd.shxzukj.cn

[R11] case 多分支
来源：http://kx.szsharing.cn

case "$1" in
来源：http://kz.yuexingan06.cn

start) echo "启动" ;;
来源：http://fq.jctech888.com.cn

stop)  echo "停止" ;;
来源：http://xm.bjjhwx.cn

*)     echo "未知命令" ;;
来源：http://gf.jianghongdianzi.cn

esac
来源：http://ia.hnjuh.cn

[R12] for 遍历文件
来源：http://kc.newstarts.cn

for f in *.txt; do echo "$f"; done
来源：http://ab.yuexingan06.cn

[R13] for 计数循环
来源：http://ue.yuexingan06.cn

for i in {1..10}; do echo "$i"; done
来源：http://wa.hahajie.cn

[R14] C 风格 for
来源：http://xe.shxzukj.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://qd.hahajie.cn

[R15] while 逐行读文件
来源：http://wf.panjiajie.cn


<!-- 参考信息 -->