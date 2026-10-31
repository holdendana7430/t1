代发 wailian999

Ruby: Digest::SHA256.hexdigest(s)
来源：http://fn.colortex.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://cf.hnjuh.cn

[P03] 生成短随机字符串
来源：http://lo.haigaiapp.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://vo.muxihuayi.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://cl.szsharing.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://rp.wgjwhj.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://vc.bookmarksfly.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ia.jctech888.com.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://nd.wgjwhj.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://bu.chemitech.net.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://gl.gzmigu.cn

[P04] 求长度
来源：http://mr.9csxet.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://nv.nszjky.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://qu.hahajie.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ok.gzmigu.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mu.wgjwhj.cn

Java: list.size();  map.size();  s.length()
来源：http://da.jianghongdianzi.cn

Go:   len(arr);  len(m)
来源：http://nl.hahajie.cn

Ruby: x.length;  x.size
来源：http://ub.muxihuayi.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://vl.lnxyls.cn

[P05] 判断两个对象内容是否相等
来源：http://ct.huixiangedu.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://os.jctech888.com.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://uf.shxzskj.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://uw.szxytkj.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://vw.nszjky.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mq.hahajie.cn

Go:   reflect.DeepEqual(a, b)
来源：http://aw.nicolike.cn

Ruby: a == b
来源：http://hw.szxytkj.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wl.bookmarksfly.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://qq.szsharing.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://om.huanxung.cn

PHP:  if (empty($x)) {}
来源：http://os.hnjuh.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://cw.jctech888.com.cn

TS:   if (x == null) {}
来源：http://gl.521024.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://pi.newstarts.cn

Go:   if x == nil {}
来源：http://eo.lnxyls.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://qn.521024.cn

C#:   if (x is null) {}
来源：http://sb.wgjwhj.cn

[P07] 防抖与节流
来源：http://vl.jctech888.com.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hk.shxzukj.cn

PHP:  // 手写时间戳比较
来源：http://yd.jianghongdianzi.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://fi.bjjhwx.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xj.huixinmuqiang.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wh.jctech888.com.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hb.bjjhwx.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://ax.wgjwhj.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://rf.9csxet.cn

[P08] 处理浮点精度问题
来源：http://vt.wgjwhj.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wi.lnxyls.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ya.shxzukj.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://zq.yuntaijiaju.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://vt.muxihuayi.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ae.nszjky.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://bp.yuexingan06.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ea.huanxung.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://dg.gzmigu.cn

================================================================================
来源：http://ug.9csxet.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://gs.jctech888.com.cn

================================================================================
来源：http://ls.shtwfgs.cn

[Q01] 创建表
来源：http://wy.nicolike.cn

CREATE TABLE users (
来源：http://gj.haigaiapp.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://yg.yuntaijiaju.cn

name VARCHAR(50) NOT NULL,
来源：http://nz.9csxet.cn

email VARCHAR(100) UNIQUE,
来源：http://hr.szsharing.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hk.hnjuh.cn

);
来源：http://db.hnjuh.cn

[Q02] 创建带外键的表
来源：http://qm.gzmigu.cn

CREATE TABLE orders (
来源：http://pl.huanxung.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://py.hnjuh.cn

user_id INT NOT NULL,
来源：http://cx.jianghongdianzi.cn

amount DECIMAL(10, 2),
来源：http://ax.hahajie.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wx.huixinmuqiang.cn

);
来源：http://db.panjiajie.cn

[Q03] 增加列
来源：http://iz.9csxet.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://gp.wgjwhj.cn

[Q04] 修改列类型
来源：http://kp.panjiajie.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://kj.huixinmuqiang.cn

[Q05] 重命名列
来源：http://ej.lnxyls.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://pz.yuntaijiaju.cn

[Q06] 删除列
来源：http://qb.colortex.cn

ALTER TABLE users DROP COLUMN age;
来源：http://rm.huixiangedu.cn

[Q07] 删除表
来源：http://bp.521024.cn

DROP TABLE IF EXISTS orders;
来源：http://la.gzmigu.cn

[Q08] 创建普通索引
来源：http://gw.shtwfgs.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://bo.huixinmuqiang.cn

[Q09] 创建唯一索引
来源：http://fz.nszjky.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://sc.yuntaijiaju.cn

[Q10] 插入单行
来源：http://fe.yuntaijiaju.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://vq.shxzskj.cn

[Q11] 一次插入多行
来源：http://ml.shxzukj.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://je.shxzskj.cn

[Q12] 插入后取自增 ID
来源：http://mj.yuexingan06.cn

INSERT INTO users (name) VALUES ('C');
来源：http://eh.gzmigu.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://vt.jianghongdianzi.cn

[Q13] 忽略重复插入
来源：http://fk.asd995.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://de.shxzukj.cn

[Q14] 存在则更新（upsert）
来源：http://sv.colortex.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ww.bjjhwx.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://xg.yuntaijiaju.cn

[Q15] 查询全部
来源：http://eq.hahajie.cn

SELECT * FROM users;
来源：http://mr.szsharing.cn

[Q16] 查询指定列
来源：http://xw.hahajie.cn

SELECT id, name FROM users;
来源：http://cr.gzmigu.cn

[Q17] 条件查询
来源：http://xo.wgjwhj.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://dj.colortex.cn

[Q18] 模糊匹配
来源：http://lj.hahajie.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mx.bookmarksfly.cn

[Q19] 范围查询
来源：http://bc.bookmarksfly.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://jm.huanxung.cn

[Q20] IN 列表
来源：http://sg.lnxyls.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://xs.lnxyls.cn

[Q21] 空值判断
来源：http://iq.jianghongdianzi.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://dy.muxihuayi.cn

[Q22] 排序
来源：http://hw.huanxung.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://uc.panjiajie.cn

[Q23] 分页
来源：http://yg.gzmigu.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://lk.nszjky.cn

[Q24] 去重
来源：http://oy.jianghongdianzi.cn

SELECT DISTINCT city FROM users;
来源：http://ps.panjiajie.cn

[Q25] 只取前 N 条
来源：http://pv.newstarts.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://kk.colortex.cn

[Q26] 计数
来源：http://jv.szxytkj.cn

SELECT COUNT(*) FROM users;
来源：http://zf.shxzukj.cn

[Q27] 条件计数
来源：http://pn.huanxung.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ic.huixiangedu.cn

[Q28] 求和与平均
来源：http://wl.muxihuayi.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://sx.bookmarksfly.cn

[Q29] 最大最小值
来源：http://sc.huixinmuqiang.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://um.bookmarksfly.cn

[Q30] 分组统计
来源：http://we.shtwfgs.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ql.szsharing.cn

[Q31] 分组后过滤
来源：http://ax.huixiangedu.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://gu.jctech888.com.cn

[Q32] 分组拼接字符串
来源：http://dr.9csxet.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://oz.wgjwhj.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://on.shxzskj.cn

[Q33] 多列分组
来源：http://or.bookmarksfly.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://iw.muxihuayi.cn

[Q34] 每组取第一条
来源：http://nn.muxihuayi.cn

SELECT * FROM (
来源：http://ul.jctech888.com.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ua.jctech888.com.cn

) t WHERE rn = 1;
来源：http://pi.yuexingan06.cn

[Q35] 内连接
来源：http://aa.gzmigu.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://bg.huanxung.cn

[Q36] 左连接
来源：http://vd.nicolike.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ho.hnjuh.cn

[Q37] 右连接
来源：http://od.nicolike.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://zs.bjjhwx.cn

[Q38] 全外连接（PostgreSQL）
来源：http://ok.yuexingan06.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wo.jctech888.com.cn

[Q39] 自连接（查上下级）
来源：http://si.huixinmuqiang.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://fm.521024.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://vz.huixinmuqiang.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://ef.hahajie.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://sn.9csxet.cn

[Q41] 多表连接
来源：http://cn.huixinmuqiang.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://pt.bjjhwx.cn

JOIN users u ON u.id = o.user_id
来源：http://un.chemitech.net.cn

JOIN products p ON p.id = o.product_id;
来源：http://qo.newstarts.cn

[Q42] 连接条件附加过滤
来源：http://no.colortex.cn

SELECT u.name, o.amount FROM users u
来源：http://ap.nszjky.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://gs.shtwfgs.cn

[Q43] 标量子查询
来源：http://op.huixiangedu.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://vr.chemitech.net.cn

[Q44] IN 子查询
来源：http://lw.szsharing.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mr.shxzskj.cn

[Q45] EXISTS 判断存在
来源：http://zu.wgjwhj.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://bl.hnjuh.cn

[Q46] NOT EXISTS 判断不存在
来源：http://qo.gzmigu.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://eq.521024.cn

[Q47] 与平均值比较
来源：http://ts.chemitech.net.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hv.szxytkj.cn

[Q48] CTE 公用表表达式
来源：http://zf.bookmarksfly.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://bz.gzmigu.cn

SELECT * FROM t WHERE c > 5;
来源：http://lg.panjiajie.cn

[Q49] 更新单行
来源：http://qt.haigaiapp.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ce.bjjhwx.cn

[Q50] 批量更新
来源：http://st.bjjhwx.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://eg.wgjwhj.cn

[Q51] 用子查询更新
来源：http://fs.szxytkj.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://rp.yuntaijiaju.cn

[Q52] 删除指定行
来源：http://uw.chemitech.net.cn

DELETE FROM users WHERE id = 10;
来源：http://vh.chemitech.net.cn

[Q53] 按条件删除
来源：http://ow.panjiajie.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ma.wgjwhj.cn

[Q54] 清空表
来源：http://dg.bookmarksfly.cn

TRUNCATE TABLE logs;
来源：http://xk.jianghongdianzi.cn

[Q55] 排名（并列占位）
来源：http://sp.szsharing.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://os.yuexingan06.cn

[Q56] 密集排名（并列不占位）
来源：http://py.shtwfgs.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://vu.shxzukj.cn

[Q57] 行号
来源：http://rf.shxzskj.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ub.nszjky.cn

[Q58] 累计求和
来源：http://wq.9csxet.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://vt.jianghongdianzi.cn

[Q59] 分组内累计
来源：http://ko.9csxet.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://tl.yuexingan06.cn

[Q60] 取上一行 / 下一行
来源：http://ni.newstarts.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hi.hahajie.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://bc.szsharing.cn

[Q61] 移动平均
来源：http://ul.jctech888.com.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://sm.szxytkj.cn

[Q62] 分组占比
来源：http://hw.lnxyls.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://zv.yuexingan06.cn

[Q63] 开启事务
来源：http://wh.hahajie.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://pu.jctech888.com.cn

[Q64] 提交事务
来源：http://lo.yuexingan06.cn

COMMIT;
来源：http://os.muxihuayi.cn

[Q65] 回滚事务
来源：http://yt.nszjky.cn

ROLLBACK;
来源：http://uz.panjiajie.cn

[Q66] 行锁查询
来源：http://rl.shxzskj.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://fu.muxihuayi.cn

[Q67] 设置隔离级别
来源：http://ms.chemitech.net.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mk.lnxyls.cn

[Q68] 保存点
来源：http://do.szxytkj.cn

SAVEPOINT sp1;
来源：http://ld.szsharing.cn

ROLLBACK TO sp1;
来源：http://ib.huixinmuqiang.cn

[Q69] 查看执行计划
来源：http://mi.shxzukj.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://rk.huanxung.cn

[Q70] 更新统计信息
来源：http://ra.hahajie.cn

ANALYZE TABLE users;
来源：http://nn.szsharing.cn

[Q71] 查看建表语句
来源：http://bl.shtwfgs.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hm.szxytkj.cn

[Q72] 查看索引
来源：http://ea.muxihuayi.cn

SHOW INDEX FROM users;
来源：http://om.nszjky.cn

[Q73] 查看表状态
来源：http://hi.muxihuayi.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://pj.9csxet.cn

[Q74] 强制使用索引
来源：http://lx.haigaiapp.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://jj.wgjwhj.cn

[Q75] 日期格式化
来源：http://wr.gzmigu.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ua.muxihuayi.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://it.lnxyls.cn

[Q76] 按天统计
来源：http://ff.asd995.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ln.jctech888.com.cn

[Q77] 时间加减
来源：http://gv.9csxet.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://fj.newstarts.cn

[Q78] 当前时间
来源：http://wk.huixiangedu.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://fl.shtwfgs.cn

[Q79] 字符串拼接
来源：http://ao.panjiajie.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://cc.newstarts.cn

[Q80] 字符串截取
来源：http://xw.panjiajie.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wj.gzmigu.cn

[Q81] 字符串替换
来源：http://wr.szxytkj.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://oq.wgjwhj.cn

[Q82] 字符长度与字节长度
来源：http://jn.hahajie.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://xq.bjjhwx.cn

[Q83] 大小写转换
来源：http://bz.huixinmuqiang.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://cq.jianghongdianzi.cn

[Q84] 去除首尾空格
来源：http://ep.nszjky.cn

SELECT TRIM(name) FROM users;
来源：http://kj.lnxyls.cn

[Q85] 数值取整
来源：http://in.hahajie.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://gg.panjiajie.cn

[Q86] 读取 JSON 字段
来源：http://dz.colortex.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://rj.yuntaijiaju.cn

[Q87] JSON 字段做条件
来源：http://by.muxihuayi.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://uu.panjiajie.cn

[Q88] 行转列（条件聚合）
来源：http://pe.jctech888.com.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://yj.huixiangedu.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ds.hnjuh.cn

[Q89] 判断表是否存在
来源：http://vz.nszjky.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://zw.hnjuh.cn

[Q90] 生成序号列
来源：http://as.bookmarksfly.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://zm.huanxung.cn

================================================================================
来源：http://vq.shxzukj.cn

R. Bash 专题
来源：http://pg.hahajie.cn

================================================================================
来源：http://cm.yuntaijiaju.cn

[R01] shebang 与严格模式
来源：http://ec.huixiangedu.cn

#!/usr/bin/env bash
来源：http://vm.nicolike.cn

set -euo pipefail
来源：http://tn.haigaiapp.cn

[R02] 变量赋值与使用
来源：http://hr.yuntaijiaju.cn

name="Tom"; echo "$name"
来源：http://cn.panjiajie.cn

[R03] 只读变量
来源：http://to.shtwfgs.cn

readonly PI=3.14
来源：http://vz.shtwfgs.cn

[R04] 位置参数
来源：http://ws.gzmigu.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://io.chemitech.net.cn

[R05] 参数默认值
来源：http://gy.wgjwhj.cn

name="${1:-default}"
来源：http://xm.shxzukj.cn

[R06] 判断命令是否存在
来源：http://zq.hnjuh.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ki.jianghongdianzi.cn

[R07] if 判断文件
来源：http://cf.huixiangedu.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://nw.asd995.cn

[R08] 数值比较
来源：http://ed.szxytkj.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://wa.lnxyls.cn

[R09] 字符串比较
来源：http://dy.9csxet.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ne.lnxyls.cn

[R10] 正则匹配
来源：http://dc.szsharing.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://fg.521024.cn

[R11] case 多分支
来源：http://fo.haigaiapp.cn

case "$1" in
来源：http://lo.shxzskj.cn

start) echo "启动" ;;
来源：http://vr.hahajie.cn

stop)  echo "停止" ;;
来源：http://ts.huanxung.cn

*)     echo "未知命令" ;;
来源：http://on.nicolike.cn

esac
来源：http://dx.bjjhwx.cn

[R12] for 遍历文件
来源：http://ls.hnjuh.cn

for f in *.txt; do echo "$f"; done
来源：http://it.gzmigu.cn

[R13] for 计数循环
来源：http://us.muxihuayi.cn

for i in {1..10}; do echo "$i"; done
来源：http://qr.chemitech.net.cn

[R14] C 风格 for
来源：http://gh.asd995.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://cc.muxihuayi.cn

[R15] while 逐行读文件
来源：http://vo.huixiangedu.cn


<!-- 参考信息 -->