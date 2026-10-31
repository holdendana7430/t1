代发 wailian999

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://bw.huanxung.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ap.huanxung.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ru.newstarts.cn

PHP:  if (empty($x)) {}
来源：http://ze.lnxyls.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://lu.huixiangedu.cn

TS:   if (x == null) {}
来源：http://fb.colortex.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://gj.shxzukj.cn

Go:   if x == nil {}
来源：http://lk.shtwfgs.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ax.huixiangedu.cn

C#:   if (x is null) {}
来源：http://qt.szsharing.cn

[P07] 防抖与节流
来源：http://qt.hnjuh.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ke.hnjuh.cn

PHP:  // 手写时间戳比较
来源：http://mr.huanxung.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qg.gzmigu.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://yg.chemitech.net.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://zu.bookmarksfly.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ya.muxihuayi.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://de.shtwfgs.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ax.szxytkj.cn

[P08] 处理浮点精度问题
来源：http://ej.bjjhwx.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://jd.chemitech.net.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://yu.yuntaijiaju.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://dj.shxzskj.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://xs.huixinmuqiang.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ko.panjiajie.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://na.jctech888.com.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://sr.szsharing.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ca.wgjwhj.cn

================================================================================
来源：http://dc.bjjhwx.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ie.hnjuh.cn

================================================================================
来源：http://ii.hahajie.cn

[Q01] 创建表
来源：http://ib.chemitech.net.cn

CREATE TABLE users (
来源：http://bo.szxytkj.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://vy.hahajie.cn

name VARCHAR(50) NOT NULL,
来源：http://dx.nicolike.cn

email VARCHAR(100) UNIQUE,
来源：http://ie.yuntaijiaju.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://du.jianghongdianzi.cn

);
来源：http://fj.bookmarksfly.cn

[Q02] 创建带外键的表
来源：http://fj.shxzukj.cn

CREATE TABLE orders (
来源：http://am.521024.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://do.panjiajie.cn

user_id INT NOT NULL,
来源：http://yz.huixinmuqiang.cn

amount DECIMAL(10, 2),
来源：http://iq.jianghongdianzi.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://vq.huixiangedu.cn

);
来源：http://zq.nicolike.cn

[Q03] 增加列
来源：http://jn.bookmarksfly.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hi.hnjuh.cn

[Q04] 修改列类型
来源：http://eq.jctech888.com.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://zo.shxzskj.cn

[Q05] 重命名列
来源：http://uo.haigaiapp.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://nf.yuexingan06.cn

[Q06] 删除列
来源：http://xc.szsharing.cn

ALTER TABLE users DROP COLUMN age;
来源：http://af.szsharing.cn

[Q07] 删除表
来源：http://ht.shtwfgs.cn

DROP TABLE IF EXISTS orders;
来源：http://vg.huixinmuqiang.cn

[Q08] 创建普通索引
来源：http://tv.9csxet.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://wk.huixiangedu.cn

[Q09] 创建唯一索引
来源：http://lf.szsharing.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ml.huanxung.cn

[Q10] 插入单行
来源：http://lo.haigaiapp.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://gn.shxzukj.cn

[Q11] 一次插入多行
来源：http://xo.colortex.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://iw.haigaiapp.cn

[Q12] 插入后取自增 ID
来源：http://yw.haigaiapp.cn

INSERT INTO users (name) VALUES ('C');
来源：http://ni.gzmigu.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://vd.colortex.cn

[Q13] 忽略重复插入
来源：http://nb.yuntaijiaju.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://qr.bookmarksfly.cn

[Q14] 存在则更新（upsert）
来源：http://ie.shtwfgs.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://xu.bjjhwx.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mz.chemitech.net.cn

[Q15] 查询全部
来源：http://jp.shxzukj.cn

SELECT * FROM users;
来源：http://wf.szxytkj.cn

[Q16] 查询指定列
来源：http://ym.huanxung.cn

SELECT id, name FROM users;
来源：http://rg.chemitech.net.cn

[Q17] 条件查询
来源：http://ga.shxzskj.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://lg.hahajie.cn

[Q18] 模糊匹配
来源：http://jn.jianghongdianzi.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ne.chemitech.net.cn

[Q19] 范围查询
来源：http://uz.haigaiapp.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://cc.shtwfgs.cn

[Q20] IN 列表
来源：http://oz.gzmigu.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://bk.shtwfgs.cn

[Q21] 空值判断
来源：http://tm.9csxet.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://db.521024.cn

[Q22] 排序
来源：http://bb.lnxyls.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://jl.szsharing.cn

[Q23] 分页
来源：http://xc.yuntaijiaju.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://dw.shtwfgs.cn

[Q24] 去重
来源：http://it.gzmigu.cn

SELECT DISTINCT city FROM users;
来源：http://jq.lnxyls.cn

[Q25] 只取前 N 条
来源：http://ld.shxzukj.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ce.shxzukj.cn

[Q26] 计数
来源：http://um.huixinmuqiang.cn

SELECT COUNT(*) FROM users;
来源：http://ai.jianghongdianzi.cn

[Q27] 条件计数
来源：http://hj.panjiajie.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mu.panjiajie.cn

[Q28] 求和与平均
来源：http://jr.haigaiapp.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://cu.hahajie.cn

[Q29] 最大最小值
来源：http://za.bookmarksfly.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://rs.nszjky.cn

[Q30] 分组统计
来源：http://vm.gzmigu.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://me.szxytkj.cn

[Q31] 分组后过滤
来源：http://tp.bookmarksfly.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mx.muxihuayi.cn

[Q32] 分组拼接字符串
来源：http://rn.huixinmuqiang.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://tn.jctech888.com.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ds.asd995.cn

[Q33] 多列分组
来源：http://ss.yuexingan06.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://he.hahajie.cn

[Q34] 每组取第一条
来源：http://rk.shxzukj.cn

SELECT * FROM (
来源：http://fr.bookmarksfly.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://om.muxihuayi.cn

) t WHERE rn = 1;
来源：http://yy.szxytkj.cn

[Q35] 内连接
来源：http://rt.haigaiapp.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://lo.shtwfgs.cn

[Q36] 左连接
来源：http://db.lnxyls.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ay.521024.cn

[Q37] 右连接
来源：http://mw.yuntaijiaju.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ze.asd995.cn

[Q38] 全外连接（PostgreSQL）
来源：http://kb.shtwfgs.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://cf.chemitech.net.cn

[Q39] 自连接（查上下级）
来源：http://hr.nicolike.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://ld.nszjky.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mw.newstarts.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://vi.panjiajie.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://oa.bookmarksfly.cn

[Q41] 多表连接
来源：http://hn.yuntaijiaju.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://ay.huanxung.cn

JOIN users u ON u.id = o.user_id
来源：http://vo.nszjky.cn

JOIN products p ON p.id = o.product_id;
来源：http://io.newstarts.cn

[Q42] 连接条件附加过滤
来源：http://mg.wgjwhj.cn

SELECT u.name, o.amount FROM users u
来源：http://vd.shxzukj.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://lp.bookmarksfly.cn

[Q43] 标量子查询
来源：http://ga.szxytkj.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ou.shxzukj.cn

[Q44] IN 子查询
来源：http://ih.huixinmuqiang.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://le.nszjky.cn

[Q45] EXISTS 判断存在
来源：http://hj.colortex.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ln.gzmigu.cn

[Q46] NOT EXISTS 判断不存在
来源：http://ct.wgjwhj.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://rv.huixiangedu.cn

[Q47] 与平均值比较
来源：http://jh.wgjwhj.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://sp.hnjuh.cn

[Q48] CTE 公用表表达式
来源：http://ut.hahajie.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://az.hahajie.cn

SELECT * FROM t WHERE c > 5;
来源：http://gl.lnxyls.cn

[Q49] 更新单行
来源：http://ds.muxihuayi.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://oq.shtwfgs.cn

[Q50] 批量更新
来源：http://sl.nszjky.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://lr.newstarts.cn

[Q51] 用子查询更新
来源：http://ms.haigaiapp.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://la.bjjhwx.cn

[Q52] 删除指定行
来源：http://sf.nszjky.cn

DELETE FROM users WHERE id = 10;
来源：http://zk.chemitech.net.cn

[Q53] 按条件删除
来源：http://xb.bookmarksfly.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://uq.haigaiapp.cn

[Q54] 清空表
来源：http://xi.szxytkj.cn

TRUNCATE TABLE logs;
来源：http://as.521024.cn

[Q55] 排名（并列占位）
来源：http://vz.hahajie.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://nl.yuntaijiaju.cn

[Q56] 密集排名（并列不占位）
来源：http://vd.huixiangedu.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://dk.lnxyls.cn

[Q57] 行号
来源：http://ra.asd995.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://bb.huixinmuqiang.cn

[Q58] 累计求和
来源：http://ao.hahajie.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ii.shtwfgs.cn

[Q59] 分组内累计
来源：http://zm.haigaiapp.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://xr.lnxyls.cn

[Q60] 取上一行 / 下一行
来源：http://yh.chemitech.net.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mz.shtwfgs.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://xe.huixiangedu.cn

[Q61] 移动平均
来源：http://kv.nicolike.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ta.asd995.cn

[Q62] 分组占比
来源：http://mk.huixinmuqiang.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://qm.shxzukj.cn

[Q63] 开启事务
来源：http://ia.yuntaijiaju.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://eh.panjiajie.cn

[Q64] 提交事务
来源：http://de.asd995.cn

COMMIT;
来源：http://ji.newstarts.cn

[Q65] 回滚事务
来源：http://hs.chemitech.net.cn

ROLLBACK;
来源：http://wf.hahajie.cn

[Q66] 行锁查询
来源：http://jw.huixinmuqiang.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ca.huixiangedu.cn

[Q67] 设置隔离级别
来源：http://ql.colortex.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://nz.gzmigu.cn

[Q68] 保存点
来源：http://vt.haigaiapp.cn

SAVEPOINT sp1;
来源：http://bk.bookmarksfly.cn

ROLLBACK TO sp1;
来源：http://fl.521024.cn

[Q69] 查看执行计划
来源：http://jn.hnjuh.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://dm.nszjky.cn

[Q70] 更新统计信息
来源：http://nr.asd995.cn

ANALYZE TABLE users;
来源：http://cr.huanxung.cn

[Q71] 查看建表语句
来源：http://em.huanxung.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://oc.muxihuayi.cn

[Q72] 查看索引
来源：http://ri.haigaiapp.cn

SHOW INDEX FROM users;
来源：http://en.szsharing.cn

[Q73] 查看表状态
来源：http://oa.lnxyls.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://fw.huixiangedu.cn

[Q74] 强制使用索引
来源：http://lg.hahajie.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://sk.wgjwhj.cn

[Q75] 日期格式化
来源：http://fu.bjjhwx.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://um.hahajie.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ch.lnxyls.cn

[Q76] 按天统计
来源：http://xd.9csxet.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://lb.shxzskj.cn

[Q77] 时间加减
来源：http://rn.bjjhwx.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://pf.jianghongdianzi.cn

[Q78] 当前时间
来源：http://gc.asd995.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ov.jianghongdianzi.cn

[Q79] 字符串拼接
来源：http://tm.shxzskj.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.chemitech.net.cn

[Q80] 字符串截取
来源：http://xb.haigaiapp.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://bg.wgjwhj.cn

[Q81] 字符串替换
来源：http://nq.521024.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://sc.nszjky.cn

[Q82] 字符长度与字节长度
来源：http://ll.shxzukj.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://cf.muxihuayi.cn

[Q83] 大小写转换
来源：http://mv.newstarts.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hr.shxzskj.cn

[Q84] 去除首尾空格
来源：http://pq.hahajie.cn

SELECT TRIM(name) FROM users;
来源：http://fw.newstarts.cn

[Q85] 数值取整
来源：http://iw.jctech888.com.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ir.szxytkj.cn

[Q86] 读取 JSON 字段
来源：http://rj.shxzukj.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://py.huixinmuqiang.cn

[Q87] JSON 字段做条件
来源：http://hq.bookmarksfly.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://fr.hnjuh.cn

[Q88] 行转列（条件聚合）
来源：http://qu.hahajie.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wj.szsharing.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://vk.shxzukj.cn

[Q89] 判断表是否存在
来源：http://zp.chemitech.net.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://lk.shxzukj.cn

[Q90] 生成序号列
来源：http://zx.wgjwhj.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mf.shxzukj.cn

================================================================================
来源：http://su.hnjuh.cn

R. Bash 专题
来源：http://hh.panjiajie.cn

================================================================================
来源：http://lm.9csxet.cn

[R01] shebang 与严格模式
来源：http://ro.hnjuh.cn

#!/usr/bin/env bash
来源：http://uu.jianghongdianzi.cn

set -euo pipefail
来源：http://pv.muxihuayi.cn

[R02] 变量赋值与使用
来源：http://tk.9csxet.cn

name="Tom"; echo "$name"
来源：http://uz.9csxet.cn

[R03] 只读变量
来源：http://wy.wgjwhj.cn

readonly PI=3.14
来源：http://se.huanxung.cn

[R04] 位置参数
来源：http://np.panjiajie.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://eu.9csxet.cn

[R05] 参数默认值
来源：http://ui.haigaiapp.cn

name="${1:-default}"
来源：http://fy.hnjuh.cn

[R06] 判断命令是否存在
来源：http://xl.gzmigu.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ud.shxzskj.cn

[R07] if 判断文件
来源：http://yx.9csxet.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://jb.jianghongdianzi.cn

[R08] 数值比较
来源：http://fh.nicolike.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://id.521024.cn

[R09] 字符串比较
来源：http://oe.yuntaijiaju.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://zx.521024.cn

[R10] 正则匹配
来源：http://ax.haigaiapp.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://tx.gzmigu.cn

[R11] case 多分支
来源：http://lb.wgjwhj.cn

case "$1" in
来源：http://tc.muxihuayi.cn

start) echo "启动" ;;
来源：http://gq.muxihuayi.cn

stop)  echo "停止" ;;
来源：http://pc.jctech888.com.cn

*)     echo "未知命令" ;;
来源：http://bo.panjiajie.cn

esac
来源：http://pg.521024.cn

[R12] for 遍历文件
来源：http://kx.wgjwhj.cn

for f in *.txt; do echo "$f"; done
来源：http://sn.chemitech.net.cn

[R13] for 计数循环
来源：http://yx.nicolike.cn

for i in {1..10}; do echo "$i"; done
来源：http://et.hnjuh.cn

[R14] C 风格 for
来源：http://rx.nicolike.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://zv.lnxyls.cn

[R15] while 逐行读文件
来源：http://gg.bjjhwx.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://qs.521024.cn

[R16] until 等待条件
来源：http://fa.panjiajie.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://tf.hnjuh.cn

[R17] 数组定义与取值
来源：http://ts.shxzskj.cn

arr=(a b c); echo "${arr[0]}"
来源：http://ht.521024.cn

[R18] 遍历数组
来源：http://ig.yuntaijiaju.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ep.panjiajie.cn

[R19] 数组长度
来源：http://jy.szsharing.cn

echo "${#arr[@]}"
来源：http://oz.yuntaijiaju.cn

[R20] 关联数组（字典）
来源：http://yo.szxytkj.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://kr.shxzukj.cn

[R21] 字符串长度
来源：http://hq.asd995.cn

echo "${#s}"
来源：http://lr.yuexingan06.cn

[R22] 截取子串
来源：http://us.gzmigu.cn

echo "${s:0:5}"
来源：http://mm.hahajie.cn

[R23] 字符串替换
来源：http://pc.haigaiapp.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://cw.chemitech.net.cn

[R24] 大小写转换
来源：http://zn.yuexingan06.cn

echo "${s^^}"; echo "${s,,}"
来源：http://lv.muxihuayi.cn

[R25] 去后缀 / 去前缀
来源：http://aa.huixiangedu.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://uf.asd995.cn

[R26] 命令替换
来源：http://re.wgjwhj.cn

now=$(date +%F); echo "$now"
来源：http://nf.gzmigu.cn

[R27] 算术展开
来源：http://zf.shxzskj.cn

echo $((1 + 2 * 3))
来源：http://rv.bjjhwx.cn

[R28] 浮点运算
来源：http://og.yuexingan06.cn

echo "scale=2; 10/3" | bc
来源：http://hg.shxzukj.cn

[R29] 定义函数
来源：http://km.shxzskj.cn


<!-- 参考信息 -->