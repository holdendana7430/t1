代发 wailian999

Java: public static void main(String[] args)
来源：http://kt.huixinmuqiang.cn

Go:   func main()
来源：http://hk.szxytkj.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://qj.szsharing.cn

C#:   static void Main(string[] args)
来源：http://uc.jctech888.com.cn

[M08] 获取系统与运行时信息
来源：http://dm.muxihuayi.cn

Py:   platform.system();  platform.python_version()
来源：http://sw.shtwfgs.cn

PHP:  PHP_OS;  phpversion();
来源：http://cd.chemitech.net.cn

JS:   process.platform;  process.version
来源：http://qo.huanxung.cn

TS:   process.platform;  process.version
来源：http://jr.muxihuayi.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://yv.shtwfgs.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://xu.lnxyls.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://qt.521024.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://an.panjiajie.cn

================================================================================
来源：http://bb.huixiangedu.cn

N. 数据结构与算法
来源：http://kq.hahajie.cn

================================================================================
来源：http://ka.chemitech.net.cn

[N01] 二分查找（有序数组）
来源：http://ok.szxytkj.cn

Py:   bisect.bisect_left(arr, x)
来源：http://jq.shxzskj.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://yr.szsharing.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://gi.haigaiapp.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://qn.nicolike.cn

Java: Arrays.binarySearch(arr, x)
来源：http://ca.bookmarksfly.cn

Go:   sort.SearchInts(arr, x)
来源：http://dx.panjiajie.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://ax.hahajie.cn

C#:   Array.BinarySearch(arr, x)
来源：http://lh.panjiajie.cn

[N02] 排序（工程实践用内置实现）
来源：http://ob.shtwfgs.cn

Py:   sorted(arr);  arr.sort()
来源：http://wq.huixiangedu.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://tm.chemitech.net.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://dw.bookmarksfly.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://ey.colortex.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://nf.huanxung.cn

Go:   slices.Sort(arr)
来源：http://su.muxihuayi.cn

Ruby: arr.sort
来源：http://kf.yuntaijiaju.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://jj.wgjwhj.cn

[N03] 快速排序（分治示例）
来源：http://ix.bookmarksfly.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://xj.yuexingan06.cn

PHP:  // 递归实现，或用 usort
来源：http://aj.huanxung.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://dh.9csxet.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://vg.muxihuayi.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://qp.9csxet.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://qb.huanxung.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ft.muxihuayi.cn

C#:   // 手写递归，或 Array.Sort
来源：http://zo.huanxung.cn

[N04] 斐波那契数列
来源：http://ne.muxihuayi.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://kz.yuntaijiaju.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ee.shtwfgs.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://gf.huixinmuqiang.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://gz.huixiangedu.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://bi.chemitech.net.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ir.huixiangedu.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ox.huixiangedu.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://vx.bjjhwx.cn

[N05] 最大公约数
来源：http://ks.shxzukj.cn

Py:   math.gcd(a, b)
来源：http://dr.chemitech.net.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hi.newstarts.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://fd.hahajie.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://yn.nszjky.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://nw.lnxyls.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ry.wgjwhj.cn

Ruby: a.gcd(b)
来源：http://ei.bjjhwx.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://zq.bjjhwx.cn

[N06] 判断回文字符串
来源：http://rb.521024.cn

Py:   s == s[::-1]
来源：http://wn.shxzskj.cn

PHP:  $s === strrev($s);
来源：http://hn.huixinmuqiang.cn

JS:   s === [...s].reverse().join("")
来源：http://vn.panjiajie.cn

TS:   s === [...s].reverse().join("")
来源：http://ug.newstarts.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://cy.huanxung.cn

Go:   // 双指针从两端比较
来源：http://qt.gzmigu.cn

Ruby: s == s.reverse
来源：http://ak.chemitech.net.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://qi.shtwfgs.cn

[N07] 两数之和（返回下标）
来源：http://um.haigaiapp.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://pj.huixiangedu.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://rj.bjjhwx.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://uc.shxzukj.cn

TS:   // 手写 Map<string, number>
来源：http://mw.yuntaijiaju.cn

Java: // 手写 HashMap
来源：http://ca.asd995.cn

Go:   // 手写 map[int]int
来源：http://tj.panjiajie.cn

Ruby: // 手写 Hash
来源：http://qd.jianghongdianzi.cn

C#:   // 手写 Dictionary<int, int>
来源：http://rr.szxytkj.cn

[N08] 生成全排列
来源：http://nc.hahajie.cn

Py:   itertools.permutations(arr)
来源：http://lu.wgjwhj.cn

PHP:  // 手写递归交换
来源：http://jg.yuexingan06.cn

JS:   // 手写回溯递归
来源：http://pg.colortex.cn

TS:   // 手写回溯递归
来源：http://dd.jianghongdianzi.cn

Java: // 手写回溯递归
来源：http://uu.shxzukj.cn

Go:   // 手写回溯递归
来源：http://fk.panjiajie.cn

Ruby: arr.permutation.to_a
来源：http://vs.hahajie.cn

C#:   // 手写回溯递归
来源：http://sc.521024.cn

[N09] 栈与队列
来源：http://kb.9csxet.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://fm.nszjky.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://rn.haigaiapp.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://gz.asd995.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://kp.shxzskj.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ey.bjjhwx.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://gh.haigaiapp.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wr.szsharing.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://bv.panjiajie.cn

[N10] 链表节点定义
来源：http://qt.colortex.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://kz.szsharing.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://fw.jianghongdianzi.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://rp.9csxet.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://fr.shtwfgs.cn

Java: class Node { int v; Node next; }
来源：http://ua.yuexingan06.cn

Go:   type Node struct { V int; Next *Node }
来源：http://xb.szxytkj.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://xp.jianghongdianzi.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://ea.panjiajie.cn

[N11] 二叉树中序遍历
来源：http://qx.colortex.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://sb.huixiangedu.cn

PHP:  // 手写递归函数
来源：http://qn.szxytkj.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hx.521024.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://py.newstarts.cn

Java: // 手写递归
来源：http://xe.huanxung.cn

Go:   // 手写递归
来源：http://dl.jianghongdianzi.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wd.asd995.cn

C#:   // 手写递归
来源：http://gt.shtwfgs.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://cm.nicolike.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://yv.nszjky.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ge.huixiangedu.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://sp.nszjky.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://vm.jianghongdianzi.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://oj.jctech888.com.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://rt.hnjuh.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ze.bjjhwx.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://vp.muxihuayi.cn

================================================================================
来源：http://rd.asd995.cn

O. 并发与异步
来源：http://bv.shxzukj.cn

================================================================================
来源：http://yz.chemitech.net.cn

[O01] 启动一个线程
来源：http://ai.huixiangedu.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://bm.huanxung.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://my.asd995.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ot.szxytkj.cn

TS:   // 同 JS
来源：http://sw.asd995.cn

Java: new Thread(() -> f()).start()
来源：http://tv.colortex.cn

Go:   go f()
来源：http://ck.yuntaijiaju.cn

Ruby: Thread.new { f }
来源：http://uh.haigaiapp.cn

C#:   Task.Run(() => F());
来源：http://up.szsharing.cn

[O02] 使用线程池
来源：http://rr.huanxung.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://vr.szxytkj.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ir.bookmarksfly.cn

JS:   // worker_threads 线程池
来源：http://pd.huixiangedu.cn

TS:   // worker_threads 线程池
来源：http://wl.haigaiapp.cn

Java: Executors.newFixedThreadPool(4)
来源：http://zd.huixinmuqiang.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://fq.huanxung.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://td.521024.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://nv.jctech888.com.cn

[O03] 加锁保护共享数据
来源：http://kl.muxihuayi.cn

Py:   with lock: shared += 1
来源：http://uv.szxytkj.cn

PHP:  // 用 flock() 做文件锁
来源：http://ol.hahajie.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://rt.wgjwhj.cn

TS:   // 同 JS
来源：http://jm.lnxyls.cn

Java: synchronized (this) { shared++; }
来源：http://bq.lnxyls.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://gy.huixiangedu.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://ow.asd995.cn

C#:   lock (gate) { shared++; }
来源：http://bl.9csxet.cn

[O04] 定义异步函数并等待
来源：http://eq.newstarts.cn

Py:   async def f():⏎    await g()
来源：http://ua.nszjky.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://is.nicolike.cn

JS:   async function f() { await g(); }
来源：http://oi.9csxet.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://gp.wgjwhj.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://kq.colortex.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://uw.jctech888.com.cn

Ruby: # 用 Fiber 或 async gem
来源：http://wt.bjjhwx.cn

C#:   async Task F() { await G(); }
来源：http://yv.muxihuayi.cn

[O05] 并发执行并等待全部完成
来源：http://xg.huanxung.cn

Py:   asyncio.gather(*tasks)
来源：http://ac.asd995.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://fn.lnxyls.cn

JS:   await Promise.all(tasks)
来源：http://mk.521024.cn

TS:   await Promise.all(tasks)
来源：http://la.9csxet.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://od.colortex.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://nl.yuntaijiaju.cn

Ruby: threads.map(&:join)
来源：http://bd.wgjwhj.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://an.panjiajie.cn

[O06] 使用进程池
来源：http://av.jianghongdianzi.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://cv.newstarts.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://zd.colortex.cn

JS:   // child_process / cluster 模块
来源：http://nu.jianghongdianzi.cn

TS:   // child_process / cluster 模块
来源：http://xt.huixinmuqiang.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hb.panjiajie.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wc.gzmigu.cn

Ruby: // fork 块
来源：http://vz.jctech888.com.cn

C#:   Parallel.For
来源：http://ip.chemitech.net.cn

================================================================================
来源：http://ha.shxzukj.cn

P. 常用工具函数
来源：http://ja.asd995.cn

================================================================================
来源：http://ai.521024.cn

[P01] 生成 UUID
来源：http://vg.szxytkj.cn

Py:   str(uuid.uuid4())
来源：http://xy.nicolike.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://fy.shxzskj.cn

JS:   crypto.randomUUID()
来源：http://fz.yuexingan06.cn

TS:   crypto.randomUUID()
来源：http://bf.9csxet.cn

Java: UUID.randomUUID().toString()
来源：http://fm.haigaiapp.cn

Go:   // 用 github.com/google/uuid
来源：http://qq.yuntaijiaju.cn

Ruby: SecureRandom.uuid
来源：http://zb.lnxyls.cn

C#:   Guid.NewGuid().ToString()
来源：http://hq.colortex.cn

[P02] MD5 / SHA256 摘要
来源：http://jo.lnxyls.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ys.panjiajie.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://sg.panjiajie.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://yp.huanxung.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://kg.nicolike.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://sa.hnjuh.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://dq.chemitech.net.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://dg.jctech888.com.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://dh.9csxet.cn

[P03] 生成短随机字符串
来源：http://hq.jianghongdianzi.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://jg.jctech888.com.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://gg.shxzskj.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://dp.asd995.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wv.shxzukj.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://bp.yuntaijiaju.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://rx.chemitech.net.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://lt.yuexingan06.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ox.hnjuh.cn

[P04] 求长度
来源：http://sw.nszjky.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://or.jctech888.com.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://eu.asd995.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ak.huixinmuqiang.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://dj.colortex.cn

Java: list.size();  map.size();  s.length()
来源：http://pu.huixiangedu.cn

Go:   len(arr);  len(m)
来源：http://af.shxzukj.cn

Ruby: x.length;  x.size
来源：http://hl.shtwfgs.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://ju.huixinmuqiang.cn

[P05] 判断两个对象内容是否相等
来源：http://yg.szsharing.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://sp.521024.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://yl.huanxung.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://sg.hnjuh.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://lg.asd995.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ts.bookmarksfly.cn

Go:   reflect.DeepEqual(a, b)
来源：http://vw.yuexingan06.cn

Ruby: a == b
来源：http://gq.hahajie.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://fd.nszjky.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ke.nicolike.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ut.colortex.cn

PHP:  if (empty($x)) {}
来源：http://ib.bookmarksfly.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://vi.nicolike.cn

TS:   if (x == null) {}
来源：http://qq.gzmigu.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://bo.nszjky.cn

Go:   if x == nil {}
来源：http://lu.newstarts.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://le.szxytkj.cn

C#:   if (x is null) {}
来源：http://sy.nszjky.cn

[P07] 防抖与节流
来源：http://vo.jianghongdianzi.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://lb.newstarts.cn

PHP:  // 手写时间戳比较
来源：http://sh.gzmigu.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ke.newstarts.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hr.hnjuh.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://do.yuntaijiaju.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hw.nicolike.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://in.shtwfgs.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://sc.huixiangedu.cn

[P08] 处理浮点精度问题
来源：http://uw.521024.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ri.bookmarksfly.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://gh.szxytkj.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ky.521024.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://vx.shtwfgs.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://fr.asd995.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ir.hnjuh.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://fh.panjiajie.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://rv.huanxung.cn

================================================================================
来源：http://no.szxytkj.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://yq.asd995.cn

================================================================================
来源：http://fp.hnjuh.cn

[Q01] 创建表
来源：http://di.shxzukj.cn

CREATE TABLE users (
来源：http://ty.shxzukj.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://bo.szxytkj.cn

name VARCHAR(50) NOT NULL,
来源：http://cg.jianghongdianzi.cn

email VARCHAR(100) UNIQUE,
来源：http://or.muxihuayi.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wq.asd995.cn

);
来源：http://hu.9csxet.cn

[Q02] 创建带外键的表
来源：http://gj.muxihuayi.cn

CREATE TABLE orders (
来源：http://cw.9csxet.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ts.shxzukj.cn

user_id INT NOT NULL,
来源：http://jn.gzmigu.cn

amount DECIMAL(10, 2),
来源：http://ia.szsharing.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ja.szxytkj.cn

);
来源：http://qb.chemitech.net.cn

[Q03] 增加列
来源：http://sf.yuexingan06.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ak.jianghongdianzi.cn

[Q04] 修改列类型
来源：http://lj.521024.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://vy.huixiangedu.cn

[Q05] 重命名列
来源：http://qq.lnxyls.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ax.hnjuh.cn

[Q06] 删除列
来源：http://ft.haigaiapp.cn

ALTER TABLE users DROP COLUMN age;
来源：http://to.9csxet.cn

[Q07] 删除表
来源：http://ih.shtwfgs.cn

DROP TABLE IF EXISTS orders;
来源：http://if.521024.cn

[Q08] 创建普通索引
来源：http://zh.jianghongdianzi.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://re.hahajie.cn

[Q09] 创建唯一索引
来源：http://xn.jctech888.com.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://qm.yuntaijiaju.cn

[Q10] 插入单行
来源：http://qr.hnjuh.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ph.shtwfgs.cn

[Q11] 一次插入多行
来源：http://mc.yuexingan06.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://fr.szsharing.cn

[Q12] 插入后取自增 ID
来源：http://bv.szxytkj.cn

INSERT INTO users (name) VALUES ('C');
来源：http://rk.huixinmuqiang.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://vg.huixiangedu.cn

[Q13] 忽略重复插入
来源：http://nz.asd995.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://gl.bjjhwx.cn

[Q14] 存在则更新（upsert）
来源：http://fu.9csxet.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://jt.shxzskj.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://vk.huixinmuqiang.cn

[Q15] 查询全部
来源：http://wk.shtwfgs.cn


<!-- 参考信息 -->