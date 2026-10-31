代发 wailian999

Py:   len(x)            # 字符串、列表、字典通用
来源：http://cq.asd995.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://vl.chemitech.net.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://zv.bjjhwx.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://kg.bookmarksfly.cn

Java: list.size();  map.size();  s.length()
来源：http://vp.haigaiapp.cn

Go:   len(arr);  len(m)
来源：http://cb.shxzskj.cn

Ruby: x.length;  x.size
来源：http://ad.hnjuh.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://ty.jctech888.com.cn

[P05] 判断两个对象内容是否相等
来源：http://fk.muxihuayi.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://dp.bjjhwx.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://xl.panjiajie.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://vg.hnjuh.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://it.yuexingan06.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://lr.huixinmuqiang.cn

Go:   reflect.DeepEqual(a, b)
来源：http://ia.bookmarksfly.cn

Ruby: a == b
来源：http://mi.haigaiapp.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://vf.jctech888.com.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://rs.huixiangedu.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://dc.shtwfgs.cn

PHP:  if (empty($x)) {}
来源：http://bh.521024.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ou.asd995.cn

TS:   if (x == null) {}
来源：http://fx.yuexingan06.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://ad.szsharing.cn

Go:   if x == nil {}
来源：http://pu.shxzukj.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wr.yuntaijiaju.cn

C#:   if (x is null) {}
来源：http://uo.huanxung.cn

[P07] 防抖与节流
来源：http://mr.huixiangedu.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://zk.lnxyls.cn

PHP:  // 手写时间戳比较
来源：http://bi.huanxung.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://eh.hahajie.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://cx.nicolike.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://qi.huixiangedu.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ot.muxihuayi.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://wh.huanxung.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://iu.hahajie.cn

[P08] 处理浮点精度问题
来源：http://qi.lnxyls.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://dx.panjiajie.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://kp.bjjhwx.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://um.colortex.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://kt.szxytkj.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://qr.nicolike.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ip.shxzskj.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://no.colortex.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ph.521024.cn

================================================================================
来源：http://oh.gzmigu.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://rw.yuntaijiaju.cn

================================================================================
来源：http://ky.yuntaijiaju.cn

[Q01] 创建表
来源：http://yi.panjiajie.cn

CREATE TABLE users (
来源：http://bm.hnjuh.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ag.lnxyls.cn

name VARCHAR(50) NOT NULL,
来源：http://mi.huanxung.cn

email VARCHAR(100) UNIQUE,
来源：http://tg.lnxyls.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://yq.521024.cn

);
来源：http://uu.hahajie.cn

[Q02] 创建带外键的表
来源：http://sg.colortex.cn

CREATE TABLE orders (
来源：http://pm.yuntaijiaju.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hn.shtwfgs.cn

user_id INT NOT NULL,
来源：http://ux.chemitech.net.cn

amount DECIMAL(10, 2),
来源：http://ho.521024.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://qw.jctech888.com.cn

);
来源：http://hw.huanxung.cn

[Q03] 增加列
来源：http://um.yuntaijiaju.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://zz.huixiangedu.cn

[Q04] 修改列类型
来源：http://nb.chemitech.net.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://md.shxzskj.cn

[Q05] 重命名列
来源：http://wm.yuexingan06.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mn.colortex.cn

[Q06] 删除列
来源：http://eu.szxytkj.cn

ALTER TABLE users DROP COLUMN age;
来源：http://zh.lnxyls.cn

[Q07] 删除表
来源：http://mh.huixiangedu.cn

DROP TABLE IF EXISTS orders;
来源：http://ty.bjjhwx.cn

[Q08] 创建普通索引
来源：http://ma.9csxet.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://xj.yuntaijiaju.cn

[Q09] 创建唯一索引
来源：http://bk.wgjwhj.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://tb.jctech888.com.cn

[Q10] 插入单行
来源：http://rv.huixinmuqiang.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://la.haigaiapp.cn

[Q11] 一次插入多行
来源：http://xc.newstarts.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://da.huixinmuqiang.cn

[Q12] 插入后取自增 ID
来源：http://bc.yuntaijiaju.cn

INSERT INTO users (name) VALUES ('C');
来源：http://uh.colortex.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://fd.haigaiapp.cn

[Q13] 忽略重复插入
来源：http://lp.szsharing.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://my.chemitech.net.cn

[Q14] 存在则更新（upsert）
来源：http://ix.huixiangedu.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wc.jctech888.com.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://gm.jctech888.com.cn

[Q15] 查询全部
来源：http://rd.521024.cn

SELECT * FROM users;
来源：http://hl.huixiangedu.cn

[Q16] 查询指定列
来源：http://nj.hnjuh.cn

SELECT id, name FROM users;
来源：http://gy.yuexingan06.cn

[Q17] 条件查询
来源：http://mu.nszjky.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wu.yuexingan06.cn

[Q18] 模糊匹配
来源：http://uf.huanxung.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://je.hnjuh.cn

[Q19] 范围查询
来源：http://rs.wgjwhj.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://sh.521024.cn

[Q20] IN 列表
来源：http://mk.521024.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://yd.huixinmuqiang.cn

[Q21] 空值判断
来源：http://cg.shtwfgs.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://qz.bookmarksfly.cn

[Q22] 排序
来源：http://da.gzmigu.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://vt.panjiajie.cn

[Q23] 分页
来源：http://ub.shxzukj.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://kx.lnxyls.cn

[Q24] 去重
来源：http://wm.yuexingan06.cn

SELECT DISTINCT city FROM users;
来源：http://uf.lnxyls.cn

[Q25] 只取前 N 条
来源：http://vk.nicolike.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://zg.panjiajie.cn

[Q26] 计数
来源：http://lp.hahajie.cn

SELECT COUNT(*) FROM users;
来源：http://bb.shxzukj.cn

[Q27] 条件计数
来源：http://qg.szxytkj.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://vj.nszjky.cn

[Q28] 求和与平均
来源：http://yj.newstarts.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://xy.huanxung.cn

[Q29] 最大最小值
来源：http://uh.huixinmuqiang.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://ni.yuntaijiaju.cn

[Q30] 分组统计
来源：http://oq.bjjhwx.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://cf.shxzukj.cn

[Q31] 分组后过滤
来源：http://nv.panjiajie.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://nj.chemitech.net.cn

[Q32] 分组拼接字符串
来源：http://mb.wgjwhj.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://pr.chemitech.net.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ar.lnxyls.cn

[Q33] 多列分组
来源：http://rv.huixiangedu.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://of.wgjwhj.cn

[Q34] 每组取第一条
来源：http://pc.jianghongdianzi.cn

SELECT * FROM (
来源：http://dz.huanxung.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://oj.shtwfgs.cn

) t WHERE rn = 1;
来源：http://ex.jctech888.com.cn

[Q35] 内连接
来源：http://ri.521024.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://up.jianghongdianzi.cn

[Q36] 左连接
来源：http://cs.newstarts.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://vu.muxihuayi.cn

[Q37] 右连接
来源：http://mx.szxytkj.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://tg.colortex.cn

[Q38] 全外连接（PostgreSQL）
来源：http://ez.huanxung.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hm.huixinmuqiang.cn

[Q39] 自连接（查上下级）
来源：http://uv.9csxet.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://ld.haigaiapp.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://gz.szxytkj.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://uv.szxytkj.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ur.colortex.cn

[Q41] 多表连接
来源：http://ku.521024.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://ah.colortex.cn

JOIN users u ON u.id = o.user_id
来源：http://ku.huixiangedu.cn

JOIN products p ON p.id = o.product_id;
来源：http://py.jianghongdianzi.cn

[Q42] 连接条件附加过滤
来源：http://ff.shxzskj.cn

SELECT u.name, o.amount FROM users u
来源：http://bd.9csxet.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://xc.huanxung.cn

[Q43] 标量子查询
来源：http://uz.huixinmuqiang.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://dp.nszjky.cn

[Q44] IN 子查询
来源：http://zi.lnxyls.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://kl.gzmigu.cn

[Q45] EXISTS 判断存在
来源：http://gk.wgjwhj.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://yv.nicolike.cn

[Q46] NOT EXISTS 判断不存在
来源：http://xj.huixiangedu.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://sf.shtwfgs.cn

[Q47] 与平均值比较
来源：http://ys.huixinmuqiang.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://cv.panjiajie.cn

[Q48] CTE 公用表表达式
来源：http://nm.bookmarksfly.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ux.hnjuh.cn

SELECT * FROM t WHERE c > 5;
来源：http://nu.shxzukj.cn

[Q49] 更新单行
来源：http://ai.yuexingan06.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://vg.panjiajie.cn

[Q50] 批量更新
来源：http://ut.chemitech.net.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://xc.huanxung.cn

[Q51] 用子查询更新
来源：http://vy.jianghongdianzi.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://nl.bjjhwx.cn

[Q52] 删除指定行
来源：http://mz.colortex.cn

DELETE FROM users WHERE id = 10;
来源：http://co.9csxet.cn

[Q53] 按条件删除
来源：http://oz.asd995.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://xj.shtwfgs.cn

[Q54] 清空表
来源：http://nq.szxytkj.cn

TRUNCATE TABLE logs;
来源：http://tv.newstarts.cn

[Q55] 排名（并列占位）
来源：http://hy.jctech888.com.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://fr.nszjky.cn

[Q56] 密集排名（并列不占位）
来源：http://ug.jianghongdianzi.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://gx.yuntaijiaju.cn

[Q57] 行号
来源：http://xc.wgjwhj.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://st.muxihuayi.cn

[Q58] 累计求和
来源：http://yp.9csxet.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://zl.shxzskj.cn

[Q59] 分组内累计
来源：http://zg.bjjhwx.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ts.9csxet.cn

[Q60] 取上一行 / 下一行
来源：http://vz.jianghongdianzi.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wr.shxzskj.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ww.haigaiapp.cn

[Q61] 移动平均
来源：http://zf.bookmarksfly.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://fl.hahajie.cn

[Q62] 分组占比
来源：http://hb.shxzukj.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://gf.9csxet.cn

[Q63] 开启事务
来源：http://kq.shtwfgs.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://zv.huixinmuqiang.cn

[Q64] 提交事务
来源：http://wy.asd995.cn

COMMIT;
来源：http://wr.colortex.cn

[Q65] 回滚事务
来源：http://dg.yuntaijiaju.cn

ROLLBACK;
来源：http://zq.szxytkj.cn

[Q66] 行锁查询
来源：http://lp.shxzskj.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ng.shxzukj.cn

[Q67] 设置隔离级别
来源：http://ff.muxihuayi.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://pd.jianghongdianzi.cn

[Q68] 保存点
来源：http://cm.nszjky.cn

SAVEPOINT sp1;
来源：http://tm.lnxyls.cn

ROLLBACK TO sp1;
来源：http://ac.hahajie.cn

[Q69] 查看执行计划
来源：http://tt.huixiangedu.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ke.shtwfgs.cn

[Q70] 更新统计信息
来源：http://bm.shtwfgs.cn

ANALYZE TABLE users;
来源：http://ti.shxzukj.cn

[Q71] 查看建表语句
来源：http://ts.jctech888.com.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://sb.jianghongdianzi.cn

[Q72] 查看索引
来源：http://oh.szsharing.cn

SHOW INDEX FROM users;
来源：http://bh.yuntaijiaju.cn

[Q73] 查看表状态
来源：http://sn.gzmigu.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://ap.wgjwhj.cn

[Q74] 强制使用索引
来源：http://ds.yuntaijiaju.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://sf.haigaiapp.cn

[Q75] 日期格式化
来源：http://jp.szsharing.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://la.newstarts.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://fy.lnxyls.cn

[Q76] 按天统计
来源：http://hc.huixinmuqiang.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://iw.jianghongdianzi.cn

[Q77] 时间加减
来源：http://jf.jianghongdianzi.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ex.gzmigu.cn

[Q78] 当前时间
来源：http://qo.colortex.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://nq.9csxet.cn

[Q79] 字符串拼接
来源：http://ye.shxzskj.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://jz.shxzskj.cn

[Q80] 字符串截取
来源：http://rw.lnxyls.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://xo.bookmarksfly.cn

[Q81] 字符串替换
来源：http://qh.panjiajie.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hg.bjjhwx.cn

[Q82] 字符长度与字节长度
来源：http://dp.newstarts.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://gs.jctech888.com.cn

[Q83] 大小写转换
来源：http://fd.haigaiapp.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ij.haigaiapp.cn

[Q84] 去除首尾空格
来源：http://ln.shxzskj.cn

SELECT TRIM(name) FROM users;
来源：http://xn.nicolike.cn

[Q85] 数值取整
来源：http://bh.haigaiapp.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://vv.asd995.cn

[Q86] 读取 JSON 字段
来源：http://ll.hnjuh.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://gt.hahajie.cn

[Q87] JSON 字段做条件
来源：http://uk.huixinmuqiang.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://vv.szxytkj.cn

[Q88] 行转列（条件聚合）
来源：http://xp.bookmarksfly.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://pz.huanxung.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mo.9csxet.cn

[Q89] 判断表是否存在
来源：http://rl.shtwfgs.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://gg.szsharing.cn

[Q90] 生成序号列
来源：http://km.huanxung.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://kr.chemitech.net.cn

================================================================================
来源：http://he.521024.cn

R. Bash 专题
来源：http://hk.huixiangedu.cn

================================================================================
来源：http://vv.jctech888.com.cn

[R01] shebang 与严格模式
来源：http://vd.lnxyls.cn

#!/usr/bin/env bash
来源：http://pw.gzmigu.cn

set -euo pipefail
来源：http://bn.bookmarksfly.cn

[R02] 变量赋值与使用
来源：http://jq.yuexingan06.cn

name="Tom"; echo "$name"
来源：http://hi.jianghongdianzi.cn

[R03] 只读变量
来源：http://ae.szsharing.cn

readonly PI=3.14
来源：http://td.yuntaijiaju.cn

[R04] 位置参数
来源：http://qe.521024.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://rt.9csxet.cn

[R05] 参数默认值
来源：http://as.newstarts.cn

name="${1:-default}"
来源：http://hj.hnjuh.cn

[R06] 判断命令是否存在
来源：http://cv.yuntaijiaju.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://yc.wgjwhj.cn

[R07] if 判断文件
来源：http://aq.hnjuh.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://zm.haigaiapp.cn

[R08] 数值比较
来源：http://bq.wgjwhj.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://im.newstarts.cn

[R09] 字符串比较
来源：http://un.asd995.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mw.yuexingan06.cn

[R10] 正则匹配
来源：http://bw.shxzskj.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://sq.hahajie.cn

[R11] case 多分支
来源：http://ge.shxzukj.cn

case "$1" in
来源：http://rd.bjjhwx.cn

start) echo "启动" ;;
来源：http://rj.bookmarksfly.cn

stop)  echo "停止" ;;
来源：http://zc.huanxung.cn

*)     echo "未知命令" ;;
来源：http://xc.huixinmuqiang.cn

esac
来源：http://kd.huanxung.cn

[R12] for 遍历文件
来源：http://jl.huixinmuqiang.cn

for f in *.txt; do echo "$f"; done
来源：http://wg.szsharing.cn

[R13] for 计数循环
来源：http://yi.shtwfgs.cn

for i in {1..10}; do echo "$i"; done
来源：http://rr.yuexingan06.cn

[R14] C 风格 for
来源：http://yx.shxzskj.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hh.huixinmuqiang.cn

[R15] while 逐行读文件
来源：http://wr.huixiangedu.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://fz.521024.cn

[R16] until 等待条件
来源：http://ai.bjjhwx.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://td.newstarts.cn

[R17] 数组定义与取值
来源：http://ql.yuntaijiaju.cn

arr=(a b c); echo "${arr[0]}"
来源：http://xq.panjiajie.cn

[R18] 遍历数组
来源：http://xn.bjjhwx.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://qm.szxytkj.cn

[R19] 数组长度
来源：http://kn.yuntaijiaju.cn

echo "${#arr[@]}"
来源：http://yy.521024.cn

[R20] 关联数组（字典）
来源：http://ut.newstarts.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://kh.panjiajie.cn

[R21] 字符串长度
来源：http://kc.jianghongdianzi.cn


<!-- 参考信息 -->