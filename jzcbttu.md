代发 wailian999

Java: list.size();  map.size();  s.length()
来源：http://of.jianghongdianzi.cn

Go:   len(arr);  len(m)
来源：http://ec.nicolike.cn

Ruby: x.length;  x.size
来源：http://qq.nicolike.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://sb.hahajie.cn

[P05] 判断两个对象内容是否相等
来源：http://qo.gzmigu.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://tg.jianghongdianzi.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ng.colortex.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://xd.szsharing.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.bookmarksfly.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mz.huanxung.cn

Go:   reflect.DeepEqual(a, b)
来源：http://wa.shxzukj.cn

Ruby: a == b
来源：http://lp.shxzukj.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wx.521024.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://tj.jctech888.com.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://bw.nszjky.cn

PHP:  if (empty($x)) {}
来源：http://dq.jianghongdianzi.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://aj.panjiajie.cn

TS:   if (x == null) {}
来源：http://nu.bjjhwx.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://hw.hnjuh.cn

Go:   if x == nil {}
来源：http://ez.szsharing.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://st.lnxyls.cn

C#:   if (x is null) {}
来源：http://ty.asd995.cn

[P07] 防抖与节流
来源：http://lz.gzmigu.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://bb.gzmigu.cn

PHP:  // 手写时间戳比较
来源：http://ju.shtwfgs.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ji.colortex.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://lu.wgjwhj.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://nf.shxzukj.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://tr.shtwfgs.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://yw.szsharing.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://cd.chemitech.net.cn

[P08] 处理浮点精度问题
来源：http://nm.shxzskj.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://bj.jctech888.com.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://qk.shxzskj.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://md.shtwfgs.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://zo.nicolike.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://gu.yuntaijiaju.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://lz.wgjwhj.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://qk.9csxet.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://pk.szsharing.cn

================================================================================
来源：http://tp.jctech888.com.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://pn.bjjhwx.cn

================================================================================
来源：http://sj.hnjuh.cn

[Q01] 创建表
来源：http://gd.shxzskj.cn

CREATE TABLE users (
来源：http://ak.asd995.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://re.yuexingan06.cn

name VARCHAR(50) NOT NULL,
来源：http://fh.nszjky.cn

email VARCHAR(100) UNIQUE,
来源：http://md.gzmigu.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ey.huixinmuqiang.cn

);
来源：http://rl.shtwfgs.cn

[Q02] 创建带外键的表
来源：http://mg.9csxet.cn

CREATE TABLE orders (
来源：http://yp.lnxyls.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://st.muxihuayi.cn

user_id INT NOT NULL,
来源：http://ds.hnjuh.cn

amount DECIMAL(10, 2),
来源：http://yl.panjiajie.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://xc.szxytkj.cn

);
来源：http://qd.chemitech.net.cn

[Q03] 增加列
来源：http://fi.yuntaijiaju.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ty.colortex.cn

[Q04] 修改列类型
来源：http://xv.jctech888.com.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://qq.newstarts.cn

[Q05] 重命名列
来源：http://lz.521024.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mw.yuexingan06.cn

[Q06] 删除列
来源：http://ev.hnjuh.cn

ALTER TABLE users DROP COLUMN age;
来源：http://zl.szsharing.cn

[Q07] 删除表
来源：http://qd.colortex.cn

DROP TABLE IF EXISTS orders;
来源：http://eo.bookmarksfly.cn

[Q08] 创建普通索引
来源：http://nk.gzmigu.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://qg.haigaiapp.cn

[Q09] 创建唯一索引
来源：http://qo.gzmigu.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://eq.szxytkj.cn

[Q10] 插入单行
来源：http://jy.szxytkj.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://xb.huanxung.cn

[Q11] 一次插入多行
来源：http://sl.gzmigu.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://yp.yuexingan06.cn

[Q12] 插入后取自增 ID
来源：http://ll.shtwfgs.cn

INSERT INTO users (name) VALUES ('C');
来源：http://ne.jctech888.com.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://jh.shxzskj.cn

[Q13] 忽略重复插入
来源：http://fj.huanxung.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ct.shtwfgs.cn

[Q14] 存在则更新（upsert）
来源：http://sc.bjjhwx.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://rg.521024.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://bd.jianghongdianzi.cn

[Q15] 查询全部
来源：http://mx.nszjky.cn

SELECT * FROM users;
来源：http://kt.bookmarksfly.cn

[Q16] 查询指定列
来源：http://ba.huanxung.cn

SELECT id, name FROM users;
来源：http://oy.haigaiapp.cn

[Q17] 条件查询
来源：http://bd.jianghongdianzi.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://jr.gzmigu.cn

[Q18] 模糊匹配
来源：http://ip.colortex.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://gj.huixinmuqiang.cn

[Q19] 范围查询
来源：http://tc.bookmarksfly.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://de.chemitech.net.cn

[Q20] IN 列表
来源：http://tj.newstarts.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://zm.huanxung.cn

[Q21] 空值判断
来源：http://ws.muxihuayi.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://mt.jctech888.com.cn

[Q22] 排序
来源：http://aq.wgjwhj.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wo.hahajie.cn

[Q23] 分页
来源：http://ss.szsharing.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hg.huixiangedu.cn

[Q24] 去重
来源：http://nf.panjiajie.cn

SELECT DISTINCT city FROM users;
来源：http://yz.lnxyls.cn

[Q25] 只取前 N 条
来源：http://ax.huixiangedu.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ko.gzmigu.cn

[Q26] 计数
来源：http://hz.hahajie.cn

SELECT COUNT(*) FROM users;
来源：http://fy.lnxyls.cn

[Q27] 条件计数
来源：http://nd.nicolike.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://bf.shtwfgs.cn

[Q28] 求和与平均
来源：http://sc.shtwfgs.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://qd.gzmigu.cn

[Q29] 最大最小值
来源：http://ja.shxzukj.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://pp.colortex.cn

[Q30] 分组统计
来源：http://vy.gzmigu.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://cf.bookmarksfly.cn

[Q31] 分组后过滤
来源：http://xa.shxzskj.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://yy.bookmarksfly.cn

[Q32] 分组拼接字符串
来源：http://wy.asd995.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://og.huanxung.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ii.shxzukj.cn

[Q33] 多列分组
来源：http://yb.szsharing.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://jj.huanxung.cn

[Q34] 每组取第一条
来源：http://qh.521024.cn

SELECT * FROM (
来源：http://lv.gzmigu.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://fz.jianghongdianzi.cn

) t WHERE rn = 1;
来源：http://rw.panjiajie.cn

[Q35] 内连接
来源：http://yd.nszjky.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ev.wgjwhj.cn

[Q36] 左连接
来源：http://ze.nicolike.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ky.gzmigu.cn

[Q37] 右连接
来源：http://ak.9csxet.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://vg.hahajie.cn

[Q38] 全外连接（PostgreSQL）
来源：http://pk.bookmarksfly.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ou.huixiangedu.cn

[Q39] 自连接（查上下级）
来源：http://bh.lnxyls.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://jm.chemitech.net.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hk.chemitech.net.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://eg.szsharing.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://uu.muxihuayi.cn

[Q41] 多表连接
来源：http://px.asd995.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://or.shxzukj.cn

JOIN users u ON u.id = o.user_id
来源：http://xz.jctech888.com.cn

JOIN products p ON p.id = o.product_id;
来源：http://wv.jctech888.com.cn

[Q42] 连接条件附加过滤
来源：http://bt.asd995.cn

SELECT u.name, o.amount FROM users u
来源：http://bk.521024.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://xk.chemitech.net.cn

[Q43] 标量子查询
来源：http://uj.shtwfgs.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://nk.9csxet.cn

[Q44] IN 子查询
来源：http://tw.gzmigu.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ja.hahajie.cn

[Q45] EXISTS 判断存在
来源：http://vz.haigaiapp.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://au.huixinmuqiang.cn

[Q46] NOT EXISTS 判断不存在
来源：http://os.shtwfgs.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wn.huanxung.cn

[Q47] 与平均值比较
来源：http://wq.huixinmuqiang.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wq.panjiajie.cn

[Q48] CTE 公用表表达式
来源：http://ic.gzmigu.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://pf.hahajie.cn

SELECT * FROM t WHERE c > 5;
来源：http://id.gzmigu.cn

[Q49] 更新单行
来源：http://ty.nszjky.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://bf.hnjuh.cn

[Q50] 批量更新
来源：http://wa.jctech888.com.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://kz.panjiajie.cn

[Q51] 用子查询更新
来源：http://sw.huanxung.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://dy.newstarts.cn

[Q52] 删除指定行
来源：http://so.nicolike.cn

DELETE FROM users WHERE id = 10;
来源：http://eq.colortex.cn

[Q53] 按条件删除
来源：http://wt.bjjhwx.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://bv.shtwfgs.cn

[Q54] 清空表
来源：http://jp.jctech888.com.cn

TRUNCATE TABLE logs;
来源：http://ee.huixiangedu.cn

[Q55] 排名（并列占位）
来源：http://iv.nicolike.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ug.muxihuayi.cn

[Q56] 密集排名（并列不占位）
来源：http://oo.shtwfgs.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://pf.asd995.cn

[Q57] 行号
来源：http://bt.hnjuh.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://dd.yuntaijiaju.cn

[Q58] 累计求和
来源：http://fp.bjjhwx.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ej.9csxet.cn

[Q59] 分组内累计
来源：http://xd.bjjhwx.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://yx.521024.cn

[Q60] 取上一行 / 下一行
来源：http://zp.yuexingan06.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://it.asd995.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ym.bookmarksfly.cn

[Q61] 移动平均
来源：http://dj.szxytkj.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://al.panjiajie.cn

[Q62] 分组占比
来源：http://gi.jianghongdianzi.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://in.panjiajie.cn

[Q63] 开启事务
来源：http://lq.wgjwhj.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://io.bjjhwx.cn

[Q64] 提交事务
来源：http://rx.gzmigu.cn

COMMIT;
来源：http://fj.shxzskj.cn

[Q65] 回滚事务
来源：http://nb.nszjky.cn

ROLLBACK;
来源：http://pc.muxihuayi.cn

[Q66] 行锁查询
来源：http://tl.jctech888.com.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ly.nicolike.cn

[Q67] 设置隔离级别
来源：http://xq.yuntaijiaju.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://er.nicolike.cn

[Q68] 保存点
来源：http://sq.521024.cn

SAVEPOINT sp1;
来源：http://pd.haigaiapp.cn

ROLLBACK TO sp1;
来源：http://bp.lnxyls.cn

[Q69] 查看执行计划
来源：http://jf.colortex.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://by.colortex.cn

[Q70] 更新统计信息
来源：http://gr.huanxung.cn

ANALYZE TABLE users;
来源：http://lk.jctech888.com.cn

[Q71] 查看建表语句
来源：http://wx.haigaiapp.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ep.szsharing.cn

[Q72] 查看索引
来源：http://jj.hahajie.cn

SHOW INDEX FROM users;
来源：http://nh.gzmigu.cn

[Q73] 查看表状态
来源：http://zz.huixinmuqiang.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://ny.lnxyls.cn

[Q74] 强制使用索引
来源：http://va.colortex.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://rl.9csxet.cn

[Q75] 日期格式化
来源：http://bp.shxzukj.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://qh.shxzukj.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://yy.yuexingan06.cn

[Q76] 按天统计
来源：http://dj.szxytkj.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ve.shtwfgs.cn

[Q77] 时间加减
来源：http://cg.muxihuayi.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://pk.jianghongdianzi.cn

[Q78] 当前时间
来源：http://pd.yuexingan06.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ha.hnjuh.cn

[Q79] 字符串拼接
来源：http://fs.yuexingan06.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hq.jianghongdianzi.cn

[Q80] 字符串截取
来源：http://eq.jctech888.com.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://yt.shxzskj.cn

[Q81] 字符串替换
来源：http://st.lnxyls.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://eg.chemitech.net.cn

[Q82] 字符长度与字节长度
来源：http://lf.huixinmuqiang.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://cq.huixinmuqiang.cn

[Q83] 大小写转换
来源：http://mq.huixiangedu.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ph.huanxung.cn

[Q84] 去除首尾空格
来源：http://xg.huanxung.cn

SELECT TRIM(name) FROM users;
来源：http://og.bookmarksfly.cn

[Q85] 数值取整
来源：http://ep.shxzskj.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ko.jianghongdianzi.cn

[Q86] 读取 JSON 字段
来源：http://rb.lnxyls.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://jb.nszjky.cn

[Q87] JSON 字段做条件
来源：http://db.yuexingan06.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://gb.shtwfgs.cn

[Q88] 行转列（条件聚合）
来源：http://sf.wgjwhj.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://dk.hnjuh.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://gc.huixiangedu.cn

[Q89] 判断表是否存在
来源：http://bq.wgjwhj.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://rk.nicolike.cn

[Q90] 生成序号列
来源：http://xp.yuexingan06.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://fe.lnxyls.cn

================================================================================
来源：http://lq.bjjhwx.cn

R. Bash 专题
来源：http://ed.shxzskj.cn

================================================================================
来源：http://ad.haigaiapp.cn

[R01] shebang 与严格模式
来源：http://vy.chemitech.net.cn

#!/usr/bin/env bash
来源：http://nj.yuntaijiaju.cn

set -euo pipefail
来源：http://ih.newstarts.cn

[R02] 变量赋值与使用
来源：http://ol.9csxet.cn

name="Tom"; echo "$name"
来源：http://av.colortex.cn

[R03] 只读变量
来源：http://xd.muxihuayi.cn

readonly PI=3.14
来源：http://zr.shxzukj.cn

[R04] 位置参数
来源：http://ey.521024.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://as.yuexingan06.cn

[R05] 参数默认值
来源：http://vd.yuntaijiaju.cn

name="${1:-default}"
来源：http://bv.muxihuayi.cn

[R06] 判断命令是否存在
来源：http://fx.muxihuayi.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://cj.newstarts.cn

[R07] if 判断文件
来源：http://mv.jianghongdianzi.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://yu.shxzukj.cn

[R08] 数值比较
来源：http://fi.521024.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://bx.muxihuayi.cn

[R09] 字符串比较
来源：http://ph.9csxet.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://qd.yuntaijiaju.cn

[R10] 正则匹配
来源：http://qo.shtwfgs.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wc.shtwfgs.cn

[R11] case 多分支
来源：http://ng.lnxyls.cn

case "$1" in
来源：http://zo.shxzskj.cn

start) echo "启动" ;;
来源：http://xj.huixinmuqiang.cn

stop)  echo "停止" ;;
来源：http://kx.jianghongdianzi.cn

*)     echo "未知命令" ;;
来源：http://uu.haigaiapp.cn

esac
来源：http://ed.huixinmuqiang.cn

[R12] for 遍历文件
来源：http://yz.huixiangedu.cn

for f in *.txt; do echo "$f"; done
来源：http://wh.huixinmuqiang.cn

[R13] for 计数循环
来源：http://qr.shxzukj.cn

for i in {1..10}; do echo "$i"; done
来源：http://zk.muxihuayi.cn

[R14] C 风格 for
来源：http://fx.panjiajie.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://if.colortex.cn

[R15] while 逐行读文件
来源：http://il.wgjwhj.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://me.huixiangedu.cn

[R16] until 等待条件
来源：http://wm.asd995.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://if.bookmarksfly.cn

[R17] 数组定义与取值
来源：http://lm.nszjky.cn

arr=(a b c); echo "${arr[0]}"
来源：http://gl.hnjuh.cn

[R18] 遍历数组
来源：http://pm.szsharing.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://rw.lnxyls.cn

[R19] 数组长度
来源：http://de.yuntaijiaju.cn

echo "${#arr[@]}"
来源：http://ve.asd995.cn

[R20] 关联数组（字典）
来源：http://kq.muxihuayi.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://sy.bjjhwx.cn

[R21] 字符串长度
来源：http://ba.hnjuh.cn

echo "${#s}"
来源：http://dc.chemitech.net.cn

[R22] 截取子串
来源：http://kc.lnxyls.cn

echo "${s:0:5}"
来源：http://ml.bjjhwx.cn

[R23] 字符串替换
来源：http://js.chemitech.net.cn


<!-- 参考信息 -->