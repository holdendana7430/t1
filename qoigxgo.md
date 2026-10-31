代发 wailian999

Ruby: exit 1
来源：http://xx.szsharing.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://nn.bjjhwx.cn

[M06] 向标准错误输出
来源：http://ku.szxytkj.cn

Py:   print("err", file=sys.stderr)
来源：http://qm.yuexingan06.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://hc.muxihuayi.cn

JS:   console.error("err")
来源：http://or.hnjuh.cn

TS:   console.error("err")
来源：http://bb.chemitech.net.cn

Java: System.err.println("err")
来源：http://jo.chemitech.net.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ud.muxihuayi.cn

Ruby: warn "err"
来源：http://or.huixinmuqiang.cn

C#:   Console.Error.WriteLine("err")
来源：http://cl.bjjhwx.cn

[M07] 判断是否为主入口
来源：http://em.huixiangedu.cn

Py:   if __name__ == "__main__":
来源：http://pm.bookmarksfly.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://cf.521024.cn

JS:   require.main === module
来源：http://hz.newstarts.cn

TS:   require.main === module
来源：http://gf.nszjky.cn

Java: public static void main(String[] args)
来源：http://oh.hnjuh.cn

Go:   func main()
来源：http://cp.colortex.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://fl.bookmarksfly.cn

C#:   static void Main(string[] args)
来源：http://zf.asd995.cn

[M08] 获取系统与运行时信息
来源：http://zr.wgjwhj.cn

Py:   platform.system();  platform.python_version()
来源：http://zh.szxytkj.cn

PHP:  PHP_OS;  phpversion();
来源：http://vx.panjiajie.cn

JS:   process.platform;  process.version
来源：http://sp.haigaiapp.cn

TS:   process.platform;  process.version
来源：http://rx.huixiangedu.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://qz.haigaiapp.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://ib.jctech888.com.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://sy.shtwfgs.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://lh.shtwfgs.cn

================================================================================
来源：http://jg.asd995.cn

N. 数据结构与算法
来源：http://ab.chemitech.net.cn

================================================================================
来源：http://zc.hahajie.cn

[N01] 二分查找（有序数组）
来源：http://tc.hahajie.cn

Py:   bisect.bisect_left(arr, x)
来源：http://ia.hahajie.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://pc.szsharing.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://rs.shxzukj.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ds.nszjky.cn

Java: Arrays.binarySearch(arr, x)
来源：http://xe.yuntaijiaju.cn

Go:   sort.SearchInts(arr, x)
来源：http://nc.hnjuh.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://gs.bjjhwx.cn

C#:   Array.BinarySearch(arr, x)
来源：http://eb.wgjwhj.cn

[N02] 排序（工程实践用内置实现）
来源：http://tm.nicolike.cn

Py:   sorted(arr);  arr.sort()
来源：http://ne.nicolike.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://sy.szsharing.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://jg.hahajie.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://is.szsharing.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://io.chemitech.net.cn

Go:   slices.Sort(arr)
来源：http://sj.yuexingan06.cn

Ruby: arr.sort
来源：http://ox.muxihuayi.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://hx.wgjwhj.cn

[N03] 快速排序（分治示例）
来源：http://qa.newstarts.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://da.huixiangedu.cn

PHP:  // 递归实现，或用 usort
来源：http://xd.521024.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ty.colortex.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://gd.hnjuh.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ga.haigaiapp.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ss.jianghongdianzi.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://nd.haigaiapp.cn

C#:   // 手写递归，或 Array.Sort
来源：http://jl.hnjuh.cn

[N04] 斐波那契数列
来源：http://lx.haigaiapp.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://sf.yuntaijiaju.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://np.shtwfgs.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hn.hahajie.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wl.hahajie.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://sw.hnjuh.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wv.bookmarksfly.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://zl.jianghongdianzi.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://bw.colortex.cn

[N05] 最大公约数
来源：http://hw.yuntaijiaju.cn

Py:   math.gcd(a, b)
来源：http://hy.nicolike.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ar.newstarts.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://bi.yuexingan06.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ln.hahajie.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ei.panjiajie.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hs.colortex.cn

Ruby: a.gcd(b)
来源：http://co.haigaiapp.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://jj.shxzskj.cn

[N06] 判断回文字符串
来源：http://vy.jctech888.com.cn

Py:   s == s[::-1]
来源：http://nn.newstarts.cn

PHP:  $s === strrev($s);
来源：http://zg.huanxung.cn

JS:   s === [...s].reverse().join("")
来源：http://ke.hnjuh.cn

TS:   s === [...s].reverse().join("")
来源：http://er.huanxung.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://du.newstarts.cn

Go:   // 双指针从两端比较
来源：http://bn.szsharing.cn

Ruby: s == s.reverse
来源：http://sg.shxzskj.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://ar.huanxung.cn

[N07] 两数之和（返回下标）
来源：http://zz.haigaiapp.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ar.bookmarksfly.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://zs.bjjhwx.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://lp.muxihuayi.cn

TS:   // 手写 Map<string, number>
来源：http://ow.bjjhwx.cn

Java: // 手写 HashMap
来源：http://xw.yuntaijiaju.cn

Go:   // 手写 map[int]int
来源：http://wu.yuexingan06.cn

Ruby: // 手写 Hash
来源：http://hi.chemitech.net.cn

C#:   // 手写 Dictionary<int, int>
来源：http://kq.hahajie.cn

[N08] 生成全排列
来源：http://xm.nicolike.cn

Py:   itertools.permutations(arr)
来源：http://om.chemitech.net.cn

PHP:  // 手写递归交换
来源：http://fc.shtwfgs.cn

JS:   // 手写回溯递归
来源：http://lp.yuexingan06.cn

TS:   // 手写回溯递归
来源：http://bw.hahajie.cn

Java: // 手写回溯递归
来源：http://lx.yuntaijiaju.cn

Go:   // 手写回溯递归
来源：http://nc.9csxet.cn

Ruby: arr.permutation.to_a
来源：http://ez.shtwfgs.cn

C#:   // 手写回溯递归
来源：http://dg.jianghongdianzi.cn

[N09] 栈与队列
来源：http://th.521024.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://di.nszjky.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://az.newstarts.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://bc.yuntaijiaju.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ih.jctech888.com.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://pf.yuexingan06.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://kr.wgjwhj.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://kp.yuntaijiaju.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://cv.panjiajie.cn

[N10] 链表节点定义
来源：http://dy.haigaiapp.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://dk.bjjhwx.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://dr.huixinmuqiang.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://tj.szxytkj.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://yq.wgjwhj.cn

Java: class Node { int v; Node next; }
来源：http://lo.nicolike.cn

Go:   type Node struct { V int; Next *Node }
来源：http://ba.haigaiapp.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://da.szxytkj.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://vb.colortex.cn

[N11] 二叉树中序遍历
来源：http://ht.521024.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://au.panjiajie.cn

PHP:  // 手写递归函数
来源：http://ob.huixinmuqiang.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://br.yuexingan06.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://si.asd995.cn

Java: // 手写递归
来源：http://ua.521024.cn

Go:   // 手写递归
来源：http://za.gzmigu.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://qy.szxytkj.cn

C#:   // 手写递归
来源：http://ne.muxihuayi.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://tc.colortex.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://uk.nicolike.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://pf.chemitech.net.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://bi.huanxung.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://kv.nicolike.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mb.jianghongdianzi.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://sn.huixiangedu.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://od.muxihuayi.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://qj.bookmarksfly.cn

================================================================================
来源：http://ka.huixinmuqiang.cn

O. 并发与异步
来源：http://qo.chemitech.net.cn

================================================================================
来源：http://qc.huixiangedu.cn

[O01] 启动一个线程
来源：http://vr.panjiajie.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://xe.szxytkj.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mz.haigaiapp.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://qb.9csxet.cn

TS:   // 同 JS
来源：http://ob.521024.cn

Java: new Thread(() -> f()).start()
来源：http://uv.haigaiapp.cn

Go:   go f()
来源：http://ul.huixiangedu.cn

Ruby: Thread.new { f }
来源：http://eo.yuexingan06.cn

C#:   Task.Run(() => F());
来源：http://dx.9csxet.cn

[O02] 使用线程池
来源：http://eg.muxihuayi.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://dz.yuexingan06.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ep.gzmigu.cn

JS:   // worker_threads 线程池
来源：http://yo.jctech888.com.cn

TS:   // worker_threads 线程池
来源：http://oy.wgjwhj.cn

Java: Executors.newFixedThreadPool(4)
来源：http://sx.chemitech.net.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://id.521024.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://uu.huanxung.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://kz.shxzskj.cn

[O03] 加锁保护共享数据
来源：http://ua.chemitech.net.cn

Py:   with lock: shared += 1
来源：http://ek.hahajie.cn

PHP:  // 用 flock() 做文件锁
来源：http://rs.shxzukj.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hx.bjjhwx.cn

TS:   // 同 JS
来源：http://fa.9csxet.cn

Java: synchronized (this) { shared++; }
来源：http://ee.hnjuh.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://zv.shtwfgs.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://bh.huixiangedu.cn

C#:   lock (gate) { shared++; }
来源：http://ho.gzmigu.cn

[O04] 定义异步函数并等待
来源：http://ed.nicolike.cn

Py:   async def f():⏎    await g()
来源：http://ve.szxytkj.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://qd.shxzskj.cn

JS:   async function f() { await g(); }
来源：http://rs.huixinmuqiang.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://gg.bjjhwx.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://gg.huixinmuqiang.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://aw.colortex.cn

Ruby: # 用 Fiber 或 async gem
来源：http://kj.nszjky.cn

C#:   async Task F() { await G(); }
来源：http://vm.jctech888.com.cn

[O05] 并发执行并等待全部完成
来源：http://mt.gzmigu.cn

Py:   asyncio.gather(*tasks)
来源：http://kz.shxzukj.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://fb.yuexingan06.cn

JS:   await Promise.all(tasks)
来源：http://dw.yuntaijiaju.cn

TS:   await Promise.all(tasks)
来源：http://cp.szsharing.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://gx.wgjwhj.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://kk.hahajie.cn

Ruby: threads.map(&:join)
来源：http://kl.asd995.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://oi.hnjuh.cn

[O06] 使用进程池
来源：http://ox.huixinmuqiang.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://iy.nszjky.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://ld.9csxet.cn

JS:   // child_process / cluster 模块
来源：http://xv.wgjwhj.cn

TS:   // child_process / cluster 模块
来源：http://hy.szsharing.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://gi.jianghongdianzi.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://xk.shxzskj.cn

Ruby: // fork 块
来源：http://pz.colortex.cn

C#:   Parallel.For
来源：http://du.shtwfgs.cn

================================================================================
来源：http://ev.521024.cn

P. 常用工具函数
来源：http://ji.yuexingan06.cn

================================================================================
来源：http://vl.muxihuayi.cn

[P01] 生成 UUID
来源：http://gi.hnjuh.cn

Py:   str(uuid.uuid4())
来源：http://qi.9csxet.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://is.szsharing.cn

JS:   crypto.randomUUID()
来源：http://hy.szxytkj.cn

TS:   crypto.randomUUID()
来源：http://cs.huixinmuqiang.cn

Java: UUID.randomUUID().toString()
来源：http://hp.hahajie.cn

Go:   // 用 github.com/google/uuid
来源：http://ky.szsharing.cn

Ruby: SecureRandom.uuid
来源：http://sg.nicolike.cn

C#:   Guid.NewGuid().ToString()
来源：http://is.jctech888.com.cn

[P02] MD5 / SHA256 摘要
来源：http://bi.gzmigu.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ve.hahajie.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://fx.shxzskj.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://yy.jctech888.com.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mc.bjjhwx.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ab.asd995.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ao.shxzukj.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://qg.colortex.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://fl.jianghongdianzi.cn

[P03] 生成短随机字符串
来源：http://je.haigaiapp.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://gu.shtwfgs.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://xf.nicolike.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ji.szsharing.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://it.panjiajie.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://lz.jctech888.com.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://nw.lnxyls.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://de.hnjuh.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ce.hahajie.cn

[P04] 求长度
来源：http://hv.wgjwhj.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mu.chemitech.net.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://qp.bookmarksfly.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://rc.nszjky.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wh.521024.cn

Java: list.size();  map.size();  s.length()
来源：http://cc.shtwfgs.cn

Go:   len(arr);  len(m)
来源：http://el.colortex.cn

Ruby: x.length;  x.size
来源：http://tz.colortex.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://wm.huanxung.cn

[P05] 判断两个对象内容是否相等
来源：http://uq.9csxet.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://kd.huixinmuqiang.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://em.huanxung.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://vw.bookmarksfly.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://sy.yuexingan06.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://qx.huixiangedu.cn

Go:   reflect.DeepEqual(a, b)
来源：http://ig.gzmigu.cn

Ruby: a == b
来源：http://wb.huixinmuqiang.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://eg.huixinmuqiang.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://qe.colortex.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://qj.panjiajie.cn

PHP:  if (empty($x)) {}
来源：http://wa.9csxet.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://vf.nszjky.cn

TS:   if (x == null) {}
来源：http://gw.gzmigu.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://si.lnxyls.cn

Go:   if x == nil {}
来源：http://ge.huanxung.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://yn.wgjwhj.cn

C#:   if (x is null) {}
来源：http://wg.nicolike.cn

[P07] 防抖与节流
来源：http://tb.panjiajie.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://kr.szxytkj.cn

PHP:  // 手写时间戳比较
来源：http://mc.shtwfgs.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://yp.colortex.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xx.yuntaijiaju.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://gj.colortex.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://cl.shxzskj.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://dz.colortex.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ld.bjjhwx.cn

[P08] 处理浮点精度问题
来源：http://mb.szsharing.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mg.haigaiapp.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://jw.newstarts.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://gq.yuexingan06.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://xn.huixiangedu.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://xb.huanxung.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hh.shxzskj.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://lk.colortex.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://tl.newstarts.cn

================================================================================
来源：http://pq.bookmarksfly.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://jv.yuntaijiaju.cn

================================================================================
来源：http://hd.lnxyls.cn

[Q01] 创建表
来源：http://mh.nicolike.cn

CREATE TABLE users (
来源：http://pa.colortex.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://rr.bjjhwx.cn

name VARCHAR(50) NOT NULL,
来源：http://pn.bookmarksfly.cn

email VARCHAR(100) UNIQUE,
来源：http://nn.shtwfgs.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ce.521024.cn

);
来源：http://wc.jianghongdianzi.cn

[Q02] 创建带外键的表
来源：http://qb.haigaiapp.cn

CREATE TABLE orders (
来源：http://wa.colortex.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://yh.nicolike.cn

user_id INT NOT NULL,
来源：http://iq.shtwfgs.cn

amount DECIMAL(10, 2),
来源：http://pe.gzmigu.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://rb.9csxet.cn

);
来源：http://vo.bjjhwx.cn

[Q03] 增加列
来源：http://qj.9csxet.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://md.bjjhwx.cn

[Q04] 修改列类型
来源：http://la.huixiangedu.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://cv.asd995.cn

[Q05] 重命名列
来源：http://rm.huixinmuqiang.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://lc.haigaiapp.cn

[Q06] 删除列
来源：http://gv.szsharing.cn

ALTER TABLE users DROP COLUMN age;
来源：http://xu.bookmarksfly.cn

[Q07] 删除表
来源：http://nz.muxihuayi.cn

DROP TABLE IF EXISTS orders;
来源：http://vj.521024.cn

[Q08] 创建普通索引
来源：http://bj.huixinmuqiang.cn


<!-- 参考信息 -->