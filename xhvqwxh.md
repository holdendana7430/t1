代发 wailian999

[M08] 获取系统与运行时信息
来源：http://ai.nicolike.cn

Py:   platform.system();  platform.python_version()
来源：http://mz.nicolike.cn

PHP:  PHP_OS;  phpversion();
来源：http://te.colortex.cn

JS:   process.platform;  process.version
来源：http://pw.colortex.cn

TS:   process.platform;  process.version
来源：http://kb.huixiangedu.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.shtwfgs.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://de.asd995.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ka.asd995.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://pu.gzmigu.cn

================================================================================
来源：http://gq.huanxung.cn

N. 数据结构与算法
来源：http://wz.szsharing.cn

================================================================================
来源：http://cw.newstarts.cn

[N01] 二分查找（有序数组）
来源：http://mj.colortex.cn

Py:   bisect.bisect_left(arr, x)
来源：http://ph.huixiangedu.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://sk.nicolike.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hp.newstarts.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ey.chemitech.net.cn

Java: Arrays.binarySearch(arr, x)
来源：http://mn.jctech888.com.cn

Go:   sort.SearchInts(arr, x)
来源：http://sx.hnjuh.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://ay.jianghongdianzi.cn

C#:   Array.BinarySearch(arr, x)
来源：http://ho.jctech888.com.cn

[N02] 排序（工程实践用内置实现）
来源：http://hc.nicolike.cn

Py:   sorted(arr);  arr.sort()
来源：http://pc.yuexingan06.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://tj.szxytkj.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://zb.shxzskj.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://lj.asd995.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://aw.bookmarksfly.cn

Go:   slices.Sort(arr)
来源：http://qa.szxytkj.cn

Ruby: arr.sort
来源：http://ri.9csxet.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://xh.huixiangedu.cn

[N03] 快速排序（分治示例）
来源：http://sz.9csxet.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://jz.colortex.cn

PHP:  // 递归实现，或用 usort
来源：http://ej.yuntaijiaju.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ps.nszjky.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://bn.huixinmuqiang.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://fk.hahajie.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://jc.asd995.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://oe.asd995.cn

C#:   // 手写递归，或 Array.Sort
来源：http://xr.lnxyls.cn

[N04] 斐波那契数列
来源：http://ve.9csxet.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://zc.muxihuayi.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://kh.521024.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://vd.yuntaijiaju.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ix.hnjuh.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://lq.jianghongdianzi.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ye.huixinmuqiang.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://gr.hahajie.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://yh.muxihuayi.cn

[N05] 最大公约数
来源：http://yj.nicolike.cn

Py:   math.gcd(a, b)
来源：http://ns.colortex.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://yp.521024.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://rd.panjiajie.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://bx.colortex.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://nl.yuexingan06.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://vn.jianghongdianzi.cn

Ruby: a.gcd(b)
来源：http://sj.shtwfgs.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://gd.9csxet.cn

[N06] 判断回文字符串
来源：http://jt.panjiajie.cn

Py:   s == s[::-1]
来源：http://aq.colortex.cn

PHP:  $s === strrev($s);
来源：http://oz.lnxyls.cn

JS:   s === [...s].reverse().join("")
来源：http://ud.9csxet.cn

TS:   s === [...s].reverse().join("")
来源：http://gl.hnjuh.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://oy.jianghongdianzi.cn

Go:   // 双指针从两端比较
来源：http://me.szxytkj.cn

Ruby: s == s.reverse
来源：http://he.lnxyls.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://fu.gzmigu.cn

[N07] 两数之和（返回下标）
来源：http://ef.bookmarksfly.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://vm.hnjuh.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://xe.colortex.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://db.muxihuayi.cn

TS:   // 手写 Map<string, number>
来源：http://wp.haigaiapp.cn

Java: // 手写 HashMap
来源：http://za.lnxyls.cn

Go:   // 手写 map[int]int
来源：http://xj.hnjuh.cn

Ruby: // 手写 Hash
来源：http://ki.jianghongdianzi.cn

C#:   // 手写 Dictionary<int, int>
来源：http://tw.yuexingan06.cn

[N08] 生成全排列
来源：http://ad.yuntaijiaju.cn

Py:   itertools.permutations(arr)
来源：http://nr.asd995.cn

PHP:  // 手写递归交换
来源：http://sc.lnxyls.cn

JS:   // 手写回溯递归
来源：http://cf.hahajie.cn

TS:   // 手写回溯递归
来源：http://ce.chemitech.net.cn

Java: // 手写回溯递归
来源：http://sn.colortex.cn

Go:   // 手写回溯递归
来源：http://fj.szsharing.cn

Ruby: arr.permutation.to_a
来源：http://ai.colortex.cn

C#:   // 手写回溯递归
来源：http://fr.521024.cn

[N09] 栈与队列
来源：http://ht.newstarts.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ds.shxzskj.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://pn.gzmigu.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://tm.panjiajie.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://va.nicolike.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://xc.chemitech.net.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ta.newstarts.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://sw.wgjwhj.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://tn.bjjhwx.cn

[N10] 链表节点定义
来源：http://yc.bookmarksfly.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://xr.szxytkj.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://nw.shxzskj.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://br.9csxet.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://si.huixiangedu.cn

Java: class Node { int v; Node next; }
来源：http://ki.bjjhwx.cn

Go:   type Node struct { V int; Next *Node }
来源：http://sj.hahajie.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://wb.jianghongdianzi.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://zo.521024.cn

[N11] 二叉树中序遍历
来源：http://is.lnxyls.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://lg.muxihuayi.cn

PHP:  // 手写递归函数
来源：http://ib.huixiangedu.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ml.nicolike.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://al.szxytkj.cn

Java: // 手写递归
来源：http://no.huanxung.cn

Go:   // 手写递归
来源：http://ia.nicolike.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mb.nicolike.cn

C#:   // 手写递归
来源：http://hl.nicolike.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wf.chemitech.net.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://cw.521024.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://oy.bookmarksfly.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://bu.huixiangedu.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://au.huixinmuqiang.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://bj.bookmarksfly.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://zl.nicolike.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://uj.panjiajie.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://yr.jctech888.com.cn

================================================================================
来源：http://yl.jctech888.com.cn

O. 并发与异步
来源：http://nq.9csxet.cn

================================================================================
来源：http://uq.shxzskj.cn

[O01] 启动一个线程
来源：http://zi.bjjhwx.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://iq.lnxyls.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hr.gzmigu.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://kb.521024.cn

TS:   // 同 JS
来源：http://sq.lnxyls.cn

Java: new Thread(() -> f()).start()
来源：http://zi.lnxyls.cn

Go:   go f()
来源：http://dv.shxzskj.cn

Ruby: Thread.new { f }
来源：http://st.bjjhwx.cn

C#:   Task.Run(() => F());
来源：http://ud.hahajie.cn

[O02] 使用线程池
来源：http://nz.szsharing.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wq.yuexingan06.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://dj.hahajie.cn

JS:   // worker_threads 线程池
来源：http://ke.gzmigu.cn

TS:   // worker_threads 线程池
来源：http://mt.yuntaijiaju.cn

Java: Executors.newFixedThreadPool(4)
来源：http://fu.asd995.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://at.wgjwhj.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://kl.bookmarksfly.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://te.szxytkj.cn

[O03] 加锁保护共享数据
来源：http://lj.hahajie.cn

Py:   with lock: shared += 1
来源：http://xe.wgjwhj.cn

PHP:  // 用 flock() 做文件锁
来源：http://ru.nicolike.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ex.newstarts.cn

TS:   // 同 JS
来源：http://wm.huixinmuqiang.cn

Java: synchronized (this) { shared++; }
来源：http://ap.hahajie.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://yg.hnjuh.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://dn.gzmigu.cn

C#:   lock (gate) { shared++; }
来源：http://pc.bookmarksfly.cn

[O04] 定义异步函数并等待
来源：http://df.huixinmuqiang.cn

Py:   async def f():⏎    await g()
来源：http://ar.shxzskj.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://rr.shxzskj.cn

JS:   async function f() { await g(); }
来源：http://wp.hahajie.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://xx.lnxyls.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mx.szxytkj.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://oq.lnxyls.cn

Ruby: # 用 Fiber 或 async gem
来源：http://jw.asd995.cn

C#:   async Task F() { await G(); }
来源：http://ox.hahajie.cn

[O05] 并发执行并等待全部完成
来源：http://sb.hahajie.cn

Py:   asyncio.gather(*tasks)
来源：http://qh.huixiangedu.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://sy.jctech888.com.cn

JS:   await Promise.all(tasks)
来源：http://ou.jctech888.com.cn

TS:   await Promise.all(tasks)
来源：http://xs.wgjwhj.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://az.asd995.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ta.panjiajie.cn

Ruby: threads.map(&:join)
来源：http://ag.szsharing.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://mr.huanxung.cn

[O06] 使用进程池
来源：http://ou.hnjuh.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://kt.nicolike.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://xg.haigaiapp.cn

JS:   // child_process / cluster 模块
来源：http://fl.szxytkj.cn

TS:   // child_process / cluster 模块
来源：http://qz.huanxung.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://fl.muxihuayi.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://sh.jianghongdianzi.cn

Ruby: // fork 块
来源：http://zc.huixinmuqiang.cn

C#:   Parallel.For
来源：http://vw.szxytkj.cn

================================================================================
来源：http://ta.muxihuayi.cn

P. 常用工具函数
来源：http://oo.lnxyls.cn

================================================================================
来源：http://mr.bjjhwx.cn

[P01] 生成 UUID
来源：http://cl.9csxet.cn

Py:   str(uuid.uuid4())
来源：http://pe.9csxet.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://bx.bjjhwx.cn

JS:   crypto.randomUUID()
来源：http://ze.9csxet.cn

TS:   crypto.randomUUID()
来源：http://vg.huanxung.cn

Java: UUID.randomUUID().toString()
来源：http://il.huixiangedu.cn

Go:   // 用 github.com/google/uuid
来源：http://ib.asd995.cn

Ruby: SecureRandom.uuid
来源：http://ud.wgjwhj.cn

C#:   Guid.NewGuid().ToString()
来源：http://pl.szsharing.cn

[P02] MD5 / SHA256 摘要
来源：http://gm.bjjhwx.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://es.panjiajie.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://ef.shxzskj.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://pf.hahajie.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://yu.haigaiapp.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mt.yuexingan06.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://cy.huanxung.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://th.jctech888.com.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://vf.nicolike.cn

[P03] 生成短随机字符串
来源：http://gc.hnjuh.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://kh.nszjky.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://sc.panjiajie.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ca.shxzskj.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ki.yuntaijiaju.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://cz.colortex.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://jh.9csxet.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://gs.wgjwhj.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://kf.yuntaijiaju.cn

[P04] 求长度
来源：http://ol.shxzukj.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://cs.bookmarksfly.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://eo.nszjky.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://oe.huixiangedu.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ja.bjjhwx.cn

Java: list.size();  map.size();  s.length()
来源：http://wk.521024.cn

Go:   len(arr);  len(m)
来源：http://lk.huixinmuqiang.cn

Ruby: x.length;  x.size
来源：http://ae.huixinmuqiang.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://yt.yuexingan06.cn

[P05] 判断两个对象内容是否相等
来源：http://ql.shtwfgs.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://qx.yuexingan06.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://vi.jctech888.com.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://cj.shxzskj.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://it.newstarts.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://qo.shtwfgs.cn

Go:   reflect.DeepEqual(a, b)
来源：http://rz.panjiajie.cn

Ruby: a == b
来源：http://jh.9csxet.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://md.lnxyls.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://pg.wgjwhj.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://qh.hahajie.cn

PHP:  if (empty($x)) {}
来源：http://bm.nicolike.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://fe.huixinmuqiang.cn

TS:   if (x == null) {}
来源：http://vh.hahajie.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://uj.yuexingan06.cn

Go:   if x == nil {}
来源：http://dm.wgjwhj.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://fz.jianghongdianzi.cn

C#:   if (x is null) {}
来源：http://fu.chemitech.net.cn

[P07] 防抖与节流
来源：http://to.chemitech.net.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://uo.haigaiapp.cn

PHP:  // 手写时间戳比较
来源：http://zx.nicolike.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://sg.shxzukj.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://gx.shxzskj.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://vt.huixinmuqiang.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://cb.shxzukj.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://tb.haigaiapp.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ma.nicolike.cn

[P08] 处理浮点精度问题
来源：http://yg.shtwfgs.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ls.asd995.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://zf.muxihuayi.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://pk.gzmigu.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://sm.bjjhwx.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://sg.nszjky.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ry.chemitech.net.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://dt.nicolike.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://uy.nszjky.cn

================================================================================
来源：http://mh.hnjuh.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://nf.yuexingan06.cn

================================================================================
来源：http://mp.chemitech.net.cn

[Q01] 创建表
来源：http://ip.9csxet.cn

CREATE TABLE users (
来源：http://ub.9csxet.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://sa.hnjuh.cn

name VARCHAR(50) NOT NULL,
来源：http://lm.huixiangedu.cn

email VARCHAR(100) UNIQUE,
来源：http://ya.lnxyls.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://jq.jianghongdianzi.cn

);
来源：http://go.yuntaijiaju.cn

[Q02] 创建带外键的表
来源：http://ks.muxihuayi.cn

CREATE TABLE orders (
来源：http://is.hahajie.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://is.hahajie.cn

user_id INT NOT NULL,
来源：http://we.huixiangedu.cn

amount DECIMAL(10, 2),
来源：http://yf.huixiangedu.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://dy.hnjuh.cn

);
来源：http://mt.muxihuayi.cn

[Q03] 增加列
来源：http://hr.huanxung.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ce.jianghongdianzi.cn

[Q04] 修改列类型
来源：http://iv.9csxet.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://uw.panjiajie.cn

[Q05] 重命名列
来源：http://ux.yuntaijiaju.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://kg.panjiajie.cn

[Q06] 删除列
来源：http://yv.haigaiapp.cn

ALTER TABLE users DROP COLUMN age;
来源：http://zo.gzmigu.cn

[Q07] 删除表
来源：http://na.szxytkj.cn

DROP TABLE IF EXISTS orders;
来源：http://lu.jctech888.com.cn

[Q08] 创建普通索引
来源：http://pn.shxzukj.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://vj.521024.cn

[Q09] 创建唯一索引
来源：http://hi.bookmarksfly.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://jr.asd995.cn

[Q10] 插入单行
来源：http://pt.chemitech.net.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://np.hnjuh.cn

[Q11] 一次插入多行
来源：http://lf.huixinmuqiang.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://yg.bjjhwx.cn

[Q12] 插入后取自增 ID
来源：http://pe.szsharing.cn

INSERT INTO users (name) VALUES ('C');
来源：http://je.haigaiapp.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ev.bjjhwx.cn

[Q13] 忽略重复插入
来源：http://lg.muxihuayi.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ny.jianghongdianzi.cn

[Q14] 存在则更新（upsert）
来源：http://sq.shtwfgs.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://sf.bjjhwx.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ol.bookmarksfly.cn

[Q15] 查询全部
来源：http://de.521024.cn

SELECT * FROM users;
来源：http://ll.shxzukj.cn

[Q16] 查询指定列
来源：http://hd.muxihuayi.cn

SELECT id, name FROM users;
来源：http://ka.szxytkj.cn

[Q17] 条件查询
来源：http://xl.yuntaijiaju.cn


<!-- 参考信息 -->