代发 wailian999

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://lp.lnxyls.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://qn.asd995.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hq.wgjwhj.cn

PHP:  if (empty($x)) {}
来源：http://hb.huixiangedu.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://bj.9csxet.cn

TS:   if (x == null) {}
来源：http://dx.yuntaijiaju.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://ih.newstarts.cn

Go:   if x == nil {}
来源：http://mu.shtwfgs.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://zq.szsharing.cn

C#:   if (x is null) {}
来源：http://yb.chemitech.net.cn

[P07] 防抖与节流
来源：http://la.lnxyls.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://qc.huanxung.cn

PHP:  // 手写时间戳比较
来源：http://fk.huixinmuqiang.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mz.shxzskj.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://fr.wgjwhj.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ps.9csxet.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://lw.lnxyls.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://ue.asd995.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hk.hnjuh.cn

[P08] 处理浮点精度问题
来源：http://bp.bookmarksfly.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://rc.9csxet.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://gw.shxzukj.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hy.nicolike.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ze.hnjuh.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mx.lnxyls.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ir.panjiajie.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ng.szsharing.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://sr.nicolike.cn

================================================================================
来源：http://pf.haigaiapp.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://gs.hnjuh.cn

================================================================================
来源：http://kn.asd995.cn

[Q01] 创建表
来源：http://us.bjjhwx.cn

CREATE TABLE users (
来源：http://em.jctech888.com.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://yy.shtwfgs.cn

name VARCHAR(50) NOT NULL,
来源：http://pg.shxzskj.cn

email VARCHAR(100) UNIQUE,
来源：http://ha.nicolike.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://dc.nicolike.cn

);
来源：http://nb.muxihuayi.cn

[Q02] 创建带外键的表
来源：http://us.shxzukj.cn

CREATE TABLE orders (
来源：http://eq.gzmigu.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ym.shxzskj.cn

user_id INT NOT NULL,
来源：http://jh.huixiangedu.cn

amount DECIMAL(10, 2),
来源：http://yt.shtwfgs.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://kz.chemitech.net.cn

);
来源：http://pl.szxytkj.cn

[Q03] 增加列
来源：http://yj.muxihuayi.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://bi.wgjwhj.cn

[Q04] 修改列类型
来源：http://te.wgjwhj.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ti.shxzukj.cn

[Q05] 重命名列
来源：http://no.bjjhwx.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ot.9csxet.cn

[Q06] 删除列
来源：http://fr.huixiangedu.cn

ALTER TABLE users DROP COLUMN age;
来源：http://hp.huanxung.cn

[Q07] 删除表
来源：http://sx.huixiangedu.cn

DROP TABLE IF EXISTS orders;
来源：http://hq.huixiangedu.cn

[Q08] 创建普通索引
来源：http://ax.shxzukj.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://le.newstarts.cn

[Q09] 创建唯一索引
来源：http://bx.szsharing.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://sv.521024.cn

[Q10] 插入单行
来源：http://br.lnxyls.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://fy.jctech888.com.cn

[Q11] 一次插入多行
来源：http://vt.jianghongdianzi.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://gl.huixinmuqiang.cn

[Q12] 插入后取自增 ID
来源：http://mt.huixiangedu.cn

INSERT INTO users (name) VALUES ('C');
来源：http://mw.bjjhwx.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ep.jctech888.com.cn

[Q13] 忽略重复插入
来源：http://gn.nicolike.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ln.nicolike.cn

[Q14] 存在则更新（upsert）
来源：http://zs.wgjwhj.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ea.szsharing.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://gx.muxihuayi.cn

[Q15] 查询全部
来源：http://sv.shxzskj.cn

SELECT * FROM users;
来源：http://pz.asd995.cn

[Q16] 查询指定列
来源：http://lh.nszjky.cn

SELECT id, name FROM users;
来源：http://wz.bookmarksfly.cn

[Q17] 条件查询
来源：http://re.chemitech.net.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ka.nicolike.cn

[Q18] 模糊匹配
来源：http://ce.huixiangedu.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://za.bookmarksfly.cn

[Q19] 范围查询
来源：http://qj.gzmigu.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://qt.yuntaijiaju.cn

[Q20] IN 列表
来源：http://yi.shxzskj.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://fc.asd995.cn

[Q21] 空值判断
来源：http://so.huixiangedu.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://td.9csxet.cn

[Q22] 排序
来源：http://ff.jctech888.com.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://em.haigaiapp.cn

[Q23] 分页
来源：http://wc.colortex.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ty.chemitech.net.cn

[Q24] 去重
来源：http://yr.huixinmuqiang.cn

SELECT DISTINCT city FROM users;
来源：http://bv.nszjky.cn

[Q25] 只取前 N 条
来源：http://lv.lnxyls.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://bk.hnjuh.cn

[Q26] 计数
来源：http://mg.521024.cn

SELECT COUNT(*) FROM users;
来源：http://iz.wgjwhj.cn

[Q27] 条件计数
来源：http://lw.9csxet.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://vg.shxzukj.cn

[Q28] 求和与平均
来源：http://ku.szxytkj.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://dv.nszjky.cn

[Q29] 最大最小值
来源：http://mb.lnxyls.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://fd.haigaiapp.cn

[Q30] 分组统计
来源：http://ua.nszjky.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://pj.chemitech.net.cn

[Q31] 分组后过滤
来源：http://op.colortex.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://qk.wgjwhj.cn

[Q32] 分组拼接字符串
来源：http://zx.shtwfgs.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://vh.muxihuayi.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://nf.bjjhwx.cn

[Q33] 多列分组
来源：http://ms.lnxyls.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ko.colortex.cn

[Q34] 每组取第一条
来源：http://xw.jianghongdianzi.cn

SELECT * FROM (
来源：http://fi.nszjky.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://eu.newstarts.cn

) t WHERE rn = 1;
来源：http://uy.huixiangedu.cn

[Q35] 内连接
来源：http://cm.panjiajie.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://bi.haigaiapp.cn

[Q36] 左连接
来源：http://fh.colortex.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://rl.newstarts.cn

[Q37] 右连接
来源：http://lx.bookmarksfly.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://nf.lnxyls.cn

[Q38] 全外连接（PostgreSQL）
来源：http://gz.newstarts.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://dp.szsharing.cn

[Q39] 自连接（查上下级）
来源：http://yd.hnjuh.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://fz.521024.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://iq.huanxung.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://kt.newstarts.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://iy.shxzukj.cn

[Q41] 多表连接
来源：http://kf.jianghongdianzi.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://sf.hahajie.cn

JOIN users u ON u.id = o.user_id
来源：http://wx.haigaiapp.cn

JOIN products p ON p.id = o.product_id;
来源：http://ov.nszjky.cn

[Q42] 连接条件附加过滤
来源：http://bj.huixiangedu.cn

SELECT u.name, o.amount FROM users u
来源：http://uf.shtwfgs.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://il.wgjwhj.cn

[Q43] 标量子查询
来源：http://xr.gzmigu.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://we.lnxyls.cn

[Q44] IN 子查询
来源：http://gv.nicolike.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ix.yuntaijiaju.cn

[Q45] EXISTS 判断存在
来源：http://ay.shxzskj.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://zv.muxihuayi.cn

[Q46] NOT EXISTS 判断不存在
来源：http://wj.szxytkj.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://lo.shxzskj.cn

[Q47] 与平均值比较
来源：http://vo.huanxung.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ve.yuexingan06.cn

[Q48] CTE 公用表表达式
来源：http://wy.huixiangedu.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://bd.shtwfgs.cn

SELECT * FROM t WHERE c > 5;
来源：http://mj.huixinmuqiang.cn

[Q49] 更新单行
来源：http://xu.9csxet.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://jp.yuntaijiaju.cn

[Q50] 批量更新
来源：http://rt.hahajie.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://ud.yuntaijiaju.cn

[Q51] 用子查询更新
来源：http://db.szxytkj.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://lo.shxzukj.cn

[Q52] 删除指定行
来源：http://vj.huanxung.cn

DELETE FROM users WHERE id = 10;
来源：http://yp.panjiajie.cn

[Q53] 按条件删除
来源：http://ia.colortex.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://nt.huanxung.cn

[Q54] 清空表
来源：http://jp.muxihuayi.cn

TRUNCATE TABLE logs;
来源：http://mz.newstarts.cn

[Q55] 排名（并列占位）
来源：http://gk.bjjhwx.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://uu.jianghongdianzi.cn

[Q56] 密集排名（并列不占位）
来源：http://cf.jianghongdianzi.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hy.shxzukj.cn

[Q57] 行号
来源：http://zp.huixiangedu.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://qk.hahajie.cn

[Q58] 累计求和
来源：http://dz.huanxung.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://lp.huixiangedu.cn

[Q59] 分组内累计
来源：http://py.huixiangedu.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://rw.gzmigu.cn

[Q60] 取上一行 / 下一行
来源：http://si.hnjuh.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ah.asd995.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hy.9csxet.cn

[Q61] 移动平均
来源：http://vj.9csxet.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://nr.521024.cn

[Q62] 分组占比
来源：http://mk.gzmigu.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://oz.nicolike.cn

[Q63] 开启事务
来源：http://wt.shxzukj.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://kp.jianghongdianzi.cn

[Q64] 提交事务
来源：http://xf.colortex.cn

COMMIT;
来源：http://aa.panjiajie.cn

[Q65] 回滚事务
来源：http://ol.huixiangedu.cn

ROLLBACK;
来源：http://dw.szsharing.cn

[Q66] 行锁查询
来源：http://aa.shxzukj.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ki.muxihuayi.cn

[Q67] 设置隔离级别
来源：http://cz.gzmigu.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://jt.yuntaijiaju.cn

[Q68] 保存点
来源：http://fn.chemitech.net.cn

SAVEPOINT sp1;
来源：http://wl.panjiajie.cn

ROLLBACK TO sp1;
来源：http://vj.lnxyls.cn

[Q69] 查看执行计划
来源：http://fx.chemitech.net.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://te.shxzskj.cn

[Q70] 更新统计信息
来源：http://og.shxzukj.cn

ANALYZE TABLE users;
来源：http://yo.huanxung.cn

[Q71] 查看建表语句
来源：http://ky.bookmarksfly.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mw.huixinmuqiang.cn

[Q72] 查看索引
来源：http://py.jianghongdianzi.cn

SHOW INDEX FROM users;
来源：http://yx.wgjwhj.cn

[Q73] 查看表状态
来源：http://ua.jianghongdianzi.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://wf.wgjwhj.cn

[Q74] 强制使用索引
来源：http://az.shtwfgs.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://dv.wgjwhj.cn

[Q75] 日期格式化
来源：http://ma.huixinmuqiang.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://od.huixiangedu.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://gq.nszjky.cn

[Q76] 按天统计
来源：http://wb.yuexingan06.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://tt.huixinmuqiang.cn

[Q77] 时间加减
来源：http://dr.newstarts.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://lc.szsharing.cn

[Q78] 当前时间
来源：http://cr.gzmigu.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://sw.9csxet.cn

[Q79] 字符串拼接
来源：http://oq.hahajie.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mk.szxytkj.cn

[Q80] 字符串截取
来源：http://kx.asd995.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://iu.chemitech.net.cn

[Q81] 字符串替换
来源：http://kr.shtwfgs.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://io.9csxet.cn

[Q82] 字符长度与字节长度
来源：http://ma.asd995.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://qz.9csxet.cn

[Q83] 大小写转换
来源：http://sc.newstarts.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ro.nicolike.cn

[Q84] 去除首尾空格
来源：http://fj.huixinmuqiang.cn

SELECT TRIM(name) FROM users;
来源：http://lf.hnjuh.cn

[Q85] 数值取整
来源：http://yb.yuntaijiaju.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://nr.hahajie.cn

[Q86] 读取 JSON 字段
来源：http://zt.hahajie.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://sl.shtwfgs.cn

[Q87] JSON 字段做条件
来源：http://xn.hnjuh.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://cp.colortex.cn

[Q88] 行转列（条件聚合）
来源：http://oj.9csxet.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://qb.jctech888.com.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://nh.newstarts.cn

[Q89] 判断表是否存在
来源：http://gu.9csxet.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://zh.szxytkj.cn

[Q90] 生成序号列
来源：http://gi.jctech888.com.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://db.yuntaijiaju.cn

================================================================================
来源：http://vo.hahajie.cn

R. Bash 专题
来源：http://jq.lnxyls.cn

================================================================================
来源：http://sc.newstarts.cn

[R01] shebang 与严格模式
来源：http://wv.bjjhwx.cn

#!/usr/bin/env bash
来源：http://bn.szxytkj.cn

set -euo pipefail
来源：http://id.jctech888.com.cn

[R02] 变量赋值与使用
来源：http://cf.hnjuh.cn

name="Tom"; echo "$name"
来源：http://jk.yuexingan06.cn

[R03] 只读变量
来源：http://wq.colortex.cn

readonly PI=3.14
来源：http://pd.muxihuayi.cn

[R04] 位置参数
来源：http://na.hahajie.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://jn.yuexingan06.cn

[R05] 参数默认值
来源：http://la.shxzskj.cn

name="${1:-default}"
来源：http://gk.jctech888.com.cn

[R06] 判断命令是否存在
来源：http://um.szsharing.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://sb.yuexingan06.cn

[R07] if 判断文件
来源：http://xs.jianghongdianzi.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mw.wgjwhj.cn

[R08] 数值比较
来源：http://eg.bjjhwx.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://hh.asd995.cn

[R09] 字符串比较
来源：http://wb.bjjhwx.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://oa.huixiangedu.cn

[R10] 正则匹配
来源：http://zb.521024.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://yp.haigaiapp.cn

[R11] case 多分支
来源：http://iw.chemitech.net.cn

case "$1" in
来源：http://um.yuntaijiaju.cn

start) echo "启动" ;;
来源：http://kl.nicolike.cn

stop)  echo "停止" ;;
来源：http://qz.lnxyls.cn

*)     echo "未知命令" ;;
来源：http://de.hnjuh.cn

esac
来源：http://wv.yuntaijiaju.cn

[R12] for 遍历文件
来源：http://gj.yuntaijiaju.cn

for f in *.txt; do echo "$f"; done
来源：http://cy.muxihuayi.cn

[R13] for 计数循环
来源：http://sy.shxzskj.cn

for i in {1..10}; do echo "$i"; done
来源：http://fc.asd995.cn

[R14] C 风格 for
来源：http://xh.asd995.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://lv.szsharing.cn

[R15] while 逐行读文件
来源：http://ze.hahajie.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://dy.nszjky.cn

[R16] until 等待条件
来源：http://ro.521024.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ut.newstarts.cn

[R17] 数组定义与取值
来源：http://jh.nszjky.cn

arr=(a b c); echo "${arr[0]}"
来源：http://qk.9csxet.cn

[R18] 遍历数组
来源：http://ty.nicolike.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://js.9csxet.cn

[R19] 数组长度
来源：http://pc.panjiajie.cn

echo "${#arr[@]}"
来源：http://nt.huanxung.cn

[R20] 关联数组（字典）
来源：http://si.nszjky.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ym.chemitech.net.cn

[R21] 字符串长度
来源：http://lj.szxytkj.cn

echo "${#s}"
来源：http://hn.asd995.cn

[R22] 截取子串
来源：http://bn.muxihuayi.cn

echo "${s:0:5}"
来源：http://xw.yuexingan06.cn

[R23] 字符串替换
来源：http://vo.shxzukj.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://sn.haigaiapp.cn

[R24] 大小写转换
来源：http://ta.haigaiapp.cn

echo "${s^^}"; echo "${s,,}"
来源：http://dh.gzmigu.cn

[R25] 去后缀 / 去前缀
来源：http://uc.bjjhwx.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://ia.jianghongdianzi.cn

[R26] 命令替换
来源：http://pe.hahajie.cn

now=$(date +%F); echo "$now"
来源：http://yy.shxzskj.cn

[R27] 算术展开
来源：http://rs.huixiangedu.cn

echo $((1 + 2 * 3))
来源：http://ys.jianghongdianzi.cn

[R28] 浮点运算
来源：http://bj.yuexingan06.cn

echo "scale=2; 10/3" | bc
来源：http://ux.9csxet.cn

[R29] 定义函数
来源：http://ga.jctech888.com.cn


<!-- 参考信息 -->