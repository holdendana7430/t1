代发 wailian999

================================================================================
来源：http://hp.shxzukj.cn

O. 并发与异步
来源：http://gh.shtwfgs.cn

================================================================================
来源：http://sd.shxzukj.cn

[O01] 启动一个线程
来源：http://lt.szsharing.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ab.jctech888.com.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ax.521024.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ns.szsharing.cn

TS:   // 同 JS
来源：http://tb.huixinmuqiang.cn

Java: new Thread(() -> f()).start()
来源：http://ai.huixinmuqiang.cn

Go:   go f()
来源：http://os.newstarts.cn

Ruby: Thread.new { f }
来源：http://jx.hahajie.cn

C#:   Task.Run(() => F());
来源：http://te.jctech888.com.cn

[O02] 使用线程池
来源：http://gx.szxytkj.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://yh.lnxyls.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://nf.wgjwhj.cn

JS:   // worker_threads 线程池
来源：http://zf.bjjhwx.cn

TS:   // worker_threads 线程池
来源：http://hn.huanxung.cn

Java: Executors.newFixedThreadPool(4)
来源：http://wd.panjiajie.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://bf.9csxet.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://rd.szxytkj.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ud.521024.cn

[O03] 加锁保护共享数据
来源：http://dl.nszjky.cn

Py:   with lock: shared += 1
来源：http://yw.gzmigu.cn

PHP:  // 用 flock() 做文件锁
来源：http://sv.colortex.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://gp.huixinmuqiang.cn

TS:   // 同 JS
来源：http://sk.yuexingan06.cn

Java: synchronized (this) { shared++; }
来源：http://mf.jianghongdianzi.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://uk.nszjky.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://gl.szxytkj.cn

C#:   lock (gate) { shared++; }
来源：http://yw.gzmigu.cn

[O04] 定义异步函数并等待
来源：http://tm.huanxung.cn

Py:   async def f():⏎    await g()
来源：http://om.huixiangedu.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://st.nszjky.cn

JS:   async function f() { await g(); }
来源：http://il.huixiangedu.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://rw.huixiangedu.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://vb.jianghongdianzi.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ef.szsharing.cn

Ruby: # 用 Fiber 或 async gem
来源：http://ou.bjjhwx.cn

C#:   async Task F() { await G(); }
来源：http://ah.gzmigu.cn

[O05] 并发执行并等待全部完成
来源：http://nm.muxihuayi.cn

Py:   asyncio.gather(*tasks)
来源：http://bx.huanxung.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://rn.muxihuayi.cn

JS:   await Promise.all(tasks)
来源：http://sf.hnjuh.cn

TS:   await Promise.all(tasks)
来源：http://wu.bookmarksfly.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://kz.shtwfgs.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://sq.huanxung.cn

Ruby: threads.map(&:join)
来源：http://qi.huixinmuqiang.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://at.gzmigu.cn

[O06] 使用进程池
来源：http://tp.panjiajie.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://vu.shxzukj.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://ri.huixiangedu.cn

JS:   // child_process / cluster 模块
来源：http://sy.jianghongdianzi.cn

TS:   // child_process / cluster 模块
来源：http://yn.shxzukj.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ms.nszjky.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://id.chemitech.net.cn

Ruby: // fork 块
来源：http://vb.muxihuayi.cn

C#:   Parallel.For
来源：http://uo.asd995.cn

================================================================================
来源：http://et.jianghongdianzi.cn

P. 常用工具函数
来源：http://gq.asd995.cn

================================================================================
来源：http://ru.9csxet.cn

[P01] 生成 UUID
来源：http://sx.muxihuayi.cn

Py:   str(uuid.uuid4())
来源：http://gu.wgjwhj.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://so.9csxet.cn

JS:   crypto.randomUUID()
来源：http://qp.shxzukj.cn

TS:   crypto.randomUUID()
来源：http://ul.shxzskj.cn

Java: UUID.randomUUID().toString()
来源：http://ew.haigaiapp.cn

Go:   // 用 github.com/google/uuid
来源：http://av.521024.cn

Ruby: SecureRandom.uuid
来源：http://fl.bjjhwx.cn

C#:   Guid.NewGuid().ToString()
来源：http://we.shtwfgs.cn

[P02] MD5 / SHA256 摘要
来源：http://zn.bjjhwx.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://oh.nszjky.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://vx.gzmigu.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://vh.gzmigu.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://xn.colortex.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ai.chemitech.net.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://tx.nszjky.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://bb.bjjhwx.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mq.lnxyls.cn

[P03] 生成短随机字符串
来源：http://jh.shtwfgs.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://xn.chemitech.net.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ox.asd995.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ap.newstarts.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://vj.nicolike.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hc.gzmigu.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://bt.9csxet.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://ox.colortex.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://kn.jianghongdianzi.cn

[P04] 求长度
来源：http://as.shxzskj.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://gz.bookmarksfly.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ks.yuntaijiaju.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://vx.huanxung.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ld.jianghongdianzi.cn

Java: list.size();  map.size();  s.length()
来源：http://ye.9csxet.cn

Go:   len(arr);  len(m)
来源：http://no.nszjky.cn

Ruby: x.length;  x.size
来源：http://gi.szxytkj.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://tr.newstarts.cn

[P05] 判断两个对象内容是否相等
来源：http://bp.521024.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://cg.shxzskj.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://xy.szsharing.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ip.panjiajie.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://uv.jianghongdianzi.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://jb.521024.cn

Go:   reflect.DeepEqual(a, b)
来源：http://nn.wgjwhj.cn

Ruby: a == b
来源：http://sn.lnxyls.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://do.panjiajie.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://uq.huixinmuqiang.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ie.newstarts.cn

PHP:  if (empty($x)) {}
来源：http://si.lnxyls.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://kp.shxzukj.cn

TS:   if (x == null) {}
来源：http://xw.yuntaijiaju.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://fq.huixiangedu.cn

Go:   if x == nil {}
来源：http://tk.bookmarksfly.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ez.newstarts.cn

C#:   if (x is null) {}
来源：http://xa.9csxet.cn

[P07] 防抖与节流
来源：http://dt.nszjky.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://gu.hnjuh.cn

PHP:  // 手写时间戳比较
来源：http://jo.asd995.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://da.huixiangedu.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ku.haigaiapp.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://os.shxzukj.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://gt.shtwfgs.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://fn.bookmarksfly.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://gz.huanxung.cn

[P08] 处理浮点精度问题
来源：http://rl.nicolike.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://xf.chemitech.net.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://zg.jianghongdianzi.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://lk.szsharing.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://gp.huanxung.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://zd.nszjky.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://kl.szsharing.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://sk.panjiajie.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.muxihuayi.cn

================================================================================
来源：http://bb.bookmarksfly.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mn.hahajie.cn

================================================================================
来源：http://th.szxytkj.cn

[Q01] 创建表
来源：http://na.newstarts.cn

CREATE TABLE users (
来源：http://kv.szsharing.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://gn.bjjhwx.cn

name VARCHAR(50) NOT NULL,
来源：http://yk.huixiangedu.cn

email VARCHAR(100) UNIQUE,
来源：http://ze.huixiangedu.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://sp.huixinmuqiang.cn

);
来源：http://lf.yuntaijiaju.cn

[Q02] 创建带外键的表
来源：http://tk.bookmarksfly.cn

CREATE TABLE orders (
来源：http://tv.muxihuayi.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ss.wgjwhj.cn

user_id INT NOT NULL,
来源：http://uy.newstarts.cn

amount DECIMAL(10, 2),
来源：http://gn.haigaiapp.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://bc.bjjhwx.cn

);
来源：http://iu.hahajie.cn

[Q03] 增加列
来源：http://ak.shtwfgs.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://gz.muxihuayi.cn

[Q04] 修改列类型
来源：http://wy.jianghongdianzi.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://on.jianghongdianzi.cn

[Q05] 重命名列
来源：http://pk.jctech888.com.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://qv.shxzukj.cn

[Q06] 删除列
来源：http://cr.9csxet.cn

ALTER TABLE users DROP COLUMN age;
来源：http://lr.shxzskj.cn

[Q07] 删除表
来源：http://eb.newstarts.cn

DROP TABLE IF EXISTS orders;
来源：http://zf.yuntaijiaju.cn

[Q08] 创建普通索引
来源：http://iz.huanxung.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://aq.gzmigu.cn

[Q09] 创建唯一索引
来源：http://gr.shtwfgs.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://oy.szxytkj.cn

[Q10] 插入单行
来源：http://qn.bjjhwx.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://jd.yuntaijiaju.cn

[Q11] 一次插入多行
来源：http://re.bjjhwx.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mc.shxzukj.cn

[Q12] 插入后取自增 ID
来源：http://nd.bjjhwx.cn

INSERT INTO users (name) VALUES ('C');
来源：http://zb.521024.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://yz.colortex.cn

[Q13] 忽略重复插入
来源：http://gf.gzmigu.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hk.jianghongdianzi.cn

[Q14] 存在则更新（upsert）
来源：http://nr.nicolike.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://bs.gzmigu.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://cp.newstarts.cn

[Q15] 查询全部
来源：http://nv.newstarts.cn

SELECT * FROM users;
来源：http://pm.muxihuayi.cn

[Q16] 查询指定列
来源：http://wr.jianghongdianzi.cn

SELECT id, name FROM users;
来源：http://cy.huanxung.cn

[Q17] 条件查询
来源：http://mf.nszjky.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://cm.bookmarksfly.cn

[Q18] 模糊匹配
来源：http://vw.wgjwhj.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ax.gzmigu.cn

[Q19] 范围查询
来源：http://qq.yuntaijiaju.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://vb.lnxyls.cn

[Q20] IN 列表
来源：http://pp.lnxyls.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://xm.panjiajie.cn

[Q21] 空值判断
来源：http://sj.huixinmuqiang.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://km.lnxyls.cn

[Q22] 排序
来源：http://ny.521024.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://oc.newstarts.cn

[Q23] 分页
来源：http://gv.yuntaijiaju.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://sx.yuntaijiaju.cn

[Q24] 去重
来源：http://df.shxzskj.cn

SELECT DISTINCT city FROM users;
来源：http://va.colortex.cn

[Q25] 只取前 N 条
来源：http://kl.hnjuh.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://rs.szxytkj.cn

[Q26] 计数
来源：http://ow.nszjky.cn

SELECT COUNT(*) FROM users;
来源：http://vv.haigaiapp.cn

[Q27] 条件计数
来源：http://qd.haigaiapp.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://dt.hahajie.cn

[Q28] 求和与平均
来源：http://sk.haigaiapp.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://zh.wgjwhj.cn

[Q29] 最大最小值
来源：http://ue.haigaiapp.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://jx.nszjky.cn

[Q30] 分组统计
来源：http://bg.nszjky.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://oz.newstarts.cn

[Q31] 分组后过滤
来源：http://qb.lnxyls.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://jg.yuntaijiaju.cn

[Q32] 分组拼接字符串
来源：http://il.szsharing.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mt.huixiangedu.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://gg.haigaiapp.cn

[Q33] 多列分组
来源：http://wo.huixiangedu.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://bq.bjjhwx.cn

[Q34] 每组取第一条
来源：http://sb.bookmarksfly.cn

SELECT * FROM (
来源：http://ki.haigaiapp.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://pr.szxytkj.cn

) t WHERE rn = 1;
来源：http://fj.521024.cn

[Q35] 内连接
来源：http://cm.bjjhwx.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://nh.haigaiapp.cn

[Q36] 左连接
来源：http://ow.gzmigu.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://lf.yuntaijiaju.cn

[Q37] 右连接
来源：http://hl.shtwfgs.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://lp.gzmigu.cn

[Q38] 全外连接（PostgreSQL）
来源：http://rf.huixinmuqiang.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ik.hnjuh.cn

[Q39] 自连接（查上下级）
来源：http://fj.szxytkj.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://wb.gzmigu.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://bb.lnxyls.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://sl.yuntaijiaju.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://xy.521024.cn

[Q41] 多表连接
来源：http://tk.shtwfgs.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://cd.lnxyls.cn

JOIN users u ON u.id = o.user_id
来源：http://wa.hnjuh.cn

JOIN products p ON p.id = o.product_id;
来源：http://sz.newstarts.cn

[Q42] 连接条件附加过滤
来源：http://vj.huixinmuqiang.cn

SELECT u.name, o.amount FROM users u
来源：http://wk.huixiangedu.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ve.yuntaijiaju.cn

[Q43] 标量子查询
来源：http://tw.haigaiapp.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://kf.nicolike.cn

[Q44] IN 子查询
来源：http://cl.nszjky.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://fs.colortex.cn

[Q45] EXISTS 判断存在
来源：http://bx.lnxyls.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://dc.jianghongdianzi.cn

[Q46] NOT EXISTS 判断不存在
来源：http://dk.hahajie.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://et.lnxyls.cn

[Q47] 与平均值比较
来源：http://gm.newstarts.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ar.panjiajie.cn

[Q48] CTE 公用表表达式
来源：http://tb.panjiajie.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://us.hahajie.cn

SELECT * FROM t WHERE c > 5;
来源：http://dg.asd995.cn

[Q49] 更新单行
来源：http://cz.shxzukj.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://xl.panjiajie.cn

[Q50] 批量更新
来源：http://gj.chemitech.net.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wj.shtwfgs.cn

[Q51] 用子查询更新
来源：http://al.huixinmuqiang.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://ro.bjjhwx.cn

[Q52] 删除指定行
来源：http://si.gzmigu.cn

DELETE FROM users WHERE id = 10;
来源：http://xg.muxihuayi.cn

[Q53] 按条件删除
来源：http://ng.yuexingan06.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wg.yuntaijiaju.cn

[Q54] 清空表
来源：http://em.shxzskj.cn

TRUNCATE TABLE logs;
来源：http://qe.shxzskj.cn

[Q55] 排名（并列占位）
来源：http://rm.nszjky.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://is.shtwfgs.cn

[Q56] 密集排名（并列不占位）
来源：http://fe.hnjuh.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://if.521024.cn

[Q57] 行号
来源：http://lp.haigaiapp.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://kx.huixiangedu.cn

[Q58] 累计求和
来源：http://sk.huixiangedu.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://he.shtwfgs.cn

[Q59] 分组内累计
来源：http://br.bjjhwx.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wg.lnxyls.cn

[Q60] 取上一行 / 下一行
来源：http://yk.bookmarksfly.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hf.chemitech.net.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://tk.shtwfgs.cn

[Q61] 移动平均
来源：http://bx.nicolike.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://uj.nszjky.cn

[Q62] 分组占比
来源：http://vh.colortex.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://cm.huixinmuqiang.cn

[Q63] 开启事务
来源：http://vn.wgjwhj.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://ds.huixinmuqiang.cn

[Q64] 提交事务
来源：http://ma.hnjuh.cn

COMMIT;
来源：http://ia.jctech888.com.cn

[Q65] 回滚事务
来源：http://re.shxzskj.cn

ROLLBACK;
来源：http://wt.yuntaijiaju.cn

[Q66] 行锁查询
来源：http://zh.hnjuh.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://bn.bookmarksfly.cn

[Q67] 设置隔离级别
来源：http://gg.asd995.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://xv.panjiajie.cn

[Q68] 保存点
来源：http://bb.colortex.cn

SAVEPOINT sp1;
来源：http://vx.jianghongdianzi.cn

ROLLBACK TO sp1;
来源：http://zw.gzmigu.cn

[Q69] 查看执行计划
来源：http://ry.szxytkj.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wd.shtwfgs.cn

[Q70] 更新统计信息
来源：http://jd.jctech888.com.cn

ANALYZE TABLE users;
来源：http://at.haigaiapp.cn

[Q71] 查看建表语句
来源：http://ob.szsharing.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://fa.huixinmuqiang.cn

[Q72] 查看索引
来源：http://lg.newstarts.cn


<!-- 参考信息 -->