代发 wailian999

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://qx.asd995.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://li.nicolike.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://gv.panjiajie.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://lr.nszjky.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ub.yuntaijiaju.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://gv.jctech888.com.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://qw.szxytkj.cn

[P04] 求长度
来源：http://by.jianghongdianzi.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ce.panjiajie.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://aa.9csxet.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://su.521024.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://vj.hnjuh.cn

Java: list.size();  map.size();  s.length()
来源：http://of.jianghongdianzi.cn

Go:   len(arr);  len(m)
来源：http://su.shtwfgs.cn

Ruby: x.length;  x.size
来源：http://dk.colortex.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://oo.nszjky.cn

[P05] 判断两个对象内容是否相等
来源：http://oi.hnjuh.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://fs.jctech888.com.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://xq.huanxung.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ge.shtwfgs.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ml.wgjwhj.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://pk.521024.cn

Go:   reflect.DeepEqual(a, b)
来源：http://kc.wgjwhj.cn

Ruby: a == b
来源：http://fg.panjiajie.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://fx.9csxet.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://bx.jctech888.com.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ss.yuntaijiaju.cn

PHP:  if (empty($x)) {}
来源：http://ie.hnjuh.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://yo.jctech888.com.cn

TS:   if (x == null) {}
来源：http://oz.gzmigu.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://ei.bjjhwx.cn

Go:   if x == nil {}
来源：http://di.yuexingan06.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://sz.lnxyls.cn

C#:   if (x is null) {}
来源：http://ux.huanxung.cn

[P07] 防抖与节流
来源：http://cr.jctech888.com.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://gb.gzmigu.cn

PHP:  // 手写时间戳比较
来源：http://pm.muxihuayi.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://fn.bjjhwx.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://dy.huixiangedu.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://er.bjjhwx.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://sy.muxihuayi.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://dn.hnjuh.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ty.haigaiapp.cn

[P08] 处理浮点精度问题
来源：http://ip.yuexingan06.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://gg.panjiajie.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://sn.hahajie.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://av.yuexingan06.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://nb.lnxyls.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://fw.haigaiapp.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ts.jianghongdianzi.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ao.yuexingan06.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://bj.hnjuh.cn

================================================================================
来源：http://ae.jianghongdianzi.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wu.hahajie.cn

================================================================================
来源：http://pl.yuexingan06.cn

[Q01] 创建表
来源：http://ul.szsharing.cn

CREATE TABLE users (
来源：http://ao.shxzskj.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mk.shtwfgs.cn

name VARCHAR(50) NOT NULL,
来源：http://or.panjiajie.cn

email VARCHAR(100) UNIQUE,
来源：http://be.gzmigu.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hl.shtwfgs.cn

);
来源：http://qx.haigaiapp.cn

[Q02] 创建带外键的表
来源：http://es.521024.cn

CREATE TABLE orders (
来源：http://qa.9csxet.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://or.muxihuayi.cn

user_id INT NOT NULL,
来源：http://fm.huixiangedu.cn

amount DECIMAL(10, 2),
来源：http://pi.huixiangedu.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mo.shxzskj.cn

);
来源：http://ln.chemitech.net.cn

[Q03] 增加列
来源：http://pk.szsharing.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wb.yuntaijiaju.cn

[Q04] 修改列类型
来源：http://jr.yuexingan06.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wy.jianghongdianzi.cn

[Q05] 重命名列
来源：http://sa.hahajie.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wy.huanxung.cn

[Q06] 删除列
来源：http://oz.521024.cn

ALTER TABLE users DROP COLUMN age;
来源：http://av.muxihuayi.cn

[Q07] 删除表
来源：http://yx.szsharing.cn

DROP TABLE IF EXISTS orders;
来源：http://ee.chemitech.net.cn

[Q08] 创建普通索引
来源：http://oq.jctech888.com.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://vo.huixiangedu.cn

[Q09] 创建唯一索引
来源：http://ot.jianghongdianzi.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://qe.nicolike.cn

[Q10] 插入单行
来源：http://ox.colortex.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://pd.yuntaijiaju.cn

[Q11] 一次插入多行
来源：http://kl.muxihuayi.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://qn.panjiajie.cn

[Q12] 插入后取自增 ID
来源：http://lr.newstarts.cn

INSERT INTO users (name) VALUES ('C');
来源：http://au.521024.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://fn.gzmigu.cn

[Q13] 忽略重复插入
来源：http://ii.panjiajie.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://kr.jianghongdianzi.cn

[Q14] 存在则更新（upsert）
来源：http://fd.hnjuh.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://vx.chemitech.net.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://kp.haigaiapp.cn

[Q15] 查询全部
来源：http://bt.gzmigu.cn

SELECT * FROM users;
来源：http://jo.huanxung.cn

[Q16] 查询指定列
来源：http://sw.yuexingan06.cn

SELECT id, name FROM users;
来源：http://vz.nszjky.cn

[Q17] 条件查询
来源：http://ec.hnjuh.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://bt.yuntaijiaju.cn

[Q18] 模糊匹配
来源：http://po.jctech888.com.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://zi.muxihuayi.cn

[Q19] 范围查询
来源：http://pf.yuntaijiaju.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ly.lnxyls.cn

[Q20] IN 列表
来源：http://ln.gzmigu.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ie.haigaiapp.cn

[Q21] 空值判断
来源：http://dc.gzmigu.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://hw.shtwfgs.cn

[Q22] 排序
来源：http://pm.chemitech.net.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://tl.bjjhwx.cn

[Q23] 分页
来源：http://uf.shxzskj.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://qf.9csxet.cn

[Q24] 去重
来源：http://ng.colortex.cn

SELECT DISTINCT city FROM users;
来源：http://rz.huixiangedu.cn

[Q25] 只取前 N 条
来源：http://fm.hahajie.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://oy.bookmarksfly.cn

[Q26] 计数
来源：http://zr.lnxyls.cn

SELECT COUNT(*) FROM users;
来源：http://pe.521024.cn

[Q27] 条件计数
来源：http://em.hahajie.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://dt.nicolike.cn

[Q28] 求和与平均
来源：http://vx.shxzskj.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://xl.yuexingan06.cn

[Q29] 最大最小值
来源：http://vh.huanxung.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://ff.shxzukj.cn

[Q30] 分组统计
来源：http://hw.yuexingan06.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://gf.hahajie.cn

[Q31] 分组后过滤
来源：http://bc.shtwfgs.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://vc.chemitech.net.cn

[Q32] 分组拼接字符串
来源：http://fz.huixiangedu.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hi.chemitech.net.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wb.haigaiapp.cn

[Q33] 多列分组
来源：http://hr.yuntaijiaju.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://uw.yuexingan06.cn

[Q34] 每组取第一条
来源：http://kn.szsharing.cn

SELECT * FROM (
来源：http://kb.newstarts.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://dl.muxihuayi.cn

) t WHERE rn = 1;
来源：http://aj.szsharing.cn

[Q35] 内连接
来源：http://ho.bjjhwx.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://qk.hnjuh.cn

[Q36] 左连接
来源：http://do.hahajie.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://da.jianghongdianzi.cn

[Q37] 右连接
来源：http://dj.panjiajie.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://sf.shtwfgs.cn

[Q38] 全外连接（PostgreSQL）
来源：http://yo.yuntaijiaju.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://df.huixinmuqiang.cn

[Q39] 自连接（查上下级）
来源：http://lv.szsharing.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://ze.yuntaijiaju.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mh.lnxyls.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://hu.newstarts.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://kc.jctech888.com.cn

[Q41] 多表连接
来源：http://cx.asd995.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://bz.szsharing.cn

JOIN users u ON u.id = o.user_id
来源：http://tx.wgjwhj.cn

JOIN products p ON p.id = o.product_id;
来源：http://jf.jianghongdianzi.cn

[Q42] 连接条件附加过滤
来源：http://qy.haigaiapp.cn

SELECT u.name, o.amount FROM users u
来源：http://bm.lnxyls.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://na.shtwfgs.cn

[Q43] 标量子查询
来源：http://zm.panjiajie.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://kz.nszjky.cn

[Q44] IN 子查询
来源：http://pq.newstarts.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://sb.nszjky.cn

[Q45] EXISTS 判断存在
来源：http://cl.jctech888.com.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://uh.shxzskj.cn

[Q46] NOT EXISTS 判断不存在
来源：http://sx.shxzskj.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://lo.521024.cn

[Q47] 与平均值比较
来源：http://co.gzmigu.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://yi.nszjky.cn

[Q48] CTE 公用表表达式
来源：http://nk.hahajie.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ba.yuntaijiaju.cn

SELECT * FROM t WHERE c > 5;
来源：http://uf.huixiangedu.cn

[Q49] 更新单行
来源：http://jm.hahajie.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wr.9csxet.cn

[Q50] 批量更新
来源：http://gm.hahajie.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://jq.colortex.cn

[Q51] 用子查询更新
来源：http://vr.bjjhwx.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://uf.szxytkj.cn

[Q52] 删除指定行
来源：http://ej.panjiajie.cn

DELETE FROM users WHERE id = 10;
来源：http://er.szsharing.cn

[Q53] 按条件删除
来源：http://tg.huanxung.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://nm.9csxet.cn

[Q54] 清空表
来源：http://wc.nszjky.cn

TRUNCATE TABLE logs;
来源：http://hi.shxzskj.cn

[Q55] 排名（并列占位）
来源：http://sw.huanxung.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://vz.szsharing.cn

[Q56] 密集排名（并列不占位）
来源：http://ry.nszjky.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://xb.szxytkj.cn

[Q57] 行号
来源：http://fv.yuntaijiaju.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://xy.asd995.cn

[Q58] 累计求和
来源：http://yk.shxzukj.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://xb.gzmigu.cn

[Q59] 分组内累计
来源：http://pt.bookmarksfly.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://cj.bjjhwx.cn

[Q60] 取上一行 / 下一行
来源：http://pi.huanxung.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://xr.9csxet.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ia.yuntaijiaju.cn

[Q61] 移动平均
来源：http://tt.9csxet.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://pj.shxzskj.cn

[Q62] 分组占比
来源：http://ue.shxzskj.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ct.bookmarksfly.cn

[Q63] 开启事务
来源：http://ew.lnxyls.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://qp.nszjky.cn

[Q64] 提交事务
来源：http://cz.colortex.cn

COMMIT;
来源：http://me.hnjuh.cn

[Q65] 回滚事务
来源：http://hf.lnxyls.cn

ROLLBACK;
来源：http://bg.shtwfgs.cn

[Q66] 行锁查询
来源：http://jz.hnjuh.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://je.nicolike.cn

[Q67] 设置隔离级别
来源：http://vr.szsharing.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://co.szsharing.cn

[Q68] 保存点
来源：http://xm.yuntaijiaju.cn

SAVEPOINT sp1;
来源：http://io.lnxyls.cn

ROLLBACK TO sp1;
来源：http://go.hnjuh.cn

[Q69] 查看执行计划
来源：http://yj.newstarts.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://um.chemitech.net.cn

[Q70] 更新统计信息
来源：http://ir.newstarts.cn

ANALYZE TABLE users;
来源：http://ll.521024.cn

[Q71] 查看建表语句
来源：http://bs.lnxyls.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ti.hahajie.cn

[Q72] 查看索引
来源：http://bo.lnxyls.cn

SHOW INDEX FROM users;
来源：http://ln.chemitech.net.cn

[Q73] 查看表状态
来源：http://pp.jianghongdianzi.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://cu.521024.cn

[Q74] 强制使用索引
来源：http://lt.shxzskj.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://cr.huixiangedu.cn

[Q75] 日期格式化
来源：http://ls.521024.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ql.nicolike.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://tz.asd995.cn

[Q76] 按天统计
来源：http://yi.szsharing.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://sk.panjiajie.cn

[Q77] 时间加减
来源：http://aw.yuexingan06.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://pt.yuexingan06.cn

[Q78] 当前时间
来源：http://xq.wgjwhj.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://oi.gzmigu.cn

[Q79] 字符串拼接
来源：http://bs.asd995.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hr.9csxet.cn

[Q80] 字符串截取
来源：http://re.yuexingan06.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mf.nszjky.cn

[Q81] 字符串替换
来源：http://xo.huixinmuqiang.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://xc.hahajie.cn

[Q82] 字符长度与字节长度
来源：http://za.huixinmuqiang.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://jd.muxihuayi.cn

[Q83] 大小写转换
来源：http://lg.bjjhwx.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hx.haigaiapp.cn

[Q84] 去除首尾空格
来源：http://bz.chemitech.net.cn

SELECT TRIM(name) FROM users;
来源：http://eb.521024.cn

[Q85] 数值取整
来源：http://lz.haigaiapp.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mz.panjiajie.cn

[Q86] 读取 JSON 字段
来源：http://bp.huixiangedu.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://re.yuexingan06.cn

[Q87] JSON 字段做条件
来源：http://nt.hahajie.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://nx.asd995.cn

[Q88] 行转列（条件聚合）
来源：http://lh.szxytkj.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://um.muxihuayi.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wk.haigaiapp.cn

[Q89] 判断表是否存在
来源：http://pr.lnxyls.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://nq.hahajie.cn

[Q90] 生成序号列
来源：http://vo.yuntaijiaju.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ea.colortex.cn

================================================================================
来源：http://yo.yuntaijiaju.cn

R. Bash 专题
来源：http://qx.asd995.cn

================================================================================
来源：http://gj.huixiangedu.cn

[R01] shebang 与严格模式
来源：http://nb.shtwfgs.cn

#!/usr/bin/env bash
来源：http://fy.chemitech.net.cn

set -euo pipefail
来源：http://yr.shtwfgs.cn

[R02] 变量赋值与使用
来源：http://zn.hnjuh.cn

name="Tom"; echo "$name"
来源：http://yp.huixinmuqiang.cn

[R03] 只读变量
来源：http://ll.bjjhwx.cn

readonly PI=3.14
来源：http://ia.gzmigu.cn

[R04] 位置参数
来源：http://al.panjiajie.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://it.hnjuh.cn

[R05] 参数默认值
来源：http://ji.jctech888.com.cn

name="${1:-default}"
来源：http://os.huixiangedu.cn

[R06] 判断命令是否存在
来源：http://zj.shxzukj.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wz.szxytkj.cn

[R07] if 判断文件
来源：http://fw.jctech888.com.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hs.hahajie.cn

[R08] 数值比较
来源：http://gh.lnxyls.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://am.hahajie.cn

[R09] 字符串比较
来源：http://rl.521024.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ls.hahajie.cn

[R10] 正则匹配
来源：http://zx.wgjwhj.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://iz.shxzukj.cn

[R11] case 多分支
来源：http://vz.hnjuh.cn

case "$1" in
来源：http://zc.chemitech.net.cn

start) echo "启动" ;;
来源：http://mk.wgjwhj.cn

stop)  echo "停止" ;;
来源：http://ol.lnxyls.cn

*)     echo "未知命令" ;;
来源：http://gt.bookmarksfly.cn

esac
来源：http://zt.shxzukj.cn

[R12] for 遍历文件
来源：http://rs.hnjuh.cn

for f in *.txt; do echo "$f"; done
来源：http://hs.haigaiapp.cn

[R13] for 计数循环
来源：http://ti.jianghongdianzi.cn

for i in {1..10}; do echo "$i"; done
来源：http://ww.9csxet.cn

[R14] C 风格 for
来源：http://pr.bjjhwx.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://kg.panjiajie.cn

[R15] while 逐行读文件
来源：http://hr.newstarts.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://rr.jctech888.com.cn

[R16] until 等待条件
来源：http://xr.asd995.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://pb.jctech888.com.cn

[R17] 数组定义与取值
来源：http://ro.yuexingan06.cn


<!-- 参考信息 -->