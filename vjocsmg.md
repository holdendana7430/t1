代发 wailian999

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ur.jctech888.com.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://jz.haigaiapp.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ea.colortex.cn

[P04] 求长度
来源：http://ch.muxihuayi.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://lv.9csxet.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://vt.asd995.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hl.hnjuh.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://np.huanxung.cn

Java: list.size();  map.size();  s.length()
来源：http://me.chemitech.net.cn

Go:   len(arr);  len(m)
来源：http://es.bookmarksfly.cn

Ruby: x.length;  x.size
来源：http://rt.bookmarksfly.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://wq.panjiajie.cn

[P05] 判断两个对象内容是否相等
来源：http://ab.haigaiapp.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://yv.bookmarksfly.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://bk.yuntaijiaju.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://fv.chemitech.net.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://rb.9csxet.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://fz.colortex.cn

Go:   reflect.DeepEqual(a, b)
来源：http://fe.jctech888.com.cn

Ruby: a == b
来源：http://ys.lnxyls.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wl.wgjwhj.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://vk.shxzskj.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://lu.gzmigu.cn

PHP:  if (empty($x)) {}
来源：http://gv.521024.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://op.shxzukj.cn

TS:   if (x == null) {}
来源：http://zb.szxytkj.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://nr.asd995.cn

Go:   if x == nil {}
来源：http://va.shtwfgs.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://bk.muxihuayi.cn

C#:   if (x is null) {}
来源：http://jg.wgjwhj.cn

[P07] 防抖与节流
来源：http://bb.hnjuh.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://om.hahajie.cn

PHP:  // 手写时间戳比较
来源：http://fr.shtwfgs.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ov.nicolike.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://lx.yuntaijiaju.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://gz.nszjky.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wc.hahajie.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://en.huanxung.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://pz.muxihuayi.cn

[P08] 处理浮点精度问题
来源：http://qa.panjiajie.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://de.gzmigu.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://zn.hnjuh.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://rd.yuexingan06.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://cc.colortex.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://kk.yuntaijiaju.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wn.521024.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://df.shtwfgs.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://uq.jianghongdianzi.cn

================================================================================
来源：http://nd.nicolike.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ef.wgjwhj.cn

================================================================================
来源：http://qc.nszjky.cn

[Q01] 创建表
来源：http://iz.wgjwhj.cn

CREATE TABLE users (
来源：http://vg.bjjhwx.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://cf.muxihuayi.cn

name VARCHAR(50) NOT NULL,
来源：http://ay.huixinmuqiang.cn

email VARCHAR(100) UNIQUE,
来源：http://wp.jianghongdianzi.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wu.gzmigu.cn

);
来源：http://dm.jctech888.com.cn

[Q02] 创建带外键的表
来源：http://yy.szsharing.cn

CREATE TABLE orders (
来源：http://wx.lnxyls.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://oi.bjjhwx.cn

user_id INT NOT NULL,
来源：http://uo.jctech888.com.cn

amount DECIMAL(10, 2),
来源：http://qe.jianghongdianzi.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://in.muxihuayi.cn

);
来源：http://kq.wgjwhj.cn

[Q03] 增加列
来源：http://hw.huixinmuqiang.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://qw.muxihuayi.cn

[Q04] 修改列类型
来源：http://vl.bookmarksfly.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://jh.chemitech.net.cn

[Q05] 重命名列
来源：http://qz.huixinmuqiang.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://xg.huixiangedu.cn

[Q06] 删除列
来源：http://fp.hahajie.cn

ALTER TABLE users DROP COLUMN age;
来源：http://hf.hahajie.cn

[Q07] 删除表
来源：http://zr.shxzskj.cn

DROP TABLE IF EXISTS orders;
来源：http://gz.521024.cn

[Q08] 创建普通索引
来源：http://he.jianghongdianzi.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://fh.bookmarksfly.cn

[Q09] 创建唯一索引
来源：http://ei.muxihuayi.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://fp.bookmarksfly.cn

[Q10] 插入单行
来源：http://pk.bjjhwx.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://tt.huixinmuqiang.cn

[Q11] 一次插入多行
来源：http://hu.haigaiapp.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://oq.szsharing.cn

[Q12] 插入后取自增 ID
来源：http://uo.521024.cn

INSERT INTO users (name) VALUES ('C');
来源：http://ne.jctech888.com.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://oc.521024.cn

[Q13] 忽略重复插入
来源：http://ks.9csxet.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://eg.szsharing.cn

[Q14] 存在则更新（upsert）
来源：http://ry.jctech888.com.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://yc.haigaiapp.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://gt.lnxyls.cn

[Q15] 查询全部
来源：http://om.nicolike.cn

SELECT * FROM users;
来源：http://hb.9csxet.cn

[Q16] 查询指定列
来源：http://ii.shtwfgs.cn

SELECT id, name FROM users;
来源：http://nv.newstarts.cn

[Q17] 条件查询
来源：http://cj.shtwfgs.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://vg.huixiangedu.cn

[Q18] 模糊匹配
来源：http://gt.bookmarksfly.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://bn.asd995.cn

[Q19] 范围查询
来源：http://uv.yuexingan06.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://lg.jctech888.com.cn

[Q20] IN 列表
来源：http://yi.muxihuayi.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ly.shxzskj.cn

[Q21] 空值判断
来源：http://ln.nicolike.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://po.jianghongdianzi.cn

[Q22] 排序
来源：http://nc.muxihuayi.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://cv.521024.cn

[Q23] 分页
来源：http://bd.shxzukj.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wf.newstarts.cn

[Q24] 去重
来源：http://od.panjiajie.cn

SELECT DISTINCT city FROM users;
来源：http://xm.jianghongdianzi.cn

[Q25] 只取前 N 条
来源：http://hb.muxihuayi.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://fi.wgjwhj.cn

[Q26] 计数
来源：http://xh.jianghongdianzi.cn

SELECT COUNT(*) FROM users;
来源：http://cd.jianghongdianzi.cn

[Q27] 条件计数
来源：http://de.hnjuh.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://zz.9csxet.cn

[Q28] 求和与平均
来源：http://gt.bookmarksfly.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://cg.hnjuh.cn

[Q29] 最大最小值
来源：http://vr.huixiangedu.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://kg.colortex.cn

[Q30] 分组统计
来源：http://gv.nszjky.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://tj.shxzskj.cn

[Q31] 分组后过滤
来源：http://sj.colortex.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://vz.shtwfgs.cn

[Q32] 分组拼接字符串
来源：http://of.wgjwhj.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://nm.szsharing.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://lv.panjiajie.cn

[Q33] 多列分组
来源：http://ef.szsharing.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ly.chemitech.net.cn

[Q34] 每组取第一条
来源：http://tu.huixinmuqiang.cn

SELECT * FROM (
来源：http://hp.bookmarksfly.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://tp.panjiajie.cn

) t WHERE rn = 1;
来源：http://lo.nszjky.cn

[Q35] 内连接
来源：http://jn.hnjuh.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://th.haigaiapp.cn

[Q36] 左连接
来源：http://xz.521024.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ou.asd995.cn

[Q37] 右连接
来源：http://bj.jctech888.com.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://sp.gzmigu.cn

[Q38] 全外连接（PostgreSQL）
来源：http://co.hahajie.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://fo.shtwfgs.cn

[Q39] 自连接（查上下级）
来源：http://xt.asd995.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://zv.chemitech.net.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://xf.haigaiapp.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://ue.wgjwhj.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://gt.szxytkj.cn

[Q41] 多表连接
来源：http://sq.jctech888.com.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://km.lnxyls.cn

JOIN users u ON u.id = o.user_id
来源：http://me.huanxung.cn

JOIN products p ON p.id = o.product_id;
来源：http://mc.shxzukj.cn

[Q42] 连接条件附加过滤
来源：http://qx.colortex.cn

SELECT u.name, o.amount FROM users u
来源：http://rx.hahajie.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://pi.nszjky.cn

[Q43] 标量子查询
来源：http://af.huanxung.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://rg.jianghongdianzi.cn

[Q44] IN 子查询
来源：http://vi.haigaiapp.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ta.shxzukj.cn

[Q45] EXISTS 判断存在
来源：http://go.bookmarksfly.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ut.huixinmuqiang.cn

[Q46] NOT EXISTS 判断不存在
来源：http://re.huanxung.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://qp.bjjhwx.cn

[Q47] 与平均值比较
来源：http://yw.lnxyls.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ij.lnxyls.cn

[Q48] CTE 公用表表达式
来源：http://eh.huixinmuqiang.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ly.huixiangedu.cn

SELECT * FROM t WHERE c > 5;
来源：http://tg.9csxet.cn

[Q49] 更新单行
来源：http://yh.szsharing.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://jh.bjjhwx.cn

[Q50] 批量更新
来源：http://rw.jctech888.com.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://xr.nicolike.cn

[Q51] 用子查询更新
来源：http://on.haigaiapp.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://kh.shxzskj.cn

[Q52] 删除指定行
来源：http://bc.szsharing.cn

DELETE FROM users WHERE id = 10;
来源：http://ir.yuexingan06.cn

[Q53] 按条件删除
来源：http://md.shxzskj.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://rr.jctech888.com.cn

[Q54] 清空表
来源：http://nc.9csxet.cn

TRUNCATE TABLE logs;
来源：http://fu.bjjhwx.cn

[Q55] 排名（并列占位）
来源：http://pt.jctech888.com.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://yj.newstarts.cn

[Q56] 密集排名（并列不占位）
来源：http://tx.asd995.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://om.lnxyls.cn

[Q57] 行号
来源：http://mb.szxytkj.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://re.asd995.cn

[Q58] 累计求和
来源：http://vc.jianghongdianzi.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://kh.shxzskj.cn

[Q59] 分组内累计
来源：http://ng.jianghongdianzi.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://fq.colortex.cn

[Q60] 取上一行 / 下一行
来源：http://xr.jianghongdianzi.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://nd.szsharing.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://gc.shtwfgs.cn

[Q61] 移动平均
来源：http://wf.nszjky.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://xo.bookmarksfly.cn

[Q62] 分组占比
来源：http://ik.hahajie.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ru.shxzskj.cn

[Q63] 开启事务
来源：http://lr.huixinmuqiang.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://qi.jianghongdianzi.cn

[Q64] 提交事务
来源：http://tw.wgjwhj.cn

COMMIT;
来源：http://br.wgjwhj.cn

[Q65] 回滚事务
来源：http://ia.wgjwhj.cn

ROLLBACK;
来源：http://oh.muxihuayi.cn

[Q66] 行锁查询
来源：http://lk.panjiajie.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://gx.szsharing.cn

[Q67] 设置隔离级别
来源：http://xf.muxihuayi.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hs.huixinmuqiang.cn

[Q68] 保存点
来源：http://ed.wgjwhj.cn

SAVEPOINT sp1;
来源：http://og.newstarts.cn

ROLLBACK TO sp1;
来源：http://uj.muxihuayi.cn

[Q69] 查看执行计划
来源：http://rw.yuntaijiaju.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hk.bookmarksfly.cn

[Q70] 更新统计信息
来源：http://xo.521024.cn

ANALYZE TABLE users;
来源：http://wm.colortex.cn

[Q71] 查看建表语句
来源：http://ul.szsharing.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.haigaiapp.cn

[Q72] 查看索引
来源：http://xg.521024.cn

SHOW INDEX FROM users;
来源：http://es.bookmarksfly.cn

[Q73] 查看表状态
来源：http://ke.shtwfgs.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://zz.szxytkj.cn

[Q74] 强制使用索引
来源：http://vp.yuexingan06.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mr.lnxyls.cn

[Q75] 日期格式化
来源：http://wj.bjjhwx.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://uf.colortex.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://pb.panjiajie.cn

[Q76] 按天统计
来源：http://tx.huanxung.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://nu.yuntaijiaju.cn

[Q77] 时间加减
来源：http://ce.colortex.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://pd.haigaiapp.cn

[Q78] 当前时间
来源：http://ug.asd995.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://nb.colortex.cn

[Q79] 字符串拼接
来源：http://ut.panjiajie.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hj.shxzskj.cn

[Q80] 字符串截取
来源：http://lj.shtwfgs.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://oy.9csxet.cn

[Q81] 字符串替换
来源：http://ru.jianghongdianzi.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://uy.hnjuh.cn

[Q82] 字符长度与字节长度
来源：http://rp.newstarts.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mz.huanxung.cn

[Q83] 大小写转换
来源：http://tj.gzmigu.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://sh.chemitech.net.cn

[Q84] 去除首尾空格
来源：http://ex.hnjuh.cn

SELECT TRIM(name) FROM users;
来源：http://ib.shtwfgs.cn

[Q85] 数值取整
来源：http://hw.colortex.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ca.521024.cn

[Q86] 读取 JSON 字段
来源：http://st.521024.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://kt.jctech888.com.cn

[Q87] JSON 字段做条件
来源：http://al.huixinmuqiang.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ja.yuexingan06.cn

[Q88] 行转列（条件聚合）
来源：http://sk.shtwfgs.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://zy.huanxung.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://tt.nszjky.cn

[Q89] 判断表是否存在
来源：http://qh.shxzukj.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hr.nszjky.cn

[Q90] 生成序号列
来源：http://mb.szxytkj.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://kf.hnjuh.cn

================================================================================
来源：http://ch.huanxung.cn

R. Bash 专题
来源：http://rd.yuexingan06.cn

================================================================================
来源：http://ch.nszjky.cn

[R01] shebang 与严格模式
来源：http://tt.shxzskj.cn

#!/usr/bin/env bash
来源：http://ca.asd995.cn

set -euo pipefail
来源：http://ak.haigaiapp.cn

[R02] 变量赋值与使用
来源：http://me.panjiajie.cn

name="Tom"; echo "$name"
来源：http://ac.chemitech.net.cn

[R03] 只读变量
来源：http://bn.newstarts.cn

readonly PI=3.14
来源：http://ym.shxzskj.cn

[R04] 位置参数
来源：http://ga.bookmarksfly.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://uj.huixiangedu.cn

[R05] 参数默认值
来源：http://nv.szsharing.cn

name="${1:-default}"
来源：http://tr.jctech888.com.cn

[R06] 判断命令是否存在
来源：http://ss.9csxet.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hr.chemitech.net.cn

[R07] if 判断文件
来源：http://pi.huixiangedu.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://pr.wgjwhj.cn

[R08] 数值比较
来源：http://nj.521024.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://go.colortex.cn

[R09] 字符串比较
来源：http://pr.colortex.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ee.wgjwhj.cn

[R10] 正则匹配
来源：http://sz.nicolike.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://jq.shxzukj.cn

[R11] case 多分支
来源：http://wq.shtwfgs.cn

case "$1" in
来源：http://bm.newstarts.cn

start) echo "启动" ;;
来源：http://ay.9csxet.cn

stop)  echo "停止" ;;
来源：http://sv.lnxyls.cn

*)     echo "未知命令" ;;
来源：http://br.jianghongdianzi.cn

esac
来源：http://sc.huixinmuqiang.cn

[R12] for 遍历文件
来源：http://fy.gzmigu.cn

for f in *.txt; do echo "$f"; done
来源：http://xf.huixinmuqiang.cn

[R13] for 计数循环
来源：http://bs.bookmarksfly.cn

for i in {1..10}; do echo "$i"; done
来源：http://eh.bjjhwx.cn

[R14] C 风格 for
来源：http://rd.lnxyls.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://jb.muxihuayi.cn

[R15] while 逐行读文件
来源：http://gr.huixinmuqiang.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://eo.9csxet.cn

[R16] until 等待条件
来源：http://fl.szsharing.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ps.colortex.cn

[R17] 数组定义与取值
来源：http://io.huixinmuqiang.cn

arr=(a b c); echo "${arr[0]}"
来源：http://yi.chemitech.net.cn

[R18] 遍历数组
来源：http://gv.shxzskj.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://sh.shxzukj.cn

[R19] 数组长度
来源：http://xw.chemitech.net.cn


<!-- 参考信息 -->