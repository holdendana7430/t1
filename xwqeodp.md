代发 wailian999

Java: list.size();  map.size();  s.length()
来源：http://zk.jianghongdianzi.cn

Go:   len(arr);  len(m)
来源：http://zp.szsharing.cn

Ruby: x.length;  x.size
来源：http://iq.chemitech.net.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://nl.shxzukj.cn

[P05] 判断两个对象内容是否相等
来源：http://no.nicolike.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://tc.jianghongdianzi.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://we.yuntaijiaju.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://zu.huixinmuqiang.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hw.huixiangedu.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://vm.shxzskj.cn

Go:   reflect.DeepEqual(a, b)
来源：http://zm.nicolike.cn

Ruby: a == b
来源：http://ec.yuexingan06.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://uj.bookmarksfly.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://oa.colortex.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://uu.gzmigu.cn

PHP:  if (empty($x)) {}
来源：http://jz.shxzskj.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://yw.muxihuayi.cn

TS:   if (x == null) {}
来源：http://li.jctech888.com.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://rl.bookmarksfly.cn

Go:   if x == nil {}
来源：http://sd.gzmigu.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://gd.hahajie.cn

C#:   if (x is null) {}
来源：http://eb.gzmigu.cn

[P07] 防抖与节流
来源：http://nh.bookmarksfly.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://fy.yuntaijiaju.cn

PHP:  // 手写时间戳比较
来源：http://cb.shtwfgs.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://od.shtwfgs.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ug.panjiajie.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://fm.gzmigu.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://yv.asd995.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://ff.lnxyls.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://qf.yuexingan06.cn

[P08] 处理浮点精度问题
来源：http://lf.panjiajie.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://xm.hnjuh.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://rf.hahajie.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://kk.yuntaijiaju.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://kv.yuntaijiaju.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ap.bjjhwx.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ue.bjjhwx.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ko.lnxyls.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://rj.shxzukj.cn

================================================================================
来源：http://cy.bjjhwx.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ka.szxytkj.cn

================================================================================
来源：http://bf.nicolike.cn

[Q01] 创建表
来源：http://vw.huixinmuqiang.cn

CREATE TABLE users (
来源：http://gi.yuntaijiaju.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hg.shxzskj.cn

name VARCHAR(50) NOT NULL,
来源：http://yv.hnjuh.cn

email VARCHAR(100) UNIQUE,
来源：http://gr.szxytkj.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mr.nicolike.cn

);
来源：http://pt.huixiangedu.cn

[Q02] 创建带外键的表
来源：http://ew.yuexingan06.cn

CREATE TABLE orders (
来源：http://mc.lnxyls.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://rq.shxzskj.cn

user_id INT NOT NULL,
来源：http://dv.bookmarksfly.cn

amount DECIMAL(10, 2),
来源：http://te.shtwfgs.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://jw.muxihuayi.cn

);
来源：http://jq.yuexingan06.cn

[Q03] 增加列
来源：http://iv.haigaiapp.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://jx.lnxyls.cn

[Q04] 修改列类型
来源：http://rb.szxytkj.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ty.jctech888.com.cn

[Q05] 重命名列
来源：http://rt.shxzukj.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://sx.bjjhwx.cn

[Q06] 删除列
来源：http://ay.haigaiapp.cn

ALTER TABLE users DROP COLUMN age;
来源：http://jk.huixiangedu.cn

[Q07] 删除表
来源：http://al.haigaiapp.cn

DROP TABLE IF EXISTS orders;
来源：http://ib.nszjky.cn

[Q08] 创建普通索引
来源：http://lm.muxihuayi.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://lk.huanxung.cn

[Q09] 创建唯一索引
来源：http://cz.nszjky.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://nz.muxihuayi.cn

[Q10] 插入单行
来源：http://ga.shxzukj.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ln.huixiangedu.cn

[Q11] 一次插入多行
来源：http://js.bookmarksfly.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://uk.gzmigu.cn

[Q12] 插入后取自增 ID
来源：http://sk.lnxyls.cn

INSERT INTO users (name) VALUES ('C');
来源：http://xe.hahajie.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://iy.huanxung.cn

[Q13] 忽略重复插入
来源：http://ad.colortex.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://nu.nszjky.cn

[Q14] 存在则更新（upsert）
来源：http://ni.jianghongdianzi.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ae.hnjuh.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://xj.shxzukj.cn

[Q15] 查询全部
来源：http://de.nicolike.cn

SELECT * FROM users;
来源：http://sf.huixinmuqiang.cn

[Q16] 查询指定列
来源：http://eu.colortex.cn

SELECT id, name FROM users;
来源：http://gc.521024.cn

[Q17] 条件查询
来源：http://nh.asd995.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ds.shtwfgs.cn

[Q18] 模糊匹配
来源：http://us.shtwfgs.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://xq.bookmarksfly.cn

[Q19] 范围查询
来源：http://tw.jianghongdianzi.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://av.shxzukj.cn

[Q20] IN 列表
来源：http://eu.colortex.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://pe.shxzskj.cn

[Q21] 空值判断
来源：http://av.jctech888.com.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://sm.huixinmuqiang.cn

[Q22] 排序
来源：http://he.huanxung.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://iu.szsharing.cn

[Q23] 分页
来源：http://ot.szxytkj.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://dq.shxzskj.cn

[Q24] 去重
来源：http://oz.nszjky.cn

SELECT DISTINCT city FROM users;
来源：http://cj.szsharing.cn

[Q25] 只取前 N 条
来源：http://lb.yuntaijiaju.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ta.gzmigu.cn

[Q26] 计数
来源：http://an.szsharing.cn

SELECT COUNT(*) FROM users;
来源：http://sz.huixinmuqiang.cn

[Q27] 条件计数
来源：http://hh.jianghongdianzi.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hy.huixinmuqiang.cn

[Q28] 求和与平均
来源：http://iz.chemitech.net.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://jx.newstarts.cn

[Q29] 最大最小值
来源：http://os.yuntaijiaju.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://vi.nicolike.cn

[Q30] 分组统计
来源：http://ow.yuexingan06.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://lh.shtwfgs.cn

[Q31] 分组后过滤
来源：http://gs.panjiajie.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ic.bookmarksfly.cn

[Q32] 分组拼接字符串
来源：http://sr.gzmigu.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://js.newstarts.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://op.hnjuh.cn

[Q33] 多列分组
来源：http://os.huanxung.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mg.shxzukj.cn

[Q34] 每组取第一条
来源：http://gc.jianghongdianzi.cn

SELECT * FROM (
来源：http://nd.huixiangedu.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ae.521024.cn

) t WHERE rn = 1;
来源：http://jr.panjiajie.cn

[Q35] 内连接
来源：http://ib.hnjuh.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://th.521024.cn

[Q36] 左连接
来源：http://wa.9csxet.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://tw.hahajie.cn

[Q37] 右连接
来源：http://xf.jianghongdianzi.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://fb.newstarts.cn

[Q38] 全外连接（PostgreSQL）
来源：http://fx.panjiajie.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://nz.lnxyls.cn

[Q39] 自连接（查上下级）
来源：http://re.haigaiapp.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://ky.bjjhwx.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ic.gzmigu.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://qt.nicolike.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://dt.gzmigu.cn

[Q41] 多表连接
来源：http://gq.hahajie.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://pv.huanxung.cn

JOIN users u ON u.id = o.user_id
来源：http://hs.bjjhwx.cn

JOIN products p ON p.id = o.product_id;
来源：http://xp.jianghongdianzi.cn

[Q42] 连接条件附加过滤
来源：http://dt.hahajie.cn

SELECT u.name, o.amount FROM users u
来源：http://kb.huixinmuqiang.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://eo.szsharing.cn

[Q43] 标量子查询
来源：http://no.jctech888.com.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://rc.szxytkj.cn

[Q44] IN 子查询
来源：http://td.chemitech.net.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://vy.huanxung.cn

[Q45] EXISTS 判断存在
来源：http://ja.hnjuh.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://bf.jianghongdianzi.cn

[Q46] NOT EXISTS 判断不存在
来源：http://no.newstarts.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://vv.szsharing.cn

[Q47] 与平均值比较
来源：http://wk.9csxet.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://rp.lnxyls.cn

[Q48] CTE 公用表表达式
来源：http://al.haigaiapp.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://nl.521024.cn

SELECT * FROM t WHERE c > 5;
来源：http://de.gzmigu.cn

[Q49] 更新单行
来源：http://je.huixinmuqiang.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://og.nszjky.cn

[Q50] 批量更新
来源：http://vk.nicolike.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://sm.haigaiapp.cn

[Q51] 用子查询更新
来源：http://vx.huixinmuqiang.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://cg.szxytkj.cn

[Q52] 删除指定行
来源：http://yw.yuexingan06.cn

DELETE FROM users WHERE id = 10;
来源：http://py.szsharing.cn

[Q53] 按条件删除
来源：http://vu.hahajie.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://uo.hnjuh.cn

[Q54] 清空表
来源：http://mt.newstarts.cn

TRUNCATE TABLE logs;
来源：http://jo.bjjhwx.cn

[Q55] 排名（并列占位）
来源：http://xv.bjjhwx.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://de.9csxet.cn

[Q56] 密集排名（并列不占位）
来源：http://uw.huanxung.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ma.nicolike.cn

[Q57] 行号
来源：http://ag.huanxung.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://gc.yuntaijiaju.cn

[Q58] 累计求和
来源：http://rx.asd995.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://dh.chemitech.net.cn

[Q59] 分组内累计
来源：http://ck.hnjuh.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ok.gzmigu.cn

[Q60] 取上一行 / 下一行
来源：http://gr.szsharing.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ea.521024.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://qi.lnxyls.cn

[Q61] 移动平均
来源：http://ui.jianghongdianzi.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ip.szxytkj.cn

[Q62] 分组占比
来源：http://cg.9csxet.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://xi.521024.cn

[Q63] 开启事务
来源：http://bo.chemitech.net.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://uy.haigaiapp.cn

[Q64] 提交事务
来源：http://fx.shxzskj.cn

COMMIT;
来源：http://ec.szxytkj.cn

[Q65] 回滚事务
来源：http://re.shtwfgs.cn

ROLLBACK;
来源：http://my.szxytkj.cn

[Q66] 行锁查询
来源：http://zq.szxytkj.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://nw.gzmigu.cn

[Q67] 设置隔离级别
来源：http://dv.szxytkj.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ko.wgjwhj.cn

[Q68] 保存点
来源：http://xp.shtwfgs.cn

SAVEPOINT sp1;
来源：http://re.bjjhwx.cn

ROLLBACK TO sp1;
来源：http://xe.chemitech.net.cn

[Q69] 查看执行计划
来源：http://tu.jctech888.com.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://yp.muxihuayi.cn

[Q70] 更新统计信息
来源：http://zu.nszjky.cn

ANALYZE TABLE users;
来源：http://su.nicolike.cn

[Q71] 查看建表语句
来源：http://ml.shtwfgs.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://cp.colortex.cn

[Q72] 查看索引
来源：http://yd.huixinmuqiang.cn

SHOW INDEX FROM users;
来源：http://mq.9csxet.cn

[Q73] 查看表状态
来源：http://gu.nszjky.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://mz.huixinmuqiang.cn

[Q74] 强制使用索引
来源：http://jm.nicolike.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ym.szxytkj.cn

[Q75] 日期格式化
来源：http://ie.9csxet.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://am.bookmarksfly.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://aw.szxytkj.cn

[Q76] 按天统计
来源：http://en.haigaiapp.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ey.colortex.cn

[Q77] 时间加减
来源：http://ry.bjjhwx.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://kj.panjiajie.cn

[Q78] 当前时间
来源：http://ku.521024.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hr.nszjky.cn

[Q79] 字符串拼接
来源：http://bx.yuexingan06.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ay.nszjky.cn

[Q80] 字符串截取
来源：http://ag.shtwfgs.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ow.shtwfgs.cn

[Q81] 字符串替换
来源：http://un.asd995.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://gr.521024.cn

[Q82] 字符长度与字节长度
来源：http://jc.lnxyls.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://qo.jianghongdianzi.cn

[Q83] 大小写转换
来源：http://ii.lnxyls.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://zm.chemitech.net.cn

[Q84] 去除首尾空格
来源：http://ar.jianghongdianzi.cn

SELECT TRIM(name) FROM users;
来源：http://ir.9csxet.cn

[Q85] 数值取整
来源：http://xe.shxzskj.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://gk.asd995.cn

[Q86] 读取 JSON 字段
来源：http://pi.jianghongdianzi.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hd.jianghongdianzi.cn

[Q87] JSON 字段做条件
来源：http://mo.szsharing.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wm.jctech888.com.cn

[Q88] 行转列（条件聚合）
来源：http://te.bookmarksfly.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://jr.huanxung.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://pn.bookmarksfly.cn

[Q89] 判断表是否存在
来源：http://pa.bookmarksfly.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ky.nicolike.cn

[Q90] 生成序号列
来源：http://ey.jianghongdianzi.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://rv.bookmarksfly.cn

================================================================================
来源：http://wb.bookmarksfly.cn

R. Bash 专题
来源：http://rj.huixinmuqiang.cn

================================================================================
来源：http://ge.hnjuh.cn

[R01] shebang 与严格模式
来源：http://gc.huixiangedu.cn

#!/usr/bin/env bash
来源：http://zd.newstarts.cn

set -euo pipefail
来源：http://if.hahajie.cn

[R02] 变量赋值与使用
来源：http://yw.nicolike.cn

name="Tom"; echo "$name"
来源：http://lp.haigaiapp.cn

[R03] 只读变量
来源：http://sp.shxzukj.cn

readonly PI=3.14
来源：http://qp.haigaiapp.cn

[R04] 位置参数
来源：http://xi.szsharing.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wz.chemitech.net.cn

[R05] 参数默认值
来源：http://dy.yuexingan06.cn

name="${1:-default}"
来源：http://pw.hnjuh.cn

[R06] 判断命令是否存在
来源：http://rw.lnxyls.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ig.shxzukj.cn

[R07] if 判断文件
来源：http://qv.huixiangedu.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wh.yuntaijiaju.cn

[R08] 数值比较
来源：http://au.colortex.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://yr.521024.cn

[R09] 字符串比较
来源：http://zz.panjiajie.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://uc.yuntaijiaju.cn

[R10] 正则匹配
来源：http://ut.hnjuh.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mc.chemitech.net.cn

[R11] case 多分支
来源：http://cm.nicolike.cn

case "$1" in
来源：http://rg.chemitech.net.cn

start) echo "启动" ;;
来源：http://zk.9csxet.cn

stop)  echo "停止" ;;
来源：http://zw.521024.cn

*)     echo "未知命令" ;;
来源：http://aw.huixiangedu.cn

esac
来源：http://xx.nicolike.cn

[R12] for 遍历文件
来源：http://lb.bookmarksfly.cn

for f in *.txt; do echo "$f"; done
来源：http://re.shxzukj.cn

[R13] for 计数循环
来源：http://vp.huixiangedu.cn

for i in {1..10}; do echo "$i"; done
来源：http://mt.9csxet.cn

[R14] C 风格 for
来源：http://vo.shxzskj.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://oa.jctech888.com.cn

[R15] while 逐行读文件
来源：http://xf.szxytkj.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://tg.huixiangedu.cn

[R16] until 等待条件
来源：http://gk.jctech888.com.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://lo.gzmigu.cn

[R17] 数组定义与取值
来源：http://hj.yuexingan06.cn

arr=(a b c); echo "${arr[0]}"
来源：http://ok.shxzskj.cn

[R18] 遍历数组
来源：http://nv.jianghongdianzi.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://xx.nszjky.cn

[R19] 数组长度
来源：http://pz.muxihuayi.cn

echo "${#arr[@]}"
来源：http://dd.colortex.cn

[R20] 关联数组（字典）
来源：http://ji.9csxet.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wu.yuexingan06.cn

[R21] 字符串长度
来源：http://cz.bjjhwx.cn

echo "${#s}"
来源：http://gj.bookmarksfly.cn

[R22] 截取子串
来源：http://fq.hnjuh.cn

echo "${s:0:5}"
来源：http://gr.muxihuayi.cn

[R23] 字符串替换
来源：http://yx.hnjuh.cn


<!-- 参考信息 -->