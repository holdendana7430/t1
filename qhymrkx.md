代发 wailian999

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://rl.shxzskj.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://sa.newstarts.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://fi.szxytkj.cn

[P04] 求长度
来源：http://dz.yuntaijiaju.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://sq.shxzukj.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://at.hnjuh.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ac.haigaiapp.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://am.yuntaijiaju.cn

Java: list.size();  map.size();  s.length()
来源：http://pt.chemitech.net.cn

Go:   len(arr);  len(m)
来源：http://xu.szxytkj.cn

Ruby: x.length;  x.size
来源：http://aa.gzmigu.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://pn.wgjwhj.cn

[P05] 判断两个对象内容是否相等
来源：http://zw.shtwfgs.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://gv.shxzukj.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://je.shtwfgs.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ju.jianghongdianzi.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://zf.asd995.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ym.lnxyls.cn

Go:   reflect.DeepEqual(a, b)
来源：http://wu.panjiajie.cn

Ruby: a == b
来源：http://wr.lnxyls.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ze.szsharing.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://nk.yuntaijiaju.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://gd.lnxyls.cn

PHP:  if (empty($x)) {}
来源：http://ai.huixinmuqiang.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://bq.bookmarksfly.cn

TS:   if (x == null) {}
来源：http://ln.nicolike.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://ma.bjjhwx.cn

Go:   if x == nil {}
来源：http://gp.huanxung.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://gh.huixinmuqiang.cn

C#:   if (x is null) {}
来源：http://kg.szxytkj.cn

[P07] 防抖与节流
来源：http://ma.haigaiapp.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ya.asd995.cn

PHP:  // 手写时间戳比较
来源：http://be.lnxyls.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hd.gzmigu.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://bs.jctech888.com.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://fb.shxzukj.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://cx.hnjuh.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://tk.huanxung.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mt.szxytkj.cn

[P08] 处理浮点精度问题
来源：http://ot.shxzskj.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://yg.nszjky.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wv.gzmigu.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://bp.shxzskj.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wy.newstarts.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://vh.521024.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://qd.szxytkj.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://my.shxzskj.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://di.szsharing.cn

================================================================================
来源：http://al.huixinmuqiang.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wt.gzmigu.cn

================================================================================
来源：http://uh.yuexingan06.cn

[Q01] 创建表
来源：http://yd.yuexingan06.cn

CREATE TABLE users (
来源：http://dw.szxytkj.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://sl.9csxet.cn

name VARCHAR(50) NOT NULL,
来源：http://wc.shtwfgs.cn

email VARCHAR(100) UNIQUE,
来源：http://cx.newstarts.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://gm.jctech888.com.cn

);
来源：http://qm.jianghongdianzi.cn

[Q02] 创建带外键的表
来源：http://yr.huanxung.cn

CREATE TABLE orders (
来源：http://cb.huanxung.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://vv.newstarts.cn

user_id INT NOT NULL,
来源：http://ox.nszjky.cn

amount DECIMAL(10, 2),
来源：http://zx.asd995.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ub.hahajie.cn

);
来源：http://gq.colortex.cn

[Q03] 增加列
来源：http://pm.asd995.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://jk.gzmigu.cn

[Q04] 修改列类型
来源：http://pk.muxihuayi.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://vx.shxzukj.cn

[Q05] 重命名列
来源：http://sw.yuexingan06.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://lk.yuexingan06.cn

[Q06] 删除列
来源：http://mt.hnjuh.cn

ALTER TABLE users DROP COLUMN age;
来源：http://mj.panjiajie.cn

[Q07] 删除表
来源：http://ug.bookmarksfly.cn

DROP TABLE IF EXISTS orders;
来源：http://zs.hnjuh.cn

[Q08] 创建普通索引
来源：http://gb.lnxyls.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://sv.szsharing.cn

[Q09] 创建唯一索引
来源：http://xv.shtwfgs.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hp.lnxyls.cn

[Q10] 插入单行
来源：http://ae.hnjuh.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wy.szsharing.cn

[Q11] 一次插入多行
来源：http://wq.jianghongdianzi.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://pw.nszjky.cn

[Q12] 插入后取自增 ID
来源：http://hb.huixiangedu.cn

INSERT INTO users (name) VALUES ('C');
来源：http://nr.9csxet.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://gk.shxzskj.cn

[Q13] 忽略重复插入
来源：http://jt.muxihuayi.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://cq.wgjwhj.cn

[Q14] 存在则更新（upsert）
来源：http://mr.newstarts.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://vl.nszjky.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://nb.szxytkj.cn

[Q15] 查询全部
来源：http://fu.muxihuayi.cn

SELECT * FROM users;
来源：http://hr.shxzukj.cn

[Q16] 查询指定列
来源：http://ja.9csxet.cn

SELECT id, name FROM users;
来源：http://dj.jctech888.com.cn

[Q17] 条件查询
来源：http://dg.muxihuayi.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://gy.colortex.cn

[Q18] 模糊匹配
来源：http://nk.haigaiapp.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://kp.newstarts.cn

[Q19] 范围查询
来源：http://op.muxihuayi.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://bl.huixinmuqiang.cn

[Q20] IN 列表
来源：http://op.huanxung.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://bv.huixinmuqiang.cn

[Q21] 空值判断
来源：http://lo.muxihuayi.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://ii.haigaiapp.cn

[Q22] 排序
来源：http://yx.jctech888.com.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://qx.huixinmuqiang.cn

[Q23] 分页
来源：http://mz.wgjwhj.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://be.wgjwhj.cn

[Q24] 去重
来源：http://vw.panjiajie.cn

SELECT DISTINCT city FROM users;
来源：http://ff.shtwfgs.cn

[Q25] 只取前 N 条
来源：http://lv.9csxet.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://bm.jctech888.com.cn

[Q26] 计数
来源：http://bu.yuexingan06.cn

SELECT COUNT(*) FROM users;
来源：http://dm.bjjhwx.cn

[Q27] 条件计数
来源：http://ox.wgjwhj.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://fh.colortex.cn

[Q28] 求和与平均
来源：http://yz.bjjhwx.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wy.wgjwhj.cn

[Q29] 最大最小值
来源：http://ca.asd995.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://zn.nszjky.cn

[Q30] 分组统计
来源：http://fg.bookmarksfly.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ez.hahajie.cn

[Q31] 分组后过滤
来源：http://gr.jctech888.com.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ib.colortex.cn

[Q32] 分组拼接字符串
来源：http://kj.nszjky.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ml.asd995.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://oz.asd995.cn

[Q33] 多列分组
来源：http://it.jianghongdianzi.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://fy.colortex.cn

[Q34] 每组取第一条
来源：http://de.shxzukj.cn

SELECT * FROM (
来源：http://nv.szsharing.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://no.gzmigu.cn

) t WHERE rn = 1;
来源：http://vw.huanxung.cn

[Q35] 内连接
来源：http://cr.huanxung.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://kv.szsharing.cn

[Q36] 左连接
来源：http://gr.bookmarksfly.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://zy.lnxyls.cn

[Q37] 右连接
来源：http://ry.nszjky.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hp.shxzukj.cn

[Q38] 全外连接（PostgreSQL）
来源：http://ic.nicolike.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wd.lnxyls.cn

[Q39] 自连接（查上下级）
来源：http://tp.szxytkj.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://ic.huanxung.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hm.muxihuayi.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://rf.nicolike.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://bv.wgjwhj.cn

[Q41] 多表连接
来源：http://oc.shxzukj.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://si.gzmigu.cn

JOIN users u ON u.id = o.user_id
来源：http://of.newstarts.cn

JOIN products p ON p.id = o.product_id;
来源：http://ld.muxihuayi.cn

[Q42] 连接条件附加过滤
来源：http://mf.9csxet.cn

SELECT u.name, o.amount FROM users u
来源：http://kj.newstarts.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://xp.shxzukj.cn

[Q43] 标量子查询
来源：http://zz.asd995.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ko.huixiangedu.cn

[Q44] IN 子查询
来源：http://gf.newstarts.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://jn.huixiangedu.cn

[Q45] EXISTS 判断存在
来源：http://yk.521024.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mg.shtwfgs.cn

[Q46] NOT EXISTS 判断不存在
来源：http://dp.yuntaijiaju.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wi.huixinmuqiang.cn

[Q47] 与平均值比较
来源：http://ob.gzmigu.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://lh.shtwfgs.cn

[Q48] CTE 公用表表达式
来源：http://ke.shxzukj.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wi.szsharing.cn

SELECT * FROM t WHERE c > 5;
来源：http://hr.colortex.cn

[Q49] 更新单行
来源：http://sv.nicolike.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ub.lnxyls.cn

[Q50] 批量更新
来源：http://rf.szsharing.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://xj.yuntaijiaju.cn

[Q51] 用子查询更新
来源：http://gg.521024.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://sj.shtwfgs.cn

[Q52] 删除指定行
来源：http://ai.chemitech.net.cn

DELETE FROM users WHERE id = 10;
来源：http://gg.nszjky.cn

[Q53] 按条件删除
来源：http://uz.nicolike.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://un.colortex.cn

[Q54] 清空表
来源：http://zn.colortex.cn

TRUNCATE TABLE logs;
来源：http://jk.jctech888.com.cn

[Q55] 排名（并列占位）
来源：http://vm.shtwfgs.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ti.hahajie.cn

[Q56] 密集排名（并列不占位）
来源：http://hf.shxzskj.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://pw.szsharing.cn

[Q57] 行号
来源：http://bo.shtwfgs.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://xu.jctech888.com.cn

[Q58] 累计求和
来源：http://mv.shtwfgs.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://so.bookmarksfly.cn

[Q59] 分组内累计
来源：http://gx.newstarts.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://pc.nszjky.cn

[Q60] 取上一行 / 下一行
来源：http://ja.bookmarksfly.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://rj.bjjhwx.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ia.huixiangedu.cn

[Q61] 移动平均
来源：http://tk.hahajie.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://gq.nszjky.cn

[Q62] 分组占比
来源：http://yv.asd995.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ev.nszjky.cn

[Q63] 开启事务
来源：http://as.shxzskj.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://au.asd995.cn

[Q64] 提交事务
来源：http://dt.huixinmuqiang.cn

COMMIT;
来源：http://hk.hahajie.cn

[Q65] 回滚事务
来源：http://jp.szsharing.cn

ROLLBACK;
来源：http://wk.9csxet.cn

[Q66] 行锁查询
来源：http://ga.nszjky.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ry.shtwfgs.cn

[Q67] 设置隔离级别
来源：http://ws.yuexingan06.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://kt.colortex.cn

[Q68] 保存点
来源：http://gf.shxzukj.cn

SAVEPOINT sp1;
来源：http://vv.bookmarksfly.cn

ROLLBACK TO sp1;
来源：http://po.jctech888.com.cn

[Q69] 查看执行计划
来源：http://gc.shxzskj.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://xt.lnxyls.cn

[Q70] 更新统计信息
来源：http://zo.yuntaijiaju.cn

ANALYZE TABLE users;
来源：http://hd.colortex.cn

[Q71] 查看建表语句
来源：http://vb.yuexingan06.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://el.yuexingan06.cn

[Q72] 查看索引
来源：http://rn.nszjky.cn

SHOW INDEX FROM users;
来源：http://ui.jianghongdianzi.cn

[Q73] 查看表状态
来源：http://bs.colortex.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://ns.9csxet.cn

[Q74] 强制使用索引
来源：http://ug.wgjwhj.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://qa.panjiajie.cn

[Q75] 日期格式化
来源：http://ez.shxzskj.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hk.jctech888.com.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://pi.bjjhwx.cn

[Q76] 按天统计
来源：http://uw.huanxung.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://zp.newstarts.cn

[Q77] 时间加减
来源：http://dy.wgjwhj.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://sm.lnxyls.cn

[Q78] 当前时间
来源：http://pm.shtwfgs.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://kj.panjiajie.cn

[Q79] 字符串拼接
来源：http://xa.huixinmuqiang.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://xb.haigaiapp.cn

[Q80] 字符串截取
来源：http://ht.bjjhwx.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ae.huixiangedu.cn

[Q81] 字符串替换
来源：http://bf.gzmigu.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://gg.asd995.cn

[Q82] 字符长度与字节长度
来源：http://ro.nszjky.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hb.jctech888.com.cn

[Q83] 大小写转换
来源：http://fl.nicolike.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://kj.9csxet.cn

[Q84] 去除首尾空格
来源：http://pe.panjiajie.cn

SELECT TRIM(name) FROM users;
来源：http://db.chemitech.net.cn

[Q85] 数值取整
来源：http://yz.yuntaijiaju.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://rd.panjiajie.cn

[Q86] 读取 JSON 字段
来源：http://vd.szxytkj.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://yy.panjiajie.cn

[Q87] JSON 字段做条件
来源：http://ij.jianghongdianzi.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wf.huanxung.cn

[Q88] 行转列（条件聚合）
来源：http://oj.gzmigu.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://sv.haigaiapp.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://qj.asd995.cn

[Q89] 判断表是否存在
来源：http://kr.jctech888.com.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://gj.lnxyls.cn

[Q90] 生成序号列
来源：http://vk.9csxet.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://pp.huixinmuqiang.cn

================================================================================
来源：http://yj.huanxung.cn

R. Bash 专题
来源：http://rm.szxytkj.cn

================================================================================
来源：http://kg.bookmarksfly.cn

[R01] shebang 与严格模式
来源：http://qi.jctech888.com.cn

#!/usr/bin/env bash
来源：http://de.asd995.cn

set -euo pipefail
来源：http://ou.szsharing.cn

[R02] 变量赋值与使用
来源：http://np.hahajie.cn

name="Tom"; echo "$name"
来源：http://cm.bjjhwx.cn

[R03] 只读变量
来源：http://dh.panjiajie.cn

readonly PI=3.14
来源：http://qh.huanxung.cn

[R04] 位置参数
来源：http://zk.jctech888.com.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ec.yuntaijiaju.cn

[R05] 参数默认值
来源：http://oj.9csxet.cn

name="${1:-default}"
来源：http://qu.lnxyls.cn

[R06] 判断命令是否存在
来源：http://cy.bookmarksfly.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://tu.jianghongdianzi.cn

[R07] if 判断文件
来源：http://pt.yuntaijiaju.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://pe.wgjwhj.cn

[R08] 数值比较
来源：http://ut.bjjhwx.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://tm.yuntaijiaju.cn

[R09] 字符串比较
来源：http://ru.huixiangedu.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://rc.asd995.cn

[R10] 正则匹配
来源：http://ry.huixinmuqiang.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://kp.hnjuh.cn

[R11] case 多分支
来源：http://oj.chemitech.net.cn

case "$1" in
来源：http://cd.asd995.cn

start) echo "启动" ;;
来源：http://hj.jctech888.com.cn

stop)  echo "停止" ;;
来源：http://lq.panjiajie.cn

*)     echo "未知命令" ;;
来源：http://bd.jianghongdianzi.cn

esac
来源：http://iz.huixiangedu.cn

[R12] for 遍历文件
来源：http://al.bookmarksfly.cn

for f in *.txt; do echo "$f"; done
来源：http://uu.muxihuayi.cn

[R13] for 计数循环
来源：http://py.bookmarksfly.cn

for i in {1..10}; do echo "$i"; done
来源：http://qj.huanxung.cn

[R14] C 风格 for
来源：http://bz.gzmigu.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://xa.hnjuh.cn

[R15] while 逐行读文件
来源：http://ip.jianghongdianzi.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://pb.panjiajie.cn

[R16] until 等待条件
来源：http://ee.hnjuh.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ep.9csxet.cn

[R17] 数组定义与取值
来源：http://tn.szsharing.cn

arr=(a b c); echo "${arr[0]}"
来源：http://fy.haigaiapp.cn

[R18] 遍历数组
来源：http://zv.hahajie.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mv.shxzskj.cn

[R19] 数组长度
来源：http://rn.yuexingan06.cn


<!-- 参考信息 -->