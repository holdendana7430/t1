代发 wailian999

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wx.huanxung.cn

Ruby: warn "err"
来源：http://pl.nicolike.cn

C#:   Console.Error.WriteLine("err")
来源：http://bv.hnjuh.cn

[M07] 判断是否为主入口
来源：http://ng.chemitech.net.cn

Py:   if __name__ == "__main__":
来源：http://la.huanxung.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://kl.haigaiapp.cn

JS:   require.main === module
来源：http://bd.huanxung.cn

TS:   require.main === module
来源：http://kx.huixiangedu.cn

Java: public static void main(String[] args)
来源：http://ze.jctech888.com.cn

Go:   func main()
来源：http://px.lnxyls.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://qy.haigaiapp.cn

C#:   static void Main(string[] args)
来源：http://vk.jianghongdianzi.cn

[M08] 获取系统与运行时信息
来源：http://ni.gzmigu.cn

Py:   platform.system();  platform.python_version()
来源：http://ec.nszjky.cn

PHP:  PHP_OS;  phpversion();
来源：http://fp.nszjky.cn

JS:   process.platform;  process.version
来源：http://eu.lnxyls.cn

TS:   process.platform;  process.version
来源：http://nu.gzmigu.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://gd.asd995.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://qq.panjiajie.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://qu.yuntaijiaju.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://yd.asd995.cn

================================================================================
来源：http://vd.huanxung.cn

N. 数据结构与算法
来源：http://re.gzmigu.cn

================================================================================
来源：http://sc.chemitech.net.cn

[N01] 二分查找（有序数组）
来源：http://jm.jctech888.com.cn

Py:   bisect.bisect_left(arr, x)
来源：http://sq.colortex.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://px.panjiajie.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://lo.haigaiapp.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://bl.bjjhwx.cn

Java: Arrays.binarySearch(arr, x)
来源：http://rl.chemitech.net.cn

Go:   sort.SearchInts(arr, x)
来源：http://hf.huixiangedu.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://bi.panjiajie.cn

C#:   Array.BinarySearch(arr, x)
来源：http://da.muxihuayi.cn

[N02] 排序（工程实践用内置实现）
来源：http://qq.jianghongdianzi.cn

Py:   sorted(arr);  arr.sort()
来源：http://fn.yuntaijiaju.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://fm.gzmigu.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://wk.yuntaijiaju.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://cz.newstarts.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://bn.lnxyls.cn

Go:   slices.Sort(arr)
来源：http://tb.newstarts.cn

Ruby: arr.sort
来源：http://bg.shxzskj.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://ol.szxytkj.cn

[N03] 快速排序（分治示例）
来源：http://qy.jianghongdianzi.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://fx.lnxyls.cn

PHP:  // 递归实现，或用 usort
来源：http://td.shxzukj.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://an.shxzskj.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://xs.shtwfgs.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mu.bjjhwx.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://qt.shtwfgs.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://rj.shxzukj.cn

C#:   // 手写递归，或 Array.Sort
来源：http://cw.gzmigu.cn

[N04] 斐波那契数列
来源：http://oy.huixiangedu.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://pf.newstarts.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://uz.bjjhwx.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://sy.szxytkj.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://bm.shtwfgs.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ar.hahajie.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ys.bookmarksfly.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://pg.wgjwhj.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mb.yuntaijiaju.cn

[N05] 最大公约数
来源：http://fo.huixiangedu.cn

Py:   math.gcd(a, b)
来源：http://cm.panjiajie.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://qj.yuexingan06.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://nr.9csxet.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hx.nszjky.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://gb.nicolike.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://jg.jctech888.com.cn

Ruby: a.gcd(b)
来源：http://ax.huixiangedu.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ec.huixiangedu.cn

[N06] 判断回文字符串
来源：http://jw.nicolike.cn

Py:   s == s[::-1]
来源：http://ha.shxzskj.cn

PHP:  $s === strrev($s);
来源：http://kb.lnxyls.cn

JS:   s === [...s].reverse().join("")
来源：http://vh.yuntaijiaju.cn

TS:   s === [...s].reverse().join("")
来源：http://df.huixiangedu.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://vz.lnxyls.cn

Go:   // 双指针从两端比较
来源：http://el.huixinmuqiang.cn

Ruby: s == s.reverse
来源：http://ha.yuntaijiaju.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://ch.gzmigu.cn

[N07] 两数之和（返回下标）
来源：http://fc.hahajie.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://zz.lnxyls.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://gm.bjjhwx.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://kt.shxzskj.cn

TS:   // 手写 Map<string, number>
来源：http://kh.521024.cn

Java: // 手写 HashMap
来源：http://gf.panjiajie.cn

Go:   // 手写 map[int]int
来源：http://uu.shxzukj.cn

Ruby: // 手写 Hash
来源：http://eg.muxihuayi.cn

C#:   // 手写 Dictionary<int, int>
来源：http://ua.muxihuayi.cn

[N08] 生成全排列
来源：http://dr.shtwfgs.cn

Py:   itertools.permutations(arr)
来源：http://om.colortex.cn

PHP:  // 手写递归交换
来源：http://ng.muxihuayi.cn

JS:   // 手写回溯递归
来源：http://kk.gzmigu.cn

TS:   // 手写回溯递归
来源：http://ig.yuexingan06.cn

Java: // 手写回溯递归
来源：http://ol.jctech888.com.cn

Go:   // 手写回溯递归
来源：http://pb.newstarts.cn

Ruby: arr.permutation.to_a
来源：http://cc.hnjuh.cn

C#:   // 手写回溯递归
来源：http://bl.nszjky.cn

[N09] 栈与队列
来源：http://ca.muxihuayi.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://rb.chemitech.net.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wt.jctech888.com.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://xc.yuexingan06.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://fn.521024.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://gp.521024.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://kj.521024.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://gt.shxzskj.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ao.shxzskj.cn

[N10] 链表节点定义
来源：http://ux.bjjhwx.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://xg.wgjwhj.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://qj.yuexingan06.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://oe.szxytkj.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hf.shtwfgs.cn

Java: class Node { int v; Node next; }
来源：http://dn.jianghongdianzi.cn

Go:   type Node struct { V int; Next *Node }
来源：http://yq.newstarts.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://tz.yuexingan06.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://no.colortex.cn

[N11] 二叉树中序遍历
来源：http://nc.wgjwhj.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://sr.lnxyls.cn

PHP:  // 手写递归函数
来源：http://ak.yuexingan06.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://gq.panjiajie.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://cg.szxytkj.cn

Java: // 手写递归
来源：http://sz.yuexingan06.cn

Go:   // 手写递归
来源：http://ne.szsharing.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.jianghongdianzi.cn

C#:   // 手写递归
来源：http://ap.szsharing.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://oy.hahajie.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://za.panjiajie.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://le.newstarts.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://pn.nicolike.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ru.shtwfgs.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wc.521024.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ov.yuntaijiaju.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://yi.szsharing.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://jg.huanxung.cn

================================================================================
来源：http://fm.nicolike.cn

O. 并发与异步
来源：http://ht.chemitech.net.cn

================================================================================
来源：http://oo.chemitech.net.cn

[O01] 启动一个线程
来源：http://mx.gzmigu.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://yz.szxytkj.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ui.szxytkj.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://nc.muxihuayi.cn

TS:   // 同 JS
来源：http://bc.wgjwhj.cn

Java: new Thread(() -> f()).start()
来源：http://fj.bookmarksfly.cn

Go:   go f()
来源：http://bj.colortex.cn

Ruby: Thread.new { f }
来源：http://qj.521024.cn

C#:   Task.Run(() => F());
来源：http://xp.gzmigu.cn

[O02] 使用线程池
来源：http://mr.jctech888.com.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wa.szxytkj.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://an.szxytkj.cn

JS:   // worker_threads 线程池
来源：http://yj.chemitech.net.cn

TS:   // worker_threads 线程池
来源：http://gj.shxzukj.cn

Java: Executors.newFixedThreadPool(4)
来源：http://hs.521024.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://jr.521024.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://xw.huixinmuqiang.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://uw.gzmigu.cn

[O03] 加锁保护共享数据
来源：http://oy.szsharing.cn

Py:   with lock: shared += 1
来源：http://gs.szsharing.cn

PHP:  // 用 flock() 做文件锁
来源：http://xp.shxzukj.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://cg.jctech888.com.cn

TS:   // 同 JS
来源：http://vv.huixinmuqiang.cn

Java: synchronized (this) { shared++; }
来源：http://ln.jianghongdianzi.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://kh.haigaiapp.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://jd.chemitech.net.cn

C#:   lock (gate) { shared++; }
来源：http://zx.chemitech.net.cn

[O04] 定义异步函数并等待
来源：http://cq.huanxung.cn

Py:   async def f():⏎    await g()
来源：http://sq.yuexingan06.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ha.colortex.cn

JS:   async function f() { await g(); }
来源：http://sl.521024.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://mp.szsharing.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://px.lnxyls.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://lu.asd995.cn

Ruby: # 用 Fiber 或 async gem
来源：http://xu.haigaiapp.cn

C#:   async Task F() { await G(); }
来源：http://fa.huixiangedu.cn

[O05] 并发执行并等待全部完成
来源：http://pj.szsharing.cn

Py:   asyncio.gather(*tasks)
来源：http://iq.jianghongdianzi.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://re.szsharing.cn

JS:   await Promise.all(tasks)
来源：http://qa.lnxyls.cn

TS:   await Promise.all(tasks)
来源：http://ek.nszjky.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://sc.colortex.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://vu.yuntaijiaju.cn

Ruby: threads.map(&:join)
来源：http://au.szsharing.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://ea.shxzskj.cn

[O06] 使用进程池
来源：http://vs.yuntaijiaju.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://il.huixinmuqiang.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://mi.shtwfgs.cn

JS:   // child_process / cluster 模块
来源：http://ag.nicolike.cn

TS:   // child_process / cluster 模块
来源：http://un.lnxyls.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ur.haigaiapp.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ao.hnjuh.cn

Ruby: // fork 块
来源：http://sf.panjiajie.cn

C#:   Parallel.For
来源：http://dz.gzmigu.cn

================================================================================
来源：http://az.lnxyls.cn

P. 常用工具函数
来源：http://cw.521024.cn

================================================================================
来源：http://ux.bjjhwx.cn

[P01] 生成 UUID
来源：http://ut.nszjky.cn

Py:   str(uuid.uuid4())
来源：http://sr.asd995.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://fa.panjiajie.cn

JS:   crypto.randomUUID()
来源：http://rm.hnjuh.cn

TS:   crypto.randomUUID()
来源：http://wz.hnjuh.cn

Java: UUID.randomUUID().toString()
来源：http://bq.yuntaijiaju.cn

Go:   // 用 github.com/google/uuid
来源：http://hv.bookmarksfly.cn

Ruby: SecureRandom.uuid
来源：http://tc.yuexingan06.cn

C#:   Guid.NewGuid().ToString()
来源：http://vi.newstarts.cn

[P02] MD5 / SHA256 摘要
来源：http://px.muxihuayi.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ns.huixiangedu.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://kc.jctech888.com.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://tk.shxzukj.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ud.bookmarksfly.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://bu.muxihuayi.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://in.nicolike.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://pr.huixinmuqiang.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hs.szxytkj.cn

[P03] 生成短随机字符串
来源：http://ie.szsharing.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://be.chemitech.net.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://tq.shxzukj.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://qm.9csxet.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://lb.newstarts.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://bl.jctech888.com.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ns.shtwfgs.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://ah.huanxung.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://gy.lnxyls.cn

[P04] 求长度
来源：http://yo.szxytkj.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://bv.panjiajie.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mv.newstarts.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://pt.jctech888.com.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://pm.jctech888.com.cn

Java: list.size();  map.size();  s.length()
来源：http://qu.jianghongdianzi.cn

Go:   len(arr);  len(m)
来源：http://bv.wgjwhj.cn

Ruby: x.length;  x.size
来源：http://sd.lnxyls.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://pn.chemitech.net.cn

[P05] 判断两个对象内容是否相等
来源：http://io.chemitech.net.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://fo.yuntaijiaju.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://jz.gzmigu.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://im.bookmarksfly.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://qe.chemitech.net.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ao.huanxung.cn

Go:   reflect.DeepEqual(a, b)
来源：http://pm.huixiangedu.cn

Ruby: a == b
来源：http://vs.huanxung.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ee.huixiangedu.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://xc.huixinmuqiang.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://lq.bjjhwx.cn

PHP:  if (empty($x)) {}
来源：http://oz.nszjky.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mv.hnjuh.cn

TS:   if (x == null) {}
来源：http://zw.jctech888.com.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://up.huixinmuqiang.cn

Go:   if x == nil {}
来源：http://ll.shtwfgs.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://zi.muxihuayi.cn

C#:   if (x is null) {}
来源：http://aw.lnxyls.cn

[P07] 防抖与节流
来源：http://zy.asd995.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ev.huixinmuqiang.cn

PHP:  // 手写时间戳比较
来源：http://cm.yuntaijiaju.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://cf.hahajie.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://dk.panjiajie.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wi.haigaiapp.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ml.newstarts.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://rw.asd995.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://di.yuexingan06.cn

[P08] 处理浮点精度问题
来源：http://yu.colortex.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://bk.bjjhwx.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://qn.bjjhwx.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://fr.muxihuayi.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://vy.lnxyls.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://rf.jctech888.com.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://nd.chemitech.net.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://kd.hnjuh.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://om.szsharing.cn

================================================================================
来源：http://wh.521024.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://sb.yuntaijiaju.cn

================================================================================
来源：http://uu.newstarts.cn

[Q01] 创建表
来源：http://lm.nszjky.cn

CREATE TABLE users (
来源：http://zm.jianghongdianzi.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://re.chemitech.net.cn

name VARCHAR(50) NOT NULL,
来源：http://sh.panjiajie.cn

email VARCHAR(100) UNIQUE,
来源：http://aa.jctech888.com.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://fb.muxihuayi.cn

);
来源：http://wl.9csxet.cn

[Q02] 创建带外键的表
来源：http://nv.gzmigu.cn

CREATE TABLE orders (
来源：http://ua.hahajie.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://oc.yuexingan06.cn

user_id INT NOT NULL,
来源：http://eu.lnxyls.cn

amount DECIMAL(10, 2),
来源：http://cm.muxihuayi.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://vg.chemitech.net.cn

);
来源：http://aj.bookmarksfly.cn

[Q03] 增加列
来源：http://kj.colortex.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ee.nicolike.cn

[Q04] 修改列类型
来源：http://sx.huixinmuqiang.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://dy.lnxyls.cn

[Q05] 重命名列
来源：http://zj.bjjhwx.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://lz.jianghongdianzi.cn

[Q06] 删除列
来源：http://dd.yuexingan06.cn

ALTER TABLE users DROP COLUMN age;
来源：http://zl.hnjuh.cn

[Q07] 删除表
来源：http://lp.huixiangedu.cn

DROP TABLE IF EXISTS orders;
来源：http://li.huixiangedu.cn

[Q08] 创建普通索引
来源：http://bq.shtwfgs.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://ju.newstarts.cn

[Q09] 创建唯一索引
来源：http://qz.panjiajie.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ra.521024.cn

[Q10] 插入单行
来源：http://lt.shxzukj.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://yb.bookmarksfly.cn

[Q11] 一次插入多行
来源：http://lv.bookmarksfly.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://kl.nszjky.cn

[Q12] 插入后取自增 ID
来源：http://fx.nicolike.cn


<!-- 参考信息 -->