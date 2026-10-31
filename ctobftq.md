代发 wailian999

TS:   arr.push(x) / arr.pop() 作栈
来源：http://gd.asd995.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://fg.huixiangedu.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://np.muxihuayi.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://em.muxihuayi.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://xq.yuexingan06.cn

[N10] 链表节点定义
来源：http://fr.gzmigu.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wm.yuexingan06.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://zh.nszjky.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://rr.9csxet.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://uw.chemitech.net.cn

Java: class Node { int v; Node next; }
来源：http://eq.huixinmuqiang.cn

Go:   type Node struct { V int; Next *Node }
来源：http://ry.panjiajie.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://rn.panjiajie.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://zb.hahajie.cn

[N11] 二叉树中序遍历
来源：http://ip.hnjuh.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hw.panjiajie.cn

PHP:  // 手写递归函数
来源：http://kj.panjiajie.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://qi.bookmarksfly.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://oh.bookmarksfly.cn

Java: // 手写递归
来源：http://jv.panjiajie.cn

Go:   // 手写递归
来源：http://pe.wgjwhj.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://br.yuntaijiaju.cn

C#:   // 手写递归
来源：http://tw.bjjhwx.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://we.asd995.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://na.shtwfgs.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://tb.521024.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://rv.panjiajie.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://pz.colortex.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://vv.hahajie.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ln.yuntaijiaju.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://rn.bjjhwx.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://su.bookmarksfly.cn

================================================================================
来源：http://lf.szxytkj.cn

O. 并发与异步
来源：http://cd.9csxet.cn

================================================================================
来源：http://xa.gzmigu.cn

[O01] 启动一个线程
来源：http://ms.nszjky.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://cw.shtwfgs.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://xu.haigaiapp.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://db.shtwfgs.cn

TS:   // 同 JS
来源：http://nz.newstarts.cn

Java: new Thread(() -> f()).start()
来源：http://wn.9csxet.cn

Go:   go f()
来源：http://em.lnxyls.cn

Ruby: Thread.new { f }
来源：http://wa.yuexingan06.cn

C#:   Task.Run(() => F());
来源：http://vw.haigaiapp.cn

[O02] 使用线程池
来源：http://wp.hnjuh.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://kn.shxzukj.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://cm.muxihuayi.cn

JS:   // worker_threads 线程池
来源：http://ey.nszjky.cn

TS:   // worker_threads 线程池
来源：http://cd.asd995.cn

Java: Executors.newFixedThreadPool(4)
来源：http://uv.521024.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ix.shtwfgs.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://lc.jctech888.com.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://tt.haigaiapp.cn

[O03] 加锁保护共享数据
来源：http://pb.huixiangedu.cn

Py:   with lock: shared += 1
来源：http://ab.yuexingan06.cn

PHP:  // 用 flock() 做文件锁
来源：http://kd.colortex.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://fn.gzmigu.cn

TS:   // 同 JS
来源：http://id.panjiajie.cn

Java: synchronized (this) { shared++; }
来源：http://zd.shxzukj.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://oi.hahajie.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://px.nicolike.cn

C#:   lock (gate) { shared++; }
来源：http://vq.yuntaijiaju.cn

[O04] 定义异步函数并等待
来源：http://bw.colortex.cn

Py:   async def f():⏎    await g()
来源：http://yl.521024.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://az.huanxung.cn

JS:   async function f() { await g(); }
来源：http://su.nszjky.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://ma.bookmarksfly.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wz.hahajie.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://gk.muxihuayi.cn

Ruby: # 用 Fiber 或 async gem
来源：http://qe.huanxung.cn

C#:   async Task F() { await G(); }
来源：http://gx.lnxyls.cn

[O05] 并发执行并等待全部完成
来源：http://zr.szsharing.cn

Py:   asyncio.gather(*tasks)
来源：http://cy.panjiajie.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://tt.panjiajie.cn

JS:   await Promise.all(tasks)
来源：http://hz.newstarts.cn

TS:   await Promise.all(tasks)
来源：http://ui.huixinmuqiang.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://sa.shtwfgs.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://my.shtwfgs.cn

Ruby: threads.map(&:join)
来源：http://tv.9csxet.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://zg.9csxet.cn

[O06] 使用进程池
来源：http://mc.szsharing.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://sm.hnjuh.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://kk.shxzskj.cn

JS:   // child_process / cluster 模块
来源：http://ze.panjiajie.cn

TS:   // child_process / cluster 模块
来源：http://lp.shxzukj.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://kp.hahajie.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ez.jctech888.com.cn

Ruby: // fork 块
来源：http://th.jctech888.com.cn

C#:   Parallel.For
来源：http://xr.yuexingan06.cn

================================================================================
来源：http://pr.9csxet.cn

P. 常用工具函数
来源：http://um.bookmarksfly.cn

================================================================================
来源：http://vt.muxihuayi.cn

[P01] 生成 UUID
来源：http://db.nszjky.cn

Py:   str(uuid.uuid4())
来源：http://ze.jctech888.com.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mk.hahajie.cn

JS:   crypto.randomUUID()
来源：http://fv.yuntaijiaju.cn

TS:   crypto.randomUUID()
来源：http://jw.huixinmuqiang.cn

Java: UUID.randomUUID().toString()
来源：http://jf.wgjwhj.cn

Go:   // 用 github.com/google/uuid
来源：http://kz.shxzukj.cn

Ruby: SecureRandom.uuid
来源：http://tt.hnjuh.cn

C#:   Guid.NewGuid().ToString()
来源：http://jt.huanxung.cn

[P02] MD5 / SHA256 摘要
来源：http://mq.bjjhwx.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://dx.chemitech.net.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://hj.newstarts.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://pi.shxzukj.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ab.szsharing.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ee.521024.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://si.nszjky.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://sc.szxytkj.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ls.hnjuh.cn

[P03] 生成短随机字符串
来源：http://ty.jctech888.com.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://jv.9csxet.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://vc.huanxung.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://eu.huanxung.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://aq.asd995.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ea.newstarts.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ld.nszjky.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://tb.huanxung.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://kp.9csxet.cn

[P04] 求长度
来源：http://ba.shxzukj.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ov.bookmarksfly.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ss.panjiajie.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://vz.colortex.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://cr.haigaiapp.cn

Java: list.size();  map.size();  s.length()
来源：http://ws.panjiajie.cn

Go:   len(arr);  len(m)
来源：http://yy.asd995.cn

Ruby: x.length;  x.size
来源：http://dw.yuexingan06.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://hy.bookmarksfly.cn

[P05] 判断两个对象内容是否相等
来源：http://fs.gzmigu.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://cj.nicolike.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://au.shxzskj.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ui.huixiangedu.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://cn.521024.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://lm.bookmarksfly.cn

Go:   reflect.DeepEqual(a, b)
来源：http://gi.lnxyls.cn

Ruby: a == b
来源：http://ei.9csxet.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ii.shtwfgs.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://vo.jianghongdianzi.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mt.521024.cn

PHP:  if (empty($x)) {}
来源：http://ck.huixiangedu.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ss.szsharing.cn

TS:   if (x == null) {}
来源：http://cq.521024.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://if.huanxung.cn

Go:   if x == nil {}
来源：http://ek.jianghongdianzi.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://pb.shxzukj.cn

C#:   if (x is null) {}
来源：http://gr.colortex.cn

[P07] 防抖与节流
来源：http://lc.gzmigu.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://rg.nszjky.cn

PHP:  // 手写时间戳比较
来源：http://fw.hnjuh.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://dl.nszjky.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://su.chemitech.net.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ve.hnjuh.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://gl.huixiangedu.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://es.haigaiapp.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://qo.gzmigu.cn

[P08] 处理浮点精度问题
来源：http://lg.muxihuayi.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ue.asd995.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://gi.521024.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ea.chemitech.net.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://qx.nszjky.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://up.hahajie.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://xe.huanxung.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ai.nicolike.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ow.hahajie.cn

================================================================================
来源：http://ki.huanxung.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://st.huixiangedu.cn

================================================================================
来源：http://wb.jianghongdianzi.cn

[Q01] 创建表
来源：http://jh.szsharing.cn

CREATE TABLE users (
来源：http://kk.shxzukj.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://nl.asd995.cn

name VARCHAR(50) NOT NULL,
来源：http://zc.shxzukj.cn

email VARCHAR(100) UNIQUE,
来源：http://tt.panjiajie.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://yl.szsharing.cn

);
来源：http://rl.nszjky.cn

[Q02] 创建带外键的表
来源：http://mk.hnjuh.cn

CREATE TABLE orders (
来源：http://qg.521024.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://tv.huanxung.cn

user_id INT NOT NULL,
来源：http://hs.shxzskj.cn

amount DECIMAL(10, 2),
来源：http://hd.yuntaijiaju.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://gj.huanxung.cn

);
来源：http://wp.521024.cn

[Q03] 增加列
来源：http://zr.yuexingan06.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ch.lnxyls.cn

[Q04] 修改列类型
来源：http://yh.521024.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ap.haigaiapp.cn

[Q05] 重命名列
来源：http://sb.jianghongdianzi.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wq.newstarts.cn

[Q06] 删除列
来源：http://tf.chemitech.net.cn

ALTER TABLE users DROP COLUMN age;
来源：http://ef.yuntaijiaju.cn

[Q07] 删除表
来源：http://qa.yuexingan06.cn

DROP TABLE IF EXISTS orders;
来源：http://zd.nszjky.cn

[Q08] 创建普通索引
来源：http://kc.nszjky.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://fe.huixinmuqiang.cn

[Q09] 创建唯一索引
来源：http://cx.yuexingan06.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://lq.shxzukj.cn

[Q10] 插入单行
来源：http://bg.jctech888.com.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://rs.huixiangedu.cn

[Q11] 一次插入多行
来源：http://ov.jianghongdianzi.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ow.lnxyls.cn

[Q12] 插入后取自增 ID
来源：http://dc.chemitech.net.cn

INSERT INTO users (name) VALUES ('C');
来源：http://oy.huixiangedu.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://do.szsharing.cn

[Q13] 忽略重复插入
来源：http://ws.szsharing.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://sx.szxytkj.cn

[Q14] 存在则更新（upsert）
来源：http://bo.yuntaijiaju.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://qu.lnxyls.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://su.bookmarksfly.cn

[Q15] 查询全部
来源：http://on.shxzukj.cn

SELECT * FROM users;
来源：http://lc.jctech888.com.cn

[Q16] 查询指定列
来源：http://it.bookmarksfly.cn

SELECT id, name FROM users;
来源：http://bf.muxihuayi.cn

[Q17] 条件查询
来源：http://te.9csxet.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ac.bjjhwx.cn

[Q18] 模糊匹配
来源：http://bm.haigaiapp.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://rr.yuntaijiaju.cn

[Q19] 范围查询
来源：http://ku.asd995.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ez.szsharing.cn

[Q20] IN 列表
来源：http://wf.wgjwhj.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ei.newstarts.cn

[Q21] 空值判断
来源：http://qp.szsharing.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://oh.panjiajie.cn

[Q22] 排序
来源：http://kh.huixinmuqiang.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://bg.yuexingan06.cn

[Q23] 分页
来源：http://es.newstarts.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://uc.shxzskj.cn

[Q24] 去重
来源：http://yc.huanxung.cn

SELECT DISTINCT city FROM users;
来源：http://kc.9csxet.cn

[Q25] 只取前 N 条
来源：http://dr.9csxet.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://lr.9csxet.cn

[Q26] 计数
来源：http://jr.shxzukj.cn

SELECT COUNT(*) FROM users;
来源：http://fj.jctech888.com.cn

[Q27] 条件计数
来源：http://rm.yuntaijiaju.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://dk.huixinmuqiang.cn

[Q28] 求和与平均
来源：http://la.shxzukj.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://qp.521024.cn

[Q29] 最大最小值
来源：http://pr.jctech888.com.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://tx.haigaiapp.cn

[Q30] 分组统计
来源：http://he.asd995.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ot.nszjky.cn

[Q31] 分组后过滤
来源：http://ly.colortex.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://pq.bookmarksfly.cn

[Q32] 分组拼接字符串
来源：http://uv.521024.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://kg.bookmarksfly.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://tl.huanxung.cn

[Q33] 多列分组
来源：http://xm.panjiajie.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wo.jianghongdianzi.cn

[Q34] 每组取第一条
来源：http://wb.newstarts.cn

SELECT * FROM (
来源：http://gw.shxzskj.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://xi.huixiangedu.cn

) t WHERE rn = 1;
来源：http://ad.521024.cn

[Q35] 内连接
来源：http://ww.szxytkj.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://gb.hahajie.cn

[Q36] 左连接
来源：http://fw.521024.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://eq.nszjky.cn

[Q37] 右连接
来源：http://rq.shxzukj.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ae.nszjky.cn

[Q38] 全外连接（PostgreSQL）
来源：http://mt.9csxet.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://lv.nicolike.cn

[Q39] 自连接（查上下级）
来源：http://uk.chemitech.net.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://eo.huanxung.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wu.wgjwhj.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://nx.szxytkj.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://cy.nicolike.cn

[Q41] 多表连接
来源：http://pw.jianghongdianzi.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://nm.nicolike.cn

JOIN users u ON u.id = o.user_id
来源：http://gh.bookmarksfly.cn

JOIN products p ON p.id = o.product_id;
来源：http://gr.yuexingan06.cn

[Q42] 连接条件附加过滤
来源：http://ti.wgjwhj.cn

SELECT u.name, o.amount FROM users u
来源：http://bz.shtwfgs.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ll.newstarts.cn

[Q43] 标量子查询
来源：http://dv.hahajie.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://oy.muxihuayi.cn

[Q44] IN 子查询
来源：http://qq.hnjuh.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://fs.nszjky.cn

[Q45] EXISTS 判断存在
来源：http://uk.nszjky.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ya.panjiajie.cn

[Q46] NOT EXISTS 判断不存在
来源：http://rm.nszjky.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://xa.huixiangedu.cn

[Q47] 与平均值比较
来源：http://ci.shxzukj.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://rh.muxihuayi.cn

[Q48] CTE 公用表表达式
来源：http://ve.szsharing.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://aa.huixinmuqiang.cn

SELECT * FROM t WHERE c > 5;
来源：http://aj.nszjky.cn

[Q49] 更新单行
来源：http://el.wgjwhj.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://cv.panjiajie.cn

[Q50] 批量更新
来源：http://vi.jctech888.com.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://vl.yuntaijiaju.cn

[Q51] 用子查询更新
来源：http://vy.nicolike.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hb.nicolike.cn

[Q52] 删除指定行
来源：http://fx.huanxung.cn

DELETE FROM users WHERE id = 10;
来源：http://uz.wgjwhj.cn

[Q53] 按条件删除
来源：http://tw.hnjuh.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://uz.newstarts.cn

[Q54] 清空表
来源：http://ki.nszjky.cn

TRUNCATE TABLE logs;
来源：http://ce.colortex.cn

[Q55] 排名（并列占位）
来源：http://of.gzmigu.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://sx.panjiajie.cn

[Q56] 密集排名（并列不占位）
来源：http://xs.hahajie.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://zh.jianghongdianzi.cn

[Q57] 行号
来源：http://kj.521024.cn


<!-- 参考信息 -->