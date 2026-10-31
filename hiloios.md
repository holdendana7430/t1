代发 wailian999

PHP:  fwrite(STDERR, "err\n");
来源：http://yf.bjjhwx.cn

JS:   console.error("err")
来源：http://an.hahajie.cn

TS:   console.error("err")
来源：http://cc.bookmarksfly.cn

Java: System.err.println("err")
来源：http://ay.newstarts.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://vm.hahajie.cn

Ruby: warn "err"
来源：http://gu.gzmigu.cn

C#:   Console.Error.WriteLine("err")
来源：http://qm.jctech888.com.cn

[M07] 判断是否为主入口
来源：http://sb.hahajie.cn

Py:   if __name__ == "__main__":
来源：http://ir.haigaiapp.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://kf.521024.cn

JS:   require.main === module
来源：http://kf.szsharing.cn

TS:   require.main === module
来源：http://ox.lnxyls.cn

Java: public static void main(String[] args)
来源：http://ro.hahajie.cn

Go:   func main()
来源：http://cb.bookmarksfly.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wo.bjjhwx.cn

C#:   static void Main(string[] args)
来源：http://lo.gzmigu.cn

[M08] 获取系统与运行时信息
来源：http://hw.nszjky.cn

Py:   platform.system();  platform.python_version()
来源：http://tv.lnxyls.cn

PHP:  PHP_OS;  phpversion();
来源：http://vd.newstarts.cn

JS:   process.platform;  process.version
来源：http://pn.szxytkj.cn

TS:   process.platform;  process.version
来源：http://iw.nszjky.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ym.521024.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://vy.szsharing.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mb.hahajie.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://bc.huanxung.cn

================================================================================
来源：http://rf.haigaiapp.cn

N. 数据结构与算法
来源：http://wg.jianghongdianzi.cn

================================================================================
来源：http://do.shxzskj.cn

[N01] 二分查找（有序数组）
来源：http://sw.shxzukj.cn

Py:   bisect.bisect_left(arr, x)
来源：http://hk.jianghongdianzi.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://zm.9csxet.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://jt.panjiajie.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://fw.newstarts.cn

Java: Arrays.binarySearch(arr, x)
来源：http://hm.szxytkj.cn

Go:   sort.SearchInts(arr, x)
来源：http://ja.haigaiapp.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://mk.hnjuh.cn

C#:   Array.BinarySearch(arr, x)
来源：http://wa.newstarts.cn

[N02] 排序（工程实践用内置实现）
来源：http://ip.yuntaijiaju.cn

Py:   sorted(arr);  arr.sort()
来源：http://nm.asd995.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://go.nszjky.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://tl.colortex.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://gi.colortex.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://pe.panjiajie.cn

Go:   slices.Sort(arr)
来源：http://vw.szxytkj.cn

Ruby: arr.sort
来源：http://zu.lnxyls.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://tu.nicolike.cn

[N03] 快速排序（分治示例）
来源：http://my.nicolike.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://kx.jctech888.com.cn

PHP:  // 递归实现，或用 usort
来源：http://jr.nszjky.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://sv.szxytkj.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://zs.jctech888.com.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://lf.szxytkj.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://cy.yuntaijiaju.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mo.yuexingan06.cn

C#:   // 手写递归，或 Array.Sort
来源：http://cs.gzmigu.cn

[N04] 斐波那契数列
来源：http://av.shtwfgs.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://gz.newstarts.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://uc.jctech888.com.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ts.521024.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://kc.521024.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ex.szsharing.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://jk.lnxyls.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ge.panjiajie.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://yd.nszjky.cn

[N05] 最大公约数
来源：http://xh.jianghongdianzi.cn

Py:   math.gcd(a, b)
来源：http://fn.huanxung.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://jj.szsharing.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ry.bookmarksfly.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://zd.panjiajie.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://dg.muxihuayi.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://go.huixinmuqiang.cn

Ruby: a.gcd(b)
来源：http://ft.chemitech.net.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ss.gzmigu.cn

[N06] 判断回文字符串
来源：http://zc.shxzskj.cn

Py:   s == s[::-1]
来源：http://qn.newstarts.cn

PHP:  $s === strrev($s);
来源：http://jm.asd995.cn

JS:   s === [...s].reverse().join("")
来源：http://fq.yuexingan06.cn

TS:   s === [...s].reverse().join("")
来源：http://et.newstarts.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://xo.jianghongdianzi.cn

Go:   // 双指针从两端比较
来源：http://zg.huanxung.cn

Ruby: s == s.reverse
来源：http://rc.asd995.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://rn.shxzskj.cn

[N07] 两数之和（返回下标）
来源：http://rm.hnjuh.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://oq.huanxung.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ce.shxzskj.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://pf.bjjhwx.cn

TS:   // 手写 Map<string, number>
来源：http://fh.9csxet.cn

Java: // 手写 HashMap
来源：http://xn.nszjky.cn

Go:   // 手写 map[int]int
来源：http://xh.521024.cn

Ruby: // 手写 Hash
来源：http://ef.521024.cn

C#:   // 手写 Dictionary<int, int>
来源：http://xw.haigaiapp.cn

[N08] 生成全排列
来源：http://pv.wgjwhj.cn

Py:   itertools.permutations(arr)
来源：http://uq.521024.cn

PHP:  // 手写递归交换
来源：http://dy.hnjuh.cn

JS:   // 手写回溯递归
来源：http://tf.gzmigu.cn

TS:   // 手写回溯递归
来源：http://jf.szsharing.cn

Java: // 手写回溯递归
来源：http://cy.szxytkj.cn

Go:   // 手写回溯递归
来源：http://gw.haigaiapp.cn

Ruby: arr.permutation.to_a
来源：http://ad.9csxet.cn

C#:   // 手写回溯递归
来源：http://ua.jctech888.com.cn

[N09] 栈与队列
来源：http://az.hnjuh.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://cm.lnxyls.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://be.muxihuayi.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mq.shtwfgs.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://yq.shtwfgs.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://rh.muxihuayi.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://jf.muxihuayi.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://bl.szxytkj.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hd.hahajie.cn

[N10] 链表节点定义
来源：http://uv.shxzskj.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ba.szsharing.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://vg.bjjhwx.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://rb.jianghongdianzi.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ry.nicolike.cn

Java: class Node { int v; Node next; }
来源：http://ok.gzmigu.cn

Go:   type Node struct { V int; Next *Node }
来源：http://em.jctech888.com.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://fb.bjjhwx.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://cz.haigaiapp.cn

[N11] 二叉树中序遍历
来源：http://ft.nszjky.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://fn.bjjhwx.cn

PHP:  // 手写递归函数
来源：http://my.jctech888.com.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://jj.jianghongdianzi.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ii.chemitech.net.cn

Java: // 手写递归
来源：http://ht.521024.cn

Go:   // 手写递归
来源：http://nv.521024.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://qx.asd995.cn

C#:   // 手写递归
来源：http://ow.panjiajie.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://jj.shxzukj.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ws.panjiajie.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wc.hahajie.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://of.yuexingan06.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://dg.szxytkj.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://to.shxzukj.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://yy.panjiajie.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ga.chemitech.net.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://fi.asd995.cn

================================================================================
来源：http://uc.bjjhwx.cn

O. 并发与异步
来源：http://bx.nicolike.cn

================================================================================
来源：http://ww.newstarts.cn

[O01] 启动一个线程
来源：http://rf.szsharing.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://kt.jianghongdianzi.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ks.szsharing.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://tg.muxihuayi.cn

TS:   // 同 JS
来源：http://sa.newstarts.cn

Java: new Thread(() -> f()).start()
来源：http://pm.bjjhwx.cn

Go:   go f()
来源：http://oo.muxihuayi.cn

Ruby: Thread.new { f }
来源：http://zq.huixinmuqiang.cn

C#:   Task.Run(() => F());
来源：http://as.haigaiapp.cn

[O02] 使用线程池
来源：http://cy.panjiajie.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://xv.szxytkj.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://jb.haigaiapp.cn

JS:   // worker_threads 线程池
来源：http://kq.huixinmuqiang.cn

TS:   // worker_threads 线程池
来源：http://wi.huixiangedu.cn

Java: Executors.newFixedThreadPool(4)
来源：http://zn.huixinmuqiang.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://kf.jianghongdianzi.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://kt.gzmigu.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://vn.haigaiapp.cn

[O03] 加锁保护共享数据
来源：http://if.panjiajie.cn

Py:   with lock: shared += 1
来源：http://fg.shtwfgs.cn

PHP:  // 用 flock() 做文件锁
来源：http://pp.huixinmuqiang.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://fh.muxihuayi.cn

TS:   // 同 JS
来源：http://fn.panjiajie.cn

Java: synchronized (this) { shared++; }
来源：http://he.huanxung.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ii.shtwfgs.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://sm.newstarts.cn

C#:   lock (gate) { shared++; }
来源：http://sv.9csxet.cn

[O04] 定义异步函数并等待
来源：http://xe.shtwfgs.cn

Py:   async def f():⏎    await g()
来源：http://zs.huanxung.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://qh.szsharing.cn

JS:   async function f() { await g(); }
来源：http://vk.huanxung.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://wc.hnjuh.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://oh.nszjky.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://gn.chemitech.net.cn

Ruby: # 用 Fiber 或 async gem
来源：http://rd.yuexingan06.cn

C#:   async Task F() { await G(); }
来源：http://ec.shtwfgs.cn

[O05] 并发执行并等待全部完成
来源：http://lz.nszjky.cn

Py:   asyncio.gather(*tasks)
来源：http://vd.haigaiapp.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://jv.bookmarksfly.cn

JS:   await Promise.all(tasks)
来源：http://ao.lnxyls.cn

TS:   await Promise.all(tasks)
来源：http://iq.chemitech.net.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://um.panjiajie.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://pz.9csxet.cn

Ruby: threads.map(&:join)
来源：http://re.szsharing.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://ib.huixiangedu.cn

[O06] 使用进程池
来源：http://mg.huixiangedu.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://fu.hnjuh.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://cp.9csxet.cn

JS:   // child_process / cluster 模块
来源：http://za.huixiangedu.cn

TS:   // child_process / cluster 模块
来源：http://kx.chemitech.net.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://sq.shxzskj.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mn.yuexingan06.cn

Ruby: // fork 块
来源：http://tx.nicolike.cn

C#:   Parallel.For
来源：http://ey.haigaiapp.cn

================================================================================
来源：http://ei.9csxet.cn

P. 常用工具函数
来源：http://jr.9csxet.cn

================================================================================
来源：http://nn.nicolike.cn

[P01] 生成 UUID
来源：http://rv.hahajie.cn

Py:   str(uuid.uuid4())
来源：http://cq.521024.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ho.wgjwhj.cn

JS:   crypto.randomUUID()
来源：http://dh.yuexingan06.cn

TS:   crypto.randomUUID()
来源：http://jb.newstarts.cn

Java: UUID.randomUUID().toString()
来源：http://bu.haigaiapp.cn

Go:   // 用 github.com/google/uuid
来源：http://qt.shxzukj.cn

Ruby: SecureRandom.uuid
来源：http://cb.huanxung.cn

C#:   Guid.NewGuid().ToString()
来源：http://xp.jianghongdianzi.cn

[P02] MD5 / SHA256 摘要
来源：http://hu.colortex.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://yj.shxzskj.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://bx.nszjky.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ln.haigaiapp.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://zy.nszjky.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://dt.jctech888.com.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://kh.bookmarksfly.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hs.huixiangedu.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://aq.gzmigu.cn

[P03] 生成短随机字符串
来源：http://lc.wgjwhj.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ws.shtwfgs.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ys.jctech888.com.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://os.nicolike.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ba.shxzskj.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ef.shxzukj.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://bt.shxzukj.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://py.chemitech.net.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://gm.bookmarksfly.cn

[P04] 求长度
来源：http://zb.huixiangedu.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://gp.gzmigu.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://pe.chemitech.net.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://te.huixiangedu.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://en.shxzskj.cn

Java: list.size();  map.size();  s.length()
来源：http://cd.huixiangedu.cn

Go:   len(arr);  len(m)
来源：http://dc.gzmigu.cn

Ruby: x.length;  x.size
来源：http://mp.jianghongdianzi.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://ai.shxzskj.cn

[P05] 判断两个对象内容是否相等
来源：http://ry.hahajie.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://iq.bookmarksfly.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wg.lnxyls.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://am.jctech888.com.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://er.shxzukj.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://bz.521024.cn

Go:   reflect.DeepEqual(a, b)
来源：http://ms.gzmigu.cn

Ruby: a == b
来源：http://gj.muxihuayi.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://el.asd995.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://zw.huixiangedu.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://pb.huanxung.cn

PHP:  if (empty($x)) {}
来源：http://ot.shtwfgs.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wa.bjjhwx.cn

TS:   if (x == null) {}
来源：http://pb.haigaiapp.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://zs.bookmarksfly.cn

Go:   if x == nil {}
来源：http://hp.shxzskj.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://pi.shxzukj.cn

C#:   if (x is null) {}
来源：http://pl.nszjky.cn

[P07] 防抖与节流
来源：http://at.chemitech.net.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ng.yuexingan06.cn

PHP:  // 手写时间戳比较
来源：http://bq.bookmarksfly.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://cm.haigaiapp.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hf.shxzskj.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://nq.bjjhwx.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://rw.szxytkj.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://rx.shtwfgs.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://nz.panjiajie.cn

[P08] 处理浮点精度问题
来源：http://qq.wgjwhj.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://vc.nszjky.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ku.9csxet.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://tj.gzmigu.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ct.jianghongdianzi.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://od.huixinmuqiang.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ej.wgjwhj.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://sa.huanxung.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://yd.hahajie.cn

================================================================================
来源：http://pw.chemitech.net.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ad.521024.cn

================================================================================
来源：http://qt.szsharing.cn

[Q01] 创建表
来源：http://gh.chemitech.net.cn

CREATE TABLE users (
来源：http://ri.muxihuayi.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://tb.shxzskj.cn

name VARCHAR(50) NOT NULL,
来源：http://xj.huixinmuqiang.cn

email VARCHAR(100) UNIQUE,
来源：http://ih.huixiangedu.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://xk.521024.cn

);
来源：http://jz.lnxyls.cn

[Q02] 创建带外键的表
来源：http://od.bjjhwx.cn

CREATE TABLE orders (
来源：http://qq.hahajie.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hi.9csxet.cn

user_id INT NOT NULL,
来源：http://pv.szsharing.cn

amount DECIMAL(10, 2),
来源：http://kd.huixiangedu.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://pi.gzmigu.cn

);
来源：http://rh.haigaiapp.cn

[Q03] 增加列
来源：http://iu.shxzukj.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://bj.shxzskj.cn

[Q04] 修改列类型
来源：http://lo.shtwfgs.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hg.newstarts.cn

[Q05] 重命名列
来源：http://zw.yuexingan06.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://kt.9csxet.cn

[Q06] 删除列
来源：http://ez.asd995.cn

ALTER TABLE users DROP COLUMN age;
来源：http://kx.haigaiapp.cn

[Q07] 删除表
来源：http://iy.muxihuayi.cn

DROP TABLE IF EXISTS orders;
来源：http://nd.hahajie.cn

[Q08] 创建普通索引
来源：http://gg.jctech888.com.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://vw.panjiajie.cn

[Q09] 创建唯一索引
来源：http://iv.colortex.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hy.asd995.cn

[Q10] 插入单行
来源：http://dz.hnjuh.cn


<!-- 参考信息 -->