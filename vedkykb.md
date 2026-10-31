代发 wailian999

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ph.bookmarksfly.cn

Ruby: warn "err"
来源：http://vh.bookmarksfly.cn

C#:   Console.Error.WriteLine("err")
来源：http://yw.wgjwhj.cn

[M07] 判断是否为主入口
来源：http://or.colortex.cn

Py:   if __name__ == "__main__":
来源：http://vy.szsharing.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://zv.shxzukj.cn

JS:   require.main === module
来源：http://tu.jianghongdianzi.cn

TS:   require.main === module
来源：http://hl.szsharing.cn

Java: public static void main(String[] args)
来源：http://yd.nszjky.cn

Go:   func main()
来源：http://tj.huanxung.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://qj.bookmarksfly.cn

C#:   static void Main(string[] args)
来源：http://bi.shxzskj.cn

[M08] 获取系统与运行时信息
来源：http://kx.newstarts.cn

Py:   platform.system();  platform.python_version()
来源：http://eo.shxzskj.cn

PHP:  PHP_OS;  phpversion();
来源：http://bq.lnxyls.cn

JS:   process.platform;  process.version
来源：http://ks.nszjky.cn

TS:   process.platform;  process.version
来源：http://gp.yuntaijiaju.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ll.bjjhwx.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://fp.colortex.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://th.chemitech.net.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://rn.yuexingan06.cn

================================================================================
来源：http://rx.shtwfgs.cn

N. 数据结构与算法
来源：http://qg.521024.cn

================================================================================
来源：http://dc.nszjky.cn

[N01] 二分查找（有序数组）
来源：http://mr.gzmigu.cn

Py:   bisect.bisect_left(arr, x)
来源：http://uj.gzmigu.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://zr.haigaiapp.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://lh.szsharing.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://xn.newstarts.cn

Java: Arrays.binarySearch(arr, x)
来源：http://rr.hahajie.cn

Go:   sort.SearchInts(arr, x)
来源：http://bn.wgjwhj.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://cf.hahajie.cn

C#:   Array.BinarySearch(arr, x)
来源：http://ge.lnxyls.cn

[N02] 排序（工程实践用内置实现）
来源：http://ip.wgjwhj.cn

Py:   sorted(arr);  arr.sort()
来源：http://rv.shxzskj.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ua.hnjuh.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://sb.szsharing.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://hv.jianghongdianzi.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://we.shxzukj.cn

Go:   slices.Sort(arr)
来源：http://zg.panjiajie.cn

Ruby: arr.sort
来源：http://lo.9csxet.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://np.szsharing.cn

[N03] 快速排序（分治示例）
来源：http://wp.huanxung.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://sz.colortex.cn

PHP:  // 递归实现，或用 usort
来源：http://bx.muxihuayi.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mk.newstarts.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://jk.yuntaijiaju.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://lt.szxytkj.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ng.yuntaijiaju.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://fn.9csxet.cn

C#:   // 手写递归，或 Array.Sort
来源：http://hq.muxihuayi.cn

[N04] 斐波那契数列
来源：http://pl.newstarts.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://og.yuexingan06.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://yn.jctech888.com.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ap.lnxyls.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://fn.hnjuh.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://pj.hnjuh.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://co.haigaiapp.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://bv.nszjky.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://pv.chemitech.net.cn

[N05] 最大公约数
来源：http://pa.yuntaijiaju.cn

Py:   math.gcd(a, b)
来源：http://mp.huixiangedu.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://lu.jctech888.com.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ym.newstarts.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hx.szxytkj.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://um.haigaiapp.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://oj.chemitech.net.cn

Ruby: a.gcd(b)
来源：http://sf.colortex.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://qi.yuntaijiaju.cn

[N06] 判断回文字符串
来源：http://uz.haigaiapp.cn

Py:   s == s[::-1]
来源：http://bo.colortex.cn

PHP:  $s === strrev($s);
来源：http://eq.huanxung.cn

JS:   s === [...s].reverse().join("")
来源：http://eq.gzmigu.cn

TS:   s === [...s].reverse().join("")
来源：http://kq.shxzskj.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ot.huixiangedu.cn

Go:   // 双指针从两端比较
来源：http://hq.szxytkj.cn

Ruby: s == s.reverse
来源：http://vu.wgjwhj.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://nz.asd995.cn

[N07] 两数之和（返回下标）
来源：http://fz.hahajie.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://xl.shxzskj.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wi.newstarts.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://ul.szsharing.cn

TS:   // 手写 Map<string, number>
来源：http://iz.colortex.cn

Java: // 手写 HashMap
来源：http://rd.shxzskj.cn

Go:   // 手写 map[int]int
来源：http://la.yuntaijiaju.cn

Ruby: // 手写 Hash
来源：http://ak.haigaiapp.cn

C#:   // 手写 Dictionary<int, int>
来源：http://at.muxihuayi.cn

[N08] 生成全排列
来源：http://bm.nicolike.cn

Py:   itertools.permutations(arr)
来源：http://zc.szsharing.cn

PHP:  // 手写递归交换
来源：http://rj.muxihuayi.cn

JS:   // 手写回溯递归
来源：http://ns.huixiangedu.cn

TS:   // 手写回溯递归
来源：http://te.nszjky.cn

Java: // 手写回溯递归
来源：http://dx.newstarts.cn

Go:   // 手写回溯递归
来源：http://fx.colortex.cn

Ruby: arr.permutation.to_a
来源：http://pl.521024.cn

C#:   // 手写回溯递归
来源：http://ww.521024.cn

[N09] 栈与队列
来源：http://mk.haigaiapp.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://bo.nszjky.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://kb.nicolike.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://kp.muxihuayi.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ot.huixinmuqiang.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://tq.haigaiapp.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://bc.jianghongdianzi.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://dk.chemitech.net.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://kt.wgjwhj.cn

[N10] 链表节点定义
来源：http://no.hnjuh.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://lv.jctech888.com.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://cn.colortex.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://gu.haigaiapp.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ko.bjjhwx.cn

Java: class Node { int v; Node next; }
来源：http://bh.9csxet.cn

Go:   type Node struct { V int; Next *Node }
来源：http://vp.panjiajie.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://so.nszjky.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://zq.szxytkj.cn

[N11] 二叉树中序遍历
来源：http://xy.9csxet.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://yy.szsharing.cn

PHP:  // 手写递归函数
来源：http://mf.shxzskj.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://zx.shxzskj.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://vg.wgjwhj.cn

Java: // 手写递归
来源：http://tf.szsharing.cn

Go:   // 手写递归
来源：http://gs.chemitech.net.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ev.haigaiapp.cn

C#:   // 手写递归
来源：http://vv.jctech888.com.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://oh.hahajie.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://eq.shxzukj.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://in.gzmigu.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ul.shxzskj.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://tx.bjjhwx.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://qi.shxzukj.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://up.szsharing.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://gm.shtwfgs.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://bs.bjjhwx.cn

================================================================================
来源：http://gm.shxzukj.cn

O. 并发与异步
来源：http://up.lnxyls.cn

================================================================================
来源：http://pc.9csxet.cn

[O01] 启动一个线程
来源：http://ra.bjjhwx.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wf.huanxung.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://cl.nicolike.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://sr.newstarts.cn

TS:   // 同 JS
来源：http://yz.muxihuayi.cn

Java: new Thread(() -> f()).start()
来源：http://ys.yuexingan06.cn

Go:   go f()
来源：http://it.bjjhwx.cn

Ruby: Thread.new { f }
来源：http://fx.szsharing.cn

C#:   Task.Run(() => F());
来源：http://ao.szsharing.cn

[O02] 使用线程池
来源：http://ci.chemitech.net.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://tt.shxzskj.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://nl.shxzukj.cn

JS:   // worker_threads 线程池
来源：http://tu.huanxung.cn

TS:   // worker_threads 线程池
来源：http://xy.hahajie.cn

Java: Executors.newFixedThreadPool(4)
来源：http://hb.nicolike.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://he.gzmigu.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hu.huixinmuqiang.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hc.yuntaijiaju.cn

[O03] 加锁保护共享数据
来源：http://eu.szsharing.cn

Py:   with lock: shared += 1
来源：http://dd.521024.cn

PHP:  // 用 flock() 做文件锁
来源：http://zr.hahajie.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wn.shxzukj.cn

TS:   // 同 JS
来源：http://uq.huanxung.cn

Java: synchronized (this) { shared++; }
来源：http://sb.nicolike.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://eh.nszjky.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://uh.hahajie.cn

C#:   lock (gate) { shared++; }
来源：http://oc.jianghongdianzi.cn

[O04] 定义异步函数并等待
来源：http://fg.jianghongdianzi.cn

Py:   async def f():⏎    await g()
来源：http://xh.haigaiapp.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://go.jctech888.com.cn

JS:   async function f() { await g(); }
来源：http://jq.lnxyls.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://tf.yuexingan06.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://yz.hnjuh.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://lq.asd995.cn

Ruby: # 用 Fiber 或 async gem
来源：http://zn.panjiajie.cn

C#:   async Task F() { await G(); }
来源：http://us.hahajie.cn

[O05] 并发执行并等待全部完成
来源：http://cl.jianghongdianzi.cn

Py:   asyncio.gather(*tasks)
来源：http://fh.9csxet.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://cn.shxzskj.cn

JS:   await Promise.all(tasks)
来源：http://gl.bookmarksfly.cn

TS:   await Promise.all(tasks)
来源：http://yk.panjiajie.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wn.yuexingan06.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ms.huixiangedu.cn

Ruby: threads.map(&:join)
来源：http://rr.huixiangedu.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://pf.lnxyls.cn

[O06] 使用进程池
来源：http://gk.huanxung.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ij.huixinmuqiang.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://oa.hahajie.cn

JS:   // child_process / cluster 模块
来源：http://ix.panjiajie.cn

TS:   // child_process / cluster 模块
来源：http://kl.huixiangedu.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ew.gzmigu.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mv.szxytkj.cn

Ruby: // fork 块
来源：http://ph.9csxet.cn

C#:   Parallel.For
来源：http://gc.huixiangedu.cn

================================================================================
来源：http://vr.shtwfgs.cn

P. 常用工具函数
来源：http://vu.haigaiapp.cn

================================================================================
来源：http://bd.9csxet.cn

[P01] 生成 UUID
来源：http://xm.newstarts.cn

Py:   str(uuid.uuid4())
来源：http://yv.asd995.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ld.szsharing.cn

JS:   crypto.randomUUID()
来源：http://um.jianghongdianzi.cn

TS:   crypto.randomUUID()
来源：http://hw.nszjky.cn

Java: UUID.randomUUID().toString()
来源：http://mj.asd995.cn

Go:   // 用 github.com/google/uuid
来源：http://km.panjiajie.cn

Ruby: SecureRandom.uuid
来源：http://vq.bookmarksfly.cn

C#:   Guid.NewGuid().ToString()
来源：http://ta.newstarts.cn

[P02] MD5 / SHA256 摘要
来源：http://cu.shtwfgs.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://en.yuexingan06.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://co.nicolike.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://jf.shxzukj.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ps.nicolike.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wb.shtwfgs.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://dr.newstarts.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://do.nszjky.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://cu.panjiajie.cn

[P03] 生成短随机字符串
来源：http://ce.newstarts.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wp.chemitech.net.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://tr.wgjwhj.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://kc.bookmarksfly.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ah.huixiangedu.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ua.haigaiapp.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://uk.panjiajie.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://ex.haigaiapp.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://xr.gzmigu.cn

[P04] 求长度
来源：http://kr.colortex.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ah.colortex.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hd.newstarts.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ur.lnxyls.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://gx.hahajie.cn

Java: list.size();  map.size();  s.length()
来源：http://dt.9csxet.cn

Go:   len(arr);  len(m)
来源：http://ct.bjjhwx.cn

Ruby: x.length;  x.size
来源：http://iw.521024.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://bt.asd995.cn

[P05] 判断两个对象内容是否相等
来源：http://ve.colortex.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://cr.jianghongdianzi.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://gz.newstarts.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://km.521024.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ys.yuexingan06.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://sn.9csxet.cn

Go:   reflect.DeepEqual(a, b)
来源：http://kb.muxihuayi.cn

Ruby: a == b
来源：http://tq.muxihuayi.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://oc.muxihuayi.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://qk.muxihuayi.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mo.wgjwhj.cn

PHP:  if (empty($x)) {}
来源：http://rf.panjiajie.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://bn.521024.cn

TS:   if (x == null) {}
来源：http://sl.lnxyls.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://by.huixinmuqiang.cn

Go:   if x == nil {}
来源：http://ko.szxytkj.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://qp.shxzukj.cn

C#:   if (x is null) {}
来源：http://bg.newstarts.cn

[P07] 防抖与节流
来源：http://wi.jianghongdianzi.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ol.hnjuh.cn

PHP:  // 手写时间戳比较
来源：http://fi.newstarts.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://jw.jctech888.com.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://nz.panjiajie.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://nn.gzmigu.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://sd.wgjwhj.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://sz.huixinmuqiang.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://yv.newstarts.cn

[P08] 处理浮点精度问题
来源：http://kp.shxzskj.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://td.9csxet.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://io.chemitech.net.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://bj.yuexingan06.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://um.szxytkj.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://bq.hnjuh.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://sh.jctech888.com.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://gt.nicolike.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://qz.huanxung.cn

================================================================================
来源：http://av.nicolike.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://tr.gzmigu.cn

================================================================================
来源：http://rv.jianghongdianzi.cn

[Q01] 创建表
来源：http://xg.521024.cn

CREATE TABLE users (
来源：http://xw.gzmigu.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://fi.shxzskj.cn

name VARCHAR(50) NOT NULL,
来源：http://zw.yuntaijiaju.cn

email VARCHAR(100) UNIQUE,
来源：http://il.yuexingan06.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://sx.nicolike.cn

);
来源：http://pc.yuexingan06.cn

[Q02] 创建带外键的表
来源：http://yt.chemitech.net.cn

CREATE TABLE orders (
来源：http://wi.wgjwhj.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://rs.chemitech.net.cn

user_id INT NOT NULL,
来源：http://dv.huanxung.cn

amount DECIMAL(10, 2),
来源：http://nf.huixiangedu.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://qo.jianghongdianzi.cn

);
来源：http://di.wgjwhj.cn

[Q03] 增加列
来源：http://pe.gzmigu.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://qk.szxytkj.cn

[Q04] 修改列类型
来源：http://xd.colortex.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ar.wgjwhj.cn

[Q05] 重命名列
来源：http://xo.nszjky.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://lu.colortex.cn

[Q06] 删除列
来源：http://lu.szsharing.cn

ALTER TABLE users DROP COLUMN age;
来源：http://gi.shxzukj.cn

[Q07] 删除表
来源：http://qb.colortex.cn

DROP TABLE IF EXISTS orders;
来源：http://aq.chemitech.net.cn

[Q08] 创建普通索引
来源：http://qj.panjiajie.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://su.szxytkj.cn

[Q09] 创建唯一索引
来源：http://cw.colortex.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mq.muxihuayi.cn

[Q10] 插入单行
来源：http://gt.jianghongdianzi.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://tg.shtwfgs.cn

[Q11] 一次插入多行
来源：http://sf.shtwfgs.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://vf.nicolike.cn

[Q12] 插入后取自增 ID
来源：http://db.shtwfgs.cn


<!-- 参考信息 -->