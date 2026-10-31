代发 wailian999

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://br.panjiajie.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://qm.nicolike.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://py.huixinmuqiang.cn

PHP:  if (empty($x)) {}
来源：http://it.chemitech.net.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ll.nicolike.cn

TS:   if (x == null) {}
来源：http://hp.nszjky.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://bo.521024.cn

Go:   if x == nil {}
来源：http://ks.wgjwhj.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ew.yuntaijiaju.cn

C#:   if (x is null) {}
来源：http://lx.521024.cn

[P07] 防抖与节流
来源：http://ly.lnxyls.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ab.bookmarksfly.cn

PHP:  // 手写时间戳比较
来源：http://ww.muxihuayi.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://yd.shxzskj.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://yf.huixiangedu.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://bv.jianghongdianzi.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://yb.newstarts.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://hn.shxzukj.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://bf.hnjuh.cn

[P08] 处理浮点精度问题
来源：http://yr.hahajie.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://aw.shxzukj.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://jz.jctech888.com.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://gv.asd995.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ox.jctech888.com.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ez.shxzukj.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://sg.huixiangedu.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ab.muxihuayi.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://jh.chemitech.net.cn

================================================================================
来源：http://es.nicolike.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://yf.521024.cn

================================================================================
来源：http://ce.521024.cn

[Q01] 创建表
来源：http://kt.yuntaijiaju.cn

CREATE TABLE users (
来源：http://pk.lnxyls.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://iq.hnjuh.cn

name VARCHAR(50) NOT NULL,
来源：http://jh.jctech888.com.cn

email VARCHAR(100) UNIQUE,
来源：http://pr.nszjky.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://yg.lnxyls.cn

);
来源：http://ho.521024.cn

[Q02] 创建带外键的表
来源：http://qr.panjiajie.cn

CREATE TABLE orders (
来源：http://qv.newstarts.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ip.muxihuayi.cn

user_id INT NOT NULL,
来源：http://fv.shtwfgs.cn

amount DECIMAL(10, 2),
来源：http://du.haigaiapp.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://yf.hnjuh.cn

);
来源：http://zo.newstarts.cn

[Q03] 增加列
来源：http://nk.szsharing.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://gz.hahajie.cn

[Q04] 修改列类型
来源：http://se.gzmigu.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://br.hahajie.cn

[Q05] 重命名列
来源：http://ip.hnjuh.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://su.shtwfgs.cn

[Q06] 删除列
来源：http://hc.shxzskj.cn

ALTER TABLE users DROP COLUMN age;
来源：http://ks.jctech888.com.cn

[Q07] 删除表
来源：http://ba.shxzukj.cn

DROP TABLE IF EXISTS orders;
来源：http://ko.lnxyls.cn

[Q08] 创建普通索引
来源：http://rf.panjiajie.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://dj.nicolike.cn

[Q09] 创建唯一索引
来源：http://jm.lnxyls.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://zn.asd995.cn

[Q10] 插入单行
来源：http://uu.szxytkj.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://nt.yuexingan06.cn

[Q11] 一次插入多行
来源：http://do.521024.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ey.newstarts.cn

[Q12] 插入后取自增 ID
来源：http://yg.huixiangedu.cn

INSERT INTO users (name) VALUES ('C');
来源：http://pi.muxihuayi.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://gj.shtwfgs.cn

[Q13] 忽略重复插入
来源：http://bq.bjjhwx.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ce.521024.cn

[Q14] 存在则更新（upsert）
来源：http://rq.panjiajie.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://sr.muxihuayi.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://fc.chemitech.net.cn

[Q15] 查询全部
来源：http://fy.lnxyls.cn

SELECT * FROM users;
来源：http://jm.newstarts.cn

[Q16] 查询指定列
来源：http://wp.panjiajie.cn

SELECT id, name FROM users;
来源：http://bm.shxzukj.cn

[Q17] 条件查询
来源：http://ev.gzmigu.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://bp.shtwfgs.cn

[Q18] 模糊匹配
来源：http://le.521024.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://qf.yuexingan06.cn

[Q19] 范围查询
来源：http://pp.asd995.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://xy.shxzskj.cn

[Q20] IN 列表
来源：http://sb.shxzukj.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://oc.hnjuh.cn

[Q21] 空值判断
来源：http://ns.nicolike.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://sf.lnxyls.cn

[Q22] 排序
来源：http://sg.hnjuh.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://vl.jianghongdianzi.cn

[Q23] 分页
来源：http://mm.huanxung.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ct.panjiajie.cn

[Q24] 去重
来源：http://ne.yuntaijiaju.cn

SELECT DISTINCT city FROM users;
来源：http://hk.huixiangedu.cn

[Q25] 只取前 N 条
来源：http://rk.yuntaijiaju.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://gh.shxzukj.cn

[Q26] 计数
来源：http://gv.haigaiapp.cn

SELECT COUNT(*) FROM users;
来源：http://ga.bjjhwx.cn

[Q27] 条件计数
来源：http://nc.nszjky.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://eg.haigaiapp.cn

[Q28] 求和与平均
来源：http://ih.szsharing.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://jq.lnxyls.cn

[Q29] 最大最小值
来源：http://lv.bookmarksfly.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://ce.nicolike.cn

[Q30] 分组统计
来源：http://uq.szsharing.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://dw.huanxung.cn

[Q31] 分组后过滤
来源：http://oq.nszjky.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://zf.shxzukj.cn

[Q32] 分组拼接字符串
来源：http://sr.newstarts.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://nq.szsharing.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://lj.huixinmuqiang.cn

[Q33] 多列分组
来源：http://wl.yuntaijiaju.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ms.bookmarksfly.cn

[Q34] 每组取第一条
来源：http://sf.newstarts.cn

SELECT * FROM (
来源：http://dm.gzmigu.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://fk.jctech888.com.cn

) t WHERE rn = 1;
来源：http://nn.chemitech.net.cn

[Q35] 内连接
来源：http://ll.newstarts.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://rm.wgjwhj.cn

[Q36] 左连接
来源：http://uk.jianghongdianzi.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://nb.lnxyls.cn

[Q37] 右连接
来源：http://cc.huixiangedu.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://lr.shxzukj.cn

[Q38] 全外连接（PostgreSQL）
来源：http://om.nicolike.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://am.lnxyls.cn

[Q39] 自连接（查上下级）
来源：http://ha.newstarts.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://xq.newstarts.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://fr.bjjhwx.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://bp.newstarts.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://nf.yuexingan06.cn

[Q41] 多表连接
来源：http://py.bookmarksfly.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://ea.panjiajie.cn

JOIN users u ON u.id = o.user_id
来源：http://kg.yuexingan06.cn

JOIN products p ON p.id = o.product_id;
来源：http://fi.yuntaijiaju.cn

[Q42] 连接条件附加过滤
来源：http://od.huixiangedu.cn

SELECT u.name, o.amount FROM users u
来源：http://rk.yuexingan06.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://xp.huixinmuqiang.cn

[Q43] 标量子查询
来源：http://av.jianghongdianzi.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://zf.huixinmuqiang.cn

[Q44] IN 子查询
来源：http://so.shtwfgs.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://pt.yuntaijiaju.cn

[Q45] EXISTS 判断存在
来源：http://nr.panjiajie.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mw.yuexingan06.cn

[Q46] NOT EXISTS 判断不存在
来源：http://jm.huanxung.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://td.yuexingan06.cn

[Q47] 与平均值比较
来源：http://kg.huixinmuqiang.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://fk.haigaiapp.cn

[Q48] CTE 公用表表达式
来源：http://lu.shxzukj.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://cm.huixiangedu.cn

SELECT * FROM t WHERE c > 5;
来源：http://wu.haigaiapp.cn

[Q49] 更新单行
来源：http://at.asd995.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://rx.wgjwhj.cn

[Q50] 批量更新
来源：http://up.colortex.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://lh.haigaiapp.cn

[Q51] 用子查询更新
来源：http://qi.szxytkj.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://jp.haigaiapp.cn

[Q52] 删除指定行
来源：http://yz.wgjwhj.cn

DELETE FROM users WHERE id = 10;
来源：http://ja.huanxung.cn

[Q53] 按条件删除
来源：http://ma.hnjuh.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://br.9csxet.cn

[Q54] 清空表
来源：http://kh.shxzskj.cn

TRUNCATE TABLE logs;
来源：http://gg.bjjhwx.cn

[Q55] 排名（并列占位）
来源：http://zs.shxzukj.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://dz.huanxung.cn

[Q56] 密集排名（并列不占位）
来源：http://tm.nicolike.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://nb.bookmarksfly.cn

[Q57] 行号
来源：http://gl.jianghongdianzi.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://po.nicolike.cn

[Q58] 累计求和
来源：http://ys.chemitech.net.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://bz.colortex.cn

[Q59] 分组内累计
来源：http://de.gzmigu.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://oo.shtwfgs.cn

[Q60] 取上一行 / 下一行
来源：http://qo.521024.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://dl.bjjhwx.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ip.szxytkj.cn

[Q61] 移动平均
来源：http://iq.yuexingan06.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://fd.panjiajie.cn

[Q62] 分组占比
来源：http://ap.newstarts.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://yn.bookmarksfly.cn

[Q63] 开启事务
来源：http://tf.nszjky.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://kq.shtwfgs.cn

[Q64] 提交事务
来源：http://jv.gzmigu.cn

COMMIT;
来源：http://ih.yuntaijiaju.cn

[Q65] 回滚事务
来源：http://ck.jctech888.com.cn

ROLLBACK;
来源：http://fv.jianghongdianzi.cn

[Q66] 行锁查询
来源：http://uj.chemitech.net.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ug.nszjky.cn

[Q67] 设置隔离级别
来源：http://bu.szxytkj.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://xp.hnjuh.cn

[Q68] 保存点
来源：http://bw.yuntaijiaju.cn

SAVEPOINT sp1;
来源：http://gu.panjiajie.cn

ROLLBACK TO sp1;
来源：http://hd.9csxet.cn

[Q69] 查看执行计划
来源：http://dy.asd995.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://cq.panjiajie.cn

[Q70] 更新统计信息
来源：http://hh.newstarts.cn

ANALYZE TABLE users;
来源：http://wy.shxzskj.cn

[Q71] 查看建表语句
来源：http://wf.yuexingan06.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hk.panjiajie.cn

[Q72] 查看索引
来源：http://ed.lnxyls.cn

SHOW INDEX FROM users;
来源：http://dr.newstarts.cn

[Q73] 查看表状态
来源：http://ho.gzmigu.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://oz.newstarts.cn

[Q74] 强制使用索引
来源：http://ie.521024.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ps.yuntaijiaju.cn

[Q75] 日期格式化
来源：http://od.chemitech.net.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ff.hnjuh.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://fa.wgjwhj.cn

[Q76] 按天统计
来源：http://hd.shxzukj.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://rn.muxihuayi.cn

[Q77] 时间加减
来源：http://db.yuexingan06.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://xc.muxihuayi.cn

[Q78] 当前时间
来源：http://xg.yuexingan06.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://yn.haigaiapp.cn

[Q79] 字符串拼接
来源：http://xa.colortex.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://xf.nszjky.cn

[Q80] 字符串截取
来源：http://ep.lnxyls.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://se.bookmarksfly.cn

[Q81] 字符串替换
来源：http://ex.yuntaijiaju.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://oz.huixinmuqiang.cn

[Q82] 字符长度与字节长度
来源：http://xr.panjiajie.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ch.muxihuayi.cn

[Q83] 大小写转换
来源：http://cj.panjiajie.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://jw.bookmarksfly.cn

[Q84] 去除首尾空格
来源：http://su.szsharing.cn

SELECT TRIM(name) FROM users;
来源：http://hn.muxihuayi.cn

[Q85] 数值取整
来源：http://cd.9csxet.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ih.colortex.cn

[Q86] 读取 JSON 字段
来源：http://cw.asd995.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://uu.shtwfgs.cn

[Q87] JSON 字段做条件
来源：http://ut.jctech888.com.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://se.hnjuh.cn

[Q88] 行转列（条件聚合）
来源：http://cl.shtwfgs.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wc.muxihuayi.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://dm.nicolike.cn

[Q89] 判断表是否存在
来源：http://hv.hnjuh.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://jt.panjiajie.cn

[Q90] 生成序号列
来源：http://cv.bjjhwx.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://zv.huanxung.cn

================================================================================
来源：http://rs.shxzukj.cn

R. Bash 专题
来源：http://zb.nicolike.cn

================================================================================
来源：http://nt.bjjhwx.cn

[R01] shebang 与严格模式
来源：http://ib.shtwfgs.cn

#!/usr/bin/env bash
来源：http://mu.haigaiapp.cn

set -euo pipefail
来源：http://ya.bookmarksfly.cn

[R02] 变量赋值与使用
来源：http://pg.newstarts.cn

name="Tom"; echo "$name"
来源：http://ca.shxzukj.cn

[R03] 只读变量
来源：http://ny.colortex.cn

readonly PI=3.14
来源：http://di.panjiajie.cn

[R04] 位置参数
来源：http://ro.jctech888.com.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://cr.asd995.cn

[R05] 参数默认值
来源：http://ek.panjiajie.cn

name="${1:-default}"
来源：http://ul.bookmarksfly.cn

[R06] 判断命令是否存在
来源：http://ch.9csxet.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://sj.newstarts.cn

[R07] if 判断文件
来源：http://dq.asd995.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://qx.wgjwhj.cn

[R08] 数值比较
来源：http://fv.haigaiapp.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://ys.hahajie.cn

[R09] 字符串比较
来源：http://sy.haigaiapp.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://zq.hahajie.cn

[R10] 正则匹配
来源：http://en.asd995.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://xz.bjjhwx.cn

[R11] case 多分支
来源：http://ij.nszjky.cn

case "$1" in
来源：http://dk.newstarts.cn

start) echo "启动" ;;
来源：http://bn.shxzskj.cn

stop)  echo "停止" ;;
来源：http://ex.huixiangedu.cn

*)     echo "未知命令" ;;
来源：http://xr.9csxet.cn

esac
来源：http://hm.bookmarksfly.cn

[R12] for 遍历文件
来源：http://cp.hnjuh.cn

for f in *.txt; do echo "$f"; done
来源：http://mj.huixiangedu.cn

[R13] for 计数循环
来源：http://wt.asd995.cn

for i in {1..10}; do echo "$i"; done
来源：http://tr.nszjky.cn

[R14] C 风格 for
来源：http://uh.chemitech.net.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://gd.jctech888.com.cn

[R15] while 逐行读文件
来源：http://mm.shtwfgs.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hr.hnjuh.cn

[R16] until 等待条件
来源：http://yt.lnxyls.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://qe.nicolike.cn

[R17] 数组定义与取值
来源：http://xb.colortex.cn

arr=(a b c); echo "${arr[0]}"
来源：http://wx.panjiajie.cn

[R18] 遍历数组
来源：http://ll.chemitech.net.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://bz.newstarts.cn

[R19] 数组长度
来源：http://yw.muxihuayi.cn

echo "${#arr[@]}"
来源：http://ly.hahajie.cn

[R20] 关联数组（字典）
来源：http://vs.haigaiapp.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://rw.bjjhwx.cn

[R21] 字符串长度
来源：http://pr.chemitech.net.cn

echo "${#s}"
来源：http://bb.jctech888.com.cn

[R22] 截取子串
来源：http://fm.bjjhwx.cn

echo "${s:0:5}"
来源：http://eu.9csxet.cn

[R23] 字符串替换
来源：http://bw.gzmigu.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://qn.shxzukj.cn

[R24] 大小写转换
来源：http://xb.521024.cn

echo "${s^^}"; echo "${s,,}"
来源：http://vq.521024.cn

[R25] 去后缀 / 去前缀
来源：http://xv.bjjhwx.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://ng.haigaiapp.cn

[R26] 命令替换
来源：http://xu.yuntaijiaju.cn

now=$(date +%F); echo "$now"
来源：http://mm.panjiajie.cn

[R27] 算术展开
来源：http://iy.bookmarksfly.cn

echo $((1 + 2 * 3))
来源：http://zz.shtwfgs.cn

[R28] 浮点运算
来源：http://ho.haigaiapp.cn

echo "scale=2; 10/3" | bc
来源：http://qz.lnxyls.cn

[R29] 定义函数
来源：http://xd.haigaiapp.cn


<!-- 参考信息 -->