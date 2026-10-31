代发 wailian999

JS:   process.exit(1)
来源：http://ud.newstarts.cn

TS:   process.exit(1)
来源：http://tt.szxytkj.cn

Java: System.exit(1)
来源：http://rk.shxzskj.cn

Go:   os.Exit(1)
来源：http://xc.hnjuh.cn

Ruby: exit 1
来源：http://gf.hnjuh.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://gp.bjjhwx.cn

[M06] 向标准错误输出
来源：http://ds.hnjuh.cn

Py:   print("err", file=sys.stderr)
来源：http://lg.wgjwhj.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://pv.hnjuh.cn

JS:   console.error("err")
来源：http://mh.9csxet.cn

TS:   console.error("err")
来源：http://qy.yuexingan06.cn

Java: System.err.println("err")
来源：http://bo.newstarts.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://oy.gzmigu.cn

Ruby: warn "err"
来源：http://wz.asd995.cn

C#:   Console.Error.WriteLine("err")
来源：http://cr.szxytkj.cn

[M07] 判断是否为主入口
来源：http://af.nszjky.cn

Py:   if __name__ == "__main__":
来源：http://ry.bookmarksfly.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://it.huanxung.cn

JS:   require.main === module
来源：http://am.szxytkj.cn

TS:   require.main === module
来源：http://za.asd995.cn

Java: public static void main(String[] args)
来源：http://zv.gzmigu.cn

Go:   func main()
来源：http://wx.bookmarksfly.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ce.haigaiapp.cn

C#:   static void Main(string[] args)
来源：http://hg.jctech888.com.cn

[M08] 获取系统与运行时信息
来源：http://iv.nszjky.cn

Py:   platform.system();  platform.python_version()
来源：http://rt.muxihuayi.cn

PHP:  PHP_OS;  phpversion();
来源：http://yn.hnjuh.cn

JS:   process.platform;  process.version
来源：http://wp.yuntaijiaju.cn

TS:   process.platform;  process.version
来源：http://re.newstarts.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://kh.chemitech.net.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://cx.huixiangedu.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mx.colortex.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://wi.9csxet.cn

================================================================================
来源：http://ag.nicolike.cn

N. 数据结构与算法
来源：http://hs.nszjky.cn

================================================================================
来源：http://uc.lnxyls.cn

[N01] 二分查找（有序数组）
来源：http://tb.huanxung.cn

Py:   bisect.bisect_left(arr, x)
来源：http://rj.szxytkj.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ko.chemitech.net.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://xk.chemitech.net.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://rz.521024.cn

Java: Arrays.binarySearch(arr, x)
来源：http://kg.colortex.cn

Go:   sort.SearchInts(arr, x)
来源：http://qr.chemitech.net.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://zz.9csxet.cn

C#:   Array.BinarySearch(arr, x)
来源：http://ml.jctech888.com.cn

[N02] 排序（工程实践用内置实现）
来源：http://gc.jianghongdianzi.cn

Py:   sorted(arr);  arr.sort()
来源：http://do.chemitech.net.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://cp.shtwfgs.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://xd.yuntaijiaju.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://ov.huixinmuqiang.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wy.hnjuh.cn

Go:   slices.Sort(arr)
来源：http://gt.shtwfgs.cn

Ruby: arr.sort
来源：http://ff.shtwfgs.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://kg.shxzukj.cn

[N03] 快速排序（分治示例）
来源：http://ad.9csxet.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://od.huixiangedu.cn

PHP:  // 递归实现，或用 usort
来源：http://yz.nicolike.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ab.haigaiapp.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ns.yuntaijiaju.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hf.muxihuayi.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://gj.asd995.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mb.szxytkj.cn

C#:   // 手写递归，或 Array.Sort
来源：http://dx.bjjhwx.cn

[N04] 斐波那契数列
来源：http://wy.shxzukj.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://vu.521024.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://bd.shxzukj.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://bn.521024.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mz.huanxung.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://di.nicolike.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ix.nszjky.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ks.shxzukj.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://el.szxytkj.cn

[N05] 最大公约数
来源：http://ez.huixiangedu.cn

Py:   math.gcd(a, b)
来源：http://fd.chemitech.net.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://rw.huixinmuqiang.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hu.huixinmuqiang.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://th.haigaiapp.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://bc.nicolike.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://in.hnjuh.cn

Ruby: a.gcd(b)
来源：http://or.asd995.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ov.gzmigu.cn

[N06] 判断回文字符串
来源：http://hj.jianghongdianzi.cn

Py:   s == s[::-1]
来源：http://xp.shxzukj.cn

PHP:  $s === strrev($s);
来源：http://ra.9csxet.cn

JS:   s === [...s].reverse().join("")
来源：http://ml.haigaiapp.cn

TS:   s === [...s].reverse().join("")
来源：http://gh.lnxyls.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://js.nszjky.cn

Go:   // 双指针从两端比较
来源：http://lm.nicolike.cn

Ruby: s == s.reverse
来源：http://hy.jctech888.com.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://cj.shxzskj.cn

[N07] 两数之和（返回下标）
来源：http://ee.gzmigu.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ll.panjiajie.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hi.huixinmuqiang.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://lm.szsharing.cn

TS:   // 手写 Map<string, number>
来源：http://en.lnxyls.cn

Java: // 手写 HashMap
来源：http://lc.chemitech.net.cn

Go:   // 手写 map[int]int
来源：http://ni.hahajie.cn

Ruby: // 手写 Hash
来源：http://kb.nicolike.cn

C#:   // 手写 Dictionary<int, int>
来源：http://no.lnxyls.cn

[N08] 生成全排列
来源：http://ck.9csxet.cn

Py:   itertools.permutations(arr)
来源：http://cn.shtwfgs.cn

PHP:  // 手写递归交换
来源：http://bj.lnxyls.cn

JS:   // 手写回溯递归
来源：http://om.szxytkj.cn

TS:   // 手写回溯递归
来源：http://fr.wgjwhj.cn

Java: // 手写回溯递归
来源：http://nm.nicolike.cn

Go:   // 手写回溯递归
来源：http://ii.hnjuh.cn

Ruby: arr.permutation.to_a
来源：http://hi.9csxet.cn

C#:   // 手写回溯递归
来源：http://np.huanxung.cn

[N09] 栈与队列
来源：http://yb.bjjhwx.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://py.hnjuh.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://zw.newstarts.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://zb.muxihuayi.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://uu.shxzskj.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://vg.lnxyls.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://si.shxzukj.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://rp.wgjwhj.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://pn.shxzskj.cn

[N10] 链表节点定义
来源：http://dw.chemitech.net.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://cy.shxzukj.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://ve.shxzskj.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://da.hnjuh.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://gj.lnxyls.cn

Java: class Node { int v; Node next; }
来源：http://ga.chemitech.net.cn

Go:   type Node struct { V int; Next *Node }
来源：http://ql.asd995.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://dy.521024.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://oy.yuntaijiaju.cn

[N11] 二叉树中序遍历
来源：http://op.yuntaijiaju.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://dq.wgjwhj.cn

PHP:  // 手写递归函数
来源：http://mz.jctech888.com.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://uy.9csxet.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://xq.hahajie.cn

Java: // 手写递归
来源：http://xk.haigaiapp.cn

Go:   // 手写递归
来源：http://vd.shxzukj.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://gg.yuexingan06.cn

C#:   // 手写递归
来源：http://qg.colortex.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hr.wgjwhj.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hp.asd995.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://pu.lnxyls.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://lu.nicolike.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://yl.shxzskj.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://rn.nszjky.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://vn.colortex.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wl.bookmarksfly.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://rt.szxytkj.cn

================================================================================
来源：http://xl.nicolike.cn

O. 并发与异步
来源：http://vz.521024.cn

================================================================================
来源：http://ks.colortex.cn

[O01] 启动一个线程
来源：http://xp.bookmarksfly.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://vd.asd995.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://gd.szxytkj.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ar.hnjuh.cn

TS:   // 同 JS
来源：http://jo.newstarts.cn

Java: new Thread(() -> f()).start()
来源：http://nl.jianghongdianzi.cn

Go:   go f()
来源：http://wh.521024.cn

Ruby: Thread.new { f }
来源：http://fh.panjiajie.cn

C#:   Task.Run(() => F());
来源：http://at.jctech888.com.cn

[O02] 使用线程池
来源：http://xb.chemitech.net.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://sm.muxihuayi.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://jq.hnjuh.cn

JS:   // worker_threads 线程池
来源：http://ot.nszjky.cn

TS:   // worker_threads 线程池
来源：http://qc.shxzukj.cn

Java: Executors.newFixedThreadPool(4)
来源：http://lk.9csxet.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ul.hahajie.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://kz.wgjwhj.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://zz.bookmarksfly.cn

[O03] 加锁保护共享数据
来源：http://xr.lnxyls.cn

Py:   with lock: shared += 1
来源：http://vs.asd995.cn

PHP:  // 用 flock() 做文件锁
来源：http://co.bookmarksfly.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://bm.yuexingan06.cn

TS:   // 同 JS
来源：http://tg.jctech888.com.cn

Java: synchronized (this) { shared++; }
来源：http://sf.szxytkj.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://tr.9csxet.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://ss.haigaiapp.cn

C#:   lock (gate) { shared++; }
来源：http://cg.jianghongdianzi.cn

[O04] 定义异步函数并等待
来源：http://iq.chemitech.net.cn

Py:   async def f():⏎    await g()
来源：http://aj.yuexingan06.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://pa.jctech888.com.cn

JS:   async function f() { await g(); }
来源：http://gi.521024.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://sn.asd995.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wn.newstarts.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://bb.muxihuayi.cn

Ruby: # 用 Fiber 或 async gem
来源：http://rr.bookmarksfly.cn

C#:   async Task F() { await G(); }
来源：http://zr.huixinmuqiang.cn

[O05] 并发执行并等待全部完成
来源：http://qu.szxytkj.cn

Py:   asyncio.gather(*tasks)
来源：http://th.shtwfgs.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://tn.muxihuayi.cn

JS:   await Promise.all(tasks)
来源：http://wy.nszjky.cn

TS:   await Promise.all(tasks)
来源：http://xz.lnxyls.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ad.chemitech.net.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://xy.asd995.cn

Ruby: threads.map(&:join)
来源：http://wu.chemitech.net.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://op.hahajie.cn

[O06] 使用进程池
来源：http://la.hnjuh.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://se.jctech888.com.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://bx.hahajie.cn

JS:   // child_process / cluster 模块
来源：http://ax.yuntaijiaju.cn

TS:   // child_process / cluster 模块
来源：http://ap.yuntaijiaju.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://qp.jianghongdianzi.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://dm.nszjky.cn

Ruby: // fork 块
来源：http://wc.muxihuayi.cn

C#:   Parallel.For
来源：http://ns.haigaiapp.cn

================================================================================
来源：http://jw.huanxung.cn

P. 常用工具函数
来源：http://so.nicolike.cn

================================================================================
来源：http://pv.huanxung.cn

[P01] 生成 UUID
来源：http://ft.panjiajie.cn

Py:   str(uuid.uuid4())
来源：http://fx.muxihuayi.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://bk.bookmarksfly.cn

JS:   crypto.randomUUID()
来源：http://df.yuexingan06.cn

TS:   crypto.randomUUID()
来源：http://pz.hnjuh.cn

Java: UUID.randomUUID().toString()
来源：http://vr.colortex.cn

Go:   // 用 github.com/google/uuid
来源：http://eu.hnjuh.cn

Ruby: SecureRandom.uuid
来源：http://gt.nszjky.cn

C#:   Guid.NewGuid().ToString()
来源：http://od.haigaiapp.cn

[P02] MD5 / SHA256 摘要
来源：http://qc.gzmigu.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://vl.gzmigu.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://er.jctech888.com.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ij.yuntaijiaju.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://uy.hahajie.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://pf.shtwfgs.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://iy.shxzukj.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ev.wgjwhj.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://vo.hahajie.cn

[P03] 生成短随机字符串
来源：http://fd.asd995.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://gc.521024.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ma.shxzukj.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ro.lnxyls.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://qd.shtwfgs.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://zf.panjiajie.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://kv.nszjky.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://ya.shxzukj.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ji.shtwfgs.cn

[P04] 求长度
来源：http://yx.panjiajie.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://rh.haigaiapp.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ic.muxihuayi.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://kb.newstarts.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mi.wgjwhj.cn

Java: list.size();  map.size();  s.length()
来源：http://ic.jctech888.com.cn

Go:   len(arr);  len(m)
来源：http://ko.bookmarksfly.cn

Ruby: x.length;  x.size
来源：http://bb.bookmarksfly.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://wy.lnxyls.cn

[P05] 判断两个对象内容是否相等
来源：http://vf.chemitech.net.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://uy.szsharing.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://cw.szxytkj.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://jl.shxzskj.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://zv.521024.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ko.shxzukj.cn

Go:   reflect.DeepEqual(a, b)
来源：http://bn.szxytkj.cn

Ruby: a == b
来源：http://xg.jianghongdianzi.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://lc.gzmigu.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://xx.bookmarksfly.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ot.wgjwhj.cn

PHP:  if (empty($x)) {}
来源：http://ef.szxytkj.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://og.nicolike.cn

TS:   if (x == null) {}
来源：http://bv.huixinmuqiang.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://yy.9csxet.cn

Go:   if x == nil {}
来源：http://ov.9csxet.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://po.shxzukj.cn

C#:   if (x is null) {}
来源：http://oj.nicolike.cn

[P07] 防抖与节流
来源：http://qo.szsharing.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://nz.9csxet.cn

PHP:  // 手写时间戳比较
来源：http://mh.gzmigu.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ir.bookmarksfly.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ij.hnjuh.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://vr.lnxyls.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://po.panjiajie.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://sq.chemitech.net.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://xb.521024.cn

[P08] 处理浮点精度问题
来源：http://no.jianghongdianzi.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://bs.muxihuayi.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://fi.hnjuh.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://qu.colortex.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://bm.jctech888.com.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ke.gzmigu.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://jo.shtwfgs.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ij.shtwfgs.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://vl.lnxyls.cn

================================================================================
来源：http://hh.shtwfgs.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://qj.huanxung.cn

================================================================================
来源：http://xj.panjiajie.cn

[Q01] 创建表
来源：http://cs.lnxyls.cn

CREATE TABLE users (
来源：http://yc.asd995.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ro.chemitech.net.cn

name VARCHAR(50) NOT NULL,
来源：http://ne.chemitech.net.cn

email VARCHAR(100) UNIQUE,
来源：http://vw.yuexingan06.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://if.huixiangedu.cn

);
来源：http://co.panjiajie.cn

[Q02] 创建带外键的表
来源：http://wj.521024.cn

CREATE TABLE orders (
来源：http://nn.gzmigu.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ky.colortex.cn

user_id INT NOT NULL,
来源：http://ly.jianghongdianzi.cn

amount DECIMAL(10, 2),
来源：http://ol.shtwfgs.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://vv.hahajie.cn

);
来源：http://ve.huixinmuqiang.cn

[Q03] 增加列
来源：http://pn.szxytkj.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://bu.haigaiapp.cn

[Q04] 修改列类型
来源：http://re.yuntaijiaju.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://po.yuexingan06.cn

[Q05] 重命名列
来源：http://tc.gzmigu.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://gl.newstarts.cn

[Q06] 删除列
来源：http://tm.chemitech.net.cn


<!-- 参考信息 -->