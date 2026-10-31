代发 wailian999

Py:   len(x)            # 字符串、列表、字典通用
来源：http://sl.jctech888.com.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ql.521024.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ou.yuexingan06.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://dt.shxzukj.cn

Java: list.size();  map.size();  s.length()
来源：http://jl.hahajie.cn

Go:   len(arr);  len(m)
来源：http://da.chemitech.net.cn

Ruby: x.length;  x.size
来源：http://vu.521024.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://fo.asd995.cn

[P05] 判断两个对象内容是否相等
来源：http://nz.haigaiapp.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://ds.521024.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://rv.yuexingan06.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://bo.521024.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hf.asd995.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://rh.huixiangedu.cn

Go:   reflect.DeepEqual(a, b)
来源：http://sc.521024.cn

Ruby: a == b
来源：http://vw.gzmigu.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://nz.shtwfgs.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://qj.muxihuayi.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://iq.muxihuayi.cn

PHP:  if (empty($x)) {}
来源：http://em.muxihuayi.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://gh.huixiangedu.cn

TS:   if (x == null) {}
来源：http://om.hahajie.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://lo.muxihuayi.cn

Go:   if x == nil {}
来源：http://ab.nszjky.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://yv.muxihuayi.cn

C#:   if (x is null) {}
来源：http://to.huixinmuqiang.cn

[P07] 防抖与节流
来源：http://ic.lnxyls.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://dl.shxzskj.cn

PHP:  // 手写时间戳比较
来源：http://nh.huixiangedu.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ha.panjiajie.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ld.colortex.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ys.muxihuayi.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://id.nicolike.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://jn.yuexingan06.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ov.muxihuayi.cn

[P08] 处理浮点精度问题
来源：http://zh.bookmarksfly.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://aj.asd995.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://xr.huixinmuqiang.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://jj.colortex.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://vm.wgjwhj.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://vb.haigaiapp.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://sn.nicolike.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://yr.shxzukj.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://jq.asd995.cn

================================================================================
来源：http://aq.huixiangedu.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ew.521024.cn

================================================================================
来源：http://au.wgjwhj.cn

[Q01] 创建表
来源：http://lv.yuexingan06.cn

CREATE TABLE users (
来源：http://pc.huixiangedu.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://vp.521024.cn

name VARCHAR(50) NOT NULL,
来源：http://jo.hnjuh.cn

email VARCHAR(100) UNIQUE,
来源：http://sp.nicolike.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://rk.nszjky.cn

);
来源：http://kj.muxihuayi.cn

[Q02] 创建带外键的表
来源：http://hi.panjiajie.cn

CREATE TABLE orders (
来源：http://au.hahajie.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://kt.9csxet.cn

user_id INT NOT NULL,
来源：http://tu.hnjuh.cn

amount DECIMAL(10, 2),
来源：http://xi.gzmigu.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ja.nszjky.cn

);
来源：http://fv.panjiajie.cn

[Q03] 增加列
来源：http://le.huanxung.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://yr.huixinmuqiang.cn

[Q04] 修改列类型
来源：http://hr.huanxung.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://pr.jianghongdianzi.cn

[Q05] 重命名列
来源：http://ng.yuntaijiaju.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ns.nicolike.cn

[Q06] 删除列
来源：http://ez.panjiajie.cn

ALTER TABLE users DROP COLUMN age;
来源：http://du.asd995.cn

[Q07] 删除表
来源：http://er.shxzskj.cn

DROP TABLE IF EXISTS orders;
来源：http://cz.huanxung.cn

[Q08] 创建普通索引
来源：http://bo.521024.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://nn.shxzskj.cn

[Q09] 创建唯一索引
来源：http://wc.gzmigu.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://qa.wgjwhj.cn

[Q10] 插入单行
来源：http://ph.huanxung.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://tw.huixiangedu.cn

[Q11] 一次插入多行
来源：http://gd.nicolike.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://no.521024.cn

[Q12] 插入后取自增 ID
来源：http://vu.shtwfgs.cn

INSERT INTO users (name) VALUES ('C');
来源：http://jo.wgjwhj.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ma.lnxyls.cn

[Q13] 忽略重复插入
来源：http://wk.shxzukj.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://iq.hnjuh.cn

[Q14] 存在则更新（upsert）
来源：http://cv.newstarts.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://tl.asd995.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://dt.lnxyls.cn

[Q15] 查询全部
来源：http://aa.shxzskj.cn

SELECT * FROM users;
来源：http://nd.yuexingan06.cn

[Q16] 查询指定列
来源：http://tj.yuntaijiaju.cn

SELECT id, name FROM users;
来源：http://qk.lnxyls.cn

[Q17] 条件查询
来源：http://zo.jianghongdianzi.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://lg.jianghongdianzi.cn

[Q18] 模糊匹配
来源：http://dx.szsharing.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://du.huixiangedu.cn

[Q19] 范围查询
来源：http://ks.panjiajie.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://vn.lnxyls.cn

[Q20] IN 列表
来源：http://xy.lnxyls.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wh.bookmarksfly.cn

[Q21] 空值判断
来源：http://il.bjjhwx.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://as.bookmarksfly.cn

[Q22] 排序
来源：http://tf.huanxung.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://dh.yuexingan06.cn

[Q23] 分页
来源：http://ya.huanxung.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ij.shxzukj.cn

[Q24] 去重
来源：http://qy.newstarts.cn

SELECT DISTINCT city FROM users;
来源：http://qi.huanxung.cn

[Q25] 只取前 N 条
来源：http://wx.chemitech.net.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://sd.shtwfgs.cn

[Q26] 计数
来源：http://en.newstarts.cn

SELECT COUNT(*) FROM users;
来源：http://oj.hnjuh.cn

[Q27] 条件计数
来源：http://oh.huixiangedu.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://fj.521024.cn

[Q28] 求和与平均
来源：http://nd.lnxyls.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://xc.shtwfgs.cn

[Q29] 最大最小值
来源：http://jb.521024.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://rl.yuexingan06.cn

[Q30] 分组统计
来源：http://jg.haigaiapp.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://sr.colortex.cn

[Q31] 分组后过滤
来源：http://dv.szsharing.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://zw.9csxet.cn

[Q32] 分组拼接字符串
来源：http://xs.chemitech.net.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://vs.haigaiapp.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ch.lnxyls.cn

[Q33] 多列分组
来源：http://qm.huixiangedu.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ds.huanxung.cn

[Q34] 每组取第一条
来源：http://hn.huanxung.cn

SELECT * FROM (
来源：http://db.szxytkj.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://tg.muxihuayi.cn

) t WHERE rn = 1;
来源：http://wf.yuntaijiaju.cn

[Q35] 内连接
来源：http://ca.chemitech.net.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://go.colortex.cn

[Q36] 左连接
来源：http://vc.szsharing.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://jm.bookmarksfly.cn

[Q37] 右连接
来源：http://pb.bookmarksfly.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://dx.jianghongdianzi.cn

[Q38] 全外连接（PostgreSQL）
来源：http://xi.huixinmuqiang.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://to.panjiajie.cn

[Q39] 自连接（查上下级）
来源：http://pw.wgjwhj.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://vb.nicolike.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://zu.szxytkj.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://hd.wgjwhj.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://lo.9csxet.cn

[Q41] 多表连接
来源：http://oo.yuntaijiaju.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://rs.szxytkj.cn

JOIN users u ON u.id = o.user_id
来源：http://xg.hnjuh.cn

JOIN products p ON p.id = o.product_id;
来源：http://yz.shtwfgs.cn

[Q42] 连接条件附加过滤
来源：http://rt.nszjky.cn

SELECT u.name, o.amount FROM users u
来源：http://wr.szsharing.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ji.bookmarksfly.cn

[Q43] 标量子查询
来源：http://oe.gzmigu.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://nx.shxzukj.cn

[Q44] IN 子查询
来源：http://ye.nicolike.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://lr.newstarts.cn

[Q45] EXISTS 判断存在
来源：http://dk.szxytkj.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mp.panjiajie.cn

[Q46] NOT EXISTS 判断不存在
来源：http://ht.521024.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://eo.hnjuh.cn

[Q47] 与平均值比较
来源：http://on.gzmigu.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hp.jianghongdianzi.cn

[Q48] CTE 公用表表达式
来源：http://hu.panjiajie.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hn.huixiangedu.cn

SELECT * FROM t WHERE c > 5;
来源：http://hk.shtwfgs.cn

[Q49] 更新单行
来源：http://ox.huanxung.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ur.panjiajie.cn

[Q50] 批量更新
来源：http://vh.hnjuh.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wa.panjiajie.cn

[Q51] 用子查询更新
来源：http://up.wgjwhj.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://xf.lnxyls.cn

[Q52] 删除指定行
来源：http://pw.hahajie.cn

DELETE FROM users WHERE id = 10;
来源：http://nf.haigaiapp.cn

[Q53] 按条件删除
来源：http://bs.jianghongdianzi.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://id.huixiangedu.cn

[Q54] 清空表
来源：http://fc.chemitech.net.cn

TRUNCATE TABLE logs;
来源：http://za.jianghongdianzi.cn

[Q55] 排名（并列占位）
来源：http://in.szsharing.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://pj.bjjhwx.cn

[Q56] 密集排名（并列不占位）
来源：http://nt.gzmigu.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://tz.szsharing.cn

[Q57] 行号
来源：http://zz.bjjhwx.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://sk.szxytkj.cn

[Q58] 累计求和
来源：http://vc.jianghongdianzi.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://dj.gzmigu.cn

[Q59] 分组内累计
来源：http://gv.521024.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://pq.newstarts.cn

[Q60] 取上一行 / 下一行
来源：http://ft.huanxung.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://gm.asd995.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mw.lnxyls.cn

[Q61] 移动平均
来源：http://ti.9csxet.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ra.yuexingan06.cn

[Q62] 分组占比
来源：http://up.yuexingan06.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://zd.gzmigu.cn

[Q63] 开启事务
来源：http://pf.huixinmuqiang.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://bs.gzmigu.cn

[Q64] 提交事务
来源：http://wj.jianghongdianzi.cn

COMMIT;
来源：http://mo.huanxung.cn

[Q65] 回滚事务
来源：http://pb.colortex.cn

ROLLBACK;
来源：http://ol.newstarts.cn

[Q66] 行锁查询
来源：http://wr.huanxung.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://jo.muxihuayi.cn

[Q67] 设置隔离级别
来源：http://fq.haigaiapp.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://nx.hnjuh.cn

[Q68] 保存点
来源：http://xx.haigaiapp.cn

SAVEPOINT sp1;
来源：http://iy.szsharing.cn

ROLLBACK TO sp1;
来源：http://hd.nicolike.cn

[Q69] 查看执行计划
来源：http://zr.haigaiapp.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://rc.colortex.cn

[Q70] 更新统计信息
来源：http://hn.hnjuh.cn

ANALYZE TABLE users;
来源：http://os.newstarts.cn

[Q71] 查看建表语句
来源：http://fs.bookmarksfly.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ww.nicolike.cn

[Q72] 查看索引
来源：http://bo.bookmarksfly.cn

SHOW INDEX FROM users;
来源：http://ds.huanxung.cn

[Q73] 查看表状态
来源：http://yd.panjiajie.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://kl.hnjuh.cn

[Q74] 强制使用索引
来源：http://di.9csxet.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://sf.haigaiapp.cn

[Q75] 日期格式化
来源：http://df.shxzukj.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ua.hahajie.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ev.bjjhwx.cn

[Q76] 按天统计
来源：http://qu.haigaiapp.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://xz.hnjuh.cn

[Q77] 时间加减
来源：http://fh.jctech888.com.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wg.9csxet.cn

[Q78] 当前时间
来源：http://ph.jctech888.com.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://xj.muxihuayi.cn

[Q79] 字符串拼接
来源：http://sb.shtwfgs.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://pg.hahajie.cn

[Q80] 字符串截取
来源：http://bk.shxzukj.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ex.jctech888.com.cn

[Q81] 字符串替换
来源：http://zn.521024.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://vf.nszjky.cn

[Q82] 字符长度与字节长度
来源：http://uw.bookmarksfly.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ol.colortex.cn

[Q83] 大小写转换
来源：http://ch.huixiangedu.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://rq.nszjky.cn

[Q84] 去除首尾空格
来源：http://xz.shtwfgs.cn

SELECT TRIM(name) FROM users;
来源：http://qb.nszjky.cn

[Q85] 数值取整
来源：http://dg.yuexingan06.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://qw.yuntaijiaju.cn

[Q86] 读取 JSON 字段
来源：http://sf.521024.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://gi.shxzskj.cn

[Q87] JSON 字段做条件
来源：http://nb.wgjwhj.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://im.gzmigu.cn

[Q88] 行转列（条件聚合）
来源：http://gi.bjjhwx.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ra.bookmarksfly.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://jt.nicolike.cn

[Q89] 判断表是否存在
来源：http://jq.huixinmuqiang.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://yt.colortex.cn

[Q90] 生成序号列
来源：http://ek.9csxet.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://yb.chemitech.net.cn

================================================================================
来源：http://da.yuntaijiaju.cn

R. Bash 专题
来源：http://wn.jctech888.com.cn

================================================================================
来源：http://tr.521024.cn

[R01] shebang 与严格模式
来源：http://ne.9csxet.cn

#!/usr/bin/env bash
来源：http://cp.hnjuh.cn

set -euo pipefail
来源：http://su.shtwfgs.cn

[R02] 变量赋值与使用
来源：http://st.9csxet.cn

name="Tom"; echo "$name"
来源：http://az.huixiangedu.cn

[R03] 只读变量
来源：http://vq.lnxyls.cn

readonly PI=3.14
来源：http://eh.bookmarksfly.cn

[R04] 位置参数
来源：http://sk.nicolike.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://gg.9csxet.cn

[R05] 参数默认值
来源：http://pv.bjjhwx.cn

name="${1:-default}"
来源：http://ay.shtwfgs.cn

[R06] 判断命令是否存在
来源：http://gy.lnxyls.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ue.hnjuh.cn

[R07] if 判断文件
来源：http://zu.newstarts.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://sc.shxzskj.cn

[R08] 数值比较
来源：http://vp.wgjwhj.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://sv.szxytkj.cn

[R09] 字符串比较
来源：http://ir.asd995.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://iy.bjjhwx.cn

[R10] 正则匹配
来源：http://jb.szsharing.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://xr.hnjuh.cn

[R11] case 多分支
来源：http://ls.newstarts.cn

case "$1" in
来源：http://bq.huanxung.cn

start) echo "启动" ;;
来源：http://ag.gzmigu.cn

stop)  echo "停止" ;;
来源：http://tl.nicolike.cn

*)     echo "未知命令" ;;
来源：http://jf.huixinmuqiang.cn

esac
来源：http://vv.huanxung.cn

[R12] for 遍历文件
来源：http://in.yuntaijiaju.cn

for f in *.txt; do echo "$f"; done
来源：http://oq.haigaiapp.cn

[R13] for 计数循环
来源：http://qy.shxzskj.cn

for i in {1..10}; do echo "$i"; done
来源：http://bl.lnxyls.cn

[R14] C 风格 for
来源：http://qi.521024.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://yw.huixiangedu.cn

[R15] while 逐行读文件
来源：http://rw.colortex.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ej.muxihuayi.cn

[R16] until 等待条件
来源：http://qi.wgjwhj.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://kr.panjiajie.cn

[R17] 数组定义与取值
来源：http://po.panjiajie.cn

arr=(a b c); echo "${arr[0]}"
来源：http://nc.wgjwhj.cn

[R18] 遍历数组
来源：http://tj.bjjhwx.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://gm.colortex.cn

[R19] 数组长度
来源：http://lk.wgjwhj.cn

echo "${#arr[@]}"
来源：http://af.jctech888.com.cn

[R20] 关联数组（字典）
来源：http://br.bjjhwx.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://lv.newstarts.cn

[R21] 字符串长度
来源：http://dj.hahajie.cn


<!-- 参考信息 -->