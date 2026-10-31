代发 wailian999

[P05] 判断两个对象内容是否相等
来源：http://zh.huanxung.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://cm.huixinmuqiang.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://oh.asd995.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://sb.shxzukj.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://yq.shxzukj.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://zr.nszjky.cn

Go:   reflect.DeepEqual(a, b)
来源：http://pi.yuntaijiaju.cn

Ruby: a == b
来源：http://fr.yuexingan06.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://lo.shtwfgs.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hy.jianghongdianzi.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ag.haigaiapp.cn

PHP:  if (empty($x)) {}
来源：http://uz.nszjky.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hg.szsharing.cn

TS:   if (x == null) {}
来源：http://ib.shtwfgs.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://ok.shxzukj.cn

Go:   if x == nil {}
来源：http://tg.hnjuh.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://rp.hahajie.cn

C#:   if (x is null) {}
来源：http://if.muxihuayi.cn

[P07] 防抖与节流
来源：http://ry.gzmigu.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://xe.haigaiapp.cn

PHP:  // 手写时间戳比较
来源：http://xa.szsharing.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://st.huanxung.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://lg.panjiajie.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://jp.colortex.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ee.9csxet.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://wi.newstarts.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://tl.nszjky.cn

[P08] 处理浮点精度问题
来源：http://fh.szxytkj.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://fo.yuexingan06.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ak.wgjwhj.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://nu.bjjhwx.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://fs.bjjhwx.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hc.yuexingan06.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://jf.shtwfgs.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ii.lnxyls.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hi.bookmarksfly.cn

================================================================================
来源：http://jz.huixinmuqiang.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://zs.yuexingan06.cn

================================================================================
来源：http://iv.panjiajie.cn

[Q01] 创建表
来源：http://eb.huixinmuqiang.cn

CREATE TABLE users (
来源：http://hd.nicolike.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://no.9csxet.cn

name VARCHAR(50) NOT NULL,
来源：http://zp.panjiajie.cn

email VARCHAR(100) UNIQUE,
来源：http://yq.huanxung.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://zx.asd995.cn

);
来源：http://lb.nicolike.cn

[Q02] 创建带外键的表
来源：http://gv.hahajie.cn

CREATE TABLE orders (
来源：http://ta.521024.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://df.bookmarksfly.cn

user_id INT NOT NULL,
来源：http://vw.9csxet.cn

amount DECIMAL(10, 2),
来源：http://ic.huixiangedu.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://lr.chemitech.net.cn

);
来源：http://kh.nszjky.cn

[Q03] 增加列
来源：http://ig.bjjhwx.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ui.jianghongdianzi.cn

[Q04] 修改列类型
来源：http://fv.wgjwhj.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://bg.szsharing.cn

[Q05] 重命名列
来源：http://es.yuexingan06.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://zz.huixinmuqiang.cn

[Q06] 删除列
来源：http://ud.yuexingan06.cn

ALTER TABLE users DROP COLUMN age;
来源：http://vn.gzmigu.cn

[Q07] 删除表
来源：http://lx.lnxyls.cn

DROP TABLE IF EXISTS orders;
来源：http://fu.bookmarksfly.cn

[Q08] 创建普通索引
来源：http://dr.hahajie.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://mx.jctech888.com.cn

[Q09] 创建唯一索引
来源：http://wf.colortex.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://in.hnjuh.cn

[Q10] 插入单行
来源：http://hm.yuntaijiaju.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://uq.yuntaijiaju.cn

[Q11] 一次插入多行
来源：http://te.shxzskj.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://qg.gzmigu.cn

[Q12] 插入后取自增 ID
来源：http://rk.lnxyls.cn

INSERT INTO users (name) VALUES ('C');
来源：http://tc.wgjwhj.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://bk.haigaiapp.cn

[Q13] 忽略重复插入
来源：http://oi.asd995.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://pa.shxzskj.cn

[Q14] 存在则更新（upsert）
来源：http://qw.shtwfgs.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ew.521024.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://gr.huixinmuqiang.cn

[Q15] 查询全部
来源：http://od.521024.cn

SELECT * FROM users;
来源：http://sb.huixiangedu.cn

[Q16] 查询指定列
来源：http://au.haigaiapp.cn

SELECT id, name FROM users;
来源：http://rz.colortex.cn

[Q17] 条件查询
来源：http://yw.9csxet.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ks.newstarts.cn

[Q18] 模糊匹配
来源：http://fy.szxytkj.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://tg.shxzskj.cn

[Q19] 范围查询
来源：http://kt.szsharing.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wm.gzmigu.cn

[Q20] IN 列表
来源：http://yq.wgjwhj.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://sz.asd995.cn

[Q21] 空值判断
来源：http://rc.szsharing.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://lw.yuexingan06.cn

[Q22] 排序
来源：http://gk.jctech888.com.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://xp.bookmarksfly.cn

[Q23] 分页
来源：http://em.shxzukj.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ve.9csxet.cn

[Q24] 去重
来源：http://zw.asd995.cn

SELECT DISTINCT city FROM users;
来源：http://xz.shxzskj.cn

[Q25] 只取前 N 条
来源：http://nk.shxzskj.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ah.jianghongdianzi.cn

[Q26] 计数
来源：http://hw.shtwfgs.cn

SELECT COUNT(*) FROM users;
来源：http://mv.hnjuh.cn

[Q27] 条件计数
来源：http://gf.jianghongdianzi.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ne.bookmarksfly.cn

[Q28] 求和与平均
来源：http://kt.bookmarksfly.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://bo.nicolike.cn

[Q29] 最大最小值
来源：http://qo.yuexingan06.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://wn.szxytkj.cn

[Q30] 分组统计
来源：http://ie.colortex.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ex.szsharing.cn

[Q31] 分组后过滤
来源：http://fl.huixinmuqiang.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://cr.jianghongdianzi.cn

[Q32] 分组拼接字符串
来源：http://rx.shxzukj.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ov.muxihuayi.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://kl.nszjky.cn

[Q33] 多列分组
来源：http://yv.asd995.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://sb.gzmigu.cn

[Q34] 每组取第一条
来源：http://tb.shxzukj.cn

SELECT * FROM (
来源：http://vc.hahajie.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://zp.jianghongdianzi.cn

) t WHERE rn = 1;
来源：http://xr.asd995.cn

[Q35] 内连接
来源：http://md.huanxung.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://fp.colortex.cn

[Q36] 左连接
来源：http://ef.lnxyls.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://cq.chemitech.net.cn

[Q37] 右连接
来源：http://rh.yuexingan06.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ta.szxytkj.cn

[Q38] 全外连接（PostgreSQL）
来源：http://ol.huixiangedu.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://im.huixiangedu.cn

[Q39] 自连接（查上下级）
来源：http://un.nszjky.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://um.wgjwhj.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://xi.gzmigu.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://rf.521024.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://fj.wgjwhj.cn

[Q41] 多表连接
来源：http://dc.shxzukj.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://mo.hnjuh.cn

JOIN users u ON u.id = o.user_id
来源：http://xc.wgjwhj.cn

JOIN products p ON p.id = o.product_id;
来源：http://mr.chemitech.net.cn

[Q42] 连接条件附加过滤
来源：http://nu.bookmarksfly.cn

SELECT u.name, o.amount FROM users u
来源：http://qp.9csxet.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ak.521024.cn

[Q43] 标量子查询
来源：http://qt.asd995.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://dx.bjjhwx.cn

[Q44] IN 子查询
来源：http://rz.asd995.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wz.huanxung.cn

[Q45] EXISTS 判断存在
来源：http://ru.asd995.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ib.jctech888.com.cn

[Q46] NOT EXISTS 判断不存在
来源：http://xi.bjjhwx.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://yl.muxihuayi.cn

[Q47] 与平均值比较
来源：http://lb.asd995.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://nd.huanxung.cn

[Q48] CTE 公用表表达式
来源：http://zq.chemitech.net.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://dp.newstarts.cn

SELECT * FROM t WHERE c > 5;
来源：http://nd.bjjhwx.cn

[Q49] 更新单行
来源：http://sx.wgjwhj.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://cb.shtwfgs.cn

[Q50] 批量更新
来源：http://hg.nszjky.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wr.bjjhwx.cn

[Q51] 用子查询更新
来源：http://ak.nszjky.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wz.nicolike.cn

[Q52] 删除指定行
来源：http://nv.hahajie.cn

DELETE FROM users WHERE id = 10;
来源：http://xt.yuexingan06.cn

[Q53] 按条件删除
来源：http://wq.lnxyls.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://fl.shtwfgs.cn

[Q54] 清空表
来源：http://sf.jianghongdianzi.cn

TRUNCATE TABLE logs;
来源：http://bg.colortex.cn

[Q55] 排名（并列占位）
来源：http://uw.asd995.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://fq.jianghongdianzi.cn

[Q56] 密集排名（并列不占位）
来源：http://rp.jctech888.com.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://yi.colortex.cn

[Q57] 行号
来源：http://vy.muxihuayi.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ne.huixiangedu.cn

[Q58] 累计求和
来源：http://xm.asd995.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ce.colortex.cn

[Q59] 分组内累计
来源：http://ug.szsharing.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://fy.nszjky.cn

[Q60] 取上一行 / 下一行
来源：http://jr.huanxung.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://gm.muxihuayi.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ek.jianghongdianzi.cn

[Q61] 移动平均
来源：http://ih.jianghongdianzi.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://au.panjiajie.cn

[Q62] 分组占比
来源：http://hz.bjjhwx.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://fd.gzmigu.cn

[Q63] 开启事务
来源：http://ks.shtwfgs.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://bc.521024.cn

[Q64] 提交事务
来源：http://dc.nszjky.cn

COMMIT;
来源：http://cy.shtwfgs.cn

[Q65] 回滚事务
来源：http://nh.szsharing.cn

ROLLBACK;
来源：http://eh.shtwfgs.cn

[Q66] 行锁查询
来源：http://vr.nszjky.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ae.huixiangedu.cn

[Q67] 设置隔离级别
来源：http://xe.nszjky.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://qu.521024.cn

[Q68] 保存点
来源：http://ce.asd995.cn

SAVEPOINT sp1;
来源：http://zo.yuexingan06.cn

ROLLBACK TO sp1;
来源：http://ah.muxihuayi.cn

[Q69] 查看执行计划
来源：http://yo.jctech888.com.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ai.szsharing.cn

[Q70] 更新统计信息
来源：http://rt.jianghongdianzi.cn

ANALYZE TABLE users;
来源：http://qt.nicolike.cn

[Q71] 查看建表语句
来源：http://sl.chemitech.net.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ob.9csxet.cn

[Q72] 查看索引
来源：http://el.yuexingan06.cn

SHOW INDEX FROM users;
来源：http://hr.yuexingan06.cn

[Q73] 查看表状态
来源：http://uf.wgjwhj.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://zq.hnjuh.cn

[Q74] 强制使用索引
来源：http://qo.bjjhwx.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://fd.gzmigu.cn

[Q75] 日期格式化
来源：http://jx.shxzukj.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://xb.chemitech.net.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ux.bjjhwx.cn

[Q76] 按天统计
来源：http://pa.521024.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://zf.shxzukj.cn

[Q77] 时间加减
来源：http://lb.shtwfgs.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://xi.jianghongdianzi.cn

[Q78] 当前时间
来源：http://pn.yuntaijiaju.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://lc.huanxung.cn

[Q79] 字符串拼接
来源：http://ob.szsharing.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://zb.huixinmuqiang.cn

[Q80] 字符串截取
来源：http://hv.colortex.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://li.huanxung.cn

[Q81] 字符串替换
来源：http://tm.yuntaijiaju.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://em.9csxet.cn

[Q82] 字符长度与字节长度
来源：http://wn.colortex.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ad.bookmarksfly.cn

[Q83] 大小写转换
来源：http://wo.yuntaijiaju.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://gp.szxytkj.cn

[Q84] 去除首尾空格
来源：http://mr.jianghongdianzi.cn

SELECT TRIM(name) FROM users;
来源：http://yf.hnjuh.cn

[Q85] 数值取整
来源：http://sw.lnxyls.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://pf.nicolike.cn

[Q86] 读取 JSON 字段
来源：http://mm.yuexingan06.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ng.chemitech.net.cn

[Q87] JSON 字段做条件
来源：http://hp.hahajie.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hx.bjjhwx.cn

[Q88] 行转列（条件聚合）
来源：http://xm.nicolike.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://cz.nicolike.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://dt.szxytkj.cn

[Q89] 判断表是否存在
来源：http://pp.nszjky.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ul.panjiajie.cn

[Q90] 生成序号列
来源：http://ez.gzmigu.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://qk.newstarts.cn

================================================================================
来源：http://ky.shxzukj.cn

R. Bash 专题
来源：http://ko.asd995.cn

================================================================================
来源：http://dz.szsharing.cn

[R01] shebang 与严格模式
来源：http://yo.szxytkj.cn

#!/usr/bin/env bash
来源：http://yt.gzmigu.cn

set -euo pipefail
来源：http://sr.chemitech.net.cn

[R02] 变量赋值与使用
来源：http://xu.nicolike.cn

name="Tom"; echo "$name"
来源：http://ko.panjiajie.cn

[R03] 只读变量
来源：http://ba.hahajie.cn

readonly PI=3.14
来源：http://qg.asd995.cn

[R04] 位置参数
来源：http://oj.bookmarksfly.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://sp.asd995.cn

[R05] 参数默认值
来源：http://xm.shtwfgs.cn

name="${1:-default}"
来源：http://hc.huanxung.cn

[R06] 判断命令是否存在
来源：http://ip.yuexingan06.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://it.hnjuh.cn

[R07] if 判断文件
来源：http://uz.bookmarksfly.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ir.nszjky.cn

[R08] 数值比较
来源：http://tb.yuntaijiaju.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://co.szsharing.cn

[R09] 字符串比较
来源：http://it.bookmarksfly.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://sc.szxytkj.cn

[R10] 正则匹配
来源：http://vk.szsharing.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://jx.szsharing.cn

[R11] case 多分支
来源：http://fz.colortex.cn

case "$1" in
来源：http://ki.shxzukj.cn

start) echo "启动" ;;
来源：http://zr.lnxyls.cn

stop)  echo "停止" ;;
来源：http://es.newstarts.cn

*)     echo "未知命令" ;;
来源：http://as.bjjhwx.cn

esac
来源：http://pj.panjiajie.cn

[R12] for 遍历文件
来源：http://lc.nszjky.cn

for f in *.txt; do echo "$f"; done
来源：http://bq.bookmarksfly.cn

[R13] for 计数循环
来源：http://mp.shxzukj.cn

for i in {1..10}; do echo "$i"; done
来源：http://db.hnjuh.cn

[R14] C 风格 for
来源：http://by.gzmigu.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://go.panjiajie.cn

[R15] while 逐行读文件
来源：http://bd.521024.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://eg.lnxyls.cn

[R16] until 等待条件
来源：http://qo.lnxyls.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://dw.hahajie.cn

[R17] 数组定义与取值
来源：http://po.wgjwhj.cn

arr=(a b c); echo "${arr[0]}"
来源：http://dh.huanxung.cn

[R18] 遍历数组
来源：http://zd.yuntaijiaju.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ai.jctech888.com.cn

[R19] 数组长度
来源：http://et.hnjuh.cn

echo "${#arr[@]}"
来源：http://pz.nszjky.cn

[R20] 关联数组（字典）
来源：http://mm.szxytkj.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://cv.wgjwhj.cn

[R21] 字符串长度
来源：http://bk.yuntaijiaju.cn

echo "${#s}"
来源：http://dl.haigaiapp.cn

[R22] 截取子串
来源：http://qb.asd995.cn

echo "${s:0:5}"
来源：http://wx.huixinmuqiang.cn

[R23] 字符串替换
来源：http://hf.521024.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ww.chemitech.net.cn

[R24] 大小写转换
来源：http://va.hahajie.cn

echo "${s^^}"; echo "${s,,}"
来源：http://xi.colortex.cn

[R25] 去后缀 / 去前缀
来源：http://so.shxzskj.cn


<!-- 参考信息 -->