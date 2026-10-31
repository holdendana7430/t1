代发 wailian999

PHP:  fwrite(STDERR, "err\n");
来源：http://wb.hnjuh.cn

JS:   console.error("err")
来源：http://qe.colortex.cn

TS:   console.error("err")
来源：http://er.9csxet.cn

Java: System.err.println("err")
来源：http://ue.hnjuh.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://tl.yuexingan06.cn

Ruby: warn "err"
来源：http://nc.shxzskj.cn

C#:   Console.Error.WriteLine("err")
来源：http://iz.yuexingan06.cn

[M07] 判断是否为主入口
来源：http://cd.nszjky.cn

Py:   if __name__ == "__main__":
来源：http://qs.huixiangedu.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://en.jianghongdianzi.cn

JS:   require.main === module
来源：http://we.colortex.cn

TS:   require.main === module
来源：http://qb.nicolike.cn

Java: public static void main(String[] args)
来源：http://zp.yuexingan06.cn

Go:   func main()
来源：http://fz.jctech888.com.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://py.huixinmuqiang.cn

C#:   static void Main(string[] args)
来源：http://dc.shtwfgs.cn

[M08] 获取系统与运行时信息
来源：http://wi.nszjky.cn

Py:   platform.system();  platform.python_version()
来源：http://sy.gzmigu.cn

PHP:  PHP_OS;  phpversion();
来源：http://lk.9csxet.cn

JS:   process.platform;  process.version
来源：http://jo.hnjuh.cn

TS:   process.platform;  process.version
来源：http://ea.hahajie.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://xy.hnjuh.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://zh.chemitech.net.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://zq.asd995.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://iy.szsharing.cn

================================================================================
来源：http://sz.szsharing.cn

N. 数据结构与算法
来源：http://cv.panjiajie.cn

================================================================================
来源：http://df.muxihuayi.cn

[N01] 二分查找（有序数组）
来源：http://ta.nszjky.cn

Py:   bisect.bisect_left(arr, x)
来源：http://mk.muxihuayi.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ai.bookmarksfly.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://dy.lnxyls.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://gc.jctech888.com.cn

Java: Arrays.binarySearch(arr, x)
来源：http://ty.yuntaijiaju.cn

Go:   sort.SearchInts(arr, x)
来源：http://os.shxzukj.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://vv.shxzskj.cn

C#:   Array.BinarySearch(arr, x)
来源：http://cw.shtwfgs.cn

[N02] 排序（工程实践用内置实现）
来源：http://xa.szsharing.cn

Py:   sorted(arr);  arr.sort()
来源：http://lt.bjjhwx.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://xm.shxzskj.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://uh.9csxet.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://fg.huixinmuqiang.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://zz.colortex.cn

Go:   slices.Sort(arr)
来源：http://cr.shxzukj.cn

Ruby: arr.sort
来源：http://ty.gzmigu.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://le.chemitech.net.cn

[N03] 快速排序（分治示例）
来源：http://jg.shxzukj.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ix.521024.cn

PHP:  // 递归实现，或用 usort
来源：http://la.szsharing.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://qu.jianghongdianzi.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mt.bookmarksfly.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://xp.panjiajie.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://bm.jianghongdianzi.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://us.yuexingan06.cn

C#:   // 手写递归，或 Array.Sort
来源：http://wr.bookmarksfly.cn

[N04] 斐波那契数列
来源：http://bk.haigaiapp.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://di.huanxung.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://tq.521024.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://bf.jctech888.com.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://qw.lnxyls.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://pk.chemitech.net.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mf.shxzukj.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://qf.lnxyls.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://tf.shxzukj.cn

[N05] 最大公约数
来源：http://tg.bjjhwx.cn

Py:   math.gcd(a, b)
来源：http://mw.szsharing.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://oz.jianghongdianzi.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://el.newstarts.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://te.shxzskj.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://qd.szsharing.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://tn.yuexingan06.cn

Ruby: a.gcd(b)
来源：http://tu.szxytkj.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ah.jctech888.com.cn

[N06] 判断回文字符串
来源：http://na.521024.cn

Py:   s == s[::-1]
来源：http://bz.shxzukj.cn

PHP:  $s === strrev($s);
来源：http://xv.9csxet.cn

JS:   s === [...s].reverse().join("")
来源：http://rm.521024.cn

TS:   s === [...s].reverse().join("")
来源：http://vq.asd995.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ed.yuexingan06.cn

Go:   // 双指针从两端比较
来源：http://uq.jianghongdianzi.cn

Ruby: s == s.reverse
来源：http://ha.521024.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://wb.nicolike.cn

[N07] 两数之和（返回下标）
来源：http://ro.hnjuh.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://xe.shxzukj.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://kb.521024.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://vl.jianghongdianzi.cn

TS:   // 手写 Map<string, number>
来源：http://to.huixinmuqiang.cn

Java: // 手写 HashMap
来源：http://wu.9csxet.cn

Go:   // 手写 map[int]int
来源：http://vx.huixiangedu.cn

Ruby: // 手写 Hash
来源：http://co.jctech888.com.cn

C#:   // 手写 Dictionary<int, int>
来源：http://ui.huixiangedu.cn

[N08] 生成全排列
来源：http://cs.521024.cn

Py:   itertools.permutations(arr)
来源：http://zk.huanxung.cn

PHP:  // 手写递归交换
来源：http://br.yuntaijiaju.cn

JS:   // 手写回溯递归
来源：http://zn.shxzukj.cn

TS:   // 手写回溯递归
来源：http://dh.yuntaijiaju.cn

Java: // 手写回溯递归
来源：http://ty.lnxyls.cn

Go:   // 手写回溯递归
来源：http://ws.521024.cn

Ruby: arr.permutation.to_a
来源：http://jj.newstarts.cn

C#:   // 手写回溯递归
来源：http://kk.yuexingan06.cn

[N09] 栈与队列
来源：http://bp.shxzukj.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://dk.nszjky.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://vn.shtwfgs.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://as.huanxung.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ad.szsharing.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://je.gzmigu.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://pa.jctech888.com.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://fx.hnjuh.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://bb.huanxung.cn

[N10] 链表节点定义
来源：http://ur.bookmarksfly.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ov.szxytkj.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://rz.huanxung.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://tx.bjjhwx.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ig.szsharing.cn

Java: class Node { int v; Node next; }
来源：http://jj.asd995.cn

Go:   type Node struct { V int; Next *Node }
来源：http://ri.jianghongdianzi.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://mn.jianghongdianzi.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://hm.yuntaijiaju.cn

[N11] 二叉树中序遍历
来源：http://jo.yuntaijiaju.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ai.wgjwhj.cn

PHP:  // 手写递归函数
来源：http://gw.yuexingan06.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://eb.jianghongdianzi.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://yb.lnxyls.cn

Java: // 手写递归
来源：http://yh.shxzskj.cn

Go:   // 手写递归
来源：http://vi.shtwfgs.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://uk.bookmarksfly.cn

C#:   // 手写递归
来源：http://wg.asd995.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ua.jctech888.com.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://pn.hahajie.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ep.jianghongdianzi.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hu.asd995.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mc.lnxyls.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ol.colortex.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hh.newstarts.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://qe.panjiajie.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mq.haigaiapp.cn

================================================================================
来源：http://fz.huixiangedu.cn

O. 并发与异步
来源：http://ze.yuexingan06.cn

================================================================================
来源：http://eg.jctech888.com.cn

[O01] 启动一个线程
来源：http://av.newstarts.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://jp.nszjky.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ej.huixiangedu.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://lk.lnxyls.cn

TS:   // 同 JS
来源：http://wx.jianghongdianzi.cn

Java: new Thread(() -> f()).start()
来源：http://pg.chemitech.net.cn

Go:   go f()
来源：http://we.nicolike.cn

Ruby: Thread.new { f }
来源：http://tl.panjiajie.cn

C#:   Task.Run(() => F());
来源：http://hc.shtwfgs.cn

[O02] 使用线程池
来源：http://qg.hahajie.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://bf.panjiajie.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://vk.shxzskj.cn

JS:   // worker_threads 线程池
来源：http://ul.szsharing.cn

TS:   // worker_threads 线程池
来源：http://yx.yuntaijiaju.cn

Java: Executors.newFixedThreadPool(4)
来源：http://uo.huanxung.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://zl.szsharing.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ax.muxihuayi.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hm.haigaiapp.cn

[O03] 加锁保护共享数据
来源：http://qy.yuntaijiaju.cn

Py:   with lock: shared += 1
来源：http://kr.shxzskj.cn

PHP:  // 用 flock() 做文件锁
来源：http://hb.bjjhwx.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://tv.shxzskj.cn

TS:   // 同 JS
来源：http://hn.nicolike.cn

Java: synchronized (this) { shared++; }
来源：http://bx.hahajie.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://eh.panjiajie.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://wt.bookmarksfly.cn

C#:   lock (gate) { shared++; }
来源：http://kl.jianghongdianzi.cn

[O04] 定义异步函数并等待
来源：http://jz.nszjky.cn

Py:   async def f():⏎    await g()
来源：http://pu.nszjky.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://qs.lnxyls.cn

JS:   async function f() { await g(); }
来源：http://my.haigaiapp.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://ma.haigaiapp.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://cq.nszjky.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://xr.colortex.cn

Ruby: # 用 Fiber 或 async gem
来源：http://gi.shxzskj.cn

C#:   async Task F() { await G(); }
来源：http://el.lnxyls.cn

[O05] 并发执行并等待全部完成
来源：http://rc.hnjuh.cn

Py:   asyncio.gather(*tasks)
来源：http://am.9csxet.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://vx.asd995.cn

JS:   await Promise.all(tasks)
来源：http://cf.521024.cn

TS:   await Promise.all(tasks)
来源：http://bp.szxytkj.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://do.gzmigu.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://uy.colortex.cn

Ruby: threads.map(&:join)
来源：http://ed.nszjky.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://hf.huanxung.cn

[O06] 使用进程池
来源：http://nx.9csxet.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://lu.shxzukj.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://qe.wgjwhj.cn

JS:   // child_process / cluster 模块
来源：http://ae.jctech888.com.cn

TS:   // child_process / cluster 模块
来源：http://rl.hahajie.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://re.jctech888.com.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://sx.gzmigu.cn

Ruby: // fork 块
来源：http://jb.9csxet.cn

C#:   Parallel.For
来源：http://dv.huixinmuqiang.cn

================================================================================
来源：http://vr.huixinmuqiang.cn

P. 常用工具函数
来源：http://ny.newstarts.cn

================================================================================
来源：http://jr.hahajie.cn

[P01] 生成 UUID
来源：http://mj.newstarts.cn

Py:   str(uuid.uuid4())
来源：http://au.szsharing.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://xj.jianghongdianzi.cn

JS:   crypto.randomUUID()
来源：http://sh.shxzukj.cn

TS:   crypto.randomUUID()
来源：http://vc.yuntaijiaju.cn

Java: UUID.randomUUID().toString()
来源：http://cb.lnxyls.cn

Go:   // 用 github.com/google/uuid
来源：http://gi.colortex.cn

Ruby: SecureRandom.uuid
来源：http://am.jianghongdianzi.cn

C#:   Guid.NewGuid().ToString()
来源：http://gu.colortex.cn

[P02] MD5 / SHA256 摘要
来源：http://ld.haigaiapp.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://fz.asd995.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://wu.shtwfgs.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://bz.newstarts.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://lw.9csxet.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://fp.yuexingan06.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://yf.bjjhwx.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://tk.jctech888.com.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ij.wgjwhj.cn

[P03] 生成短随机字符串
来源：http://fa.yuntaijiaju.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://db.wgjwhj.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://vu.nicolike.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://rf.hnjuh.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://zb.shxzukj.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://vt.asd995.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://fq.huixinmuqiang.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://kr.nicolike.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://vi.yuntaijiaju.cn

[P04] 求长度
来源：http://nq.shxzskj.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://oi.hnjuh.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://cx.jianghongdianzi.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://jv.haigaiapp.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://pp.colortex.cn

Java: list.size();  map.size();  s.length()
来源：http://et.lnxyls.cn

Go:   len(arr);  len(m)
来源：http://sa.bjjhwx.cn

Ruby: x.length;  x.size
来源：http://tk.newstarts.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://fj.yuexingan06.cn

[P05] 判断两个对象内容是否相等
来源：http://my.colortex.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://st.jctech888.com.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wr.9csxet.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.yuntaijiaju.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://iv.bjjhwx.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ye.szxytkj.cn

Go:   reflect.DeepEqual(a, b)
来源：http://dt.shtwfgs.cn

Ruby: a == b
来源：http://ji.9csxet.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://gt.jctech888.com.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ri.muxihuayi.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://lr.bookmarksfly.cn

PHP:  if (empty($x)) {}
来源：http://nk.nicolike.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://lh.gzmigu.cn

TS:   if (x == null) {}
来源：http://pj.gzmigu.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://rd.asd995.cn

Go:   if x == nil {}
来源：http://gq.jianghongdianzi.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://rs.wgjwhj.cn

C#:   if (x is null) {}
来源：http://cr.muxihuayi.cn

[P07] 防抖与节流
来源：http://zb.chemitech.net.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://tw.nszjky.cn

PHP:  // 手写时间戳比较
来源：http://gt.chemitech.net.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://gf.haigaiapp.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hb.muxihuayi.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://vy.hnjuh.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://eg.hnjuh.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://gp.hahajie.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://yk.huanxung.cn

[P08] 处理浮点精度问题
来源：http://we.hnjuh.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://eh.szxytkj.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://jp.hahajie.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ai.jctech888.com.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mo.huanxung.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hi.chemitech.net.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://bx.nicolike.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://cw.chemitech.net.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hl.shtwfgs.cn

================================================================================
来源：http://zl.yuntaijiaju.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://yd.huixiangedu.cn

================================================================================
来源：http://mu.gzmigu.cn

[Q01] 创建表
来源：http://fy.shxzukj.cn

CREATE TABLE users (
来源：http://fc.newstarts.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://zz.bjjhwx.cn

name VARCHAR(50) NOT NULL,
来源：http://jm.newstarts.cn

email VARCHAR(100) UNIQUE,
来源：http://xa.shxzskj.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ll.yuexingan06.cn

);
来源：http://nu.asd995.cn

[Q02] 创建带外键的表
来源：http://ld.bookmarksfly.cn

CREATE TABLE orders (
来源：http://lo.521024.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://fu.lnxyls.cn

user_id INT NOT NULL,
来源：http://yi.nszjky.cn

amount DECIMAL(10, 2),
来源：http://xj.huixiangedu.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hg.asd995.cn

);
来源：http://kj.jctech888.com.cn

[Q03] 增加列
来源：http://vi.yuntaijiaju.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ij.huanxung.cn

[Q04] 修改列类型
来源：http://cn.nszjky.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://tc.szxytkj.cn

[Q05] 重命名列
来源：http://ij.jctech888.com.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://nu.huanxung.cn

[Q06] 删除列
来源：http://hb.newstarts.cn

ALTER TABLE users DROP COLUMN age;
来源：http://dy.hahajie.cn

[Q07] 删除表
来源：http://nx.hahajie.cn

DROP TABLE IF EXISTS orders;
来源：http://bk.colortex.cn

[Q08] 创建普通索引
来源：http://mo.hahajie.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://ip.nicolike.cn

[Q09] 创建唯一索引
来源：http://wq.jctech888.com.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://bk.shtwfgs.cn

[Q10] 插入单行
来源：http://za.panjiajie.cn


<!-- 参考信息 -->