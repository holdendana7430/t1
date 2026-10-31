代发 wailian999

Py:   len(x)            # 字符串、列表、字典通用
来源：http://al.wgjwhj.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://lc.shxzukj.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://xd.szsharing.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://lf.hahajie.cn

Java: list.size();  map.size();  s.length()
来源：http://my.shxzukj.cn

Go:   len(arr);  len(m)
来源：http://sp.yuntaijiaju.cn

Ruby: x.length;  x.size
来源：http://ey.shxzskj.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://ue.asd995.cn

[P05] 判断两个对象内容是否相等
来源：http://bl.huixinmuqiang.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://rx.haigaiapp.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://lu.panjiajie.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://fs.chemitech.net.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://jx.jianghongdianzi.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://yu.nicolike.cn

Go:   reflect.DeepEqual(a, b)
来源：http://bz.9csxet.cn

Ruby: a == b
来源：http://bv.huanxung.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://sv.521024.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://vq.yuntaijiaju.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://xi.huixiangedu.cn

PHP:  if (empty($x)) {}
来源：http://ee.nszjky.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://rw.hnjuh.cn

TS:   if (x == null) {}
来源：http://xd.521024.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://kg.shtwfgs.cn

Go:   if x == nil {}
来源：http://lm.jctech888.com.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hr.chemitech.net.cn

C#:   if (x is null) {}
来源：http://ak.nszjky.cn

[P07] 防抖与节流
来源：http://oy.nszjky.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wq.yuexingan06.cn

PHP:  // 手写时间戳比较
来源：http://de.lnxyls.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://pp.asd995.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qd.bookmarksfly.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://fj.hnjuh.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://jy.bjjhwx.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://yz.szsharing.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://dr.huixiangedu.cn

[P08] 处理浮点精度问题
来源：http://bh.szsharing.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hd.muxihuayi.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://zy.yuntaijiaju.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://xy.huixinmuqiang.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ho.hahajie.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://rx.nicolike.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ls.muxihuayi.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://tw.muxihuayi.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://le.szsharing.cn

================================================================================
来源：http://nk.nszjky.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://gf.huanxung.cn

================================================================================
来源：http://dd.muxihuayi.cn

[Q01] 创建表
来源：http://wd.muxihuayi.cn

CREATE TABLE users (
来源：http://tl.panjiajie.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ij.colortex.cn

name VARCHAR(50) NOT NULL,
来源：http://ji.521024.cn

email VARCHAR(100) UNIQUE,
来源：http://cr.newstarts.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wq.jctech888.com.cn

);
来源：http://dl.shxzskj.cn

[Q02] 创建带外键的表
来源：http://yy.haigaiapp.cn

CREATE TABLE orders (
来源：http://zp.nicolike.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://kw.wgjwhj.cn

user_id INT NOT NULL,
来源：http://hf.yuntaijiaju.cn

amount DECIMAL(10, 2),
来源：http://qn.wgjwhj.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ks.colortex.cn

);
来源：http://ym.colortex.cn

[Q03] 增加列
来源：http://mx.yuntaijiaju.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://zi.hahajie.cn

[Q04] 修改列类型
来源：http://ga.yuntaijiaju.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://qu.gzmigu.cn

[Q05] 重命名列
来源：http://aa.nicolike.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mw.szsharing.cn

[Q06] 删除列
来源：http://lr.szxytkj.cn

ALTER TABLE users DROP COLUMN age;
来源：http://vn.521024.cn

[Q07] 删除表
来源：http://cs.bjjhwx.cn

DROP TABLE IF EXISTS orders;
来源：http://nx.jctech888.com.cn

[Q08] 创建普通索引
来源：http://bf.yuexingan06.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://qw.lnxyls.cn

[Q09] 创建唯一索引
来源：http://jq.yuntaijiaju.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://yk.huixinmuqiang.cn

[Q10] 插入单行
来源：http://ly.hnjuh.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mu.yuexingan06.cn

[Q11] 一次插入多行
来源：http://rg.chemitech.net.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ga.lnxyls.cn

[Q12] 插入后取自增 ID
来源：http://lh.asd995.cn

INSERT INTO users (name) VALUES ('C');
来源：http://gm.huixiangedu.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://nk.hahajie.cn

[Q13] 忽略重复插入
来源：http://du.gzmigu.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://xz.bjjhwx.cn

[Q14] 存在则更新（upsert）
来源：http://ik.gzmigu.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://zj.newstarts.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://cu.hnjuh.cn

[Q15] 查询全部
来源：http://tl.shxzukj.cn

SELECT * FROM users;
来源：http://ay.huixinmuqiang.cn

[Q16] 查询指定列
来源：http://fj.jianghongdianzi.cn

SELECT id, name FROM users;
来源：http://th.newstarts.cn

[Q17] 条件查询
来源：http://hn.muxihuayi.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://jn.shxzskj.cn

[Q18] 模糊匹配
来源：http://wy.bookmarksfly.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ws.panjiajie.cn

[Q19] 范围查询
来源：http://fj.huixinmuqiang.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://nt.bjjhwx.cn

[Q20] IN 列表
来源：http://df.wgjwhj.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://vw.panjiajie.cn

[Q21] 空值判断
来源：http://pj.shxzskj.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://rf.9csxet.cn

[Q22] 排序
来源：http://vf.szxytkj.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://on.huixiangedu.cn

[Q23] 分页
来源：http://wd.jctech888.com.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://cr.jianghongdianzi.cn

[Q24] 去重
来源：http://vo.jianghongdianzi.cn

SELECT DISTINCT city FROM users;
来源：http://zr.chemitech.net.cn

[Q25] 只取前 N 条
来源：http://iv.szsharing.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mf.hnjuh.cn

[Q26] 计数
来源：http://rc.bjjhwx.cn

SELECT COUNT(*) FROM users;
来源：http://gf.shxzskj.cn

[Q27] 条件计数
来源：http://iy.yuntaijiaju.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hb.shtwfgs.cn

[Q28] 求和与平均
来源：http://nt.gzmigu.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://vn.nszjky.cn

[Q29] 最大最小值
来源：http://bm.hahajie.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://lz.nicolike.cn

[Q30] 分组统计
来源：http://ns.jianghongdianzi.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://gv.chemitech.net.cn

[Q31] 分组后过滤
来源：http://uc.nicolike.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://yd.bookmarksfly.cn

[Q32] 分组拼接字符串
来源：http://vt.gzmigu.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://nt.hnjuh.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://la.yuntaijiaju.cn

[Q33] 多列分组
来源：http://xc.szsharing.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://gt.521024.cn

[Q34] 每组取第一条
来源：http://sx.colortex.cn

SELECT * FROM (
来源：http://go.hnjuh.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://gd.9csxet.cn

) t WHERE rn = 1;
来源：http://bz.newstarts.cn

[Q35] 内连接
来源：http://qb.yuntaijiaju.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://uc.asd995.cn

[Q36] 左连接
来源：http://wi.colortex.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://rh.szsharing.cn

[Q37] 右连接
来源：http://ov.hnjuh.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ry.gzmigu.cn

[Q38] 全外连接（PostgreSQL）
来源：http://yb.wgjwhj.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://jb.wgjwhj.cn

[Q39] 自连接（查上下级）
来源：http://em.szsharing.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://ed.9csxet.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mr.gzmigu.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://rt.jctech888.com.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://qn.521024.cn

[Q41] 多表连接
来源：http://bd.521024.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://fw.gzmigu.cn

JOIN users u ON u.id = o.user_id
来源：http://ao.newstarts.cn

JOIN products p ON p.id = o.product_id;
来源：http://ng.jianghongdianzi.cn

[Q42] 连接条件附加过滤
来源：http://bg.haigaiapp.cn

SELECT u.name, o.amount FROM users u
来源：http://od.shtwfgs.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://xy.huanxung.cn

[Q43] 标量子查询
来源：http://mz.colortex.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://of.szxytkj.cn

[Q44] IN 子查询
来源：http://td.colortex.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://qd.huixiangedu.cn

[Q45] EXISTS 判断存在
来源：http://vq.shtwfgs.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://eh.chemitech.net.cn

[Q46] NOT EXISTS 判断不存在
来源：http://zw.hahajie.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://gw.szxytkj.cn

[Q47] 与平均值比较
来源：http://ek.shtwfgs.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://fl.shtwfgs.cn

[Q48] CTE 公用表表达式
来源：http://ju.huanxung.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://gs.gzmigu.cn

SELECT * FROM t WHERE c > 5;
来源：http://fh.asd995.cn

[Q49] 更新单行
来源：http://ih.bookmarksfly.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://kx.shxzukj.cn

[Q50] 批量更新
来源：http://ge.asd995.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://xf.bookmarksfly.cn

[Q51] 用子查询更新
来源：http://mu.huixinmuqiang.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://ox.szsharing.cn

[Q52] 删除指定行
来源：http://wx.newstarts.cn

DELETE FROM users WHERE id = 10;
来源：http://bz.bookmarksfly.cn

[Q53] 按条件删除
来源：http://en.huixinmuqiang.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ba.bjjhwx.cn

[Q54] 清空表
来源：http://yy.hnjuh.cn

TRUNCATE TABLE logs;
来源：http://ep.gzmigu.cn

[Q55] 排名（并列占位）
来源：http://co.haigaiapp.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://rs.chemitech.net.cn

[Q56] 密集排名（并列不占位）
来源：http://rp.521024.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://tf.nicolike.cn

[Q57] 行号
来源：http://mo.bjjhwx.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ay.newstarts.cn

[Q58] 累计求和
来源：http://bt.szxytkj.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mx.panjiajie.cn

[Q59] 分组内累计
来源：http://zl.szsharing.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://bc.gzmigu.cn

[Q60] 取上一行 / 下一行
来源：http://oj.panjiajie.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://rr.bjjhwx.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://vp.panjiajie.cn

[Q61] 移动平均
来源：http://ud.szsharing.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://pv.nszjky.cn

[Q62] 分组占比
来源：http://iu.shxzukj.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mh.9csxet.cn

[Q63] 开启事务
来源：http://eo.asd995.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://gs.hahajie.cn

[Q64] 提交事务
来源：http://pw.lnxyls.cn

COMMIT;
来源：http://iv.jctech888.com.cn

[Q65] 回滚事务
来源：http://gl.jctech888.com.cn

ROLLBACK;
来源：http://fa.huixinmuqiang.cn

[Q66] 行锁查询
来源：http://bf.chemitech.net.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mx.hahajie.cn

[Q67] 设置隔离级别
来源：http://oe.huixiangedu.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ht.haigaiapp.cn

[Q68] 保存点
来源：http://pf.huanxung.cn

SAVEPOINT sp1;
来源：http://lq.muxihuayi.cn

ROLLBACK TO sp1;
来源：http://vy.colortex.cn

[Q69] 查看执行计划
来源：http://sc.chemitech.net.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://gi.newstarts.cn

[Q70] 更新统计信息
来源：http://li.gzmigu.cn

ANALYZE TABLE users;
来源：http://mo.asd995.cn

[Q71] 查看建表语句
来源：http://dp.newstarts.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://pg.muxihuayi.cn

[Q72] 查看索引
来源：http://kj.huixiangedu.cn

SHOW INDEX FROM users;
来源：http://ez.shtwfgs.cn

[Q73] 查看表状态
来源：http://cu.colortex.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://po.szsharing.cn

[Q74] 强制使用索引
来源：http://pq.gzmigu.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://oh.gzmigu.cn

[Q75] 日期格式化
来源：http://yf.yuexingan06.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://bb.jctech888.com.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ai.panjiajie.cn

[Q76] 按天统计
来源：http://qt.jianghongdianzi.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://gk.szxytkj.cn

[Q77] 时间加减
来源：http://kt.huanxung.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://xm.nszjky.cn

[Q78] 当前时间
来源：http://ht.nicolike.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://op.bookmarksfly.cn

[Q79] 字符串拼接
来源：http://kc.chemitech.net.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hs.nicolike.cn

[Q80] 字符串截取
来源：http://co.chemitech.net.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://zt.nszjky.cn

[Q81] 字符串替换
来源：http://yq.yuexingan06.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://gb.huixiangedu.cn

[Q82] 字符长度与字节长度
来源：http://pc.asd995.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://xv.nszjky.cn

[Q83] 大小写转换
来源：http://qg.huixiangedu.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://lm.gzmigu.cn

[Q84] 去除首尾空格
来源：http://ut.szxytkj.cn

SELECT TRIM(name) FROM users;
来源：http://ty.jctech888.com.cn

[Q85] 数值取整
来源：http://ww.yuntaijiaju.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ef.gzmigu.cn

[Q86] 读取 JSON 字段
来源：http://bw.chemitech.net.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ce.bookmarksfly.cn

[Q87] JSON 字段做条件
来源：http://eo.huanxung.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hp.yuntaijiaju.cn

[Q88] 行转列（条件聚合）
来源：http://se.chemitech.net.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://rb.muxihuayi.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://du.gzmigu.cn

[Q89] 判断表是否存在
来源：http://jx.nicolike.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://dh.9csxet.cn

[Q90] 生成序号列
来源：http://cu.shxzskj.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://da.haigaiapp.cn

================================================================================
来源：http://la.huixinmuqiang.cn

R. Bash 专题
来源：http://pa.szsharing.cn

================================================================================
来源：http://mt.colortex.cn

[R01] shebang 与严格模式
来源：http://qp.bookmarksfly.cn

#!/usr/bin/env bash
来源：http://se.nicolike.cn

set -euo pipefail
来源：http://id.chemitech.net.cn

[R02] 变量赋值与使用
来源：http://fi.gzmigu.cn

name="Tom"; echo "$name"
来源：http://sn.lnxyls.cn

[R03] 只读变量
来源：http://jx.newstarts.cn

readonly PI=3.14
来源：http://un.hahajie.cn

[R04] 位置参数
来源：http://al.hnjuh.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ao.colortex.cn

[R05] 参数默认值
来源：http://wc.shxzukj.cn

name="${1:-default}"
来源：http://wr.bookmarksfly.cn

[R06] 判断命令是否存在
来源：http://mg.yuexingan06.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ol.asd995.cn

[R07] if 判断文件
来源：http://bp.newstarts.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://jr.panjiajie.cn

[R08] 数值比较
来源：http://yh.jianghongdianzi.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://fs.hnjuh.cn

[R09] 字符串比较
来源：http://ri.shxzskj.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://je.shxzskj.cn

[R10] 正则匹配
来源：http://rs.huixiangedu.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://zp.jianghongdianzi.cn

[R11] case 多分支
来源：http://yt.nszjky.cn

case "$1" in
来源：http://jy.panjiajie.cn

start) echo "启动" ;;
来源：http://zx.521024.cn

stop)  echo "停止" ;;
来源：http://xn.yuexingan06.cn

*)     echo "未知命令" ;;
来源：http://hr.hahajie.cn

esac
来源：http://vp.shxzukj.cn

[R12] for 遍历文件
来源：http://iy.jctech888.com.cn

for f in *.txt; do echo "$f"; done
来源：http://dw.lnxyls.cn

[R13] for 计数循环
来源：http://vh.hahajie.cn

for i in {1..10}; do echo "$i"; done
来源：http://ze.newstarts.cn

[R14] C 风格 for
来源：http://kv.newstarts.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://nf.shxzukj.cn

[R15] while 逐行读文件
来源：http://uk.wgjwhj.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wl.szxytkj.cn

[R16] until 等待条件
来源：http://ao.yuntaijiaju.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ou.shxzskj.cn

[R17] 数组定义与取值
来源：http://yh.huixiangedu.cn

arr=(a b c); echo "${arr[0]}"
来源：http://cc.lnxyls.cn

[R18] 遍历数组
来源：http://oh.shxzskj.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://iu.nicolike.cn

[R19] 数组长度
来源：http://vn.wgjwhj.cn

echo "${#arr[@]}"
来源：http://sa.colortex.cn

[R20] 关联数组（字典）
来源：http://zf.jianghongdianzi.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hb.haigaiapp.cn

[R21] 字符串长度
来源：http://as.shxzukj.cn


<!-- 参考信息 -->