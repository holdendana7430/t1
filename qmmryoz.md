代发 wailian999

[M04] 获取当前工作目录
来源：http://yj.shtwfgs.cn

Py:   os.getcwd()
来源：http://bw.asd995.cn

PHP:  getcwd();
来源：http://xk.nicolike.cn

JS:   process.cwd()
来源：http://ww.jianghongdianzi.cn

TS:   process.cwd()
来源：http://sn.yuntaijiaju.cn

Java: Path.of("").toAbsolutePath()
来源：http://ku.shxzukj.cn

Go:   os.Getwd()
来源：http://bu.haigaiapp.cn

Ruby: Dir.pwd
来源：http://pc.521024.cn

C#:   Directory.GetCurrentDirectory()
来源：http://xq.huanxung.cn

[M05] 设置退出码
来源：http://ru.nicolike.cn

Py:   sys.exit(1)
来源：http://sv.gzmigu.cn

PHP:  exit(1);
来源：http://dr.shxzukj.cn

JS:   process.exit(1)
来源：http://rr.asd995.cn

TS:   process.exit(1)
来源：http://pt.hahajie.cn

Java: System.exit(1)
来源：http://xx.panjiajie.cn

Go:   os.Exit(1)
来源：http://hf.jctech888.com.cn

Ruby: exit 1
来源：http://ug.colortex.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ki.nszjky.cn

[M06] 向标准错误输出
来源：http://fk.shtwfgs.cn

Py:   print("err", file=sys.stderr)
来源：http://qz.521024.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://gl.shxzukj.cn

JS:   console.error("err")
来源：http://ir.shxzskj.cn

TS:   console.error("err")
来源：http://pa.521024.cn

Java: System.err.println("err")
来源：http://ho.hnjuh.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ch.asd995.cn

Ruby: warn "err"
来源：http://sv.hahajie.cn

C#:   Console.Error.WriteLine("err")
来源：http://iu.szsharing.cn

[M07] 判断是否为主入口
来源：http://iy.szsharing.cn

Py:   if __name__ == "__main__":
来源：http://dr.wgjwhj.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://bn.jctech888.com.cn

JS:   require.main === module
来源：http://av.huixiangedu.cn

TS:   require.main === module
来源：http://dk.newstarts.cn

Java: public static void main(String[] args)
来源：http://xw.haigaiapp.cn

Go:   func main()
来源：http://kk.hahajie.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ms.bookmarksfly.cn

C#:   static void Main(string[] args)
来源：http://zq.haigaiapp.cn

[M08] 获取系统与运行时信息
来源：http://ln.colortex.cn

Py:   platform.system();  platform.python_version()
来源：http://km.chemitech.net.cn

PHP:  PHP_OS;  phpversion();
来源：http://au.huixinmuqiang.cn

JS:   process.platform;  process.version
来源：http://ej.huixinmuqiang.cn

TS:   process.platform;  process.version
来源：http://kh.colortex.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://os.jctech888.com.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://bg.521024.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://cu.jctech888.com.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://fo.jianghongdianzi.cn

================================================================================
来源：http://wy.gzmigu.cn

N. 数据结构与算法
来源：http://ko.newstarts.cn

================================================================================
来源：http://lf.wgjwhj.cn

[N01] 二分查找（有序数组）
来源：http://tf.lnxyls.cn

Py:   bisect.bisect_left(arr, x)
来源：http://gi.panjiajie.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ne.nicolike.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wk.521024.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://jg.yuexingan06.cn

Java: Arrays.binarySearch(arr, x)
来源：http://uh.panjiajie.cn

Go:   sort.SearchInts(arr, x)
来源：http://ag.shtwfgs.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://vj.chemitech.net.cn

C#:   Array.BinarySearch(arr, x)
来源：http://tr.bjjhwx.cn

[N02] 排序（工程实践用内置实现）
来源：http://vv.szsharing.cn

Py:   sorted(arr);  arr.sort()
来源：http://lb.panjiajie.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://au.gzmigu.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://ns.9csxet.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://fz.yuntaijiaju.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://fz.bookmarksfly.cn

Go:   slices.Sort(arr)
来源：http://gu.newstarts.cn

Ruby: arr.sort
来源：http://zt.hahajie.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://oe.shxzskj.cn

[N03] 快速排序（分治示例）
来源：http://ad.muxihuayi.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ke.nszjky.cn

PHP:  // 递归实现，或用 usort
来源：http://ls.jctech888.com.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://kf.hnjuh.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://xp.hnjuh.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://me.huixinmuqiang.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://fu.shxzukj.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ej.gzmigu.cn

C#:   // 手写递归，或 Array.Sort
来源：http://wc.521024.cn

[N04] 斐波那契数列
来源：http://cq.huixiangedu.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://md.wgjwhj.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://dd.9csxet.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wo.nszjky.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://lp.muxihuayi.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://nl.shxzskj.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ps.bjjhwx.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://lt.szsharing.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://cw.huixiangedu.cn

[N05] 最大公约数
来源：http://og.yuexingan06.cn

Py:   math.gcd(a, b)
来源：http://st.newstarts.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://of.szxytkj.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ik.haigaiapp.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://if.bjjhwx.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://nf.muxihuayi.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://px.bjjhwx.cn

Ruby: a.gcd(b)
来源：http://fb.nicolike.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://iq.bjjhwx.cn

[N06] 判断回文字符串
来源：http://xj.wgjwhj.cn

Py:   s == s[::-1]
来源：http://xd.colortex.cn

PHP:  $s === strrev($s);
来源：http://kg.521024.cn

JS:   s === [...s].reverse().join("")
来源：http://tn.szsharing.cn

TS:   s === [...s].reverse().join("")
来源：http://oc.huixinmuqiang.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wt.huanxung.cn

Go:   // 双指针从两端比较
来源：http://fu.yuntaijiaju.cn

Ruby: s == s.reverse
来源：http://sm.bookmarksfly.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://hd.huixiangedu.cn

[N07] 两数之和（返回下标）
来源：http://tl.newstarts.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://gv.9csxet.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://sv.lnxyls.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://ac.shxzukj.cn

TS:   // 手写 Map<string, number>
来源：http://ca.colortex.cn

Java: // 手写 HashMap
来源：http://hi.colortex.cn

Go:   // 手写 map[int]int
来源：http://qo.9csxet.cn

Ruby: // 手写 Hash
来源：http://py.newstarts.cn

C#:   // 手写 Dictionary<int, int>
来源：http://aa.nszjky.cn

[N08] 生成全排列
来源：http://kg.gzmigu.cn

Py:   itertools.permutations(arr)
来源：http://ic.chemitech.net.cn

PHP:  // 手写递归交换
来源：http://jq.yuexingan06.cn

JS:   // 手写回溯递归
来源：http://ol.nicolike.cn

TS:   // 手写回溯递归
来源：http://bo.jctech888.com.cn

Java: // 手写回溯递归
来源：http://ga.yuexingan06.cn

Go:   // 手写回溯递归
来源：http://gl.gzmigu.cn

Ruby: arr.permutation.to_a
来源：http://mu.haigaiapp.cn

C#:   // 手写回溯递归
来源：http://iw.newstarts.cn

[N09] 栈与队列
来源：http://aq.szsharing.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://jx.chemitech.net.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mm.gzmigu.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://si.yuexingan06.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://tc.hahajie.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://rk.chemitech.net.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://cj.yuexingan06.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ai.lnxyls.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://eq.nicolike.cn

[N10] 链表节点定义
来源：http://kv.yuntaijiaju.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://oy.huanxung.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.shxzukj.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://df.wgjwhj.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ls.haigaiapp.cn

Java: class Node { int v; Node next; }
来源：http://tk.shxzukj.cn

Go:   type Node struct { V int; Next *Node }
来源：http://do.jctech888.com.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://yy.muxihuayi.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://oe.yuexingan06.cn

[N11] 二叉树中序遍历
来源：http://yx.wgjwhj.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://tp.shtwfgs.cn

PHP:  // 手写递归函数
来源：http://fm.gzmigu.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://yi.jianghongdianzi.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://po.521024.cn

Java: // 手写递归
来源：http://wg.nszjky.cn

Go:   // 手写递归
来源：http://lv.jianghongdianzi.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ef.huixinmuqiang.cn

C#:   // 手写递归
来源：http://lb.jctech888.com.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wl.yuntaijiaju.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://vv.chemitech.net.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://vk.nicolike.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://fn.muxihuayi.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://tc.shxzskj.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://cp.colortex.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://tl.shxzskj.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://id.szxytkj.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://oo.szxytkj.cn

================================================================================
来源：http://kl.gzmigu.cn

O. 并发与异步
来源：http://ba.bjjhwx.cn

================================================================================
来源：http://ny.newstarts.cn

[O01] 启动一个线程
来源：http://fd.wgjwhj.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://xk.yuntaijiaju.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://nc.yuexingan06.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://bj.newstarts.cn

TS:   // 同 JS
来源：http://bo.jianghongdianzi.cn

Java: new Thread(() -> f()).start()
来源：http://wf.huanxung.cn

Go:   go f()
来源：http://kd.nicolike.cn

Ruby: Thread.new { f }
来源：http://gm.newstarts.cn

C#:   Task.Run(() => F());
来源：http://oh.haigaiapp.cn

[O02] 使用线程池
来源：http://ca.haigaiapp.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mg.asd995.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ic.9csxet.cn

JS:   // worker_threads 线程池
来源：http://fk.521024.cn

TS:   // worker_threads 线程池
来源：http://dt.muxihuayi.cn

Java: Executors.newFixedThreadPool(4)
来源：http://lg.huanxung.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ob.jctech888.com.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://sh.521024.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://xb.huixinmuqiang.cn

[O03] 加锁保护共享数据
来源：http://fd.shxzukj.cn

Py:   with lock: shared += 1
来源：http://ip.szxytkj.cn

PHP:  // 用 flock() 做文件锁
来源：http://wn.nicolike.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://zq.lnxyls.cn

TS:   // 同 JS
来源：http://iy.gzmigu.cn

Java: synchronized (this) { shared++; }
来源：http://lh.nicolike.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://cy.yuntaijiaju.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://sy.lnxyls.cn

C#:   lock (gate) { shared++; }
来源：http://yv.muxihuayi.cn

[O04] 定义异步函数并等待
来源：http://qu.panjiajie.cn

Py:   async def f():⏎    await g()
来源：http://qe.muxihuayi.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://xw.shxzskj.cn

JS:   async function f() { await g(); }
来源：http://kr.bookmarksfly.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://kp.muxihuayi.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://pu.gzmigu.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ho.hnjuh.cn

Ruby: # 用 Fiber 或 async gem
来源：http://nf.hnjuh.cn

C#:   async Task F() { await G(); }
来源：http://gp.szsharing.cn

[O05] 并发执行并等待全部完成
来源：http://ga.hahajie.cn

Py:   asyncio.gather(*tasks)
来源：http://im.szxytkj.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://zn.wgjwhj.cn

JS:   await Promise.all(tasks)
来源：http://ix.panjiajie.cn

TS:   await Promise.all(tasks)
来源：http://hk.lnxyls.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://pj.wgjwhj.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ku.jctech888.com.cn

Ruby: threads.map(&:join)
来源：http://hx.bookmarksfly.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://cp.shxzukj.cn

[O06] 使用进程池
来源：http://pa.shtwfgs.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://zv.yuntaijiaju.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://yr.gzmigu.cn

JS:   // child_process / cluster 模块
来源：http://wa.gzmigu.cn

TS:   // child_process / cluster 模块
来源：http://hw.bjjhwx.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://al.wgjwhj.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ft.szsharing.cn

Ruby: // fork 块
来源：http://sl.shxzskj.cn

C#:   Parallel.For
来源：http://tf.hnjuh.cn

================================================================================
来源：http://lu.hahajie.cn

P. 常用工具函数
来源：http://zj.gzmigu.cn

================================================================================
来源：http://zr.gzmigu.cn

[P01] 生成 UUID
来源：http://hs.9csxet.cn

Py:   str(uuid.uuid4())
来源：http://ve.szxytkj.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mk.newstarts.cn

JS:   crypto.randomUUID()
来源：http://mf.shxzskj.cn

TS:   crypto.randomUUID()
来源：http://gp.haigaiapp.cn

Java: UUID.randomUUID().toString()
来源：http://kq.gzmigu.cn

Go:   // 用 github.com/google/uuid
来源：http://dx.nszjky.cn

Ruby: SecureRandom.uuid
来源：http://eh.shtwfgs.cn

C#:   Guid.NewGuid().ToString()
来源：http://ok.jianghongdianzi.cn

[P02] MD5 / SHA256 摘要
来源：http://vv.panjiajie.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ra.muxihuayi.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://rz.hahajie.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://it.huixiangedu.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mx.szsharing.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://bl.521024.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ib.panjiajie.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://sv.jianghongdianzi.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://sm.huixinmuqiang.cn

[P03] 生成短随机字符串
来源：http://bw.muxihuayi.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://vc.bookmarksfly.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ne.jctech888.com.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://pm.shtwfgs.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://yr.yuntaijiaju.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://fe.huixinmuqiang.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://dn.shxzukj.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://co.jctech888.com.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ej.bookmarksfly.cn

[P04] 求长度
来源：http://xh.lnxyls.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wl.nicolike.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://fb.huanxung.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://nz.521024.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hs.huixiangedu.cn

Java: list.size();  map.size();  s.length()
来源：http://io.haigaiapp.cn

Go:   len(arr);  len(m)
来源：http://yp.newstarts.cn

Ruby: x.length;  x.size
来源：http://za.chemitech.net.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://ue.szsharing.cn

[P05] 判断两个对象内容是否相等
来源：http://mr.muxihuayi.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://em.nicolike.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://lu.szsharing.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ee.nicolike.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ce.hnjuh.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://gf.gzmigu.cn

Go:   reflect.DeepEqual(a, b)
来源：http://wo.asd995.cn

Ruby: a == b
来源：http://fv.bookmarksfly.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ae.szsharing.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://yz.jctech888.com.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://gu.asd995.cn

PHP:  if (empty($x)) {}
来源：http://vt.521024.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://vm.bookmarksfly.cn

TS:   if (x == null) {}
来源：http://xs.hahajie.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://uk.huixinmuqiang.cn

Go:   if x == nil {}
来源：http://vy.shtwfgs.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://cb.521024.cn

C#:   if (x is null) {}
来源：http://ja.panjiajie.cn

[P07] 防抖与节流
来源：http://zq.yuntaijiaju.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://cm.huixinmuqiang.cn

PHP:  // 手写时间戳比较
来源：http://ae.yuexingan06.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://rh.muxihuayi.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://nu.jctech888.com.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://tn.hnjuh.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ju.jianghongdianzi.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://uh.wgjwhj.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://tn.521024.cn

[P08] 处理浮点精度问题
来源：http://sw.huixiangedu.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://cj.panjiajie.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://kg.haigaiapp.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://pi.hahajie.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://dt.huixiangedu.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://nx.shxzskj.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://dp.nicolike.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ds.jianghongdianzi.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://im.haigaiapp.cn

================================================================================
来源：http://qz.szxytkj.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ae.bookmarksfly.cn

================================================================================
来源：http://hj.shtwfgs.cn

[Q01] 创建表
来源：http://mn.huixiangedu.cn

CREATE TABLE users (
来源：http://ea.muxihuayi.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://tw.colortex.cn

name VARCHAR(50) NOT NULL,
来源：http://fn.huanxung.cn

email VARCHAR(100) UNIQUE,
来源：http://xb.huixiangedu.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mk.hnjuh.cn

);
来源：http://kv.szxytkj.cn

[Q02] 创建带外键的表
来源：http://mv.panjiajie.cn

CREATE TABLE orders (
来源：http://kt.shxzukj.cn


<!-- 参考信息 -->