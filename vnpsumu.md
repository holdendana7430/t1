代发 wailian999

Java: list.size();  map.size();  s.length()
来源：http://ys.yuntaijiaju.cn

Go:   len(arr);  len(m)
来源：http://pe.shxzukj.cn

Ruby: x.length;  x.size
来源：http://ve.wgjwhj.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://pc.bookmarksfly.cn

[P05] 判断两个对象内容是否相等
来源：http://tg.jianghongdianzi.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://zs.nicolike.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://dj.jianghongdianzi.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://zf.hnjuh.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hq.gzmigu.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://pq.yuntaijiaju.cn

Go:   reflect.DeepEqual(a, b)
来源：http://pw.521024.cn

Ruby: a == b
来源：http://rg.yuexingan06.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://zb.yuntaijiaju.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://kl.asd995.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://sk.chemitech.net.cn

PHP:  if (empty($x)) {}
来源：http://nv.asd995.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://vs.muxihuayi.cn

TS:   if (x == null) {}
来源：http://zq.szxytkj.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://dk.yuexingan06.cn

Go:   if x == nil {}
来源：http://te.lnxyls.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://bc.nszjky.cn

C#:   if (x is null) {}
来源：http://iz.haigaiapp.cn

[P07] 防抖与节流
来源：http://bq.shxzskj.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://fz.9csxet.cn

PHP:  // 手写时间戳比较
来源：http://wh.huixinmuqiang.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qf.lnxyls.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://nh.szxytkj.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ej.521024.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://zn.gzmigu.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://so.huixinmuqiang.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://sd.huixinmuqiang.cn

[P08] 处理浮点精度问题
来源：http://qt.huixinmuqiang.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ez.yuntaijiaju.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://qt.asd995.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://gc.huanxung.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://dj.yuntaijiaju.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://lx.panjiajie.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://qj.jctech888.com.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://in.chemitech.net.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://cr.asd995.cn

================================================================================
来源：http://jz.bjjhwx.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://qq.yuexingan06.cn

================================================================================
来源：http://wb.nszjky.cn

[Q01] 创建表
来源：http://vp.shxzskj.cn

CREATE TABLE users (
来源：http://fi.huixiangedu.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://sv.colortex.cn

name VARCHAR(50) NOT NULL,
来源：http://gu.jianghongdianzi.cn

email VARCHAR(100) UNIQUE,
来源：http://gc.colortex.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://pg.lnxyls.cn

);
来源：http://im.bjjhwx.cn

[Q02] 创建带外键的表
来源：http://bs.jctech888.com.cn

CREATE TABLE orders (
来源：http://so.muxihuayi.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://bl.bjjhwx.cn

user_id INT NOT NULL,
来源：http://ch.newstarts.cn

amount DECIMAL(10, 2),
来源：http://pq.panjiajie.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ys.colortex.cn

);
来源：http://sv.hahajie.cn

[Q03] 增加列
来源：http://yh.hahajie.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ck.colortex.cn

[Q04] 修改列类型
来源：http://hr.nicolike.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://dn.haigaiapp.cn

[Q05] 重命名列
来源：http://tn.chemitech.net.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://lv.hahajie.cn

[Q06] 删除列
来源：http://eo.yuntaijiaju.cn

ALTER TABLE users DROP COLUMN age;
来源：http://ln.asd995.cn

[Q07] 删除表
来源：http://sm.huixiangedu.cn

DROP TABLE IF EXISTS orders;
来源：http://hq.hahajie.cn

[Q08] 创建普通索引
来源：http://ou.colortex.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://xk.yuntaijiaju.cn

[Q09] 创建唯一索引
来源：http://ur.szsharing.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://yq.wgjwhj.cn

[Q10] 插入单行
来源：http://qf.shxzskj.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://vi.muxihuayi.cn

[Q11] 一次插入多行
来源：http://yj.bookmarksfly.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://nj.szsharing.cn

[Q12] 插入后取自增 ID
来源：http://na.huanxung.cn

INSERT INTO users (name) VALUES ('C');
来源：http://vl.huixiangedu.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://jl.bookmarksfly.cn

[Q13] 忽略重复插入
来源：http://sr.huanxung.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://xw.szsharing.cn

[Q14] 存在则更新（upsert）
来源：http://wb.shxzukj.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://md.lnxyls.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://io.jianghongdianzi.cn

[Q15] 查询全部
来源：http://he.newstarts.cn

SELECT * FROM users;
来源：http://sj.shtwfgs.cn

[Q16] 查询指定列
来源：http://tj.shtwfgs.cn

SELECT id, name FROM users;
来源：http://jt.9csxet.cn

[Q17] 条件查询
来源：http://sw.bjjhwx.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://oz.nszjky.cn

[Q18] 模糊匹配
来源：http://hb.asd995.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://kt.9csxet.cn

[Q19] 范围查询
来源：http://xg.bookmarksfly.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://tn.asd995.cn

[Q20] IN 列表
来源：http://fx.wgjwhj.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ks.muxihuayi.cn

[Q21] 空值判断
来源：http://on.nicolike.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://zr.bookmarksfly.cn

[Q22] 排序
来源：http://gm.haigaiapp.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://yk.panjiajie.cn

[Q23] 分页
来源：http://ll.shtwfgs.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://il.muxihuayi.cn

[Q24] 去重
来源：http://oj.nszjky.cn

SELECT DISTINCT city FROM users;
来源：http://jy.9csxet.cn

[Q25] 只取前 N 条
来源：http://yk.muxihuayi.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ox.yuexingan06.cn

[Q26] 计数
来源：http://nw.bookmarksfly.cn

SELECT COUNT(*) FROM users;
来源：http://rq.hnjuh.cn

[Q27] 条件计数
来源：http://vx.jctech888.com.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://el.hnjuh.cn

[Q28] 求和与平均
来源：http://kl.newstarts.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://tp.colortex.cn

[Q29] 最大最小值
来源：http://ud.shxzskj.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://oz.chemitech.net.cn

[Q30] 分组统计
来源：http://xg.asd995.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://va.haigaiapp.cn

[Q31] 分组后过滤
来源：http://th.shxzskj.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://rh.521024.cn

[Q32] 分组拼接字符串
来源：http://jx.asd995.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://yz.hahajie.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://rg.panjiajie.cn

[Q33] 多列分组
来源：http://mc.hnjuh.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ro.jianghongdianzi.cn

[Q34] 每组取第一条
来源：http://yn.9csxet.cn

SELECT * FROM (
来源：http://zt.newstarts.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://im.yuntaijiaju.cn

) t WHERE rn = 1;
来源：http://am.shxzukj.cn

[Q35] 内连接
来源：http://xf.huixinmuqiang.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://qr.huixinmuqiang.cn

[Q36] 左连接
来源：http://gk.bjjhwx.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://sr.wgjwhj.cn

[Q37] 右连接
来源：http://gq.huixiangedu.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://xh.shtwfgs.cn

[Q38] 全外连接（PostgreSQL）
来源：http://dz.521024.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ou.jctech888.com.cn

[Q39] 自连接（查上下级）
来源：http://ic.lnxyls.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://zz.hahajie.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ff.bjjhwx.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://lj.muxihuayi.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://jm.hahajie.cn

[Q41] 多表连接
来源：http://oi.huixinmuqiang.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://pv.nszjky.cn

JOIN users u ON u.id = o.user_id
来源：http://tx.asd995.cn

JOIN products p ON p.id = o.product_id;
来源：http://ll.yuntaijiaju.cn

[Q42] 连接条件附加过滤
来源：http://gv.shxzskj.cn

SELECT u.name, o.amount FROM users u
来源：http://km.muxihuayi.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ks.muxihuayi.cn

[Q43] 标量子查询
来源：http://kt.szsharing.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://kv.shtwfgs.cn

[Q44] IN 子查询
来源：http://us.jctech888.com.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://vd.muxihuayi.cn

[Q45] EXISTS 判断存在
来源：http://dp.9csxet.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://tz.shxzskj.cn

[Q46] NOT EXISTS 判断不存在
来源：http://fp.lnxyls.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ti.szsharing.cn

[Q47] 与平均值比较
来源：http://jx.shxzskj.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://tb.huanxung.cn

[Q48] CTE 公用表表达式
来源：http://kh.newstarts.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://rr.nicolike.cn

SELECT * FROM t WHERE c > 5;
来源：http://us.9csxet.cn

[Q49] 更新单行
来源：http://zc.jctech888.com.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ag.huixinmuqiang.cn

[Q50] 批量更新
来源：http://vk.shxzukj.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://gi.shtwfgs.cn

[Q51] 用子查询更新
来源：http://vq.bookmarksfly.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://qg.newstarts.cn

[Q52] 删除指定行
来源：http://tg.chemitech.net.cn

DELETE FROM users WHERE id = 10;
来源：http://fn.nszjky.cn

[Q53] 按条件删除
来源：http://vp.jctech888.com.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ir.wgjwhj.cn

[Q54] 清空表
来源：http://cn.colortex.cn

TRUNCATE TABLE logs;
来源：http://hr.yuntaijiaju.cn

[Q55] 排名（并列占位）
来源：http://to.lnxyls.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ou.asd995.cn

[Q56] 密集排名（并列不占位）
来源：http://cc.nicolike.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://sf.haigaiapp.cn

[Q57] 行号
来源：http://mr.yuntaijiaju.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://lt.gzmigu.cn

[Q58] 累计求和
来源：http://qt.shxzskj.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ky.huixinmuqiang.cn

[Q59] 分组内累计
来源：http://tm.wgjwhj.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ri.yuexingan06.cn

[Q60] 取上一行 / 下一行
来源：http://km.bookmarksfly.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ah.nicolike.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://md.szxytkj.cn

[Q61] 移动平均
来源：http://kl.jianghongdianzi.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://nc.muxihuayi.cn

[Q62] 分组占比
来源：http://vg.hahajie.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://vo.gzmigu.cn

[Q63] 开启事务
来源：http://vf.szxytkj.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://ui.muxihuayi.cn

[Q64] 提交事务
来源：http://oe.chemitech.net.cn

COMMIT;
来源：http://xu.huixinmuqiang.cn

[Q65] 回滚事务
来源：http://bo.huixiangedu.cn

ROLLBACK;
来源：http://ci.shxzukj.cn

[Q66] 行锁查询
来源：http://lx.nicolike.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://jy.wgjwhj.cn

[Q67] 设置隔离级别
来源：http://yl.szxytkj.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://jv.9csxet.cn

[Q68] 保存点
来源：http://ba.szxytkj.cn

SAVEPOINT sp1;
来源：http://vo.hnjuh.cn

ROLLBACK TO sp1;
来源：http://yc.521024.cn

[Q69] 查看执行计划
来源：http://la.panjiajie.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hp.nszjky.cn

[Q70] 更新统计信息
来源：http://dk.wgjwhj.cn

ANALYZE TABLE users;
来源：http://pj.shxzukj.cn

[Q71] 查看建表语句
来源：http://hz.jctech888.com.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://yo.shxzskj.cn

[Q72] 查看索引
来源：http://ty.szxytkj.cn

SHOW INDEX FROM users;
来源：http://kc.yuntaijiaju.cn

[Q73] 查看表状态
来源：http://ur.bjjhwx.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://ud.jianghongdianzi.cn

[Q74] 强制使用索引
来源：http://jj.huanxung.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://gs.gzmigu.cn

[Q75] 日期格式化
来源：http://rx.asd995.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://bz.panjiajie.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://dw.wgjwhj.cn

[Q76] 按天统计
来源：http://gm.asd995.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hg.huixinmuqiang.cn

[Q77] 时间加减
来源：http://et.wgjwhj.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://sd.lnxyls.cn

[Q78] 当前时间
来源：http://cb.hahajie.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://jo.521024.cn

[Q79] 字符串拼接
来源：http://si.hahajie.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://qc.521024.cn

[Q80] 字符串截取
来源：http://ul.gzmigu.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://eg.hahajie.cn

[Q81] 字符串替换
来源：http://cf.bookmarksfly.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://lw.shtwfgs.cn

[Q82] 字符长度与字节长度
来源：http://so.521024.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://xm.shtwfgs.cn

[Q83] 大小写转换
来源：http://ao.shxzukj.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://rc.gzmigu.cn

[Q84] 去除首尾空格
来源：http://nz.yuexingan06.cn

SELECT TRIM(name) FROM users;
来源：http://wr.haigaiapp.cn

[Q85] 数值取整
来源：http://uv.521024.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://yl.szsharing.cn

[Q86] 读取 JSON 字段
来源：http://sj.szsharing.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wi.huixiangedu.cn

[Q87] JSON 字段做条件
来源：http://bg.newstarts.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://qw.wgjwhj.cn

[Q88] 行转列（条件聚合）
来源：http://wo.yuexingan06.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://bb.haigaiapp.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://fl.shxzukj.cn

[Q89] 判断表是否存在
来源：http://lb.muxihuayi.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://zx.bookmarksfly.cn

[Q90] 生成序号列
来源：http://xn.asd995.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://av.asd995.cn

================================================================================
来源：http://hn.huixinmuqiang.cn

R. Bash 专题
来源：http://xk.yuntaijiaju.cn

================================================================================
来源：http://mw.nicolike.cn

[R01] shebang 与严格模式
来源：http://xa.hnjuh.cn

#!/usr/bin/env bash
来源：http://px.muxihuayi.cn

set -euo pipefail
来源：http://wq.9csxet.cn

[R02] 变量赋值与使用
来源：http://of.muxihuayi.cn

name="Tom"; echo "$name"
来源：http://yt.jctech888.com.cn

[R03] 只读变量
来源：http://fa.haigaiapp.cn

readonly PI=3.14
来源：http://vr.huixiangedu.cn

[R04] 位置参数
来源：http://si.521024.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://qb.huixinmuqiang.cn

[R05] 参数默认值
来源：http://nx.yuexingan06.cn

name="${1:-default}"
来源：http://dm.huixinmuqiang.cn

[R06] 判断命令是否存在
来源：http://kx.bookmarksfly.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://qj.szxytkj.cn

[R07] if 判断文件
来源：http://hj.gzmigu.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ql.lnxyls.cn

[R08] 数值比较
来源：http://ir.huixinmuqiang.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://lw.lnxyls.cn

[R09] 字符串比较
来源：http://dt.gzmigu.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://vg.chemitech.net.cn

[R10] 正则匹配
来源：http://dt.gzmigu.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://qj.huixiangedu.cn

[R11] case 多分支
来源：http://ne.9csxet.cn

case "$1" in
来源：http://ol.lnxyls.cn

start) echo "启动" ;;
来源：http://bt.panjiajie.cn

stop)  echo "停止" ;;
来源：http://es.jianghongdianzi.cn

*)     echo "未知命令" ;;
来源：http://pn.yuntaijiaju.cn

esac
来源：http://sr.newstarts.cn

[R12] for 遍历文件
来源：http://oa.yuntaijiaju.cn

for f in *.txt; do echo "$f"; done
来源：http://nc.9csxet.cn

[R13] for 计数循环
来源：http://nf.yuexingan06.cn

for i in {1..10}; do echo "$i"; done
来源：http://is.nicolike.cn

[R14] C 风格 for
来源：http://is.newstarts.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://pt.panjiajie.cn

[R15] while 逐行读文件
来源：http://sm.hnjuh.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://cl.chemitech.net.cn

[R16] until 等待条件
来源：http://bf.colortex.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wl.hahajie.cn

[R17] 数组定义与取值
来源：http://xg.panjiajie.cn

arr=(a b c); echo "${arr[0]}"
来源：http://fh.hnjuh.cn

[R18] 遍历数组
来源：http://km.shtwfgs.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://du.jianghongdianzi.cn

[R19] 数组长度
来源：http://tj.shxzukj.cn

echo "${#arr[@]}"
来源：http://lo.bjjhwx.cn

[R20] 关联数组（字典）
来源：http://ek.chemitech.net.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://er.wgjwhj.cn

[R21] 字符串长度
来源：http://hb.huixinmuqiang.cn

echo "${#s}"
来源：http://ee.szsharing.cn

[R22] 截取子串
来源：http://dj.wgjwhj.cn

echo "${s:0:5}"
来源：http://gi.haigaiapp.cn

[R23] 字符串替换
来源：http://me.shxzskj.cn


<!-- 参考信息 -->