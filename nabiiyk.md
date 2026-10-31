代发 wailian999

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ps.huixiangedu.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ek.shxzskj.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hl.yuntaijiaju.cn

PHP:  if (empty($x)) {}
来源：http://pl.shxzukj.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://um.jctech888.com.cn

TS:   if (x == null) {}
来源：http://yy.bookmarksfly.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://cd.wgjwhj.cn

Go:   if x == nil {}
来源：http://ej.asd995.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://iu.huanxung.cn

C#:   if (x is null) {}
来源：http://ik.szxytkj.cn

[P07] 防抖与节流
来源：http://pl.yuntaijiaju.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://gg.nicolike.cn

PHP:  // 手写时间戳比较
来源：http://xk.jianghongdianzi.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://pk.shxzskj.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ii.hahajie.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://pm.jianghongdianzi.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ti.newstarts.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://js.shxzukj.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ka.yuexingan06.cn

[P08] 处理浮点精度问题
来源：http://mg.jctech888.com.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ax.jianghongdianzi.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ol.huanxung.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ga.lnxyls.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ny.jctech888.com.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ob.chemitech.net.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hw.gzmigu.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://zn.jctech888.com.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wb.521024.cn

================================================================================
来源：http://rd.521024.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://te.shtwfgs.cn

================================================================================
来源：http://hf.yuexingan06.cn

[Q01] 创建表
来源：http://ie.newstarts.cn

CREATE TABLE users (
来源：http://tk.muxihuayi.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://uj.lnxyls.cn

name VARCHAR(50) NOT NULL,
来源：http://iu.panjiajie.cn

email VARCHAR(100) UNIQUE,
来源：http://ck.nicolike.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://rt.huanxung.cn

);
来源：http://ho.panjiajie.cn

[Q02] 创建带外键的表
来源：http://oy.newstarts.cn

CREATE TABLE orders (
来源：http://hy.yuexingan06.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://dg.hahajie.cn

user_id INT NOT NULL,
来源：http://qs.nszjky.cn

amount DECIMAL(10, 2),
来源：http://dx.hahajie.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ud.muxihuayi.cn

);
来源：http://dk.jianghongdianzi.cn

[Q03] 增加列
来源：http://jl.gzmigu.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://fr.shtwfgs.cn

[Q04] 修改列类型
来源：http://ur.shtwfgs.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://xh.muxihuayi.cn

[Q05] 重命名列
来源：http://bc.521024.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://rk.yuexingan06.cn

[Q06] 删除列
来源：http://tx.huixiangedu.cn

ALTER TABLE users DROP COLUMN age;
来源：http://jm.shxzukj.cn

[Q07] 删除表
来源：http://or.huixiangedu.cn

DROP TABLE IF EXISTS orders;
来源：http://az.nszjky.cn

[Q08] 创建普通索引
来源：http://uz.szxytkj.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://da.colortex.cn

[Q09] 创建唯一索引
来源：http://ed.hnjuh.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ux.shtwfgs.cn

[Q10] 插入单行
来源：http://sh.9csxet.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://zv.nicolike.cn

[Q11] 一次插入多行
来源：http://py.bjjhwx.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ed.bookmarksfly.cn

[Q12] 插入后取自增 ID
来源：http://mu.bookmarksfly.cn

INSERT INTO users (name) VALUES ('C');
来源：http://lz.chemitech.net.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://pd.haigaiapp.cn

[Q13] 忽略重复插入
来源：http://gd.nszjky.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://kf.jianghongdianzi.cn

[Q14] 存在则更新（upsert）
来源：http://im.jctech888.com.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://gw.asd995.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://pt.shxzukj.cn

[Q15] 查询全部
来源：http://th.bjjhwx.cn

SELECT * FROM users;
来源：http://rf.huixiangedu.cn

[Q16] 查询指定列
来源：http://qn.yuntaijiaju.cn

SELECT id, name FROM users;
来源：http://jt.shtwfgs.cn

[Q17] 条件查询
来源：http://py.nszjky.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://qa.yuexingan06.cn

[Q18] 模糊匹配
来源：http://sj.shxzukj.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://cv.newstarts.cn

[Q19] 范围查询
来源：http://ti.hnjuh.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ys.colortex.cn

[Q20] IN 列表
来源：http://zv.gzmigu.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://yj.newstarts.cn

[Q21] 空值判断
来源：http://ih.panjiajie.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://ad.shxzukj.cn

[Q22] 排序
来源：http://bi.szxytkj.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ic.gzmigu.cn

[Q23] 分页
来源：http://ia.jctech888.com.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://bk.yuntaijiaju.cn

[Q24] 去重
来源：http://iw.521024.cn

SELECT DISTINCT city FROM users;
来源：http://pv.asd995.cn

[Q25] 只取前 N 条
来源：http://zq.panjiajie.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://jm.newstarts.cn

[Q26] 计数
来源：http://dz.szxytkj.cn

SELECT COUNT(*) FROM users;
来源：http://hs.shxzukj.cn

[Q27] 条件计数
来源：http://qs.nicolike.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ww.newstarts.cn

[Q28] 求和与平均
来源：http://bs.hnjuh.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://zv.panjiajie.cn

[Q29] 最大最小值
来源：http://ef.yuntaijiaju.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://uk.yuexingan06.cn

[Q30] 分组统计
来源：http://fw.muxihuayi.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://zq.colortex.cn

[Q31] 分组后过滤
来源：http://ol.asd995.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://td.szsharing.cn

[Q32] 分组拼接字符串
来源：http://dk.muxihuayi.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://id.shxzukj.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://vu.jctech888.com.cn

[Q33] 多列分组
来源：http://eg.hnjuh.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ta.huanxung.cn

[Q34] 每组取第一条
来源：http://lh.huanxung.cn

SELECT * FROM (
来源：http://jn.szxytkj.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://sn.jctech888.com.cn

) t WHERE rn = 1;
来源：http://vv.szsharing.cn

[Q35] 内连接
来源：http://yr.521024.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mj.hahajie.cn

[Q36] 左连接
来源：http://vq.gzmigu.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://vk.wgjwhj.cn

[Q37] 右连接
来源：http://xh.jianghongdianzi.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://lm.panjiajie.cn

[Q38] 全外连接（PostgreSQL）
来源：http://ap.shtwfgs.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://uk.colortex.cn

[Q39] 自连接（查上下级）
来源：http://mv.lnxyls.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://wi.hahajie.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://it.bookmarksfly.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://bo.yuexingan06.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://fb.hnjuh.cn

[Q41] 多表连接
来源：http://nl.szxytkj.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://bg.newstarts.cn

JOIN users u ON u.id = o.user_id
来源：http://qo.hnjuh.cn

JOIN products p ON p.id = o.product_id;
来源：http://kz.szxytkj.cn

[Q42] 连接条件附加过滤
来源：http://uy.yuntaijiaju.cn

SELECT u.name, o.amount FROM users u
来源：http://mn.nicolike.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://lx.yuexingan06.cn

[Q43] 标量子查询
来源：http://hq.szxytkj.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://aa.huixinmuqiang.cn

[Q44] IN 子查询
来源：http://fm.colortex.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://fv.nicolike.cn

[Q45] EXISTS 判断存在
来源：http://bm.haigaiapp.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://pw.521024.cn

[Q46] NOT EXISTS 判断不存在
来源：http://yi.jianghongdianzi.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ml.szsharing.cn

[Q47] 与平均值比较
来源：http://lm.521024.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://kw.szsharing.cn

[Q48] CTE 公用表表达式
来源：http://qh.chemitech.net.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://sp.shtwfgs.cn

SELECT * FROM t WHERE c > 5;
来源：http://kp.szsharing.cn

[Q49] 更新单行
来源：http://uf.shtwfgs.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://sa.shxzukj.cn

[Q50] 批量更新
来源：http://tt.jctech888.com.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://ad.wgjwhj.cn

[Q51] 用子查询更新
来源：http://uc.haigaiapp.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://uy.muxihuayi.cn

[Q52] 删除指定行
来源：http://ae.huixinmuqiang.cn

DELETE FROM users WHERE id = 10;
来源：http://sx.bookmarksfly.cn

[Q53] 按条件删除
来源：http://wm.shxzskj.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://dl.chemitech.net.cn

[Q54] 清空表
来源：http://yi.colortex.cn

TRUNCATE TABLE logs;
来源：http://sc.yuexingan06.cn

[Q55] 排名（并列占位）
来源：http://ep.haigaiapp.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://gy.szsharing.cn

[Q56] 密集排名（并列不占位）
来源：http://nx.asd995.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://xp.jctech888.com.cn

[Q57] 行号
来源：http://aq.panjiajie.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://iu.huanxung.cn

[Q58] 累计求和
来源：http://lh.nszjky.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ia.bookmarksfly.cn

[Q59] 分组内累计
来源：http://po.szxytkj.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://yg.lnxyls.cn

[Q60] 取上一行 / 下一行
来源：http://fr.nszjky.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://jl.szsharing.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hw.bjjhwx.cn

[Q61] 移动平均
来源：http://hq.wgjwhj.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://yd.9csxet.cn

[Q62] 分组占比
来源：http://tz.huanxung.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://zn.panjiajie.cn

[Q63] 开启事务
来源：http://ms.szxytkj.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://xv.nszjky.cn

[Q64] 提交事务
来源：http://xx.szxytkj.cn

COMMIT;
来源：http://it.chemitech.net.cn

[Q65] 回滚事务
来源：http://bv.muxihuayi.cn

ROLLBACK;
来源：http://do.bookmarksfly.cn

[Q66] 行锁查询
来源：http://cq.lnxyls.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://zj.colortex.cn

[Q67] 设置隔离级别
来源：http://dq.colortex.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ah.muxihuayi.cn

[Q68] 保存点
来源：http://pi.shtwfgs.cn

SAVEPOINT sp1;
来源：http://ya.yuntaijiaju.cn

ROLLBACK TO sp1;
来源：http://oi.yuexingan06.cn

[Q69] 查看执行计划
来源：http://fa.hahajie.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ed.szsharing.cn

[Q70] 更新统计信息
来源：http://dt.yuexingan06.cn

ANALYZE TABLE users;
来源：http://mc.shtwfgs.cn

[Q71] 查看建表语句
来源：http://ez.huixiangedu.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mx.shxzskj.cn

[Q72] 查看索引
来源：http://ig.asd995.cn

SHOW INDEX FROM users;
来源：http://av.huixinmuqiang.cn

[Q73] 查看表状态
来源：http://lm.huixiangedu.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://ke.jianghongdianzi.cn

[Q74] 强制使用索引
来源：http://ah.9csxet.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://fh.gzmigu.cn

[Q75] 日期格式化
来源：http://fb.hnjuh.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://xe.bjjhwx.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wn.shxzskj.cn

[Q76] 按天统计
来源：http://nh.nszjky.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://fb.wgjwhj.cn

[Q77] 时间加减
来源：http://we.jctech888.com.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wi.colortex.cn

[Q78] 当前时间
来源：http://fj.panjiajie.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ag.szxytkj.cn

[Q79] 字符串拼接
来源：http://sp.newstarts.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://kt.huixinmuqiang.cn

[Q80] 字符串截取
来源：http://wn.hahajie.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://sn.nszjky.cn

[Q81] 字符串替换
来源：http://vf.521024.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ts.jctech888.com.cn

[Q82] 字符长度与字节长度
来源：http://bv.hnjuh.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://vh.asd995.cn

[Q83] 大小写转换
来源：http://tw.huanxung.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://yq.huixinmuqiang.cn

[Q84] 去除首尾空格
来源：http://zp.gzmigu.cn

SELECT TRIM(name) FROM users;
来源：http://lj.szsharing.cn

[Q85] 数值取整
来源：http://hg.muxihuayi.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://tr.lnxyls.cn

[Q86] 读取 JSON 字段
来源：http://wl.huanxung.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://qn.muxihuayi.cn

[Q87] JSON 字段做条件
来源：http://oe.9csxet.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://pe.bjjhwx.cn

[Q88] 行转列（条件聚合）
来源：http://tu.shxzukj.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ap.521024.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wp.wgjwhj.cn

[Q89] 判断表是否存在
来源：http://de.jianghongdianzi.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ho.bookmarksfly.cn

[Q90] 生成序号列
来源：http://if.shxzskj.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ec.gzmigu.cn

================================================================================
来源：http://md.huixiangedu.cn

R. Bash 专题
来源：http://wh.jianghongdianzi.cn

================================================================================
来源：http://zb.521024.cn

[R01] shebang 与严格模式
来源：http://yt.bjjhwx.cn

#!/usr/bin/env bash
来源：http://bo.521024.cn

set -euo pipefail
来源：http://mc.hahajie.cn

[R02] 变量赋值与使用
来源：http://tb.huixinmuqiang.cn

name="Tom"; echo "$name"
来源：http://st.szxytkj.cn

[R03] 只读变量
来源：http://bn.lnxyls.cn

readonly PI=3.14
来源：http://cm.gzmigu.cn

[R04] 位置参数
来源：http://dc.9csxet.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ph.szxytkj.cn

[R05] 参数默认值
来源：http://ee.haigaiapp.cn

name="${1:-default}"
来源：http://hg.jctech888.com.cn

[R06] 判断命令是否存在
来源：http://qj.nszjky.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://kr.shxzukj.cn

[R07] if 判断文件
来源：http://rt.huixiangedu.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ug.jianghongdianzi.cn

[R08] 数值比较
来源：http://dc.chemitech.net.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://tu.huixiangedu.cn

[R09] 字符串比较
来源：http://ak.jianghongdianzi.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://pl.jctech888.com.cn

[R10] 正则匹配
来源：http://px.bjjhwx.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://df.jianghongdianzi.cn

[R11] case 多分支
来源：http://ph.szsharing.cn

case "$1" in
来源：http://br.nszjky.cn

start) echo "启动" ;;
来源：http://hu.jianghongdianzi.cn

stop)  echo "停止" ;;
来源：http://sq.wgjwhj.cn

*)     echo "未知命令" ;;
来源：http://uu.gzmigu.cn

esac
来源：http://eg.shxzukj.cn

[R12] for 遍历文件
来源：http://im.newstarts.cn

for f in *.txt; do echo "$f"; done
来源：http://dp.wgjwhj.cn

[R13] for 计数循环
来源：http://hv.huixiangedu.cn

for i in {1..10}; do echo "$i"; done
来源：http://wm.hnjuh.cn

[R14] C 风格 for
来源：http://jh.jctech888.com.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ee.bookmarksfly.cn

[R15] while 逐行读文件
来源：http://hb.lnxyls.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://if.panjiajie.cn

[R16] until 等待条件
来源：http://wm.shxzukj.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://oy.szxytkj.cn

[R17] 数组定义与取值
来源：http://fa.9csxet.cn

arr=(a b c); echo "${arr[0]}"
来源：http://kd.nszjky.cn

[R18] 遍历数组
来源：http://xb.nszjky.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ix.bookmarksfly.cn

[R19] 数组长度
来源：http://bm.chemitech.net.cn

echo "${#arr[@]}"
来源：http://xn.9csxet.cn

[R20] 关联数组（字典）
来源：http://oj.521024.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://cq.bjjhwx.cn

[R21] 字符串长度
来源：http://au.yuexingan06.cn

echo "${#s}"
来源：http://gt.bookmarksfly.cn

[R22] 截取子串
来源：http://dw.huixiangedu.cn

echo "${s:0:5}"
来源：http://st.huanxung.cn

[R23] 字符串替换
来源：http://ay.haigaiapp.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ab.szxytkj.cn

[R24] 大小写转换
来源：http://pj.jctech888.com.cn

echo "${s^^}"; echo "${s,,}"
来源：http://kq.colortex.cn

[R25] 去后缀 / 去前缀
来源：http://sq.jianghongdianzi.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://cr.huanxung.cn

[R26] 命令替换
来源：http://ju.jctech888.com.cn

now=$(date +%F); echo "$now"
来源：http://um.yuntaijiaju.cn

[R27] 算术展开
来源：http://vh.521024.cn

echo $((1 + 2 * 3))
来源：http://eb.huixiangedu.cn

[R28] 浮点运算
来源：http://du.jianghongdianzi.cn

echo "scale=2; 10/3" | bc
来源：http://gj.shxzukj.cn

[R29] 定义函数
来源：http://tb.shtwfgs.cn


<!-- 参考信息 -->