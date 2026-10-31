代发 wailian999

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ok.panjiajie.cn

JS:   async function f() { await g(); }
来源：http://es.9csxet.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://lw.gzmigu.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://zu.newstarts.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ml.yuexingan06.cn

Ruby: # 用 Fiber 或 async gem
来源：http://io.hahajie.cn

C#:   async Task F() { await G(); }
来源：http://wb.nicolike.cn

[O05] 并发执行并等待全部完成
来源：http://lq.shxzskj.cn

Py:   asyncio.gather(*tasks)
来源：http://wx.yuexingan06.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ca.jctech888.com.cn

JS:   await Promise.all(tasks)
来源：http://nd.shxzskj.cn

TS:   await Promise.all(tasks)
来源：http://vg.wgjwhj.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://vf.jianghongdianzi.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://zx.haigaiapp.cn

Ruby: threads.map(&:join)
来源：http://kh.hnjuh.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://de.9csxet.cn

[O06] 使用进程池
来源：http://tj.521024.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://sy.lnxyls.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://zk.haigaiapp.cn

JS:   // child_process / cluster 模块
来源：http://em.nicolike.cn

TS:   // child_process / cluster 模块
来源：http://gj.huixinmuqiang.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ei.yuntaijiaju.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://oo.newstarts.cn

Ruby: // fork 块
来源：http://ba.jianghongdianzi.cn

C#:   Parallel.For
来源：http://bu.nszjky.cn

================================================================================
来源：http://tb.hahajie.cn

P. 常用工具函数
来源：http://zz.haigaiapp.cn

================================================================================
来源：http://kv.muxihuayi.cn

[P01] 生成 UUID
来源：http://de.lnxyls.cn

Py:   str(uuid.uuid4())
来源：http://dn.jctech888.com.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://py.9csxet.cn

JS:   crypto.randomUUID()
来源：http://og.nicolike.cn

TS:   crypto.randomUUID()
来源：http://js.huanxung.cn

Java: UUID.randomUUID().toString()
来源：http://iy.shxzskj.cn

Go:   // 用 github.com/google/uuid
来源：http://gr.panjiajie.cn

Ruby: SecureRandom.uuid
来源：http://sd.hnjuh.cn

C#:   Guid.NewGuid().ToString()
来源：http://hq.521024.cn

[P02] MD5 / SHA256 摘要
来源：http://oq.chemitech.net.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://fj.colortex.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://wy.huixinmuqiang.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://lp.shxzukj.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://yc.huanxung.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ct.newstarts.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ew.shxzukj.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://su.szsharing.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://pp.panjiajie.cn

[P03] 生成短随机字符串
来源：http://vi.521024.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mm.colortex.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://sl.jianghongdianzi.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://xh.chemitech.net.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ww.shxzskj.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://vl.nszjky.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://go.yuexingan06.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://jt.asd995.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://bj.shxzskj.cn

[P04] 求长度
来源：http://yy.shxzskj.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://zq.szsharing.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://uf.muxihuayi.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://an.newstarts.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://zy.wgjwhj.cn

Java: list.size();  map.size();  s.length()
来源：http://mq.bjjhwx.cn

Go:   len(arr);  len(m)
来源：http://bj.newstarts.cn

Ruby: x.length;  x.size
来源：http://ej.bjjhwx.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://ns.lnxyls.cn

[P05] 判断两个对象内容是否相等
来源：http://zn.9csxet.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://ik.nszjky.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mi.nszjky.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ph.shtwfgs.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://cg.hnjuh.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://jx.szsharing.cn

Go:   reflect.DeepEqual(a, b)
来源：http://qs.chemitech.net.cn

Ruby: a == b
来源：http://ap.asd995.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://di.chemitech.net.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://yh.szsharing.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://zw.hnjuh.cn

PHP:  if (empty($x)) {}
来源：http://qo.huanxung.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://xs.shtwfgs.cn

TS:   if (x == null) {}
来源：http://vg.jianghongdianzi.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://uz.newstarts.cn

Go:   if x == nil {}
来源：http://sy.szxytkj.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://jw.jctech888.com.cn

C#:   if (x is null) {}
来源：http://dl.szsharing.cn

[P07] 防抖与节流
来源：http://tb.huixiangedu.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://zf.muxihuayi.cn

PHP:  // 手写时间戳比较
来源：http://sv.shtwfgs.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://iw.hnjuh.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://jz.asd995.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ac.panjiajie.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://kj.lnxyls.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://ko.chemitech.net.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://sp.szxytkj.cn

[P08] 处理浮点精度问题
来源：http://fk.jctech888.com.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://fg.jctech888.com.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://zs.yuexingan06.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://qp.hahajie.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ys.shxzukj.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ed.muxihuayi.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://yq.haigaiapp.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://aj.haigaiapp.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://bx.521024.cn

================================================================================
来源：http://ue.yuntaijiaju.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://jb.huixiangedu.cn

================================================================================
来源：http://js.wgjwhj.cn

[Q01] 创建表
来源：http://tn.muxihuayi.cn

CREATE TABLE users (
来源：http://pu.haigaiapp.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://cy.hnjuh.cn

name VARCHAR(50) NOT NULL,
来源：http://ms.panjiajie.cn

email VARCHAR(100) UNIQUE,
来源：http://ax.szsharing.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://og.jctech888.com.cn

);
来源：http://jo.hahajie.cn

[Q02] 创建带外键的表
来源：http://ar.9csxet.cn

CREATE TABLE orders (
来源：http://gk.szxytkj.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://pb.shtwfgs.cn

user_id INT NOT NULL,
来源：http://wg.shtwfgs.cn

amount DECIMAL(10, 2),
来源：http://tl.521024.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://qv.bjjhwx.cn

);
来源：http://io.nicolike.cn

[Q03] 增加列
来源：http://cg.lnxyls.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wl.hahajie.cn

[Q04] 修改列类型
来源：http://em.jctech888.com.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://kj.colortex.cn

[Q05] 重命名列
来源：http://mz.gzmigu.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://zc.chemitech.net.cn

[Q06] 删除列
来源：http://fe.szxytkj.cn

ALTER TABLE users DROP COLUMN age;
来源：http://bj.huanxung.cn

[Q07] 删除表
来源：http://ft.jianghongdianzi.cn

DROP TABLE IF EXISTS orders;
来源：http://sn.jianghongdianzi.cn

[Q08] 创建普通索引
来源：http://ad.shxzukj.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://kg.bjjhwx.cn

[Q09] 创建唯一索引
来源：http://df.chemitech.net.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://tt.newstarts.cn

[Q10] 插入单行
来源：http://es.colortex.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ox.jctech888.com.cn

[Q11] 一次插入多行
来源：http://ej.huanxung.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://bs.9csxet.cn

[Q12] 插入后取自增 ID
来源：http://fc.lnxyls.cn

INSERT INTO users (name) VALUES ('C');
来源：http://mt.521024.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://yk.huixiangedu.cn

[Q13] 忽略重复插入
来源：http://pv.huixinmuqiang.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mj.gzmigu.cn

[Q14] 存在则更新（upsert）
来源：http://pm.lnxyls.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mt.wgjwhj.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://yb.yuexingan06.cn

[Q15] 查询全部
来源：http://eu.nicolike.cn

SELECT * FROM users;
来源：http://lq.newstarts.cn

[Q16] 查询指定列
来源：http://dc.huanxung.cn

SELECT id, name FROM users;
来源：http://hv.huixiangedu.cn

[Q17] 条件查询
来源：http://cj.asd995.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://qx.szsharing.cn

[Q18] 模糊匹配
来源：http://wh.nicolike.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://uh.yuntaijiaju.cn

[Q19] 范围查询
来源：http://vw.yuntaijiaju.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://aa.newstarts.cn

[Q20] IN 列表
来源：http://sp.wgjwhj.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://gy.shxzukj.cn

[Q21] 空值判断
来源：http://tv.nszjky.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://yd.jctech888.com.cn

[Q22] 排序
来源：http://jm.haigaiapp.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://dg.521024.cn

[Q23] 分页
来源：http://vd.huixiangedu.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://br.szxytkj.cn

[Q24] 去重
来源：http://wd.panjiajie.cn

SELECT DISTINCT city FROM users;
来源：http://az.huixinmuqiang.cn

[Q25] 只取前 N 条
来源：http://ok.panjiajie.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ep.521024.cn

[Q26] 计数
来源：http://jb.nszjky.cn

SELECT COUNT(*) FROM users;
来源：http://hn.colortex.cn

[Q27] 条件计数
来源：http://zw.bookmarksfly.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://bp.nszjky.cn

[Q28] 求和与平均
来源：http://va.gzmigu.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://gb.chemitech.net.cn

[Q29] 最大最小值
来源：http://ab.jctech888.com.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://gu.chemitech.net.cn

[Q30] 分组统计
来源：http://fl.shtwfgs.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ns.huanxung.cn

[Q31] 分组后过滤
来源：http://hc.huixinmuqiang.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://vf.nszjky.cn

[Q32] 分组拼接字符串
来源：http://ak.haigaiapp.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://xv.colortex.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://gd.yuexingan06.cn

[Q33] 多列分组
来源：http://qo.colortex.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hb.szxytkj.cn

[Q34] 每组取第一条
来源：http://oc.gzmigu.cn

SELECT * FROM (
来源：http://ac.huanxung.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://zb.shxzukj.cn

) t WHERE rn = 1;
来源：http://qc.yuntaijiaju.cn

[Q35] 内连接
来源：http://eo.jctech888.com.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://un.newstarts.cn

[Q36] 左连接
来源：http://bg.muxihuayi.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ab.yuntaijiaju.cn

[Q37] 右连接
来源：http://vo.hahajie.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.shxzukj.cn

[Q38] 全外连接（PostgreSQL）
来源：http://lb.panjiajie.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ql.shxzskj.cn

[Q39] 自连接（查上下级）
来源：http://gg.chemitech.net.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://ba.szsharing.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://dr.huanxung.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://gb.chemitech.net.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://oe.jctech888.com.cn

[Q41] 多表连接
来源：http://ou.huixinmuqiang.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://li.jctech888.com.cn

JOIN users u ON u.id = o.user_id
来源：http://sa.jianghongdianzi.cn

JOIN products p ON p.id = o.product_id;
来源：http://vw.hahajie.cn

[Q42] 连接条件附加过滤
来源：http://bw.jctech888.com.cn

SELECT u.name, o.amount FROM users u
来源：http://ke.huixiangedu.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://kf.huixinmuqiang.cn

[Q43] 标量子查询
来源：http://un.nicolike.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wo.muxihuayi.cn

[Q44] IN 子查询
来源：http://wh.colortex.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://uf.muxihuayi.cn

[Q45] EXISTS 判断存在
来源：http://jx.chemitech.net.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://si.shtwfgs.cn

[Q46] NOT EXISTS 判断不存在
来源：http://io.jctech888.com.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://jz.muxihuayi.cn

[Q47] 与平均值比较
来源：http://ak.huanxung.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ph.panjiajie.cn

[Q48] CTE 公用表表达式
来源：http://gt.bookmarksfly.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://vp.hnjuh.cn

SELECT * FROM t WHERE c > 5;
来源：http://sv.haigaiapp.cn

[Q49] 更新单行
来源：http://qa.bjjhwx.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://zs.nszjky.cn

[Q50] 批量更新
来源：http://bd.asd995.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://dp.muxihuayi.cn

[Q51] 用子查询更新
来源：http://up.shtwfgs.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://gx.panjiajie.cn

[Q52] 删除指定行
来源：http://ky.bookmarksfly.cn

DELETE FROM users WHERE id = 10;
来源：http://qh.panjiajie.cn

[Q53] 按条件删除
来源：http://bp.huixiangedu.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://fn.lnxyls.cn

[Q54] 清空表
来源：http://hu.colortex.cn

TRUNCATE TABLE logs;
来源：http://xj.shxzskj.cn

[Q55] 排名（并列占位）
来源：http://ed.gzmigu.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://by.jctech888.com.cn

[Q56] 密集排名（并列不占位）
来源：http://al.shxzukj.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://pg.gzmigu.cn

[Q57] 行号
来源：http://il.hahajie.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://kc.shxzskj.cn

[Q58] 累计求和
来源：http://dt.bjjhwx.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://rn.9csxet.cn

[Q59] 分组内累计
来源：http://wi.nicolike.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://zy.szsharing.cn

[Q60] 取上一行 / 下一行
来源：http://bh.colortex.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://fx.wgjwhj.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://sj.hnjuh.cn

[Q61] 移动平均
来源：http://ng.jianghongdianzi.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://im.haigaiapp.cn

[Q62] 分组占比
来源：http://ns.huanxung.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ev.szsharing.cn

[Q63] 开启事务
来源：http://tn.szsharing.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://jd.hahajie.cn

[Q64] 提交事务
来源：http://vn.huixinmuqiang.cn

COMMIT;
来源：http://zi.shxzskj.cn

[Q65] 回滚事务
来源：http://xn.bookmarksfly.cn

ROLLBACK;
来源：http://pr.nicolike.cn

[Q66] 行锁查询
来源：http://rs.haigaiapp.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://gn.hnjuh.cn

[Q67] 设置隔离级别
来源：http://qa.nszjky.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://qf.szxytkj.cn

[Q68] 保存点
来源：http://us.huanxung.cn

SAVEPOINT sp1;
来源：http://to.szsharing.cn

ROLLBACK TO sp1;
来源：http://af.yuexingan06.cn

[Q69] 查看执行计划
来源：http://tj.szxytkj.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mp.lnxyls.cn

[Q70] 更新统计信息
来源：http://lz.nicolike.cn

ANALYZE TABLE users;
来源：http://xm.yuntaijiaju.cn

[Q71] 查看建表语句
来源：http://vv.wgjwhj.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://oo.hnjuh.cn

[Q72] 查看索引
来源：http://iw.wgjwhj.cn

SHOW INDEX FROM users;
来源：http://vh.asd995.cn

[Q73] 查看表状态
来源：http://dx.lnxyls.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://oy.huixiangedu.cn

[Q74] 强制使用索引
来源：http://bb.nicolike.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://uh.shxzukj.cn

[Q75] 日期格式化
来源：http://nc.panjiajie.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://pm.gzmigu.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://qy.lnxyls.cn

[Q76] 按天统计
来源：http://sb.yuexingan06.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hf.huixiangedu.cn

[Q77] 时间加减
来源：http://xx.colortex.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ce.nicolike.cn

[Q78] 当前时间
来源：http://iw.shxzskj.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ws.wgjwhj.cn

[Q79] 字符串拼接
来源：http://ja.bookmarksfly.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://oj.hnjuh.cn

[Q80] 字符串截取
来源：http://re.yuexingan06.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://zd.panjiajie.cn

[Q81] 字符串替换
来源：http://bi.muxihuayi.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://af.szsharing.cn

[Q82] 字符长度与字节长度
来源：http://iq.chemitech.net.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://az.szsharing.cn

[Q83] 大小写转换
来源：http://fr.nicolike.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://db.asd995.cn

[Q84] 去除首尾空格
来源：http://jv.szsharing.cn

SELECT TRIM(name) FROM users;
来源：http://km.panjiajie.cn

[Q85] 数值取整
来源：http://qj.newstarts.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://nl.lnxyls.cn

[Q86] 读取 JSON 字段
来源：http://xp.hnjuh.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://xp.yuexingan06.cn

[Q87] JSON 字段做条件
来源：http://en.yuntaijiaju.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://nu.gzmigu.cn


<!-- 参考信息 -->