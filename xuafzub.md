代发 wailian999

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wj.chemitech.net.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://aj.jianghongdianzi.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://yh.521024.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ya.hnjuh.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ur.hnjuh.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://wd.huanxung.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://cr.asd995.cn

[P04] 求长度
来源：http://hy.panjiajie.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://en.shtwfgs.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://za.jctech888.com.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://qo.9csxet.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://sa.colortex.cn

Java: list.size();  map.size();  s.length()
来源：http://uc.9csxet.cn

Go:   len(arr);  len(m)
来源：http://ck.yuexingan06.cn

Ruby: x.length;  x.size
来源：http://vg.szxytkj.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://yp.muxihuayi.cn

[P05] 判断两个对象内容是否相等
来源：http://bu.wgjwhj.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://ia.bookmarksfly.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://co.yuntaijiaju.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://eg.shxzukj.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://kh.huixinmuqiang.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://lg.huixinmuqiang.cn

Go:   reflect.DeepEqual(a, b)
来源：http://vr.wgjwhj.cn

Ruby: a == b
来源：http://ww.nicolike.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ou.muxihuayi.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://iq.jctech888.com.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://id.szxytkj.cn

PHP:  if (empty($x)) {}
来源：http://as.haigaiapp.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wo.shxzskj.cn

TS:   if (x == null) {}
来源：http://nl.chemitech.net.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.9csxet.cn

Go:   if x == nil {}
来源：http://mt.lnxyls.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://gk.nicolike.cn

C#:   if (x is null) {}
来源：http://nc.huixinmuqiang.cn

[P07] 防抖与节流
来源：http://uu.colortex.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://tr.bjjhwx.cn

PHP:  // 手写时间戳比较
来源：http://pv.haigaiapp.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://pd.colortex.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hb.shtwfgs.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://lb.521024.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://bc.bookmarksfly.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://ey.huixinmuqiang.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://qg.wgjwhj.cn

[P08] 处理浮点精度问题
来源：http://lf.wgjwhj.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wd.colortex.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://fs.9csxet.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://qj.9csxet.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://yc.panjiajie.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://go.newstarts.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hq.szxytkj.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://fr.bjjhwx.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://pf.shxzukj.cn

================================================================================
来源：http://im.huanxung.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://pv.huixiangedu.cn

================================================================================
来源：http://df.huanxung.cn

[Q01] 创建表
来源：http://ds.chemitech.net.cn

CREATE TABLE users (
来源：http://zo.shxzukj.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://kb.521024.cn

name VARCHAR(50) NOT NULL,
来源：http://pe.bookmarksfly.cn

email VARCHAR(100) UNIQUE,
来源：http://oo.huixiangedu.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mb.521024.cn

);
来源：http://mx.shtwfgs.cn

[Q02] 创建带外键的表
来源：http://xe.szsharing.cn

CREATE TABLE orders (
来源：http://bq.nszjky.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://xq.shxzskj.cn

user_id INT NOT NULL,
来源：http://bd.haigaiapp.cn

amount DECIMAL(10, 2),
来源：http://zl.szxytkj.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wg.lnxyls.cn

);
来源：http://ps.nicolike.cn

[Q03] 增加列
来源：http://vb.newstarts.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ez.szxytkj.cn

[Q04] 修改列类型
来源：http://pf.hnjuh.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://uy.hahajie.cn

[Q05] 重命名列
来源：http://dh.hahajie.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://sh.9csxet.cn

[Q06] 删除列
来源：http://pp.nszjky.cn

ALTER TABLE users DROP COLUMN age;
来源：http://bi.shtwfgs.cn

[Q07] 删除表
来源：http://dz.newstarts.cn

DROP TABLE IF EXISTS orders;
来源：http://to.chemitech.net.cn

[Q08] 创建普通索引
来源：http://rf.chemitech.net.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://oe.wgjwhj.cn

[Q09] 创建唯一索引
来源：http://qu.wgjwhj.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://tp.bjjhwx.cn

[Q10] 插入单行
来源：http://el.lnxyls.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://nv.wgjwhj.cn

[Q11] 一次插入多行
来源：http://sv.hnjuh.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mw.szsharing.cn

[Q12] 插入后取自增 ID
来源：http://jy.huixiangedu.cn

INSERT INTO users (name) VALUES ('C');
来源：http://yx.huixinmuqiang.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://xs.jctech888.com.cn

[Q13] 忽略重复插入
来源：http://jq.szxytkj.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://qm.bookmarksfly.cn

[Q14] 存在则更新（upsert）
来源：http://im.jianghongdianzi.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://xk.panjiajie.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://iv.9csxet.cn

[Q15] 查询全部
来源：http://is.huanxung.cn

SELECT * FROM users;
来源：http://yp.shxzukj.cn

[Q16] 查询指定列
来源：http://zd.yuntaijiaju.cn

SELECT id, name FROM users;
来源：http://xw.newstarts.cn

[Q17] 条件查询
来源：http://cn.huixiangedu.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hu.yuexingan06.cn

[Q18] 模糊匹配
来源：http://ut.jctech888.com.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://dj.szsharing.cn

[Q19] 范围查询
来源：http://oa.hahajie.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://sv.huixiangedu.cn

[Q20] IN 列表
来源：http://sf.colortex.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ch.wgjwhj.cn

[Q21] 空值判断
来源：http://gg.newstarts.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://ix.huixiangedu.cn

[Q22] 排序
来源：http://pe.521024.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ji.wgjwhj.cn

[Q23] 分页
来源：http://wz.bjjhwx.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://en.jctech888.com.cn

[Q24] 去重
来源：http://jt.yuntaijiaju.cn

SELECT DISTINCT city FROM users;
来源：http://pw.newstarts.cn

[Q25] 只取前 N 条
来源：http://ln.muxihuayi.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://xs.shxzskj.cn

[Q26] 计数
来源：http://dy.colortex.cn

SELECT COUNT(*) FROM users;
来源：http://bh.nszjky.cn

[Q27] 条件计数
来源：http://js.yuntaijiaju.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://kj.9csxet.cn

[Q28] 求和与平均
来源：http://fd.bjjhwx.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://gj.colortex.cn

[Q29] 最大最小值
来源：http://tu.colortex.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://kz.chemitech.net.cn

[Q30] 分组统计
来源：http://ec.muxihuayi.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://xt.panjiajie.cn

[Q31] 分组后过滤
来源：http://hy.chemitech.net.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wl.huixiangedu.cn

[Q32] 分组拼接字符串
来源：http://eg.bookmarksfly.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://uj.shxzukj.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ox.haigaiapp.cn

[Q33] 多列分组
来源：http://wl.panjiajie.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hi.chemitech.net.cn

[Q34] 每组取第一条
来源：http://dc.huanxung.cn

SELECT * FROM (
来源：http://en.hnjuh.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://pc.lnxyls.cn

) t WHERE rn = 1;
来源：http://db.jianghongdianzi.cn

[Q35] 内连接
来源：http://ug.huixinmuqiang.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://kq.bookmarksfly.cn

[Q36] 左连接
来源：http://ng.szsharing.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://bv.wgjwhj.cn

[Q37] 右连接
来源：http://ks.asd995.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://pt.hnjuh.cn

[Q38] 全外连接（PostgreSQL）
来源：http://du.yuexingan06.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://gf.shxzukj.cn

[Q39] 自连接（查上下级）
来源：http://mw.muxihuayi.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://we.huixiangedu.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://vj.nicolike.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://ca.nszjky.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://zb.panjiajie.cn

[Q41] 多表连接
来源：http://xk.huixiangedu.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://ha.panjiajie.cn

JOIN users u ON u.id = o.user_id
来源：http://nc.huixinmuqiang.cn

JOIN products p ON p.id = o.product_id;
来源：http://vv.shtwfgs.cn

[Q42] 连接条件附加过滤
来源：http://lb.521024.cn

SELECT u.name, o.amount FROM users u
来源：http://jk.shxzskj.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://eb.yuexingan06.cn

[Q43] 标量子查询
来源：http://bc.yuexingan06.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://bu.hahajie.cn

[Q44] IN 子查询
来源：http://qq.yuexingan06.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://cx.9csxet.cn

[Q45] EXISTS 判断存在
来源：http://cz.shxzukj.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://et.panjiajie.cn

[Q46] NOT EXISTS 判断不存在
来源：http://hj.bjjhwx.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ne.shxzukj.cn

[Q47] 与平均值比较
来源：http://ys.bookmarksfly.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://vj.shxzskj.cn

[Q48] CTE 公用表表达式
来源：http://oj.hnjuh.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://bv.hnjuh.cn

SELECT * FROM t WHERE c > 5;
来源：http://hr.asd995.cn

[Q49] 更新单行
来源：http://dw.hahajie.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://at.521024.cn

[Q50] 批量更新
来源：http://wf.szsharing.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://tq.nszjky.cn

[Q51] 用子查询更新
来源：http://id.huixinmuqiang.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://dz.newstarts.cn

[Q52] 删除指定行
来源：http://hr.huixiangedu.cn

DELETE FROM users WHERE id = 10;
来源：http://jh.wgjwhj.cn

[Q53] 按条件删除
来源：http://tl.newstarts.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://gg.jctech888.com.cn

[Q54] 清空表
来源：http://jz.panjiajie.cn

TRUNCATE TABLE logs;
来源：http://im.shxzskj.cn

[Q55] 排名（并列占位）
来源：http://db.huixiangedu.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ks.hnjuh.cn

[Q56] 密集排名（并列不占位）
来源：http://ns.nicolike.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hp.wgjwhj.cn

[Q57] 行号
来源：http://ol.bjjhwx.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://zk.gzmigu.cn

[Q58] 累计求和
来源：http://zo.jianghongdianzi.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ze.521024.cn

[Q59] 分组内累计
来源：http://vj.bjjhwx.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://dt.colortex.cn

[Q60] 取上一行 / 下一行
来源：http://fy.shtwfgs.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://kx.gzmigu.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://bd.yuexingan06.cn

[Q61] 移动平均
来源：http://fm.colortex.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://fm.shxzukj.cn

[Q62] 分组占比
来源：http://ix.521024.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ba.panjiajie.cn

[Q63] 开启事务
来源：http://bx.shxzskj.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://be.newstarts.cn

[Q64] 提交事务
来源：http://jc.panjiajie.cn

COMMIT;
来源：http://tt.haigaiapp.cn

[Q65] 回滚事务
来源：http://kb.hahajie.cn

ROLLBACK;
来源：http://ml.yuntaijiaju.cn

[Q66] 行锁查询
来源：http://td.wgjwhj.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://zj.yuntaijiaju.cn

[Q67] 设置隔离级别
来源：http://yk.bjjhwx.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://th.huixiangedu.cn

[Q68] 保存点
来源：http://oc.shtwfgs.cn

SAVEPOINT sp1;
来源：http://mo.colortex.cn

ROLLBACK TO sp1;
来源：http://wr.huixinmuqiang.cn

[Q69] 查看执行计划
来源：http://yn.hnjuh.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://kh.gzmigu.cn

[Q70] 更新统计信息
来源：http://qm.szxytkj.cn

ANALYZE TABLE users;
来源：http://io.hahajie.cn

[Q71] 查看建表语句
来源：http://oq.wgjwhj.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://xa.bookmarksfly.cn

[Q72] 查看索引
来源：http://wu.szsharing.cn

SHOW INDEX FROM users;
来源：http://dr.9csxet.cn

[Q73] 查看表状态
来源：http://dh.yuntaijiaju.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://qz.huixinmuqiang.cn

[Q74] 强制使用索引
来源：http://ge.huixinmuqiang.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://rs.hnjuh.cn

[Q75] 日期格式化
来源：http://ym.shxzukj.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://qs.szxytkj.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://rc.nszjky.cn

[Q76] 按天统计
来源：http://vs.chemitech.net.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://po.yuntaijiaju.cn

[Q77] 时间加减
来源：http://du.asd995.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://gt.jctech888.com.cn

[Q78] 当前时间
来源：http://ni.jianghongdianzi.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://kt.nicolike.cn

[Q79] 字符串拼接
来源：http://sg.asd995.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://nv.shxzskj.cn

[Q80] 字符串截取
来源：http://ag.nicolike.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://om.szsharing.cn

[Q81] 字符串替换
来源：http://vm.hahajie.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://kj.bjjhwx.cn

[Q82] 字符长度与字节长度
来源：http://bo.bookmarksfly.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://qb.newstarts.cn

[Q83] 大小写转换
来源：http://cq.hahajie.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ga.wgjwhj.cn

[Q84] 去除首尾空格
来源：http://sw.panjiajie.cn

SELECT TRIM(name) FROM users;
来源：http://gf.nicolike.cn

[Q85] 数值取整
来源：http://go.huanxung.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://xi.bookmarksfly.cn

[Q86] 读取 JSON 字段
来源：http://yp.hahajie.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://yq.shxzukj.cn

[Q87] JSON 字段做条件
来源：http://xe.jctech888.com.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://nu.szxytkj.cn

[Q88] 行转列（条件聚合）
来源：http://gv.jctech888.com.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://aa.521024.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://sq.nicolike.cn

[Q89] 判断表是否存在
来源：http://jj.jianghongdianzi.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://kt.hnjuh.cn

[Q90] 生成序号列
来源：http://re.haigaiapp.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://yu.jctech888.com.cn

================================================================================
来源：http://cv.shxzskj.cn

R. Bash 专题
来源：http://af.bjjhwx.cn

================================================================================
来源：http://pu.nicolike.cn

[R01] shebang 与严格模式
来源：http://tp.521024.cn

#!/usr/bin/env bash
来源：http://tb.jctech888.com.cn

set -euo pipefail
来源：http://az.shxzukj.cn

[R02] 变量赋值与使用
来源：http://mp.huanxung.cn

name="Tom"; echo "$name"
来源：http://vq.szxytkj.cn

[R03] 只读变量
来源：http://hw.huixiangedu.cn

readonly PI=3.14
来源：http://jh.jianghongdianzi.cn

[R04] 位置参数
来源：http://pj.muxihuayi.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://cz.bookmarksfly.cn

[R05] 参数默认值
来源：http://ss.huixinmuqiang.cn

name="${1:-default}"
来源：http://ay.yuexingan06.cn

[R06] 判断命令是否存在
来源：http://uy.jianghongdianzi.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ky.jianghongdianzi.cn

[R07] if 判断文件
来源：http://bl.huixinmuqiang.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://dm.jctech888.com.cn

[R08] 数值比较
来源：http://bn.newstarts.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://da.shxzukj.cn

[R09] 字符串比较
来源：http://xw.hnjuh.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://nd.gzmigu.cn

[R10] 正则匹配
来源：http://cn.hahajie.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://pw.521024.cn

[R11] case 多分支
来源：http://bd.asd995.cn

case "$1" in
来源：http://dt.521024.cn

start) echo "启动" ;;
来源：http://yd.shxzukj.cn

stop)  echo "停止" ;;
来源：http://sh.shxzskj.cn

*)     echo "未知命令" ;;
来源：http://aj.shtwfgs.cn

esac
来源：http://vz.hnjuh.cn

[R12] for 遍历文件
来源：http://po.muxihuayi.cn

for f in *.txt; do echo "$f"; done
来源：http://on.nszjky.cn

[R13] for 计数循环
来源：http://wp.szsharing.cn

for i in {1..10}; do echo "$i"; done
来源：http://ef.haigaiapp.cn

[R14] C 风格 for
来源：http://yf.wgjwhj.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hx.hnjuh.cn

[R15] while 逐行读文件
来源：http://hq.huixinmuqiang.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://bk.panjiajie.cn

[R16] until 等待条件
来源：http://rl.shxzukj.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://xs.haigaiapp.cn

[R17] 数组定义与取值
来源：http://ak.nicolike.cn


<!-- 参考信息 -->