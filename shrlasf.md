代发 wailian999

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://fb.shxzukj.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://py.huanxung.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://qo.wgjwhj.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hf.9csxet.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hx.bookmarksfly.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://xf.muxihuayi.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://tf.huixinmuqiang.cn

[P04] 求长度
来源：http://uz.bookmarksfly.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wr.gzmigu.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://vt.gzmigu.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://qo.jctech888.com.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://iu.panjiajie.cn

Java: list.size();  map.size();  s.length()
来源：http://ui.bjjhwx.cn

Go:   len(arr);  len(m)
来源：http://hr.bjjhwx.cn

Ruby: x.length;  x.size
来源：http://zk.jianghongdianzi.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://qw.nicolike.cn

[P05] 判断两个对象内容是否相等
来源：http://gh.panjiajie.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://ch.jianghongdianzi.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://kj.newstarts.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://zf.nszjky.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://os.hnjuh.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://gz.panjiajie.cn

Go:   reflect.DeepEqual(a, b)
来源：http://lw.asd995.cn

Ruby: a == b
来源：http://th.hnjuh.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://gs.hnjuh.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://am.9csxet.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ve.lnxyls.cn

PHP:  if (empty($x)) {}
来源：http://ue.hahajie.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ip.muxihuayi.cn

TS:   if (x == null) {}
来源：http://vh.jctech888.com.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://at.jianghongdianzi.cn

Go:   if x == nil {}
来源：http://za.yuexingan06.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://um.521024.cn

C#:   if (x is null) {}
来源：http://cr.muxihuayi.cn

[P07] 防抖与节流
来源：http://da.9csxet.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://sd.huanxung.cn

PHP:  // 手写时间戳比较
来源：http://ib.haigaiapp.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://sm.huanxung.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://uh.521024.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://kr.hnjuh.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://us.nicolike.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://zs.wgjwhj.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://fw.szsharing.cn

[P08] 处理浮点精度问题
来源：http://ed.wgjwhj.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://vq.yuexingan06.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://uq.szsharing.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://gh.huixinmuqiang.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://iv.muxihuayi.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://bj.yuexingan06.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ya.nicolike.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://sl.szsharing.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://bq.shxzskj.cn

================================================================================
来源：http://yc.nicolike.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://qj.hnjuh.cn

================================================================================
来源：http://gc.huanxung.cn

[Q01] 创建表
来源：http://if.nszjky.cn

CREATE TABLE users (
来源：http://ro.521024.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://gw.jctech888.com.cn

name VARCHAR(50) NOT NULL,
来源：http://em.bookmarksfly.cn

email VARCHAR(100) UNIQUE,
来源：http://na.hahajie.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wk.hnjuh.cn

);
来源：http://dd.huixiangedu.cn

[Q02] 创建带外键的表
来源：http://ka.bookmarksfly.cn

CREATE TABLE orders (
来源：http://ph.gzmigu.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://pg.jianghongdianzi.cn

user_id INT NOT NULL,
来源：http://tu.szxytkj.cn

amount DECIMAL(10, 2),
来源：http://zd.szsharing.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://sf.asd995.cn

);
来源：http://ly.shtwfgs.cn

[Q03] 增加列
来源：http://yr.bjjhwx.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://jb.jianghongdianzi.cn

[Q04] 修改列类型
来源：http://bj.muxihuayi.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://dl.haigaiapp.cn

[Q05] 重命名列
来源：http://kb.colortex.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://xh.panjiajie.cn

[Q06] 删除列
来源：http://nw.huanxung.cn

ALTER TABLE users DROP COLUMN age;
来源：http://ru.521024.cn

[Q07] 删除表
来源：http://sw.huixinmuqiang.cn

DROP TABLE IF EXISTS orders;
来源：http://sr.jctech888.com.cn

[Q08] 创建普通索引
来源：http://zx.bookmarksfly.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://gs.asd995.cn

[Q09] 创建唯一索引
来源：http://qc.wgjwhj.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://nf.huixinmuqiang.cn

[Q10] 插入单行
来源：http://zb.haigaiapp.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://fd.hahajie.cn

[Q11] 一次插入多行
来源：http://qf.szxytkj.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://vu.yuexingan06.cn

[Q12] 插入后取自增 ID
来源：http://nz.shtwfgs.cn

INSERT INTO users (name) VALUES ('C');
来源：http://lk.colortex.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ot.wgjwhj.cn

[Q13] 忽略重复插入
来源：http://vq.gzmigu.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://xz.hnjuh.cn

[Q14] 存在则更新（upsert）
来源：http://lz.hahajie.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ps.jctech888.com.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ew.shxzukj.cn

[Q15] 查询全部
来源：http://vi.huanxung.cn

SELECT * FROM users;
来源：http://ug.shtwfgs.cn

[Q16] 查询指定列
来源：http://db.jianghongdianzi.cn

SELECT id, name FROM users;
来源：http://dw.szsharing.cn

[Q17] 条件查询
来源：http://ka.huixiangedu.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://lg.huanxung.cn

[Q18] 模糊匹配
来源：http://bc.jianghongdianzi.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ub.shxzukj.cn

[Q19] 范围查询
来源：http://zn.szxytkj.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://kp.muxihuayi.cn

[Q20] IN 列表
来源：http://bo.shxzskj.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://zx.nicolike.cn

[Q21] 空值判断
来源：http://jy.huixiangedu.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://ad.bookmarksfly.cn

[Q22] 排序
来源：http://qc.shxzskj.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ma.nicolike.cn

[Q23] 分页
来源：http://rt.nszjky.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://bo.newstarts.cn

[Q24] 去重
来源：http://xf.bjjhwx.cn

SELECT DISTINCT city FROM users;
来源：http://dv.9csxet.cn

[Q25] 只取前 N 条
来源：http://ft.jctech888.com.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://si.jctech888.com.cn

[Q26] 计数
来源：http://sr.shxzukj.cn

SELECT COUNT(*) FROM users;
来源：http://mt.colortex.cn

[Q27] 条件计数
来源：http://pc.jctech888.com.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ml.hnjuh.cn

[Q28] 求和与平均
来源：http://oe.wgjwhj.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://ic.bjjhwx.cn

[Q29] 最大最小值
来源：http://al.yuntaijiaju.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://pz.huixiangedu.cn

[Q30] 分组统计
来源：http://sj.haigaiapp.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ha.haigaiapp.cn

[Q31] 分组后过滤
来源：http://iv.nszjky.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://os.shtwfgs.cn

[Q32] 分组拼接字符串
来源：http://sx.chemitech.net.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://rk.bjjhwx.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ol.colortex.cn

[Q33] 多列分组
来源：http://mu.chemitech.net.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://vh.asd995.cn

[Q34] 每组取第一条
来源：http://uh.wgjwhj.cn

SELECT * FROM (
来源：http://oq.lnxyls.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wp.shxzukj.cn

) t WHERE rn = 1;
来源：http://wg.shxzukj.cn

[Q35] 内连接
来源：http://ix.panjiajie.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://bj.newstarts.cn

[Q36] 左连接
来源：http://ce.nicolike.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mv.huanxung.cn

[Q37] 右连接
来源：http://kp.newstarts.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://dk.muxihuayi.cn

[Q38] 全外连接（PostgreSQL）
来源：http://iv.jctech888.com.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://qh.bjjhwx.cn

[Q39] 自连接（查上下级）
来源：http://ly.shxzukj.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://mi.yuntaijiaju.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ei.nszjky.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://yp.muxihuayi.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://fo.newstarts.cn

[Q41] 多表连接
来源：http://jk.bjjhwx.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://yk.yuexingan06.cn

JOIN users u ON u.id = o.user_id
来源：http://qg.wgjwhj.cn

JOIN products p ON p.id = o.product_id;
来源：http://bl.9csxet.cn

[Q42] 连接条件附加过滤
来源：http://om.jianghongdianzi.cn

SELECT u.name, o.amount FROM users u
来源：http://rt.szxytkj.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://vr.9csxet.cn

[Q43] 标量子查询
来源：http://tj.newstarts.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://nj.yuntaijiaju.cn

[Q44] IN 子查询
来源：http://sy.huixinmuqiang.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://aa.wgjwhj.cn

[Q45] EXISTS 判断存在
来源：http://lu.colortex.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ht.shxzukj.cn

[Q46] NOT EXISTS 判断不存在
来源：http://cg.chemitech.net.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://fc.muxihuayi.cn

[Q47] 与平均值比较
来源：http://zi.bjjhwx.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://tw.hnjuh.cn

[Q48] CTE 公用表表达式
来源：http://ic.nszjky.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://db.nicolike.cn

SELECT * FROM t WHERE c > 5;
来源：http://mr.nszjky.cn

[Q49] 更新单行
来源：http://fu.jctech888.com.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://gg.asd995.cn

[Q50] 批量更新
来源：http://ol.panjiajie.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://pu.gzmigu.cn

[Q51] 用子查询更新
来源：http://rz.lnxyls.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://zx.nszjky.cn

[Q52] 删除指定行
来源：http://jw.lnxyls.cn

DELETE FROM users WHERE id = 10;
来源：http://jk.newstarts.cn

[Q53] 按条件删除
来源：http://sy.jianghongdianzi.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ns.szsharing.cn

[Q54] 清空表
来源：http://eb.colortex.cn

TRUNCATE TABLE logs;
来源：http://tr.szsharing.cn

[Q55] 排名（并列占位）
来源：http://zq.huixinmuqiang.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://zr.gzmigu.cn

[Q56] 密集排名（并列不占位）
来源：http://ks.yuntaijiaju.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mp.huanxung.cn

[Q57] 行号
来源：http://sg.9csxet.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://qp.9csxet.cn

[Q58] 累计求和
来源：http://hc.muxihuayi.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://it.muxihuayi.cn

[Q59] 分组内累计
来源：http://zn.gzmigu.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://rk.haigaiapp.cn

[Q60] 取上一行 / 下一行
来源：http://hq.gzmigu.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://jw.chemitech.net.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://cg.lnxyls.cn

[Q61] 移动平均
来源：http://sa.nicolike.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hn.9csxet.cn

[Q62] 分组占比
来源：http://fs.hahajie.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://nu.colortex.cn

[Q63] 开启事务
来源：http://ok.muxihuayi.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://jg.jianghongdianzi.cn

[Q64] 提交事务
来源：http://zl.bjjhwx.cn

COMMIT;
来源：http://ao.521024.cn

[Q65] 回滚事务
来源：http://iz.bookmarksfly.cn

ROLLBACK;
来源：http://hs.yuexingan06.cn

[Q66] 行锁查询
来源：http://ym.huixiangedu.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://lh.yuexingan06.cn

[Q67] 设置隔离级别
来源：http://ys.panjiajie.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://pg.hnjuh.cn

[Q68] 保存点
来源：http://me.haigaiapp.cn

SAVEPOINT sp1;
来源：http://xw.9csxet.cn

ROLLBACK TO sp1;
来源：http://ez.shxzskj.cn

[Q69] 查看执行计划
来源：http://bi.shtwfgs.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://yn.nszjky.cn

[Q70] 更新统计信息
来源：http://rz.asd995.cn

ANALYZE TABLE users;
来源：http://qn.muxihuayi.cn

[Q71] 查看建表语句
来源：http://iu.jianghongdianzi.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ic.haigaiapp.cn

[Q72] 查看索引
来源：http://aw.521024.cn

SHOW INDEX FROM users;
来源：http://as.huanxung.cn

[Q73] 查看表状态
来源：http://ep.szsharing.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://mq.gzmigu.cn

[Q74] 强制使用索引
来源：http://qp.muxihuayi.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://sq.nicolike.cn

[Q75] 日期格式化
来源：http://fw.panjiajie.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://sp.huixiangedu.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://zh.newstarts.cn

[Q76] 按天统计
来源：http://es.chemitech.net.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ua.newstarts.cn

[Q77] 时间加减
来源：http://vi.huixinmuqiang.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://di.hnjuh.cn

[Q78] 当前时间
来源：http://ww.yuntaijiaju.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://od.hahajie.cn

[Q79] 字符串拼接
来源：http://gh.hahajie.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wk.szsharing.cn

[Q80] 字符串截取
来源：http://el.lnxyls.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://gu.hnjuh.cn

[Q81] 字符串替换
来源：http://ib.nicolike.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://su.nicolike.cn

[Q82] 字符长度与字节长度
来源：http://wq.bookmarksfly.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://pt.haigaiapp.cn

[Q83] 大小写转换
来源：http://us.szsharing.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ur.szsharing.cn

[Q84] 去除首尾空格
来源：http://xv.hahajie.cn

SELECT TRIM(name) FROM users;
来源：http://cm.huixinmuqiang.cn

[Q85] 数值取整
来源：http://tj.huanxung.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://jm.colortex.cn

[Q86] 读取 JSON 字段
来源：http://gj.jianghongdianzi.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://xy.haigaiapp.cn

[Q87] JSON 字段做条件
来源：http://ia.muxihuayi.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wn.chemitech.net.cn

[Q88] 行转列（条件聚合）
来源：http://pg.gzmigu.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://pu.colortex.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://rn.colortex.cn

[Q89] 判断表是否存在
来源：http://wp.shtwfgs.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://xn.wgjwhj.cn

[Q90] 生成序号列
来源：http://ub.wgjwhj.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://qv.huixiangedu.cn

================================================================================
来源：http://dv.newstarts.cn

R. Bash 专题
来源：http://oz.jctech888.com.cn

================================================================================
来源：http://nd.9csxet.cn

[R01] shebang 与严格模式
来源：http://aq.huixinmuqiang.cn

#!/usr/bin/env bash
来源：http://jf.asd995.cn

set -euo pipefail
来源：http://rt.jctech888.com.cn

[R02] 变量赋值与使用
来源：http://tk.nszjky.cn

name="Tom"; echo "$name"
来源：http://ll.asd995.cn

[R03] 只读变量
来源：http://pj.hnjuh.cn

readonly PI=3.14
来源：http://xj.newstarts.cn

[R04] 位置参数
来源：http://mt.hnjuh.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://fz.nszjky.cn

[R05] 参数默认值
来源：http://ym.lnxyls.cn

name="${1:-default}"
来源：http://fo.colortex.cn

[R06] 判断命令是否存在
来源：http://nu.szxytkj.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://vn.hahajie.cn

[R07] if 判断文件
来源：http://td.hnjuh.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ts.bookmarksfly.cn

[R08] 数值比较
来源：http://ky.panjiajie.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://ll.huixiangedu.cn

[R09] 字符串比较
来源：http://cn.newstarts.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ee.shxzukj.cn

[R10] 正则匹配
来源：http://tm.521024.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://bn.shxzskj.cn

[R11] case 多分支
来源：http://gd.nszjky.cn

case "$1" in
来源：http://gl.nicolike.cn

start) echo "启动" ;;
来源：http://ts.gzmigu.cn

stop)  echo "停止" ;;
来源：http://pb.nicolike.cn

*)     echo "未知命令" ;;
来源：http://nq.bookmarksfly.cn

esac
来源：http://qq.muxihuayi.cn

[R12] for 遍历文件
来源：http://vn.huixinmuqiang.cn

for f in *.txt; do echo "$f"; done
来源：http://bm.haigaiapp.cn

[R13] for 计数循环
来源：http://gs.wgjwhj.cn

for i in {1..10}; do echo "$i"; done
来源：http://bo.bookmarksfly.cn

[R14] C 风格 for
来源：http://rl.hnjuh.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://cg.bjjhwx.cn

[R15] while 逐行读文件
来源：http://bi.asd995.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hd.yuexingan06.cn

[R16] until 等待条件
来源：http://mc.shtwfgs.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://cp.szxytkj.cn

[R17] 数组定义与取值
来源：http://xb.hahajie.cn


<!-- 参考信息 -->