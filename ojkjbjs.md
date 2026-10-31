代发 wailian999

TS:   process.platform;  process.version
来源：http://zp.lnxyls.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://lo.huanxung.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://fz.szxytkj.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://dz.shxzukj.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://qj.9csxet.cn

================================================================================
来源：http://jt.haigaiapp.cn

N. 数据结构与算法
来源：http://pw.nicolike.cn

================================================================================
来源：http://sp.yuexingan06.cn

[N01] 二分查找（有序数组）
来源：http://fh.shxzukj.cn

Py:   bisect.bisect_left(arr, x)
来源：http://sq.colortex.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://gm.chemitech.net.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ho.521024.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://vg.shxzukj.cn

Java: Arrays.binarySearch(arr, x)
来源：http://qf.newstarts.cn

Go:   sort.SearchInts(arr, x)
来源：http://cu.muxihuayi.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://ig.haigaiapp.cn

C#:   Array.BinarySearch(arr, x)
来源：http://xf.nicolike.cn

[N02] 排序（工程实践用内置实现）
来源：http://us.nszjky.cn

Py:   sorted(arr);  arr.sort()
来源：http://hr.shxzskj.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://eq.521024.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://sy.muxihuayi.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://gg.muxihuayi.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wr.szxytkj.cn

Go:   slices.Sort(arr)
来源：http://bq.huixiangedu.cn

Ruby: arr.sort
来源：http://jn.jctech888.com.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://sm.shxzskj.cn

[N03] 快速排序（分治示例）
来源：http://yv.shxzskj.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://by.bjjhwx.cn

PHP:  // 递归实现，或用 usort
来源：http://ae.chemitech.net.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://gx.jianghongdianzi.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://lv.newstarts.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://gs.szxytkj.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://he.hnjuh.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://tl.szxytkj.cn

C#:   // 手写递归，或 Array.Sort
来源：http://er.huixinmuqiang.cn

[N04] 斐波那契数列
来源：http://tq.panjiajie.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://uw.shtwfgs.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://kf.hahajie.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://vb.szsharing.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://sq.panjiajie.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ck.jctech888.com.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://nl.yuntaijiaju.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://kt.521024.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://xc.nszjky.cn

[N05] 最大公约数
来源：http://yu.jianghongdianzi.cn

Py:   math.gcd(a, b)
来源：http://gb.muxihuayi.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://cx.szxytkj.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ph.nicolike.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://uv.shxzukj.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://pd.szxytkj.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://fi.newstarts.cn

Ruby: a.gcd(b)
来源：http://gh.asd995.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://so.chemitech.net.cn

[N06] 判断回文字符串
来源：http://eu.asd995.cn

Py:   s == s[::-1]
来源：http://kp.nszjky.cn

PHP:  $s === strrev($s);
来源：http://kb.huanxung.cn

JS:   s === [...s].reverse().join("")
来源：http://tc.szsharing.cn

TS:   s === [...s].reverse().join("")
来源：http://fv.bookmarksfly.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://yy.hahajie.cn

Go:   // 双指针从两端比较
来源：http://rj.newstarts.cn

Ruby: s == s.reverse
来源：http://mn.nszjky.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://zt.bookmarksfly.cn

[N07] 两数之和（返回下标）
来源：http://mv.huixiangedu.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://zj.szxytkj.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wg.wgjwhj.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://fi.shxzukj.cn

TS:   // 手写 Map<string, number>
来源：http://ks.lnxyls.cn

Java: // 手写 HashMap
来源：http://yb.nicolike.cn

Go:   // 手写 map[int]int
来源：http://cr.jctech888.com.cn

Ruby: // 手写 Hash
来源：http://jg.panjiajie.cn

C#:   // 手写 Dictionary<int, int>
来源：http://kx.bjjhwx.cn

[N08] 生成全排列
来源：http://pn.bjjhwx.cn

Py:   itertools.permutations(arr)
来源：http://jq.newstarts.cn

PHP:  // 手写递归交换
来源：http://yc.nszjky.cn

JS:   // 手写回溯递归
来源：http://je.szsharing.cn

TS:   // 手写回溯递归
来源：http://pi.szsharing.cn

Java: // 手写回溯递归
来源：http://lf.colortex.cn

Go:   // 手写回溯递归
来源：http://jp.colortex.cn

Ruby: arr.permutation.to_a
来源：http://ed.chemitech.net.cn

C#:   // 手写回溯递归
来源：http://kc.bjjhwx.cn

[N09] 栈与队列
来源：http://tx.shxzskj.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://zh.szsharing.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://xs.asd995.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://xm.huanxung.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://lx.lnxyls.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://yc.wgjwhj.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://pa.huixiangedu.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://rh.gzmigu.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://vn.nicolike.cn

[N10] 链表节点定义
来源：http://np.huixinmuqiang.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ys.jctech888.com.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://hs.bjjhwx.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wk.9csxet.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://uf.huixiangedu.cn

Java: class Node { int v; Node next; }
来源：http://an.muxihuayi.cn

Go:   type Node struct { V int; Next *Node }
来源：http://rl.huanxung.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://vo.asd995.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://dx.nszjky.cn

[N11] 二叉树中序遍历
来源：http://wo.521024.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://fs.colortex.cn

PHP:  // 手写递归函数
来源：http://xf.chemitech.net.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://as.bookmarksfly.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://lt.huixiangedu.cn

Java: // 手写递归
来源：http://pu.shxzskj.cn

Go:   // 手写递归
来源：http://gb.huixiangedu.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://uz.yuntaijiaju.cn

C#:   // 手写递归
来源：http://uw.nszjky.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://gh.szxytkj.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://gn.muxihuayi.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://tp.panjiajie.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://di.chemitech.net.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ma.hahajie.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://zy.yuexingan06.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://as.chemitech.net.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://pd.gzmigu.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://dp.muxihuayi.cn

================================================================================
来源：http://wt.huixiangedu.cn

O. 并发与异步
来源：http://mq.shxzukj.cn

================================================================================
来源：http://to.chemitech.net.cn

[O01] 启动一个线程
来源：http://oh.huanxung.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://os.yuntaijiaju.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wu.szsharing.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://sq.colortex.cn

TS:   // 同 JS
来源：http://se.jianghongdianzi.cn

Java: new Thread(() -> f()).start()
来源：http://af.huanxung.cn

Go:   go f()
来源：http://ub.jianghongdianzi.cn

Ruby: Thread.new { f }
来源：http://eq.huanxung.cn

C#:   Task.Run(() => F());
来源：http://qz.asd995.cn

[O02] 使用线程池
来源：http://ma.huixiangedu.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://sd.muxihuayi.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://jp.nicolike.cn

JS:   // worker_threads 线程池
来源：http://js.chemitech.net.cn

TS:   // worker_threads 线程池
来源：http://jm.szxytkj.cn

Java: Executors.newFixedThreadPool(4)
来源：http://ps.nszjky.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://by.muxihuayi.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://jp.nszjky.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://rz.gzmigu.cn

[O03] 加锁保护共享数据
来源：http://sp.gzmigu.cn

Py:   with lock: shared += 1
来源：http://nq.huixinmuqiang.cn

PHP:  // 用 flock() 做文件锁
来源：http://xw.nicolike.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hn.shxzukj.cn

TS:   // 同 JS
来源：http://as.bookmarksfly.cn

Java: synchronized (this) { shared++; }
来源：http://vi.newstarts.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ar.chemitech.net.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://ns.shxzskj.cn

C#:   lock (gate) { shared++; }
来源：http://jw.muxihuayi.cn

[O04] 定义异步函数并等待
来源：http://fv.yuntaijiaju.cn

Py:   async def f():⏎    await g()
来源：http://pg.colortex.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://zj.shxzskj.cn

JS:   async function f() { await g(); }
来源：http://qw.shxzskj.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://vc.szsharing.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ym.szxytkj.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ug.chemitech.net.cn

Ruby: # 用 Fiber 或 async gem
来源：http://yw.szsharing.cn

C#:   async Task F() { await G(); }
来源：http://wh.shxzskj.cn

[O05] 并发执行并等待全部完成
来源：http://fy.nicolike.cn

Py:   asyncio.gather(*tasks)
来源：http://dc.colortex.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ka.szxytkj.cn

JS:   await Promise.all(tasks)
来源：http://gl.bjjhwx.cn

TS:   await Promise.all(tasks)
来源：http://pg.wgjwhj.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ac.asd995.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://md.jctech888.com.cn

Ruby: threads.map(&:join)
来源：http://nt.jctech888.com.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://yj.521024.cn

[O06] 使用进程池
来源：http://pf.szsharing.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hg.nszjky.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://jy.szsharing.cn

JS:   // child_process / cluster 模块
来源：http://aj.nicolike.cn

TS:   // child_process / cluster 模块
来源：http://ji.asd995.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://di.hnjuh.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://vh.lnxyls.cn

Ruby: // fork 块
来源：http://fq.huixinmuqiang.cn

C#:   Parallel.For
来源：http://wl.panjiajie.cn

================================================================================
来源：http://zy.nicolike.cn

P. 常用工具函数
来源：http://ms.521024.cn

================================================================================
来源：http://tt.shxzskj.cn

[P01] 生成 UUID
来源：http://bh.nicolike.cn

Py:   str(uuid.uuid4())
来源：http://kk.yuntaijiaju.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ek.haigaiapp.cn

JS:   crypto.randomUUID()
来源：http://zi.gzmigu.cn

TS:   crypto.randomUUID()
来源：http://bt.521024.cn

Java: UUID.randomUUID().toString()
来源：http://lj.muxihuayi.cn

Go:   // 用 github.com/google/uuid
来源：http://hn.yuntaijiaju.cn

Ruby: SecureRandom.uuid
来源：http://kw.jctech888.com.cn

C#:   Guid.NewGuid().ToString()
来源：http://tg.9csxet.cn

[P02] MD5 / SHA256 摘要
来源：http://xh.asd995.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://rc.wgjwhj.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://rj.9csxet.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://nv.bookmarksfly.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://kv.haigaiapp.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://jg.huixinmuqiang.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://cf.haigaiapp.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://rz.chemitech.net.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://vb.lnxyls.cn

[P03] 生成短随机字符串
来源：http://ua.gzmigu.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://nz.jianghongdianzi.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://bb.newstarts.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://cd.shxzskj.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://cg.shtwfgs.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://iq.nicolike.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wm.huixiangedu.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://du.hahajie.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://do.chemitech.net.cn

[P04] 求长度
来源：http://gb.hahajie.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://on.asd995.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ug.colortex.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://cw.colortex.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://lz.521024.cn

Java: list.size();  map.size();  s.length()
来源：http://qh.521024.cn

Go:   len(arr);  len(m)
来源：http://pl.colortex.cn

Ruby: x.length;  x.size
来源：http://nd.huixiangedu.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://yd.newstarts.cn

[P05] 判断两个对象内容是否相等
来源：http://xl.nicolike.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://wa.muxihuayi.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://yu.bookmarksfly.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://yc.szsharing.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://rq.shxzskj.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://re.haigaiapp.cn

Go:   reflect.DeepEqual(a, b)
来源：http://ks.yuntaijiaju.cn

Ruby: a == b
来源：http://lw.huanxung.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ws.huixiangedu.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ei.9csxet.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://nx.9csxet.cn

PHP:  if (empty($x)) {}
来源：http://id.lnxyls.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://up.shtwfgs.cn

TS:   if (x == null) {}
来源：http://pa.nicolike.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://wx.colortex.cn

Go:   if x == nil {}
来源：http://eg.huixinmuqiang.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://rx.shxzskj.cn

C#:   if (x is null) {}
来源：http://wu.bookmarksfly.cn

[P07] 防抖与节流
来源：http://sd.haigaiapp.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://vx.nszjky.cn

PHP:  // 手写时间戳比较
来源：http://bp.bjjhwx.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://eq.hnjuh.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://pu.panjiajie.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://xa.huixinmuqiang.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://du.haigaiapp.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://vj.hnjuh.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://pg.shxzukj.cn

[P08] 处理浮点精度问题
来源：http://mt.521024.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ny.szxytkj.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ia.szxytkj.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ix.jctech888.com.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://zm.haigaiapp.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://jf.huanxung.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hx.521024.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://od.muxihuayi.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://nu.szxytkj.cn

================================================================================
来源：http://db.szxytkj.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://dn.521024.cn

================================================================================
来源：http://nv.huixiangedu.cn

[Q01] 创建表
来源：http://ks.haigaiapp.cn

CREATE TABLE users (
来源：http://vv.hnjuh.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://zi.panjiajie.cn

name VARCHAR(50) NOT NULL,
来源：http://gf.colortex.cn

email VARCHAR(100) UNIQUE,
来源：http://ey.jianghongdianzi.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ht.nszjky.cn

);
来源：http://xn.shtwfgs.cn

[Q02] 创建带外键的表
来源：http://ed.9csxet.cn

CREATE TABLE orders (
来源：http://hk.haigaiapp.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://xt.shxzskj.cn

user_id INT NOT NULL,
来源：http://bc.521024.cn

amount DECIMAL(10, 2),
来源：http://hj.wgjwhj.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ng.hnjuh.cn

);
来源：http://az.jctech888.com.cn

[Q03] 增加列
来源：http://ik.hnjuh.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://xb.asd995.cn

[Q04] 修改列类型
来源：http://sw.asd995.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://np.nicolike.cn

[Q05] 重命名列
来源：http://uw.jctech888.com.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://vs.huanxung.cn

[Q06] 删除列
来源：http://kb.nicolike.cn

ALTER TABLE users DROP COLUMN age;
来源：http://pf.521024.cn

[Q07] 删除表
来源：http://se.huixinmuqiang.cn

DROP TABLE IF EXISTS orders;
来源：http://gp.hnjuh.cn

[Q08] 创建普通索引
来源：http://ag.bookmarksfly.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://vw.szxytkj.cn

[Q09] 创建唯一索引
来源：http://ow.shtwfgs.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://de.huanxung.cn

[Q10] 插入单行
来源：http://cu.szxytkj.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wl.newstarts.cn

[Q11] 一次插入多行
来源：http://au.huanxung.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://cd.huixinmuqiang.cn

[Q12] 插入后取自增 ID
来源：http://fo.hnjuh.cn

INSERT INTO users (name) VALUES ('C');
来源：http://av.hahajie.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://fv.bjjhwx.cn

[Q13] 忽略重复插入
来源：http://bo.jctech888.com.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wm.szsharing.cn

[Q14] 存在则更新（upsert）
来源：http://he.jianghongdianzi.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://pn.colortex.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://rv.huixiangedu.cn

[Q15] 查询全部
来源：http://er.szxytkj.cn

SELECT * FROM users;
来源：http://qa.huixiangedu.cn

[Q16] 查询指定列
来源：http://fk.hnjuh.cn

SELECT id, name FROM users;
来源：http://os.haigaiapp.cn

[Q17] 条件查询
来源：http://vy.huanxung.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ob.wgjwhj.cn

[Q18] 模糊匹配
来源：http://ye.521024.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://rp.9csxet.cn

[Q19] 范围查询
来源：http://zz.chemitech.net.cn


<!-- 参考信息 -->