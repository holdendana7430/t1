代发 wailian999

Ruby: exit 1
来源：http://fc.newstarts.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://po.hahajie.cn

[M06] 向标准错误输出
来源：http://qr.huanxung.cn

Py:   print("err", file=sys.stderr)
来源：http://ep.jianghongdianzi.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://lu.szsharing.cn

JS:   console.error("err")
来源：http://gl.jctech888.com.cn

TS:   console.error("err")
来源：http://th.muxihuayi.cn

Java: System.err.println("err")
来源：http://zp.yuntaijiaju.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://qu.szsharing.cn

Ruby: warn "err"
来源：http://jm.lnxyls.cn

C#:   Console.Error.WriteLine("err")
来源：http://em.huanxung.cn

[M07] 判断是否为主入口
来源：http://kl.newstarts.cn

Py:   if __name__ == "__main__":
来源：http://xf.huixiangedu.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://dv.jctech888.com.cn

JS:   require.main === module
来源：http://mf.shtwfgs.cn

TS:   require.main === module
来源：http://yr.chemitech.net.cn

Java: public static void main(String[] args)
来源：http://ys.jianghongdianzi.cn

Go:   func main()
来源：http://ap.yuntaijiaju.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://yj.shtwfgs.cn

C#:   static void Main(string[] args)
来源：http://ct.hnjuh.cn

[M08] 获取系统与运行时信息
来源：http://jl.jctech888.com.cn

Py:   platform.system();  platform.python_version()
来源：http://nf.szxytkj.cn

PHP:  PHP_OS;  phpversion();
来源：http://vb.panjiajie.cn

JS:   process.platform;  process.version
来源：http://jl.yuntaijiaju.cn

TS:   process.platform;  process.version
来源：http://nc.gzmigu.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ss.shtwfgs.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://vx.shxzukj.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://qz.lnxyls.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://el.hahajie.cn

================================================================================
来源：http://jr.newstarts.cn

N. 数据结构与算法
来源：http://vp.szsharing.cn

================================================================================
来源：http://bn.9csxet.cn

[N01] 二分查找（有序数组）
来源：http://yn.nszjky.cn

Py:   bisect.bisect_left(arr, x)
来源：http://hb.huixinmuqiang.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://pi.hahajie.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mk.asd995.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://nm.521024.cn

Java: Arrays.binarySearch(arr, x)
来源：http://hm.gzmigu.cn

Go:   sort.SearchInts(arr, x)
来源：http://uj.muxihuayi.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://bv.shxzukj.cn

C#:   Array.BinarySearch(arr, x)
来源：http://bp.huanxung.cn

[N02] 排序（工程实践用内置实现）
来源：http://or.chemitech.net.cn

Py:   sorted(arr);  arr.sort()
来源：http://da.muxihuayi.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ya.newstarts.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://ii.muxihuayi.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://op.hnjuh.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://qu.szxytkj.cn

Go:   slices.Sort(arr)
来源：http://ze.chemitech.net.cn

Ruby: arr.sort
来源：http://fc.9csxet.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://so.nszjky.cn

[N03] 快速排序（分治示例）
来源：http://cm.shtwfgs.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://tf.muxihuayi.cn

PHP:  // 递归实现，或用 usort
来源：http://bb.huixiangedu.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://zg.szxytkj.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://yj.jianghongdianzi.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://we.shxzukj.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://zy.9csxet.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://rd.bookmarksfly.cn

C#:   // 手写递归，或 Array.Sort
来源：http://up.shxzukj.cn

[N04] 斐波那契数列
来源：http://bh.gzmigu.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://xb.shxzskj.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://gf.yuntaijiaju.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mt.bookmarksfly.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://vx.muxihuayi.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ej.gzmigu.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://zb.szsharing.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ov.wgjwhj.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://er.bookmarksfly.cn

[N05] 最大公约数
来源：http://yu.jianghongdianzi.cn

Py:   math.gcd(a, b)
来源：http://cj.hnjuh.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://iw.shtwfgs.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mm.huixinmuqiang.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://zg.asd995.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://il.huixinmuqiang.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://jm.colortex.cn

Ruby: a.gcd(b)
来源：http://dk.newstarts.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://th.nszjky.cn

[N06] 判断回文字符串
来源：http://cy.jianghongdianzi.cn

Py:   s == s[::-1]
来源：http://wj.asd995.cn

PHP:  $s === strrev($s);
来源：http://uk.muxihuayi.cn

JS:   s === [...s].reverse().join("")
来源：http://ik.newstarts.cn

TS:   s === [...s].reverse().join("")
来源：http://wg.jianghongdianzi.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://cn.colortex.cn

Go:   // 双指针从两端比较
来源：http://nq.colortex.cn

Ruby: s == s.reverse
来源：http://jc.bookmarksfly.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://fa.gzmigu.cn

[N07] 两数之和（返回下标）
来源：http://ur.wgjwhj.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://rf.colortex.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ez.hahajie.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://it.nicolike.cn

TS:   // 手写 Map<string, number>
来源：http://bk.szsharing.cn

Java: // 手写 HashMap
来源：http://gk.9csxet.cn

Go:   // 手写 map[int]int
来源：http://mi.nicolike.cn

Ruby: // 手写 Hash
来源：http://au.hnjuh.cn

C#:   // 手写 Dictionary<int, int>
来源：http://bn.chemitech.net.cn

[N08] 生成全排列
来源：http://am.gzmigu.cn

Py:   itertools.permutations(arr)
来源：http://as.shxzukj.cn

PHP:  // 手写递归交换
来源：http://ps.hnjuh.cn

JS:   // 手写回溯递归
来源：http://nm.9csxet.cn

TS:   // 手写回溯递归
来源：http://fw.huanxung.cn

Java: // 手写回溯递归
来源：http://hj.yuexingan06.cn

Go:   // 手写回溯递归
来源：http://ny.shtwfgs.cn

Ruby: arr.permutation.to_a
来源：http://ch.gzmigu.cn

C#:   // 手写回溯递归
来源：http://jk.szxytkj.cn

[N09] 栈与队列
来源：http://za.huixinmuqiang.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wz.nszjky.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mx.lnxyls.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://bf.hnjuh.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wy.hahajie.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://qc.9csxet.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://zr.jctech888.com.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://sn.panjiajie.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ai.jctech888.com.cn

[N10] 链表节点定义
来源：http://ud.jctech888.com.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://qx.huanxung.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://nq.szsharing.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://xl.szxytkj.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wr.shxzskj.cn

Java: class Node { int v; Node next; }
来源：http://rr.muxihuayi.cn

Go:   type Node struct { V int; Next *Node }
来源：http://cf.shxzskj.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://xm.shxzukj.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://ka.yuexingan06.cn

[N11] 二叉树中序遍历
来源：http://uo.jianghongdianzi.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://pq.colortex.cn

PHP:  // 手写递归函数
来源：http://dy.muxihuayi.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://rs.gzmigu.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://zz.huixiangedu.cn

Java: // 手写递归
来源：http://xy.huixinmuqiang.cn

Go:   // 手写递归
来源：http://md.shtwfgs.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://bv.jianghongdianzi.cn

C#:   // 手写递归
来源：http://os.yuexingan06.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://al.bjjhwx.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ik.hnjuh.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://cn.521024.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://cq.huixiangedu.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://bn.wgjwhj.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://xt.panjiajie.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hr.shxzskj.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://kq.panjiajie.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hl.szsharing.cn

================================================================================
来源：http://qg.shxzukj.cn

O. 并发与异步
来源：http://ns.jctech888.com.cn

================================================================================
来源：http://up.yuexingan06.cn

[O01] 启动一个线程
来源：http://nb.panjiajie.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ij.jctech888.com.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://qc.newstarts.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ij.newstarts.cn

TS:   // 同 JS
来源：http://xe.jctech888.com.cn

Java: new Thread(() -> f()).start()
来源：http://qq.huanxung.cn

Go:   go f()
来源：http://kx.muxihuayi.cn

Ruby: Thread.new { f }
来源：http://qa.chemitech.net.cn

C#:   Task.Run(() => F());
来源：http://zs.asd995.cn

[O02] 使用线程池
来源：http://jt.huixiangedu.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://vk.nszjky.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ze.hahajie.cn

JS:   // worker_threads 线程池
来源：http://vp.9csxet.cn

TS:   // worker_threads 线程池
来源：http://tz.wgjwhj.cn

Java: Executors.newFixedThreadPool(4)
来源：http://mf.asd995.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://qn.jctech888.com.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://cv.nszjky.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ij.asd995.cn

[O03] 加锁保护共享数据
来源：http://st.muxihuayi.cn

Py:   with lock: shared += 1
来源：http://rk.huanxung.cn

PHP:  // 用 flock() 做文件锁
来源：http://cd.asd995.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://rv.chemitech.net.cn

TS:   // 同 JS
来源：http://sz.huixinmuqiang.cn

Java: synchronized (this) { shared++; }
来源：http://mp.jianghongdianzi.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ox.colortex.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://ol.lnxyls.cn

C#:   lock (gate) { shared++; }
来源：http://oj.lnxyls.cn

[O04] 定义异步函数并等待
来源：http://gk.nicolike.cn

Py:   async def f():⏎    await g()
来源：http://sc.panjiajie.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ew.yuexingan06.cn

JS:   async function f() { await g(); }
来源：http://kb.yuntaijiaju.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://id.shxzskj.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://nx.szxytkj.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ss.haigaiapp.cn

Ruby: # 用 Fiber 或 async gem
来源：http://ny.chemitech.net.cn

C#:   async Task F() { await G(); }
来源：http://xq.szxytkj.cn

[O05] 并发执行并等待全部完成
来源：http://ya.jctech888.com.cn

Py:   asyncio.gather(*tasks)
来源：http://yo.9csxet.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ys.szxytkj.cn

JS:   await Promise.all(tasks)
来源：http://pz.chemitech.net.cn

TS:   await Promise.all(tasks)
来源：http://rn.muxihuayi.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://um.muxihuayi.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://tl.shtwfgs.cn

Ruby: threads.map(&:join)
来源：http://xc.wgjwhj.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://xt.gzmigu.cn

[O06] 使用进程池
来源：http://sr.huixiangedu.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://lw.yuexingan06.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://od.huixinmuqiang.cn

JS:   // child_process / cluster 模块
来源：http://ym.hnjuh.cn

TS:   // child_process / cluster 模块
来源：http://cy.chemitech.net.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://qm.huixiangedu.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ux.shtwfgs.cn

Ruby: // fork 块
来源：http://ph.panjiajie.cn

C#:   Parallel.For
来源：http://ba.muxihuayi.cn

================================================================================
来源：http://ye.9csxet.cn

P. 常用工具函数
来源：http://qd.yuexingan06.cn

================================================================================
来源：http://kl.hnjuh.cn

[P01] 生成 UUID
来源：http://vn.muxihuayi.cn

Py:   str(uuid.uuid4())
来源：http://lz.newstarts.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://zx.huixinmuqiang.cn

JS:   crypto.randomUUID()
来源：http://pc.bjjhwx.cn

TS:   crypto.randomUUID()
来源：http://qn.panjiajie.cn

Java: UUID.randomUUID().toString()
来源：http://gi.gzmigu.cn

Go:   // 用 github.com/google/uuid
来源：http://zz.521024.cn

Ruby: SecureRandom.uuid
来源：http://ir.hnjuh.cn

C#:   Guid.NewGuid().ToString()
来源：http://yz.9csxet.cn

[P02] MD5 / SHA256 摘要
来源：http://rd.szxytkj.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://nf.panjiajie.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://xr.colortex.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mn.nszjky.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ea.shxzskj.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://sr.jctech888.com.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hi.szsharing.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://je.colortex.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://cc.huixiangedu.cn

[P03] 生成短随机字符串
来源：http://wv.chemitech.net.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://tv.521024.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://su.yuntaijiaju.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://uy.hnjuh.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://by.hahajie.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://kq.9csxet.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ai.colortex.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://jb.shtwfgs.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wm.huixinmuqiang.cn

[P04] 求长度
来源：http://kt.9csxet.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://nj.yuntaijiaju.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://yj.yuexingan06.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://zh.colortex.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wd.521024.cn

Java: list.size();  map.size();  s.length()
来源：http://an.newstarts.cn

Go:   len(arr);  len(m)
来源：http://ci.panjiajie.cn

Ruby: x.length;  x.size
来源：http://xm.newstarts.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://ry.521024.cn

[P05] 判断两个对象内容是否相等
来源：http://db.hnjuh.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://xn.shxzukj.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://og.bjjhwx.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ou.huixinmuqiang.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://sb.szxytkj.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://kd.huanxung.cn

Go:   reflect.DeepEqual(a, b)
来源：http://ze.yuntaijiaju.cn

Ruby: a == b
来源：http://ln.szxytkj.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://fj.nicolike.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://zz.hnjuh.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://gp.newstarts.cn

PHP:  if (empty($x)) {}
来源：http://de.wgjwhj.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://yb.haigaiapp.cn

TS:   if (x == null) {}
来源：http://wq.huanxung.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://ga.nicolike.cn

Go:   if x == nil {}
来源：http://rq.jctech888.com.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://lv.chemitech.net.cn

C#:   if (x is null) {}
来源：http://pm.colortex.cn

[P07] 防抖与节流
来源：http://nd.asd995.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://te.shxzukj.cn

PHP:  // 手写时间戳比较
来源：http://hl.hahajie.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ie.chemitech.net.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ug.521024.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wn.panjiajie.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://fa.nszjky.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://vp.huanxung.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://rf.huixinmuqiang.cn

[P08] 处理浮点精度问题
来源：http://dt.lnxyls.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ol.nicolike.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://tv.muxihuayi.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://yx.huixinmuqiang.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://cq.yuntaijiaju.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://uh.lnxyls.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://iz.panjiajie.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://li.shtwfgs.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://pz.9csxet.cn

================================================================================
来源：http://fs.gzmigu.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://we.shxzukj.cn

================================================================================
来源：http://ll.panjiajie.cn

[Q01] 创建表
来源：http://ln.jctech888.com.cn

CREATE TABLE users (
来源：http://qq.muxihuayi.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://gr.panjiajie.cn

name VARCHAR(50) NOT NULL,
来源：http://kp.shxzskj.cn

email VARCHAR(100) UNIQUE,
来源：http://pe.szsharing.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://oe.chemitech.net.cn

);
来源：http://hw.yuntaijiaju.cn

[Q02] 创建带外键的表
来源：http://na.hahajie.cn

CREATE TABLE orders (
来源：http://qy.yuntaijiaju.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ng.jctech888.com.cn

user_id INT NOT NULL,
来源：http://ps.shtwfgs.cn

amount DECIMAL(10, 2),
来源：http://bt.shtwfgs.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://np.muxihuayi.cn

);
来源：http://dn.wgjwhj.cn

[Q03] 增加列
来源：http://wi.muxihuayi.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://da.wgjwhj.cn

[Q04] 修改列类型
来源：http://yq.szxytkj.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://yh.bookmarksfly.cn

[Q05] 重命名列
来源：http://pe.chemitech.net.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://fc.wgjwhj.cn

[Q06] 删除列
来源：http://oo.hahajie.cn

ALTER TABLE users DROP COLUMN age;
来源：http://in.panjiajie.cn

[Q07] 删除表
来源：http://jl.szsharing.cn

DROP TABLE IF EXISTS orders;
来源：http://lw.nszjky.cn

[Q08] 创建普通索引
来源：http://md.hahajie.cn


<!-- 参考信息 -->