代发 wailian999

TS:   process.cwd()
来源：http://kv.521024.cn

Java: Path.of("").toAbsolutePath()
来源：http://im.panjiajie.cn

Go:   os.Getwd()
来源：http://ce.jianghongdianzi.cn

Ruby: Dir.pwd
来源：http://gt.colortex.cn

C#:   Directory.GetCurrentDirectory()
来源：http://nq.asd995.cn

[M05] 设置退出码
来源：http://hc.wgjwhj.cn

Py:   sys.exit(1)
来源：http://lp.chemitech.net.cn

PHP:  exit(1);
来源：http://qd.szxytkj.cn

JS:   process.exit(1)
来源：http://uf.huixinmuqiang.cn

TS:   process.exit(1)
来源：http://ef.huixinmuqiang.cn

Java: System.exit(1)
来源：http://vw.521024.cn

Go:   os.Exit(1)
来源：http://zp.shtwfgs.cn

Ruby: exit 1
来源：http://hj.yuntaijiaju.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ds.chemitech.net.cn

[M06] 向标准错误输出
来源：http://nn.shxzskj.cn

Py:   print("err", file=sys.stderr)
来源：http://ik.bjjhwx.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://pw.muxihuayi.cn

JS:   console.error("err")
来源：http://eo.huixinmuqiang.cn

TS:   console.error("err")
来源：http://it.huixiangedu.cn

Java: System.err.println("err")
来源：http://of.jianghongdianzi.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://iz.newstarts.cn

Ruby: warn "err"
来源：http://sa.jianghongdianzi.cn

C#:   Console.Error.WriteLine("err")
来源：http://nr.nszjky.cn

[M07] 判断是否为主入口
来源：http://sk.shtwfgs.cn

Py:   if __name__ == "__main__":
来源：http://xy.szsharing.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://lk.shtwfgs.cn

JS:   require.main === module
来源：http://ii.muxihuayi.cn

TS:   require.main === module
来源：http://ot.asd995.cn

Java: public static void main(String[] args)
来源：http://fi.jctech888.com.cn

Go:   func main()
来源：http://wd.huixinmuqiang.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://cu.shxzskj.cn

C#:   static void Main(string[] args)
来源：http://fr.shtwfgs.cn

[M08] 获取系统与运行时信息
来源：http://qd.shxzskj.cn

Py:   platform.system();  platform.python_version()
来源：http://xt.shxzukj.cn

PHP:  PHP_OS;  phpversion();
来源：http://da.newstarts.cn

JS:   process.platform;  process.version
来源：http://hz.nicolike.cn

TS:   process.platform;  process.version
来源：http://km.asd995.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://pq.shtwfgs.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://hl.yuexingan06.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wf.panjiajie.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://ra.szxytkj.cn

================================================================================
来源：http://dr.haigaiapp.cn

N. 数据结构与算法
来源：http://ra.huanxung.cn

================================================================================
来源：http://co.huanxung.cn

[N01] 二分查找（有序数组）
来源：http://ke.gzmigu.cn

Py:   bisect.bisect_left(arr, x)
来源：http://is.shxzskj.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://rv.szxytkj.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mz.huixiangedu.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://qc.yuexingan06.cn

Java: Arrays.binarySearch(arr, x)
来源：http://wv.szxytkj.cn

Go:   sort.SearchInts(arr, x)
来源：http://ad.521024.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://hu.nicolike.cn

C#:   Array.BinarySearch(arr, x)
来源：http://ow.lnxyls.cn

[N02] 排序（工程实践用内置实现）
来源：http://aa.szsharing.cn

Py:   sorted(arr);  arr.sort()
来源：http://pn.huixiangedu.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://zj.gzmigu.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://vj.bjjhwx.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://ky.bjjhwx.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://dy.gzmigu.cn

Go:   slices.Sort(arr)
来源：http://gz.shxzukj.cn

Ruby: arr.sort
来源：http://fl.haigaiapp.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://oh.szsharing.cn

[N03] 快速排序（分治示例）
来源：http://yf.wgjwhj.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mz.jctech888.com.cn

PHP:  // 递归实现，或用 usort
来源：http://ka.jianghongdianzi.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://yt.colortex.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://fm.newstarts.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://dx.szxytkj.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://fs.huixinmuqiang.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://nc.szsharing.cn

C#:   // 手写递归，或 Array.Sort
来源：http://rb.jianghongdianzi.cn

[N04] 斐波那契数列
来源：http://ju.lnxyls.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ky.szsharing.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://uu.chemitech.net.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://bs.shxzskj.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://kd.szxytkj.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ia.szsharing.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ct.bjjhwx.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://jz.haigaiapp.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://uk.shxzukj.cn

[N05] 最大公约数
来源：http://pr.wgjwhj.cn

Py:   math.gcd(a, b)
来源：http://nu.bookmarksfly.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://nj.muxihuayi.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://tj.colortex.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://zx.szxytkj.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://nh.521024.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://bv.jctech888.com.cn

Ruby: a.gcd(b)
来源：http://ol.chemitech.net.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://oc.shtwfgs.cn

[N06] 判断回文字符串
来源：http://sd.jctech888.com.cn

Py:   s == s[::-1]
来源：http://cr.jianghongdianzi.cn

PHP:  $s === strrev($s);
来源：http://eg.hnjuh.cn

JS:   s === [...s].reverse().join("")
来源：http://ur.jctech888.com.cn

TS:   s === [...s].reverse().join("")
来源：http://kz.hahajie.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wu.newstarts.cn

Go:   // 双指针从两端比较
来源：http://gs.szsharing.cn

Ruby: s == s.reverse
来源：http://eq.wgjwhj.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://cg.muxihuayi.cn

[N07] 两数之和（返回下标）
来源：http://rz.szsharing.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://yu.lnxyls.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://xn.jianghongdianzi.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://gk.bookmarksfly.cn

TS:   // 手写 Map<string, number>
来源：http://ki.lnxyls.cn

Java: // 手写 HashMap
来源：http://jz.shtwfgs.cn

Go:   // 手写 map[int]int
来源：http://bw.muxihuayi.cn

Ruby: // 手写 Hash
来源：http://dr.hahajie.cn

C#:   // 手写 Dictionary<int, int>
来源：http://td.shxzukj.cn

[N08] 生成全排列
来源：http://sm.haigaiapp.cn

Py:   itertools.permutations(arr)
来源：http://wr.yuexingan06.cn

PHP:  // 手写递归交换
来源：http://gl.yuexingan06.cn

JS:   // 手写回溯递归
来源：http://ln.huixinmuqiang.cn

TS:   // 手写回溯递归
来源：http://lb.colortex.cn

Java: // 手写回溯递归
来源：http://yi.wgjwhj.cn

Go:   // 手写回溯递归
来源：http://bh.shxzskj.cn

Ruby: arr.permutation.to_a
来源：http://ca.muxihuayi.cn

C#:   // 手写回溯递归
来源：http://yv.bookmarksfly.cn

[N09] 栈与队列
来源：http://xl.bjjhwx.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://it.wgjwhj.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ix.jianghongdianzi.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://cv.shtwfgs.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://co.wgjwhj.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://te.yuexingan06.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://od.chemitech.net.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://xj.szxytkj.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://lh.lnxyls.cn

[N10] 链表节点定义
来源：http://ol.lnxyls.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mp.yuntaijiaju.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://bz.lnxyls.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://vj.newstarts.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ap.bookmarksfly.cn

Java: class Node { int v; Node next; }
来源：http://qj.nszjky.cn

Go:   type Node struct { V int; Next *Node }
来源：http://ak.panjiajie.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://mb.hnjuh.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://xb.panjiajie.cn

[N11] 二叉树中序遍历
来源：http://uh.shxzukj.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ww.nszjky.cn

PHP:  // 手写递归函数
来源：http://ca.wgjwhj.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ay.shxzskj.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wu.colortex.cn

Java: // 手写递归
来源：http://vl.huixiangedu.cn

Go:   // 手写递归
来源：http://ev.521024.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hb.nszjky.cn

C#:   // 手写递归
来源：http://wc.521024.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://qc.newstarts.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://fs.lnxyls.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ic.nszjky.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ya.yuntaijiaju.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://oq.9csxet.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://tn.haigaiapp.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://xg.yuexingan06.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://vt.huixiangedu.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hm.colortex.cn

================================================================================
来源：http://ts.szxytkj.cn

O. 并发与异步
来源：http://kx.szxytkj.cn

================================================================================
来源：http://nw.9csxet.cn

[O01] 启动一个线程
来源：http://rs.hahajie.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wu.szxytkj.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://tu.bjjhwx.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ew.bjjhwx.cn

TS:   // 同 JS
来源：http://ga.9csxet.cn

Java: new Thread(() -> f()).start()
来源：http://si.panjiajie.cn

Go:   go f()
来源：http://yh.huixiangedu.cn

Ruby: Thread.new { f }
来源：http://ul.huanxung.cn

C#:   Task.Run(() => F());
来源：http://rt.hnjuh.cn

[O02] 使用线程池
来源：http://xr.hahajie.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://pq.asd995.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://df.521024.cn

JS:   // worker_threads 线程池
来源：http://sy.szxytkj.cn

TS:   // worker_threads 线程池
来源：http://da.szsharing.cn

Java: Executors.newFixedThreadPool(4)
来源：http://wp.szxytkj.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://sj.nszjky.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://aj.9csxet.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://eg.shtwfgs.cn

[O03] 加锁保护共享数据
来源：http://zj.hnjuh.cn

Py:   with lock: shared += 1
来源：http://hf.bookmarksfly.cn

PHP:  // 用 flock() 做文件锁
来源：http://av.asd995.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://sx.521024.cn

TS:   // 同 JS
来源：http://bi.yuexingan06.cn

Java: synchronized (this) { shared++; }
来源：http://jn.yuexingan06.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://qk.haigaiapp.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://mb.gzmigu.cn

C#:   lock (gate) { shared++; }
来源：http://mt.panjiajie.cn

[O04] 定义异步函数并等待
来源：http://sc.wgjwhj.cn

Py:   async def f():⏎    await g()
来源：http://tg.nszjky.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://rf.jctech888.com.cn

JS:   async function f() { await g(); }
来源：http://yw.shtwfgs.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://gs.shxzskj.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://zq.yuntaijiaju.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://cp.nszjky.cn

Ruby: # 用 Fiber 或 async gem
来源：http://cb.huixiangedu.cn

C#:   async Task F() { await G(); }
来源：http://yf.shxzskj.cn

[O05] 并发执行并等待全部完成
来源：http://zc.chemitech.net.cn

Py:   asyncio.gather(*tasks)
来源：http://kw.jianghongdianzi.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://od.huixinmuqiang.cn

JS:   await Promise.all(tasks)
来源：http://bn.chemitech.net.cn

TS:   await Promise.all(tasks)
来源：http://bx.huixiangedu.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://iy.nszjky.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ru.chemitech.net.cn

Ruby: threads.map(&:join)
来源：http://lg.asd995.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://cm.huanxung.cn

[O06] 使用进程池
来源：http://ya.chemitech.net.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://xr.huanxung.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://yr.bookmarksfly.cn

JS:   // child_process / cluster 模块
来源：http://uz.jianghongdianzi.cn

TS:   // child_process / cluster 模块
来源：http://dn.9csxet.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://qp.huixinmuqiang.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ca.chemitech.net.cn

Ruby: // fork 块
来源：http://my.panjiajie.cn

C#:   Parallel.For
来源：http://ac.asd995.cn

================================================================================
来源：http://xu.shtwfgs.cn

P. 常用工具函数
来源：http://xn.jianghongdianzi.cn

================================================================================
来源：http://nd.haigaiapp.cn

[P01] 生成 UUID
来源：http://bp.yuntaijiaju.cn

Py:   str(uuid.uuid4())
来源：http://qc.newstarts.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://rl.shxzukj.cn

JS:   crypto.randomUUID()
来源：http://il.nicolike.cn

TS:   crypto.randomUUID()
来源：http://wa.9csxet.cn

Java: UUID.randomUUID().toString()
来源：http://fp.haigaiapp.cn

Go:   // 用 github.com/google/uuid
来源：http://yr.jctech888.com.cn

Ruby: SecureRandom.uuid
来源：http://gi.gzmigu.cn

C#:   Guid.NewGuid().ToString()
来源：http://gm.jianghongdianzi.cn

[P02] MD5 / SHA256 摘要
来源：http://oa.shxzukj.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://oz.bjjhwx.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://tc.szxytkj.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://nf.9csxet.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ll.colortex.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://zm.asd995.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://lv.chemitech.net.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://rp.hnjuh.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wp.gzmigu.cn

[P03] 生成短随机字符串
来源：http://xr.huanxung.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://bh.yuntaijiaju.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://nx.hnjuh.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wz.jianghongdianzi.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://yg.muxihuayi.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://dn.9csxet.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ns.chemitech.net.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://ke.huixiangedu.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ge.gzmigu.cn

[P04] 求长度
来源：http://fb.shxzukj.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wd.jctech888.com.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://tb.shxzukj.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://vq.shtwfgs.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://xk.shtwfgs.cn

Java: list.size();  map.size();  s.length()
来源：http://fy.huixiangedu.cn

Go:   len(arr);  len(m)
来源：http://ev.lnxyls.cn

Ruby: x.length;  x.size
来源：http://lv.huanxung.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://qt.chemitech.net.cn

[P05] 判断两个对象内容是否相等
来源：http://td.yuntaijiaju.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://xi.szsharing.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://by.shxzskj.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ql.wgjwhj.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ea.colortex.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://pr.szsharing.cn

Go:   reflect.DeepEqual(a, b)
来源：http://ui.bookmarksfly.cn

Ruby: a == b
来源：http://mr.shxzskj.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://xp.huixiangedu.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://jf.jctech888.com.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://xw.haigaiapp.cn

PHP:  if (empty($x)) {}
来源：http://mu.shxzukj.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ot.yuexingan06.cn

TS:   if (x == null) {}
来源：http://su.shxzukj.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://ow.huixinmuqiang.cn

Go:   if x == nil {}
来源：http://dk.szxytkj.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wv.jianghongdianzi.cn

C#:   if (x is null) {}
来源：http://rg.panjiajie.cn

[P07] 防抖与节流
来源：http://cu.shtwfgs.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ox.szsharing.cn

PHP:  // 手写时间戳比较
来源：http://zh.asd995.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ok.huixinmuqiang.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://jc.bookmarksfly.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://pn.haigaiapp.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://xq.huixinmuqiang.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://ar.521024.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://tc.jianghongdianzi.cn

[P08] 处理浮点精度问题
来源：http://uc.shtwfgs.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ba.9csxet.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://kv.panjiajie.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://fc.jianghongdianzi.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://bn.szxytkj.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://tr.asd995.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://xv.bookmarksfly.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://cz.521024.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://gk.newstarts.cn

================================================================================
来源：http://td.szxytkj.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://fs.huixiangedu.cn

================================================================================
来源：http://co.nicolike.cn

[Q01] 创建表
来源：http://rj.nicolike.cn

CREATE TABLE users (
来源：http://kx.yuntaijiaju.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://vd.gzmigu.cn

name VARCHAR(50) NOT NULL,
来源：http://zt.newstarts.cn

email VARCHAR(100) UNIQUE,
来源：http://jq.szxytkj.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://no.gzmigu.cn

);
来源：http://ty.wgjwhj.cn

[Q02] 创建带外键的表
来源：http://gf.asd995.cn

CREATE TABLE orders (
来源：http://lc.hahajie.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mi.lnxyls.cn

user_id INT NOT NULL,
来源：http://kk.huixinmuqiang.cn

amount DECIMAL(10, 2),
来源：http://pa.shtwfgs.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://nt.yuexingan06.cn


<!-- 参考信息 -->