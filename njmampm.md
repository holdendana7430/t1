代发 wailian999

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://et.9csxet.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://xh.wgjwhj.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://iq.newstarts.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://rt.9csxet.cn

[N05] 最大公约数
来源：http://uz.jctech888.com.cn

Py:   math.gcd(a, b)
来源：http://sk.shtwfgs.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://pq.asd995.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://jv.newstarts.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://sd.panjiajie.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ly.szxytkj.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://yl.gzmigu.cn

Ruby: a.gcd(b)
来源：http://ga.9csxet.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://eb.haigaiapp.cn

[N06] 判断回文字符串
来源：http://sy.szxytkj.cn

Py:   s == s[::-1]
来源：http://vj.gzmigu.cn

PHP:  $s === strrev($s);
来源：http://ht.nicolike.cn

JS:   s === [...s].reverse().join("")
来源：http://bg.newstarts.cn

TS:   s === [...s].reverse().join("")
来源：http://ap.shxzskj.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://az.panjiajie.cn

Go:   // 双指针从两端比较
来源：http://gd.colortex.cn

Ruby: s == s.reverse
来源：http://la.bookmarksfly.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://ds.lnxyls.cn

[N07] 两数之和（返回下标）
来源：http://qx.panjiajie.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://oa.9csxet.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://nt.hahajie.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://ua.hnjuh.cn

TS:   // 手写 Map<string, number>
来源：http://gp.nszjky.cn

Java: // 手写 HashMap
来源：http://re.haigaiapp.cn

Go:   // 手写 map[int]int
来源：http://jo.jctech888.com.cn

Ruby: // 手写 Hash
来源：http://yu.asd995.cn

C#:   // 手写 Dictionary<int, int>
来源：http://lx.haigaiapp.cn

[N08] 生成全排列
来源：http://zk.nszjky.cn

Py:   itertools.permutations(arr)
来源：http://ns.nszjky.cn

PHP:  // 手写递归交换
来源：http://ow.521024.cn

JS:   // 手写回溯递归
来源：http://pk.huixiangedu.cn

TS:   // 手写回溯递归
来源：http://ip.newstarts.cn

Java: // 手写回溯递归
来源：http://qi.haigaiapp.cn

Go:   // 手写回溯递归
来源：http://lt.huixiangedu.cn

Ruby: arr.permutation.to_a
来源：http://ni.lnxyls.cn

C#:   // 手写回溯递归
来源：http://rf.huixinmuqiang.cn

[N09] 栈与队列
来源：http://nh.shxzukj.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://fu.hnjuh.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ph.huixiangedu.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://gl.newstarts.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://vi.muxihuayi.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://fw.nszjky.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ir.huixinmuqiang.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hk.bookmarksfly.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://fo.panjiajie.cn

[N10] 链表节点定义
来源：http://db.hahajie.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wl.newstarts.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://sn.bookmarksfly.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://pq.lnxyls.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://jf.jctech888.com.cn

Java: class Node { int v; Node next; }
来源：http://no.9csxet.cn

Go:   type Node struct { V int; Next *Node }
来源：http://iy.wgjwhj.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://cs.muxihuayi.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://gq.9csxet.cn

[N11] 二叉树中序遍历
来源：http://nj.panjiajie.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://vk.szxytkj.cn

PHP:  // 手写递归函数
来源：http://hw.asd995.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://it.wgjwhj.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://pr.haigaiapp.cn

Java: // 手写递归
来源：http://ks.huixinmuqiang.cn

Go:   // 手写递归
来源：http://sb.nicolike.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wq.chemitech.net.cn

C#:   // 手写递归
来源：http://ks.newstarts.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://nh.hnjuh.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://of.nicolike.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://vq.hnjuh.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://gs.yuexingan06.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://fr.bjjhwx.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://qk.521024.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://lz.wgjwhj.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ms.haigaiapp.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://qy.hnjuh.cn

================================================================================
来源：http://hh.newstarts.cn

O. 并发与异步
来源：http://ju.9csxet.cn

================================================================================
来源：http://ka.szxytkj.cn

[O01] 启动一个线程
来源：http://sg.shxzukj.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://fb.yuntaijiaju.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://gv.muxihuayi.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://rw.panjiajie.cn

TS:   // 同 JS
来源：http://ys.szsharing.cn

Java: new Thread(() -> f()).start()
来源：http://xd.bjjhwx.cn

Go:   go f()
来源：http://qw.jianghongdianzi.cn

Ruby: Thread.new { f }
来源：http://mf.gzmigu.cn

C#:   Task.Run(() => F());
来源：http://cx.gzmigu.cn

[O02] 使用线程池
来源：http://rb.hahajie.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://qy.colortex.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ti.asd995.cn

JS:   // worker_threads 线程池
来源：http://nm.nszjky.cn

TS:   // worker_threads 线程池
来源：http://tz.wgjwhj.cn

Java: Executors.newFixedThreadPool(4)
来源：http://nh.asd995.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ei.shtwfgs.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://nj.shxzukj.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://sf.jianghongdianzi.cn

[O03] 加锁保护共享数据
来源：http://ic.muxihuayi.cn

Py:   with lock: shared += 1
来源：http://yk.huixinmuqiang.cn

PHP:  // 用 flock() 做文件锁
来源：http://yc.lnxyls.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mz.huanxung.cn

TS:   // 同 JS
来源：http://je.nszjky.cn

Java: synchronized (this) { shared++; }
来源：http://mr.hahajie.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://qv.nszjky.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://br.jctech888.com.cn

C#:   lock (gate) { shared++; }
来源：http://yb.nicolike.cn

[O04] 定义异步函数并等待
来源：http://sx.huixiangedu.cn

Py:   async def f():⏎    await g()
来源：http://ru.huixinmuqiang.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://pw.wgjwhj.cn

JS:   async function f() { await g(); }
来源：http://ma.huixiangedu.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://lu.jctech888.com.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://lg.panjiajie.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://cf.shxzukj.cn

Ruby: # 用 Fiber 或 async gem
来源：http://gb.huanxung.cn

C#:   async Task F() { await G(); }
来源：http://sv.chemitech.net.cn

[O05] 并发执行并等待全部完成
来源：http://ma.chemitech.net.cn

Py:   asyncio.gather(*tasks)
来源：http://ek.yuexingan06.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://fb.shxzskj.cn

JS:   await Promise.all(tasks)
来源：http://ht.szsharing.cn

TS:   await Promise.all(tasks)
来源：http://bd.shtwfgs.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://bu.nicolike.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://vl.huixinmuqiang.cn

Ruby: threads.map(&:join)
来源：http://af.bookmarksfly.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://po.newstarts.cn

[O06] 使用进程池
来源：http://fb.chemitech.net.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://fh.szsharing.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://lx.huixinmuqiang.cn

JS:   // child_process / cluster 模块
来源：http://br.yuntaijiaju.cn

TS:   // child_process / cluster 模块
来源：http://dd.szxytkj.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://jh.hahajie.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ml.szxytkj.cn

Ruby: // fork 块
来源：http://di.shxzskj.cn

C#:   Parallel.For
来源：http://ls.bookmarksfly.cn

================================================================================
来源：http://kn.yuexingan06.cn

P. 常用工具函数
来源：http://mw.newstarts.cn

================================================================================
来源：http://du.huixiangedu.cn

[P01] 生成 UUID
来源：http://ur.521024.cn

Py:   str(uuid.uuid4())
来源：http://as.newstarts.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://xv.huanxung.cn

JS:   crypto.randomUUID()
来源：http://vz.yuexingan06.cn

TS:   crypto.randomUUID()
来源：http://bp.wgjwhj.cn

Java: UUID.randomUUID().toString()
来源：http://lx.newstarts.cn

Go:   // 用 github.com/google/uuid
来源：http://ve.521024.cn

Ruby: SecureRandom.uuid
来源：http://zg.szsharing.cn

C#:   Guid.NewGuid().ToString()
来源：http://se.521024.cn

[P02] MD5 / SHA256 摘要
来源：http://li.jianghongdianzi.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://sv.muxihuayi.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://fo.hnjuh.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://pi.colortex.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://as.newstarts.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://qp.szxytkj.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://gh.gzmigu.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://it.yuexingan06.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://tt.shxzukj.cn

[P03] 生成短随机字符串
来源：http://cj.lnxyls.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://rw.szsharing.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://qw.huixiangedu.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://dz.huixiangedu.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://je.colortex.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://cr.nszjky.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://sx.gzmigu.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://ov.jctech888.com.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ga.bjjhwx.cn

[P04] 求长度
来源：http://sw.gzmigu.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wu.jctech888.com.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ys.hahajie.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://tl.jianghongdianzi.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wc.asd995.cn

Java: list.size();  map.size();  s.length()
来源：http://zo.chemitech.net.cn

Go:   len(arr);  len(m)
来源：http://tf.shxzskj.cn

Ruby: x.length;  x.size
来源：http://kn.szsharing.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://bl.nszjky.cn

[P05] 判断两个对象内容是否相等
来源：http://xd.yuntaijiaju.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://go.shxzukj.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://jk.lnxyls.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://yc.huanxung.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://df.shtwfgs.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://lq.haigaiapp.cn

Go:   reflect.DeepEqual(a, b)
来源：http://wn.chemitech.net.cn

Ruby: a == b
来源：http://wj.jianghongdianzi.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://sv.jctech888.com.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://dn.huixiangedu.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://sb.szxytkj.cn

PHP:  if (empty($x)) {}
来源：http://ke.bookmarksfly.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ln.szsharing.cn

TS:   if (x == null) {}
来源：http://wv.huanxung.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://wv.yuexingan06.cn

Go:   if x == nil {}
来源：http://dt.521024.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://po.chemitech.net.cn

C#:   if (x is null) {}
来源：http://jq.huixinmuqiang.cn

[P07] 防抖与节流
来源：http://gj.jianghongdianzi.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://zx.nszjky.cn

PHP:  // 手写时间戳比较
来源：http://mk.jianghongdianzi.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://gg.panjiajie.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://jl.bookmarksfly.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://rj.muxihuayi.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://gr.gzmigu.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://jm.chemitech.net.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://dh.colortex.cn

[P08] 处理浮点精度问题
来源：http://lp.lnxyls.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://dh.9csxet.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://sz.yuntaijiaju.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ev.jianghongdianzi.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://qp.haigaiapp.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://lp.bookmarksfly.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ab.bookmarksfly.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ty.lnxyls.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://bg.bjjhwx.cn

================================================================================
来源：http://bj.yuexingan06.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hw.shxzukj.cn

================================================================================
来源：http://xb.panjiajie.cn

[Q01] 创建表
来源：http://wc.yuntaijiaju.cn

CREATE TABLE users (
来源：http://gj.huixiangedu.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://gw.haigaiapp.cn

name VARCHAR(50) NOT NULL,
来源：http://yz.huixiangedu.cn

email VARCHAR(100) UNIQUE,
来源：http://ny.huixiangedu.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://gl.9csxet.cn

);
来源：http://vs.bookmarksfly.cn

[Q02] 创建带外键的表
来源：http://dg.bookmarksfly.cn

CREATE TABLE orders (
来源：http://sa.shxzskj.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://tq.yuexingan06.cn

user_id INT NOT NULL,
来源：http://dl.huixiangedu.cn

amount DECIMAL(10, 2),
来源：http://dh.jianghongdianzi.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://um.521024.cn

);
来源：http://gg.yuexingan06.cn

[Q03] 增加列
来源：http://cl.nicolike.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hi.shxzukj.cn

[Q04] 修改列类型
来源：http://av.jianghongdianzi.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://eg.szxytkj.cn

[Q05] 重命名列
来源：http://ix.hnjuh.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://fp.lnxyls.cn

[Q06] 删除列
来源：http://am.yuntaijiaju.cn

ALTER TABLE users DROP COLUMN age;
来源：http://vf.wgjwhj.cn

[Q07] 删除表
来源：http://ay.nszjky.cn

DROP TABLE IF EXISTS orders;
来源：http://sk.newstarts.cn

[Q08] 创建普通索引
来源：http://hz.szxytkj.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://er.huixiangedu.cn

[Q09] 创建唯一索引
来源：http://hg.muxihuayi.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://em.newstarts.cn

[Q10] 插入单行
来源：http://og.jianghongdianzi.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://at.jctech888.com.cn

[Q11] 一次插入多行
来源：http://ui.colortex.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://yb.huanxung.cn

[Q12] 插入后取自增 ID
来源：http://yf.shtwfgs.cn

INSERT INTO users (name) VALUES ('C');
来源：http://gu.panjiajie.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://lx.shxzskj.cn

[Q13] 忽略重复插入
来源：http://ol.hahajie.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://jo.jianghongdianzi.cn

[Q14] 存在则更新（upsert）
来源：http://nm.huixinmuqiang.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://yn.haigaiapp.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://vo.nicolike.cn

[Q15] 查询全部
来源：http://kd.yuntaijiaju.cn

SELECT * FROM users;
来源：http://ay.shxzskj.cn

[Q16] 查询指定列
来源：http://hc.nszjky.cn

SELECT id, name FROM users;
来源：http://rb.yuntaijiaju.cn

[Q17] 条件查询
来源：http://ey.bookmarksfly.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ip.nszjky.cn

[Q18] 模糊匹配
来源：http://yz.9csxet.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://zu.shxzukj.cn

[Q19] 范围查询
来源：http://zu.huixinmuqiang.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ok.shxzukj.cn

[Q20] IN 列表
来源：http://pr.yuexingan06.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://vz.huixiangedu.cn

[Q21] 空值判断
来源：http://lt.huixiangedu.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://wc.521024.cn

[Q22] 排序
来源：http://ku.muxihuayi.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://of.wgjwhj.cn

[Q23] 分页
来源：http://ga.shxzukj.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://oh.bookmarksfly.cn

[Q24] 去重
来源：http://xo.lnxyls.cn

SELECT DISTINCT city FROM users;
来源：http://vj.huixiangedu.cn

[Q25] 只取前 N 条
来源：http://zk.9csxet.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://qu.shxzukj.cn

[Q26] 计数
来源：http://hg.shtwfgs.cn

SELECT COUNT(*) FROM users;
来源：http://lh.szxytkj.cn

[Q27] 条件计数
来源：http://vi.huixiangedu.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://iu.yuexingan06.cn

[Q28] 求和与平均
来源：http://nl.colortex.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://ti.bjjhwx.cn

[Q29] 最大最小值
来源：http://oi.huixiangedu.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://ne.asd995.cn

[Q30] 分组统计
来源：http://xo.hahajie.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mk.yuntaijiaju.cn

[Q31] 分组后过滤
来源：http://zc.hnjuh.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://bb.muxihuayi.cn

[Q32] 分组拼接字符串
来源：http://en.hnjuh.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://li.shxzukj.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://fu.huixiangedu.cn

[Q33] 多列分组
来源：http://uz.shxzukj.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://jr.521024.cn

[Q34] 每组取第一条
来源：http://li.yuntaijiaju.cn

SELECT * FROM (
来源：http://bh.huixiangedu.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ao.colortex.cn

) t WHERE rn = 1;
来源：http://xr.jianghongdianzi.cn

[Q35] 内连接
来源：http://yh.huanxung.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hc.521024.cn

[Q36] 左连接
来源：http://xr.panjiajie.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://nw.521024.cn

[Q37] 右连接
来源：http://zm.nszjky.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://jd.huanxung.cn


<!-- 参考信息 -->