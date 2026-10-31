代发 wailian999

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://vz.panjiajie.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://bf.huanxung.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://oj.szxytkj.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://an.jctech888.com.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://al.lnxyls.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://dn.szsharing.cn

[P03] 生成短随机字符串
来源：http://pf.9csxet.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://dg.szsharing.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://xy.hahajie.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://gw.nszjky.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://bs.muxihuayi.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://lv.lnxyls.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ad.nicolike.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://br.chemitech.net.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://tt.huixiangedu.cn

[P04] 求长度
来源：http://gc.nicolike.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://fq.521024.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ru.shtwfgs.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://lx.chemitech.net.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://kv.gzmigu.cn

Java: list.size();  map.size();  s.length()
来源：http://ps.gzmigu.cn

Go:   len(arr);  len(m)
来源：http://ml.szsharing.cn

Ruby: x.length;  x.size
来源：http://nn.hnjuh.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://xi.asd995.cn

[P05] 判断两个对象内容是否相等
来源：http://ha.shxzukj.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://ub.lnxyls.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://tf.shxzukj.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://eh.gzmigu.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ru.gzmigu.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://dt.szxytkj.cn

Go:   reflect.DeepEqual(a, b)
来源：http://pe.haigaiapp.cn

Ruby: a == b
来源：http://gd.nszjky.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://fk.shxzskj.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ev.shxzskj.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://kl.shxzukj.cn

PHP:  if (empty($x)) {}
来源：http://gt.shxzukj.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://sy.shtwfgs.cn

TS:   if (x == null) {}
来源：http://sp.huixiangedu.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://yb.szxytkj.cn

Go:   if x == nil {}
来源：http://zc.jctech888.com.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://pm.jianghongdianzi.cn

C#:   if (x is null) {}
来源：http://eh.bookmarksfly.cn

[P07] 防抖与节流
来源：http://qs.521024.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://bx.lnxyls.cn

PHP:  // 手写时间戳比较
来源：http://mz.huixinmuqiang.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://se.haigaiapp.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://zr.yuexingan06.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ld.huixinmuqiang.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://us.szxytkj.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://rs.hahajie.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://kv.szxytkj.cn

[P08] 处理浮点精度问题
来源：http://ze.wgjwhj.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://jo.chemitech.net.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://sc.jctech888.com.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://cp.szsharing.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wj.yuexingan06.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://gp.huanxung.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://zp.szsharing.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ct.jctech888.com.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wr.muxihuayi.cn

================================================================================
来源：http://wv.huixiangedu.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ox.huixiangedu.cn

================================================================================
来源：http://hy.asd995.cn

[Q01] 创建表
来源：http://ps.yuexingan06.cn

CREATE TABLE users (
来源：http://yp.jianghongdianzi.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ne.jctech888.com.cn

name VARCHAR(50) NOT NULL,
来源：http://cg.newstarts.cn

email VARCHAR(100) UNIQUE,
来源：http://th.hahajie.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://oc.shxzskj.cn

);
来源：http://cn.asd995.cn

[Q02] 创建带外键的表
来源：http://zs.shtwfgs.cn

CREATE TABLE orders (
来源：http://ot.nszjky.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://qt.yuexingan06.cn

user_id INT NOT NULL,
来源：http://gu.shxzukj.cn

amount DECIMAL(10, 2),
来源：http://or.lnxyls.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://tg.haigaiapp.cn

);
来源：http://mu.colortex.cn

[Q03] 增加列
来源：http://vj.huanxung.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ma.yuntaijiaju.cn

[Q04] 修改列类型
来源：http://yy.asd995.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://zl.bookmarksfly.cn

[Q05] 重命名列
来源：http://fb.jctech888.com.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://zw.muxihuayi.cn

[Q06] 删除列
来源：http://xb.bookmarksfly.cn

ALTER TABLE users DROP COLUMN age;
来源：http://kg.wgjwhj.cn

[Q07] 删除表
来源：http://cf.yuntaijiaju.cn

DROP TABLE IF EXISTS orders;
来源：http://lk.newstarts.cn

[Q08] 创建普通索引
来源：http://ze.hahajie.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://jz.9csxet.cn

[Q09] 创建唯一索引
来源：http://os.newstarts.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ky.szsharing.cn

[Q10] 插入单行
来源：http://av.9csxet.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mz.huanxung.cn

[Q11] 一次插入多行
来源：http://se.huixinmuqiang.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://gv.huixinmuqiang.cn

[Q12] 插入后取自增 ID
来源：http://rg.jctech888.com.cn

INSERT INTO users (name) VALUES ('C');
来源：http://jm.shxzskj.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://qy.nicolike.cn

[Q13] 忽略重复插入
来源：http://jq.521024.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mo.nszjky.cn

[Q14] 存在则更新（upsert）
来源：http://sb.gzmigu.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://sw.haigaiapp.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://fn.muxihuayi.cn

[Q15] 查询全部
来源：http://yy.muxihuayi.cn

SELECT * FROM users;
来源：http://fk.bjjhwx.cn

[Q16] 查询指定列
来源：http://cq.jctech888.com.cn

SELECT id, name FROM users;
来源：http://sd.yuexingan06.cn

[Q17] 条件查询
来源：http://bv.bjjhwx.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://uu.bjjhwx.cn

[Q18] 模糊匹配
来源：http://ma.yuntaijiaju.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://jy.521024.cn

[Q19] 范围查询
来源：http://zv.nicolike.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://if.shtwfgs.cn

[Q20] IN 列表
来源：http://lx.9csxet.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://bt.jctech888.com.cn

[Q21] 空值判断
来源：http://sw.muxihuayi.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://eq.bjjhwx.cn

[Q22] 排序
来源：http://xr.lnxyls.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://iu.chemitech.net.cn

[Q23] 分页
来源：http://ah.yuntaijiaju.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://bt.9csxet.cn

[Q24] 去重
来源：http://yj.colortex.cn

SELECT DISTINCT city FROM users;
来源：http://fj.szsharing.cn

[Q25] 只取前 N 条
来源：http://ev.nszjky.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ri.yuexingan06.cn

[Q26] 计数
来源：http://va.nicolike.cn

SELECT COUNT(*) FROM users;
来源：http://mv.huixiangedu.cn

[Q27] 条件计数
来源：http://kk.asd995.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mr.asd995.cn

[Q28] 求和与平均
来源：http://os.muxihuayi.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://ah.szxytkj.cn

[Q29] 最大最小值
来源：http://kp.jianghongdianzi.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://vo.wgjwhj.cn

[Q30] 分组统计
来源：http://gj.muxihuayi.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://nw.hnjuh.cn

[Q31] 分组后过滤
来源：http://cy.huixinmuqiang.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mm.yuntaijiaju.cn

[Q32] 分组拼接字符串
来源：http://yw.bjjhwx.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://uj.newstarts.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://la.hahajie.cn

[Q33] 多列分组
来源：http://jm.asd995.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://bt.bookmarksfly.cn

[Q34] 每组取第一条
来源：http://ru.shtwfgs.cn

SELECT * FROM (
来源：http://ha.newstarts.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://zg.szxytkj.cn

) t WHERE rn = 1;
来源：http://au.shtwfgs.cn

[Q35] 内连接
来源：http://na.huixiangedu.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://kc.bjjhwx.cn

[Q36] 左连接
来源：http://df.nicolike.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://xk.yuexingan06.cn

[Q37] 右连接
来源：http://an.newstarts.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://gd.shtwfgs.cn

[Q38] 全外连接（PostgreSQL）
来源：http://xk.jctech888.com.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://oi.huixinmuqiang.cn

[Q39] 自连接（查上下级）
来源：http://oa.521024.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://fo.521024.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://es.haigaiapp.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://ya.jianghongdianzi.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://vg.panjiajie.cn

[Q41] 多表连接
来源：http://qq.huixinmuqiang.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://ua.muxihuayi.cn

JOIN users u ON u.id = o.user_id
来源：http://vz.jianghongdianzi.cn

JOIN products p ON p.id = o.product_id;
来源：http://iu.huanxung.cn

[Q42] 连接条件附加过滤
来源：http://lw.huixinmuqiang.cn

SELECT u.name, o.amount FROM users u
来源：http://xe.shxzskj.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ex.lnxyls.cn

[Q43] 标量子查询
来源：http://sh.bookmarksfly.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://yn.huixinmuqiang.cn

[Q44] IN 子查询
来源：http://ux.bookmarksfly.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://vo.shxzukj.cn

[Q45] EXISTS 判断存在
来源：http://to.gzmigu.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://nn.jianghongdianzi.cn

[Q46] NOT EXISTS 判断不存在
来源：http://bt.9csxet.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://zq.9csxet.cn

[Q47] 与平均值比较
来源：http://wb.lnxyls.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ea.muxihuayi.cn

[Q48] CTE 公用表表达式
来源：http://be.szxytkj.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://zq.wgjwhj.cn

SELECT * FROM t WHERE c > 5;
来源：http://rz.huixinmuqiang.cn

[Q49] 更新单行
来源：http://xm.szsharing.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mf.newstarts.cn

[Q50] 批量更新
来源：http://zp.jianghongdianzi.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://lv.panjiajie.cn

[Q51] 用子查询更新
来源：http://fl.yuexingan06.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://vc.521024.cn

[Q52] 删除指定行
来源：http://zk.newstarts.cn

DELETE FROM users WHERE id = 10;
来源：http://ha.jctech888.com.cn

[Q53] 按条件删除
来源：http://tm.huixiangedu.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://lr.panjiajie.cn

[Q54] 清空表
来源：http://km.chemitech.net.cn

TRUNCATE TABLE logs;
来源：http://bl.jianghongdianzi.cn

[Q55] 排名（并列占位）
来源：http://uy.haigaiapp.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://my.shtwfgs.cn

[Q56] 密集排名（并列不占位）
来源：http://mk.bjjhwx.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://da.hahajie.cn

[Q57] 行号
来源：http://ve.yuexingan06.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://jh.colortex.cn

[Q58] 累计求和
来源：http://yo.szxytkj.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://qq.panjiajie.cn

[Q59] 分组内累计
来源：http://vp.huixinmuqiang.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://lj.muxihuayi.cn

[Q60] 取上一行 / 下一行
来源：http://hk.bookmarksfly.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://je.hahajie.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://fo.nicolike.cn

[Q61] 移动平均
来源：http://jg.panjiajie.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://vy.huanxung.cn

[Q62] 分组占比
来源：http://rm.nicolike.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://pc.newstarts.cn

[Q63] 开启事务
来源：http://oa.chemitech.net.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://sk.hahajie.cn

[Q64] 提交事务
来源：http://di.haigaiapp.cn

COMMIT;
来源：http://rd.hahajie.cn

[Q65] 回滚事务
来源：http://ej.gzmigu.cn

ROLLBACK;
来源：http://go.shxzukj.cn

[Q66] 行锁查询
来源：http://bw.chemitech.net.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://sy.szxytkj.cn

[Q67] 设置隔离级别
来源：http://wm.nicolike.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://qk.szsharing.cn

[Q68] 保存点
来源：http://ww.huixiangedu.cn

SAVEPOINT sp1;
来源：http://mc.panjiajie.cn

ROLLBACK TO sp1;
来源：http://lu.shtwfgs.cn

[Q69] 查看执行计划
来源：http://rk.huanxung.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://cg.gzmigu.cn

[Q70] 更新统计信息
来源：http://dg.yuexingan06.cn

ANALYZE TABLE users;
来源：http://px.jctech888.com.cn

[Q71] 查看建表语句
来源：http://cb.bjjhwx.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hp.bookmarksfly.cn

[Q72] 查看索引
来源：http://np.hahajie.cn

SHOW INDEX FROM users;
来源：http://rt.yuntaijiaju.cn

[Q73] 查看表状态
来源：http://yb.bookmarksfly.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://fh.nszjky.cn

[Q74] 强制使用索引
来源：http://zu.muxihuayi.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://af.wgjwhj.cn

[Q75] 日期格式化
来源：http://qo.shtwfgs.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mt.muxihuayi.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://kv.521024.cn

[Q76] 按天统计
来源：http://pf.huixiangedu.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://la.bjjhwx.cn

[Q77] 时间加减
来源：http://oa.nszjky.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://nr.gzmigu.cn

[Q78] 当前时间
来源：http://pr.huixiangedu.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mj.newstarts.cn

[Q79] 字符串拼接
来源：http://zh.nicolike.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://fm.shtwfgs.cn

[Q80] 字符串截取
来源：http://ii.nszjky.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://qg.jctech888.com.cn

[Q81] 字符串替换
来源：http://xr.huanxung.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wx.jianghongdianzi.cn

[Q82] 字符长度与字节长度
来源：http://up.szxytkj.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://pd.gzmigu.cn

[Q83] 大小写转换
来源：http://wo.colortex.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ut.lnxyls.cn

[Q84] 去除首尾空格
来源：http://dj.asd995.cn

SELECT TRIM(name) FROM users;
来源：http://ag.asd995.cn

[Q85] 数值取整
来源：http://br.yuexingan06.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://jl.nszjky.cn

[Q86] 读取 JSON 字段
来源：http://ju.colortex.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://my.szxytkj.cn

[Q87] JSON 字段做条件
来源：http://ii.chemitech.net.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://pq.hnjuh.cn

[Q88] 行转列（条件聚合）
来源：http://us.nicolike.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hb.shxzukj.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mm.yuntaijiaju.cn

[Q89] 判断表是否存在
来源：http://rk.9csxet.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://il.chemitech.net.cn

[Q90] 生成序号列
来源：http://bk.huixiangedu.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://dl.huixinmuqiang.cn

================================================================================
来源：http://mt.shxzukj.cn

R. Bash 专题
来源：http://mi.yuexingan06.cn

================================================================================
来源：http://vx.panjiajie.cn

[R01] shebang 与严格模式
来源：http://ch.haigaiapp.cn

#!/usr/bin/env bash
来源：http://ja.jianghongdianzi.cn

set -euo pipefail
来源：http://yy.nicolike.cn

[R02] 变量赋值与使用
来源：http://kp.jianghongdianzi.cn

name="Tom"; echo "$name"
来源：http://po.9csxet.cn

[R03] 只读变量
来源：http://ud.haigaiapp.cn

readonly PI=3.14
来源：http://qf.newstarts.cn

[R04] 位置参数
来源：http://jd.shtwfgs.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://nf.nszjky.cn

[R05] 参数默认值
来源：http://wj.newstarts.cn

name="${1:-default}"
来源：http://ff.colortex.cn

[R06] 判断命令是否存在
来源：http://df.muxihuayi.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://bx.yuntaijiaju.cn

[R07] if 判断文件
来源：http://yr.huixinmuqiang.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://np.yuexingan06.cn

[R08] 数值比较
来源：http://yc.szsharing.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://gk.nszjky.cn

[R09] 字符串比较
来源：http://cm.haigaiapp.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://dn.haigaiapp.cn

[R10] 正则匹配
来源：http://fr.hahajie.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ev.9csxet.cn

[R11] case 多分支
来源：http://um.hnjuh.cn

case "$1" in
来源：http://mx.shxzukj.cn

start) echo "启动" ;;
来源：http://sn.newstarts.cn

stop)  echo "停止" ;;
来源：http://gt.shtwfgs.cn

*)     echo "未知命令" ;;
来源：http://kb.nszjky.cn

esac
来源：http://rz.huixiangedu.cn

[R12] for 遍历文件
来源：http://mw.yuexingan06.cn

for f in *.txt; do echo "$f"; done
来源：http://sj.shxzskj.cn

[R13] for 计数循环
来源：http://nv.shxzukj.cn


<!-- 参考信息 -->