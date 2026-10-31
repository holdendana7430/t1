代发 wailian999

Ruby: Digest::SHA256.hexdigest(s)
来源：http://zc.huanxung.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hx.nszjky.cn

[P03] 生成短随机字符串
来源：http://ca.shxzukj.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://nf.521024.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hb.hnjuh.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ab.nicolike.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://dv.bjjhwx.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://iu.lnxyls.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wd.nszjky.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://fn.chemitech.net.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ep.bjjhwx.cn

[P04] 求长度
来源：http://jo.521024.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://zt.lnxyls.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://gz.jianghongdianzi.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://xs.shtwfgs.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://si.lnxyls.cn

Java: list.size();  map.size();  s.length()
来源：http://pl.colortex.cn

Go:   len(arr);  len(m)
来源：http://pe.chemitech.net.cn

Ruby: x.length;  x.size
来源：http://ly.hahajie.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://am.shxzskj.cn

[P05] 判断两个对象内容是否相等
来源：http://eq.wgjwhj.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://ca.lnxyls.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://xg.wgjwhj.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://os.szxytkj.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ix.chemitech.net.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ms.bookmarksfly.cn

Go:   reflect.DeepEqual(a, b)
来源：http://gb.hahajie.cn

Ruby: a == b
来源：http://yp.bjjhwx.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://sm.hahajie.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://zy.bjjhwx.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ua.muxihuayi.cn

PHP:  if (empty($x)) {}
来源：http://bo.panjiajie.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://zs.gzmigu.cn

TS:   if (x == null) {}
来源：http://rp.muxihuayi.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://py.szsharing.cn

Go:   if x == nil {}
来源：http://fv.huanxung.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ig.yuexingan06.cn

C#:   if (x is null) {}
来源：http://zr.chemitech.net.cn

[P07] 防抖与节流
来源：http://tp.newstarts.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://jh.shtwfgs.cn

PHP:  // 手写时间戳比较
来源：http://sr.wgjwhj.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://cl.huanxung.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://bb.wgjwhj.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://jo.muxihuayi.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ld.huixiangedu.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://is.521024.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://zl.9csxet.cn

[P08] 处理浮点精度问题
来源：http://ge.szxytkj.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://au.hahajie.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://bf.wgjwhj.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://iz.panjiajie.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wo.nicolike.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://lc.shxzskj.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.bookmarksfly.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ev.nicolike.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://af.gzmigu.cn

================================================================================
来源：http://yy.yuexingan06.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://zp.yuexingan06.cn

================================================================================
来源：http://fi.gzmigu.cn

[Q01] 创建表
来源：http://du.shxzskj.cn

CREATE TABLE users (
来源：http://tb.jianghongdianzi.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://sl.huanxung.cn

name VARCHAR(50) NOT NULL,
来源：http://bz.haigaiapp.cn

email VARCHAR(100) UNIQUE,
来源：http://hy.bjjhwx.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://tx.jctech888.com.cn

);
来源：http://qq.szxytkj.cn

[Q02] 创建带外键的表
来源：http://no.hahajie.cn

CREATE TABLE orders (
来源：http://br.yuntaijiaju.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://dd.shxzukj.cn

user_id INT NOT NULL,
来源：http://gg.newstarts.cn

amount DECIMAL(10, 2),
来源：http://cj.huixiangedu.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://lk.wgjwhj.cn

);
来源：http://lx.hahajie.cn

[Q03] 增加列
来源：http://nu.muxihuayi.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://vz.jctech888.com.cn

[Q04] 修改列类型
来源：http://vs.huixinmuqiang.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://gc.huanxung.cn

[Q05] 重命名列
来源：http://nf.haigaiapp.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://vr.521024.cn

[Q06] 删除列
来源：http://bu.szsharing.cn

ALTER TABLE users DROP COLUMN age;
来源：http://kx.huixiangedu.cn

[Q07] 删除表
来源：http://wj.shxzukj.cn

DROP TABLE IF EXISTS orders;
来源：http://xx.haigaiapp.cn

[Q08] 创建普通索引
来源：http://yn.yuntaijiaju.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://ij.huixinmuqiang.cn

[Q09] 创建唯一索引
来源：http://yr.shxzskj.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://il.hahajie.cn

[Q10] 插入单行
来源：http://xq.huixiangedu.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://jy.yuexingan06.cn

[Q11] 一次插入多行
来源：http://he.huixiangedu.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://tm.asd995.cn

[Q12] 插入后取自增 ID
来源：http://kk.haigaiapp.cn

INSERT INTO users (name) VALUES ('C');
来源：http://tq.muxihuayi.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://gt.shxzskj.cn

[Q13] 忽略重复插入
来源：http://ur.yuntaijiaju.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://bu.szsharing.cn

[Q14] 存在则更新（upsert）
来源：http://ug.szsharing.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://dp.huixiangedu.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://lj.yuntaijiaju.cn

[Q15] 查询全部
来源：http://ji.chemitech.net.cn

SELECT * FROM users;
来源：http://fh.newstarts.cn

[Q16] 查询指定列
来源：http://ou.asd995.cn

SELECT id, name FROM users;
来源：http://uw.shxzskj.cn

[Q17] 条件查询
来源：http://ik.yuntaijiaju.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://xi.huixiangedu.cn

[Q18] 模糊匹配
来源：http://re.chemitech.net.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://we.bookmarksfly.cn

[Q19] 范围查询
来源：http://kc.bjjhwx.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ef.9csxet.cn

[Q20] IN 列表
来源：http://ek.szsharing.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ak.wgjwhj.cn

[Q21] 空值判断
来源：http://lh.yuexingan06.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://xw.haigaiapp.cn

[Q22] 排序
来源：http://qb.521024.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ua.gzmigu.cn

[Q23] 分页
来源：http://gu.szxytkj.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.asd995.cn

[Q24] 去重
来源：http://ce.huanxung.cn

SELECT DISTINCT city FROM users;
来源：http://va.hnjuh.cn

[Q25] 只取前 N 条
来源：http://mm.haigaiapp.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://vb.nicolike.cn

[Q26] 计数
来源：http://cl.521024.cn

SELECT COUNT(*) FROM users;
来源：http://vo.yuntaijiaju.cn

[Q27] 条件计数
来源：http://sw.hnjuh.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://pb.521024.cn

[Q28] 求和与平均
来源：http://pz.hnjuh.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://io.wgjwhj.cn

[Q29] 最大最小值
来源：http://xa.huixinmuqiang.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://yh.nicolike.cn

[Q30] 分组统计
来源：http://qz.szsharing.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://nh.hahajie.cn

[Q31] 分组后过滤
来源：http://sf.shtwfgs.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://qe.muxihuayi.cn

[Q32] 分组拼接字符串
来源：http://wd.newstarts.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://zz.9csxet.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://cw.chemitech.net.cn

[Q33] 多列分组
来源：http://vm.colortex.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mq.bjjhwx.cn

[Q34] 每组取第一条
来源：http://kb.asd995.cn

SELECT * FROM (
来源：http://bx.panjiajie.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://pk.muxihuayi.cn

) t WHERE rn = 1;
来源：http://cd.bookmarksfly.cn

[Q35] 内连接
来源：http://gy.wgjwhj.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://zq.wgjwhj.cn

[Q36] 左连接
来源：http://of.shxzskj.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wo.huixiangedu.cn

[Q37] 右连接
来源：http://ku.shxzskj.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wa.bookmarksfly.cn

[Q38] 全外连接（PostgreSQL）
来源：http://pq.panjiajie.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://av.521024.cn

[Q39] 自连接（查上下级）
来源：http://fk.shxzukj.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://ok.521024.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://pw.szsharing.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://os.huixinmuqiang.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://rt.hnjuh.cn

[Q41] 多表连接
来源：http://vl.bjjhwx.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://xz.hnjuh.cn

JOIN users u ON u.id = o.user_id
来源：http://ha.huixiangedu.cn

JOIN products p ON p.id = o.product_id;
来源：http://qv.gzmigu.cn

[Q42] 连接条件附加过滤
来源：http://oz.colortex.cn

SELECT u.name, o.amount FROM users u
来源：http://nq.hnjuh.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://dq.chemitech.net.cn

[Q43] 标量子查询
来源：http://oi.szsharing.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://fk.yuexingan06.cn

[Q44] IN 子查询
来源：http://os.521024.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://gi.nszjky.cn

[Q45] EXISTS 判断存在
来源：http://kb.yuntaijiaju.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://vs.szxytkj.cn

[Q46] NOT EXISTS 判断不存在
来源：http://jz.asd995.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://co.yuexingan06.cn

[Q47] 与平均值比较
来源：http://vp.szsharing.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://qp.colortex.cn

[Q48] CTE 公用表表达式
来源：http://ch.newstarts.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ok.9csxet.cn

SELECT * FROM t WHERE c > 5;
来源：http://sj.wgjwhj.cn

[Q49] 更新单行
来源：http://nw.shxzukj.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://jo.haigaiapp.cn

[Q50] 批量更新
来源：http://mq.newstarts.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mj.shxzukj.cn

[Q51] 用子查询更新
来源：http://cp.huanxung.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://yq.huixiangedu.cn

[Q52] 删除指定行
来源：http://tq.shxzukj.cn

DELETE FROM users WHERE id = 10;
来源：http://ew.jianghongdianzi.cn

[Q53] 按条件删除
来源：http://sh.9csxet.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://rh.asd995.cn

[Q54] 清空表
来源：http://me.panjiajie.cn

TRUNCATE TABLE logs;
来源：http://ke.huanxung.cn

[Q55] 排名（并列占位）
来源：http://cr.szxytkj.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ja.wgjwhj.cn

[Q56] 密集排名（并列不占位）
来源：http://ex.newstarts.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://bo.szsharing.cn

[Q57] 行号
来源：http://ur.huixinmuqiang.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://li.szxytkj.cn

[Q58] 累计求和
来源：http://xb.colortex.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://tu.asd995.cn

[Q59] 分组内累计
来源：http://mq.colortex.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://nh.lnxyls.cn

[Q60] 取上一行 / 下一行
来源：http://eh.yuexingan06.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://gy.wgjwhj.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ew.asd995.cn

[Q61] 移动平均
来源：http://cm.bookmarksfly.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ml.huanxung.cn

[Q62] 分组占比
来源：http://ah.bjjhwx.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://yi.szxytkj.cn

[Q63] 开启事务
来源：http://fd.muxihuayi.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://ud.asd995.cn

[Q64] 提交事务
来源：http://ck.szsharing.cn

COMMIT;
来源：http://cn.haigaiapp.cn

[Q65] 回滚事务
来源：http://ze.shtwfgs.cn

ROLLBACK;
来源：http://py.asd995.cn

[Q66] 行锁查询
来源：http://ue.lnxyls.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://vc.szxytkj.cn

[Q67] 设置隔离级别
来源：http://cf.shxzukj.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ib.yuntaijiaju.cn

[Q68] 保存点
来源：http://gh.jianghongdianzi.cn

SAVEPOINT sp1;
来源：http://qp.huanxung.cn

ROLLBACK TO sp1;
来源：http://hb.hahajie.cn

[Q69] 查看执行计划
来源：http://pn.yuntaijiaju.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://uk.bjjhwx.cn

[Q70] 更新统计信息
来源：http://uk.huixinmuqiang.cn

ANALYZE TABLE users;
来源：http://jz.shxzukj.cn

[Q71] 查看建表语句
来源：http://if.hnjuh.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wh.shtwfgs.cn

[Q72] 查看索引
来源：http://gy.huixinmuqiang.cn

SHOW INDEX FROM users;
来源：http://pb.gzmigu.cn

[Q73] 查看表状态
来源：http://ng.hahajie.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://gk.bjjhwx.cn

[Q74] 强制使用索引
来源：http://ry.hnjuh.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://tb.bookmarksfly.cn

[Q75] 日期格式化
来源：http://lo.jctech888.com.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://pl.nicolike.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://qo.huixinmuqiang.cn

[Q76] 按天统计
来源：http://qe.jianghongdianzi.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://na.nicolike.cn

[Q77] 时间加减
来源：http://wa.lnxyls.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://uu.jianghongdianzi.cn

[Q78] 当前时间
来源：http://hj.wgjwhj.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://tr.shtwfgs.cn

[Q79] 字符串拼接
来源：http://ev.jianghongdianzi.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://cw.szsharing.cn

[Q80] 字符串截取
来源：http://at.lnxyls.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://cm.newstarts.cn

[Q81] 字符串替换
来源：http://fd.chemitech.net.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ot.nicolike.cn

[Q82] 字符长度与字节长度
来源：http://ph.huixiangedu.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://qy.nicolike.cn

[Q83] 大小写转换
来源：http://lk.jianghongdianzi.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://pe.szxytkj.cn

[Q84] 去除首尾空格
来源：http://fo.shxzskj.cn

SELECT TRIM(name) FROM users;
来源：http://sv.shxzskj.cn

[Q85] 数值取整
来源：http://jq.yuexingan06.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://fw.shxzskj.cn

[Q86] 读取 JSON 字段
来源：http://cw.hahajie.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ix.hnjuh.cn

[Q87] JSON 字段做条件
来源：http://jd.chemitech.net.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://gb.huixiangedu.cn

[Q88] 行转列（条件聚合）
来源：http://cv.hahajie.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://xr.hnjuh.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mv.jctech888.com.cn

[Q89] 判断表是否存在
来源：http://si.szxytkj.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://xi.yuntaijiaju.cn

[Q90] 生成序号列
来源：http://qj.colortex.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://cf.szxytkj.cn

================================================================================
来源：http://yl.panjiajie.cn

R. Bash 专题
来源：http://nd.panjiajie.cn

================================================================================
来源：http://jp.jianghongdianzi.cn

[R01] shebang 与严格模式
来源：http://ws.yuntaijiaju.cn

#!/usr/bin/env bash
来源：http://mz.szsharing.cn

set -euo pipefail
来源：http://qa.shxzskj.cn

[R02] 变量赋值与使用
来源：http://if.asd995.cn

name="Tom"; echo "$name"
来源：http://nr.asd995.cn

[R03] 只读变量
来源：http://bb.huixiangedu.cn

readonly PI=3.14
来源：http://dg.muxihuayi.cn

[R04] 位置参数
来源：http://qs.yuexingan06.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://vb.huanxung.cn

[R05] 参数默认值
来源：http://kr.shtwfgs.cn

name="${1:-default}"
来源：http://ff.huixinmuqiang.cn

[R06] 判断命令是否存在
来源：http://go.asd995.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://fn.jianghongdianzi.cn

[R07] if 判断文件
来源：http://cc.huixiangedu.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://nr.jctech888.com.cn

[R08] 数值比较
来源：http://rx.asd995.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://eq.huanxung.cn

[R09] 字符串比较
来源：http://pp.huanxung.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://nk.hnjuh.cn

[R10] 正则匹配
来源：http://xr.muxihuayi.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://om.bjjhwx.cn

[R11] case 多分支
来源：http://ca.521024.cn

case "$1" in
来源：http://cp.bjjhwx.cn

start) echo "启动" ;;
来源：http://tw.szxytkj.cn

stop)  echo "停止" ;;
来源：http://ft.bookmarksfly.cn

*)     echo "未知命令" ;;
来源：http://cf.haigaiapp.cn

esac
来源：http://ef.yuntaijiaju.cn

[R12] for 遍历文件
来源：http://my.chemitech.net.cn

for f in *.txt; do echo "$f"; done
来源：http://od.hnjuh.cn

[R13] for 计数循环
来源：http://cm.nicolike.cn

for i in {1..10}; do echo "$i"; done
来源：http://de.bookmarksfly.cn

[R14] C 风格 for
来源：http://rq.jianghongdianzi.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://qp.huanxung.cn

[R15] while 逐行读文件
来源：http://dz.nszjky.cn


<!-- 参考信息 -->