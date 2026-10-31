代发 wailian999

[P05] 判断两个对象内容是否相等
来源：http://lk.asd995.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://mc.colortex.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://cv.bjjhwx.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ci.jianghongdianzi.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://qw.nicolike.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://fx.szsharing.cn

Go:   reflect.DeepEqual(a, b)
来源：http://hz.bjjhwx.cn

Ruby: a == b
来源：http://sg.shxzukj.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://uh.newstarts.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mq.bookmarksfly.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://yg.9csxet.cn

PHP:  if (empty($x)) {}
来源：http://qj.panjiajie.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://bg.colortex.cn

TS:   if (x == null) {}
来源：http://gs.newstarts.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://sz.panjiajie.cn

Go:   if x == nil {}
来源：http://zx.bjjhwx.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ui.huixiangedu.cn

C#:   if (x is null) {}
来源：http://xv.yuntaijiaju.cn

[P07] 防抖与节流
来源：http://el.bjjhwx.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://vn.jianghongdianzi.cn

PHP:  // 手写时间戳比较
来源：http://eo.szxytkj.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://pe.nicolike.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://pe.newstarts.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://nf.shxzskj.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://oh.haigaiapp.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://ka.huixiangedu.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ct.hahajie.cn

[P08] 处理浮点精度问题
来源：http://bt.wgjwhj.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://dm.wgjwhj.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hd.panjiajie.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://gc.asd995.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ja.521024.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://gy.shtwfgs.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://tf.huixiangedu.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://tj.nszjky.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ji.hahajie.cn

================================================================================
来源：http://px.yuexingan06.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://sf.nicolike.cn

================================================================================
来源：http://yo.muxihuayi.cn

[Q01] 创建表
来源：http://rh.nicolike.cn

CREATE TABLE users (
来源：http://sk.muxihuayi.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://is.panjiajie.cn

name VARCHAR(50) NOT NULL,
来源：http://tr.szxytkj.cn

email VARCHAR(100) UNIQUE,
来源：http://pq.hahajie.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://gi.lnxyls.cn

);
来源：http://cl.gzmigu.cn

[Q02] 创建带外键的表
来源：http://hu.jianghongdianzi.cn

CREATE TABLE orders (
来源：http://le.shtwfgs.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://kb.szxytkj.cn

user_id INT NOT NULL,
来源：http://yl.wgjwhj.cn

amount DECIMAL(10, 2),
来源：http://rw.yuexingan06.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://es.lnxyls.cn

);
来源：http://zr.muxihuayi.cn

[Q03] 增加列
来源：http://qo.jctech888.com.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://yn.nicolike.cn

[Q04] 修改列类型
来源：http://rn.jianghongdianzi.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ee.jianghongdianzi.cn

[Q05] 重命名列
来源：http://mv.nicolike.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://up.shxzukj.cn

[Q06] 删除列
来源：http://dx.nicolike.cn

ALTER TABLE users DROP COLUMN age;
来源：http://gp.jianghongdianzi.cn

[Q07] 删除表
来源：http://nb.asd995.cn

DROP TABLE IF EXISTS orders;
来源：http://lc.newstarts.cn

[Q08] 创建普通索引
来源：http://pb.huanxung.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://xk.yuexingan06.cn

[Q09] 创建唯一索引
来源：http://nz.jianghongdianzi.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://cu.shxzukj.cn

[Q10] 插入单行
来源：http://rf.jianghongdianzi.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://qt.hahajie.cn

[Q11] 一次插入多行
来源：http://wn.jianghongdianzi.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wg.nicolike.cn

[Q12] 插入后取自增 ID
来源：http://lz.shxzskj.cn

INSERT INTO users (name) VALUES ('C');
来源：http://ob.hnjuh.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://tu.yuntaijiaju.cn

[Q13] 忽略重复插入
来源：http://fx.yuexingan06.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://xp.nicolike.cn

[Q14] 存在则更新（upsert）
来源：http://fn.huanxung.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://qs.jianghongdianzi.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://fi.shxzskj.cn

[Q15] 查询全部
来源：http://jd.szsharing.cn

SELECT * FROM users;
来源：http://xr.panjiajie.cn

[Q16] 查询指定列
来源：http://ig.9csxet.cn

SELECT id, name FROM users;
来源：http://mn.shxzukj.cn

[Q17] 条件查询
来源：http://fl.gzmigu.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://cl.newstarts.cn

[Q18] 模糊匹配
来源：http://cw.521024.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mx.hahajie.cn

[Q19] 范围查询
来源：http://hf.newstarts.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ke.bookmarksfly.cn

[Q20] IN 列表
来源：http://su.newstarts.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mo.bookmarksfly.cn

[Q21] 空值判断
来源：http://sf.yuntaijiaju.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://eo.chemitech.net.cn

[Q22] 排序
来源：http://me.yuntaijiaju.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ov.huixinmuqiang.cn

[Q23] 分页
来源：http://jm.huixinmuqiang.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://eq.bjjhwx.cn

[Q24] 去重
来源：http://ys.hahajie.cn

SELECT DISTINCT city FROM users;
来源：http://lv.panjiajie.cn

[Q25] 只取前 N 条
来源：http://tf.nszjky.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://bq.lnxyls.cn

[Q26] 计数
来源：http://cv.szsharing.cn

SELECT COUNT(*) FROM users;
来源：http://pw.hahajie.cn

[Q27] 条件计数
来源：http://qn.hnjuh.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://lu.hnjuh.cn

[Q28] 求和与平均
来源：http://by.bookmarksfly.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://tn.lnxyls.cn

[Q29] 最大最小值
来源：http://yv.muxihuayi.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://yj.nicolike.cn

[Q30] 分组统计
来源：http://fo.haigaiapp.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://kv.szxytkj.cn

[Q31] 分组后过滤
来源：http://nb.nicolike.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ve.yuntaijiaju.cn

[Q32] 分组拼接字符串
来源：http://gp.panjiajie.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://yz.nicolike.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://qk.shxzskj.cn

[Q33] 多列分组
来源：http://io.nszjky.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://rh.panjiajie.cn

[Q34] 每组取第一条
来源：http://ik.lnxyls.cn

SELECT * FROM (
来源：http://ql.jctech888.com.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://pz.colortex.cn

) t WHERE rn = 1;
来源：http://fs.shtwfgs.cn

[Q35] 内连接
来源：http://fl.huanxung.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://po.9csxet.cn

[Q36] 左连接
来源：http://eo.9csxet.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://rk.panjiajie.cn

[Q37] 右连接
来源：http://qt.hnjuh.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://gb.521024.cn

[Q38] 全外连接（PostgreSQL）
来源：http://zm.nszjky.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://xq.hahajie.cn

[Q39] 自连接（查上下级）
来源：http://ex.shxzukj.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://fh.muxihuayi.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ik.szsharing.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://vw.panjiajie.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ml.yuntaijiaju.cn

[Q41] 多表连接
来源：http://fy.bjjhwx.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://pw.hnjuh.cn

JOIN users u ON u.id = o.user_id
来源：http://gm.colortex.cn

JOIN products p ON p.id = o.product_id;
来源：http://kz.jianghongdianzi.cn

[Q42] 连接条件附加过滤
来源：http://qs.wgjwhj.cn

SELECT u.name, o.amount FROM users u
来源：http://mu.huanxung.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://si.bookmarksfly.cn

[Q43] 标量子查询
来源：http://my.yuexingan06.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ht.gzmigu.cn

[Q44] IN 子查询
来源：http://ff.nszjky.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://fq.shxzukj.cn

[Q45] EXISTS 判断存在
来源：http://cr.colortex.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://xz.521024.cn

[Q46] NOT EXISTS 判断不存在
来源：http://fp.shtwfgs.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://kk.huanxung.cn

[Q47] 与平均值比较
来源：http://ob.nszjky.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ue.shxzukj.cn

[Q48] CTE 公用表表达式
来源：http://hb.colortex.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://bk.hahajie.cn

SELECT * FROM t WHERE c > 5;
来源：http://jl.huixinmuqiang.cn

[Q49] 更新单行
来源：http://gu.newstarts.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://au.szxytkj.cn

[Q50] 批量更新
来源：http://bt.521024.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://lc.huixiangedu.cn

[Q51] 用子查询更新
来源：http://at.bookmarksfly.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://ut.yuexingan06.cn

[Q52] 删除指定行
来源：http://xj.shtwfgs.cn

DELETE FROM users WHERE id = 10;
来源：http://cx.shtwfgs.cn

[Q53] 按条件删除
来源：http://zh.gzmigu.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://me.jianghongdianzi.cn

[Q54] 清空表
来源：http://fa.jctech888.com.cn

TRUNCATE TABLE logs;
来源：http://fs.chemitech.net.cn

[Q55] 排名（并列占位）
来源：http://ro.bjjhwx.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://bu.hnjuh.cn

[Q56] 密集排名（并列不占位）
来源：http://tw.jianghongdianzi.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://je.lnxyls.cn

[Q57] 行号
来源：http://gf.9csxet.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://cz.lnxyls.cn

[Q58] 累计求和
来源：http://mw.gzmigu.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://sk.huanxung.cn

[Q59] 分组内累计
来源：http://fo.jianghongdianzi.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://am.shxzskj.cn

[Q60] 取上一行 / 下一行
来源：http://rq.nicolike.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://vd.lnxyls.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ka.shxzukj.cn

[Q61] 移动平均
来源：http://wo.jctech888.com.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://eu.bookmarksfly.cn

[Q62] 分组占比
来源：http://mt.huixiangedu.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://gx.bookmarksfly.cn

[Q63] 开启事务
来源：http://ac.yuntaijiaju.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://by.lnxyls.cn

[Q64] 提交事务
来源：http://zl.9csxet.cn

COMMIT;
来源：http://ki.haigaiapp.cn

[Q65] 回滚事务
来源：http://zd.hahajie.cn

ROLLBACK;
来源：http://tm.chemitech.net.cn

[Q66] 行锁查询
来源：http://zs.shxzukj.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://on.jianghongdianzi.cn

[Q67] 设置隔离级别
来源：http://qf.hnjuh.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://pt.lnxyls.cn

[Q68] 保存点
来源：http://jp.9csxet.cn

SAVEPOINT sp1;
来源：http://kp.lnxyls.cn

ROLLBACK TO sp1;
来源：http://fg.wgjwhj.cn

[Q69] 查看执行计划
来源：http://rj.chemitech.net.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://us.bjjhwx.cn

[Q70] 更新统计信息
来源：http://er.shtwfgs.cn

ANALYZE TABLE users;
来源：http://bc.huanxung.cn

[Q71] 查看建表语句
来源：http://qt.jctech888.com.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://fh.chemitech.net.cn

[Q72] 查看索引
来源：http://dl.9csxet.cn

SHOW INDEX FROM users;
来源：http://bj.szsharing.cn

[Q73] 查看表状态
来源：http://qh.panjiajie.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://ta.muxihuayi.cn

[Q74] 强制使用索引
来源：http://fh.bjjhwx.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://gz.muxihuayi.cn

[Q75] 日期格式化
来源：http://om.bookmarksfly.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://kw.newstarts.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ji.nicolike.cn

[Q76] 按天统计
来源：http://dt.haigaiapp.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://yx.bjjhwx.cn

[Q77] 时间加减
来源：http://hm.bookmarksfly.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://td.asd995.cn

[Q78] 当前时间
来源：http://bs.hnjuh.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://og.shtwfgs.cn

[Q79] 字符串拼接
来源：http://hw.szxytkj.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wz.chemitech.net.cn

[Q80] 字符串截取
来源：http://uz.gzmigu.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://tq.chemitech.net.cn

[Q81] 字符串替换
来源：http://fs.jianghongdianzi.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://my.szxytkj.cn

[Q82] 字符长度与字节长度
来源：http://kq.panjiajie.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://gu.colortex.cn

[Q83] 大小写转换
来源：http://ev.panjiajie.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://nz.shtwfgs.cn

[Q84] 去除首尾空格
来源：http://up.muxihuayi.cn

SELECT TRIM(name) FROM users;
来源：http://zu.lnxyls.cn

[Q85] 数值取整
来源：http://qb.huanxung.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://qn.huanxung.cn

[Q86] 读取 JSON 字段
来源：http://ix.asd995.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://vw.9csxet.cn

[Q87] JSON 字段做条件
来源：http://tg.hahajie.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://to.asd995.cn

[Q88] 行转列（条件聚合）
来源：http://uh.shxzukj.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://vm.haigaiapp.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://pz.wgjwhj.cn

[Q89] 判断表是否存在
来源：http://xn.newstarts.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://bf.chemitech.net.cn

[Q90] 生成序号列
来源：http://vu.shxzskj.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://xa.huixiangedu.cn

================================================================================
来源：http://bw.yuntaijiaju.cn

R. Bash 专题
来源：http://jn.nicolike.cn

================================================================================
来源：http://ay.bookmarksfly.cn

[R01] shebang 与严格模式
来源：http://zc.lnxyls.cn

#!/usr/bin/env bash
来源：http://fm.huixiangedu.cn

set -euo pipefail
来源：http://wl.lnxyls.cn

[R02] 变量赋值与使用
来源：http://rb.shtwfgs.cn

name="Tom"; echo "$name"
来源：http://oq.panjiajie.cn

[R03] 只读变量
来源：http://vs.nszjky.cn

readonly PI=3.14
来源：http://ii.haigaiapp.cn

[R04] 位置参数
来源：http://yc.muxihuayi.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://pc.jianghongdianzi.cn

[R05] 参数默认值
来源：http://hi.lnxyls.cn

name="${1:-default}"
来源：http://bn.gzmigu.cn

[R06] 判断命令是否存在
来源：http://nn.nicolike.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://gf.chemitech.net.cn

[R07] if 判断文件
来源：http://nz.haigaiapp.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ai.chemitech.net.cn

[R08] 数值比较
来源：http://xh.chemitech.net.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://ip.521024.cn

[R09] 字符串比较
来源：http://un.521024.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://bz.shxzukj.cn

[R10] 正则匹配
来源：http://mc.huixiangedu.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mo.nszjky.cn

[R11] case 多分支
来源：http://bp.huixinmuqiang.cn

case "$1" in
来源：http://az.wgjwhj.cn

start) echo "启动" ;;
来源：http://xx.9csxet.cn

stop)  echo "停止" ;;
来源：http://fu.asd995.cn

*)     echo "未知命令" ;;
来源：http://rr.newstarts.cn

esac
来源：http://wc.wgjwhj.cn

[R12] for 遍历文件
来源：http://od.yuexingan06.cn

for f in *.txt; do echo "$f"; done
来源：http://qr.newstarts.cn

[R13] for 计数循环
来源：http://rg.newstarts.cn

for i in {1..10}; do echo "$i"; done
来源：http://it.lnxyls.cn

[R14] C 风格 for
来源：http://ak.nicolike.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://nn.bookmarksfly.cn

[R15] while 逐行读文件
来源：http://de.shxzskj.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://sa.yuntaijiaju.cn

[R16] until 等待条件
来源：http://wi.521024.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://px.huixinmuqiang.cn

[R17] 数组定义与取值
来源：http://lk.huanxung.cn

arr=(a b c); echo "${arr[0]}"
来源：http://eo.chemitech.net.cn

[R18] 遍历数组
来源：http://gb.yuexingan06.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://vc.szsharing.cn

[R19] 数组长度
来源：http://cx.asd995.cn

echo "${#arr[@]}"
来源：http://vb.hnjuh.cn

[R20] 关联数组（字典）
来源：http://vo.panjiajie.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://jj.yuntaijiaju.cn

[R21] 字符串长度
来源：http://ft.shxzskj.cn

echo "${#s}"
来源：http://pp.wgjwhj.cn

[R22] 截取子串
来源：http://cw.jctech888.com.cn

echo "${s:0:5}"
来源：http://fx.szxytkj.cn

[R23] 字符串替换
来源：http://gx.wgjwhj.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ce.shtwfgs.cn

[R24] 大小写转换
来源：http://qe.chemitech.net.cn

echo "${s^^}"; echo "${s,,}"
来源：http://aj.yuexingan06.cn

[R25] 去后缀 / 去前缀
来源：http://wl.shxzskj.cn


<!-- 参考信息 -->