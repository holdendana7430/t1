代发 wailian999

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mx.nicolike.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://sq.bjjhwx.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://jc.asd995.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://kj.bjjhwx.cn

Java: list.size();  map.size();  s.length()
来源：http://oh.wgjwhj.cn

Go:   len(arr);  len(m)
来源：http://te.lnxyls.cn

Ruby: x.length;  x.size
来源：http://ft.shxzukj.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://vo.newstarts.cn

[P05] 判断两个对象内容是否相等
来源：http://ro.9csxet.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://jr.jianghongdianzi.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://xd.shtwfgs.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://or.newstarts.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://vs.shxzskj.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ns.bookmarksfly.cn

Go:   reflect.DeepEqual(a, b)
来源：http://fa.nszjky.cn

Ruby: a == b
来源：http://vr.9csxet.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://kj.szsharing.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://kb.haigaiapp.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hy.9csxet.cn

PHP:  if (empty($x)) {}
来源：http://of.yuntaijiaju.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ar.muxihuayi.cn

TS:   if (x == null) {}
来源：http://lw.panjiajie.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://rl.hahajie.cn

Go:   if x == nil {}
来源：http://rb.521024.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://cx.hahajie.cn

C#:   if (x is null) {}
来源：http://bc.hahajie.cn

[P07] 防抖与节流
来源：http://op.shxzukj.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://tw.wgjwhj.cn

PHP:  // 手写时间戳比较
来源：http://mm.nszjky.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://sh.521024.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://cw.shxzukj.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://fp.521024.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://jv.nszjky.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://bt.9csxet.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://jj.panjiajie.cn

[P08] 处理浮点精度问题
来源：http://fr.huanxung.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://sl.bookmarksfly.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://bf.shtwfgs.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wx.huixiangedu.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://df.jctech888.com.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://to.nicolike.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mj.bjjhwx.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://se.panjiajie.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mo.asd995.cn

================================================================================
来源：http://el.521024.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://rx.newstarts.cn

================================================================================
来源：http://ye.hahajie.cn

[Q01] 创建表
来源：http://mx.newstarts.cn

CREATE TABLE users (
来源：http://wm.muxihuayi.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://px.gzmigu.cn

name VARCHAR(50) NOT NULL,
来源：http://yu.9csxet.cn

email VARCHAR(100) UNIQUE,
来源：http://hf.haigaiapp.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://zb.szxytkj.cn

);
来源：http://xz.colortex.cn

[Q02] 创建带外键的表
来源：http://xs.shtwfgs.cn

CREATE TABLE orders (
来源：http://qi.panjiajie.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://oj.shxzskj.cn

user_id INT NOT NULL,
来源：http://xg.szxytkj.cn

amount DECIMAL(10, 2),
来源：http://jf.haigaiapp.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://cg.bjjhwx.cn

);
来源：http://om.panjiajie.cn

[Q03] 增加列
来源：http://st.521024.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://xb.521024.cn

[Q04] 修改列类型
来源：http://qf.shtwfgs.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://zw.gzmigu.cn

[Q05] 重命名列
来源：http://nn.shxzukj.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://nj.nszjky.cn

[Q06] 删除列
来源：http://mz.muxihuayi.cn

ALTER TABLE users DROP COLUMN age;
来源：http://zp.haigaiapp.cn

[Q07] 删除表
来源：http://bo.gzmigu.cn

DROP TABLE IF EXISTS orders;
来源：http://ps.wgjwhj.cn

[Q08] 创建普通索引
来源：http://ry.yuexingan06.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://ql.huixiangedu.cn

[Q09] 创建唯一索引
来源：http://tx.wgjwhj.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://bg.bookmarksfly.cn

[Q10] 插入单行
来源：http://lw.muxihuayi.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ce.newstarts.cn

[Q11] 一次插入多行
来源：http://zp.colortex.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://eh.muxihuayi.cn

[Q12] 插入后取自增 ID
来源：http://va.nszjky.cn

INSERT INTO users (name) VALUES ('C');
来源：http://ob.huixiangedu.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://bm.huixinmuqiang.cn

[Q13] 忽略重复插入
来源：http://ds.chemitech.net.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://em.colortex.cn

[Q14] 存在则更新（upsert）
来源：http://wj.szsharing.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://vv.521024.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://fk.asd995.cn

[Q15] 查询全部
来源：http://pn.colortex.cn

SELECT * FROM users;
来源：http://ux.szxytkj.cn

[Q16] 查询指定列
来源：http://ff.panjiajie.cn

SELECT id, name FROM users;
来源：http://og.shxzskj.cn

[Q17] 条件查询
来源：http://wi.huixinmuqiang.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://qr.hnjuh.cn

[Q18] 模糊匹配
来源：http://ed.yuntaijiaju.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://no.szxytkj.cn

[Q19] 范围查询
来源：http://bv.huixinmuqiang.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wt.bjjhwx.cn

[Q20] IN 列表
来源：http://cp.bookmarksfly.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://tf.9csxet.cn

[Q21] 空值判断
来源：http://cx.asd995.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://kr.chemitech.net.cn

[Q22] 排序
来源：http://gc.521024.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://sm.newstarts.cn

[Q23] 分页
来源：http://fr.wgjwhj.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://us.hnjuh.cn

[Q24] 去重
来源：http://fu.colortex.cn

SELECT DISTINCT city FROM users;
来源：http://zj.yuexingan06.cn

[Q25] 只取前 N 条
来源：http://pb.hnjuh.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://eg.panjiajie.cn

[Q26] 计数
来源：http://xo.nszjky.cn

SELECT COUNT(*) FROM users;
来源：http://xd.shxzukj.cn

[Q27] 条件计数
来源：http://mm.lnxyls.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ev.panjiajie.cn

[Q28] 求和与平均
来源：http://nl.huixinmuqiang.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://jp.shxzskj.cn

[Q29] 最大最小值
来源：http://by.huixinmuqiang.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://ab.lnxyls.cn

[Q30] 分组统计
来源：http://re.newstarts.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://tu.hnjuh.cn

[Q31] 分组后过滤
来源：http://sa.hahajie.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://xx.shtwfgs.cn

[Q32] 分组拼接字符串
来源：http://so.bjjhwx.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ai.shtwfgs.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://el.wgjwhj.cn

[Q33] 多列分组
来源：http://qd.yuexingan06.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://gm.9csxet.cn

[Q34] 每组取第一条
来源：http://bw.asd995.cn

SELECT * FROM (
来源：http://mz.9csxet.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://jy.nszjky.cn

) t WHERE rn = 1;
来源：http://zn.huanxung.cn

[Q35] 内连接
来源：http://ta.nszjky.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://qh.shxzskj.cn

[Q36] 左连接
来源：http://qq.shxzukj.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://kp.asd995.cn

[Q37] 右连接
来源：http://dr.asd995.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://dm.hahajie.cn

[Q38] 全外连接（PostgreSQL）
来源：http://ua.lnxyls.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://as.9csxet.cn

[Q39] 自连接（查上下级）
来源：http://gw.haigaiapp.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://ue.lnxyls.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://sb.szsharing.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://wl.9csxet.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://jt.nszjky.cn

[Q41] 多表连接
来源：http://xk.yuexingan06.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://it.chemitech.net.cn

JOIN users u ON u.id = o.user_id
来源：http://hj.shxzukj.cn

JOIN products p ON p.id = o.product_id;
来源：http://nu.shxzskj.cn

[Q42] 连接条件附加过滤
来源：http://dm.bjjhwx.cn

SELECT u.name, o.amount FROM users u
来源：http://jo.lnxyls.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://kh.chemitech.net.cn

[Q43] 标量子查询
来源：http://rr.jctech888.com.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://zh.wgjwhj.cn

[Q44] IN 子查询
来源：http://sz.jianghongdianzi.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://zw.chemitech.net.cn

[Q45] EXISTS 判断存在
来源：http://ho.nicolike.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://os.nicolike.cn

[Q46] NOT EXISTS 判断不存在
来源：http://hx.hnjuh.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://bg.521024.cn

[Q47] 与平均值比较
来源：http://bh.shxzukj.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://jg.yuexingan06.cn

[Q48] CTE 公用表表达式
来源：http://pt.521024.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://fn.asd995.cn

SELECT * FROM t WHERE c > 5;
来源：http://mu.lnxyls.cn

[Q49] 更新单行
来源：http://pj.panjiajie.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://yx.panjiajie.cn

[Q50] 批量更新
来源：http://en.shxzskj.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://fi.haigaiapp.cn

[Q51] 用子查询更新
来源：http://sg.9csxet.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://cg.jianghongdianzi.cn

[Q52] 删除指定行
来源：http://tc.9csxet.cn

DELETE FROM users WHERE id = 10;
来源：http://mg.newstarts.cn

[Q53] 按条件删除
来源：http://ef.panjiajie.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://gp.nicolike.cn

[Q54] 清空表
来源：http://xg.haigaiapp.cn

TRUNCATE TABLE logs;
来源：http://qf.gzmigu.cn

[Q55] 排名（并列占位）
来源：http://vo.szxytkj.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://da.panjiajie.cn

[Q56] 密集排名（并列不占位）
来源：http://cz.chemitech.net.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://yp.jctech888.com.cn

[Q57] 行号
来源：http://ev.newstarts.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://cl.yuntaijiaju.cn

[Q58] 累计求和
来源：http://rt.nicolike.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://lh.newstarts.cn

[Q59] 分组内累计
来源：http://uq.huixinmuqiang.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ko.muxihuayi.cn

[Q60] 取上一行 / 下一行
来源：http://cb.huanxung.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://if.shtwfgs.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://dx.yuexingan06.cn

[Q61] 移动平均
来源：http://oc.huixiangedu.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://zo.bookmarksfly.cn

[Q62] 分组占比
来源：http://lw.gzmigu.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wy.bookmarksfly.cn

[Q63] 开启事务
来源：http://tv.colortex.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://ue.yuntaijiaju.cn

[Q64] 提交事务
来源：http://cu.colortex.cn

COMMIT;
来源：http://gv.szsharing.cn

[Q65] 回滚事务
来源：http://rq.nicolike.cn

ROLLBACK;
来源：http://ys.nszjky.cn

[Q66] 行锁查询
来源：http://re.bookmarksfly.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://li.yuexingan06.cn

[Q67] 设置隔离级别
来源：http://zg.9csxet.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://qz.hnjuh.cn

[Q68] 保存点
来源：http://yu.asd995.cn

SAVEPOINT sp1;
来源：http://dd.colortex.cn

ROLLBACK TO sp1;
来源：http://mk.hnjuh.cn

[Q69] 查看执行计划
来源：http://cb.yuntaijiaju.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ov.nszjky.cn

[Q70] 更新统计信息
来源：http://nu.panjiajie.cn

ANALYZE TABLE users;
来源：http://xt.jctech888.com.cn

[Q71] 查看建表语句
来源：http://fk.asd995.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://rk.newstarts.cn

[Q72] 查看索引
来源：http://wd.asd995.cn

SHOW INDEX FROM users;
来源：http://qc.lnxyls.cn

[Q73] 查看表状态
来源：http://dt.jianghongdianzi.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://ah.szxytkj.cn

[Q74] 强制使用索引
来源：http://na.huixiangedu.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://gz.muxihuayi.cn

[Q75] 日期格式化
来源：http://ck.colortex.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://op.hnjuh.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://jz.huixiangedu.cn

[Q76] 按天统计
来源：http://gc.szsharing.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wf.panjiajie.cn

[Q77] 时间加减
来源：http://kk.szsharing.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ey.gzmigu.cn

[Q78] 当前时间
来源：http://if.nicolike.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://lh.huixinmuqiang.cn

[Q79] 字符串拼接
来源：http://uy.bookmarksfly.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://zn.chemitech.net.cn

[Q80] 字符串截取
来源：http://ck.jctech888.com.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ip.muxihuayi.cn

[Q81] 字符串替换
来源：http://wm.chemitech.net.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://gx.hnjuh.cn

[Q82] 字符长度与字节长度
来源：http://lb.huixinmuqiang.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://co.hnjuh.cn

[Q83] 大小写转换
来源：http://rk.hahajie.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://vn.panjiajie.cn

[Q84] 去除首尾空格
来源：http://vn.colortex.cn

SELECT TRIM(name) FROM users;
来源：http://tq.521024.cn

[Q85] 数值取整
来源：http://fy.szsharing.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://pb.shxzskj.cn

[Q86] 读取 JSON 字段
来源：http://hl.huanxung.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wl.jctech888.com.cn

[Q87] JSON 字段做条件
来源：http://js.hnjuh.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mp.szxytkj.cn

[Q88] 行转列（条件聚合）
来源：http://ea.yuexingan06.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wm.panjiajie.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hv.lnxyls.cn

[Q89] 判断表是否存在
来源：http://qo.huixiangedu.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://xj.colortex.cn

[Q90] 生成序号列
来源：http://cx.shxzukj.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mk.shxzskj.cn

================================================================================
来源：http://of.hnjuh.cn

R. Bash 专题
来源：http://yv.jctech888.com.cn

================================================================================
来源：http://mc.huanxung.cn

[R01] shebang 与严格模式
来源：http://vy.panjiajie.cn

#!/usr/bin/env bash
来源：http://rs.lnxyls.cn

set -euo pipefail
来源：http://ct.shtwfgs.cn

[R02] 变量赋值与使用
来源：http://ep.hnjuh.cn

name="Tom"; echo "$name"
来源：http://yu.hnjuh.cn

[R03] 只读变量
来源：http://pn.panjiajie.cn

readonly PI=3.14
来源：http://as.gzmigu.cn

[R04] 位置参数
来源：http://km.huanxung.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://fk.yuntaijiaju.cn

[R05] 参数默认值
来源：http://sl.wgjwhj.cn

name="${1:-default}"
来源：http://lt.huixiangedu.cn

[R06] 判断命令是否存在
来源：http://xf.szxytkj.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://xj.yuntaijiaju.cn

[R07] if 判断文件
来源：http://em.newstarts.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ze.huanxung.cn

[R08] 数值比较
来源：http://rc.muxihuayi.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://ax.521024.cn

[R09] 字符串比较
来源：http://sx.szxytkj.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://yp.lnxyls.cn

[R10] 正则匹配
来源：http://go.shxzskj.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://of.jctech888.com.cn

[R11] case 多分支
来源：http://md.huanxung.cn

case "$1" in
来源：http://rg.huanxung.cn

start) echo "启动" ;;
来源：http://vy.asd995.cn

stop)  echo "停止" ;;
来源：http://bm.yuntaijiaju.cn

*)     echo "未知命令" ;;
来源：http://en.hahajie.cn

esac
来源：http://ks.szsharing.cn

[R12] for 遍历文件
来源：http://up.muxihuayi.cn

for f in *.txt; do echo "$f"; done
来源：http://hz.jctech888.com.cn

[R13] for 计数循环
来源：http://de.szxytkj.cn

for i in {1..10}; do echo "$i"; done
来源：http://ec.bookmarksfly.cn

[R14] C 风格 for
来源：http://mu.hahajie.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://sz.huanxung.cn

[R15] while 逐行读文件
来源：http://wc.colortex.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://cf.shxzskj.cn

[R16] until 等待条件
来源：http://ui.colortex.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://vr.jctech888.com.cn

[R17] 数组定义与取值
来源：http://ay.huixiangedu.cn

arr=(a b c); echo "${arr[0]}"
来源：http://bo.shxzukj.cn

[R18] 遍历数组
来源：http://ex.huanxung.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ln.yuexingan06.cn

[R19] 数组长度
来源：http://qt.chemitech.net.cn

echo "${#arr[@]}"
来源：http://pw.hnjuh.cn

[R20] 关联数组（字典）
来源：http://qw.bjjhwx.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ex.huixinmuqiang.cn

[R21] 字符串长度
来源：http://uz.nicolike.cn


<!-- 参考信息 -->