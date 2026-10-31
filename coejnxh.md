代发 wailian999

Java: list.size();  map.size();  s.length()
来源：http://kz.chemitech.net.cn

Go:   len(arr);  len(m)
来源：http://uf.jctech888.com.cn

Ruby: x.length;  x.size
来源：http://yh.nszjky.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://mf.hnjuh.cn

[P05] 判断两个对象内容是否相等
来源：http://jm.hnjuh.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://wu.newstarts.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://sl.yuexingan06.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://zc.nicolike.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://vk.asd995.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://vr.colortex.cn

Go:   reflect.DeepEqual(a, b)
来源：http://wk.panjiajie.cn

Ruby: a == b
来源：http://dl.9csxet.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ky.521024.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://zg.bookmarksfly.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://iw.huanxung.cn

PHP:  if (empty($x)) {}
来源：http://pd.wgjwhj.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wc.panjiajie.cn

TS:   if (x == null) {}
来源：http://gl.nszjky.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://ai.newstarts.cn

Go:   if x == nil {}
来源：http://hh.yuntaijiaju.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://dx.huixinmuqiang.cn

C#:   if (x is null) {}
来源：http://yf.newstarts.cn

[P07] 防抖与节流
来源：http://it.wgjwhj.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://vs.haigaiapp.cn

PHP:  // 手写时间戳比较
来源：http://jb.bookmarksfly.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://gr.shxzukj.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://gr.shxzukj.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://dq.jctech888.com.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://cf.szsharing.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://zx.haigaiapp.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mt.shxzskj.cn

[P08] 处理浮点精度问题
来源：http://me.colortex.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://fn.shtwfgs.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ey.huixinmuqiang.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://lg.colortex.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://er.jianghongdianzi.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wy.hahajie.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://fg.szxytkj.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://lk.panjiajie.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://jb.9csxet.cn

================================================================================
来源：http://ss.shxzukj.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://pu.huixiangedu.cn

================================================================================
来源：http://ug.chemitech.net.cn

[Q01] 创建表
来源：http://is.bookmarksfly.cn

CREATE TABLE users (
来源：http://ux.yuexingan06.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://cx.szxytkj.cn

name VARCHAR(50) NOT NULL,
来源：http://fx.lnxyls.cn

email VARCHAR(100) UNIQUE,
来源：http://pq.asd995.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ov.szxytkj.cn

);
来源：http://wc.hahajie.cn

[Q02] 创建带外键的表
来源：http://po.yuntaijiaju.cn

CREATE TABLE orders (
来源：http://xg.jctech888.com.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://rt.lnxyls.cn

user_id INT NOT NULL,
来源：http://ac.panjiajie.cn

amount DECIMAL(10, 2),
来源：http://fa.panjiajie.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ep.muxihuayi.cn

);
来源：http://tz.hahajie.cn

[Q03] 增加列
来源：http://sx.panjiajie.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://tu.asd995.cn

[Q04] 修改列类型
来源：http://iy.huixiangedu.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ht.hnjuh.cn

[Q05] 重命名列
来源：http://kf.bookmarksfly.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://am.chemitech.net.cn

[Q06] 删除列
来源：http://aj.jianghongdianzi.cn

ALTER TABLE users DROP COLUMN age;
来源：http://eo.szxytkj.cn

[Q07] 删除表
来源：http://px.shxzukj.cn

DROP TABLE IF EXISTS orders;
来源：http://sc.hnjuh.cn

[Q08] 创建普通索引
来源：http://tv.wgjwhj.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://dy.yuexingan06.cn

[Q09] 创建唯一索引
来源：http://ih.hnjuh.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ux.asd995.cn

[Q10] 插入单行
来源：http://gh.huixinmuqiang.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://kz.bjjhwx.cn

[Q11] 一次插入多行
来源：http://zj.jctech888.com.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://al.shxzskj.cn

[Q12] 插入后取自增 ID
来源：http://mq.huixinmuqiang.cn

INSERT INTO users (name) VALUES ('C');
来源：http://vc.asd995.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ko.huixinmuqiang.cn

[Q13] 忽略重复插入
来源：http://ca.szsharing.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ma.lnxyls.cn

[Q14] 存在则更新（upsert）
来源：http://ta.nszjky.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://fs.gzmigu.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ot.szxytkj.cn

[Q15] 查询全部
来源：http://cz.9csxet.cn

SELECT * FROM users;
来源：http://ov.colortex.cn

[Q16] 查询指定列
来源：http://gn.nszjky.cn

SELECT id, name FROM users;
来源：http://xk.muxihuayi.cn

[Q17] 条件查询
来源：http://dj.bjjhwx.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://vq.shxzskj.cn

[Q18] 模糊匹配
来源：http://qk.nszjky.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wn.9csxet.cn

[Q19] 范围查询
来源：http://nu.bjjhwx.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://jb.jctech888.com.cn

[Q20] IN 列表
来源：http://ft.huixinmuqiang.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://qf.shxzukj.cn

[Q21] 空值判断
来源：http://nd.huanxung.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://id.haigaiapp.cn

[Q22] 排序
来源：http://bp.asd995.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://uz.shtwfgs.cn

[Q23] 分页
来源：http://na.shtwfgs.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://jb.yuntaijiaju.cn

[Q24] 去重
来源：http://fv.yuexingan06.cn

SELECT DISTINCT city FROM users;
来源：http://tr.haigaiapp.cn

[Q25] 只取前 N 条
来源：http://gi.chemitech.net.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://og.szxytkj.cn

[Q26] 计数
来源：http://xu.bookmarksfly.cn

SELECT COUNT(*) FROM users;
来源：http://yx.panjiajie.cn

[Q27] 条件计数
来源：http://wc.huixiangedu.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://vi.lnxyls.cn

[Q28] 求和与平均
来源：http://id.gzmigu.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://qv.panjiajie.cn

[Q29] 最大最小值
来源：http://pz.hnjuh.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://wv.hahajie.cn

[Q30] 分组统计
来源：http://ie.shtwfgs.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hl.szxytkj.cn

[Q31] 分组后过滤
来源：http://la.nicolike.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://uu.shxzukj.cn

[Q32] 分组拼接字符串
来源：http://bk.lnxyls.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://qy.colortex.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://sh.newstarts.cn

[Q33] 多列分组
来源：http://dg.jctech888.com.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://dx.haigaiapp.cn

[Q34] 每组取第一条
来源：http://vg.shtwfgs.cn

SELECT * FROM (
来源：http://jg.colortex.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://uf.jctech888.com.cn

) t WHERE rn = 1;
来源：http://wa.huixinmuqiang.cn

[Q35] 内连接
来源：http://co.newstarts.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://xs.szxytkj.cn

[Q36] 左连接
来源：http://fq.huixiangedu.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wj.nicolike.cn

[Q37] 右连接
来源：http://me.521024.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://tf.gzmigu.cn

[Q38] 全外连接（PostgreSQL）
来源：http://gr.nicolike.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ra.colortex.cn

[Q39] 自连接（查上下级）
来源：http://qn.nszjky.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://om.jctech888.com.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wy.nszjky.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://gl.yuntaijiaju.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ly.yuntaijiaju.cn

[Q41] 多表连接
来源：http://ic.huixinmuqiang.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://tc.wgjwhj.cn

JOIN users u ON u.id = o.user_id
来源：http://vx.yuexingan06.cn

JOIN products p ON p.id = o.product_id;
来源：http://iy.hahajie.cn

[Q42] 连接条件附加过滤
来源：http://oz.hahajie.cn

SELECT u.name, o.amount FROM users u
来源：http://oc.bjjhwx.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://la.asd995.cn

[Q43] 标量子查询
来源：http://dm.yuntaijiaju.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ps.huixinmuqiang.cn

[Q44] IN 子查询
来源：http://fq.521024.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://bg.shxzskj.cn

[Q45] EXISTS 判断存在
来源：http://gv.wgjwhj.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://fp.bookmarksfly.cn

[Q46] NOT EXISTS 判断不存在
来源：http://ji.colortex.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://es.9csxet.cn

[Q47] 与平均值比较
来源：http://mv.chemitech.net.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://cy.haigaiapp.cn

[Q48] CTE 公用表表达式
来源：http://qz.shxzukj.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://dn.yuexingan06.cn

SELECT * FROM t WHERE c > 5;
来源：http://mx.colortex.cn

[Q49] 更新单行
来源：http://fq.shxzukj.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://nd.haigaiapp.cn

[Q50] 批量更新
来源：http://xg.szsharing.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://tk.huanxung.cn

[Q51] 用子查询更新
来源：http://wx.lnxyls.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://pd.lnxyls.cn

[Q52] 删除指定行
来源：http://jd.newstarts.cn

DELETE FROM users WHERE id = 10;
来源：http://ym.shxzskj.cn

[Q53] 按条件删除
来源：http://jp.yuntaijiaju.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://re.shxzskj.cn

[Q54] 清空表
来源：http://bw.huixinmuqiang.cn

TRUNCATE TABLE logs;
来源：http://tx.shxzukj.cn

[Q55] 排名（并列占位）
来源：http://hs.bookmarksfly.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://vy.nszjky.cn

[Q56] 密集排名（并列不占位）
来源：http://ey.jianghongdianzi.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hi.shxzskj.cn

[Q57] 行号
来源：http://er.szsharing.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://pq.szxytkj.cn

[Q58] 累计求和
来源：http://qb.yuntaijiaju.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://rr.asd995.cn

[Q59] 分组内累计
来源：http://ro.shxzukj.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://gv.huanxung.cn

[Q60] 取上一行 / 下一行
来源：http://uo.szxytkj.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://bu.wgjwhj.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ya.hahajie.cn

[Q61] 移动平均
来源：http://kz.huixinmuqiang.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://gq.huixinmuqiang.cn

[Q62] 分组占比
来源：http://av.newstarts.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://zg.bookmarksfly.cn

[Q63] 开启事务
来源：http://uy.shxzskj.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://ge.nicolike.cn

[Q64] 提交事务
来源：http://co.521024.cn

COMMIT;
来源：http://at.chemitech.net.cn

[Q65] 回滚事务
来源：http://nj.haigaiapp.cn

ROLLBACK;
来源：http://fy.lnxyls.cn

[Q66] 行锁查询
来源：http://ig.huixinmuqiang.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://oq.chemitech.net.cn

[Q67] 设置隔离级别
来源：http://oj.lnxyls.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://cl.hahajie.cn

[Q68] 保存点
来源：http://sp.shtwfgs.cn

SAVEPOINT sp1;
来源：http://nm.huixiangedu.cn

ROLLBACK TO sp1;
来源：http://se.szsharing.cn

[Q69] 查看执行计划
来源：http://mh.huixinmuqiang.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mq.bjjhwx.cn

[Q70] 更新统计信息
来源：http://qu.yuntaijiaju.cn

ANALYZE TABLE users;
来源：http://lt.colortex.cn

[Q71] 查看建表语句
来源：http://zm.huixiangedu.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://un.bookmarksfly.cn

[Q72] 查看索引
来源：http://ai.szxytkj.cn

SHOW INDEX FROM users;
来源：http://dl.shxzskj.cn

[Q73] 查看表状态
来源：http://kv.yuntaijiaju.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://we.jctech888.com.cn

[Q74] 强制使用索引
来源：http://em.yuexingan06.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://bh.521024.cn

[Q75] 日期格式化
来源：http://ng.9csxet.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://yf.hahajie.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://sl.nicolike.cn

[Q76] 按天统计
来源：http://io.521024.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://av.chemitech.net.cn

[Q77] 时间加减
来源：http://cx.hahajie.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://sg.haigaiapp.cn

[Q78] 当前时间
来源：http://ar.gzmigu.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://yy.shxzukj.cn

[Q79] 字符串拼接
来源：http://wu.9csxet.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wr.gzmigu.cn

[Q80] 字符串截取
来源：http://na.shxzskj.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wc.szxytkj.cn

[Q81] 字符串替换
来源：http://sx.huanxung.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ic.muxihuayi.cn

[Q82] 字符长度与字节长度
来源：http://nq.chemitech.net.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ip.lnxyls.cn

[Q83] 大小写转换
来源：http://ps.hahajie.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://it.newstarts.cn

[Q84] 去除首尾空格
来源：http://sp.gzmigu.cn

SELECT TRIM(name) FROM users;
来源：http://ye.9csxet.cn

[Q85] 数值取整
来源：http://mw.521024.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ks.bookmarksfly.cn

[Q86] 读取 JSON 字段
来源：http://wj.nszjky.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://xx.hnjuh.cn

[Q87] JSON 字段做条件
来源：http://fp.shtwfgs.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ri.nicolike.cn

[Q88] 行转列（条件聚合）
来源：http://ku.szxytkj.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://cs.nicolike.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://qv.huixinmuqiang.cn

[Q89] 判断表是否存在
来源：http://tr.newstarts.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://br.bjjhwx.cn

[Q90] 生成序号列
来源：http://td.gzmigu.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://yu.521024.cn

================================================================================
来源：http://ej.jianghongdianzi.cn

R. Bash 专题
来源：http://fz.huixiangedu.cn

================================================================================
来源：http://vk.asd995.cn

[R01] shebang 与严格模式
来源：http://qo.newstarts.cn

#!/usr/bin/env bash
来源：http://lk.yuexingan06.cn

set -euo pipefail
来源：http://ne.521024.cn

[R02] 变量赋值与使用
来源：http://bs.bookmarksfly.cn

name="Tom"; echo "$name"
来源：http://xt.newstarts.cn

[R03] 只读变量
来源：http://xn.jctech888.com.cn

readonly PI=3.14
来源：http://kw.yuexingan06.cn

[R04] 位置参数
来源：http://pv.shxzukj.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://yc.szsharing.cn

[R05] 参数默认值
来源：http://st.colortex.cn

name="${1:-default}"
来源：http://cj.szsharing.cn

[R06] 判断命令是否存在
来源：http://os.jctech888.com.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://vm.asd995.cn

[R07] if 判断文件
来源：http://qh.jianghongdianzi.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://qf.yuntaijiaju.cn

[R08] 数值比较
来源：http://mj.nicolike.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://kt.jianghongdianzi.cn

[R09] 字符串比较
来源：http://rc.bjjhwx.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://sh.panjiajie.cn

[R10] 正则匹配
来源：http://ay.bjjhwx.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://vn.wgjwhj.cn

[R11] case 多分支
来源：http://ml.bjjhwx.cn

case "$1" in
来源：http://ul.newstarts.cn

start) echo "启动" ;;
来源：http://hh.nicolike.cn

stop)  echo "停止" ;;
来源：http://bp.wgjwhj.cn

*)     echo "未知命令" ;;
来源：http://cf.hahajie.cn

esac
来源：http://yr.hnjuh.cn

[R12] for 遍历文件
来源：http://aa.yuntaijiaju.cn

for f in *.txt; do echo "$f"; done
来源：http://fs.haigaiapp.cn

[R13] for 计数循环
来源：http://ar.colortex.cn

for i in {1..10}; do echo "$i"; done
来源：http://xo.yuntaijiaju.cn

[R14] C 风格 for
来源：http://vy.szxytkj.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ej.bookmarksfly.cn

[R15] while 逐行读文件
来源：http://jc.huixiangedu.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wv.colortex.cn

[R16] until 等待条件
来源：http://sy.jctech888.com.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://bm.nicolike.cn

[R17] 数组定义与取值
来源：http://yq.jianghongdianzi.cn

arr=(a b c); echo "${arr[0]}"
来源：http://dt.haigaiapp.cn

[R18] 遍历数组
来源：http://is.yuexingan06.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://fh.muxihuayi.cn

[R19] 数组长度
来源：http://it.newstarts.cn

echo "${#arr[@]}"
来源：http://fr.bookmarksfly.cn

[R20] 关联数组（字典）
来源：http://rl.panjiajie.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://yy.jianghongdianzi.cn

[R21] 字符串长度
来源：http://by.wgjwhj.cn

echo "${#s}"
来源：http://ev.huixiangedu.cn

[R22] 截取子串
来源：http://sl.nszjky.cn

echo "${s:0:5}"
来源：http://aa.lnxyls.cn

[R23] 字符串替换
来源：http://uv.nszjky.cn


<!-- 参考信息 -->