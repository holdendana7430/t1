代发 wailian999

Java: public static void main(String[] args)
来源：http://qp.9csxet.cn

Go:   func main()
来源：http://bu.muxihuayi.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://vu.521024.cn

C#:   static void Main(string[] args)
来源：http://jf.szxytkj.cn

[M08] 获取系统与运行时信息
来源：http://md.huanxung.cn

Py:   platform.system();  platform.python_version()
来源：http://kc.szsharing.cn

PHP:  PHP_OS;  phpversion();
来源：http://ls.bjjhwx.cn

JS:   process.platform;  process.version
来源：http://oi.shxzukj.cn

TS:   process.platform;  process.version
来源：http://ei.gzmigu.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://am.bjjhwx.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://yc.9csxet.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://kb.bjjhwx.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://vx.shxzskj.cn

================================================================================
来源：http://km.9csxet.cn

N. 数据结构与算法
来源：http://yo.szxytkj.cn

================================================================================
来源：http://sh.colortex.cn

[N01] 二分查找（有序数组）
来源：http://gx.jctech888.com.cn

Py:   bisect.bisect_left(arr, x)
来源：http://ej.9csxet.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://qq.hnjuh.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://yf.asd995.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ky.bookmarksfly.cn

Java: Arrays.binarySearch(arr, x)
来源：http://me.nszjky.cn

Go:   sort.SearchInts(arr, x)
来源：http://lr.muxihuayi.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://vn.huixinmuqiang.cn

C#:   Array.BinarySearch(arr, x)
来源：http://jy.lnxyls.cn

[N02] 排序（工程实践用内置实现）
来源：http://hn.szxytkj.cn

Py:   sorted(arr);  arr.sort()
来源：http://ce.muxihuayi.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://dw.bookmarksfly.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://wn.hnjuh.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://bu.shtwfgs.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://es.haigaiapp.cn

Go:   slices.Sort(arr)
来源：http://jw.521024.cn

Ruby: arr.sort
来源：http://to.yuntaijiaju.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://vi.jctech888.com.cn

[N03] 快速排序（分治示例）
来源：http://fe.hahajie.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://es.shxzskj.cn

PHP:  // 递归实现，或用 usort
来源：http://an.jctech888.com.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://xb.huixinmuqiang.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://tl.shtwfgs.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://vx.shxzukj.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://tk.lnxyls.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ud.hahajie.cn

C#:   // 手写递归，或 Array.Sort
来源：http://ih.szxytkj.cn

[N04] 斐波那契数列
来源：http://lm.asd995.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ju.newstarts.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ui.nicolike.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://bl.521024.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://zf.huixiangedu.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ia.huixiangedu.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ku.colortex.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ju.huixiangedu.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://rq.shxzukj.cn

[N05] 最大公约数
来源：http://ys.newstarts.cn

Py:   math.gcd(a, b)
来源：http://gj.jianghongdianzi.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://gl.shxzukj.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://oe.szsharing.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://kv.nszjky.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://rn.muxihuayi.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://zo.panjiajie.cn

Ruby: a.gcd(b)
来源：http://uk.shtwfgs.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://dj.521024.cn

[N06] 判断回文字符串
来源：http://if.huixiangedu.cn

Py:   s == s[::-1]
来源：http://op.shtwfgs.cn

PHP:  $s === strrev($s);
来源：http://ve.newstarts.cn

JS:   s === [...s].reverse().join("")
来源：http://fr.jctech888.com.cn

TS:   s === [...s].reverse().join("")
来源：http://uj.chemitech.net.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ca.hahajie.cn

Go:   // 双指针从两端比较
来源：http://ds.gzmigu.cn

Ruby: s == s.reverse
来源：http://ho.yuntaijiaju.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://ko.chemitech.net.cn

[N07] 两数之和（返回下标）
来源：http://mq.colortex.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://sf.shxzukj.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://cr.lnxyls.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://mf.gzmigu.cn

TS:   // 手写 Map<string, number>
来源：http://vo.nicolike.cn

Java: // 手写 HashMap
来源：http://vl.huixiangedu.cn

Go:   // 手写 map[int]int
来源：http://mf.9csxet.cn

Ruby: // 手写 Hash
来源：http://su.bjjhwx.cn

C#:   // 手写 Dictionary<int, int>
来源：http://wl.521024.cn

[N08] 生成全排列
来源：http://st.gzmigu.cn

Py:   itertools.permutations(arr)
来源：http://ib.yuexingan06.cn

PHP:  // 手写递归交换
来源：http://oz.newstarts.cn

JS:   // 手写回溯递归
来源：http://au.yuntaijiaju.cn

TS:   // 手写回溯递归
来源：http://vp.yuexingan06.cn

Java: // 手写回溯递归
来源：http://dl.yuexingan06.cn

Go:   // 手写回溯递归
来源：http://zb.jctech888.com.cn

Ruby: arr.permutation.to_a
来源：http://ra.shxzskj.cn

C#:   // 手写回溯递归
来源：http://ut.haigaiapp.cn

[N09] 栈与队列
来源：http://xx.szsharing.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://iy.muxihuayi.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://nv.bjjhwx.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://sz.nicolike.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ge.yuntaijiaju.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://fc.chemitech.net.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mi.yuexingan06.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ct.9csxet.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://kc.shtwfgs.cn

[N10] 链表节点定义
来源：http://al.asd995.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://eo.lnxyls.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://jw.newstarts.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://bf.newstarts.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://dj.bjjhwx.cn

Java: class Node { int v; Node next; }
来源：http://ge.huixiangedu.cn

Go:   type Node struct { V int; Next *Node }
来源：http://yo.newstarts.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://at.shxzskj.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://dd.haigaiapp.cn

[N11] 二叉树中序遍历
来源：http://jb.9csxet.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://qt.9csxet.cn

PHP:  // 手写递归函数
来源：http://mu.huixinmuqiang.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://kv.gzmigu.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://jh.521024.cn

Java: // 手写递归
来源：http://es.hnjuh.cn

Go:   // 手写递归
来源：http://qn.huanxung.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://fs.9csxet.cn

C#:   // 手写递归
来源：http://ke.panjiajie.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://fb.wgjwhj.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://tg.yuntaijiaju.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://cd.lnxyls.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://vv.yuexingan06.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://tw.yuexingan06.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://pm.muxihuayi.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mm.nicolike.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://rk.nszjky.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://sb.asd995.cn

================================================================================
来源：http://fn.huixinmuqiang.cn

O. 并发与异步
来源：http://wr.colortex.cn

================================================================================
来源：http://al.shxzukj.cn

[O01] 启动一个线程
来源：http://bn.hnjuh.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ou.hahajie.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://gu.yuntaijiaju.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://xu.bjjhwx.cn

TS:   // 同 JS
来源：http://fl.lnxyls.cn

Java: new Thread(() -> f()).start()
来源：http://mc.chemitech.net.cn

Go:   go f()
来源：http://tg.huixiangedu.cn

Ruby: Thread.new { f }
来源：http://oh.wgjwhj.cn

C#:   Task.Run(() => F());
来源：http://ud.colortex.cn

[O02] 使用线程池
来源：http://hk.9csxet.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://oy.wgjwhj.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hf.yuntaijiaju.cn

JS:   // worker_threads 线程池
来源：http://fz.yuntaijiaju.cn

TS:   // worker_threads 线程池
来源：http://mb.yuexingan06.cn

Java: Executors.newFixedThreadPool(4)
来源：http://qn.szsharing.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://dm.nicolike.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://vy.lnxyls.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ea.bookmarksfly.cn

[O03] 加锁保护共享数据
来源：http://af.panjiajie.cn

Py:   with lock: shared += 1
来源：http://vc.shxzukj.cn

PHP:  // 用 flock() 做文件锁
来源：http://xg.newstarts.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://bm.gzmigu.cn

TS:   // 同 JS
来源：http://qf.asd995.cn

Java: synchronized (this) { shared++; }
来源：http://gp.huixinmuqiang.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://fe.huanxung.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://jx.newstarts.cn

C#:   lock (gate) { shared++; }
来源：http://vp.nszjky.cn

[O04] 定义异步函数并等待
来源：http://pz.asd995.cn

Py:   async def f():⏎    await g()
来源：http://mh.wgjwhj.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://rp.huixiangedu.cn

JS:   async function f() { await g(); }
来源：http://un.huanxung.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://sl.yuntaijiaju.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://lm.yuexingan06.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ig.nszjky.cn

Ruby: # 用 Fiber 或 async gem
来源：http://hy.newstarts.cn

C#:   async Task F() { await G(); }
来源：http://fm.gzmigu.cn

[O05] 并发执行并等待全部完成
来源：http://yo.szsharing.cn

Py:   asyncio.gather(*tasks)
来源：http://oj.nicolike.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://kv.jctech888.com.cn

JS:   await Promise.all(tasks)
来源：http://hb.bookmarksfly.cn

TS:   await Promise.all(tasks)
来源：http://qz.panjiajie.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://rq.hahajie.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ye.bookmarksfly.cn

Ruby: threads.map(&:join)
来源：http://cc.bookmarksfly.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://oe.lnxyls.cn

[O06] 使用进程池
来源：http://wn.szsharing.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://sf.nszjky.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://yl.521024.cn

JS:   // child_process / cluster 模块
来源：http://rt.shxzukj.cn

TS:   // child_process / cluster 模块
来源：http://wo.gzmigu.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://av.asd995.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://tq.huanxung.cn

Ruby: // fork 块
来源：http://dp.yuexingan06.cn

C#:   Parallel.For
来源：http://sp.yuntaijiaju.cn

================================================================================
来源：http://xd.asd995.cn

P. 常用工具函数
来源：http://cf.haigaiapp.cn

================================================================================
来源：http://uh.asd995.cn

[P01] 生成 UUID
来源：http://hs.chemitech.net.cn

Py:   str(uuid.uuid4())
来源：http://rw.shxzskj.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ha.muxihuayi.cn

JS:   crypto.randomUUID()
来源：http://yd.asd995.cn

TS:   crypto.randomUUID()
来源：http://ir.shxzskj.cn

Java: UUID.randomUUID().toString()
来源：http://to.colortex.cn

Go:   // 用 github.com/google/uuid
来源：http://pl.chemitech.net.cn

Ruby: SecureRandom.uuid
来源：http://os.shtwfgs.cn

C#:   Guid.NewGuid().ToString()
来源：http://hj.shtwfgs.cn

[P02] MD5 / SHA256 摘要
来源：http://rr.shxzukj.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wy.huixiangedu.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://va.shtwfgs.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://zb.nszjky.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wa.panjiajie.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://jc.yuexingan06.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://of.asd995.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ff.nicolike.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ct.gzmigu.cn

[P03] 生成短随机字符串
来源：http://xo.muxihuayi.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://nx.newstarts.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://zh.yuntaijiaju.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://do.wgjwhj.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://oq.521024.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://va.haigaiapp.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://pl.jianghongdianzi.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://lt.szxytkj.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://cw.wgjwhj.cn

[P04] 求长度
来源：http://yl.shxzskj.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://nx.haigaiapp.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://jq.huixinmuqiang.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ue.jctech888.com.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://yl.521024.cn

Java: list.size();  map.size();  s.length()
来源：http://vg.szsharing.cn

Go:   len(arr);  len(m)
来源：http://ei.colortex.cn

Ruby: x.length;  x.size
来源：http://ph.shtwfgs.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://gf.lnxyls.cn

[P05] 判断两个对象内容是否相等
来源：http://vy.hnjuh.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://zi.lnxyls.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://gl.hnjuh.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ib.huixiangedu.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://nj.huixiangedu.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://yh.nszjky.cn

Go:   reflect.DeepEqual(a, b)
来源：http://op.wgjwhj.cn

Ruby: a == b
来源：http://ed.yuexingan06.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://fo.haigaiapp.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://qd.panjiajie.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://yz.gzmigu.cn

PHP:  if (empty($x)) {}
来源：http://pv.9csxet.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://af.yuexingan06.cn

TS:   if (x == null) {}
来源：http://pu.lnxyls.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://xy.haigaiapp.cn

Go:   if x == nil {}
来源：http://hb.newstarts.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ok.huixiangedu.cn

C#:   if (x is null) {}
来源：http://qb.newstarts.cn

[P07] 防抖与节流
来源：http://av.chemitech.net.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://df.jianghongdianzi.cn

PHP:  // 手写时间戳比较
来源：http://dw.jctech888.com.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://vo.szxytkj.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://kf.wgjwhj.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://jq.colortex.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://vw.muxihuayi.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://cq.shtwfgs.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://kv.521024.cn

[P08] 处理浮点精度问题
来源：http://ye.gzmigu.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://qq.nicolike.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ck.gzmigu.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://kv.colortex.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ps.jctech888.com.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mh.lnxyls.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wk.bjjhwx.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://cm.huanxung.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://iz.colortex.cn

================================================================================
来源：http://vn.newstarts.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://gg.szxytkj.cn

================================================================================
来源：http://eo.jianghongdianzi.cn

[Q01] 创建表
来源：http://cv.haigaiapp.cn

CREATE TABLE users (
来源：http://fw.shxzukj.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://zw.nszjky.cn

name VARCHAR(50) NOT NULL,
来源：http://hu.szxytkj.cn

email VARCHAR(100) UNIQUE,
来源：http://xi.hahajie.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://zx.haigaiapp.cn

);
来源：http://cr.bookmarksfly.cn

[Q02] 创建带外键的表
来源：http://oh.nicolike.cn

CREATE TABLE orders (
来源：http://xk.hahajie.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://dv.szxytkj.cn

user_id INT NOT NULL,
来源：http://fo.yuntaijiaju.cn

amount DECIMAL(10, 2),
来源：http://sr.bookmarksfly.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://fp.chemitech.net.cn

);
来源：http://ow.chemitech.net.cn

[Q03] 增加列
来源：http://rp.huanxung.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ud.521024.cn

[Q04] 修改列类型
来源：http://of.hahajie.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://rz.shtwfgs.cn

[Q05] 重命名列
来源：http://zl.wgjwhj.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ho.521024.cn

[Q06] 删除列
来源：http://wn.521024.cn

ALTER TABLE users DROP COLUMN age;
来源：http://ne.panjiajie.cn

[Q07] 删除表
来源：http://bv.gzmigu.cn

DROP TABLE IF EXISTS orders;
来源：http://ws.nicolike.cn

[Q08] 创建普通索引
来源：http://rd.nszjky.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://sb.newstarts.cn

[Q09] 创建唯一索引
来源：http://an.wgjwhj.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://fc.asd995.cn

[Q10] 插入单行
来源：http://qx.hahajie.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://dr.newstarts.cn

[Q11] 一次插入多行
来源：http://bc.colortex.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ui.hahajie.cn

[Q12] 插入后取自增 ID
来源：http://rn.haigaiapp.cn

INSERT INTO users (name) VALUES ('C');
来源：http://rr.panjiajie.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://kb.lnxyls.cn

[Q13] 忽略重复插入
来源：http://qv.muxihuayi.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://un.bjjhwx.cn

[Q14] 存在则更新（upsert）
来源：http://iv.szxytkj.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://py.yuntaijiaju.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://zv.nicolike.cn

[Q15] 查询全部
来源：http://ki.hnjuh.cn


<!-- 参考信息 -->