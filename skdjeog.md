代发 wailian999

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://jl.gzmigu.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://pn.nszjky.cn

Go:   reflect.DeepEqual(a, b)
来源：http://ux.shxzukj.cn

Ruby: a == b
来源：http://vp.wgjwhj.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://nc.asd995.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wn.9csxet.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://sm.szsharing.cn

PHP:  if (empty($x)) {}
来源：http://ox.shtwfgs.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hn.lnxyls.cn

TS:   if (x == null) {}
来源：http://mv.521024.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://qr.gzmigu.cn

Go:   if x == nil {}
来源：http://rs.haigaiapp.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://uv.szsharing.cn

C#:   if (x is null) {}
来源：http://nj.newstarts.cn

[P07] 防抖与节流
来源：http://jv.nicolike.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://xr.muxihuayi.cn

PHP:  // 手写时间戳比较
来源：http://is.nicolike.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://me.muxihuayi.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://zh.chemitech.net.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wh.yuntaijiaju.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://pc.hahajie.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://nu.colortex.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://xt.shxzskj.cn

[P08] 处理浮点精度问题
来源：http://id.nszjky.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://lo.yuexingan06.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://it.yuexingan06.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://az.jctech888.com.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://rg.panjiajie.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://kk.haigaiapp.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://fe.gzmigu.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://co.nszjky.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wx.huixinmuqiang.cn

================================================================================
来源：http://yx.nszjky.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ob.jctech888.com.cn

================================================================================
来源：http://dt.shxzukj.cn

[Q01] 创建表
来源：http://fx.colortex.cn

CREATE TABLE users (
来源：http://ki.panjiajie.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ym.wgjwhj.cn

name VARCHAR(50) NOT NULL,
来源：http://rc.jianghongdianzi.cn

email VARCHAR(100) UNIQUE,
来源：http://gi.szsharing.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ef.wgjwhj.cn

);
来源：http://tz.hahajie.cn

[Q02] 创建带外键的表
来源：http://mg.huixiangedu.cn

CREATE TABLE orders (
来源：http://de.huanxung.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wi.colortex.cn

user_id INT NOT NULL,
来源：http://op.jctech888.com.cn

amount DECIMAL(10, 2),
来源：http://rc.bjjhwx.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://yn.wgjwhj.cn

);
来源：http://mw.colortex.cn

[Q03] 增加列
来源：http://to.haigaiapp.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ym.bookmarksfly.cn

[Q04] 修改列类型
来源：http://sp.shtwfgs.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://xv.asd995.cn

[Q05] 重命名列
来源：http://cb.huixinmuqiang.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ww.9csxet.cn

[Q06] 删除列
来源：http://gs.yuntaijiaju.cn

ALTER TABLE users DROP COLUMN age;
来源：http://vb.hnjuh.cn

[Q07] 删除表
来源：http://wc.wgjwhj.cn

DROP TABLE IF EXISTS orders;
来源：http://bo.szsharing.cn

[Q08] 创建普通索引
来源：http://xp.shxzskj.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://lx.gzmigu.cn

[Q09] 创建唯一索引
来源：http://wn.muxihuayi.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ph.shxzukj.cn

[Q10] 插入单行
来源：http://cc.newstarts.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://kp.lnxyls.cn

[Q11] 一次插入多行
来源：http://mi.szxytkj.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ye.huixinmuqiang.cn

[Q12] 插入后取自增 ID
来源：http://jj.panjiajie.cn

INSERT INTO users (name) VALUES ('C');
来源：http://zw.yuexingan06.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://oj.yuntaijiaju.cn

[Q13] 忽略重复插入
来源：http://yp.jianghongdianzi.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://dg.szsharing.cn

[Q14] 存在则更新（upsert）
来源：http://kh.colortex.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://in.muxihuayi.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://jn.shxzukj.cn

[Q15] 查询全部
来源：http://vc.shxzukj.cn

SELECT * FROM users;
来源：http://un.shxzukj.cn

[Q16] 查询指定列
来源：http://cy.shxzskj.cn

SELECT id, name FROM users;
来源：http://jv.muxihuayi.cn

[Q17] 条件查询
来源：http://ww.newstarts.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ja.shxzukj.cn

[Q18] 模糊匹配
来源：http://ku.shxzukj.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://bd.shtwfgs.cn

[Q19] 范围查询
来源：http://lq.jctech888.com.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ez.521024.cn

[Q20] IN 列表
来源：http://lf.hnjuh.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ul.nszjky.cn

[Q21] 空值判断
来源：http://ij.bjjhwx.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://ly.muxihuayi.cn

[Q22] 排序
来源：http://jo.haigaiapp.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://iy.lnxyls.cn

[Q23] 分页
来源：http://fq.shxzukj.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://uy.chemitech.net.cn

[Q24] 去重
来源：http://cg.chemitech.net.cn

SELECT DISTINCT city FROM users;
来源：http://ph.szxytkj.cn

[Q25] 只取前 N 条
来源：http://bg.colortex.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://is.szsharing.cn

[Q26] 计数
来源：http://ei.shxzskj.cn

SELECT COUNT(*) FROM users;
来源：http://un.huanxung.cn

[Q27] 条件计数
来源：http://zv.bookmarksfly.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://fk.nszjky.cn

[Q28] 求和与平均
来源：http://ky.shxzukj.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://bi.haigaiapp.cn

[Q29] 最大最小值
来源：http://xs.huanxung.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://mq.haigaiapp.cn

[Q30] 分组统计
来源：http://wn.jctech888.com.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://gf.asd995.cn

[Q31] 分组后过滤
来源：http://kd.haigaiapp.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ka.yuexingan06.cn

[Q32] 分组拼接字符串
来源：http://gq.jianghongdianzi.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://bw.hahajie.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://lc.nicolike.cn

[Q33] 多列分组
来源：http://zw.9csxet.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://cd.shxzskj.cn

[Q34] 每组取第一条
来源：http://gg.shxzskj.cn

SELECT * FROM (
来源：http://op.haigaiapp.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://yj.shtwfgs.cn

) t WHERE rn = 1;
来源：http://kf.asd995.cn

[Q35] 内连接
来源：http://qc.shxzskj.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://bl.shxzukj.cn

[Q36] 左连接
来源：http://jl.szxytkj.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://yw.hahajie.cn

[Q37] 右连接
来源：http://jc.nszjky.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ig.huanxung.cn

[Q38] 全外连接（PostgreSQL）
来源：http://go.wgjwhj.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://gv.huanxung.cn

[Q39] 自连接（查上下级）
来源：http://cz.huixinmuqiang.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://zx.nszjky.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://vd.haigaiapp.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://tr.shtwfgs.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ck.bjjhwx.cn

[Q41] 多表连接
来源：http://qo.jctech888.com.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://xb.bjjhwx.cn

JOIN users u ON u.id = o.user_id
来源：http://um.huixiangedu.cn

JOIN products p ON p.id = o.product_id;
来源：http://ta.jianghongdianzi.cn

[Q42] 连接条件附加过滤
来源：http://cu.yuexingan06.cn

SELECT u.name, o.amount FROM users u
来源：http://qt.9csxet.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://gq.shtwfgs.cn

[Q43] 标量子查询
来源：http://ng.hnjuh.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://qe.colortex.cn

[Q44] IN 子查询
来源：http://xv.chemitech.net.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://yf.wgjwhj.cn

[Q45] EXISTS 判断存在
来源：http://mw.jctech888.com.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://dx.nicolike.cn

[Q46] NOT EXISTS 判断不存在
来源：http://ye.jianghongdianzi.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://kc.9csxet.cn

[Q47] 与平均值比较
来源：http://lm.jctech888.com.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://uf.shxzskj.cn

[Q48] CTE 公用表表达式
来源：http://aw.9csxet.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://vd.lnxyls.cn

SELECT * FROM t WHERE c > 5;
来源：http://ei.shtwfgs.cn

[Q49] 更新单行
来源：http://ln.shtwfgs.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ro.521024.cn

[Q50] 批量更新
来源：http://hl.521024.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://zz.muxihuayi.cn

[Q51] 用子查询更新
来源：http://my.wgjwhj.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://op.hahajie.cn

[Q52] 删除指定行
来源：http://qo.panjiajie.cn

DELETE FROM users WHERE id = 10;
来源：http://nb.jctech888.com.cn

[Q53] 按条件删除
来源：http://zr.shtwfgs.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hb.newstarts.cn

[Q54] 清空表
来源：http://nc.wgjwhj.cn

TRUNCATE TABLE logs;
来源：http://aj.szxytkj.cn

[Q55] 排名（并列占位）
来源：http://zb.szsharing.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ob.huixinmuqiang.cn

[Q56] 密集排名（并列不占位）
来源：http://pp.huanxung.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://au.wgjwhj.cn

[Q57] 行号
来源：http://ru.hnjuh.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://po.wgjwhj.cn

[Q58] 累计求和
来源：http://rw.jctech888.com.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://bt.jianghongdianzi.cn

[Q59] 分组内累计
来源：http://al.yuexingan06.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://sd.lnxyls.cn

[Q60] 取上一行 / 下一行
来源：http://mk.szsharing.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://qe.yuexingan06.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://xb.shxzskj.cn

[Q61] 移动平均
来源：http://pu.shxzukj.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ww.hahajie.cn

[Q62] 分组占比
来源：http://jb.huixinmuqiang.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hu.colortex.cn

[Q63] 开启事务
来源：http://db.hahajie.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://qw.hnjuh.cn

[Q64] 提交事务
来源：http://go.bookmarksfly.cn

COMMIT;
来源：http://gd.9csxet.cn

[Q65] 回滚事务
来源：http://er.muxihuayi.cn

ROLLBACK;
来源：http://oc.bjjhwx.cn

[Q66] 行锁查询
来源：http://zl.huixinmuqiang.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://lt.szxytkj.cn

[Q67] 设置隔离级别
来源：http://um.shxzskj.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ud.colortex.cn

[Q68] 保存点
来源：http://pw.szxytkj.cn

SAVEPOINT sp1;
来源：http://jg.szsharing.cn

ROLLBACK TO sp1;
来源：http://rj.jctech888.com.cn

[Q69] 查看执行计划
来源：http://rx.newstarts.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://af.hnjuh.cn

[Q70] 更新统计信息
来源：http://ul.nszjky.cn

ANALYZE TABLE users;
来源：http://uq.asd995.cn

[Q71] 查看建表语句
来源：http://bk.haigaiapp.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ou.huixiangedu.cn

[Q72] 查看索引
来源：http://ww.9csxet.cn

SHOW INDEX FROM users;
来源：http://pu.hahajie.cn

[Q73] 查看表状态
来源：http://bg.asd995.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://qm.521024.cn

[Q74] 强制使用索引
来源：http://rg.wgjwhj.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hj.521024.cn

[Q75] 日期格式化
来源：http://cb.haigaiapp.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hs.szsharing.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ok.jctech888.com.cn

[Q76] 按天统计
来源：http://jl.muxihuayi.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://rb.hnjuh.cn

[Q77] 时间加减
来源：http://bl.huixinmuqiang.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://rm.haigaiapp.cn

[Q78] 当前时间
来源：http://kv.szsharing.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://oo.nicolike.cn

[Q79] 字符串拼接
来源：http://or.panjiajie.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://bd.asd995.cn

[Q80] 字符串截取
来源：http://tr.huixinmuqiang.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://jg.newstarts.cn

[Q81] 字符串替换
来源：http://an.chemitech.net.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://qt.bjjhwx.cn

[Q82] 字符长度与字节长度
来源：http://ye.huanxung.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://xz.lnxyls.cn

[Q83] 大小写转换
来源：http://sl.panjiajie.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://md.nicolike.cn

[Q84] 去除首尾空格
来源：http://mv.jianghongdianzi.cn

SELECT TRIM(name) FROM users;
来源：http://gn.szsharing.cn

[Q85] 数值取整
来源：http://ii.jianghongdianzi.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://jo.shxzukj.cn

[Q86] 读取 JSON 字段
来源：http://jf.yuexingan06.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ge.colortex.cn

[Q87] JSON 字段做条件
来源：http://rd.hahajie.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ws.shxzukj.cn

[Q88] 行转列（条件聚合）
来源：http://di.muxihuayi.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://cb.521024.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://fq.gzmigu.cn

[Q89] 判断表是否存在
来源：http://yi.gzmigu.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://pw.huixinmuqiang.cn

[Q90] 生成序号列
来源：http://ru.szsharing.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://om.jctech888.com.cn

================================================================================
来源：http://om.panjiajie.cn

R. Bash 专题
来源：http://ig.newstarts.cn

================================================================================
来源：http://tc.shxzskj.cn

[R01] shebang 与严格模式
来源：http://go.yuexingan06.cn

#!/usr/bin/env bash
来源：http://tm.yuntaijiaju.cn

set -euo pipefail
来源：http://jf.panjiajie.cn

[R02] 变量赋值与使用
来源：http://wo.colortex.cn

name="Tom"; echo "$name"
来源：http://nr.chemitech.net.cn

[R03] 只读变量
来源：http://qj.lnxyls.cn

readonly PI=3.14
来源：http://xu.colortex.cn

[R04] 位置参数
来源：http://xu.shxzskj.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mc.bjjhwx.cn

[R05] 参数默认值
来源：http://yj.muxihuayi.cn

name="${1:-default}"
来源：http://yl.jctech888.com.cn

[R06] 判断命令是否存在
来源：http://hj.huixinmuqiang.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wi.muxihuayi.cn

[R07] if 判断文件
来源：http://hr.huixinmuqiang.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://qq.shxzukj.cn

[R08] 数值比较
来源：http://fg.jianghongdianzi.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://yj.chemitech.net.cn

[R09] 字符串比较
来源：http://uy.panjiajie.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://pw.nszjky.cn

[R10] 正则匹配
来源：http://rg.hnjuh.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://pl.hahajie.cn

[R11] case 多分支
来源：http://jn.yuexingan06.cn

case "$1" in
来源：http://zn.hnjuh.cn

start) echo "启动" ;;
来源：http://un.panjiajie.cn

stop)  echo "停止" ;;
来源：http://jj.haigaiapp.cn

*)     echo "未知命令" ;;
来源：http://bs.muxihuayi.cn

esac
来源：http://il.haigaiapp.cn

[R12] for 遍历文件
来源：http://ja.nicolike.cn

for f in *.txt; do echo "$f"; done
来源：http://og.jctech888.com.cn

[R13] for 计数循环
来源：http://yk.huixinmuqiang.cn

for i in {1..10}; do echo "$i"; done
来源：http://eh.chemitech.net.cn

[R14] C 风格 for
来源：http://sp.nszjky.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://us.yuntaijiaju.cn

[R15] while 逐行读文件
来源：http://sd.jianghongdianzi.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://xe.panjiajie.cn

[R16] until 等待条件
来源：http://nb.panjiajie.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://up.yuexingan06.cn

[R17] 数组定义与取值
来源：http://iu.colortex.cn

arr=(a b c); echo "${arr[0]}"
来源：http://pf.newstarts.cn

[R18] 遍历数组
来源：http://uj.bjjhwx.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://cf.bookmarksfly.cn

[R19] 数组长度
来源：http://mb.szxytkj.cn

echo "${#arr[@]}"
来源：http://lz.jctech888.com.cn

[R20] 关联数组（字典）
来源：http://kv.wgjwhj.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://so.jctech888.com.cn

[R21] 字符串长度
来源：http://aq.yuntaijiaju.cn

echo "${#s}"
来源：http://as.shtwfgs.cn

[R22] 截取子串
来源：http://dq.haigaiapp.cn

echo "${s:0:5}"
来源：http://og.szsharing.cn

[R23] 字符串替换
来源：http://jq.jianghongdianzi.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ba.shxzukj.cn

[R24] 大小写转换
来源：http://ij.bookmarksfly.cn

echo "${s^^}"; echo "${s,,}"
来源：http://bd.szsharing.cn

[R25] 去后缀 / 去前缀
来源：http://wz.wgjwhj.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://pe.9csxet.cn

[R26] 命令替换
来源：http://oy.bjjhwx.cn

now=$(date +%F); echo "$now"
来源：http://za.hnjuh.cn

[R27] 算术展开
来源：http://uc.nszjky.cn


<!-- 参考信息 -->