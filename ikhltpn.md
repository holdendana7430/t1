代发 wailian999

Ruby: mutex.synchronize { shared += 1 }
来源：http://dg.lnxyls.cn

C#:   lock (gate) { shared++; }
来源：http://yf.nicolike.cn

[O04] 定义异步函数并等待
来源：http://vz.jctech888.com.cn

Py:   async def f():⏎    await g()
来源：http://lz.hahajie.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://pf.newstarts.cn

JS:   async function f() { await g(); }
来源：http://sh.newstarts.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://ww.yuntaijiaju.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://eh.huixiangedu.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://rm.nicolike.cn

Ruby: # 用 Fiber 或 async gem
来源：http://rq.jctech888.com.cn

C#:   async Task F() { await G(); }
来源：http://hq.jianghongdianzi.cn

[O05] 并发执行并等待全部完成
来源：http://ks.521024.cn

Py:   asyncio.gather(*tasks)
来源：http://ds.huixiangedu.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://jv.9csxet.cn

JS:   await Promise.all(tasks)
来源：http://qk.521024.cn

TS:   await Promise.all(tasks)
来源：http://yq.lnxyls.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://iy.gzmigu.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://of.nicolike.cn

Ruby: threads.map(&:join)
来源：http://jc.shtwfgs.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://fg.szxytkj.cn

[O06] 使用进程池
来源：http://pa.huixiangedu.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ld.wgjwhj.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://ea.colortex.cn

JS:   // child_process / cluster 模块
来源：http://yb.yuexingan06.cn

TS:   // child_process / cluster 模块
来源：http://jt.nicolike.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://tb.bookmarksfly.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://lc.huanxung.cn

Ruby: // fork 块
来源：http://ln.shtwfgs.cn

C#:   Parallel.For
来源：http://zo.shtwfgs.cn

================================================================================
来源：http://cy.huixinmuqiang.cn

P. 常用工具函数
来源：http://mv.asd995.cn

================================================================================
来源：http://qj.9csxet.cn

[P01] 生成 UUID
来源：http://vc.asd995.cn

Py:   str(uuid.uuid4())
来源：http://xk.lnxyls.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://jq.colortex.cn

JS:   crypto.randomUUID()
来源：http://fy.bookmarksfly.cn

TS:   crypto.randomUUID()
来源：http://hf.shxzukj.cn

Java: UUID.randomUUID().toString()
来源：http://ci.wgjwhj.cn

Go:   // 用 github.com/google/uuid
来源：http://ib.shxzukj.cn

Ruby: SecureRandom.uuid
来源：http://vv.muxihuayi.cn

C#:   Guid.NewGuid().ToString()
来源：http://ni.yuexingan06.cn

[P02] MD5 / SHA256 摘要
来源：http://zj.huixinmuqiang.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://as.521024.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://tk.bookmarksfly.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://jx.bjjhwx.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://kj.bjjhwx.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://vv.huanxung.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://vi.colortex.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ir.huixiangedu.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://iq.szxytkj.cn

[P03] 生成短随机字符串
来源：http://cw.muxihuayi.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://de.huanxung.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://uv.asd995.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://sk.huanxung.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://et.muxihuayi.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://pg.lnxyls.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://lf.jctech888.com.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://mg.hahajie.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mk.521024.cn

[P04] 求长度
来源：http://gi.muxihuayi.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://bs.nicolike.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://uw.wgjwhj.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://rz.nicolike.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hf.asd995.cn

Java: list.size();  map.size();  s.length()
来源：http://ju.yuexingan06.cn

Go:   len(arr);  len(m)
来源：http://tc.bookmarksfly.cn

Ruby: x.length;  x.size
来源：http://tr.asd995.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://wm.huanxung.cn

[P05] 判断两个对象内容是否相等
来源：http://vt.yuexingan06.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://mt.szxytkj.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://dt.muxihuayi.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://pe.huixiangedu.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://jl.yuntaijiaju.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ug.gzmigu.cn

Go:   reflect.DeepEqual(a, b)
来源：http://er.szsharing.cn

Ruby: a == b
来源：http://wk.muxihuayi.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://lj.gzmigu.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://yx.yuntaijiaju.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://yo.panjiajie.cn

PHP:  if (empty($x)) {}
来源：http://zg.muxihuayi.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://en.bookmarksfly.cn

TS:   if (x == null) {}
来源：http://mk.yuntaijiaju.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://ti.huixiangedu.cn

Go:   if x == nil {}
来源：http://wo.newstarts.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://vy.9csxet.cn

C#:   if (x is null) {}
来源：http://kn.nszjky.cn

[P07] 防抖与节流
来源：http://gt.panjiajie.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mt.szxytkj.cn

PHP:  // 手写时间戳比较
来源：http://iz.521024.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://bi.newstarts.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mc.hahajie.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://kg.wgjwhj.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://bv.bjjhwx.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://ez.asd995.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ta.9csxet.cn

[P08] 处理浮点精度问题
来源：http://dl.jctech888.com.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mo.gzmigu.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ww.newstarts.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://bp.jctech888.com.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://zz.shxzukj.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://el.colortex.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ot.nicolike.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://qs.jianghongdianzi.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://xf.shxzskj.cn

================================================================================
来源：http://lv.nicolike.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://qt.panjiajie.cn

================================================================================
来源：http://jo.nicolike.cn

[Q01] 创建表
来源：http://lo.gzmigu.cn

CREATE TABLE users (
来源：http://ap.colortex.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ge.9csxet.cn

name VARCHAR(50) NOT NULL,
来源：http://um.panjiajie.cn

email VARCHAR(100) UNIQUE,
来源：http://of.lnxyls.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ie.shxzukj.cn

);
来源：http://za.jianghongdianzi.cn

[Q02] 创建带外键的表
来源：http://wt.bjjhwx.cn

CREATE TABLE orders (
来源：http://hn.panjiajie.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://gk.huanxung.cn

user_id INT NOT NULL,
来源：http://ox.chemitech.net.cn

amount DECIMAL(10, 2),
来源：http://oh.lnxyls.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://iq.shxzukj.cn

);
来源：http://ok.panjiajie.cn

[Q03] 增加列
来源：http://pb.gzmigu.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://yc.521024.cn

[Q04] 修改列类型
来源：http://zr.huanxung.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://qi.jianghongdianzi.cn

[Q05] 重命名列
来源：http://eb.lnxyls.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://bs.huixinmuqiang.cn

[Q06] 删除列
来源：http://pu.bjjhwx.cn

ALTER TABLE users DROP COLUMN age;
来源：http://go.yuexingan06.cn

[Q07] 删除表
来源：http://is.bookmarksfly.cn

DROP TABLE IF EXISTS orders;
来源：http://ai.asd995.cn

[Q08] 创建普通索引
来源：http://ct.huixiangedu.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://lu.yuexingan06.cn

[Q09] 创建唯一索引
来源：http://ys.huixiangedu.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ji.muxihuayi.cn

[Q10] 插入单行
来源：http://nv.bookmarksfly.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://uk.bookmarksfly.cn

[Q11] 一次插入多行
来源：http://gp.asd995.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wa.shxzukj.cn

[Q12] 插入后取自增 ID
来源：http://sw.nicolike.cn

INSERT INTO users (name) VALUES ('C');
来源：http://ax.jctech888.com.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://iy.szxytkj.cn

[Q13] 忽略重复插入
来源：http://zn.lnxyls.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://cm.muxihuayi.cn

[Q14] 存在则更新（upsert）
来源：http://ik.shtwfgs.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ry.newstarts.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://it.newstarts.cn

[Q15] 查询全部
来源：http://kg.shxzukj.cn

SELECT * FROM users;
来源：http://kx.haigaiapp.cn

[Q16] 查询指定列
来源：http://ve.asd995.cn

SELECT id, name FROM users;
来源：http://ub.jianghongdianzi.cn

[Q17] 条件查询
来源：http://du.asd995.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://es.yuexingan06.cn

[Q18] 模糊匹配
来源：http://jq.bjjhwx.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://tb.gzmigu.cn

[Q19] 范围查询
来源：http://oq.chemitech.net.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://to.9csxet.cn

[Q20] IN 列表
来源：http://ce.9csxet.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://lz.wgjwhj.cn

[Q21] 空值判断
来源：http://bi.asd995.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://ur.yuexingan06.cn

[Q22] 排序
来源：http://je.huixinmuqiang.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://zk.asd995.cn

[Q23] 分页
来源：http://kt.szxytkj.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ol.shxzskj.cn

[Q24] 去重
来源：http://kf.shtwfgs.cn

SELECT DISTINCT city FROM users;
来源：http://gk.yuexingan06.cn

[Q25] 只取前 N 条
来源：http://aa.bookmarksfly.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://pb.chemitech.net.cn

[Q26] 计数
来源：http://re.yuntaijiaju.cn

SELECT COUNT(*) FROM users;
来源：http://ma.yuntaijiaju.cn

[Q27] 条件计数
来源：http://ww.huanxung.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://gz.panjiajie.cn

[Q28] 求和与平均
来源：http://io.gzmigu.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://kh.521024.cn

[Q29] 最大最小值
来源：http://ow.chemitech.net.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://na.muxihuayi.cn

[Q30] 分组统计
来源：http://pq.shxzskj.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://tv.nicolike.cn

[Q31] 分组后过滤
来源：http://vs.huanxung.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://oh.huixiangedu.cn

[Q32] 分组拼接字符串
来源：http://qs.hnjuh.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://rp.chemitech.net.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://oi.hahajie.cn

[Q33] 多列分组
来源：http://zi.hnjuh.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://fz.huixiangedu.cn

[Q34] 每组取第一条
来源：http://vo.shtwfgs.cn

SELECT * FROM (
来源：http://fj.haigaiapp.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://fg.huixiangedu.cn

) t WHERE rn = 1;
来源：http://sc.bookmarksfly.cn

[Q35] 内连接
来源：http://at.lnxyls.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://vw.szsharing.cn

[Q36] 左连接
来源：http://ax.bjjhwx.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://pd.hahajie.cn

[Q37] 右连接
来源：http://dv.colortex.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wn.hahajie.cn

[Q38] 全外连接（PostgreSQL）
来源：http://bd.bookmarksfly.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://so.hnjuh.cn

[Q39] 自连接（查上下级）
来源：http://zs.wgjwhj.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://qu.szxytkj.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://zc.lnxyls.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://tw.muxihuayi.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://rj.jctech888.com.cn

[Q41] 多表连接
来源：http://by.panjiajie.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://zl.yuntaijiaju.cn

JOIN users u ON u.id = o.user_id
来源：http://ge.colortex.cn

JOIN products p ON p.id = o.product_id;
来源：http://ua.yuexingan06.cn

[Q42] 连接条件附加过滤
来源：http://qw.hnjuh.cn

SELECT u.name, o.amount FROM users u
来源：http://ao.bjjhwx.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://zj.muxihuayi.cn

[Q43] 标量子查询
来源：http://vl.9csxet.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://fv.jianghongdianzi.cn

[Q44] IN 子查询
来源：http://xa.bookmarksfly.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://jx.huanxung.cn

[Q45] EXISTS 判断存在
来源：http://wq.yuntaijiaju.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://et.wgjwhj.cn

[Q46] NOT EXISTS 判断不存在
来源：http://yf.yuexingan06.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://cs.wgjwhj.cn

[Q47] 与平均值比较
来源：http://hr.asd995.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://js.colortex.cn

[Q48] CTE 公用表表达式
来源：http://dr.521024.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://yy.wgjwhj.cn

SELECT * FROM t WHERE c > 5;
来源：http://bh.jianghongdianzi.cn

[Q49] 更新单行
来源：http://py.chemitech.net.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ia.lnxyls.cn

[Q50] 批量更新
来源：http://zr.521024.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://iw.jctech888.com.cn

[Q51] 用子查询更新
来源：http://cg.lnxyls.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mk.9csxet.cn

[Q52] 删除指定行
来源：http://uo.bookmarksfly.cn

DELETE FROM users WHERE id = 10;
来源：http://bm.nszjky.cn

[Q53] 按条件删除
来源：http://mk.szxytkj.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://lj.jianghongdianzi.cn

[Q54] 清空表
来源：http://zu.nszjky.cn

TRUNCATE TABLE logs;
来源：http://wk.jctech888.com.cn

[Q55] 排名（并列占位）
来源：http://cc.9csxet.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://io.huixinmuqiang.cn

[Q56] 密集排名（并列不占位）
来源：http://iy.9csxet.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ln.colortex.cn

[Q57] 行号
来源：http://hf.lnxyls.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://jg.9csxet.cn

[Q58] 累计求和
来源：http://wx.jctech888.com.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hm.9csxet.cn

[Q59] 分组内累计
来源：http://mz.huixiangedu.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hc.9csxet.cn

[Q60] 取上一行 / 下一行
来源：http://el.521024.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://kg.9csxet.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://lb.huixinmuqiang.cn

[Q61] 移动平均
来源：http://cj.muxihuayi.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://md.colortex.cn

[Q62] 分组占比
来源：http://ru.jctech888.com.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ck.huixinmuqiang.cn

[Q63] 开启事务
来源：http://ba.yuexingan06.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://yz.szsharing.cn

[Q64] 提交事务
来源：http://db.jctech888.com.cn

COMMIT;
来源：http://rf.newstarts.cn

[Q65] 回滚事务
来源：http://wa.muxihuayi.cn

ROLLBACK;
来源：http://ru.shtwfgs.cn

[Q66] 行锁查询
来源：http://wn.yuntaijiaju.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://nw.muxihuayi.cn

[Q67] 设置隔离级别
来源：http://az.shxzukj.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://yn.gzmigu.cn

[Q68] 保存点
来源：http://ap.asd995.cn

SAVEPOINT sp1;
来源：http://je.newstarts.cn

ROLLBACK TO sp1;
来源：http://gi.9csxet.cn

[Q69] 查看执行计划
来源：http://ud.wgjwhj.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ch.huixinmuqiang.cn

[Q70] 更新统计信息
来源：http://pk.chemitech.net.cn

ANALYZE TABLE users;
来源：http://ge.9csxet.cn

[Q71] 查看建表语句
来源：http://tv.bjjhwx.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://oi.yuexingan06.cn

[Q72] 查看索引
来源：http://sg.wgjwhj.cn

SHOW INDEX FROM users;
来源：http://mp.hnjuh.cn

[Q73] 查看表状态
来源：http://gs.muxihuayi.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://xk.shxzskj.cn

[Q74] 强制使用索引
来源：http://yf.muxihuayi.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://dl.521024.cn

[Q75] 日期格式化
来源：http://zw.huixiangedu.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://yk.gzmigu.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://fw.asd995.cn

[Q76] 按天统计
来源：http://sc.chemitech.net.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://dv.huanxung.cn

[Q77] 时间加减
来源：http://wb.huixinmuqiang.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://kh.shxzukj.cn

[Q78] 当前时间
来源：http://wn.huixinmuqiang.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wh.nicolike.cn

[Q79] 字符串拼接
来源：http://iu.colortex.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://by.huixinmuqiang.cn

[Q80] 字符串截取
来源：http://pi.hahajie.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://jv.newstarts.cn

[Q81] 字符串替换
来源：http://dx.nicolike.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://cz.yuexingan06.cn

[Q82] 字符长度与字节长度
来源：http://we.nszjky.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ro.huixiangedu.cn

[Q83] 大小写转换
来源：http://yi.chemitech.net.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ko.hahajie.cn

[Q84] 去除首尾空格
来源：http://vz.wgjwhj.cn

SELECT TRIM(name) FROM users;
来源：http://mp.huanxung.cn

[Q85] 数值取整
来源：http://pl.jctech888.com.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://as.hahajie.cn


<!-- 参考信息 -->