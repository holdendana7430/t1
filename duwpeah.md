代发 wailian999

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ep.colortex.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://lt.jctech888.com.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://dd.gzmigu.cn

PHP:  if (empty($x)) {}
来源：http://uk.bookmarksfly.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://rt.gzmigu.cn

TS:   if (x == null) {}
来源：http://mn.nicolike.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://at.muxihuayi.cn

Go:   if x == nil {}
来源：http://qw.asd995.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://rr.521024.cn

C#:   if (x is null) {}
来源：http://qz.bjjhwx.cn

[P07] 防抖与节流
来源：http://kr.jianghongdianzi.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://sa.wgjwhj.cn

PHP:  // 手写时间戳比较
来源：http://vu.yuntaijiaju.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xc.szxytkj.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://sa.shxzukj.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://go.jianghongdianzi.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ci.jianghongdianzi.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://pc.bjjhwx.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://vw.jctech888.com.cn

[P08] 处理浮点精度问题
来源：http://pg.bookmarksfly.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://cm.muxihuayi.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://lu.nicolike.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://eu.shxzskj.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://vv.lnxyls.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://vp.newstarts.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://vj.hahajie.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hw.huixiangedu.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://tr.chemitech.net.cn

================================================================================
来源：http://wv.szsharing.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://qo.yuntaijiaju.cn

================================================================================
来源：http://bg.hnjuh.cn

[Q01] 创建表
来源：http://vc.shtwfgs.cn

CREATE TABLE users (
来源：http://yj.yuntaijiaju.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ad.asd995.cn

name VARCHAR(50) NOT NULL,
来源：http://jp.yuntaijiaju.cn

email VARCHAR(100) UNIQUE,
来源：http://ee.huixiangedu.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://oe.shxzukj.cn

);
来源：http://zw.yuntaijiaju.cn

[Q02] 创建带外键的表
来源：http://je.521024.cn

CREATE TABLE orders (
来源：http://jb.newstarts.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://cr.chemitech.net.cn

user_id INT NOT NULL,
来源：http://qe.muxihuayi.cn

amount DECIMAL(10, 2),
来源：http://cr.shxzskj.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ua.nszjky.cn

);
来源：http://af.nicolike.cn

[Q03] 增加列
来源：http://fb.gzmigu.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ob.shtwfgs.cn

[Q04] 修改列类型
来源：http://qu.newstarts.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hm.hahajie.cn

[Q05] 重命名列
来源：http://yg.nszjky.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://sg.colortex.cn

[Q06] 删除列
来源：http://nu.colortex.cn

ALTER TABLE users DROP COLUMN age;
来源：http://pd.yuntaijiaju.cn

[Q07] 删除表
来源：http://nh.asd995.cn

DROP TABLE IF EXISTS orders;
来源：http://az.yuntaijiaju.cn

[Q08] 创建普通索引
来源：http://ve.muxihuayi.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://ug.colortex.cn

[Q09] 创建唯一索引
来源：http://hp.szxytkj.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wc.muxihuayi.cn

[Q10] 插入单行
来源：http://hm.haigaiapp.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://pi.521024.cn

[Q11] 一次插入多行
来源：http://uq.nszjky.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://jh.wgjwhj.cn

[Q12] 插入后取自增 ID
来源：http://fu.hnjuh.cn

INSERT INTO users (name) VALUES ('C');
来源：http://az.szxytkj.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wt.chemitech.net.cn

[Q13] 忽略重复插入
来源：http://jr.nszjky.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://fp.bookmarksfly.cn

[Q14] 存在则更新（upsert）
来源：http://we.jianghongdianzi.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://sw.yuntaijiaju.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://dg.hahajie.cn

[Q15] 查询全部
来源：http://nw.asd995.cn

SELECT * FROM users;
来源：http://jm.huixinmuqiang.cn

[Q16] 查询指定列
来源：http://as.shxzukj.cn

SELECT id, name FROM users;
来源：http://gy.shtwfgs.cn

[Q17] 条件查询
来源：http://ty.huixinmuqiang.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://vb.szsharing.cn

[Q18] 模糊匹配
来源：http://uq.lnxyls.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://xy.lnxyls.cn

[Q19] 范围查询
来源：http://fb.szsharing.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ko.haigaiapp.cn

[Q20] IN 列表
来源：http://nq.9csxet.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://vs.muxihuayi.cn

[Q21] 空值判断
来源：http://nx.lnxyls.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://jz.jianghongdianzi.cn

[Q22] 排序
来源：http://dx.hnjuh.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://bc.haigaiapp.cn

[Q23] 分页
来源：http://ku.bjjhwx.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ju.szxytkj.cn

[Q24] 去重
来源：http://sh.lnxyls.cn

SELECT DISTINCT city FROM users;
来源：http://wp.huanxung.cn

[Q25] 只取前 N 条
来源：http://vj.chemitech.net.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://fz.huixinmuqiang.cn

[Q26] 计数
来源：http://ef.hahajie.cn

SELECT COUNT(*) FROM users;
来源：http://mc.szsharing.cn

[Q27] 条件计数
来源：http://oy.nszjky.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ed.9csxet.cn

[Q28] 求和与平均
来源：http://uf.huanxung.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://ja.521024.cn

[Q29] 最大最小值
来源：http://ji.yuntaijiaju.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://kq.huanxung.cn

[Q30] 分组统计
来源：http://gj.hnjuh.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wm.muxihuayi.cn

[Q31] 分组后过滤
来源：http://uw.jianghongdianzi.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ni.huanxung.cn

[Q32] 分组拼接字符串
来源：http://ms.muxihuayi.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://nv.chemitech.net.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wv.shtwfgs.cn

[Q33] 多列分组
来源：http://oy.asd995.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://qs.nicolike.cn

[Q34] 每组取第一条
来源：http://dh.lnxyls.cn

SELECT * FROM (
来源：http://zl.shxzukj.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ht.hnjuh.cn

) t WHERE rn = 1;
来源：http://rr.bookmarksfly.cn

[Q35] 内连接
来源：http://ay.huixiangedu.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://rx.lnxyls.cn

[Q36] 左连接
来源：http://yi.huixinmuqiang.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ee.huixiangedu.cn

[Q37] 右连接
来源：http://pz.hnjuh.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ve.nszjky.cn

[Q38] 全外连接（PostgreSQL）
来源：http://cv.hnjuh.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ap.nicolike.cn

[Q39] 自连接（查上下级）
来源：http://sp.nszjky.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://kv.bjjhwx.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://vz.haigaiapp.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://jy.bookmarksfly.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://kh.jctech888.com.cn

[Q41] 多表连接
来源：http://pl.shxzskj.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://ug.huixinmuqiang.cn

JOIN users u ON u.id = o.user_id
来源：http://lx.panjiajie.cn

JOIN products p ON p.id = o.product_id;
来源：http://lg.huixiangedu.cn

[Q42] 连接条件附加过滤
来源：http://fu.haigaiapp.cn

SELECT u.name, o.amount FROM users u
来源：http://ox.hahajie.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ab.huanxung.cn

[Q43] 标量子查询
来源：http://zm.muxihuayi.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ws.shxzukj.cn

[Q44] IN 子查询
来源：http://kb.shxzukj.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ou.lnxyls.cn

[Q45] EXISTS 判断存在
来源：http://xv.bjjhwx.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://qi.lnxyls.cn

[Q46] NOT EXISTS 判断不存在
来源：http://iu.colortex.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ap.nicolike.cn

[Q47] 与平均值比较
来源：http://gx.yuntaijiaju.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ni.panjiajie.cn

[Q48] CTE 公用表表达式
来源：http://uv.gzmigu.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://gb.lnxyls.cn

SELECT * FROM t WHERE c > 5;
来源：http://ul.huixinmuqiang.cn

[Q49] 更新单行
来源：http://ce.bookmarksfly.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://bq.colortex.cn

[Q50] 批量更新
来源：http://nw.szsharing.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://is.huanxung.cn

[Q51] 用子查询更新
来源：http://qn.gzmigu.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://im.szxytkj.cn

[Q52] 删除指定行
来源：http://br.lnxyls.cn

DELETE FROM users WHERE id = 10;
来源：http://xq.huixiangedu.cn

[Q53] 按条件删除
来源：http://ih.9csxet.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://zm.9csxet.cn

[Q54] 清空表
来源：http://qm.jianghongdianzi.cn

TRUNCATE TABLE logs;
来源：http://jd.newstarts.cn

[Q55] 排名（并列占位）
来源：http://ak.huixinmuqiang.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://sg.bookmarksfly.cn

[Q56] 密集排名（并列不占位）
来源：http://ua.lnxyls.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://bp.yuntaijiaju.cn

[Q57] 行号
来源：http://vf.lnxyls.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://zm.gzmigu.cn

[Q58] 累计求和
来源：http://tj.hnjuh.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://rq.bjjhwx.cn

[Q59] 分组内累计
来源：http://is.nszjky.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://un.huixinmuqiang.cn

[Q60] 取上一行 / 下一行
来源：http://vl.shtwfgs.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://cm.9csxet.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ey.huixinmuqiang.cn

[Q61] 移动平均
来源：http://ab.bookmarksfly.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://oy.9csxet.cn

[Q62] 分组占比
来源：http://uc.521024.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://qn.huixiangedu.cn

[Q63] 开启事务
来源：http://vt.haigaiapp.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://bz.szsharing.cn

[Q64] 提交事务
来源：http://xp.jctech888.com.cn

COMMIT;
来源：http://yr.muxihuayi.cn

[Q65] 回滚事务
来源：http://cv.yuexingan06.cn

ROLLBACK;
来源：http://iz.wgjwhj.cn

[Q66] 行锁查询
来源：http://do.huixiangedu.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://on.gzmigu.cn

[Q67] 设置隔离级别
来源：http://nh.asd995.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hw.bjjhwx.cn

[Q68] 保存点
来源：http://ld.521024.cn

SAVEPOINT sp1;
来源：http://nd.newstarts.cn

ROLLBACK TO sp1;
来源：http://tw.haigaiapp.cn

[Q69] 查看执行计划
来源：http://bx.newstarts.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://jv.hahajie.cn

[Q70] 更新统计信息
来源：http://np.asd995.cn

ANALYZE TABLE users;
来源：http://zi.muxihuayi.cn

[Q71] 查看建表语句
来源：http://gi.nicolike.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://rc.wgjwhj.cn

[Q72] 查看索引
来源：http://aw.9csxet.cn

SHOW INDEX FROM users;
来源：http://fl.wgjwhj.cn

[Q73] 查看表状态
来源：http://sg.chemitech.net.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://id.gzmigu.cn

[Q74] 强制使用索引
来源：http://uo.521024.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://kk.lnxyls.cn

[Q75] 日期格式化
来源：http://wa.bookmarksfly.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://qp.nszjky.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wy.gzmigu.cn

[Q76] 按天统计
来源：http://vy.huixinmuqiang.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://nl.bookmarksfly.cn

[Q77] 时间加减
来源：http://dg.nszjky.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://eh.huanxung.cn

[Q78] 当前时间
来源：http://mw.jctech888.com.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://jh.szsharing.cn

[Q79] 字符串拼接
来源：http://uo.panjiajie.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://fm.nicolike.cn

[Q80] 字符串截取
来源：http://wh.lnxyls.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mt.shxzukj.cn

[Q81] 字符串替换
来源：http://lk.lnxyls.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://oi.nicolike.cn

[Q82] 字符长度与字节长度
来源：http://jm.shtwfgs.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://dk.lnxyls.cn

[Q83] 大小写转换
来源：http://ik.nicolike.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://qc.bookmarksfly.cn

[Q84] 去除首尾空格
来源：http://oa.muxihuayi.cn

SELECT TRIM(name) FROM users;
来源：http://fk.newstarts.cn

[Q85] 数值取整
来源：http://vz.9csxet.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://xm.bjjhwx.cn

[Q86] 读取 JSON 字段
来源：http://xo.lnxyls.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://us.newstarts.cn

[Q87] JSON 字段做条件
来源：http://uw.muxihuayi.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://zq.shxzskj.cn

[Q88] 行转列（条件聚合）
来源：http://op.shxzukj.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://th.yuexingan06.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://bc.chemitech.net.cn

[Q89] 判断表是否存在
来源：http://dr.lnxyls.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ed.jianghongdianzi.cn

[Q90] 生成序号列
来源：http://he.nszjky.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://sr.huixinmuqiang.cn

================================================================================
来源：http://sf.szxytkj.cn

R. Bash 专题
来源：http://py.bookmarksfly.cn

================================================================================
来源：http://gb.521024.cn

[R01] shebang 与严格模式
来源：http://sa.huixinmuqiang.cn

#!/usr/bin/env bash
来源：http://yn.wgjwhj.cn

set -euo pipefail
来源：http://mv.haigaiapp.cn

[R02] 变量赋值与使用
来源：http://ow.shxzskj.cn

name="Tom"; echo "$name"
来源：http://nk.shxzukj.cn

[R03] 只读变量
来源：http://uj.asd995.cn

readonly PI=3.14
来源：http://rh.muxihuayi.cn

[R04] 位置参数
来源：http://gm.szsharing.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ms.hahajie.cn

[R05] 参数默认值
来源：http://lt.huixinmuqiang.cn

name="${1:-default}"
来源：http://as.haigaiapp.cn

[R06] 判断命令是否存在
来源：http://ax.muxihuayi.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ri.szsharing.cn

[R07] if 判断文件
来源：http://fx.huixinmuqiang.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://iz.szsharing.cn

[R08] 数值比较
来源：http://hl.521024.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://ea.hahajie.cn

[R09] 字符串比较
来源：http://hr.haigaiapp.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://jn.shtwfgs.cn

[R10] 正则匹配
来源：http://lq.jctech888.com.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://xw.yuexingan06.cn

[R11] case 多分支
来源：http://dh.shxzskj.cn

case "$1" in
来源：http://pu.9csxet.cn

start) echo "启动" ;;
来源：http://kv.nicolike.cn

stop)  echo "停止" ;;
来源：http://dg.lnxyls.cn

*)     echo "未知命令" ;;
来源：http://rg.muxihuayi.cn

esac
来源：http://za.huixiangedu.cn

[R12] for 遍历文件
来源：http://sb.wgjwhj.cn

for f in *.txt; do echo "$f"; done
来源：http://im.nszjky.cn

[R13] for 计数循环
来源：http://br.shxzukj.cn

for i in {1..10}; do echo "$i"; done
来源：http://of.nicolike.cn

[R14] C 风格 for
来源：http://zf.haigaiapp.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ec.shxzskj.cn

[R15] while 逐行读文件
来源：http://tc.szsharing.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://on.nicolike.cn

[R16] until 等待条件
来源：http://an.yuexingan06.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ae.yuexingan06.cn

[R17] 数组定义与取值
来源：http://tz.szxytkj.cn

arr=(a b c); echo "${arr[0]}"
来源：http://co.lnxyls.cn

[R18] 遍历数组
来源：http://ry.colortex.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ya.shtwfgs.cn

[R19] 数组长度
来源：http://id.haigaiapp.cn

echo "${#arr[@]}"
来源：http://zr.wgjwhj.cn

[R20] 关联数组（字典）
来源：http://my.szxytkj.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ld.jianghongdianzi.cn

[R21] 字符串长度
来源：http://qy.szsharing.cn

echo "${#s}"
来源：http://wc.huixiangedu.cn

[R22] 截取子串
来源：http://vm.huixiangedu.cn

echo "${s:0:5}"
来源：http://wj.bookmarksfly.cn

[R23] 字符串替换
来源：http://ei.lnxyls.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://jp.haigaiapp.cn

[R24] 大小写转换
来源：http://fl.huanxung.cn

echo "${s^^}"; echo "${s,,}"
来源：http://xz.shtwfgs.cn

[R25] 去后缀 / 去前缀
来源：http://kv.huixiangedu.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://an.shtwfgs.cn

[R26] 命令替换
来源：http://dy.shtwfgs.cn

now=$(date +%F); echo "$now"
来源：http://zr.szxytkj.cn

[R27] 算术展开
来源：http://ud.chemitech.net.cn

echo $((1 + 2 * 3))
来源：http://sf.colortex.cn

[R28] 浮点运算
来源：http://ly.yuntaijiaju.cn

echo "scale=2; 10/3" | bc
来源：http://yh.shxzskj.cn

[R29] 定义函数
来源：http://rm.yuexingan06.cn


<!-- 参考信息 -->