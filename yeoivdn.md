代发 wailian999

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://gc.huanxung.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://it.huixinmuqiang.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://oc.huanxung.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://yg.hahajie.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://kh.chemitech.net.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://ao.lnxyls.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://vp.bookmarksfly.cn

[P04] 求长度
来源：http://be.521024.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://kw.hnjuh.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ga.bjjhwx.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ee.521024.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://sy.shxzukj.cn

Java: list.size();  map.size();  s.length()
来源：http://oz.nszjky.cn

Go:   len(arr);  len(m)
来源：http://mk.gzmigu.cn

Ruby: x.length;  x.size
来源：http://wy.szxytkj.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://sz.shxzukj.cn

[P05] 判断两个对象内容是否相等
来源：http://tb.shtwfgs.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://za.521024.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://qv.bookmarksfly.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wh.szsharing.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://nd.jianghongdianzi.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://xu.lnxyls.cn

Go:   reflect.DeepEqual(a, b)
来源：http://dy.9csxet.cn

Ruby: a == b
来源：http://qz.521024.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hw.wgjwhj.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://kl.shxzukj.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hd.bookmarksfly.cn

PHP:  if (empty($x)) {}
来源：http://ht.asd995.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://qg.szsharing.cn

TS:   if (x == null) {}
来源：http://zw.shtwfgs.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://mc.jctech888.com.cn

Go:   if x == nil {}
来源：http://uk.yuntaijiaju.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://of.huanxung.cn

C#:   if (x is null) {}
来源：http://dg.bookmarksfly.cn

[P07] 防抖与节流
来源：http://bm.nicolike.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://lk.bjjhwx.cn

PHP:  // 手写时间戳比较
来源：http://bn.jctech888.com.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://cc.jctech888.com.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://zv.9csxet.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ja.bjjhwx.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://du.panjiajie.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://ho.huanxung.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mj.jctech888.com.cn

[P08] 处理浮点精度问题
来源：http://wj.521024.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ik.9csxet.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://oy.yuntaijiaju.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hu.yuexingan06.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://gn.9csxet.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://nl.szsharing.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://zu.9csxet.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ck.nszjky.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hx.huanxung.cn

================================================================================
来源：http://wg.jctech888.com.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://oq.nszjky.cn

================================================================================
来源：http://ju.wgjwhj.cn

[Q01] 创建表
来源：http://ic.lnxyls.cn

CREATE TABLE users (
来源：http://jt.shxzukj.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://sx.hnjuh.cn

name VARCHAR(50) NOT NULL,
来源：http://sa.huixiangedu.cn

email VARCHAR(100) UNIQUE,
来源：http://yf.colortex.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ak.szxytkj.cn

);
来源：http://gp.nicolike.cn

[Q02] 创建带外键的表
来源：http://my.jianghongdianzi.cn

CREATE TABLE orders (
来源：http://nv.chemitech.net.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://gq.bjjhwx.cn

user_id INT NOT NULL,
来源：http://vv.chemitech.net.cn

amount DECIMAL(10, 2),
来源：http://jr.huixinmuqiang.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ys.haigaiapp.cn

);
来源：http://ed.chemitech.net.cn

[Q03] 增加列
来源：http://fb.chemitech.net.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wj.9csxet.cn

[Q04] 修改列类型
来源：http://tk.jctech888.com.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://by.haigaiapp.cn

[Q05] 重命名列
来源：http://wu.huixiangedu.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://er.shxzukj.cn

[Q06] 删除列
来源：http://uy.lnxyls.cn

ALTER TABLE users DROP COLUMN age;
来源：http://ym.colortex.cn

[Q07] 删除表
来源：http://qo.huixinmuqiang.cn

DROP TABLE IF EXISTS orders;
来源：http://tc.huixinmuqiang.cn

[Q08] 创建普通索引
来源：http://fu.shtwfgs.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://ba.yuntaijiaju.cn

[Q09] 创建唯一索引
来源：http://me.bjjhwx.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://xq.wgjwhj.cn

[Q10] 插入单行
来源：http://xr.hnjuh.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://lk.szsharing.cn

[Q11] 一次插入多行
来源：http://yx.shtwfgs.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://tk.yuntaijiaju.cn

[Q12] 插入后取自增 ID
来源：http://hd.colortex.cn

INSERT INTO users (name) VALUES ('C');
来源：http://ug.jctech888.com.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mm.panjiajie.cn

[Q13] 忽略重复插入
来源：http://mj.bookmarksfly.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://si.9csxet.cn

[Q14] 存在则更新（upsert）
来源：http://ho.shxzukj.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://lg.colortex.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://jl.shtwfgs.cn

[Q15] 查询全部
来源：http://ny.shtwfgs.cn

SELECT * FROM users;
来源：http://ie.muxihuayi.cn

[Q16] 查询指定列
来源：http://le.wgjwhj.cn

SELECT id, name FROM users;
来源：http://ny.jianghongdianzi.cn

[Q17] 条件查询
来源：http://wl.9csxet.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://lt.yuntaijiaju.cn

[Q18] 模糊匹配
来源：http://yv.szxytkj.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://jj.shtwfgs.cn

[Q19] 范围查询
来源：http://zo.szxytkj.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ft.muxihuayi.cn

[Q20] IN 列表
来源：http://nw.huixiangedu.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://rl.shtwfgs.cn

[Q21] 空值判断
来源：http://rj.nszjky.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://ui.yuntaijiaju.cn

[Q22] 排序
来源：http://qy.nszjky.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://pk.9csxet.cn

[Q23] 分页
来源：http://rn.lnxyls.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://cq.szsharing.cn

[Q24] 去重
来源：http://ka.shxzskj.cn

SELECT DISTINCT city FROM users;
来源：http://wo.lnxyls.cn

[Q25] 只取前 N 条
来源：http://hw.9csxet.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://sz.wgjwhj.cn

[Q26] 计数
来源：http://ov.gzmigu.cn

SELECT COUNT(*) FROM users;
来源：http://av.nicolike.cn

[Q27] 条件计数
来源：http://qa.asd995.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://yf.huixinmuqiang.cn

[Q28] 求和与平均
来源：http://eh.wgjwhj.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://gi.colortex.cn

[Q29] 最大最小值
来源：http://cu.lnxyls.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://ha.9csxet.cn

[Q30] 分组统计
来源：http://gq.huixinmuqiang.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://qf.shxzukj.cn

[Q31] 分组后过滤
来源：http://sk.panjiajie.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://uc.bjjhwx.cn

[Q32] 分组拼接字符串
来源：http://de.shtwfgs.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://yi.wgjwhj.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://pg.9csxet.cn

[Q33] 多列分组
来源：http://af.asd995.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://fq.bjjhwx.cn

[Q34] 每组取第一条
来源：http://ur.newstarts.cn

SELECT * FROM (
来源：http://yj.521024.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://vo.huixinmuqiang.cn

) t WHERE rn = 1;
来源：http://yv.shxzukj.cn

[Q35] 内连接
来源：http://pm.panjiajie.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://yp.colortex.cn

[Q36] 左连接
来源：http://wi.wgjwhj.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://bm.yuntaijiaju.cn

[Q37] 右连接
来源：http://zw.asd995.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://rn.haigaiapp.cn

[Q38] 全外连接（PostgreSQL）
来源：http://pm.huanxung.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ca.shxzukj.cn

[Q39] 自连接（查上下级）
来源：http://em.newstarts.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://gp.muxihuayi.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://yn.huanxung.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://df.yuntaijiaju.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ez.bookmarksfly.cn

[Q41] 多表连接
来源：http://ez.haigaiapp.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://pa.shxzukj.cn

JOIN users u ON u.id = o.user_id
来源：http://ba.9csxet.cn

JOIN products p ON p.id = o.product_id;
来源：http://ww.hnjuh.cn

[Q42] 连接条件附加过滤
来源：http://ps.haigaiapp.cn

SELECT u.name, o.amount FROM users u
来源：http://bb.wgjwhj.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://pk.shxzskj.cn

[Q43] 标量子查询
来源：http://ey.jianghongdianzi.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ny.huanxung.cn

[Q44] IN 子查询
来源：http://pg.nszjky.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://oo.bjjhwx.cn

[Q45] EXISTS 判断存在
来源：http://lv.szxytkj.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://kd.huixiangedu.cn

[Q46] NOT EXISTS 判断不存在
来源：http://hb.colortex.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ge.wgjwhj.cn

[Q47] 与平均值比较
来源：http://yi.hnjuh.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://gb.bookmarksfly.cn

[Q48] CTE 公用表表达式
来源：http://yi.nszjky.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hb.asd995.cn

SELECT * FROM t WHERE c > 5;
来源：http://ao.szsharing.cn

[Q49] 更新单行
来源：http://pg.szxytkj.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://cz.szxytkj.cn

[Q50] 批量更新
来源：http://sm.lnxyls.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://oi.shxzskj.cn

[Q51] 用子查询更新
来源：http://yh.yuexingan06.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://ec.huixiangedu.cn

[Q52] 删除指定行
来源：http://ke.panjiajie.cn

DELETE FROM users WHERE id = 10;
来源：http://wt.yuexingan06.cn

[Q53] 按条件删除
来源：http://tt.lnxyls.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://tr.chemitech.net.cn

[Q54] 清空表
来源：http://iu.hnjuh.cn

TRUNCATE TABLE logs;
来源：http://qn.9csxet.cn

[Q55] 排名（并列占位）
来源：http://ih.9csxet.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://py.asd995.cn

[Q56] 密集排名（并列不占位）
来源：http://cw.wgjwhj.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://zw.haigaiapp.cn

[Q57] 行号
来源：http://cb.huixinmuqiang.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://bt.jianghongdianzi.cn

[Q58] 累计求和
来源：http://ka.muxihuayi.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ia.szxytkj.cn

[Q59] 分组内累计
来源：http://wb.chemitech.net.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://kq.521024.cn

[Q60] 取上一行 / 下一行
来源：http://vc.jianghongdianzi.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://sh.9csxet.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://zz.bjjhwx.cn

[Q61] 移动平均
来源：http://yw.shtwfgs.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://iz.newstarts.cn

[Q62] 分组占比
来源：http://mk.muxihuayi.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://fd.521024.cn

[Q63] 开启事务
来源：http://yl.lnxyls.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://pm.newstarts.cn

[Q64] 提交事务
来源：http://xf.shxzukj.cn

COMMIT;
来源：http://nd.nszjky.cn

[Q65] 回滚事务
来源：http://dc.panjiajie.cn

ROLLBACK;
来源：http://tl.asd995.cn

[Q66] 行锁查询
来源：http://ud.chemitech.net.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ku.newstarts.cn

[Q67] 设置隔离级别
来源：http://et.hahajie.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://vx.bookmarksfly.cn

[Q68] 保存点
来源：http://qy.521024.cn

SAVEPOINT sp1;
来源：http://js.szsharing.cn

ROLLBACK TO sp1;
来源：http://od.haigaiapp.cn

[Q69] 查看执行计划
来源：http://xh.bookmarksfly.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://gm.hahajie.cn

[Q70] 更新统计信息
来源：http://nq.hnjuh.cn

ANALYZE TABLE users;
来源：http://qb.nszjky.cn

[Q71] 查看建表语句
来源：http://lx.bjjhwx.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://pm.wgjwhj.cn

[Q72] 查看索引
来源：http://mr.yuntaijiaju.cn

SHOW INDEX FROM users;
来源：http://gy.szxytkj.cn

[Q73] 查看表状态
来源：http://ej.bookmarksfly.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://dy.muxihuayi.cn

[Q74] 强制使用索引
来源：http://pg.newstarts.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://do.chemitech.net.cn

[Q75] 日期格式化
来源：http://ki.newstarts.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://up.jianghongdianzi.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ut.asd995.cn

[Q76] 按天统计
来源：http://fw.lnxyls.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ip.yuexingan06.cn

[Q77] 时间加减
来源：http://lt.hnjuh.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://sj.newstarts.cn

[Q78] 当前时间
来源：http://bs.shtwfgs.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://cc.bjjhwx.cn

[Q79] 字符串拼接
来源：http://cm.huixiangedu.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://bf.haigaiapp.cn

[Q80] 字符串截取
来源：http://qg.szsharing.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hf.gzmigu.cn

[Q81] 字符串替换
来源：http://mf.newstarts.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hv.asd995.cn

[Q82] 字符长度与字节长度
来源：http://db.chemitech.net.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ux.huixinmuqiang.cn

[Q83] 大小写转换
来源：http://jr.hahajie.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://xb.newstarts.cn

[Q84] 去除首尾空格
来源：http://qp.9csxet.cn

SELECT TRIM(name) FROM users;
来源：http://vq.szxytkj.cn

[Q85] 数值取整
来源：http://mp.yuntaijiaju.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://xn.huixiangedu.cn

[Q86] 读取 JSON 字段
来源：http://wz.huixiangedu.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://oy.panjiajie.cn

[Q87] JSON 字段做条件
来源：http://je.huanxung.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hh.521024.cn

[Q88] 行转列（条件聚合）
来源：http://kz.huixinmuqiang.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ig.9csxet.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://px.shxzukj.cn

[Q89] 判断表是否存在
来源：http://jz.bjjhwx.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://cz.jctech888.com.cn

[Q90] 生成序号列
来源：http://qw.colortex.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hc.bjjhwx.cn

================================================================================
来源：http://zi.wgjwhj.cn

R. Bash 专题
来源：http://zl.newstarts.cn

================================================================================
来源：http://uh.hnjuh.cn

[R01] shebang 与严格模式
来源：http://je.shxzukj.cn

#!/usr/bin/env bash
来源：http://bc.shxzskj.cn

set -euo pipefail
来源：http://ff.yuntaijiaju.cn

[R02] 变量赋值与使用
来源：http://st.shtwfgs.cn

name="Tom"; echo "$name"
来源：http://xw.hahajie.cn

[R03] 只读变量
来源：http://pu.bookmarksfly.cn

readonly PI=3.14
来源：http://gm.lnxyls.cn

[R04] 位置参数
来源：http://cd.huanxung.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://qu.asd995.cn

[R05] 参数默认值
来源：http://aj.nicolike.cn

name="${1:-default}"
来源：http://og.9csxet.cn

[R06] 判断命令是否存在
来源：http://dp.hahajie.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://kh.szxytkj.cn

[R07] if 判断文件
来源：http://yy.huanxung.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://rq.hahajie.cn

[R08] 数值比较
来源：http://gv.newstarts.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://be.wgjwhj.cn

[R09] 字符串比较
来源：http://pk.yuntaijiaju.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://kg.shxzukj.cn

[R10] 正则匹配
来源：http://ik.jianghongdianzi.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://rg.yuntaijiaju.cn

[R11] case 多分支
来源：http://df.bjjhwx.cn

case "$1" in
来源：http://vg.bookmarksfly.cn

start) echo "启动" ;;
来源：http://jj.shtwfgs.cn

stop)  echo "停止" ;;
来源：http://ot.panjiajie.cn

*)     echo "未知命令" ;;
来源：http://id.szsharing.cn

esac
来源：http://rp.asd995.cn

[R12] for 遍历文件
来源：http://od.wgjwhj.cn

for f in *.txt; do echo "$f"; done
来源：http://lz.nszjky.cn

[R13] for 计数循环
来源：http://ln.hahajie.cn

for i in {1..10}; do echo "$i"; done
来源：http://ec.yuntaijiaju.cn

[R14] C 风格 for
来源：http://un.jctech888.com.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ch.panjiajie.cn

[R15] while 逐行读文件
来源：http://li.colortex.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ys.9csxet.cn

[R16] until 等待条件
来源：http://ad.hnjuh.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://rm.wgjwhj.cn

[R17] 数组定义与取值
来源：http://qt.bookmarksfly.cn


<!-- 参考信息 -->