代发 wailian999

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://pr.shtwfgs.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://yb.szsharing.cn

Go:   reflect.DeepEqual(a, b)
来源：http://gc.bookmarksfly.cn

Ruby: a == b
来源：http://dm.huixiangedu.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ix.nicolike.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ft.shxzukj.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://yd.asd995.cn

PHP:  if (empty($x)) {}
来源：http://nx.szsharing.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://id.haigaiapp.cn

TS:   if (x == null) {}
来源：http://so.haigaiapp.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://su.521024.cn

Go:   if x == nil {}
来源：http://sa.huanxung.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://vz.hahajie.cn

C#:   if (x is null) {}
来源：http://vo.nszjky.cn

[P07] 防抖与节流
来源：http://hu.huanxung.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://qv.yuexingan06.cn

PHP:  // 手写时间戳比较
来源：http://rf.szsharing.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xx.hahajie.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://sv.szsharing.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ke.shtwfgs.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://gz.haigaiapp.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://ic.521024.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://oi.hahajie.cn

[P08] 处理浮点精度问题
来源：http://zj.jianghongdianzi.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://di.szsharing.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://uk.huixiangedu.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ms.521024.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ma.newstarts.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://fu.muxihuayi.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://nk.nicolike.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://rq.yuntaijiaju.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://nh.newstarts.cn

================================================================================
来源：http://mt.huixinmuqiang.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://xz.shxzskj.cn

================================================================================
来源：http://vz.colortex.cn

[Q01] 创建表
来源：http://ae.bjjhwx.cn

CREATE TABLE users (
来源：http://uz.muxihuayi.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wp.shtwfgs.cn

name VARCHAR(50) NOT NULL,
来源：http://kl.haigaiapp.cn

email VARCHAR(100) UNIQUE,
来源：http://yl.shxzskj.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wu.shtwfgs.cn

);
来源：http://kb.jctech888.com.cn

[Q02] 创建带外键的表
来源：http://cq.haigaiapp.cn

CREATE TABLE orders (
来源：http://nm.nszjky.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://eh.newstarts.cn

user_id INT NOT NULL,
来源：http://tt.jianghongdianzi.cn

amount DECIMAL(10, 2),
来源：http://xr.colortex.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://be.hnjuh.cn

);
来源：http://ba.huanxung.cn

[Q03] 增加列
来源：http://nh.colortex.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ts.huixiangedu.cn

[Q04] 修改列类型
来源：http://lr.nszjky.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://bv.muxihuayi.cn

[Q05] 重命名列
来源：http://xc.yuexingan06.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ar.hahajie.cn

[Q06] 删除列
来源：http://da.521024.cn

ALTER TABLE users DROP COLUMN age;
来源：http://nc.shxzskj.cn

[Q07] 删除表
来源：http://xb.haigaiapp.cn

DROP TABLE IF EXISTS orders;
来源：http://de.shtwfgs.cn

[Q08] 创建普通索引
来源：http://qm.shtwfgs.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://qh.huanxung.cn

[Q09] 创建唯一索引
来源：http://ov.chemitech.net.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://sv.colortex.cn

[Q10] 插入单行
来源：http://rm.nszjky.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://us.szxytkj.cn

[Q11] 一次插入多行
来源：http://iw.shxzukj.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://dx.newstarts.cn

[Q12] 插入后取自增 ID
来源：http://dp.haigaiapp.cn

INSERT INTO users (name) VALUES ('C');
来源：http://hv.521024.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mv.newstarts.cn

[Q13] 忽略重复插入
来源：http://kp.9csxet.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ru.szsharing.cn

[Q14] 存在则更新（upsert）
来源：http://ki.muxihuayi.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ng.bookmarksfly.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://gm.szxytkj.cn

[Q15] 查询全部
来源：http://np.jianghongdianzi.cn

SELECT * FROM users;
来源：http://qt.shxzukj.cn

[Q16] 查询指定列
来源：http://ti.huixiangedu.cn

SELECT id, name FROM users;
来源：http://nm.huanxung.cn

[Q17] 条件查询
来源：http://qk.hahajie.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://vi.haigaiapp.cn

[Q18] 模糊匹配
来源：http://ws.newstarts.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://jl.huixinmuqiang.cn

[Q19] 范围查询
来源：http://ux.lnxyls.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://me.muxihuayi.cn

[Q20] IN 列表
来源：http://vg.nicolike.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hw.nicolike.cn

[Q21] 空值判断
来源：http://up.yuexingan06.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://ks.lnxyls.cn

[Q22] 排序
来源：http://ev.huixiangedu.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://om.lnxyls.cn

[Q23] 分页
来源：http://tb.yuexingan06.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://xb.shxzukj.cn

[Q24] 去重
来源：http://up.newstarts.cn

SELECT DISTINCT city FROM users;
来源：http://pu.gzmigu.cn

[Q25] 只取前 N 条
来源：http://jj.chemitech.net.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://rb.jianghongdianzi.cn

[Q26] 计数
来源：http://le.huixiangedu.cn

SELECT COUNT(*) FROM users;
来源：http://xz.jctech888.com.cn

[Q27] 条件计数
来源：http://pk.huanxung.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://nm.huixiangedu.cn

[Q28] 求和与平均
来源：http://rh.nicolike.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://rb.colortex.cn

[Q29] 最大最小值
来源：http://nw.hnjuh.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://tc.bookmarksfly.cn

[Q30] 分组统计
来源：http://ny.jianghongdianzi.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://di.yuexingan06.cn

[Q31] 分组后过滤
来源：http://el.colortex.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://jm.nicolike.cn

[Q32] 分组拼接字符串
来源：http://vy.shxzukj.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ib.huixiangedu.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mk.panjiajie.cn

[Q33] 多列分组
来源：http://nd.jctech888.com.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ob.huanxung.cn

[Q34] 每组取第一条
来源：http://jk.asd995.cn

SELECT * FROM (
来源：http://rz.huanxung.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://at.shxzukj.cn

) t WHERE rn = 1;
来源：http://js.szxytkj.cn

[Q35] 内连接
来源：http://bv.bjjhwx.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://gg.hnjuh.cn

[Q36] 左连接
来源：http://yr.chemitech.net.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://gb.shxzukj.cn

[Q37] 右连接
来源：http://kz.huanxung.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ed.panjiajie.cn

[Q38] 全外连接（PostgreSQL）
来源：http://ym.nszjky.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://yk.521024.cn

[Q39] 自连接（查上下级）
来源：http://bv.jianghongdianzi.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://df.szxytkj.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://af.szsharing.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://vg.shtwfgs.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://va.bookmarksfly.cn

[Q41] 多表连接
来源：http://pe.bookmarksfly.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://om.9csxet.cn

JOIN users u ON u.id = o.user_id
来源：http://cx.bjjhwx.cn

JOIN products p ON p.id = o.product_id;
来源：http://km.bookmarksfly.cn

[Q42] 连接条件附加过滤
来源：http://dz.muxihuayi.cn

SELECT u.name, o.amount FROM users u
来源：http://hm.jianghongdianzi.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ua.lnxyls.cn

[Q43] 标量子查询
来源：http://zd.shxzskj.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://io.jctech888.com.cn

[Q44] IN 子查询
来源：http://op.wgjwhj.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://el.hnjuh.cn

[Q45] EXISTS 判断存在
来源：http://ez.hnjuh.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ku.hnjuh.cn

[Q46] NOT EXISTS 判断不存在
来源：http://by.huanxung.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://bc.yuexingan06.cn

[Q47] 与平均值比较
来源：http://tj.haigaiapp.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ao.shxzskj.cn

[Q48] CTE 公用表表达式
来源：http://rx.gzmigu.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://pd.hahajie.cn

SELECT * FROM t WHERE c > 5;
来源：http://ks.shxzskj.cn

[Q49] 更新单行
来源：http://ms.nicolike.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://yt.hahajie.cn

[Q50] 批量更新
来源：http://nc.szxytkj.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://fl.huixinmuqiang.cn

[Q51] 用子查询更新
来源：http://du.hahajie.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://rh.asd995.cn

[Q52] 删除指定行
来源：http://ep.muxihuayi.cn

DELETE FROM users WHERE id = 10;
来源：http://sp.bookmarksfly.cn

[Q53] 按条件删除
来源：http://jw.lnxyls.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://po.szxytkj.cn

[Q54] 清空表
来源：http://wn.muxihuayi.cn

TRUNCATE TABLE logs;
来源：http://lg.huanxung.cn

[Q55] 排名（并列占位）
来源：http://oy.huanxung.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://uu.muxihuayi.cn

[Q56] 密集排名（并列不占位）
来源：http://vy.jctech888.com.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://uc.nszjky.cn

[Q57] 行号
来源：http://kv.jctech888.com.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://jv.9csxet.cn

[Q58] 累计求和
来源：http://ka.gzmigu.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://cr.haigaiapp.cn

[Q59] 分组内累计
来源：http://ic.wgjwhj.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hk.haigaiapp.cn

[Q60] 取上一行 / 下一行
来源：http://zc.haigaiapp.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://tw.shxzukj.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://uq.nszjky.cn

[Q61] 移动平均
来源：http://vx.asd995.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://nw.nicolike.cn

[Q62] 分组占比
来源：http://qd.jctech888.com.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://al.9csxet.cn

[Q63] 开启事务
来源：http://yf.newstarts.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://pq.szsharing.cn

[Q64] 提交事务
来源：http://sp.huanxung.cn

COMMIT;
来源：http://kr.jianghongdianzi.cn

[Q65] 回滚事务
来源：http://hs.shtwfgs.cn

ROLLBACK;
来源：http://ej.9csxet.cn

[Q66] 行锁查询
来源：http://tr.9csxet.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://qt.shtwfgs.cn

[Q67] 设置隔离级别
来源：http://sf.wgjwhj.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://rl.hnjuh.cn

[Q68] 保存点
来源：http://kp.yuntaijiaju.cn

SAVEPOINT sp1;
来源：http://oi.521024.cn

ROLLBACK TO sp1;
来源：http://fg.shxzskj.cn

[Q69] 查看执行计划
来源：http://sv.gzmigu.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://kx.hnjuh.cn

[Q70] 更新统计信息
来源：http://mu.colortex.cn

ANALYZE TABLE users;
来源：http://pa.chemitech.net.cn

[Q71] 查看建表语句
来源：http://yv.hahajie.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://sp.chemitech.net.cn

[Q72] 查看索引
来源：http://cr.colortex.cn

SHOW INDEX FROM users;
来源：http://qq.nicolike.cn

[Q73] 查看表状态
来源：http://gg.yuntaijiaju.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://hq.jctech888.com.cn

[Q74] 强制使用索引
来源：http://su.shxzukj.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://cq.hnjuh.cn

[Q75] 日期格式化
来源：http://uy.wgjwhj.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://xx.9csxet.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://yk.yuexingan06.cn

[Q76] 按天统计
来源：http://rx.jctech888.com.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ay.yuntaijiaju.cn

[Q77] 时间加减
来源：http://qk.szsharing.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ha.shxzskj.cn

[Q78] 当前时间
来源：http://ff.gzmigu.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://jv.bookmarksfly.cn

[Q79] 字符串拼接
来源：http://wf.yuntaijiaju.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://xh.huixiangedu.cn

[Q80] 字符串截取
来源：http://ol.9csxet.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://pf.newstarts.cn

[Q81] 字符串替换
来源：http://ad.lnxyls.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://pz.lnxyls.cn

[Q82] 字符长度与字节长度
来源：http://xw.muxihuayi.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://qr.hnjuh.cn

[Q83] 大小写转换
来源：http://bx.gzmigu.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://yl.nicolike.cn

[Q84] 去除首尾空格
来源：http://gj.wgjwhj.cn

SELECT TRIM(name) FROM users;
来源：http://zp.jianghongdianzi.cn

[Q85] 数值取整
来源：http://wu.shxzukj.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://nw.newstarts.cn

[Q86] 读取 JSON 字段
来源：http://to.huixinmuqiang.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://jy.9csxet.cn

[Q87] JSON 字段做条件
来源：http://gn.haigaiapp.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hb.colortex.cn

[Q88] 行转列（条件聚合）
来源：http://sd.huanxung.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://fp.hnjuh.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://tj.bjjhwx.cn

[Q89] 判断表是否存在
来源：http://mv.hnjuh.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://jd.hahajie.cn

[Q90] 生成序号列
来源：http://dz.newstarts.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://it.jctech888.com.cn

================================================================================
来源：http://gq.szxytkj.cn

R. Bash 专题
来源：http://cd.huixinmuqiang.cn

================================================================================
来源：http://fv.jctech888.com.cn

[R01] shebang 与严格模式
来源：http://dy.haigaiapp.cn

#!/usr/bin/env bash
来源：http://ib.nszjky.cn

set -euo pipefail
来源：http://ek.521024.cn

[R02] 变量赋值与使用
来源：http://gp.hnjuh.cn

name="Tom"; echo "$name"
来源：http://bd.521024.cn

[R03] 只读变量
来源：http://ik.jianghongdianzi.cn

readonly PI=3.14
来源：http://rb.lnxyls.cn

[R04] 位置参数
来源：http://sp.szsharing.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://qu.bjjhwx.cn

[R05] 参数默认值
来源：http://ji.szsharing.cn

name="${1:-default}"
来源：http://lp.muxihuayi.cn

[R06] 判断命令是否存在
来源：http://jj.gzmigu.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://gl.bookmarksfly.cn

[R07] if 判断文件
来源：http://cx.nszjky.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://yp.shtwfgs.cn

[R08] 数值比较
来源：http://wn.chemitech.net.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://fp.521024.cn

[R09] 字符串比较
来源：http://hj.jctech888.com.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://cx.huanxung.cn

[R10] 正则匹配
来源：http://ms.huixiangedu.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ov.9csxet.cn

[R11] case 多分支
来源：http://uy.shtwfgs.cn

case "$1" in
来源：http://ew.chemitech.net.cn

start) echo "启动" ;;
来源：http://ud.jctech888.com.cn

stop)  echo "停止" ;;
来源：http://lc.nicolike.cn

*)     echo "未知命令" ;;
来源：http://gf.huixiangedu.cn

esac
来源：http://oa.newstarts.cn

[R12] for 遍历文件
来源：http://mu.nicolike.cn

for f in *.txt; do echo "$f"; done
来源：http://qu.nszjky.cn

[R13] for 计数循环
来源：http://al.yuntaijiaju.cn

for i in {1..10}; do echo "$i"; done
来源：http://gq.bjjhwx.cn

[R14] C 风格 for
来源：http://hi.newstarts.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ly.asd995.cn

[R15] while 逐行读文件
来源：http://wa.shxzskj.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ea.9csxet.cn

[R16] until 等待条件
来源：http://jx.9csxet.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://un.szsharing.cn

[R17] 数组定义与取值
来源：http://rb.szsharing.cn

arr=(a b c); echo "${arr[0]}"
来源：http://kq.hahajie.cn

[R18] 遍历数组
来源：http://jd.huanxung.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://io.jctech888.com.cn

[R19] 数组长度
来源：http://bg.huixinmuqiang.cn

echo "${#arr[@]}"
来源：http://mm.shtwfgs.cn

[R20] 关联数组（字典）
来源：http://pf.wgjwhj.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://js.lnxyls.cn

[R21] 字符串长度
来源：http://ab.9csxet.cn

echo "${#s}"
来源：http://io.colortex.cn

[R22] 截取子串
来源：http://fu.lnxyls.cn

echo "${s:0:5}"
来源：http://ru.szsharing.cn

[R23] 字符串替换
来源：http://be.szxytkj.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://fc.9csxet.cn

[R24] 大小写转换
来源：http://tu.huixinmuqiang.cn

echo "${s^^}"; echo "${s,,}"
来源：http://rx.nszjky.cn

[R25] 去后缀 / 去前缀
来源：http://tg.gzmigu.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://mb.shxzskj.cn

[R26] 命令替换
来源：http://wp.huanxung.cn

now=$(date +%F); echo "$now"
来源：http://du.jianghongdianzi.cn

[R27] 算术展开
来源：http://ey.wgjwhj.cn


<!-- 参考信息 -->