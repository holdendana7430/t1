代发 wailian999

[P05] 判断两个对象内容是否相等
来源：http://la.chemitech.net.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://cp.bookmarksfly.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://yf.huixiangedu.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://iu.szsharing.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://np.newstarts.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ei.huanxung.cn

Go:   reflect.DeepEqual(a, b)
来源：http://fq.nszjky.cn

Ruby: a == b
来源：http://ye.huixinmuqiang.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://fa.bookmarksfly.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://bb.muxihuayi.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://rk.yuntaijiaju.cn

PHP:  if (empty($x)) {}
来源：http://wt.muxihuayi.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://gj.9csxet.cn

TS:   if (x == null) {}
来源：http://ls.yuexingan06.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://tj.muxihuayi.cn

Go:   if x == nil {}
来源：http://zo.nicolike.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ex.nszjky.cn

C#:   if (x is null) {}
来源：http://jy.szsharing.cn

[P07] 防抖与节流
来源：http://sq.haigaiapp.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mm.muxihuayi.cn

PHP:  // 手写时间戳比较
来源：http://ds.9csxet.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://me.yuntaijiaju.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://tx.jctech888.com.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://dt.hahajie.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://yt.huixinmuqiang.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://qf.jctech888.com.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://md.gzmigu.cn

[P08] 处理浮点精度问题
来源：http://mb.nszjky.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mk.wgjwhj.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mr.yuntaijiaju.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://oi.yuexingan06.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://pf.szxytkj.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://lq.huanxung.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://fe.nicolike.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://qq.521024.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://fe.asd995.cn

================================================================================
来源：http://do.yuntaijiaju.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://kk.panjiajie.cn

================================================================================
来源：http://dq.panjiajie.cn

[Q01] 创建表
来源：http://aj.haigaiapp.cn

CREATE TABLE users (
来源：http://zd.yuntaijiaju.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://aa.panjiajie.cn

name VARCHAR(50) NOT NULL,
来源：http://xq.gzmigu.cn

email VARCHAR(100) UNIQUE,
来源：http://sx.chemitech.net.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://bj.9csxet.cn

);
来源：http://gv.panjiajie.cn

[Q02] 创建带外键的表
来源：http://fr.jianghongdianzi.cn

CREATE TABLE orders (
来源：http://yc.asd995.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ex.haigaiapp.cn

user_id INT NOT NULL,
来源：http://qs.asd995.cn

amount DECIMAL(10, 2),
来源：http://dv.asd995.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://gk.jctech888.com.cn

);
来源：http://aw.hahajie.cn

[Q03] 增加列
来源：http://ky.hahajie.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://of.hahajie.cn

[Q04] 修改列类型
来源：http://vh.asd995.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://kq.newstarts.cn

[Q05] 重命名列
来源：http://xm.szsharing.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://gb.9csxet.cn

[Q06] 删除列
来源：http://nx.haigaiapp.cn

ALTER TABLE users DROP COLUMN age;
来源：http://su.gzmigu.cn

[Q07] 删除表
来源：http://su.colortex.cn

DROP TABLE IF EXISTS orders;
来源：http://gf.szxytkj.cn

[Q08] 创建普通索引
来源：http://kz.jianghongdianzi.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://es.yuntaijiaju.cn

[Q09] 创建唯一索引
来源：http://fc.jianghongdianzi.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ut.shxzskj.cn

[Q10] 插入单行
来源：http://qz.muxihuayi.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://di.lnxyls.cn

[Q11] 一次插入多行
来源：http://wi.asd995.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://oo.shtwfgs.cn

[Q12] 插入后取自增 ID
来源：http://be.huixinmuqiang.cn

INSERT INTO users (name) VALUES ('C');
来源：http://xs.yuexingan06.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://qv.wgjwhj.cn

[Q13] 忽略重复插入
来源：http://vx.shtwfgs.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://pn.newstarts.cn

[Q14] 存在则更新（upsert）
来源：http://ty.huixiangedu.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://nj.colortex.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://dl.shxzukj.cn

[Q15] 查询全部
来源：http://vm.chemitech.net.cn

SELECT * FROM users;
来源：http://zg.yuexingan06.cn

[Q16] 查询指定列
来源：http://ia.gzmigu.cn

SELECT id, name FROM users;
来源：http://nn.shxzskj.cn

[Q17] 条件查询
来源：http://cf.jianghongdianzi.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ci.nszjky.cn

[Q18] 模糊匹配
来源：http://zy.muxihuayi.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://fy.huixinmuqiang.cn

[Q19] 范围查询
来源：http://zb.hahajie.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ey.huanxung.cn

[Q20] IN 列表
来源：http://gb.newstarts.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ag.newstarts.cn

[Q21] 空值判断
来源：http://ja.521024.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://sp.521024.cn

[Q22] 排序
来源：http://vl.szsharing.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://bt.yuexingan06.cn

[Q23] 分页
来源：http://eo.shxzskj.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://rp.yuexingan06.cn

[Q24] 去重
来源：http://zk.szxytkj.cn

SELECT DISTINCT city FROM users;
来源：http://sh.huixiangedu.cn

[Q25] 只取前 N 条
来源：http://cz.bookmarksfly.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://zb.shxzukj.cn

[Q26] 计数
来源：http://ge.asd995.cn

SELECT COUNT(*) FROM users;
来源：http://ui.gzmigu.cn

[Q27] 条件计数
来源：http://aa.huixinmuqiang.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://yj.521024.cn

[Q28] 求和与平均
来源：http://uq.szsharing.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://xf.521024.cn

[Q29] 最大最小值
来源：http://av.muxihuayi.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://fs.huixinmuqiang.cn

[Q30] 分组统计
来源：http://jo.nicolike.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://qe.jianghongdianzi.cn

[Q31] 分组后过滤
来源：http://ak.newstarts.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://cg.huixiangedu.cn

[Q32] 分组拼接字符串
来源：http://ju.yuntaijiaju.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://oq.yuntaijiaju.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://qk.huixiangedu.cn

[Q33] 多列分组
来源：http://ie.asd995.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://pu.chemitech.net.cn

[Q34] 每组取第一条
来源：http://es.hnjuh.cn

SELECT * FROM (
来源：http://vr.huanxung.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mh.yuexingan06.cn

) t WHERE rn = 1;
来源：http://rj.huixiangedu.cn

[Q35] 内连接
来源：http://wy.huixiangedu.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mr.bjjhwx.cn

[Q36] 左连接
来源：http://pp.asd995.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://gb.colortex.cn

[Q37] 右连接
来源：http://zh.huanxung.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wc.jctech888.com.cn

[Q38] 全外连接（PostgreSQL）
来源：http://iz.huanxung.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ji.newstarts.cn

[Q39] 自连接（查上下级）
来源：http://by.nszjky.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://hj.shxzskj.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://tv.shtwfgs.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://gy.yuntaijiaju.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://rw.jctech888.com.cn

[Q41] 多表连接
来源：http://jn.hnjuh.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://vv.colortex.cn

JOIN users u ON u.id = o.user_id
来源：http://an.shxzskj.cn

JOIN products p ON p.id = o.product_id;
来源：http://ad.gzmigu.cn

[Q42] 连接条件附加过滤
来源：http://sc.shxzskj.cn

SELECT u.name, o.amount FROM users u
来源：http://mo.szsharing.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://kc.wgjwhj.cn

[Q43] 标量子查询
来源：http://hu.nszjky.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ek.521024.cn

[Q44] IN 子查询
来源：http://zf.shxzskj.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://oh.asd995.cn

[Q45] EXISTS 判断存在
来源：http://lp.521024.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://rk.hnjuh.cn

[Q46] NOT EXISTS 判断不存在
来源：http://go.wgjwhj.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://dw.szxytkj.cn

[Q47] 与平均值比较
来源：http://gw.muxihuayi.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://xi.shxzskj.cn

[Q48] CTE 公用表表达式
来源：http://ya.haigaiapp.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://xh.newstarts.cn

SELECT * FROM t WHERE c > 5;
来源：http://vs.panjiajie.cn

[Q49] 更新单行
来源：http://tr.521024.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mk.jctech888.com.cn

[Q50] 批量更新
来源：http://db.gzmigu.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://ui.chemitech.net.cn

[Q51] 用子查询更新
来源：http://hv.chemitech.net.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://au.lnxyls.cn

[Q52] 删除指定行
来源：http://jf.newstarts.cn

DELETE FROM users WHERE id = 10;
来源：http://nd.hnjuh.cn

[Q53] 按条件删除
来源：http://jh.bjjhwx.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://av.nszjky.cn

[Q54] 清空表
来源：http://pc.asd995.cn

TRUNCATE TABLE logs;
来源：http://mk.bookmarksfly.cn

[Q55] 排名（并列占位）
来源：http://qx.haigaiapp.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hp.huixiangedu.cn

[Q56] 密集排名（并列不占位）
来源：http://yn.colortex.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ob.yuexingan06.cn

[Q57] 行号
来源：http://un.shtwfgs.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hw.bjjhwx.cn

[Q58] 累计求和
来源：http://mi.shtwfgs.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://je.yuexingan06.cn

[Q59] 分组内累计
来源：http://jq.jianghongdianzi.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://jb.newstarts.cn

[Q60] 取上一行 / 下一行
来源：http://hy.nszjky.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://sr.muxihuayi.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wo.hahajie.cn

[Q61] 移动平均
来源：http://bq.newstarts.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wp.yuexingan06.cn

[Q62] 分组占比
来源：http://st.521024.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ns.asd995.cn

[Q63] 开启事务
来源：http://fq.hnjuh.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://bt.nszjky.cn

[Q64] 提交事务
来源：http://cx.wgjwhj.cn

COMMIT;
来源：http://gv.muxihuayi.cn

[Q65] 回滚事务
来源：http://yd.521024.cn

ROLLBACK;
来源：http://zj.szxytkj.cn

[Q66] 行锁查询
来源：http://rj.szsharing.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://la.yuexingan06.cn

[Q67] 设置隔离级别
来源：http://gh.bookmarksfly.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://sy.yuexingan06.cn

[Q68] 保存点
来源：http://gj.nicolike.cn

SAVEPOINT sp1;
来源：http://fb.chemitech.net.cn

ROLLBACK TO sp1;
来源：http://rf.szsharing.cn

[Q69] 查看执行计划
来源：http://ta.bookmarksfly.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hi.521024.cn

[Q70] 更新统计信息
来源：http://mq.newstarts.cn

ANALYZE TABLE users;
来源：http://ze.9csxet.cn

[Q71] 查看建表语句
来源：http://am.shxzukj.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ga.newstarts.cn

[Q72] 查看索引
来源：http://ry.shxzukj.cn

SHOW INDEX FROM users;
来源：http://ih.bjjhwx.cn

[Q73] 查看表状态
来源：http://hf.huixiangedu.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://tt.shtwfgs.cn

[Q74] 强制使用索引
来源：http://fx.shxzskj.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ax.newstarts.cn

[Q75] 日期格式化
来源：http://eo.521024.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://kb.gzmigu.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://qi.nicolike.cn

[Q76] 按天统计
来源：http://zu.panjiajie.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://vj.huixinmuqiang.cn

[Q77] 时间加减
来源：http://lp.muxihuayi.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://sv.521024.cn

[Q78] 当前时间
来源：http://qp.muxihuayi.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://cz.hnjuh.cn

[Q79] 字符串拼接
来源：http://ml.bookmarksfly.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ni.szxytkj.cn

[Q80] 字符串截取
来源：http://sn.asd995.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://vj.huixinmuqiang.cn

[Q81] 字符串替换
来源：http://jm.huanxung.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://lo.huixiangedu.cn

[Q82] 字符长度与字节长度
来源：http://pw.gzmigu.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://av.muxihuayi.cn

[Q83] 大小写转换
来源：http://la.hnjuh.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://qb.haigaiapp.cn

[Q84] 去除首尾空格
来源：http://gg.haigaiapp.cn

SELECT TRIM(name) FROM users;
来源：http://cm.colortex.cn

[Q85] 数值取整
来源：http://gq.lnxyls.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://qt.haigaiapp.cn

[Q86] 读取 JSON 字段
来源：http://fb.yuntaijiaju.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wq.colortex.cn

[Q87] JSON 字段做条件
来源：http://kn.jianghongdianzi.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ik.nicolike.cn

[Q88] 行转列（条件聚合）
来源：http://tv.jctech888.com.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://no.shtwfgs.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://pu.szsharing.cn

[Q89] 判断表是否存在
来源：http://bq.gzmigu.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://if.jctech888.com.cn

[Q90] 生成序号列
来源：http://nk.huanxung.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://br.shxzskj.cn

================================================================================
来源：http://rt.nicolike.cn

R. Bash 专题
来源：http://ne.9csxet.cn

================================================================================
来源：http://cq.shxzukj.cn

[R01] shebang 与严格模式
来源：http://km.chemitech.net.cn

#!/usr/bin/env bash
来源：http://ya.bookmarksfly.cn

set -euo pipefail
来源：http://np.colortex.cn

[R02] 变量赋值与使用
来源：http://xh.wgjwhj.cn

name="Tom"; echo "$name"
来源：http://iq.panjiajie.cn

[R03] 只读变量
来源：http://yx.colortex.cn

readonly PI=3.14
来源：http://iw.szxytkj.cn

[R04] 位置参数
来源：http://gv.chemitech.net.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://av.shxzukj.cn

[R05] 参数默认值
来源：http://kc.haigaiapp.cn

name="${1:-default}"
来源：http://ft.yuntaijiaju.cn

[R06] 判断命令是否存在
来源：http://ho.panjiajie.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ek.huixinmuqiang.cn

[R07] if 判断文件
来源：http://jd.szxytkj.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://el.jianghongdianzi.cn

[R08] 数值比较
来源：http://yy.szxytkj.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://dg.asd995.cn

[R09] 字符串比较
来源：http://pe.lnxyls.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://pt.shxzskj.cn

[R10] 正则匹配
来源：http://my.bookmarksfly.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://qf.hahajie.cn

[R11] case 多分支
来源：http://jh.huixiangedu.cn

case "$1" in
来源：http://pr.9csxet.cn

start) echo "启动" ;;
来源：http://qv.bookmarksfly.cn

stop)  echo "停止" ;;
来源：http://tk.lnxyls.cn

*)     echo "未知命令" ;;
来源：http://lw.chemitech.net.cn

esac
来源：http://rt.shxzukj.cn

[R12] for 遍历文件
来源：http://sx.muxihuayi.cn

for f in *.txt; do echo "$f"; done
来源：http://hg.szxytkj.cn

[R13] for 计数循环
来源：http://mq.haigaiapp.cn

for i in {1..10}; do echo "$i"; done
来源：http://um.colortex.cn

[R14] C 风格 for
来源：http://rb.521024.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://rb.nicolike.cn

[R15] while 逐行读文件
来源：http://iw.yuexingan06.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ta.gzmigu.cn

[R16] until 等待条件
来源：http://mu.shxzukj.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://om.9csxet.cn

[R17] 数组定义与取值
来源：http://gr.nszjky.cn

arr=(a b c); echo "${arr[0]}"
来源：http://uv.huanxung.cn

[R18] 遍历数组
来源：http://bm.521024.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://bj.9csxet.cn

[R19] 数组长度
来源：http://ev.haigaiapp.cn

echo "${#arr[@]}"
来源：http://jh.hnjuh.cn

[R20] 关联数组（字典）
来源：http://ee.shxzskj.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://cu.jianghongdianzi.cn

[R21] 字符串长度
来源：http://uj.jianghongdianzi.cn

echo "${#s}"
来源：http://ll.huixiangedu.cn

[R22] 截取子串
来源：http://zz.huixinmuqiang.cn

echo "${s:0:5}"
来源：http://fn.shxzskj.cn

[R23] 字符串替换
来源：http://rf.huixiangedu.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://yt.bookmarksfly.cn

[R24] 大小写转换
来源：http://xf.panjiajie.cn

echo "${s^^}"; echo "${s,,}"
来源：http://uu.bjjhwx.cn

[R25] 去后缀 / 去前缀
来源：http://qu.hahajie.cn


<!-- 参考信息 -->