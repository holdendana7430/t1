代发 wailian999

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://qu.wgjwhj.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://vm.chemitech.net.cn

Go:   reflect.DeepEqual(a, b)
来源：http://ay.shxzskj.cn

Ruby: a == b
来源：http://mu.szsharing.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://bh.jianghongdianzi.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://tv.huanxung.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://fi.hahajie.cn

PHP:  if (empty($x)) {}
来源：http://hk.wgjwhj.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://lk.jctech888.com.cn

TS:   if (x == null) {}
来源：http://ss.bookmarksfly.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://ku.shtwfgs.cn

Go:   if x == nil {}
来源：http://yq.haigaiapp.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://st.lnxyls.cn

C#:   if (x is null) {}
来源：http://lr.colortex.cn

[P07] 防抖与节流
来源：http://tm.szsharing.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://yj.colortex.cn

PHP:  // 手写时间戳比较
来源：http://lm.szsharing.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://yh.jctech888.com.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://at.gzmigu.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://nt.szxytkj.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://cy.muxihuayi.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://wt.gzmigu.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ok.lnxyls.cn

[P08] 处理浮点精度问题
来源：http://bc.panjiajie.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://he.hahajie.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://yk.hahajie.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://lz.szxytkj.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://oh.bjjhwx.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://qj.bookmarksfly.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wr.shxzukj.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ze.jctech888.com.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://yo.hahajie.cn

================================================================================
来源：http://xq.huixinmuqiang.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ah.chemitech.net.cn

================================================================================
来源：http://lh.hahajie.cn

[Q01] 创建表
来源：http://gr.bjjhwx.cn

CREATE TABLE users (
来源：http://mu.asd995.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://iy.lnxyls.cn

name VARCHAR(50) NOT NULL,
来源：http://jl.panjiajie.cn

email VARCHAR(100) UNIQUE,
来源：http://ve.521024.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hm.hnjuh.cn

);
来源：http://dn.bjjhwx.cn

[Q02] 创建带外键的表
来源：http://xb.jianghongdianzi.cn

CREATE TABLE orders (
来源：http://es.shxzukj.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ut.huixiangedu.cn

user_id INT NOT NULL,
来源：http://kj.shxzskj.cn

amount DECIMAL(10, 2),
来源：http://hp.szxytkj.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hu.bjjhwx.cn

);
来源：http://xa.haigaiapp.cn

[Q03] 增加列
来源：http://kw.panjiajie.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://jg.yuexingan06.cn

[Q04] 修改列类型
来源：http://eu.nszjky.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ki.nszjky.cn

[Q05] 重命名列
来源：http://he.gzmigu.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ok.yuntaijiaju.cn

[Q06] 删除列
来源：http://gp.asd995.cn

ALTER TABLE users DROP COLUMN age;
来源：http://iz.lnxyls.cn

[Q07] 删除表
来源：http://tl.jianghongdianzi.cn

DROP TABLE IF EXISTS orders;
来源：http://rz.gzmigu.cn

[Q08] 创建普通索引
来源：http://jv.huanxung.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://io.huanxung.cn

[Q09] 创建唯一索引
来源：http://tv.yuntaijiaju.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ip.hahajie.cn

[Q10] 插入单行
来源：http://hp.newstarts.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://fz.lnxyls.cn

[Q11] 一次插入多行
来源：http://pu.huixinmuqiang.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://cl.asd995.cn

[Q12] 插入后取自增 ID
来源：http://va.bjjhwx.cn

INSERT INTO users (name) VALUES ('C');
来源：http://qg.521024.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://rm.colortex.cn

[Q13] 忽略重复插入
来源：http://fh.panjiajie.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://el.huixiangedu.cn

[Q14] 存在则更新（upsert）
来源：http://uh.shxzskj.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ui.gzmigu.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ps.nicolike.cn

[Q15] 查询全部
来源：http://bs.chemitech.net.cn

SELECT * FROM users;
来源：http://bc.hahajie.cn

[Q16] 查询指定列
来源：http://cr.nszjky.cn

SELECT id, name FROM users;
来源：http://ix.asd995.cn

[Q17] 条件查询
来源：http://vz.szxytkj.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://zk.huixiangedu.cn

[Q18] 模糊匹配
来源：http://yn.nszjky.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://bo.muxihuayi.cn

[Q19] 范围查询
来源：http://yc.huixiangedu.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://dy.wgjwhj.cn

[Q20] IN 列表
来源：http://ru.szsharing.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://db.szsharing.cn

[Q21] 空值判断
来源：http://me.shtwfgs.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://ji.jctech888.com.cn

[Q22] 排序
来源：http://fi.colortex.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://tr.nicolike.cn

[Q23] 分页
来源：http://hi.chemitech.net.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://cl.huanxung.cn

[Q24] 去重
来源：http://tm.haigaiapp.cn

SELECT DISTINCT city FROM users;
来源：http://qs.521024.cn

[Q25] 只取前 N 条
来源：http://ac.wgjwhj.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://cu.muxihuayi.cn

[Q26] 计数
来源：http://yg.panjiajie.cn

SELECT COUNT(*) FROM users;
来源：http://oh.521024.cn

[Q27] 条件计数
来源：http://nq.jianghongdianzi.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://zu.hnjuh.cn

[Q28] 求和与平均
来源：http://um.panjiajie.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hb.9csxet.cn

[Q29] 最大最小值
来源：http://jg.jianghongdianzi.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://tv.bookmarksfly.cn

[Q30] 分组统计
来源：http://dw.muxihuayi.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://fi.jctech888.com.cn

[Q31] 分组后过滤
来源：http://tl.muxihuayi.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://tu.newstarts.cn

[Q32] 分组拼接字符串
来源：http://au.newstarts.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ny.nicolike.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://rx.bjjhwx.cn

[Q33] 多列分组
来源：http://bv.panjiajie.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ni.hnjuh.cn

[Q34] 每组取第一条
来源：http://cu.huixinmuqiang.cn

SELECT * FROM (
来源：http://py.bookmarksfly.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://xc.haigaiapp.cn

) t WHERE rn = 1;
来源：http://mm.9csxet.cn

[Q35] 内连接
来源：http://cq.hahajie.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ao.szsharing.cn

[Q36] 左连接
来源：http://fg.shxzskj.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://iy.huanxung.cn

[Q37] 右连接
来源：http://le.colortex.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://vm.jianghongdianzi.cn

[Q38] 全外连接（PostgreSQL）
来源：http://yz.szxytkj.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://qz.haigaiapp.cn

[Q39] 自连接（查上下级）
来源：http://ta.bjjhwx.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://fa.521024.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.muxihuayi.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://rp.asd995.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://du.bookmarksfly.cn

[Q41] 多表连接
来源：http://ru.haigaiapp.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://hc.521024.cn

JOIN users u ON u.id = o.user_id
来源：http://pg.shxzskj.cn

JOIN products p ON p.id = o.product_id;
来源：http://ln.yuntaijiaju.cn

[Q42] 连接条件附加过滤
来源：http://az.muxihuayi.cn

SELECT u.name, o.amount FROM users u
来源：http://ow.newstarts.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wo.huanxung.cn

[Q43] 标量子查询
来源：http://de.shxzukj.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://cp.haigaiapp.cn

[Q44] IN 子查询
来源：http://tg.shtwfgs.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ag.shtwfgs.cn

[Q45] EXISTS 判断存在
来源：http://oc.muxihuayi.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://no.yuntaijiaju.cn

[Q46] NOT EXISTS 判断不存在
来源：http://vu.asd995.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://nw.hahajie.cn

[Q47] 与平均值比较
来源：http://eh.hnjuh.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://rv.gzmigu.cn

[Q48] CTE 公用表表达式
来源：http://kp.9csxet.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://sr.yuntaijiaju.cn

SELECT * FROM t WHERE c > 5;
来源：http://bx.hahajie.cn

[Q49] 更新单行
来源：http://nq.hahajie.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ce.gzmigu.cn

[Q50] 批量更新
来源：http://ai.yuexingan06.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://jl.huixinmuqiang.cn

[Q51] 用子查询更新
来源：http://hp.shxzukj.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://cd.wgjwhj.cn

[Q52] 删除指定行
来源：http://gw.bjjhwx.cn

DELETE FROM users WHERE id = 10;
来源：http://yd.asd995.cn

[Q53] 按条件删除
来源：http://iq.9csxet.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ba.bookmarksfly.cn

[Q54] 清空表
来源：http://eb.panjiajie.cn

TRUNCATE TABLE logs;
来源：http://sb.9csxet.cn

[Q55] 排名（并列占位）
来源：http://oj.huixinmuqiang.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ai.nicolike.cn

[Q56] 密集排名（并列不占位）
来源：http://qt.hahajie.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://qq.wgjwhj.cn

[Q57] 行号
来源：http://ca.hnjuh.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://qc.huixiangedu.cn

[Q58] 累计求和
来源：http://cy.shtwfgs.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://gq.9csxet.cn

[Q59] 分组内累计
来源：http://xb.wgjwhj.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://gy.yuexingan06.cn

[Q60] 取上一行 / 下一行
来源：http://zv.szsharing.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://qv.521024.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://co.szxytkj.cn

[Q61] 移动平均
来源：http://pg.szsharing.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wt.shtwfgs.cn

[Q62] 分组占比
来源：http://sl.yuntaijiaju.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://yd.jctech888.com.cn

[Q63] 开启事务
来源：http://va.gzmigu.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://vk.szsharing.cn

[Q64] 提交事务
来源：http://au.newstarts.cn

COMMIT;
来源：http://ko.shxzukj.cn

[Q65] 回滚事务
来源：http://pa.wgjwhj.cn

ROLLBACK;
来源：http://ts.521024.cn

[Q66] 行锁查询
来源：http://jq.huixinmuqiang.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://cz.hnjuh.cn

[Q67] 设置隔离级别
来源：http://qu.jctech888.com.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ug.huixiangedu.cn

[Q68] 保存点
来源：http://ri.muxihuayi.cn

SAVEPOINT sp1;
来源：http://gi.colortex.cn

ROLLBACK TO sp1;
来源：http://nx.haigaiapp.cn

[Q69] 查看执行计划
来源：http://pq.newstarts.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://gq.521024.cn

[Q70] 更新统计信息
来源：http://jv.asd995.cn

ANALYZE TABLE users;
来源：http://uu.szsharing.cn

[Q71] 查看建表语句
来源：http://se.huixinmuqiang.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ds.yuntaijiaju.cn

[Q72] 查看索引
来源：http://ne.9csxet.cn

SHOW INDEX FROM users;
来源：http://mb.bjjhwx.cn

[Q73] 查看表状态
来源：http://ic.asd995.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://pt.colortex.cn

[Q74] 强制使用索引
来源：http://ze.huixinmuqiang.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ud.hnjuh.cn

[Q75] 日期格式化
来源：http://ux.yuexingan06.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ok.shxzskj.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://va.bookmarksfly.cn

[Q76] 按天统计
来源：http://ku.newstarts.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ji.szsharing.cn

[Q77] 时间加减
来源：http://xk.yuexingan06.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://qq.jctech888.com.cn

[Q78] 当前时间
来源：http://da.shxzskj.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://aj.huixinmuqiang.cn

[Q79] 字符串拼接
来源：http://ws.nicolike.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://cq.nszjky.cn

[Q80] 字符串截取
来源：http://rx.huixiangedu.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hh.huixinmuqiang.cn

[Q81] 字符串替换
来源：http://nf.chemitech.net.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://zz.szxytkj.cn

[Q82] 字符长度与字节长度
来源：http://kw.nicolike.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://oy.muxihuayi.cn

[Q83] 大小写转换
来源：http://qp.newstarts.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://up.hnjuh.cn

[Q84] 去除首尾空格
来源：http://hb.szxytkj.cn

SELECT TRIM(name) FROM users;
来源：http://gw.shxzukj.cn

[Q85] 数值取整
来源：http://yc.jctech888.com.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://da.9csxet.cn

[Q86] 读取 JSON 字段
来源：http://df.szsharing.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ld.chemitech.net.cn

[Q87] JSON 字段做条件
来源：http://fw.hnjuh.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://vj.panjiajie.cn

[Q88] 行转列（条件聚合）
来源：http://rz.yuntaijiaju.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ko.9csxet.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://kq.521024.cn

[Q89] 判断表是否存在
来源：http://vv.huixinmuqiang.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ys.nicolike.cn

[Q90] 生成序号列
来源：http://qs.colortex.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://lg.gzmigu.cn

================================================================================
来源：http://ic.huanxung.cn

R. Bash 专题
来源：http://wn.newstarts.cn

================================================================================
来源：http://sw.newstarts.cn

[R01] shebang 与严格模式
来源：http://ow.chemitech.net.cn

#!/usr/bin/env bash
来源：http://qc.chemitech.net.cn

set -euo pipefail
来源：http://bz.gzmigu.cn

[R02] 变量赋值与使用
来源：http://nt.chemitech.net.cn

name="Tom"; echo "$name"
来源：http://li.yuexingan06.cn

[R03] 只读变量
来源：http://pb.yuntaijiaju.cn

readonly PI=3.14
来源：http://wu.huanxung.cn

[R04] 位置参数
来源：http://db.nszjky.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ym.haigaiapp.cn

[R05] 参数默认值
来源：http://ws.shxzskj.cn

name="${1:-default}"
来源：http://ob.521024.cn

[R06] 判断命令是否存在
来源：http://eg.muxihuayi.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://gz.lnxyls.cn

[R07] if 判断文件
来源：http://yu.chemitech.net.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://pl.bjjhwx.cn

[R08] 数值比较
来源：http://zm.shxzskj.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://kv.bjjhwx.cn

[R09] 字符串比较
来源：http://cy.huixinmuqiang.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://yg.9csxet.cn

[R10] 正则匹配
来源：http://vn.huixiangedu.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://sq.hahajie.cn

[R11] case 多分支
来源：http://bo.hahajie.cn

case "$1" in
来源：http://fn.shtwfgs.cn

start) echo "启动" ;;
来源：http://vi.muxihuayi.cn

stop)  echo "停止" ;;
来源：http://yk.colortex.cn

*)     echo "未知命令" ;;
来源：http://nj.lnxyls.cn

esac
来源：http://zb.hnjuh.cn

[R12] for 遍历文件
来源：http://ic.huixiangedu.cn

for f in *.txt; do echo "$f"; done
来源：http://fl.huixiangedu.cn

[R13] for 计数循环
来源：http://ve.bjjhwx.cn

for i in {1..10}; do echo "$i"; done
来源：http://sc.bookmarksfly.cn

[R14] C 风格 for
来源：http://rm.wgjwhj.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://vu.jctech888.com.cn

[R15] while 逐行读文件
来源：http://rw.bookmarksfly.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://sx.gzmigu.cn

[R16] until 等待条件
来源：http://tl.shxzukj.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ko.hahajie.cn

[R17] 数组定义与取值
来源：http://wd.muxihuayi.cn

arr=(a b c); echo "${arr[0]}"
来源：http://fx.yuexingan06.cn

[R18] 遍历数组
来源：http://sc.bjjhwx.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://pt.panjiajie.cn

[R19] 数组长度
来源：http://yj.muxihuayi.cn

echo "${#arr[@]}"
来源：http://rx.huixinmuqiang.cn

[R20] 关联数组（字典）
来源：http://os.shtwfgs.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://dj.huixinmuqiang.cn

[R21] 字符串长度
来源：http://ux.asd995.cn

echo "${#s}"
来源：http://ny.wgjwhj.cn

[R22] 截取子串
来源：http://wf.huixinmuqiang.cn

echo "${s:0:5}"
来源：http://zr.shxzskj.cn

[R23] 字符串替换
来源：http://bs.nszjky.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://yj.colortex.cn

[R24] 大小写转换
来源：http://jp.muxihuayi.cn

echo "${s^^}"; echo "${s,,}"
来源：http://su.nszjky.cn

[R25] 去后缀 / 去前缀
来源：http://yd.521024.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://kx.szsharing.cn

[R26] 命令替换
来源：http://ct.muxihuayi.cn

now=$(date +%F); echo "$now"
来源：http://bb.chemitech.net.cn

[R27] 算术展开
来源：http://vy.9csxet.cn


<!-- 参考信息 -->