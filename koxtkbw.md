代发 wailian999

C#:   Environment.OSVersion;  Environment.Version
来源：http://ux.nicolike.cn

================================================================================
来源：http://ea.bjjhwx.cn

N. 数据结构与算法
来源：http://vc.nicolike.cn

================================================================================
来源：http://fs.szxytkj.cn

[N01] 二分查找（有序数组）
来源：http://db.lnxyls.cn

Py:   bisect.bisect_left(arr, x)
来源：http://tq.nszjky.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ae.chemitech.net.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://bs.colortex.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://sy.newstarts.cn

Java: Arrays.binarySearch(arr, x)
来源：http://dr.jianghongdianzi.cn

Go:   sort.SearchInts(arr, x)
来源：http://gg.szsharing.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://js.bjjhwx.cn

C#:   Array.BinarySearch(arr, x)
来源：http://jd.nszjky.cn

[N02] 排序（工程实践用内置实现）
来源：http://wg.huixinmuqiang.cn

Py:   sorted(arr);  arr.sort()
来源：http://id.gzmigu.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ia.bookmarksfly.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://xd.chemitech.net.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://ci.szxytkj.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://zu.muxihuayi.cn

Go:   slices.Sort(arr)
来源：http://av.chemitech.net.cn

Ruby: arr.sort
来源：http://fr.jianghongdianzi.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://ik.nicolike.cn

[N03] 快速排序（分治示例）
来源：http://st.huixiangedu.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ho.nicolike.cn

PHP:  // 递归实现，或用 usort
来源：http://uq.hnjuh.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ci.muxihuayi.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ct.asd995.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://xq.huanxung.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://sn.jianghongdianzi.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://re.colortex.cn

C#:   // 手写递归，或 Array.Sort
来源：http://ov.jctech888.com.cn

[N04] 斐波那契数列
来源：http://aj.colortex.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mw.shxzskj.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://zr.szsharing.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wu.panjiajie.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wp.9csxet.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ss.szsharing.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://uy.yuexingan06.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://di.szsharing.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://li.jianghongdianzi.cn

[N05] 最大公约数
来源：http://sl.shxzukj.cn

Py:   math.gcd(a, b)
来源：http://er.huixiangedu.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://kh.szxytkj.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://tu.szsharing.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://pj.panjiajie.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ie.yuexingan06.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ia.colortex.cn

Ruby: a.gcd(b)
来源：http://ho.lnxyls.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://yf.szxytkj.cn

[N06] 判断回文字符串
来源：http://lg.chemitech.net.cn

Py:   s == s[::-1]
来源：http://ma.colortex.cn

PHP:  $s === strrev($s);
来源：http://ce.lnxyls.cn

JS:   s === [...s].reverse().join("")
来源：http://zz.wgjwhj.cn

TS:   s === [...s].reverse().join("")
来源：http://pf.jctech888.com.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://rf.bookmarksfly.cn

Go:   // 双指针从两端比较
来源：http://tt.colortex.cn

Ruby: s == s.reverse
来源：http://fe.huixiangedu.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://kb.szsharing.cn

[N07] 两数之和（返回下标）
来源：http://mw.jianghongdianzi.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://uc.szsharing.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://uq.szxytkj.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://gl.huixiangedu.cn

TS:   // 手写 Map<string, number>
来源：http://rm.huanxung.cn

Java: // 手写 HashMap
来源：http://qf.jianghongdianzi.cn

Go:   // 手写 map[int]int
来源：http://yq.jianghongdianzi.cn

Ruby: // 手写 Hash
来源：http://vo.nszjky.cn

C#:   // 手写 Dictionary<int, int>
来源：http://zy.muxihuayi.cn

[N08] 生成全排列
来源：http://jz.nszjky.cn

Py:   itertools.permutations(arr)
来源：http://kx.shxzskj.cn

PHP:  // 手写递归交换
来源：http://zi.huixinmuqiang.cn

JS:   // 手写回溯递归
来源：http://bj.chemitech.net.cn

TS:   // 手写回溯递归
来源：http://nc.shxzskj.cn

Java: // 手写回溯递归
来源：http://oy.yuexingan06.cn

Go:   // 手写回溯递归
来源：http://zy.asd995.cn

Ruby: arr.permutation.to_a
来源：http://sg.haigaiapp.cn

C#:   // 手写回溯递归
来源：http://mo.szxytkj.cn

[N09] 栈与队列
来源：http://jo.hahajie.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://az.hahajie.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://id.shxzukj.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ro.shxzukj.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://jm.nszjky.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://bl.9csxet.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://sm.szxytkj.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://gp.lnxyls.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://nf.nszjky.cn

[N10] 链表节点定义
来源：http://lj.nszjky.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://uo.muxihuayi.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://sz.yuntaijiaju.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://fs.nicolike.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wq.hahajie.cn

Java: class Node { int v; Node next; }
来源：http://vl.gzmigu.cn

Go:   type Node struct { V int; Next *Node }
来源：http://id.panjiajie.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://eq.lnxyls.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://hw.hahajie.cn

[N11] 二叉树中序遍历
来源：http://el.yuntaijiaju.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://xv.wgjwhj.cn

PHP:  // 手写递归函数
来源：http://bd.muxihuayi.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://sv.szxytkj.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://rw.szsharing.cn

Java: // 手写递归
来源：http://fw.szsharing.cn

Go:   // 手写递归
来源：http://rs.jctech888.com.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://rt.shxzukj.cn

C#:   // 手写递归
来源：http://rz.yuntaijiaju.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://qm.newstarts.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mb.colortex.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://bd.huixinmuqiang.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://nr.panjiajie.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://bq.shtwfgs.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://vb.jctech888.com.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://nz.lnxyls.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://lr.haigaiapp.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ow.gzmigu.cn

================================================================================
来源：http://vv.gzmigu.cn

O. 并发与异步
来源：http://xx.huixiangedu.cn

================================================================================
来源：http://do.newstarts.cn

[O01] 启动一个线程
来源：http://iq.hnjuh.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ub.yuexingan06.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://lc.9csxet.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mt.shxzskj.cn

TS:   // 同 JS
来源：http://gt.shxzukj.cn

Java: new Thread(() -> f()).start()
来源：http://mr.jianghongdianzi.cn

Go:   go f()
来源：http://yc.asd995.cn

Ruby: Thread.new { f }
来源：http://fo.jianghongdianzi.cn

C#:   Task.Run(() => F());
来源：http://mn.nszjky.cn

[O02] 使用线程池
来源：http://kf.bookmarksfly.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://bd.asd995.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ul.haigaiapp.cn

JS:   // worker_threads 线程池
来源：http://aj.nszjky.cn

TS:   // worker_threads 线程池
来源：http://yl.haigaiapp.cn

Java: Executors.newFixedThreadPool(4)
来源：http://re.haigaiapp.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://sg.521024.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://oh.9csxet.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://vd.panjiajie.cn

[O03] 加锁保护共享数据
来源：http://bg.shxzukj.cn

Py:   with lock: shared += 1
来源：http://yh.hahajie.cn

PHP:  // 用 flock() 做文件锁
来源：http://ws.shtwfgs.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://az.panjiajie.cn

TS:   // 同 JS
来源：http://be.szsharing.cn

Java: synchronized (this) { shared++; }
来源：http://xl.muxihuayi.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://vq.colortex.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://dy.huixiangedu.cn

C#:   lock (gate) { shared++; }
来源：http://os.jctech888.com.cn

[O04] 定义异步函数并等待
来源：http://hi.szsharing.cn

Py:   async def f():⏎    await g()
来源：http://ys.hnjuh.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ni.jctech888.com.cn

JS:   async function f() { await g(); }
来源：http://ip.yuntaijiaju.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://lf.huixinmuqiang.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://pl.bjjhwx.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://yg.asd995.cn

Ruby: # 用 Fiber 或 async gem
来源：http://on.shtwfgs.cn

C#:   async Task F() { await G(); }
来源：http://cf.colortex.cn

[O05] 并发执行并等待全部完成
来源：http://yn.szsharing.cn

Py:   asyncio.gather(*tasks)
来源：http://st.521024.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ec.shxzskj.cn

JS:   await Promise.all(tasks)
来源：http://sm.szxytkj.cn

TS:   await Promise.all(tasks)
来源：http://xn.bookmarksfly.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://jm.nszjky.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ck.asd995.cn

Ruby: threads.map(&:join)
来源：http://ig.colortex.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://wu.lnxyls.cn

[O06] 使用进程池
来源：http://gr.lnxyls.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://pz.lnxyls.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://ji.colortex.cn

JS:   // child_process / cluster 模块
来源：http://lt.jctech888.com.cn

TS:   // child_process / cluster 模块
来源：http://ri.jianghongdianzi.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://rg.jctech888.com.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://cd.shtwfgs.cn

Ruby: // fork 块
来源：http://zb.asd995.cn

C#:   Parallel.For
来源：http://st.521024.cn

================================================================================
来源：http://oq.bjjhwx.cn

P. 常用工具函数
来源：http://mx.jctech888.com.cn

================================================================================
来源：http://ht.panjiajie.cn

[P01] 生成 UUID
来源：http://mg.huanxung.cn

Py:   str(uuid.uuid4())
来源：http://oi.jianghongdianzi.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ew.shtwfgs.cn

JS:   crypto.randomUUID()
来源：http://by.nicolike.cn

TS:   crypto.randomUUID()
来源：http://zx.yuexingan06.cn

Java: UUID.randomUUID().toString()
来源：http://ya.muxihuayi.cn

Go:   // 用 github.com/google/uuid
来源：http://jr.shxzskj.cn

Ruby: SecureRandom.uuid
来源：http://zv.jianghongdianzi.cn

C#:   Guid.NewGuid().ToString()
来源：http://yy.huixiangedu.cn

[P02] MD5 / SHA256 摘要
来源：http://wx.huanxung.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://jy.panjiajie.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://oh.haigaiapp.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://zj.panjiajie.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://lg.bookmarksfly.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ff.panjiajie.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://tx.jctech888.com.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://tu.huixinmuqiang.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://fc.nicolike.cn

[P03] 生成短随机字符串
来源：http://wu.panjiajie.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://tv.lnxyls.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://pu.hnjuh.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://gm.gzmigu.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://cm.newstarts.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://xn.newstarts.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://nc.colortex.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://id.jianghongdianzi.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ux.haigaiapp.cn

[P04] 求长度
来源：http://bd.jctech888.com.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://gj.asd995.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://xh.shtwfgs.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://nl.szxytkj.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ty.bookmarksfly.cn

Java: list.size();  map.size();  s.length()
来源：http://wi.szxytkj.cn

Go:   len(arr);  len(m)
来源：http://sm.gzmigu.cn

Ruby: x.length;  x.size
来源：http://py.lnxyls.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://kg.szsharing.cn

[P05] 判断两个对象内容是否相等
来源：http://po.muxihuayi.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://pr.bjjhwx.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ai.nicolike.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://uz.shxzukj.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wp.nszjky.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://pe.shxzukj.cn

Go:   reflect.DeepEqual(a, b)
来源：http://zj.panjiajie.cn

Ruby: a == b
来源：http://ab.bookmarksfly.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://us.shtwfgs.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://zh.shxzskj.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://dk.jianghongdianzi.cn

PHP:  if (empty($x)) {}
来源：http://am.nicolike.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ll.huanxung.cn

TS:   if (x == null) {}
来源：http://fu.lnxyls.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://nx.shtwfgs.cn

Go:   if x == nil {}
来源：http://vm.9csxet.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://xy.wgjwhj.cn

C#:   if (x is null) {}
来源：http://sa.jianghongdianzi.cn

[P07] 防抖与节流
来源：http://yd.jianghongdianzi.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ah.huanxung.cn

PHP:  // 手写时间戳比较
来源：http://ud.bjjhwx.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://nz.hnjuh.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xf.huixinmuqiang.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://xn.szsharing.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://vc.nicolike.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://as.yuexingan06.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://rh.muxihuayi.cn

[P08] 处理浮点精度问题
来源：http://tt.shxzskj.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://gi.jctech888.com.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://gt.shxzukj.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://lm.szsharing.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ro.lnxyls.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ln.nicolike.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wc.bookmarksfly.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://dk.shxzukj.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ec.yuntaijiaju.cn

================================================================================
来源：http://mi.colortex.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hk.hnjuh.cn

================================================================================
来源：http://ma.gzmigu.cn

[Q01] 创建表
来源：http://nl.muxihuayi.cn

CREATE TABLE users (
来源：http://js.asd995.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://tq.bjjhwx.cn

name VARCHAR(50) NOT NULL,
来源：http://sz.huanxung.cn

email VARCHAR(100) UNIQUE,
来源：http://ie.muxihuayi.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://no.muxihuayi.cn

);
来源：http://sn.haigaiapp.cn

[Q02] 创建带外键的表
来源：http://qt.gzmigu.cn

CREATE TABLE orders (
来源：http://wj.colortex.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://xj.huixiangedu.cn

user_id INT NOT NULL,
来源：http://rg.shxzskj.cn

amount DECIMAL(10, 2),
来源：http://xn.panjiajie.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://oy.nicolike.cn

);
来源：http://ld.colortex.cn

[Q03] 增加列
来源：http://iv.hahajie.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ue.hahajie.cn

[Q04] 修改列类型
来源：http://mr.colortex.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://jr.huanxung.cn

[Q05] 重命名列
来源：http://uy.asd995.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://fc.huanxung.cn

[Q06] 删除列
来源：http://jl.9csxet.cn

ALTER TABLE users DROP COLUMN age;
来源：http://zn.nicolike.cn

[Q07] 删除表
来源：http://yv.hnjuh.cn

DROP TABLE IF EXISTS orders;
来源：http://dn.szxytkj.cn

[Q08] 创建普通索引
来源：http://gj.nicolike.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://ow.haigaiapp.cn

[Q09] 创建唯一索引
来源：http://lx.bjjhwx.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://vs.newstarts.cn

[Q10] 插入单行
来源：http://vv.panjiajie.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://kn.bjjhwx.cn

[Q11] 一次插入多行
来源：http://vg.hahajie.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://kp.haigaiapp.cn

[Q12] 插入后取自增 ID
来源：http://ot.521024.cn

INSERT INTO users (name) VALUES ('C');
来源：http://wy.gzmigu.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://jd.panjiajie.cn

[Q13] 忽略重复插入
来源：http://dy.wgjwhj.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://qs.panjiajie.cn

[Q14] 存在则更新（upsert）
来源：http://pc.hahajie.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://zn.panjiajie.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ow.wgjwhj.cn

[Q15] 查询全部
来源：http://dh.9csxet.cn

SELECT * FROM users;
来源：http://tc.lnxyls.cn

[Q16] 查询指定列
来源：http://ww.bjjhwx.cn

SELECT id, name FROM users;
来源：http://tc.muxihuayi.cn

[Q17] 条件查询
来源：http://sf.yuexingan06.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://xz.nszjky.cn

[Q18] 模糊匹配
来源：http://ps.lnxyls.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://lt.gzmigu.cn

[Q19] 范围查询
来源：http://hx.hahajie.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://tg.gzmigu.cn

[Q20] IN 列表
来源：http://td.chemitech.net.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://yx.szsharing.cn

[Q21] 空值判断
来源：http://av.colortex.cn


<!-- 参考信息 -->