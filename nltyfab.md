代发 wailian999

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mc.huanxung.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://rl.bjjhwx.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://jh.hahajie.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ej.nszjky.cn

Java: list.size();  map.size();  s.length()
来源：http://gj.gzmigu.cn

Go:   len(arr);  len(m)
来源：http://eq.colortex.cn

Ruby: x.length;  x.size
来源：http://nw.hnjuh.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://ad.wgjwhj.cn

[P05] 判断两个对象内容是否相等
来源：http://um.nicolike.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://zt.panjiajie.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ew.chemitech.net.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://yx.huanxung.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://qx.lnxyls.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://lv.yuexingan06.cn

Go:   reflect.DeepEqual(a, b)
来源：http://pk.521024.cn

Ruby: a == b
来源：http://pn.chemitech.net.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://rj.szxytkj.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://vg.wgjwhj.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://gr.huixinmuqiang.cn

PHP:  if (empty($x)) {}
来源：http://id.shtwfgs.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://qj.nszjky.cn

TS:   if (x == null) {}
来源：http://hq.hnjuh.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://fl.wgjwhj.cn

Go:   if x == nil {}
来源：http://vm.muxihuayi.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ie.yuexingan06.cn

C#:   if (x is null) {}
来源：http://kr.colortex.cn

[P07] 防抖与节流
来源：http://jx.huanxung.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://or.huanxung.cn

PHP:  // 手写时间戳比较
来源：http://dj.szxytkj.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://er.hnjuh.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ob.hahajie.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://en.bjjhwx.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://jl.asd995.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://io.jianghongdianzi.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://dk.huixinmuqiang.cn

[P08] 处理浮点精度问题
来源：http://be.muxihuayi.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ar.nszjky.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://us.jianghongdianzi.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://yg.bookmarksfly.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ac.huixiangedu.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://xk.yuntaijiaju.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://pd.yuntaijiaju.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://dm.colortex.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://rg.nszjky.cn

================================================================================
来源：http://qs.bookmarksfly.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ip.jianghongdianzi.cn

================================================================================
来源：http://gc.9csxet.cn

[Q01] 创建表
来源：http://xe.bookmarksfly.cn

CREATE TABLE users (
来源：http://qh.shtwfgs.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://zl.haigaiapp.cn

name VARCHAR(50) NOT NULL,
来源：http://qs.muxihuayi.cn

email VARCHAR(100) UNIQUE,
来源：http://zm.huixiangedu.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ow.shxzukj.cn

);
来源：http://lh.yuntaijiaju.cn

[Q02] 创建带外键的表
来源：http://ar.wgjwhj.cn

CREATE TABLE orders (
来源：http://oq.chemitech.net.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://da.huanxung.cn

user_id INT NOT NULL,
来源：http://se.jianghongdianzi.cn

amount DECIMAL(10, 2),
来源：http://ik.bookmarksfly.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://dc.shxzukj.cn

);
来源：http://mm.huixiangedu.cn

[Q03] 增加列
来源：http://hc.bjjhwx.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://kd.nicolike.cn

[Q04] 修改列类型
来源：http://bw.lnxyls.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://lt.colortex.cn

[Q05] 重命名列
来源：http://gh.521024.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://nv.muxihuayi.cn

[Q06] 删除列
来源：http://ls.bjjhwx.cn

ALTER TABLE users DROP COLUMN age;
来源：http://nd.shxzskj.cn

[Q07] 删除表
来源：http://uw.haigaiapp.cn

DROP TABLE IF EXISTS orders;
来源：http://dp.huixinmuqiang.cn

[Q08] 创建普通索引
来源：http://oa.bookmarksfly.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://rj.nszjky.cn

[Q09] 创建唯一索引
来源：http://ia.chemitech.net.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://cm.huixinmuqiang.cn

[Q10] 插入单行
来源：http://wi.huanxung.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://pm.huanxung.cn

[Q11] 一次插入多行
来源：http://kb.9csxet.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ly.jianghongdianzi.cn

[Q12] 插入后取自增 ID
来源：http://gl.nicolike.cn

INSERT INTO users (name) VALUES ('C');
来源：http://cg.hahajie.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ea.panjiajie.cn

[Q13] 忽略重复插入
来源：http://vg.newstarts.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://yw.9csxet.cn

[Q14] 存在则更新（upsert）
来源：http://ny.lnxyls.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://kk.521024.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://cq.gzmigu.cn

[Q15] 查询全部
来源：http://ua.szxytkj.cn

SELECT * FROM users;
来源：http://wf.521024.cn

[Q16] 查询指定列
来源：http://gp.nszjky.cn

SELECT id, name FROM users;
来源：http://sn.panjiajie.cn

[Q17] 条件查询
来源：http://or.asd995.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://up.9csxet.cn

[Q18] 模糊匹配
来源：http://cf.yuntaijiaju.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://co.szsharing.cn

[Q19] 范围查询
来源：http://rh.yuntaijiaju.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://vy.yuntaijiaju.cn

[Q20] IN 列表
来源：http://oy.panjiajie.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://fb.521024.cn

[Q21] 空值判断
来源：http://fo.newstarts.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://ey.chemitech.net.cn

[Q22] 排序
来源：http://gz.hahajie.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://rx.yuntaijiaju.cn

[Q23] 分页
来源：http://jf.gzmigu.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://bn.shtwfgs.cn

[Q24] 去重
来源：http://kr.muxihuayi.cn

SELECT DISTINCT city FROM users;
来源：http://wq.szsharing.cn

[Q25] 只取前 N 条
来源：http://rr.nicolike.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mm.haigaiapp.cn

[Q26] 计数
来源：http://gz.haigaiapp.cn

SELECT COUNT(*) FROM users;
来源：http://pm.szxytkj.cn

[Q27] 条件计数
来源：http://tu.yuexingan06.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://qk.huixiangedu.cn

[Q28] 求和与平均
来源：http://xl.yuexingan06.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://md.chemitech.net.cn

[Q29] 最大最小值
来源：http://ja.huanxung.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://ys.hnjuh.cn

[Q30] 分组统计
来源：http://xn.huixinmuqiang.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mx.panjiajie.cn

[Q31] 分组后过滤
来源：http://tb.jctech888.com.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://yo.szxytkj.cn

[Q32] 分组拼接字符串
来源：http://ou.yuexingan06.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://rd.yuexingan06.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://kb.panjiajie.cn

[Q33] 多列分组
来源：http://wg.shxzukj.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://pp.szxytkj.cn

[Q34] 每组取第一条
来源：http://hl.bjjhwx.cn

SELECT * FROM (
来源：http://wn.szxytkj.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://oq.wgjwhj.cn

) t WHERE rn = 1;
来源：http://of.wgjwhj.cn

[Q35] 内连接
来源：http://hr.gzmigu.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://uj.haigaiapp.cn

[Q36] 左连接
来源：http://so.lnxyls.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://sq.gzmigu.cn

[Q37] 右连接
来源：http://zj.huixinmuqiang.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://uy.colortex.cn

[Q38] 全外连接（PostgreSQL）
来源：http://fq.huanxung.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://uk.newstarts.cn

[Q39] 自连接（查上下级）
来源：http://qy.jctech888.com.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://pl.shxzukj.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://uj.wgjwhj.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://go.jianghongdianzi.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hb.huixiangedu.cn

[Q41] 多表连接
来源：http://cy.hahajie.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://bl.panjiajie.cn

JOIN users u ON u.id = o.user_id
来源：http://at.huanxung.cn

JOIN products p ON p.id = o.product_id;
来源：http://hc.bjjhwx.cn

[Q42] 连接条件附加过滤
来源：http://hr.newstarts.cn

SELECT u.name, o.amount FROM users u
来源：http://oz.szsharing.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://jm.shxzukj.cn

[Q43] 标量子查询
来源：http://fs.521024.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ea.szxytkj.cn

[Q44] IN 子查询
来源：http://aa.huanxung.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://xr.panjiajie.cn

[Q45] EXISTS 判断存在
来源：http://wt.szsharing.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://kb.huixinmuqiang.cn

[Q46] NOT EXISTS 判断不存在
来源：http://yo.shxzukj.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ig.colortex.cn

[Q47] 与平均值比较
来源：http://uy.huixinmuqiang.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://dz.colortex.cn

[Q48] CTE 公用表表达式
来源：http://zd.colortex.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://zn.9csxet.cn

SELECT * FROM t WHERE c > 5;
来源：http://wf.yuntaijiaju.cn

[Q49] 更新单行
来源：http://ft.haigaiapp.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://sp.newstarts.cn

[Q50] 批量更新
来源：http://ml.huixinmuqiang.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://an.huixinmuqiang.cn

[Q51] 用子查询更新
来源：http://qx.bookmarksfly.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://vm.521024.cn

[Q52] 删除指定行
来源：http://qr.muxihuayi.cn

DELETE FROM users WHERE id = 10;
来源：http://lr.shtwfgs.cn

[Q53] 按条件删除
来源：http://rb.shtwfgs.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://dl.haigaiapp.cn

[Q54] 清空表
来源：http://mo.szxytkj.cn

TRUNCATE TABLE logs;
来源：http://xy.szsharing.cn

[Q55] 排名（并列占位）
来源：http://lp.jctech888.com.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://pa.bjjhwx.cn

[Q56] 密集排名（并列不占位）
来源：http://cq.asd995.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ru.haigaiapp.cn

[Q57] 行号
来源：http://ge.9csxet.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://kk.chemitech.net.cn

[Q58] 累计求和
来源：http://mg.jctech888.com.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://nc.hnjuh.cn

[Q59] 分组内累计
来源：http://ft.szxytkj.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://bp.nicolike.cn

[Q60] 取上一行 / 下一行
来源：http://ms.szxytkj.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://tw.huanxung.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://za.hnjuh.cn

[Q61] 移动平均
来源：http://zr.yuexingan06.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://yb.bjjhwx.cn

[Q62] 分组占比
来源：http://wh.yuexingan06.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://tk.huixiangedu.cn

[Q63] 开启事务
来源：http://eu.szsharing.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://wo.hnjuh.cn

[Q64] 提交事务
来源：http://ch.szxytkj.cn

COMMIT;
来源：http://gn.shtwfgs.cn

[Q65] 回滚事务
来源：http://ga.521024.cn

ROLLBACK;
来源：http://xv.jianghongdianzi.cn

[Q66] 行锁查询
来源：http://hn.muxihuayi.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ly.muxihuayi.cn

[Q67] 设置隔离级别
来源：http://sf.bjjhwx.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wm.lnxyls.cn

[Q68] 保存点
来源：http://ze.shtwfgs.cn

SAVEPOINT sp1;
来源：http://sq.gzmigu.cn

ROLLBACK TO sp1;
来源：http://xa.lnxyls.cn

[Q69] 查看执行计划
来源：http://qu.huixinmuqiang.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mf.nszjky.cn

[Q70] 更新统计信息
来源：http://ru.haigaiapp.cn

ANALYZE TABLE users;
来源：http://jd.asd995.cn

[Q71] 查看建表语句
来源：http://qz.lnxyls.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://va.szsharing.cn

[Q72] 查看索引
来源：http://ih.shxzukj.cn

SHOW INDEX FROM users;
来源：http://ve.huanxung.cn

[Q73] 查看表状态
来源：http://we.szsharing.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://rv.asd995.cn

[Q74] 强制使用索引
来源：http://ry.gzmigu.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://fm.haigaiapp.cn

[Q75] 日期格式化
来源：http://bl.szxytkj.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://gk.shxzskj.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://fq.9csxet.cn

[Q76] 按天统计
来源：http://te.nszjky.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://yu.bookmarksfly.cn

[Q77] 时间加减
来源：http://bc.nicolike.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://xk.huanxung.cn

[Q78] 当前时间
来源：http://fn.shtwfgs.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ea.bookmarksfly.cn

[Q79] 字符串拼接
来源：http://qx.shxzskj.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://nx.newstarts.cn

[Q80] 字符串截取
来源：http://wz.shxzukj.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://fa.9csxet.cn

[Q81] 字符串替换
来源：http://vy.panjiajie.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ce.newstarts.cn

[Q82] 字符长度与字节长度
来源：http://tg.jctech888.com.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://cc.newstarts.cn

[Q83] 大小写转换
来源：http://jl.newstarts.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://nu.nicolike.cn

[Q84] 去除首尾空格
来源：http://uo.szsharing.cn

SELECT TRIM(name) FROM users;
来源：http://sk.haigaiapp.cn

[Q85] 数值取整
来源：http://va.jianghongdianzi.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://fi.yuexingan06.cn

[Q86] 读取 JSON 字段
来源：http://ja.jctech888.com.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://dy.bjjhwx.cn

[Q87] JSON 字段做条件
来源：http://ek.szsharing.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://tc.hahajie.cn

[Q88] 行转列（条件聚合）
来源：http://kk.521024.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://nv.nicolike.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://xh.shtwfgs.cn

[Q89] 判断表是否存在
来源：http://lv.szxytkj.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.jianghongdianzi.cn

[Q90] 生成序号列
来源：http://iy.bjjhwx.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://tc.haigaiapp.cn

================================================================================
来源：http://xz.hahajie.cn

R. Bash 专题
来源：http://ux.521024.cn

================================================================================
来源：http://le.shxzukj.cn

[R01] shebang 与严格模式
来源：http://jt.hahajie.cn

#!/usr/bin/env bash
来源：http://xv.huixiangedu.cn

set -euo pipefail
来源：http://fn.newstarts.cn

[R02] 变量赋值与使用
来源：http://zu.jianghongdianzi.cn

name="Tom"; echo "$name"
来源：http://bu.shxzskj.cn

[R03] 只读变量
来源：http://sz.panjiajie.cn

readonly PI=3.14
来源：http://fb.huixiangedu.cn

[R04] 位置参数
来源：http://ro.hahajie.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ju.szxytkj.cn

[R05] 参数默认值
来源：http://ig.huanxung.cn

name="${1:-default}"
来源：http://ks.huixiangedu.cn

[R06] 判断命令是否存在
来源：http://ct.hnjuh.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://aa.szsharing.cn

[R07] if 判断文件
来源：http://pn.newstarts.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://vv.huixinmuqiang.cn

[R08] 数值比较
来源：http://ts.muxihuayi.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://yu.szxytkj.cn

[R09] 字符串比较
来源：http://ti.nicolike.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://jb.gzmigu.cn

[R10] 正则匹配
来源：http://hi.hahajie.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://cw.9csxet.cn

[R11] case 多分支
来源：http://gw.lnxyls.cn

case "$1" in
来源：http://tp.jianghongdianzi.cn

start) echo "启动" ;;
来源：http://hi.shxzukj.cn

stop)  echo "停止" ;;
来源：http://en.bookmarksfly.cn

*)     echo "未知命令" ;;
来源：http://wf.huanxung.cn

esac
来源：http://hn.gzmigu.cn

[R12] for 遍历文件
来源：http://qg.bookmarksfly.cn

for f in *.txt; do echo "$f"; done
来源：http://jz.yuexingan06.cn

[R13] for 计数循环
来源：http://eb.hahajie.cn

for i in {1..10}; do echo "$i"; done
来源：http://mz.jianghongdianzi.cn

[R14] C 风格 for
来源：http://ek.huixiangedu.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://yy.bookmarksfly.cn

[R15] while 逐行读文件
来源：http://cs.jctech888.com.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://jv.asd995.cn

[R16] until 等待条件
来源：http://vk.hnjuh.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://gn.wgjwhj.cn

[R17] 数组定义与取值
来源：http://re.newstarts.cn

arr=(a b c); echo "${arr[0]}"
来源：http://zp.nicolike.cn

[R18] 遍历数组
来源：http://jn.yuexingan06.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://px.shxzskj.cn

[R19] 数组长度
来源：http://sj.huanxung.cn

echo "${#arr[@]}"
来源：http://fb.haigaiapp.cn

[R20] 关联数组（字典）
来源：http://fo.wgjwhj.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://uy.hahajie.cn

[R21] 字符串长度
来源：http://hc.jianghongdianzi.cn


<!-- 参考信息 -->