代发 wailian999

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://jy.shxzskj.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://pr.hnjuh.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hr.panjiajie.cn

[P04] 求长度
来源：http://kt.nszjky.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ys.chemitech.net.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://bt.shxzskj.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://df.hahajie.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wt.hahajie.cn

Java: list.size();  map.size();  s.length()
来源：http://dp.chemitech.net.cn

Go:   len(arr);  len(m)
来源：http://fl.bjjhwx.cn

Ruby: x.length;  x.size
来源：http://ez.huixiangedu.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://bu.lnxyls.cn

[P05] 判断两个对象内容是否相等
来源：http://mf.huanxung.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://rt.nicolike.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://cb.colortex.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://qg.hnjuh.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://bu.yuntaijiaju.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://cy.asd995.cn

Go:   reflect.DeepEqual(a, b)
来源：http://ee.nicolike.cn

Ruby: a == b
来源：http://wd.jctech888.com.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://zo.gzmigu.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://sn.gzmigu.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://he.jianghongdianzi.cn

PHP:  if (empty($x)) {}
来源：http://zc.asd995.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://xo.521024.cn

TS:   if (x == null) {}
来源：http://uf.panjiajie.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://jf.panjiajie.cn

Go:   if x == nil {}
来源：http://nw.bookmarksfly.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://yk.nszjky.cn

C#:   if (x is null) {}
来源：http://ir.jianghongdianzi.cn

[P07] 防抖与节流
来源：http://ix.haigaiapp.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hu.hahajie.cn

PHP:  // 手写时间戳比较
来源：http://bu.panjiajie.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://nc.jianghongdianzi.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://yd.yuexingan06.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hg.nicolike.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://lx.jctech888.com.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://tk.haigaiapp.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://rh.yuntaijiaju.cn

[P08] 处理浮点精度问题
来源：http://tt.szxytkj.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wi.nszjky.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://sx.colortex.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://zd.521024.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://pu.panjiajie.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://kg.asd995.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://bd.jctech888.com.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://gp.szxytkj.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://uf.chemitech.net.cn

================================================================================
来源：http://gs.wgjwhj.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://th.gzmigu.cn

================================================================================
来源：http://vi.huanxung.cn

[Q01] 创建表
来源：http://kk.yuexingan06.cn

CREATE TABLE users (
来源：http://kq.nicolike.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://id.bjjhwx.cn

name VARCHAR(50) NOT NULL,
来源：http://ly.nszjky.cn

email VARCHAR(100) UNIQUE,
来源：http://tf.colortex.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://tf.newstarts.cn

);
来源：http://yn.panjiajie.cn

[Q02] 创建带外键的表
来源：http://rx.shtwfgs.cn

CREATE TABLE orders (
来源：http://df.nicolike.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ao.jctech888.com.cn

user_id INT NOT NULL,
来源：http://ii.shxzskj.cn

amount DECIMAL(10, 2),
来源：http://ri.jianghongdianzi.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://rc.newstarts.cn

);
来源：http://wq.shxzukj.cn

[Q03] 增加列
来源：http://jv.colortex.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://uc.muxihuayi.cn

[Q04] 修改列类型
来源：http://ht.huixiangedu.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://zm.chemitech.net.cn

[Q05] 重命名列
来源：http://tr.gzmigu.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://np.jctech888.com.cn

[Q06] 删除列
来源：http://tn.huanxung.cn

ALTER TABLE users DROP COLUMN age;
来源：http://cr.nszjky.cn

[Q07] 删除表
来源：http://cb.panjiajie.cn

DROP TABLE IF EXISTS orders;
来源：http://bv.haigaiapp.cn

[Q08] 创建普通索引
来源：http://dr.huanxung.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://ch.nicolike.cn

[Q09] 创建唯一索引
来源：http://as.muxihuayi.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://vz.colortex.cn

[Q10] 插入单行
来源：http://aj.shxzukj.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ex.shxzukj.cn

[Q11] 一次插入多行
来源：http://ov.szxytkj.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ne.panjiajie.cn

[Q12] 插入后取自增 ID
来源：http://ug.gzmigu.cn

INSERT INTO users (name) VALUES ('C');
来源：http://jx.colortex.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://tv.bookmarksfly.cn

[Q13] 忽略重复插入
来源：http://mr.nszjky.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://fu.shxzskj.cn

[Q14] 存在则更新（upsert）
来源：http://sx.wgjwhj.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wg.huanxung.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://va.nszjky.cn

[Q15] 查询全部
来源：http://cz.hahajie.cn

SELECT * FROM users;
来源：http://by.asd995.cn

[Q16] 查询指定列
来源：http://fa.asd995.cn

SELECT id, name FROM users;
来源：http://cp.chemitech.net.cn

[Q17] 条件查询
来源：http://bt.asd995.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://bx.yuexingan06.cn

[Q18] 模糊匹配
来源：http://ez.huanxung.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ln.nicolike.cn

[Q19] 范围查询
来源：http://df.colortex.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ep.lnxyls.cn

[Q20] IN 列表
来源：http://qv.bjjhwx.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ta.panjiajie.cn

[Q21] 空值判断
来源：http://da.gzmigu.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://xg.bjjhwx.cn

[Q22] 排序
来源：http://xm.shxzukj.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://uh.nszjky.cn

[Q23] 分页
来源：http://dz.asd995.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://aj.bjjhwx.cn

[Q24] 去重
来源：http://yo.panjiajie.cn

SELECT DISTINCT city FROM users;
来源：http://ah.asd995.cn

[Q25] 只取前 N 条
来源：http://yp.huixiangedu.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://gi.chemitech.net.cn

[Q26] 计数
来源：http://sy.jctech888.com.cn

SELECT COUNT(*) FROM users;
来源：http://ew.hnjuh.cn

[Q27] 条件计数
来源：http://hp.huixinmuqiang.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://pq.9csxet.cn

[Q28] 求和与平均
来源：http://rw.shtwfgs.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://cu.shxzskj.cn

[Q29] 最大最小值
来源：http://jv.hnjuh.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://uh.hahajie.cn

[Q30] 分组统计
来源：http://gu.gzmigu.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ok.muxihuayi.cn

[Q31] 分组后过滤
来源：http://ye.jianghongdianzi.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://nj.bjjhwx.cn

[Q32] 分组拼接字符串
来源：http://zo.chemitech.net.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://su.haigaiapp.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://lv.bjjhwx.cn

[Q33] 多列分组
来源：http://qu.lnxyls.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://gj.shtwfgs.cn

[Q34] 每组取第一条
来源：http://ac.lnxyls.cn

SELECT * FROM (
来源：http://qv.jianghongdianzi.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://tg.huixinmuqiang.cn

) t WHERE rn = 1;
来源：http://jl.521024.cn

[Q35] 内连接
来源：http://uo.shxzukj.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://cx.nicolike.cn

[Q36] 左连接
来源：http://vr.haigaiapp.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://pn.asd995.cn

[Q37] 右连接
来源：http://hd.yuntaijiaju.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://uj.szxytkj.cn

[Q38] 全外连接（PostgreSQL）
来源：http://ft.bookmarksfly.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://oq.bookmarksfly.cn

[Q39] 自连接（查上下级）
来源：http://ti.yuntaijiaju.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://zi.521024.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wp.nicolike.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://rc.bookmarksfly.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ey.chemitech.net.cn

[Q41] 多表连接
来源：http://mr.panjiajie.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://kw.shxzukj.cn

JOIN users u ON u.id = o.user_id
来源：http://ch.hnjuh.cn

JOIN products p ON p.id = o.product_id;
来源：http://ge.huixinmuqiang.cn

[Q42] 连接条件附加过滤
来源：http://xm.jctech888.com.cn

SELECT u.name, o.amount FROM users u
来源：http://lc.huixinmuqiang.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ep.haigaiapp.cn

[Q43] 标量子查询
来源：http://ou.jianghongdianzi.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://fs.521024.cn

[Q44] IN 子查询
来源：http://zv.nszjky.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://rr.9csxet.cn

[Q45] EXISTS 判断存在
来源：http://gi.yuexingan06.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mw.shxzskj.cn

[Q46] NOT EXISTS 判断不存在
来源：http://zx.jianghongdianzi.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://tr.nicolike.cn

[Q47] 与平均值比较
来源：http://aw.newstarts.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wy.panjiajie.cn

[Q48] CTE 公用表表达式
来源：http://gn.colortex.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://la.yuexingan06.cn

SELECT * FROM t WHERE c > 5;
来源：http://uv.521024.cn

[Q49] 更新单行
来源：http://hp.huanxung.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ry.panjiajie.cn

[Q50] 批量更新
来源：http://mg.panjiajie.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://su.yuntaijiaju.cn

[Q51] 用子查询更新
来源：http://zi.9csxet.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://yf.shxzskj.cn

[Q52] 删除指定行
来源：http://gv.chemitech.net.cn

DELETE FROM users WHERE id = 10;
来源：http://eb.haigaiapp.cn

[Q53] 按条件删除
来源：http://ha.shxzukj.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://so.szsharing.cn

[Q54] 清空表
来源：http://fx.panjiajie.cn

TRUNCATE TABLE logs;
来源：http://fi.colortex.cn

[Q55] 排名（并列占位）
来源：http://di.gzmigu.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://bk.nszjky.cn

[Q56] 密集排名（并列不占位）
来源：http://ar.wgjwhj.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://dk.colortex.cn

[Q57] 行号
来源：http://df.szsharing.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://vw.yuntaijiaju.cn

[Q58] 累计求和
来源：http://zb.szsharing.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://kt.nicolike.cn

[Q59] 分组内累计
来源：http://rm.nszjky.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://jl.nszjky.cn

[Q60] 取上一行 / 下一行
来源：http://rc.bookmarksfly.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://rb.yuexingan06.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://em.panjiajie.cn

[Q61] 移动平均
来源：http://lk.gzmigu.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://kb.newstarts.cn

[Q62] 分组占比
来源：http://jk.szxytkj.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://pv.szxytkj.cn

[Q63] 开启事务
来源：http://pb.panjiajie.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://ic.gzmigu.cn

[Q64] 提交事务
来源：http://bf.jctech888.com.cn

COMMIT;
来源：http://rr.nicolike.cn

[Q65] 回滚事务
来源：http://po.szsharing.cn

ROLLBACK;
来源：http://fi.hnjuh.cn

[Q66] 行锁查询
来源：http://hb.huanxung.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ob.9csxet.cn

[Q67] 设置隔离级别
来源：http://vd.jctech888.com.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://au.nicolike.cn

[Q68] 保存点
来源：http://sd.huanxung.cn

SAVEPOINT sp1;
来源：http://jx.huixiangedu.cn

ROLLBACK TO sp1;
来源：http://kd.lnxyls.cn

[Q69] 查看执行计划
来源：http://ah.chemitech.net.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://xv.gzmigu.cn

[Q70] 更新统计信息
来源：http://ez.nicolike.cn

ANALYZE TABLE users;
来源：http://rh.huixinmuqiang.cn

[Q71] 查看建表语句
来源：http://pp.9csxet.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wi.huixiangedu.cn

[Q72] 查看索引
来源：http://kk.newstarts.cn

SHOW INDEX FROM users;
来源：http://kp.9csxet.cn

[Q73] 查看表状态
来源：http://vc.chemitech.net.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://em.gzmigu.cn

[Q74] 强制使用索引
来源：http://yu.bjjhwx.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ju.shxzskj.cn

[Q75] 日期格式化
来源：http://zj.wgjwhj.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://bk.hnjuh.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://dc.asd995.cn

[Q76] 按天统计
来源：http://ow.szsharing.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ql.asd995.cn

[Q77] 时间加减
来源：http://xc.huixinmuqiang.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ac.yuexingan06.cn

[Q78] 当前时间
来源：http://tu.szsharing.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://fi.haigaiapp.cn

[Q79] 字符串拼接
来源：http://nm.jianghongdianzi.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://qg.huixinmuqiang.cn

[Q80] 字符串截取
来源：http://tk.shxzskj.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ii.hnjuh.cn

[Q81] 字符串替换
来源：http://kd.shtwfgs.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ww.muxihuayi.cn

[Q82] 字符长度与字节长度
来源：http://ge.jianghongdianzi.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ar.shtwfgs.cn

[Q83] 大小写转换
来源：http://nr.hahajie.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://au.shtwfgs.cn

[Q84] 去除首尾空格
来源：http://lz.panjiajie.cn

SELECT TRIM(name) FROM users;
来源：http://jw.jctech888.com.cn

[Q85] 数值取整
来源：http://qv.lnxyls.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mg.hahajie.cn

[Q86] 读取 JSON 字段
来源：http://tw.hnjuh.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://zc.shxzskj.cn

[Q87] JSON 字段做条件
来源：http://sf.newstarts.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://fs.yuexingan06.cn

[Q88] 行转列（条件聚合）
来源：http://ie.haigaiapp.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://bg.newstarts.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wp.newstarts.cn

[Q89] 判断表是否存在
来源：http://lt.asd995.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://dz.wgjwhj.cn

[Q90] 生成序号列
来源：http://tp.chemitech.net.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://kq.szsharing.cn

================================================================================
来源：http://ox.hahajie.cn

R. Bash 专题
来源：http://ia.wgjwhj.cn

================================================================================
来源：http://yv.hahajie.cn

[R01] shebang 与严格模式
来源：http://iw.muxihuayi.cn

#!/usr/bin/env bash
来源：http://eu.shtwfgs.cn

set -euo pipefail
来源：http://oc.shtwfgs.cn

[R02] 变量赋值与使用
来源：http://ep.shxzskj.cn

name="Tom"; echo "$name"
来源：http://zo.shtwfgs.cn

[R03] 只读变量
来源：http://pm.huixinmuqiang.cn

readonly PI=3.14
来源：http://wk.nszjky.cn

[R04] 位置参数
来源：http://ab.huanxung.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://oq.huanxung.cn

[R05] 参数默认值
来源：http://do.asd995.cn

name="${1:-default}"
来源：http://jb.chemitech.net.cn

[R06] 判断命令是否存在
来源：http://ue.huanxung.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://at.muxihuayi.cn

[R07] if 判断文件
来源：http://jz.huixinmuqiang.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://qb.gzmigu.cn

[R08] 数值比较
来源：http://ii.yuexingan06.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://wh.panjiajie.cn

[R09] 字符串比较
来源：http://ra.szxytkj.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mn.colortex.cn

[R10] 正则匹配
来源：http://hy.9csxet.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://vh.yuexingan06.cn

[R11] case 多分支
来源：http://uh.yuexingan06.cn

case "$1" in
来源：http://zb.colortex.cn

start) echo "启动" ;;
来源：http://sp.huanxung.cn

stop)  echo "停止" ;;
来源：http://wv.yuexingan06.cn

*)     echo "未知命令" ;;
来源：http://lg.szsharing.cn

esac
来源：http://ed.hahajie.cn

[R12] for 遍历文件
来源：http://qk.szxytkj.cn

for f in *.txt; do echo "$f"; done
来源：http://js.newstarts.cn

[R13] for 计数循环
来源：http://ur.jianghongdianzi.cn

for i in {1..10}; do echo "$i"; done
来源：http://nn.asd995.cn

[R14] C 风格 for
来源：http://zn.szsharing.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://kv.huanxung.cn

[R15] while 逐行读文件
来源：http://st.szsharing.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ay.haigaiapp.cn

[R16] until 等待条件
来源：http://nd.szxytkj.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://oz.gzmigu.cn

[R17] 数组定义与取值
来源：http://ja.wgjwhj.cn

arr=(a b c); echo "${arr[0]}"
来源：http://rt.jctech888.com.cn

[R18] 遍历数组
来源：http://xn.hahajie.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://zl.panjiajie.cn

[R19] 数组长度
来源：http://ua.lnxyls.cn


<!-- 参考信息 -->