代发 wailian999

[P05] 判断两个对象内容是否相等
来源：http://fh.newstarts.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://ex.colortex.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://nv.jctech888.com.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://tn.wgjwhj.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mo.szsharing.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://zt.bjjhwx.cn

Go:   reflect.DeepEqual(a, b)
来源：http://jx.newstarts.cn

Ruby: a == b
来源：http://kl.asd995.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://lu.9csxet.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mh.muxihuayi.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://yx.lnxyls.cn

PHP:  if (empty($x)) {}
来源：http://ov.lnxyls.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://dp.nicolike.cn

TS:   if (x == null) {}
来源：http://rq.shxzskj.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://au.bookmarksfly.cn

Go:   if x == nil {}
来源：http://sc.szxytkj.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://tn.huanxung.cn

C#:   if (x is null) {}
来源：http://jd.yuntaijiaju.cn

[P07] 防抖与节流
来源：http://qc.nicolike.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://fq.huixinmuqiang.cn

PHP:  // 手写时间戳比较
来源：http://ow.huixiangedu.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ro.colortex.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://vt.gzmigu.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ps.yuntaijiaju.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://pw.hnjuh.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://gz.wgjwhj.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://qz.shxzskj.cn

[P08] 处理浮点精度问题
来源：http://so.bookmarksfly.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://zu.huixinmuqiang.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://lu.bjjhwx.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://sm.shxzukj.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://gr.hnjuh.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://po.chemitech.net.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://bq.colortex.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://vv.jianghongdianzi.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://uo.huanxung.cn

================================================================================
来源：http://tb.9csxet.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://jw.panjiajie.cn

================================================================================
来源：http://ey.huixinmuqiang.cn

[Q01] 创建表
来源：http://pe.muxihuayi.cn

CREATE TABLE users (
来源：http://hi.9csxet.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://zz.colortex.cn

name VARCHAR(50) NOT NULL,
来源：http://vd.shxzukj.cn

email VARCHAR(100) UNIQUE,
来源：http://cz.hahajie.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://tw.gzmigu.cn

);
来源：http://zb.haigaiapp.cn

[Q02] 创建带外键的表
来源：http://km.jctech888.com.cn

CREATE TABLE orders (
来源：http://cq.jctech888.com.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://me.nszjky.cn

user_id INT NOT NULL,
来源：http://qv.hnjuh.cn

amount DECIMAL(10, 2),
来源：http://ks.gzmigu.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://fh.lnxyls.cn

);
来源：http://lp.chemitech.net.cn

[Q03] 增加列
来源：http://fg.shxzukj.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://bo.gzmigu.cn

[Q04] 修改列类型
来源：http://ib.colortex.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://yb.hnjuh.cn

[Q05] 重命名列
来源：http://bi.shxzskj.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://rq.yuntaijiaju.cn

[Q06] 删除列
来源：http://ba.wgjwhj.cn

ALTER TABLE users DROP COLUMN age;
来源：http://sh.shxzukj.cn

[Q07] 删除表
来源：http://sw.colortex.cn

DROP TABLE IF EXISTS orders;
来源：http://ar.nicolike.cn

[Q08] 创建普通索引
来源：http://dw.bjjhwx.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://oz.lnxyls.cn

[Q09] 创建唯一索引
来源：http://vx.chemitech.net.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://zr.huixinmuqiang.cn

[Q10] 插入单行
来源：http://tm.521024.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://je.muxihuayi.cn

[Q11] 一次插入多行
来源：http://zu.jianghongdianzi.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hs.hahajie.cn

[Q12] 插入后取自增 ID
来源：http://uw.huanxung.cn

INSERT INTO users (name) VALUES ('C');
来源：http://aa.gzmigu.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://xg.haigaiapp.cn

[Q13] 忽略重复插入
来源：http://qc.nicolike.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ws.asd995.cn

[Q14] 存在则更新（upsert）
来源：http://cn.wgjwhj.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://zg.huixinmuqiang.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://vo.colortex.cn

[Q15] 查询全部
来源：http://jf.9csxet.cn

SELECT * FROM users;
来源：http://el.panjiajie.cn

[Q16] 查询指定列
来源：http://ch.hnjuh.cn

SELECT id, name FROM users;
来源：http://yi.9csxet.cn

[Q17] 条件查询
来源：http://nk.9csxet.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://gv.huixiangedu.cn

[Q18] 模糊匹配
来源：http://cm.hahajie.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hd.yuntaijiaju.cn

[Q19] 范围查询
来源：http://bz.chemitech.net.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ek.huixiangedu.cn

[Q20] IN 列表
来源：http://zq.huixiangedu.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ce.nszjky.cn

[Q21] 空值判断
来源：http://jb.panjiajie.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://ln.nszjky.cn

[Q22] 排序
来源：http://cn.huixinmuqiang.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://rh.nszjky.cn

[Q23] 分页
来源：http://ax.lnxyls.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://gf.huixinmuqiang.cn

[Q24] 去重
来源：http://tw.jianghongdianzi.cn

SELECT DISTINCT city FROM users;
来源：http://vc.gzmigu.cn

[Q25] 只取前 N 条
来源：http://ns.yuexingan06.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.lnxyls.cn

[Q26] 计数
来源：http://re.panjiajie.cn

SELECT COUNT(*) FROM users;
来源：http://rs.nicolike.cn

[Q27] 条件计数
来源：http://qp.bjjhwx.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://gx.nicolike.cn

[Q28] 求和与平均
来源：http://ne.jctech888.com.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://dm.huixinmuqiang.cn

[Q29] 最大最小值
来源：http://tx.bjjhwx.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://xg.hnjuh.cn

[Q30] 分组统计
来源：http://uj.hnjuh.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://yf.shxzskj.cn

[Q31] 分组后过滤
来源：http://mp.shxzskj.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://zv.shxzukj.cn

[Q32] 分组拼接字符串
来源：http://gm.szsharing.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://fj.nicolike.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mj.hnjuh.cn

[Q33] 多列分组
来源：http://jv.chemitech.net.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://gh.huanxung.cn

[Q34] 每组取第一条
来源：http://mu.gzmigu.cn

SELECT * FROM (
来源：http://gs.9csxet.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://rj.bjjhwx.cn

) t WHERE rn = 1;
来源：http://uo.hnjuh.cn

[Q35] 内连接
来源：http://oc.shtwfgs.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hb.newstarts.cn

[Q36] 左连接
来源：http://dz.shtwfgs.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://vg.huixiangedu.cn

[Q37] 右连接
来源：http://ge.shxzukj.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://nt.hahajie.cn

[Q38] 全外连接（PostgreSQL）
来源：http://bc.szxytkj.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://zx.huixiangedu.cn

[Q39] 自连接（查上下级）
来源：http://dd.nszjky.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://hp.newstarts.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mn.yuexingan06.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://bv.panjiajie.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://vv.bjjhwx.cn

[Q41] 多表连接
来源：http://ac.huixinmuqiang.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://sb.jianghongdianzi.cn

JOIN users u ON u.id = o.user_id
来源：http://wk.newstarts.cn

JOIN products p ON p.id = o.product_id;
来源：http://rf.hahajie.cn

[Q42] 连接条件附加过滤
来源：http://xg.hahajie.cn

SELECT u.name, o.amount FROM users u
来源：http://zu.haigaiapp.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ot.shxzskj.cn

[Q43] 标量子查询
来源：http://sv.bjjhwx.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ky.panjiajie.cn

[Q44] IN 子查询
来源：http://jf.huixinmuqiang.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://lb.lnxyls.cn

[Q45] EXISTS 判断存在
来源：http://mu.newstarts.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://jl.nicolike.cn

[Q46] NOT EXISTS 判断不存在
来源：http://oz.asd995.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://vc.jianghongdianzi.cn

[Q47] 与平均值比较
来源：http://xh.colortex.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://kh.muxihuayi.cn

[Q48] CTE 公用表表达式
来源：http://vo.shtwfgs.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://pc.lnxyls.cn

SELECT * FROM t WHERE c > 5;
来源：http://lz.bjjhwx.cn

[Q49] 更新单行
来源：http://eo.lnxyls.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://eg.shxzukj.cn

[Q50] 批量更新
来源：http://bi.jctech888.com.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://kv.huixinmuqiang.cn

[Q51] 用子查询更新
来源：http://cf.jctech888.com.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://tp.colortex.cn

[Q52] 删除指定行
来源：http://vb.colortex.cn

DELETE FROM users WHERE id = 10;
来源：http://nz.colortex.cn

[Q53] 按条件删除
来源：http://ns.jctech888.com.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://jh.chemitech.net.cn

[Q54] 清空表
来源：http://qq.panjiajie.cn

TRUNCATE TABLE logs;
来源：http://ul.9csxet.cn

[Q55] 排名（并列占位）
来源：http://fy.huixinmuqiang.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://bn.shxzskj.cn

[Q56] 密集排名（并列不占位）
来源：http://rx.panjiajie.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://sb.521024.cn

[Q57] 行号
来源：http://do.szsharing.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ko.nicolike.cn

[Q58] 累计求和
来源：http://lj.nszjky.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://uf.shtwfgs.cn

[Q59] 分组内累计
来源：http://ov.hahajie.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://fa.nicolike.cn

[Q60] 取上一行 / 下一行
来源：http://ah.yuexingan06.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ue.chemitech.net.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://tm.jctech888.com.cn

[Q61] 移动平均
来源：http://td.chemitech.net.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://jm.chemitech.net.cn

[Q62] 分组占比
来源：http://bp.jianghongdianzi.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ex.9csxet.cn

[Q63] 开启事务
来源：http://vr.muxihuayi.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://cy.yuexingan06.cn

[Q64] 提交事务
来源：http://nz.colortex.cn

COMMIT;
来源：http://tf.bookmarksfly.cn

[Q65] 回滚事务
来源：http://uv.yuntaijiaju.cn

ROLLBACK;
来源：http://cf.jctech888.com.cn

[Q66] 行锁查询
来源：http://ye.yuexingan06.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://fd.lnxyls.cn

[Q67] 设置隔离级别
来源：http://op.szsharing.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://zn.yuexingan06.cn

[Q68] 保存点
来源：http://ux.gzmigu.cn

SAVEPOINT sp1;
来源：http://mx.szxytkj.cn

ROLLBACK TO sp1;
来源：http://oj.nicolike.cn

[Q69] 查看执行计划
来源：http://le.jianghongdianzi.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://cv.muxihuayi.cn

[Q70] 更新统计信息
来源：http://xq.wgjwhj.cn

ANALYZE TABLE users;
来源：http://pa.wgjwhj.cn

[Q71] 查看建表语句
来源：http://iu.lnxyls.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://jw.yuntaijiaju.cn

[Q72] 查看索引
来源：http://cy.chemitech.net.cn

SHOW INDEX FROM users;
来源：http://xz.haigaiapp.cn

[Q73] 查看表状态
来源：http://ox.shtwfgs.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://zx.huixiangedu.cn

[Q74] 强制使用索引
来源：http://zb.shxzukj.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://tb.szxytkj.cn

[Q75] 日期格式化
来源：http://mo.szxytkj.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://rz.wgjwhj.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://rq.panjiajie.cn

[Q76] 按天统计
来源：http://nw.asd995.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://du.shtwfgs.cn

[Q77] 时间加减
来源：http://dl.nszjky.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ix.haigaiapp.cn

[Q78] 当前时间
来源：http://mx.asd995.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://bk.bjjhwx.cn

[Q79] 字符串拼接
来源：http://ua.szxytkj.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mn.shtwfgs.cn

[Q80] 字符串截取
来源：http://so.huixinmuqiang.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://pp.szsharing.cn

[Q81] 字符串替换
来源：http://if.jctech888.com.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://sl.huixinmuqiang.cn

[Q82] 字符长度与字节长度
来源：http://eh.newstarts.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://jl.lnxyls.cn

[Q83] 大小写转换
来源：http://bv.shxzukj.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://lj.colortex.cn

[Q84] 去除首尾空格
来源：http://hr.yuexingan06.cn

SELECT TRIM(name) FROM users;
来源：http://uv.colortex.cn

[Q85] 数值取整
来源：http://of.haigaiapp.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://nl.chemitech.net.cn

[Q86] 读取 JSON 字段
来源：http://pl.nicolike.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hv.lnxyls.cn

[Q87] JSON 字段做条件
来源：http://rr.9csxet.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://tx.hnjuh.cn

[Q88] 行转列（条件聚合）
来源：http://kl.shxzukj.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://dm.wgjwhj.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wo.nicolike.cn

[Q89] 判断表是否存在
来源：http://uq.colortex.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hg.muxihuayi.cn

[Q90] 生成序号列
来源：http://qf.newstarts.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://tf.huixiangedu.cn

================================================================================
来源：http://ai.nicolike.cn

R. Bash 专题
来源：http://jx.shxzskj.cn

================================================================================
来源：http://ty.szsharing.cn

[R01] shebang 与严格模式
来源：http://ww.asd995.cn

#!/usr/bin/env bash
来源：http://ks.9csxet.cn

set -euo pipefail
来源：http://ke.jctech888.com.cn

[R02] 变量赋值与使用
来源：http://gy.colortex.cn

name="Tom"; echo "$name"
来源：http://so.nicolike.cn

[R03] 只读变量
来源：http://kd.bjjhwx.cn

readonly PI=3.14
来源：http://qy.colortex.cn

[R04] 位置参数
来源：http://xr.huixinmuqiang.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://up.bookmarksfly.cn

[R05] 参数默认值
来源：http://gh.9csxet.cn

name="${1:-default}"
来源：http://at.szxytkj.cn

[R06] 判断命令是否存在
来源：http://qq.jianghongdianzi.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://nw.jctech888.com.cn

[R07] if 判断文件
来源：http://lg.asd995.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://sy.lnxyls.cn

[R08] 数值比较
来源：http://ib.lnxyls.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://mm.hahajie.cn

[R09] 字符串比较
来源：http://vr.muxihuayi.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://kl.shtwfgs.cn

[R10] 正则匹配
来源：http://qx.521024.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ni.huixinmuqiang.cn

[R11] case 多分支
来源：http://fj.huixiangedu.cn

case "$1" in
来源：http://yd.szxytkj.cn

start) echo "启动" ;;
来源：http://jl.newstarts.cn

stop)  echo "停止" ;;
来源：http://rg.nicolike.cn

*)     echo "未知命令" ;;
来源：http://vt.9csxet.cn

esac
来源：http://wm.nicolike.cn

[R12] for 遍历文件
来源：http://gh.asd995.cn

for f in *.txt; do echo "$f"; done
来源：http://jm.lnxyls.cn

[R13] for 计数循环
来源：http://ls.szsharing.cn

for i in {1..10}; do echo "$i"; done
来源：http://xg.asd995.cn

[R14] C 风格 for
来源：http://zn.colortex.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://su.jianghongdianzi.cn

[R15] while 逐行读文件
来源：http://lu.nszjky.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://vp.9csxet.cn

[R16] until 等待条件
来源：http://mf.nszjky.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ly.shtwfgs.cn

[R17] 数组定义与取值
来源：http://bc.panjiajie.cn

arr=(a b c); echo "${arr[0]}"
来源：http://bv.huanxung.cn

[R18] 遍历数组
来源：http://hg.yuntaijiaju.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ed.bjjhwx.cn

[R19] 数组长度
来源：http://vl.lnxyls.cn

echo "${#arr[@]}"
来源：http://fs.hnjuh.cn

[R20] 关联数组（字典）
来源：http://ng.haigaiapp.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://lj.shxzskj.cn

[R21] 字符串长度
来源：http://hv.gzmigu.cn

echo "${#s}"
来源：http://ns.hnjuh.cn

[R22] 截取子串
来源：http://bz.chemitech.net.cn

echo "${s:0:5}"
来源：http://pb.hnjuh.cn

[R23] 字符串替换
来源：http://fk.szsharing.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://po.nszjky.cn

[R24] 大小写转换
来源：http://pk.jianghongdianzi.cn

echo "${s^^}"; echo "${s,,}"
来源：http://nd.colortex.cn

[R25] 去后缀 / 去前缀
来源：http://ef.huixinmuqiang.cn


<!-- 参考信息 -->