代发 wailian999

Java: list.size();  map.size();  s.length()
来源：http://bh.gzmigu.cn

Go:   len(arr);  len(m)
来源：http://ym.muxihuayi.cn

Ruby: x.length;  x.size
来源：http://gq.jianghongdianzi.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://ls.jianghongdianzi.cn

[P05] 判断两个对象内容是否相等
来源：http://ck.newstarts.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://dh.asd995.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wq.colortex.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://gp.hnjuh.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://vs.hnjuh.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ss.shtwfgs.cn

Go:   reflect.DeepEqual(a, b)
来源：http://zb.huixinmuqiang.cn

Ruby: a == b
来源：http://dr.shtwfgs.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://il.lnxyls.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://vz.shtwfgs.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ib.9csxet.cn

PHP:  if (empty($x)) {}
来源：http://bt.521024.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://xo.shtwfgs.cn

TS:   if (x == null) {}
来源：http://lk.521024.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://vi.panjiajie.cn

Go:   if x == nil {}
来源：http://ik.nszjky.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://zs.chemitech.net.cn

C#:   if (x is null) {}
来源：http://bm.shxzskj.cn

[P07] 防抖与节流
来源：http://cx.asd995.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://uh.bjjhwx.cn

PHP:  // 手写时间戳比较
来源：http://kv.jianghongdianzi.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ow.newstarts.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mg.bjjhwx.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ak.nszjky.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://da.huixiangedu.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://tp.lnxyls.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ni.nszjky.cn

[P08] 处理浮点精度问题
来源：http://vs.bjjhwx.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://et.bjjhwx.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://rp.huanxung.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://cx.shxzukj.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://bp.wgjwhj.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hn.szsharing.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://qh.panjiajie.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ff.colortex.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://st.panjiajie.cn

================================================================================
来源：http://yf.haigaiapp.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://bq.haigaiapp.cn

================================================================================
来源：http://ng.shxzukj.cn

[Q01] 创建表
来源：http://uz.shtwfgs.cn

CREATE TABLE users (
来源：http://jh.lnxyls.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ya.wgjwhj.cn

name VARCHAR(50) NOT NULL,
来源：http://re.bookmarksfly.cn

email VARCHAR(100) UNIQUE,
来源：http://dr.szxytkj.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mt.haigaiapp.cn

);
来源：http://ey.hahajie.cn

[Q02] 创建带外键的表
来源：http://ux.szsharing.cn

CREATE TABLE orders (
来源：http://sx.bjjhwx.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://vg.bjjhwx.cn

user_id INT NOT NULL,
来源：http://ss.szxytkj.cn

amount DECIMAL(10, 2),
来源：http://ys.jianghongdianzi.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://zz.jianghongdianzi.cn

);
来源：http://zi.shxzukj.cn

[Q03] 增加列
来源：http://eo.hahajie.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://xq.yuexingan06.cn

[Q04] 修改列类型
来源：http://db.yuexingan06.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://rt.panjiajie.cn

[Q05] 重命名列
来源：http://xg.newstarts.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://jk.panjiajie.cn

[Q06] 删除列
来源：http://cx.huanxung.cn

ALTER TABLE users DROP COLUMN age;
来源：http://se.chemitech.net.cn

[Q07] 删除表
来源：http://xv.hnjuh.cn

DROP TABLE IF EXISTS orders;
来源：http://wk.chemitech.net.cn

[Q08] 创建普通索引
来源：http://ct.newstarts.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://cn.hahajie.cn

[Q09] 创建唯一索引
来源：http://mc.shxzukj.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ef.shtwfgs.cn

[Q10] 插入单行
来源：http://ke.yuntaijiaju.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://so.lnxyls.cn

[Q11] 一次插入多行
来源：http://yg.gzmigu.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://yn.huixiangedu.cn

[Q12] 插入后取自增 ID
来源：http://zw.shxzukj.cn

INSERT INTO users (name) VALUES ('C');
来源：http://ei.chemitech.net.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://sb.huixiangedu.cn

[Q13] 忽略重复插入
来源：http://xq.panjiajie.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://vd.nszjky.cn

[Q14] 存在则更新（upsert）
来源：http://oo.shxzukj.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://xq.yuntaijiaju.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://qn.9csxet.cn

[Q15] 查询全部
来源：http://xe.panjiajie.cn

SELECT * FROM users;
来源：http://co.9csxet.cn

[Q16] 查询指定列
来源：http://qj.gzmigu.cn

SELECT id, name FROM users;
来源：http://ra.nicolike.cn

[Q17] 条件查询
来源：http://vp.wgjwhj.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://yu.huixiangedu.cn

[Q18] 模糊匹配
来源：http://ev.gzmigu.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hh.shxzukj.cn

[Q19] 范围查询
来源：http://od.shxzukj.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mb.521024.cn

[Q20] IN 列表
来源：http://tg.panjiajie.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://rp.szsharing.cn

[Q21] 空值判断
来源：http://cy.szsharing.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://pb.newstarts.cn

[Q22] 排序
来源：http://am.chemitech.net.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://uy.bjjhwx.cn

[Q23] 分页
来源：http://dz.bjjhwx.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://sl.newstarts.cn

[Q24] 去重
来源：http://sf.nszjky.cn

SELECT DISTINCT city FROM users;
来源：http://kz.yuntaijiaju.cn

[Q25] 只取前 N 条
来源：http://rd.huixinmuqiang.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://pc.nicolike.cn

[Q26] 计数
来源：http://zz.muxihuayi.cn

SELECT COUNT(*) FROM users;
来源：http://uh.yuntaijiaju.cn

[Q27] 条件计数
来源：http://wi.shxzskj.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://tw.jianghongdianzi.cn

[Q28] 求和与平均
来源：http://nw.hnjuh.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://tg.huixiangedu.cn

[Q29] 最大最小值
来源：http://mc.yuntaijiaju.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://zw.jctech888.com.cn

[Q30] 分组统计
来源：http://sz.521024.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://qq.jctech888.com.cn

[Q31] 分组后过滤
来源：http://sc.chemitech.net.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ia.szsharing.cn

[Q32] 分组拼接字符串
来源：http://md.bjjhwx.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://sy.panjiajie.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ul.chemitech.net.cn

[Q33] 多列分组
来源：http://fq.szsharing.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://kp.colortex.cn

[Q34] 每组取第一条
来源：http://rt.jctech888.com.cn

SELECT * FROM (
来源：http://rj.asd995.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://xy.asd995.cn

) t WHERE rn = 1;
来源：http://ze.521024.cn

[Q35] 内连接
来源：http://cv.colortex.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://tj.lnxyls.cn

[Q36] 左连接
来源：http://wd.huixinmuqiang.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://gp.szsharing.cn

[Q37] 右连接
来源：http://dv.yuntaijiaju.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://jo.lnxyls.cn

[Q38] 全外连接（PostgreSQL）
来源：http://vo.yuntaijiaju.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mm.521024.cn

[Q39] 自连接（查上下级）
来源：http://yz.szxytkj.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://we.wgjwhj.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://jj.chemitech.net.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://wd.huanxung.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://pc.lnxyls.cn

[Q41] 多表连接
来源：http://bd.bjjhwx.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://rm.bookmarksfly.cn

JOIN users u ON u.id = o.user_id
来源：http://nn.521024.cn

JOIN products p ON p.id = o.product_id;
来源：http://jh.jctech888.com.cn

[Q42] 连接条件附加过滤
来源：http://eh.wgjwhj.cn

SELECT u.name, o.amount FROM users u
来源：http://xk.huixinmuqiang.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ct.chemitech.net.cn

[Q43] 标量子查询
来源：http://bh.shtwfgs.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://fh.huixinmuqiang.cn

[Q44] IN 子查询
来源：http://uo.521024.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ic.bjjhwx.cn

[Q45] EXISTS 判断存在
来源：http://tv.colortex.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://fj.newstarts.cn

[Q46] NOT EXISTS 判断不存在
来源：http://pr.shxzskj.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://qr.chemitech.net.cn

[Q47] 与平均值比较
来源：http://bj.521024.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://es.huixinmuqiang.cn

[Q48] CTE 公用表表达式
来源：http://tr.bookmarksfly.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://um.shxzukj.cn

SELECT * FROM t WHERE c > 5;
来源：http://zg.lnxyls.cn

[Q49] 更新单行
来源：http://qf.szsharing.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://uk.muxihuayi.cn

[Q50] 批量更新
来源：http://kn.yuntaijiaju.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://dh.szxytkj.cn

[Q51] 用子查询更新
来源：http://im.huanxung.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://fz.chemitech.net.cn

[Q52] 删除指定行
来源：http://yh.gzmigu.cn

DELETE FROM users WHERE id = 10;
来源：http://pl.gzmigu.cn

[Q53] 按条件删除
来源：http://up.bookmarksfly.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://jp.9csxet.cn

[Q54] 清空表
来源：http://yn.521024.cn

TRUNCATE TABLE logs;
来源：http://in.haigaiapp.cn

[Q55] 排名（并列占位）
来源：http://hp.bjjhwx.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://tv.yuntaijiaju.cn

[Q56] 密集排名（并列不占位）
来源：http://jm.hnjuh.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://rj.asd995.cn

[Q57] 行号
来源：http://bx.huixiangedu.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://br.9csxet.cn

[Q58] 累计求和
来源：http://pi.hnjuh.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://nv.szsharing.cn

[Q59] 分组内累计
来源：http://gf.yuexingan06.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://fg.nicolike.cn

[Q60] 取上一行 / 下一行
来源：http://nf.huixinmuqiang.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ri.hahajie.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://eu.shxzskj.cn

[Q61] 移动平均
来源：http://ur.chemitech.net.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://lb.nszjky.cn

[Q62] 分组占比
来源：http://mr.gzmigu.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://cb.shtwfgs.cn

[Q63] 开启事务
来源：http://am.chemitech.net.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://fd.nicolike.cn

[Q64] 提交事务
来源：http://le.haigaiapp.cn

COMMIT;
来源：http://ob.colortex.cn

[Q65] 回滚事务
来源：http://in.yuntaijiaju.cn

ROLLBACK;
来源：http://gn.shxzukj.cn

[Q66] 行锁查询
来源：http://vg.bookmarksfly.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://jl.jctech888.com.cn

[Q67] 设置隔离级别
来源：http://mz.nszjky.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://cx.huixiangedu.cn

[Q68] 保存点
来源：http://yd.szxytkj.cn

SAVEPOINT sp1;
来源：http://fc.hnjuh.cn

ROLLBACK TO sp1;
来源：http://el.bjjhwx.cn

[Q69] 查看执行计划
来源：http://km.hnjuh.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://tu.nicolike.cn

[Q70] 更新统计信息
来源：http://xs.jctech888.com.cn

ANALYZE TABLE users;
来源：http://il.nicolike.cn

[Q71] 查看建表语句
来源：http://ob.haigaiapp.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ur.wgjwhj.cn

[Q72] 查看索引
来源：http://pu.wgjwhj.cn

SHOW INDEX FROM users;
来源：http://hl.wgjwhj.cn

[Q73] 查看表状态
来源：http://fb.panjiajie.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://il.9csxet.cn

[Q74] 强制使用索引
来源：http://nk.newstarts.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://rd.newstarts.cn

[Q75] 日期格式化
来源：http://gm.shxzukj.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://pe.panjiajie.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://sb.huixinmuqiang.cn

[Q76] 按天统计
来源：http://tz.shxzukj.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://tt.gzmigu.cn

[Q77] 时间加减
来源：http://lc.hahajie.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hc.chemitech.net.cn

[Q78] 当前时间
来源：http://hk.nszjky.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://un.9csxet.cn

[Q79] 字符串拼接
来源：http://fg.shtwfgs.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ni.huixiangedu.cn

[Q80] 字符串截取
来源：http://pk.haigaiapp.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://kg.bookmarksfly.cn

[Q81] 字符串替换
来源：http://iy.yuntaijiaju.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://pv.colortex.cn

[Q82] 字符长度与字节长度
来源：http://lp.huixiangedu.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://kv.bjjhwx.cn

[Q83] 大小写转换
来源：http://jl.haigaiapp.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://kd.hahajie.cn

[Q84] 去除首尾空格
来源：http://so.colortex.cn

SELECT TRIM(name) FROM users;
来源：http://ao.panjiajie.cn

[Q85] 数值取整
来源：http://yo.muxihuayi.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ni.bjjhwx.cn

[Q86] 读取 JSON 字段
来源：http://az.wgjwhj.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hv.shxzskj.cn

[Q87] JSON 字段做条件
来源：http://by.gzmigu.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ua.huixiangedu.cn

[Q88] 行转列（条件聚合）
来源：http://qn.shtwfgs.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://my.szxytkj.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://md.shxzukj.cn

[Q89] 判断表是否存在
来源：http://is.shtwfgs.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://zq.521024.cn

[Q90] 生成序号列
来源：http://ad.huixiangedu.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://jt.bjjhwx.cn

================================================================================
来源：http://ox.bookmarksfly.cn

R. Bash 专题
来源：http://je.shtwfgs.cn

================================================================================
来源：http://qt.yuexingan06.cn

[R01] shebang 与严格模式
来源：http://av.nszjky.cn

#!/usr/bin/env bash
来源：http://nw.lnxyls.cn

set -euo pipefail
来源：http://la.shtwfgs.cn

[R02] 变量赋值与使用
来源：http://uc.nicolike.cn

name="Tom"; echo "$name"
来源：http://nm.szxytkj.cn

[R03] 只读变量
来源：http://qu.shxzskj.cn

readonly PI=3.14
来源：http://wk.lnxyls.cn

[R04] 位置参数
来源：http://du.gzmigu.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://vf.521024.cn

[R05] 参数默认值
来源：http://bk.szsharing.cn

name="${1:-default}"
来源：http://zc.521024.cn

[R06] 判断命令是否存在
来源：http://oz.szsharing.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://jf.gzmigu.cn

[R07] if 判断文件
来源：http://bg.9csxet.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://kf.hahajie.cn

[R08] 数值比较
来源：http://ak.shtwfgs.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://qc.huixinmuqiang.cn

[R09] 字符串比较
来源：http://zp.colortex.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://oz.szsharing.cn

[R10] 正则匹配
来源：http://sr.szsharing.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wg.chemitech.net.cn

[R11] case 多分支
来源：http://th.shxzskj.cn

case "$1" in
来源：http://xd.newstarts.cn

start) echo "启动" ;;
来源：http://vc.huixiangedu.cn

stop)  echo "停止" ;;
来源：http://gi.521024.cn

*)     echo "未知命令" ;;
来源：http://zb.hnjuh.cn

esac
来源：http://mq.shxzukj.cn

[R12] for 遍历文件
来源：http://xu.panjiajie.cn

for f in *.txt; do echo "$f"; done
来源：http://bj.szxytkj.cn

[R13] for 计数循环
来源：http://kj.jianghongdianzi.cn

for i in {1..10}; do echo "$i"; done
来源：http://ew.newstarts.cn

[R14] C 风格 for
来源：http://zt.shxzukj.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ww.gzmigu.cn

[R15] while 逐行读文件
来源：http://ta.muxihuayi.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://xg.bookmarksfly.cn

[R16] until 等待条件
来源：http://im.nicolike.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ch.bookmarksfly.cn

[R17] 数组定义与取值
来源：http://ij.panjiajie.cn

arr=(a b c); echo "${arr[0]}"
来源：http://eq.lnxyls.cn

[R18] 遍历数组
来源：http://hl.shxzukj.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://cj.521024.cn

[R19] 数组长度
来源：http://tx.shtwfgs.cn

echo "${#arr[@]}"
来源：http://sh.shtwfgs.cn

[R20] 关联数组（字典）
来源：http://uw.szsharing.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://er.hahajie.cn

[R21] 字符串长度
来源：http://gw.muxihuayi.cn

echo "${#s}"
来源：http://xn.9csxet.cn

[R22] 截取子串
来源：http://xc.szxytkj.cn

echo "${s:0:5}"
来源：http://bv.lnxyls.cn

[R23] 字符串替换
来源：http://fp.yuexingan06.cn


<!-- 参考信息 -->