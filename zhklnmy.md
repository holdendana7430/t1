代发 wailian999

PHP:  fwrite(STDERR, "err\n");
来源：http://ia.hahajie.cn

JS:   console.error("err")
来源：http://qy.szxytkj.cn

TS:   console.error("err")
来源：http://rl.szsharing.cn

Java: System.err.println("err")
来源：http://ec.hnjuh.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://jx.chemitech.net.cn

Ruby: warn "err"
来源：http://og.hahajie.cn

C#:   Console.Error.WriteLine("err")
来源：http://pa.9csxet.cn

[M07] 判断是否为主入口
来源：http://ou.szxytkj.cn

Py:   if __name__ == "__main__":
来源：http://wj.huanxung.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://gk.asd995.cn

JS:   require.main === module
来源：http://kb.bookmarksfly.cn

TS:   require.main === module
来源：http://zc.wgjwhj.cn

Java: public static void main(String[] args)
来源：http://ai.huixiangedu.cn

Go:   func main()
来源：http://eu.huixinmuqiang.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hb.hahajie.cn

C#:   static void Main(string[] args)
来源：http://fa.jianghongdianzi.cn

[M08] 获取系统与运行时信息
来源：http://jt.colortex.cn

Py:   platform.system();  platform.python_version()
来源：http://ug.huixinmuqiang.cn

PHP:  PHP_OS;  phpversion();
来源：http://rf.9csxet.cn

JS:   process.platform;  process.version
来源：http://vi.asd995.cn

TS:   process.platform;  process.version
来源：http://bv.huixinmuqiang.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://gu.shtwfgs.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://ad.huanxung.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://nu.chemitech.net.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://yy.nicolike.cn

================================================================================
来源：http://mf.yuexingan06.cn

N. 数据结构与算法
来源：http://dd.nszjky.cn

================================================================================
来源：http://un.szsharing.cn

[N01] 二分查找（有序数组）
来源：http://bw.szsharing.cn

Py:   bisect.bisect_left(arr, x)
来源：http://ou.szxytkj.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://pn.bjjhwx.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ev.shxzukj.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://yo.shxzukj.cn

Java: Arrays.binarySearch(arr, x)
来源：http://hu.yuntaijiaju.cn

Go:   sort.SearchInts(arr, x)
来源：http://od.huixinmuqiang.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://qw.panjiajie.cn

C#:   Array.BinarySearch(arr, x)
来源：http://vn.colortex.cn

[N02] 排序（工程实践用内置实现）
来源：http://ft.shxzukj.cn

Py:   sorted(arr);  arr.sort()
来源：http://gq.nicolike.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://xm.9csxet.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://oh.huanxung.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://wo.yuexingan06.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://bt.shxzskj.cn

Go:   slices.Sort(arr)
来源：http://ak.bookmarksfly.cn

Ruby: arr.sort
来源：http://ot.shxzskj.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://vd.yuntaijiaju.cn

[N03] 快速排序（分治示例）
来源：http://oj.9csxet.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://bj.szxytkj.cn

PHP:  // 递归实现，或用 usort
来源：http://zn.hahajie.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://cq.szsharing.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://pn.yuexingan06.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://qi.jctech888.com.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://nk.shtwfgs.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://yj.bookmarksfly.cn

C#:   // 手写递归，或 Array.Sort
来源：http://wk.hahajie.cn

[N04] 斐波那契数列
来源：http://al.9csxet.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ou.haigaiapp.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://vy.huanxung.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://cr.shtwfgs.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mq.shxzukj.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://an.lnxyls.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://yo.huixiangedu.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://bg.szsharing.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hp.shxzukj.cn

[N05] 最大公约数
来源：http://db.gzmigu.cn

Py:   math.gcd(a, b)
来源：http://fi.shxzskj.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mg.huixiangedu.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://uf.newstarts.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://fp.gzmigu.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://zx.haigaiapp.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ws.haigaiapp.cn

Ruby: a.gcd(b)
来源：http://sm.gzmigu.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://aj.jctech888.com.cn

[N06] 判断回文字符串
来源：http://go.panjiajie.cn

Py:   s == s[::-1]
来源：http://lu.newstarts.cn

PHP:  $s === strrev($s);
来源：http://xk.asd995.cn

JS:   s === [...s].reverse().join("")
来源：http://rb.yuexingan06.cn

TS:   s === [...s].reverse().join("")
来源：http://ej.nszjky.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://km.nszjky.cn

Go:   // 双指针从两端比较
来源：http://ig.huixiangedu.cn

Ruby: s == s.reverse
来源：http://ca.bookmarksfly.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://kj.lnxyls.cn

[N07] 两数之和（返回下标）
来源：http://wp.haigaiapp.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://rb.9csxet.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mb.huixinmuqiang.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://cn.bookmarksfly.cn

TS:   // 手写 Map<string, number>
来源：http://en.bjjhwx.cn

Java: // 手写 HashMap
来源：http://qb.huixiangedu.cn

Go:   // 手写 map[int]int
来源：http://bn.chemitech.net.cn

Ruby: // 手写 Hash
来源：http://kj.newstarts.cn

C#:   // 手写 Dictionary<int, int>
来源：http://nw.huanxung.cn

[N08] 生成全排列
来源：http://va.bookmarksfly.cn

Py:   itertools.permutations(arr)
来源：http://yy.gzmigu.cn

PHP:  // 手写递归交换
来源：http://ci.asd995.cn

JS:   // 手写回溯递归
来源：http://le.shxzskj.cn

TS:   // 手写回溯递归
来源：http://cl.shxzskj.cn

Java: // 手写回溯递归
来源：http://ip.wgjwhj.cn

Go:   // 手写回溯递归
来源：http://vu.szxytkj.cn

Ruby: arr.permutation.to_a
来源：http://ic.yuexingan06.cn

C#:   // 手写回溯递归
来源：http://ko.huixiangedu.cn

[N09] 栈与队列
来源：http://dv.asd995.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ut.bookmarksfly.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://cr.yuntaijiaju.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wv.lnxyls.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://yg.szxytkj.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ue.shxzukj.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://et.nicolike.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://cv.szsharing.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ag.asd995.cn

[N10] 链表节点定义
来源：http://nm.nszjky.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://fo.shxzukj.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://lb.panjiajie.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://cj.yuntaijiaju.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ia.9csxet.cn

Java: class Node { int v; Node next; }
来源：http://ha.lnxyls.cn

Go:   type Node struct { V int; Next *Node }
来源：http://ur.huixiangedu.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://jj.shxzskj.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://wf.jianghongdianzi.cn

[N11] 二叉树中序遍历
来源：http://kb.nszjky.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://lt.lnxyls.cn

PHP:  // 手写递归函数
来源：http://sx.gzmigu.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://nh.521024.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://kl.huanxung.cn

Java: // 手写递归
来源：http://id.panjiajie.cn

Go:   // 手写递归
来源：http://cm.haigaiapp.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://lt.gzmigu.cn

C#:   // 手写递归
来源：http://cu.chemitech.net.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ll.chemitech.net.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ir.muxihuayi.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://kb.jianghongdianzi.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://aq.521024.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://tx.haigaiapp.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://kf.yuntaijiaju.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://fr.haigaiapp.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://xf.newstarts.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://dr.jctech888.com.cn

================================================================================
来源：http://wu.hahajie.cn

O. 并发与异步
来源：http://wh.jctech888.com.cn

================================================================================
来源：http://rz.hahajie.cn

[O01] 启动一个线程
来源：http://fj.shxzskj.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ym.jianghongdianzi.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hk.haigaiapp.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ms.newstarts.cn

TS:   // 同 JS
来源：http://vt.lnxyls.cn

Java: new Thread(() -> f()).start()
来源：http://ga.gzmigu.cn

Go:   go f()
来源：http://zm.chemitech.net.cn

Ruby: Thread.new { f }
来源：http://lw.chemitech.net.cn

C#:   Task.Run(() => F());
来源：http://vg.newstarts.cn

[O02] 使用线程池
来源：http://an.huanxung.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://sc.nszjky.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ht.bjjhwx.cn

JS:   // worker_threads 线程池
来源：http://ff.panjiajie.cn

TS:   // worker_threads 线程池
来源：http://xw.newstarts.cn

Java: Executors.newFixedThreadPool(4)
来源：http://fc.gzmigu.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wx.bjjhwx.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mc.haigaiapp.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://yk.jctech888.com.cn

[O03] 加锁保护共享数据
来源：http://tk.shxzukj.cn

Py:   with lock: shared += 1
来源：http://vd.huixinmuqiang.cn

PHP:  // 用 flock() 做文件锁
来源：http://ra.9csxet.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://pm.hahajie.cn

TS:   // 同 JS
来源：http://ra.colortex.cn

Java: synchronized (this) { shared++; }
来源：http://eo.521024.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://jv.jctech888.com.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://il.hnjuh.cn

C#:   lock (gate) { shared++; }
来源：http://hu.9csxet.cn

[O04] 定义异步函数并等待
来源：http://hb.panjiajie.cn

Py:   async def f():⏎    await g()
来源：http://pi.lnxyls.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://re.shxzukj.cn

JS:   async function f() { await g(); }
来源：http://wk.bookmarksfly.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://mz.colortex.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://at.colortex.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://dc.bjjhwx.cn

Ruby: # 用 Fiber 或 async gem
来源：http://ln.szsharing.cn

C#:   async Task F() { await G(); }
来源：http://vq.lnxyls.cn

[O05] 并发执行并等待全部完成
来源：http://ko.jctech888.com.cn

Py:   asyncio.gather(*tasks)
来源：http://np.huixiangedu.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://np.huanxung.cn

JS:   await Promise.all(tasks)
来源：http://pj.nszjky.cn

TS:   await Promise.all(tasks)
来源：http://dy.hahajie.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://dm.muxihuayi.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://dz.huixinmuqiang.cn

Ruby: threads.map(&:join)
来源：http://uq.wgjwhj.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://zx.chemitech.net.cn

[O06] 使用进程池
来源：http://tn.colortex.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://id.szsharing.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://ix.shxzukj.cn

JS:   // child_process / cluster 模块
来源：http://mb.gzmigu.cn

TS:   // child_process / cluster 模块
来源：http://wh.newstarts.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://nl.huixiangedu.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://dh.gzmigu.cn

Ruby: // fork 块
来源：http://pg.9csxet.cn

C#:   Parallel.For
来源：http://iv.panjiajie.cn

================================================================================
来源：http://jp.yuntaijiaju.cn

P. 常用工具函数
来源：http://vp.bjjhwx.cn

================================================================================
来源：http://ly.newstarts.cn

[P01] 生成 UUID
来源：http://do.hahajie.cn

Py:   str(uuid.uuid4())
来源：http://ur.chemitech.net.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://rn.newstarts.cn

JS:   crypto.randomUUID()
来源：http://yv.lnxyls.cn

TS:   crypto.randomUUID()
来源：http://xp.haigaiapp.cn

Java: UUID.randomUUID().toString()
来源：http://mc.colortex.cn

Go:   // 用 github.com/google/uuid
来源：http://uj.szsharing.cn

Ruby: SecureRandom.uuid
来源：http://so.hnjuh.cn

C#:   Guid.NewGuid().ToString()
来源：http://au.9csxet.cn

[P02] MD5 / SHA256 摘要
来源：http://ki.huixinmuqiang.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://rp.haigaiapp.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://oa.asd995.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ca.colortex.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://fg.shxzskj.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ak.szsharing.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ti.wgjwhj.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://cw.9csxet.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://bt.haigaiapp.cn

[P03] 生成短随机字符串
来源：http://km.huixiangedu.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ff.jianghongdianzi.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://xe.hahajie.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://cd.panjiajie.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ic.nszjky.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://xy.lnxyls.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ej.bjjhwx.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://cd.jianghongdianzi.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wt.gzmigu.cn

[P04] 求长度
来源：http://nv.huixinmuqiang.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://eb.yuntaijiaju.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://yx.huanxung.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://xp.huanxung.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://bh.huanxung.cn

Java: list.size();  map.size();  s.length()
来源：http://ge.nszjky.cn

Go:   len(arr);  len(m)
来源：http://qz.colortex.cn

Ruby: x.length;  x.size
来源：http://ak.shxzskj.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://dz.gzmigu.cn

[P05] 判断两个对象内容是否相等
来源：http://tw.bookmarksfly.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://ew.shtwfgs.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://se.bookmarksfly.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wy.nszjky.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ug.hnjuh.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ac.colortex.cn

Go:   reflect.DeepEqual(a, b)
来源：http://tg.newstarts.cn

Ruby: a == b
来源：http://pr.yuexingan06.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://bc.wgjwhj.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ly.asd995.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://cl.yuntaijiaju.cn

PHP:  if (empty($x)) {}
来源：http://bf.jctech888.com.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://on.newstarts.cn

TS:   if (x == null) {}
来源：http://ej.bjjhwx.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://lk.colortex.cn

Go:   if x == nil {}
来源：http://zq.hahajie.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://uk.yuexingan06.cn

C#:   if (x is null) {}
来源：http://ny.wgjwhj.cn

[P07] 防抖与节流
来源：http://qm.9csxet.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ht.muxihuayi.cn

PHP:  // 手写时间戳比较
来源：http://lo.asd995.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ge.haigaiapp.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ym.newstarts.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mp.yuexingan06.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://zj.bjjhwx.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://oi.wgjwhj.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://rl.521024.cn

[P08] 处理浮点精度问题
来源：http://nz.yuntaijiaju.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://zu.nszjky.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://nx.huanxung.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ml.hahajie.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://by.huanxung.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://le.panjiajie.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://fd.jctech888.com.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ig.521024.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://tk.colortex.cn

================================================================================
来源：http://lk.asd995.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://dn.wgjwhj.cn

================================================================================
来源：http://nz.szsharing.cn

[Q01] 创建表
来源：http://ga.hnjuh.cn

CREATE TABLE users (
来源：http://yh.chemitech.net.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://xx.shxzskj.cn

name VARCHAR(50) NOT NULL,
来源：http://rb.yuexingan06.cn

email VARCHAR(100) UNIQUE,
来源：http://yf.huixinmuqiang.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://pv.9csxet.cn

);
来源：http://xh.yuexingan06.cn

[Q02] 创建带外键的表
来源：http://qj.newstarts.cn

CREATE TABLE orders (
来源：http://yg.wgjwhj.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ej.gzmigu.cn

user_id INT NOT NULL,
来源：http://ml.jctech888.com.cn

amount DECIMAL(10, 2),
来源：http://qj.shxzskj.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://uy.huixinmuqiang.cn

);
来源：http://jc.lnxyls.cn

[Q03] 增加列
来源：http://fo.shtwfgs.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://pb.nszjky.cn

[Q04] 修改列类型
来源：http://zm.nszjky.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://kv.shxzukj.cn

[Q05] 重命名列
来源：http://la.9csxet.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://az.hnjuh.cn

[Q06] 删除列
来源：http://ek.wgjwhj.cn

ALTER TABLE users DROP COLUMN age;
来源：http://fz.newstarts.cn

[Q07] 删除表
来源：http://ut.huixinmuqiang.cn

DROP TABLE IF EXISTS orders;
来源：http://qf.bookmarksfly.cn

[Q08] 创建普通索引
来源：http://nn.bookmarksfly.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://il.haigaiapp.cn

[Q09] 创建唯一索引
来源：http://rq.jianghongdianzi.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://cl.haigaiapp.cn

[Q10] 插入单行
来源：http://bp.bjjhwx.cn


<!-- 参考信息 -->