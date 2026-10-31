代发 wailian999

[P05] 判断两个对象内容是否相等
来源：http://mb.shxzskj.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://yv.huixinmuqiang.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://on.muxihuayi.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://qx.nicolike.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ub.yuexingan06.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://vg.yuntaijiaju.cn

Go:   reflect.DeepEqual(a, b)
来源：http://lh.521024.cn

Ruby: a == b
来源：http://wn.shxzukj.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://nq.newstarts.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://al.shxzukj.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://us.szsharing.cn

PHP:  if (empty($x)) {}
来源：http://nt.huixinmuqiang.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://xb.asd995.cn

TS:   if (x == null) {}
来源：http://mb.szxytkj.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://kc.jianghongdianzi.cn

Go:   if x == nil {}
来源：http://sd.wgjwhj.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ms.huixiangedu.cn

C#:   if (x is null) {}
来源：http://em.yuexingan06.cn

[P07] 防抖与节流
来源：http://ct.nszjky.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://pl.9csxet.cn

PHP:  // 手写时间戳比较
来源：http://ho.hnjuh.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://nq.hnjuh.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ed.yuntaijiaju.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://tv.newstarts.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://zw.haigaiapp.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://fb.bookmarksfly.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://jx.jctech888.com.cn

[P08] 处理浮点精度问题
来源：http://kc.shxzukj.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://al.yuexingan06.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://km.huanxung.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://oe.bookmarksfly.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ab.newstarts.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://io.bookmarksfly.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wr.nszjky.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://jm.hnjuh.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://jd.shtwfgs.cn

================================================================================
来源：http://hw.asd995.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://fm.jianghongdianzi.cn

================================================================================
来源：http://kb.muxihuayi.cn

[Q01] 创建表
来源：http://jc.huixiangedu.cn

CREATE TABLE users (
来源：http://vt.hnjuh.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ef.huanxung.cn

name VARCHAR(50) NOT NULL,
来源：http://ug.muxihuayi.cn

email VARCHAR(100) UNIQUE,
来源：http://um.shtwfgs.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://oz.shxzskj.cn

);
来源：http://ft.szsharing.cn

[Q02] 创建带外键的表
来源：http://vg.jianghongdianzi.cn

CREATE TABLE orders (
来源：http://eb.muxihuayi.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ij.bjjhwx.cn

user_id INT NOT NULL,
来源：http://yl.colortex.cn

amount DECIMAL(10, 2),
来源：http://cp.colortex.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://vw.asd995.cn

);
来源：http://qk.hahajie.cn

[Q03] 增加列
来源：http://cb.panjiajie.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ih.wgjwhj.cn

[Q04] 修改列类型
来源：http://wc.jianghongdianzi.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://xw.hahajie.cn

[Q05] 重命名列
来源：http://ce.huixiangedu.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://pu.yuntaijiaju.cn

[Q06] 删除列
来源：http://he.bookmarksfly.cn

ALTER TABLE users DROP COLUMN age;
来源：http://lm.hnjuh.cn

[Q07] 删除表
来源：http://ko.huanxung.cn

DROP TABLE IF EXISTS orders;
来源：http://iy.gzmigu.cn

[Q08] 创建普通索引
来源：http://za.bjjhwx.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://zx.yuntaijiaju.cn

[Q09] 创建唯一索引
来源：http://nm.yuntaijiaju.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://fb.bookmarksfly.cn

[Q10] 插入单行
来源：http://wx.szsharing.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://yy.yuntaijiaju.cn

[Q11] 一次插入多行
来源：http://wi.wgjwhj.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://vc.nszjky.cn

[Q12] 插入后取自增 ID
来源：http://gh.jianghongdianzi.cn

INSERT INTO users (name) VALUES ('C');
来源：http://lq.colortex.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hc.szxytkj.cn

[Q13] 忽略重复插入
来源：http://eb.huixinmuqiang.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://vn.9csxet.cn

[Q14] 存在则更新（upsert）
来源：http://ip.colortex.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wh.shtwfgs.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mj.bjjhwx.cn

[Q15] 查询全部
来源：http://tw.521024.cn

SELECT * FROM users;
来源：http://rr.shxzukj.cn

[Q16] 查询指定列
来源：http://ot.muxihuayi.cn

SELECT id, name FROM users;
来源：http://pb.yuexingan06.cn

[Q17] 条件查询
来源：http://wr.hnjuh.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://tf.huixinmuqiang.cn

[Q18] 模糊匹配
来源：http://tx.shxzukj.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://nb.shxzskj.cn

[Q19] 范围查询
来源：http://ox.huanxung.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://at.huixinmuqiang.cn

[Q20] IN 列表
来源：http://sl.muxihuayi.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://gv.huixinmuqiang.cn

[Q21] 空值判断
来源：http://sa.bjjhwx.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://dz.yuntaijiaju.cn

[Q22] 排序
来源：http://rr.lnxyls.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://en.hahajie.cn

[Q23] 分页
来源：http://ra.yuntaijiaju.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://nl.gzmigu.cn

[Q24] 去重
来源：http://ui.hahajie.cn

SELECT DISTINCT city FROM users;
来源：http://yz.bookmarksfly.cn

[Q25] 只取前 N 条
来源：http://hg.hahajie.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://qd.shxzukj.cn

[Q26] 计数
来源：http://nc.521024.cn

SELECT COUNT(*) FROM users;
来源：http://nz.jctech888.com.cn

[Q27] 条件计数
来源：http://wz.shxzskj.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://jm.hahajie.cn

[Q28] 求和与平均
来源：http://sv.gzmigu.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://ym.jctech888.com.cn

[Q29] 最大最小值
来源：http://vn.panjiajie.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://bd.huanxung.cn

[Q30] 分组统计
来源：http://qc.huixinmuqiang.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://bj.colortex.cn

[Q31] 分组后过滤
来源：http://ox.gzmigu.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://lw.colortex.cn

[Q32] 分组拼接字符串
来源：http://ph.bookmarksfly.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ku.gzmigu.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://tx.9csxet.cn

[Q33] 多列分组
来源：http://fl.yuexingan06.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://cj.shxzskj.cn

[Q34] 每组取第一条
来源：http://fc.muxihuayi.cn

SELECT * FROM (
来源：http://qy.yuexingan06.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://rv.521024.cn

) t WHERE rn = 1;
来源：http://gp.hnjuh.cn

[Q35] 内连接
来源：http://qt.chemitech.net.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mc.shxzukj.cn

[Q36] 左连接
来源：http://ei.yuexingan06.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ru.panjiajie.cn

[Q37] 右连接
来源：http://ls.nicolike.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://li.newstarts.cn

[Q38] 全外连接（PostgreSQL）
来源：http://pr.yuntaijiaju.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://lv.shtwfgs.cn

[Q39] 自连接（查上下级）
来源：http://jy.yuntaijiaju.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://of.shtwfgs.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://tr.nicolike.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://xm.hahajie.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://bt.hahajie.cn

[Q41] 多表连接
来源：http://jz.szsharing.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://zr.gzmigu.cn

JOIN users u ON u.id = o.user_id
来源：http://xm.shxzskj.cn

JOIN products p ON p.id = o.product_id;
来源：http://ga.hnjuh.cn

[Q42] 连接条件附加过滤
来源：http://lr.szxytkj.cn

SELECT u.name, o.amount FROM users u
来源：http://ow.wgjwhj.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://oc.szxytkj.cn

[Q43] 标量子查询
来源：http://fy.szsharing.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ek.huanxung.cn

[Q44] IN 子查询
来源：http://hb.szxytkj.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://nu.newstarts.cn

[Q45] EXISTS 判断存在
来源：http://yp.yuntaijiaju.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ro.lnxyls.cn

[Q46] NOT EXISTS 判断不存在
来源：http://xg.hnjuh.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://lj.nszjky.cn

[Q47] 与平均值比较
来源：http://dx.shxzukj.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ds.lnxyls.cn

[Q48] CTE 公用表表达式
来源：http://wm.nszjky.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ad.szsharing.cn

SELECT * FROM t WHERE c > 5;
来源：http://an.szxytkj.cn

[Q49] 更新单行
来源：http://jb.asd995.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://so.jctech888.com.cn

[Q50] 批量更新
来源：http://li.nicolike.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://av.hahajie.cn

[Q51] 用子查询更新
来源：http://by.haigaiapp.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://ol.bookmarksfly.cn

[Q52] 删除指定行
来源：http://xs.521024.cn

DELETE FROM users WHERE id = 10;
来源：http://ob.jianghongdianzi.cn

[Q53] 按条件删除
来源：http://os.9csxet.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://nd.yuntaijiaju.cn

[Q54] 清空表
来源：http://cr.shxzskj.cn

TRUNCATE TABLE logs;
来源：http://er.szsharing.cn

[Q55] 排名（并列占位）
来源：http://la.nszjky.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://bq.panjiajie.cn

[Q56] 密集排名（并列不占位）
来源：http://lu.nicolike.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://we.nszjky.cn

[Q57] 行号
来源：http://mn.newstarts.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://st.jianghongdianzi.cn

[Q58] 累计求和
来源：http://ay.szsharing.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://bv.huixiangedu.cn

[Q59] 分组内累计
来源：http://bz.haigaiapp.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ds.wgjwhj.cn

[Q60] 取上一行 / 下一行
来源：http://dq.hahajie.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wy.nicolike.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://tu.shxzukj.cn

[Q61] 移动平均
来源：http://lm.newstarts.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://gf.shtwfgs.cn

[Q62] 分组占比
来源：http://eh.yuexingan06.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://gq.huixiangedu.cn

[Q63] 开启事务
来源：http://ll.colortex.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://oe.asd995.cn

[Q64] 提交事务
来源：http://fo.521024.cn

COMMIT;
来源：http://pl.lnxyls.cn

[Q65] 回滚事务
来源：http://ri.jctech888.com.cn

ROLLBACK;
来源：http://kt.bjjhwx.cn

[Q66] 行锁查询
来源：http://vd.yuexingan06.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://me.gzmigu.cn

[Q67] 设置隔离级别
来源：http://py.huixiangedu.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://vh.shtwfgs.cn

[Q68] 保存点
来源：http://bh.szxytkj.cn

SAVEPOINT sp1;
来源：http://ra.hnjuh.cn

ROLLBACK TO sp1;
来源：http://pq.colortex.cn

[Q69] 查看执行计划
来源：http://ll.haigaiapp.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ty.lnxyls.cn

[Q70] 更新统计信息
来源：http://sg.colortex.cn

ANALYZE TABLE users;
来源：http://wn.hnjuh.cn

[Q71] 查看建表语句
来源：http://nv.szxytkj.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://gp.nicolike.cn

[Q72] 查看索引
来源：http://gh.shtwfgs.cn

SHOW INDEX FROM users;
来源：http://gq.wgjwhj.cn

[Q73] 查看表状态
来源：http://tm.huixinmuqiang.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://ii.shxzukj.cn

[Q74] 强制使用索引
来源：http://wi.yuntaijiaju.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://jq.bookmarksfly.cn

[Q75] 日期格式化
来源：http://pd.hahajie.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://pq.jianghongdianzi.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://yj.shxzskj.cn

[Q76] 按天统计
来源：http://lm.colortex.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://rq.gzmigu.cn

[Q77] 时间加减
来源：http://fm.asd995.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mn.szsharing.cn

[Q78] 当前时间
来源：http://td.hnjuh.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://tq.gzmigu.cn

[Q79] 字符串拼接
来源：http://ne.szsharing.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://tr.yuntaijiaju.cn

[Q80] 字符串截取
来源：http://vh.colortex.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://lb.chemitech.net.cn

[Q81] 字符串替换
来源：http://zr.jianghongdianzi.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hm.bjjhwx.cn

[Q82] 字符长度与字节长度
来源：http://hs.huixiangedu.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://af.haigaiapp.cn

[Q83] 大小写转换
来源：http://hc.shxzukj.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://uj.gzmigu.cn

[Q84] 去除首尾空格
来源：http://xk.newstarts.cn

SELECT TRIM(name) FROM users;
来源：http://hi.shxzskj.cn

[Q85] 数值取整
来源：http://up.asd995.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://xe.bjjhwx.cn

[Q86] 读取 JSON 字段
来源：http://cu.huixiangedu.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hj.wgjwhj.cn

[Q87] JSON 字段做条件
来源：http://jh.jianghongdianzi.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://by.yuexingan06.cn

[Q88] 行转列（条件聚合）
来源：http://cw.jctech888.com.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://rn.shxzukj.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ef.hahajie.cn

[Q89] 判断表是否存在
来源：http://lj.hnjuh.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://cp.hahajie.cn

[Q90] 生成序号列
来源：http://pp.shxzskj.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://th.521024.cn

================================================================================
来源：http://ar.huanxung.cn

R. Bash 专题
来源：http://dj.huanxung.cn

================================================================================
来源：http://kb.chemitech.net.cn

[R01] shebang 与严格模式
来源：http://uf.jianghongdianzi.cn

#!/usr/bin/env bash
来源：http://ea.shxzukj.cn

set -euo pipefail
来源：http://ng.gzmigu.cn

[R02] 变量赋值与使用
来源：http://ci.nszjky.cn

name="Tom"; echo "$name"
来源：http://nt.huixiangedu.cn

[R03] 只读变量
来源：http://en.yuexingan06.cn

readonly PI=3.14
来源：http://po.jianghongdianzi.cn

[R04] 位置参数
来源：http://te.colortex.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://rc.nicolike.cn

[R05] 参数默认值
来源：http://lb.muxihuayi.cn

name="${1:-default}"
来源：http://fm.panjiajie.cn

[R06] 判断命令是否存在
来源：http://ly.nszjky.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://iv.lnxyls.cn

[R07] if 判断文件
来源：http://sx.muxihuayi.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://po.nicolike.cn

[R08] 数值比较
来源：http://bj.muxihuayi.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://wg.wgjwhj.cn

[R09] 字符串比较
来源：http://fa.newstarts.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://nq.muxihuayi.cn

[R10] 正则匹配
来源：http://xt.bjjhwx.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://fh.bookmarksfly.cn

[R11] case 多分支
来源：http://tp.gzmigu.cn

case "$1" in
来源：http://ri.nszjky.cn

start) echo "启动" ;;
来源：http://do.hahajie.cn

stop)  echo "停止" ;;
来源：http://qb.shtwfgs.cn

*)     echo "未知命令" ;;
来源：http://uo.haigaiapp.cn

esac
来源：http://po.lnxyls.cn

[R12] for 遍历文件
来源：http://qc.huixiangedu.cn

for f in *.txt; do echo "$f"; done
来源：http://sv.9csxet.cn

[R13] for 计数循环
来源：http://se.9csxet.cn

for i in {1..10}; do echo "$i"; done
来源：http://jh.huanxung.cn

[R14] C 风格 for
来源：http://bg.huanxung.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://nt.lnxyls.cn

[R15] while 逐行读文件
来源：http://zq.nszjky.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://aq.wgjwhj.cn

[R16] until 等待条件
来源：http://fj.shxzukj.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://qp.huanxung.cn

[R17] 数组定义与取值
来源：http://lj.haigaiapp.cn

arr=(a b c); echo "${arr[0]}"
来源：http://gd.wgjwhj.cn

[R18] 遍历数组
来源：http://il.huixiangedu.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://dr.jianghongdianzi.cn

[R19] 数组长度
来源：http://mk.hnjuh.cn

echo "${#arr[@]}"
来源：http://jt.yuntaijiaju.cn

[R20] 关联数组（字典）
来源：http://wx.yuexingan06.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://pf.shxzukj.cn

[R21] 字符串长度
来源：http://hk.wgjwhj.cn

echo "${#s}"
来源：http://nj.shxzskj.cn

[R22] 截取子串
来源：http://yf.huixinmuqiang.cn

echo "${s:0:5}"
来源：http://te.shxzukj.cn

[R23] 字符串替换
来源：http://rw.lnxyls.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://bc.haigaiapp.cn

[R24] 大小写转换
来源：http://hw.szsharing.cn

echo "${s^^}"; echo "${s,,}"
来源：http://li.huanxung.cn

[R25] 去后缀 / 去前缀
来源：http://cr.colortex.cn


<!-- 参考信息 -->