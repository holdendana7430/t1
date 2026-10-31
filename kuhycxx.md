代发 wailian999

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://cf.huixiangedu.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://rf.gzmigu.cn

Go:   reflect.DeepEqual(a, b)
来源：http://iy.shxzskj.cn

Ruby: a == b
来源：http://ti.newstarts.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ga.hahajie.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mw.szxytkj.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://kb.huanxung.cn

PHP:  if (empty($x)) {}
来源：http://jo.521024.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://pb.huanxung.cn

TS:   if (x == null) {}
来源：http://hi.yuexingan06.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://fm.yuexingan06.cn

Go:   if x == nil {}
来源：http://tu.yuexingan06.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ii.haigaiapp.cn

C#:   if (x is null) {}
来源：http://kx.jctech888.com.cn

[P07] 防抖与节流
来源：http://ci.shxzukj.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://zp.haigaiapp.cn

PHP:  // 手写时间戳比较
来源：http://ke.szsharing.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://bf.hahajie.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://zb.nszjky.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://jl.521024.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://xp.panjiajie.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://ka.yuntaijiaju.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://bh.bookmarksfly.cn

[P08] 处理浮点精度问题
来源：http://dc.shxzskj.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://gl.szsharing.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://zx.9csxet.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://kd.colortex.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://es.nszjky.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://yp.szsharing.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://pg.nicolike.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://kv.nicolike.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://fd.bjjhwx.cn

================================================================================
来源：http://ep.jctech888.com.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ir.haigaiapp.cn

================================================================================
来源：http://yq.huixiangedu.cn

[Q01] 创建表
来源：http://xs.szxytkj.cn

CREATE TABLE users (
来源：http://vo.jctech888.com.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://sl.shtwfgs.cn

name VARCHAR(50) NOT NULL,
来源：http://sw.hahajie.cn

email VARCHAR(100) UNIQUE,
来源：http://nr.shxzskj.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://uf.colortex.cn

);
来源：http://gr.jianghongdianzi.cn

[Q02] 创建带外键的表
来源：http://wo.nszjky.cn

CREATE TABLE orders (
来源：http://bd.521024.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://iw.jctech888.com.cn

user_id INT NOT NULL,
来源：http://rl.9csxet.cn

amount DECIMAL(10, 2),
来源：http://vk.szsharing.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://bh.panjiajie.cn

);
来源：http://gq.chemitech.net.cn

[Q03] 增加列
来源：http://bg.bookmarksfly.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://se.hnjuh.cn

[Q04] 修改列类型
来源：http://tk.521024.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://pp.shxzukj.cn

[Q05] 重命名列
来源：http://yf.haigaiapp.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://cp.shxzukj.cn

[Q06] 删除列
来源：http://pg.shxzskj.cn

ALTER TABLE users DROP COLUMN age;
来源：http://wv.szsharing.cn

[Q07] 删除表
来源：http://ui.nicolike.cn

DROP TABLE IF EXISTS orders;
来源：http://im.huixiangedu.cn

[Q08] 创建普通索引
来源：http://zd.shtwfgs.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://gm.huanxung.cn

[Q09] 创建唯一索引
来源：http://ce.bookmarksfly.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://jr.bookmarksfly.cn

[Q10] 插入单行
来源：http://kp.hnjuh.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://tp.yuexingan06.cn

[Q11] 一次插入多行
来源：http://ec.nszjky.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://lh.muxihuayi.cn

[Q12] 插入后取自增 ID
来源：http://bc.bjjhwx.cn

INSERT INTO users (name) VALUES ('C');
来源：http://rv.huixiangedu.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://tq.9csxet.cn

[Q13] 忽略重复插入
来源：http://ga.wgjwhj.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://vw.9csxet.cn

[Q14] 存在则更新（upsert）
来源：http://cx.gzmigu.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wg.bookmarksfly.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://sr.szsharing.cn

[Q15] 查询全部
来源：http://yf.hnjuh.cn

SELECT * FROM users;
来源：http://dh.huanxung.cn

[Q16] 查询指定列
来源：http://ms.muxihuayi.cn

SELECT id, name FROM users;
来源：http://mc.lnxyls.cn

[Q17] 条件查询
来源：http://fg.asd995.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://gx.bjjhwx.cn

[Q18] 模糊匹配
来源：http://lm.muxihuayi.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ex.huixinmuqiang.cn

[Q19] 范围查询
来源：http://fn.bjjhwx.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://yr.shtwfgs.cn

[Q20] IN 列表
来源：http://yo.newstarts.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://vc.muxihuayi.cn

[Q21] 空值判断
来源：http://ud.szxytkj.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://ol.bookmarksfly.cn

[Q22] 排序
来源：http://sr.bookmarksfly.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://lq.hahajie.cn

[Q23] 分页
来源：http://dx.yuexingan06.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://pc.lnxyls.cn

[Q24] 去重
来源：http://zo.huanxung.cn

SELECT DISTINCT city FROM users;
来源：http://sl.newstarts.cn

[Q25] 只取前 N 条
来源：http://nl.huixinmuqiang.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://pb.newstarts.cn

[Q26] 计数
来源：http://at.9csxet.cn

SELECT COUNT(*) FROM users;
来源：http://vf.gzmigu.cn

[Q27] 条件计数
来源：http://qx.asd995.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://yu.gzmigu.cn

[Q28] 求和与平均
来源：http://es.huanxung.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://lg.shxzskj.cn

[Q29] 最大最小值
来源：http://sz.szxytkj.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://jl.hahajie.cn

[Q30] 分组统计
来源：http://pu.lnxyls.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://de.huanxung.cn

[Q31] 分组后过滤
来源：http://nn.huanxung.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://gw.huanxung.cn

[Q32] 分组拼接字符串
来源：http://pf.wgjwhj.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ee.jctech888.com.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://tp.huixinmuqiang.cn

[Q33] 多列分组
来源：http://iu.yuntaijiaju.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ra.jctech888.com.cn

[Q34] 每组取第一条
来源：http://lw.yuexingan06.cn

SELECT * FROM (
来源：http://zo.bookmarksfly.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://cj.asd995.cn

) t WHERE rn = 1;
来源：http://yb.shxzukj.cn

[Q35] 内连接
来源：http://dx.nicolike.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://qb.shxzskj.cn

[Q36] 左连接
来源：http://fl.huixinmuqiang.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://jx.jianghongdianzi.cn

[Q37] 右连接
来源：http://lz.hnjuh.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ti.colortex.cn

[Q38] 全外连接（PostgreSQL）
来源：http://vk.521024.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://zc.shxzskj.cn

[Q39] 自连接（查上下级）
来源：http://lz.panjiajie.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://we.huanxung.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mh.bjjhwx.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://vt.bjjhwx.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ij.jianghongdianzi.cn

[Q41] 多表连接
来源：http://xr.jctech888.com.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://wm.muxihuayi.cn

JOIN users u ON u.id = o.user_id
来源：http://iq.shtwfgs.cn

JOIN products p ON p.id = o.product_id;
来源：http://dx.bookmarksfly.cn

[Q42] 连接条件附加过滤
来源：http://gk.haigaiapp.cn

SELECT u.name, o.amount FROM users u
来源：http://uj.521024.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://vu.hahajie.cn

[Q43] 标量子查询
来源：http://ki.muxihuayi.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://oy.hahajie.cn

[Q44] IN 子查询
来源：http://if.colortex.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://xe.asd995.cn

[Q45] EXISTS 判断存在
来源：http://cn.shtwfgs.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://tp.jctech888.com.cn

[Q46] NOT EXISTS 判断不存在
来源：http://mw.521024.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ah.9csxet.cn

[Q47] 与平均值比较
来源：http://ty.muxihuayi.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ug.bookmarksfly.cn

[Q48] CTE 公用表表达式
来源：http://ys.shxzskj.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ce.newstarts.cn

SELECT * FROM t WHERE c > 5;
来源：http://if.szsharing.cn

[Q49] 更新单行
来源：http://tb.gzmigu.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ok.szxytkj.cn

[Q50] 批量更新
来源：http://rn.9csxet.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://oe.szsharing.cn

[Q51] 用子查询更新
来源：http://xj.shtwfgs.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wa.bookmarksfly.cn

[Q52] 删除指定行
来源：http://vl.lnxyls.cn

DELETE FROM users WHERE id = 10;
来源：http://pl.huanxung.cn

[Q53] 按条件删除
来源：http://fl.jctech888.com.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://sq.shxzskj.cn

[Q54] 清空表
来源：http://kc.newstarts.cn

TRUNCATE TABLE logs;
来源：http://ej.szxytkj.cn

[Q55] 排名（并列占位）
来源：http://vt.jctech888.com.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://dy.gzmigu.cn

[Q56] 密集排名（并列不占位）
来源：http://yb.muxihuayi.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://be.szsharing.cn

[Q57] 行号
来源：http://gw.lnxyls.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://pz.hahajie.cn

[Q58] 累计求和
来源：http://sl.asd995.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://rh.jctech888.com.cn

[Q59] 分组内累计
来源：http://sk.panjiajie.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://zz.yuexingan06.cn

[Q60] 取上一行 / 下一行
来源：http://sc.hahajie.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://up.nicolike.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://vm.colortex.cn

[Q61] 移动平均
来源：http://iw.9csxet.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://bv.jianghongdianzi.cn

[Q62] 分组占比
来源：http://cr.asd995.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ol.szsharing.cn

[Q63] 开启事务
来源：http://cz.muxihuayi.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://ng.nicolike.cn

[Q64] 提交事务
来源：http://ix.521024.cn

COMMIT;
来源：http://et.huanxung.cn

[Q65] 回滚事务
来源：http://sp.wgjwhj.cn

ROLLBACK;
来源：http://hs.jctech888.com.cn

[Q66] 行锁查询
来源：http://gt.szsharing.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ln.bjjhwx.cn

[Q67] 设置隔离级别
来源：http://ub.wgjwhj.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.shxzskj.cn

[Q68] 保存点
来源：http://ut.shxzukj.cn

SAVEPOINT sp1;
来源：http://sl.newstarts.cn

ROLLBACK TO sp1;
来源：http://hu.lnxyls.cn

[Q69] 查看执行计划
来源：http://jz.colortex.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://kc.hahajie.cn

[Q70] 更新统计信息
来源：http://da.jianghongdianzi.cn

ANALYZE TABLE users;
来源：http://qy.jianghongdianzi.cn

[Q71] 查看建表语句
来源：http://yb.muxihuayi.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://rp.9csxet.cn

[Q72] 查看索引
来源：http://vj.nicolike.cn

SHOW INDEX FROM users;
来源：http://hh.colortex.cn

[Q73] 查看表状态
来源：http://zb.jianghongdianzi.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://rh.wgjwhj.cn

[Q74] 强制使用索引
来源：http://jc.szsharing.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ij.szsharing.cn

[Q75] 日期格式化
来源：http://rf.9csxet.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wa.nszjky.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://og.nicolike.cn

[Q76] 按天统计
来源：http://zk.shxzskj.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://gk.huanxung.cn

[Q77] 时间加减
来源：http://oe.bookmarksfly.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://qd.jctech888.com.cn

[Q78] 当前时间
来源：http://fu.szsharing.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://vo.asd995.cn

[Q79] 字符串拼接
来源：http://rf.haigaiapp.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://oa.wgjwhj.cn

[Q80] 字符串截取
来源：http://xx.lnxyls.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ib.haigaiapp.cn

[Q81] 字符串替换
来源：http://bq.yuntaijiaju.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://jc.huixiangedu.cn

[Q82] 字符长度与字节长度
来源：http://yr.jianghongdianzi.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wc.chemitech.net.cn

[Q83] 大小写转换
来源：http://kb.shxzukj.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://pi.bookmarksfly.cn

[Q84] 去除首尾空格
来源：http://ck.yuntaijiaju.cn

SELECT TRIM(name) FROM users;
来源：http://fb.jctech888.com.cn

[Q85] 数值取整
来源：http://be.nicolike.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://xv.lnxyls.cn

[Q86] 读取 JSON 字段
来源：http://oa.huixinmuqiang.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ky.9csxet.cn

[Q87] JSON 字段做条件
来源：http://wm.bookmarksfly.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://no.chemitech.net.cn

[Q88] 行转列（条件聚合）
来源：http://bv.yuexingan06.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://xe.jianghongdianzi.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://rn.szxytkj.cn

[Q89] 判断表是否存在
来源：http://cu.haigaiapp.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://xa.hahajie.cn

[Q90] 生成序号列
来源：http://gv.bookmarksfly.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://un.huanxung.cn

================================================================================
来源：http://oh.wgjwhj.cn

R. Bash 专题
来源：http://rr.haigaiapp.cn

================================================================================
来源：http://xc.nszjky.cn

[R01] shebang 与严格模式
来源：http://dc.hahajie.cn

#!/usr/bin/env bash
来源：http://mb.yuexingan06.cn

set -euo pipefail
来源：http://km.wgjwhj.cn

[R02] 变量赋值与使用
来源：http://uf.jctech888.com.cn

name="Tom"; echo "$name"
来源：http://bu.nszjky.cn

[R03] 只读变量
来源：http://kh.shxzskj.cn

readonly PI=3.14
来源：http://sn.wgjwhj.cn

[R04] 位置参数
来源：http://vg.shtwfgs.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://dz.colortex.cn

[R05] 参数默认值
来源：http://lq.nszjky.cn

name="${1:-default}"
来源：http://it.chemitech.net.cn

[R06] 判断命令是否存在
来源：http://nu.hnjuh.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wz.colortex.cn

[R07] if 判断文件
来源：http://rk.lnxyls.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://zm.hahajie.cn

[R08] 数值比较
来源：http://pi.szxytkj.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://xl.huixinmuqiang.cn

[R09] 字符串比较
来源：http://qf.panjiajie.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://sn.shtwfgs.cn

[R10] 正则匹配
来源：http://hw.bookmarksfly.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://yz.shtwfgs.cn

[R11] case 多分支
来源：http://vk.521024.cn

case "$1" in
来源：http://dx.nszjky.cn

start) echo "启动" ;;
来源：http://sz.yuntaijiaju.cn

stop)  echo "停止" ;;
来源：http://sq.colortex.cn

*)     echo "未知命令" ;;
来源：http://zq.szxytkj.cn

esac
来源：http://rw.huixiangedu.cn

[R12] for 遍历文件
来源：http://sh.newstarts.cn

for f in *.txt; do echo "$f"; done
来源：http://zs.colortex.cn

[R13] for 计数循环
来源：http://rn.bookmarksfly.cn

for i in {1..10}; do echo "$i"; done
来源：http://ri.jctech888.com.cn

[R14] C 风格 for
来源：http://rt.hnjuh.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://so.nicolike.cn

[R15] while 逐行读文件
来源：http://ze.bookmarksfly.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://td.asd995.cn

[R16] until 等待条件
来源：http://zc.huixinmuqiang.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ls.colortex.cn

[R17] 数组定义与取值
来源：http://re.huixinmuqiang.cn

arr=(a b c); echo "${arr[0]}"
来源：http://kt.521024.cn

[R18] 遍历数组
来源：http://wt.huixinmuqiang.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wc.hnjuh.cn

[R19] 数组长度
来源：http://et.colortex.cn

echo "${#arr[@]}"
来源：http://fk.lnxyls.cn

[R20] 关联数组（字典）
来源：http://ur.lnxyls.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://fb.yuexingan06.cn

[R21] 字符串长度
来源：http://aw.gzmigu.cn

echo "${#s}"
来源：http://lx.colortex.cn

[R22] 截取子串
来源：http://fq.nszjky.cn

echo "${s:0:5}"
来源：http://yt.huanxung.cn

[R23] 字符串替换
来源：http://tp.asd995.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://dv.newstarts.cn

[R24] 大小写转换
来源：http://wu.wgjwhj.cn

echo "${s^^}"; echo "${s,,}"
来源：http://br.huixinmuqiang.cn

[R25] 去后缀 / 去前缀
来源：http://uo.muxihuayi.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://dn.jctech888.com.cn

[R26] 命令替换
来源：http://sf.bjjhwx.cn

now=$(date +%F); echo "$now"
来源：http://xt.huixinmuqiang.cn

[R27] 算术展开
来源：http://as.yuexingan06.cn


<!-- 参考信息 -->