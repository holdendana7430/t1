代发 wailian999

Java: list.size();  map.size();  s.length()
来源：http://ut.szsharing.cn

Go:   len(arr);  len(m)
来源：http://vg.shxzukj.cn

Ruby: x.length;  x.size
来源：http://mg.chemitech.net.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://qx.nicolike.cn

[P05] 判断两个对象内容是否相等
来源：http://nu.colortex.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://zs.yuexingan06.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://qj.chemitech.net.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ho.szsharing.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://sk.jctech888.com.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ue.jianghongdianzi.cn

Go:   reflect.DeepEqual(a, b)
来源：http://qx.9csxet.cn

Ruby: a == b
来源：http://is.shxzskj.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ts.bjjhwx.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://zn.yuexingan06.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://pw.jctech888.com.cn

PHP:  if (empty($x)) {}
来源：http://wh.szxytkj.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ri.521024.cn

TS:   if (x == null) {}
来源：http://re.jctech888.com.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://lt.hnjuh.cn

Go:   if x == nil {}
来源：http://fx.huanxung.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://xv.shxzskj.cn

C#:   if (x is null) {}
来源：http://uc.huanxung.cn

[P07] 防抖与节流
来源：http://wq.nicolike.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://jd.hnjuh.cn

PHP:  // 手写时间戳比较
来源：http://rc.colortex.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ri.shxzukj.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ot.bjjhwx.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://rw.huixiangedu.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://km.shtwfgs.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://km.bjjhwx.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://uf.521024.cn

[P08] 处理浮点精度问题
来源：http://by.szsharing.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ta.521024.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hh.bookmarksfly.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://pz.hahajie.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ka.hnjuh.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wi.nszjky.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://yp.lnxyls.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://le.jianghongdianzi.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://lb.newstarts.cn

================================================================================
来源：http://cj.asd995.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://lt.hahajie.cn

================================================================================
来源：http://ra.muxihuayi.cn

[Q01] 创建表
来源：http://ru.wgjwhj.cn

CREATE TABLE users (
来源：http://xh.colortex.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://he.muxihuayi.cn

name VARCHAR(50) NOT NULL,
来源：http://of.shtwfgs.cn

email VARCHAR(100) UNIQUE,
来源：http://my.shtwfgs.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://sf.newstarts.cn

);
来源：http://nq.muxihuayi.cn

[Q02] 创建带外键的表
来源：http://ft.szxytkj.cn

CREATE TABLE orders (
来源：http://fl.jctech888.com.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://no.muxihuayi.cn

user_id INT NOT NULL,
来源：http://qu.9csxet.cn

amount DECIMAL(10, 2),
来源：http://wb.muxihuayi.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ig.huixinmuqiang.cn

);
来源：http://dj.wgjwhj.cn

[Q03] 增加列
来源：http://qd.hnjuh.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hk.jctech888.com.cn

[Q04] 修改列类型
来源：http://yy.szxytkj.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://lq.huanxung.cn

[Q05] 重命名列
来源：http://is.shxzukj.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://nq.newstarts.cn

[Q06] 删除列
来源：http://ty.haigaiapp.cn

ALTER TABLE users DROP COLUMN age;
来源：http://ar.colortex.cn

[Q07] 删除表
来源：http://bh.jctech888.com.cn

DROP TABLE IF EXISTS orders;
来源：http://kw.panjiajie.cn

[Q08] 创建普通索引
来源：http://ys.huixiangedu.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://dj.szxytkj.cn

[Q09] 创建唯一索引
来源：http://cq.szxytkj.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://pz.huanxung.cn

[Q10] 插入单行
来源：http://qw.chemitech.net.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://iv.bjjhwx.cn

[Q11] 一次插入多行
来源：http://ux.haigaiapp.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://yx.shxzskj.cn

[Q12] 插入后取自增 ID
来源：http://qd.wgjwhj.cn

INSERT INTO users (name) VALUES ('C');
来源：http://rb.asd995.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://pd.jianghongdianzi.cn

[Q13] 忽略重复插入
来源：http://my.huanxung.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://gt.521024.cn

[Q14] 存在则更新（upsert）
来源：http://ba.yuexingan06.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://zu.hahajie.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://sg.colortex.cn

[Q15] 查询全部
来源：http://pc.yuexingan06.cn

SELECT * FROM users;
来源：http://kq.huanxung.cn

[Q16] 查询指定列
来源：http://uf.panjiajie.cn

SELECT id, name FROM users;
来源：http://eo.nicolike.cn

[Q17] 条件查询
来源：http://bv.nszjky.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://rx.haigaiapp.cn

[Q18] 模糊匹配
来源：http://ke.521024.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://yf.szsharing.cn

[Q19] 范围查询
来源：http://gl.huixinmuqiang.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ur.hahajie.cn

[Q20] IN 列表
来源：http://vb.newstarts.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ln.gzmigu.cn

[Q21] 空值判断
来源：http://cf.huanxung.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://qp.bookmarksfly.cn

[Q22] 排序
来源：http://kk.huixiangedu.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://po.gzmigu.cn

[Q23] 分页
来源：http://fs.panjiajie.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://lw.wgjwhj.cn

[Q24] 去重
来源：http://gn.colortex.cn

SELECT DISTINCT city FROM users;
来源：http://vp.huixiangedu.cn

[Q25] 只取前 N 条
来源：http://wj.wgjwhj.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://in.jianghongdianzi.cn

[Q26] 计数
来源：http://kq.gzmigu.cn

SELECT COUNT(*) FROM users;
来源：http://oy.panjiajie.cn

[Q27] 条件计数
来源：http://it.bjjhwx.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://cg.shtwfgs.cn

[Q28] 求和与平均
来源：http://kt.yuexingan06.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://kn.huixinmuqiang.cn

[Q29] 最大最小值
来源：http://mt.wgjwhj.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://ms.gzmigu.cn

[Q30] 分组统计
来源：http://mp.huanxung.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://en.shtwfgs.cn

[Q31] 分组后过滤
来源：http://uj.521024.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://uu.521024.cn

[Q32] 分组拼接字符串
来源：http://hu.bookmarksfly.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wn.nicolike.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ac.521024.cn

[Q33] 多列分组
来源：http://oq.jianghongdianzi.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mr.lnxyls.cn

[Q34] 每组取第一条
来源：http://xw.shxzskj.cn

SELECT * FROM (
来源：http://qh.hnjuh.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://qh.hnjuh.cn

) t WHERE rn = 1;
来源：http://gm.szsharing.cn

[Q35] 内连接
来源：http://qa.shtwfgs.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://fw.lnxyls.cn

[Q36] 左连接
来源：http://tp.huanxung.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://qw.9csxet.cn

[Q37] 右连接
来源：http://gu.yuexingan06.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://st.panjiajie.cn

[Q38] 全外连接（PostgreSQL）
来源：http://eg.9csxet.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://lt.lnxyls.cn

[Q39] 自连接（查上下级）
来源：http://hn.bookmarksfly.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://on.haigaiapp.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://dk.nicolike.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://nu.bjjhwx.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wg.huixiangedu.cn

[Q41] 多表连接
来源：http://cq.panjiajie.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://gu.huanxung.cn

JOIN users u ON u.id = o.user_id
来源：http://ca.lnxyls.cn

JOIN products p ON p.id = o.product_id;
来源：http://xy.9csxet.cn

[Q42] 连接条件附加过滤
来源：http://bb.bookmarksfly.cn

SELECT u.name, o.amount FROM users u
来源：http://kd.bjjhwx.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ee.szxytkj.cn

[Q43] 标量子查询
来源：http://rs.bookmarksfly.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://kn.yuexingan06.cn

[Q44] IN 子查询
来源：http://iq.521024.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://dy.gzmigu.cn

[Q45] EXISTS 判断存在
来源：http://ax.shxzskj.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ax.hnjuh.cn

[Q46] NOT EXISTS 判断不存在
来源：http://dw.shxzskj.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://gi.shxzskj.cn

[Q47] 与平均值比较
来源：http://xs.yuexingan06.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://er.shxzskj.cn

[Q48] CTE 公用表表达式
来源：http://zn.gzmigu.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://po.panjiajie.cn

SELECT * FROM t WHERE c > 5;
来源：http://zd.521024.cn

[Q49] 更新单行
来源：http://dz.521024.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://tc.wgjwhj.cn

[Q50] 批量更新
来源：http://oz.lnxyls.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://qw.gzmigu.cn

[Q51] 用子查询更新
来源：http://zt.bookmarksfly.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://is.haigaiapp.cn

[Q52] 删除指定行
来源：http://rg.jctech888.com.cn

DELETE FROM users WHERE id = 10;
来源：http://fv.muxihuayi.cn

[Q53] 按条件删除
来源：http://ga.bjjhwx.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://cr.jianghongdianzi.cn

[Q54] 清空表
来源：http://ku.hnjuh.cn

TRUNCATE TABLE logs;
来源：http://tn.huixinmuqiang.cn

[Q55] 排名（并列占位）
来源：http://rt.szxytkj.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://xs.nszjky.cn

[Q56] 密集排名（并列不占位）
来源：http://bl.szxytkj.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://tr.huanxung.cn

[Q57] 行号
来源：http://vm.hahajie.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://tp.muxihuayi.cn

[Q58] 累计求和
来源：http://cl.bjjhwx.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://sa.9csxet.cn

[Q59] 分组内累计
来源：http://ya.yuntaijiaju.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://cq.nszjky.cn

[Q60] 取上一行 / 下一行
来源：http://jy.huixinmuqiang.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://dq.muxihuayi.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://lr.jianghongdianzi.cn

[Q61] 移动平均
来源：http://zn.yuexingan06.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ug.asd995.cn

[Q62] 分组占比
来源：http://wm.hnjuh.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://lr.haigaiapp.cn

[Q63] 开启事务
来源：http://ta.yuexingan06.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://kd.huixiangedu.cn

[Q64] 提交事务
来源：http://og.bookmarksfly.cn

COMMIT;
来源：http://hs.huanxung.cn

[Q65] 回滚事务
来源：http://ti.shxzukj.cn

ROLLBACK;
来源：http://xo.hnjuh.cn

[Q66] 行锁查询
来源：http://de.panjiajie.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://rq.chemitech.net.cn

[Q67] 设置隔离级别
来源：http://gk.nicolike.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://vn.haigaiapp.cn

[Q68] 保存点
来源：http://wm.shxzukj.cn

SAVEPOINT sp1;
来源：http://vc.yuntaijiaju.cn

ROLLBACK TO sp1;
来源：http://gq.szxytkj.cn

[Q69] 查看执行计划
来源：http://ku.shxzukj.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ce.hahajie.cn

[Q70] 更新统计信息
来源：http://bw.szxytkj.cn

ANALYZE TABLE users;
来源：http://pp.jctech888.com.cn

[Q71] 查看建表语句
来源：http://an.lnxyls.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://cs.muxihuayi.cn

[Q72] 查看索引
来源：http://li.shxzukj.cn

SHOW INDEX FROM users;
来源：http://yd.szxytkj.cn

[Q73] 查看表状态
来源：http://mx.wgjwhj.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://yl.newstarts.cn

[Q74] 强制使用索引
来源：http://og.nicolike.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://sj.huixinmuqiang.cn

[Q75] 日期格式化
来源：http://tw.gzmigu.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ce.colortex.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ru.jctech888.com.cn

[Q76] 按天统计
来源：http://sd.huixiangedu.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://bu.newstarts.cn

[Q77] 时间加减
来源：http://hs.asd995.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://pq.shtwfgs.cn

[Q78] 当前时间
来源：http://rj.szxytkj.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://bn.wgjwhj.cn

[Q79] 字符串拼接
来源：http://xt.jianghongdianzi.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://aq.newstarts.cn

[Q80] 字符串截取
来源：http://ub.hahajie.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ox.colortex.cn

[Q81] 字符串替换
来源：http://gd.huixinmuqiang.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://xw.panjiajie.cn

[Q82] 字符长度与字节长度
来源：http://pe.nicolike.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://fe.hahajie.cn

[Q83] 大小写转换
来源：http://yq.gzmigu.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ec.shxzukj.cn

[Q84] 去除首尾空格
来源：http://dw.nicolike.cn

SELECT TRIM(name) FROM users;
来源：http://bk.haigaiapp.cn

[Q85] 数值取整
来源：http://cj.nszjky.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://lz.yuexingan06.cn

[Q86] 读取 JSON 字段
来源：http://ow.huanxung.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.wgjwhj.cn

[Q87] JSON 字段做条件
来源：http://cz.hahajie.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://zk.shxzukj.cn

[Q88] 行转列（条件聚合）
来源：http://ns.shxzskj.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://xc.asd995.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ig.wgjwhj.cn

[Q89] 判断表是否存在
来源：http://gj.yuntaijiaju.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://pw.panjiajie.cn

[Q90] 生成序号列
来源：http://al.bookmarksfly.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hh.jianghongdianzi.cn

================================================================================
来源：http://nz.muxihuayi.cn

R. Bash 专题
来源：http://lh.bjjhwx.cn

================================================================================
来源：http://yx.gzmigu.cn

[R01] shebang 与严格模式
来源：http://qs.shxzskj.cn

#!/usr/bin/env bash
来源：http://na.colortex.cn

set -euo pipefail
来源：http://ij.huanxung.cn

[R02] 变量赋值与使用
来源：http://jv.hahajie.cn

name="Tom"; echo "$name"
来源：http://pe.shtwfgs.cn

[R03] 只读变量
来源：http://lg.muxihuayi.cn

readonly PI=3.14
来源：http://dg.gzmigu.cn

[R04] 位置参数
来源：http://ih.chemitech.net.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ck.bjjhwx.cn

[R05] 参数默认值
来源：http://ou.shxzskj.cn

name="${1:-default}"
来源：http://ug.newstarts.cn

[R06] 判断命令是否存在
来源：http://wx.hnjuh.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ja.nicolike.cn

[R07] if 判断文件
来源：http://sm.bjjhwx.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wg.9csxet.cn

[R08] 数值比较
来源：http://so.9csxet.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://ga.panjiajie.cn

[R09] 字符串比较
来源：http://sy.521024.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://qj.haigaiapp.cn

[R10] 正则匹配
来源：http://pq.muxihuayi.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://qv.huixiangedu.cn

[R11] case 多分支
来源：http://sn.wgjwhj.cn

case "$1" in
来源：http://qt.bjjhwx.cn

start) echo "启动" ;;
来源：http://bg.newstarts.cn

stop)  echo "停止" ;;
来源：http://ac.haigaiapp.cn

*)     echo "未知命令" ;;
来源：http://gi.huixiangedu.cn

esac
来源：http://gm.panjiajie.cn

[R12] for 遍历文件
来源：http://dx.nicolike.cn

for f in *.txt; do echo "$f"; done
来源：http://yi.huanxung.cn

[R13] for 计数循环
来源：http://bs.haigaiapp.cn

for i in {1..10}; do echo "$i"; done
来源：http://yy.szxytkj.cn

[R14] C 风格 for
来源：http://kw.newstarts.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://pt.nszjky.cn

[R15] while 逐行读文件
来源：http://go.shxzskj.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hk.szxytkj.cn

[R16] until 等待条件
来源：http://ms.shtwfgs.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://td.bookmarksfly.cn

[R17] 数组定义与取值
来源：http://aa.panjiajie.cn

arr=(a b c); echo "${arr[0]}"
来源：http://uj.nicolike.cn

[R18] 遍历数组
来源：http://yy.shtwfgs.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ho.muxihuayi.cn

[R19] 数组长度
来源：http://ti.huixinmuqiang.cn

echo "${#arr[@]}"
来源：http://fa.shtwfgs.cn

[R20] 关联数组（字典）
来源：http://xz.nicolike.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://bq.bjjhwx.cn

[R21] 字符串长度
来源：http://hh.hahajie.cn

echo "${#s}"
来源：http://bh.colortex.cn

[R22] 截取子串
来源：http://oe.521024.cn

echo "${s:0:5}"
来源：http://jd.yuntaijiaju.cn

[R23] 字符串替换
来源：http://nh.colortex.cn


<!-- 参考信息 -->