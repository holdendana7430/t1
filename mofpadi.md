代发 wailian999

[P05] 判断两个对象内容是否相等
来源：http://md.panjiajie.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://cj.newstarts.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://tv.colortex.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://oi.nicolike.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://uv.shxzukj.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://jn.huanxung.cn

Go:   reflect.DeepEqual(a, b)
来源：http://no.haigaiapp.cn

Ruby: a == b
来源：http://ai.huixinmuqiang.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wp.huixiangedu.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://dx.newstarts.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://zd.hahajie.cn

PHP:  if (empty($x)) {}
来源：http://tf.chemitech.net.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://bp.huixiangedu.cn

TS:   if (x == null) {}
来源：http://gj.hnjuh.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://gc.lnxyls.cn

Go:   if x == nil {}
来源：http://si.gzmigu.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://st.huixinmuqiang.cn

C#:   if (x is null) {}
来源：http://yd.asd995.cn

[P07] 防抖与节流
来源：http://es.hahajie.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://gc.shxzukj.cn

PHP:  // 手写时间戳比较
来源：http://wu.gzmigu.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xp.shxzukj.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://jg.panjiajie.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mc.bookmarksfly.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://tu.chemitech.net.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://vn.huixinmuqiang.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://vu.huixinmuqiang.cn

[P08] 处理浮点精度问题
来源：http://qy.huanxung.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://of.nszjky.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://gu.bookmarksfly.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://sa.huixinmuqiang.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://bz.521024.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hs.shxzskj.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hc.shxzukj.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://xl.bjjhwx.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hh.asd995.cn

================================================================================
来源：http://rw.colortex.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://rj.szxytkj.cn

================================================================================
来源：http://vh.huanxung.cn

[Q01] 创建表
来源：http://av.nszjky.cn

CREATE TABLE users (
来源：http://lm.jctech888.com.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://rv.colortex.cn

name VARCHAR(50) NOT NULL,
来源：http://zr.szsharing.cn

email VARCHAR(100) UNIQUE,
来源：http://hg.asd995.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://qv.colortex.cn

);
来源：http://ux.muxihuayi.cn

[Q02] 创建带外键的表
来源：http://jz.gzmigu.cn

CREATE TABLE orders (
来源：http://do.wgjwhj.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ti.huixiangedu.cn

user_id INT NOT NULL,
来源：http://xe.asd995.cn

amount DECIMAL(10, 2),
来源：http://pk.huixinmuqiang.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://tx.panjiajie.cn

);
来源：http://zb.lnxyls.cn

[Q03] 增加列
来源：http://qo.nicolike.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://oe.hahajie.cn

[Q04] 修改列类型
来源：http://zt.bookmarksfly.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://zz.hnjuh.cn

[Q05] 重命名列
来源：http://dd.nszjky.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://qz.huanxung.cn

[Q06] 删除列
来源：http://ra.szxytkj.cn

ALTER TABLE users DROP COLUMN age;
来源：http://fm.yuntaijiaju.cn

[Q07] 删除表
来源：http://zu.chemitech.net.cn

DROP TABLE IF EXISTS orders;
来源：http://pl.hnjuh.cn

[Q08] 创建普通索引
来源：http://zf.shxzukj.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://mb.bookmarksfly.cn

[Q09] 创建唯一索引
来源：http://qa.hnjuh.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ud.lnxyls.cn

[Q10] 插入单行
来源：http://ul.jctech888.com.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://yw.huixinmuqiang.cn

[Q11] 一次插入多行
来源：http://bu.nszjky.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://up.szsharing.cn

[Q12] 插入后取自增 ID
来源：http://rn.gzmigu.cn

INSERT INTO users (name) VALUES ('C');
来源：http://na.chemitech.net.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://th.huixinmuqiang.cn

[Q13] 忽略重复插入
来源：http://yw.shxzskj.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ue.huixinmuqiang.cn

[Q14] 存在则更新（upsert）
来源：http://gw.chemitech.net.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://jr.szsharing.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://bz.9csxet.cn

[Q15] 查询全部
来源：http://uo.szxytkj.cn

SELECT * FROM users;
来源：http://bi.szxytkj.cn

[Q16] 查询指定列
来源：http://ps.newstarts.cn

SELECT id, name FROM users;
来源：http://yg.521024.cn

[Q17] 条件查询
来源：http://rx.gzmigu.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://xp.yuntaijiaju.cn

[Q18] 模糊匹配
来源：http://lu.521024.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://vr.colortex.cn

[Q19] 范围查询
来源：http://jv.panjiajie.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hi.huanxung.cn

[Q20] IN 列表
来源：http://qn.gzmigu.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://lv.huixinmuqiang.cn

[Q21] 空值判断
来源：http://iq.muxihuayi.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://ku.shxzskj.cn

[Q22] 排序
来源：http://ir.muxihuayi.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://tt.wgjwhj.cn

[Q23] 分页
来源：http://hj.szsharing.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ut.yuexingan06.cn

[Q24] 去重
来源：http://ay.chemitech.net.cn

SELECT DISTINCT city FROM users;
来源：http://kj.asd995.cn

[Q25] 只取前 N 条
来源：http://nq.szxytkj.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://zx.nicolike.cn

[Q26] 计数
来源：http://bt.nicolike.cn

SELECT COUNT(*) FROM users;
来源：http://ar.muxihuayi.cn

[Q27] 条件计数
来源：http://kf.panjiajie.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://rz.panjiajie.cn

[Q28] 求和与平均
来源：http://er.gzmigu.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://bi.huixiangedu.cn

[Q29] 最大最小值
来源：http://pl.asd995.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://og.newstarts.cn

[Q30] 分组统计
来源：http://bk.jianghongdianzi.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://xb.shxzskj.cn

[Q31] 分组后过滤
来源：http://yp.shxzukj.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://zs.colortex.cn

[Q32] 分组拼接字符串
来源：http://zb.yuexingan06.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://bk.jianghongdianzi.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://go.huixinmuqiang.cn

[Q33] 多列分组
来源：http://tq.shtwfgs.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://io.lnxyls.cn

[Q34] 每组取第一条
来源：http://ox.wgjwhj.cn

SELECT * FROM (
来源：http://el.huanxung.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mx.szsharing.cn

) t WHERE rn = 1;
来源：http://ny.huixinmuqiang.cn

[Q35] 内连接
来源：http://zj.panjiajie.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://zf.shxzskj.cn

[Q36] 左连接
来源：http://ne.nszjky.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://yq.jctech888.com.cn

[Q37] 右连接
来源：http://nr.shtwfgs.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ec.szsharing.cn

[Q38] 全外连接（PostgreSQL）
来源：http://ly.lnxyls.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://po.asd995.cn

[Q39] 自连接（查上下级）
来源：http://ej.yuntaijiaju.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://xw.panjiajie.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://my.9csxet.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://sn.shtwfgs.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hl.bjjhwx.cn

[Q41] 多表连接
来源：http://bn.521024.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://cg.wgjwhj.cn

JOIN users u ON u.id = o.user_id
来源：http://yj.hahajie.cn

JOIN products p ON p.id = o.product_id;
来源：http://wr.szsharing.cn

[Q42] 连接条件附加过滤
来源：http://xy.huixinmuqiang.cn

SELECT u.name, o.amount FROM users u
来源：http://hf.hahajie.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://qz.wgjwhj.cn

[Q43] 标量子查询
来源：http://ls.yuexingan06.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://le.bjjhwx.cn

[Q44] IN 子查询
来源：http://nt.huanxung.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ui.521024.cn

[Q45] EXISTS 判断存在
来源：http://jx.huixiangedu.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ra.shxzskj.cn

[Q46] NOT EXISTS 判断不存在
来源：http://dw.colortex.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://as.asd995.cn

[Q47] 与平均值比较
来源：http://gp.shxzukj.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://uk.9csxet.cn

[Q48] CTE 公用表表达式
来源：http://xe.haigaiapp.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://xv.huixiangedu.cn

SELECT * FROM t WHERE c > 5;
来源：http://ig.huixiangedu.cn

[Q49] 更新单行
来源：http://pi.colortex.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://jb.asd995.cn

[Q50] 批量更新
来源：http://lw.panjiajie.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://oh.shtwfgs.cn

[Q51] 用子查询更新
来源：http://hy.521024.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://yf.chemitech.net.cn

[Q52] 删除指定行
来源：http://wb.gzmigu.cn

DELETE FROM users WHERE id = 10;
来源：http://cg.huanxung.cn

[Q53] 按条件删除
来源：http://wd.huixinmuqiang.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://oj.nszjky.cn

[Q54] 清空表
来源：http://ch.yuntaijiaju.cn

TRUNCATE TABLE logs;
来源：http://nv.nicolike.cn

[Q55] 排名（并列占位）
来源：http://gr.szsharing.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://tc.shxzukj.cn

[Q56] 密集排名（并列不占位）
来源：http://sv.panjiajie.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://bi.panjiajie.cn

[Q57] 行号
来源：http://ul.huixinmuqiang.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://us.szsharing.cn

[Q58] 累计求和
来源：http://et.hahajie.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ms.huanxung.cn

[Q59] 分组内累计
来源：http://zy.bookmarksfly.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://pn.wgjwhj.cn

[Q60] 取上一行 / 下一行
来源：http://wl.lnxyls.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://od.szxytkj.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://lo.nszjky.cn

[Q61] 移动平均
来源：http://uk.asd995.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hr.shxzskj.cn

[Q62] 分组占比
来源：http://ow.szxytkj.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://jo.nicolike.cn

[Q63] 开启事务
来源：http://gi.muxihuayi.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://jx.shxzskj.cn

[Q64] 提交事务
来源：http://nc.hnjuh.cn

COMMIT;
来源：http://qq.lnxyls.cn

[Q65] 回滚事务
来源：http://zt.yuexingan06.cn

ROLLBACK;
来源：http://uz.huanxung.cn

[Q66] 行锁查询
来源：http://tk.panjiajie.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://lb.asd995.cn

[Q67] 设置隔离级别
来源：http://ig.nszjky.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://gy.hnjuh.cn

[Q68] 保存点
来源：http://yr.nicolike.cn

SAVEPOINT sp1;
来源：http://gz.nszjky.cn

ROLLBACK TO sp1;
来源：http://qn.yuntaijiaju.cn

[Q69] 查看执行计划
来源：http://jt.bjjhwx.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ap.wgjwhj.cn

[Q70] 更新统计信息
来源：http://tf.9csxet.cn

ANALYZE TABLE users;
来源：http://vw.szxytkj.cn

[Q71] 查看建表语句
来源：http://uh.hnjuh.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ue.huanxung.cn

[Q72] 查看索引
来源：http://df.asd995.cn

SHOW INDEX FROM users;
来源：http://bv.wgjwhj.cn

[Q73] 查看表状态
来源：http://ev.newstarts.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://dm.panjiajie.cn

[Q74] 强制使用索引
来源：http://ly.muxihuayi.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ij.huixinmuqiang.cn

[Q75] 日期格式化
来源：http://bv.hnjuh.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ny.hahajie.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://pm.colortex.cn

[Q76] 按天统计
来源：http://pp.jctech888.com.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://pw.hnjuh.cn

[Q77] 时间加减
来源：http://zl.gzmigu.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://kv.lnxyls.cn

[Q78] 当前时间
来源：http://rz.bjjhwx.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wa.gzmigu.cn

[Q79] 字符串拼接
来源：http://lh.nicolike.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://vs.huixinmuqiang.cn

[Q80] 字符串截取
来源：http://bs.newstarts.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ay.wgjwhj.cn

[Q81] 字符串替换
来源：http://fg.colortex.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://vh.nszjky.cn

[Q82] 字符长度与字节长度
来源：http://dc.nszjky.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://oj.nicolike.cn

[Q83] 大小写转换
来源：http://fe.newstarts.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://bq.bookmarksfly.cn

[Q84] 去除首尾空格
来源：http://vl.yuntaijiaju.cn

SELECT TRIM(name) FROM users;
来源：http://qj.521024.cn

[Q85] 数值取整
来源：http://vf.9csxet.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://nq.szsharing.cn

[Q86] 读取 JSON 字段
来源：http://ao.panjiajie.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://do.bjjhwx.cn

[Q87] JSON 字段做条件
来源：http://bw.nicolike.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://lf.jctech888.com.cn

[Q88] 行转列（条件聚合）
来源：http://ga.haigaiapp.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ev.9csxet.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ul.szsharing.cn

[Q89] 判断表是否存在
来源：http://uo.huixiangedu.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://gq.wgjwhj.cn

[Q90] 生成序号列
来源：http://ai.nszjky.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ee.huanxung.cn

================================================================================
来源：http://no.newstarts.cn

R. Bash 专题
来源：http://aq.nicolike.cn

================================================================================
来源：http://jo.shxzukj.cn

[R01] shebang 与严格模式
来源：http://rc.shtwfgs.cn

#!/usr/bin/env bash
来源：http://tg.yuexingan06.cn

set -euo pipefail
来源：http://bv.yuntaijiaju.cn

[R02] 变量赋值与使用
来源：http://wp.muxihuayi.cn

name="Tom"; echo "$name"
来源：http://cj.shtwfgs.cn

[R03] 只读变量
来源：http://yd.521024.cn

readonly PI=3.14
来源：http://ap.panjiajie.cn

[R04] 位置参数
来源：http://sb.9csxet.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://my.colortex.cn

[R05] 参数默认值
来源：http://qn.jctech888.com.cn

name="${1:-default}"
来源：http://mb.newstarts.cn

[R06] 判断命令是否存在
来源：http://io.szxytkj.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://gp.nicolike.cn

[R07] if 判断文件
来源：http://xt.panjiajie.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://jd.nszjky.cn

[R08] 数值比较
来源：http://jz.9csxet.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://ik.shxzukj.cn

[R09] 字符串比较
来源：http://eb.521024.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://af.yuexingan06.cn

[R10] 正则匹配
来源：http://jv.haigaiapp.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://fr.panjiajie.cn

[R11] case 多分支
来源：http://wh.9csxet.cn

case "$1" in
来源：http://pk.9csxet.cn

start) echo "启动" ;;
来源：http://cj.muxihuayi.cn

stop)  echo "停止" ;;
来源：http://vl.szsharing.cn

*)     echo "未知命令" ;;
来源：http://kf.gzmigu.cn

esac
来源：http://jz.huanxung.cn

[R12] for 遍历文件
来源：http://vx.colortex.cn

for f in *.txt; do echo "$f"; done
来源：http://sm.yuexingan06.cn

[R13] for 计数循环
来源：http://ad.9csxet.cn

for i in {1..10}; do echo "$i"; done
来源：http://ru.shxzukj.cn

[R14] C 风格 for
来源：http://pt.chemitech.net.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ve.hnjuh.cn

[R15] while 逐行读文件
来源：http://od.wgjwhj.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://zv.hnjuh.cn

[R16] until 等待条件
来源：http://gu.wgjwhj.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mc.shxzukj.cn

[R17] 数组定义与取值
来源：http://ib.521024.cn

arr=(a b c); echo "${arr[0]}"
来源：http://ms.jianghongdianzi.cn

[R18] 遍历数组
来源：http://wk.huanxung.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://lo.yuntaijiaju.cn

[R19] 数组长度
来源：http://ll.gzmigu.cn

echo "${#arr[@]}"
来源：http://uv.asd995.cn

[R20] 关联数组（字典）
来源：http://ia.jianghongdianzi.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wq.gzmigu.cn

[R21] 字符串长度
来源：http://bl.shtwfgs.cn

echo "${#s}"
来源：http://aj.jianghongdianzi.cn

[R22] 截取子串
来源：http://pv.chemitech.net.cn

echo "${s:0:5}"
来源：http://dp.shxzskj.cn

[R23] 字符串替换
来源：http://tb.jianghongdianzi.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://an.hahajie.cn

[R24] 大小写转换
来源：http://ls.521024.cn

echo "${s^^}"; echo "${s,,}"
来源：http://zb.jianghongdianzi.cn

[R25] 去后缀 / 去前缀
来源：http://ga.asd995.cn


<!-- 参考信息 -->