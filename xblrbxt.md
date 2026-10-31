代发 wailian999

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ss.jctech888.com.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://hl.huanxung.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://nx.jctech888.com.cn

[P04] 求长度
来源：http://sq.colortex.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://xo.nszjky.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://bb.yuntaijiaju.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://rf.shtwfgs.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://in.chemitech.net.cn

Java: list.size();  map.size();  s.length()
来源：http://dg.hahajie.cn

Go:   len(arr);  len(m)
来源：http://xq.hahajie.cn

Ruby: x.length;  x.size
来源：http://mo.huixinmuqiang.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://ea.jianghongdianzi.cn

[P05] 判断两个对象内容是否相等
来源：http://at.asd995.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://bl.nicolike.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://yn.haigaiapp.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://jb.asd995.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://do.szsharing.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://fs.chemitech.net.cn

Go:   reflect.DeepEqual(a, b)
来源：http://uj.hnjuh.cn

Ruby: a == b
来源：http://qo.huixinmuqiang.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://vx.gzmigu.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ps.521024.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://qb.jianghongdianzi.cn

PHP:  if (empty($x)) {}
来源：http://on.gzmigu.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ju.asd995.cn

TS:   if (x == null) {}
来源：http://dd.jctech888.com.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://zb.bookmarksfly.cn

Go:   if x == nil {}
来源：http://up.yuexingan06.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hw.jctech888.com.cn

C#:   if (x is null) {}
来源：http://uo.haigaiapp.cn

[P07] 防抖与节流
来源：http://nz.asd995.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://km.nszjky.cn

PHP:  // 手写时间戳比较
来源：http://et.shtwfgs.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ic.bookmarksfly.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wb.szsharing.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hv.nicolike.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://pi.huixiangedu.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://cm.bjjhwx.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://pd.wgjwhj.cn

[P08] 处理浮点精度问题
来源：http://zu.521024.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wj.szxytkj.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ny.szsharing.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://sb.colortex.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://kr.chemitech.net.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://in.szxytkj.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://qg.gzmigu.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://xr.gzmigu.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://eo.chemitech.net.cn

================================================================================
来源：http://oz.shxzukj.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://fe.bjjhwx.cn

================================================================================
来源：http://lu.hahajie.cn

[Q01] 创建表
来源：http://os.521024.cn

CREATE TABLE users (
来源：http://df.newstarts.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://yh.hnjuh.cn

name VARCHAR(50) NOT NULL,
来源：http://ds.nszjky.cn

email VARCHAR(100) UNIQUE,
来源：http://fn.nszjky.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://su.asd995.cn

);
来源：http://bv.asd995.cn

[Q02] 创建带外键的表
来源：http://tq.yuexingan06.cn

CREATE TABLE orders (
来源：http://eb.haigaiapp.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://sv.521024.cn

user_id INT NOT NULL,
来源：http://tg.hnjuh.cn

amount DECIMAL(10, 2),
来源：http://oq.nszjky.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://xz.shxzukj.cn

);
来源：http://ys.colortex.cn

[Q03] 增加列
来源：http://iv.haigaiapp.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://nb.huanxung.cn

[Q04] 修改列类型
来源：http://vj.huixiangedu.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ne.9csxet.cn

[Q05] 重命名列
来源：http://ef.521024.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://bh.huanxung.cn

[Q06] 删除列
来源：http://rz.newstarts.cn

ALTER TABLE users DROP COLUMN age;
来源：http://lx.wgjwhj.cn

[Q07] 删除表
来源：http://gv.huixinmuqiang.cn

DROP TABLE IF EXISTS orders;
来源：http://vm.bookmarksfly.cn

[Q08] 创建普通索引
来源：http://ld.lnxyls.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://xi.bookmarksfly.cn

[Q09] 创建唯一索引
来源：http://qb.bjjhwx.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://zs.haigaiapp.cn

[Q10] 插入单行
来源：http://br.hnjuh.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://no.shxzskj.cn

[Q11] 一次插入多行
来源：http://vm.nicolike.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://fd.nicolike.cn

[Q12] 插入后取自增 ID
来源：http://lg.9csxet.cn

INSERT INTO users (name) VALUES ('C');
来源：http://vi.huixinmuqiang.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://jf.colortex.cn

[Q13] 忽略重复插入
来源：http://dx.bookmarksfly.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://zd.huixinmuqiang.cn

[Q14] 存在则更新（upsert）
来源：http://je.newstarts.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://zl.hnjuh.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://lk.panjiajie.cn

[Q15] 查询全部
来源：http://gy.huixiangedu.cn

SELECT * FROM users;
来源：http://bt.panjiajie.cn

[Q16] 查询指定列
来源：http://ph.muxihuayi.cn

SELECT id, name FROM users;
来源：http://nd.yuntaijiaju.cn

[Q17] 条件查询
来源：http://it.yuexingan06.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://on.newstarts.cn

[Q18] 模糊匹配
来源：http://zk.szxytkj.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ia.jctech888.com.cn

[Q19] 范围查询
来源：http://da.yuexingan06.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://sv.9csxet.cn

[Q20] IN 列表
来源：http://ma.yuntaijiaju.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://al.huixinmuqiang.cn

[Q21] 空值判断
来源：http://nu.huixiangedu.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://ui.nicolike.cn

[Q22] 排序
来源：http://ln.yuexingan06.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ed.nszjky.cn

[Q23] 分页
来源：http://mh.chemitech.net.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://gb.yuntaijiaju.cn

[Q24] 去重
来源：http://wj.shtwfgs.cn

SELECT DISTINCT city FROM users;
来源：http://uz.lnxyls.cn

[Q25] 只取前 N 条
来源：http://wg.bjjhwx.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://iz.huixiangedu.cn

[Q26] 计数
来源：http://lf.panjiajie.cn

SELECT COUNT(*) FROM users;
来源：http://qm.huixiangedu.cn

[Q27] 条件计数
来源：http://hh.shxzskj.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ot.yuntaijiaju.cn

[Q28] 求和与平均
来源：http://as.nicolike.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://uk.9csxet.cn

[Q29] 最大最小值
来源：http://il.9csxet.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://hf.hahajie.cn

[Q30] 分组统计
来源：http://to.wgjwhj.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://fc.huanxung.cn

[Q31] 分组后过滤
来源：http://er.shxzukj.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://xw.panjiajie.cn

[Q32] 分组拼接字符串
来源：http://bu.wgjwhj.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://dl.shxzskj.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://bk.muxihuayi.cn

[Q33] 多列分组
来源：http://uz.yuexingan06.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://sk.huanxung.cn

[Q34] 每组取第一条
来源：http://fi.haigaiapp.cn

SELECT * FROM (
来源：http://ev.nicolike.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://lw.szsharing.cn

) t WHERE rn = 1;
来源：http://vv.szxytkj.cn

[Q35] 内连接
来源：http://gb.shxzskj.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://bz.jctech888.com.cn

[Q36] 左连接
来源：http://vc.huixiangedu.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://gp.asd995.cn

[Q37] 右连接
来源：http://ef.hnjuh.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ut.newstarts.cn

[Q38] 全外连接（PostgreSQL）
来源：http://ml.szsharing.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ys.jianghongdianzi.cn

[Q39] 自连接（查上下级）
来源：http://tf.shxzukj.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://ti.bookmarksfly.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://zj.panjiajie.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://lj.haigaiapp.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://lm.szsharing.cn

[Q41] 多表连接
来源：http://cx.jianghongdianzi.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://mk.yuntaijiaju.cn

JOIN users u ON u.id = o.user_id
来源：http://ar.muxihuayi.cn

JOIN products p ON p.id = o.product_id;
来源：http://hg.asd995.cn

[Q42] 连接条件附加过滤
来源：http://dk.yuexingan06.cn

SELECT u.name, o.amount FROM users u
来源：http://wl.asd995.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://yh.nszjky.cn

[Q43] 标量子查询
来源：http://xh.huixiangedu.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mk.yuexingan06.cn

[Q44] IN 子查询
来源：http://od.szsharing.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://iy.muxihuayi.cn

[Q45] EXISTS 判断存在
来源：http://jg.hahajie.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://bz.colortex.cn

[Q46] NOT EXISTS 判断不存在
来源：http://nb.haigaiapp.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://iw.huixinmuqiang.cn

[Q47] 与平均值比较
来源：http://nx.nicolike.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ck.huixinmuqiang.cn

[Q48] CTE 公用表表达式
来源：http://nn.nicolike.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://vi.9csxet.cn

SELECT * FROM t WHERE c > 5;
来源：http://zi.hahajie.cn

[Q49] 更新单行
来源：http://un.hnjuh.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ee.wgjwhj.cn

[Q50] 批量更新
来源：http://ap.shtwfgs.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://nd.yuexingan06.cn

[Q51] 用子查询更新
来源：http://rl.hnjuh.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://bv.bookmarksfly.cn

[Q52] 删除指定行
来源：http://cz.hnjuh.cn

DELETE FROM users WHERE id = 10;
来源：http://od.szxytkj.cn

[Q53] 按条件删除
来源：http://ct.yuexingan06.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://yd.muxihuayi.cn

[Q54] 清空表
来源：http://ba.szxytkj.cn

TRUNCATE TABLE logs;
来源：http://jx.nicolike.cn

[Q55] 排名（并列占位）
来源：http://we.521024.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://cu.yuntaijiaju.cn

[Q56] 密集排名（并列不占位）
来源：http://xt.nicolike.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ct.huixiangedu.cn

[Q57] 行号
来源：http://jo.colortex.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://dv.jctech888.com.cn

[Q58] 累计求和
来源：http://ax.jianghongdianzi.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://by.huixiangedu.cn

[Q59] 分组内累计
来源：http://iz.jianghongdianzi.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ni.wgjwhj.cn

[Q60] 取上一行 / 下一行
来源：http://kv.chemitech.net.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://gy.9csxet.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://yp.panjiajie.cn

[Q61] 移动平均
来源：http://tx.yuntaijiaju.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://vd.nicolike.cn

[Q62] 分组占比
来源：http://vk.shxzskj.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://vn.chemitech.net.cn

[Q63] 开启事务
来源：http://wx.newstarts.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://yq.asd995.cn

[Q64] 提交事务
来源：http://wu.nicolike.cn

COMMIT;
来源：http://mi.szsharing.cn

[Q65] 回滚事务
来源：http://oz.bjjhwx.cn

ROLLBACK;
来源：http://bc.9csxet.cn

[Q66] 行锁查询
来源：http://ox.gzmigu.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hl.huanxung.cn

[Q67] 设置隔离级别
来源：http://rc.huixiangedu.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://le.szsharing.cn

[Q68] 保存点
来源：http://cc.newstarts.cn

SAVEPOINT sp1;
来源：http://zl.lnxyls.cn

ROLLBACK TO sp1;
来源：http://mc.nicolike.cn

[Q69] 查看执行计划
来源：http://ql.shxzukj.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wp.hnjuh.cn

[Q70] 更新统计信息
来源：http://ep.9csxet.cn

ANALYZE TABLE users;
来源：http://vm.yuexingan06.cn

[Q71] 查看建表语句
来源：http://xy.asd995.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://zz.colortex.cn

[Q72] 查看索引
来源：http://qe.yuntaijiaju.cn

SHOW INDEX FROM users;
来源：http://df.huixiangedu.cn

[Q73] 查看表状态
来源：http://wc.newstarts.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://zc.huixiangedu.cn

[Q74] 强制使用索引
来源：http://wp.hahajie.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ml.muxihuayi.cn

[Q75] 日期格式化
来源：http://wy.hnjuh.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://bu.huixiangedu.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ze.chemitech.net.cn

[Q76] 按天统计
来源：http://mb.huixinmuqiang.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://az.haigaiapp.cn

[Q77] 时间加减
来源：http://qy.huanxung.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://iy.bookmarksfly.cn

[Q78] 当前时间
来源：http://qs.hahajie.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://zj.szxytkj.cn

[Q79] 字符串拼接
来源：http://he.muxihuayi.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://zb.huixinmuqiang.cn

[Q80] 字符串截取
来源：http://dy.haigaiapp.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ze.gzmigu.cn

[Q81] 字符串替换
来源：http://rf.shtwfgs.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://tl.colortex.cn

[Q82] 字符长度与字节长度
来源：http://bv.shxzukj.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://tv.huixiangedu.cn

[Q83] 大小写转换
来源：http://rv.hahajie.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://sp.bookmarksfly.cn

[Q84] 去除首尾空格
来源：http://bk.asd995.cn

SELECT TRIM(name) FROM users;
来源：http://gt.asd995.cn

[Q85] 数值取整
来源：http://ds.muxihuayi.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ow.szsharing.cn

[Q86] 读取 JSON 字段
来源：http://vm.521024.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ay.hnjuh.cn

[Q87] JSON 字段做条件
来源：http://dz.hahajie.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://xb.chemitech.net.cn

[Q88] 行转列（条件聚合）
来源：http://zo.bjjhwx.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://qz.huixinmuqiang.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://gm.huixinmuqiang.cn

[Q89] 判断表是否存在
来源：http://hg.521024.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://bn.nszjky.cn

[Q90] 生成序号列
来源：http://tp.asd995.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://pf.shtwfgs.cn

================================================================================
来源：http://ft.haigaiapp.cn

R. Bash 专题
来源：http://oj.szxytkj.cn

================================================================================
来源：http://fn.colortex.cn

[R01] shebang 与严格模式
来源：http://di.gzmigu.cn

#!/usr/bin/env bash
来源：http://ja.szsharing.cn

set -euo pipefail
来源：http://bf.muxihuayi.cn

[R02] 变量赋值与使用
来源：http://zd.jctech888.com.cn

name="Tom"; echo "$name"
来源：http://mn.yuexingan06.cn

[R03] 只读变量
来源：http://mq.hahajie.cn

readonly PI=3.14
来源：http://ve.shxzukj.cn

[R04] 位置参数
来源：http://mv.muxihuayi.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://kv.bjjhwx.cn

[R05] 参数默认值
来源：http://vk.521024.cn

name="${1:-default}"
来源：http://ty.newstarts.cn

[R06] 判断命令是否存在
来源：http://tc.wgjwhj.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://kn.newstarts.cn

[R07] if 判断文件
来源：http://ec.haigaiapp.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://uo.shtwfgs.cn

[R08] 数值比较
来源：http://sb.newstarts.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://xu.huanxung.cn

[R09] 字符串比较
来源：http://gi.shxzskj.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ap.huixinmuqiang.cn

[R10] 正则匹配
来源：http://cv.bookmarksfly.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://tx.jianghongdianzi.cn

[R11] case 多分支
来源：http://ou.jianghongdianzi.cn

case "$1" in
来源：http://mn.lnxyls.cn

start) echo "启动" ;;
来源：http://wl.panjiajie.cn

stop)  echo "停止" ;;
来源：http://sz.muxihuayi.cn

*)     echo "未知命令" ;;
来源：http://gl.9csxet.cn

esac
来源：http://cc.gzmigu.cn

[R12] for 遍历文件
来源：http://ci.panjiajie.cn

for f in *.txt; do echo "$f"; done
来源：http://cs.chemitech.net.cn

[R13] for 计数循环
来源：http://ga.yuexingan06.cn

for i in {1..10}; do echo "$i"; done
来源：http://rr.newstarts.cn

[R14] C 风格 for
来源：http://xs.shxzukj.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ya.muxihuayi.cn

[R15] while 逐行读文件
来源：http://mw.newstarts.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://dz.haigaiapp.cn

[R16] until 等待条件
来源：http://sl.muxihuayi.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://fu.wgjwhj.cn

[R17] 数组定义与取值
来源：http://zq.panjiajie.cn

arr=(a b c); echo "${arr[0]}"
来源：http://zm.huixiangedu.cn

[R18] 遍历数组
来源：http://ud.yuexingan06.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mw.shxzukj.cn

[R19] 数组长度
来源：http://lk.521024.cn


<!-- 参考信息 -->