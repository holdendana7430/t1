代发 wailian999

Go:   // 手写 map[int]int
来源：http://zh.yuexingan06.cn

Ruby: // 手写 Hash
来源：http://be.haigaiapp.cn

C#:   // 手写 Dictionary<int, int>
来源：http://ic.asd995.cn

[N08] 生成全排列
来源：http://pn.yuntaijiaju.cn

Py:   itertools.permutations(arr)
来源：http://rp.haigaiapp.cn

PHP:  // 手写递归交换
来源：http://rb.szsharing.cn

JS:   // 手写回溯递归
来源：http://ab.nicolike.cn

TS:   // 手写回溯递归
来源：http://ho.yuntaijiaju.cn

Java: // 手写回溯递归
来源：http://es.haigaiapp.cn

Go:   // 手写回溯递归
来源：http://xg.muxihuayi.cn

Ruby: arr.permutation.to_a
来源：http://ra.9csxet.cn

C#:   // 手写回溯递归
来源：http://mm.wgjwhj.cn

[N09] 栈与队列
来源：http://yy.yuntaijiaju.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://xj.jctech888.com.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ou.gzmigu.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://yj.yuntaijiaju.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wv.521024.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://vc.huixinmuqiang.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://bu.yuntaijiaju.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://vu.shxzukj.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ob.panjiajie.cn

[N10] 链表节点定义
来源：http://nc.hnjuh.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://pz.colortex.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://zl.shxzskj.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://zx.asd995.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ew.shxzukj.cn

Java: class Node { int v; Node next; }
来源：http://zn.wgjwhj.cn

Go:   type Node struct { V int; Next *Node }
来源：http://yo.huixinmuqiang.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://zx.lnxyls.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://cq.asd995.cn

[N11] 二叉树中序遍历
来源：http://jg.9csxet.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://gs.asd995.cn

PHP:  // 手写递归函数
来源：http://zq.huixiangedu.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://og.huanxung.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://nv.yuntaijiaju.cn

Java: // 手写递归
来源：http://zx.huixiangedu.cn

Go:   // 手写递归
来源：http://rd.shtwfgs.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://jg.muxihuayi.cn

C#:   // 手写递归
来源：http://am.yuntaijiaju.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ec.nicolike.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://nt.panjiajie.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://vk.hahajie.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ud.nicolike.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://nv.bookmarksfly.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://kz.huixiangedu.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://qp.nicolike.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://bj.jctech888.com.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://kg.panjiajie.cn

================================================================================
来源：http://kz.huanxung.cn

O. 并发与异步
来源：http://tu.shxzukj.cn

================================================================================
来源：http://zt.chemitech.net.cn

[O01] 启动一个线程
来源：http://rf.colortex.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://bo.bookmarksfly.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ih.shxzukj.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ye.wgjwhj.cn

TS:   // 同 JS
来源：http://id.huixiangedu.cn

Java: new Thread(() -> f()).start()
来源：http://nh.bookmarksfly.cn

Go:   go f()
来源：http://qd.lnxyls.cn

Ruby: Thread.new { f }
来源：http://js.wgjwhj.cn

C#:   Task.Run(() => F());
来源：http://rg.shxzskj.cn

[O02] 使用线程池
来源：http://rw.jianghongdianzi.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://nf.jctech888.com.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://it.newstarts.cn

JS:   // worker_threads 线程池
来源：http://oy.521024.cn

TS:   // worker_threads 线程池
来源：http://ig.521024.cn

Java: Executors.newFixedThreadPool(4)
来源：http://tw.szsharing.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://sb.jianghongdianzi.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://pw.huixiangedu.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ud.hahajie.cn

[O03] 加锁保护共享数据
来源：http://pa.chemitech.net.cn

Py:   with lock: shared += 1
来源：http://op.shxzukj.cn

PHP:  // 用 flock() 做文件锁
来源：http://ym.jianghongdianzi.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ix.gzmigu.cn

TS:   // 同 JS
来源：http://ue.huixiangedu.cn

Java: synchronized (this) { shared++; }
来源：http://mw.asd995.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ch.huixiangedu.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://wu.huixiangedu.cn

C#:   lock (gate) { shared++; }
来源：http://kq.bjjhwx.cn

[O04] 定义异步函数并等待
来源：http://qf.jctech888.com.cn

Py:   async def f():⏎    await g()
来源：http://yv.huanxung.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://el.muxihuayi.cn

JS:   async function f() { await g(); }
来源：http://zq.muxihuayi.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://rl.nszjky.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://sk.huanxung.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://kz.lnxyls.cn

Ruby: # 用 Fiber 或 async gem
来源：http://sa.newstarts.cn

C#:   async Task F() { await G(); }
来源：http://pn.shxzukj.cn

[O05] 并发执行并等待全部完成
来源：http://rq.nicolike.cn

Py:   asyncio.gather(*tasks)
来源：http://mq.shxzukj.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://lj.szxytkj.cn

JS:   await Promise.all(tasks)
来源：http://jn.haigaiapp.cn

TS:   await Promise.all(tasks)
来源：http://ai.hnjuh.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://xl.9csxet.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://bc.bjjhwx.cn

Ruby: threads.map(&:join)
来源：http://zk.9csxet.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://cx.bjjhwx.cn

[O06] 使用进程池
来源：http://gi.huixiangedu.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mp.panjiajie.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://ye.muxihuayi.cn

JS:   // child_process / cluster 模块
来源：http://ln.9csxet.cn

TS:   // child_process / cluster 模块
来源：http://wf.colortex.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://xs.szxytkj.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://kl.chemitech.net.cn

Ruby: // fork 块
来源：http://lg.hahajie.cn

C#:   Parallel.For
来源：http://ud.gzmigu.cn

================================================================================
来源：http://us.521024.cn

P. 常用工具函数
来源：http://tk.szsharing.cn

================================================================================
来源：http://hj.huixiangedu.cn

[P01] 生成 UUID
来源：http://sc.bjjhwx.cn

Py:   str(uuid.uuid4())
来源：http://hg.yuntaijiaju.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://xd.yuntaijiaju.cn

JS:   crypto.randomUUID()
来源：http://ko.huixiangedu.cn

TS:   crypto.randomUUID()
来源：http://tk.huixiangedu.cn

Java: UUID.randomUUID().toString()
来源：http://jh.szsharing.cn

Go:   // 用 github.com/google/uuid
来源：http://kq.szxytkj.cn

Ruby: SecureRandom.uuid
来源：http://nv.521024.cn

C#:   Guid.NewGuid().ToString()
来源：http://rf.9csxet.cn

[P02] MD5 / SHA256 摘要
来源：http://ik.521024.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://cy.haigaiapp.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://gw.asd995.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ji.nszjky.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://rm.muxihuayi.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://lm.hahajie.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://pb.newstarts.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hx.hahajie.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://va.yuexingan06.cn

[P03] 生成短随机字符串
来源：http://pz.huixiangedu.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://qh.yuntaijiaju.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://pu.haigaiapp.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wl.yuntaijiaju.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://tn.gzmigu.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://uw.gzmigu.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://oq.huixinmuqiang.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://rp.521024.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://bh.yuntaijiaju.cn

[P04] 求长度
来源：http://fh.wgjwhj.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://xj.nicolike.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://az.wgjwhj.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://bj.haigaiapp.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://zi.nszjky.cn

Java: list.size();  map.size();  s.length()
来源：http://il.jctech888.com.cn

Go:   len(arr);  len(m)
来源：http://du.hahajie.cn

Ruby: x.length;  x.size
来源：http://pg.shxzskj.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://xg.gzmigu.cn

[P05] 判断两个对象内容是否相等
来源：http://ti.nszjky.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://if.9csxet.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://fx.bjjhwx.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://fg.colortex.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://dp.jctech888.com.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://yi.jianghongdianzi.cn

Go:   reflect.DeepEqual(a, b)
来源：http://ce.huixiangedu.cn

Ruby: a == b
来源：http://zf.nicolike.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://de.bjjhwx.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://yw.lnxyls.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://lo.shxzukj.cn

PHP:  if (empty($x)) {}
来源：http://jy.bjjhwx.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ea.szxytkj.cn

TS:   if (x == null) {}
来源：http://mw.newstarts.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://sx.chemitech.net.cn

Go:   if x == nil {}
来源：http://rq.lnxyls.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ds.huixiangedu.cn

C#:   if (x is null) {}
来源：http://sg.szxytkj.cn

[P07] 防抖与节流
来源：http://jk.hnjuh.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ad.nicolike.cn

PHP:  // 手写时间戳比较
来源：http://wh.muxihuayi.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ci.hahajie.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mk.wgjwhj.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://xq.huixinmuqiang.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://jk.gzmigu.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://mb.jctech888.com.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ej.lnxyls.cn

[P08] 处理浮点精度问题
来源：http://vd.chemitech.net.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://vt.huanxung.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ua.bjjhwx.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://df.yuntaijiaju.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ti.muxihuayi.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://op.gzmigu.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://nh.hnjuh.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wz.wgjwhj.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://xy.huixinmuqiang.cn

================================================================================
来源：http://ht.521024.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://qc.yuexingan06.cn

================================================================================
来源：http://lz.panjiajie.cn

[Q01] 创建表
来源：http://io.nicolike.cn

CREATE TABLE users (
来源：http://zo.lnxyls.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://vq.haigaiapp.cn

name VARCHAR(50) NOT NULL,
来源：http://eo.wgjwhj.cn

email VARCHAR(100) UNIQUE,
来源：http://ad.panjiajie.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ve.jianghongdianzi.cn

);
来源：http://es.yuexingan06.cn

[Q02] 创建带外键的表
来源：http://mm.nszjky.cn

CREATE TABLE orders (
来源：http://cr.chemitech.net.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://tn.shxzukj.cn

user_id INT NOT NULL,
来源：http://tl.shxzskj.cn

amount DECIMAL(10, 2),
来源：http://gz.huixiangedu.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://sg.yuntaijiaju.cn

);
来源：http://cf.huanxung.cn

[Q03] 增加列
来源：http://sd.wgjwhj.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://si.yuexingan06.cn

[Q04] 修改列类型
来源：http://ia.shxzukj.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://zn.9csxet.cn

[Q05] 重命名列
来源：http://nm.colortex.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://tu.yuntaijiaju.cn

[Q06] 删除列
来源：http://ty.lnxyls.cn

ALTER TABLE users DROP COLUMN age;
来源：http://su.szsharing.cn

[Q07] 删除表
来源：http://yw.nicolike.cn

DROP TABLE IF EXISTS orders;
来源：http://fr.muxihuayi.cn

[Q08] 创建普通索引
来源：http://jf.huixinmuqiang.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://wr.szxytkj.cn

[Q09] 创建唯一索引
来源：http://xo.bjjhwx.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ty.haigaiapp.cn

[Q10] 插入单行
来源：http://vy.bookmarksfly.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://eu.bookmarksfly.cn

[Q11] 一次插入多行
来源：http://xe.nicolike.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://fb.huanxung.cn

[Q12] 插入后取自增 ID
来源：http://ji.yuntaijiaju.cn

INSERT INTO users (name) VALUES ('C');
来源：http://xc.szsharing.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://xr.shtwfgs.cn

[Q13] 忽略重复插入
来源：http://ot.panjiajie.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hr.bookmarksfly.cn

[Q14] 存在则更新（upsert）
来源：http://wz.gzmigu.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://no.yuexingan06.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://bh.chemitech.net.cn

[Q15] 查询全部
来源：http://vb.chemitech.net.cn

SELECT * FROM users;
来源：http://wa.haigaiapp.cn

[Q16] 查询指定列
来源：http://tv.jctech888.com.cn

SELECT id, name FROM users;
来源：http://zb.panjiajie.cn

[Q17] 条件查询
来源：http://ub.gzmigu.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://qy.haigaiapp.cn

[Q18] 模糊匹配
来源：http://lg.9csxet.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://zw.szsharing.cn

[Q19] 范围查询
来源：http://sd.yuexingan06.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://zb.muxihuayi.cn

[Q20] IN 列表
来源：http://lr.gzmigu.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ke.bjjhwx.cn

[Q21] 空值判断
来源：http://hw.jctech888.com.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://nh.hahajie.cn

[Q22] 排序
来源：http://wy.bookmarksfly.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ff.hahajie.cn

[Q23] 分页
来源：http://xu.nicolike.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://fz.asd995.cn

[Q24] 去重
来源：http://ev.szsharing.cn

SELECT DISTINCT city FROM users;
来源：http://sx.jctech888.com.cn

[Q25] 只取前 N 条
来源：http://gh.panjiajie.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://vu.szsharing.cn

[Q26] 计数
来源：http://ga.asd995.cn

SELECT COUNT(*) FROM users;
来源：http://rh.shxzukj.cn

[Q27] 条件计数
来源：http://qs.hnjuh.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://dz.jctech888.com.cn

[Q28] 求和与平均
来源：http://wv.bjjhwx.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://sg.wgjwhj.cn

[Q29] 最大最小值
来源：http://gj.newstarts.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://lg.lnxyls.cn

[Q30] 分组统计
来源：http://wi.lnxyls.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://cc.521024.cn

[Q31] 分组后过滤
来源：http://hm.shtwfgs.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://iq.jianghongdianzi.cn

[Q32] 分组拼接字符串
来源：http://xa.newstarts.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://gb.huixinmuqiang.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://pi.hahajie.cn

[Q33] 多列分组
来源：http://hi.huixinmuqiang.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://yb.bjjhwx.cn

[Q34] 每组取第一条
来源：http://rj.yuntaijiaju.cn

SELECT * FROM (
来源：http://ns.shtwfgs.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ou.shxzskj.cn

) t WHERE rn = 1;
来源：http://ld.panjiajie.cn

[Q35] 内连接
来源：http://wr.shtwfgs.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mh.muxihuayi.cn

[Q36] 左连接
来源：http://wg.bjjhwx.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://vk.lnxyls.cn

[Q37] 右连接
来源：http://jg.chemitech.net.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://rn.yuntaijiaju.cn

[Q38] 全外连接（PostgreSQL）
来源：http://bj.yuntaijiaju.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hy.lnxyls.cn

[Q39] 自连接（查上下级）
来源：http://zt.asd995.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://hn.szxytkj.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://bt.yuntaijiaju.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://hi.jctech888.com.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://lg.yuntaijiaju.cn

[Q41] 多表连接
来源：http://eq.huixiangedu.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://er.colortex.cn

JOIN users u ON u.id = o.user_id
来源：http://jb.nicolike.cn

JOIN products p ON p.id = o.product_id;
来源：http://ge.wgjwhj.cn

[Q42] 连接条件附加过滤
来源：http://mq.huixiangedu.cn

SELECT u.name, o.amount FROM users u
来源：http://yc.9csxet.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://it.hnjuh.cn

[Q43] 标量子查询
来源：http://vs.asd995.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wv.lnxyls.cn

[Q44] IN 子查询
来源：http://gy.huixiangedu.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ac.muxihuayi.cn

[Q45] EXISTS 判断存在
来源：http://wu.wgjwhj.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://gu.colortex.cn

[Q46] NOT EXISTS 判断不存在
来源：http://vc.shtwfgs.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://lh.shxzskj.cn

[Q47] 与平均值比较
来源：http://cz.asd995.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hb.lnxyls.cn

[Q48] CTE 公用表表达式
来源：http://eu.szxytkj.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ry.shtwfgs.cn

SELECT * FROM t WHERE c > 5;
来源：http://bq.bookmarksfly.cn

[Q49] 更新单行
来源：http://bs.521024.cn


<!-- 参考信息 -->