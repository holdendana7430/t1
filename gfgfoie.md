代发 wailian999

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ls.muxihuayi.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://aq.jctech888.com.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://gu.nszjky.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://uz.9csxet.cn

Java: list.size();  map.size();  s.length()
来源：http://bm.shtwfgs.cn

Go:   len(arr);  len(m)
来源：http://fz.shxzukj.cn

Ruby: x.length;  x.size
来源：http://so.hnjuh.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://sg.lnxyls.cn

[P05] 判断两个对象内容是否相等
来源：http://fi.shxzukj.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://oy.newstarts.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://zu.hahajie.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://gt.wgjwhj.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://di.asd995.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ip.shtwfgs.cn

Go:   reflect.DeepEqual(a, b)
来源：http://pi.jianghongdianzi.cn

Ruby: a == b
来源：http://xc.panjiajie.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://eq.newstarts.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://rp.shtwfgs.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://zy.9csxet.cn

PHP:  if (empty($x)) {}
来源：http://tu.gzmigu.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mv.haigaiapp.cn

TS:   if (x == null) {}
来源：http://jd.wgjwhj.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://pw.huixiangedu.cn

Go:   if x == nil {}
来源：http://ov.haigaiapp.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://fj.shxzskj.cn

C#:   if (x is null) {}
来源：http://tf.yuexingan06.cn

[P07] 防抖与节流
来源：http://om.yuexingan06.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://sb.huixinmuqiang.cn

PHP:  // 手写时间戳比较
来源：http://gg.nszjky.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://zj.chemitech.net.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qk.lnxyls.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://cp.jctech888.com.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://pr.shxzskj.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://kf.9csxet.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wm.jianghongdianzi.cn

[P08] 处理浮点精度问题
来源：http://xf.521024.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hr.yuntaijiaju.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ku.jianghongdianzi.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://tc.yuexingan06.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://vy.huixinmuqiang.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://lu.gzmigu.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://eu.chemitech.net.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://lp.szsharing.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://md.jianghongdianzi.cn

================================================================================
来源：http://ny.haigaiapp.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://bo.szxytkj.cn

================================================================================
来源：http://jm.wgjwhj.cn

[Q01] 创建表
来源：http://ml.szsharing.cn

CREATE TABLE users (
来源：http://rd.yuntaijiaju.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://fh.gzmigu.cn

name VARCHAR(50) NOT NULL,
来源：http://ky.lnxyls.cn

email VARCHAR(100) UNIQUE,
来源：http://ov.newstarts.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://eg.chemitech.net.cn

);
来源：http://xr.szsharing.cn

[Q02] 创建带外键的表
来源：http://si.jianghongdianzi.cn

CREATE TABLE orders (
来源：http://pt.huixinmuqiang.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ib.gzmigu.cn

user_id INT NOT NULL,
来源：http://vp.muxihuayi.cn

amount DECIMAL(10, 2),
来源：http://vd.huanxung.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://tp.newstarts.cn

);
来源：http://eq.newstarts.cn

[Q03] 增加列
来源：http://od.hnjuh.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://nz.gzmigu.cn

[Q04] 修改列类型
来源：http://cv.nicolike.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://rn.nszjky.cn

[Q05] 重命名列
来源：http://yx.9csxet.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://cg.9csxet.cn

[Q06] 删除列
来源：http://my.asd995.cn

ALTER TABLE users DROP COLUMN age;
来源：http://ix.huixinmuqiang.cn

[Q07] 删除表
来源：http://yp.hahajie.cn

DROP TABLE IF EXISTS orders;
来源：http://ct.hnjuh.cn

[Q08] 创建普通索引
来源：http://pk.haigaiapp.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://fb.newstarts.cn

[Q09] 创建唯一索引
来源：http://lt.lnxyls.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://cg.shxzskj.cn

[Q10] 插入单行
来源：http://um.wgjwhj.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ly.bookmarksfly.cn

[Q11] 一次插入多行
来源：http://lh.9csxet.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://vu.szsharing.cn

[Q12] 插入后取自增 ID
来源：http://fh.shtwfgs.cn

INSERT INTO users (name) VALUES ('C');
来源：http://zj.colortex.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ux.jianghongdianzi.cn

[Q13] 忽略重复插入
来源：http://wp.colortex.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://qv.521024.cn

[Q14] 存在则更新（upsert）
来源：http://ig.newstarts.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://kw.521024.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ak.hnjuh.cn

[Q15] 查询全部
来源：http://zb.lnxyls.cn

SELECT * FROM users;
来源：http://hr.shtwfgs.cn

[Q16] 查询指定列
来源：http://mk.nszjky.cn

SELECT id, name FROM users;
来源：http://ob.shtwfgs.cn

[Q17] 条件查询
来源：http://vu.shtwfgs.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://it.haigaiapp.cn

[Q18] 模糊匹配
来源：http://up.shxzskj.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://na.muxihuayi.cn

[Q19] 范围查询
来源：http://al.yuexingan06.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://lo.asd995.cn

[Q20] IN 列表
来源：http://cu.wgjwhj.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ub.gzmigu.cn

[Q21] 空值判断
来源：http://sv.521024.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://zd.asd995.cn

[Q22] 排序
来源：http://lz.gzmigu.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mj.jctech888.com.cn

[Q23] 分页
来源：http://sr.hnjuh.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://yd.yuntaijiaju.cn

[Q24] 去重
来源：http://ir.muxihuayi.cn

SELECT DISTINCT city FROM users;
来源：http://da.hahajie.cn

[Q25] 只取前 N 条
来源：http://jg.jctech888.com.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://gh.hnjuh.cn

[Q26] 计数
来源：http://ss.newstarts.cn

SELECT COUNT(*) FROM users;
来源：http://pi.asd995.cn

[Q27] 条件计数
来源：http://jy.nicolike.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://iy.szxytkj.cn

[Q28] 求和与平均
来源：http://eb.521024.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://rg.szsharing.cn

[Q29] 最大最小值
来源：http://hx.haigaiapp.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://fb.hnjuh.cn

[Q30] 分组统计
来源：http://gl.asd995.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://dd.chemitech.net.cn

[Q31] 分组后过滤
来源：http://qb.hnjuh.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://jy.9csxet.cn

[Q32] 分组拼接字符串
来源：http://gv.bookmarksfly.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://py.shxzskj.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://td.chemitech.net.cn

[Q33] 多列分组
来源：http://gi.chemitech.net.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ba.haigaiapp.cn

[Q34] 每组取第一条
来源：http://wg.521024.cn

SELECT * FROM (
来源：http://ss.shxzukj.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ay.szxytkj.cn

) t WHERE rn = 1;
来源：http://tl.yuexingan06.cn

[Q35] 内连接
来源：http://ud.shxzskj.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://dp.colortex.cn

[Q36] 左连接
来源：http://uj.jctech888.com.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://tz.huixinmuqiang.cn

[Q37] 右连接
来源：http://zy.haigaiapp.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://jg.hnjuh.cn

[Q38] 全外连接（PostgreSQL）
来源：http://mg.hnjuh.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mu.nicolike.cn

[Q39] 自连接（查上下级）
来源：http://gm.nszjky.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://zq.colortex.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mh.huanxung.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://wg.shxzskj.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://pf.9csxet.cn

[Q41] 多表连接
来源：http://gb.gzmigu.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://ya.lnxyls.cn

JOIN users u ON u.id = o.user_id
来源：http://qw.colortex.cn

JOIN products p ON p.id = o.product_id;
来源：http://vy.9csxet.cn

[Q42] 连接条件附加过滤
来源：http://cn.hnjuh.cn

SELECT u.name, o.amount FROM users u
来源：http://lm.bjjhwx.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://cv.chemitech.net.cn

[Q43] 标量子查询
来源：http://ml.yuexingan06.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ua.huixiangedu.cn

[Q44] IN 子查询
来源：http://vt.huixinmuqiang.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://dn.asd995.cn

[Q45] EXISTS 判断存在
来源：http://mn.colortex.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://rr.muxihuayi.cn

[Q46] NOT EXISTS 判断不存在
来源：http://mo.521024.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hd.yuexingan06.cn

[Q47] 与平均值比较
来源：http://vd.colortex.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://dc.521024.cn

[Q48] CTE 公用表表达式
来源：http://ot.huanxung.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://qf.newstarts.cn

SELECT * FROM t WHERE c > 5;
来源：http://ye.chemitech.net.cn

[Q49] 更新单行
来源：http://dr.jianghongdianzi.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://sw.gzmigu.cn

[Q50] 批量更新
来源：http://zl.newstarts.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://gc.shxzukj.cn

[Q51] 用子查询更新
来源：http://na.huixinmuqiang.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://ki.huixiangedu.cn

[Q52] 删除指定行
来源：http://kg.huixiangedu.cn

DELETE FROM users WHERE id = 10;
来源：http://xr.lnxyls.cn

[Q53] 按条件删除
来源：http://zp.huanxung.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://fb.huanxung.cn

[Q54] 清空表
来源：http://ga.jctech888.com.cn

TRUNCATE TABLE logs;
来源：http://vy.shtwfgs.cn

[Q55] 排名（并列占位）
来源：http://cv.huixinmuqiang.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hj.huixinmuqiang.cn

[Q56] 密集排名（并列不占位）
来源：http://ip.shxzukj.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ck.yuexingan06.cn

[Q57] 行号
来源：http://zj.huixinmuqiang.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://to.bjjhwx.cn

[Q58] 累计求和
来源：http://pq.yuntaijiaju.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://iy.muxihuayi.cn

[Q59] 分组内累计
来源：http://ma.shxzskj.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://sa.hnjuh.cn

[Q60] 取上一行 / 下一行
来源：http://ga.yuexingan06.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://bz.521024.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://db.521024.cn

[Q61] 移动平均
来源：http://hk.nicolike.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://qh.colortex.cn

[Q62] 分组占比
来源：http://wc.huixinmuqiang.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mp.bookmarksfly.cn

[Q63] 开启事务
来源：http://ek.huanxung.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://lp.521024.cn

[Q64] 提交事务
来源：http://pj.asd995.cn

COMMIT;
来源：http://fr.shxzskj.cn

[Q65] 回滚事务
来源：http://yo.jianghongdianzi.cn

ROLLBACK;
来源：http://yc.panjiajie.cn

[Q66] 行锁查询
来源：http://cw.shxzukj.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wt.huanxung.cn

[Q67] 设置隔离级别
来源：http://wl.hnjuh.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://pt.hahajie.cn

[Q68] 保存点
来源：http://ui.9csxet.cn

SAVEPOINT sp1;
来源：http://nz.hnjuh.cn

ROLLBACK TO sp1;
来源：http://em.bjjhwx.cn

[Q69] 查看执行计划
来源：http://tm.shxzukj.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://xe.yuexingan06.cn

[Q70] 更新统计信息
来源：http://rw.huixiangedu.cn

ANALYZE TABLE users;
来源：http://uy.hahajie.cn

[Q71] 查看建表语句
来源：http://pm.yuntaijiaju.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://dl.gzmigu.cn

[Q72] 查看索引
来源：http://wo.yuntaijiaju.cn

SHOW INDEX FROM users;
来源：http://oj.hahajie.cn

[Q73] 查看表状态
来源：http://rf.shxzskj.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://fo.hnjuh.cn

[Q74] 强制使用索引
来源：http://dl.bjjhwx.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://gi.shtwfgs.cn

[Q75] 日期格式化
来源：http://ff.nicolike.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://qe.szxytkj.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://nl.szxytkj.cn

[Q76] 按天统计
来源：http://mi.bjjhwx.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://cy.shxzukj.cn

[Q77] 时间加减
来源：http://ov.huixinmuqiang.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://aw.szxytkj.cn

[Q78] 当前时间
来源：http://rv.haigaiapp.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://pp.huanxung.cn

[Q79] 字符串拼接
来源：http://kg.hnjuh.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://tj.shtwfgs.cn

[Q80] 字符串截取
来源：http://ew.huixiangedu.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://aa.9csxet.cn

[Q81] 字符串替换
来源：http://ez.hahajie.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://fu.hnjuh.cn

[Q82] 字符长度与字节长度
来源：http://ro.yuntaijiaju.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://xu.colortex.cn

[Q83] 大小写转换
来源：http://ja.hnjuh.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://vj.nicolike.cn

[Q84] 去除首尾空格
来源：http://gk.yuexingan06.cn

SELECT TRIM(name) FROM users;
来源：http://ph.colortex.cn

[Q85] 数值取整
来源：http://eo.jctech888.com.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://bd.gzmigu.cn

[Q86] 读取 JSON 字段
来源：http://hm.asd995.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://cu.shtwfgs.cn

[Q87] JSON 字段做条件
来源：http://hk.shxzukj.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://nk.bjjhwx.cn

[Q88] 行转列（条件聚合）
来源：http://hv.szxytkj.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://xo.colortex.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://qi.asd995.cn

[Q89] 判断表是否存在
来源：http://wk.hahajie.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://jf.shxzskj.cn

[Q90] 生成序号列
来源：http://fj.muxihuayi.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ln.lnxyls.cn

================================================================================
来源：http://hd.shxzukj.cn

R. Bash 专题
来源：http://fx.nszjky.cn

================================================================================
来源：http://jl.huixiangedu.cn

[R01] shebang 与严格模式
来源：http://kd.muxihuayi.cn

#!/usr/bin/env bash
来源：http://dr.szsharing.cn

set -euo pipefail
来源：http://os.bjjhwx.cn

[R02] 变量赋值与使用
来源：http://dg.hnjuh.cn

name="Tom"; echo "$name"
来源：http://lm.shxzukj.cn

[R03] 只读变量
来源：http://ou.jianghongdianzi.cn

readonly PI=3.14
来源：http://jb.hahajie.cn

[R04] 位置参数
来源：http://rz.huanxung.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ql.jianghongdianzi.cn

[R05] 参数默认值
来源：http://je.huixinmuqiang.cn

name="${1:-default}"
来源：http://in.chemitech.net.cn

[R06] 判断命令是否存在
来源：http://kz.nicolike.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://cd.newstarts.cn

[R07] if 判断文件
来源：http://zq.jianghongdianzi.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://eo.muxihuayi.cn

[R08] 数值比较
来源：http://lj.bookmarksfly.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://jl.jianghongdianzi.cn

[R09] 字符串比较
来源：http://nw.newstarts.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ar.jianghongdianzi.cn

[R10] 正则匹配
来源：http://lj.lnxyls.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://bt.yuexingan06.cn

[R11] case 多分支
来源：http://fj.shxzskj.cn

case "$1" in
来源：http://uz.nicolike.cn

start) echo "启动" ;;
来源：http://ar.yuexingan06.cn

stop)  echo "停止" ;;
来源：http://uk.nszjky.cn

*)     echo "未知命令" ;;
来源：http://ph.9csxet.cn

esac
来源：http://fj.haigaiapp.cn

[R12] for 遍历文件
来源：http://ex.jianghongdianzi.cn

for f in *.txt; do echo "$f"; done
来源：http://ym.hnjuh.cn

[R13] for 计数循环
来源：http://cb.lnxyls.cn

for i in {1..10}; do echo "$i"; done
来源：http://rw.shxzukj.cn

[R14] C 风格 for
来源：http://oo.gzmigu.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://sy.colortex.cn

[R15] while 逐行读文件
来源：http://sa.colortex.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://sa.huixinmuqiang.cn

[R16] until 等待条件
来源：http://ja.shxzskj.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mz.szsharing.cn

[R17] 数组定义与取值
来源：http://jg.szsharing.cn

arr=(a b c); echo "${arr[0]}"
来源：http://hf.asd995.cn

[R18] 遍历数组
来源：http://qm.jctech888.com.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ff.szsharing.cn

[R19] 数组长度
来源：http://bk.haigaiapp.cn

echo "${#arr[@]}"
来源：http://rf.nicolike.cn

[R20] 关联数组（字典）
来源：http://es.jianghongdianzi.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://jk.hnjuh.cn

[R21] 字符串长度
来源：http://ru.hahajie.cn


<!-- 参考信息 -->