代发 wailian999

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://za.shtwfgs.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://xk.shxzskj.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://do.shtwfgs.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://sb.newstarts.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://zs.9csxet.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://pj.9csxet.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wi.nicolike.cn

[P04] 求长度
来源：http://nn.shxzukj.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://jp.jctech888.com.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://gb.szxytkj.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ze.hnjuh.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://lb.bjjhwx.cn

Java: list.size();  map.size();  s.length()
来源：http://tu.szsharing.cn

Go:   len(arr);  len(m)
来源：http://th.hahajie.cn

Ruby: x.length;  x.size
来源：http://he.jctech888.com.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://qt.szsharing.cn

[P05] 判断两个对象内容是否相等
来源：http://du.haigaiapp.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://ew.nicolike.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://yh.shtwfgs.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://lh.yuntaijiaju.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://cy.yuntaijiaju.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://vd.szxytkj.cn

Go:   reflect.DeepEqual(a, b)
来源：http://uo.yuexingan06.cn

Ruby: a == b
来源：http://ex.shtwfgs.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ot.nszjky.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://zq.hahajie.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ku.521024.cn

PHP:  if (empty($x)) {}
来源：http://ui.bjjhwx.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://gh.szxytkj.cn

TS:   if (x == null) {}
来源：http://we.szsharing.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://ye.521024.cn

Go:   if x == nil {}
来源：http://xi.haigaiapp.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://qm.jianghongdianzi.cn

C#:   if (x is null) {}
来源：http://fy.szsharing.cn

[P07] 防抖与节流
来源：http://wv.yuexingan06.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ag.panjiajie.cn

PHP:  // 手写时间戳比较
来源：http://ke.bjjhwx.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://fw.szxytkj.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://pm.nicolike.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://gm.asd995.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://er.colortex.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://ti.521024.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://gz.nszjky.cn

[P08] 处理浮点精度问题
来源：http://aa.haigaiapp.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://nw.wgjwhj.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://vv.nicolike.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hy.521024.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ng.huixiangedu.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://jc.bookmarksfly.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://kd.yuntaijiaju.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ar.hnjuh.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://xs.9csxet.cn

================================================================================
来源：http://og.hahajie.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://vj.huixinmuqiang.cn

================================================================================
来源：http://ls.jianghongdianzi.cn

[Q01] 创建表
来源：http://ii.lnxyls.cn

CREATE TABLE users (
来源：http://bv.gzmigu.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://bf.chemitech.net.cn

name VARCHAR(50) NOT NULL,
来源：http://vt.shtwfgs.cn

email VARCHAR(100) UNIQUE,
来源：http://eg.hahajie.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://oy.panjiajie.cn

);
来源：http://yw.hnjuh.cn

[Q02] 创建带外键的表
来源：http://rt.muxihuayi.cn

CREATE TABLE orders (
来源：http://qu.shxzukj.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://oz.haigaiapp.cn

user_id INT NOT NULL,
来源：http://ll.lnxyls.cn

amount DECIMAL(10, 2),
来源：http://qs.huixinmuqiang.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://li.yuntaijiaju.cn

);
来源：http://tc.lnxyls.cn

[Q03] 增加列
来源：http://bk.lnxyls.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://kv.huanxung.cn

[Q04] 修改列类型
来源：http://dh.yuntaijiaju.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hi.shxzukj.cn

[Q05] 重命名列
来源：http://mc.haigaiapp.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://gn.chemitech.net.cn

[Q06] 删除列
来源：http://hs.panjiajie.cn

ALTER TABLE users DROP COLUMN age;
来源：http://dz.huixiangedu.cn

[Q07] 删除表
来源：http://xs.newstarts.cn

DROP TABLE IF EXISTS orders;
来源：http://tq.huixiangedu.cn

[Q08] 创建普通索引
来源：http://xl.szxytkj.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://bv.shxzskj.cn

[Q09] 创建唯一索引
来源：http://ib.hahajie.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://jz.shxzskj.cn

[Q10] 插入单行
来源：http://cm.hahajie.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://nd.nicolike.cn

[Q11] 一次插入多行
来源：http://fh.asd995.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://aj.9csxet.cn

[Q12] 插入后取自增 ID
来源：http://rg.panjiajie.cn

INSERT INTO users (name) VALUES ('C');
来源：http://of.colortex.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://nx.asd995.cn

[Q13] 忽略重复插入
来源：http://fd.jctech888.com.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://yx.panjiajie.cn

[Q14] 存在则更新（upsert）
来源：http://pe.jianghongdianzi.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://aj.szxytkj.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://vp.panjiajie.cn

[Q15] 查询全部
来源：http://gq.szsharing.cn

SELECT * FROM users;
来源：http://tw.panjiajie.cn

[Q16] 查询指定列
来源：http://db.huixinmuqiang.cn

SELECT id, name FROM users;
来源：http://np.hahajie.cn

[Q17] 条件查询
来源：http://qb.gzmigu.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://se.huixiangedu.cn

[Q18] 模糊匹配
来源：http://qg.yuntaijiaju.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://qx.hahajie.cn

[Q19] 范围查询
来源：http://zq.chemitech.net.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://rs.asd995.cn

[Q20] IN 列表
来源：http://ud.chemitech.net.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://yv.chemitech.net.cn

[Q21] 空值判断
来源：http://sn.asd995.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://yv.panjiajie.cn

[Q22] 排序
来源：http://hk.asd995.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://vp.bjjhwx.cn

[Q23] 分页
来源：http://iu.bookmarksfly.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ei.haigaiapp.cn

[Q24] 去重
来源：http://cp.nicolike.cn

SELECT DISTINCT city FROM users;
来源：http://ep.hahajie.cn

[Q25] 只取前 N 条
来源：http://yv.shxzskj.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wq.newstarts.cn

[Q26] 计数
来源：http://zk.yuntaijiaju.cn

SELECT COUNT(*) FROM users;
来源：http://yt.shtwfgs.cn

[Q27] 条件计数
来源：http://dv.521024.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://zw.yuexingan06.cn

[Q28] 求和与平均
来源：http://om.panjiajie.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://ux.521024.cn

[Q29] 最大最小值
来源：http://jd.bookmarksfly.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://gn.asd995.cn

[Q30] 分组统计
来源：http://ym.huanxung.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ji.hahajie.cn

[Q31] 分组后过滤
来源：http://rf.szxytkj.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hm.nszjky.cn

[Q32] 分组拼接字符串
来源：http://vo.lnxyls.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://zc.huanxung.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://rj.colortex.cn

[Q33] 多列分组
来源：http://rj.wgjwhj.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://as.hnjuh.cn

[Q34] 每组取第一条
来源：http://je.yuexingan06.cn

SELECT * FROM (
来源：http://cy.bjjhwx.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://rr.yuntaijiaju.cn

) t WHERE rn = 1;
来源：http://jb.wgjwhj.cn

[Q35] 内连接
来源：http://ue.lnxyls.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://zu.hahajie.cn

[Q36] 左连接
来源：http://pv.hahajie.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://av.gzmigu.cn

[Q37] 右连接
来源：http://kg.huanxung.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://qv.colortex.cn

[Q38] 全外连接（PostgreSQL）
来源：http://hq.shxzskj.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ph.yuexingan06.cn

[Q39] 自连接（查上下级）
来源：http://vz.bookmarksfly.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://lb.gzmigu.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ri.shxzskj.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://kv.chemitech.net.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://xb.shxzukj.cn

[Q41] 多表连接
来源：http://cs.yuexingan06.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://tn.521024.cn

JOIN users u ON u.id = o.user_id
来源：http://ob.asd995.cn

JOIN products p ON p.id = o.product_id;
来源：http://vn.haigaiapp.cn

[Q42] 连接条件附加过滤
来源：http://eq.yuexingan06.cn

SELECT u.name, o.amount FROM users u
来源：http://xu.nicolike.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://bz.szxytkj.cn

[Q43] 标量子查询
来源：http://uj.hahajie.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://et.jctech888.com.cn

[Q44] IN 子查询
来源：http://mb.bookmarksfly.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://qb.jctech888.com.cn

[Q45] EXISTS 判断存在
来源：http://gi.asd995.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ve.lnxyls.cn

[Q46] NOT EXISTS 判断不存在
来源：http://uy.nicolike.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ji.shxzskj.cn

[Q47] 与平均值比较
来源：http://rv.bjjhwx.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://rl.shxzskj.cn

[Q48] CTE 公用表表达式
来源：http://bl.nicolike.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://nn.haigaiapp.cn

SELECT * FROM t WHERE c > 5;
来源：http://zi.asd995.cn

[Q49] 更新单行
来源：http://us.szxytkj.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://aq.yuntaijiaju.cn

[Q50] 批量更新
来源：http://cx.gzmigu.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hr.panjiajie.cn

[Q51] 用子查询更新
来源：http://po.nicolike.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://ta.huixinmuqiang.cn

[Q52] 删除指定行
来源：http://uk.gzmigu.cn

DELETE FROM users WHERE id = 10;
来源：http://qu.hnjuh.cn

[Q53] 按条件删除
来源：http://vt.shtwfgs.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://kf.asd995.cn

[Q54] 清空表
来源：http://gi.szxytkj.cn

TRUNCATE TABLE logs;
来源：http://et.yuntaijiaju.cn

[Q55] 排名（并列占位）
来源：http://vo.newstarts.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://db.shxzskj.cn

[Q56] 密集排名（并列不占位）
来源：http://oz.asd995.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ju.jctech888.com.cn

[Q57] 行号
来源：http://bd.gzmigu.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://oy.shtwfgs.cn

[Q58] 累计求和
来源：http://ul.bookmarksfly.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ql.yuntaijiaju.cn

[Q59] 分组内累计
来源：http://ae.shtwfgs.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://we.jianghongdianzi.cn

[Q60] 取上一行 / 下一行
来源：http://ip.nszjky.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://vk.shtwfgs.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://pl.jctech888.com.cn

[Q61] 移动平均
来源：http://zc.jctech888.com.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://tx.nicolike.cn

[Q62] 分组占比
来源：http://dn.newstarts.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://bk.shtwfgs.cn

[Q63] 开启事务
来源：http://tz.asd995.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://pd.hahajie.cn

[Q64] 提交事务
来源：http://fo.chemitech.net.cn

COMMIT;
来源：http://br.shxzukj.cn

[Q65] 回滚事务
来源：http://tx.gzmigu.cn

ROLLBACK;
来源：http://jz.521024.cn

[Q66] 行锁查询
来源：http://ri.bookmarksfly.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://al.haigaiapp.cn

[Q67] 设置隔离级别
来源：http://jf.shxzukj.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://tb.szsharing.cn

[Q68] 保存点
来源：http://fm.bjjhwx.cn

SAVEPOINT sp1;
来源：http://pm.lnxyls.cn

ROLLBACK TO sp1;
来源：http://sv.9csxet.cn

[Q69] 查看执行计划
来源：http://ku.shxzukj.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://qx.huanxung.cn

[Q70] 更新统计信息
来源：http://sc.bookmarksfly.cn

ANALYZE TABLE users;
来源：http://tn.chemitech.net.cn

[Q71] 查看建表语句
来源：http://at.jctech888.com.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://td.yuntaijiaju.cn

[Q72] 查看索引
来源：http://up.shtwfgs.cn

SHOW INDEX FROM users;
来源：http://sq.huanxung.cn

[Q73] 查看表状态
来源：http://em.nszjky.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://zb.haigaiapp.cn

[Q74] 强制使用索引
来源：http://mx.muxihuayi.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://np.muxihuayi.cn

[Q75] 日期格式化
来源：http://pe.jctech888.com.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ha.hahajie.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://xm.521024.cn

[Q76] 按天统计
来源：http://sg.hahajie.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ug.lnxyls.cn

[Q77] 时间加减
来源：http://qw.newstarts.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://cw.colortex.cn

[Q78] 当前时间
来源：http://ea.huixinmuqiang.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://da.yuntaijiaju.cn

[Q79] 字符串拼接
来源：http://jx.newstarts.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://df.yuexingan06.cn

[Q80] 字符串截取
来源：http://jr.huixinmuqiang.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://cf.wgjwhj.cn

[Q81] 字符串替换
来源：http://wd.shxzukj.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://pn.huixinmuqiang.cn

[Q82] 字符长度与字节长度
来源：http://qw.9csxet.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://vq.jianghongdianzi.cn

[Q83] 大小写转换
来源：http://bu.9csxet.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hg.huixinmuqiang.cn

[Q84] 去除首尾空格
来源：http://hz.huanxung.cn

SELECT TRIM(name) FROM users;
来源：http://qr.bookmarksfly.cn

[Q85] 数值取整
来源：http://jo.shxzskj.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://nw.wgjwhj.cn

[Q86] 读取 JSON 字段
来源：http://wk.hnjuh.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://pw.panjiajie.cn

[Q87] JSON 字段做条件
来源：http://gs.nszjky.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wc.lnxyls.cn

[Q88] 行转列（条件聚合）
来源：http://dg.muxihuayi.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://eo.chemitech.net.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://dn.huixiangedu.cn

[Q89] 判断表是否存在
来源：http://mh.huanxung.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://dj.yuntaijiaju.cn

[Q90] 生成序号列
来源：http://jy.szsharing.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ya.wgjwhj.cn

================================================================================
来源：http://kg.panjiajie.cn

R. Bash 专题
来源：http://sr.yuexingan06.cn

================================================================================
来源：http://ld.szxytkj.cn

[R01] shebang 与严格模式
来源：http://qx.9csxet.cn

#!/usr/bin/env bash
来源：http://hs.asd995.cn

set -euo pipefail
来源：http://ue.szsharing.cn

[R02] 变量赋值与使用
来源：http://gs.szsharing.cn

name="Tom"; echo "$name"
来源：http://vj.lnxyls.cn

[R03] 只读变量
来源：http://gh.yuntaijiaju.cn

readonly PI=3.14
来源：http://hm.bjjhwx.cn

[R04] 位置参数
来源：http://kx.shtwfgs.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://zy.9csxet.cn

[R05] 参数默认值
来源：http://uv.gzmigu.cn

name="${1:-default}"
来源：http://jq.haigaiapp.cn

[R06] 判断命令是否存在
来源：http://bj.chemitech.net.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://go.chemitech.net.cn

[R07] if 判断文件
来源：http://th.szsharing.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://br.newstarts.cn

[R08] 数值比较
来源：http://zp.jctech888.com.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://be.shxzukj.cn

[R09] 字符串比较
来源：http://he.panjiajie.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://gh.szxytkj.cn

[R10] 正则匹配
来源：http://np.bjjhwx.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hd.huixiangedu.cn

[R11] case 多分支
来源：http://xt.shxzukj.cn

case "$1" in
来源：http://px.jctech888.com.cn

start) echo "启动" ;;
来源：http://ma.muxihuayi.cn

stop)  echo "停止" ;;
来源：http://tv.jianghongdianzi.cn

*)     echo "未知命令" ;;
来源：http://be.521024.cn

esac
来源：http://kq.yuexingan06.cn

[R12] for 遍历文件
来源：http://tl.huixinmuqiang.cn

for f in *.txt; do echo "$f"; done
来源：http://ym.jctech888.com.cn

[R13] for 计数循环
来源：http://al.shtwfgs.cn

for i in {1..10}; do echo "$i"; done
来源：http://cq.bjjhwx.cn

[R14] C 风格 for
来源：http://qx.shxzukj.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ji.colortex.cn

[R15] while 逐行读文件
来源：http://zk.hnjuh.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://gj.yuexingan06.cn

[R16] until 等待条件
来源：http://so.chemitech.net.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://xm.shxzukj.cn

[R17] 数组定义与取值
来源：http://lx.jianghongdianzi.cn


<!-- 参考信息 -->