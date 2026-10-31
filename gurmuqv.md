代发 wailian999

[N01] 二分查找（有序数组）
来源：http://jp.szsharing.cn

Py:   bisect.bisect_left(arr, x)
来源：http://lj.asd995.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mj.huixiangedu.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://lz.gzmigu.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://bo.9csxet.cn

Java: Arrays.binarySearch(arr, x)
来源：http://nd.huixiangedu.cn

Go:   sort.SearchInts(arr, x)
来源：http://ex.yuntaijiaju.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://xy.jctech888.com.cn

C#:   Array.BinarySearch(arr, x)
来源：http://uo.jctech888.com.cn

[N02] 排序（工程实践用内置实现）
来源：http://cu.jctech888.com.cn

Py:   sorted(arr);  arr.sort()
来源：http://ea.szxytkj.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://md.nszjky.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://ms.szsharing.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://zf.shtwfgs.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ar.shtwfgs.cn

Go:   slices.Sort(arr)
来源：http://dm.gzmigu.cn

Ruby: arr.sort
来源：http://is.9csxet.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://yw.521024.cn

[N03] 快速排序（分治示例）
来源：http://et.shxzskj.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://zs.haigaiapp.cn

PHP:  // 递归实现，或用 usort
来源：http://wt.panjiajie.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://qv.haigaiapp.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ba.yuntaijiaju.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://da.shxzukj.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://xn.haigaiapp.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://nh.9csxet.cn

C#:   // 手写递归，或 Array.Sort
来源：http://go.szsharing.cn

[N04] 斐波那契数列
来源：http://qe.lnxyls.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://jy.huixiangedu.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://rh.yuntaijiaju.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mm.nszjky.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://gg.hahajie.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://uh.bjjhwx.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://fq.huixiangedu.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://xs.9csxet.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://vq.huixinmuqiang.cn

[N05] 最大公约数
来源：http://xs.panjiajie.cn

Py:   math.gcd(a, b)
来源：http://fy.colortex.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ax.chemitech.net.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://gw.jianghongdianzi.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://px.huixiangedu.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://eg.panjiajie.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ir.yuexingan06.cn

Ruby: a.gcd(b)
来源：http://lh.shtwfgs.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://yd.bjjhwx.cn

[N06] 判断回文字符串
来源：http://jy.shxzskj.cn

Py:   s == s[::-1]
来源：http://zh.newstarts.cn

PHP:  $s === strrev($s);
来源：http://kf.nszjky.cn

JS:   s === [...s].reverse().join("")
来源：http://ko.panjiajie.cn

TS:   s === [...s].reverse().join("")
来源：http://gk.shtwfgs.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://sq.yuexingan06.cn

Go:   // 双指针从两端比较
来源：http://cs.szsharing.cn

Ruby: s == s.reverse
来源：http://vn.colortex.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://hs.huixinmuqiang.cn

[N07] 两数之和（返回下标）
来源：http://tc.lnxyls.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://vm.nszjky.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://te.521024.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://hv.szsharing.cn

TS:   // 手写 Map<string, number>
来源：http://lt.jctech888.com.cn

Java: // 手写 HashMap
来源：http://tf.hahajie.cn

Go:   // 手写 map[int]int
来源：http://mz.yuntaijiaju.cn

Ruby: // 手写 Hash
来源：http://ip.colortex.cn

C#:   // 手写 Dictionary<int, int>
来源：http://cl.haigaiapp.cn

[N08] 生成全排列
来源：http://er.nicolike.cn

Py:   itertools.permutations(arr)
来源：http://ww.szxytkj.cn

PHP:  // 手写递归交换
来源：http://oi.nicolike.cn

JS:   // 手写回溯递归
来源：http://wu.shxzukj.cn

TS:   // 手写回溯递归
来源：http://ci.bookmarksfly.cn

Java: // 手写回溯递归
来源：http://jx.shxzskj.cn

Go:   // 手写回溯递归
来源：http://pl.nszjky.cn

Ruby: arr.permutation.to_a
来源：http://mk.huixiangedu.cn

C#:   // 手写回溯递归
来源：http://sf.szsharing.cn

[N09] 栈与队列
来源：http://ck.szsharing.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://bj.shtwfgs.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://vi.shxzskj.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ua.szsharing.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://rx.szxytkj.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ci.yuexingan06.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://jw.hahajie.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ss.newstarts.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://tu.bjjhwx.cn

[N10] 链表节点定义
来源：http://xd.nszjky.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ak.shxzskj.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://dm.panjiajie.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ic.szxytkj.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://et.colortex.cn

Java: class Node { int v; Node next; }
来源：http://jd.gzmigu.cn

Go:   type Node struct { V int; Next *Node }
来源：http://fr.lnxyls.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://du.shxzukj.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://sg.jctech888.com.cn

[N11] 二叉树中序遍历
来源：http://gb.huanxung.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mq.nszjky.cn

PHP:  // 手写递归函数
来源：http://rl.huanxung.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://uv.nicolike.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://sv.colortex.cn

Java: // 手写递归
来源：http://lw.newstarts.cn

Go:   // 手写递归
来源：http://xw.lnxyls.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://bs.colortex.cn

C#:   // 手写递归
来源：http://tl.521024.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wx.chemitech.net.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://jo.shxzskj.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://tm.hahajie.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ew.chemitech.net.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://kp.521024.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://lv.yuexingan06.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://qg.muxihuayi.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://fz.jianghongdianzi.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://uj.hahajie.cn

================================================================================
来源：http://oh.gzmigu.cn

O. 并发与异步
来源：http://oo.jctech888.com.cn

================================================================================
来源：http://jv.huixiangedu.cn

[O01] 启动一个线程
来源：http://xc.bjjhwx.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ed.newstarts.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://iq.colortex.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://qi.nicolike.cn

TS:   // 同 JS
来源：http://if.jctech888.com.cn

Java: new Thread(() -> f()).start()
来源：http://bw.lnxyls.cn

Go:   go f()
来源：http://ek.chemitech.net.cn

Ruby: Thread.new { f }
来源：http://jk.chemitech.net.cn

C#:   Task.Run(() => F());
来源：http://bm.huixinmuqiang.cn

[O02] 使用线程池
来源：http://pz.huixinmuqiang.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://qp.szsharing.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ef.shxzukj.cn

JS:   // worker_threads 线程池
来源：http://ja.hnjuh.cn

TS:   // worker_threads 线程池
来源：http://cp.hahajie.cn

Java: Executors.newFixedThreadPool(4)
来源：http://mz.hnjuh.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://yd.yuexingan06.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ew.asd995.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://kk.szsharing.cn

[O03] 加锁保护共享数据
来源：http://gt.newstarts.cn

Py:   with lock: shared += 1
来源：http://bo.nszjky.cn

PHP:  // 用 flock() 做文件锁
来源：http://yc.huixinmuqiang.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://kw.shxzukj.cn

TS:   // 同 JS
来源：http://fv.huanxung.cn

Java: synchronized (this) { shared++; }
来源：http://qy.9csxet.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://he.yuexingan06.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://yf.panjiajie.cn

C#:   lock (gate) { shared++; }
来源：http://ro.chemitech.net.cn

[O04] 定义异步函数并等待
来源：http://ki.hahajie.cn

Py:   async def f():⏎    await g()
来源：http://tw.huixinmuqiang.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://bj.shxzukj.cn

JS:   async function f() { await g(); }
来源：http://pe.szxytkj.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://uz.shtwfgs.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://kb.szsharing.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wa.jctech888.com.cn

Ruby: # 用 Fiber 或 async gem
来源：http://qm.521024.cn

C#:   async Task F() { await G(); }
来源：http://lg.szsharing.cn

[O05] 并发执行并等待全部完成
来源：http://ev.szsharing.cn

Py:   asyncio.gather(*tasks)
来源：http://dr.hnjuh.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://sr.jianghongdianzi.cn

JS:   await Promise.all(tasks)
来源：http://xm.jctech888.com.cn

TS:   await Promise.all(tasks)
来源：http://lj.bookmarksfly.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ul.jianghongdianzi.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://dm.nicolike.cn

Ruby: threads.map(&:join)
来源：http://fv.asd995.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://pd.colortex.cn

[O06] 使用进程池
来源：http://sm.gzmigu.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://pl.hahajie.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://tz.huanxung.cn

JS:   // child_process / cluster 模块
来源：http://qn.521024.cn

TS:   // child_process / cluster 模块
来源：http://fw.muxihuayi.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://sj.szxytkj.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wn.muxihuayi.cn

Ruby: // fork 块
来源：http://gu.gzmigu.cn

C#:   Parallel.For
来源：http://xh.szxytkj.cn

================================================================================
来源：http://yi.szxytkj.cn

P. 常用工具函数
来源：http://me.hnjuh.cn

================================================================================
来源：http://np.lnxyls.cn

[P01] 生成 UUID
来源：http://sr.muxihuayi.cn

Py:   str(uuid.uuid4())
来源：http://sj.9csxet.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://zk.shxzukj.cn

JS:   crypto.randomUUID()
来源：http://fv.hahajie.cn

TS:   crypto.randomUUID()
来源：http://mk.bookmarksfly.cn

Java: UUID.randomUUID().toString()
来源：http://go.jctech888.com.cn

Go:   // 用 github.com/google/uuid
来源：http://jo.szsharing.cn

Ruby: SecureRandom.uuid
来源：http://ay.colortex.cn

C#:   Guid.NewGuid().ToString()
来源：http://vi.bjjhwx.cn

[P02] MD5 / SHA256 摘要
来源：http://tm.yuntaijiaju.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://zx.shxzskj.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://od.jctech888.com.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://le.hahajie.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://pc.jianghongdianzi.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mv.muxihuayi.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://do.jctech888.com.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://cq.yuntaijiaju.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hi.gzmigu.cn

[P03] 生成短随机字符串
来源：http://az.jianghongdianzi.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://tm.shxzukj.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://fv.jianghongdianzi.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://dw.9csxet.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://zt.jianghongdianzi.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://zx.gzmigu.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://rl.newstarts.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://cr.shxzskj.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ca.jctech888.com.cn

[P04] 求长度
来源：http://ff.colortex.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://xt.wgjwhj.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ji.nszjky.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ho.gzmigu.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://xk.huixinmuqiang.cn

Java: list.size();  map.size();  s.length()
来源：http://gg.asd995.cn

Go:   len(arr);  len(m)
来源：http://ud.asd995.cn

Ruby: x.length;  x.size
来源：http://mw.huixinmuqiang.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://dg.9csxet.cn

[P05] 判断两个对象内容是否相等
来源：http://cc.jctech888.com.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://pk.muxihuayi.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://yy.yuntaijiaju.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ht.huanxung.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hx.jctech888.com.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ny.shxzukj.cn

Go:   reflect.DeepEqual(a, b)
来源：http://oj.bookmarksfly.cn

Ruby: a == b
来源：http://ek.hnjuh.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://aj.haigaiapp.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://gh.chemitech.net.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://af.hahajie.cn

PHP:  if (empty($x)) {}
来源：http://lr.lnxyls.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://rt.hahajie.cn

TS:   if (x == null) {}
来源：http://nr.yuntaijiaju.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://nl.bjjhwx.cn

Go:   if x == nil {}
来源：http://wo.chemitech.net.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://kb.haigaiapp.cn

C#:   if (x is null) {}
来源：http://wd.huanxung.cn

[P07] 防抖与节流
来源：http://jo.szxytkj.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://yw.haigaiapp.cn

PHP:  // 手写时间戳比较
来源：http://ri.chemitech.net.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://nu.colortex.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xe.shxzskj.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ec.shtwfgs.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://un.nicolike.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://qb.9csxet.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://sk.yuexingan06.cn

[P08] 处理浮点精度问题
来源：http://dc.yuexingan06.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://vl.gzmigu.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://zi.gzmigu.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://bm.nszjky.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://jk.gzmigu.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://xw.huixiangedu.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://lk.colortex.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://bm.yuexingan06.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hw.shxzskj.cn

================================================================================
来源：http://wf.nszjky.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ql.asd995.cn

================================================================================
来源：http://dz.lnxyls.cn

[Q01] 创建表
来源：http://ku.gzmigu.cn

CREATE TABLE users (
来源：http://jy.panjiajie.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ro.jctech888.com.cn

name VARCHAR(50) NOT NULL,
来源：http://es.panjiajie.cn

email VARCHAR(100) UNIQUE,
来源：http://zw.colortex.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://lc.bjjhwx.cn

);
来源：http://gn.wgjwhj.cn

[Q02] 创建带外键的表
来源：http://cz.hnjuh.cn

CREATE TABLE orders (
来源：http://ad.asd995.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hn.hahajie.cn

user_id INT NOT NULL,
来源：http://vm.shxzukj.cn

amount DECIMAL(10, 2),
来源：http://lk.huixinmuqiang.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://do.shtwfgs.cn

);
来源：http://ik.bjjhwx.cn

[Q03] 增加列
来源：http://mv.wgjwhj.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://oz.lnxyls.cn

[Q04] 修改列类型
来源：http://xb.szxytkj.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://rw.newstarts.cn

[Q05] 重命名列
来源：http://ij.muxihuayi.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://be.nszjky.cn

[Q06] 删除列
来源：http://jh.chemitech.net.cn

ALTER TABLE users DROP COLUMN age;
来源：http://ym.chemitech.net.cn

[Q07] 删除表
来源：http://nl.jianghongdianzi.cn

DROP TABLE IF EXISTS orders;
来源：http://yp.panjiajie.cn

[Q08] 创建普通索引
来源：http://ne.wgjwhj.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://cj.521024.cn

[Q09] 创建唯一索引
来源：http://cn.nicolike.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://fh.szxytkj.cn

[Q10] 插入单行
来源：http://zt.colortex.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://oa.huixinmuqiang.cn

[Q11] 一次插入多行
来源：http://sb.chemitech.net.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://rk.panjiajie.cn

[Q12] 插入后取自增 ID
来源：http://qm.jctech888.com.cn

INSERT INTO users (name) VALUES ('C');
来源：http://uj.muxihuayi.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://or.nicolike.cn

[Q13] 忽略重复插入
来源：http://dd.asd995.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://am.bookmarksfly.cn

[Q14] 存在则更新（upsert）
来源：http://fp.gzmigu.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wq.muxihuayi.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://my.9csxet.cn

[Q15] 查询全部
来源：http://lf.haigaiapp.cn

SELECT * FROM users;
来源：http://xm.shxzskj.cn

[Q16] 查询指定列
来源：http://xa.gzmigu.cn

SELECT id, name FROM users;
来源：http://rp.yuexingan06.cn

[Q17] 条件查询
来源：http://xg.bookmarksfly.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://lm.colortex.cn

[Q18] 模糊匹配
来源：http://lx.521024.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://po.haigaiapp.cn

[Q19] 范围查询
来源：http://vj.nszjky.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://jd.hahajie.cn

[Q20] IN 列表
来源：http://dg.lnxyls.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ys.hnjuh.cn

[Q21] 空值判断
来源：http://nb.asd995.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://ue.yuexingan06.cn

[Q22] 排序
来源：http://gj.colortex.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://yy.9csxet.cn

[Q23] 分页
来源：http://uy.huixinmuqiang.cn


<!-- 参考信息 -->