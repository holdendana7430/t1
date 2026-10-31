代发 wailian999

Ruby: Digest::SHA256.hexdigest(s)
来源：http://dl.colortex.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://dg.huixiangedu.cn

[P03] 生成短随机字符串
来源：http://ff.9csxet.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://qn.huanxung.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ec.chemitech.net.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://yj.newstarts.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://jm.newstarts.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://la.asd995.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ld.hnjuh.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://jk.szxytkj.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://kf.gzmigu.cn

[P04] 求长度
来源：http://go.wgjwhj.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://qm.haigaiapp.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ll.shxzukj.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://zx.shtwfgs.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://tf.szsharing.cn

Java: list.size();  map.size();  s.length()
来源：http://yw.yuexingan06.cn

Go:   len(arr);  len(m)
来源：http://qb.wgjwhj.cn

Ruby: x.length;  x.size
来源：http://vs.szsharing.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://op.bookmarksfly.cn

[P05] 判断两个对象内容是否相等
来源：http://xs.szsharing.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://lp.9csxet.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://vx.shxzskj.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ff.bjjhwx.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://tn.nicolike.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://bw.muxihuayi.cn

Go:   reflect.DeepEqual(a, b)
来源：http://xi.szxytkj.cn

Ruby: a == b
来源：http://mq.lnxyls.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://vf.hahajie.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://nw.newstarts.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ew.szxytkj.cn

PHP:  if (empty($x)) {}
来源：http://kk.nszjky.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://kk.hahajie.cn

TS:   if (x == null) {}
来源：http://tv.521024.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://ok.haigaiapp.cn

Go:   if x == nil {}
来源：http://hz.newstarts.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://xh.9csxet.cn

C#:   if (x is null) {}
来源：http://eg.jctech888.com.cn

[P07] 防抖与节流
来源：http://gy.wgjwhj.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://lb.haigaiapp.cn

PHP:  // 手写时间戳比较
来源：http://cn.hahajie.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://no.muxihuayi.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://co.hnjuh.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ez.shtwfgs.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://yw.nszjky.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://la.bookmarksfly.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.huanxung.cn

[P08] 处理浮点精度问题
来源：http://yb.shtwfgs.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://uz.huixiangedu.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://yn.jctech888.com.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://er.szxytkj.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://vx.nszjky.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://du.colortex.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://jc.521024.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hy.shxzukj.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hk.jianghongdianzi.cn

================================================================================
来源：http://yo.yuexingan06.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://tk.nszjky.cn

================================================================================
来源：http://eg.9csxet.cn

[Q01] 创建表
来源：http://rp.chemitech.net.cn

CREATE TABLE users (
来源：http://fv.szxytkj.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://vb.shxzskj.cn

name VARCHAR(50) NOT NULL,
来源：http://la.nicolike.cn

email VARCHAR(100) UNIQUE,
来源：http://eu.szxytkj.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://el.yuexingan06.cn

);
来源：http://em.muxihuayi.cn

[Q02] 创建带外键的表
来源：http://tg.szsharing.cn

CREATE TABLE orders (
来源：http://sw.hahajie.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hq.huixiangedu.cn

user_id INT NOT NULL,
来源：http://nl.shxzukj.cn

amount DECIMAL(10, 2),
来源：http://nq.9csxet.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://sk.jctech888.com.cn

);
来源：http://bu.huixinmuqiang.cn

[Q03] 增加列
来源：http://co.lnxyls.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wk.9csxet.cn

[Q04] 修改列类型
来源：http://ma.panjiajie.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://gq.haigaiapp.cn

[Q05] 重命名列
来源：http://cn.asd995.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://my.huanxung.cn

[Q06] 删除列
来源：http://vo.9csxet.cn

ALTER TABLE users DROP COLUMN age;
来源：http://ft.jianghongdianzi.cn

[Q07] 删除表
来源：http://cf.shxzukj.cn

DROP TABLE IF EXISTS orders;
来源：http://tl.szsharing.cn

[Q08] 创建普通索引
来源：http://py.haigaiapp.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://ek.szxytkj.cn

[Q09] 创建唯一索引
来源：http://fd.szsharing.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://yl.huixinmuqiang.cn

[Q10] 插入单行
来源：http://qg.szxytkj.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://lk.huixinmuqiang.cn

[Q11] 一次插入多行
来源：http://wj.9csxet.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://uu.lnxyls.cn

[Q12] 插入后取自增 ID
来源：http://cz.haigaiapp.cn

INSERT INTO users (name) VALUES ('C');
来源：http://hh.shxzskj.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://kz.nszjky.cn

[Q13] 忽略重复插入
来源：http://qx.muxihuayi.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://qd.shxzskj.cn

[Q14] 存在则更新（upsert）
来源：http://na.jianghongdianzi.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://yj.jctech888.com.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ev.yuntaijiaju.cn

[Q15] 查询全部
来源：http://io.gzmigu.cn

SELECT * FROM users;
来源：http://zs.nicolike.cn

[Q16] 查询指定列
来源：http://sb.shxzukj.cn

SELECT id, name FROM users;
来源：http://dt.shxzskj.cn

[Q17] 条件查询
来源：http://fl.jctech888.com.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://vv.9csxet.cn

[Q18] 模糊匹配
来源：http://ge.shtwfgs.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://yi.szxytkj.cn

[Q19] 范围查询
来源：http://qq.nszjky.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://qo.huanxung.cn

[Q20] IN 列表
来源：http://th.521024.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://vj.szxytkj.cn

[Q21] 空值判断
来源：http://kd.asd995.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://hx.bookmarksfly.cn

[Q22] 排序
来源：http://hi.bjjhwx.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://vd.gzmigu.cn

[Q23] 分页
来源：http://ey.hnjuh.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://nc.panjiajie.cn

[Q24] 去重
来源：http://cz.lnxyls.cn

SELECT DISTINCT city FROM users;
来源：http://av.chemitech.net.cn

[Q25] 只取前 N 条
来源：http://jh.yuntaijiaju.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wu.wgjwhj.cn

[Q26] 计数
来源：http://hh.colortex.cn

SELECT COUNT(*) FROM users;
来源：http://uf.panjiajie.cn

[Q27] 条件计数
来源：http://wn.yuntaijiaju.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://al.nicolike.cn

[Q28] 求和与平均
来源：http://sc.huixinmuqiang.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://sr.wgjwhj.cn

[Q29] 最大最小值
来源：http://nq.bjjhwx.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://vg.jctech888.com.cn

[Q30] 分组统计
来源：http://ks.shtwfgs.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://im.wgjwhj.cn

[Q31] 分组后过滤
来源：http://gv.yuexingan06.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://uq.panjiajie.cn

[Q32] 分组拼接字符串
来源：http://vu.hnjuh.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://xe.shtwfgs.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wn.shxzukj.cn

[Q33] 多列分组
来源：http://yc.newstarts.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://xc.newstarts.cn

[Q34] 每组取第一条
来源：http://gy.szxytkj.cn

SELECT * FROM (
来源：http://ce.bookmarksfly.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://un.huixinmuqiang.cn

) t WHERE rn = 1;
来源：http://nw.huixiangedu.cn

[Q35] 内连接
来源：http://pp.nszjky.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hk.nicolike.cn

[Q36] 左连接
来源：http://sx.shtwfgs.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://nu.gzmigu.cn

[Q37] 右连接
来源：http://zd.newstarts.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://yn.muxihuayi.cn

[Q38] 全外连接（PostgreSQL）
来源：http://kd.bookmarksfly.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://oq.yuntaijiaju.cn

[Q39] 自连接（查上下级）
来源：http://ts.gzmigu.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://gn.yuntaijiaju.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://kb.yuexingan06.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://ab.shxzukj.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://kq.muxihuayi.cn

[Q41] 多表连接
来源：http://vj.lnxyls.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://tj.newstarts.cn

JOIN users u ON u.id = o.user_id
来源：http://nf.huixiangedu.cn

JOIN products p ON p.id = o.product_id;
来源：http://ww.szsharing.cn

[Q42] 连接条件附加过滤
来源：http://qy.521024.cn

SELECT u.name, o.amount FROM users u
来源：http://uu.521024.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://dh.panjiajie.cn

[Q43] 标量子查询
来源：http://kr.newstarts.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://lj.asd995.cn

[Q44] IN 子查询
来源：http://sy.lnxyls.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ly.huixinmuqiang.cn

[Q45] EXISTS 判断存在
来源：http://lg.jctech888.com.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mp.haigaiapp.cn

[Q46] NOT EXISTS 判断不存在
来源：http://qi.yuntaijiaju.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://qg.wgjwhj.cn

[Q47] 与平均值比较
来源：http://rw.yuexingan06.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ej.szxytkj.cn

[Q48] CTE 公用表表达式
来源：http://gt.chemitech.net.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://tj.haigaiapp.cn

SELECT * FROM t WHERE c > 5;
来源：http://kg.huixiangedu.cn

[Q49] 更新单行
来源：http://hz.yuexingan06.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://fc.yuexingan06.cn

[Q50] 批量更新
来源：http://ls.shxzskj.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://fj.nszjky.cn

[Q51] 用子查询更新
来源：http://rl.gzmigu.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://lt.lnxyls.cn

[Q52] 删除指定行
来源：http://nx.shxzskj.cn

DELETE FROM users WHERE id = 10;
来源：http://ba.haigaiapp.cn

[Q53] 按条件删除
来源：http://wg.colortex.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ci.huixinmuqiang.cn

[Q54] 清空表
来源：http://eh.shtwfgs.cn

TRUNCATE TABLE logs;
来源：http://vk.newstarts.cn

[Q55] 排名（并列占位）
来源：http://en.nszjky.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://uy.huanxung.cn

[Q56] 密集排名（并列不占位）
来源：http://cw.shtwfgs.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://xy.muxihuayi.cn

[Q57] 行号
来源：http://bz.chemitech.net.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ez.szxytkj.cn

[Q58] 累计求和
来源：http://qz.gzmigu.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://gi.huixiangedu.cn

[Q59] 分组内累计
来源：http://uc.panjiajie.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://zh.huanxung.cn

[Q60] 取上一行 / 下一行
来源：http://mi.9csxet.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://va.huanxung.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://al.jctech888.com.cn

[Q61] 移动平均
来源：http://pt.haigaiapp.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ih.yuexingan06.cn

[Q62] 分组占比
来源：http://zs.muxihuayi.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://dz.nszjky.cn

[Q63] 开启事务
来源：http://rj.yuexingan06.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://ex.jctech888.com.cn

[Q64] 提交事务
来源：http://lu.muxihuayi.cn

COMMIT;
来源：http://cf.huanxung.cn

[Q65] 回滚事务
来源：http://vy.shxzskj.cn

ROLLBACK;
来源：http://af.nszjky.cn

[Q66] 行锁查询
来源：http://zz.panjiajie.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://cp.bookmarksfly.cn

[Q67] 设置隔离级别
来源：http://pr.huixinmuqiang.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://fe.521024.cn

[Q68] 保存点
来源：http://en.huixiangedu.cn

SAVEPOINT sp1;
来源：http://dq.lnxyls.cn

ROLLBACK TO sp1;
来源：http://wf.gzmigu.cn

[Q69] 查看执行计划
来源：http://ll.huanxung.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://dv.nicolike.cn

[Q70] 更新统计信息
来源：http://dc.yuexingan06.cn

ANALYZE TABLE users;
来源：http://hh.nszjky.cn

[Q71] 查看建表语句
来源：http://ln.newstarts.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ac.huixiangedu.cn

[Q72] 查看索引
来源：http://gd.jctech888.com.cn

SHOW INDEX FROM users;
来源：http://iw.huixinmuqiang.cn

[Q73] 查看表状态
来源：http://uy.shtwfgs.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://tx.wgjwhj.cn

[Q74] 强制使用索引
来源：http://ae.newstarts.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://uo.hahajie.cn

[Q75] 日期格式化
来源：http://vk.hahajie.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://zl.hnjuh.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://jb.521024.cn

[Q76] 按天统计
来源：http://et.nicolike.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ak.wgjwhj.cn

[Q77] 时间加减
来源：http://rm.newstarts.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wq.huixinmuqiang.cn

[Q78] 当前时间
来源：http://wf.hahajie.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://vf.shxzskj.cn

[Q79] 字符串拼接
来源：http://xc.yuexingan06.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://rn.huanxung.cn

[Q80] 字符串截取
来源：http://nu.huanxung.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://pi.shxzskj.cn

[Q81] 字符串替换
来源：http://ci.shxzukj.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://rq.nicolike.cn

[Q82] 字符长度与字节长度
来源：http://rb.muxihuayi.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://xa.jctech888.com.cn

[Q83] 大小写转换
来源：http://gk.bjjhwx.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://qh.bookmarksfly.cn

[Q84] 去除首尾空格
来源：http://pd.colortex.cn

SELECT TRIM(name) FROM users;
来源：http://qi.shxzskj.cn

[Q85] 数值取整
来源：http://oj.asd995.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ej.muxihuayi.cn

[Q86] 读取 JSON 字段
来源：http://pi.shxzskj.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://yg.szsharing.cn

[Q87] JSON 字段做条件
来源：http://pv.bjjhwx.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://xf.nicolike.cn

[Q88] 行转列（条件聚合）
来源：http://ka.huixiangedu.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ay.newstarts.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://sv.hahajie.cn

[Q89] 判断表是否存在
来源：http://aw.lnxyls.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://lq.huanxung.cn

[Q90] 生成序号列
来源：http://ic.jianghongdianzi.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://sy.asd995.cn

================================================================================
来源：http://ne.bjjhwx.cn

R. Bash 专题
来源：http://ts.9csxet.cn

================================================================================
来源：http://ap.9csxet.cn

[R01] shebang 与严格模式
来源：http://dm.szsharing.cn

#!/usr/bin/env bash
来源：http://su.jianghongdianzi.cn

set -euo pipefail
来源：http://vs.chemitech.net.cn

[R02] 变量赋值与使用
来源：http://rl.lnxyls.cn

name="Tom"; echo "$name"
来源：http://il.9csxet.cn

[R03] 只读变量
来源：http://ov.huixinmuqiang.cn

readonly PI=3.14
来源：http://en.9csxet.cn

[R04] 位置参数
来源：http://bx.newstarts.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wp.asd995.cn

[R05] 参数默认值
来源：http://ox.wgjwhj.cn

name="${1:-default}"
来源：http://xg.lnxyls.cn

[R06] 判断命令是否存在
来源：http://lf.shtwfgs.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://xd.szsharing.cn

[R07] if 判断文件
来源：http://lo.huixiangedu.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://if.lnxyls.cn

[R08] 数值比较
来源：http://mw.nicolike.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://mj.szxytkj.cn

[R09] 字符串比较
来源：http://pd.szsharing.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://kt.shxzukj.cn

[R10] 正则匹配
来源：http://hl.szxytkj.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://la.chemitech.net.cn

[R11] case 多分支
来源：http://el.yuntaijiaju.cn

case "$1" in
来源：http://pa.szxytkj.cn

start) echo "启动" ;;
来源：http://dh.newstarts.cn

stop)  echo "停止" ;;
来源：http://at.newstarts.cn

*)     echo "未知命令" ;;
来源：http://br.521024.cn

esac
来源：http://gk.newstarts.cn

[R12] for 遍历文件
来源：http://yl.lnxyls.cn

for f in *.txt; do echo "$f"; done
来源：http://jv.haigaiapp.cn

[R13] for 计数循环
来源：http://qq.wgjwhj.cn

for i in {1..10}; do echo "$i"; done
来源：http://ay.521024.cn

[R14] C 风格 for
来源：http://aq.nszjky.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://bz.jianghongdianzi.cn

[R15] while 逐行读文件
来源：http://se.shxzskj.cn


<!-- 参考信息 -->