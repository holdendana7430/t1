代发 wailian999

Py:   len(x)            # 字符串、列表、字典通用
来源：http://kv.asd995.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mj.gzmigu.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://oc.9csxet.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://au.szxytkj.cn

Java: list.size();  map.size();  s.length()
来源：http://xp.gzmigu.cn

Go:   len(arr);  len(m)
来源：http://ez.colortex.cn

Ruby: x.length;  x.size
来源：http://lb.nicolike.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://nn.nicolike.cn

[P05] 判断两个对象内容是否相等
来源：http://pv.asd995.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://vu.hnjuh.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://un.521024.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://fc.lnxyls.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://di.jianghongdianzi.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://xz.muxihuayi.cn

Go:   reflect.DeepEqual(a, b)
来源：http://jv.hnjuh.cn

Ruby: a == b
来源：http://fu.newstarts.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://zf.chemitech.net.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ow.nszjky.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://cv.lnxyls.cn

PHP:  if (empty($x)) {}
来源：http://rn.colortex.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ie.shtwfgs.cn

TS:   if (x == null) {}
来源：http://lx.jianghongdianzi.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://cb.huixinmuqiang.cn

Go:   if x == nil {}
来源：http://sz.colortex.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://xl.muxihuayi.cn

C#:   if (x is null) {}
来源：http://dh.jianghongdianzi.cn

[P07] 防抖与节流
来源：http://sk.huixiangedu.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wt.szxytkj.cn

PHP:  // 手写时间戳比较
来源：http://dw.jctech888.com.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://fo.asd995.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://cs.chemitech.net.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ge.wgjwhj.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://yr.nszjky.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://ns.asd995.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://kf.yuexingan06.cn

[P08] 处理浮点精度问题
来源：http://pv.panjiajie.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ob.newstarts.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hd.hnjuh.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://zm.shxzskj.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ym.shxzskj.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://rc.lnxyls.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hu.huanxung.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://vl.huixiangedu.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://qx.szsharing.cn

================================================================================
来源：http://ll.colortex.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ry.asd995.cn

================================================================================
来源：http://ws.wgjwhj.cn

[Q01] 创建表
来源：http://yv.newstarts.cn

CREATE TABLE users (
来源：http://wf.shxzukj.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://zi.gzmigu.cn

name VARCHAR(50) NOT NULL,
来源：http://un.panjiajie.cn

email VARCHAR(100) UNIQUE,
来源：http://yg.shtwfgs.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wo.yuntaijiaju.cn

);
来源：http://vb.yuexingan06.cn

[Q02] 创建带外键的表
来源：http://fs.jianghongdianzi.cn

CREATE TABLE orders (
来源：http://hb.shxzskj.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ps.jctech888.com.cn

user_id INT NOT NULL,
来源：http://jd.nszjky.cn

amount DECIMAL(10, 2),
来源：http://kj.chemitech.net.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://fs.huixiangedu.cn

);
来源：http://of.nicolike.cn

[Q03] 增加列
来源：http://mx.bookmarksfly.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://pb.newstarts.cn

[Q04] 修改列类型
来源：http://qj.newstarts.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ro.shtwfgs.cn

[Q05] 重命名列
来源：http://yj.panjiajie.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://xg.panjiajie.cn

[Q06] 删除列
来源：http://rt.wgjwhj.cn

ALTER TABLE users DROP COLUMN age;
来源：http://yf.huixiangedu.cn

[Q07] 删除表
来源：http://qz.newstarts.cn

DROP TABLE IF EXISTS orders;
来源：http://kj.chemitech.net.cn

[Q08] 创建普通索引
来源：http://nl.colortex.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://qg.huixinmuqiang.cn

[Q09] 创建唯一索引
来源：http://ne.asd995.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://vi.chemitech.net.cn

[Q10] 插入单行
来源：http://og.wgjwhj.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ap.shxzukj.cn

[Q11] 一次插入多行
来源：http://jq.huixiangedu.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://de.huixiangedu.cn

[Q12] 插入后取自增 ID
来源：http://ny.bjjhwx.cn

INSERT INTO users (name) VALUES ('C');
来源：http://pm.bookmarksfly.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ak.newstarts.cn

[Q13] 忽略重复插入
来源：http://wz.shtwfgs.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ff.nszjky.cn

[Q14] 存在则更新（upsert）
来源：http://qs.muxihuayi.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hd.hahajie.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ct.hahajie.cn

[Q15] 查询全部
来源：http://an.shxzskj.cn

SELECT * FROM users;
来源：http://sn.panjiajie.cn

[Q16] 查询指定列
来源：http://fo.nicolike.cn

SELECT id, name FROM users;
来源：http://pq.muxihuayi.cn

[Q17] 条件查询
来源：http://ih.nszjky.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://cm.yuntaijiaju.cn

[Q18] 模糊匹配
来源：http://kk.yuntaijiaju.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://kf.panjiajie.cn

[Q19] 范围查询
来源：http://hu.nszjky.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://xg.shxzukj.cn

[Q20] IN 列表
来源：http://zo.wgjwhj.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://gw.nszjky.cn

[Q21] 空值判断
来源：http://ta.asd995.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://hc.bookmarksfly.cn

[Q22] 排序
来源：http://lt.521024.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hs.jctech888.com.cn

[Q23] 分页
来源：http://sq.panjiajie.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hp.nicolike.cn

[Q24] 去重
来源：http://cs.asd995.cn

SELECT DISTINCT city FROM users;
来源：http://xm.huixiangedu.cn

[Q25] 只取前 N 条
来源：http://cc.panjiajie.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mt.nszjky.cn

[Q26] 计数
来源：http://ri.yuntaijiaju.cn

SELECT COUNT(*) FROM users;
来源：http://co.nszjky.cn

[Q27] 条件计数
来源：http://gq.yuntaijiaju.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://kz.nicolike.cn

[Q28] 求和与平均
来源：http://jg.huixinmuqiang.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://lo.lnxyls.cn

[Q29] 最大最小值
来源：http://oy.jctech888.com.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://jb.jctech888.com.cn

[Q30] 分组统计
来源：http://xz.szsharing.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://sz.yuntaijiaju.cn

[Q31] 分组后过滤
来源：http://nt.gzmigu.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://pf.colortex.cn

[Q32] 分组拼接字符串
来源：http://gu.9csxet.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ct.jctech888.com.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hr.hahajie.cn

[Q33] 多列分组
来源：http://zc.yuntaijiaju.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ht.521024.cn

[Q34] 每组取第一条
来源：http://jz.9csxet.cn

SELECT * FROM (
来源：http://pt.jianghongdianzi.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://oi.szxytkj.cn

) t WHERE rn = 1;
来源：http://fy.nszjky.cn

[Q35] 内连接
来源：http://zg.yuexingan06.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hi.lnxyls.cn

[Q36] 左连接
来源：http://jg.muxihuayi.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://my.gzmigu.cn

[Q37] 右连接
来源：http://eh.wgjwhj.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://vl.nszjky.cn

[Q38] 全外连接（PostgreSQL）
来源：http://ii.yuntaijiaju.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://bw.521024.cn

[Q39] 自连接（查上下级）
来源：http://jj.yuexingan06.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://pw.jianghongdianzi.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ga.9csxet.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://xj.hnjuh.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://fv.hahajie.cn

[Q41] 多表连接
来源：http://af.szsharing.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://my.muxihuayi.cn

JOIN users u ON u.id = o.user_id
来源：http://hu.yuntaijiaju.cn

JOIN products p ON p.id = o.product_id;
来源：http://rp.chemitech.net.cn

[Q42] 连接条件附加过滤
来源：http://rt.muxihuayi.cn

SELECT u.name, o.amount FROM users u
来源：http://ft.haigaiapp.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ch.jianghongdianzi.cn

[Q43] 标量子查询
来源：http://gn.bookmarksfly.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://jr.shxzskj.cn

[Q44] IN 子查询
来源：http://dt.shxzukj.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://xu.huixinmuqiang.cn

[Q45] EXISTS 判断存在
来源：http://lb.gzmigu.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://aj.shxzskj.cn

[Q46] NOT EXISTS 判断不存在
来源：http://ry.gzmigu.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hu.shtwfgs.cn

[Q47] 与平均值比较
来源：http://su.jianghongdianzi.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://gd.hnjuh.cn

[Q48] CTE 公用表表达式
来源：http://xo.haigaiapp.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://to.chemitech.net.cn

SELECT * FROM t WHERE c > 5;
来源：http://xc.hahajie.cn

[Q49] 更新单行
来源：http://dm.haigaiapp.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wg.nszjky.cn

[Q50] 批量更新
来源：http://gk.bjjhwx.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://es.yuntaijiaju.cn

[Q51] 用子查询更新
来源：http://bi.bookmarksfly.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://vg.shxzukj.cn

[Q52] 删除指定行
来源：http://iq.szxytkj.cn

DELETE FROM users WHERE id = 10;
来源：http://ip.szxytkj.cn

[Q53] 按条件删除
来源：http://to.muxihuayi.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://qd.wgjwhj.cn

[Q54] 清空表
来源：http://jq.huixinmuqiang.cn

TRUNCATE TABLE logs;
来源：http://iw.nszjky.cn

[Q55] 排名（并列占位）
来源：http://qo.wgjwhj.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mx.huixiangedu.cn

[Q56] 密集排名（并列不占位）
来源：http://tx.szsharing.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://al.asd995.cn

[Q57] 行号
来源：http://ei.colortex.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://to.bjjhwx.cn

[Q58] 累计求和
来源：http://wg.shxzukj.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://rn.chemitech.net.cn

[Q59] 分组内累计
来源：http://xc.hnjuh.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://an.chemitech.net.cn

[Q60] 取上一行 / 下一行
来源：http://uh.chemitech.net.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wr.wgjwhj.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://gh.huanxung.cn

[Q61] 移动平均
来源：http://ce.wgjwhj.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://xt.shtwfgs.cn

[Q62] 分组占比
来源：http://sp.haigaiapp.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://kc.szsharing.cn

[Q63] 开启事务
来源：http://ya.yuexingan06.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://uv.huixiangedu.cn

[Q64] 提交事务
来源：http://fu.lnxyls.cn

COMMIT;
来源：http://wf.shxzukj.cn

[Q65] 回滚事务
来源：http://xt.newstarts.cn

ROLLBACK;
来源：http://to.chemitech.net.cn

[Q66] 行锁查询
来源：http://bv.jctech888.com.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://yn.asd995.cn

[Q67] 设置隔离级别
来源：http://ct.bookmarksfly.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://yl.shtwfgs.cn

[Q68] 保存点
来源：http://at.muxihuayi.cn

SAVEPOINT sp1;
来源：http://yh.hahajie.cn

ROLLBACK TO sp1;
来源：http://kp.bjjhwx.cn

[Q69] 查看执行计划
来源：http://qj.hnjuh.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://dd.jianghongdianzi.cn

[Q70] 更新统计信息
来源：http://ja.hnjuh.cn

ANALYZE TABLE users;
来源：http://jw.chemitech.net.cn

[Q71] 查看建表语句
来源：http://id.colortex.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://vl.hahajie.cn

[Q72] 查看索引
来源：http://ai.wgjwhj.cn

SHOW INDEX FROM users;
来源：http://tf.haigaiapp.cn

[Q73] 查看表状态
来源：http://zn.shxzukj.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://fl.9csxet.cn

[Q74] 强制使用索引
来源：http://pd.yuntaijiaju.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://li.asd995.cn

[Q75] 日期格式化
来源：http://vp.huixinmuqiang.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://vv.bjjhwx.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mx.nszjky.cn

[Q76] 按天统计
来源：http://tx.yuntaijiaju.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://cx.shxzskj.cn

[Q77] 时间加减
来源：http://zm.wgjwhj.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://jp.yuntaijiaju.cn

[Q78] 当前时间
来源：http://it.jianghongdianzi.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://xn.bookmarksfly.cn

[Q79] 字符串拼接
来源：http://ck.hahajie.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://sl.hnjuh.cn

[Q80] 字符串截取
来源：http://uu.szsharing.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://es.colortex.cn

[Q81] 字符串替换
来源：http://rh.521024.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://au.yuntaijiaju.cn

[Q82] 字符长度与字节长度
来源：http://du.chemitech.net.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://kg.szxytkj.cn

[Q83] 大小写转换
来源：http://ic.9csxet.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://jj.gzmigu.cn

[Q84] 去除首尾空格
来源：http://kj.huixinmuqiang.cn

SELECT TRIM(name) FROM users;
来源：http://tq.jianghongdianzi.cn

[Q85] 数值取整
来源：http://nj.huixiangedu.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://dw.chemitech.net.cn

[Q86] 读取 JSON 字段
来源：http://gg.yuexingan06.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://kt.hahajie.cn

[Q87] JSON 字段做条件
来源：http://hi.wgjwhj.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://on.newstarts.cn

[Q88] 行转列（条件聚合）
来源：http://pf.shxzskj.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ye.huanxung.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://br.521024.cn

[Q89] 判断表是否存在
来源：http://uk.hnjuh.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://gz.panjiajie.cn

[Q90] 生成序号列
来源：http://xe.521024.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mx.asd995.cn

================================================================================
来源：http://zm.szsharing.cn

R. Bash 专题
来源：http://kb.shtwfgs.cn

================================================================================
来源：http://sp.yuexingan06.cn

[R01] shebang 与严格模式
来源：http://gn.lnxyls.cn

#!/usr/bin/env bash
来源：http://uq.nicolike.cn

set -euo pipefail
来源：http://dl.huixinmuqiang.cn

[R02] 变量赋值与使用
来源：http://wf.shxzskj.cn

name="Tom"; echo "$name"
来源：http://su.szsharing.cn

[R03] 只读变量
来源：http://rw.lnxyls.cn

readonly PI=3.14
来源：http://aw.hnjuh.cn

[R04] 位置参数
来源：http://oy.wgjwhj.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ig.huixiangedu.cn

[R05] 参数默认值
来源：http://ia.nicolike.cn

name="${1:-default}"
来源：http://io.panjiajie.cn

[R06] 判断命令是否存在
来源：http://ke.shxzukj.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://nr.muxihuayi.cn

[R07] if 判断文件
来源：http://po.nicolike.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://kj.colortex.cn

[R08] 数值比较
来源：http://ey.jianghongdianzi.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://lh.asd995.cn

[R09] 字符串比较
来源：http://rj.jianghongdianzi.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://dp.9csxet.cn

[R10] 正则匹配
来源：http://po.lnxyls.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://qi.huixinmuqiang.cn

[R11] case 多分支
来源：http://hf.hahajie.cn

case "$1" in
来源：http://bs.shtwfgs.cn

start) echo "启动" ;;
来源：http://hn.lnxyls.cn

stop)  echo "停止" ;;
来源：http://tk.yuexingan06.cn

*)     echo "未知命令" ;;
来源：http://ss.shtwfgs.cn

esac
来源：http://wd.shtwfgs.cn

[R12] for 遍历文件
来源：http://qs.nicolike.cn

for f in *.txt; do echo "$f"; done
来源：http://us.chemitech.net.cn

[R13] for 计数循环
来源：http://ow.nicolike.cn

for i in {1..10}; do echo "$i"; done
来源：http://tt.haigaiapp.cn

[R14] C 风格 for
来源：http://ih.jianghongdianzi.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wz.szxytkj.cn

[R15] while 逐行读文件
来源：http://kq.colortex.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://zw.shtwfgs.cn

[R16] until 等待条件
来源：http://fj.hnjuh.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://iu.hahajie.cn

[R17] 数组定义与取值
来源：http://fo.jianghongdianzi.cn

arr=(a b c); echo "${arr[0]}"
来源：http://em.521024.cn

[R18] 遍历数组
来源：http://lu.huixinmuqiang.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://sg.hahajie.cn

[R19] 数组长度
来源：http://pj.muxihuayi.cn

echo "${#arr[@]}"
来源：http://az.jianghongdianzi.cn

[R20] 关联数组（字典）
来源：http://vr.huanxung.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://jm.panjiajie.cn

[R21] 字符串长度
来源：http://kx.bookmarksfly.cn


<!-- 参考信息 -->