代发 wailian999

JS:   process.exit(1)
来源：http://vn.yuntaijiaju.cn

TS:   process.exit(1)
来源：http://yl.yuexingan06.cn

Java: System.exit(1)
来源：http://zu.jctech888.com.cn

Go:   os.Exit(1)
来源：http://qf.yuntaijiaju.cn

Ruby: exit 1
来源：http://um.colortex.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://tl.hnjuh.cn

[M06] 向标准错误输出
来源：http://kl.nicolike.cn

Py:   print("err", file=sys.stderr)
来源：http://qc.nicolike.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://gn.newstarts.cn

JS:   console.error("err")
来源：http://il.yuexingan06.cn

TS:   console.error("err")
来源：http://lh.wgjwhj.cn

Java: System.err.println("err")
来源：http://sp.huixinmuqiang.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://fa.521024.cn

Ruby: warn "err"
来源：http://yh.huixiangedu.cn

C#:   Console.Error.WriteLine("err")
来源：http://oq.9csxet.cn

[M07] 判断是否为主入口
来源：http://kb.szxytkj.cn

Py:   if __name__ == "__main__":
来源：http://yt.gzmigu.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://rb.chemitech.net.cn

JS:   require.main === module
来源：http://vq.huixinmuqiang.cn

TS:   require.main === module
来源：http://ii.huanxung.cn

Java: public static void main(String[] args)
来源：http://fl.yuntaijiaju.cn

Go:   func main()
来源：http://aa.nicolike.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://pl.hahajie.cn

C#:   static void Main(string[] args)
来源：http://gw.shxzskj.cn

[M08] 获取系统与运行时信息
来源：http://xn.haigaiapp.cn

Py:   platform.system();  platform.python_version()
来源：http://xj.jianghongdianzi.cn

PHP:  PHP_OS;  phpversion();
来源：http://xf.gzmigu.cn

JS:   process.platform;  process.version
来源：http://pb.nszjky.cn

TS:   process.platform;  process.version
来源：http://oa.wgjwhj.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://cs.panjiajie.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://ud.chemitech.net.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://yw.huixinmuqiang.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://po.gzmigu.cn

================================================================================
来源：http://er.bookmarksfly.cn

N. 数据结构与算法
来源：http://ra.bookmarksfly.cn

================================================================================
来源：http://dn.shtwfgs.cn

[N01] 二分查找（有序数组）
来源：http://an.szxytkj.cn

Py:   bisect.bisect_left(arr, x)
来源：http://qo.asd995.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://qr.jianghongdianzi.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://bp.szsharing.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://tc.huanxung.cn

Java: Arrays.binarySearch(arr, x)
来源：http://aj.newstarts.cn

Go:   sort.SearchInts(arr, x)
来源：http://ne.shxzskj.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://aq.asd995.cn

C#:   Array.BinarySearch(arr, x)
来源：http://zr.jianghongdianzi.cn

[N02] 排序（工程实践用内置实现）
来源：http://fh.wgjwhj.cn

Py:   sorted(arr);  arr.sort()
来源：http://ru.shxzskj.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://vh.colortex.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://jx.huanxung.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://zz.panjiajie.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://it.shxzukj.cn

Go:   slices.Sort(arr)
来源：http://dz.jctech888.com.cn

Ruby: arr.sort
来源：http://sj.szxytkj.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://at.szxytkj.cn

[N03] 快速排序（分治示例）
来源：http://yb.yuexingan06.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ai.shxzukj.cn

PHP:  // 递归实现，或用 usort
来源：http://ws.lnxyls.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://to.521024.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://tf.szxytkj.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://tx.hahajie.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ou.newstarts.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wt.haigaiapp.cn

C#:   // 手写递归，或 Array.Sort
来源：http://vi.9csxet.cn

[N04] 斐波那契数列
来源：http://wl.chemitech.net.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://zs.shxzskj.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hu.panjiajie.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://yl.jctech888.com.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://dr.huanxung.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://tj.9csxet.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://zt.asd995.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ze.wgjwhj.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://kd.newstarts.cn

[N05] 最大公约数
来源：http://dd.bookmarksfly.cn

Py:   math.gcd(a, b)
来源：http://wf.newstarts.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://zy.hahajie.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://zw.jianghongdianzi.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://no.szsharing.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://fp.gzmigu.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mr.huixiangedu.cn

Ruby: a.gcd(b)
来源：http://qa.shxzskj.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://lt.nszjky.cn

[N06] 判断回文字符串
来源：http://zw.bjjhwx.cn

Py:   s == s[::-1]
来源：http://kt.yuexingan06.cn

PHP:  $s === strrev($s);
来源：http://wn.muxihuayi.cn

JS:   s === [...s].reverse().join("")
来源：http://eh.hahajie.cn

TS:   s === [...s].reverse().join("")
来源：http://yu.newstarts.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://pt.lnxyls.cn

Go:   // 双指针从两端比较
来源：http://xy.521024.cn

Ruby: s == s.reverse
来源：http://bz.bookmarksfly.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://nt.jctech888.com.cn

[N07] 两数之和（返回下标）
来源：http://uj.gzmigu.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ey.szsharing.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://qr.hnjuh.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://ks.muxihuayi.cn

TS:   // 手写 Map<string, number>
来源：http://tb.shtwfgs.cn

Java: // 手写 HashMap
来源：http://bf.wgjwhj.cn

Go:   // 手写 map[int]int
来源：http://nm.nszjky.cn

Ruby: // 手写 Hash
来源：http://xp.szsharing.cn

C#:   // 手写 Dictionary<int, int>
来源：http://pr.szxytkj.cn

[N08] 生成全排列
来源：http://ja.panjiajie.cn

Py:   itertools.permutations(arr)
来源：http://wp.colortex.cn

PHP:  // 手写递归交换
来源：http://fx.newstarts.cn

JS:   // 手写回溯递归
来源：http://do.jianghongdianzi.cn

TS:   // 手写回溯递归
来源：http://kv.hnjuh.cn

Java: // 手写回溯递归
来源：http://ij.colortex.cn

Go:   // 手写回溯递归
来源：http://rw.haigaiapp.cn

Ruby: arr.permutation.to_a
来源：http://gv.bookmarksfly.cn

C#:   // 手写回溯递归
来源：http://ds.asd995.cn

[N09] 栈与队列
来源：http://hm.chemitech.net.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://tw.521024.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://yx.huanxung.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://av.wgjwhj.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wa.hahajie.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://nl.huixiangedu.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://dh.bjjhwx.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://zp.panjiajie.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://dd.shxzskj.cn

[N10] 链表节点定义
来源：http://lh.huixiangedu.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://xk.huixinmuqiang.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://ed.haigaiapp.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://qp.bjjhwx.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://sd.szsharing.cn

Java: class Node { int v; Node next; }
来源：http://ii.chemitech.net.cn

Go:   type Node struct { V int; Next *Node }
来源：http://ep.yuexingan06.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://sj.asd995.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://mw.szsharing.cn

[N11] 二叉树中序遍历
来源：http://oe.521024.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://du.nszjky.cn

PHP:  // 手写递归函数
来源：http://jz.asd995.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://km.nicolike.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://je.bookmarksfly.cn

Java: // 手写递归
来源：http://yo.9csxet.cn

Go:   // 手写递归
来源：http://df.newstarts.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://kl.asd995.cn

C#:   // 手写递归
来源：http://nl.newstarts.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://vn.colortex.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://rc.shxzukj.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://sy.szxytkj.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ci.huixinmuqiang.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://jt.shtwfgs.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ao.nszjky.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://kv.szxytkj.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://br.szxytkj.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://uo.colortex.cn

================================================================================
来源：http://fx.hnjuh.cn

O. 并发与异步
来源：http://un.lnxyls.cn

================================================================================
来源：http://qj.shxzukj.cn

[O01] 启动一个线程
来源：http://pa.szsharing.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://in.yuntaijiaju.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://es.bookmarksfly.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://bd.huanxung.cn

TS:   // 同 JS
来源：http://qg.szxytkj.cn

Java: new Thread(() -> f()).start()
来源：http://zt.jianghongdianzi.cn

Go:   go f()
来源：http://lo.huanxung.cn

Ruby: Thread.new { f }
来源：http://ed.yuexingan06.cn

C#:   Task.Run(() => F());
来源：http://td.521024.cn

[O02] 使用线程池
来源：http://me.shxzskj.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://kl.hnjuh.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://nv.asd995.cn

JS:   // worker_threads 线程池
来源：http://ci.bookmarksfly.cn

TS:   // worker_threads 线程池
来源：http://vp.asd995.cn

Java: Executors.newFixedThreadPool(4)
来源：http://ie.shtwfgs.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://fb.nicolike.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hj.nicolike.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://al.huixiangedu.cn

[O03] 加锁保护共享数据
来源：http://sw.hahajie.cn

Py:   with lock: shared += 1
来源：http://ov.shxzskj.cn

PHP:  // 用 flock() 做文件锁
来源：http://fz.yuntaijiaju.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ir.asd995.cn

TS:   // 同 JS
来源：http://tw.panjiajie.cn

Java: synchronized (this) { shared++; }
来源：http://ln.szsharing.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://re.shxzukj.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://pg.521024.cn

C#:   lock (gate) { shared++; }
来源：http://ka.haigaiapp.cn

[O04] 定义异步函数并等待
来源：http://en.yuexingan06.cn

Py:   async def f():⏎    await g()
来源：http://lo.nszjky.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://sg.521024.cn

JS:   async function f() { await g(); }
来源：http://gm.newstarts.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://cg.521024.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://sz.shxzukj.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://zw.gzmigu.cn

Ruby: # 用 Fiber 或 async gem
来源：http://cv.panjiajie.cn

C#:   async Task F() { await G(); }
来源：http://sm.huixiangedu.cn

[O05] 并发执行并等待全部完成
来源：http://us.hnjuh.cn

Py:   asyncio.gather(*tasks)
来源：http://sz.nszjky.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://jx.hahajie.cn

JS:   await Promise.all(tasks)
来源：http://fd.szsharing.cn

TS:   await Promise.all(tasks)
来源：http://sd.colortex.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ug.521024.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://re.shxzukj.cn

Ruby: threads.map(&:join)
来源：http://ml.gzmigu.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://ey.shtwfgs.cn

[O06] 使用进程池
来源：http://mj.nszjky.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://tb.bookmarksfly.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://fj.shxzskj.cn

JS:   // child_process / cluster 模块
来源：http://db.chemitech.net.cn

TS:   // child_process / cluster 模块
来源：http://gl.haigaiapp.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hm.bookmarksfly.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://sc.nszjky.cn

Ruby: // fork 块
来源：http://zk.bjjhwx.cn

C#:   Parallel.For
来源：http://da.asd995.cn

================================================================================
来源：http://oh.jctech888.com.cn

P. 常用工具函数
来源：http://dy.shxzukj.cn

================================================================================
来源：http://bi.muxihuayi.cn

[P01] 生成 UUID
来源：http://zx.szxytkj.cn

Py:   str(uuid.uuid4())
来源：http://cy.colortex.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://kp.huixiangedu.cn

JS:   crypto.randomUUID()
来源：http://py.szsharing.cn

TS:   crypto.randomUUID()
来源：http://cs.szxytkj.cn

Java: UUID.randomUUID().toString()
来源：http://cb.jianghongdianzi.cn

Go:   // 用 github.com/google/uuid
来源：http://qk.chemitech.net.cn

Ruby: SecureRandom.uuid
来源：http://jp.asd995.cn

C#:   Guid.NewGuid().ToString()
来源：http://dk.hnjuh.cn

[P02] MD5 / SHA256 摘要
来源：http://mp.colortex.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://fp.521024.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://dc.lnxyls.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://vk.nicolike.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://bl.yuexingan06.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://fk.panjiajie.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://vf.muxihuayi.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://da.hnjuh.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://sy.szsharing.cn

[P03] 生成短随机字符串
来源：http://mv.huixinmuqiang.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://gd.colortex.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ye.wgjwhj.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://zw.lnxyls.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://he.chemitech.net.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ox.shtwfgs.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hl.9csxet.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://ub.panjiajie.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://kj.huixiangedu.cn

[P04] 求长度
来源：http://aj.huanxung.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hy.szxytkj.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://xq.yuexingan06.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://au.9csxet.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://xr.colortex.cn

Java: list.size();  map.size();  s.length()
来源：http://rl.muxihuayi.cn

Go:   len(arr);  len(m)
来源：http://bb.yuexingan06.cn

Ruby: x.length;  x.size
来源：http://eo.gzmigu.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://cl.colortex.cn

[P05] 判断两个对象内容是否相等
来源：http://wo.lnxyls.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://lv.nicolike.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://kr.colortex.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://iq.shxzskj.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://cf.hahajie.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://yi.bjjhwx.cn

Go:   reflect.DeepEqual(a, b)
来源：http://jv.jctech888.com.cn

Ruby: a == b
来源：http://zs.gzmigu.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://er.chemitech.net.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ru.colortex.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://uv.panjiajie.cn

PHP:  if (empty($x)) {}
来源：http://xu.wgjwhj.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://rh.newstarts.cn

TS:   if (x == null) {}
来源：http://oz.521024.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://mj.huixiangedu.cn

Go:   if x == nil {}
来源：http://uj.shxzukj.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://kb.szsharing.cn

C#:   if (x is null) {}
来源：http://kv.huixinmuqiang.cn

[P07] 防抖与节流
来源：http://ge.panjiajie.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://oc.haigaiapp.cn

PHP:  // 手写时间戳比较
来源：http://dg.huixiangedu.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://cf.hahajie.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://zm.521024.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://by.9csxet.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ym.bookmarksfly.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://hp.shxzukj.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ij.jianghongdianzi.cn

[P08] 处理浮点精度问题
来源：http://li.szsharing.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://er.521024.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://br.shxzukj.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://rh.panjiajie.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://lh.9csxet.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wf.shxzukj.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://vl.szsharing.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ah.muxihuayi.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://fv.newstarts.cn

================================================================================
来源：http://ak.shxzukj.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ia.lnxyls.cn

================================================================================
来源：http://gg.jianghongdianzi.cn

[Q01] 创建表
来源：http://xm.huixiangedu.cn

CREATE TABLE users (
来源：http://uw.shxzukj.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://kn.colortex.cn

name VARCHAR(50) NOT NULL,
来源：http://vt.chemitech.net.cn

email VARCHAR(100) UNIQUE,
来源：http://og.shxzskj.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://vl.jianghongdianzi.cn

);
来源：http://at.newstarts.cn

[Q02] 创建带外键的表
来源：http://nl.shtwfgs.cn

CREATE TABLE orders (
来源：http://ve.wgjwhj.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://jj.szsharing.cn

user_id INT NOT NULL,
来源：http://qu.gzmigu.cn

amount DECIMAL(10, 2),
来源：http://lh.newstarts.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ry.asd995.cn

);
来源：http://tz.hahajie.cn

[Q03] 增加列
来源：http://yh.jctech888.com.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://bx.wgjwhj.cn

[Q04] 修改列类型
来源：http://bt.gzmigu.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://fb.gzmigu.cn

[Q05] 重命名列
来源：http://gh.gzmigu.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ja.521024.cn

[Q06] 删除列
来源：http://ke.shxzukj.cn


<!-- 参考信息 -->