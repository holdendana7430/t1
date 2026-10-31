代发 wailian999

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://oc.lnxyls.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://cy.hahajie.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://kg.nszjky.cn

[P04] 求长度
来源：http://rx.wgjwhj.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://rn.asd995.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://lp.hnjuh.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://fz.9csxet.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://vt.nszjky.cn

Java: list.size();  map.size();  s.length()
来源：http://sy.hahajie.cn

Go:   len(arr);  len(m)
来源：http://tq.huanxung.cn

Ruby: x.length;  x.size
来源：http://dl.521024.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://cq.newstarts.cn

[P05] 判断两个对象内容是否相等
来源：http://gr.jianghongdianzi.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://bd.shxzukj.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://cb.huixinmuqiang.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mu.chemitech.net.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ju.yuntaijiaju.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://bh.wgjwhj.cn

Go:   reflect.DeepEqual(a, b)
来源：http://xr.huanxung.cn

Ruby: a == b
来源：http://ti.nicolike.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://xn.nicolike.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://yx.nicolike.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://tw.521024.cn

PHP:  if (empty($x)) {}
来源：http://ih.hnjuh.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://lx.yuexingan06.cn

TS:   if (x == null) {}
来源：http://wt.huixiangedu.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://ni.huanxung.cn

Go:   if x == nil {}
来源：http://zy.wgjwhj.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://dy.szsharing.cn

C#:   if (x is null) {}
来源：http://ym.huixinmuqiang.cn

[P07] 防抖与节流
来源：http://gv.nszjky.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://zr.lnxyls.cn

PHP:  // 手写时间戳比较
来源：http://wc.huixinmuqiang.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ni.panjiajie.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://gg.yuntaijiaju.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ff.bjjhwx.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://nx.9csxet.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://ji.hnjuh.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://lw.yuntaijiaju.cn

[P08] 处理浮点精度问题
来源：http://sl.shxzskj.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://so.shxzskj.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://rb.nszjky.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://fq.haigaiapp.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ww.nszjky.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://kv.hahajie.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://tu.jianghongdianzi.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://py.bjjhwx.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://di.newstarts.cn

================================================================================
来源：http://cr.muxihuayi.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://rp.yuexingan06.cn

================================================================================
来源：http://el.nszjky.cn

[Q01] 创建表
来源：http://ft.colortex.cn

CREATE TABLE users (
来源：http://rx.jianghongdianzi.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mn.yuexingan06.cn

name VARCHAR(50) NOT NULL,
来源：http://vm.huixinmuqiang.cn

email VARCHAR(100) UNIQUE,
来源：http://ko.bookmarksfly.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hv.panjiajie.cn

);
来源：http://nr.szxytkj.cn

[Q02] 创建带外键的表
来源：http://fa.lnxyls.cn

CREATE TABLE orders (
来源：http://bf.colortex.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ns.hahajie.cn

user_id INT NOT NULL,
来源：http://sj.huixiangedu.cn

amount DECIMAL(10, 2),
来源：http://kv.huixinmuqiang.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ua.jctech888.com.cn

);
来源：http://gy.bookmarksfly.cn

[Q03] 增加列
来源：http://xn.colortex.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hp.huanxung.cn

[Q04] 修改列类型
来源：http://qf.lnxyls.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ak.szsharing.cn

[Q05] 重命名列
来源：http://if.jianghongdianzi.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ee.yuexingan06.cn

[Q06] 删除列
来源：http://pm.huixiangedu.cn

ALTER TABLE users DROP COLUMN age;
来源：http://dh.gzmigu.cn

[Q07] 删除表
来源：http://fd.521024.cn

DROP TABLE IF EXISTS orders;
来源：http://gh.haigaiapp.cn

[Q08] 创建普通索引
来源：http://sn.9csxet.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://oa.chemitech.net.cn

[Q09] 创建唯一索引
来源：http://ds.szxytkj.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://rl.gzmigu.cn

[Q10] 插入单行
来源：http://tr.jctech888.com.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ht.huanxung.cn

[Q11] 一次插入多行
来源：http://sa.521024.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://cz.hahajie.cn

[Q12] 插入后取自增 ID
来源：http://tt.huixinmuqiang.cn

INSERT INTO users (name) VALUES ('C');
来源：http://at.huixinmuqiang.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://qf.9csxet.cn

[Q13] 忽略重复插入
来源：http://yh.szsharing.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://kr.9csxet.cn

[Q14] 存在则更新（upsert）
来源：http://xh.colortex.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mr.9csxet.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://cd.huixinmuqiang.cn

[Q15] 查询全部
来源：http://dn.gzmigu.cn

SELECT * FROM users;
来源：http://gt.newstarts.cn

[Q16] 查询指定列
来源：http://mk.asd995.cn

SELECT id, name FROM users;
来源：http://tf.huanxung.cn

[Q17] 条件查询
来源：http://cn.asd995.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://kn.nszjky.cn

[Q18] 模糊匹配
来源：http://hm.szxytkj.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://bb.haigaiapp.cn

[Q19] 范围查询
来源：http://sq.9csxet.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ct.yuntaijiaju.cn

[Q20] IN 列表
来源：http://qk.panjiajie.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://tf.panjiajie.cn

[Q21] 空值判断
来源：http://sl.gzmigu.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://vg.huanxung.cn

[Q22] 排序
来源：http://jb.521024.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://yu.shxzskj.cn

[Q23] 分页
来源：http://wu.lnxyls.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://gf.hahajie.cn

[Q24] 去重
来源：http://rg.shxzskj.cn

SELECT DISTINCT city FROM users;
来源：http://ff.bjjhwx.cn

[Q25] 只取前 N 条
来源：http://ml.lnxyls.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ch.9csxet.cn

[Q26] 计数
来源：http://dz.wgjwhj.cn

SELECT COUNT(*) FROM users;
来源：http://dz.9csxet.cn

[Q27] 条件计数
来源：http://ee.huixinmuqiang.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://jb.jctech888.com.cn

[Q28] 求和与平均
来源：http://ux.lnxyls.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://kl.colortex.cn

[Q29] 最大最小值
来源：http://mn.bookmarksfly.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://ex.szsharing.cn

[Q30] 分组统计
来源：http://dc.szsharing.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://tn.lnxyls.cn

[Q31] 分组后过滤
来源：http://ws.chemitech.net.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ep.hnjuh.cn

[Q32] 分组拼接字符串
来源：http://sa.shxzskj.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://yv.gzmigu.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://xq.shtwfgs.cn

[Q33] 多列分组
来源：http://pb.nszjky.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://de.shxzukj.cn

[Q34] 每组取第一条
来源：http://vo.newstarts.cn

SELECT * FROM (
来源：http://tz.nicolike.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://sx.huixiangedu.cn

) t WHERE rn = 1;
来源：http://nx.lnxyls.cn

[Q35] 内连接
来源：http://tf.huixiangedu.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wb.nszjky.cn

[Q36] 左连接
来源：http://cv.colortex.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://pv.szsharing.cn

[Q37] 右连接
来源：http://go.521024.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://bg.newstarts.cn

[Q38] 全外连接（PostgreSQL）
来源：http://ed.huixiangedu.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://eg.huixiangedu.cn

[Q39] 自连接（查上下级）
来源：http://su.jctech888.com.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://qn.lnxyls.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://lw.szxytkj.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://nz.muxihuayi.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://qs.asd995.cn

[Q41] 多表连接
来源：http://tf.nicolike.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://ta.shxzukj.cn

JOIN users u ON u.id = o.user_id
来源：http://ik.szxytkj.cn

JOIN products p ON p.id = o.product_id;
来源：http://rb.haigaiapp.cn

[Q42] 连接条件附加过滤
来源：http://mo.jianghongdianzi.cn

SELECT u.name, o.amount FROM users u
来源：http://ma.jianghongdianzi.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://rs.chemitech.net.cn

[Q43] 标量子查询
来源：http://vt.huixiangedu.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://zr.asd995.cn

[Q44] IN 子查询
来源：http://aj.hahajie.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://pe.shtwfgs.cn

[Q45] EXISTS 判断存在
来源：http://xj.muxihuayi.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://rx.jianghongdianzi.cn

[Q46] NOT EXISTS 判断不存在
来源：http://df.hnjuh.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://cf.jianghongdianzi.cn

[Q47] 与平均值比较
来源：http://ec.9csxet.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://no.shtwfgs.cn

[Q48] CTE 公用表表达式
来源：http://el.9csxet.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://eq.asd995.cn

SELECT * FROM t WHERE c > 5;
来源：http://do.newstarts.cn

[Q49] 更新单行
来源：http://aj.shtwfgs.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://do.muxihuayi.cn

[Q50] 批量更新
来源：http://sf.nszjky.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://bc.wgjwhj.cn

[Q51] 用子查询更新
来源：http://ti.huixinmuqiang.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://sq.haigaiapp.cn

[Q52] 删除指定行
来源：http://by.hnjuh.cn

DELETE FROM users WHERE id = 10;
来源：http://va.lnxyls.cn

[Q53] 按条件删除
来源：http://ki.shxzukj.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://kb.shxzukj.cn

[Q54] 清空表
来源：http://mf.huixiangedu.cn

TRUNCATE TABLE logs;
来源：http://bz.9csxet.cn

[Q55] 排名（并列占位）
来源：http://fz.chemitech.net.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://nf.huanxung.cn

[Q56] 密集排名（并列不占位）
来源：http://pi.huanxung.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://pz.colortex.cn

[Q57] 行号
来源：http://ym.szsharing.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://sr.hnjuh.cn

[Q58] 累计求和
来源：http://ge.nszjky.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://tv.jctech888.com.cn

[Q59] 分组内累计
来源：http://lt.bookmarksfly.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://xe.bookmarksfly.cn

[Q60] 取上一行 / 下一行
来源：http://bc.521024.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ya.panjiajie.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://rs.9csxet.cn

[Q61] 移动平均
来源：http://fj.muxihuayi.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://aa.shxzukj.cn

[Q62] 分组占比
来源：http://ey.nicolike.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://vk.hnjuh.cn

[Q63] 开启事务
来源：http://ge.huixinmuqiang.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://pv.muxihuayi.cn

[Q64] 提交事务
来源：http://hf.bjjhwx.cn

COMMIT;
来源：http://jx.panjiajie.cn

[Q65] 回滚事务
来源：http://au.bookmarksfly.cn

ROLLBACK;
来源：http://ue.muxihuayi.cn

[Q66] 行锁查询
来源：http://tm.jctech888.com.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://qs.yuntaijiaju.cn

[Q67] 设置隔离级别
来源：http://dr.shxzukj.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://lo.gzmigu.cn

[Q68] 保存点
来源：http://mq.haigaiapp.cn

SAVEPOINT sp1;
来源：http://ho.nicolike.cn

ROLLBACK TO sp1;
来源：http://cg.jctech888.com.cn

[Q69] 查看执行计划
来源：http://ke.nicolike.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hp.521024.cn

[Q70] 更新统计信息
来源：http://im.yuntaijiaju.cn

ANALYZE TABLE users;
来源：http://he.asd995.cn

[Q71] 查看建表语句
来源：http://hh.9csxet.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://vx.lnxyls.cn

[Q72] 查看索引
来源：http://fo.shtwfgs.cn

SHOW INDEX FROM users;
来源：http://ia.shtwfgs.cn

[Q73] 查看表状态
来源：http://sp.bjjhwx.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://zm.wgjwhj.cn

[Q74] 强制使用索引
来源：http://zu.bjjhwx.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://gg.shxzukj.cn

[Q75] 日期格式化
来源：http://uc.nicolike.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://yk.521024.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://bh.hnjuh.cn

[Q76] 按天统计
来源：http://yp.haigaiapp.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hw.huixinmuqiang.cn

[Q77] 时间加减
来源：http://dp.haigaiapp.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://gy.shxzskj.cn

[Q78] 当前时间
来源：http://pk.szsharing.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://bz.huanxung.cn

[Q79] 字符串拼接
来源：http://ky.huixiangedu.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://tu.szxytkj.cn

[Q80] 字符串截取
来源：http://cl.szxytkj.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ao.chemitech.net.cn

[Q81] 字符串替换
来源：http://oe.asd995.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ge.hnjuh.cn

[Q82] 字符长度与字节长度
来源：http://na.yuexingan06.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ig.bjjhwx.cn

[Q83] 大小写转换
来源：http://xp.521024.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://dl.chemitech.net.cn

[Q84] 去除首尾空格
来源：http://vs.hnjuh.cn

SELECT TRIM(name) FROM users;
来源：http://vu.jianghongdianzi.cn

[Q85] 数值取整
来源：http://pt.shtwfgs.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ox.haigaiapp.cn

[Q86] 读取 JSON 字段
来源：http://rq.shxzskj.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://me.lnxyls.cn

[Q87] JSON 字段做条件
来源：http://tp.huanxung.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://pp.huanxung.cn

[Q88] 行转列（条件聚合）
来源：http://dd.jianghongdianzi.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hl.nicolike.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://qp.nszjky.cn

[Q89] 判断表是否存在
来源：http://br.bjjhwx.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://bg.9csxet.cn

[Q90] 生成序号列
来源：http://sb.yuntaijiaju.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ga.wgjwhj.cn

================================================================================
来源：http://ys.hahajie.cn

R. Bash 专题
来源：http://ve.nicolike.cn

================================================================================
来源：http://az.huixinmuqiang.cn

[R01] shebang 与严格模式
来源：http://cm.jianghongdianzi.cn

#!/usr/bin/env bash
来源：http://hq.muxihuayi.cn

set -euo pipefail
来源：http://jz.nicolike.cn

[R02] 变量赋值与使用
来源：http://jl.nicolike.cn

name="Tom"; echo "$name"
来源：http://fx.szsharing.cn

[R03] 只读变量
来源：http://lw.szxytkj.cn

readonly PI=3.14
来源：http://vc.bjjhwx.cn

[R04] 位置参数
来源：http://ak.hahajie.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://zd.nszjky.cn

[R05] 参数默认值
来源：http://zd.hnjuh.cn

name="${1:-default}"
来源：http://hc.yuexingan06.cn

[R06] 判断命令是否存在
来源：http://zo.colortex.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://yy.shxzskj.cn

[R07] if 判断文件
来源：http://ua.yuexingan06.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://lv.panjiajie.cn

[R08] 数值比较
来源：http://qk.521024.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://np.hahajie.cn

[R09] 字符串比较
来源：http://hm.huixinmuqiang.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://sz.huixinmuqiang.cn

[R10] 正则匹配
来源：http://yu.shxzskj.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://di.shxzukj.cn

[R11] case 多分支
来源：http://nj.9csxet.cn

case "$1" in
来源：http://oc.jctech888.com.cn

start) echo "启动" ;;
来源：http://dz.newstarts.cn

stop)  echo "停止" ;;
来源：http://wh.asd995.cn

*)     echo "未知命令" ;;
来源：http://mo.chemitech.net.cn

esac
来源：http://dn.nicolike.cn

[R12] for 遍历文件
来源：http://vg.chemitech.net.cn

for f in *.txt; do echo "$f"; done
来源：http://mu.szsharing.cn

[R13] for 计数循环
来源：http://mo.shxzskj.cn

for i in {1..10}; do echo "$i"; done
来源：http://rz.bookmarksfly.cn

[R14] C 风格 for
来源：http://tq.panjiajie.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hh.jianghongdianzi.cn

[R15] while 逐行读文件
来源：http://qa.shtwfgs.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://fy.521024.cn

[R16] until 等待条件
来源：http://cs.szsharing.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://vi.szsharing.cn

[R17] 数组定义与取值
来源：http://gx.colortex.cn

arr=(a b c); echo "${arr[0]}"
来源：http://ck.huixiangedu.cn

[R18] 遍历数组
来源：http://gv.wgjwhj.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://lp.yuntaijiaju.cn

[R19] 数组长度
来源：http://hs.hnjuh.cn


<!-- 参考信息 -->