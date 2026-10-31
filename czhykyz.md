代发 wailian999

[N01] 二分查找（有序数组）
来源：http://ou.shxzskj.cn

Py:   bisect.bisect_left(arr, x)
来源：http://fa.521024.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://we.jctech888.com.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://zi.newstarts.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://tw.lnxyls.cn

Java: Arrays.binarySearch(arr, x)
来源：http://by.shxzukj.cn

Go:   sort.SearchInts(arr, x)
来源：http://zl.colortex.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://fn.hahajie.cn

C#:   Array.BinarySearch(arr, x)
来源：http://bk.shxzukj.cn

[N02] 排序（工程实践用内置实现）
来源：http://ix.huixiangedu.cn

Py:   sorted(arr);  arr.sort()
来源：http://kq.huixinmuqiang.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ra.gzmigu.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://km.shxzskj.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://nq.bjjhwx.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://cp.huixinmuqiang.cn

Go:   slices.Sort(arr)
来源：http://fd.huixiangedu.cn

Ruby: arr.sort
来源：http://qm.huixinmuqiang.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://by.yuntaijiaju.cn

[N03] 快速排序（分治示例）
来源：http://ld.jianghongdianzi.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://rj.szsharing.cn

PHP:  // 递归实现，或用 usort
来源：http://yd.huixinmuqiang.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://et.hahajie.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://xs.hnjuh.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ed.shxzskj.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://aa.gzmigu.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hf.jianghongdianzi.cn

C#:   // 手写递归，或 Array.Sort
来源：http://sx.bookmarksfly.cn

[N04] 斐波那契数列
来源：http://po.hahajie.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://cs.yuexingan06.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://qa.szxytkj.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ay.nicolike.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ny.muxihuayi.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://vh.panjiajie.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wy.jctech888.com.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://er.shxzskj.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ct.hnjuh.cn

[N05] 最大公约数
来源：http://pc.huixiangedu.cn

Py:   math.gcd(a, b)
来源：http://tk.newstarts.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://dc.haigaiapp.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://qe.chemitech.net.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ua.hnjuh.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://bw.szxytkj.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wx.asd995.cn

Ruby: a.gcd(b)
来源：http://sv.jianghongdianzi.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://yp.shxzukj.cn

[N06] 判断回文字符串
来源：http://ja.nicolike.cn

Py:   s == s[::-1]
来源：http://ds.szxytkj.cn

PHP:  $s === strrev($s);
来源：http://hv.shxzukj.cn

JS:   s === [...s].reverse().join("")
来源：http://fv.colortex.cn

TS:   s === [...s].reverse().join("")
来源：http://wk.szxytkj.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://qe.shxzskj.cn

Go:   // 双指针从两端比较
来源：http://nd.hahajie.cn

Ruby: s == s.reverse
来源：http://zg.panjiajie.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://jd.huixinmuqiang.cn

[N07] 两数之和（返回下标）
来源：http://xj.jianghongdianzi.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mg.yuntaijiaju.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://nf.shtwfgs.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://xt.wgjwhj.cn

TS:   // 手写 Map<string, number>
来源：http://dy.wgjwhj.cn

Java: // 手写 HashMap
来源：http://jh.colortex.cn

Go:   // 手写 map[int]int
来源：http://kd.huanxung.cn

Ruby: // 手写 Hash
来源：http://kw.asd995.cn

C#:   // 手写 Dictionary<int, int>
来源：http://iq.huixiangedu.cn

[N08] 生成全排列
来源：http://pn.bookmarksfly.cn

Py:   itertools.permutations(arr)
来源：http://zw.bookmarksfly.cn

PHP:  // 手写递归交换
来源：http://id.huixiangedu.cn

JS:   // 手写回溯递归
来源：http://uo.hnjuh.cn

TS:   // 手写回溯递归
来源：http://gd.yuexingan06.cn

Java: // 手写回溯递归
来源：http://uf.haigaiapp.cn

Go:   // 手写回溯递归
来源：http://hi.asd995.cn

Ruby: arr.permutation.to_a
来源：http://uy.nszjky.cn

C#:   // 手写回溯递归
来源：http://ot.wgjwhj.cn

[N09] 栈与队列
来源：http://pj.muxihuayi.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://qm.shtwfgs.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mj.yuntaijiaju.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://jv.gzmigu.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ka.newstarts.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://zm.shxzukj.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://rq.szsharing.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://tr.yuntaijiaju.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ow.shxzukj.cn

[N10] 链表节点定义
来源：http://pd.colortex.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ff.colortex.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://uv.gzmigu.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hg.nszjky.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://uz.wgjwhj.cn

Java: class Node { int v; Node next; }
来源：http://je.yuntaijiaju.cn

Go:   type Node struct { V int; Next *Node }
来源：http://am.hnjuh.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://pg.haigaiapp.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://zx.shxzskj.cn

[N11] 二叉树中序遍历
来源：http://kp.colortex.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://xo.haigaiapp.cn

PHP:  // 手写递归函数
来源：http://wu.panjiajie.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://if.haigaiapp.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://zj.lnxyls.cn

Java: // 手写递归
来源：http://pr.bjjhwx.cn

Go:   // 手写递归
来源：http://zj.jianghongdianzi.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wt.bookmarksfly.cn

C#:   // 手写递归
来源：http://ww.hnjuh.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://xf.panjiajie.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://xx.9csxet.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ov.nszjky.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://gq.colortex.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://zo.bjjhwx.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ti.yuexingan06.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://rg.9csxet.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mv.shtwfgs.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://rl.jianghongdianzi.cn

================================================================================
来源：http://hn.bjjhwx.cn

O. 并发与异步
来源：http://hg.bookmarksfly.cn

================================================================================
来源：http://ka.gzmigu.cn

[O01] 启动一个线程
来源：http://pu.hnjuh.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://lu.chemitech.net.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://qn.521024.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mj.bookmarksfly.cn

TS:   // 同 JS
来源：http://dd.huanxung.cn

Java: new Thread(() -> f()).start()
来源：http://sg.bookmarksfly.cn

Go:   go f()
来源：http://rv.shtwfgs.cn

Ruby: Thread.new { f }
来源：http://jp.hnjuh.cn

C#:   Task.Run(() => F());
来源：http://on.newstarts.cn

[O02] 使用线程池
来源：http://tu.huanxung.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://cs.521024.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://aq.muxihuayi.cn

JS:   // worker_threads 线程池
来源：http://cz.nszjky.cn

TS:   // worker_threads 线程池
来源：http://in.yuntaijiaju.cn

Java: Executors.newFixedThreadPool(4)
来源：http://gp.huixiangedu.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://sv.wgjwhj.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://vz.9csxet.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ll.bjjhwx.cn

[O03] 加锁保护共享数据
来源：http://nt.hahajie.cn

Py:   with lock: shared += 1
来源：http://gz.asd995.cn

PHP:  // 用 flock() 做文件锁
来源：http://wp.hnjuh.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://db.huanxung.cn

TS:   // 同 JS
来源：http://hr.huixiangedu.cn

Java: synchronized (this) { shared++; }
来源：http://pb.szxytkj.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://lm.wgjwhj.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://bc.szsharing.cn

C#:   lock (gate) { shared++; }
来源：http://yn.jctech888.com.cn

[O04] 定义异步函数并等待
来源：http://no.shtwfgs.cn

Py:   async def f():⏎    await g()
来源：http://ob.colortex.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://bc.bookmarksfly.cn

JS:   async function f() { await g(); }
来源：http://du.huixinmuqiang.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://zh.szxytkj.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://cy.bjjhwx.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://zs.huixiangedu.cn

Ruby: # 用 Fiber 或 async gem
来源：http://ov.hnjuh.cn

C#:   async Task F() { await G(); }
来源：http://ns.521024.cn

[O05] 并发执行并等待全部完成
来源：http://ey.jianghongdianzi.cn

Py:   asyncio.gather(*tasks)
来源：http://xs.chemitech.net.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://fd.huanxung.cn

JS:   await Promise.all(tasks)
来源：http://eq.asd995.cn

TS:   await Promise.all(tasks)
来源：http://zq.nicolike.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ve.yuexingan06.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://tf.9csxet.cn

Ruby: threads.map(&:join)
来源：http://fs.panjiajie.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://sm.chemitech.net.cn

[O06] 使用进程池
来源：http://ez.9csxet.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://om.9csxet.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://bm.newstarts.cn

JS:   // child_process / cluster 模块
来源：http://rc.huixiangedu.cn

TS:   // child_process / cluster 模块
来源：http://wu.haigaiapp.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://do.haigaiapp.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wd.shxzskj.cn

Ruby: // fork 块
来源：http://zh.521024.cn

C#:   Parallel.For
来源：http://tq.haigaiapp.cn

================================================================================
来源：http://ll.yuntaijiaju.cn

P. 常用工具函数
来源：http://cb.shxzukj.cn

================================================================================
来源：http://fj.szsharing.cn

[P01] 生成 UUID
来源：http://uc.9csxet.cn

Py:   str(uuid.uuid4())
来源：http://mv.nszjky.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://au.newstarts.cn

JS:   crypto.randomUUID()
来源：http://yx.chemitech.net.cn

TS:   crypto.randomUUID()
来源：http://rg.chemitech.net.cn

Java: UUID.randomUUID().toString()
来源：http://yu.lnxyls.cn

Go:   // 用 github.com/google/uuid
来源：http://xc.yuntaijiaju.cn

Ruby: SecureRandom.uuid
来源：http://en.9csxet.cn

C#:   Guid.NewGuid().ToString()
来源：http://mu.bookmarksfly.cn

[P02] MD5 / SHA256 摘要
来源：http://zw.wgjwhj.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://zw.521024.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://jv.bjjhwx.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hs.huixiangedu.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://np.huixinmuqiang.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hp.hnjuh.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://sz.szsharing.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://jn.gzmigu.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://cz.muxihuayi.cn

[P03] 生成短随机字符串
来源：http://eu.huanxung.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://pc.hnjuh.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://fr.muxihuayi.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://eq.huixinmuqiang.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ki.bookmarksfly.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://le.haigaiapp.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://rd.nszjky.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://in.hahajie.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://uk.nszjky.cn

[P04] 求长度
来源：http://zk.hnjuh.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wg.yuntaijiaju.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://tj.szsharing.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://vu.bookmarksfly.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ov.shxzukj.cn

Java: list.size();  map.size();  s.length()
来源：http://vu.panjiajie.cn

Go:   len(arr);  len(m)
来源：http://nf.chemitech.net.cn

Ruby: x.length;  x.size
来源：http://cj.521024.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://za.gzmigu.cn

[P05] 判断两个对象内容是否相等
来源：http://vx.szxytkj.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://ln.asd995.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ph.bjjhwx.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://zw.huixinmuqiang.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://jk.colortex.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://xu.newstarts.cn

Go:   reflect.DeepEqual(a, b)
来源：http://oy.shxzskj.cn

Ruby: a == b
来源：http://om.shxzskj.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://nc.wgjwhj.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ja.yuntaijiaju.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://jz.bjjhwx.cn

PHP:  if (empty($x)) {}
来源：http://ex.bookmarksfly.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://nt.bjjhwx.cn

TS:   if (x == null) {}
来源：http://or.haigaiapp.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://id.szsharing.cn

Go:   if x == nil {}
来源：http://hw.bookmarksfly.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://vu.9csxet.cn

C#:   if (x is null) {}
来源：http://pu.jianghongdianzi.cn

[P07] 防抖与节流
来源：http://ob.wgjwhj.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ym.huanxung.cn

PHP:  // 手写时间戳比较
来源：http://ss.hnjuh.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://bm.shxzskj.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://fd.haigaiapp.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ic.hahajie.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://md.9csxet.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://pm.chemitech.net.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://gr.bookmarksfly.cn

[P08] 处理浮点精度问题
来源：http://kf.panjiajie.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://kb.bookmarksfly.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://eq.bookmarksfly.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ni.bookmarksfly.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://pu.hnjuh.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://uf.chemitech.net.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hx.newstarts.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wr.chemitech.net.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://qu.newstarts.cn

================================================================================
来源：http://mb.yuntaijiaju.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hf.jctech888.com.cn

================================================================================
来源：http://ds.panjiajie.cn

[Q01] 创建表
来源：http://qj.nszjky.cn

CREATE TABLE users (
来源：http://so.jianghongdianzi.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ge.521024.cn

name VARCHAR(50) NOT NULL,
来源：http://de.huixiangedu.cn

email VARCHAR(100) UNIQUE,
来源：http://kq.shxzskj.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://fi.hahajie.cn

);
来源：http://ac.chemitech.net.cn

[Q02] 创建带外键的表
来源：http://tp.yuexingan06.cn

CREATE TABLE orders (
来源：http://ne.nszjky.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://yf.hnjuh.cn

user_id INT NOT NULL,
来源：http://gl.jctech888.com.cn

amount DECIMAL(10, 2),
来源：http://eh.shxzskj.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://fb.shtwfgs.cn

);
来源：http://fu.colortex.cn

[Q03] 增加列
来源：http://in.asd995.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://gw.nicolike.cn

[Q04] 修改列类型
来源：http://ge.jianghongdianzi.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://fc.gzmigu.cn

[Q05] 重命名列
来源：http://ul.9csxet.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://td.szsharing.cn

[Q06] 删除列
来源：http://zw.9csxet.cn

ALTER TABLE users DROP COLUMN age;
来源：http://ug.huixiangedu.cn

[Q07] 删除表
来源：http://fq.nicolike.cn

DROP TABLE IF EXISTS orders;
来源：http://bq.521024.cn

[Q08] 创建普通索引
来源：http://eh.521024.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://bg.colortex.cn

[Q09] 创建唯一索引
来源：http://yu.9csxet.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hh.panjiajie.cn

[Q10] 插入单行
来源：http://xq.szsharing.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://tn.colortex.cn

[Q11] 一次插入多行
来源：http://rf.colortex.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://pk.huixinmuqiang.cn

[Q12] 插入后取自增 ID
来源：http://bi.panjiajie.cn

INSERT INTO users (name) VALUES ('C');
来源：http://qd.jianghongdianzi.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ap.huixiangedu.cn

[Q13] 忽略重复插入
来源：http://wl.muxihuayi.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wb.nicolike.cn

[Q14] 存在则更新（upsert）
来源：http://ah.yuntaijiaju.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://cu.asd995.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mi.jctech888.com.cn

[Q15] 查询全部
来源：http://lh.colortex.cn

SELECT * FROM users;
来源：http://nw.huixiangedu.cn

[Q16] 查询指定列
来源：http://fy.huixiangedu.cn

SELECT id, name FROM users;
来源：http://ke.lnxyls.cn

[Q17] 条件查询
来源：http://ig.haigaiapp.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wa.jianghongdianzi.cn

[Q18] 模糊匹配
来源：http://qd.shxzskj.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://kz.chemitech.net.cn

[Q19] 范围查询
来源：http://lz.shxzukj.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ph.521024.cn

[Q20] IN 列表
来源：http://df.yuexingan06.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ou.asd995.cn

[Q21] 空值判断
来源：http://pv.huixinmuqiang.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://mr.yuexingan06.cn

[Q22] 排序
来源：http://ij.yuexingan06.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://de.huixinmuqiang.cn

[Q23] 分页
来源：http://zx.haigaiapp.cn


<!-- 参考信息 -->