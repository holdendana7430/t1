代发 wailian999

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ti.szsharing.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://zu.yuexingan06.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mf.hnjuh.cn

[P04] 求长度
来源：http://gv.nszjky.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://lz.jctech888.com.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wc.lnxyls.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://sy.9csxet.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ma.521024.cn

Java: list.size();  map.size();  s.length()
来源：http://zc.szxytkj.cn

Go:   len(arr);  len(m)
来源：http://pe.shxzskj.cn

Ruby: x.length;  x.size
来源：http://fd.9csxet.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://xk.nicolike.cn

[P05] 判断两个对象内容是否相等
来源：http://lt.jianghongdianzi.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://de.szxytkj.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://cm.gzmigu.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ms.muxihuayi.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://lv.bjjhwx.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://zz.shxzukj.cn

Go:   reflect.DeepEqual(a, b)
来源：http://ca.newstarts.cn

Ruby: a == b
来源：http://vu.hahajie.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ni.nszjky.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://oe.huanxung.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://tl.bjjhwx.cn

PHP:  if (empty($x)) {}
来源：http://kw.szsharing.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://cv.huanxung.cn

TS:   if (x == null) {}
来源：http://jp.shxzukj.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://ns.wgjwhj.cn

Go:   if x == nil {}
来源：http://sb.lnxyls.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://go.521024.cn

C#:   if (x is null) {}
来源：http://px.shxzskj.cn

[P07] 防抖与节流
来源：http://xi.asd995.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://uv.muxihuayi.cn

PHP:  // 手写时间戳比较
来源：http://ze.shxzskj.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qt.yuexingan06.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://yq.nicolike.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://nr.muxihuayi.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://if.bjjhwx.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://ly.nszjky.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://pt.panjiajie.cn

[P08] 处理浮点精度问题
来源：http://io.hnjuh.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ws.newstarts.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://vr.nszjky.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://xa.bookmarksfly.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://bu.szxytkj.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://vj.hahajie.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wu.521024.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hx.nicolike.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://sk.bookmarksfly.cn

================================================================================
来源：http://so.jctech888.com.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ng.colortex.cn

================================================================================
来源：http://ic.szsharing.cn

[Q01] 创建表
来源：http://pi.bjjhwx.cn

CREATE TABLE users (
来源：http://lp.yuntaijiaju.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://zy.huixinmuqiang.cn

name VARCHAR(50) NOT NULL,
来源：http://iz.bjjhwx.cn

email VARCHAR(100) UNIQUE,
来源：http://kt.shxzukj.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wr.nszjky.cn

);
来源：http://rk.muxihuayi.cn

[Q02] 创建带外键的表
来源：http://nu.yuexingan06.cn

CREATE TABLE orders (
来源：http://vi.wgjwhj.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://cc.yuntaijiaju.cn

user_id INT NOT NULL,
来源：http://sy.nicolike.cn

amount DECIMAL(10, 2),
来源：http://dg.huanxung.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://gf.chemitech.net.cn

);
来源：http://fa.lnxyls.cn

[Q03] 增加列
来源：http://ac.9csxet.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://oz.yuexingan06.cn

[Q04] 修改列类型
来源：http://wf.bookmarksfly.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mt.shtwfgs.cn

[Q05] 重命名列
来源：http://fk.hahajie.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://kx.jctech888.com.cn

[Q06] 删除列
来源：http://sx.asd995.cn

ALTER TABLE users DROP COLUMN age;
来源：http://ca.panjiajie.cn

[Q07] 删除表
来源：http://dp.chemitech.net.cn

DROP TABLE IF EXISTS orders;
来源：http://ko.nszjky.cn

[Q08] 创建普通索引
来源：http://ye.wgjwhj.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://rc.hnjuh.cn

[Q09] 创建唯一索引
来源：http://ua.newstarts.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ck.9csxet.cn

[Q10] 插入单行
来源：http://zs.panjiajie.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://gf.newstarts.cn

[Q11] 一次插入多行
来源：http://oj.chemitech.net.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ea.shxzukj.cn

[Q12] 插入后取自增 ID
来源：http://zm.asd995.cn

INSERT INTO users (name) VALUES ('C');
来源：http://ey.wgjwhj.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://lw.lnxyls.cn

[Q13] 忽略重复插入
来源：http://ow.huixiangedu.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wq.newstarts.cn

[Q14] 存在则更新（upsert）
来源：http://xw.muxihuayi.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://kf.asd995.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://zr.chemitech.net.cn

[Q15] 查询全部
来源：http://jb.huanxung.cn

SELECT * FROM users;
来源：http://ja.nicolike.cn

[Q16] 查询指定列
来源：http://za.gzmigu.cn

SELECT id, name FROM users;
来源：http://ho.bjjhwx.cn

[Q17] 条件查询
来源：http://ew.chemitech.net.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ib.gzmigu.cn

[Q18] 模糊匹配
来源：http://qv.lnxyls.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ue.bjjhwx.cn

[Q19] 范围查询
来源：http://dd.chemitech.net.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mx.jianghongdianzi.cn

[Q20] IN 列表
来源：http://qa.hnjuh.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ug.yuexingan06.cn

[Q21] 空值判断
来源：http://fw.newstarts.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://aj.haigaiapp.cn

[Q22] 排序
来源：http://ec.panjiajie.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hl.shtwfgs.cn

[Q23] 分页
来源：http://oi.hahajie.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://qp.hahajie.cn

[Q24] 去重
来源：http://ha.muxihuayi.cn

SELECT DISTINCT city FROM users;
来源：http://de.nszjky.cn

[Q25] 只取前 N 条
来源：http://ft.huixinmuqiang.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://jm.huixiangedu.cn

[Q26] 计数
来源：http://ip.panjiajie.cn

SELECT COUNT(*) FROM users;
来源：http://cd.muxihuayi.cn

[Q27] 条件计数
来源：http://jj.muxihuayi.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://rg.panjiajie.cn

[Q28] 求和与平均
来源：http://lj.asd995.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://jk.yuntaijiaju.cn

[Q29] 最大最小值
来源：http://tb.gzmigu.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://vz.jianghongdianzi.cn

[Q30] 分组统计
来源：http://rj.yuexingan06.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://cc.huanxung.cn

[Q31] 分组后过滤
来源：http://gx.newstarts.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://tk.lnxyls.cn

[Q32] 分组拼接字符串
来源：http://xz.521024.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://cb.hnjuh.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://uf.panjiajie.cn

[Q33] 多列分组
来源：http://cn.yuexingan06.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://st.chemitech.net.cn

[Q34] 每组取第一条
来源：http://wt.shxzukj.cn

SELECT * FROM (
来源：http://mg.newstarts.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://vi.shtwfgs.cn

) t WHERE rn = 1;
来源：http://fs.haigaiapp.cn

[Q35] 内连接
来源：http://kc.shxzskj.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://zi.jctech888.com.cn

[Q36] 左连接
来源：http://rm.nicolike.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://vz.asd995.cn

[Q37] 右连接
来源：http://gz.huixiangedu.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://er.yuexingan06.cn

[Q38] 全外连接（PostgreSQL）
来源：http://oz.szxytkj.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://tc.hnjuh.cn

[Q39] 自连接（查上下级）
来源：http://mh.muxihuayi.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://ks.asd995.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ny.huixiangedu.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://rd.bookmarksfly.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://uv.hnjuh.cn

[Q41] 多表连接
来源：http://ca.shtwfgs.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://zj.yuexingan06.cn

JOIN users u ON u.id = o.user_id
来源：http://tp.yuntaijiaju.cn

JOIN products p ON p.id = o.product_id;
来源：http://gp.gzmigu.cn

[Q42] 连接条件附加过滤
来源：http://tx.9csxet.cn

SELECT u.name, o.amount FROM users u
来源：http://ty.521024.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://cc.huixiangedu.cn

[Q43] 标量子查询
来源：http://sv.shtwfgs.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://pr.newstarts.cn

[Q44] IN 子查询
来源：http://ui.9csxet.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://kq.chemitech.net.cn

[Q45] EXISTS 判断存在
来源：http://lr.shxzskj.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://di.bjjhwx.cn

[Q46] NOT EXISTS 判断不存在
来源：http://zg.haigaiapp.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://vx.bookmarksfly.cn

[Q47] 与平均值比较
来源：http://hy.wgjwhj.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ta.muxihuayi.cn

[Q48] CTE 公用表表达式
来源：http://ry.jianghongdianzi.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://dg.newstarts.cn

SELECT * FROM t WHERE c > 5;
来源：http://jv.521024.cn

[Q49] 更新单行
来源：http://ly.jctech888.com.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://pe.hnjuh.cn

[Q50] 批量更新
来源：http://lm.nicolike.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://xi.wgjwhj.cn

[Q51] 用子查询更新
来源：http://ej.hnjuh.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://rk.hahajie.cn

[Q52] 删除指定行
来源：http://lg.newstarts.cn

DELETE FROM users WHERE id = 10;
来源：http://vp.szsharing.cn

[Q53] 按条件删除
来源：http://lj.szxytkj.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://aj.muxihuayi.cn

[Q54] 清空表
来源：http://kx.muxihuayi.cn

TRUNCATE TABLE logs;
来源：http://pq.newstarts.cn

[Q55] 排名（并列占位）
来源：http://es.wgjwhj.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://vc.huixinmuqiang.cn

[Q56] 密集排名（并列不占位）
来源：http://gv.shxzskj.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://yn.szsharing.cn

[Q57] 行号
来源：http://ba.nicolike.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://vj.newstarts.cn

[Q58] 累计求和
来源：http://fb.gzmigu.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://nv.newstarts.cn

[Q59] 分组内累计
来源：http://dt.panjiajie.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://pv.szxytkj.cn

[Q60] 取上一行 / 下一行
来源：http://ny.huanxung.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://gj.hahajie.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hn.szxytkj.cn

[Q61] 移动平均
来源：http://yf.huanxung.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://qu.yuexingan06.cn

[Q62] 分组占比
来源：http://pr.chemitech.net.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://uk.szxytkj.cn

[Q63] 开启事务
来源：http://cj.jctech888.com.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://xj.bjjhwx.cn

[Q64] 提交事务
来源：http://qi.hnjuh.cn

COMMIT;
来源：http://kx.shxzskj.cn

[Q65] 回滚事务
来源：http://vz.nicolike.cn

ROLLBACK;
来源：http://mi.panjiajie.cn

[Q66] 行锁查询
来源：http://tq.jctech888.com.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hj.yuntaijiaju.cn

[Q67] 设置隔离级别
来源：http://tl.bookmarksfly.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://fo.szsharing.cn

[Q68] 保存点
来源：http://lk.hahajie.cn

SAVEPOINT sp1;
来源：http://vt.yuexingan06.cn

ROLLBACK TO sp1;
来源：http://os.jianghongdianzi.cn

[Q69] 查看执行计划
来源：http://nu.colortex.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://cc.colortex.cn

[Q70] 更新统计信息
来源：http://lb.bjjhwx.cn

ANALYZE TABLE users;
来源：http://zj.szxytkj.cn

[Q71] 查看建表语句
来源：http://rc.nszjky.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://uw.haigaiapp.cn

[Q72] 查看索引
来源：http://dq.szxytkj.cn

SHOW INDEX FROM users;
来源：http://yg.yuntaijiaju.cn

[Q73] 查看表状态
来源：http://cu.colortex.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://tl.lnxyls.cn

[Q74] 强制使用索引
来源：http://dq.jctech888.com.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://bj.9csxet.cn

[Q75] 日期格式化
来源：http://md.panjiajie.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ly.shxzukj.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hk.bookmarksfly.cn

[Q76] 按天统计
来源：http://eo.muxihuayi.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ha.yuntaijiaju.cn

[Q77] 时间加减
来源：http://qs.yuexingan06.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://al.shxzukj.cn

[Q78] 当前时间
来源：http://ty.haigaiapp.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://sk.521024.cn

[Q79] 字符串拼接
来源：http://ex.nszjky.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://vy.szxytkj.cn

[Q80] 字符串截取
来源：http://jh.haigaiapp.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ra.newstarts.cn

[Q81] 字符串替换
来源：http://zc.chemitech.net.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://pw.huixiangedu.cn

[Q82] 字符长度与字节长度
来源：http://hj.521024.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wy.chemitech.net.cn

[Q83] 大小写转换
来源：http://lx.lnxyls.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://gu.hnjuh.cn

[Q84] 去除首尾空格
来源：http://pb.newstarts.cn

SELECT TRIM(name) FROM users;
来源：http://os.9csxet.cn

[Q85] 数值取整
来源：http://et.muxihuayi.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://zy.gzmigu.cn

[Q86] 读取 JSON 字段
来源：http://af.szxytkj.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://eb.hnjuh.cn

[Q87] JSON 字段做条件
来源：http://bp.szsharing.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://yq.9csxet.cn

[Q88] 行转列（条件聚合）
来源：http://es.chemitech.net.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://im.muxihuayi.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ny.haigaiapp.cn

[Q89] 判断表是否存在
来源：http://lb.asd995.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://tv.jianghongdianzi.cn

[Q90] 生成序号列
来源：http://ak.bjjhwx.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://gz.hnjuh.cn

================================================================================
来源：http://ct.521024.cn

R. Bash 专题
来源：http://zn.panjiajie.cn

================================================================================
来源：http://hf.521024.cn

[R01] shebang 与严格模式
来源：http://xv.hnjuh.cn

#!/usr/bin/env bash
来源：http://pb.nicolike.cn

set -euo pipefail
来源：http://bx.colortex.cn

[R02] 变量赋值与使用
来源：http://eh.hahajie.cn

name="Tom"; echo "$name"
来源：http://iv.lnxyls.cn

[R03] 只读变量
来源：http://wi.jianghongdianzi.cn

readonly PI=3.14
来源：http://er.hnjuh.cn

[R04] 位置参数
来源：http://xz.wgjwhj.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://fm.yuexingan06.cn

[R05] 参数默认值
来源：http://qi.panjiajie.cn

name="${1:-default}"
来源：http://uc.muxihuayi.cn

[R06] 判断命令是否存在
来源：http://eb.newstarts.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://be.bookmarksfly.cn

[R07] if 判断文件
来源：http://re.szsharing.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://xa.szxytkj.cn

[R08] 数值比较
来源：http://ye.9csxet.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://rj.hahajie.cn

[R09] 字符串比较
来源：http://em.huixiangedu.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://nf.wgjwhj.cn

[R10] 正则匹配
来源：http://gy.jctech888.com.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ft.haigaiapp.cn

[R11] case 多分支
来源：http://tz.shxzukj.cn

case "$1" in
来源：http://wp.bookmarksfly.cn

start) echo "启动" ;;
来源：http://am.yuntaijiaju.cn

stop)  echo "停止" ;;
来源：http://to.newstarts.cn

*)     echo "未知命令" ;;
来源：http://rb.wgjwhj.cn

esac
来源：http://dl.haigaiapp.cn

[R12] for 遍历文件
来源：http://qk.wgjwhj.cn

for f in *.txt; do echo "$f"; done
来源：http://qc.haigaiapp.cn

[R13] for 计数循环
来源：http://qn.shtwfgs.cn

for i in {1..10}; do echo "$i"; done
来源：http://cb.panjiajie.cn

[R14] C 风格 for
来源：http://od.hahajie.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://fe.bookmarksfly.cn

[R15] while 逐行读文件
来源：http://rf.jctech888.com.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://gz.9csxet.cn

[R16] until 等待条件
来源：http://wd.bjjhwx.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://rm.asd995.cn

[R17] 数组定义与取值
来源：http://mh.jctech888.com.cn

arr=(a b c); echo "${arr[0]}"
来源：http://um.jctech888.com.cn

[R18] 遍历数组
来源：http://ni.shxzskj.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://cb.huixinmuqiang.cn

[R19] 数组长度
来源：http://cn.haigaiapp.cn


<!-- 参考信息 -->