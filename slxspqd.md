代发 wailian999

Py:   len(x)            # 字符串、列表、字典通用
来源：http://gr.muxihuayi.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://pc.panjiajie.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://gn.chemitech.net.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://tk.shtwfgs.cn

Java: list.size();  map.size();  s.length()
来源：http://ei.chemitech.net.cn

Go:   len(arr);  len(m)
来源：http://jb.gzmigu.cn

Ruby: x.length;  x.size
来源：http://en.yuntaijiaju.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://hy.huanxung.cn

[P05] 判断两个对象内容是否相等
来源：http://qf.9csxet.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://xk.nszjky.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ed.9csxet.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ad.gzmigu.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://bo.shxzskj.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ed.shxzskj.cn

Go:   reflect.DeepEqual(a, b)
来源：http://xv.shxzskj.cn

Ruby: a == b
来源：http://mj.szsharing.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://es.jctech888.com.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mu.9csxet.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://md.hnjuh.cn

PHP:  if (empty($x)) {}
来源：http://lp.panjiajie.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://dv.521024.cn

TS:   if (x == null) {}
来源：http://wg.huanxung.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://gw.lnxyls.cn

Go:   if x == nil {}
来源：http://ji.muxihuayi.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ik.haigaiapp.cn

C#:   if (x is null) {}
来源：http://bx.newstarts.cn

[P07] 防抖与节流
来源：http://sx.haigaiapp.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://md.huixiangedu.cn

PHP:  // 手写时间戳比较
来源：http://xc.huanxung.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://zw.szsharing.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://fq.colortex.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://yb.shxzukj.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://va.szsharing.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://ky.huixiangedu.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ag.bookmarksfly.cn

[P08] 处理浮点精度问题
来源：http://oy.bjjhwx.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://pb.muxihuayi.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://uk.asd995.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://lu.hahajie.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://pw.shxzskj.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://xn.huanxung.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ov.shxzskj.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://lj.huixinmuqiang.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://cc.szsharing.cn

================================================================================
来源：http://fg.shxzskj.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://le.huanxung.cn

================================================================================
来源：http://zl.asd995.cn

[Q01] 创建表
来源：http://sg.hnjuh.cn

CREATE TABLE users (
来源：http://pq.hnjuh.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://qc.shxzukj.cn

name VARCHAR(50) NOT NULL,
来源：http://mx.chemitech.net.cn

email VARCHAR(100) UNIQUE,
来源：http://dq.shtwfgs.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://xx.huixiangedu.cn

);
来源：http://sn.panjiajie.cn

[Q02] 创建带外键的表
来源：http://ti.521024.cn

CREATE TABLE orders (
来源：http://qd.nszjky.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://he.asd995.cn

user_id INT NOT NULL,
来源：http://tc.bookmarksfly.cn

amount DECIMAL(10, 2),
来源：http://xz.9csxet.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://zq.shtwfgs.cn

);
来源：http://jv.hahajie.cn

[Q03] 增加列
来源：http://zd.huanxung.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://gn.szxytkj.cn

[Q04] 修改列类型
来源：http://xy.hnjuh.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://al.lnxyls.cn

[Q05] 重命名列
来源：http://wy.hahajie.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hc.wgjwhj.cn

[Q06] 删除列
来源：http://kt.hnjuh.cn

ALTER TABLE users DROP COLUMN age;
来源：http://ty.hahajie.cn

[Q07] 删除表
来源：http://ry.nszjky.cn

DROP TABLE IF EXISTS orders;
来源：http://fk.shtwfgs.cn

[Q08] 创建普通索引
来源：http://hs.hnjuh.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://wx.gzmigu.cn

[Q09] 创建唯一索引
来源：http://dg.haigaiapp.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://bj.yuntaijiaju.cn

[Q10] 插入单行
来源：http://qx.huixiangedu.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ay.nicolike.cn

[Q11] 一次插入多行
来源：http://kp.nszjky.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://gt.shxzukj.cn

[Q12] 插入后取自增 ID
来源：http://hn.jctech888.com.cn

INSERT INTO users (name) VALUES ('C');
来源：http://vq.yuntaijiaju.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://cg.szsharing.cn

[Q13] 忽略重复插入
来源：http://jj.hnjuh.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wi.bjjhwx.cn

[Q14] 存在则更新（upsert）
来源：http://ib.szxytkj.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ij.huanxung.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://vo.yuntaijiaju.cn

[Q15] 查询全部
来源：http://mr.asd995.cn

SELECT * FROM users;
来源：http://ik.shxzskj.cn

[Q16] 查询指定列
来源：http://bw.panjiajie.cn

SELECT id, name FROM users;
来源：http://gp.yuexingan06.cn

[Q17] 条件查询
来源：http://ap.jctech888.com.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://xm.asd995.cn

[Q18] 模糊匹配
来源：http://ft.szxytkj.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://sq.hnjuh.cn

[Q19] 范围查询
来源：http://ux.shxzskj.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://kj.szxytkj.cn

[Q20] IN 列表
来源：http://dn.shtwfgs.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://az.szsharing.cn

[Q21] 空值判断
来源：http://cr.chemitech.net.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://sd.bookmarksfly.cn

[Q22] 排序
来源：http://nu.nicolike.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://dy.colortex.cn

[Q23] 分页
来源：http://xp.huanxung.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://kg.huixinmuqiang.cn

[Q24] 去重
来源：http://es.shxzskj.cn

SELECT DISTINCT city FROM users;
来源：http://gm.yuexingan06.cn

[Q25] 只取前 N 条
来源：http://sl.yuntaijiaju.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://lt.yuexingan06.cn

[Q26] 计数
来源：http://ux.bookmarksfly.cn

SELECT COUNT(*) FROM users;
来源：http://ud.9csxet.cn

[Q27] 条件计数
来源：http://cq.jianghongdianzi.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://oo.wgjwhj.cn

[Q28] 求和与平均
来源：http://lk.chemitech.net.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://os.lnxyls.cn

[Q29] 最大最小值
来源：http://dc.huanxung.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://iy.gzmigu.cn

[Q30] 分组统计
来源：http://dh.huanxung.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://qr.panjiajie.cn

[Q31] 分组后过滤
来源：http://px.huixinmuqiang.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://vy.jianghongdianzi.cn

[Q32] 分组拼接字符串
来源：http://mt.huixinmuqiang.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ul.haigaiapp.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://gr.nszjky.cn

[Q33] 多列分组
来源：http://pj.huixiangedu.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://nq.chemitech.net.cn

[Q34] 每组取第一条
来源：http://ol.jianghongdianzi.cn

SELECT * FROM (
来源：http://dw.bookmarksfly.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://dx.nszjky.cn

) t WHERE rn = 1;
来源：http://qy.gzmigu.cn

[Q35] 内连接
来源：http://ta.haigaiapp.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://bd.lnxyls.cn

[Q36] 左连接
来源：http://th.huixiangedu.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://nw.lnxyls.cn

[Q37] 右连接
来源：http://ni.nszjky.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://aj.yuexingan06.cn

[Q38] 全外连接（PostgreSQL）
来源：http://to.hnjuh.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://na.szsharing.cn

[Q39] 自连接（查上下级）
来源：http://wh.521024.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://vw.521024.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://vv.shtwfgs.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://ki.yuntaijiaju.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://jk.szxytkj.cn

[Q41] 多表连接
来源：http://rg.bookmarksfly.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://eu.wgjwhj.cn

JOIN users u ON u.id = o.user_id
来源：http://xe.wgjwhj.cn

JOIN products p ON p.id = o.product_id;
来源：http://rh.shxzukj.cn

[Q42] 连接条件附加过滤
来源：http://ie.lnxyls.cn

SELECT u.name, o.amount FROM users u
来源：http://uz.hahajie.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://dw.bjjhwx.cn

[Q43] 标量子查询
来源：http://wt.wgjwhj.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://fy.yuexingan06.cn

[Q44] IN 子查询
来源：http://rn.haigaiapp.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://nl.bookmarksfly.cn

[Q45] EXISTS 判断存在
来源：http://kd.hnjuh.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ld.jianghongdianzi.cn

[Q46] NOT EXISTS 判断不存在
来源：http://iy.9csxet.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://je.shxzukj.cn

[Q47] 与平均值比较
来源：http://ws.shtwfgs.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mw.bjjhwx.cn

[Q48] CTE 公用表表达式
来源：http://rh.colortex.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://pr.shtwfgs.cn

SELECT * FROM t WHERE c > 5;
来源：http://aw.huixiangedu.cn

[Q49] 更新单行
来源：http://wu.asd995.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://qw.panjiajie.cn

[Q50] 批量更新
来源：http://vl.nicolike.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://yy.lnxyls.cn

[Q51] 用子查询更新
来源：http://lf.szxytkj.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://zg.hnjuh.cn

[Q52] 删除指定行
来源：http://ls.bjjhwx.cn

DELETE FROM users WHERE id = 10;
来源：http://yk.hahajie.cn

[Q53] 按条件删除
来源：http://cp.jianghongdianzi.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ls.yuntaijiaju.cn

[Q54] 清空表
来源：http://uc.huixiangedu.cn

TRUNCATE TABLE logs;
来源：http://ze.yuntaijiaju.cn

[Q55] 排名（并列占位）
来源：http://hr.panjiajie.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://jh.panjiajie.cn

[Q56] 密集排名（并列不占位）
来源：http://in.gzmigu.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://zl.9csxet.cn

[Q57] 行号
来源：http://gr.9csxet.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://uv.hnjuh.cn

[Q58] 累计求和
来源：http://us.shxzukj.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://yx.szsharing.cn

[Q59] 分组内累计
来源：http://oj.gzmigu.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://my.colortex.cn

[Q60] 取上一行 / 下一行
来源：http://ej.asd995.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://em.nicolike.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ch.chemitech.net.cn

[Q61] 移动平均
来源：http://ub.asd995.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://qq.huanxung.cn

[Q62] 分组占比
来源：http://fv.nicolike.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://vl.yuexingan06.cn

[Q63] 开启事务
来源：http://yq.nicolike.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://xe.wgjwhj.cn

[Q64] 提交事务
来源：http://ef.9csxet.cn

COMMIT;
来源：http://fh.jctech888.com.cn

[Q65] 回滚事务
来源：http://fi.yuntaijiaju.cn

ROLLBACK;
来源：http://ya.lnxyls.cn

[Q66] 行锁查询
来源：http://nv.szsharing.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://bk.shxzskj.cn

[Q67] 设置隔离级别
来源：http://ck.yuntaijiaju.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://kq.yuntaijiaju.cn

[Q68] 保存点
来源：http://of.chemitech.net.cn

SAVEPOINT sp1;
来源：http://ay.bjjhwx.cn

ROLLBACK TO sp1;
来源：http://oz.bookmarksfly.cn

[Q69] 查看执行计划
来源：http://ag.521024.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ep.shxzskj.cn

[Q70] 更新统计信息
来源：http://gg.muxihuayi.cn

ANALYZE TABLE users;
来源：http://di.9csxet.cn

[Q71] 查看建表语句
来源：http://km.hnjuh.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://kw.jianghongdianzi.cn

[Q72] 查看索引
来源：http://hn.colortex.cn

SHOW INDEX FROM users;
来源：http://bg.nszjky.cn

[Q73] 查看表状态
来源：http://zq.nicolike.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://ld.szsharing.cn

[Q74] 强制使用索引
来源：http://kp.jctech888.com.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://sp.huanxung.cn

[Q75] 日期格式化
来源：http://lg.hnjuh.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://pb.yuexingan06.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://bb.shtwfgs.cn

[Q76] 按天统计
来源：http://ld.asd995.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://sp.szsharing.cn

[Q77] 时间加减
来源：http://fk.yuntaijiaju.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://al.521024.cn

[Q78] 当前时间
来源：http://us.jctech888.com.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://gj.newstarts.cn

[Q79] 字符串拼接
来源：http://sz.bookmarksfly.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ws.jianghongdianzi.cn

[Q80] 字符串截取
来源：http://ml.wgjwhj.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://er.shtwfgs.cn

[Q81] 字符串替换
来源：http://et.gzmigu.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://at.shxzskj.cn

[Q82] 字符长度与字节长度
来源：http://he.shtwfgs.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://fv.huixiangedu.cn

[Q83] 大小写转换
来源：http://ln.panjiajie.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://bn.shxzskj.cn

[Q84] 去除首尾空格
来源：http://dl.yuexingan06.cn

SELECT TRIM(name) FROM users;
来源：http://sk.shtwfgs.cn

[Q85] 数值取整
来源：http://oi.gzmigu.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ji.bookmarksfly.cn

[Q86] 读取 JSON 字段
来源：http://xw.huixinmuqiang.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://zt.nicolike.cn

[Q87] JSON 字段做条件
来源：http://os.newstarts.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://jk.nicolike.cn

[Q88] 行转列（条件聚合）
来源：http://ws.szxytkj.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://aa.nicolike.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://fx.asd995.cn

[Q89] 判断表是否存在
来源：http://xs.panjiajie.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://at.shtwfgs.cn

[Q90] 生成序号列
来源：http://rw.newstarts.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://do.521024.cn

================================================================================
来源：http://lp.nicolike.cn

R. Bash 专题
来源：http://ln.nszjky.cn

================================================================================
来源：http://qg.hnjuh.cn

[R01] shebang 与严格模式
来源：http://dc.haigaiapp.cn

#!/usr/bin/env bash
来源：http://my.nicolike.cn

set -euo pipefail
来源：http://nv.huanxung.cn

[R02] 变量赋值与使用
来源：http://bc.shtwfgs.cn

name="Tom"; echo "$name"
来源：http://iq.jianghongdianzi.cn

[R03] 只读变量
来源：http://hn.hahajie.cn

readonly PI=3.14
来源：http://xg.colortex.cn

[R04] 位置参数
来源：http://ly.huanxung.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://av.bjjhwx.cn

[R05] 参数默认值
来源：http://ni.panjiajie.cn

name="${1:-default}"
来源：http://lo.shtwfgs.cn

[R06] 判断命令是否存在
来源：http://lo.shtwfgs.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hu.nszjky.cn

[R07] if 判断文件
来源：http://ov.asd995.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://xk.shtwfgs.cn

[R08] 数值比较
来源：http://bo.huixiangedu.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://zw.jianghongdianzi.cn

[R09] 字符串比较
来源：http://eh.panjiajie.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ef.jianghongdianzi.cn

[R10] 正则匹配
来源：http://dm.colortex.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://es.jctech888.com.cn

[R11] case 多分支
来源：http://vv.jianghongdianzi.cn

case "$1" in
来源：http://ws.nicolike.cn

start) echo "启动" ;;
来源：http://ja.haigaiapp.cn

stop)  echo "停止" ;;
来源：http://tz.szxytkj.cn

*)     echo "未知命令" ;;
来源：http://ug.wgjwhj.cn

esac
来源：http://pp.panjiajie.cn

[R12] for 遍历文件
来源：http://ol.huixiangedu.cn

for f in *.txt; do echo "$f"; done
来源：http://ts.jctech888.com.cn

[R13] for 计数循环
来源：http://vc.bookmarksfly.cn

for i in {1..10}; do echo "$i"; done
来源：http://um.shxzukj.cn

[R14] C 风格 for
来源：http://mu.nszjky.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://te.yuntaijiaju.cn

[R15] while 逐行读文件
来源：http://ms.huixinmuqiang.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://pw.nicolike.cn

[R16] until 等待条件
来源：http://bg.szxytkj.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://dn.hnjuh.cn

[R17] 数组定义与取值
来源：http://ij.hnjuh.cn

arr=(a b c); echo "${arr[0]}"
来源：http://rp.nszjky.cn

[R18] 遍历数组
来源：http://mo.asd995.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wk.szsharing.cn

[R19] 数组长度
来源：http://xu.bookmarksfly.cn

echo "${#arr[@]}"
来源：http://nf.gzmigu.cn

[R20] 关联数组（字典）
来源：http://eg.shxzukj.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ta.9csxet.cn

[R21] 字符串长度
来源：http://uy.9csxet.cn


<!-- 参考信息 -->