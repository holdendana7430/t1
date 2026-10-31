代发 wailian999

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://vt.muxihuayi.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://cz.lnxyls.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://pr.bjjhwx.cn

PHP:  if (empty($x)) {}
来源：http://cr.asd995.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ri.asd995.cn

TS:   if (x == null) {}
来源：http://nt.newstarts.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://wm.colortex.cn

Go:   if x == nil {}
来源：http://uc.hnjuh.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://oj.asd995.cn

C#:   if (x is null) {}
来源：http://sr.nicolike.cn

[P07] 防抖与节流
来源：http://ak.lnxyls.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://lw.shtwfgs.cn

PHP:  // 手写时间戳比较
来源：http://ho.shxzukj.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ow.521024.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://og.panjiajie.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://kc.panjiajie.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://zz.hahajie.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://kn.shtwfgs.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://et.nszjky.cn

[P08] 处理浮点精度问题
来源：http://zp.bookmarksfly.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://rh.huixiangedu.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ww.asd995.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hp.panjiajie.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ia.shtwfgs.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://qd.huanxung.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ur.9csxet.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ra.lnxyls.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://md.yuntaijiaju.cn

================================================================================
来源：http://iv.haigaiapp.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wx.jctech888.com.cn

================================================================================
来源：http://jg.colortex.cn

[Q01] 创建表
来源：http://sq.lnxyls.cn

CREATE TABLE users (
来源：http://so.huixiangedu.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://uq.521024.cn

name VARCHAR(50) NOT NULL,
来源：http://no.gzmigu.cn

email VARCHAR(100) UNIQUE,
来源：http://rk.muxihuayi.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://zw.szsharing.cn

);
来源：http://ma.colortex.cn

[Q02] 创建带外键的表
来源：http://ya.wgjwhj.cn

CREATE TABLE orders (
来源：http://ju.haigaiapp.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://bn.hahajie.cn

user_id INT NOT NULL,
来源：http://jt.jianghongdianzi.cn

amount DECIMAL(10, 2),
来源：http://nu.gzmigu.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://tl.9csxet.cn

);
来源：http://iy.huanxung.cn

[Q03] 增加列
来源：http://ng.panjiajie.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hy.panjiajie.cn

[Q04] 修改列类型
来源：http://ni.chemitech.net.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://gl.asd995.cn

[Q05] 重命名列
来源：http://ei.shxzskj.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ch.hnjuh.cn

[Q06] 删除列
来源：http://vu.shxzskj.cn

ALTER TABLE users DROP COLUMN age;
来源：http://xu.colortex.cn

[Q07] 删除表
来源：http://om.nszjky.cn

DROP TABLE IF EXISTS orders;
来源：http://wc.chemitech.net.cn

[Q08] 创建普通索引
来源：http://gn.asd995.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://gr.shxzukj.cn

[Q09] 创建唯一索引
来源：http://ws.521024.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://au.huixiangedu.cn

[Q10] 插入单行
来源：http://yd.bookmarksfly.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://kf.yuntaijiaju.cn

[Q11] 一次插入多行
来源：http://gt.gzmigu.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://jd.hahajie.cn

[Q12] 插入后取自增 ID
来源：http://uc.bookmarksfly.cn

INSERT INTO users (name) VALUES ('C');
来源：http://fw.hnjuh.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://pq.521024.cn

[Q13] 忽略重复插入
来源：http://rm.shxzskj.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://al.shtwfgs.cn

[Q14] 存在则更新（upsert）
来源：http://td.szsharing.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://pp.9csxet.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mu.asd995.cn

[Q15] 查询全部
来源：http://mw.huixiangedu.cn

SELECT * FROM users;
来源：http://tp.colortex.cn

[Q16] 查询指定列
来源：http://yw.yuexingan06.cn

SELECT id, name FROM users;
来源：http://by.gzmigu.cn

[Q17] 条件查询
来源：http://qh.wgjwhj.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://fi.muxihuayi.cn

[Q18] 模糊匹配
来源：http://hl.shxzukj.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://pw.szsharing.cn

[Q19] 范围查询
来源：http://pj.9csxet.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://rx.huixinmuqiang.cn

[Q20] IN 列表
来源：http://eq.wgjwhj.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://dw.wgjwhj.cn

[Q21] 空值判断
来源：http://wq.nicolike.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://md.shxzskj.cn

[Q22] 排序
来源：http://uv.szxytkj.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://aj.hnjuh.cn

[Q23] 分页
来源：http://fa.chemitech.net.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://jm.nicolike.cn

[Q24] 去重
来源：http://in.szxytkj.cn

SELECT DISTINCT city FROM users;
来源：http://uh.jctech888.com.cn

[Q25] 只取前 N 条
来源：http://fr.shtwfgs.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mz.nszjky.cn

[Q26] 计数
来源：http://bx.521024.cn

SELECT COUNT(*) FROM users;
来源：http://tj.huanxung.cn

[Q27] 条件计数
来源：http://rt.bjjhwx.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://gk.huixiangedu.cn

[Q28] 求和与平均
来源：http://it.shxzskj.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://xb.szsharing.cn

[Q29] 最大最小值
来源：http://qf.hahajie.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://sz.bjjhwx.cn

[Q30] 分组统计
来源：http://iu.huixinmuqiang.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://xd.chemitech.net.cn

[Q31] 分组后过滤
来源：http://qr.huanxung.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hc.shxzukj.cn

[Q32] 分组拼接字符串
来源：http://rb.shtwfgs.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://qw.chemitech.net.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hj.jctech888.com.cn

[Q33] 多列分组
来源：http://yo.521024.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://fs.panjiajie.cn

[Q34] 每组取第一条
来源：http://rk.nicolike.cn

SELECT * FROM (
来源：http://ug.lnxyls.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://rf.jctech888.com.cn

) t WHERE rn = 1;
来源：http://fu.hahajie.cn

[Q35] 内连接
来源：http://et.chemitech.net.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mv.521024.cn

[Q36] 左连接
来源：http://ol.huanxung.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ac.bjjhwx.cn

[Q37] 右连接
来源：http://wd.szxytkj.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ae.hahajie.cn

[Q38] 全外连接（PostgreSQL）
来源：http://wp.newstarts.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://oc.huixiangedu.cn

[Q39] 自连接（查上下级）
来源：http://ih.lnxyls.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://vb.shxzukj.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://lk.jianghongdianzi.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://mf.yuexingan06.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://yg.gzmigu.cn

[Q41] 多表连接
来源：http://qh.shxzskj.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://sr.hahajie.cn

JOIN users u ON u.id = o.user_id
来源：http://fg.nicolike.cn

JOIN products p ON p.id = o.product_id;
来源：http://ni.jianghongdianzi.cn

[Q42] 连接条件附加过滤
来源：http://ww.chemitech.net.cn

SELECT u.name, o.amount FROM users u
来源：http://tz.colortex.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://se.shxzukj.cn

[Q43] 标量子查询
来源：http://pj.yuntaijiaju.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://li.szsharing.cn

[Q44] IN 子查询
来源：http://lm.521024.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://qx.panjiajie.cn

[Q45] EXISTS 判断存在
来源：http://le.lnxyls.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://nu.yuexingan06.cn

[Q46] NOT EXISTS 判断不存在
来源：http://tv.bookmarksfly.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://bt.huixiangedu.cn

[Q47] 与平均值比较
来源：http://ab.huixiangedu.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mk.hnjuh.cn

[Q48] CTE 公用表表达式
来源：http://dj.shxzskj.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ma.shxzskj.cn

SELECT * FROM t WHERE c > 5;
来源：http://kw.bjjhwx.cn

[Q49] 更新单行
来源：http://sj.huanxung.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://zg.bjjhwx.cn

[Q50] 批量更新
来源：http://di.gzmigu.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://cr.szsharing.cn

[Q51] 用子查询更新
来源：http://nl.hahajie.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://zz.colortex.cn

[Q52] 删除指定行
来源：http://um.bookmarksfly.cn

DELETE FROM users WHERE id = 10;
来源：http://en.jianghongdianzi.cn

[Q53] 按条件删除
来源：http://oi.nicolike.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://nm.hahajie.cn

[Q54] 清空表
来源：http://jw.jctech888.com.cn

TRUNCATE TABLE logs;
来源：http://un.hahajie.cn

[Q55] 排名（并列占位）
来源：http://oy.nicolike.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://cm.colortex.cn

[Q56] 密集排名（并列不占位）
来源：http://oq.muxihuayi.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://qc.nszjky.cn

[Q57] 行号
来源：http://py.huanxung.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ad.huanxung.cn

[Q58] 累计求和
来源：http://hq.nicolike.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://fe.chemitech.net.cn

[Q59] 分组内累计
来源：http://wi.huanxung.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://rv.yuntaijiaju.cn

[Q60] 取上一行 / 下一行
来源：http://ru.bookmarksfly.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hv.jctech888.com.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://nz.hahajie.cn

[Q61] 移动平均
来源：http://bu.jctech888.com.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://il.chemitech.net.cn

[Q62] 分组占比
来源：http://xw.gzmigu.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ee.muxihuayi.cn

[Q63] 开启事务
来源：http://pu.bookmarksfly.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://rk.colortex.cn

[Q64] 提交事务
来源：http://pz.nicolike.cn

COMMIT;
来源：http://hp.yuexingan06.cn

[Q65] 回滚事务
来源：http://kv.521024.cn

ROLLBACK;
来源：http://hs.panjiajie.cn

[Q66] 行锁查询
来源：http://ic.yuexingan06.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://qk.colortex.cn

[Q67] 设置隔离级别
来源：http://ki.huixinmuqiang.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://po.szxytkj.cn

[Q68] 保存点
来源：http://yx.yuntaijiaju.cn

SAVEPOINT sp1;
来源：http://xb.haigaiapp.cn

ROLLBACK TO sp1;
来源：http://jd.muxihuayi.cn

[Q69] 查看执行计划
来源：http://qv.asd995.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://gw.yuexingan06.cn

[Q70] 更新统计信息
来源：http://wi.nszjky.cn

ANALYZE TABLE users;
来源：http://ur.yuexingan06.cn

[Q71] 查看建表语句
来源：http://ip.lnxyls.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://fc.muxihuayi.cn

[Q72] 查看索引
来源：http://wa.521024.cn

SHOW INDEX FROM users;
来源：http://gw.yuntaijiaju.cn

[Q73] 查看表状态
来源：http://ou.bjjhwx.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://gq.szxytkj.cn

[Q74] 强制使用索引
来源：http://to.newstarts.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ak.hnjuh.cn

[Q75] 日期格式化
来源：http://bh.nszjky.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ge.yuexingan06.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://sg.colortex.cn

[Q76] 按天统计
来源：http://mm.haigaiapp.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mi.szsharing.cn

[Q77] 时间加减
来源：http://rm.jianghongdianzi.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://yh.bjjhwx.cn

[Q78] 当前时间
来源：http://nx.shxzskj.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://cl.yuntaijiaju.cn

[Q79] 字符串拼接
来源：http://gh.yuntaijiaju.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://jl.nszjky.cn

[Q80] 字符串截取
来源：http://en.9csxet.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://zf.bjjhwx.cn

[Q81] 字符串替换
来源：http://rn.shxzskj.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://et.colortex.cn

[Q82] 字符长度与字节长度
来源：http://xb.yuntaijiaju.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://qu.yuntaijiaju.cn

[Q83] 大小写转换
来源：http://sc.hahajie.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://xd.asd995.cn

[Q84] 去除首尾空格
来源：http://ne.panjiajie.cn

SELECT TRIM(name) FROM users;
来源：http://ju.9csxet.cn

[Q85] 数值取整
来源：http://gd.nszjky.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mh.szsharing.cn

[Q86] 读取 JSON 字段
来源：http://go.asd995.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://nl.bookmarksfly.cn

[Q87] JSON 字段做条件
来源：http://ff.yuexingan06.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://cf.szxytkj.cn

[Q88] 行转列（条件聚合）
来源：http://rx.hnjuh.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ag.yuexingan06.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ch.9csxet.cn

[Q89] 判断表是否存在
来源：http://ci.shtwfgs.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://pm.szsharing.cn

[Q90] 生成序号列
来源：http://it.colortex.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://rp.bjjhwx.cn

================================================================================
来源：http://la.panjiajie.cn

R. Bash 专题
来源：http://si.521024.cn

================================================================================
来源：http://js.nszjky.cn

[R01] shebang 与严格模式
来源：http://ee.haigaiapp.cn

#!/usr/bin/env bash
来源：http://sm.lnxyls.cn

set -euo pipefail
来源：http://mm.bookmarksfly.cn

[R02] 变量赋值与使用
来源：http://jz.521024.cn

name="Tom"; echo "$name"
来源：http://ki.muxihuayi.cn

[R03] 只读变量
来源：http://bp.nszjky.cn

readonly PI=3.14
来源：http://vw.hnjuh.cn

[R04] 位置参数
来源：http://ca.wgjwhj.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hn.panjiajie.cn

[R05] 参数默认值
来源：http://yi.huanxung.cn

name="${1:-default}"
来源：http://pa.colortex.cn

[R06] 判断命令是否存在
来源：http://wn.hahajie.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://jm.huixinmuqiang.cn

[R07] if 判断文件
来源：http://ox.yuexingan06.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://qd.huixiangedu.cn

[R08] 数值比较
来源：http://fc.lnxyls.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://rm.huixiangedu.cn

[R09] 字符串比较
来源：http://ub.szsharing.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://zo.haigaiapp.cn

[R10] 正则匹配
来源：http://sr.wgjwhj.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://pj.lnxyls.cn

[R11] case 多分支
来源：http://oo.jianghongdianzi.cn

case "$1" in
来源：http://do.asd995.cn

start) echo "启动" ;;
来源：http://yc.hahajie.cn

stop)  echo "停止" ;;
来源：http://qo.chemitech.net.cn

*)     echo "未知命令" ;;
来源：http://lv.shtwfgs.cn

esac
来源：http://ps.newstarts.cn

[R12] for 遍历文件
来源：http://mx.szxytkj.cn

for f in *.txt; do echo "$f"; done
来源：http://jj.huixinmuqiang.cn

[R13] for 计数循环
来源：http://ro.9csxet.cn

for i in {1..10}; do echo "$i"; done
来源：http://it.muxihuayi.cn

[R14] C 风格 for
来源：http://vu.szxytkj.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://gs.haigaiapp.cn

[R15] while 逐行读文件
来源：http://yy.nszjky.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ko.muxihuayi.cn

[R16] until 等待条件
来源：http://zi.gzmigu.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://dn.nicolike.cn

[R17] 数组定义与取值
来源：http://lf.yuexingan06.cn

arr=(a b c); echo "${arr[0]}"
来源：http://au.panjiajie.cn

[R18] 遍历数组
来源：http://bg.shxzskj.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ic.huixiangedu.cn

[R19] 数组长度
来源：http://jz.shtwfgs.cn

echo "${#arr[@]}"
来源：http://yo.hnjuh.cn

[R20] 关联数组（字典）
来源：http://fu.wgjwhj.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://kg.nszjky.cn

[R21] 字符串长度
来源：http://zp.newstarts.cn

echo "${#s}"
来源：http://av.newstarts.cn

[R22] 截取子串
来源：http://eh.9csxet.cn

echo "${s:0:5}"
来源：http://zc.shtwfgs.cn

[R23] 字符串替换
来源：http://hj.shxzskj.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://yq.lnxyls.cn

[R24] 大小写转换
来源：http://td.nicolike.cn

echo "${s^^}"; echo "${s,,}"
来源：http://de.shxzskj.cn

[R25] 去后缀 / 去前缀
来源：http://wc.wgjwhj.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://mt.lnxyls.cn

[R26] 命令替换
来源：http://fv.muxihuayi.cn

now=$(date +%F); echo "$now"
来源：http://xb.jianghongdianzi.cn

[R27] 算术展开
来源：http://st.nszjky.cn

echo $((1 + 2 * 3))
来源：http://mz.chemitech.net.cn

[R28] 浮点运算
来源：http://jd.huixinmuqiang.cn

echo "scale=2; 10/3" | bc
来源：http://ct.521024.cn

[R29] 定义函数
来源：http://bg.9csxet.cn


<!-- 参考信息 -->