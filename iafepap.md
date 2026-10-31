代发 wailian999

PHP:  // 手写递归函数
来源：http://fr.huixiangedu.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://to.jianghongdianzi.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://tn.asd995.cn

Java: // 手写递归
来源：http://zq.asd995.cn

Go:   // 手写递归
来源：http://vb.hahajie.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ac.hahajie.cn

C#:   // 手写递归
来源：http://uc.chemitech.net.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://lh.wgjwhj.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ky.asd995.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hk.hnjuh.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://fr.9csxet.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://bn.jctech888.com.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wh.chemitech.net.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://dj.jctech888.com.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wb.szxytkj.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://lk.jianghongdianzi.cn

================================================================================
来源：http://re.huixinmuqiang.cn

O. 并发与异步
来源：http://xn.shxzukj.cn

================================================================================
来源：http://vz.szxytkj.cn

[O01] 启动一个线程
来源：http://xi.bjjhwx.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://fy.panjiajie.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://fh.nszjky.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ne.asd995.cn

TS:   // 同 JS
来源：http://nj.nicolike.cn

Java: new Thread(() -> f()).start()
来源：http://do.huanxung.cn

Go:   go f()
来源：http://hx.9csxet.cn

Ruby: Thread.new { f }
来源：http://kj.szxytkj.cn

C#:   Task.Run(() => F());
来源：http://vl.bookmarksfly.cn

[O02] 使用线程池
来源：http://nx.nszjky.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mu.colortex.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ha.hnjuh.cn

JS:   // worker_threads 线程池
来源：http://fv.gzmigu.cn

TS:   // worker_threads 线程池
来源：http://ha.shtwfgs.cn

Java: Executors.newFixedThreadPool(4)
来源：http://gm.521024.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://rc.nszjky.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://iz.bjjhwx.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wx.chemitech.net.cn

[O03] 加锁保护共享数据
来源：http://up.szsharing.cn

Py:   with lock: shared += 1
来源：http://ad.hnjuh.cn

PHP:  // 用 flock() 做文件锁
来源：http://st.bookmarksfly.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://cl.huixinmuqiang.cn

TS:   // 同 JS
来源：http://pn.panjiajie.cn

Java: synchronized (this) { shared++; }
来源：http://sx.colortex.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ap.521024.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://xh.bookmarksfly.cn

C#:   lock (gate) { shared++; }
来源：http://rr.panjiajie.cn

[O04] 定义异步函数并等待
来源：http://db.panjiajie.cn

Py:   async def f():⏎    await g()
来源：http://sh.wgjwhj.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://qm.wgjwhj.cn

JS:   async function f() { await g(); }
来源：http://xk.huixiangedu.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://ok.nicolike.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://zq.jianghongdianzi.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hb.nicolike.cn

Ruby: # 用 Fiber 或 async gem
来源：http://xt.huixinmuqiang.cn

C#:   async Task F() { await G(); }
来源：http://qm.bjjhwx.cn

[O05] 并发执行并等待全部完成
来源：http://rq.hnjuh.cn

Py:   asyncio.gather(*tasks)
来源：http://ys.lnxyls.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://pv.hahajie.cn

JS:   await Promise.all(tasks)
来源：http://qo.nicolike.cn

TS:   await Promise.all(tasks)
来源：http://pz.bookmarksfly.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://gs.nicolike.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ih.shxzskj.cn

Ruby: threads.map(&:join)
来源：http://jv.szxytkj.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://qf.muxihuayi.cn

[O06] 使用进程池
来源：http://kt.jctech888.com.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://px.shxzukj.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://vb.521024.cn

JS:   // child_process / cluster 模块
来源：http://wj.shxzskj.cn

TS:   // child_process / cluster 模块
来源：http://tz.panjiajie.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://iz.szxytkj.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mz.szxytkj.cn

Ruby: // fork 块
来源：http://wq.bjjhwx.cn

C#:   Parallel.For
来源：http://nl.lnxyls.cn

================================================================================
来源：http://bh.huixiangedu.cn

P. 常用工具函数
来源：http://xi.lnxyls.cn

================================================================================
来源：http://dz.huixinmuqiang.cn

[P01] 生成 UUID
来源：http://ul.jianghongdianzi.cn

Py:   str(uuid.uuid4())
来源：http://vw.wgjwhj.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://jd.chemitech.net.cn

JS:   crypto.randomUUID()
来源：http://ds.panjiajie.cn

TS:   crypto.randomUUID()
来源：http://aa.huanxung.cn

Java: UUID.randomUUID().toString()
来源：http://rb.jianghongdianzi.cn

Go:   // 用 github.com/google/uuid
来源：http://ib.jctech888.com.cn

Ruby: SecureRandom.uuid
来源：http://he.haigaiapp.cn

C#:   Guid.NewGuid().ToString()
来源：http://ez.bookmarksfly.cn

[P02] MD5 / SHA256 摘要
来源：http://zp.bjjhwx.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://gn.szxytkj.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://xy.wgjwhj.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://zx.nicolike.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://px.muxihuayi.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://yf.hnjuh.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://xq.colortex.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://to.shxzukj.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://gf.nszjky.cn

[P03] 生成短随机字符串
来源：http://ec.panjiajie.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://zu.chemitech.net.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mh.bookmarksfly.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://jr.haigaiapp.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://zk.newstarts.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://of.huixinmuqiang.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://xo.jianghongdianzi.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://ik.panjiajie.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://rw.wgjwhj.cn

[P04] 求长度
来源：http://um.shxzukj.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://fs.colortex.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://xc.szsharing.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://xi.huixiangedu.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://jb.hahajie.cn

Java: list.size();  map.size();  s.length()
来源：http://eq.gzmigu.cn

Go:   len(arr);  len(m)
来源：http://rl.chemitech.net.cn

Ruby: x.length;  x.size
来源：http://bf.muxihuayi.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://wg.colortex.cn

[P05] 判断两个对象内容是否相等
来源：http://jt.gzmigu.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://kv.nszjky.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://bq.huixinmuqiang.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mx.chemitech.net.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hi.newstarts.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ii.wgjwhj.cn

Go:   reflect.DeepEqual(a, b)
来源：http://qw.colortex.cn

Ruby: a == b
来源：http://kq.szsharing.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://fe.lnxyls.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://kk.szxytkj.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://uv.jianghongdianzi.cn

PHP:  if (empty($x)) {}
来源：http://fk.chemitech.net.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://qy.szxytkj.cn

TS:   if (x == null) {}
来源：http://ke.shtwfgs.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://hc.hnjuh.cn

Go:   if x == nil {}
来源：http://jq.jctech888.com.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ox.wgjwhj.cn

C#:   if (x is null) {}
来源：http://bs.newstarts.cn

[P07] 防抖与节流
来源：http://ee.nszjky.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://xg.jctech888.com.cn

PHP:  // 手写时间戳比较
来源：http://kz.9csxet.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://cz.huanxung.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mf.szsharing.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://dx.asd995.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://qn.shxzskj.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://sg.szsharing.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://aq.9csxet.cn

[P08] 处理浮点精度问题
来源：http://bj.jctech888.com.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://gt.shtwfgs.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ns.521024.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://kp.bjjhwx.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://nx.lnxyls.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://kx.szsharing.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://un.shtwfgs.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://bl.gzmigu.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://xf.jctech888.com.cn

================================================================================
来源：http://dq.nicolike.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://rn.huixiangedu.cn

================================================================================
来源：http://ej.chemitech.net.cn

[Q01] 创建表
来源：http://yd.shtwfgs.cn

CREATE TABLE users (
来源：http://kt.jianghongdianzi.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://tq.colortex.cn

name VARCHAR(50) NOT NULL,
来源：http://lb.hnjuh.cn

email VARCHAR(100) UNIQUE,
来源：http://us.shxzskj.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://oj.jctech888.com.cn

);
来源：http://yr.asd995.cn

[Q02] 创建带外键的表
来源：http://xi.huixinmuqiang.cn

CREATE TABLE orders (
来源：http://ys.shxzukj.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://kd.huixinmuqiang.cn

user_id INT NOT NULL,
来源：http://sr.shxzukj.cn

amount DECIMAL(10, 2),
来源：http://au.colortex.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://yy.szxytkj.cn

);
来源：http://dj.szxytkj.cn

[Q03] 增加列
来源：http://nz.panjiajie.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://lx.huanxung.cn

[Q04] 修改列类型
来源：http://jj.colortex.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ng.yuexingan06.cn

[Q05] 重命名列
来源：http://ga.asd995.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://pp.yuntaijiaju.cn

[Q06] 删除列
来源：http://or.9csxet.cn

ALTER TABLE users DROP COLUMN age;
来源：http://cc.chemitech.net.cn

[Q07] 删除表
来源：http://gj.huanxung.cn

DROP TABLE IF EXISTS orders;
来源：http://hc.hnjuh.cn

[Q08] 创建普通索引
来源：http://oa.bookmarksfly.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://bu.colortex.cn

[Q09] 创建唯一索引
来源：http://dw.szxytkj.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://jj.newstarts.cn

[Q10] 插入单行
来源：http://yx.muxihuayi.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://al.bookmarksfly.cn

[Q11] 一次插入多行
来源：http://qe.shtwfgs.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://gs.bjjhwx.cn

[Q12] 插入后取自增 ID
来源：http://pp.newstarts.cn

INSERT INTO users (name) VALUES ('C');
来源：http://sc.jianghongdianzi.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://qu.hahajie.cn

[Q13] 忽略重复插入
来源：http://pe.hnjuh.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ei.shxzskj.cn

[Q14] 存在则更新（upsert）
来源：http://qy.bjjhwx.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://in.bjjhwx.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mq.huanxung.cn

[Q15] 查询全部
来源：http://lx.nicolike.cn

SELECT * FROM users;
来源：http://kr.haigaiapp.cn

[Q16] 查询指定列
来源：http://va.bookmarksfly.cn

SELECT id, name FROM users;
来源：http://up.hahajie.cn

[Q17] 条件查询
来源：http://my.colortex.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://qv.szxytkj.cn

[Q18] 模糊匹配
来源：http://by.wgjwhj.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://nk.asd995.cn

[Q19] 范围查询
来源：http://cr.lnxyls.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://pm.newstarts.cn

[Q20] IN 列表
来源：http://ga.haigaiapp.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://yd.hnjuh.cn

[Q21] 空值判断
来源：http://dz.newstarts.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://zk.chemitech.net.cn

[Q22] 排序
来源：http://sd.wgjwhj.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://pf.huixinmuqiang.cn

[Q23] 分页
来源：http://ok.nicolike.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://dp.huixiangedu.cn

[Q24] 去重
来源：http://nt.yuntaijiaju.cn

SELECT DISTINCT city FROM users;
来源：http://sx.jctech888.com.cn

[Q25] 只取前 N 条
来源：http://li.9csxet.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ig.asd995.cn

[Q26] 计数
来源：http://iv.9csxet.cn

SELECT COUNT(*) FROM users;
来源：http://hl.wgjwhj.cn

[Q27] 条件计数
来源：http://bl.hahajie.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ie.bookmarksfly.cn

[Q28] 求和与平均
来源：http://zp.haigaiapp.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://ki.jctech888.com.cn

[Q29] 最大最小值
来源：http://fd.panjiajie.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://gl.jianghongdianzi.cn

[Q30] 分组统计
来源：http://mj.szxytkj.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://gj.jctech888.com.cn

[Q31] 分组后过滤
来源：http://wx.gzmigu.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://le.gzmigu.cn

[Q32] 分组拼接字符串
来源：http://io.chemitech.net.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://sd.wgjwhj.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://qj.panjiajie.cn

[Q33] 多列分组
来源：http://jk.hnjuh.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://is.yuntaijiaju.cn

[Q34] 每组取第一条
来源：http://nf.szxytkj.cn

SELECT * FROM (
来源：http://qy.muxihuayi.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://dm.shxzukj.cn

) t WHERE rn = 1;
来源：http://ge.bookmarksfly.cn

[Q35] 内连接
来源：http://qm.shxzskj.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://cg.huanxung.cn

[Q36] 左连接
来源：http://jn.huanxung.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://xg.muxihuayi.cn

[Q37] 右连接
来源：http://nx.bjjhwx.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://oq.shtwfgs.cn

[Q38] 全外连接（PostgreSQL）
来源：http://hb.muxihuayi.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://oq.haigaiapp.cn

[Q39] 自连接（查上下级）
来源：http://st.hnjuh.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://oh.jctech888.com.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://jz.yuexingan06.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://ok.szxytkj.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ae.lnxyls.cn

[Q41] 多表连接
来源：http://gn.huixiangedu.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://yd.hnjuh.cn

JOIN users u ON u.id = o.user_id
来源：http://id.colortex.cn

JOIN products p ON p.id = o.product_id;
来源：http://xs.newstarts.cn

[Q42] 连接条件附加过滤
来源：http://gv.nicolike.cn

SELECT u.name, o.amount FROM users u
来源：http://uv.nicolike.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://la.bookmarksfly.cn

[Q43] 标量子查询
来源：http://la.haigaiapp.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wb.colortex.cn

[Q44] IN 子查询
来源：http://vh.haigaiapp.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://to.szsharing.cn

[Q45] EXISTS 判断存在
来源：http://xd.jianghongdianzi.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://te.nicolike.cn

[Q46] NOT EXISTS 判断不存在
来源：http://sr.bookmarksfly.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://zi.huixiangedu.cn

[Q47] 与平均值比较
来源：http://wq.haigaiapp.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://it.huanxung.cn

[Q48] CTE 公用表表达式
来源：http://ik.muxihuayi.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://bk.shxzskj.cn

SELECT * FROM t WHERE c > 5;
来源：http://ul.newstarts.cn

[Q49] 更新单行
来源：http://jh.wgjwhj.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://zs.szsharing.cn

[Q50] 批量更新
来源：http://wx.gzmigu.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://ap.huanxung.cn

[Q51] 用子查询更新
来源：http://wn.panjiajie.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://nt.newstarts.cn

[Q52] 删除指定行
来源：http://if.hnjuh.cn

DELETE FROM users WHERE id = 10;
来源：http://qj.jctech888.com.cn

[Q53] 按条件删除
来源：http://ij.shxzukj.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://zk.jctech888.com.cn

[Q54] 清空表
来源：http://eb.muxihuayi.cn

TRUNCATE TABLE logs;
来源：http://vh.bookmarksfly.cn

[Q55] 排名（并列占位）
来源：http://he.szsharing.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://vd.yuexingan06.cn

[Q56] 密集排名（并列不占位）
来源：http://bv.shxzukj.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mv.szsharing.cn

[Q57] 行号
来源：http://kq.newstarts.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://jr.9csxet.cn

[Q58] 累计求和
来源：http://js.huixinmuqiang.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://lj.yuntaijiaju.cn

[Q59] 分组内累计
来源：http://kw.yuexingan06.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://gx.huixinmuqiang.cn

[Q60] 取上一行 / 下一行
来源：http://im.shxzskj.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://zz.newstarts.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://uf.yuexingan06.cn

[Q61] 移动平均
来源：http://vy.shxzukj.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://dl.wgjwhj.cn

[Q62] 分组占比
来源：http://pf.szsharing.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wl.bookmarksfly.cn

[Q63] 开启事务
来源：http://do.colortex.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://ov.gzmigu.cn

[Q64] 提交事务
来源：http://ay.szsharing.cn

COMMIT;
来源：http://mo.hnjuh.cn


<!-- 参考信息 -->