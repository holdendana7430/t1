代发 wailian999

Java: list.size();  map.size();  s.length()
来源：http://ds.haigaiapp.cn

Go:   len(arr);  len(m)
来源：http://wd.hnjuh.cn

Ruby: x.length;  x.size
来源：http://ye.bookmarksfly.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://nm.muxihuayi.cn

[P05] 判断两个对象内容是否相等
来源：http://ph.9csxet.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://fa.521024.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://zh.jianghongdianzi.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://cf.chemitech.net.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://xo.bjjhwx.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://iv.colortex.cn

Go:   reflect.DeepEqual(a, b)
来源：http://su.shxzukj.cn

Ruby: a == b
来源：http://nd.hnjuh.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://rz.yuexingan06.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://zg.huanxung.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://jh.szsharing.cn

PHP:  if (empty($x)) {}
来源：http://sk.szsharing.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://kt.lnxyls.cn

TS:   if (x == null) {}
来源：http://ln.szsharing.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://ez.szsharing.cn

Go:   if x == nil {}
来源：http://tv.lnxyls.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://zf.muxihuayi.cn

C#:   if (x is null) {}
来源：http://sl.haigaiapp.cn

[P07] 防抖与节流
来源：http://jv.szsharing.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mx.szsharing.cn

PHP:  // 手写时间戳比较
来源：http://dm.nszjky.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qn.szsharing.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.shxzskj.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://is.chemitech.net.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://om.gzmigu.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://xr.yuntaijiaju.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://sm.shxzskj.cn

[P08] 处理浮点精度问题
来源：http://ms.szxytkj.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://gn.wgjwhj.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://gw.bjjhwx.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ek.jianghongdianzi.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://av.yuexingan06.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://eu.muxihuayi.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://es.9csxet.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://gc.szxytkj.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ox.bookmarksfly.cn

================================================================================
来源：http://ka.nszjky.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://qe.shxzukj.cn

================================================================================
来源：http://dh.bjjhwx.cn

[Q01] 创建表
来源：http://bn.jctech888.com.cn

CREATE TABLE users (
来源：http://rc.yuexingan06.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://sq.gzmigu.cn

name VARCHAR(50) NOT NULL,
来源：http://le.muxihuayi.cn

email VARCHAR(100) UNIQUE,
来源：http://ab.nicolike.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ez.jianghongdianzi.cn

);
来源：http://kr.szsharing.cn

[Q02] 创建带外键的表
来源：http://fu.wgjwhj.cn

CREATE TABLE orders (
来源：http://am.szxytkj.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ew.yuexingan06.cn

user_id INT NOT NULL,
来源：http://hm.newstarts.cn

amount DECIMAL(10, 2),
来源：http://yn.shxzskj.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://cv.jctech888.com.cn

);
来源：http://fj.shtwfgs.cn

[Q03] 增加列
来源：http://kz.colortex.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://fd.bjjhwx.cn

[Q04] 修改列类型
来源：http://io.shxzukj.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wy.yuexingan06.cn

[Q05] 重命名列
来源：http://hl.bookmarksfly.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://zs.521024.cn

[Q06] 删除列
来源：http://ke.panjiajie.cn

ALTER TABLE users DROP COLUMN age;
来源：http://ga.yuexingan06.cn

[Q07] 删除表
来源：http://zf.shtwfgs.cn

DROP TABLE IF EXISTS orders;
来源：http://vu.huixiangedu.cn

[Q08] 创建普通索引
来源：http://fq.bjjhwx.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://kv.shxzskj.cn

[Q09] 创建唯一索引
来源：http://dj.wgjwhj.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://gl.panjiajie.cn

[Q10] 插入单行
来源：http://yc.gzmigu.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://zs.jianghongdianzi.cn

[Q11] 一次插入多行
来源：http://vl.panjiajie.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://xc.szsharing.cn

[Q12] 插入后取自增 ID
来源：http://qu.hahajie.cn

INSERT INTO users (name) VALUES ('C');
来源：http://ve.521024.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://lb.lnxyls.cn

[Q13] 忽略重复插入
来源：http://jl.huixiangedu.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://rg.shxzskj.cn

[Q14] 存在则更新（upsert）
来源：http://gh.yuntaijiaju.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://sq.jctech888.com.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://aa.nszjky.cn

[Q15] 查询全部
来源：http://pe.wgjwhj.cn

SELECT * FROM users;
来源：http://sm.wgjwhj.cn

[Q16] 查询指定列
来源：http://bf.nicolike.cn

SELECT id, name FROM users;
来源：http://fq.huixiangedu.cn

[Q17] 条件查询
来源：http://xy.panjiajie.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ht.lnxyls.cn

[Q18] 模糊匹配
来源：http://be.huixiangedu.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ln.yuexingan06.cn

[Q19] 范围查询
来源：http://ch.lnxyls.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://in.9csxet.cn

[Q20] IN 列表
来源：http://bj.muxihuayi.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://nc.shxzskj.cn

[Q21] 空值判断
来源：http://zg.newstarts.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://mk.szsharing.cn

[Q22] 排序
来源：http://gp.huixiangedu.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://nw.chemitech.net.cn

[Q23] 分页
来源：http://jm.bookmarksfly.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ej.newstarts.cn

[Q24] 去重
来源：http://bz.huanxung.cn

SELECT DISTINCT city FROM users;
来源：http://gx.521024.cn

[Q25] 只取前 N 条
来源：http://tp.hnjuh.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://tv.newstarts.cn

[Q26] 计数
来源：http://or.szxytkj.cn

SELECT COUNT(*) FROM users;
来源：http://kd.wgjwhj.cn

[Q27] 条件计数
来源：http://gc.huixiangedu.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ei.colortex.cn

[Q28] 求和与平均
来源：http://ln.lnxyls.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://ne.bookmarksfly.cn

[Q29] 最大最小值
来源：http://ap.szsharing.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://qw.haigaiapp.cn

[Q30] 分组统计
来源：http://yc.wgjwhj.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://or.jianghongdianzi.cn

[Q31] 分组后过滤
来源：http://ux.panjiajie.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ev.521024.cn

[Q32] 分组拼接字符串
来源：http://vg.huixiangedu.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hv.gzmigu.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://vp.shxzukj.cn

[Q33] 多列分组
来源：http://vp.jctech888.com.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://uu.jctech888.com.cn

[Q34] 每组取第一条
来源：http://zg.jianghongdianzi.cn

SELECT * FROM (
来源：http://bm.yuntaijiaju.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wh.chemitech.net.cn

) t WHERE rn = 1;
来源：http://wp.nszjky.cn

[Q35] 内连接
来源：http://qa.shxzskj.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://cw.muxihuayi.cn

[Q36] 左连接
来源：http://kg.shxzukj.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://fo.haigaiapp.cn

[Q37] 右连接
来源：http://cn.shtwfgs.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.chemitech.net.cn

[Q38] 全外连接（PostgreSQL）
来源：http://jt.521024.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://yo.panjiajie.cn

[Q39] 自连接（查上下级）
来源：http://uf.nicolike.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://sj.huixinmuqiang.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ui.wgjwhj.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://pe.huixinmuqiang.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://rw.huanxung.cn

[Q41] 多表连接
来源：http://rr.shxzskj.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://do.jctech888.com.cn

JOIN users u ON u.id = o.user_id
来源：http://we.nszjky.cn

JOIN products p ON p.id = o.product_id;
来源：http://mm.shxzukj.cn

[Q42] 连接条件附加过滤
来源：http://uk.muxihuayi.cn

SELECT u.name, o.amount FROM users u
来源：http://tt.nicolike.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://vi.bookmarksfly.cn

[Q43] 标量子查询
来源：http://te.wgjwhj.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://zv.szsharing.cn

[Q44] IN 子查询
来源：http://mb.yuexingan06.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://bk.521024.cn

[Q45] EXISTS 判断存在
来源：http://dh.shxzskj.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://pq.jctech888.com.cn

[Q46] NOT EXISTS 判断不存在
来源：http://fw.szxytkj.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://zv.szxytkj.cn

[Q47] 与平均值比较
来源：http://ml.shxzukj.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://oi.jianghongdianzi.cn

[Q48] CTE 公用表表达式
来源：http://fg.asd995.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://fn.lnxyls.cn

SELECT * FROM t WHERE c > 5;
来源：http://dq.shxzukj.cn

[Q49] 更新单行
来源：http://eh.colortex.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://yy.wgjwhj.cn

[Q50] 批量更新
来源：http://ap.shxzskj.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://lt.huixinmuqiang.cn

[Q51] 用子查询更新
来源：http://mi.bjjhwx.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://ns.asd995.cn

[Q52] 删除指定行
来源：http://yo.bookmarksfly.cn

DELETE FROM users WHERE id = 10;
来源：http://rf.nicolike.cn

[Q53] 按条件删除
来源：http://oj.jctech888.com.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://zl.asd995.cn

[Q54] 清空表
来源：http://ah.hnjuh.cn

TRUNCATE TABLE logs;
来源：http://bb.shxzskj.cn

[Q55] 排名（并列占位）
来源：http://xq.hnjuh.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://qy.haigaiapp.cn

[Q56] 密集排名（并列不占位）
来源：http://hs.huixiangedu.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://fs.haigaiapp.cn

[Q57] 行号
来源：http://lh.hahajie.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://kw.bookmarksfly.cn

[Q58] 累计求和
来源：http://tn.panjiajie.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ry.yuntaijiaju.cn

[Q59] 分组内累计
来源：http://xb.yuexingan06.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://zy.jctech888.com.cn

[Q60] 取上一行 / 下一行
来源：http://se.szsharing.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ml.huixiangedu.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wt.huanxung.cn

[Q61] 移动平均
来源：http://yo.shxzskj.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://jc.panjiajie.cn

[Q62] 分组占比
来源：http://fe.haigaiapp.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mr.yuexingan06.cn

[Q63] 开启事务
来源：http://bg.szsharing.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://ko.lnxyls.cn

[Q64] 提交事务
来源：http://nr.colortex.cn

COMMIT;
来源：http://xa.shtwfgs.cn

[Q65] 回滚事务
来源：http://od.bookmarksfly.cn

ROLLBACK;
来源：http://cr.lnxyls.cn

[Q66] 行锁查询
来源：http://hc.huixiangedu.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://iz.hnjuh.cn

[Q67] 设置隔离级别
来源：http://so.shxzukj.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://zj.lnxyls.cn

[Q68] 保存点
来源：http://vh.shxzukj.cn

SAVEPOINT sp1;
来源：http://ck.newstarts.cn

ROLLBACK TO sp1;
来源：http://eo.panjiajie.cn

[Q69] 查看执行计划
来源：http://jt.yuexingan06.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wa.jctech888.com.cn

[Q70] 更新统计信息
来源：http://en.bookmarksfly.cn

ANALYZE TABLE users;
来源：http://ha.yuntaijiaju.cn

[Q71] 查看建表语句
来源：http://zd.hahajie.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ta.chemitech.net.cn

[Q72] 查看索引
来源：http://bf.shxzukj.cn

SHOW INDEX FROM users;
来源：http://tx.muxihuayi.cn

[Q73] 查看表状态
来源：http://nb.nicolike.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://aq.wgjwhj.cn

[Q74] 强制使用索引
来源：http://nz.asd995.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://vt.szsharing.cn

[Q75] 日期格式化
来源：http://ld.hahajie.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://qz.yuntaijiaju.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wg.haigaiapp.cn

[Q76] 按天统计
来源：http://jr.bjjhwx.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://qh.shxzskj.cn

[Q77] 时间加减
来源：http://no.huixiangedu.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://qa.muxihuayi.cn

[Q78] 当前时间
来源：http://ul.hahajie.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ao.hahajie.cn

[Q79] 字符串拼接
来源：http://vi.huanxung.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://qp.jctech888.com.cn

[Q80] 字符串截取
来源：http://ps.huixinmuqiang.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://cm.newstarts.cn

[Q81] 字符串替换
来源：http://au.panjiajie.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://bh.jianghongdianzi.cn

[Q82] 字符长度与字节长度
来源：http://tb.shxzukj.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ip.szxytkj.cn

[Q83] 大小写转换
来源：http://uc.bjjhwx.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://uh.gzmigu.cn

[Q84] 去除首尾空格
来源：http://hv.szxytkj.cn

SELECT TRIM(name) FROM users;
来源：http://xk.haigaiapp.cn

[Q85] 数值取整
来源：http://lb.bjjhwx.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ki.gzmigu.cn

[Q86] 读取 JSON 字段
来源：http://kz.9csxet.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://zw.yuexingan06.cn

[Q87] JSON 字段做条件
来源：http://dr.521024.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ee.9csxet.cn

[Q88] 行转列（条件聚合）
来源：http://cl.yuntaijiaju.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://nj.huixinmuqiang.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://du.jctech888.com.cn

[Q89] 判断表是否存在
来源：http://iy.panjiajie.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ek.bjjhwx.cn

[Q90] 生成序号列
来源：http://ki.huixinmuqiang.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://vr.shxzskj.cn

================================================================================
来源：http://pm.lnxyls.cn

R. Bash 专题
来源：http://tl.shxzskj.cn

================================================================================
来源：http://ls.asd995.cn

[R01] shebang 与严格模式
来源：http://ka.yuntaijiaju.cn

#!/usr/bin/env bash
来源：http://ym.nszjky.cn

set -euo pipefail
来源：http://lu.szsharing.cn

[R02] 变量赋值与使用
来源：http://gx.nszjky.cn

name="Tom"; echo "$name"
来源：http://ap.yuntaijiaju.cn

[R03] 只读变量
来源：http://qf.bjjhwx.cn

readonly PI=3.14
来源：http://vx.asd995.cn

[R04] 位置参数
来源：http://rv.shtwfgs.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://fa.huanxung.cn

[R05] 参数默认值
来源：http://ux.haigaiapp.cn

name="${1:-default}"
来源：http://uk.yuexingan06.cn

[R06] 判断命令是否存在
来源：http://tt.9csxet.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://vj.lnxyls.cn

[R07] if 判断文件
来源：http://sn.lnxyls.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://vf.jctech888.com.cn

[R08] 数值比较
来源：http://lm.huixinmuqiang.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://lx.jctech888.com.cn

[R09] 字符串比较
来源：http://ij.colortex.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://uf.hahajie.cn

[R10] 正则匹配
来源：http://vh.muxihuayi.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://fh.gzmigu.cn

[R11] case 多分支
来源：http://af.shxzukj.cn

case "$1" in
来源：http://hw.9csxet.cn

start) echo "启动" ;;
来源：http://pf.nicolike.cn

stop)  echo "停止" ;;
来源：http://qw.nicolike.cn

*)     echo "未知命令" ;;
来源：http://at.yuexingan06.cn

esac
来源：http://qw.bookmarksfly.cn

[R12] for 遍历文件
来源：http://xu.shtwfgs.cn

for f in *.txt; do echo "$f"; done
来源：http://hl.yuexingan06.cn

[R13] for 计数循环
来源：http://xh.hahajie.cn

for i in {1..10}; do echo "$i"; done
来源：http://vd.jianghongdianzi.cn

[R14] C 风格 for
来源：http://ay.yuexingan06.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://yh.jianghongdianzi.cn

[R15] while 逐行读文件
来源：http://qy.lnxyls.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://sc.521024.cn

[R16] until 等待条件
来源：http://bt.jianghongdianzi.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://es.szxytkj.cn

[R17] 数组定义与取值
来源：http://tq.newstarts.cn

arr=(a b c); echo "${arr[0]}"
来源：http://xp.panjiajie.cn

[R18] 遍历数组
来源：http://na.bjjhwx.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hy.shtwfgs.cn

[R19] 数组长度
来源：http://pk.wgjwhj.cn

echo "${#arr[@]}"
来源：http://af.nszjky.cn

[R20] 关联数组（字典）
来源：http://mw.9csxet.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://dd.chemitech.net.cn

[R21] 字符串长度
来源：http://mi.panjiajie.cn

echo "${#s}"
来源：http://br.jctech888.com.cn

[R22] 截取子串
来源：http://ml.huanxung.cn

echo "${s:0:5}"
来源：http://vg.panjiajie.cn

[R23] 字符串替换
来源：http://sx.521024.cn


<!-- 参考信息 -->