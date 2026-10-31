代发 wailian999

TS:   process.platform;  process.version
来源：http://fd.panjiajie.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://lw.bjjhwx.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://wv.shtwfgs.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://dc.nszjky.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://yk.9csxet.cn

================================================================================
来源：http://tr.jctech888.com.cn

N. 数据结构与算法
来源：http://tt.huixinmuqiang.cn

================================================================================
来源：http://ug.newstarts.cn

[N01] 二分查找（有序数组）
来源：http://wv.9csxet.cn

Py:   bisect.bisect_left(arr, x)
来源：http://ri.colortex.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://kt.huixiangedu.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://yu.haigaiapp.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://bk.szsharing.cn

Java: Arrays.binarySearch(arr, x)
来源：http://ac.huixiangedu.cn

Go:   sort.SearchInts(arr, x)
来源：http://rm.hnjuh.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://rf.wgjwhj.cn

C#:   Array.BinarySearch(arr, x)
来源：http://io.panjiajie.cn

[N02] 排序（工程实践用内置实现）
来源：http://zr.hnjuh.cn

Py:   sorted(arr);  arr.sort()
来源：http://lc.panjiajie.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://yh.yuexingan06.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://mp.yuntaijiaju.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://xi.yuexingan06.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://gv.szsharing.cn

Go:   slices.Sort(arr)
来源：http://jt.gzmigu.cn

Ruby: arr.sort
来源：http://iv.colortex.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://xn.huixiangedu.cn

[N03] 快速排序（分治示例）
来源：http://cx.hahajie.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://xz.yuntaijiaju.cn

PHP:  // 递归实现，或用 usort
来源：http://gr.szsharing.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://nn.bjjhwx.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hk.hnjuh.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://qw.jianghongdianzi.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://pb.nszjky.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://xn.wgjwhj.cn

C#:   // 手写递归，或 Array.Sort
来源：http://eo.asd995.cn

[N04] 斐波那契数列
来源：http://bf.shtwfgs.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://gy.shxzskj.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://lt.shtwfgs.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://il.huanxung.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://tg.9csxet.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ar.haigaiapp.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ni.szsharing.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://be.nszjky.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://cu.shxzskj.cn

[N05] 最大公约数
来源：http://ft.haigaiapp.cn

Py:   math.gcd(a, b)
来源：http://aw.shtwfgs.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://gm.shtwfgs.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://po.huixiangedu.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://rz.szsharing.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hi.jctech888.com.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://xt.szxytkj.cn

Ruby: a.gcd(b)
来源：http://gy.jianghongdianzi.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://pl.shtwfgs.cn

[N06] 判断回文字符串
来源：http://uq.9csxet.cn

Py:   s == s[::-1]
来源：http://vh.gzmigu.cn

PHP:  $s === strrev($s);
来源：http://fb.gzmigu.cn

JS:   s === [...s].reverse().join("")
来源：http://gd.gzmigu.cn

TS:   s === [...s].reverse().join("")
来源：http://dl.jctech888.com.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://gs.hahajie.cn

Go:   // 双指针从两端比较
来源：http://na.wgjwhj.cn

Ruby: s == s.reverse
来源：http://dm.szsharing.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://ym.muxihuayi.cn

[N07] 两数之和（返回下标）
来源：http://ff.asd995.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://et.521024.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://nq.chemitech.net.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://tf.asd995.cn

TS:   // 手写 Map<string, number>
来源：http://ak.yuexingan06.cn

Java: // 手写 HashMap
来源：http://rd.newstarts.cn

Go:   // 手写 map[int]int
来源：http://mk.hnjuh.cn

Ruby: // 手写 Hash
来源：http://pu.shtwfgs.cn

C#:   // 手写 Dictionary<int, int>
来源：http://iz.haigaiapp.cn

[N08] 生成全排列
来源：http://uz.muxihuayi.cn

Py:   itertools.permutations(arr)
来源：http://nm.hnjuh.cn

PHP:  // 手写递归交换
来源：http://cy.colortex.cn

JS:   // 手写回溯递归
来源：http://sq.bjjhwx.cn

TS:   // 手写回溯递归
来源：http://yf.jianghongdianzi.cn

Java: // 手写回溯递归
来源：http://xj.shtwfgs.cn

Go:   // 手写回溯递归
来源：http://vi.huixiangedu.cn

Ruby: arr.permutation.to_a
来源：http://yy.shxzukj.cn

C#:   // 手写回溯递归
来源：http://po.jctech888.com.cn

[N09] 栈与队列
来源：http://fj.hahajie.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://aa.yuexingan06.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://cp.nszjky.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wf.chemitech.net.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ca.huixinmuqiang.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://nj.panjiajie.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mk.nszjky.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ex.shxzukj.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mz.shxzukj.cn

[N10] 链表节点定义
来源：http://yp.wgjwhj.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://rh.bookmarksfly.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://hu.nszjky.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ql.shtwfgs.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ge.yuexingan06.cn

Java: class Node { int v; Node next; }
来源：http://nc.9csxet.cn

Go:   type Node struct { V int; Next *Node }
来源：http://ao.nicolike.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://jo.nszjky.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://xp.jianghongdianzi.cn

[N11] 二叉树中序遍历
来源：http://nz.gzmigu.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://vf.haigaiapp.cn

PHP:  // 手写递归函数
来源：http://zu.huanxung.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ns.szxytkj.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://rl.muxihuayi.cn

Java: // 手写递归
来源：http://ri.chemitech.net.cn

Go:   // 手写递归
来源：http://vk.haigaiapp.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://yg.huixiangedu.cn

C#:   // 手写递归
来源：http://cy.jctech888.com.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://qx.newstarts.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wh.wgjwhj.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://vs.9csxet.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://uc.nszjky.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ls.yuexingan06.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://fi.9csxet.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hl.szsharing.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://qh.szxytkj.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://kx.szxytkj.cn

================================================================================
来源：http://id.hnjuh.cn

O. 并发与异步
来源：http://mz.jianghongdianzi.cn

================================================================================
来源：http://qs.haigaiapp.cn

[O01] 启动一个线程
来源：http://ac.9csxet.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://fm.jianghongdianzi.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://fa.yuntaijiaju.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://uw.bjjhwx.cn

TS:   // 同 JS
来源：http://re.nicolike.cn

Java: new Thread(() -> f()).start()
来源：http://vg.bjjhwx.cn

Go:   go f()
来源：http://nn.shtwfgs.cn

Ruby: Thread.new { f }
来源：http://ww.shxzskj.cn

C#:   Task.Run(() => F());
来源：http://rn.jianghongdianzi.cn

[O02] 使用线程池
来源：http://zz.gzmigu.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hr.9csxet.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://go.jianghongdianzi.cn

JS:   // worker_threads 线程池
来源：http://dn.chemitech.net.cn

TS:   // worker_threads 线程池
来源：http://xa.yuexingan06.cn

Java: Executors.newFixedThreadPool(4)
来源：http://rb.bookmarksfly.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mt.asd995.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mw.nszjky.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://za.szxytkj.cn

[O03] 加锁保护共享数据
来源：http://rn.chemitech.net.cn

Py:   with lock: shared += 1
来源：http://jo.gzmigu.cn

PHP:  // 用 flock() 做文件锁
来源：http://bs.panjiajie.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ts.huanxung.cn

TS:   // 同 JS
来源：http://wi.panjiajie.cn

Java: synchronized (this) { shared++; }
来源：http://nj.chemitech.net.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://jz.bjjhwx.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://te.hahajie.cn

C#:   lock (gate) { shared++; }
来源：http://mz.haigaiapp.cn

[O04] 定义异步函数并等待
来源：http://to.colortex.cn

Py:   async def f():⏎    await g()
来源：http://co.huixinmuqiang.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://pe.newstarts.cn

JS:   async function f() { await g(); }
来源：http://ik.nicolike.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://yl.bjjhwx.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ha.bookmarksfly.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://rv.huixiangedu.cn

Ruby: # 用 Fiber 或 async gem
来源：http://zi.huixinmuqiang.cn

C#:   async Task F() { await G(); }
来源：http://vb.shxzskj.cn

[O05] 并发执行并等待全部完成
来源：http://ok.huixiangedu.cn

Py:   asyncio.gather(*tasks)
来源：http://gk.nszjky.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ux.bookmarksfly.cn

JS:   await Promise.all(tasks)
来源：http://sr.hahajie.cn

TS:   await Promise.all(tasks)
来源：http://ms.shtwfgs.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://pd.jctech888.com.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://gn.yuexingan06.cn

Ruby: threads.map(&:join)
来源：http://ar.nszjky.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://ny.shxzskj.cn

[O06] 使用进程池
来源：http://oo.chemitech.net.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ei.lnxyls.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://co.9csxet.cn

JS:   // child_process / cluster 模块
来源：http://av.nicolike.cn

TS:   // child_process / cluster 模块
来源：http://kq.muxihuayi.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ig.huanxung.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ol.jianghongdianzi.cn

Ruby: // fork 块
来源：http://ny.shxzskj.cn

C#:   Parallel.For
来源：http://mv.huixiangedu.cn

================================================================================
来源：http://to.lnxyls.cn

P. 常用工具函数
来源：http://ro.wgjwhj.cn

================================================================================
来源：http://de.521024.cn

[P01] 生成 UUID
来源：http://dk.nszjky.cn

Py:   str(uuid.uuid4())
来源：http://gl.huixinmuqiang.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://yp.bjjhwx.cn

JS:   crypto.randomUUID()
来源：http://pq.chemitech.net.cn

TS:   crypto.randomUUID()
来源：http://cp.bookmarksfly.cn

Java: UUID.randomUUID().toString()
来源：http://gy.bjjhwx.cn

Go:   // 用 github.com/google/uuid
来源：http://fn.hnjuh.cn

Ruby: SecureRandom.uuid
来源：http://cy.nszjky.cn

C#:   Guid.NewGuid().ToString()
来源：http://fi.bookmarksfly.cn

[P02] MD5 / SHA256 摘要
来源：http://px.nszjky.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://aw.panjiajie.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://qk.newstarts.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://dr.huixinmuqiang.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://fj.yuexingan06.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://se.bjjhwx.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://eq.hnjuh.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ia.szxytkj.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://pj.huanxung.cn

[P03] 生成短随机字符串
来源：http://zq.jctech888.com.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://oj.gzmigu.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://eb.huixiangedu.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://to.huixinmuqiang.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://dr.bookmarksfly.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ju.521024.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://oo.chemitech.net.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://hf.shxzukj.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://zg.shtwfgs.cn

[P04] 求长度
来源：http://bw.panjiajie.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mz.lnxyls.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://pv.bjjhwx.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://bf.gzmigu.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://pe.colortex.cn

Java: list.size();  map.size();  s.length()
来源：http://ry.hnjuh.cn

Go:   len(arr);  len(m)
来源：http://dq.szxytkj.cn

Ruby: x.length;  x.size
来源：http://vw.bookmarksfly.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://nt.bjjhwx.cn

[P05] 判断两个对象内容是否相等
来源：http://uf.wgjwhj.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://os.huixiangedu.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://go.szsharing.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mt.bookmarksfly.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ks.nszjky.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ff.yuexingan06.cn

Go:   reflect.DeepEqual(a, b)
来源：http://yn.521024.cn

Ruby: a == b
来源：http://to.hahajie.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://if.gzmigu.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wf.hahajie.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ex.asd995.cn

PHP:  if (empty($x)) {}
来源：http://kp.haigaiapp.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://dy.huixiangedu.cn

TS:   if (x == null) {}
来源：http://hn.muxihuayi.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://lh.hahajie.cn

Go:   if x == nil {}
来源：http://zf.muxihuayi.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://na.521024.cn

C#:   if (x is null) {}
来源：http://sn.521024.cn

[P07] 防抖与节流
来源：http://fx.wgjwhj.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://zq.shxzskj.cn

PHP:  // 手写时间戳比较
来源：http://db.wgjwhj.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://di.yuexingan06.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ct.jctech888.com.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://un.asd995.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://zg.lnxyls.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://gf.hahajie.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://jm.bookmarksfly.cn

[P08] 处理浮点精度问题
来源：http://qb.szxytkj.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://we.shxzskj.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://om.muxihuayi.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://fg.hnjuh.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ip.jctech888.com.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://tw.wgjwhj.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mu.hnjuh.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://oq.szsharing.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://pa.chemitech.net.cn

================================================================================
来源：http://it.huixiangedu.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://rv.asd995.cn

================================================================================
来源：http://qj.nicolike.cn

[Q01] 创建表
来源：http://st.hahajie.cn

CREATE TABLE users (
来源：http://vd.shtwfgs.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mc.panjiajie.cn

name VARCHAR(50) NOT NULL,
来源：http://io.hnjuh.cn

email VARCHAR(100) UNIQUE,
来源：http://pl.yuntaijiaju.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ed.bookmarksfly.cn

);
来源：http://fh.shxzukj.cn

[Q02] 创建带外键的表
来源：http://aj.chemitech.net.cn

CREATE TABLE orders (
来源：http://gd.bjjhwx.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://cu.bjjhwx.cn

user_id INT NOT NULL,
来源：http://zn.asd995.cn

amount DECIMAL(10, 2),
来源：http://zh.chemitech.net.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mk.shtwfgs.cn

);
来源：http://zq.muxihuayi.cn

[Q03] 增加列
来源：http://az.bookmarksfly.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ut.asd995.cn

[Q04] 修改列类型
来源：http://xp.yuexingan06.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ia.chemitech.net.cn

[Q05] 重命名列
来源：http://kb.muxihuayi.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://br.shxzskj.cn

[Q06] 删除列
来源：http://nl.lnxyls.cn

ALTER TABLE users DROP COLUMN age;
来源：http://ku.muxihuayi.cn

[Q07] 删除表
来源：http://ye.huanxung.cn

DROP TABLE IF EXISTS orders;
来源：http://dm.szxytkj.cn

[Q08] 创建普通索引
来源：http://yu.panjiajie.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://ij.nszjky.cn

[Q09] 创建唯一索引
来源：http://kx.wgjwhj.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://bu.muxihuayi.cn

[Q10] 插入单行
来源：http://nd.shxzskj.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mc.521024.cn

[Q11] 一次插入多行
来源：http://zz.huanxung.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://dn.shxzukj.cn

[Q12] 插入后取自增 ID
来源：http://rx.bookmarksfly.cn

INSERT INTO users (name) VALUES ('C');
来源：http://kt.huixinmuqiang.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://jx.szsharing.cn

[Q13] 忽略重复插入
来源：http://hl.newstarts.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wc.szsharing.cn

[Q14] 存在则更新（upsert）
来源：http://nz.shxzukj.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://od.newstarts.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://fl.jctech888.com.cn

[Q15] 查询全部
来源：http://vf.huanxung.cn

SELECT * FROM users;
来源：http://vh.lnxyls.cn

[Q16] 查询指定列
来源：http://ge.nicolike.cn

SELECT id, name FROM users;
来源：http://hv.jctech888.com.cn

[Q17] 条件查询
来源：http://vn.szxytkj.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://jb.jctech888.com.cn

[Q18] 模糊匹配
来源：http://wk.gzmigu.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://gq.chemitech.net.cn

[Q19] 范围查询
来源：http://od.bookmarksfly.cn


<!-- 参考信息 -->