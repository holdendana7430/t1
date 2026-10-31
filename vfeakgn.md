代发 wailian999

TS:   // worker_threads 线程池
来源：http://nk.521024.cn

Java: Executors.newFixedThreadPool(4)
来源：http://fn.colortex.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ya.jctech888.com.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://br.szxytkj.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://nj.wgjwhj.cn

[O03] 加锁保护共享数据
来源：http://cg.shxzukj.cn

Py:   with lock: shared += 1
来源：http://ou.muxihuayi.cn

PHP:  // 用 flock() 做文件锁
来源：http://og.hnjuh.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://jh.szxytkj.cn

TS:   // 同 JS
来源：http://ni.shtwfgs.cn

Java: synchronized (this) { shared++; }
来源：http://zs.shxzukj.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ox.nszjky.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://el.colortex.cn

C#:   lock (gate) { shared++; }
来源：http://zi.shxzukj.cn

[O04] 定义异步函数并等待
来源：http://vf.huixinmuqiang.cn

Py:   async def f():⏎    await g()
来源：http://kn.hahajie.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://dt.muxihuayi.cn

JS:   async function f() { await g(); }
来源：http://ax.shxzskj.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://bn.hahajie.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://um.jctech888.com.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://qx.wgjwhj.cn

Ruby: # 用 Fiber 或 async gem
来源：http://vl.yuexingan06.cn

C#:   async Task F() { await G(); }
来源：http://fk.hahajie.cn

[O05] 并发执行并等待全部完成
来源：http://ic.yuntaijiaju.cn

Py:   asyncio.gather(*tasks)
来源：http://go.colortex.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://yu.muxihuayi.cn

JS:   await Promise.all(tasks)
来源：http://mh.muxihuayi.cn

TS:   await Promise.all(tasks)
来源：http://ke.panjiajie.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://pk.jctech888.com.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://og.shtwfgs.cn

Ruby: threads.map(&:join)
来源：http://rk.wgjwhj.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://bl.chemitech.net.cn

[O06] 使用进程池
来源：http://li.shtwfgs.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hp.bookmarksfly.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://zi.jianghongdianzi.cn

JS:   // child_process / cluster 模块
来源：http://sq.shxzukj.cn

TS:   // child_process / cluster 模块
来源：http://ly.shtwfgs.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://et.shxzukj.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://tx.gzmigu.cn

Ruby: // fork 块
来源：http://uw.shxzukj.cn

C#:   Parallel.For
来源：http://eg.bookmarksfly.cn

================================================================================
来源：http://ev.huanxung.cn

P. 常用工具函数
来源：http://pd.shxzskj.cn

================================================================================
来源：http://ot.newstarts.cn

[P01] 生成 UUID
来源：http://la.yuexingan06.cn

Py:   str(uuid.uuid4())
来源：http://qy.huixiangedu.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://pi.huanxung.cn

JS:   crypto.randomUUID()
来源：http://jn.shxzukj.cn

TS:   crypto.randomUUID()
来源：http://nc.shxzukj.cn

Java: UUID.randomUUID().toString()
来源：http://wf.muxihuayi.cn

Go:   // 用 github.com/google/uuid
来源：http://ua.colortex.cn

Ruby: SecureRandom.uuid
来源：http://oy.wgjwhj.cn

C#:   Guid.NewGuid().ToString()
来源：http://dn.9csxet.cn

[P02] MD5 / SHA256 摘要
来源：http://an.szxytkj.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://rh.shxzukj.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://gk.huixiangedu.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ee.bookmarksfly.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://bp.asd995.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://iv.9csxet.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://dg.panjiajie.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://rw.szsharing.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://oc.lnxyls.cn

[P03] 生成短随机字符串
来源：http://pi.muxihuayi.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://db.asd995.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://yb.wgjwhj.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://he.huanxung.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://eu.huanxung.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://cf.gzmigu.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://oh.nicolike.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://tf.lnxyls.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://nw.huixinmuqiang.cn

[P04] 求长度
来源：http://dz.bookmarksfly.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://eu.wgjwhj.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://nc.yuntaijiaju.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ql.shtwfgs.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://vf.bjjhwx.cn

Java: list.size();  map.size();  s.length()
来源：http://tj.asd995.cn

Go:   len(arr);  len(m)
来源：http://kd.hahajie.cn

Ruby: x.length;  x.size
来源：http://eb.shxzukj.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://cu.haigaiapp.cn

[P05] 判断两个对象内容是否相等
来源：http://wk.lnxyls.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://do.521024.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://zu.colortex.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ie.huixinmuqiang.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ah.panjiajie.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mi.yuntaijiaju.cn

Go:   reflect.DeepEqual(a, b)
来源：http://kq.jctech888.com.cn

Ruby: a == b
来源：http://iz.nicolike.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://fb.huixinmuqiang.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://bq.haigaiapp.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://bd.9csxet.cn

PHP:  if (empty($x)) {}
来源：http://xo.asd995.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ho.asd995.cn

TS:   if (x == null) {}
来源：http://nb.newstarts.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://iv.yuexingan06.cn

Go:   if x == nil {}
来源：http://hz.yuexingan06.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://qw.nszjky.cn

C#:   if (x is null) {}
来源：http://ml.hnjuh.cn

[P07] 防抖与节流
来源：http://mo.haigaiapp.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://aj.shxzskj.cn

PHP:  // 手写时间戳比较
来源：http://iq.shxzukj.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://fq.shxzskj.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ln.huixiangedu.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hq.9csxet.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://nw.9csxet.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://qc.bookmarksfly.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://va.bookmarksfly.cn

[P08] 处理浮点精度问题
来源：http://rr.jianghongdianzi.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ax.bookmarksfly.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hc.szxytkj.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://uv.jctech888.com.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://de.hahajie.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://tg.shxzukj.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://kq.shtwfgs.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mw.shxzukj.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://kj.hnjuh.cn

================================================================================
来源：http://nt.jianghongdianzi.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://px.521024.cn

================================================================================
来源：http://xg.newstarts.cn

[Q01] 创建表
来源：http://ra.haigaiapp.cn

CREATE TABLE users (
来源：http://zi.gzmigu.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ur.panjiajie.cn

name VARCHAR(50) NOT NULL,
来源：http://mp.chemitech.net.cn

email VARCHAR(100) UNIQUE,
来源：http://oj.shxzskj.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ca.shtwfgs.cn

);
来源：http://ac.hnjuh.cn

[Q02] 创建带外键的表
来源：http://yt.jianghongdianzi.cn

CREATE TABLE orders (
来源：http://oi.newstarts.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ub.huixiangedu.cn

user_id INT NOT NULL,
来源：http://kt.shxzukj.cn

amount DECIMAL(10, 2),
来源：http://bf.shxzskj.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ag.bookmarksfly.cn

);
来源：http://nh.bjjhwx.cn

[Q03] 增加列
来源：http://wq.panjiajie.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hk.newstarts.cn

[Q04] 修改列类型
来源：http://vm.huanxung.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hj.lnxyls.cn

[Q05] 重命名列
来源：http://ds.panjiajie.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://xz.jianghongdianzi.cn

[Q06] 删除列
来源：http://if.chemitech.net.cn

ALTER TABLE users DROP COLUMN age;
来源：http://zh.jianghongdianzi.cn

[Q07] 删除表
来源：http://jb.wgjwhj.cn

DROP TABLE IF EXISTS orders;
来源：http://hm.hnjuh.cn

[Q08] 创建普通索引
来源：http://zz.colortex.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://wd.bjjhwx.cn

[Q09] 创建唯一索引
来源：http://qv.yuntaijiaju.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://qs.huixiangedu.cn

[Q10] 插入单行
来源：http://xh.szsharing.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://sv.chemitech.net.cn

[Q11] 一次插入多行
来源：http://ah.huanxung.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mi.szsharing.cn

[Q12] 插入后取自增 ID
来源：http://oo.huixinmuqiang.cn

INSERT INTO users (name) VALUES ('C');
来源：http://cy.szxytkj.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://qk.nicolike.cn

[Q13] 忽略重复插入
来源：http://wx.haigaiapp.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://dw.gzmigu.cn

[Q14] 存在则更新（upsert）
来源：http://hk.chemitech.net.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://nc.shtwfgs.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://fc.colortex.cn

[Q15] 查询全部
来源：http://ts.colortex.cn

SELECT * FROM users;
来源：http://fl.huixiangedu.cn

[Q16] 查询指定列
来源：http://ap.yuntaijiaju.cn

SELECT id, name FROM users;
来源：http://qt.chemitech.net.cn

[Q17] 条件查询
来源：http://cs.panjiajie.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wf.colortex.cn

[Q18] 模糊匹配
来源：http://zw.asd995.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://na.chemitech.net.cn

[Q19] 范围查询
来源：http://ww.muxihuayi.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wt.chemitech.net.cn

[Q20] IN 列表
来源：http://qo.panjiajie.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://qb.hahajie.cn

[Q21] 空值判断
来源：http://qp.9csxet.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://km.chemitech.net.cn

[Q22] 排序
来源：http://yw.newstarts.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://pf.9csxet.cn

[Q23] 分页
来源：http://dt.nicolike.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://id.jianghongdianzi.cn

[Q24] 去重
来源：http://fz.haigaiapp.cn

SELECT DISTINCT city FROM users;
来源：http://su.haigaiapp.cn

[Q25] 只取前 N 条
来源：http://bu.jctech888.com.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://sf.bookmarksfly.cn

[Q26] 计数
来源：http://wy.bjjhwx.cn

SELECT COUNT(*) FROM users;
来源：http://as.hahajie.cn

[Q27] 条件计数
来源：http://jk.colortex.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ah.szsharing.cn

[Q28] 求和与平均
来源：http://uj.szsharing.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://pu.colortex.cn

[Q29] 最大最小值
来源：http://st.bjjhwx.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://kr.huanxung.cn

[Q30] 分组统计
来源：http://ow.bjjhwx.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://pm.colortex.cn

[Q31] 分组后过滤
来源：http://lt.muxihuayi.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://rn.jianghongdianzi.cn

[Q32] 分组拼接字符串
来源：http://au.nicolike.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://bf.muxihuayi.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://gk.huanxung.cn

[Q33] 多列分组
来源：http://ft.bjjhwx.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ag.hahajie.cn

[Q34] 每组取第一条
来源：http://fs.huixiangedu.cn

SELECT * FROM (
来源：http://ae.jianghongdianzi.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://is.yuexingan06.cn

) t WHERE rn = 1;
来源：http://rr.yuexingan06.cn

[Q35] 内连接
来源：http://ly.521024.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://xg.bjjhwx.cn

[Q36] 左连接
来源：http://xn.hahajie.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://qf.nszjky.cn

[Q37] 右连接
来源：http://pi.9csxet.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ef.yuexingan06.cn

[Q38] 全外连接（PostgreSQL）
来源：http://zy.lnxyls.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://so.chemitech.net.cn

[Q39] 自连接（查上下级）
来源：http://ps.huixinmuqiang.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://th.bookmarksfly.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://sb.jianghongdianzi.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://no.huixiangedu.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://zv.szsharing.cn

[Q41] 多表连接
来源：http://zb.szxytkj.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://dq.shtwfgs.cn

JOIN users u ON u.id = o.user_id
来源：http://eh.nicolike.cn

JOIN products p ON p.id = o.product_id;
来源：http://wr.szsharing.cn

[Q42] 连接条件附加过滤
来源：http://tk.asd995.cn

SELECT u.name, o.amount FROM users u
来源：http://wv.haigaiapp.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://bm.hnjuh.cn

[Q43] 标量子查询
来源：http://eb.bjjhwx.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ug.jianghongdianzi.cn

[Q44] IN 子查询
来源：http://oe.huanxung.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://cy.huixinmuqiang.cn

[Q45] EXISTS 判断存在
来源：http://xv.nicolike.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://pp.newstarts.cn

[Q46] NOT EXISTS 判断不存在
来源：http://od.asd995.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ac.lnxyls.cn

[Q47] 与平均值比较
来源：http://ty.szsharing.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ie.wgjwhj.cn

[Q48] CTE 公用表表达式
来源：http://fz.huixiangedu.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://gj.szsharing.cn

SELECT * FROM t WHERE c > 5;
来源：http://lb.gzmigu.cn

[Q49] 更新单行
来源：http://cs.jianghongdianzi.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ks.bookmarksfly.cn

[Q50] 批量更新
来源：http://ky.nszjky.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://nz.nszjky.cn

[Q51] 用子查询更新
来源：http://xh.huanxung.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://gp.huanxung.cn

[Q52] 删除指定行
来源：http://hr.huixinmuqiang.cn

DELETE FROM users WHERE id = 10;
来源：http://qs.chemitech.net.cn

[Q53] 按条件删除
来源：http://ah.asd995.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://pt.nicolike.cn

[Q54] 清空表
来源：http://bx.panjiajie.cn

TRUNCATE TABLE logs;
来源：http://nf.wgjwhj.cn

[Q55] 排名（并列占位）
来源：http://hn.nszjky.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://cu.chemitech.net.cn

[Q56] 密集排名（并列不占位）
来源：http://qc.szxytkj.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ib.szsharing.cn

[Q57] 行号
来源：http://yf.haigaiapp.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ra.szxytkj.cn

[Q58] 累计求和
来源：http://lu.chemitech.net.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://bb.muxihuayi.cn

[Q59] 分组内累计
来源：http://ev.hnjuh.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://it.szsharing.cn

[Q60] 取上一行 / 下一行
来源：http://rp.huixinmuqiang.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://zu.szxytkj.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://lb.huixinmuqiang.cn

[Q61] 移动平均
来源：http://zl.chemitech.net.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wv.huixiangedu.cn

[Q62] 分组占比
来源：http://fv.gzmigu.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://jb.jianghongdianzi.cn

[Q63] 开启事务
来源：http://xd.panjiajie.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://mx.lnxyls.cn

[Q64] 提交事务
来源：http://ux.nszjky.cn

COMMIT;
来源：http://rt.huixinmuqiang.cn

[Q65] 回滚事务
来源：http://qe.bjjhwx.cn

ROLLBACK;
来源：http://wt.wgjwhj.cn

[Q66] 行锁查询
来源：http://pe.haigaiapp.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://tk.wgjwhj.cn

[Q67] 设置隔离级别
来源：http://ao.hnjuh.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ut.szsharing.cn

[Q68] 保存点
来源：http://ri.hnjuh.cn

SAVEPOINT sp1;
来源：http://gd.szsharing.cn

ROLLBACK TO sp1;
来源：http://kn.yuntaijiaju.cn

[Q69] 查看执行计划
来源：http://jv.9csxet.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://vb.jctech888.com.cn

[Q70] 更新统计信息
来源：http://qm.haigaiapp.cn

ANALYZE TABLE users;
来源：http://mv.jctech888.com.cn

[Q71] 查看建表语句
来源：http://iw.haigaiapp.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://kv.yuntaijiaju.cn

[Q72] 查看索引
来源：http://kg.asd995.cn

SHOW INDEX FROM users;
来源：http://ny.wgjwhj.cn

[Q73] 查看表状态
来源：http://uo.szxytkj.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://gi.huixiangedu.cn

[Q74] 强制使用索引
来源：http://xu.9csxet.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://eu.muxihuayi.cn

[Q75] 日期格式化
来源：http://xa.hnjuh.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://xo.9csxet.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://kn.yuexingan06.cn

[Q76] 按天统计
来源：http://ol.bjjhwx.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://qi.nicolike.cn

[Q77] 时间加减
来源：http://ol.yuntaijiaju.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://gr.shxzukj.cn

[Q78] 当前时间
来源：http://jf.hnjuh.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://su.huanxung.cn

[Q79] 字符串拼接
来源：http://ws.jianghongdianzi.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ww.521024.cn


<!-- 参考信息 -->