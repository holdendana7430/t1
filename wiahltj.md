代发 wailian999

Java: list.size();  map.size();  s.length()
来源：http://ss.shtwfgs.cn

Go:   len(arr);  len(m)
来源：http://da.asd995.cn

Ruby: x.length;  x.size
来源：http://zj.colortex.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://xb.hnjuh.cn

[P05] 判断两个对象内容是否相等
来源：http://sn.bookmarksfly.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://ja.shxzukj.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://lk.jianghongdianzi.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://dl.szxytkj.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://pq.jctech888.com.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://nx.gzmigu.cn

Go:   reflect.DeepEqual(a, b)
来源：http://ur.jianghongdianzi.cn

Ruby: a == b
来源：http://uv.jctech888.com.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://vu.wgjwhj.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://an.szsharing.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://cm.gzmigu.cn

PHP:  if (empty($x)) {}
来源：http://iq.huixiangedu.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://tf.gzmigu.cn

TS:   if (x == null) {}
来源：http://rd.hnjuh.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://wk.chemitech.net.cn

Go:   if x == nil {}
来源：http://ue.lnxyls.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://rk.colortex.cn

C#:   if (x is null) {}
来源：http://sn.jianghongdianzi.cn

[P07] 防抖与节流
来源：http://mk.huanxung.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://st.colortex.cn

PHP:  // 手写时间戳比较
来源：http://sg.asd995.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://tr.gzmigu.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://du.huanxung.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://pu.panjiajie.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://jv.panjiajie.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://il.lnxyls.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wa.chemitech.net.cn

[P08] 处理浮点精度问题
来源：http://up.jctech888.com.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ab.huixiangedu.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://yb.panjiajie.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://fe.asd995.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://fe.shtwfgs.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ta.szsharing.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://nm.wgjwhj.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://lu.panjiajie.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://zq.shxzukj.cn

================================================================================
来源：http://qe.9csxet.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://he.jctech888.com.cn

================================================================================
来源：http://bj.asd995.cn

[Q01] 创建表
来源：http://ad.shxzukj.cn

CREATE TABLE users (
来源：http://az.haigaiapp.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://vd.nszjky.cn

name VARCHAR(50) NOT NULL,
来源：http://qx.nszjky.cn

email VARCHAR(100) UNIQUE,
来源：http://qi.hnjuh.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hi.yuntaijiaju.cn

);
来源：http://sr.colortex.cn

[Q02] 创建带外键的表
来源：http://cu.colortex.cn

CREATE TABLE orders (
来源：http://hx.521024.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://kr.hahajie.cn

user_id INT NOT NULL,
来源：http://lr.9csxet.cn

amount DECIMAL(10, 2),
来源：http://zv.haigaiapp.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://sv.haigaiapp.cn

);
来源：http://is.9csxet.cn

[Q03] 增加列
来源：http://hd.wgjwhj.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://lb.asd995.cn

[Q04] 修改列类型
来源：http://dv.panjiajie.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://zc.huanxung.cn

[Q05] 重命名列
来源：http://lp.chemitech.net.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://iz.shxzukj.cn

[Q06] 删除列
来源：http://sb.hnjuh.cn

ALTER TABLE users DROP COLUMN age;
来源：http://oq.jianghongdianzi.cn

[Q07] 删除表
来源：http://qo.panjiajie.cn

DROP TABLE IF EXISTS orders;
来源：http://rk.haigaiapp.cn

[Q08] 创建普通索引
来源：http://go.szxytkj.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://qc.newstarts.cn

[Q09] 创建唯一索引
来源：http://ln.chemitech.net.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wl.asd995.cn

[Q10] 插入单行
来源：http://qe.gzmigu.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://tp.huanxung.cn

[Q11] 一次插入多行
来源：http://xa.szsharing.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://rb.huixiangedu.cn

[Q12] 插入后取自增 ID
来源：http://ss.szsharing.cn

INSERT INTO users (name) VALUES ('C');
来源：http://qv.shxzskj.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ih.muxihuayi.cn

[Q13] 忽略重复插入
来源：http://gi.yuexingan06.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ua.hnjuh.cn

[Q14] 存在则更新（upsert）
来源：http://ed.huixinmuqiang.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wk.hahajie.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ny.jianghongdianzi.cn

[Q15] 查询全部
来源：http://wl.gzmigu.cn

SELECT * FROM users;
来源：http://ys.yuntaijiaju.cn

[Q16] 查询指定列
来源：http://qz.bookmarksfly.cn

SELECT id, name FROM users;
来源：http://iq.szsharing.cn

[Q17] 条件查询
来源：http://lo.wgjwhj.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://kq.bjjhwx.cn

[Q18] 模糊匹配
来源：http://ip.nicolike.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://pn.hnjuh.cn

[Q19] 范围查询
来源：http://ag.shxzskj.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ct.shtwfgs.cn

[Q20] IN 列表
来源：http://fx.huanxung.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://nj.szsharing.cn

[Q21] 空值判断
来源：http://np.yuntaijiaju.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://vp.gzmigu.cn

[Q22] 排序
来源：http://sb.huixinmuqiang.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ac.jctech888.com.cn

[Q23] 分页
来源：http://ys.521024.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ux.shtwfgs.cn

[Q24] 去重
来源：http://rc.jianghongdianzi.cn

SELECT DISTINCT city FROM users;
来源：http://sf.wgjwhj.cn

[Q25] 只取前 N 条
来源：http://bs.wgjwhj.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ek.hahajie.cn

[Q26] 计数
来源：http://se.yuntaijiaju.cn

SELECT COUNT(*) FROM users;
来源：http://qb.jianghongdianzi.cn

[Q27] 条件计数
来源：http://om.jctech888.com.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://pq.nicolike.cn

[Q28] 求和与平均
来源：http://hh.shtwfgs.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://bc.lnxyls.cn

[Q29] 最大最小值
来源：http://le.hnjuh.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://ou.szsharing.cn

[Q30] 分组统计
来源：http://om.yuexingan06.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://tx.nicolike.cn

[Q31] 分组后过滤
来源：http://sn.nicolike.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://kl.huixinmuqiang.cn

[Q32] 分组拼接字符串
来源：http://vd.lnxyls.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wn.colortex.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://lq.wgjwhj.cn

[Q33] 多列分组
来源：http://jv.muxihuayi.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://kk.szxytkj.cn

[Q34] 每组取第一条
来源：http://yh.szsharing.cn

SELECT * FROM (
来源：http://na.szxytkj.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ee.shxzukj.cn

) t WHERE rn = 1;
来源：http://vr.newstarts.cn

[Q35] 内连接
来源：http://ps.lnxyls.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://fm.jctech888.com.cn

[Q36] 左连接
来源：http://po.nicolike.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://qa.huixinmuqiang.cn

[Q37] 右连接
来源：http://fg.nszjky.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://lr.jctech888.com.cn

[Q38] 全外连接（PostgreSQL）
来源：http://ka.bookmarksfly.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wf.asd995.cn

[Q39] 自连接（查上下级）
来源：http://bc.nszjky.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://vm.wgjwhj.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://tm.lnxyls.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://ai.haigaiapp.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://vl.haigaiapp.cn

[Q41] 多表连接
来源：http://wj.bjjhwx.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://bm.chemitech.net.cn

JOIN users u ON u.id = o.user_id
来源：http://iz.szsharing.cn

JOIN products p ON p.id = o.product_id;
来源：http://we.huixiangedu.cn

[Q42] 连接条件附加过滤
来源：http://ke.jianghongdianzi.cn

SELECT u.name, o.amount FROM users u
来源：http://au.bjjhwx.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://xu.shxzukj.cn

[Q43] 标量子查询
来源：http://jo.shtwfgs.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://nd.shxzukj.cn

[Q44] IN 子查询
来源：http://hv.nszjky.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://nh.huixinmuqiang.cn

[Q45] EXISTS 判断存在
来源：http://ul.jctech888.com.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mp.hahajie.cn

[Q46] NOT EXISTS 判断不存在
来源：http://ld.9csxet.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mh.shxzukj.cn

[Q47] 与平均值比较
来源：http://if.szsharing.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://at.gzmigu.cn

[Q48] CTE 公用表表达式
来源：http://cp.colortex.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://lh.nicolike.cn

SELECT * FROM t WHERE c > 5;
来源：http://mn.huanxung.cn

[Q49] 更新单行
来源：http://oj.bookmarksfly.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ox.hnjuh.cn

[Q50] 批量更新
来源：http://fr.9csxet.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wk.wgjwhj.cn

[Q51] 用子查询更新
来源：http://yg.szxytkj.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://gd.chemitech.net.cn

[Q52] 删除指定行
来源：http://lk.wgjwhj.cn

DELETE FROM users WHERE id = 10;
来源：http://ph.lnxyls.cn

[Q53] 按条件删除
来源：http://os.bjjhwx.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://jj.521024.cn

[Q54] 清空表
来源：http://ma.szsharing.cn

TRUNCATE TABLE logs;
来源：http://xy.huixiangedu.cn

[Q55] 排名（并列占位）
来源：http://tl.jctech888.com.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://bb.muxihuayi.cn

[Q56] 密集排名（并列不占位）
来源：http://np.gzmigu.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://cn.bookmarksfly.cn

[Q57] 行号
来源：http://eq.wgjwhj.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://xb.bookmarksfly.cn

[Q58] 累计求和
来源：http://oe.asd995.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://je.gzmigu.cn

[Q59] 分组内累计
来源：http://rk.szsharing.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://nh.yuexingan06.cn

[Q60] 取上一行 / 下一行
来源：http://pr.szxytkj.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ay.huixiangedu.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://qs.jctech888.com.cn

[Q61] 移动平均
来源：http://kr.yuexingan06.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://nu.lnxyls.cn

[Q62] 分组占比
来源：http://iv.colortex.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://nh.gzmigu.cn

[Q63] 开启事务
来源：http://ey.shxzukj.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://cp.gzmigu.cn

[Q64] 提交事务
来源：http://sw.lnxyls.cn

COMMIT;
来源：http://xv.muxihuayi.cn

[Q65] 回滚事务
来源：http://qv.9csxet.cn

ROLLBACK;
来源：http://qq.jctech888.com.cn

[Q66] 行锁查询
来源：http://rz.521024.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://bh.muxihuayi.cn

[Q67] 设置隔离级别
来源：http://je.jianghongdianzi.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ip.yuntaijiaju.cn

[Q68] 保存点
来源：http://kd.szxytkj.cn

SAVEPOINT sp1;
来源：http://ot.gzmigu.cn

ROLLBACK TO sp1;
来源：http://yg.yuntaijiaju.cn

[Q69] 查看执行计划
来源：http://zo.hahajie.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ni.szxytkj.cn

[Q70] 更新统计信息
来源：http://yn.nszjky.cn

ANALYZE TABLE users;
来源：http://cz.shxzskj.cn

[Q71] 查看建表语句
来源：http://gn.nicolike.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://tg.gzmigu.cn

[Q72] 查看索引
来源：http://st.gzmigu.cn

SHOW INDEX FROM users;
来源：http://ls.jianghongdianzi.cn

[Q73] 查看表状态
来源：http://wp.huixinmuqiang.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://ob.jctech888.com.cn

[Q74] 强制使用索引
来源：http://ra.hahajie.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://xq.huixiangedu.cn

[Q75] 日期格式化
来源：http://xr.nszjky.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mw.jianghongdianzi.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ui.huixiangedu.cn

[Q76] 按天统计
来源：http://xf.huixinmuqiang.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ht.521024.cn

[Q77] 时间加减
来源：http://hm.haigaiapp.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://uz.yuntaijiaju.cn

[Q78] 当前时间
来源：http://hz.bookmarksfly.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ux.chemitech.net.cn

[Q79] 字符串拼接
来源：http://jy.panjiajie.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://fp.huanxung.cn

[Q80] 字符串截取
来源：http://fp.shtwfgs.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://yp.huixinmuqiang.cn

[Q81] 字符串替换
来源：http://am.lnxyls.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://na.huixinmuqiang.cn

[Q82] 字符长度与字节长度
来源：http://ih.huixinmuqiang.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://qq.huixiangedu.cn

[Q83] 大小写转换
来源：http://zj.hnjuh.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://gh.colortex.cn

[Q84] 去除首尾空格
来源：http://rk.chemitech.net.cn

SELECT TRIM(name) FROM users;
来源：http://aa.huixinmuqiang.cn

[Q85] 数值取整
来源：http://sr.hahajie.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://sl.lnxyls.cn

[Q86] 读取 JSON 字段
来源：http://hp.lnxyls.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://jt.lnxyls.cn

[Q87] JSON 字段做条件
来源：http://mq.nicolike.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ap.wgjwhj.cn

[Q88] 行转列（条件聚合）
来源：http://fe.chemitech.net.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://pr.chemitech.net.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://cg.huanxung.cn

[Q89] 判断表是否存在
来源：http://tu.jianghongdianzi.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://dz.nszjky.cn

[Q90] 生成序号列
来源：http://kv.huixinmuqiang.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://et.521024.cn

================================================================================
来源：http://tc.huanxung.cn

R. Bash 专题
来源：http://nz.hnjuh.cn

================================================================================
来源：http://sv.jianghongdianzi.cn

[R01] shebang 与严格模式
来源：http://we.haigaiapp.cn

#!/usr/bin/env bash
来源：http://mt.huanxung.cn

set -euo pipefail
来源：http://ld.huanxung.cn

[R02] 变量赋值与使用
来源：http://mg.nszjky.cn

name="Tom"; echo "$name"
来源：http://zp.bjjhwx.cn

[R03] 只读变量
来源：http://yd.bjjhwx.cn

readonly PI=3.14
来源：http://qw.panjiajie.cn

[R04] 位置参数
来源：http://mi.szsharing.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://jf.huixiangedu.cn

[R05] 参数默认值
来源：http://cs.jianghongdianzi.cn

name="${1:-default}"
来源：http://lt.szxytkj.cn

[R06] 判断命令是否存在
来源：http://vj.huixinmuqiang.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://xo.shxzukj.cn

[R07] if 判断文件
来源：http://ta.szsharing.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://lz.jianghongdianzi.cn

[R08] 数值比较
来源：http://zp.colortex.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://br.yuexingan06.cn

[R09] 字符串比较
来源：http://ao.hahajie.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://cq.szsharing.cn

[R10] 正则匹配
来源：http://tk.shxzukj.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://gc.bookmarksfly.cn

[R11] case 多分支
来源：http://ws.yuntaijiaju.cn

case "$1" in
来源：http://xu.wgjwhj.cn

start) echo "启动" ;;
来源：http://ow.nicolike.cn

stop)  echo "停止" ;;
来源：http://as.9csxet.cn

*)     echo "未知命令" ;;
来源：http://dy.521024.cn

esac
来源：http://ee.muxihuayi.cn

[R12] for 遍历文件
来源：http://tk.wgjwhj.cn

for f in *.txt; do echo "$f"; done
来源：http://pj.panjiajie.cn

[R13] for 计数循环
来源：http://cw.hnjuh.cn

for i in {1..10}; do echo "$i"; done
来源：http://os.hahajie.cn

[R14] C 风格 for
来源：http://dj.szxytkj.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ug.huanxung.cn

[R15] while 逐行读文件
来源：http://ro.gzmigu.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://an.9csxet.cn

[R16] until 等待条件
来源：http://ac.chemitech.net.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://lk.huixiangedu.cn

[R17] 数组定义与取值
来源：http://wo.nicolike.cn

arr=(a b c); echo "${arr[0]}"
来源：http://tq.asd995.cn

[R18] 遍历数组
来源：http://ry.panjiajie.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://re.haigaiapp.cn

[R19] 数组长度
来源：http://lj.shxzukj.cn

echo "${#arr[@]}"
来源：http://wv.nicolike.cn

[R20] 关联数组（字典）
来源：http://ez.shxzukj.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://kj.nszjky.cn

[R21] 字符串长度
来源：http://ya.haigaiapp.cn

echo "${#s}"
来源：http://cj.9csxet.cn

[R22] 截取子串
来源：http://ef.hahajie.cn

echo "${s:0:5}"
来源：http://ll.wgjwhj.cn

[R23] 字符串替换
来源：http://sj.muxihuayi.cn


<!-- 参考信息 -->