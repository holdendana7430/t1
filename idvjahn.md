代发 wailian999

Java: list.size();  map.size();  s.length()
来源：http://kq.521024.cn

Go:   len(arr);  len(m)
来源：http://vq.jctech888.com.cn

Ruby: x.length;  x.size
来源：http://xy.hnjuh.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://xj.muxihuayi.cn

[P05] 判断两个对象内容是否相等
来源：http://fy.521024.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://rs.colortex.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://me.nicolike.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://xp.panjiajie.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://vx.chemitech.net.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://bu.panjiajie.cn

Go:   reflect.DeepEqual(a, b)
来源：http://le.jianghongdianzi.cn

Ruby: a == b
来源：http://lj.shxzskj.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://uh.szsharing.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://rr.yuntaijiaju.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ns.szxytkj.cn

PHP:  if (empty($x)) {}
来源：http://cs.asd995.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ck.bjjhwx.cn

TS:   if (x == null) {}
来源：http://be.asd995.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://yt.newstarts.cn

Go:   if x == nil {}
来源：http://cy.9csxet.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hc.haigaiapp.cn

C#:   if (x is null) {}
来源：http://pf.521024.cn

[P07] 防抖与节流
来源：http://zn.wgjwhj.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://sf.gzmigu.cn

PHP:  // 手写时间戳比较
来源：http://ip.huixiangedu.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://gi.shtwfgs.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://lu.shxzskj.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://jc.gzmigu.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://jv.huanxung.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://it.wgjwhj.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mh.haigaiapp.cn

[P08] 处理浮点精度问题
来源：http://my.szxytkj.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://rr.shxzukj.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://zx.huanxung.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://tt.bjjhwx.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ls.haigaiapp.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ie.nszjky.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://sd.szxytkj.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://kc.haigaiapp.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://tv.szsharing.cn

================================================================================
来源：http://fa.shtwfgs.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://tw.521024.cn

================================================================================
来源：http://as.panjiajie.cn

[Q01] 创建表
来源：http://gg.newstarts.cn

CREATE TABLE users (
来源：http://zq.colortex.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ol.panjiajie.cn

name VARCHAR(50) NOT NULL,
来源：http://kk.newstarts.cn

email VARCHAR(100) UNIQUE,
来源：http://ev.yuntaijiaju.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://md.szsharing.cn

);
来源：http://yr.jianghongdianzi.cn

[Q02] 创建带外键的表
来源：http://zc.hahajie.cn

CREATE TABLE orders (
来源：http://fe.nszjky.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://eq.bookmarksfly.cn

user_id INT NOT NULL,
来源：http://mp.yuntaijiaju.cn

amount DECIMAL(10, 2),
来源：http://zf.hnjuh.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://iz.bjjhwx.cn

);
来源：http://pi.muxihuayi.cn

[Q03] 增加列
来源：http://gx.nszjky.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ob.szsharing.cn

[Q04] 修改列类型
来源：http://tm.nicolike.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mh.jianghongdianzi.cn

[Q05] 重命名列
来源：http://ry.szxytkj.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://bs.asd995.cn

[Q06] 删除列
来源：http://mb.nicolike.cn

ALTER TABLE users DROP COLUMN age;
来源：http://ol.shxzskj.cn

[Q07] 删除表
来源：http://gk.colortex.cn

DROP TABLE IF EXISTS orders;
来源：http://oc.huixiangedu.cn

[Q08] 创建普通索引
来源：http://pm.szsharing.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://kv.bjjhwx.cn

[Q09] 创建唯一索引
来源：http://xn.hnjuh.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mi.colortex.cn

[Q10] 插入单行
来源：http://fh.nicolike.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://fx.jctech888.com.cn

[Q11] 一次插入多行
来源：http://bc.huixinmuqiang.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://eq.colortex.cn

[Q12] 插入后取自增 ID
来源：http://ho.szsharing.cn

INSERT INTO users (name) VALUES ('C');
来源：http://om.chemitech.net.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://bf.9csxet.cn

[Q13] 忽略重复插入
来源：http://fu.haigaiapp.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://fi.9csxet.cn

[Q14] 存在则更新（upsert）
来源：http://cq.shxzukj.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://he.newstarts.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://za.shxzskj.cn

[Q15] 查询全部
来源：http://wr.newstarts.cn

SELECT * FROM users;
来源：http://hj.gzmigu.cn

[Q16] 查询指定列
来源：http://dh.shxzskj.cn

SELECT id, name FROM users;
来源：http://mn.nszjky.cn

[Q17] 条件查询
来源：http://pl.szsharing.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://lc.chemitech.net.cn

[Q18] 模糊匹配
来源：http://kb.bookmarksfly.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://tz.hahajie.cn

[Q19] 范围查询
来源：http://ye.asd995.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://uj.wgjwhj.cn

[Q20] IN 列表
来源：http://ed.hnjuh.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://th.shtwfgs.cn

[Q21] 空值判断
来源：http://ub.nszjky.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://zw.panjiajie.cn

[Q22] 排序
来源：http://ya.chemitech.net.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://vd.shxzskj.cn

[Q23] 分页
来源：http://mk.panjiajie.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hr.huanxung.cn

[Q24] 去重
来源：http://nm.shtwfgs.cn

SELECT DISTINCT city FROM users;
来源：http://ug.jianghongdianzi.cn

[Q25] 只取前 N 条
来源：http://dz.huixiangedu.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hl.nszjky.cn

[Q26] 计数
来源：http://gr.chemitech.net.cn

SELECT COUNT(*) FROM users;
来源：http://us.shtwfgs.cn

[Q27] 条件计数
来源：http://ym.hnjuh.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://vl.chemitech.net.cn

[Q28] 求和与平均
来源：http://jn.szxytkj.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://ye.newstarts.cn

[Q29] 最大最小值
来源：http://sc.szsharing.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://fh.yuntaijiaju.cn

[Q30] 分组统计
来源：http://bu.shtwfgs.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://zl.gzmigu.cn

[Q31] 分组后过滤
来源：http://se.shxzskj.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hh.gzmigu.cn

[Q32] 分组拼接字符串
来源：http://ja.huanxung.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://kq.nicolike.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mh.huixinmuqiang.cn

[Q33] 多列分组
来源：http://ar.bookmarksfly.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://bc.shtwfgs.cn

[Q34] 每组取第一条
来源：http://qo.gzmigu.cn

SELECT * FROM (
来源：http://vs.muxihuayi.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://bo.gzmigu.cn

) t WHERE rn = 1;
来源：http://fl.huanxung.cn

[Q35] 内连接
来源：http://lf.szxytkj.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://sb.huanxung.cn

[Q36] 左连接
来源：http://uo.shxzskj.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ve.panjiajie.cn

[Q37] 右连接
来源：http://qm.lnxyls.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://xb.haigaiapp.cn

[Q38] 全外连接（PostgreSQL）
来源：http://wd.nicolike.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://uz.521024.cn

[Q39] 自连接（查上下级）
来源：http://bi.shxzskj.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://fh.shtwfgs.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ow.521024.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://gb.yuexingan06.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://qn.chemitech.net.cn

[Q41] 多表连接
来源：http://ls.shtwfgs.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://mk.huixiangedu.cn

JOIN users u ON u.id = o.user_id
来源：http://dv.wgjwhj.cn

JOIN products p ON p.id = o.product_id;
来源：http://vt.shxzukj.cn

[Q42] 连接条件附加过滤
来源：http://zx.szxytkj.cn

SELECT u.name, o.amount FROM users u
来源：http://ed.asd995.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ow.szxytkj.cn

[Q43] 标量子查询
来源：http://rc.newstarts.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://vc.521024.cn

[Q44] IN 子查询
来源：http://kw.newstarts.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://jw.muxihuayi.cn

[Q45] EXISTS 判断存在
来源：http://pr.lnxyls.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://gi.muxihuayi.cn

[Q46] NOT EXISTS 判断不存在
来源：http://ea.lnxyls.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://zc.nszjky.cn

[Q47] 与平均值比较
来源：http://gw.shxzskj.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://pg.szsharing.cn

[Q48] CTE 公用表表达式
来源：http://da.shxzukj.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://zl.lnxyls.cn

SELECT * FROM t WHERE c > 5;
来源：http://ku.huixiangedu.cn

[Q49] 更新单行
来源：http://bf.muxihuayi.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://dw.huanxung.cn

[Q50] 批量更新
来源：http://xx.huanxung.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hc.szsharing.cn

[Q51] 用子查询更新
来源：http://dv.panjiajie.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wp.jctech888.com.cn

[Q52] 删除指定行
来源：http://yw.chemitech.net.cn

DELETE FROM users WHERE id = 10;
来源：http://qn.newstarts.cn

[Q53] 按条件删除
来源：http://nh.hahajie.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://vb.bjjhwx.cn

[Q54] 清空表
来源：http://nf.yuntaijiaju.cn

TRUNCATE TABLE logs;
来源：http://yb.jctech888.com.cn

[Q55] 排名（并列占位）
来源：http://sw.nszjky.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://fn.nszjky.cn

[Q56] 密集排名（并列不占位）
来源：http://an.huanxung.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ya.nicolike.cn

[Q57] 行号
来源：http://qb.chemitech.net.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ko.muxihuayi.cn

[Q58] 累计求和
来源：http://yk.wgjwhj.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hb.gzmigu.cn

[Q59] 分组内累计
来源：http://jp.shxzukj.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://kv.lnxyls.cn

[Q60] 取上一行 / 下一行
来源：http://rn.huanxung.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://od.9csxet.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hq.szsharing.cn

[Q61] 移动平均
来源：http://of.lnxyls.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://yz.bjjhwx.cn

[Q62] 分组占比
来源：http://qy.huixinmuqiang.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://xj.muxihuayi.cn

[Q63] 开启事务
来源：http://qg.nszjky.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://dn.bjjhwx.cn

[Q64] 提交事务
来源：http://sg.gzmigu.cn

COMMIT;
来源：http://wb.bookmarksfly.cn

[Q65] 回滚事务
来源：http://gn.lnxyls.cn

ROLLBACK;
来源：http://ip.yuexingan06.cn

[Q66] 行锁查询
来源：http://sp.wgjwhj.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://gj.hnjuh.cn

[Q67] 设置隔离级别
来源：http://sy.chemitech.net.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ix.jianghongdianzi.cn

[Q68] 保存点
来源：http://sn.yuexingan06.cn

SAVEPOINT sp1;
来源：http://we.bookmarksfly.cn

ROLLBACK TO sp1;
来源：http://er.gzmigu.cn

[Q69] 查看执行计划
来源：http://cc.huanxung.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://tt.colortex.cn

[Q70] 更新统计信息
来源：http://nv.shxzukj.cn

ANALYZE TABLE users;
来源：http://en.lnxyls.cn

[Q71] 查看建表语句
来源：http://fj.szxytkj.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://np.shtwfgs.cn

[Q72] 查看索引
来源：http://ei.haigaiapp.cn

SHOW INDEX FROM users;
来源：http://rk.panjiajie.cn

[Q73] 查看表状态
来源：http://hs.jctech888.com.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://mm.nszjky.cn

[Q74] 强制使用索引
来源：http://ao.huixinmuqiang.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://td.jctech888.com.cn

[Q75] 日期格式化
来源：http://pt.colortex.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://oo.panjiajie.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ul.huixiangedu.cn

[Q76] 按天统计
来源：http://ol.asd995.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mm.hahajie.cn

[Q77] 时间加减
来源：http://bj.huanxung.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://zv.shtwfgs.cn

[Q78] 当前时间
来源：http://ou.asd995.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ra.shxzskj.cn

[Q79] 字符串拼接
来源：http://hy.huixinmuqiang.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ic.nicolike.cn

[Q80] 字符串截取
来源：http://ya.szsharing.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://bl.huanxung.cn

[Q81] 字符串替换
来源：http://rs.huixinmuqiang.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://vi.nicolike.cn

[Q82] 字符长度与字节长度
来源：http://ol.521024.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hq.shxzukj.cn

[Q83] 大小写转换
来源：http://ch.chemitech.net.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ja.nicolike.cn

[Q84] 去除首尾空格
来源：http://yn.gzmigu.cn

SELECT TRIM(name) FROM users;
来源：http://ax.shxzskj.cn

[Q85] 数值取整
来源：http://wb.yuntaijiaju.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://az.shtwfgs.cn

[Q86] 读取 JSON 字段
来源：http://eu.asd995.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://qw.szsharing.cn

[Q87] JSON 字段做条件
来源：http://vb.huanxung.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ux.hnjuh.cn

[Q88] 行转列（条件聚合）
来源：http://rl.szsharing.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://no.huixiangedu.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://gm.huixiangedu.cn

[Q89] 判断表是否存在
来源：http://kt.muxihuayi.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://my.asd995.cn

[Q90] 生成序号列
来源：http://sk.panjiajie.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://pl.haigaiapp.cn

================================================================================
来源：http://gt.shxzskj.cn

R. Bash 专题
来源：http://rr.muxihuayi.cn

================================================================================
来源：http://tt.shxzskj.cn

[R01] shebang 与严格模式
来源：http://au.szxytkj.cn

#!/usr/bin/env bash
来源：http://jh.jctech888.com.cn

set -euo pipefail
来源：http://id.shxzskj.cn

[R02] 变量赋值与使用
来源：http://my.muxihuayi.cn

name="Tom"; echo "$name"
来源：http://xi.huanxung.cn

[R03] 只读变量
来源：http://ub.szsharing.cn

readonly PI=3.14
来源：http://sm.chemitech.net.cn

[R04] 位置参数
来源：http://eh.lnxyls.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mp.hnjuh.cn

[R05] 参数默认值
来源：http://hw.huanxung.cn

name="${1:-default}"
来源：http://mq.shxzukj.cn

[R06] 判断命令是否存在
来源：http://rp.huixiangedu.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://cb.szxytkj.cn

[R07] if 判断文件
来源：http://ac.shxzukj.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://jb.szsharing.cn

[R08] 数值比较
来源：http://ln.huanxung.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://hd.wgjwhj.cn

[R09] 字符串比较
来源：http://ci.huixinmuqiang.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://tj.9csxet.cn

[R10] 正则匹配
来源：http://uu.huanxung.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://us.chemitech.net.cn

[R11] case 多分支
来源：http://lj.bjjhwx.cn

case "$1" in
来源：http://rb.shtwfgs.cn

start) echo "启动" ;;
来源：http://qq.huanxung.cn

stop)  echo "停止" ;;
来源：http://cu.panjiajie.cn

*)     echo "未知命令" ;;
来源：http://ww.gzmigu.cn

esac
来源：http://tm.shxzskj.cn

[R12] for 遍历文件
来源：http://nr.huixiangedu.cn

for f in *.txt; do echo "$f"; done
来源：http://kh.521024.cn

[R13] for 计数循环
来源：http://vm.shtwfgs.cn

for i in {1..10}; do echo "$i"; done
来源：http://cz.shxzskj.cn

[R14] C 风格 for
来源：http://im.panjiajie.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://rg.nicolike.cn

[R15] while 逐行读文件
来源：http://kk.shtwfgs.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://kk.shxzskj.cn

[R16] until 等待条件
来源：http://gp.hnjuh.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://gl.hnjuh.cn

[R17] 数组定义与取值
来源：http://my.hahajie.cn

arr=(a b c); echo "${arr[0]}"
来源：http://le.yuexingan06.cn

[R18] 遍历数组
来源：http://qc.yuexingan06.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://zo.hnjuh.cn

[R19] 数组长度
来源：http://kl.wgjwhj.cn

echo "${#arr[@]}"
来源：http://eo.jianghongdianzi.cn

[R20] 关联数组（字典）
来源：http://qd.shxzskj.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://vl.haigaiapp.cn

[R21] 字符串长度
来源：http://gv.asd995.cn

echo "${#s}"
来源：http://co.newstarts.cn

[R22] 截取子串
来源：http://iz.yuexingan06.cn

echo "${s:0:5}"
来源：http://sb.huanxung.cn

[R23] 字符串替换
来源：http://xt.bookmarksfly.cn


<!-- 参考信息 -->