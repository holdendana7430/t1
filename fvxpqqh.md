代发 wailian999

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://rg.bjjhwx.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://pm.jctech888.com.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wx.yuntaijiaju.cn

[P04] 求长度
来源：http://br.huixiangedu.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wn.szsharing.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://yl.muxihuayi.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hu.yuntaijiaju.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://br.szsharing.cn

Java: list.size();  map.size();  s.length()
来源：http://tw.szsharing.cn

Go:   len(arr);  len(m)
来源：http://qn.shxzskj.cn

Ruby: x.length;  x.size
来源：http://hx.jctech888.com.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://uk.jctech888.com.cn

[P05] 判断两个对象内容是否相等
来源：http://mj.newstarts.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://fp.521024.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ag.nicolike.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hg.yuexingan06.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://qy.szxytkj.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://uz.huixinmuqiang.cn

Go:   reflect.DeepEqual(a, b)
来源：http://od.yuexingan06.cn

Ruby: a == b
来源：http://sn.muxihuayi.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://vb.huixinmuqiang.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hh.hahajie.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://zh.bjjhwx.cn

PHP:  if (empty($x)) {}
来源：http://an.huanxung.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ne.colortex.cn

TS:   if (x == null) {}
来源：http://dg.bookmarksfly.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://sn.hnjuh.cn

Go:   if x == nil {}
来源：http://ip.chemitech.net.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ty.haigaiapp.cn

C#:   if (x is null) {}
来源：http://tl.lnxyls.cn

[P07] 防抖与节流
来源：http://pt.szxytkj.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://nc.shxzukj.cn

PHP:  // 手写时间戳比较
来源：http://wn.nszjky.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://fd.nszjky.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://oh.wgjwhj.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ol.yuexingan06.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hg.jctech888.com.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://gx.colortex.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://jk.gzmigu.cn

[P08] 处理浮点精度问题
来源：http://hj.szsharing.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://dk.asd995.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://lr.bjjhwx.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://bt.huixiangedu.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hs.gzmigu.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ay.yuexingan06.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://yv.yuexingan06.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://at.shxzukj.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://lh.9csxet.cn

================================================================================
来源：http://jq.szsharing.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ti.muxihuayi.cn

================================================================================
来源：http://xk.chemitech.net.cn

[Q01] 创建表
来源：http://ld.hnjuh.cn

CREATE TABLE users (
来源：http://ss.nicolike.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://xl.shxzskj.cn

name VARCHAR(50) NOT NULL,
来源：http://hx.chemitech.net.cn

email VARCHAR(100) UNIQUE,
来源：http://ld.shtwfgs.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ah.szxytkj.cn

);
来源：http://jn.jctech888.com.cn

[Q02] 创建带外键的表
来源：http://rd.haigaiapp.cn

CREATE TABLE orders (
来源：http://jy.jctech888.com.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://fa.nszjky.cn

user_id INT NOT NULL,
来源：http://fx.szxytkj.cn

amount DECIMAL(10, 2),
来源：http://yh.bjjhwx.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ku.huixiangedu.cn

);
来源：http://ku.hahajie.cn

[Q03] 增加列
来源：http://em.haigaiapp.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://eq.haigaiapp.cn

[Q04] 修改列类型
来源：http://wq.newstarts.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://gn.huanxung.cn

[Q05] 重命名列
来源：http://fa.wgjwhj.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://kn.gzmigu.cn

[Q06] 删除列
来源：http://we.shtwfgs.cn

ALTER TABLE users DROP COLUMN age;
来源：http://zh.colortex.cn

[Q07] 删除表
来源：http://uy.shxzskj.cn

DROP TABLE IF EXISTS orders;
来源：http://vi.521024.cn

[Q08] 创建普通索引
来源：http://zb.521024.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://mm.haigaiapp.cn

[Q09] 创建唯一索引
来源：http://ll.haigaiapp.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://pn.jianghongdianzi.cn

[Q10] 插入单行
来源：http://tu.huanxung.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://vx.521024.cn

[Q11] 一次插入多行
来源：http://xg.yuntaijiaju.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://sb.huanxung.cn

[Q12] 插入后取自增 ID
来源：http://go.haigaiapp.cn

INSERT INTO users (name) VALUES ('C');
来源：http://mb.jctech888.com.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://jj.lnxyls.cn

[Q13] 忽略重复插入
来源：http://mt.shtwfgs.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://tt.asd995.cn

[Q14] 存在则更新（upsert）
来源：http://ko.shtwfgs.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://bo.9csxet.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://kw.newstarts.cn

[Q15] 查询全部
来源：http://qo.haigaiapp.cn

SELECT * FROM users;
来源：http://rt.wgjwhj.cn

[Q16] 查询指定列
来源：http://lj.panjiajie.cn

SELECT id, name FROM users;
来源：http://zg.shtwfgs.cn

[Q17] 条件查询
来源：http://nz.nicolike.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://bh.9csxet.cn

[Q18] 模糊匹配
来源：http://bl.hahajie.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hm.nszjky.cn

[Q19] 范围查询
来源：http://mp.shxzskj.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://kl.jctech888.com.cn

[Q20] IN 列表
来源：http://cq.szsharing.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://er.huanxung.cn

[Q21] 空值判断
来源：http://qr.nicolike.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://ee.huanxung.cn

[Q22] 排序
来源：http://cr.shxzskj.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://kd.hahajie.cn

[Q23] 分页
来源：http://fy.newstarts.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://db.yuexingan06.cn

[Q24] 去重
来源：http://ry.szxytkj.cn

SELECT DISTINCT city FROM users;
来源：http://mt.szxytkj.cn

[Q25] 只取前 N 条
来源：http://tz.chemitech.net.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://tw.jctech888.com.cn

[Q26] 计数
来源：http://xh.newstarts.cn

SELECT COUNT(*) FROM users;
来源：http://zg.huanxung.cn

[Q27] 条件计数
来源：http://rv.huixinmuqiang.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://yg.huixiangedu.cn

[Q28] 求和与平均
来源：http://dr.jianghongdianzi.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://sp.chemitech.net.cn

[Q29] 最大最小值
来源：http://sn.szxytkj.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://yz.nicolike.cn

[Q30] 分组统计
来源：http://uo.colortex.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wj.haigaiapp.cn

[Q31] 分组后过滤
来源：http://ya.hnjuh.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://re.yuexingan06.cn

[Q32] 分组拼接字符串
来源：http://xu.huanxung.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://xf.gzmigu.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://fj.nszjky.cn

[Q33] 多列分组
来源：http://ii.hahajie.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://po.yuntaijiaju.cn

[Q34] 每组取第一条
来源：http://pl.muxihuayi.cn

SELECT * FROM (
来源：http://ck.bjjhwx.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://gt.lnxyls.cn

) t WHERE rn = 1;
来源：http://wz.yuntaijiaju.cn

[Q35] 内连接
来源：http://ya.haigaiapp.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://qk.shtwfgs.cn

[Q36] 左连接
来源：http://ul.hnjuh.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://az.9csxet.cn

[Q37] 右连接
来源：http://ct.jianghongdianzi.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://nj.wgjwhj.cn

[Q38] 全外连接（PostgreSQL）
来源：http://lw.shxzskj.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://rd.hnjuh.cn

[Q39] 自连接（查上下级）
来源：http://gn.gzmigu.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://ns.shxzukj.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://nh.panjiajie.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://yd.jianghongdianzi.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://nt.yuntaijiaju.cn

[Q41] 多表连接
来源：http://fh.asd995.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://ex.muxihuayi.cn

JOIN users u ON u.id = o.user_id
来源：http://sh.panjiajie.cn

JOIN products p ON p.id = o.product_id;
来源：http://vy.bjjhwx.cn

[Q42] 连接条件附加过滤
来源：http://pv.huixinmuqiang.cn

SELECT u.name, o.amount FROM users u
来源：http://qd.shtwfgs.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://rp.521024.cn

[Q43] 标量子查询
来源：http://qv.hnjuh.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://uu.gzmigu.cn

[Q44] IN 子查询
来源：http://jv.szsharing.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://sd.nicolike.cn

[Q45] EXISTS 判断存在
来源：http://ls.jctech888.com.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hc.huixiangedu.cn

[Q46] NOT EXISTS 判断不存在
来源：http://ff.panjiajie.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://lh.haigaiapp.cn

[Q47] 与平均值比较
来源：http://mt.nszjky.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://nd.gzmigu.cn

[Q48] CTE 公用表表达式
来源：http://re.9csxet.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://nk.521024.cn

SELECT * FROM t WHERE c > 5;
来源：http://rf.lnxyls.cn

[Q49] 更新单行
来源：http://wr.521024.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://gy.shxzukj.cn

[Q50] 批量更新
来源：http://ex.szsharing.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mg.shxzukj.cn

[Q51] 用子查询更新
来源：http://xe.colortex.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://ai.bjjhwx.cn

[Q52] 删除指定行
来源：http://tj.jctech888.com.cn

DELETE FROM users WHERE id = 10;
来源：http://dk.huixiangedu.cn

[Q53] 按条件删除
来源：http://yc.521024.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wp.huixinmuqiang.cn

[Q54] 清空表
来源：http://ax.colortex.cn

TRUNCATE TABLE logs;
来源：http://es.shxzukj.cn

[Q55] 排名（并列占位）
来源：http://kn.521024.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://to.521024.cn

[Q56] 密集排名（并列不占位）
来源：http://cu.jianghongdianzi.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ey.wgjwhj.cn

[Q57] 行号
来源：http://ff.shtwfgs.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://du.bjjhwx.cn

[Q58] 累计求和
来源：http://qw.jctech888.com.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ac.lnxyls.cn

[Q59] 分组内累计
来源：http://sm.colortex.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ot.521024.cn

[Q60] 取上一行 / 下一行
来源：http://zu.szsharing.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://qg.bookmarksfly.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://gp.chemitech.net.cn

[Q61] 移动平均
来源：http://lj.chemitech.net.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wy.chemitech.net.cn

[Q62] 分组占比
来源：http://vd.bjjhwx.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://oz.shxzukj.cn

[Q63] 开启事务
来源：http://wb.colortex.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://oy.nszjky.cn

[Q64] 提交事务
来源：http://pu.yuexingan06.cn

COMMIT;
来源：http://yl.hahajie.cn

[Q65] 回滚事务
来源：http://bp.hahajie.cn

ROLLBACK;
来源：http://rf.bookmarksfly.cn

[Q66] 行锁查询
来源：http://yi.shtwfgs.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://qp.panjiajie.cn

[Q67] 设置隔离级别
来源：http://lx.nszjky.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mt.yuexingan06.cn

[Q68] 保存点
来源：http://eg.9csxet.cn

SAVEPOINT sp1;
来源：http://lm.nicolike.cn

ROLLBACK TO sp1;
来源：http://iq.newstarts.cn

[Q69] 查看执行计划
来源：http://jj.521024.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://em.gzmigu.cn

[Q70] 更新统计信息
来源：http://fj.lnxyls.cn

ANALYZE TABLE users;
来源：http://xz.szxytkj.cn

[Q71] 查看建表语句
来源：http://hj.asd995.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://eq.lnxyls.cn

[Q72] 查看索引
来源：http://oy.szsharing.cn

SHOW INDEX FROM users;
来源：http://ep.szxytkj.cn

[Q73] 查看表状态
来源：http://ed.panjiajie.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://vi.jctech888.com.cn

[Q74] 强制使用索引
来源：http://lr.colortex.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ni.nszjky.cn

[Q75] 日期格式化
来源：http://bk.jianghongdianzi.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://eo.shxzskj.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hh.bjjhwx.cn

[Q76] 按天统计
来源：http://ca.gzmigu.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ce.wgjwhj.cn

[Q77] 时间加减
来源：http://wb.panjiajie.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://qc.colortex.cn

[Q78] 当前时间
来源：http://ko.jianghongdianzi.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://uu.huanxung.cn

[Q79] 字符串拼接
来源：http://nl.hnjuh.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://zg.lnxyls.cn

[Q80] 字符串截取
来源：http://dg.colortex.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://pj.shxzskj.cn

[Q81] 字符串替换
来源：http://om.shxzukj.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://xq.hnjuh.cn

[Q82] 字符长度与字节长度
来源：http://qf.chemitech.net.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://pd.hahajie.cn

[Q83] 大小写转换
来源：http://yu.jctech888.com.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://yf.shtwfgs.cn

[Q84] 去除首尾空格
来源：http://jb.huanxung.cn

SELECT TRIM(name) FROM users;
来源：http://px.hahajie.cn

[Q85] 数值取整
来源：http://nn.9csxet.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://zp.521024.cn

[Q86] 读取 JSON 字段
来源：http://wt.yuexingan06.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://oo.szxytkj.cn

[Q87] JSON 字段做条件
来源：http://pj.szxytkj.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://eu.shxzskj.cn

[Q88] 行转列（条件聚合）
来源：http://fq.shtwfgs.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://yu.bookmarksfly.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://we.wgjwhj.cn

[Q89] 判断表是否存在
来源：http://te.nszjky.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://vg.521024.cn

[Q90] 生成序号列
来源：http://fm.muxihuayi.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ct.muxihuayi.cn

================================================================================
来源：http://kv.wgjwhj.cn

R. Bash 专题
来源：http://hl.asd995.cn

================================================================================
来源：http://ui.colortex.cn

[R01] shebang 与严格模式
来源：http://sw.yuntaijiaju.cn

#!/usr/bin/env bash
来源：http://rd.gzmigu.cn

set -euo pipefail
来源：http://vv.yuexingan06.cn

[R02] 变量赋值与使用
来源：http://xs.huixiangedu.cn

name="Tom"; echo "$name"
来源：http://ph.yuntaijiaju.cn

[R03] 只读变量
来源：http://qm.yuntaijiaju.cn

readonly PI=3.14
来源：http://qb.wgjwhj.cn

[R04] 位置参数
来源：http://ls.hahajie.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://sb.bookmarksfly.cn

[R05] 参数默认值
来源：http://lq.huixiangedu.cn

name="${1:-default}"
来源：http://vq.shtwfgs.cn

[R06] 判断命令是否存在
来源：http://iy.yuexingan06.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://kh.muxihuayi.cn

[R07] if 判断文件
来源：http://cw.haigaiapp.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://go.shxzukj.cn

[R08] 数值比较
来源：http://et.hnjuh.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://ow.huixinmuqiang.cn

[R09] 字符串比较
来源：http://pp.huanxung.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://sy.nicolike.cn

[R10] 正则匹配
来源：http://kq.haigaiapp.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wg.9csxet.cn

[R11] case 多分支
来源：http://ik.lnxyls.cn

case "$1" in
来源：http://he.wgjwhj.cn

start) echo "启动" ;;
来源：http://fw.nicolike.cn

stop)  echo "停止" ;;
来源：http://em.huixiangedu.cn

*)     echo "未知命令" ;;
来源：http://sx.yuntaijiaju.cn

esac
来源：http://fd.9csxet.cn

[R12] for 遍历文件
来源：http://lv.nicolike.cn

for f in *.txt; do echo "$f"; done
来源：http://ui.gzmigu.cn

[R13] for 计数循环
来源：http://ng.hahajie.cn

for i in {1..10}; do echo "$i"; done
来源：http://ec.haigaiapp.cn

[R14] C 风格 for
来源：http://yi.hnjuh.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://rn.hnjuh.cn

[R15] while 逐行读文件
来源：http://tw.9csxet.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wz.jianghongdianzi.cn

[R16] until 等待条件
来源：http://sm.huanxung.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://pd.hahajie.cn

[R17] 数组定义与取值
来源：http://gp.huixiangedu.cn

arr=(a b c); echo "${arr[0]}"
来源：http://mu.gzmigu.cn

[R18] 遍历数组
来源：http://lc.huanxung.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://er.yuexingan06.cn

[R19] 数组长度
来源：http://pp.szxytkj.cn


<!-- 参考信息 -->