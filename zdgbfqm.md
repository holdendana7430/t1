代发 wailian999

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ch.wgjwhj.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://lp.bjjhwx.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://um.shxzukj.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://qp.haigaiapp.cn

Java: list.size();  map.size();  s.length()
来源：http://ch.bookmarksfly.cn

Go:   len(arr);  len(m)
来源：http://th.lnxyls.cn

Ruby: x.length;  x.size
来源：http://ej.panjiajie.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://qe.asd995.cn

[P05] 判断两个对象内容是否相等
来源：http://xb.colortex.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://nm.panjiajie.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://qm.bjjhwx.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://dt.panjiajie.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ve.shxzskj.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://lo.521024.cn

Go:   reflect.DeepEqual(a, b)
来源：http://gp.asd995.cn

Ruby: a == b
来源：http://jt.hnjuh.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://tm.shxzukj.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://pd.bookmarksfly.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://fa.panjiajie.cn

PHP:  if (empty($x)) {}
来源：http://ul.jctech888.com.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://lb.huixiangedu.cn

TS:   if (x == null) {}
来源：http://iy.gzmigu.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://gq.521024.cn

Go:   if x == nil {}
来源：http://kl.huixinmuqiang.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://sh.haigaiapp.cn

C#:   if (x is null) {}
来源：http://hd.hahajie.cn

[P07] 防抖与节流
来源：http://pj.panjiajie.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://jj.bookmarksfly.cn

PHP:  // 手写时间戳比较
来源：http://rt.asd995.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://zz.bookmarksfly.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ya.bookmarksfly.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://pu.newstarts.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://pz.9csxet.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://mh.huanxung.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ip.huixiangedu.cn

[P08] 处理浮点精度问题
来源：http://iy.yuexingan06.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://tg.haigaiapp.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://bi.huanxung.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://cz.nicolike.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://qa.nszjky.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://qe.huixiangedu.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://it.nszjky.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://jm.shxzukj.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://vw.jctech888.com.cn

================================================================================
来源：http://ng.lnxyls.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://lp.panjiajie.cn

================================================================================
来源：http://jn.9csxet.cn

[Q01] 创建表
来源：http://sg.shtwfgs.cn

CREATE TABLE users (
来源：http://fy.panjiajie.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://nx.huixiangedu.cn

name VARCHAR(50) NOT NULL,
来源：http://is.newstarts.cn

email VARCHAR(100) UNIQUE,
来源：http://su.panjiajie.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://cd.shxzukj.cn

);
来源：http://kf.bookmarksfly.cn

[Q02] 创建带外键的表
来源：http://oe.hnjuh.cn

CREATE TABLE orders (
来源：http://qi.colortex.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://bc.huanxung.cn

user_id INT NOT NULL,
来源：http://cf.hahajie.cn

amount DECIMAL(10, 2),
来源：http://te.asd995.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://oq.yuntaijiaju.cn

);
来源：http://de.huanxung.cn

[Q03] 增加列
来源：http://yc.panjiajie.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://kb.colortex.cn

[Q04] 修改列类型
来源：http://my.bjjhwx.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://rv.bookmarksfly.cn

[Q05] 重命名列
来源：http://ta.muxihuayi.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ov.jianghongdianzi.cn

[Q06] 删除列
来源：http://fe.shxzskj.cn

ALTER TABLE users DROP COLUMN age;
来源：http://fe.chemitech.net.cn

[Q07] 删除表
来源：http://ya.9csxet.cn

DROP TABLE IF EXISTS orders;
来源：http://ao.huanxung.cn

[Q08] 创建普通索引
来源：http://km.shxzukj.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://zy.lnxyls.cn

[Q09] 创建唯一索引
来源：http://fa.jctech888.com.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://vl.newstarts.cn

[Q10] 插入单行
来源：http://lx.hnjuh.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ux.jianghongdianzi.cn

[Q11] 一次插入多行
来源：http://yv.haigaiapp.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ap.gzmigu.cn

[Q12] 插入后取自增 ID
来源：http://je.521024.cn

INSERT INTO users (name) VALUES ('C');
来源：http://eb.hahajie.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://zp.asd995.cn

[Q13] 忽略重复插入
来源：http://sk.panjiajie.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hg.haigaiapp.cn

[Q14] 存在则更新（upsert）
来源：http://ss.huixiangedu.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://bc.huixinmuqiang.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mi.colortex.cn

[Q15] 查询全部
来源：http://fd.chemitech.net.cn

SELECT * FROM users;
来源：http://nd.panjiajie.cn

[Q16] 查询指定列
来源：http://sv.521024.cn

SELECT id, name FROM users;
来源：http://hc.newstarts.cn

[Q17] 条件查询
来源：http://md.asd995.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://oe.jianghongdianzi.cn

[Q18] 模糊匹配
来源：http://pc.asd995.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://zg.shxzukj.cn

[Q19] 范围查询
来源：http://fc.szxytkj.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://jd.hahajie.cn

[Q20] IN 列表
来源：http://tr.muxihuayi.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://yg.haigaiapp.cn

[Q21] 空值判断
来源：http://iz.colortex.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://xw.bookmarksfly.cn

[Q22] 排序
来源：http://gb.nszjky.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://tq.521024.cn

[Q23] 分页
来源：http://hd.shtwfgs.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ad.shxzukj.cn

[Q24] 去重
来源：http://lg.lnxyls.cn

SELECT DISTINCT city FROM users;
来源：http://hz.yuntaijiaju.cn

[Q25] 只取前 N 条
来源：http://py.shxzskj.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://sc.muxihuayi.cn

[Q26] 计数
来源：http://ek.yuntaijiaju.cn

SELECT COUNT(*) FROM users;
来源：http://mk.shxzskj.cn

[Q27] 条件计数
来源：http://kt.nszjky.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://qd.bookmarksfly.cn

[Q28] 求和与平均
来源：http://vt.bookmarksfly.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://cw.bookmarksfly.cn

[Q29] 最大最小值
来源：http://fe.shtwfgs.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://ef.wgjwhj.cn

[Q30] 分组统计
来源：http://xo.wgjwhj.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://uk.nicolike.cn

[Q31] 分组后过滤
来源：http://gq.yuntaijiaju.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://sk.wgjwhj.cn

[Q32] 分组拼接字符串
来源：http://kz.shtwfgs.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://vl.asd995.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://lh.jctech888.com.cn

[Q33] 多列分组
来源：http://ih.haigaiapp.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://jf.colortex.cn

[Q34] 每组取第一条
来源：http://rn.szxytkj.cn

SELECT * FROM (
来源：http://qy.muxihuayi.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://iv.newstarts.cn

) t WHERE rn = 1;
来源：http://tm.huixinmuqiang.cn

[Q35] 内连接
来源：http://li.asd995.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://gx.521024.cn

[Q36] 左连接
来源：http://zc.shtwfgs.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://sc.yuntaijiaju.cn

[Q37] 右连接
来源：http://wa.szsharing.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://rm.panjiajie.cn

[Q38] 全外连接（PostgreSQL）
来源：http://gb.9csxet.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mr.szsharing.cn

[Q39] 自连接（查上下级）
来源：http://zi.yuntaijiaju.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://mj.nszjky.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://jl.bjjhwx.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://xw.shtwfgs.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://on.bjjhwx.cn

[Q41] 多表连接
来源：http://gk.lnxyls.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://zt.szxytkj.cn

JOIN users u ON u.id = o.user_id
来源：http://fe.huixinmuqiang.cn

JOIN products p ON p.id = o.product_id;
来源：http://tc.haigaiapp.cn

[Q42] 连接条件附加过滤
来源：http://im.jctech888.com.cn

SELECT u.name, o.amount FROM users u
来源：http://pg.hnjuh.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ec.yuexingan06.cn

[Q43] 标量子查询
来源：http://pl.jianghongdianzi.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://gn.shtwfgs.cn

[Q44] IN 子查询
来源：http://ti.yuntaijiaju.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://uj.huanxung.cn

[Q45] EXISTS 判断存在
来源：http://jf.hahajie.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://gv.shtwfgs.cn

[Q46] NOT EXISTS 判断不存在
来源：http://ft.jctech888.com.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wm.jctech888.com.cn

[Q47] 与平均值比较
来源：http://xk.wgjwhj.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://oo.9csxet.cn

[Q48] CTE 公用表表达式
来源：http://we.shtwfgs.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://am.jianghongdianzi.cn

SELECT * FROM t WHERE c > 5;
来源：http://ol.szxytkj.cn

[Q49] 更新单行
来源：http://bk.wgjwhj.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://eo.bookmarksfly.cn

[Q50] 批量更新
来源：http://gf.chemitech.net.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://ha.hnjuh.cn

[Q51] 用子查询更新
来源：http://bu.hnjuh.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://rt.nszjky.cn

[Q52] 删除指定行
来源：http://wk.wgjwhj.cn

DELETE FROM users WHERE id = 10;
来源：http://ua.szsharing.cn

[Q53] 按条件删除
来源：http://eb.521024.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ec.jctech888.com.cn

[Q54] 清空表
来源：http://tk.yuntaijiaju.cn

TRUNCATE TABLE logs;
来源：http://mr.huixinmuqiang.cn

[Q55] 排名（并列占位）
来源：http://ol.jctech888.com.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://vq.szxytkj.cn

[Q56] 密集排名（并列不占位）
来源：http://hk.shxzskj.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://vu.521024.cn

[Q57] 行号
来源：http://ar.asd995.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ux.huanxung.cn

[Q58] 累计求和
来源：http://mv.nicolike.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://cb.muxihuayi.cn

[Q59] 分组内累计
来源：http://ox.muxihuayi.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://xh.colortex.cn

[Q60] 取上一行 / 下一行
来源：http://lj.colortex.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ya.jianghongdianzi.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://nh.huixiangedu.cn

[Q61] 移动平均
来源：http://sb.szxytkj.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://uq.yuexingan06.cn

[Q62] 分组占比
来源：http://xv.yuexingan06.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://zr.yuexingan06.cn

[Q63] 开启事务
来源：http://ac.nicolike.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://mb.shtwfgs.cn

[Q64] 提交事务
来源：http://xb.hahajie.cn

COMMIT;
来源：http://at.huixiangedu.cn

[Q65] 回滚事务
来源：http://fg.huixiangedu.cn

ROLLBACK;
来源：http://fe.chemitech.net.cn

[Q66] 行锁查询
来源：http://oe.huanxung.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wf.yuexingan06.cn

[Q67] 设置隔离级别
来源：http://qy.shtwfgs.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://xc.wgjwhj.cn

[Q68] 保存点
来源：http://pk.huixinmuqiang.cn

SAVEPOINT sp1;
来源：http://po.hahajie.cn

ROLLBACK TO sp1;
来源：http://mf.nszjky.cn

[Q69] 查看执行计划
来源：http://qz.jctech888.com.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://oq.huanxung.cn

[Q70] 更新统计信息
来源：http://yf.muxihuayi.cn

ANALYZE TABLE users;
来源：http://sx.panjiajie.cn

[Q71] 查看建表语句
来源：http://nb.newstarts.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://dl.yuntaijiaju.cn

[Q72] 查看索引
来源：http://wq.bjjhwx.cn

SHOW INDEX FROM users;
来源：http://wv.newstarts.cn

[Q73] 查看表状态
来源：http://rv.asd995.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://wc.muxihuayi.cn

[Q74] 强制使用索引
来源：http://wf.hnjuh.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://rr.szsharing.cn

[Q75] 日期格式化
来源：http://de.jianghongdianzi.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://vz.szsharing.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://bg.wgjwhj.cn

[Q76] 按天统计
来源：http://kl.newstarts.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ph.hahajie.cn

[Q77] 时间加减
来源：http://bx.panjiajie.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://cg.huanxung.cn

[Q78] 当前时间
来源：http://ev.colortex.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://xs.yuexingan06.cn

[Q79] 字符串拼接
来源：http://uf.haigaiapp.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ow.chemitech.net.cn

[Q80] 字符串截取
来源：http://gw.panjiajie.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ja.bjjhwx.cn

[Q81] 字符串替换
来源：http://su.asd995.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://zh.gzmigu.cn

[Q82] 字符长度与字节长度
来源：http://ru.hnjuh.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://nz.huixinmuqiang.cn

[Q83] 大小写转换
来源：http://wn.haigaiapp.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://of.9csxet.cn

[Q84] 去除首尾空格
来源：http://gs.chemitech.net.cn

SELECT TRIM(name) FROM users;
来源：http://yb.yuntaijiaju.cn

[Q85] 数值取整
来源：http://lz.bjjhwx.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://iz.shxzskj.cn

[Q86] 读取 JSON 字段
来源：http://pz.muxihuayi.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://up.huixinmuqiang.cn

[Q87] JSON 字段做条件
来源：http://wy.lnxyls.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hl.jianghongdianzi.cn

[Q88] 行转列（条件聚合）
来源：http://xm.haigaiapp.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://lc.huanxung.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://fh.szsharing.cn

[Q89] 判断表是否存在
来源：http://fm.haigaiapp.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://cl.haigaiapp.cn

[Q90] 生成序号列
来源：http://fx.yuexingan06.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ki.9csxet.cn

================================================================================
来源：http://mc.9csxet.cn

R. Bash 专题
来源：http://nj.gzmigu.cn

================================================================================
来源：http://fs.nicolike.cn

[R01] shebang 与严格模式
来源：http://nf.haigaiapp.cn

#!/usr/bin/env bash
来源：http://kf.jctech888.com.cn

set -euo pipefail
来源：http://bw.shtwfgs.cn

[R02] 变量赋值与使用
来源：http://st.huixiangedu.cn

name="Tom"; echo "$name"
来源：http://tg.yuexingan06.cn

[R03] 只读变量
来源：http://vp.gzmigu.cn

readonly PI=3.14
来源：http://wi.chemitech.net.cn

[R04] 位置参数
来源：http://uo.shtwfgs.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ue.shtwfgs.cn

[R05] 参数默认值
来源：http://ds.yuexingan06.cn

name="${1:-default}"
来源：http://be.panjiajie.cn

[R06] 判断命令是否存在
来源：http://ck.muxihuayi.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ej.huixiangedu.cn

[R07] if 判断文件
来源：http://sb.hnjuh.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ey.szsharing.cn

[R08] 数值比较
来源：http://uk.yuntaijiaju.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://dz.9csxet.cn

[R09] 字符串比较
来源：http://yf.shxzskj.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://tt.colortex.cn

[R10] 正则匹配
来源：http://jh.muxihuayi.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ab.colortex.cn

[R11] case 多分支
来源：http://nn.haigaiapp.cn

case "$1" in
来源：http://bj.shxzukj.cn

start) echo "启动" ;;
来源：http://hw.bookmarksfly.cn

stop)  echo "停止" ;;
来源：http://iv.9csxet.cn

*)     echo "未知命令" ;;
来源：http://qs.bjjhwx.cn

esac
来源：http://yc.huanxung.cn

[R12] for 遍历文件
来源：http://zd.nicolike.cn

for f in *.txt; do echo "$f"; done
来源：http://am.shxzskj.cn

[R13] for 计数循环
来源：http://wc.wgjwhj.cn

for i in {1..10}; do echo "$i"; done
来源：http://gc.bookmarksfly.cn

[R14] C 风格 for
来源：http://xr.colortex.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://qa.haigaiapp.cn

[R15] while 逐行读文件
来源：http://dy.521024.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://vg.panjiajie.cn

[R16] until 等待条件
来源：http://ot.chemitech.net.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://am.szxytkj.cn

[R17] 数组定义与取值
来源：http://ea.szxytkj.cn

arr=(a b c); echo "${arr[0]}"
来源：http://on.gzmigu.cn

[R18] 遍历数组
来源：http://rk.hahajie.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ei.yuexingan06.cn

[R19] 数组长度
来源：http://lz.colortex.cn

echo "${#arr[@]}"
来源：http://it.haigaiapp.cn

[R20] 关联数组（字典）
来源：http://bc.521024.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://fk.wgjwhj.cn

[R21] 字符串长度
来源：http://id.huanxung.cn


<!-- 参考信息 -->