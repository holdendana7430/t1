代发 wailian999

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://si.newstarts.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mk.chemitech.net.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://yh.wgjwhj.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://dj.yuexingan06.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ed.bjjhwx.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://kw.panjiajie.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://xg.lnxyls.cn

[P04] 求长度
来源：http://es.yuntaijiaju.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ut.szsharing.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://pr.521024.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ba.colortex.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ms.shtwfgs.cn

Java: list.size();  map.size();  s.length()
来源：http://dl.jianghongdianzi.cn

Go:   len(arr);  len(m)
来源：http://mi.colortex.cn

Ruby: x.length;  x.size
来源：http://xh.jianghongdianzi.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://hy.bjjhwx.cn

[P05] 判断两个对象内容是否相等
来源：http://lh.nszjky.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://zt.yuntaijiaju.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://gf.521024.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://yj.huixinmuqiang.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://nj.huixinmuqiang.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://rg.shxzukj.cn

Go:   reflect.DeepEqual(a, b)
来源：http://ll.panjiajie.cn

Ruby: a == b
来源：http://yo.yuntaijiaju.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://kg.huixiangedu.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://qt.chemitech.net.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://qg.szsharing.cn

PHP:  if (empty($x)) {}
来源：http://dz.chemitech.net.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://nl.nicolike.cn

TS:   if (x == null) {}
来源：http://bt.gzmigu.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://pp.jctech888.com.cn

Go:   if x == nil {}
来源：http://kn.nicolike.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://bf.shxzukj.cn

C#:   if (x is null) {}
来源：http://yo.521024.cn

[P07] 防抖与节流
来源：http://sg.huanxung.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://nq.panjiajie.cn

PHP:  // 手写时间戳比较
来源：http://sr.nicolike.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wi.colortex.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://sp.nicolike.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://kx.newstarts.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://kn.lnxyls.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://vz.muxihuayi.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://lg.haigaiapp.cn

[P08] 处理浮点精度问题
来源：http://wd.huixiangedu.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wm.szsharing.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ck.szxytkj.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://pb.panjiajie.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://xe.colortex.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mu.lnxyls.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://xs.hahajie.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ha.szxytkj.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://qx.521024.cn

================================================================================
来源：http://zb.hahajie.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ai.huixiangedu.cn

================================================================================
来源：http://st.wgjwhj.cn

[Q01] 创建表
来源：http://wf.huixiangedu.cn

CREATE TABLE users (
来源：http://cl.lnxyls.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ml.wgjwhj.cn

name VARCHAR(50) NOT NULL,
来源：http://st.jianghongdianzi.cn

email VARCHAR(100) UNIQUE,
来源：http://ut.shxzukj.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wt.newstarts.cn

);
来源：http://oq.yuexingan06.cn

[Q02] 创建带外键的表
来源：http://bf.newstarts.cn

CREATE TABLE orders (
来源：http://lt.yuntaijiaju.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://af.bookmarksfly.cn

user_id INT NOT NULL,
来源：http://rf.yuntaijiaju.cn

amount DECIMAL(10, 2),
来源：http://nf.szxytkj.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://uj.bjjhwx.cn

);
来源：http://mj.gzmigu.cn

[Q03] 增加列
来源：http://bc.haigaiapp.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://xc.9csxet.cn

[Q04] 修改列类型
来源：http://ib.bookmarksfly.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://rb.9csxet.cn

[Q05] 重命名列
来源：http://vg.szxytkj.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://he.jctech888.com.cn

[Q06] 删除列
来源：http://tj.chemitech.net.cn

ALTER TABLE users DROP COLUMN age;
来源：http://pu.shxzskj.cn

[Q07] 删除表
来源：http://am.hahajie.cn

DROP TABLE IF EXISTS orders;
来源：http://qj.yuntaijiaju.cn

[Q08] 创建普通索引
来源：http://dn.huanxung.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://gd.chemitech.net.cn

[Q09] 创建唯一索引
来源：http://bt.shxzskj.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://bl.colortex.cn

[Q10] 插入单行
来源：http://fi.gzmigu.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://xo.521024.cn

[Q11] 一次插入多行
来源：http://sh.hnjuh.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ft.haigaiapp.cn

[Q12] 插入后取自增 ID
来源：http://aq.gzmigu.cn

INSERT INTO users (name) VALUES ('C');
来源：http://hy.muxihuayi.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://xx.nicolike.cn

[Q13] 忽略重复插入
来源：http://dy.jianghongdianzi.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://fl.9csxet.cn

[Q14] 存在则更新（upsert）
来源：http://wo.gzmigu.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://eg.521024.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://vg.jctech888.com.cn

[Q15] 查询全部
来源：http://dg.newstarts.cn

SELECT * FROM users;
来源：http://br.yuntaijiaju.cn

[Q16] 查询指定列
来源：http://ka.wgjwhj.cn

SELECT id, name FROM users;
来源：http://ta.bookmarksfly.cn

[Q17] 条件查询
来源：http://tz.asd995.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://yl.shtwfgs.cn

[Q18] 模糊匹配
来源：http://qu.yuntaijiaju.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://kc.jianghongdianzi.cn

[Q19] 范围查询
来源：http://re.9csxet.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ll.asd995.cn

[Q20] IN 列表
来源：http://hq.haigaiapp.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://rq.9csxet.cn

[Q21] 空值判断
来源：http://fb.nszjky.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://fw.szsharing.cn

[Q22] 排序
来源：http://am.yuexingan06.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ot.521024.cn

[Q23] 分页
来源：http://ss.bookmarksfly.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ob.bjjhwx.cn

[Q24] 去重
来源：http://pd.chemitech.net.cn

SELECT DISTINCT city FROM users;
来源：http://rt.shxzukj.cn

[Q25] 只取前 N 条
来源：http://nj.wgjwhj.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ur.szsharing.cn

[Q26] 计数
来源：http://le.shxzskj.cn

SELECT COUNT(*) FROM users;
来源：http://zy.bookmarksfly.cn

[Q27] 条件计数
来源：http://ca.huixiangedu.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://cc.521024.cn

[Q28] 求和与平均
来源：http://vp.nszjky.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://eb.huixiangedu.cn

[Q29] 最大最小值
来源：http://og.huixiangedu.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://tx.hnjuh.cn

[Q30] 分组统计
来源：http://xj.colortex.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://af.hahajie.cn

[Q31] 分组后过滤
来源：http://zb.yuntaijiaju.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ns.huixiangedu.cn

[Q32] 分组拼接字符串
来源：http://ke.asd995.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://py.shxzukj.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://js.gzmigu.cn

[Q33] 多列分组
来源：http://uc.nicolike.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://pp.szsharing.cn

[Q34] 每组取第一条
来源：http://mv.szsharing.cn

SELECT * FROM (
来源：http://ad.wgjwhj.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://fc.hnjuh.cn

) t WHERE rn = 1;
来源：http://fg.huanxung.cn

[Q35] 内连接
来源：http://kj.hahajie.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://cb.nicolike.cn

[Q36] 左连接
来源：http://ei.nicolike.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ab.yuexingan06.cn

[Q37] 右连接
来源：http://dg.asd995.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://if.hahajie.cn

[Q38] 全外连接（PostgreSQL）
来源：http://ag.gzmigu.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://sy.hahajie.cn

[Q39] 自连接（查上下级）
来源：http://ao.muxihuayi.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://dw.huixiangedu.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://rs.huixiangedu.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://ut.9csxet.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://jt.yuexingan06.cn

[Q41] 多表连接
来源：http://mm.nszjky.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://ln.bjjhwx.cn

JOIN users u ON u.id = o.user_id
来源：http://tq.haigaiapp.cn

JOIN products p ON p.id = o.product_id;
来源：http://dw.nszjky.cn

[Q42] 连接条件附加过滤
来源：http://xv.wgjwhj.cn

SELECT u.name, o.amount FROM users u
来源：http://jw.yuntaijiaju.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://sv.szsharing.cn

[Q43] 标量子查询
来源：http://py.wgjwhj.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://iu.bookmarksfly.cn

[Q44] IN 子查询
来源：http://kv.wgjwhj.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://qn.nszjky.cn

[Q45] EXISTS 判断存在
来源：http://yk.huixiangedu.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://lf.bookmarksfly.cn

[Q46] NOT EXISTS 判断不存在
来源：http://df.bookmarksfly.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://go.haigaiapp.cn

[Q47] 与平均值比较
来源：http://qd.jctech888.com.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://tk.nicolike.cn

[Q48] CTE 公用表表达式
来源：http://gd.yuexingan06.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ut.lnxyls.cn

SELECT * FROM t WHERE c > 5;
来源：http://cw.szxytkj.cn

[Q49] 更新单行
来源：http://ug.szsharing.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://qa.muxihuayi.cn

[Q50] 批量更新
来源：http://vo.bjjhwx.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://yv.szxytkj.cn

[Q51] 用子查询更新
来源：http://hh.gzmigu.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://kj.huixinmuqiang.cn

[Q52] 删除指定行
来源：http://fq.hahajie.cn

DELETE FROM users WHERE id = 10;
来源：http://tw.shxzukj.cn

[Q53] 按条件删除
来源：http://bs.bjjhwx.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://se.szsharing.cn

[Q54] 清空表
来源：http://nx.chemitech.net.cn

TRUNCATE TABLE logs;
来源：http://kc.bjjhwx.cn

[Q55] 排名（并列占位）
来源：http://ed.huixinmuqiang.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hg.panjiajie.cn

[Q56] 密集排名（并列不占位）
来源：http://by.chemitech.net.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ar.yuexingan06.cn

[Q57] 行号
来源：http://ei.bookmarksfly.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ni.nicolike.cn

[Q58] 累计求和
来源：http://ai.asd995.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://zz.hnjuh.cn

[Q59] 分组内累计
来源：http://sx.hnjuh.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://pr.9csxet.cn

[Q60] 取上一行 / 下一行
来源：http://og.gzmigu.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://cc.yuexingan06.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://er.521024.cn

[Q61] 移动平均
来源：http://oj.asd995.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://lc.shtwfgs.cn

[Q62] 分组占比
来源：http://jb.shxzskj.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://xt.huixiangedu.cn

[Q63] 开启事务
来源：http://gq.huixiangedu.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://lt.shxzskj.cn

[Q64] 提交事务
来源：http://pa.521024.cn

COMMIT;
来源：http://rc.bjjhwx.cn

[Q65] 回滚事务
来源：http://ms.panjiajie.cn

ROLLBACK;
来源：http://ml.newstarts.cn

[Q66] 行锁查询
来源：http://su.huixinmuqiang.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://fq.521024.cn

[Q67] 设置隔离级别
来源：http://mu.muxihuayi.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://du.9csxet.cn

[Q68] 保存点
来源：http://bz.panjiajie.cn

SAVEPOINT sp1;
来源：http://bh.hahajie.cn

ROLLBACK TO sp1;
来源：http://vk.lnxyls.cn

[Q69] 查看执行计划
来源：http://qy.lnxyls.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://nc.bjjhwx.cn

[Q70] 更新统计信息
来源：http://an.newstarts.cn

ANALYZE TABLE users;
来源：http://vk.yuntaijiaju.cn

[Q71] 查看建表语句
来源：http://mw.colortex.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://kk.shtwfgs.cn

[Q72] 查看索引
来源：http://kc.huixinmuqiang.cn

SHOW INDEX FROM users;
来源：http://oa.huanxung.cn

[Q73] 查看表状态
来源：http://fq.panjiajie.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://gd.huanxung.cn

[Q74] 强制使用索引
来源：http://qf.9csxet.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ym.panjiajie.cn

[Q75] 日期格式化
来源：http://xq.gzmigu.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://sc.yuntaijiaju.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hy.bookmarksfly.cn

[Q76] 按天统计
来源：http://tr.huixinmuqiang.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ok.shxzskj.cn

[Q77] 时间加减
来源：http://ia.chemitech.net.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ga.nszjky.cn

[Q78] 当前时间
来源：http://wo.newstarts.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://pf.panjiajie.cn

[Q79] 字符串拼接
来源：http://fh.yuntaijiaju.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ed.9csxet.cn

[Q80] 字符串截取
来源：http://jp.yuntaijiaju.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://pt.yuntaijiaju.cn

[Q81] 字符串替换
来源：http://yq.shxzukj.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://kc.yuntaijiaju.cn

[Q82] 字符长度与字节长度
来源：http://nk.chemitech.net.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://yq.huixinmuqiang.cn

[Q83] 大小写转换
来源：http://nf.gzmigu.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://cx.yuntaijiaju.cn

[Q84] 去除首尾空格
来源：http://um.hnjuh.cn

SELECT TRIM(name) FROM users;
来源：http://rj.wgjwhj.cn

[Q85] 数值取整
来源：http://be.nicolike.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://tc.nicolike.cn

[Q86] 读取 JSON 字段
来源：http://cw.jctech888.com.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://al.lnxyls.cn

[Q87] JSON 字段做条件
来源：http://ud.jianghongdianzi.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://sl.hnjuh.cn

[Q88] 行转列（条件聚合）
来源：http://cr.bjjhwx.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://xg.shtwfgs.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ty.gzmigu.cn

[Q89] 判断表是否存在
来源：http://xp.huixinmuqiang.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hr.hnjuh.cn

[Q90] 生成序号列
来源：http://sc.huixiangedu.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://le.jianghongdianzi.cn

================================================================================
来源：http://tm.huixinmuqiang.cn

R. Bash 专题
来源：http://nf.colortex.cn

================================================================================
来源：http://dx.asd995.cn

[R01] shebang 与严格模式
来源：http://ip.9csxet.cn

#!/usr/bin/env bash
来源：http://yg.nicolike.cn

set -euo pipefail
来源：http://oh.yuexingan06.cn

[R02] 变量赋值与使用
来源：http://qn.chemitech.net.cn

name="Tom"; echo "$name"
来源：http://xm.shxzukj.cn

[R03] 只读变量
来源：http://yd.huanxung.cn

readonly PI=3.14
来源：http://tc.nicolike.cn

[R04] 位置参数
来源：http://rr.szxytkj.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hu.9csxet.cn

[R05] 参数默认值
来源：http://rt.muxihuayi.cn

name="${1:-default}"
来源：http://xo.hnjuh.cn

[R06] 判断命令是否存在
来源：http://pt.bookmarksfly.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://vb.jctech888.com.cn

[R07] if 判断文件
来源：http://un.bjjhwx.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ry.shtwfgs.cn

[R08] 数值比较
来源：http://rq.bjjhwx.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://yw.9csxet.cn

[R09] 字符串比较
来源：http://du.gzmigu.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://kn.9csxet.cn

[R10] 正则匹配
来源：http://fl.bjjhwx.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://io.haigaiapp.cn

[R11] case 多分支
来源：http://ba.colortex.cn

case "$1" in
来源：http://mb.hnjuh.cn

start) echo "启动" ;;
来源：http://yy.huanxung.cn

stop)  echo "停止" ;;
来源：http://jg.colortex.cn

*)     echo "未知命令" ;;
来源：http://nv.szsharing.cn

esac
来源：http://oh.jianghongdianzi.cn

[R12] for 遍历文件
来源：http://oj.bookmarksfly.cn

for f in *.txt; do echo "$f"; done
来源：http://nz.jctech888.com.cn

[R13] for 计数循环
来源：http://jr.521024.cn

for i in {1..10}; do echo "$i"; done
来源：http://ut.bjjhwx.cn

[R14] C 风格 for
来源：http://lc.9csxet.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://vu.nicolike.cn

[R15] while 逐行读文件
来源：http://wt.muxihuayi.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://fz.szsharing.cn

[R16] until 等待条件
来源：http://fr.lnxyls.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://sm.nszjky.cn

[R17] 数组定义与取值
来源：http://wr.bookmarksfly.cn


<!-- 参考信息 -->