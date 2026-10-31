代发 wailian999

C#:   Directory.GetCurrentDirectory()
来源：http://xh.chemitech.net.cn

[M05] 设置退出码
来源：http://se.newstarts.cn

Py:   sys.exit(1)
来源：http://aa.panjiajie.cn

PHP:  exit(1);
来源：http://zd.gzmigu.cn

JS:   process.exit(1)
来源：http://rv.9csxet.cn

TS:   process.exit(1)
来源：http://ss.hahajie.cn

Java: System.exit(1)
来源：http://cg.9csxet.cn

Go:   os.Exit(1)
来源：http://wl.bjjhwx.cn

Ruby: exit 1
来源：http://yf.lnxyls.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://tb.huixiangedu.cn

[M06] 向标准错误输出
来源：http://hv.nicolike.cn

Py:   print("err", file=sys.stderr)
来源：http://ny.jianghongdianzi.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://bh.wgjwhj.cn

JS:   console.error("err")
来源：http://eu.gzmigu.cn

TS:   console.error("err")
来源：http://zv.yuexingan06.cn

Java: System.err.println("err")
来源：http://zm.jianghongdianzi.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://nh.szsharing.cn

Ruby: warn "err"
来源：http://zh.muxihuayi.cn

C#:   Console.Error.WriteLine("err")
来源：http://cz.newstarts.cn

[M07] 判断是否为主入口
来源：http://xb.hnjuh.cn

Py:   if __name__ == "__main__":
来源：http://oc.huanxung.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://cc.yuexingan06.cn

JS:   require.main === module
来源：http://jo.jianghongdianzi.cn

TS:   require.main === module
来源：http://gv.lnxyls.cn

Java: public static void main(String[] args)
来源：http://gq.shxzskj.cn

Go:   func main()
来源：http://pr.shtwfgs.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ui.9csxet.cn

C#:   static void Main(string[] args)
来源：http://of.shxzukj.cn

[M08] 获取系统与运行时信息
来源：http://kr.panjiajie.cn

Py:   platform.system();  platform.python_version()
来源：http://oy.shxzukj.cn

PHP:  PHP_OS;  phpversion();
来源：http://pm.muxihuayi.cn

JS:   process.platform;  process.version
来源：http://fw.hahajie.cn

TS:   process.platform;  process.version
来源：http://ua.szxytkj.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hm.bookmarksfly.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://zj.9csxet.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://uj.yuntaijiaju.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://sn.haigaiapp.cn

================================================================================
来源：http://tw.wgjwhj.cn

N. 数据结构与算法
来源：http://za.bookmarksfly.cn

================================================================================
来源：http://qg.hnjuh.cn

[N01] 二分查找（有序数组）
来源：http://vp.shtwfgs.cn

Py:   bisect.bisect_left(arr, x)
来源：http://ep.colortex.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mm.shxzukj.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://pp.lnxyls.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ac.lnxyls.cn

Java: Arrays.binarySearch(arr, x)
来源：http://rc.asd995.cn

Go:   sort.SearchInts(arr, x)
来源：http://sp.521024.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://ji.hahajie.cn

C#:   Array.BinarySearch(arr, x)
来源：http://hg.9csxet.cn

[N02] 排序（工程实践用内置实现）
来源：http://bm.chemitech.net.cn

Py:   sorted(arr);  arr.sort()
来源：http://hr.chemitech.net.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://pk.shtwfgs.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://pc.szsharing.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://jt.lnxyls.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://sp.shtwfgs.cn

Go:   slices.Sort(arr)
来源：http://ur.nszjky.cn

Ruby: arr.sort
来源：http://ca.521024.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://ue.bjjhwx.cn

[N03] 快速排序（分治示例）
来源：http://ju.gzmigu.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://is.szsharing.cn

PHP:  // 递归实现，或用 usort
来源：http://mp.shxzskj.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://oa.shtwfgs.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ut.jctech888.com.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://el.shxzukj.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://rb.hnjuh.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wg.bookmarksfly.cn

C#:   // 手写递归，或 Array.Sort
来源：http://xq.wgjwhj.cn

[N04] 斐波那契数列
来源：http://qv.chemitech.net.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://oz.shxzskj.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://rx.9csxet.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://gx.nszjky.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://pn.huixinmuqiang.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wc.szxytkj.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://pj.hnjuh.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://nt.huixiangedu.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://vu.haigaiapp.cn

[N05] 最大公约数
来源：http://wg.newstarts.cn

Py:   math.gcd(a, b)
来源：http://po.shxzskj.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ym.jctech888.com.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://dy.szsharing.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hu.huixiangedu.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://xk.wgjwhj.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://qh.bookmarksfly.cn

Ruby: a.gcd(b)
来源：http://kt.shxzukj.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://aw.nszjky.cn

[N06] 判断回文字符串
来源：http://dv.huixiangedu.cn

Py:   s == s[::-1]
来源：http://jh.shxzskj.cn

PHP:  $s === strrev($s);
来源：http://zo.9csxet.cn

JS:   s === [...s].reverse().join("")
来源：http://pg.colortex.cn

TS:   s === [...s].reverse().join("")
来源：http://gr.nszjky.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://aw.shxzukj.cn

Go:   // 双指针从两端比较
来源：http://od.yuntaijiaju.cn

Ruby: s == s.reverse
来源：http://ur.shxzskj.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://xs.panjiajie.cn

[N07] 两数之和（返回下标）
来源：http://lu.jctech888.com.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://sd.szxytkj.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://cz.huixinmuqiang.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://ee.szsharing.cn

TS:   // 手写 Map<string, number>
来源：http://ly.jctech888.com.cn

Java: // 手写 HashMap
来源：http://we.muxihuayi.cn

Go:   // 手写 map[int]int
来源：http://vm.asd995.cn

Ruby: // 手写 Hash
来源：http://tm.lnxyls.cn

C#:   // 手写 Dictionary<int, int>
来源：http://ah.chemitech.net.cn

[N08] 生成全排列
来源：http://wu.nszjky.cn

Py:   itertools.permutations(arr)
来源：http://xf.huixiangedu.cn

PHP:  // 手写递归交换
来源：http://nj.huixinmuqiang.cn

JS:   // 手写回溯递归
来源：http://eo.jctech888.com.cn

TS:   // 手写回溯递归
来源：http://gx.hnjuh.cn

Java: // 手写回溯递归
来源：http://tv.gzmigu.cn

Go:   // 手写回溯递归
来源：http://ao.nicolike.cn

Ruby: arr.permutation.to_a
来源：http://nr.huixinmuqiang.cn

C#:   // 手写回溯递归
来源：http://sp.lnxyls.cn

[N09] 栈与队列
来源：http://aa.jianghongdianzi.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://le.huixiangedu.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wo.bjjhwx.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://tf.yuexingan06.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ub.szsharing.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://kg.haigaiapp.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://rn.asd995.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://yq.huanxung.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://oa.lnxyls.cn

[N10] 链表节点定义
来源：http://lu.nszjky.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://fi.nszjky.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://jt.lnxyls.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://xw.521024.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://xc.bjjhwx.cn

Java: class Node { int v; Node next; }
来源：http://xf.wgjwhj.cn

Go:   type Node struct { V int; Next *Node }
来源：http://ov.huixinmuqiang.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://nw.newstarts.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://bc.shtwfgs.cn

[N11] 二叉树中序遍历
来源：http://jr.szsharing.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://jk.jianghongdianzi.cn

PHP:  // 手写递归函数
来源：http://eq.newstarts.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://nj.haigaiapp.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://yd.9csxet.cn

Java: // 手写递归
来源：http://vk.yuexingan06.cn

Go:   // 手写递归
来源：http://ik.colortex.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://pq.shxzskj.cn

C#:   // 手写递归
来源：http://cm.huixinmuqiang.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ol.nszjky.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://by.nszjky.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://li.huixinmuqiang.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://jo.szxytkj.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://qj.shxzskj.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://bz.huanxung.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wa.muxihuayi.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://av.huanxung.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://qo.yuexingan06.cn

================================================================================
来源：http://br.shxzskj.cn

O. 并发与异步
来源：http://ae.lnxyls.cn

================================================================================
来源：http://hz.panjiajie.cn

[O01] 启动一个线程
来源：http://dl.shxzskj.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://nc.shxzukj.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://rm.gzmigu.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mu.shtwfgs.cn

TS:   // 同 JS
来源：http://jb.lnxyls.cn

Java: new Thread(() -> f()).start()
来源：http://ep.muxihuayi.cn

Go:   go f()
来源：http://jo.521024.cn

Ruby: Thread.new { f }
来源：http://tw.chemitech.net.cn

C#:   Task.Run(() => F());
来源：http://ir.muxihuayi.cn

[O02] 使用线程池
来源：http://cm.521024.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://db.newstarts.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://oa.huixinmuqiang.cn

JS:   // worker_threads 线程池
来源：http://dd.jianghongdianzi.cn

TS:   // worker_threads 线程池
来源：http://la.szxytkj.cn

Java: Executors.newFixedThreadPool(4)
来源：http://ew.szxytkj.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ls.jianghongdianzi.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ii.szsharing.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://pf.nicolike.cn

[O03] 加锁保护共享数据
来源：http://mr.asd995.cn

Py:   with lock: shared += 1
来源：http://px.521024.cn

PHP:  // 用 flock() 做文件锁
来源：http://ed.nicolike.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ky.yuexingan06.cn

TS:   // 同 JS
来源：http://pa.yuexingan06.cn

Java: synchronized (this) { shared++; }
来源：http://wm.bookmarksfly.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://uk.colortex.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://ou.nicolike.cn

C#:   lock (gate) { shared++; }
来源：http://lm.colortex.cn

[O04] 定义异步函数并等待
来源：http://bf.wgjwhj.cn

Py:   async def f():⏎    await g()
来源：http://tn.colortex.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://rb.panjiajie.cn

JS:   async function f() { await g(); }
来源：http://ql.bjjhwx.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://sq.panjiajie.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://cz.nszjky.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://jw.huanxung.cn

Ruby: # 用 Fiber 或 async gem
来源：http://ao.szsharing.cn

C#:   async Task F() { await G(); }
来源：http://fx.bjjhwx.cn

[O05] 并发执行并等待全部完成
来源：http://az.shtwfgs.cn

Py:   asyncio.gather(*tasks)
来源：http://ts.haigaiapp.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://vs.yuexingan06.cn

JS:   await Promise.all(tasks)
来源：http://ly.bookmarksfly.cn

TS:   await Promise.all(tasks)
来源：http://lp.newstarts.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ue.jctech888.com.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://qd.colortex.cn

Ruby: threads.map(&:join)
来源：http://ht.newstarts.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://wl.szsharing.cn

[O06] 使用进程池
来源：http://ep.wgjwhj.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wx.panjiajie.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://qm.huanxung.cn

JS:   // child_process / cluster 模块
来源：http://nx.panjiajie.cn

TS:   // child_process / cluster 模块
来源：http://kg.chemitech.net.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://tw.bookmarksfly.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ws.muxihuayi.cn

Ruby: // fork 块
来源：http://zp.yuntaijiaju.cn

C#:   Parallel.For
来源：http://fo.szxytkj.cn

================================================================================
来源：http://ia.nszjky.cn

P. 常用工具函数
来源：http://qi.shxzskj.cn

================================================================================
来源：http://et.szxytkj.cn

[P01] 生成 UUID
来源：http://wj.nicolike.cn

Py:   str(uuid.uuid4())
来源：http://bz.jianghongdianzi.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://fp.nicolike.cn

JS:   crypto.randomUUID()
来源：http://sp.bookmarksfly.cn

TS:   crypto.randomUUID()
来源：http://hh.hnjuh.cn

Java: UUID.randomUUID().toString()
来源：http://fy.wgjwhj.cn

Go:   // 用 github.com/google/uuid
来源：http://wt.lnxyls.cn

Ruby: SecureRandom.uuid
来源：http://lu.jianghongdianzi.cn

C#:   Guid.NewGuid().ToString()
来源：http://bl.asd995.cn

[P02] MD5 / SHA256 摘要
来源：http://oh.asd995.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://fe.panjiajie.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://za.yuexingan06.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hf.huixiangedu.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ml.nszjky.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://oq.hnjuh.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://vw.shxzukj.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://le.jctech888.com.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://sh.shxzskj.cn

[P03] 生成短随机字符串
来源：http://up.muxihuayi.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wj.nszjky.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://pj.jianghongdianzi.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ff.muxihuayi.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wa.shxzskj.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://yz.hnjuh.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://pz.9csxet.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://iz.panjiajie.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://oq.hnjuh.cn

[P04] 求长度
来源：http://mp.shtwfgs.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://qf.asd995.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://jl.gzmigu.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://fz.colortex.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://iq.lnxyls.cn

Java: list.size();  map.size();  s.length()
来源：http://ol.yuntaijiaju.cn

Go:   len(arr);  len(m)
来源：http://qv.muxihuayi.cn

Ruby: x.length;  x.size
来源：http://zp.szsharing.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://xo.lnxyls.cn

[P05] 判断两个对象内容是否相等
来源：http://zq.shxzskj.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://kb.wgjwhj.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://nc.szsharing.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hk.colortex.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://lo.hnjuh.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://dr.yuntaijiaju.cn

Go:   reflect.DeepEqual(a, b)
来源：http://tf.521024.cn

Ruby: a == b
来源：http://nz.haigaiapp.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://pw.yuntaijiaju.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hm.haigaiapp.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://df.shxzskj.cn

PHP:  if (empty($x)) {}
来源：http://de.yuntaijiaju.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://zc.huanxung.cn

TS:   if (x == null) {}
来源：http://pn.nicolike.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://sq.nszjky.cn

Go:   if x == nil {}
来源：http://fw.gzmigu.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://gv.nicolike.cn

C#:   if (x is null) {}
来源：http://vq.szsharing.cn

[P07] 防抖与节流
来源：http://yx.jianghongdianzi.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ig.9csxet.cn

PHP:  // 手写时间戳比较
来源：http://ts.hnjuh.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://zi.yuntaijiaju.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://sv.huixinmuqiang.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://uj.nicolike.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ad.colortex.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://rf.newstarts.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://et.shxzukj.cn

[P08] 处理浮点精度问题
来源：http://zv.shtwfgs.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://du.hahajie.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://lr.jianghongdianzi.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://qd.bookmarksfly.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://qv.jianghongdianzi.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://cb.hnjuh.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://un.hnjuh.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://am.haigaiapp.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ql.huanxung.cn

================================================================================
来源：http://tr.yuexingan06.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://fw.shtwfgs.cn

================================================================================
来源：http://mu.muxihuayi.cn

[Q01] 创建表
来源：http://px.shxzukj.cn

CREATE TABLE users (
来源：http://pl.521024.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://me.yuexingan06.cn

name VARCHAR(50) NOT NULL,
来源：http://uf.chemitech.net.cn

email VARCHAR(100) UNIQUE,
来源：http://kt.chemitech.net.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://tt.jctech888.com.cn

);
来源：http://vj.szxytkj.cn

[Q02] 创建带外键的表
来源：http://xc.shtwfgs.cn

CREATE TABLE orders (
来源：http://ti.yuexingan06.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://an.lnxyls.cn

user_id INT NOT NULL,
来源：http://hu.newstarts.cn

amount DECIMAL(10, 2),
来源：http://uw.yuexingan06.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://od.bjjhwx.cn

);
来源：http://wn.gzmigu.cn

[Q03] 增加列
来源：http://ys.huixinmuqiang.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://sk.chemitech.net.cn

[Q04] 修改列类型
来源：http://ai.shxzukj.cn


<!-- 参考信息 -->