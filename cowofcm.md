代发 wailian999

Ruby: Digest::SHA256.hexdigest(s)
来源：http://nj.gzmigu.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ok.9csxet.cn

[P03] 生成短随机字符串
来源：http://ij.newstarts.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://oq.asd995.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://gc.huixiangedu.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ah.521024.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://oc.jianghongdianzi.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ok.shtwfgs.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://nc.asd995.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://gc.9csxet.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://vm.jianghongdianzi.cn

[P04] 求长度
来源：http://gn.haigaiapp.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ls.chemitech.net.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://rk.hahajie.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ef.huixiangedu.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://uk.newstarts.cn

Java: list.size();  map.size();  s.length()
来源：http://xn.huixiangedu.cn

Go:   len(arr);  len(m)
来源：http://kn.hahajie.cn

Ruby: x.length;  x.size
来源：http://qh.bjjhwx.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://ok.bjjhwx.cn

[P05] 判断两个对象内容是否相等
来源：http://qe.521024.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://ms.huixinmuqiang.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://jj.haigaiapp.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ox.yuntaijiaju.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ug.asd995.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://jy.jianghongdianzi.cn

Go:   reflect.DeepEqual(a, b)
来源：http://zd.yuntaijiaju.cn

Ruby: a == b
来源：http://pm.nszjky.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wn.yuexingan06.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://fd.jctech888.com.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ep.colortex.cn

PHP:  if (empty($x)) {}
来源：http://to.hnjuh.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://oq.shxzskj.cn

TS:   if (x == null) {}
来源：http://pi.hnjuh.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://bm.jianghongdianzi.cn

Go:   if x == nil {}
来源：http://lq.bjjhwx.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://zu.shtwfgs.cn

C#:   if (x is null) {}
来源：http://xy.wgjwhj.cn

[P07] 防抖与节流
来源：http://ux.hnjuh.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://xc.nszjky.cn

PHP:  // 手写时间戳比较
来源：http://qp.521024.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://lt.nszjky.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wz.gzmigu.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://uw.newstarts.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ud.yuexingan06.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://ei.nicolike.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://po.bookmarksfly.cn

[P08] 处理浮点精度问题
来源：http://tu.huixinmuqiang.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://zh.colortex.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://jo.newstarts.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ng.nszjky.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ix.jianghongdianzi.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ob.gzmigu.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://nk.hnjuh.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ra.szsharing.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ch.huixinmuqiang.cn

================================================================================
来源：http://nt.hnjuh.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hm.szsharing.cn

================================================================================
来源：http://dm.szxytkj.cn

[Q01] 创建表
来源：http://pk.haigaiapp.cn

CREATE TABLE users (
来源：http://ml.szsharing.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://rw.wgjwhj.cn

name VARCHAR(50) NOT NULL,
来源：http://ie.haigaiapp.cn

email VARCHAR(100) UNIQUE,
来源：http://cl.shxzukj.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://bn.huanxung.cn

);
来源：http://ky.chemitech.net.cn

[Q02] 创建带外键的表
来源：http://wg.szsharing.cn

CREATE TABLE orders (
来源：http://mq.hnjuh.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://vu.shxzukj.cn

user_id INT NOT NULL,
来源：http://so.szxytkj.cn

amount DECIMAL(10, 2),
来源：http://wc.panjiajie.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ao.jianghongdianzi.cn

);
来源：http://tu.colortex.cn

[Q03] 增加列
来源：http://bh.lnxyls.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://cy.newstarts.cn

[Q04] 修改列类型
来源：http://qv.lnxyls.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://zr.asd995.cn

[Q05] 重命名列
来源：http://xz.wgjwhj.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://sc.lnxyls.cn

[Q06] 删除列
来源：http://xc.szsharing.cn

ALTER TABLE users DROP COLUMN age;
来源：http://ib.9csxet.cn

[Q07] 删除表
来源：http://my.jctech888.com.cn

DROP TABLE IF EXISTS orders;
来源：http://hq.newstarts.cn

[Q08] 创建普通索引
来源：http://ns.colortex.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://sy.szxytkj.cn

[Q09] 创建唯一索引
来源：http://cr.jianghongdianzi.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mr.asd995.cn

[Q10] 插入单行
来源：http://gm.newstarts.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://to.lnxyls.cn

[Q11] 一次插入多行
来源：http://kn.shtwfgs.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://im.yuexingan06.cn

[Q12] 插入后取自增 ID
来源：http://dq.muxihuayi.cn

INSERT INTO users (name) VALUES ('C');
来源：http://zi.newstarts.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://xa.9csxet.cn

[Q13] 忽略重复插入
来源：http://rj.hnjuh.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://nz.wgjwhj.cn

[Q14] 存在则更新（upsert）
来源：http://om.jianghongdianzi.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wk.newstarts.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://cn.yuntaijiaju.cn

[Q15] 查询全部
来源：http://iy.hahajie.cn

SELECT * FROM users;
来源：http://oo.jctech888.com.cn

[Q16] 查询指定列
来源：http://hk.jianghongdianzi.cn

SELECT id, name FROM users;
来源：http://ks.yuexingan06.cn

[Q17] 条件查询
来源：http://ni.chemitech.net.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mi.nszjky.cn

[Q18] 模糊匹配
来源：http://vz.panjiajie.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mf.newstarts.cn

[Q19] 范围查询
来源：http://ep.jianghongdianzi.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://xo.gzmigu.cn

[Q20] IN 列表
来源：http://lk.jctech888.com.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://lk.huixinmuqiang.cn

[Q21] 空值判断
来源：http://oo.jianghongdianzi.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://bu.hnjuh.cn

[Q22] 排序
来源：http://jy.huixiangedu.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://bj.yuexingan06.cn

[Q23] 分页
来源：http://fo.jctech888.com.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://zh.chemitech.net.cn

[Q24] 去重
来源：http://on.yuntaijiaju.cn

SELECT DISTINCT city FROM users;
来源：http://va.bjjhwx.cn

[Q25] 只取前 N 条
来源：http://ir.nicolike.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://yg.muxihuayi.cn

[Q26] 计数
来源：http://la.jianghongdianzi.cn

SELECT COUNT(*) FROM users;
来源：http://bu.haigaiapp.cn

[Q27] 条件计数
来源：http://rf.hnjuh.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://tw.muxihuayi.cn

[Q28] 求和与平均
来源：http://lb.huanxung.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wu.huixiangedu.cn

[Q29] 最大最小值
来源：http://jq.nicolike.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://fr.jctech888.com.cn

[Q30] 分组统计
来源：http://mz.jianghongdianzi.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://an.nicolike.cn

[Q31] 分组后过滤
来源：http://sg.gzmigu.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ly.bjjhwx.cn

[Q32] 分组拼接字符串
来源：http://ej.jctech888.com.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://vy.gzmigu.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://pj.muxihuayi.cn

[Q33] 多列分组
来源：http://ss.szxytkj.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://xg.9csxet.cn

[Q34] 每组取第一条
来源：http://oz.nszjky.cn

SELECT * FROM (
来源：http://os.chemitech.net.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://gx.gzmigu.cn

) t WHERE rn = 1;
来源：http://qg.muxihuayi.cn

[Q35] 内连接
来源：http://ap.lnxyls.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://my.yuntaijiaju.cn

[Q36] 左连接
来源：http://bl.panjiajie.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://nr.jianghongdianzi.cn

[Q37] 右连接
来源：http://fq.asd995.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wl.shtwfgs.cn

[Q38] 全外连接（PostgreSQL）
来源：http://do.shxzukj.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ir.asd995.cn

[Q39] 自连接（查上下级）
来源：http://su.shtwfgs.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://jl.panjiajie.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://tn.jianghongdianzi.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://kj.lnxyls.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://jj.hahajie.cn

[Q41] 多表连接
来源：http://ts.bjjhwx.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://uw.jianghongdianzi.cn

JOIN users u ON u.id = o.user_id
来源：http://gc.9csxet.cn

JOIN products p ON p.id = o.product_id;
来源：http://zi.jianghongdianzi.cn

[Q42] 连接条件附加过滤
来源：http://fh.szsharing.cn

SELECT u.name, o.amount FROM users u
来源：http://iw.jctech888.com.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hk.lnxyls.cn

[Q43] 标量子查询
来源：http://eo.chemitech.net.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://tm.hahajie.cn

[Q44] IN 子查询
来源：http://zg.shtwfgs.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://pn.szxytkj.cn

[Q45] EXISTS 判断存在
来源：http://me.huanxung.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mz.yuntaijiaju.cn

[Q46] NOT EXISTS 判断不存在
来源：http://yt.shxzukj.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://fx.nszjky.cn

[Q47] 与平均值比较
来源：http://vv.hnjuh.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://xv.bookmarksfly.cn

[Q48] CTE 公用表表达式
来源：http://qh.9csxet.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://au.huanxung.cn

SELECT * FROM t WHERE c > 5;
来源：http://hp.huixiangedu.cn

[Q49] 更新单行
来源：http://fq.muxihuayi.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://fh.huanxung.cn

[Q50] 批量更新
来源：http://qi.9csxet.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://ex.bookmarksfly.cn

[Q51] 用子查询更新
来源：http://qx.shxzukj.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wj.bookmarksfly.cn

[Q52] 删除指定行
来源：http://ny.huixiangedu.cn

DELETE FROM users WHERE id = 10;
来源：http://by.521024.cn

[Q53] 按条件删除
来源：http://sk.shxzukj.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mx.shxzskj.cn

[Q54] 清空表
来源：http://jm.wgjwhj.cn

TRUNCATE TABLE logs;
来源：http://ww.panjiajie.cn

[Q55] 排名（并列占位）
来源：http://nd.huixiangedu.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://xh.bookmarksfly.cn

[Q56] 密集排名（并列不占位）
来源：http://nu.szsharing.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://nq.shtwfgs.cn

[Q57] 行号
来源：http://it.haigaiapp.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mh.asd995.cn

[Q58] 累计求和
来源：http://il.asd995.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wc.wgjwhj.cn

[Q59] 分组内累计
来源：http://rm.yuexingan06.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://yy.lnxyls.cn

[Q60] 取上一行 / 下一行
来源：http://eb.jianghongdianzi.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mw.yuexingan06.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://fc.521024.cn

[Q61] 移动平均
来源：http://hd.jianghongdianzi.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ak.yuexingan06.cn

[Q62] 分组占比
来源：http://ms.hnjuh.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ak.szxytkj.cn

[Q63] 开启事务
来源：http://pz.newstarts.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://ur.haigaiapp.cn

[Q64] 提交事务
来源：http://qa.hnjuh.cn

COMMIT;
来源：http://oh.colortex.cn

[Q65] 回滚事务
来源：http://vs.szsharing.cn

ROLLBACK;
来源：http://tq.chemitech.net.cn

[Q66] 行锁查询
来源：http://kp.521024.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ng.haigaiapp.cn

[Q67] 设置隔离级别
来源：http://jg.haigaiapp.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ya.haigaiapp.cn

[Q68] 保存点
来源：http://uw.wgjwhj.cn

SAVEPOINT sp1;
来源：http://dh.chemitech.net.cn

ROLLBACK TO sp1;
来源：http://lz.nszjky.cn

[Q69] 查看执行计划
来源：http://hy.shtwfgs.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ai.szsharing.cn

[Q70] 更新统计信息
来源：http://ov.lnxyls.cn

ANALYZE TABLE users;
来源：http://zm.hnjuh.cn

[Q71] 查看建表语句
来源：http://ai.asd995.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://nx.shxzskj.cn

[Q72] 查看索引
来源：http://ad.chemitech.net.cn

SHOW INDEX FROM users;
来源：http://lq.colortex.cn

[Q73] 查看表状态
来源：http://vi.nicolike.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://ib.asd995.cn

[Q74] 强制使用索引
来源：http://hk.shtwfgs.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://xu.jctech888.com.cn

[Q75] 日期格式化
来源：http://gm.shxzukj.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://rl.panjiajie.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://xx.panjiajie.cn

[Q76] 按天统计
来源：http://xb.hnjuh.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://pv.jianghongdianzi.cn

[Q77] 时间加减
来源：http://rb.gzmigu.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://gh.chemitech.net.cn

[Q78] 当前时间
来源：http://pq.gzmigu.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://au.muxihuayi.cn

[Q79] 字符串拼接
来源：http://gy.jctech888.com.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ec.nicolike.cn

[Q80] 字符串截取
来源：http://qt.haigaiapp.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://nw.asd995.cn

[Q81] 字符串替换
来源：http://ux.jianghongdianzi.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://os.nszjky.cn

[Q82] 字符长度与字节长度
来源：http://ce.nszjky.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://je.lnxyls.cn

[Q83] 大小写转换
来源：http://cd.521024.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ug.nicolike.cn

[Q84] 去除首尾空格
来源：http://pa.szsharing.cn

SELECT TRIM(name) FROM users;
来源：http://be.huanxung.cn

[Q85] 数值取整
来源：http://xi.9csxet.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://tp.szsharing.cn

[Q86] 读取 JSON 字段
来源：http://im.9csxet.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ow.bookmarksfly.cn

[Q87] JSON 字段做条件
来源：http://ww.yuntaijiaju.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://js.hnjuh.cn

[Q88] 行转列（条件聚合）
来源：http://iu.9csxet.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://jx.chemitech.net.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://uu.panjiajie.cn

[Q89] 判断表是否存在
来源：http://od.521024.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://qv.nicolike.cn

[Q90] 生成序号列
来源：http://xh.hnjuh.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ph.szsharing.cn

================================================================================
来源：http://dv.hnjuh.cn

R. Bash 专题
来源：http://rl.gzmigu.cn

================================================================================
来源：http://vm.panjiajie.cn

[R01] shebang 与严格模式
来源：http://dn.bookmarksfly.cn

#!/usr/bin/env bash
来源：http://lc.hahajie.cn

set -euo pipefail
来源：http://uy.gzmigu.cn

[R02] 变量赋值与使用
来源：http://xt.chemitech.net.cn

name="Tom"; echo "$name"
来源：http://qa.yuntaijiaju.cn

[R03] 只读变量
来源：http://cb.hahajie.cn

readonly PI=3.14
来源：http://tx.lnxyls.cn

[R04] 位置参数
来源：http://zv.colortex.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://go.yuntaijiaju.cn

[R05] 参数默认值
来源：http://ha.bookmarksfly.cn

name="${1:-default}"
来源：http://vb.huixiangedu.cn

[R06] 判断命令是否存在
来源：http://en.szxytkj.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://jc.yuexingan06.cn

[R07] if 判断文件
来源：http://kh.huixiangedu.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ry.gzmigu.cn

[R08] 数值比较
来源：http://fn.jianghongdianzi.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://nx.asd995.cn

[R09] 字符串比较
来源：http://qr.asd995.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://va.hahajie.cn

[R10] 正则匹配
来源：http://mk.szsharing.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://sk.muxihuayi.cn

[R11] case 多分支
来源：http://pq.jctech888.com.cn

case "$1" in
来源：http://ja.yuntaijiaju.cn

start) echo "启动" ;;
来源：http://hv.colortex.cn

stop)  echo "停止" ;;
来源：http://qx.9csxet.cn

*)     echo "未知命令" ;;
来源：http://ze.huixinmuqiang.cn

esac
来源：http://ym.yuntaijiaju.cn

[R12] for 遍历文件
来源：http://lt.jianghongdianzi.cn

for f in *.txt; do echo "$f"; done
来源：http://iu.jianghongdianzi.cn

[R13] for 计数循环
来源：http://fz.gzmigu.cn

for i in {1..10}; do echo "$i"; done
来源：http://fo.huixiangedu.cn

[R14] C 风格 for
来源：http://lp.wgjwhj.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://al.huixiangedu.cn

[R15] while 逐行读文件
来源：http://cn.chemitech.net.cn


<!-- 参考信息 -->