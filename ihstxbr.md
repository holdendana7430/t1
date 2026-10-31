代发 wailian999

Py:   len(x)            # 字符串、列表、字典通用
来源：http://tw.lnxyls.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://es.hnjuh.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ed.gzmigu.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://pv.muxihuayi.cn

Java: list.size();  map.size();  s.length()
来源：http://jq.huixinmuqiang.cn

Go:   len(arr);  len(m)
来源：http://gu.panjiajie.cn

Ruby: x.length;  x.size
来源：http://mb.9csxet.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://hl.nszjky.cn

[P05] 判断两个对象内容是否相等
来源：http://oa.panjiajie.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://qx.gzmigu.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://rz.huanxung.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://jw.haigaiapp.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://lt.hnjuh.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://rh.asd995.cn

Go:   reflect.DeepEqual(a, b)
来源：http://ny.newstarts.cn

Ruby: a == b
来源：http://fl.hnjuh.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ph.shxzukj.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://xl.bjjhwx.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ic.hnjuh.cn

PHP:  if (empty($x)) {}
来源：http://qu.yuexingan06.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mt.muxihuayi.cn

TS:   if (x == null) {}
来源：http://or.shxzskj.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://mc.yuexingan06.cn

Go:   if x == nil {}
来源：http://ui.shxzskj.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://sv.gzmigu.cn

C#:   if (x is null) {}
来源：http://qs.hnjuh.cn

[P07] 防抖与节流
来源：http://la.hnjuh.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mj.bjjhwx.cn

PHP:  // 手写时间戳比较
来源：http://jl.newstarts.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://co.szsharing.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://yu.nszjky.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://pu.shtwfgs.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ev.szxytkj.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://ks.szsharing.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ed.hahajie.cn

[P08] 处理浮点精度问题
来源：http://jm.9csxet.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://kf.jctech888.com.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://eh.panjiajie.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://sg.hahajie.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hj.nicolike.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://xv.yuexingan06.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ef.huixiangedu.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://px.huixinmuqiang.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://vi.yuntaijiaju.cn

================================================================================
来源：http://ow.521024.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://vi.huixinmuqiang.cn

================================================================================
来源：http://fu.huixinmuqiang.cn

[Q01] 创建表
来源：http://jj.huixiangedu.cn

CREATE TABLE users (
来源：http://ef.huixinmuqiang.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hg.szsharing.cn

name VARCHAR(50) NOT NULL,
来源：http://eb.haigaiapp.cn

email VARCHAR(100) UNIQUE,
来源：http://ac.shxzukj.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://jw.yuntaijiaju.cn

);
来源：http://lq.yuexingan06.cn

[Q02] 创建带外键的表
来源：http://dt.huanxung.cn

CREATE TABLE orders (
来源：http://zk.colortex.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://rf.bjjhwx.cn

user_id INT NOT NULL,
来源：http://jh.huixiangedu.cn

amount DECIMAL(10, 2),
来源：http://jn.newstarts.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://vq.asd995.cn

);
来源：http://mt.yuntaijiaju.cn

[Q03] 增加列
来源：http://an.huanxung.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://oo.hahajie.cn

[Q04] 修改列类型
来源：http://ts.haigaiapp.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://fm.szsharing.cn

[Q05] 重命名列
来源：http://mb.9csxet.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ca.hnjuh.cn

[Q06] 删除列
来源：http://cg.lnxyls.cn

ALTER TABLE users DROP COLUMN age;
来源：http://ji.bjjhwx.cn

[Q07] 删除表
来源：http://tm.asd995.cn

DROP TABLE IF EXISTS orders;
来源：http://ak.huixinmuqiang.cn

[Q08] 创建普通索引
来源：http://im.jianghongdianzi.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://oo.yuntaijiaju.cn

[Q09] 创建唯一索引
来源：http://sa.521024.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ar.huixiangedu.cn

[Q10] 插入单行
来源：http://xf.shxzskj.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://by.huanxung.cn

[Q11] 一次插入多行
来源：http://zk.jctech888.com.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://xt.huixiangedu.cn

[Q12] 插入后取自增 ID
来源：http://jf.huixiangedu.cn

INSERT INTO users (name) VALUES ('C');
来源：http://ob.521024.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://to.shxzukj.cn

[Q13] 忽略重复插入
来源：http://lb.shtwfgs.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://et.hnjuh.cn

[Q14] 存在则更新（upsert）
来源：http://ng.muxihuayi.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://zg.huixinmuqiang.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://jn.jctech888.com.cn

[Q15] 查询全部
来源：http://dz.yuntaijiaju.cn

SELECT * FROM users;
来源：http://ui.lnxyls.cn

[Q16] 查询指定列
来源：http://zl.hnjuh.cn

SELECT id, name FROM users;
来源：http://ut.wgjwhj.cn

[Q17] 条件查询
来源：http://uv.lnxyls.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mj.colortex.cn

[Q18] 模糊匹配
来源：http://rr.bjjhwx.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://nf.lnxyls.cn

[Q19] 范围查询
来源：http://kz.chemitech.net.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://sl.gzmigu.cn

[Q20] IN 列表
来源：http://eq.bjjhwx.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://rd.asd995.cn

[Q21] 空值判断
来源：http://xk.szsharing.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://fj.shtwfgs.cn

[Q22] 排序
来源：http://bx.yuexingan06.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://kx.shtwfgs.cn

[Q23] 分页
来源：http://vw.haigaiapp.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ql.gzmigu.cn

[Q24] 去重
来源：http://qx.panjiajie.cn

SELECT DISTINCT city FROM users;
来源：http://ay.wgjwhj.cn

[Q25] 只取前 N 条
来源：http://jo.colortex.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://fk.bookmarksfly.cn

[Q26] 计数
来源：http://zl.nszjky.cn

SELECT COUNT(*) FROM users;
来源：http://mq.asd995.cn

[Q27] 条件计数
来源：http://ni.newstarts.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://zd.colortex.cn

[Q28] 求和与平均
来源：http://dq.huanxung.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://qt.newstarts.cn

[Q29] 最大最小值
来源：http://ri.haigaiapp.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://hn.hnjuh.cn

[Q30] 分组统计
来源：http://sg.hnjuh.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://kt.newstarts.cn

[Q31] 分组后过滤
来源：http://fg.yuntaijiaju.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://rh.muxihuayi.cn

[Q32] 分组拼接字符串
来源：http://zf.9csxet.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://bx.jctech888.com.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ww.nszjky.cn

[Q33] 多列分组
来源：http://mb.haigaiapp.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://xp.shtwfgs.cn

[Q34] 每组取第一条
来源：http://ox.panjiajie.cn

SELECT * FROM (
来源：http://mo.jianghongdianzi.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hc.panjiajie.cn

) t WHERE rn = 1;
来源：http://ju.bjjhwx.cn

[Q35] 内连接
来源：http://nr.szxytkj.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ea.gzmigu.cn

[Q36] 左连接
来源：http://eo.hahajie.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://xt.panjiajie.cn

[Q37] 右连接
来源：http://ky.hnjuh.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://qg.lnxyls.cn

[Q38] 全外连接（PostgreSQL）
来源：http://sh.muxihuayi.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://jl.szxytkj.cn

[Q39] 自连接（查上下级）
来源：http://af.huixinmuqiang.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://ei.hnjuh.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://em.chemitech.net.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://nk.wgjwhj.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://nu.gzmigu.cn

[Q41] 多表连接
来源：http://su.jianghongdianzi.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://tf.shxzskj.cn

JOIN users u ON u.id = o.user_id
来源：http://ca.huixinmuqiang.cn

JOIN products p ON p.id = o.product_id;
来源：http://sb.9csxet.cn

[Q42] 连接条件附加过滤
来源：http://qz.wgjwhj.cn

SELECT u.name, o.amount FROM users u
来源：http://ef.huanxung.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://we.nszjky.cn

[Q43] 标量子查询
来源：http://nq.colortex.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://kq.colortex.cn

[Q44] IN 子查询
来源：http://ei.nicolike.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://do.shtwfgs.cn

[Q45] EXISTS 判断存在
来源：http://sx.asd995.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://vu.yuexingan06.cn

[Q46] NOT EXISTS 判断不存在
来源：http://bg.szsharing.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://xp.szsharing.cn

[Q47] 与平均值比较
来源：http://jz.9csxet.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://we.newstarts.cn

[Q48] CTE 公用表表达式
来源：http://bz.shtwfgs.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://px.newstarts.cn

SELECT * FROM t WHERE c > 5;
来源：http://yj.gzmigu.cn

[Q49] 更新单行
来源：http://aq.yuntaijiaju.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://em.lnxyls.cn

[Q50] 批量更新
来源：http://yj.jctech888.com.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://gs.shtwfgs.cn

[Q51] 用子查询更新
来源：http://db.hahajie.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://cw.bookmarksfly.cn

[Q52] 删除指定行
来源：http://km.yuexingan06.cn

DELETE FROM users WHERE id = 10;
来源：http://gl.asd995.cn

[Q53] 按条件删除
来源：http://sf.521024.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://vg.521024.cn

[Q54] 清空表
来源：http://zm.newstarts.cn

TRUNCATE TABLE logs;
来源：http://aa.haigaiapp.cn

[Q55] 排名（并列占位）
来源：http://bn.shtwfgs.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://gz.wgjwhj.cn

[Q56] 密集排名（并列不占位）
来源：http://sx.szsharing.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://su.panjiajie.cn

[Q57] 行号
来源：http://om.hahajie.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ne.yuexingan06.cn

[Q58] 累计求和
来源：http://ba.shxzskj.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://gt.wgjwhj.cn

[Q59] 分组内累计
来源：http://wo.jctech888.com.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://cq.nszjky.cn

[Q60] 取上一行 / 下一行
来源：http://lc.wgjwhj.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ha.asd995.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://qi.bjjhwx.cn

[Q61] 移动平均
来源：http://ps.huixinmuqiang.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://la.huixiangedu.cn

[Q62] 分组占比
来源：http://ag.jctech888.com.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://kg.panjiajie.cn

[Q63] 开启事务
来源：http://jf.521024.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://qc.bjjhwx.cn

[Q64] 提交事务
来源：http://xg.panjiajie.cn

COMMIT;
来源：http://wj.hahajie.cn

[Q65] 回滚事务
来源：http://vk.shxzukj.cn

ROLLBACK;
来源：http://ki.szxytkj.cn

[Q66] 行锁查询
来源：http://tv.gzmigu.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://rw.521024.cn

[Q67] 设置隔离级别
来源：http://ev.yuntaijiaju.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://tq.huixiangedu.cn

[Q68] 保存点
来源：http://gs.shxzukj.cn

SAVEPOINT sp1;
来源：http://rk.newstarts.cn

ROLLBACK TO sp1;
来源：http://ix.szxytkj.cn

[Q69] 查看执行计划
来源：http://eh.lnxyls.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://zx.szsharing.cn

[Q70] 更新统计信息
来源：http://tw.jctech888.com.cn

ANALYZE TABLE users;
来源：http://lh.muxihuayi.cn

[Q71] 查看建表语句
来源：http://su.szsharing.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://cc.szxytkj.cn

[Q72] 查看索引
来源：http://kl.huanxung.cn

SHOW INDEX FROM users;
来源：http://hd.panjiajie.cn

[Q73] 查看表状态
来源：http://qd.muxihuayi.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://rb.hnjuh.cn

[Q74] 强制使用索引
来源：http://th.bjjhwx.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://nn.hnjuh.cn

[Q75] 日期格式化
来源：http://eg.bjjhwx.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://no.yuexingan06.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://jc.shtwfgs.cn

[Q76] 按天统计
来源：http://ff.huixiangedu.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://fi.wgjwhj.cn

[Q77] 时间加减
来源：http://ev.newstarts.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://cn.wgjwhj.cn

[Q78] 当前时间
来源：http://fk.huixinmuqiang.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://pk.huanxung.cn

[Q79] 字符串拼接
来源：http://jp.521024.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wf.colortex.cn

[Q80] 字符串截取
来源：http://px.colortex.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://pd.shxzskj.cn

[Q81] 字符串替换
来源：http://xg.huixinmuqiang.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ul.huixinmuqiang.cn

[Q82] 字符长度与字节长度
来源：http://ui.jctech888.com.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://dq.hnjuh.cn

[Q83] 大小写转换
来源：http://va.hnjuh.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://sq.chemitech.net.cn

[Q84] 去除首尾空格
来源：http://ws.szxytkj.cn

SELECT TRIM(name) FROM users;
来源：http://wm.hnjuh.cn

[Q85] 数值取整
来源：http://uu.asd995.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://rq.szxytkj.cn

[Q86] 读取 JSON 字段
来源：http://bl.yuexingan06.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://fm.wgjwhj.cn

[Q87] JSON 字段做条件
来源：http://kg.hahajie.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://me.shxzskj.cn

[Q88] 行转列（条件聚合）
来源：http://am.yuntaijiaju.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://oq.szxytkj.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ol.huanxung.cn

[Q89] 判断表是否存在
来源：http://yn.szxytkj.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://yb.chemitech.net.cn

[Q90] 生成序号列
来源：http://mo.panjiajie.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://rd.colortex.cn

================================================================================
来源：http://yk.bjjhwx.cn

R. Bash 专题
来源：http://to.wgjwhj.cn

================================================================================
来源：http://vg.gzmigu.cn

[R01] shebang 与严格模式
来源：http://ye.szxytkj.cn

#!/usr/bin/env bash
来源：http://dg.bookmarksfly.cn

set -euo pipefail
来源：http://qw.szxytkj.cn

[R02] 变量赋值与使用
来源：http://ta.lnxyls.cn

name="Tom"; echo "$name"
来源：http://cv.shtwfgs.cn

[R03] 只读变量
来源：http://td.huixiangedu.cn

readonly PI=3.14
来源：http://uy.jctech888.com.cn

[R04] 位置参数
来源：http://rl.huixiangedu.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://am.yuexingan06.cn

[R05] 参数默认值
来源：http://vq.shtwfgs.cn

name="${1:-default}"
来源：http://xn.jianghongdianzi.cn

[R06] 判断命令是否存在
来源：http://ww.bookmarksfly.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://eo.shxzukj.cn

[R07] if 判断文件
来源：http://dl.newstarts.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://zf.szsharing.cn

[R08] 数值比较
来源：http://ev.jctech888.com.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://kw.9csxet.cn

[R09] 字符串比较
来源：http://hj.521024.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://nq.lnxyls.cn

[R10] 正则匹配
来源：http://cr.huixinmuqiang.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://qj.9csxet.cn

[R11] case 多分支
来源：http://kv.shxzukj.cn

case "$1" in
来源：http://ah.huanxung.cn

start) echo "启动" ;;
来源：http://sy.jctech888.com.cn

stop)  echo "停止" ;;
来源：http://zv.jctech888.com.cn

*)     echo "未知命令" ;;
来源：http://kr.huixiangedu.cn

esac
来源：http://wh.panjiajie.cn

[R12] for 遍历文件
来源：http://bo.colortex.cn

for f in *.txt; do echo "$f"; done
来源：http://qj.bjjhwx.cn

[R13] for 计数循环
来源：http://hr.haigaiapp.cn

for i in {1..10}; do echo "$i"; done
来源：http://ka.huixinmuqiang.cn

[R14] C 风格 for
来源：http://ig.shxzukj.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://zl.huanxung.cn

[R15] while 逐行读文件
来源：http://go.bjjhwx.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://bv.yuexingan06.cn

[R16] until 等待条件
来源：http://qr.asd995.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://yg.huixiangedu.cn

[R17] 数组定义与取值
来源：http://aw.panjiajie.cn

arr=(a b c); echo "${arr[0]}"
来源：http://ay.yuntaijiaju.cn

[R18] 遍历数组
来源：http://yp.shxzukj.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://px.huixinmuqiang.cn

[R19] 数组长度
来源：http://rk.bookmarksfly.cn

echo "${#arr[@]}"
来源：http://nv.jianghongdianzi.cn

[R20] 关联数组（字典）
来源：http://xd.bjjhwx.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://kt.asd995.cn

[R21] 字符串长度
来源：http://zy.hahajie.cn


<!-- 参考信息 -->