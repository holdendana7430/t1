代发 wailian999

[N01] 二分查找（有序数组）
来源：http://cj.hahajie.cn

Py:   bisect.bisect_left(arr, x)
来源：http://dv.shxzukj.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://yn.panjiajie.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mx.yuexingan06.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ai.panjiajie.cn

Java: Arrays.binarySearch(arr, x)
来源：http://iv.shtwfgs.cn

Go:   sort.SearchInts(arr, x)
来源：http://hi.shxzskj.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://pf.jianghongdianzi.cn

C#:   Array.BinarySearch(arr, x)
来源：http://ov.huixinmuqiang.cn

[N02] 排序（工程实践用内置实现）
来源：http://kp.asd995.cn

Py:   sorted(arr);  arr.sort()
来源：http://or.huixinmuqiang.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://bm.521024.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://yw.nicolike.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://zk.huixinmuqiang.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://oj.szxytkj.cn

Go:   slices.Sort(arr)
来源：http://pi.yuntaijiaju.cn

Ruby: arr.sort
来源：http://dn.hnjuh.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://lw.huixinmuqiang.cn

[N03] 快速排序（分治示例）
来源：http://uc.wgjwhj.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://pl.bookmarksfly.cn

PHP:  // 递归实现，或用 usort
来源：http://zt.hnjuh.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://oh.panjiajie.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://qw.huixiangedu.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://vf.lnxyls.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wi.szsharing.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://dq.szxytkj.cn

C#:   // 手写递归，或 Array.Sort
来源：http://zc.haigaiapp.cn

[N04] 斐波那契数列
来源：http://mk.chemitech.net.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ey.szxytkj.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ab.jianghongdianzi.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://dn.9csxet.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://lq.muxihuayi.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://tr.hnjuh.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ff.muxihuayi.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ir.jctech888.com.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://qr.nszjky.cn

[N05] 最大公约数
来源：http://na.shtwfgs.cn

Py:   math.gcd(a, b)
来源：http://th.hnjuh.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://vw.huanxung.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ta.szxytkj.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://vy.jianghongdianzi.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://nf.gzmigu.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wj.wgjwhj.cn

Ruby: a.gcd(b)
来源：http://hu.shxzukj.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://po.muxihuayi.cn

[N06] 判断回文字符串
来源：http://bk.wgjwhj.cn

Py:   s == s[::-1]
来源：http://sr.jctech888.com.cn

PHP:  $s === strrev($s);
来源：http://xw.wgjwhj.cn

JS:   s === [...s].reverse().join("")
来源：http://ms.haigaiapp.cn

TS:   s === [...s].reverse().join("")
来源：http://ak.shtwfgs.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://av.huixinmuqiang.cn

Go:   // 双指针从两端比较
来源：http://zv.muxihuayi.cn

Ruby: s == s.reverse
来源：http://qm.9csxet.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://oa.jctech888.com.cn

[N07] 两数之和（返回下标）
来源：http://yl.wgjwhj.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ft.lnxyls.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ln.bookmarksfly.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://oi.gzmigu.cn

TS:   // 手写 Map<string, number>
来源：http://sl.chemitech.net.cn

Java: // 手写 HashMap
来源：http://at.yuexingan06.cn

Go:   // 手写 map[int]int
来源：http://lv.muxihuayi.cn

Ruby: // 手写 Hash
来源：http://jl.jianghongdianzi.cn

C#:   // 手写 Dictionary<int, int>
来源：http://fu.bjjhwx.cn

[N08] 生成全排列
来源：http://an.wgjwhj.cn

Py:   itertools.permutations(arr)
来源：http://ki.jctech888.com.cn

PHP:  // 手写递归交换
来源：http://zb.9csxet.cn

JS:   // 手写回溯递归
来源：http://pu.szsharing.cn

TS:   // 手写回溯递归
来源：http://mp.shtwfgs.cn

Java: // 手写回溯递归
来源：http://oq.shxzukj.cn

Go:   // 手写回溯递归
来源：http://be.chemitech.net.cn

Ruby: arr.permutation.to_a
来源：http://ds.shxzskj.cn

C#:   // 手写回溯递归
来源：http://pa.szsharing.cn

[N09] 栈与队列
来源：http://hd.shtwfgs.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://bl.bookmarksfly.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://zx.huixinmuqiang.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://jc.szsharing.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://yn.panjiajie.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ji.yuntaijiaju.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://zm.asd995.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://pb.jctech888.com.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wd.jctech888.com.cn

[N10] 链表节点定义
来源：http://lr.panjiajie.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ln.jianghongdianzi.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://xz.colortex.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ks.521024.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://lq.nszjky.cn

Java: class Node { int v; Node next; }
来源：http://sh.hnjuh.cn

Go:   type Node struct { V int; Next *Node }
来源：http://en.szsharing.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://xv.nszjky.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://lk.nszjky.cn

[N11] 二叉树中序遍历
来源：http://qp.haigaiapp.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://pv.colortex.cn

PHP:  // 手写递归函数
来源：http://lj.szsharing.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://nk.haigaiapp.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://zi.shxzskj.cn

Java: // 手写递归
来源：http://cq.huanxung.cn

Go:   // 手写递归
来源：http://ab.hahajie.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://io.huanxung.cn

C#:   // 手写递归
来源：http://hl.shtwfgs.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ba.shtwfgs.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://tj.muxihuayi.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ta.szsharing.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://uy.lnxyls.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://lv.gzmigu.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://qp.szsharing.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ra.nicolike.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://lv.huixinmuqiang.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://iu.panjiajie.cn

================================================================================
来源：http://tq.chemitech.net.cn

O. 并发与异步
来源：http://dj.huixiangedu.cn

================================================================================
来源：http://rv.szxytkj.cn

[O01] 启动一个线程
来源：http://ud.bookmarksfly.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mx.hahajie.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://xa.nszjky.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://pb.asd995.cn

TS:   // 同 JS
来源：http://dy.panjiajie.cn

Java: new Thread(() -> f()).start()
来源：http://av.muxihuayi.cn

Go:   go f()
来源：http://nu.jianghongdianzi.cn

Ruby: Thread.new { f }
来源：http://wu.lnxyls.cn

C#:   Task.Run(() => F());
来源：http://nx.muxihuayi.cn

[O02] 使用线程池
来源：http://jg.asd995.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://zn.bjjhwx.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://jq.chemitech.net.cn

JS:   // worker_threads 线程池
来源：http://oj.haigaiapp.cn

TS:   // worker_threads 线程池
来源：http://pq.shxzskj.cn

Java: Executors.newFixedThreadPool(4)
来源：http://qo.szxytkj.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://jz.jctech888.com.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wi.hahajie.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ik.wgjwhj.cn

[O03] 加锁保护共享数据
来源：http://pa.gzmigu.cn

Py:   with lock: shared += 1
来源：http://cc.bookmarksfly.cn

PHP:  // 用 flock() 做文件锁
来源：http://qd.wgjwhj.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://lx.wgjwhj.cn

TS:   // 同 JS
来源：http://yb.shxzskj.cn

Java: synchronized (this) { shared++; }
来源：http://lc.hahajie.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://cs.bookmarksfly.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://iy.nszjky.cn

C#:   lock (gate) { shared++; }
来源：http://cm.hnjuh.cn

[O04] 定义异步函数并等待
来源：http://br.shtwfgs.cn

Py:   async def f():⏎    await g()
来源：http://kt.hahajie.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://pk.bjjhwx.cn

JS:   async function f() { await g(); }
来源：http://dj.yuexingan06.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://bh.asd995.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://je.nicolike.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://gk.szxytkj.cn

Ruby: # 用 Fiber 或 async gem
来源：http://cz.jctech888.com.cn

C#:   async Task F() { await G(); }
来源：http://bv.szxytkj.cn

[O05] 并发执行并等待全部完成
来源：http://dv.gzmigu.cn

Py:   asyncio.gather(*tasks)
来源：http://xi.shxzskj.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ap.haigaiapp.cn

JS:   await Promise.all(tasks)
来源：http://pf.bjjhwx.cn

TS:   await Promise.all(tasks)
来源：http://zi.colortex.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://sj.panjiajie.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://pz.szsharing.cn

Ruby: threads.map(&:join)
来源：http://fw.szsharing.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://kp.szsharing.cn

[O06] 使用进程池
来源：http://tl.chemitech.net.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://su.bookmarksfly.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://ab.shtwfgs.cn

JS:   // child_process / cluster 模块
来源：http://sw.bjjhwx.cn

TS:   // child_process / cluster 模块
来源：http://tw.huanxung.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://zx.hnjuh.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ja.newstarts.cn

Ruby: // fork 块
来源：http://gs.asd995.cn

C#:   Parallel.For
来源：http://fm.9csxet.cn

================================================================================
来源：http://gh.bjjhwx.cn

P. 常用工具函数
来源：http://ky.yuntaijiaju.cn

================================================================================
来源：http://hm.muxihuayi.cn

[P01] 生成 UUID
来源：http://rh.szxytkj.cn

Py:   str(uuid.uuid4())
来源：http://fh.9csxet.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hj.panjiajie.cn

JS:   crypto.randomUUID()
来源：http://ml.yuntaijiaju.cn

TS:   crypto.randomUUID()
来源：http://bo.yuexingan06.cn

Java: UUID.randomUUID().toString()
来源：http://hr.gzmigu.cn

Go:   // 用 github.com/google/uuid
来源：http://tv.jianghongdianzi.cn

Ruby: SecureRandom.uuid
来源：http://vx.asd995.cn

C#:   Guid.NewGuid().ToString()
来源：http://el.panjiajie.cn

[P02] MD5 / SHA256 摘要
来源：http://rd.haigaiapp.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://pk.panjiajie.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://ga.muxihuayi.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://zj.gzmigu.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ls.9csxet.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://kx.huanxung.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://eq.asd995.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://pr.asd995.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://nw.huanxung.cn

[P03] 生成短随机字符串
来源：http://tz.colortex.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://eb.yuexingan06.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ak.chemitech.net.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://xu.yuntaijiaju.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://nk.szsharing.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ow.521024.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://rj.huixinmuqiang.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://qb.shxzukj.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://na.hnjuh.cn

[P04] 求长度
来源：http://qo.9csxet.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://dk.jianghongdianzi.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://vr.hnjuh.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wo.szxytkj.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://fz.bookmarksfly.cn

Java: list.size();  map.size();  s.length()
来源：http://pv.haigaiapp.cn

Go:   len(arr);  len(m)
来源：http://ev.haigaiapp.cn

Ruby: x.length;  x.size
来源：http://vi.lnxyls.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://dd.jianghongdianzi.cn

[P05] 判断两个对象内容是否相等
来源：http://fq.bookmarksfly.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://ad.hnjuh.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://xs.huixinmuqiang.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ut.colortex.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://pw.asd995.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://we.panjiajie.cn

Go:   reflect.DeepEqual(a, b)
来源：http://pm.521024.cn

Ruby: a == b
来源：http://jv.jianghongdianzi.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://jv.bjjhwx.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mk.colortex.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ub.bjjhwx.cn

PHP:  if (empty($x)) {}
来源：http://xd.wgjwhj.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://og.hahajie.cn

TS:   if (x == null) {}
来源：http://ij.nicolike.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://cz.haigaiapp.cn

Go:   if x == nil {}
来源：http://kq.newstarts.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://fm.chemitech.net.cn

C#:   if (x is null) {}
来源：http://rb.nicolike.cn

[P07] 防抖与节流
来源：http://cu.521024.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://sk.lnxyls.cn

PHP:  // 手写时间戳比较
来源：http://bf.shxzukj.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://lz.colortex.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://rg.wgjwhj.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://sw.nszjky.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://fa.nicolike.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://kk.panjiajie.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://el.szxytkj.cn

[P08] 处理浮点精度问题
来源：http://yl.nicolike.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://js.nszjky.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://tc.haigaiapp.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://vu.nicolike.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://xi.haigaiapp.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ep.huanxung.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://oe.huixinmuqiang.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://za.9csxet.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://yw.szxytkj.cn

================================================================================
来源：http://mm.panjiajie.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://nk.chemitech.net.cn

================================================================================
来源：http://ds.shxzukj.cn

[Q01] 创建表
来源：http://dm.colortex.cn

CREATE TABLE users (
来源：http://ne.lnxyls.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://og.haigaiapp.cn

name VARCHAR(50) NOT NULL,
来源：http://ak.newstarts.cn

email VARCHAR(100) UNIQUE,
来源：http://ax.gzmigu.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ih.newstarts.cn

);
来源：http://gx.newstarts.cn

[Q02] 创建带外键的表
来源：http://ff.chemitech.net.cn

CREATE TABLE orders (
来源：http://bp.shxzskj.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ex.nszjky.cn

user_id INT NOT NULL,
来源：http://hu.hnjuh.cn

amount DECIMAL(10, 2),
来源：http://ue.9csxet.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://kc.huixinmuqiang.cn

);
来源：http://sm.bookmarksfly.cn

[Q03] 增加列
来源：http://hu.panjiajie.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://or.yuntaijiaju.cn

[Q04] 修改列类型
来源：http://ci.newstarts.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://yf.haigaiapp.cn

[Q05] 重命名列
来源：http://xl.muxihuayi.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wl.jctech888.com.cn

[Q06] 删除列
来源：http://oi.muxihuayi.cn

ALTER TABLE users DROP COLUMN age;
来源：http://aa.yuntaijiaju.cn

[Q07] 删除表
来源：http://rz.bjjhwx.cn

DROP TABLE IF EXISTS orders;
来源：http://io.shxzskj.cn

[Q08] 创建普通索引
来源：http://gs.521024.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://pg.asd995.cn

[Q09] 创建唯一索引
来源：http://wc.lnxyls.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://vb.newstarts.cn

[Q10] 插入单行
来源：http://zw.huanxung.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://rh.shtwfgs.cn

[Q11] 一次插入多行
来源：http://ya.521024.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://av.shxzskj.cn

[Q12] 插入后取自增 ID
来源：http://sz.newstarts.cn

INSERT INTO users (name) VALUES ('C');
来源：http://tx.jctech888.com.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://nu.nicolike.cn

[Q13] 忽略重复插入
来源：http://xy.szxytkj.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://te.shxzukj.cn

[Q14] 存在则更新（upsert）
来源：http://bn.521024.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://kq.gzmigu.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ae.hnjuh.cn

[Q15] 查询全部
来源：http://zp.panjiajie.cn

SELECT * FROM users;
来源：http://gp.yuntaijiaju.cn

[Q16] 查询指定列
来源：http://gj.shxzukj.cn

SELECT id, name FROM users;
来源：http://nq.nicolike.cn

[Q17] 条件查询
来源：http://pv.bookmarksfly.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://iq.huixiangedu.cn

[Q18] 模糊匹配
来源：http://kj.newstarts.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://zp.wgjwhj.cn

[Q19] 范围查询
来源：http://tz.huixiangedu.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mk.shxzskj.cn

[Q20] IN 列表
来源：http://ag.shxzskj.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hy.wgjwhj.cn

[Q21] 空值判断
来源：http://nr.szxytkj.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://ph.huanxung.cn

[Q22] 排序
来源：http://sz.yuntaijiaju.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ca.asd995.cn

[Q23] 分页
来源：http://wy.521024.cn


<!-- 参考信息 -->