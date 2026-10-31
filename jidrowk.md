代发 wailian999

Py:   asyncio.gather(*tasks)
来源：http://wh.jctech888.com.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://tl.bjjhwx.cn

JS:   await Promise.all(tasks)
来源：http://mw.yuntaijiaju.cn

TS:   await Promise.all(tasks)
来源：http://xt.asd995.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://zb.muxihuayi.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://qq.9csxet.cn

Ruby: threads.map(&:join)
来源：http://ti.yuexingan06.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://it.hnjuh.cn

[O06] 使用进程池
来源：http://dh.newstarts.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://fa.nicolike.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://nu.gzmigu.cn

JS:   // child_process / cluster 模块
来源：http://mm.wgjwhj.cn

TS:   // child_process / cluster 模块
来源：http://we.wgjwhj.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://yu.nicolike.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://fg.lnxyls.cn

Ruby: // fork 块
来源：http://fg.bookmarksfly.cn

C#:   Parallel.For
来源：http://ak.asd995.cn

================================================================================
来源：http://du.bookmarksfly.cn

P. 常用工具函数
来源：http://ef.bookmarksfly.cn

================================================================================
来源：http://zz.jctech888.com.cn

[P01] 生成 UUID
来源：http://vz.lnxyls.cn

Py:   str(uuid.uuid4())
来源：http://gn.haigaiapp.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hi.shxzskj.cn

JS:   crypto.randomUUID()
来源：http://br.szsharing.cn

TS:   crypto.randomUUID()
来源：http://dk.lnxyls.cn

Java: UUID.randomUUID().toString()
来源：http://oh.muxihuayi.cn

Go:   // 用 github.com/google/uuid
来源：http://yk.haigaiapp.cn

Ruby: SecureRandom.uuid
来源：http://xw.panjiajie.cn

C#:   Guid.NewGuid().ToString()
来源：http://rj.bookmarksfly.cn

[P02] MD5 / SHA256 摘要
来源：http://cm.huanxung.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://dn.chemitech.net.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://he.chemitech.net.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://zb.521024.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://vu.nszjky.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://du.hahajie.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://tx.panjiajie.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://le.szxytkj.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://jj.jianghongdianzi.cn

[P03] 生成短随机字符串
来源：http://pm.hnjuh.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://px.nszjky.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://zp.panjiajie.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://dw.muxihuayi.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://bq.bjjhwx.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://rg.panjiajie.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://kt.jianghongdianzi.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://dw.9csxet.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://rs.nszjky.cn

[P04] 求长度
来源：http://ql.521024.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://kk.haigaiapp.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ag.nicolike.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://db.gzmigu.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://kb.nicolike.cn

Java: list.size();  map.size();  s.length()
来源：http://rg.newstarts.cn

Go:   len(arr);  len(m)
来源：http://rd.shtwfgs.cn

Ruby: x.length;  x.size
来源：http://qp.nszjky.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://pe.9csxet.cn

[P05] 判断两个对象内容是否相等
来源：http://zc.gzmigu.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://ff.newstarts.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://sa.hnjuh.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://gm.chemitech.net.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ck.shtwfgs.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://kf.yuntaijiaju.cn

Go:   reflect.DeepEqual(a, b)
来源：http://yh.jianghongdianzi.cn

Ruby: a == b
来源：http://gl.gzmigu.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://bp.521024.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wz.jctech888.com.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://al.haigaiapp.cn

PHP:  if (empty($x)) {}
来源：http://zq.lnxyls.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hu.muxihuayi.cn

TS:   if (x == null) {}
来源：http://kf.bjjhwx.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://lh.chemitech.net.cn

Go:   if x == nil {}
来源：http://uz.shtwfgs.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://xv.bookmarksfly.cn

C#:   if (x is null) {}
来源：http://mu.huixiangedu.cn

[P07] 防抖与节流
来源：http://ub.jianghongdianzi.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://id.huixiangedu.cn

PHP:  // 手写时间戳比较
来源：http://rh.nicolike.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hy.wgjwhj.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://bp.jianghongdianzi.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://fz.panjiajie.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://zh.newstarts.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://wq.huanxung.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://dw.bookmarksfly.cn

[P08] 处理浮点精度问题
来源：http://mk.yuexingan06.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://yl.nicolike.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://vb.szxytkj.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://dq.szxytkj.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://xi.nszjky.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://rt.shxzukj.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mr.colortex.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://em.colortex.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://vt.haigaiapp.cn

================================================================================
来源：http://yx.yuexingan06.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://uu.shxzukj.cn

================================================================================
来源：http://lg.shtwfgs.cn

[Q01] 创建表
来源：http://er.hnjuh.cn

CREATE TABLE users (
来源：http://om.9csxet.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ur.yuntaijiaju.cn

name VARCHAR(50) NOT NULL,
来源：http://im.nszjky.cn

email VARCHAR(100) UNIQUE,
来源：http://tt.hahajie.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://jd.huixiangedu.cn

);
来源：http://ca.shxzskj.cn

[Q02] 创建带外键的表
来源：http://fa.wgjwhj.cn

CREATE TABLE orders (
来源：http://bl.hahajie.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://br.nszjky.cn

user_id INT NOT NULL,
来源：http://ea.shxzskj.cn

amount DECIMAL(10, 2),
来源：http://ux.jctech888.com.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://bp.shxzskj.cn

);
来源：http://kb.panjiajie.cn

[Q03] 增加列
来源：http://ea.asd995.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://yn.nszjky.cn

[Q04] 修改列类型
来源：http://uu.colortex.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://pb.huixinmuqiang.cn

[Q05] 重命名列
来源：http://di.nszjky.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wv.nicolike.cn

[Q06] 删除列
来源：http://sy.yuntaijiaju.cn

ALTER TABLE users DROP COLUMN age;
来源：http://ts.bookmarksfly.cn

[Q07] 删除表
来源：http://yp.wgjwhj.cn

DROP TABLE IF EXISTS orders;
来源：http://tv.colortex.cn

[Q08] 创建普通索引
来源：http://be.yuntaijiaju.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://cw.shxzskj.cn

[Q09] 创建唯一索引
来源：http://bn.nszjky.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ae.jianghongdianzi.cn

[Q10] 插入单行
来源：http://oh.hnjuh.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://lt.newstarts.cn

[Q11] 一次插入多行
来源：http://rp.521024.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://lf.521024.cn

[Q12] 插入后取自增 ID
来源：http://pu.lnxyls.cn

INSERT INTO users (name) VALUES ('C');
来源：http://sp.chemitech.net.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://kl.hahajie.cn

[Q13] 忽略重复插入
来源：http://cr.521024.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://yg.shxzukj.cn

[Q14] 存在则更新（upsert）
来源：http://ar.gzmigu.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ge.chemitech.net.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ms.nicolike.cn

[Q15] 查询全部
来源：http://ak.muxihuayi.cn

SELECT * FROM users;
来源：http://gh.colortex.cn

[Q16] 查询指定列
来源：http://rd.wgjwhj.cn

SELECT id, name FROM users;
来源：http://iu.huixinmuqiang.cn

[Q17] 条件查询
来源：http://ym.asd995.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://td.hnjuh.cn

[Q18] 模糊匹配
来源：http://zb.wgjwhj.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://sb.muxihuayi.cn

[Q19] 范围查询
来源：http://mw.hahajie.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://qt.jctech888.com.cn

[Q20] IN 列表
来源：http://gi.9csxet.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://de.shxzskj.cn

[Q21] 空值判断
来源：http://kl.panjiajie.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://hb.newstarts.cn

[Q22] 排序
来源：http://yi.hahajie.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://cv.shtwfgs.cn

[Q23] 分页
来源：http://du.muxihuayi.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ki.panjiajie.cn

[Q24] 去重
来源：http://km.nicolike.cn

SELECT DISTINCT city FROM users;
来源：http://ow.muxihuayi.cn

[Q25] 只取前 N 条
来源：http://sf.huanxung.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://nl.lnxyls.cn

[Q26] 计数
来源：http://ca.jianghongdianzi.cn

SELECT COUNT(*) FROM users;
来源：http://sk.asd995.cn

[Q27] 条件计数
来源：http://ze.shxzskj.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://tu.521024.cn

[Q28] 求和与平均
来源：http://sm.nicolike.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mo.huixiangedu.cn

[Q29] 最大最小值
来源：http://xf.muxihuayi.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://et.asd995.cn

[Q30] 分组统计
来源：http://sd.521024.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ir.jctech888.com.cn

[Q31] 分组后过滤
来源：http://ck.szxytkj.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ln.colortex.cn

[Q32] 分组拼接字符串
来源：http://hn.shxzskj.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://my.hahajie.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://qu.nszjky.cn

[Q33] 多列分组
来源：http://re.jctech888.com.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://xb.haigaiapp.cn

[Q34] 每组取第一条
来源：http://aa.yuntaijiaju.cn

SELECT * FROM (
来源：http://bl.yuexingan06.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://xy.szsharing.cn

) t WHERE rn = 1;
来源：http://ux.nszjky.cn

[Q35] 内连接
来源：http://aa.shxzukj.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wn.lnxyls.cn

[Q36] 左连接
来源：http://sk.szsharing.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://qt.hahajie.cn

[Q37] 右连接
来源：http://gi.jctech888.com.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://bb.szxytkj.cn

[Q38] 全外连接（PostgreSQL）
来源：http://bg.shxzukj.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://zg.hnjuh.cn

[Q39] 自连接（查上下级）
来源：http://it.panjiajie.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://wv.gzmigu.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://xc.gzmigu.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://sk.hnjuh.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://so.szxytkj.cn

[Q41] 多表连接
来源：http://pi.haigaiapp.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://qw.yuntaijiaju.cn

JOIN users u ON u.id = o.user_id
来源：http://dn.wgjwhj.cn

JOIN products p ON p.id = o.product_id;
来源：http://uv.jctech888.com.cn

[Q42] 连接条件附加过滤
来源：http://ad.chemitech.net.cn

SELECT u.name, o.amount FROM users u
来源：http://dx.huanxung.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://yt.wgjwhj.cn

[Q43] 标量子查询
来源：http://bv.yuntaijiaju.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://dy.bookmarksfly.cn

[Q44] IN 子查询
来源：http://yg.9csxet.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://fq.shxzskj.cn

[Q45] EXISTS 判断存在
来源：http://qz.szxytkj.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://uh.szxytkj.cn

[Q46] NOT EXISTS 判断不存在
来源：http://yp.nicolike.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://jz.shxzskj.cn

[Q47] 与平均值比较
来源：http://is.panjiajie.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://nc.huanxung.cn

[Q48] CTE 公用表表达式
来源：http://ee.shxzskj.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://yg.muxihuayi.cn

SELECT * FROM t WHERE c > 5;
来源：http://nc.jctech888.com.cn

[Q49] 更新单行
来源：http://ab.muxihuayi.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://vt.yuntaijiaju.cn

[Q50] 批量更新
来源：http://yw.huixinmuqiang.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://ie.bjjhwx.cn

[Q51] 用子查询更新
来源：http://py.yuexingan06.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://nq.szsharing.cn

[Q52] 删除指定行
来源：http://kt.colortex.cn

DELETE FROM users WHERE id = 10;
来源：http://oe.newstarts.cn

[Q53] 按条件删除
来源：http://zn.chemitech.net.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://xg.muxihuayi.cn

[Q54] 清空表
来源：http://af.jctech888.com.cn

TRUNCATE TABLE logs;
来源：http://rx.asd995.cn

[Q55] 排名（并列占位）
来源：http://pr.muxihuayi.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ao.huanxung.cn

[Q56] 密集排名（并列不占位）
来源：http://nd.szxytkj.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ww.shxzukj.cn

[Q57] 行号
来源：http://ir.gzmigu.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://av.yuexingan06.cn

[Q58] 累计求和
来源：http://py.wgjwhj.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://rj.nicolike.cn

[Q59] 分组内累计
来源：http://gg.hnjuh.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://on.shtwfgs.cn

[Q60] 取上一行 / 下一行
来源：http://pp.nszjky.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://jf.521024.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://bt.huanxung.cn

[Q61] 移动平均
来源：http://qm.9csxet.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://vl.asd995.cn

[Q62] 分组占比
来源：http://av.szxytkj.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mm.chemitech.net.cn

[Q63] 开启事务
来源：http://du.huixiangedu.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://zc.szsharing.cn

[Q64] 提交事务
来源：http://js.huanxung.cn

COMMIT;
来源：http://vm.wgjwhj.cn

[Q65] 回滚事务
来源：http://ka.colortex.cn

ROLLBACK;
来源：http://go.shxzukj.cn

[Q66] 行锁查询
来源：http://gf.huixinmuqiang.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://cy.huixiangedu.cn

[Q67] 设置隔离级别
来源：http://ia.jianghongdianzi.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://fc.shxzukj.cn

[Q68] 保存点
来源：http://uq.yuntaijiaju.cn

SAVEPOINT sp1;
来源：http://zf.shxzskj.cn

ROLLBACK TO sp1;
来源：http://do.shtwfgs.cn

[Q69] 查看执行计划
来源：http://vg.wgjwhj.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://uc.shxzskj.cn

[Q70] 更新统计信息
来源：http://ml.huanxung.cn

ANALYZE TABLE users;
来源：http://yv.huixinmuqiang.cn

[Q71] 查看建表语句
来源：http://ex.jianghongdianzi.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://yj.panjiajie.cn

[Q72] 查看索引
来源：http://rr.jianghongdianzi.cn

SHOW INDEX FROM users;
来源：http://ey.szsharing.cn

[Q73] 查看表状态
来源：http://hi.panjiajie.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://nh.shxzskj.cn

[Q74] 强制使用索引
来源：http://pf.shxzskj.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://vo.nicolike.cn

[Q75] 日期格式化
来源：http://tf.shxzskj.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wp.nszjky.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mo.shtwfgs.cn

[Q76] 按天统计
来源：http://sk.shtwfgs.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://iu.bjjhwx.cn

[Q77] 时间加减
来源：http://sx.muxihuayi.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ww.hnjuh.cn

[Q78] 当前时间
来源：http://ug.wgjwhj.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://gl.huixiangedu.cn

[Q79] 字符串拼接
来源：http://bi.shtwfgs.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://el.huanxung.cn

[Q80] 字符串截取
来源：http://du.shxzskj.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ly.szxytkj.cn

[Q81] 字符串替换
来源：http://dc.lnxyls.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ya.nszjky.cn

[Q82] 字符长度与字节长度
来源：http://co.asd995.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://lm.gzmigu.cn

[Q83] 大小写转换
来源：http://sp.nszjky.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://qr.huixinmuqiang.cn

[Q84] 去除首尾空格
来源：http://jq.bookmarksfly.cn

SELECT TRIM(name) FROM users;
来源：http://nf.shxzskj.cn

[Q85] 数值取整
来源：http://le.shxzskj.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://qd.szsharing.cn

[Q86] 读取 JSON 字段
来源：http://fr.shtwfgs.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://qw.colortex.cn

[Q87] JSON 字段做条件
来源：http://fz.lnxyls.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://yh.shtwfgs.cn

[Q88] 行转列（条件聚合）
来源：http://wk.panjiajie.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://pw.lnxyls.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ck.bookmarksfly.cn

[Q89] 判断表是否存在
来源：http://kv.chemitech.net.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wd.shxzukj.cn

[Q90] 生成序号列
来源：http://qs.9csxet.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ph.nszjky.cn

================================================================================
来源：http://ie.521024.cn


<!-- 参考信息 -->