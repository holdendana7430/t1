代发 wailian999

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://dl.panjiajie.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://tb.haigaiapp.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://iv.gzmigu.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://xo.haigaiapp.cn

================================================================================
来源：http://zq.shtwfgs.cn

O. 并发与异步
来源：http://gx.haigaiapp.cn

================================================================================
来源：http://ge.szxytkj.cn

[O01] 启动一个线程
来源：http://za.521024.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://fv.lnxyls.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://fu.9csxet.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://sh.lnxyls.cn

TS:   // 同 JS
来源：http://aq.szxytkj.cn

Java: new Thread(() -> f()).start()
来源：http://lu.nicolike.cn

Go:   go f()
来源：http://ef.huixinmuqiang.cn

Ruby: Thread.new { f }
来源：http://pb.panjiajie.cn

C#:   Task.Run(() => F());
来源：http://gd.shxzskj.cn

[O02] 使用线程池
来源：http://jv.jctech888.com.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://db.lnxyls.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ko.chemitech.net.cn

JS:   // worker_threads 线程池
来源：http://yr.muxihuayi.cn

TS:   // worker_threads 线程池
来源：http://ky.bookmarksfly.cn

Java: Executors.newFixedThreadPool(4)
来源：http://gv.huixiangedu.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ev.shxzskj.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://oa.huixiangedu.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://xb.nszjky.cn

[O03] 加锁保护共享数据
来源：http://bv.521024.cn

Py:   with lock: shared += 1
来源：http://re.nszjky.cn

PHP:  // 用 flock() 做文件锁
来源：http://gg.asd995.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://tu.9csxet.cn

TS:   // 同 JS
来源：http://wy.shtwfgs.cn

Java: synchronized (this) { shared++; }
来源：http://th.jianghongdianzi.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ov.bookmarksfly.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://lm.hahajie.cn

C#:   lock (gate) { shared++; }
来源：http://eo.huixiangedu.cn

[O04] 定义异步函数并等待
来源：http://lb.9csxet.cn

Py:   async def f():⏎    await g()
来源：http://rc.colortex.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://it.panjiajie.cn

JS:   async function f() { await g(); }
来源：http://ew.wgjwhj.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://cm.hahajie.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://os.asd995.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://uc.jianghongdianzi.cn

Ruby: # 用 Fiber 或 async gem
来源：http://nl.9csxet.cn

C#:   async Task F() { await G(); }
来源：http://hl.haigaiapp.cn

[O05] 并发执行并等待全部完成
来源：http://zp.shxzukj.cn

Py:   asyncio.gather(*tasks)
来源：http://uh.hnjuh.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://zs.yuexingan06.cn

JS:   await Promise.all(tasks)
来源：http://tg.bookmarksfly.cn

TS:   await Promise.all(tasks)
来源：http://ou.huixiangedu.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mt.szsharing.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://oo.9csxet.cn

Ruby: threads.map(&:join)
来源：http://in.colortex.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://xq.lnxyls.cn

[O06] 使用进程池
来源：http://jr.hahajie.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://dt.huanxung.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://ut.lnxyls.cn

JS:   // child_process / cluster 模块
来源：http://yj.huanxung.cn

TS:   // child_process / cluster 模块
来源：http://sc.asd995.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://gd.yuexingan06.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://kl.hnjuh.cn

Ruby: // fork 块
来源：http://wg.asd995.cn

C#:   Parallel.For
来源：http://ee.colortex.cn

================================================================================
来源：http://rk.lnxyls.cn

P. 常用工具函数
来源：http://nn.chemitech.net.cn

================================================================================
来源：http://zy.huanxung.cn

[P01] 生成 UUID
来源：http://vi.szxytkj.cn

Py:   str(uuid.uuid4())
来源：http://zm.huixiangedu.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://gj.521024.cn

JS:   crypto.randomUUID()
来源：http://yl.shxzukj.cn

TS:   crypto.randomUUID()
来源：http://it.jianghongdianzi.cn

Java: UUID.randomUUID().toString()
来源：http://nj.shxzskj.cn

Go:   // 用 github.com/google/uuid
来源：http://cp.chemitech.net.cn

Ruby: SecureRandom.uuid
来源：http://hn.chemitech.net.cn

C#:   Guid.NewGuid().ToString()
来源：http://ni.hahajie.cn

[P02] MD5 / SHA256 摘要
来源：http://mv.szxytkj.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://pu.521024.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://lg.9csxet.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://gr.huixinmuqiang.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://eu.yuntaijiaju.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://te.szxytkj.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hn.colortex.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ps.nicolike.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://qy.yuexingan06.cn

[P03] 生成短随机字符串
来源：http://zn.521024.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ea.521024.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ba.shxzskj.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://td.nszjky.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://dw.chemitech.net.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://dr.haigaiapp.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://fp.muxihuayi.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://mw.hahajie.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://qn.jctech888.com.cn

[P04] 求长度
来源：http://ie.huixinmuqiang.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://br.colortex.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://um.szxytkj.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hr.bookmarksfly.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://lz.panjiajie.cn

Java: list.size();  map.size();  s.length()
来源：http://ti.huanxung.cn

Go:   len(arr);  len(m)
来源：http://rh.jianghongdianzi.cn

Ruby: x.length;  x.size
来源：http://ax.gzmigu.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://kn.huixinmuqiang.cn

[P05] 判断两个对象内容是否相等
来源：http://gm.bookmarksfly.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://il.yuexingan06.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://na.asd995.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://cp.lnxyls.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ur.nszjky.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://oi.nszjky.cn

Go:   reflect.DeepEqual(a, b)
来源：http://fv.9csxet.cn

Ruby: a == b
来源：http://iy.panjiajie.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://os.hnjuh.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://kk.hnjuh.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://fl.lnxyls.cn

PHP:  if (empty($x)) {}
来源：http://hl.muxihuayi.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://cc.nicolike.cn

TS:   if (x == null) {}
来源：http://km.huixinmuqiang.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://js.haigaiapp.cn

Go:   if x == nil {}
来源：http://yt.szxytkj.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://kx.bookmarksfly.cn

C#:   if (x is null) {}
来源：http://bw.newstarts.cn

[P07] 防抖与节流
来源：http://vs.wgjwhj.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://xt.chemitech.net.cn

PHP:  // 手写时间戳比较
来源：http://dt.bjjhwx.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ol.muxihuayi.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qc.jianghongdianzi.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://lr.chemitech.net.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://th.521024.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://wr.yuntaijiaju.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ou.shxzukj.cn

[P08] 处理浮点精度问题
来源：http://wm.shxzskj.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://cs.9csxet.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://kj.chemitech.net.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://od.yuntaijiaju.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://fn.muxihuayi.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://pt.yuexingan06.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://rk.haigaiapp.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ca.gzmigu.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://xy.colortex.cn

================================================================================
来源：http://vl.panjiajie.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://px.colortex.cn

================================================================================
来源：http://et.asd995.cn

[Q01] 创建表
来源：http://hm.muxihuayi.cn

CREATE TABLE users (
来源：http://hv.lnxyls.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://rg.colortex.cn

name VARCHAR(50) NOT NULL,
来源：http://yz.yuntaijiaju.cn

email VARCHAR(100) UNIQUE,
来源：http://jq.haigaiapp.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://qg.panjiajie.cn

);
来源：http://cl.hnjuh.cn

[Q02] 创建带外键的表
来源：http://on.muxihuayi.cn

CREATE TABLE orders (
来源：http://jb.szsharing.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ts.bjjhwx.cn

user_id INT NOT NULL,
来源：http://ht.bjjhwx.cn

amount DECIMAL(10, 2),
来源：http://gc.hnjuh.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://un.bookmarksfly.cn

);
来源：http://hc.hahajie.cn

[Q03] 增加列
来源：http://rw.shxzukj.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://zy.huixiangedu.cn

[Q04] 修改列类型
来源：http://wb.haigaiapp.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wb.huanxung.cn

[Q05] 重命名列
来源：http://jz.huanxung.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ny.hnjuh.cn

[Q06] 删除列
来源：http://ca.huanxung.cn

ALTER TABLE users DROP COLUMN age;
来源：http://on.chemitech.net.cn

[Q07] 删除表
来源：http://ah.shtwfgs.cn

DROP TABLE IF EXISTS orders;
来源：http://mj.bjjhwx.cn

[Q08] 创建普通索引
来源：http://wz.newstarts.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://ak.hahajie.cn

[Q09] 创建唯一索引
来源：http://hr.yuntaijiaju.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://dj.9csxet.cn

[Q10] 插入单行
来源：http://ir.muxihuayi.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://lp.jctech888.com.cn

[Q11] 一次插入多行
来源：http://mi.muxihuayi.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wf.asd995.cn

[Q12] 插入后取自增 ID
来源：http://cy.bjjhwx.cn

INSERT INTO users (name) VALUES ('C');
来源：http://aa.huanxung.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://yn.521024.cn

[Q13] 忽略重复插入
来源：http://pm.shxzukj.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://gf.yuntaijiaju.cn

[Q14] 存在则更新（upsert）
来源：http://fc.521024.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ku.panjiajie.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://xk.9csxet.cn

[Q15] 查询全部
来源：http://pr.nicolike.cn

SELECT * FROM users;
来源：http://mx.szxytkj.cn

[Q16] 查询指定列
来源：http://kd.yuexingan06.cn

SELECT id, name FROM users;
来源：http://nw.jianghongdianzi.cn

[Q17] 条件查询
来源：http://fe.panjiajie.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://bp.9csxet.cn

[Q18] 模糊匹配
来源：http://sn.yuntaijiaju.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://rg.lnxyls.cn

[Q19] 范围查询
来源：http://ta.chemitech.net.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://so.szxytkj.cn

[Q20] IN 列表
来源：http://jc.hnjuh.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ek.shtwfgs.cn

[Q21] 空值判断
来源：http://qq.nicolike.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://ke.gzmigu.cn

[Q22] 排序
来源：http://hi.bjjhwx.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ze.hnjuh.cn

[Q23] 分页
来源：http://bf.panjiajie.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://cy.bookmarksfly.cn

[Q24] 去重
来源：http://pg.nszjky.cn

SELECT DISTINCT city FROM users;
来源：http://dy.521024.cn

[Q25] 只取前 N 条
来源：http://re.colortex.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://kj.jianghongdianzi.cn

[Q26] 计数
来源：http://va.chemitech.net.cn

SELECT COUNT(*) FROM users;
来源：http://tn.shxzskj.cn

[Q27] 条件计数
来源：http://ig.newstarts.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wm.asd995.cn

[Q28] 求和与平均
来源：http://pv.bjjhwx.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://gg.bjjhwx.cn

[Q29] 最大最小值
来源：http://rp.chemitech.net.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://om.shtwfgs.cn

[Q30] 分组统计
来源：http://od.yuntaijiaju.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://lc.hnjuh.cn

[Q31] 分组后过滤
来源：http://pq.wgjwhj.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://zu.shtwfgs.cn

[Q32] 分组拼接字符串
来源：http://ii.shxzskj.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ki.newstarts.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://fy.huanxung.cn

[Q33] 多列分组
来源：http://sk.jctech888.com.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://jq.asd995.cn

[Q34] 每组取第一条
来源：http://ja.huixiangedu.cn

SELECT * FROM (
来源：http://qa.szxytkj.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://oo.lnxyls.cn

) t WHERE rn = 1;
来源：http://sy.shxzskj.cn

[Q35] 内连接
来源：http://gi.shtwfgs.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://gj.521024.cn

[Q36] 左连接
来源：http://dd.wgjwhj.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mf.yuexingan06.cn

[Q37] 右连接
来源：http://ki.shtwfgs.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ze.9csxet.cn

[Q38] 全外连接（PostgreSQL）
来源：http://dq.huixiangedu.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hp.chemitech.net.cn

[Q39] 自连接（查上下级）
来源：http://ci.nicolike.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://oy.jianghongdianzi.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hv.jctech888.com.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://cm.9csxet.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://dp.hnjuh.cn

[Q41] 多表连接
来源：http://wz.shxzukj.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://iq.shxzskj.cn

JOIN users u ON u.id = o.user_id
来源：http://an.9csxet.cn

JOIN products p ON p.id = o.product_id;
来源：http://bb.hahajie.cn

[Q42] 连接条件附加过滤
来源：http://ny.shxzskj.cn

SELECT u.name, o.amount FROM users u
来源：http://ee.521024.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ht.shxzskj.cn

[Q43] 标量子查询
来源：http://ba.colortex.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://vv.shtwfgs.cn

[Q44] IN 子查询
来源：http://hy.szsharing.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://sn.asd995.cn

[Q45] EXISTS 判断存在
来源：http://ma.szxytkj.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://no.szsharing.cn

[Q46] NOT EXISTS 判断不存在
来源：http://zm.jctech888.com.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://th.9csxet.cn

[Q47] 与平均值比较
来源：http://as.shxzukj.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://kf.nicolike.cn

[Q48] CTE 公用表表达式
来源：http://ps.huixinmuqiang.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://uc.szxytkj.cn

SELECT * FROM t WHERE c > 5;
来源：http://jc.521024.cn

[Q49] 更新单行
来源：http://eo.bookmarksfly.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://dn.521024.cn

[Q50] 批量更新
来源：http://qm.chemitech.net.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mo.newstarts.cn

[Q51] 用子查询更新
来源：http://cc.newstarts.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hn.huixiangedu.cn

[Q52] 删除指定行
来源：http://xc.jianghongdianzi.cn

DELETE FROM users WHERE id = 10;
来源：http://ju.bookmarksfly.cn

[Q53] 按条件删除
来源：http://yz.gzmigu.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mi.chemitech.net.cn

[Q54] 清空表
来源：http://tj.hnjuh.cn

TRUNCATE TABLE logs;
来源：http://su.newstarts.cn

[Q55] 排名（并列占位）
来源：http://zh.521024.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://cj.wgjwhj.cn

[Q56] 密集排名（并列不占位）
来源：http://bn.nicolike.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://qu.shxzukj.cn

[Q57] 行号
来源：http://vu.nszjky.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ec.newstarts.cn

[Q58] 累计求和
来源：http://pz.bjjhwx.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://jm.haigaiapp.cn

[Q59] 分组内累计
来源：http://lt.bjjhwx.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://df.muxihuayi.cn

[Q60] 取上一行 / 下一行
来源：http://ne.bookmarksfly.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://nl.muxihuayi.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://vj.shtwfgs.cn

[Q61] 移动平均
来源：http://ey.szxytkj.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mr.hnjuh.cn

[Q62] 分组占比
来源：http://si.hahajie.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wb.huixinmuqiang.cn

[Q63] 开启事务
来源：http://mc.shxzskj.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://ne.newstarts.cn

[Q64] 提交事务
来源：http://mb.nicolike.cn

COMMIT;
来源：http://hi.szsharing.cn

[Q65] 回滚事务
来源：http://cw.szxytkj.cn

ROLLBACK;
来源：http://lh.hahajie.cn

[Q66] 行锁查询
来源：http://cd.newstarts.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mf.huixinmuqiang.cn

[Q67] 设置隔离级别
来源：http://md.9csxet.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hn.wgjwhj.cn

[Q68] 保存点
来源：http://mk.huixinmuqiang.cn

SAVEPOINT sp1;
来源：http://mo.nicolike.cn

ROLLBACK TO sp1;
来源：http://vs.colortex.cn

[Q69] 查看执行计划
来源：http://xj.huixinmuqiang.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ix.huixiangedu.cn

[Q70] 更新统计信息
来源：http://ho.szsharing.cn


<!-- 参考信息 -->