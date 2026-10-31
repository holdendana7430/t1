代发 wailian999

JS:   process.exit(1)
来源：http://ob.jianghongdianzi.cn

TS:   process.exit(1)
来源：http://bj.newstarts.cn

Java: System.exit(1)
来源：http://ek.huixinmuqiang.cn

Go:   os.Exit(1)
来源：http://kb.lnxyls.cn

Ruby: exit 1
来源：http://bc.jctech888.com.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://bl.huanxung.cn

[M06] 向标准错误输出
来源：http://ow.szsharing.cn

Py:   print("err", file=sys.stderr)
来源：http://oc.huixiangedu.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://qh.huixinmuqiang.cn

JS:   console.error("err")
来源：http://bk.yuexingan06.cn

TS:   console.error("err")
来源：http://mk.hahajie.cn

Java: System.err.println("err")
来源：http://au.shxzskj.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://fe.szsharing.cn

Ruby: warn "err"
来源：http://dk.9csxet.cn

C#:   Console.Error.WriteLine("err")
来源：http://la.nicolike.cn

[M07] 判断是否为主入口
来源：http://qo.nszjky.cn

Py:   if __name__ == "__main__":
来源：http://qh.huixiangedu.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wy.chemitech.net.cn

JS:   require.main === module
来源：http://uu.9csxet.cn

TS:   require.main === module
来源：http://dl.9csxet.cn

Java: public static void main(String[] args)
来源：http://kc.hnjuh.cn

Go:   func main()
来源：http://ho.bookmarksfly.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://fr.newstarts.cn

C#:   static void Main(string[] args)
来源：http://ut.gzmigu.cn

[M08] 获取系统与运行时信息
来源：http://vw.newstarts.cn

Py:   platform.system();  platform.python_version()
来源：http://hf.521024.cn

PHP:  PHP_OS;  phpversion();
来源：http://hj.shxzskj.cn

JS:   process.platform;  process.version
来源：http://ht.szsharing.cn

TS:   process.platform;  process.version
来源：http://kf.9csxet.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://zn.nszjky.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://cc.muxihuayi.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://cd.gzmigu.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://rc.newstarts.cn

================================================================================
来源：http://hc.muxihuayi.cn

N. 数据结构与算法
来源：http://ya.jianghongdianzi.cn

================================================================================
来源：http://or.521024.cn

[N01] 二分查找（有序数组）
来源：http://gp.shtwfgs.cn

Py:   bisect.bisect_left(arr, x)
来源：http://ie.gzmigu.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://vm.hahajie.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://yp.huixinmuqiang.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mi.bookmarksfly.cn

Java: Arrays.binarySearch(arr, x)
来源：http://am.nszjky.cn

Go:   sort.SearchInts(arr, x)
来源：http://ys.huanxung.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://bf.9csxet.cn

C#:   Array.BinarySearch(arr, x)
来源：http://ep.nicolike.cn

[N02] 排序（工程实践用内置实现）
来源：http://iw.hahajie.cn

Py:   sorted(arr);  arr.sort()
来源：http://mq.chemitech.net.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://az.nicolike.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://lq.huixiangedu.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://ld.bookmarksfly.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hb.huanxung.cn

Go:   slices.Sort(arr)
来源：http://cr.muxihuayi.cn

Ruby: arr.sort
来源：http://qe.yuexingan06.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://gk.yuexingan06.cn

[N03] 快速排序（分治示例）
来源：http://mv.yuntaijiaju.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://sf.lnxyls.cn

PHP:  // 递归实现，或用 usort
来源：http://fs.huixinmuqiang.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://nd.szxytkj.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://nl.9csxet.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://zu.shtwfgs.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ci.bookmarksfly.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://bt.bookmarksfly.cn

C#:   // 手写递归，或 Array.Sort
来源：http://jj.gzmigu.cn

[N04] 斐波那契数列
来源：http://aa.hnjuh.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://su.szsharing.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://jw.muxihuayi.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://td.newstarts.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://fo.shxzukj.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ld.yuexingan06.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://lu.jianghongdianzi.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://bh.gzmigu.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://kz.huixiangedu.cn

[N05] 最大公约数
来源：http://xr.colortex.cn

Py:   math.gcd(a, b)
来源：http://tq.huixinmuqiang.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://gm.jianghongdianzi.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://kw.colortex.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://bo.asd995.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://se.shxzukj.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://pw.lnxyls.cn

Ruby: a.gcd(b)
来源：http://hq.muxihuayi.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://xd.jianghongdianzi.cn

[N06] 判断回文字符串
来源：http://mu.panjiajie.cn

Py:   s == s[::-1]
来源：http://zf.hahajie.cn

PHP:  $s === strrev($s);
来源：http://dc.panjiajie.cn

JS:   s === [...s].reverse().join("")
来源：http://jt.colortex.cn

TS:   s === [...s].reverse().join("")
来源：http://pw.wgjwhj.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://yx.nszjky.cn

Go:   // 双指针从两端比较
来源：http://wi.colortex.cn

Ruby: s == s.reverse
来源：http://gz.nszjky.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://so.huixiangedu.cn

[N07] 两数之和（返回下标）
来源：http://xd.wgjwhj.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://qd.haigaiapp.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://se.521024.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://og.muxihuayi.cn

TS:   // 手写 Map<string, number>
来源：http://ov.asd995.cn

Java: // 手写 HashMap
来源：http://jq.shxzukj.cn

Go:   // 手写 map[int]int
来源：http://sv.huanxung.cn

Ruby: // 手写 Hash
来源：http://ym.nszjky.cn

C#:   // 手写 Dictionary<int, int>
来源：http://ku.bjjhwx.cn

[N08] 生成全排列
来源：http://po.521024.cn

Py:   itertools.permutations(arr)
来源：http://xn.hahajie.cn

PHP:  // 手写递归交换
来源：http://ol.hnjuh.cn

JS:   // 手写回溯递归
来源：http://ue.colortex.cn

TS:   // 手写回溯递归
来源：http://bb.szsharing.cn

Java: // 手写回溯递归
来源：http://ne.szsharing.cn

Go:   // 手写回溯递归
来源：http://lw.yuexingan06.cn

Ruby: arr.permutation.to_a
来源：http://qz.szsharing.cn

C#:   // 手写回溯递归
来源：http://qu.huixinmuqiang.cn

[N09] 栈与队列
来源：http://xe.bookmarksfly.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://la.hnjuh.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wx.szsharing.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ui.muxihuayi.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://dr.wgjwhj.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://xb.szsharing.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hv.szxytkj.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hq.yuntaijiaju.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://nl.gzmigu.cn

[N10] 链表节点定义
来源：http://ha.lnxyls.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://tx.9csxet.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://ks.jctech888.com.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://pk.bookmarksfly.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mb.bjjhwx.cn

Java: class Node { int v; Node next; }
来源：http://lu.gzmigu.cn

Go:   type Node struct { V int; Next *Node }
来源：http://vh.haigaiapp.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://uh.shxzukj.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://je.yuntaijiaju.cn

[N11] 二叉树中序遍历
来源：http://gc.nszjky.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://me.hahajie.cn

PHP:  // 手写递归函数
来源：http://fe.newstarts.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://jm.asd995.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://vf.hnjuh.cn

Java: // 手写递归
来源：http://kz.huanxung.cn

Go:   // 手写递归
来源：http://jj.asd995.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://fm.huanxung.cn

C#:   // 手写递归
来源：http://xk.shxzskj.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://yf.shxzukj.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://zz.bjjhwx.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://bb.haigaiapp.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://bb.jctech888.com.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://fl.colortex.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://xs.nszjky.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://xp.shtwfgs.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://oy.huanxung.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://rg.panjiajie.cn

================================================================================
来源：http://pq.yuexingan06.cn

O. 并发与异步
来源：http://lf.newstarts.cn

================================================================================
来源：http://rx.huixiangedu.cn

[O01] 启动一个线程
来源：http://gt.lnxyls.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ww.huixinmuqiang.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ly.shxzskj.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://bv.panjiajie.cn

TS:   // 同 JS
来源：http://yy.huixinmuqiang.cn

Java: new Thread(() -> f()).start()
来源：http://gi.shxzukj.cn

Go:   go f()
来源：http://ve.huixinmuqiang.cn

Ruby: Thread.new { f }
来源：http://rd.521024.cn

C#:   Task.Run(() => F());
来源：http://sa.huixiangedu.cn

[O02] 使用线程池
来源：http://gf.haigaiapp.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://qi.newstarts.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://js.szxytkj.cn

JS:   // worker_threads 线程池
来源：http://ht.shxzskj.cn

TS:   // worker_threads 线程池
来源：http://uu.nszjky.cn

Java: Executors.newFixedThreadPool(4)
来源：http://aj.asd995.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ot.shxzukj.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://eb.yuexingan06.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://vw.asd995.cn

[O03] 加锁保护共享数据
来源：http://zy.yuntaijiaju.cn

Py:   with lock: shared += 1
来源：http://fu.nicolike.cn

PHP:  // 用 flock() 做文件锁
来源：http://yu.huixinmuqiang.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wf.szxytkj.cn

TS:   // 同 JS
来源：http://nv.nicolike.cn

Java: synchronized (this) { shared++; }
来源：http://bm.shxzukj.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://zi.szxytkj.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://au.lnxyls.cn

C#:   lock (gate) { shared++; }
来源：http://gd.nicolike.cn

[O04] 定义异步函数并等待
来源：http://fs.szsharing.cn

Py:   async def f():⏎    await g()
来源：http://pk.jianghongdianzi.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://vi.9csxet.cn

JS:   async function f() { await g(); }
来源：http://ka.bjjhwx.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://wj.asd995.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hq.hahajie.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://il.shxzskj.cn

Ruby: # 用 Fiber 或 async gem
来源：http://wg.yuntaijiaju.cn

C#:   async Task F() { await G(); }
来源：http://fp.yuntaijiaju.cn

[O05] 并发执行并等待全部完成
来源：http://ci.shxzukj.cn

Py:   asyncio.gather(*tasks)
来源：http://zv.panjiajie.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://zm.bjjhwx.cn

JS:   await Promise.all(tasks)
来源：http://ww.gzmigu.cn

TS:   await Promise.all(tasks)
来源：http://ef.szxytkj.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://fc.shxzskj.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://py.bookmarksfly.cn

Ruby: threads.map(&:join)
来源：http://jc.shxzukj.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://uc.jianghongdianzi.cn

[O06] 使用进程池
来源：http://kp.colortex.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://bt.colortex.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://tg.521024.cn

JS:   // child_process / cluster 模块
来源：http://kk.lnxyls.cn

TS:   // child_process / cluster 模块
来源：http://qr.lnxyls.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://fx.bjjhwx.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://na.shxzskj.cn

Ruby: // fork 块
来源：http://vu.hahajie.cn

C#:   Parallel.For
来源：http://xh.lnxyls.cn

================================================================================
来源：http://zo.jctech888.com.cn

P. 常用工具函数
来源：http://mi.521024.cn

================================================================================
来源：http://yy.asd995.cn

[P01] 生成 UUID
来源：http://bb.huixiangedu.cn

Py:   str(uuid.uuid4())
来源：http://ev.shtwfgs.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://dw.haigaiapp.cn

JS:   crypto.randomUUID()
来源：http://pn.bookmarksfly.cn

TS:   crypto.randomUUID()
来源：http://pc.yuexingan06.cn

Java: UUID.randomUUID().toString()
来源：http://dj.bjjhwx.cn

Go:   // 用 github.com/google/uuid
来源：http://cp.nszjky.cn

Ruby: SecureRandom.uuid
来源：http://og.jctech888.com.cn

C#:   Guid.NewGuid().ToString()
来源：http://kb.chemitech.net.cn

[P02] MD5 / SHA256 摘要
来源：http://ht.yuntaijiaju.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://jp.newstarts.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://pj.bjjhwx.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hi.szsharing.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://fv.shxzskj.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://vb.chemitech.net.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ue.hnjuh.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://go.bookmarksfly.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ec.nszjky.cn

[P03] 生成短随机字符串
来源：http://av.huixiangedu.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://kl.521024.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://bt.huanxung.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://zw.huixiangedu.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hv.huixiangedu.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://am.panjiajie.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://dn.huixinmuqiang.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://fw.szsharing.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://nt.bjjhwx.cn

[P04] 求长度
来源：http://eo.jianghongdianzi.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://tk.asd995.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://nl.panjiajie.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://kn.yuexingan06.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ow.muxihuayi.cn

Java: list.size();  map.size();  s.length()
来源：http://vb.jianghongdianzi.cn

Go:   len(arr);  len(m)
来源：http://qa.haigaiapp.cn

Ruby: x.length;  x.size
来源：http://ph.nicolike.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://lt.shxzskj.cn

[P05] 判断两个对象内容是否相等
来源：http://ni.szxytkj.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://nb.szsharing.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://oy.jctech888.com.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://tx.huanxung.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://zl.wgjwhj.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://tn.newstarts.cn

Go:   reflect.DeepEqual(a, b)
来源：http://qx.hahajie.cn

Ruby: a == b
来源：http://ie.yuntaijiaju.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://sw.chemitech.net.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ry.szsharing.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hs.newstarts.cn

PHP:  if (empty($x)) {}
来源：http://io.asd995.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://qn.bookmarksfly.cn

TS:   if (x == null) {}
来源：http://yz.jianghongdianzi.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://ds.yuexingan06.cn

Go:   if x == nil {}
来源：http://cp.huixiangedu.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://pj.szxytkj.cn

C#:   if (x is null) {}
来源：http://un.szsharing.cn

[P07] 防抖与节流
来源：http://ye.huanxung.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://qo.huixiangedu.cn

PHP:  // 手写时间戳比较
来源：http://go.wgjwhj.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://jn.yuexingan06.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://er.wgjwhj.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ug.yuntaijiaju.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://lp.asd995.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://ll.huixinmuqiang.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://gr.newstarts.cn

[P08] 处理浮点精度问题
来源：http://kg.asd995.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://tg.huixinmuqiang.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://gy.szsharing.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ne.huixinmuqiang.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hu.shxzukj.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://de.shxzukj.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wp.9csxet.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://gh.muxihuayi.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://kt.huixinmuqiang.cn

================================================================================
来源：http://zu.yuexingan06.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://da.szxytkj.cn

================================================================================
来源：http://dx.9csxet.cn

[Q01] 创建表
来源：http://jh.yuexingan06.cn

CREATE TABLE users (
来源：http://mi.bookmarksfly.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ff.shxzskj.cn

name VARCHAR(50) NOT NULL,
来源：http://bb.521024.cn

email VARCHAR(100) UNIQUE,
来源：http://ku.nszjky.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://nf.jianghongdianzi.cn

);
来源：http://su.nszjky.cn

[Q02] 创建带外键的表
来源：http://pc.shtwfgs.cn

CREATE TABLE orders (
来源：http://my.521024.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://vv.shxzskj.cn

user_id INT NOT NULL,
来源：http://jc.shxzskj.cn

amount DECIMAL(10, 2),
来源：http://oo.huixiangedu.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mo.521024.cn

);
来源：http://zn.newstarts.cn

[Q03] 增加列
来源：http://yi.shtwfgs.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://xp.asd995.cn

[Q04] 修改列类型
来源：http://nc.huixiangedu.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://so.panjiajie.cn

[Q05] 重命名列
来源：http://lj.yuexingan06.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://gr.nszjky.cn

[Q06] 删除列
来源：http://yo.521024.cn


<!-- 参考信息 -->