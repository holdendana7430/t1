代发 wailian999

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://jd.nszjky.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://sy.jianghongdianzi.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://pa.szsharing.cn

[P04] 求长度
来源：http://ta.gzmigu.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://vj.muxihuayi.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ej.asd995.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://qb.lnxyls.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://lr.hahajie.cn

Java: list.size();  map.size();  s.length()
来源：http://cx.szsharing.cn

Go:   len(arr);  len(m)
来源：http://jg.hnjuh.cn

Ruby: x.length;  x.size
来源：http://nz.chemitech.net.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://sj.colortex.cn

[P05] 判断两个对象内容是否相等
来源：http://lx.szsharing.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://rx.jianghongdianzi.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mb.jianghongdianzi.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://te.muxihuayi.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://kb.huixinmuqiang.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ny.jctech888.com.cn

Go:   reflect.DeepEqual(a, b)
来源：http://by.hahajie.cn

Ruby: a == b
来源：http://gt.lnxyls.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://tw.asd995.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wh.521024.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://qc.panjiajie.cn

PHP:  if (empty($x)) {}
来源：http://ql.bjjhwx.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://vy.lnxyls.cn

TS:   if (x == null) {}
来源：http://mv.haigaiapp.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://vo.panjiajie.cn

Go:   if x == nil {}
来源：http://ow.colortex.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mj.hnjuh.cn

C#:   if (x is null) {}
来源：http://qq.panjiajie.cn

[P07] 防抖与节流
来源：http://sd.panjiajie.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://fa.huixinmuqiang.cn

PHP:  // 手写时间戳比较
来源：http://dk.yuntaijiaju.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://gv.colortex.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wz.muxihuayi.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://jr.szxytkj.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://oa.huixiangedu.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://uu.shxzskj.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ie.wgjwhj.cn

[P08] 处理浮点精度问题
来源：http://mj.huixiangedu.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://jl.colortex.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ge.newstarts.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ps.lnxyls.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wh.chemitech.net.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://pc.gzmigu.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://qb.shxzskj.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ep.521024.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://cf.hahajie.cn

================================================================================
来源：http://yv.shxzskj.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://tz.jianghongdianzi.cn

================================================================================
来源：http://qm.chemitech.net.cn

[Q01] 创建表
来源：http://sn.521024.cn

CREATE TABLE users (
来源：http://fz.huixiangedu.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ds.haigaiapp.cn

name VARCHAR(50) NOT NULL,
来源：http://ph.huixinmuqiang.cn

email VARCHAR(100) UNIQUE,
来源：http://qk.szxytkj.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://xb.nicolike.cn

);
来源：http://ud.jianghongdianzi.cn

[Q02] 创建带外键的表
来源：http://wv.shxzskj.cn

CREATE TABLE orders (
来源：http://uu.jianghongdianzi.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://vq.yuntaijiaju.cn

user_id INT NOT NULL,
来源：http://nm.bookmarksfly.cn

amount DECIMAL(10, 2),
来源：http://bs.huixiangedu.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://md.yuexingan06.cn

);
来源：http://rt.nszjky.cn

[Q03] 增加列
来源：http://nk.szsharing.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://cy.lnxyls.cn

[Q04] 修改列类型
来源：http://ti.shxzskj.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://qb.colortex.cn

[Q05] 重命名列
来源：http://ut.szxytkj.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://gu.bookmarksfly.cn

[Q06] 删除列
来源：http://yz.hahajie.cn

ALTER TABLE users DROP COLUMN age;
来源：http://dm.wgjwhj.cn

[Q07] 删除表
来源：http://kt.yuexingan06.cn

DROP TABLE IF EXISTS orders;
来源：http://kx.bookmarksfly.cn

[Q08] 创建普通索引
来源：http://pm.muxihuayi.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://pc.huixinmuqiang.cn

[Q09] 创建唯一索引
来源：http://ha.szsharing.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://om.jianghongdianzi.cn

[Q10] 插入单行
来源：http://ep.bookmarksfly.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://pi.colortex.cn

[Q11] 一次插入多行
来源：http://cs.jianghongdianzi.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wu.panjiajie.cn

[Q12] 插入后取自增 ID
来源：http://cf.jctech888.com.cn

INSERT INTO users (name) VALUES ('C');
来源：http://zk.muxihuayi.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ei.nszjky.cn

[Q13] 忽略重复插入
来源：http://cd.shxzskj.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://qi.asd995.cn

[Q14] 存在则更新（upsert）
来源：http://ab.shtwfgs.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://yk.jctech888.com.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://xd.yuexingan06.cn

[Q15] 查询全部
来源：http://vw.szxytkj.cn

SELECT * FROM users;
来源：http://ax.nicolike.cn

[Q16] 查询指定列
来源：http://fn.jianghongdianzi.cn

SELECT id, name FROM users;
来源：http://nx.hahajie.cn

[Q17] 条件查询
来源：http://vv.521024.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mi.shxzskj.cn

[Q18] 模糊匹配
来源：http://kt.huixinmuqiang.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://yo.huanxung.cn

[Q19] 范围查询
来源：http://mc.jianghongdianzi.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://gy.szsharing.cn

[Q20] IN 列表
来源：http://ra.szxytkj.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://rc.huanxung.cn

[Q21] 空值判断
来源：http://sc.colortex.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://gj.muxihuayi.cn

[Q22] 排序
来源：http://mi.lnxyls.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ym.yuexingan06.cn

[Q23] 分页
来源：http://cw.521024.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://je.huixinmuqiang.cn

[Q24] 去重
来源：http://ax.wgjwhj.cn

SELECT DISTINCT city FROM users;
来源：http://zu.yuntaijiaju.cn

[Q25] 只取前 N 条
来源：http://ki.wgjwhj.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://or.shxzskj.cn

[Q26] 计数
来源：http://qw.hnjuh.cn

SELECT COUNT(*) FROM users;
来源：http://be.panjiajie.cn

[Q27] 条件计数
来源：http://cz.nicolike.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ah.hahajie.cn

[Q28] 求和与平均
来源：http://lq.shxzukj.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://jy.newstarts.cn

[Q29] 最大最小值
来源：http://sv.shxzskj.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://ks.asd995.cn

[Q30] 分组统计
来源：http://iu.yuexingan06.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://qn.yuntaijiaju.cn

[Q31] 分组后过滤
来源：http://hg.huanxung.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://be.panjiajie.cn

[Q32] 分组拼接字符串
来源：http://bg.haigaiapp.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://gc.haigaiapp.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://bc.jctech888.com.cn

[Q33] 多列分组
来源：http://cz.yuexingan06.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://iq.muxihuayi.cn

[Q34] 每组取第一条
来源：http://fk.9csxet.cn

SELECT * FROM (
来源：http://oc.521024.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://yj.yuexingan06.cn

) t WHERE rn = 1;
来源：http://of.szxytkj.cn

[Q35] 内连接
来源：http://bh.muxihuayi.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hf.bjjhwx.cn

[Q36] 左连接
来源：http://cc.yuexingan06.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://pr.shxzukj.cn

[Q37] 右连接
来源：http://xl.shtwfgs.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ph.chemitech.net.cn

[Q38] 全外连接（PostgreSQL）
来源：http://fa.yuntaijiaju.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://gm.huanxung.cn

[Q39] 自连接（查上下级）
来源：http://yw.bookmarksfly.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://ik.huixiangedu.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://tz.panjiajie.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://ls.nszjky.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://kb.9csxet.cn

[Q41] 多表连接
来源：http://kn.nicolike.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://mp.gzmigu.cn

JOIN users u ON u.id = o.user_id
来源：http://ws.wgjwhj.cn

JOIN products p ON p.id = o.product_id;
来源：http://xl.panjiajie.cn

[Q42] 连接条件附加过滤
来源：http://at.szsharing.cn

SELECT u.name, o.amount FROM users u
来源：http://kc.shtwfgs.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://yv.szsharing.cn

[Q43] 标量子查询
来源：http://rm.shxzskj.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://bz.muxihuayi.cn

[Q44] IN 子查询
来源：http://gy.szsharing.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://gf.yuexingan06.cn

[Q45] EXISTS 判断存在
来源：http://tr.chemitech.net.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://cx.shtwfgs.cn

[Q46] NOT EXISTS 判断不存在
来源：http://lh.bookmarksfly.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://cx.gzmigu.cn

[Q47] 与平均值比较
来源：http://ff.szsharing.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://up.bookmarksfly.cn

[Q48] CTE 公用表表达式
来源：http://nj.chemitech.net.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://sn.colortex.cn

SELECT * FROM t WHERE c > 5;
来源：http://zb.yuexingan06.cn

[Q49] 更新单行
来源：http://uy.521024.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://dv.gzmigu.cn

[Q50] 批量更新
来源：http://br.nicolike.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://rq.jianghongdianzi.cn

[Q51] 用子查询更新
来源：http://bh.szsharing.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://af.hahajie.cn

[Q52] 删除指定行
来源：http://kt.9csxet.cn

DELETE FROM users WHERE id = 10;
来源：http://ta.wgjwhj.cn

[Q53] 按条件删除
来源：http://fz.asd995.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://yg.huixiangedu.cn

[Q54] 清空表
来源：http://yk.hnjuh.cn

TRUNCATE TABLE logs;
来源：http://mn.nicolike.cn

[Q55] 排名（并列占位）
来源：http://ax.huanxung.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ca.huixinmuqiang.cn

[Q56] 密集排名（并列不占位）
来源：http://ph.yuntaijiaju.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://va.muxihuayi.cn

[Q57] 行号
来源：http://et.shxzskj.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mp.haigaiapp.cn

[Q58] 累计求和
来源：http://pj.szxytkj.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://zj.9csxet.cn

[Q59] 分组内累计
来源：http://lf.hnjuh.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://im.nicolike.cn

[Q60] 取上一行 / 下一行
来源：http://ye.szxytkj.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://pw.9csxet.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://gw.haigaiapp.cn

[Q61] 移动平均
来源：http://ou.szxytkj.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://io.szxytkj.cn

[Q62] 分组占比
来源：http://gd.panjiajie.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ot.bjjhwx.cn

[Q63] 开启事务
来源：http://kv.521024.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://pn.9csxet.cn

[Q64] 提交事务
来源：http://kj.hahajie.cn

COMMIT;
来源：http://dk.bookmarksfly.cn

[Q65] 回滚事务
来源：http://yq.huixinmuqiang.cn

ROLLBACK;
来源：http://ke.bookmarksfly.cn

[Q66] 行锁查询
来源：http://pv.jianghongdianzi.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://uq.asd995.cn

[Q67] 设置隔离级别
来源：http://ov.yuntaijiaju.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://st.muxihuayi.cn

[Q68] 保存点
来源：http://ky.newstarts.cn

SAVEPOINT sp1;
来源：http://pg.lnxyls.cn

ROLLBACK TO sp1;
来源：http://cz.shxzukj.cn

[Q69] 查看执行计划
来源：http://mj.szsharing.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hb.521024.cn

[Q70] 更新统计信息
来源：http://tj.jianghongdianzi.cn

ANALYZE TABLE users;
来源：http://ro.hahajie.cn

[Q71] 查看建表语句
来源：http://ss.newstarts.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://bj.9csxet.cn

[Q72] 查看索引
来源：http://am.yuexingan06.cn

SHOW INDEX FROM users;
来源：http://vf.nicolike.cn

[Q73] 查看表状态
来源：http://jg.521024.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://am.521024.cn

[Q74] 强制使用索引
来源：http://ur.shxzukj.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ea.hahajie.cn

[Q75] 日期格式化
来源：http://xa.panjiajie.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://vg.jctech888.com.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://xc.bookmarksfly.cn

[Q76] 按天统计
来源：http://hl.yuexingan06.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://co.huixiangedu.cn

[Q77] 时间加减
来源：http://px.muxihuayi.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://sx.chemitech.net.cn

[Q78] 当前时间
来源：http://iy.panjiajie.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ba.huixiangedu.cn

[Q79] 字符串拼接
来源：http://bc.shxzskj.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://le.bookmarksfly.cn

[Q80] 字符串截取
来源：http://jy.9csxet.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://qo.panjiajie.cn

[Q81] 字符串替换
来源：http://yh.szsharing.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hj.szsharing.cn

[Q82] 字符长度与字节长度
来源：http://hw.lnxyls.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://lk.colortex.cn

[Q83] 大小写转换
来源：http://wx.shxzskj.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://dq.newstarts.cn

[Q84] 去除首尾空格
来源：http://nk.asd995.cn

SELECT TRIM(name) FROM users;
来源：http://jf.muxihuayi.cn

[Q85] 数值取整
来源：http://ev.huixinmuqiang.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://bw.haigaiapp.cn

[Q86] 读取 JSON 字段
来源：http://rz.yuntaijiaju.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://cs.haigaiapp.cn

[Q87] JSON 字段做条件
来源：http://ok.bookmarksfly.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://cd.newstarts.cn

[Q88] 行转列（条件聚合）
来源：http://mm.haigaiapp.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://lm.hnjuh.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://be.muxihuayi.cn

[Q89] 判断表是否存在
来源：http://ro.huixiangedu.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://qq.huanxung.cn

[Q90] 生成序号列
来源：http://ub.asd995.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://un.nszjky.cn

================================================================================
来源：http://tt.muxihuayi.cn

R. Bash 专题
来源：http://vc.muxihuayi.cn

================================================================================
来源：http://bj.wgjwhj.cn

[R01] shebang 与严格模式
来源：http://gj.nszjky.cn

#!/usr/bin/env bash
来源：http://gg.haigaiapp.cn

set -euo pipefail
来源：http://of.colortex.cn

[R02] 变量赋值与使用
来源：http://dj.huixiangedu.cn

name="Tom"; echo "$name"
来源：http://ep.hnjuh.cn

[R03] 只读变量
来源：http://zq.huixiangedu.cn

readonly PI=3.14
来源：http://pi.521024.cn

[R04] 位置参数
来源：http://xr.yuexingan06.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://zy.jianghongdianzi.cn

[R05] 参数默认值
来源：http://cq.nszjky.cn

name="${1:-default}"
来源：http://mw.gzmigu.cn

[R06] 判断命令是否存在
来源：http://qj.panjiajie.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://jc.521024.cn

[R07] if 判断文件
来源：http://dx.hnjuh.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mc.yuntaijiaju.cn

[R08] 数值比较
来源：http://zv.panjiajie.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://fb.lnxyls.cn

[R09] 字符串比较
来源：http://va.shtwfgs.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ai.shxzukj.cn

[R10] 正则匹配
来源：http://yd.colortex.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://rd.nszjky.cn

[R11] case 多分支
来源：http://sv.colortex.cn

case "$1" in
来源：http://se.colortex.cn

start) echo "启动" ;;
来源：http://nl.shxzskj.cn

stop)  echo "停止" ;;
来源：http://dv.panjiajie.cn

*)     echo "未知命令" ;;
来源：http://wg.wgjwhj.cn

esac
来源：http://wn.shtwfgs.cn

[R12] for 遍历文件
来源：http://ql.jianghongdianzi.cn

for f in *.txt; do echo "$f"; done
来源：http://wl.panjiajie.cn

[R13] for 计数循环
来源：http://lt.huanxung.cn

for i in {1..10}; do echo "$i"; done
来源：http://jj.shxzskj.cn

[R14] C 风格 for
来源：http://cj.nszjky.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mp.haigaiapp.cn

[R15] while 逐行读文件
来源：http://wi.shxzskj.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://az.wgjwhj.cn

[R16] until 等待条件
来源：http://mn.colortex.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://di.521024.cn

[R17] 数组定义与取值
来源：http://mb.szxytkj.cn

arr=(a b c); echo "${arr[0]}"
来源：http://in.nszjky.cn

[R18] 遍历数组
来源：http://lp.yuexingan06.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://gw.szsharing.cn

[R19] 数组长度
来源：http://sq.haigaiapp.cn


<!-- 参考信息 -->