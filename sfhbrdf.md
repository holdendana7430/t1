代发 wailian999

Ruby: arr.sort
来源：http://ks.szsharing.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://se.huixiangedu.cn

[N03] 快速排序（分治示例）
来源：http://du.chemitech.net.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ux.jctech888.com.cn

PHP:  // 递归实现，或用 usort
来源：http://wz.jctech888.com.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wm.shxzskj.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://eo.521024.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ol.lnxyls.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://vh.jianghongdianzi.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://zj.bjjhwx.cn

C#:   // 手写递归，或 Array.Sort
来源：http://lr.haigaiapp.cn

[N04] 斐波那契数列
来源：http://tg.szsharing.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://zi.jctech888.com.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://le.hnjuh.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://bq.jianghongdianzi.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://pr.nszjky.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://eo.panjiajie.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://yi.bookmarksfly.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://pg.bookmarksfly.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://uc.szxytkj.cn

[N05] 最大公约数
来源：http://yv.gzmigu.cn

Py:   math.gcd(a, b)
来源：http://jg.muxihuayi.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://gs.nszjky.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mq.nicolike.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://oa.szxytkj.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://os.panjiajie.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://zr.jianghongdianzi.cn

Ruby: a.gcd(b)
来源：http://sa.newstarts.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://pl.gzmigu.cn

[N06] 判断回文字符串
来源：http://fr.9csxet.cn

Py:   s == s[::-1]
来源：http://zt.wgjwhj.cn

PHP:  $s === strrev($s);
来源：http://ll.hahajie.cn

JS:   s === [...s].reverse().join("")
来源：http://bc.shxzukj.cn

TS:   s === [...s].reverse().join("")
来源：http://hc.gzmigu.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://oi.hnjuh.cn

Go:   // 双指针从两端比较
来源：http://fv.hnjuh.cn

Ruby: s == s.reverse
来源：http://ps.bjjhwx.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://pr.shtwfgs.cn

[N07] 两数之和（返回下标）
来源：http://hj.wgjwhj.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ev.jianghongdianzi.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://xa.huanxung.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://hh.haigaiapp.cn

TS:   // 手写 Map<string, number>
来源：http://rw.shtwfgs.cn

Java: // 手写 HashMap
来源：http://yv.huanxung.cn

Go:   // 手写 map[int]int
来源：http://tj.szsharing.cn

Ruby: // 手写 Hash
来源：http://kv.panjiajie.cn

C#:   // 手写 Dictionary<int, int>
来源：http://lu.haigaiapp.cn

[N08] 生成全排列
来源：http://yu.haigaiapp.cn

Py:   itertools.permutations(arr)
来源：http://hx.szxytkj.cn

PHP:  // 手写递归交换
来源：http://rt.muxihuayi.cn

JS:   // 手写回溯递归
来源：http://ay.yuntaijiaju.cn

TS:   // 手写回溯递归
来源：http://mq.huixiangedu.cn

Java: // 手写回溯递归
来源：http://yf.asd995.cn

Go:   // 手写回溯递归
来源：http://dr.jctech888.com.cn

Ruby: arr.permutation.to_a
来源：http://un.chemitech.net.cn

C#:   // 手写回溯递归
来源：http://mu.bookmarksfly.cn

[N09] 栈与队列
来源：http://ud.panjiajie.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ti.hahajie.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://df.muxihuayi.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://pa.huanxung.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ma.jianghongdianzi.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://gw.panjiajie.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ld.yuntaijiaju.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wh.panjiajie.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://cq.521024.cn

[N10] 链表节点定义
来源：http://dc.nszjky.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://zh.panjiajie.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://iy.newstarts.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://gf.huixiangedu.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://fh.nszjky.cn

Java: class Node { int v; Node next; }
来源：http://nj.nszjky.cn

Go:   type Node struct { V int; Next *Node }
来源：http://mt.hahajie.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://sb.lnxyls.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://xb.521024.cn

[N11] 二叉树中序遍历
来源：http://an.jianghongdianzi.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://xa.huixinmuqiang.cn

PHP:  // 手写递归函数
来源：http://qj.huixiangedu.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://eu.nicolike.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://fr.hahajie.cn

Java: // 手写递归
来源：http://ta.shxzskj.cn

Go:   // 手写递归
来源：http://jh.lnxyls.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hu.shtwfgs.cn

C#:   // 手写递归
来源：http://zh.shtwfgs.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://gf.hahajie.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ho.bookmarksfly.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wa.panjiajie.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://sk.colortex.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://jv.shxzskj.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mb.panjiajie.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://qc.bookmarksfly.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://iu.muxihuayi.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://lr.huixiangedu.cn

================================================================================
来源：http://uu.muxihuayi.cn

O. 并发与异步
来源：http://zp.szsharing.cn

================================================================================
来源：http://yv.hahajie.cn

[O01] 启动一个线程
来源：http://eh.9csxet.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ra.lnxyls.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://yq.shxzukj.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://az.nicolike.cn

TS:   // 同 JS
来源：http://xw.yuntaijiaju.cn

Java: new Thread(() -> f()).start()
来源：http://zr.yuexingan06.cn

Go:   go f()
来源：http://tk.huanxung.cn

Ruby: Thread.new { f }
来源：http://dx.shxzukj.cn

C#:   Task.Run(() => F());
来源：http://uo.bjjhwx.cn

[O02] 使用线程池
来源：http://mf.newstarts.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://kp.bookmarksfly.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://kq.9csxet.cn

JS:   // worker_threads 线程池
来源：http://hm.jctech888.com.cn

TS:   // worker_threads 线程池
来源：http://jp.huixinmuqiang.cn

Java: Executors.newFixedThreadPool(4)
来源：http://fn.panjiajie.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://xt.colortex.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://tb.asd995.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://dz.yuexingan06.cn

[O03] 加锁保护共享数据
来源：http://qb.newstarts.cn

Py:   with lock: shared += 1
来源：http://uh.shxzskj.cn

PHP:  // 用 flock() 做文件锁
来源：http://lz.gzmigu.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://jz.huixinmuqiang.cn

TS:   // 同 JS
来源：http://bx.szsharing.cn

Java: synchronized (this) { shared++; }
来源：http://ec.shxzukj.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mc.hahajie.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://am.shtwfgs.cn

C#:   lock (gate) { shared++; }
来源：http://iv.haigaiapp.cn

[O04] 定义异步函数并等待
来源：http://ab.gzmigu.cn

Py:   async def f():⏎    await g()
来源：http://ht.hnjuh.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hn.panjiajie.cn

JS:   async function f() { await g(); }
来源：http://qg.nicolike.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://ci.bookmarksfly.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://an.shtwfgs.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://dm.9csxet.cn

Ruby: # 用 Fiber 或 async gem
来源：http://qb.bookmarksfly.cn

C#:   async Task F() { await G(); }
来源：http://hy.haigaiapp.cn

[O05] 并发执行并等待全部完成
来源：http://gm.shxzukj.cn

Py:   asyncio.gather(*tasks)
来源：http://wc.asd995.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://vf.chemitech.net.cn

JS:   await Promise.all(tasks)
来源：http://ad.szsharing.cn

TS:   await Promise.all(tasks)
来源：http://wb.huixiangedu.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://di.yuexingan06.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://dw.lnxyls.cn

Ruby: threads.map(&:join)
来源：http://zn.yuntaijiaju.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://mu.haigaiapp.cn

[O06] 使用进程池
来源：http://uq.jctech888.com.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://rr.lnxyls.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://as.huanxung.cn

JS:   // child_process / cluster 模块
来源：http://ez.asd995.cn

TS:   // child_process / cluster 模块
来源：http://fh.asd995.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://oa.shxzukj.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ze.yuexingan06.cn

Ruby: // fork 块
来源：http://ju.shxzskj.cn

C#:   Parallel.For
来源：http://fu.gzmigu.cn

================================================================================
来源：http://cr.huixinmuqiang.cn

P. 常用工具函数
来源：http://nx.shtwfgs.cn

================================================================================
来源：http://yo.521024.cn

[P01] 生成 UUID
来源：http://xh.panjiajie.cn

Py:   str(uuid.uuid4())
来源：http://ni.nszjky.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://am.haigaiapp.cn

JS:   crypto.randomUUID()
来源：http://ap.bookmarksfly.cn

TS:   crypto.randomUUID()
来源：http://fp.haigaiapp.cn

Java: UUID.randomUUID().toString()
来源：http://gd.muxihuayi.cn

Go:   // 用 github.com/google/uuid
来源：http://cm.bookmarksfly.cn

Ruby: SecureRandom.uuid
来源：http://bj.jctech888.com.cn

C#:   Guid.NewGuid().ToString()
来源：http://nv.shxzskj.cn

[P02] MD5 / SHA256 摘要
来源：http://ue.yuexingan06.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ul.shxzskj.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://rc.bookmarksfly.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ci.nszjky.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://bb.shxzukj.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://vw.nszjky.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://bd.wgjwhj.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ez.9csxet.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://zk.haigaiapp.cn

[P03] 生成短随机字符串
来源：http://xk.huixinmuqiang.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://dp.yuntaijiaju.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://rw.szsharing.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://tn.panjiajie.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://au.hahajie.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://yt.asd995.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://rx.muxihuayi.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://ml.panjiajie.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hr.hnjuh.cn

[P04] 求长度
来源：http://wf.9csxet.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://za.jianghongdianzi.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://un.szxytkj.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://xu.hnjuh.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://gd.muxihuayi.cn

Java: list.size();  map.size();  s.length()
来源：http://ih.panjiajie.cn

Go:   len(arr);  len(m)
来源：http://gq.muxihuayi.cn

Ruby: x.length;  x.size
来源：http://tz.szsharing.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://wd.nszjky.cn

[P05] 判断两个对象内容是否相等
来源：http://am.huanxung.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://lr.lnxyls.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ol.yuexingan06.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://gu.nszjky.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://og.huanxung.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://me.yuexingan06.cn

Go:   reflect.DeepEqual(a, b)
来源：http://wi.521024.cn

Ruby: a == b
来源：http://nm.yuntaijiaju.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://td.haigaiapp.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://lq.huanxung.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://zi.shtwfgs.cn

PHP:  if (empty($x)) {}
来源：http://lt.newstarts.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ut.gzmigu.cn

TS:   if (x == null) {}
来源：http://hl.hahajie.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://rr.szxytkj.cn

Go:   if x == nil {}
来源：http://ii.panjiajie.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://tc.shtwfgs.cn

C#:   if (x is null) {}
来源：http://fs.newstarts.cn

[P07] 防抖与节流
来源：http://er.huanxung.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://qj.shtwfgs.cn

PHP:  // 手写时间戳比较
来源：http://vs.panjiajie.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://sj.jianghongdianzi.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://he.9csxet.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://qx.muxihuayi.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://rc.huixiangedu.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://tr.szsharing.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://qw.hnjuh.cn

[P08] 处理浮点精度问题
来源：http://jf.asd995.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://no.nicolike.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://pk.jctech888.com.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://lj.chemitech.net.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://vi.shxzukj.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://en.lnxyls.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ms.wgjwhj.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://th.szxytkj.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://jt.huixinmuqiang.cn

================================================================================
来源：http://uj.jianghongdianzi.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://cr.bjjhwx.cn

================================================================================
来源：http://tv.muxihuayi.cn

[Q01] 创建表
来源：http://zt.colortex.cn

CREATE TABLE users (
来源：http://bd.shxzukj.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://bk.newstarts.cn

name VARCHAR(50) NOT NULL,
来源：http://sd.huixiangedu.cn

email VARCHAR(100) UNIQUE,
来源：http://ve.yuntaijiaju.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://xr.nicolike.cn

);
来源：http://so.muxihuayi.cn

[Q02] 创建带外键的表
来源：http://uh.jianghongdianzi.cn

CREATE TABLE orders (
来源：http://vo.hahajie.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://oc.colortex.cn

user_id INT NOT NULL,
来源：http://tl.shtwfgs.cn

amount DECIMAL(10, 2),
来源：http://sl.lnxyls.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://yq.gzmigu.cn

);
来源：http://fx.hnjuh.cn

[Q03] 增加列
来源：http://rt.lnxyls.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://bs.huixinmuqiang.cn

[Q04] 修改列类型
来源：http://gm.gzmigu.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://qe.szxytkj.cn

[Q05] 重命名列
来源：http://gl.huixinmuqiang.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://dz.521024.cn

[Q06] 删除列
来源：http://cb.nicolike.cn

ALTER TABLE users DROP COLUMN age;
来源：http://tz.bookmarksfly.cn

[Q07] 删除表
来源：http://bs.huixiangedu.cn

DROP TABLE IF EXISTS orders;
来源：http://id.chemitech.net.cn

[Q08] 创建普通索引
来源：http://pv.szsharing.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://fs.nszjky.cn

[Q09] 创建唯一索引
来源：http://jl.wgjwhj.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://qi.jctech888.com.cn

[Q10] 插入单行
来源：http://rb.colortex.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://tg.shxzskj.cn

[Q11] 一次插入多行
来源：http://wj.shxzskj.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://cs.lnxyls.cn

[Q12] 插入后取自增 ID
来源：http://rs.521024.cn

INSERT INTO users (name) VALUES ('C');
来源：http://ps.newstarts.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://cm.shtwfgs.cn

[Q13] 忽略重复插入
来源：http://rr.colortex.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://rk.newstarts.cn

[Q14] 存在则更新（upsert）
来源：http://gd.bjjhwx.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://al.hnjuh.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ei.shxzukj.cn

[Q15] 查询全部
来源：http://js.nszjky.cn

SELECT * FROM users;
来源：http://re.yuntaijiaju.cn

[Q16] 查询指定列
来源：http://cb.haigaiapp.cn

SELECT id, name FROM users;
来源：http://cl.chemitech.net.cn

[Q17] 条件查询
来源：http://al.huanxung.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ja.hahajie.cn

[Q18] 模糊匹配
来源：http://yo.9csxet.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://kk.521024.cn

[Q19] 范围查询
来源：http://nq.haigaiapp.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://lc.shtwfgs.cn

[Q20] IN 列表
来源：http://fn.nszjky.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://uu.haigaiapp.cn

[Q21] 空值判断
来源：http://qu.chemitech.net.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://il.lnxyls.cn

[Q22] 排序
来源：http://un.panjiajie.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ui.haigaiapp.cn

[Q23] 分页
来源：http://ov.wgjwhj.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://lm.yuexingan06.cn

[Q24] 去重
来源：http://rh.muxihuayi.cn

SELECT DISTINCT city FROM users;
来源：http://nf.newstarts.cn

[Q25] 只取前 N 条
来源：http://te.huanxung.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://xn.huixinmuqiang.cn

[Q26] 计数
来源：http://ce.muxihuayi.cn

SELECT COUNT(*) FROM users;
来源：http://ly.chemitech.net.cn

[Q27] 条件计数
来源：http://dx.lnxyls.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://gr.shtwfgs.cn

[Q28] 求和与平均
来源：http://ra.bookmarksfly.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://ct.huixiangedu.cn

[Q29] 最大最小值
来源：http://xn.haigaiapp.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://jz.jianghongdianzi.cn

[Q30] 分组统计
来源：http://ok.szxytkj.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://lf.asd995.cn

[Q31] 分组后过滤
来源：http://sn.yuexingan06.cn


<!-- 参考信息 -->