代发 wailian999

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://rk.jianghongdianzi.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ad.jianghongdianzi.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ps.huixiangedu.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://vr.szsharing.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ik.lnxyls.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://nj.huixinmuqiang.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://kx.shtwfgs.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ko.gzmigu.cn

[N05] 最大公约数
来源：http://ns.bookmarksfly.cn

Py:   math.gcd(a, b)
来源：http://ls.asd995.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://zt.nszjky.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ve.9csxet.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://fz.nicolike.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://va.asd995.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ud.huixiangedu.cn

Ruby: a.gcd(b)
来源：http://we.bookmarksfly.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://fm.asd995.cn

[N06] 判断回文字符串
来源：http://pu.colortex.cn

Py:   s == s[::-1]
来源：http://pb.huixiangedu.cn

PHP:  $s === strrev($s);
来源：http://ro.nszjky.cn

JS:   s === [...s].reverse().join("")
来源：http://li.muxihuayi.cn

TS:   s === [...s].reverse().join("")
来源：http://pz.szxytkj.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://zw.chemitech.net.cn

Go:   // 双指针从两端比较
来源：http://gd.szxytkj.cn

Ruby: s == s.reverse
来源：http://md.yuexingan06.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://zs.shxzukj.cn

[N07] 两数之和（返回下标）
来源：http://nd.521024.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://oe.chemitech.net.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ui.chemitech.net.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://ka.9csxet.cn

TS:   // 手写 Map<string, number>
来源：http://mv.bjjhwx.cn

Java: // 手写 HashMap
来源：http://ir.szsharing.cn

Go:   // 手写 map[int]int
来源：http://cv.wgjwhj.cn

Ruby: // 手写 Hash
来源：http://nz.jianghongdianzi.cn

C#:   // 手写 Dictionary<int, int>
来源：http://uh.colortex.cn

[N08] 生成全排列
来源：http://bz.shxzukj.cn

Py:   itertools.permutations(arr)
来源：http://fj.haigaiapp.cn

PHP:  // 手写递归交换
来源：http://ay.shxzskj.cn

JS:   // 手写回溯递归
来源：http://vt.shtwfgs.cn

TS:   // 手写回溯递归
来源：http://ch.hahajie.cn

Java: // 手写回溯递归
来源：http://kx.bookmarksfly.cn

Go:   // 手写回溯递归
来源：http://iv.wgjwhj.cn

Ruby: arr.permutation.to_a
来源：http://qj.nszjky.cn

C#:   // 手写回溯递归
来源：http://zp.nicolike.cn

[N09] 栈与队列
来源：http://eh.lnxyls.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://cc.shxzskj.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://io.lnxyls.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://zn.chemitech.net.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://no.wgjwhj.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ll.yuntaijiaju.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://bh.9csxet.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://je.panjiajie.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://cv.jctech888.com.cn

[N10] 链表节点定义
来源：http://on.colortex.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://pk.huixinmuqiang.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://im.huixinmuqiang.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hv.bjjhwx.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ss.chemitech.net.cn

Java: class Node { int v; Node next; }
来源：http://qm.hahajie.cn

Go:   type Node struct { V int; Next *Node }
来源：http://ce.huanxung.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://ff.haigaiapp.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://ce.shxzukj.cn

[N11] 二叉树中序遍历
来源：http://ih.gzmigu.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://fg.shxzskj.cn

PHP:  // 手写递归函数
来源：http://cd.nszjky.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ch.hahajie.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hy.lnxyls.cn

Java: // 手写递归
来源：http://zx.9csxet.cn

Go:   // 手写递归
来源：http://px.huixiangedu.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://pw.9csxet.cn

C#:   // 手写递归
来源：http://ji.shtwfgs.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wr.huixinmuqiang.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://up.nicolike.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://in.asd995.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ar.lnxyls.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://jx.asd995.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://xe.szsharing.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://am.jctech888.com.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://gd.bookmarksfly.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wd.hahajie.cn

================================================================================
来源：http://gi.colortex.cn

O. 并发与异步
来源：http://ql.colortex.cn

================================================================================
来源：http://ba.muxihuayi.cn

[O01] 启动一个线程
来源：http://pz.bookmarksfly.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://tf.wgjwhj.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://yy.521024.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://nm.huixiangedu.cn

TS:   // 同 JS
来源：http://mi.wgjwhj.cn

Java: new Thread(() -> f()).start()
来源：http://zg.hahajie.cn

Go:   go f()
来源：http://lk.szsharing.cn

Ruby: Thread.new { f }
来源：http://wu.szxytkj.cn

C#:   Task.Run(() => F());
来源：http://aq.huanxung.cn

[O02] 使用线程池
来源：http://qf.muxihuayi.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://rv.haigaiapp.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ps.hahajie.cn

JS:   // worker_threads 线程池
来源：http://an.huixinmuqiang.cn

TS:   // worker_threads 线程池
来源：http://wj.panjiajie.cn

Java: Executors.newFixedThreadPool(4)
来源：http://mt.chemitech.net.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://rc.bjjhwx.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://st.huixiangedu.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://dr.panjiajie.cn

[O03] 加锁保护共享数据
来源：http://cs.shtwfgs.cn

Py:   with lock: shared += 1
来源：http://st.wgjwhj.cn

PHP:  // 用 flock() 做文件锁
来源：http://rl.huanxung.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://jw.bjjhwx.cn

TS:   // 同 JS
来源：http://tx.9csxet.cn

Java: synchronized (this) { shared++; }
来源：http://yn.9csxet.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://gf.newstarts.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://pz.wgjwhj.cn

C#:   lock (gate) { shared++; }
来源：http://tz.lnxyls.cn

[O04] 定义异步函数并等待
来源：http://vw.haigaiapp.cn

Py:   async def f():⏎    await g()
来源：http://tt.szxytkj.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mz.nszjky.cn

JS:   async function f() { await g(); }
来源：http://sa.newstarts.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://gw.jctech888.com.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hn.nszjky.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ix.shxzskj.cn

Ruby: # 用 Fiber 或 async gem
来源：http://do.huanxung.cn

C#:   async Task F() { await G(); }
来源：http://ju.colortex.cn

[O05] 并发执行并等待全部完成
来源：http://ks.newstarts.cn

Py:   asyncio.gather(*tasks)
来源：http://gn.szsharing.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://yi.jctech888.com.cn

JS:   await Promise.all(tasks)
来源：http://ja.bjjhwx.cn

TS:   await Promise.all(tasks)
来源：http://bw.huanxung.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ej.521024.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://am.shxzskj.cn

Ruby: threads.map(&:join)
来源：http://fn.szxytkj.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://ff.huixiangedu.cn

[O06] 使用进程池
来源：http://lk.colortex.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://yi.huixinmuqiang.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://pk.muxihuayi.cn

JS:   // child_process / cluster 模块
来源：http://me.bookmarksfly.cn

TS:   // child_process / cluster 模块
来源：http://mh.wgjwhj.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ci.shxzukj.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://sx.9csxet.cn

Ruby: // fork 块
来源：http://jv.haigaiapp.cn

C#:   Parallel.For
来源：http://je.lnxyls.cn

================================================================================
来源：http://mm.bookmarksfly.cn

P. 常用工具函数
来源：http://vf.shxzukj.cn

================================================================================
来源：http://ix.bookmarksfly.cn

[P01] 生成 UUID
来源：http://gk.gzmigu.cn

Py:   str(uuid.uuid4())
来源：http://fj.yuexingan06.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mj.nicolike.cn

JS:   crypto.randomUUID()
来源：http://lh.huanxung.cn

TS:   crypto.randomUUID()
来源：http://pr.colortex.cn

Java: UUID.randomUUID().toString()
来源：http://tl.wgjwhj.cn

Go:   // 用 github.com/google/uuid
来源：http://tr.521024.cn

Ruby: SecureRandom.uuid
来源：http://yc.bjjhwx.cn

C#:   Guid.NewGuid().ToString()
来源：http://zu.jctech888.com.cn

[P02] MD5 / SHA256 摘要
来源：http://gi.yuntaijiaju.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://zz.huixinmuqiang.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://hi.shxzukj.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://uj.huixinmuqiang.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://sg.yuexingan06.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://fu.newstarts.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ay.gzmigu.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hp.yuexingan06.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://bc.hnjuh.cn

[P03] 生成短随机字符串
来源：http://vd.bookmarksfly.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://fv.hnjuh.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mt.gzmigu.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://yd.panjiajie.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://js.nicolike.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://jw.nszjky.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://zt.huixinmuqiang.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://cl.colortex.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://sq.lnxyls.cn

[P04] 求长度
来源：http://qi.nszjky.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://tl.bjjhwx.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ds.newstarts.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://bo.huixiangedu.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wx.chemitech.net.cn

Java: list.size();  map.size();  s.length()
来源：http://ta.szxytkj.cn

Go:   len(arr);  len(m)
来源：http://vz.huixiangedu.cn

Ruby: x.length;  x.size
来源：http://ky.bjjhwx.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://wb.yuntaijiaju.cn

[P05] 判断两个对象内容是否相等
来源：http://dl.shxzukj.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://ko.bookmarksfly.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://iw.yuexingan06.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wo.muxihuayi.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://pz.jianghongdianzi.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://zu.gzmigu.cn

Go:   reflect.DeepEqual(a, b)
来源：http://em.yuntaijiaju.cn

Ruby: a == b
来源：http://re.wgjwhj.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://yr.shxzskj.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://yl.bookmarksfly.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wp.yuntaijiaju.cn

PHP:  if (empty($x)) {}
来源：http://er.newstarts.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://oc.hnjuh.cn

TS:   if (x == null) {}
来源：http://wa.bjjhwx.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://wc.szxytkj.cn

Go:   if x == nil {}
来源：http://kw.nszjky.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://yq.521024.cn

C#:   if (x is null) {}
来源：http://qw.haigaiapp.cn

[P07] 防抖与节流
来源：http://nx.colortex.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wx.huixiangedu.cn

PHP:  // 手写时间戳比较
来源：http://hf.jianghongdianzi.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://nc.jctech888.com.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://nf.hahajie.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://bn.panjiajie.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://sn.asd995.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://ia.bookmarksfly.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://py.521024.cn

[P08] 处理浮点精度问题
来源：http://aa.521024.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://uh.colortex.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://vn.newstarts.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://gl.bookmarksfly.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ja.panjiajie.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://us.bookmarksfly.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://va.gzmigu.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://vu.szxytkj.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://uy.chemitech.net.cn

================================================================================
来源：http://to.bjjhwx.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ue.shtwfgs.cn

================================================================================
来源：http://mm.bjjhwx.cn

[Q01] 创建表
来源：http://ot.shxzskj.cn

CREATE TABLE users (
来源：http://wd.9csxet.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://bo.panjiajie.cn

name VARCHAR(50) NOT NULL,
来源：http://bl.muxihuayi.cn

email VARCHAR(100) UNIQUE,
来源：http://bt.jctech888.com.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ws.huixiangedu.cn

);
来源：http://ri.wgjwhj.cn

[Q02] 创建带外键的表
来源：http://ph.nszjky.cn

CREATE TABLE orders (
来源：http://fu.9csxet.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hv.521024.cn

user_id INT NOT NULL,
来源：http://us.colortex.cn

amount DECIMAL(10, 2),
来源：http://zy.hahajie.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://nh.wgjwhj.cn

);
来源：http://wk.jianghongdianzi.cn

[Q03] 增加列
来源：http://tb.asd995.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://vu.bookmarksfly.cn

[Q04] 修改列类型
来源：http://sw.szsharing.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://yo.muxihuayi.cn

[Q05] 重命名列
来源：http://vd.asd995.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://pq.bookmarksfly.cn

[Q06] 删除列
来源：http://zb.yuexingan06.cn

ALTER TABLE users DROP COLUMN age;
来源：http://so.colortex.cn

[Q07] 删除表
来源：http://ns.chemitech.net.cn

DROP TABLE IF EXISTS orders;
来源：http://er.shxzskj.cn

[Q08] 创建普通索引
来源：http://hd.hnjuh.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://wa.huanxung.cn

[Q09] 创建唯一索引
来源：http://up.huixinmuqiang.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://zh.huixiangedu.cn

[Q10] 插入单行
来源：http://qp.jctech888.com.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://cd.nszjky.cn

[Q11] 一次插入多行
来源：http://kd.colortex.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://oi.shxzukj.cn

[Q12] 插入后取自增 ID
来源：http://ek.9csxet.cn

INSERT INTO users (name) VALUES ('C');
来源：http://af.huixiangedu.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://zd.bookmarksfly.cn

[Q13] 忽略重复插入
来源：http://td.huanxung.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://io.nszjky.cn

[Q14] 存在则更新（upsert）
来源：http://bc.jctech888.com.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://be.wgjwhj.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://oi.yuexingan06.cn

[Q15] 查询全部
来源：http://bb.bjjhwx.cn

SELECT * FROM users;
来源：http://zk.yuexingan06.cn

[Q16] 查询指定列
来源：http://md.jctech888.com.cn

SELECT id, name FROM users;
来源：http://oh.bjjhwx.cn

[Q17] 条件查询
来源：http://cg.haigaiapp.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mt.nicolike.cn

[Q18] 模糊匹配
来源：http://lf.asd995.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://zl.muxihuayi.cn

[Q19] 范围查询
来源：http://qa.huixiangedu.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ta.colortex.cn

[Q20] IN 列表
来源：http://ry.yuexingan06.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://fm.nszjky.cn

[Q21] 空值判断
来源：http://eq.huixiangedu.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://zn.hahajie.cn

[Q22] 排序
来源：http://zi.huixinmuqiang.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://jy.huixiangedu.cn

[Q23] 分页
来源：http://wt.newstarts.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ed.yuntaijiaju.cn

[Q24] 去重
来源：http://xm.szsharing.cn

SELECT DISTINCT city FROM users;
来源：http://kq.yuntaijiaju.cn

[Q25] 只取前 N 条
来源：http://bq.shxzskj.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://cc.yuexingan06.cn

[Q26] 计数
来源：http://xs.521024.cn

SELECT COUNT(*) FROM users;
来源：http://wb.huanxung.cn

[Q27] 条件计数
来源：http://ha.newstarts.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://df.newstarts.cn

[Q28] 求和与平均
来源：http://za.nszjky.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://jz.hahajie.cn

[Q29] 最大最小值
来源：http://fh.bjjhwx.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://xy.bjjhwx.cn

[Q30] 分组统计
来源：http://tb.szxytkj.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://kh.bjjhwx.cn

[Q31] 分组后过滤
来源：http://ov.panjiajie.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://av.muxihuayi.cn

[Q32] 分组拼接字符串
来源：http://bf.wgjwhj.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://tn.chemitech.net.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hh.szxytkj.cn

[Q33] 多列分组
来源：http://py.chemitech.net.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://gn.shxzukj.cn

[Q34] 每组取第一条
来源：http://rc.bookmarksfly.cn

SELECT * FROM (
来源：http://db.shxzukj.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://zs.asd995.cn

) t WHERE rn = 1;
来源：http://zw.jctech888.com.cn

[Q35] 内连接
来源：http://pv.szsharing.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://pb.shtwfgs.cn


<!-- 参考信息 -->