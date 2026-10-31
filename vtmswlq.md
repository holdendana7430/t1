代发 wailian999

TS:   process.cwd()
来源：http://aq.yuntaijiaju.cn

Java: Path.of("").toAbsolutePath()
来源：http://la.wgjwhj.cn

Go:   os.Getwd()
来源：http://tv.shxzukj.cn

Ruby: Dir.pwd
来源：http://jr.colortex.cn

C#:   Directory.GetCurrentDirectory()
来源：http://sq.9csxet.cn

[M05] 设置退出码
来源：http://hf.huixinmuqiang.cn

Py:   sys.exit(1)
来源：http://ts.huixiangedu.cn

PHP:  exit(1);
来源：http://gc.shxzukj.cn

JS:   process.exit(1)
来源：http://eu.jctech888.com.cn

TS:   process.exit(1)
来源：http://wh.huixiangedu.cn

Java: System.exit(1)
来源：http://um.nszjky.cn

Go:   os.Exit(1)
来源：http://ce.colortex.cn

Ruby: exit 1
来源：http://wz.jctech888.com.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://rz.yuntaijiaju.cn

[M06] 向标准错误输出
来源：http://lb.9csxet.cn

Py:   print("err", file=sys.stderr)
来源：http://ug.shxzukj.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://su.muxihuayi.cn

JS:   console.error("err")
来源：http://pn.muxihuayi.cn

TS:   console.error("err")
来源：http://ti.lnxyls.cn

Java: System.err.println("err")
来源：http://yz.gzmigu.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://cg.huixinmuqiang.cn

Ruby: warn "err"
来源：http://pt.jianghongdianzi.cn

C#:   Console.Error.WriteLine("err")
来源：http://cn.gzmigu.cn

[M07] 判断是否为主入口
来源：http://pa.shxzukj.cn

Py:   if __name__ == "__main__":
来源：http://xw.521024.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://oq.shxzukj.cn

JS:   require.main === module
来源：http://ny.jctech888.com.cn

TS:   require.main === module
来源：http://ab.szsharing.cn

Java: public static void main(String[] args)
来源：http://mp.shxzukj.cn

Go:   func main()
来源：http://ie.gzmigu.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://qe.huixiangedu.cn

C#:   static void Main(string[] args)
来源：http://we.huanxung.cn

[M08] 获取系统与运行时信息
来源：http://we.shxzskj.cn

Py:   platform.system();  platform.python_version()
来源：http://wd.bookmarksfly.cn

PHP:  PHP_OS;  phpversion();
来源：http://pf.huanxung.cn

JS:   process.platform;  process.version
来源：http://tw.bjjhwx.cn

TS:   process.platform;  process.version
来源：http://tk.hahajie.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://zv.jctech888.com.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://nq.huanxung.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://qr.nszjky.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://jc.yuexingan06.cn

================================================================================
来源：http://dx.shxzukj.cn

N. 数据结构与算法
来源：http://ix.bjjhwx.cn

================================================================================
来源：http://es.szsharing.cn

[N01] 二分查找（有序数组）
来源：http://sc.yuntaijiaju.cn

Py:   bisect.bisect_left(arr, x)
来源：http://mi.9csxet.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://di.yuntaijiaju.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ul.panjiajie.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://rq.nszjky.cn

Java: Arrays.binarySearch(arr, x)
来源：http://ra.yuexingan06.cn

Go:   sort.SearchInts(arr, x)
来源：http://un.huanxung.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://zj.gzmigu.cn

C#:   Array.BinarySearch(arr, x)
来源：http://je.wgjwhj.cn

[N02] 排序（工程实践用内置实现）
来源：http://ew.9csxet.cn

Py:   sorted(arr);  arr.sort()
来源：http://ys.asd995.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://vx.bookmarksfly.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://bz.yuntaijiaju.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://xi.nszjky.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://pd.bjjhwx.cn

Go:   slices.Sort(arr)
来源：http://nf.bookmarksfly.cn

Ruby: arr.sort
来源：http://pb.haigaiapp.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://sz.jctech888.com.cn

[N03] 快速排序（分治示例）
来源：http://xl.gzmigu.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://sr.nszjky.cn

PHP:  // 递归实现，或用 usort
来源：http://jc.shxzskj.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://sk.huixiangedu.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://fr.bjjhwx.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://gi.wgjwhj.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hq.hahajie.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://vm.gzmigu.cn

C#:   // 手写递归，或 Array.Sort
来源：http://dh.colortex.cn

[N04] 斐波那契数列
来源：http://ps.gzmigu.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ji.muxihuayi.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://cl.shxzskj.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://um.huanxung.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hj.nszjky.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://kv.gzmigu.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wu.huanxung.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://yp.panjiajie.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ln.huixiangedu.cn

[N05] 最大公约数
来源：http://vf.bookmarksfly.cn

Py:   math.gcd(a, b)
来源：http://iv.hnjuh.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hm.wgjwhj.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://rw.panjiajie.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ia.muxihuayi.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ep.lnxyls.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ka.lnxyls.cn

Ruby: a.gcd(b)
来源：http://ls.huanxung.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://qa.muxihuayi.cn

[N06] 判断回文字符串
来源：http://dp.huixiangedu.cn

Py:   s == s[::-1]
来源：http://ug.wgjwhj.cn

PHP:  $s === strrev($s);
来源：http://sz.huixinmuqiang.cn

JS:   s === [...s].reverse().join("")
来源：http://zb.szxytkj.cn

TS:   s === [...s].reverse().join("")
来源：http://oa.newstarts.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wb.huanxung.cn

Go:   // 双指针从两端比较
来源：http://fr.panjiajie.cn

Ruby: s == s.reverse
来源：http://id.huixiangedu.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://pt.yuntaijiaju.cn

[N07] 两数之和（返回下标）
来源：http://kh.panjiajie.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://zk.huixiangedu.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wh.nszjky.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://kj.lnxyls.cn

TS:   // 手写 Map<string, number>
来源：http://dk.jctech888.com.cn

Java: // 手写 HashMap
来源：http://hy.colortex.cn

Go:   // 手写 map[int]int
来源：http://eu.gzmigu.cn

Ruby: // 手写 Hash
来源：http://ew.9csxet.cn

C#:   // 手写 Dictionary<int, int>
来源：http://ue.521024.cn

[N08] 生成全排列
来源：http://rr.521024.cn

Py:   itertools.permutations(arr)
来源：http://lj.szsharing.cn

PHP:  // 手写递归交换
来源：http://zu.shtwfgs.cn

JS:   // 手写回溯递归
来源：http://cs.szxytkj.cn

TS:   // 手写回溯递归
来源：http://fa.nszjky.cn

Java: // 手写回溯递归
来源：http://no.szxytkj.cn

Go:   // 手写回溯递归
来源：http://pn.wgjwhj.cn

Ruby: arr.permutation.to_a
来源：http://gs.lnxyls.cn

C#:   // 手写回溯递归
来源：http://zv.haigaiapp.cn

[N09] 栈与队列
来源：http://ez.huixinmuqiang.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://kh.muxihuayi.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://vj.nszjky.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://xf.szxytkj.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://pm.yuntaijiaju.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://pw.huixiangedu.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ds.asd995.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://qc.gzmigu.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://jg.huanxung.cn

[N10] 链表节点定义
来源：http://of.hahajie.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://kn.huixinmuqiang.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://zo.shtwfgs.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ku.gzmigu.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://nk.lnxyls.cn

Java: class Node { int v; Node next; }
来源：http://ad.jianghongdianzi.cn

Go:   type Node struct { V int; Next *Node }
来源：http://fg.newstarts.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://jv.szxytkj.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://yn.jctech888.com.cn

[N11] 二叉树中序遍历
来源：http://mo.newstarts.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mt.lnxyls.cn

PHP:  // 手写递归函数
来源：http://jp.chemitech.net.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://iq.wgjwhj.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ky.asd995.cn

Java: // 手写递归
来源：http://ln.yuntaijiaju.cn

Go:   // 手写递归
来源：http://km.wgjwhj.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mj.hnjuh.cn

C#:   // 手写递归
来源：http://zm.newstarts.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ss.newstarts.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://uo.panjiajie.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://tt.hahajie.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://il.szsharing.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://km.nicolike.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://vm.panjiajie.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ez.colortex.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ol.nszjky.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://vp.szxytkj.cn

================================================================================
来源：http://ki.colortex.cn

O. 并发与异步
来源：http://yg.muxihuayi.cn

================================================================================
来源：http://st.shtwfgs.cn

[O01] 启动一个线程
来源：http://tl.newstarts.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wx.jianghongdianzi.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://uo.muxihuayi.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ja.lnxyls.cn

TS:   // 同 JS
来源：http://mt.bookmarksfly.cn

Java: new Thread(() -> f()).start()
来源：http://fc.lnxyls.cn

Go:   go f()
来源：http://yd.shxzskj.cn

Ruby: Thread.new { f }
来源：http://rk.newstarts.cn

C#:   Task.Run(() => F());
来源：http://fk.shxzskj.cn

[O02] 使用线程池
来源：http://ci.gzmigu.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ly.szsharing.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://cy.yuexingan06.cn

JS:   // worker_threads 线程池
来源：http://dq.shxzskj.cn

TS:   // worker_threads 线程池
来源：http://ue.9csxet.cn

Java: Executors.newFixedThreadPool(4)
来源：http://gq.huixiangedu.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://po.shtwfgs.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://gk.521024.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://dc.nicolike.cn

[O03] 加锁保护共享数据
来源：http://wn.shxzskj.cn

Py:   with lock: shared += 1
来源：http://pc.jianghongdianzi.cn

PHP:  // 用 flock() 做文件锁
来源：http://vk.lnxyls.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://uk.nicolike.cn

TS:   // 同 JS
来源：http://fz.panjiajie.cn

Java: synchronized (this) { shared++; }
来源：http://ts.asd995.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mm.521024.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://pm.chemitech.net.cn

C#:   lock (gate) { shared++; }
来源：http://qo.chemitech.net.cn

[O04] 定义异步函数并等待
来源：http://sx.nicolike.cn

Py:   async def f():⏎    await g()
来源：http://wc.shxzskj.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://yq.nicolike.cn

JS:   async function f() { await g(); }
来源：http://rj.jctech888.com.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://ei.hahajie.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://vd.chemitech.net.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://nj.shxzskj.cn

Ruby: # 用 Fiber 或 async gem
来源：http://up.wgjwhj.cn

C#:   async Task F() { await G(); }
来源：http://xc.huixiangedu.cn

[O05] 并发执行并等待全部完成
来源：http://et.yuntaijiaju.cn

Py:   asyncio.gather(*tasks)
来源：http://qf.haigaiapp.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hd.asd995.cn

JS:   await Promise.all(tasks)
来源：http://vb.muxihuayi.cn

TS:   await Promise.all(tasks)
来源：http://ej.lnxyls.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://cv.huixinmuqiang.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ns.nszjky.cn

Ruby: threads.map(&:join)
来源：http://ga.yuexingan06.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://pu.panjiajie.cn

[O06] 使用进程池
来源：http://cy.colortex.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://bf.wgjwhj.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://se.huixinmuqiang.cn

JS:   // child_process / cluster 模块
来源：http://gz.chemitech.net.cn

TS:   // child_process / cluster 模块
来源：http://ru.szsharing.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://vo.yuexingan06.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://en.wgjwhj.cn

Ruby: // fork 块
来源：http://vo.colortex.cn

C#:   Parallel.For
来源：http://dq.shxzskj.cn

================================================================================
来源：http://xa.chemitech.net.cn

P. 常用工具函数
来源：http://re.yuntaijiaju.cn

================================================================================
来源：http://gj.panjiajie.cn

[P01] 生成 UUID
来源：http://rx.bookmarksfly.cn

Py:   str(uuid.uuid4())
来源：http://ad.nicolike.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ui.wgjwhj.cn

JS:   crypto.randomUUID()
来源：http://av.haigaiapp.cn

TS:   crypto.randomUUID()
来源：http://sy.hnjuh.cn

Java: UUID.randomUUID().toString()
来源：http://ve.jianghongdianzi.cn

Go:   // 用 github.com/google/uuid
来源：http://hs.muxihuayi.cn

Ruby: SecureRandom.uuid
来源：http://fw.huixiangedu.cn

C#:   Guid.NewGuid().ToString()
来源：http://bz.gzmigu.cn

[P02] MD5 / SHA256 摘要
来源：http://gf.521024.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://eb.shxzukj.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://ji.panjiajie.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://du.yuntaijiaju.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://pd.szsharing.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://kp.shxzukj.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://cc.chemitech.net.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://nk.nicolike.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://dr.521024.cn

[P03] 生成短随机字符串
来源：http://vk.szsharing.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hc.colortex.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://df.yuexingan06.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ca.szsharing.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://bz.hahajie.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ac.bjjhwx.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://pb.chemitech.net.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://up.yuntaijiaju.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://rz.haigaiapp.cn

[P04] 求长度
来源：http://af.hnjuh.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wl.panjiajie.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ly.shxzukj.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://sr.muxihuayi.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://qa.panjiajie.cn

Java: list.size();  map.size();  s.length()
来源：http://yb.huixiangedu.cn

Go:   len(arr);  len(m)
来源：http://od.asd995.cn

Ruby: x.length;  x.size
来源：http://jj.szxytkj.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://mn.bookmarksfly.cn

[P05] 判断两个对象内容是否相等
来源：http://kw.521024.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://sd.yuexingan06.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://tj.jianghongdianzi.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hu.lnxyls.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://lv.lnxyls.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://si.shtwfgs.cn

Go:   reflect.DeepEqual(a, b)
来源：http://bh.hahajie.cn

Ruby: a == b
来源：http://wj.yuntaijiaju.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ac.shxzukj.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://er.jianghongdianzi.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wj.asd995.cn

PHP:  if (empty($x)) {}
来源：http://zn.nszjky.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wo.muxihuayi.cn

TS:   if (x == null) {}
来源：http://al.szsharing.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://zb.yuexingan06.cn

Go:   if x == nil {}
来源：http://co.shtwfgs.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://pz.asd995.cn

C#:   if (x is null) {}
来源：http://ut.shxzukj.cn

[P07] 防抖与节流
来源：http://rv.huixinmuqiang.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://gg.jianghongdianzi.cn

PHP:  // 手写时间戳比较
来源：http://qt.shtwfgs.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xg.shtwfgs.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://zb.muxihuayi.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://nj.yuntaijiaju.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ml.szsharing.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://hn.asd995.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://bd.shxzukj.cn

[P08] 处理浮点精度问题
来源：http://gg.jctech888.com.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://rb.szsharing.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://kr.huanxung.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://xo.hnjuh.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://qh.shxzskj.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://lz.newstarts.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://bl.bookmarksfly.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ct.huanxung.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://yz.haigaiapp.cn

================================================================================
来源：http://ai.jctech888.com.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://fk.colortex.cn

================================================================================
来源：http://kf.bookmarksfly.cn

[Q01] 创建表
来源：http://vf.bookmarksfly.cn

CREATE TABLE users (
来源：http://oj.wgjwhj.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ks.bookmarksfly.cn

name VARCHAR(50) NOT NULL,
来源：http://km.bookmarksfly.cn

email VARCHAR(100) UNIQUE,
来源：http://pw.lnxyls.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://fm.haigaiapp.cn

);
来源：http://qf.9csxet.cn

[Q02] 创建带外键的表
来源：http://lp.newstarts.cn

CREATE TABLE orders (
来源：http://yo.haigaiapp.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://jk.huixiangedu.cn

user_id INT NOT NULL,
来源：http://st.521024.cn

amount DECIMAL(10, 2),
来源：http://nz.hnjuh.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://gu.asd995.cn


<!-- 参考信息 -->