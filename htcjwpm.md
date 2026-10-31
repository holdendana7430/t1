代发 wailian999

C#:   Directory.GetCurrentDirectory()
来源：http://ay.colortex.cn

[M05] 设置退出码
来源：http://wl.shxzskj.cn

Py:   sys.exit(1)
来源：http://hk.nicolike.cn

PHP:  exit(1);
来源：http://fm.521024.cn

JS:   process.exit(1)
来源：http://jt.huanxung.cn

TS:   process.exit(1)
来源：http://od.muxihuayi.cn

Java: System.exit(1)
来源：http://gb.huanxung.cn

Go:   os.Exit(1)
来源：http://ey.shtwfgs.cn

Ruby: exit 1
来源：http://zh.521024.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://rc.yuntaijiaju.cn

[M06] 向标准错误输出
来源：http://zd.muxihuayi.cn

Py:   print("err", file=sys.stderr)
来源：http://cy.panjiajie.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://az.hahajie.cn

JS:   console.error("err")
来源：http://tw.jctech888.com.cn

TS:   console.error("err")
来源：http://gg.jianghongdianzi.cn

Java: System.err.println("err")
来源：http://ss.muxihuayi.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://xu.wgjwhj.cn

Ruby: warn "err"
来源：http://zj.bookmarksfly.cn

C#:   Console.Error.WriteLine("err")
来源：http://iv.jctech888.com.cn

[M07] 判断是否为主入口
来源：http://ty.szsharing.cn

Py:   if __name__ == "__main__":
来源：http://kb.muxihuayi.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://bz.chemitech.net.cn

JS:   require.main === module
来源：http://kx.huixinmuqiang.cn

TS:   require.main === module
来源：http://qs.9csxet.cn

Java: public static void main(String[] args)
来源：http://bs.jctech888.com.cn

Go:   func main()
来源：http://ya.nszjky.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://qu.shtwfgs.cn

C#:   static void Main(string[] args)
来源：http://fb.nicolike.cn

[M08] 获取系统与运行时信息
来源：http://tc.9csxet.cn

Py:   platform.system();  platform.python_version()
来源：http://ur.yuexingan06.cn

PHP:  PHP_OS;  phpversion();
来源：http://ai.521024.cn

JS:   process.platform;  process.version
来源：http://zo.huanxung.cn

TS:   process.platform;  process.version
来源：http://fm.shxzskj.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://we.hahajie.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://qk.wgjwhj.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://qh.newstarts.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://bi.521024.cn

================================================================================
来源：http://ns.nicolike.cn

N. 数据结构与算法
来源：http://et.colortex.cn

================================================================================
来源：http://zp.wgjwhj.cn

[N01] 二分查找（有序数组）
来源：http://ip.9csxet.cn

Py:   bisect.bisect_left(arr, x)
来源：http://by.hnjuh.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://uh.szsharing.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://re.hnjuh.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ch.hnjuh.cn

Java: Arrays.binarySearch(arr, x)
来源：http://ui.gzmigu.cn

Go:   sort.SearchInts(arr, x)
来源：http://gd.huixiangedu.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://tb.hahajie.cn

C#:   Array.BinarySearch(arr, x)
来源：http://ic.newstarts.cn

[N02] 排序（工程实践用内置实现）
来源：http://jj.9csxet.cn

Py:   sorted(arr);  arr.sort()
来源：http://ni.newstarts.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://qe.chemitech.net.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://mr.shxzukj.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://gc.asd995.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://sr.shxzukj.cn

Go:   slices.Sort(arr)
来源：http://rw.asd995.cn

Ruby: arr.sort
来源：http://yt.jctech888.com.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://dj.wgjwhj.cn

[N03] 快速排序（分治示例）
来源：http://ln.lnxyls.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hb.huixinmuqiang.cn

PHP:  // 递归实现，或用 usort
来源：http://iz.szsharing.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://zf.newstarts.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://qh.bookmarksfly.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://kx.asd995.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://yo.shxzukj.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://pu.chemitech.net.cn

C#:   // 手写递归，或 Array.Sort
来源：http://zr.wgjwhj.cn

[N04] 斐波那契数列
来源：http://aq.shtwfgs.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://bb.nszjky.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://am.szxytkj.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ji.521024.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://eo.asd995.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://sc.haigaiapp.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://vn.gzmigu.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hl.lnxyls.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mb.yuntaijiaju.cn

[N05] 最大公约数
来源：http://qv.huixinmuqiang.cn

Py:   math.gcd(a, b)
来源：http://rj.nszjky.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://qi.jianghongdianzi.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://cj.bookmarksfly.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://cy.newstarts.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ef.nszjky.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://af.chemitech.net.cn

Ruby: a.gcd(b)
来源：http://az.nicolike.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://re.wgjwhj.cn

[N06] 判断回文字符串
来源：http://jz.newstarts.cn

Py:   s == s[::-1]
来源：http://rn.nszjky.cn

PHP:  $s === strrev($s);
来源：http://nm.chemitech.net.cn

JS:   s === [...s].reverse().join("")
来源：http://cm.yuexingan06.cn

TS:   s === [...s].reverse().join("")
来源：http://uu.bookmarksfly.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://la.jianghongdianzi.cn

Go:   // 双指针从两端比较
来源：http://rk.panjiajie.cn

Ruby: s == s.reverse
来源：http://sm.nszjky.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://bn.colortex.cn

[N07] 两数之和（返回下标）
来源：http://tb.gzmigu.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ki.shtwfgs.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://po.shxzukj.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://iv.shtwfgs.cn

TS:   // 手写 Map<string, number>
来源：http://ri.colortex.cn

Java: // 手写 HashMap
来源：http://fn.jctech888.com.cn

Go:   // 手写 map[int]int
来源：http://hm.nicolike.cn

Ruby: // 手写 Hash
来源：http://gn.jctech888.com.cn

C#:   // 手写 Dictionary<int, int>
来源：http://km.hnjuh.cn

[N08] 生成全排列
来源：http://pi.9csxet.cn

Py:   itertools.permutations(arr)
来源：http://vf.newstarts.cn

PHP:  // 手写递归交换
来源：http://vw.szxytkj.cn

JS:   // 手写回溯递归
来源：http://rd.chemitech.net.cn

TS:   // 手写回溯递归
来源：http://nt.newstarts.cn

Java: // 手写回溯递归
来源：http://sx.shxzukj.cn

Go:   // 手写回溯递归
来源：http://xj.chemitech.net.cn

Ruby: arr.permutation.to_a
来源：http://bq.9csxet.cn

C#:   // 手写回溯递归
来源：http://px.asd995.cn

[N09] 栈与队列
来源：http://nw.shxzukj.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://yl.colortex.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://gy.bjjhwx.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://rj.jianghongdianzi.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://er.wgjwhj.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ij.asd995.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://jg.521024.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://im.hnjuh.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ay.gzmigu.cn

[N10] 链表节点定义
来源：http://nv.lnxyls.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://rk.jctech888.com.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://ph.shxzukj.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ni.gzmigu.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ca.shtwfgs.cn

Java: class Node { int v; Node next; }
来源：http://ul.shxzukj.cn

Go:   type Node struct { V int; Next *Node }
来源：http://xb.hahajie.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://ix.colortex.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://if.nszjky.cn

[N11] 二叉树中序遍历
来源：http://bk.jianghongdianzi.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://fx.yuntaijiaju.cn

PHP:  // 手写递归函数
来源：http://un.shxzskj.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ft.panjiajie.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ih.szxytkj.cn

Java: // 手写递归
来源：http://yj.huanxung.cn

Go:   // 手写递归
来源：http://ba.szsharing.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://pd.haigaiapp.cn

C#:   // 手写递归
来源：http://le.muxihuayi.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://je.shxzukj.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://dg.nszjky.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ni.huixiangedu.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.chemitech.net.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://zw.lnxyls.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://eo.huixinmuqiang.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://my.wgjwhj.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://yu.nszjky.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://yd.szsharing.cn

================================================================================
来源：http://rc.hnjuh.cn

O. 并发与异步
来源：http://ih.jianghongdianzi.cn

================================================================================
来源：http://xb.chemitech.net.cn

[O01] 启动一个线程
来源：http://qf.huixinmuqiang.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://vs.muxihuayi.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://xb.gzmigu.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://qu.nicolike.cn

TS:   // 同 JS
来源：http://xy.muxihuayi.cn

Java: new Thread(() -> f()).start()
来源：http://bt.gzmigu.cn

Go:   go f()
来源：http://do.chemitech.net.cn

Ruby: Thread.new { f }
来源：http://rw.haigaiapp.cn

C#:   Task.Run(() => F());
来源：http://eg.bookmarksfly.cn

[O02] 使用线程池
来源：http://kd.panjiajie.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://fn.haigaiapp.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://vs.chemitech.net.cn

JS:   // worker_threads 线程池
来源：http://mo.haigaiapp.cn

TS:   // worker_threads 线程池
来源：http://rm.huixinmuqiang.cn

Java: Executors.newFixedThreadPool(4)
来源：http://ro.shxzskj.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hm.wgjwhj.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ob.chemitech.net.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://td.bjjhwx.cn

[O03] 加锁保护共享数据
来源：http://tj.newstarts.cn

Py:   with lock: shared += 1
来源：http://hc.hnjuh.cn

PHP:  // 用 flock() 做文件锁
来源：http://hx.haigaiapp.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ah.panjiajie.cn

TS:   // 同 JS
来源：http://mq.panjiajie.cn

Java: synchronized (this) { shared++; }
来源：http://tb.hahajie.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ca.nszjky.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://id.muxihuayi.cn

C#:   lock (gate) { shared++; }
来源：http://ec.nicolike.cn

[O04] 定义异步函数并等待
来源：http://rf.jianghongdianzi.cn

Py:   async def f():⏎    await g()
来源：http://mp.jianghongdianzi.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://tq.bookmarksfly.cn

JS:   async function f() { await g(); }
来源：http://ug.gzmigu.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://ap.gzmigu.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://nr.haigaiapp.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://gb.9csxet.cn

Ruby: # 用 Fiber 或 async gem
来源：http://cg.haigaiapp.cn

C#:   async Task F() { await G(); }
来源：http://ev.huixinmuqiang.cn

[O05] 并发执行并等待全部完成
来源：http://pr.nszjky.cn

Py:   asyncio.gather(*tasks)
来源：http://iy.bjjhwx.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://yx.panjiajie.cn

JS:   await Promise.all(tasks)
来源：http://bu.521024.cn

TS:   await Promise.all(tasks)
来源：http://xl.newstarts.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://zm.panjiajie.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wu.jianghongdianzi.cn

Ruby: threads.map(&:join)
来源：http://ia.nszjky.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://te.wgjwhj.cn

[O06] 使用进程池
来源：http://wo.bookmarksfly.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ri.lnxyls.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://yq.chemitech.net.cn

JS:   // child_process / cluster 模块
来源：http://xw.szxytkj.cn

TS:   // child_process / cluster 模块
来源：http://cs.yuntaijiaju.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://he.nszjky.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://dk.szsharing.cn

Ruby: // fork 块
来源：http://ie.nicolike.cn

C#:   Parallel.For
来源：http://fi.szsharing.cn

================================================================================
来源：http://zs.521024.cn

P. 常用工具函数
来源：http://ab.szxytkj.cn

================================================================================
来源：http://hc.lnxyls.cn

[P01] 生成 UUID
来源：http://mx.bjjhwx.cn

Py:   str(uuid.uuid4())
来源：http://me.yuntaijiaju.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://qq.hahajie.cn

JS:   crypto.randomUUID()
来源：http://pi.asd995.cn

TS:   crypto.randomUUID()
来源：http://ql.shxzukj.cn

Java: UUID.randomUUID().toString()
来源：http://sp.gzmigu.cn

Go:   // 用 github.com/google/uuid
来源：http://fv.szsharing.cn

Ruby: SecureRandom.uuid
来源：http://rv.hahajie.cn

C#:   Guid.NewGuid().ToString()
来源：http://wz.huixinmuqiang.cn

[P02] MD5 / SHA256 摘要
来源：http://qr.szsharing.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ne.gzmigu.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://ac.huixinmuqiang.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://op.yuexingan06.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://rn.shxzukj.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://as.wgjwhj.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://uz.gzmigu.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://fg.huanxung.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ya.huixinmuqiang.cn

[P03] 生成短随机字符串
来源：http://ag.shtwfgs.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hy.yuexingan06.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://um.yuntaijiaju.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://de.yuntaijiaju.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wz.jctech888.com.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://yl.hnjuh.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://zv.chemitech.net.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://qb.panjiajie.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hy.shtwfgs.cn

[P04] 求长度
来源：http://ux.bjjhwx.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://em.bookmarksfly.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ut.gzmigu.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ic.nszjky.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://gl.newstarts.cn

Java: list.size();  map.size();  s.length()
来源：http://lx.chemitech.net.cn

Go:   len(arr);  len(m)
来源：http://jc.huanxung.cn

Ruby: x.length;  x.size
来源：http://gs.haigaiapp.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://um.shxzskj.cn

[P05] 判断两个对象内容是否相等
来源：http://sy.szxytkj.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://ww.huixinmuqiang.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://dh.chemitech.net.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://jr.colortex.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://yg.jianghongdianzi.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://pf.shxzukj.cn

Go:   reflect.DeepEqual(a, b)
来源：http://ue.asd995.cn

Ruby: a == b
来源：http://pp.hnjuh.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://xr.shxzukj.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://cm.panjiajie.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://co.jctech888.com.cn

PHP:  if (empty($x)) {}
来源：http://ig.colortex.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://jn.panjiajie.cn

TS:   if (x == null) {}
来源：http://yr.bookmarksfly.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://ng.newstarts.cn

Go:   if x == nil {}
来源：http://nb.yuexingan06.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://io.asd995.cn

C#:   if (x is null) {}
来源：http://jk.huixiangedu.cn

[P07] 防抖与节流
来源：http://er.newstarts.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://eo.chemitech.net.cn

PHP:  // 手写时间戳比较
来源：http://wk.bjjhwx.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://rv.colortex.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ve.jctech888.com.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://pt.colortex.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ya.shxzukj.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://qn.shtwfgs.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://dl.9csxet.cn

[P08] 处理浮点精度问题
来源：http://mk.szxytkj.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://dw.hahajie.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://jk.nicolike.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://cz.nszjky.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://pt.huanxung.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://gn.521024.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mp.newstarts.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://rv.shtwfgs.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ja.521024.cn

================================================================================
来源：http://te.szxytkj.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ys.shxzskj.cn

================================================================================
来源：http://ia.asd995.cn

[Q01] 创建表
来源：http://ya.9csxet.cn

CREATE TABLE users (
来源：http://qs.shxzskj.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://yw.shxzskj.cn

name VARCHAR(50) NOT NULL,
来源：http://bs.szsharing.cn

email VARCHAR(100) UNIQUE,
来源：http://py.newstarts.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mi.haigaiapp.cn

);
来源：http://et.huanxung.cn

[Q02] 创建带外键的表
来源：http://cx.bjjhwx.cn

CREATE TABLE orders (
来源：http://qv.hahajie.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://up.huixinmuqiang.cn

user_id INT NOT NULL,
来源：http://xv.shxzskj.cn

amount DECIMAL(10, 2),
来源：http://le.shtwfgs.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://om.nicolike.cn

);
来源：http://rt.colortex.cn

[Q03] 增加列
来源：http://ne.chemitech.net.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wo.yuntaijiaju.cn

[Q04] 修改列类型
来源：http://yb.haigaiapp.cn


<!-- 参考信息 -->