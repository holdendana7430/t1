代发 wailian999

Java: list.size();  map.size();  s.length()
来源：http://ha.bjjhwx.cn

Go:   len(arr);  len(m)
来源：http://ob.yuexingan06.cn

Ruby: x.length;  x.size
来源：http://mz.huixinmuqiang.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://lk.nszjky.cn

[P05] 判断两个对象内容是否相等
来源：http://qd.lnxyls.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://jm.9csxet.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ga.muxihuayi.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://rc.lnxyls.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://fw.yuntaijiaju.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://nc.bookmarksfly.cn

Go:   reflect.DeepEqual(a, b)
来源：http://mo.newstarts.cn

Ruby: a == b
来源：http://gt.panjiajie.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://cf.szsharing.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mo.shtwfgs.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://gm.lnxyls.cn

PHP:  if (empty($x)) {}
来源：http://kd.bookmarksfly.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ot.huixiangedu.cn

TS:   if (x == null) {}
来源：http://sj.newstarts.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://zy.huanxung.cn

Go:   if x == nil {}
来源：http://sh.huixiangedu.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ni.colortex.cn

C#:   if (x is null) {}
来源：http://gr.huixinmuqiang.cn

[P07] 防抖与节流
来源：http://ug.colortex.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://um.521024.cn

PHP:  // 手写时间戳比较
来源：http://kj.haigaiapp.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ry.shxzukj.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://sx.szsharing.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://za.521024.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://uu.wgjwhj.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://fa.hnjuh.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://kv.newstarts.cn

[P08] 处理浮点精度问题
来源：http://in.bookmarksfly.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://rv.shxzukj.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://rs.nszjky.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://nc.521024.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ge.521024.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://qm.newstarts.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://cu.colortex.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ol.hahajie.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://yk.huixinmuqiang.cn

================================================================================
来源：http://th.jctech888.com.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mc.szsharing.cn

================================================================================
来源：http://wk.nicolike.cn

[Q01] 创建表
来源：http://lv.nicolike.cn

CREATE TABLE users (
来源：http://lq.9csxet.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ar.hnjuh.cn

name VARCHAR(50) NOT NULL,
来源：http://cp.gzmigu.cn

email VARCHAR(100) UNIQUE,
来源：http://yl.lnxyls.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://qn.nszjky.cn

);
来源：http://zh.hnjuh.cn

[Q02] 创建带外键的表
来源：http://ou.muxihuayi.cn

CREATE TABLE orders (
来源：http://yi.huixiangedu.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://xv.yuntaijiaju.cn

user_id INT NOT NULL,
来源：http://cl.szsharing.cn

amount DECIMAL(10, 2),
来源：http://lc.jctech888.com.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mw.jianghongdianzi.cn

);
来源：http://rz.jianghongdianzi.cn

[Q03] 增加列
来源：http://kc.gzmigu.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://dg.wgjwhj.cn

[Q04] 修改列类型
来源：http://dq.chemitech.net.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://sd.gzmigu.cn

[Q05] 重命名列
来源：http://ro.newstarts.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://zq.bjjhwx.cn

[Q06] 删除列
来源：http://hi.muxihuayi.cn

ALTER TABLE users DROP COLUMN age;
来源：http://nj.nszjky.cn

[Q07] 删除表
来源：http://ky.muxihuayi.cn

DROP TABLE IF EXISTS orders;
来源：http://xn.nszjky.cn

[Q08] 创建普通索引
来源：http://it.szsharing.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.hahajie.cn

[Q09] 创建唯一索引
来源：http://ti.yuexingan06.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://qf.muxihuayi.cn

[Q10] 插入单行
来源：http://cc.yuntaijiaju.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://da.shtwfgs.cn

[Q11] 一次插入多行
来源：http://zn.9csxet.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://bb.colortex.cn

[Q12] 插入后取自增 ID
来源：http://hl.jctech888.com.cn

INSERT INTO users (name) VALUES ('C');
来源：http://tf.hahajie.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://da.huanxung.cn

[Q13] 忽略重复插入
来源：http://wi.nszjky.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://do.nszjky.cn

[Q14] 存在则更新（upsert）
来源：http://ld.huixiangedu.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mc.colortex.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://fq.huixiangedu.cn

[Q15] 查询全部
来源：http://rt.huixinmuqiang.cn

SELECT * FROM users;
来源：http://yh.nicolike.cn

[Q16] 查询指定列
来源：http://bw.gzmigu.cn

SELECT id, name FROM users;
来源：http://rx.huixiangedu.cn

[Q17] 条件查询
来源：http://ea.521024.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://fk.szsharing.cn

[Q18] 模糊匹配
来源：http://uj.muxihuayi.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://am.szsharing.cn

[Q19] 范围查询
来源：http://me.hahajie.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://re.nicolike.cn

[Q20] IN 列表
来源：http://ee.hahajie.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://vl.muxihuayi.cn

[Q21] 空值判断
来源：http://vo.huixiangedu.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://xt.hnjuh.cn

[Q22] 排序
来源：http://tk.9csxet.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://il.huixiangedu.cn

[Q23] 分页
来源：http://vq.colortex.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://jk.shxzskj.cn

[Q24] 去重
来源：http://su.szsharing.cn

SELECT DISTINCT city FROM users;
来源：http://oc.hahajie.cn

[Q25] 只取前 N 条
来源：http://wi.huanxung.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://id.nicolike.cn

[Q26] 计数
来源：http://sh.hnjuh.cn

SELECT COUNT(*) FROM users;
来源：http://jq.bjjhwx.cn

[Q27] 条件计数
来源：http://tz.lnxyls.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://bx.haigaiapp.cn

[Q28] 求和与平均
来源：http://gs.shxzukj.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://er.szsharing.cn

[Q29] 最大最小值
来源：http://cm.shtwfgs.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://xl.chemitech.net.cn

[Q30] 分组统计
来源：http://jf.panjiajie.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ov.panjiajie.cn

[Q31] 分组后过滤
来源：http://rj.wgjwhj.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ma.panjiajie.cn

[Q32] 分组拼接字符串
来源：http://aj.yuntaijiaju.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://fb.chemitech.net.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://qu.newstarts.cn

[Q33] 多列分组
来源：http://xj.jianghongdianzi.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://es.gzmigu.cn

[Q34] 每组取第一条
来源：http://iq.shtwfgs.cn

SELECT * FROM (
来源：http://hw.jctech888.com.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hs.huixinmuqiang.cn

) t WHERE rn = 1;
来源：http://pk.muxihuayi.cn

[Q35] 内连接
来源：http://cn.chemitech.net.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hj.szsharing.cn

[Q36] 左连接
来源：http://uu.chemitech.net.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ns.nicolike.cn

[Q37] 右连接
来源：http://mn.szxytkj.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://dx.bookmarksfly.cn

[Q38] 全外连接（PostgreSQL）
来源：http://za.colortex.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://nr.nszjky.cn

[Q39] 自连接（查上下级）
来源：http://qn.haigaiapp.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://nb.521024.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://uc.shtwfgs.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://ug.szsharing.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ma.bjjhwx.cn

[Q41] 多表连接
来源：http://jb.hahajie.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://bh.muxihuayi.cn

JOIN users u ON u.id = o.user_id
来源：http://cq.gzmigu.cn

JOIN products p ON p.id = o.product_id;
来源：http://yk.9csxet.cn

[Q42] 连接条件附加过滤
来源：http://za.huanxung.cn

SELECT u.name, o.amount FROM users u
来源：http://gf.yuexingan06.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://vi.shxzukj.cn

[Q43] 标量子查询
来源：http://hr.shxzukj.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://fc.wgjwhj.cn

[Q44] IN 子查询
来源：http://vj.haigaiapp.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wc.shtwfgs.cn

[Q45] EXISTS 判断存在
来源：http://si.asd995.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hs.panjiajie.cn

[Q46] NOT EXISTS 判断不存在
来源：http://uz.muxihuayi.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ul.bjjhwx.cn

[Q47] 与平均值比较
来源：http://zv.yuntaijiaju.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://de.huanxung.cn

[Q48] CTE 公用表表达式
来源：http://ua.gzmigu.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://az.szsharing.cn

SELECT * FROM t WHERE c > 5;
来源：http://tc.yuexingan06.cn

[Q49] 更新单行
来源：http://fy.nszjky.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://dp.haigaiapp.cn

[Q50] 批量更新
来源：http://uu.newstarts.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://gm.yuexingan06.cn

[Q51] 用子查询更新
来源：http://wv.lnxyls.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://qi.asd995.cn

[Q52] 删除指定行
来源：http://ml.shxzskj.cn

DELETE FROM users WHERE id = 10;
来源：http://rt.jianghongdianzi.cn

[Q53] 按条件删除
来源：http://hk.yuntaijiaju.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://yx.bookmarksfly.cn

[Q54] 清空表
来源：http://ny.wgjwhj.cn

TRUNCATE TABLE logs;
来源：http://aq.521024.cn

[Q55] 排名（并列占位）
来源：http://qf.chemitech.net.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://rc.hahajie.cn

[Q56] 密集排名（并列不占位）
来源：http://yw.panjiajie.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://gp.bookmarksfly.cn

[Q57] 行号
来源：http://sy.haigaiapp.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://kh.asd995.cn

[Q58] 累计求和
来源：http://ji.yuexingan06.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://vk.haigaiapp.cn

[Q59] 分组内累计
来源：http://je.nszjky.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://bw.yuexingan06.cn

[Q60] 取上一行 / 下一行
来源：http://ga.bjjhwx.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://cj.haigaiapp.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://th.chemitech.net.cn

[Q61] 移动平均
来源：http://jz.jianghongdianzi.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://nl.panjiajie.cn

[Q62] 分组占比
来源：http://aj.hnjuh.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://pr.szxytkj.cn

[Q63] 开启事务
来源：http://la.huixinmuqiang.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://eh.colortex.cn

[Q64] 提交事务
来源：http://hb.nicolike.cn

COMMIT;
来源：http://sd.gzmigu.cn

[Q65] 回滚事务
来源：http://gr.nszjky.cn

ROLLBACK;
来源：http://bk.huixiangedu.cn

[Q66] 行锁查询
来源：http://ek.huixiangedu.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ju.yuexingan06.cn

[Q67] 设置隔离级别
来源：http://ei.bjjhwx.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://rg.huixiangedu.cn

[Q68] 保存点
来源：http://bu.gzmigu.cn

SAVEPOINT sp1;
来源：http://pq.chemitech.net.cn

ROLLBACK TO sp1;
来源：http://pp.bjjhwx.cn

[Q69] 查看执行计划
来源：http://yt.shtwfgs.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ku.newstarts.cn

[Q70] 更新统计信息
来源：http://ls.haigaiapp.cn

ANALYZE TABLE users;
来源：http://pw.shxzskj.cn

[Q71] 查看建表语句
来源：http://ri.nicolike.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://fq.nicolike.cn

[Q72] 查看索引
来源：http://th.521024.cn

SHOW INDEX FROM users;
来源：http://dc.asd995.cn

[Q73] 查看表状态
来源：http://yp.hnjuh.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://mx.muxihuayi.cn

[Q74] 强制使用索引
来源：http://el.lnxyls.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://tk.jianghongdianzi.cn

[Q75] 日期格式化
来源：http://gu.wgjwhj.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ht.szsharing.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mt.colortex.cn

[Q76] 按天统计
来源：http://sk.hahajie.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://rv.bjjhwx.cn

[Q77] 时间加减
来源：http://lk.shtwfgs.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ti.shtwfgs.cn

[Q78] 当前时间
来源：http://sm.shxzskj.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://jn.szxytkj.cn

[Q79] 字符串拼接
来源：http://pg.lnxyls.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://nf.gzmigu.cn

[Q80] 字符串截取
来源：http://or.bjjhwx.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://yu.hnjuh.cn

[Q81] 字符串替换
来源：http://cp.yuntaijiaju.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://qt.bjjhwx.cn

[Q82] 字符长度与字节长度
来源：http://dx.bookmarksfly.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://qw.bjjhwx.cn

[Q83] 大小写转换
来源：http://mz.bookmarksfly.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ij.asd995.cn

[Q84] 去除首尾空格
来源：http://fo.lnxyls.cn

SELECT TRIM(name) FROM users;
来源：http://jj.huixiangedu.cn

[Q85] 数值取整
来源：http://ms.huanxung.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://my.huixiangedu.cn

[Q86] 读取 JSON 字段
来源：http://np.newstarts.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://dt.jctech888.com.cn

[Q87] JSON 字段做条件
来源：http://ar.521024.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hw.wgjwhj.cn

[Q88] 行转列（条件聚合）
来源：http://lr.szsharing.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://it.muxihuayi.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mk.shxzskj.cn

[Q89] 判断表是否存在
来源：http://hb.panjiajie.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://xq.jctech888.com.cn

[Q90] 生成序号列
来源：http://ny.gzmigu.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://uy.shxzukj.cn

================================================================================
来源：http://ut.shxzskj.cn

R. Bash 专题
来源：http://gz.gzmigu.cn

================================================================================
来源：http://co.newstarts.cn

[R01] shebang 与严格模式
来源：http://qw.colortex.cn

#!/usr/bin/env bash
来源：http://ti.shtwfgs.cn

set -euo pipefail
来源：http://rt.muxihuayi.cn

[R02] 变量赋值与使用
来源：http://et.shxzukj.cn

name="Tom"; echo "$name"
来源：http://tl.panjiajie.cn

[R03] 只读变量
来源：http://ph.yuntaijiaju.cn

readonly PI=3.14
来源：http://ft.nszjky.cn

[R04] 位置参数
来源：http://bp.colortex.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ap.shxzukj.cn

[R05] 参数默认值
来源：http://gp.huixiangedu.cn

name="${1:-default}"
来源：http://vy.bjjhwx.cn

[R06] 判断命令是否存在
来源：http://rn.shxzukj.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://dp.szxytkj.cn

[R07] if 判断文件
来源：http://tv.521024.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ox.521024.cn

[R08] 数值比较
来源：http://nz.asd995.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://iw.panjiajie.cn

[R09] 字符串比较
来源：http://zp.jianghongdianzi.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://nz.szsharing.cn

[R10] 正则匹配
来源：http://dq.chemitech.net.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://pw.hnjuh.cn

[R11] case 多分支
来源：http://vz.nszjky.cn

case "$1" in
来源：http://fd.lnxyls.cn

start) echo "启动" ;;
来源：http://zf.bjjhwx.cn

stop)  echo "停止" ;;
来源：http://zs.szsharing.cn

*)     echo "未知命令" ;;
来源：http://pp.521024.cn

esac
来源：http://cn.nszjky.cn

[R12] for 遍历文件
来源：http://bd.hahajie.cn

for f in *.txt; do echo "$f"; done
来源：http://mx.huixiangedu.cn

[R13] for 计数循环
来源：http://zy.jianghongdianzi.cn

for i in {1..10}; do echo "$i"; done
来源：http://xu.haigaiapp.cn

[R14] C 风格 for
来源：http://is.chemitech.net.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hd.yuexingan06.cn

[R15] while 逐行读文件
来源：http://zk.haigaiapp.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ln.yuexingan06.cn

[R16] until 等待条件
来源：http://le.huanxung.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://gy.bjjhwx.cn

[R17] 数组定义与取值
来源：http://it.huixiangedu.cn

arr=(a b c); echo "${arr[0]}"
来源：http://jj.muxihuayi.cn

[R18] 遍历数组
来源：http://xk.muxihuayi.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://rt.asd995.cn

[R19] 数组长度
来源：http://bq.newstarts.cn

echo "${#arr[@]}"
来源：http://jv.521024.cn

[R20] 关联数组（字典）
来源：http://ed.shtwfgs.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://zs.nszjky.cn

[R21] 字符串长度
来源：http://pi.shxzukj.cn

echo "${#s}"
来源：http://sq.szsharing.cn

[R22] 截取子串
来源：http://mb.lnxyls.cn

echo "${s:0:5}"
来源：http://ou.yuexingan06.cn

[R23] 字符串替换
来源：http://ca.jctech888.com.cn


<!-- 参考信息 -->