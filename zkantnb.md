代发 wailian999

Ruby: exit 1
来源：http://qs.yuexingan06.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ti.521024.cn

[M06] 向标准错误输出
来源：http://ex.yuexingan06.cn

Py:   print("err", file=sys.stderr)
来源：http://os.huanxung.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://by.hahajie.cn

JS:   console.error("err")
来源：http://av.jianghongdianzi.cn

TS:   console.error("err")
来源：http://is.shtwfgs.cn

Java: System.err.println("err")
来源：http://bk.hnjuh.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://yf.huanxung.cn

Ruby: warn "err"
来源：http://az.yuexingan06.cn

C#:   Console.Error.WriteLine("err")
来源：http://af.haigaiapp.cn

[M07] 判断是否为主入口
来源：http://hl.nicolike.cn

Py:   if __name__ == "__main__":
来源：http://md.szxytkj.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wd.huixiangedu.cn

JS:   require.main === module
来源：http://kr.wgjwhj.cn

TS:   require.main === module
来源：http://kc.colortex.cn

Java: public static void main(String[] args)
来源：http://vg.muxihuayi.cn

Go:   func main()
来源：http://lv.haigaiapp.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ca.asd995.cn

C#:   static void Main(string[] args)
来源：http://al.gzmigu.cn

[M08] 获取系统与运行时信息
来源：http://he.szxytkj.cn

Py:   platform.system();  platform.python_version()
来源：http://mn.asd995.cn

PHP:  PHP_OS;  phpversion();
来源：http://cb.bookmarksfly.cn

JS:   process.platform;  process.version
来源：http://gc.hahajie.cn

TS:   process.platform;  process.version
来源：http://rb.bjjhwx.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://uq.szsharing.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://uo.chemitech.net.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ms.wgjwhj.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://gd.colortex.cn

================================================================================
来源：http://sr.wgjwhj.cn

N. 数据结构与算法
来源：http://em.nszjky.cn

================================================================================
来源：http://ic.newstarts.cn

[N01] 二分查找（有序数组）
来源：http://js.shxzukj.cn

Py:   bisect.bisect_left(arr, x)
来源：http://nk.asd995.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mj.jianghongdianzi.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://sm.asd995.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://kr.newstarts.cn

Java: Arrays.binarySearch(arr, x)
来源：http://pa.colortex.cn

Go:   sort.SearchInts(arr, x)
来源：http://vd.muxihuayi.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://uk.panjiajie.cn

C#:   Array.BinarySearch(arr, x)
来源：http://gf.szsharing.cn

[N02] 排序（工程实践用内置实现）
来源：http://wi.lnxyls.cn

Py:   sorted(arr);  arr.sort()
来源：http://iv.szsharing.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ky.szxytkj.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://vc.chemitech.net.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://ei.wgjwhj.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://md.yuntaijiaju.cn

Go:   slices.Sort(arr)
来源：http://ni.521024.cn

Ruby: arr.sort
来源：http://ic.muxihuayi.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://pb.shtwfgs.cn

[N03] 快速排序（分治示例）
来源：http://ga.huanxung.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hf.shxzskj.cn

PHP:  // 递归实现，或用 usort
来源：http://dy.shtwfgs.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://jx.hahajie.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wj.wgjwhj.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://tk.shxzukj.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://vp.colortex.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ws.asd995.cn

C#:   // 手写递归，或 Array.Sort
来源：http://zg.colortex.cn

[N04] 斐波那契数列
来源：http://xe.bjjhwx.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://pg.521024.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://pz.shxzskj.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://rp.jianghongdianzi.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mg.shtwfgs.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://dg.huanxung.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ym.nicolike.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://bl.jctech888.com.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://fd.nicolike.cn

[N05] 最大公约数
来源：http://om.bjjhwx.cn

Py:   math.gcd(a, b)
来源：http://cb.hahajie.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://fz.szsharing.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://om.9csxet.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ca.nicolike.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://oo.colortex.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://me.jianghongdianzi.cn

Ruby: a.gcd(b)
来源：http://mv.wgjwhj.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://lz.shxzskj.cn

[N06] 判断回文字符串
来源：http://qs.panjiajie.cn

Py:   s == s[::-1]
来源：http://wi.muxihuayi.cn

PHP:  $s === strrev($s);
来源：http://rs.yuntaijiaju.cn

JS:   s === [...s].reverse().join("")
来源：http://ew.huanxung.cn

TS:   s === [...s].reverse().join("")
来源：http://jv.lnxyls.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ct.chemitech.net.cn

Go:   // 双指针从两端比较
来源：http://on.bjjhwx.cn

Ruby: s == s.reverse
来源：http://fj.jianghongdianzi.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://gl.hnjuh.cn

[N07] 两数之和（返回下标）
来源：http://ml.nszjky.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://je.newstarts.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://lx.hahajie.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://tm.haigaiapp.cn

TS:   // 手写 Map<string, number>
来源：http://pp.shtwfgs.cn

Java: // 手写 HashMap
来源：http://pd.szxytkj.cn

Go:   // 手写 map[int]int
来源：http://db.shxzukj.cn

Ruby: // 手写 Hash
来源：http://ob.lnxyls.cn

C#:   // 手写 Dictionary<int, int>
来源：http://tq.muxihuayi.cn

[N08] 生成全排列
来源：http://mi.nszjky.cn

Py:   itertools.permutations(arr)
来源：http://iv.wgjwhj.cn

PHP:  // 手写递归交换
来源：http://ig.szxytkj.cn

JS:   // 手写回溯递归
来源：http://nk.huixiangedu.cn

TS:   // 手写回溯递归
来源：http://vz.shtwfgs.cn

Java: // 手写回溯递归
来源：http://si.521024.cn

Go:   // 手写回溯递归
来源：http://wz.huanxung.cn

Ruby: arr.permutation.to_a
来源：http://mo.nicolike.cn

C#:   // 手写回溯递归
来源：http://zt.9csxet.cn

[N09] 栈与队列
来源：http://ax.muxihuayi.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mw.huixiangedu.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://nd.jctech888.com.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mf.nicolike.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ec.szsharing.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hh.asd995.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wk.hahajie.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://xu.colortex.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://bq.jianghongdianzi.cn

[N10] 链表节点定义
来源：http://ik.panjiajie.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://sv.jianghongdianzi.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://sn.bookmarksfly.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://gz.gzmigu.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ys.jctech888.com.cn

Java: class Node { int v; Node next; }
来源：http://ml.szxytkj.cn

Go:   type Node struct { V int; Next *Node }
来源：http://ry.9csxet.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://ua.huixinmuqiang.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://ed.hahajie.cn

[N11] 二叉树中序遍历
来源：http://if.shxzukj.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://zx.hahajie.cn

PHP:  // 手写递归函数
来源：http://jx.bookmarksfly.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ku.lnxyls.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hm.shxzskj.cn

Java: // 手写递归
来源：http://oz.521024.cn

Go:   // 手写递归
来源：http://na.panjiajie.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://lg.haigaiapp.cn

C#:   // 手写递归
来源：http://ek.huixinmuqiang.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://at.shtwfgs.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://gm.huixinmuqiang.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mm.asd995.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ch.lnxyls.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wa.shtwfgs.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://st.chemitech.net.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://qz.chemitech.net.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://rg.hnjuh.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://na.wgjwhj.cn

================================================================================
来源：http://gb.hnjuh.cn

O. 并发与异步
来源：http://mp.jianghongdianzi.cn

================================================================================
来源：http://xe.huanxung.cn

[O01] 启动一个线程
来源：http://vj.szsharing.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://es.szsharing.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://np.newstarts.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://iy.shtwfgs.cn

TS:   // 同 JS
来源：http://qy.yuntaijiaju.cn

Java: new Thread(() -> f()).start()
来源：http://ln.9csxet.cn

Go:   go f()
来源：http://ab.jctech888.com.cn

Ruby: Thread.new { f }
来源：http://cu.newstarts.cn

C#:   Task.Run(() => F());
来源：http://jh.nicolike.cn

[O02] 使用线程池
来源：http://wk.szxytkj.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://di.gzmigu.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://dy.shtwfgs.cn

JS:   // worker_threads 线程池
来源：http://cc.yuexingan06.cn

TS:   // worker_threads 线程池
来源：http://om.yuexingan06.cn

Java: Executors.newFixedThreadPool(4)
来源：http://xe.yuexingan06.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mi.panjiajie.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wi.jianghongdianzi.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://df.muxihuayi.cn

[O03] 加锁保护共享数据
来源：http://el.bjjhwx.cn

Py:   with lock: shared += 1
来源：http://ab.hahajie.cn

PHP:  // 用 flock() 做文件锁
来源：http://kj.panjiajie.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ez.muxihuayi.cn

TS:   // 同 JS
来源：http://pj.muxihuayi.cn

Java: synchronized (this) { shared++; }
来源：http://ed.gzmigu.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wf.bookmarksfly.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://po.huanxung.cn

C#:   lock (gate) { shared++; }
来源：http://cv.bookmarksfly.cn

[O04] 定义异步函数并等待
来源：http://yf.huixinmuqiang.cn

Py:   async def f():⏎    await g()
来源：http://ik.colortex.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wa.gzmigu.cn

JS:   async function f() { await g(); }
来源：http://yn.hnjuh.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://eo.9csxet.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://fi.newstarts.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://fv.jctech888.com.cn

Ruby: # 用 Fiber 或 async gem
来源：http://aq.521024.cn

C#:   async Task F() { await G(); }
来源：http://vb.asd995.cn

[O05] 并发执行并等待全部完成
来源：http://lm.yuntaijiaju.cn

Py:   asyncio.gather(*tasks)
来源：http://ym.521024.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://fa.huanxung.cn

JS:   await Promise.all(tasks)
来源：http://ne.yuntaijiaju.cn

TS:   await Promise.all(tasks)
来源：http://mh.muxihuayi.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://pi.521024.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://tb.bjjhwx.cn

Ruby: threads.map(&:join)
来源：http://qw.haigaiapp.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://ad.huixinmuqiang.cn

[O06] 使用进程池
来源：http://vy.jctech888.com.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://nw.muxihuayi.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://xr.shtwfgs.cn

JS:   // child_process / cluster 模块
来源：http://jn.hahajie.cn

TS:   // child_process / cluster 模块
来源：http://eh.asd995.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://gi.newstarts.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ct.shxzskj.cn

Ruby: // fork 块
来源：http://bb.nszjky.cn

C#:   Parallel.For
来源：http://jw.bookmarksfly.cn

================================================================================
来源：http://ur.szsharing.cn

P. 常用工具函数
来源：http://rw.nicolike.cn

================================================================================
来源：http://kh.hnjuh.cn

[P01] 生成 UUID
来源：http://iu.bjjhwx.cn

Py:   str(uuid.uuid4())
来源：http://er.huixinmuqiang.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://pt.jctech888.com.cn

JS:   crypto.randomUUID()
来源：http://di.nicolike.cn

TS:   crypto.randomUUID()
来源：http://yz.asd995.cn

Java: UUID.randomUUID().toString()
来源：http://xg.shxzskj.cn

Go:   // 用 github.com/google/uuid
来源：http://us.chemitech.net.cn

Ruby: SecureRandom.uuid
来源：http://so.521024.cn

C#:   Guid.NewGuid().ToString()
来源：http://yf.yuntaijiaju.cn

[P02] MD5 / SHA256 摘要
来源：http://ob.yuexingan06.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hu.colortex.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://oz.9csxet.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ei.hahajie.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wl.shtwfgs.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ud.huanxung.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wk.hnjuh.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ib.yuntaijiaju.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://tu.haigaiapp.cn

[P03] 生成短随机字符串
来源：http://tt.panjiajie.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://az.yuntaijiaju.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wu.wgjwhj.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://eh.shxzskj.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://xp.yuexingan06.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ks.huixinmuqiang.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ng.asd995.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://bc.yuexingan06.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://yn.muxihuayi.cn

[P04] 求长度
来源：http://by.shtwfgs.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://jx.shtwfgs.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ao.shxzukj.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ks.huanxung.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ot.wgjwhj.cn

Java: list.size();  map.size();  s.length()
来源：http://fu.hahajie.cn

Go:   len(arr);  len(m)
来源：http://ft.huixiangedu.cn

Ruby: x.length;  x.size
来源：http://tr.hahajie.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://nh.nicolike.cn

[P05] 判断两个对象内容是否相等
来源：http://dc.9csxet.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://fv.hnjuh.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://yl.szsharing.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://pb.haigaiapp.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ej.szxytkj.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://qu.yuntaijiaju.cn

Go:   reflect.DeepEqual(a, b)
来源：http://wb.newstarts.cn

Ruby: a == b
来源：http://gd.panjiajie.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://le.hahajie.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ca.huixiangedu.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://tc.newstarts.cn

PHP:  if (empty($x)) {}
来源：http://qs.haigaiapp.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ix.shxzukj.cn

TS:   if (x == null) {}
来源：http://el.9csxet.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://pi.bookmarksfly.cn

Go:   if x == nil {}
来源：http://nf.lnxyls.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://fm.nicolike.cn

C#:   if (x is null) {}
来源：http://nv.jctech888.com.cn

[P07] 防抖与节流
来源：http://nv.shxzskj.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://at.shtwfgs.cn

PHP:  // 手写时间戳比较
来源：http://ko.yuntaijiaju.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ke.wgjwhj.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hd.bjjhwx.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://eb.hahajie.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://oz.bookmarksfly.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://ls.panjiajie.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wj.jianghongdianzi.cn

[P08] 处理浮点精度问题
来源：http://rw.lnxyls.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://nj.yuexingan06.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://yf.shtwfgs.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://pk.szxytkj.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://lu.wgjwhj.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://pf.shxzskj.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ws.9csxet.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ey.bookmarksfly.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://or.yuntaijiaju.cn

================================================================================
来源：http://qv.lnxyls.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://pc.9csxet.cn

================================================================================
来源：http://dz.huanxung.cn

[Q01] 创建表
来源：http://lr.jianghongdianzi.cn

CREATE TABLE users (
来源：http://kp.bookmarksfly.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://xk.asd995.cn

name VARCHAR(50) NOT NULL,
来源：http://ip.haigaiapp.cn

email VARCHAR(100) UNIQUE,
来源：http://xg.wgjwhj.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wj.jianghongdianzi.cn

);
来源：http://tn.panjiajie.cn

[Q02] 创建带外键的表
来源：http://ix.hahajie.cn

CREATE TABLE orders (
来源：http://yj.jianghongdianzi.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ej.asd995.cn

user_id INT NOT NULL,
来源：http://hh.nicolike.cn

amount DECIMAL(10, 2),
来源：http://ss.521024.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ak.szxytkj.cn

);
来源：http://dl.wgjwhj.cn

[Q03] 增加列
来源：http://pe.9csxet.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://rf.huixinmuqiang.cn

[Q04] 修改列类型
来源：http://hm.asd995.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://jv.muxihuayi.cn

[Q05] 重命名列
来源：http://uh.shtwfgs.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mh.shtwfgs.cn

[Q06] 删除列
来源：http://qx.newstarts.cn

ALTER TABLE users DROP COLUMN age;
来源：http://xl.hahajie.cn

[Q07] 删除表
来源：http://ik.wgjwhj.cn

DROP TABLE IF EXISTS orders;
来源：http://bc.haigaiapp.cn

[Q08] 创建普通索引
来源：http://gy.muxihuayi.cn


<!-- 参考信息 -->