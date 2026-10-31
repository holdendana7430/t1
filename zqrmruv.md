代发 wailian999

[N01] 二分查找（有序数组）
来源：http://qa.panjiajie.cn

Py:   bisect.bisect_left(arr, x)
来源：http://zd.521024.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://rm.nszjky.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://xl.asd995.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://pf.shxzskj.cn

Java: Arrays.binarySearch(arr, x)
来源：http://bh.haigaiapp.cn

Go:   sort.SearchInts(arr, x)
来源：http://au.nicolike.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://vw.hnjuh.cn

C#:   Array.BinarySearch(arr, x)
来源：http://sx.9csxet.cn

[N02] 排序（工程实践用内置实现）
来源：http://dh.gzmigu.cn

Py:   sorted(arr);  arr.sort()
来源：http://gd.yuexingan06.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://pf.szsharing.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://ja.shtwfgs.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://gm.nszjky.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://om.muxihuayi.cn

Go:   slices.Sort(arr)
来源：http://cg.szsharing.cn

Ruby: arr.sort
来源：http://cp.521024.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://vr.wgjwhj.cn

[N03] 快速排序（分治示例）
来源：http://bk.nszjky.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://bq.shxzskj.cn

PHP:  // 递归实现，或用 usort
来源：http://aa.szsharing.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ut.colortex.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://jd.521024.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://kg.huixiangedu.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ar.chemitech.net.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://oh.huanxung.cn

C#:   // 手写递归，或 Array.Sort
来源：http://wm.gzmigu.cn

[N04] 斐波那契数列
来源：http://ek.nszjky.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://yl.shtwfgs.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://vt.muxihuayi.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://qd.shxzskj.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://rh.asd995.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hw.szxytkj.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://at.colortex.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mj.wgjwhj.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://dz.panjiajie.cn

[N05] 最大公约数
来源：http://ri.9csxet.cn

Py:   math.gcd(a, b)
来源：http://xr.shxzskj.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://yg.haigaiapp.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mq.9csxet.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://cz.nicolike.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://en.bookmarksfly.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://sb.shxzskj.cn

Ruby: a.gcd(b)
来源：http://ud.hnjuh.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://tm.shxzukj.cn

[N06] 判断回文字符串
来源：http://sb.wgjwhj.cn

Py:   s == s[::-1]
来源：http://ix.jctech888.com.cn

PHP:  $s === strrev($s);
来源：http://wb.asd995.cn

JS:   s === [...s].reverse().join("")
来源：http://mz.shxzskj.cn

TS:   s === [...s].reverse().join("")
来源：http://jy.yuexingan06.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://xo.szxytkj.cn

Go:   // 双指针从两端比较
来源：http://ff.bookmarksfly.cn

Ruby: s == s.reverse
来源：http://ka.yuexingan06.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://hm.newstarts.cn

[N07] 两数之和（返回下标）
来源：http://tj.wgjwhj.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://jn.asd995.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://lc.shxzskj.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://kt.hahajie.cn

TS:   // 手写 Map<string, number>
来源：http://mw.521024.cn

Java: // 手写 HashMap
来源：http://am.szxytkj.cn

Go:   // 手写 map[int]int
来源：http://is.shxzukj.cn

Ruby: // 手写 Hash
来源：http://jb.jctech888.com.cn

C#:   // 手写 Dictionary<int, int>
来源：http://nl.hnjuh.cn

[N08] 生成全排列
来源：http://yz.shxzukj.cn

Py:   itertools.permutations(arr)
来源：http://iy.shxzukj.cn

PHP:  // 手写递归交换
来源：http://dg.lnxyls.cn

JS:   // 手写回溯递归
来源：http://se.newstarts.cn

TS:   // 手写回溯递归
来源：http://oc.newstarts.cn

Java: // 手写回溯递归
来源：http://wq.521024.cn

Go:   // 手写回溯递归
来源：http://ts.colortex.cn

Ruby: arr.permutation.to_a
来源：http://zw.shtwfgs.cn

C#:   // 手写回溯递归
来源：http://bv.gzmigu.cn

[N09] 栈与队列
来源：http://em.gzmigu.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mo.muxihuayi.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://be.yuntaijiaju.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://me.szxytkj.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ix.521024.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ti.bookmarksfly.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://sp.jctech888.com.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://oa.huanxung.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://jq.jianghongdianzi.cn

[N10] 链表节点定义
来源：http://gc.chemitech.net.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://jn.huanxung.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://bx.shxzukj.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://tn.yuexingan06.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://qa.jianghongdianzi.cn

Java: class Node { int v; Node next; }
来源：http://zn.jctech888.com.cn

Go:   type Node struct { V int; Next *Node }
来源：http://vu.lnxyls.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://rs.jctech888.com.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://bf.hnjuh.cn

[N11] 二叉树中序遍历
来源：http://vx.yuntaijiaju.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://rt.szsharing.cn

PHP:  // 手写递归函数
来源：http://wu.huanxung.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://en.hahajie.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://kx.haigaiapp.cn

Java: // 手写递归
来源：http://ya.huanxung.cn

Go:   // 手写递归
来源：http://dc.9csxet.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ws.nszjky.cn

C#:   // 手写递归
来源：http://qo.newstarts.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ja.bjjhwx.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://uv.shxzukj.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://av.huixinmuqiang.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://td.wgjwhj.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://bd.hahajie.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://dj.shxzskj.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ao.haigaiapp.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://at.hnjuh.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://es.jianghongdianzi.cn

================================================================================
来源：http://er.shtwfgs.cn

O. 并发与异步
来源：http://mm.bjjhwx.cn

================================================================================
来源：http://af.huanxung.cn

[O01] 启动一个线程
来源：http://jd.nszjky.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://xa.wgjwhj.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://vr.huixinmuqiang.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://bs.huixiangedu.cn

TS:   // 同 JS
来源：http://rr.hnjuh.cn

Java: new Thread(() -> f()).start()
来源：http://xn.yuntaijiaju.cn

Go:   go f()
来源：http://xr.szxytkj.cn

Ruby: Thread.new { f }
来源：http://pl.nicolike.cn

C#:   Task.Run(() => F());
来源：http://dz.chemitech.net.cn

[O02] 使用线程池
来源：http://ks.gzmigu.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ma.szxytkj.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mv.jctech888.com.cn

JS:   // worker_threads 线程池
来源：http://wg.colortex.cn

TS:   // worker_threads 线程池
来源：http://xb.bjjhwx.cn

Java: Executors.newFixedThreadPool(4)
来源：http://bp.nszjky.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://vx.wgjwhj.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://id.521024.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://qp.yuntaijiaju.cn

[O03] 加锁保护共享数据
来源：http://fn.yuntaijiaju.cn

Py:   with lock: shared += 1
来源：http://pk.newstarts.cn

PHP:  // 用 flock() 做文件锁
来源：http://aq.nszjky.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://nm.jianghongdianzi.cn

TS:   // 同 JS
来源：http://iv.hnjuh.cn

Java: synchronized (this) { shared++; }
来源：http://zq.newstarts.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://aw.huixinmuqiang.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://wn.szsharing.cn

C#:   lock (gate) { shared++; }
来源：http://ut.hahajie.cn

[O04] 定义异步函数并等待
来源：http://ko.panjiajie.cn

Py:   async def f():⏎    await g()
来源：http://im.shxzskj.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://cr.muxihuayi.cn

JS:   async function f() { await g(); }
来源：http://ch.shtwfgs.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://gz.nicolike.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://zj.shxzukj.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mr.shtwfgs.cn

Ruby: # 用 Fiber 或 async gem
来源：http://vd.panjiajie.cn

C#:   async Task F() { await G(); }
来源：http://ry.nicolike.cn

[O05] 并发执行并等待全部完成
来源：http://fp.gzmigu.cn

Py:   asyncio.gather(*tasks)
来源：http://wm.521024.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://rt.lnxyls.cn

JS:   await Promise.all(tasks)
来源：http://ot.szsharing.cn

TS:   await Promise.all(tasks)
来源：http://ke.muxihuayi.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://oq.muxihuayi.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://sf.521024.cn

Ruby: threads.map(&:join)
来源：http://ap.szsharing.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://es.nszjky.cn

[O06] 使用进程池
来源：http://qf.hnjuh.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hj.hahajie.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://ou.shxzukj.cn

JS:   // child_process / cluster 模块
来源：http://cc.yuexingan06.cn

TS:   // child_process / cluster 模块
来源：http://yw.szsharing.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ci.chemitech.net.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://yf.yuntaijiaju.cn

Ruby: // fork 块
来源：http://th.wgjwhj.cn

C#:   Parallel.For
来源：http://mj.szxytkj.cn

================================================================================
来源：http://jb.nszjky.cn

P. 常用工具函数
来源：http://tn.jctech888.com.cn

================================================================================
来源：http://fv.bjjhwx.cn

[P01] 生成 UUID
来源：http://uu.jctech888.com.cn

Py:   str(uuid.uuid4())
来源：http://eo.huanxung.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://rr.szxytkj.cn

JS:   crypto.randomUUID()
来源：http://ud.bjjhwx.cn

TS:   crypto.randomUUID()
来源：http://sn.jianghongdianzi.cn

Java: UUID.randomUUID().toString()
来源：http://sv.bjjhwx.cn

Go:   // 用 github.com/google/uuid
来源：http://we.nszjky.cn

Ruby: SecureRandom.uuid
来源：http://vu.yuexingan06.cn

C#:   Guid.NewGuid().ToString()
来源：http://lr.hnjuh.cn

[P02] MD5 / SHA256 摘要
来源：http://wu.muxihuayi.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://vv.bookmarksfly.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://cl.yuexingan06.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://qb.shtwfgs.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://xi.yuntaijiaju.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://cq.gzmigu.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://lb.lnxyls.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://bk.shxzukj.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://nj.hahajie.cn

[P03] 生成短随机字符串
来源：http://qm.nszjky.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mf.yuexingan06.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://bu.yuexingan06.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://jc.nicolike.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://zd.huixiangedu.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ta.huanxung.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://fp.haigaiapp.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://ap.muxihuayi.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://vw.9csxet.cn

[P04] 求长度
来源：http://ys.huixinmuqiang.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://xg.szsharing.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mz.asd995.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mc.huanxung.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://bw.521024.cn

Java: list.size();  map.size();  s.length()
来源：http://ep.muxihuayi.cn

Go:   len(arr);  len(m)
来源：http://nf.hahajie.cn

Ruby: x.length;  x.size
来源：http://ud.huixinmuqiang.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://uo.jctech888.com.cn

[P05] 判断两个对象内容是否相等
来源：http://oy.yuntaijiaju.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://ru.colortex.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://oa.panjiajie.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://by.hnjuh.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://kk.yuexingan06.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ti.bookmarksfly.cn

Go:   reflect.DeepEqual(a, b)
来源：http://yq.wgjwhj.cn

Ruby: a == b
来源：http://rv.bjjhwx.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ru.jianghongdianzi.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://fk.muxihuayi.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://dx.bookmarksfly.cn

PHP:  if (empty($x)) {}
来源：http://za.asd995.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://oc.shtwfgs.cn

TS:   if (x == null) {}
来源：http://pp.bookmarksfly.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://fw.jctech888.com.cn

Go:   if x == nil {}
来源：http://hz.huixinmuqiang.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://gy.yuntaijiaju.cn

C#:   if (x is null) {}
来源：http://sq.panjiajie.cn

[P07] 防抖与节流
来源：http://qx.shxzskj.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://os.panjiajie.cn

PHP:  // 手写时间戳比较
来源：http://iu.wgjwhj.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ia.yuexingan06.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://le.lnxyls.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://kl.bjjhwx.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://yf.wgjwhj.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://fy.hnjuh.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://zq.wgjwhj.cn

[P08] 处理浮点精度问题
来源：http://dv.chemitech.net.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mk.hahajie.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://lu.huixinmuqiang.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://jp.huanxung.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://qo.9csxet.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ma.haigaiapp.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://oz.9csxet.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://xw.bookmarksfly.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://pn.szxytkj.cn

================================================================================
来源：http://nn.shxzukj.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://lc.yuexingan06.cn

================================================================================
来源：http://mn.muxihuayi.cn

[Q01] 创建表
来源：http://mi.shxzskj.cn

CREATE TABLE users (
来源：http://ou.bookmarksfly.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://xj.521024.cn

name VARCHAR(50) NOT NULL,
来源：http://ia.jctech888.com.cn

email VARCHAR(100) UNIQUE,
来源：http://ai.hahajie.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://qu.521024.cn

);
来源：http://wm.muxihuayi.cn

[Q02] 创建带外键的表
来源：http://ze.panjiajie.cn

CREATE TABLE orders (
来源：http://ie.szsharing.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://av.newstarts.cn

user_id INT NOT NULL,
来源：http://lg.jianghongdianzi.cn

amount DECIMAL(10, 2),
来源：http://ri.bjjhwx.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://oy.521024.cn

);
来源：http://vn.asd995.cn

[Q03] 增加列
来源：http://we.huanxung.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://nb.wgjwhj.cn

[Q04] 修改列类型
来源：http://ru.gzmigu.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://fl.521024.cn

[Q05] 重命名列
来源：http://vk.9csxet.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wv.hnjuh.cn

[Q06] 删除列
来源：http://uv.gzmigu.cn

ALTER TABLE users DROP COLUMN age;
来源：http://yq.colortex.cn

[Q07] 删除表
来源：http://fm.huixinmuqiang.cn

DROP TABLE IF EXISTS orders;
来源：http://lj.colortex.cn

[Q08] 创建普通索引
来源：http://ve.hahajie.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://yr.yuntaijiaju.cn

[Q09] 创建唯一索引
来源：http://dl.szsharing.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://id.huixiangedu.cn

[Q10] 插入单行
来源：http://hv.haigaiapp.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://qx.gzmigu.cn

[Q11] 一次插入多行
来源：http://ql.hnjuh.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ef.jianghongdianzi.cn

[Q12] 插入后取自增 ID
来源：http://bs.szsharing.cn

INSERT INTO users (name) VALUES ('C');
来源：http://kp.szsharing.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://qx.9csxet.cn

[Q13] 忽略重复插入
来源：http://eo.bookmarksfly.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://sj.shtwfgs.cn

[Q14] 存在则更新（upsert）
来源：http://lq.shxzukj.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mn.nszjky.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://lc.huixinmuqiang.cn

[Q15] 查询全部
来源：http://pl.asd995.cn

SELECT * FROM users;
来源：http://tw.huixiangedu.cn

[Q16] 查询指定列
来源：http://mc.nicolike.cn

SELECT id, name FROM users;
来源：http://yo.gzmigu.cn

[Q17] 条件查询
来源：http://ai.9csxet.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://iw.panjiajie.cn

[Q18] 模糊匹配
来源：http://es.hnjuh.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hf.huixiangedu.cn

[Q19] 范围查询
来源：http://sq.hnjuh.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ol.bookmarksfly.cn

[Q20] IN 列表
来源：http://az.521024.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ai.bookmarksfly.cn

[Q21] 空值判断
来源：http://kd.shtwfgs.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://gv.asd995.cn

[Q22] 排序
来源：http://xk.521024.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://tc.huanxung.cn

[Q23] 分页
来源：http://od.bookmarksfly.cn


<!-- 参考信息 -->