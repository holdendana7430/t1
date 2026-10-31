代发 wailian999

C#:   Environment.OSVersion;  Environment.Version
来源：http://rz.9csxet.cn

================================================================================
来源：http://gc.muxihuayi.cn

N. 数据结构与算法
来源：http://ki.shxzskj.cn

================================================================================
来源：http://mx.bjjhwx.cn

[N01] 二分查找（有序数组）
来源：http://kf.wgjwhj.cn

Py:   bisect.bisect_left(arr, x)
来源：http://yh.yuexingan06.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://jx.bookmarksfly.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ex.yuntaijiaju.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hg.hnjuh.cn

Java: Arrays.binarySearch(arr, x)
来源：http://fi.lnxyls.cn

Go:   sort.SearchInts(arr, x)
来源：http://zh.bjjhwx.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://tn.jianghongdianzi.cn

C#:   Array.BinarySearch(arr, x)
来源：http://jd.yuexingan06.cn

[N02] 排序（工程实践用内置实现）
来源：http://in.nicolike.cn

Py:   sorted(arr);  arr.sort()
来源：http://ls.szxytkj.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://bt.chemitech.net.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://tm.chemitech.net.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://et.hahajie.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ao.wgjwhj.cn

Go:   slices.Sort(arr)
来源：http://ut.shxzskj.cn

Ruby: arr.sort
来源：http://my.szxytkj.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://bn.gzmigu.cn

[N03] 快速排序（分治示例）
来源：http://mt.gzmigu.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://os.nszjky.cn

PHP:  // 递归实现，或用 usort
来源：http://zl.shtwfgs.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://id.colortex.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://fd.hnjuh.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://xh.yuntaijiaju.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://zz.huixiangedu.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hr.521024.cn

C#:   // 手写递归，或 Array.Sort
来源：http://tn.szxytkj.cn

[N04] 斐波那契数列
来源：http://tw.shxzskj.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://gr.huanxung.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://zf.colortex.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://qb.muxihuayi.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://at.haigaiapp.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://bx.bookmarksfly.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://vg.lnxyls.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://xs.shxzskj.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.bjjhwx.cn

[N05] 最大公约数
来源：http://sq.521024.cn

Py:   math.gcd(a, b)
来源：http://he.colortex.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://lg.yuntaijiaju.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://oz.bjjhwx.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://kw.yuntaijiaju.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://jh.yuntaijiaju.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://vu.hahajie.cn

Ruby: a.gcd(b)
来源：http://re.gzmigu.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ua.muxihuayi.cn

[N06] 判断回文字符串
来源：http://uz.521024.cn

Py:   s == s[::-1]
来源：http://ca.shxzukj.cn

PHP:  $s === strrev($s);
来源：http://ol.yuexingan06.cn

JS:   s === [...s].reverse().join("")
来源：http://lj.521024.cn

TS:   s === [...s].reverse().join("")
来源：http://db.szsharing.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://pz.newstarts.cn

Go:   // 双指针从两端比较
来源：http://ut.9csxet.cn

Ruby: s == s.reverse
来源：http://rt.asd995.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://ka.shtwfgs.cn

[N07] 两数之和（返回下标）
来源：http://qt.521024.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://nq.hnjuh.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ga.521024.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://cs.bjjhwx.cn

TS:   // 手写 Map<string, number>
来源：http://nx.bjjhwx.cn

Java: // 手写 HashMap
来源：http://ti.jianghongdianzi.cn

Go:   // 手写 map[int]int
来源：http://qg.chemitech.net.cn

Ruby: // 手写 Hash
来源：http://ow.shxzskj.cn

C#:   // 手写 Dictionary<int, int>
来源：http://io.lnxyls.cn

[N08] 生成全排列
来源：http://ps.colortex.cn

Py:   itertools.permutations(arr)
来源：http://rn.jianghongdianzi.cn

PHP:  // 手写递归交换
来源：http://dl.muxihuayi.cn

JS:   // 手写回溯递归
来源：http://xm.muxihuayi.cn

TS:   // 手写回溯递归
来源：http://dl.nszjky.cn

Java: // 手写回溯递归
来源：http://es.shxzukj.cn

Go:   // 手写回溯递归
来源：http://jb.asd995.cn

Ruby: arr.permutation.to_a
来源：http://jp.hahajie.cn

C#:   // 手写回溯递归
来源：http://sj.huixinmuqiang.cn

[N09] 栈与队列
来源：http://gm.asd995.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://sl.521024.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ty.bookmarksfly.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hr.huanxung.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://bo.huixinmuqiang.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://up.nicolike.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mi.lnxyls.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://uy.bookmarksfly.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://kj.shxzskj.cn

[N10] 链表节点定义
来源：http://ot.gzmigu.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://uy.9csxet.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://as.bookmarksfly.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://vp.9csxet.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://tm.panjiajie.cn

Java: class Node { int v; Node next; }
来源：http://on.bookmarksfly.cn

Go:   type Node struct { V int; Next *Node }
来源：http://ss.lnxyls.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://ot.szxytkj.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://id.shtwfgs.cn

[N11] 二叉树中序遍历
来源：http://lm.chemitech.net.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hu.shxzukj.cn

PHP:  // 手写递归函数
来源：http://dp.huixinmuqiang.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://az.huanxung.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://uc.jianghongdianzi.cn

Java: // 手写递归
来源：http://au.jianghongdianzi.cn

Go:   // 手写递归
来源：http://ex.521024.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://dc.shtwfgs.cn

C#:   // 手写递归
来源：http://ix.jianghongdianzi.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ue.lnxyls.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://dp.yuexingan06.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://sz.chemitech.net.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://kn.colortex.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://yo.haigaiapp.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://rv.yuexingan06.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://yf.nszjky.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://fy.nicolike.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://pa.521024.cn

================================================================================
来源：http://sz.jianghongdianzi.cn

O. 并发与异步
来源：http://th.yuntaijiaju.cn

================================================================================
来源：http://kv.nszjky.cn

[O01] 启动一个线程
来源：http://uz.asd995.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ir.hahajie.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://zl.yuntaijiaju.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ef.nicolike.cn

TS:   // 同 JS
来源：http://oa.nszjky.cn

Java: new Thread(() -> f()).start()
来源：http://bq.jctech888.com.cn

Go:   go f()
来源：http://qc.nszjky.cn

Ruby: Thread.new { f }
来源：http://ul.muxihuayi.cn

C#:   Task.Run(() => F());
来源：http://gg.chemitech.net.cn

[O02] 使用线程池
来源：http://xd.hahajie.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wu.yuntaijiaju.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://kw.shtwfgs.cn

JS:   // worker_threads 线程池
来源：http://rf.nicolike.cn

TS:   // worker_threads 线程池
来源：http://uw.hahajie.cn

Java: Executors.newFixedThreadPool(4)
来源：http://xb.lnxyls.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://gq.huixiangedu.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://aw.bjjhwx.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://sf.muxihuayi.cn

[O03] 加锁保护共享数据
来源：http://ne.colortex.cn

Py:   with lock: shared += 1
来源：http://eq.gzmigu.cn

PHP:  // 用 flock() 做文件锁
来源：http://xz.lnxyls.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ez.nszjky.cn

TS:   // 同 JS
来源：http://es.nicolike.cn

Java: synchronized (this) { shared++; }
来源：http://it.bookmarksfly.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://rk.shxzukj.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://ec.asd995.cn

C#:   lock (gate) { shared++; }
来源：http://zc.nicolike.cn

[O04] 定义异步函数并等待
来源：http://rw.huixinmuqiang.cn

Py:   async def f():⏎    await g()
来源：http://yy.bookmarksfly.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://vi.panjiajie.cn

JS:   async function f() { await g(); }
来源：http://iq.9csxet.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://jp.shtwfgs.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://rd.wgjwhj.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://zq.haigaiapp.cn

Ruby: # 用 Fiber 或 async gem
来源：http://ez.szsharing.cn

C#:   async Task F() { await G(); }
来源：http://ph.shtwfgs.cn

[O05] 并发执行并等待全部完成
来源：http://ih.jctech888.com.cn

Py:   asyncio.gather(*tasks)
来源：http://zl.shxzukj.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hm.huixiangedu.cn

JS:   await Promise.all(tasks)
来源：http://ur.yuexingan06.cn

TS:   await Promise.all(tasks)
来源：http://vw.hnjuh.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://yq.szsharing.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://gw.huixiangedu.cn

Ruby: threads.map(&:join)
来源：http://wu.hnjuh.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://ve.nicolike.cn

[O06] 使用进程池
来源：http://ti.lnxyls.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://rf.jianghongdianzi.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://tx.haigaiapp.cn

JS:   // child_process / cluster 模块
来源：http://nw.shxzskj.cn

TS:   // child_process / cluster 模块
来源：http://on.521024.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://bh.szsharing.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://fg.gzmigu.cn

Ruby: // fork 块
来源：http://iq.szsharing.cn

C#:   Parallel.For
来源：http://sy.haigaiapp.cn

================================================================================
来源：http://mf.lnxyls.cn

P. 常用工具函数
来源：http://gg.lnxyls.cn

================================================================================
来源：http://nq.bookmarksfly.cn

[P01] 生成 UUID
来源：http://iq.newstarts.cn

Py:   str(uuid.uuid4())
来源：http://ud.nicolike.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://yk.yuntaijiaju.cn

JS:   crypto.randomUUID()
来源：http://ag.huixiangedu.cn

TS:   crypto.randomUUID()
来源：http://ha.szxytkj.cn

Java: UUID.randomUUID().toString()
来源：http://yh.shxzskj.cn

Go:   // 用 github.com/google/uuid
来源：http://jo.jctech888.com.cn

Ruby: SecureRandom.uuid
来源：http://hr.yuexingan06.cn

C#:   Guid.NewGuid().ToString()
来源：http://ib.colortex.cn

[P02] MD5 / SHA256 摘要
来源：http://qk.panjiajie.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://dj.nszjky.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://ui.szsharing.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://tf.shtwfgs.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://si.muxihuayi.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ze.newstarts.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://fw.bookmarksfly.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://xt.muxihuayi.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://su.jianghongdianzi.cn

[P03] 生成短随机字符串
来源：http://hy.asd995.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://bh.jianghongdianzi.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://vd.shxzukj.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://nt.huixinmuqiang.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://aq.yuntaijiaju.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://uk.chemitech.net.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ly.nszjky.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://rj.hnjuh.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://zl.gzmigu.cn

[P04] 求长度
来源：http://ul.chemitech.net.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://oy.lnxyls.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://pf.9csxet.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wy.asd995.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://bd.muxihuayi.cn

Java: list.size();  map.size();  s.length()
来源：http://rc.bookmarksfly.cn

Go:   len(arr);  len(m)
来源：http://hp.hahajie.cn

Ruby: x.length;  x.size
来源：http://xt.colortex.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://sz.colortex.cn

[P05] 判断两个对象内容是否相等
来源：http://ln.newstarts.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://nz.shtwfgs.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://dz.panjiajie.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ln.shxzskj.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://lu.jianghongdianzi.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ht.huanxung.cn

Go:   reflect.DeepEqual(a, b)
来源：http://zp.jianghongdianzi.cn

Ruby: a == b
来源：http://qt.shxzukj.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://aj.shxzskj.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ru.wgjwhj.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://sk.huixinmuqiang.cn

PHP:  if (empty($x)) {}
来源：http://it.muxihuayi.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://nh.jctech888.com.cn

TS:   if (x == null) {}
来源：http://yk.haigaiapp.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://ry.bookmarksfly.cn

Go:   if x == nil {}
来源：http://xn.jctech888.com.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://oe.nszjky.cn

C#:   if (x is null) {}
来源：http://pm.colortex.cn

[P07] 防抖与节流
来源：http://fg.huixiangedu.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://vq.huixinmuqiang.cn

PHP:  // 手写时间戳比较
来源：http://rx.szsharing.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://yy.chemitech.net.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hr.shxzukj.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://fb.szsharing.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://rc.9csxet.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://ce.yuexingan06.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://km.newstarts.cn

[P08] 处理浮点精度问题
来源：http://yr.hnjuh.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ww.panjiajie.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://iz.newstarts.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://cl.bjjhwx.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://my.hnjuh.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ir.huixinmuqiang.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ww.gzmigu.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://pg.haigaiapp.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://uo.chemitech.net.cn

================================================================================
来源：http://us.gzmigu.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://jv.shxzskj.cn

================================================================================
来源：http://nf.521024.cn

[Q01] 创建表
来源：http://at.yuntaijiaju.cn

CREATE TABLE users (
来源：http://di.yuexingan06.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ez.chemitech.net.cn

name VARCHAR(50) NOT NULL,
来源：http://zt.jianghongdianzi.cn

email VARCHAR(100) UNIQUE,
来源：http://xv.jianghongdianzi.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://cz.panjiajie.cn

);
来源：http://rn.haigaiapp.cn

[Q02] 创建带外键的表
来源：http://dt.panjiajie.cn

CREATE TABLE orders (
来源：http://pe.jctech888.com.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://gz.nicolike.cn

user_id INT NOT NULL,
来源：http://vs.yuntaijiaju.cn

amount DECIMAL(10, 2),
来源：http://ir.nszjky.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://pa.bjjhwx.cn

);
来源：http://re.shxzukj.cn

[Q03] 增加列
来源：http://pi.szsharing.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://tn.yuntaijiaju.cn

[Q04] 修改列类型
来源：http://fw.521024.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://lc.lnxyls.cn

[Q05] 重命名列
来源：http://zn.szxytkj.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://dz.huanxung.cn

[Q06] 删除列
来源：http://he.chemitech.net.cn

ALTER TABLE users DROP COLUMN age;
来源：http://ok.lnxyls.cn

[Q07] 删除表
来源：http://rw.newstarts.cn

DROP TABLE IF EXISTS orders;
来源：http://qe.newstarts.cn

[Q08] 创建普通索引
来源：http://dw.szxytkj.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://kp.huanxung.cn

[Q09] 创建唯一索引
来源：http://ea.shxzukj.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ij.colortex.cn

[Q10] 插入单行
来源：http://cb.hahajie.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://gx.shxzskj.cn

[Q11] 一次插入多行
来源：http://qb.chemitech.net.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://nc.hnjuh.cn

[Q12] 插入后取自增 ID
来源：http://fg.panjiajie.cn

INSERT INTO users (name) VALUES ('C');
来源：http://ur.bookmarksfly.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://bl.chemitech.net.cn

[Q13] 忽略重复插入
来源：http://sz.bjjhwx.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://eo.jianghongdianzi.cn

[Q14] 存在则更新（upsert）
来源：http://dk.hahajie.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://yv.asd995.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://cy.shtwfgs.cn

[Q15] 查询全部
来源：http://xu.szxytkj.cn

SELECT * FROM users;
来源：http://ea.521024.cn

[Q16] 查询指定列
来源：http://vn.bjjhwx.cn

SELECT id, name FROM users;
来源：http://on.jctech888.com.cn

[Q17] 条件查询
来源：http://sm.muxihuayi.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://yk.huanxung.cn

[Q18] 模糊匹配
来源：http://fs.521024.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://js.jianghongdianzi.cn

[Q19] 范围查询
来源：http://yk.huixinmuqiang.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ys.szxytkj.cn

[Q20] IN 列表
来源：http://xf.huixinmuqiang.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://fy.bjjhwx.cn

[Q21] 空值判断
来源：http://oe.huixinmuqiang.cn


<!-- 参考信息 -->