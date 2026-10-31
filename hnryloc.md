代发 wailian999

[N01] 二分查找（有序数组）
来源：http://oc.huixinmuqiang.cn

Py:   bisect.bisect_left(arr, x)
来源：http://an.colortex.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ny.9csxet.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ot.asd995.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ld.panjiajie.cn

Java: Arrays.binarySearch(arr, x)
来源：http://qd.9csxet.cn

Go:   sort.SearchInts(arr, x)
来源：http://pb.chemitech.net.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://ut.huanxung.cn

C#:   Array.BinarySearch(arr, x)
来源：http://bs.huixiangedu.cn

[N02] 排序（工程实践用内置实现）
来源：http://yf.szsharing.cn

Py:   sorted(arr);  arr.sort()
来源：http://dm.jctech888.com.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://bm.shxzukj.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://vh.newstarts.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://zo.nicolike.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://nd.hnjuh.cn

Go:   slices.Sort(arr)
来源：http://em.haigaiapp.cn

Ruby: arr.sort
来源：http://av.shtwfgs.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://jk.chemitech.net.cn

[N03] 快速排序（分治示例）
来源：http://jl.nicolike.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://is.huixinmuqiang.cn

PHP:  // 递归实现，或用 usort
来源：http://kd.hnjuh.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://yv.hahajie.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://es.muxihuayi.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://bd.lnxyls.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://rm.panjiajie.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wm.jctech888.com.cn

C#:   // 手写递归，或 Array.Sort
来源：http://aw.nszjky.cn

[N04] 斐波那契数列
来源：http://fc.colortex.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://dh.jctech888.com.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://um.521024.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://nj.yuexingan06.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://pe.huixiangedu.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ra.yuntaijiaju.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ss.huanxung.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://lg.yuexingan06.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://rf.bookmarksfly.cn

[N05] 最大公约数
来源：http://bn.lnxyls.cn

Py:   math.gcd(a, b)
来源：http://ed.szxytkj.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ir.jianghongdianzi.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://xh.yuexingan06.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://jf.hahajie.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://rv.shxzskj.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wk.huanxung.cn

Ruby: a.gcd(b)
来源：http://tk.yuexingan06.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://xr.yuexingan06.cn

[N06] 判断回文字符串
来源：http://dv.huanxung.cn

Py:   s == s[::-1]
来源：http://oq.nszjky.cn

PHP:  $s === strrev($s);
来源：http://wj.wgjwhj.cn

JS:   s === [...s].reverse().join("")
来源：http://bf.newstarts.cn

TS:   s === [...s].reverse().join("")
来源：http://ml.nicolike.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ns.bookmarksfly.cn

Go:   // 双指针从两端比较
来源：http://ur.yuntaijiaju.cn

Ruby: s == s.reverse
来源：http://wk.bookmarksfly.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://zu.bookmarksfly.cn

[N07] 两数之和（返回下标）
来源：http://gh.huixiangedu.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://na.szsharing.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://am.szxytkj.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://os.newstarts.cn

TS:   // 手写 Map<string, number>
来源：http://ib.hahajie.cn

Java: // 手写 HashMap
来源：http://pa.hahajie.cn

Go:   // 手写 map[int]int
来源：http://up.hnjuh.cn

Ruby: // 手写 Hash
来源：http://vq.shxzskj.cn

C#:   // 手写 Dictionary<int, int>
来源：http://gc.huixinmuqiang.cn

[N08] 生成全排列
来源：http://ln.newstarts.cn

Py:   itertools.permutations(arr)
来源：http://ud.shtwfgs.cn

PHP:  // 手写递归交换
来源：http://vd.9csxet.cn

JS:   // 手写回溯递归
来源：http://dp.bookmarksfly.cn

TS:   // 手写回溯递归
来源：http://vq.panjiajie.cn

Java: // 手写回溯递归
来源：http://qs.huanxung.cn

Go:   // 手写回溯递归
来源：http://lu.muxihuayi.cn

Ruby: arr.permutation.to_a
来源：http://jm.9csxet.cn

C#:   // 手写回溯递归
来源：http://ci.chemitech.net.cn

[N09] 栈与队列
来源：http://hx.gzmigu.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://rq.muxihuayi.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://di.chemitech.net.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ah.szsharing.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ot.hnjuh.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://vl.shtwfgs.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://dq.newstarts.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ip.szxytkj.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://fr.bjjhwx.cn

[N10] 链表节点定义
来源：http://wt.nicolike.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://kz.huixinmuqiang.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://uv.521024.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://pd.hahajie.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://jo.wgjwhj.cn

Java: class Node { int v; Node next; }
来源：http://nv.panjiajie.cn

Go:   type Node struct { V int; Next *Node }
来源：http://cm.yuexingan06.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://md.wgjwhj.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://so.wgjwhj.cn

[N11] 二叉树中序遍历
来源：http://up.9csxet.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hi.szsharing.cn

PHP:  // 手写递归函数
来源：http://sv.huixiangedu.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://vj.shtwfgs.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://np.gzmigu.cn

Java: // 手写递归
来源：http://rp.szsharing.cn

Go:   // 手写递归
来源：http://iq.colortex.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://gl.jctech888.com.cn

C#:   // 手写递归
来源：http://sd.gzmigu.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://la.colortex.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://me.huixinmuqiang.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://gt.hahajie.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://zj.huixinmuqiang.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://in.haigaiapp.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://vx.szxytkj.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://vo.hahajie.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://vi.huixinmuqiang.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ub.huixinmuqiang.cn

================================================================================
来源：http://oy.nicolike.cn

O. 并发与异步
来源：http://ek.jctech888.com.cn

================================================================================
来源：http://gl.yuntaijiaju.cn

[O01] 启动一个线程
来源：http://lg.jianghongdianzi.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://zy.muxihuayi.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wl.wgjwhj.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://co.szxytkj.cn

TS:   // 同 JS
来源：http://hm.muxihuayi.cn

Java: new Thread(() -> f()).start()
来源：http://ev.huanxung.cn

Go:   go f()
来源：http://mr.jctech888.com.cn

Ruby: Thread.new { f }
来源：http://dn.shtwfgs.cn

C#:   Task.Run(() => F());
来源：http://kz.asd995.cn

[O02] 使用线程池
来源：http://mr.521024.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://sz.9csxet.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://iu.shxzskj.cn

JS:   // worker_threads 线程池
来源：http://uu.asd995.cn

TS:   // worker_threads 线程池
来源：http://qr.shxzskj.cn

Java: Executors.newFixedThreadPool(4)
来源：http://eo.jianghongdianzi.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://js.jianghongdianzi.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://sl.huanxung.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://oa.jctech888.com.cn

[O03] 加锁保护共享数据
来源：http://dr.gzmigu.cn

Py:   with lock: shared += 1
来源：http://st.huixiangedu.cn

PHP:  // 用 flock() 做文件锁
来源：http://bt.shtwfgs.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://yp.521024.cn

TS:   // 同 JS
来源：http://me.hahajie.cn

Java: synchronized (this) { shared++; }
来源：http://wz.haigaiapp.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://me.521024.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://ys.bookmarksfly.cn

C#:   lock (gate) { shared++; }
来源：http://ws.nszjky.cn

[O04] 定义异步函数并等待
来源：http://qm.shtwfgs.cn

Py:   async def f():⏎    await g()
来源：http://ag.lnxyls.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://qe.yuntaijiaju.cn

JS:   async function f() { await g(); }
来源：http://eb.jctech888.com.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://vn.nicolike.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://be.lnxyls.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://jl.szxytkj.cn

Ruby: # 用 Fiber 或 async gem
来源：http://vg.gzmigu.cn

C#:   async Task F() { await G(); }
来源：http://nn.shxzukj.cn

[O05] 并发执行并等待全部完成
来源：http://qv.nicolike.cn

Py:   asyncio.gather(*tasks)
来源：http://rq.nszjky.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://dn.szxytkj.cn

JS:   await Promise.all(tasks)
来源：http://ns.yuexingan06.cn

TS:   await Promise.all(tasks)
来源：http://hb.yuexingan06.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wj.nicolike.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://jc.hahajie.cn

Ruby: threads.map(&:join)
来源：http://ph.hahajie.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://dp.asd995.cn

[O06] 使用进程池
来源：http://bd.szxytkj.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ob.hahajie.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://my.panjiajie.cn

JS:   // child_process / cluster 模块
来源：http://wm.huixinmuqiang.cn

TS:   // child_process / cluster 模块
来源：http://za.colortex.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ew.huixinmuqiang.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ux.panjiajie.cn

Ruby: // fork 块
来源：http://ka.jctech888.com.cn

C#:   Parallel.For
来源：http://kp.panjiajie.cn

================================================================================
来源：http://nm.wgjwhj.cn

P. 常用工具函数
来源：http://zb.9csxet.cn

================================================================================
来源：http://ht.lnxyls.cn

[P01] 生成 UUID
来源：http://jv.chemitech.net.cn

Py:   str(uuid.uuid4())
来源：http://ay.chemitech.net.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://de.colortex.cn

JS:   crypto.randomUUID()
来源：http://ah.hnjuh.cn

TS:   crypto.randomUUID()
来源：http://rr.bjjhwx.cn

Java: UUID.randomUUID().toString()
来源：http://tr.newstarts.cn

Go:   // 用 github.com/google/uuid
来源：http://jz.panjiajie.cn

Ruby: SecureRandom.uuid
来源：http://ki.asd995.cn

C#:   Guid.NewGuid().ToString()
来源：http://vk.jianghongdianzi.cn

[P02] MD5 / SHA256 摘要
来源：http://yl.wgjwhj.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://tc.chemitech.net.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://hv.huanxung.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://aa.521024.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wx.haigaiapp.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ar.chemitech.net.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://se.shtwfgs.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://lp.bookmarksfly.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://da.hnjuh.cn

[P03] 生成短随机字符串
来源：http://aq.gzmigu.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://zz.haigaiapp.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://rz.panjiajie.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ui.nszjky.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://te.chemitech.net.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wz.bjjhwx.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://xa.szxytkj.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://aa.huanxung.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://if.nicolike.cn

[P04] 求长度
来源：http://sp.haigaiapp.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ke.panjiajie.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://to.haigaiapp.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://nw.hnjuh.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://er.huanxung.cn

Java: list.size();  map.size();  s.length()
来源：http://lm.chemitech.net.cn

Go:   len(arr);  len(m)
来源：http://cv.huixinmuqiang.cn

Ruby: x.length;  x.size
来源：http://tf.bookmarksfly.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://yl.521024.cn

[P05] 判断两个对象内容是否相等
来源：http://pe.lnxyls.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://dl.521024.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wn.shxzskj.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://he.shtwfgs.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://fs.yuntaijiaju.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ks.muxihuayi.cn

Go:   reflect.DeepEqual(a, b)
来源：http://ts.jctech888.com.cn

Ruby: a == b
来源：http://cs.gzmigu.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://by.nszjky.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://kc.wgjwhj.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ix.bjjhwx.cn

PHP:  if (empty($x)) {}
来源：http://zv.huixiangedu.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://vj.wgjwhj.cn

TS:   if (x == null) {}
来源：http://nv.hahajie.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://sl.9csxet.cn

Go:   if x == nil {}
来源：http://yf.gzmigu.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://id.colortex.cn

C#:   if (x is null) {}
来源：http://dt.nicolike.cn

[P07] 防抖与节流
来源：http://wz.asd995.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://fa.wgjwhj.cn

PHP:  // 手写时间戳比较
来源：http://ub.chemitech.net.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://fs.chemitech.net.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.newstarts.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://dp.bjjhwx.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://vs.chemitech.net.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://mt.yuntaijiaju.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://cv.chemitech.net.cn

[P08] 处理浮点精度问题
来源：http://el.yuexingan06.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://kd.szsharing.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wq.jianghongdianzi.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://vq.panjiajie.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://th.lnxyls.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://vc.haigaiapp.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://sj.shtwfgs.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://lb.szxytkj.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://tv.newstarts.cn

================================================================================
来源：http://fr.wgjwhj.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://at.lnxyls.cn

================================================================================
来源：http://ae.szsharing.cn

[Q01] 创建表
来源：http://gj.lnxyls.cn

CREATE TABLE users (
来源：http://ts.nicolike.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mq.gzmigu.cn

name VARCHAR(50) NOT NULL,
来源：http://jb.wgjwhj.cn

email VARCHAR(100) UNIQUE,
来源：http://im.huixiangedu.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://se.shtwfgs.cn

);
来源：http://xj.nicolike.cn

[Q02] 创建带外键的表
来源：http://ie.panjiajie.cn

CREATE TABLE orders (
来源：http://yo.szxytkj.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://zd.9csxet.cn

user_id INT NOT NULL,
来源：http://jh.szsharing.cn

amount DECIMAL(10, 2),
来源：http://ba.hahajie.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://xy.huanxung.cn

);
来源：http://le.bjjhwx.cn

[Q03] 增加列
来源：http://tk.bjjhwx.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://pl.asd995.cn

[Q04] 修改列类型
来源：http://jc.bjjhwx.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://nu.panjiajie.cn

[Q05] 重命名列
来源：http://lb.yuntaijiaju.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://zd.colortex.cn

[Q06] 删除列
来源：http://cl.huixiangedu.cn

ALTER TABLE users DROP COLUMN age;
来源：http://sf.muxihuayi.cn

[Q07] 删除表
来源：http://lq.hnjuh.cn

DROP TABLE IF EXISTS orders;
来源：http://dh.huixinmuqiang.cn

[Q08] 创建普通索引
来源：http://jn.wgjwhj.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://bj.asd995.cn

[Q09] 创建唯一索引
来源：http://hm.shxzukj.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://do.huixiangedu.cn

[Q10] 插入单行
来源：http://fr.huixinmuqiang.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://sp.9csxet.cn

[Q11] 一次插入多行
来源：http://qe.huixinmuqiang.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://nn.colortex.cn

[Q12] 插入后取自增 ID
来源：http://ck.szsharing.cn

INSERT INTO users (name) VALUES ('C');
来源：http://df.haigaiapp.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://nk.shtwfgs.cn

[Q13] 忽略重复插入
来源：http://ju.asd995.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://gq.shtwfgs.cn

[Q14] 存在则更新（upsert）
来源：http://yc.hnjuh.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://yu.gzmigu.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://uu.muxihuayi.cn

[Q15] 查询全部
来源：http://go.muxihuayi.cn

SELECT * FROM users;
来源：http://hm.panjiajie.cn

[Q16] 查询指定列
来源：http://ps.yuntaijiaju.cn

SELECT id, name FROM users;
来源：http://fv.szxytkj.cn

[Q17] 条件查询
来源：http://jq.jianghongdianzi.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ad.bookmarksfly.cn

[Q18] 模糊匹配
来源：http://en.hnjuh.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hr.shxzskj.cn

[Q19] 范围查询
来源：http://bj.wgjwhj.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ut.9csxet.cn

[Q20] IN 列表
来源：http://dp.huanxung.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://dk.muxihuayi.cn

[Q21] 空值判断
来源：http://sd.bjjhwx.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://iy.hnjuh.cn

[Q22] 排序
来源：http://jo.huixinmuqiang.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hl.hnjuh.cn

[Q23] 分页
来源：http://bb.yuntaijiaju.cn


<!-- 参考信息 -->