代发 wailian999

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://nn.huixiangedu.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://eb.huixinmuqiang.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://km.nszjky.cn

[P04] 求长度
来源：http://di.nicolike.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://uv.hnjuh.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://by.521024.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://sc.bjjhwx.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://fg.nszjky.cn

Java: list.size();  map.size();  s.length()
来源：http://dh.huanxung.cn

Go:   len(arr);  len(m)
来源：http://wj.shxzukj.cn

Ruby: x.length;  x.size
来源：http://fb.gzmigu.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://ss.hnjuh.cn

[P05] 判断两个对象内容是否相等
来源：http://xk.panjiajie.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://zy.shxzukj.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wm.muxihuayi.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ck.nicolike.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://pa.hahajie.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://lh.bjjhwx.cn

Go:   reflect.DeepEqual(a, b)
来源：http://cp.hnjuh.cn

Ruby: a == b
来源：http://bv.huixinmuqiang.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://bs.yuexingan06.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://vn.wgjwhj.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://kn.yuexingan06.cn

PHP:  if (empty($x)) {}
来源：http://ay.newstarts.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://tf.panjiajie.cn

TS:   if (x == null) {}
来源：http://at.shxzukj.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://xc.gzmigu.cn

Go:   if x == nil {}
来源：http://zd.hnjuh.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://la.bookmarksfly.cn

C#:   if (x is null) {}
来源：http://zj.szsharing.cn

[P07] 防抖与节流
来源：http://jx.yuexingan06.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://sf.panjiajie.cn

PHP:  // 手写时间戳比较
来源：http://zx.colortex.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ve.9csxet.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wo.szxytkj.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://oe.haigaiapp.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hc.nicolike.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://br.newstarts.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ym.yuexingan06.cn

[P08] 处理浮点精度问题
来源：http://iu.shtwfgs.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://py.hahajie.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ns.chemitech.net.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://uf.huanxung.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://vj.huixinmuqiang.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://of.newstarts.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://uk.wgjwhj.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://lz.shtwfgs.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://rk.nicolike.cn

================================================================================
来源：http://kg.chemitech.net.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wb.hahajie.cn

================================================================================
来源：http://gk.9csxet.cn

[Q01] 创建表
来源：http://kr.nszjky.cn

CREATE TABLE users (
来源：http://th.colortex.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://tw.jianghongdianzi.cn

name VARCHAR(50) NOT NULL,
来源：http://xb.jctech888.com.cn

email VARCHAR(100) UNIQUE,
来源：http://gk.newstarts.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mm.huanxung.cn

);
来源：http://ai.huanxung.cn

[Q02] 创建带外键的表
来源：http://je.szxytkj.cn

CREATE TABLE orders (
来源：http://fb.wgjwhj.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://br.szxytkj.cn

user_id INT NOT NULL,
来源：http://ze.muxihuayi.cn

amount DECIMAL(10, 2),
来源：http://ef.huanxung.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hq.nicolike.cn

);
来源：http://ki.wgjwhj.cn

[Q03] 增加列
来源：http://uo.szxytkj.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://bs.haigaiapp.cn

[Q04] 修改列类型
来源：http://oj.hnjuh.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ul.asd995.cn

[Q05] 重命名列
来源：http://fg.huixinmuqiang.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://kp.hnjuh.cn

[Q06] 删除列
来源：http://zf.bookmarksfly.cn

ALTER TABLE users DROP COLUMN age;
来源：http://zn.haigaiapp.cn

[Q07] 删除表
来源：http://zm.9csxet.cn

DROP TABLE IF EXISTS orders;
来源：http://qj.nicolike.cn

[Q08] 创建普通索引
来源：http://rg.nszjky.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://pk.shtwfgs.cn

[Q09] 创建唯一索引
来源：http://hf.huanxung.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wm.chemitech.net.cn

[Q10] 插入单行
来源：http://np.newstarts.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://cq.huixiangedu.cn

[Q11] 一次插入多行
来源：http://su.huixinmuqiang.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://et.asd995.cn

[Q12] 插入后取自增 ID
来源：http://ur.szsharing.cn

INSERT INTO users (name) VALUES ('C');
来源：http://lp.521024.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://rw.yuntaijiaju.cn

[Q13] 忽略重复插入
来源：http://kr.wgjwhj.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://gg.jianghongdianzi.cn

[Q14] 存在则更新（upsert）
来源：http://bf.szxytkj.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://gf.hahajie.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://cl.asd995.cn

[Q15] 查询全部
来源：http://or.lnxyls.cn

SELECT * FROM users;
来源：http://wj.gzmigu.cn

[Q16] 查询指定列
来源：http://hf.jctech888.com.cn

SELECT id, name FROM users;
来源：http://lu.bookmarksfly.cn

[Q17] 条件查询
来源：http://kr.yuexingan06.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://uc.bjjhwx.cn

[Q18] 模糊匹配
来源：http://wd.huixinmuqiang.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://yn.huixinmuqiang.cn

[Q19] 范围查询
来源：http://ui.wgjwhj.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://bc.chemitech.net.cn

[Q20] IN 列表
来源：http://od.bookmarksfly.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://lh.shxzskj.cn

[Q21] 空值判断
来源：http://vx.bookmarksfly.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://ui.colortex.cn

[Q22] 排序
来源：http://jo.shxzskj.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wg.huixiangedu.cn

[Q23] 分页
来源：http://bd.nszjky.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://bw.huixinmuqiang.cn

[Q24] 去重
来源：http://sd.wgjwhj.cn

SELECT DISTINCT city FROM users;
来源：http://qg.huanxung.cn

[Q25] 只取前 N 条
来源：http://oc.huixiangedu.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ol.bookmarksfly.cn

[Q26] 计数
来源：http://ur.gzmigu.cn

SELECT COUNT(*) FROM users;
来源：http://vv.huanxung.cn

[Q27] 条件计数
来源：http://or.yuntaijiaju.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wo.lnxyls.cn

[Q28] 求和与平均
来源：http://jy.muxihuayi.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://kd.huanxung.cn

[Q29] 最大最小值
来源：http://ix.nicolike.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://qb.bjjhwx.cn

[Q30] 分组统计
来源：http://gz.wgjwhj.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://id.asd995.cn

[Q31] 分组后过滤
来源：http://xa.nszjky.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://im.szxytkj.cn

[Q32] 分组拼接字符串
来源：http://fx.haigaiapp.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://vy.wgjwhj.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://kx.jianghongdianzi.cn

[Q33] 多列分组
来源：http://dv.nicolike.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://zm.yuntaijiaju.cn

[Q34] 每组取第一条
来源：http://ko.bookmarksfly.cn

SELECT * FROM (
来源：http://ck.colortex.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://yo.jianghongdianzi.cn

) t WHERE rn = 1;
来源：http://jy.bookmarksfly.cn

[Q35] 内连接
来源：http://vh.huixinmuqiang.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://uv.huixiangedu.cn

[Q36] 左连接
来源：http://kj.colortex.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ff.colortex.cn

[Q37] 右连接
来源：http://ce.huixiangedu.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ie.shtwfgs.cn

[Q38] 全外连接（PostgreSQL）
来源：http://rx.colortex.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://kl.huanxung.cn

[Q39] 自连接（查上下级）
来源：http://ti.lnxyls.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://vr.lnxyls.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://qu.9csxet.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://ta.shtwfgs.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://xu.huixiangedu.cn

[Q41] 多表连接
来源：http://ht.muxihuayi.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://sw.yuntaijiaju.cn

JOIN users u ON u.id = o.user_id
来源：http://lb.wgjwhj.cn

JOIN products p ON p.id = o.product_id;
来源：http://kg.hahajie.cn

[Q42] 连接条件附加过滤
来源：http://jh.colortex.cn

SELECT u.name, o.amount FROM users u
来源：http://pi.huixinmuqiang.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://tm.shxzskj.cn

[Q43] 标量子查询
来源：http://oy.9csxet.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://jy.jianghongdianzi.cn

[Q44] IN 子查询
来源：http://as.hnjuh.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://pl.bookmarksfly.cn

[Q45] EXISTS 判断存在
来源：http://xn.szxytkj.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://dv.hnjuh.cn

[Q46] NOT EXISTS 判断不存在
来源：http://go.shtwfgs.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://vm.lnxyls.cn

[Q47] 与平均值比较
来源：http://oj.521024.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wx.shtwfgs.cn

[Q48] CTE 公用表表达式
来源：http://nh.asd995.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://lg.asd995.cn

SELECT * FROM t WHERE c > 5;
来源：http://tn.newstarts.cn

[Q49] 更新单行
来源：http://jg.szsharing.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://zb.shxzskj.cn

[Q50] 批量更新
来源：http://pj.bjjhwx.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://sb.nszjky.cn

[Q51] 用子查询更新
来源：http://pb.chemitech.net.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://ru.lnxyls.cn

[Q52] 删除指定行
来源：http://xj.asd995.cn

DELETE FROM users WHERE id = 10;
来源：http://gc.chemitech.net.cn

[Q53] 按条件删除
来源：http://tk.newstarts.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://zk.szxytkj.cn

[Q54] 清空表
来源：http://yv.hahajie.cn

TRUNCATE TABLE logs;
来源：http://ff.huixinmuqiang.cn

[Q55] 排名（并列占位）
来源：http://qe.bookmarksfly.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://yi.szsharing.cn

[Q56] 密集排名（并列不占位）
来源：http://oo.jianghongdianzi.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ue.chemitech.net.cn

[Q57] 行号
来源：http://pm.szxytkj.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://gc.huixiangedu.cn

[Q58] 累计求和
来源：http://ha.shxzukj.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://iq.hnjuh.cn

[Q59] 分组内累计
来源：http://mb.nicolike.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://nr.bjjhwx.cn

[Q60] 取上一行 / 下一行
来源：http://xt.panjiajie.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://gb.wgjwhj.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://jx.shxzskj.cn

[Q61] 移动平均
来源：http://dc.hnjuh.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://df.521024.cn

[Q62] 分组占比
来源：http://nw.nicolike.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://se.muxihuayi.cn

[Q63] 开启事务
来源：http://iz.shtwfgs.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://bk.huanxung.cn

[Q64] 提交事务
来源：http://gd.huixiangedu.cn

COMMIT;
来源：http://me.panjiajie.cn

[Q65] 回滚事务
来源：http://zb.shxzskj.cn

ROLLBACK;
来源：http://lp.colortex.cn

[Q66] 行锁查询
来源：http://jm.szsharing.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://lj.panjiajie.cn

[Q67] 设置隔离级别
来源：http://sz.nicolike.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://iq.yuntaijiaju.cn

[Q68] 保存点
来源：http://fv.yuexingan06.cn

SAVEPOINT sp1;
来源：http://ww.yuexingan06.cn

ROLLBACK TO sp1;
来源：http://ns.yuntaijiaju.cn

[Q69] 查看执行计划
来源：http://qu.colortex.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://as.wgjwhj.cn

[Q70] 更新统计信息
来源：http://fu.muxihuayi.cn

ANALYZE TABLE users;
来源：http://gu.521024.cn

[Q71] 查看建表语句
来源：http://sw.lnxyls.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://gc.jctech888.com.cn

[Q72] 查看索引
来源：http://aq.shtwfgs.cn

SHOW INDEX FROM users;
来源：http://kv.colortex.cn

[Q73] 查看表状态
来源：http://hd.szxytkj.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://mh.hahajie.cn

[Q74] 强制使用索引
来源：http://pu.szxytkj.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://eh.shxzskj.cn

[Q75] 日期格式化
来源：http://ng.shtwfgs.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://yy.nszjky.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://fk.szsharing.cn

[Q76] 按天统计
来源：http://gq.panjiajie.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://gd.lnxyls.cn

[Q77] 时间加减
来源：http://pc.szsharing.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://dx.nicolike.cn

[Q78] 当前时间
来源：http://cs.muxihuayi.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hs.lnxyls.cn

[Q79] 字符串拼接
来源：http://gw.yuexingan06.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://xk.jctech888.com.cn

[Q80] 字符串截取
来源：http://oa.hnjuh.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://kc.shxzskj.cn

[Q81] 字符串替换
来源：http://ob.chemitech.net.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ol.newstarts.cn

[Q82] 字符长度与字节长度
来源：http://er.gzmigu.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://iy.huixiangedu.cn

[Q83] 大小写转换
来源：http://gl.bjjhwx.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://il.muxihuayi.cn

[Q84] 去除首尾空格
来源：http://je.521024.cn

SELECT TRIM(name) FROM users;
来源：http://xa.gzmigu.cn

[Q85] 数值取整
来源：http://co.hahajie.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ro.jianghongdianzi.cn

[Q86] 读取 JSON 字段
来源：http://sp.gzmigu.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://sh.haigaiapp.cn

[Q87] JSON 字段做条件
来源：http://sy.huanxung.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ka.521024.cn

[Q88] 行转列（条件聚合）
来源：http://ii.wgjwhj.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ze.nicolike.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ej.shtwfgs.cn

[Q89] 判断表是否存在
来源：http://rh.wgjwhj.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://gb.asd995.cn

[Q90] 生成序号列
来源：http://kw.shxzskj.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://at.shxzukj.cn

================================================================================
来源：http://ga.yuexingan06.cn

R. Bash 专题
来源：http://cq.shtwfgs.cn

================================================================================
来源：http://fb.wgjwhj.cn

[R01] shebang 与严格模式
来源：http://ua.haigaiapp.cn

#!/usr/bin/env bash
来源：http://lj.shtwfgs.cn

set -euo pipefail
来源：http://tx.shxzskj.cn

[R02] 变量赋值与使用
来源：http://pe.colortex.cn

name="Tom"; echo "$name"
来源：http://rb.gzmigu.cn

[R03] 只读变量
来源：http://tv.colortex.cn

readonly PI=3.14
来源：http://aq.yuntaijiaju.cn

[R04] 位置参数
来源：http://jr.szxytkj.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hx.jianghongdianzi.cn

[R05] 参数默认值
来源：http://ir.nicolike.cn

name="${1:-default}"
来源：http://qd.szxytkj.cn

[R06] 判断命令是否存在
来源：http://gh.yuexingan06.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://aa.hahajie.cn

[R07] if 判断文件
来源：http://df.gzmigu.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://dt.hahajie.cn

[R08] 数值比较
来源：http://nb.chemitech.net.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://xy.huixinmuqiang.cn

[R09] 字符串比较
来源：http://un.szxytkj.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://lq.lnxyls.cn

[R10] 正则匹配
来源：http://ex.huixiangedu.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://vq.nszjky.cn

[R11] case 多分支
来源：http://al.asd995.cn

case "$1" in
来源：http://ep.lnxyls.cn

start) echo "启动" ;;
来源：http://py.szsharing.cn

stop)  echo "停止" ;;
来源：http://sf.shxzukj.cn

*)     echo "未知命令" ;;
来源：http://kb.muxihuayi.cn

esac
来源：http://kx.nszjky.cn

[R12] for 遍历文件
来源：http://qa.asd995.cn

for f in *.txt; do echo "$f"; done
来源：http://xx.muxihuayi.cn

[R13] for 计数循环
来源：http://hg.haigaiapp.cn

for i in {1..10}; do echo "$i"; done
来源：http://dx.jctech888.com.cn

[R14] C 风格 for
来源：http://ak.asd995.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://gv.hnjuh.cn

[R15] while 逐行读文件
来源：http://nb.wgjwhj.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ow.yuntaijiaju.cn

[R16] until 等待条件
来源：http://vy.9csxet.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://fc.hahajie.cn

[R17] 数组定义与取值
来源：http://nw.shxzskj.cn

arr=(a b c); echo "${arr[0]}"
来源：http://ao.hahajie.cn

[R18] 遍历数组
来源：http://rs.newstarts.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://il.szsharing.cn

[R19] 数组长度
来源：http://ir.nicolike.cn


<!-- 参考信息 -->