代发 wailian999

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ld.panjiajie.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://mm.lnxyls.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://et.shtwfgs.cn

[P04] 求长度
来源：http://lx.yuntaijiaju.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://kz.colortex.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://nh.gzmigu.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://lc.shxzukj.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://rf.shtwfgs.cn

Java: list.size();  map.size();  s.length()
来源：http://ty.huanxung.cn

Go:   len(arr);  len(m)
来源：http://ej.colortex.cn

Ruby: x.length;  x.size
来源：http://ml.haigaiapp.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://ji.bookmarksfly.cn

[P05] 判断两个对象内容是否相等
来源：http://xk.nicolike.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://rv.wgjwhj.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://pz.521024.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://kr.nicolike.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://cy.9csxet.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://dj.muxihuayi.cn

Go:   reflect.DeepEqual(a, b)
来源：http://wv.shxzskj.cn

Ruby: a == b
来源：http://sy.nszjky.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ze.bjjhwx.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mn.yuntaijiaju.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://vw.szxytkj.cn

PHP:  if (empty($x)) {}
来源：http://cx.newstarts.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://tu.bookmarksfly.cn

TS:   if (x == null) {}
来源：http://eq.haigaiapp.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://rs.nicolike.cn

Go:   if x == nil {}
来源：http://pf.panjiajie.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://fr.huixinmuqiang.cn

C#:   if (x is null) {}
来源：http://qk.bookmarksfly.cn

[P07] 防抖与节流
来源：http://gt.muxihuayi.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mn.szsharing.cn

PHP:  // 手写时间戳比较
来源：http://cy.nicolike.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://kh.panjiajie.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wu.jianghongdianzi.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ej.huixinmuqiang.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://sh.huanxung.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://vk.yuntaijiaju.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://zj.jianghongdianzi.cn

[P08] 处理浮点精度问题
来源：http://tm.shtwfgs.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://cu.yuntaijiaju.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://qv.newstarts.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wy.chemitech.net.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mg.bookmarksfly.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ku.jctech888.com.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://jy.shxzskj.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://qk.yuexingan06.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://id.asd995.cn

================================================================================
来源：http://gg.jianghongdianzi.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://op.nicolike.cn

================================================================================
来源：http://hk.haigaiapp.cn

[Q01] 创建表
来源：http://vy.muxihuayi.cn

CREATE TABLE users (
来源：http://yh.yuntaijiaju.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://yb.muxihuayi.cn

name VARCHAR(50) NOT NULL,
来源：http://qw.shtwfgs.cn

email VARCHAR(100) UNIQUE,
来源：http://vs.yuexingan06.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ax.huixinmuqiang.cn

);
来源：http://oq.haigaiapp.cn

[Q02] 创建带外键的表
来源：http://ai.jianghongdianzi.cn

CREATE TABLE orders (
来源：http://cv.haigaiapp.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://yf.yuexingan06.cn

user_id INT NOT NULL,
来源：http://pa.panjiajie.cn

amount DECIMAL(10, 2),
来源：http://fy.chemitech.net.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ja.shxzskj.cn

);
来源：http://xo.9csxet.cn

[Q03] 增加列
来源：http://ve.bookmarksfly.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ne.szsharing.cn

[Q04] 修改列类型
来源：http://cr.asd995.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://rl.lnxyls.cn

[Q05] 重命名列
来源：http://il.shtwfgs.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://pq.szxytkj.cn

[Q06] 删除列
来源：http://zu.wgjwhj.cn

ALTER TABLE users DROP COLUMN age;
来源：http://vr.bookmarksfly.cn

[Q07] 删除表
来源：http://cl.shxzskj.cn

DROP TABLE IF EXISTS orders;
来源：http://bl.haigaiapp.cn

[Q08] 创建普通索引
来源：http://pk.shxzskj.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://hi.shtwfgs.cn

[Q09] 创建唯一索引
来源：http://gf.jianghongdianzi.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ec.nicolike.cn

[Q10] 插入单行
来源：http://at.panjiajie.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://yd.bjjhwx.cn

[Q11] 一次插入多行
来源：http://hw.hahajie.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://aw.gzmigu.cn

[Q12] 插入后取自增 ID
来源：http://xl.gzmigu.cn

INSERT INTO users (name) VALUES ('C');
来源：http://il.jianghongdianzi.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://lp.wgjwhj.cn

[Q13] 忽略重复插入
来源：http://cx.yuexingan06.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hm.shtwfgs.cn

[Q14] 存在则更新（upsert）
来源：http://cf.asd995.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://bj.szsharing.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://lm.szxytkj.cn

[Q15] 查询全部
来源：http://py.huixiangedu.cn

SELECT * FROM users;
来源：http://uf.jianghongdianzi.cn

[Q16] 查询指定列
来源：http://tf.yuntaijiaju.cn

SELECT id, name FROM users;
来源：http://yv.hahajie.cn

[Q17] 条件查询
来源：http://tu.9csxet.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ol.shxzskj.cn

[Q18] 模糊匹配
来源：http://za.shtwfgs.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://nf.nszjky.cn

[Q19] 范围查询
来源：http://fb.wgjwhj.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mn.szsharing.cn

[Q20] IN 列表
来源：http://oq.chemitech.net.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://xl.yuexingan06.cn

[Q21] 空值判断
来源：http://ee.shxzukj.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://et.jianghongdianzi.cn

[Q22] 排序
来源：http://el.bjjhwx.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://tf.huanxung.cn

[Q23] 分页
来源：http://sf.wgjwhj.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://yx.muxihuayi.cn

[Q24] 去重
来源：http://ma.muxihuayi.cn

SELECT DISTINCT city FROM users;
来源：http://ot.panjiajie.cn

[Q25] 只取前 N 条
来源：http://ux.szsharing.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://jg.bjjhwx.cn

[Q26] 计数
来源：http://ed.wgjwhj.cn

SELECT COUNT(*) FROM users;
来源：http://th.huanxung.cn

[Q27] 条件计数
来源：http://ma.gzmigu.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://de.colortex.cn

[Q28] 求和与平均
来源：http://ot.hahajie.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://nt.huixiangedu.cn

[Q29] 最大最小值
来源：http://xk.huanxung.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://tt.521024.cn

[Q30] 分组统计
来源：http://yi.huanxung.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://pw.szxytkj.cn

[Q31] 分组后过滤
来源：http://kb.szxytkj.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://fj.9csxet.cn

[Q32] 分组拼接字符串
来源：http://tx.gzmigu.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://do.wgjwhj.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://gj.nszjky.cn

[Q33] 多列分组
来源：http://vp.gzmigu.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ux.szsharing.cn

[Q34] 每组取第一条
来源：http://xx.haigaiapp.cn

SELECT * FROM (
来源：http://lp.haigaiapp.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://tn.gzmigu.cn

) t WHERE rn = 1;
来源：http://iw.nicolike.cn

[Q35] 内连接
来源：http://om.nicolike.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ct.nszjky.cn

[Q36] 左连接
来源：http://sy.newstarts.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://bp.hnjuh.cn

[Q37] 右连接
来源：http://bf.jianghongdianzi.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://fd.muxihuayi.cn

[Q38] 全外连接（PostgreSQL）
来源：http://jk.jctech888.com.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://yd.newstarts.cn

[Q39] 自连接（查上下级）
来源：http://su.huanxung.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://fp.nicolike.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://pf.shxzskj.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://dr.lnxyls.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://zu.521024.cn

[Q41] 多表连接
来源：http://rf.shxzskj.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://jz.szsharing.cn

JOIN users u ON u.id = o.user_id
来源：http://hh.shxzskj.cn

JOIN products p ON p.id = o.product_id;
来源：http://qg.bjjhwx.cn

[Q42] 连接条件附加过滤
来源：http://my.shtwfgs.cn

SELECT u.name, o.amount FROM users u
来源：http://kb.szxytkj.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mg.9csxet.cn

[Q43] 标量子查询
来源：http://wf.jianghongdianzi.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://uc.yuntaijiaju.cn

[Q44] IN 子查询
来源：http://nh.szsharing.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://sc.shxzukj.cn

[Q45] EXISTS 判断存在
来源：http://kz.gzmigu.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://br.yuexingan06.cn

[Q46] NOT EXISTS 判断不存在
来源：http://df.szxytkj.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mw.nszjky.cn

[Q47] 与平均值比较
来源：http://io.haigaiapp.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://xx.newstarts.cn

[Q48] CTE 公用表表达式
来源：http://yt.szxytkj.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://gq.yuexingan06.cn

SELECT * FROM t WHERE c > 5;
来源：http://tr.gzmigu.cn

[Q49] 更新单行
来源：http://vj.lnxyls.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hu.haigaiapp.cn

[Q50] 批量更新
来源：http://zr.huixinmuqiang.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://gc.shxzskj.cn

[Q51] 用子查询更新
来源：http://mx.colortex.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://ip.haigaiapp.cn

[Q52] 删除指定行
来源：http://ms.panjiajie.cn

DELETE FROM users WHERE id = 10;
来源：http://wt.szxytkj.cn

[Q53] 按条件删除
来源：http://re.colortex.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://kh.521024.cn

[Q54] 清空表
来源：http://ab.gzmigu.cn

TRUNCATE TABLE logs;
来源：http://cs.yuexingan06.cn

[Q55] 排名（并列占位）
来源：http://ni.huixiangedu.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://zf.szsharing.cn

[Q56] 密集排名（并列不占位）
来源：http://cp.shxzukj.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://yt.szxytkj.cn

[Q57] 行号
来源：http://yy.huixinmuqiang.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://vu.muxihuayi.cn

[Q58] 累计求和
来源：http://rt.huixinmuqiang.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ev.shtwfgs.cn

[Q59] 分组内累计
来源：http://lq.hnjuh.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://jj.panjiajie.cn

[Q60] 取上一行 / 下一行
来源：http://gh.nicolike.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://te.lnxyls.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://kh.521024.cn

[Q61] 移动平均
来源：http://bm.shxzskj.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://as.shxzskj.cn

[Q62] 分组占比
来源：http://is.wgjwhj.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://jf.jctech888.com.cn

[Q63] 开启事务
来源：http://ij.asd995.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://zf.bookmarksfly.cn

[Q64] 提交事务
来源：http://jd.haigaiapp.cn

COMMIT;
来源：http://hk.huixiangedu.cn

[Q65] 回滚事务
来源：http://mh.wgjwhj.cn

ROLLBACK;
来源：http://vl.szsharing.cn

[Q66] 行锁查询
来源：http://re.hnjuh.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wp.shxzukj.cn

[Q67] 设置隔离级别
来源：http://ql.szsharing.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://tj.lnxyls.cn

[Q68] 保存点
来源：http://bj.szsharing.cn

SAVEPOINT sp1;
来源：http://mc.szxytkj.cn

ROLLBACK TO sp1;
来源：http://qo.huixiangedu.cn

[Q69] 查看执行计划
来源：http://zk.lnxyls.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://pn.newstarts.cn

[Q70] 更新统计信息
来源：http://co.newstarts.cn

ANALYZE TABLE users;
来源：http://yt.hnjuh.cn

[Q71] 查看建表语句
来源：http://tn.nicolike.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://bt.shxzukj.cn

[Q72] 查看索引
来源：http://bn.muxihuayi.cn

SHOW INDEX FROM users;
来源：http://jw.szsharing.cn

[Q73] 查看表状态
来源：http://io.colortex.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://ou.yuntaijiaju.cn

[Q74] 强制使用索引
来源：http://nk.shtwfgs.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://im.panjiajie.cn

[Q75] 日期格式化
来源：http://yp.szxytkj.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://xs.huixinmuqiang.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://kd.szxytkj.cn

[Q76] 按天统计
来源：http://ld.bookmarksfly.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://dl.panjiajie.cn

[Q77] 时间加减
来源：http://px.asd995.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wh.panjiajie.cn

[Q78] 当前时间
来源：http://jz.shxzukj.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://eu.panjiajie.cn

[Q79] 字符串拼接
来源：http://ie.bookmarksfly.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ni.hahajie.cn

[Q80] 字符串截取
来源：http://pc.nszjky.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://do.hnjuh.cn

[Q81] 字符串替换
来源：http://pl.muxihuayi.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mt.jianghongdianzi.cn

[Q82] 字符长度与字节长度
来源：http://qr.huixinmuqiang.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://eo.colortex.cn

[Q83] 大小写转换
来源：http://lv.shxzukj.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://bd.chemitech.net.cn

[Q84] 去除首尾空格
来源：http://ht.wgjwhj.cn

SELECT TRIM(name) FROM users;
来源：http://yl.newstarts.cn

[Q85] 数值取整
来源：http://oj.wgjwhj.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://vv.yuntaijiaju.cn

[Q86] 读取 JSON 字段
来源：http://iv.huixinmuqiang.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hj.szxytkj.cn

[Q87] JSON 字段做条件
来源：http://mu.521024.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ja.panjiajie.cn

[Q88] 行转列（条件聚合）
来源：http://zs.asd995.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://nw.muxihuayi.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://lh.shtwfgs.cn

[Q89] 判断表是否存在
来源：http://df.shxzskj.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hi.huixiangedu.cn

[Q90] 生成序号列
来源：http://tm.bjjhwx.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://kn.lnxyls.cn

================================================================================
来源：http://se.shxzukj.cn

R. Bash 专题
来源：http://tn.shtwfgs.cn

================================================================================
来源：http://rb.asd995.cn

[R01] shebang 与严格模式
来源：http://gy.gzmigu.cn

#!/usr/bin/env bash
来源：http://fd.lnxyls.cn

set -euo pipefail
来源：http://ti.gzmigu.cn

[R02] 变量赋值与使用
来源：http://gt.nicolike.cn

name="Tom"; echo "$name"
来源：http://zv.shxzukj.cn

[R03] 只读变量
来源：http://yj.hahajie.cn

readonly PI=3.14
来源：http://jt.521024.cn

[R04] 位置参数
来源：http://pz.huanxung.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mk.jctech888.com.cn

[R05] 参数默认值
来源：http://aa.hahajie.cn

name="${1:-default}"
来源：http://eq.shxzskj.cn

[R06] 判断命令是否存在
来源：http://iv.asd995.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://qp.hahajie.cn

[R07] if 判断文件
来源：http://hs.huanxung.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://qt.gzmigu.cn

[R08] 数值比较
来源：http://kq.yuexingan06.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://uu.9csxet.cn

[R09] 字符串比较
来源：http://dv.gzmigu.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://oq.asd995.cn

[R10] 正则匹配
来源：http://ha.521024.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ad.newstarts.cn

[R11] case 多分支
来源：http://qx.huixinmuqiang.cn

case "$1" in
来源：http://px.bookmarksfly.cn

start) echo "启动" ;;
来源：http://pd.nszjky.cn

stop)  echo "停止" ;;
来源：http://kz.hahajie.cn

*)     echo "未知命令" ;;
来源：http://lf.asd995.cn

esac
来源：http://bg.gzmigu.cn

[R12] for 遍历文件
来源：http://ul.nszjky.cn

for f in *.txt; do echo "$f"; done
来源：http://ex.newstarts.cn

[R13] for 计数循环
来源：http://xt.hnjuh.cn

for i in {1..10}; do echo "$i"; done
来源：http://ge.shxzukj.cn

[R14] C 风格 for
来源：http://uk.wgjwhj.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://cw.yuntaijiaju.cn

[R15] while 逐行读文件
来源：http://kh.szsharing.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://xw.haigaiapp.cn

[R16] until 等待条件
来源：http://sy.szsharing.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://nm.wgjwhj.cn

[R17] 数组定义与取值
来源：http://dq.shxzukj.cn

arr=(a b c); echo "${arr[0]}"
来源：http://fp.9csxet.cn

[R18] 遍历数组
来源：http://mt.asd995.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wl.colortex.cn

[R19] 数组长度
来源：http://ur.szsharing.cn


<!-- 参考信息 -->