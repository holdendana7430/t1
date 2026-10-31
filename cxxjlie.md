代发 wailian999

PHP:  fwrite(STDERR, "err\n");
来源：http://ie.gzmigu.cn

JS:   console.error("err")
来源：http://iz.shxzukj.cn

TS:   console.error("err")
来源：http://mr.huixiangedu.cn

Java: System.err.println("err")
来源：http://ab.huixiangedu.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://iw.bjjhwx.cn

Ruby: warn "err"
来源：http://ds.shtwfgs.cn

C#:   Console.Error.WriteLine("err")
来源：http://wk.wgjwhj.cn

[M07] 判断是否为主入口
来源：http://tx.asd995.cn

Py:   if __name__ == "__main__":
来源：http://tl.szxytkj.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ej.panjiajie.cn

JS:   require.main === module
来源：http://nf.jianghongdianzi.cn

TS:   require.main === module
来源：http://aj.huixinmuqiang.cn

Java: public static void main(String[] args)
来源：http://ly.shtwfgs.cn

Go:   func main()
来源：http://ei.shxzskj.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://se.huixiangedu.cn

C#:   static void Main(string[] args)
来源：http://sh.huixinmuqiang.cn

[M08] 获取系统与运行时信息
来源：http://hm.nszjky.cn

Py:   platform.system();  platform.python_version()
来源：http://va.hnjuh.cn

PHP:  PHP_OS;  phpversion();
来源：http://bk.lnxyls.cn

JS:   process.platform;  process.version
来源：http://bh.szsharing.cn

TS:   process.platform;  process.version
来源：http://um.huanxung.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hy.jianghongdianzi.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://im.huanxung.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://xu.521024.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://gw.hahajie.cn

================================================================================
来源：http://xv.haigaiapp.cn

N. 数据结构与算法
来源：http://ip.szsharing.cn

================================================================================
来源：http://dz.shxzukj.cn

[N01] 二分查找（有序数组）
来源：http://ou.9csxet.cn

Py:   bisect.bisect_left(arr, x)
来源：http://sy.huixiangedu.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ed.nszjky.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://gt.szxytkj.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://gb.hnjuh.cn

Java: Arrays.binarySearch(arr, x)
来源：http://rm.chemitech.net.cn

Go:   sort.SearchInts(arr, x)
来源：http://ts.yuntaijiaju.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://fk.nszjky.cn

C#:   Array.BinarySearch(arr, x)
来源：http://nf.nszjky.cn

[N02] 排序（工程实践用内置实现）
来源：http://iv.jianghongdianzi.cn

Py:   sorted(arr);  arr.sort()
来源：http://nn.hahajie.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://eu.9csxet.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://we.hnjuh.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://wg.panjiajie.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://jt.521024.cn

Go:   slices.Sort(arr)
来源：http://ec.muxihuayi.cn

Ruby: arr.sort
来源：http://gj.szsharing.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://bi.chemitech.net.cn

[N03] 快速排序（分治示例）
来源：http://ni.panjiajie.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://tw.colortex.cn

PHP:  // 递归实现，或用 usort
来源：http://cr.hahajie.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://fr.newstarts.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://cq.lnxyls.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://fg.newstarts.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://xm.huixinmuqiang.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ox.chemitech.net.cn

C#:   // 手写递归，或 Array.Sort
来源：http://qz.gzmigu.cn

[N04] 斐波那契数列
来源：http://pk.muxihuayi.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://xd.szsharing.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://vl.shxzukj.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://we.9csxet.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://np.bookmarksfly.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://jy.haigaiapp.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ho.gzmigu.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://aj.asd995.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ux.shxzukj.cn

[N05] 最大公约数
来源：http://vm.bjjhwx.cn

Py:   math.gcd(a, b)
来源：http://qs.panjiajie.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ep.chemitech.net.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://jn.bookmarksfly.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://cm.bjjhwx.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://zz.yuexingan06.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ql.asd995.cn

Ruby: a.gcd(b)
来源：http://ag.szxytkj.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://us.yuntaijiaju.cn

[N06] 判断回文字符串
来源：http://ji.521024.cn

Py:   s == s[::-1]
来源：http://no.chemitech.net.cn

PHP:  $s === strrev($s);
来源：http://tb.haigaiapp.cn

JS:   s === [...s].reverse().join("")
来源：http://yf.521024.cn

TS:   s === [...s].reverse().join("")
来源：http://fv.bookmarksfly.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://xd.yuntaijiaju.cn

Go:   // 双指针从两端比较
来源：http://by.chemitech.net.cn

Ruby: s == s.reverse
来源：http://uy.huanxung.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://vr.yuexingan06.cn

[N07] 两数之和（返回下标）
来源：http://ap.nicolike.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://yl.chemitech.net.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://zd.panjiajie.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://cw.asd995.cn

TS:   // 手写 Map<string, number>
来源：http://wo.yuexingan06.cn

Java: // 手写 HashMap
来源：http://cj.huixinmuqiang.cn

Go:   // 手写 map[int]int
来源：http://yg.hahajie.cn

Ruby: // 手写 Hash
来源：http://hl.hnjuh.cn

C#:   // 手写 Dictionary<int, int>
来源：http://ly.gzmigu.cn

[N08] 生成全排列
来源：http://ej.chemitech.net.cn

Py:   itertools.permutations(arr)
来源：http://zu.hnjuh.cn

PHP:  // 手写递归交换
来源：http://bv.lnxyls.cn

JS:   // 手写回溯递归
来源：http://vu.jianghongdianzi.cn

TS:   // 手写回溯递归
来源：http://uv.nszjky.cn

Java: // 手写回溯递归
来源：http://ei.hahajie.cn

Go:   // 手写回溯递归
来源：http://su.521024.cn

Ruby: arr.permutation.to_a
来源：http://do.hnjuh.cn

C#:   // 手写回溯递归
来源：http://ii.shxzskj.cn

[N09] 栈与队列
来源：http://xv.huanxung.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wt.shtwfgs.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://kn.huixinmuqiang.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://kt.wgjwhj.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://if.jctech888.com.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ef.hahajie.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://tt.shxzskj.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ii.shxzukj.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ef.lnxyls.cn

[N10] 链表节点定义
来源：http://hb.newstarts.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ox.haigaiapp.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://is.shxzukj.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://io.lnxyls.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://lc.muxihuayi.cn

Java: class Node { int v; Node next; }
来源：http://zb.nszjky.cn

Go:   type Node struct { V int; Next *Node }
来源：http://uf.521024.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://hv.colortex.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://ys.yuntaijiaju.cn

[N11] 二叉树中序遍历
来源：http://gc.chemitech.net.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://dk.asd995.cn

PHP:  // 手写递归函数
来源：http://gv.chemitech.net.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://yq.colortex.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://pc.yuntaijiaju.cn

Java: // 手写递归
来源：http://it.nicolike.cn

Go:   // 手写递归
来源：http://al.wgjwhj.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://al.chemitech.net.cn

C#:   // 手写递归
来源：http://pk.asd995.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://xg.nszjky.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ls.panjiajie.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://gk.chemitech.net.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://eq.jctech888.com.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://xy.nszjky.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hj.jianghongdianzi.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://yu.hahajie.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://up.colortex.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://tr.colortex.cn

================================================================================
来源：http://ih.muxihuayi.cn

O. 并发与异步
来源：http://kq.bookmarksfly.cn

================================================================================
来源：http://tv.nszjky.cn

[O01] 启动一个线程
来源：http://na.chemitech.net.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://tf.huanxung.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://jo.jianghongdianzi.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://cw.gzmigu.cn

TS:   // 同 JS
来源：http://pm.bookmarksfly.cn

Java: new Thread(() -> f()).start()
来源：http://rr.haigaiapp.cn

Go:   go f()
来源：http://jw.huixinmuqiang.cn

Ruby: Thread.new { f }
来源：http://ll.nicolike.cn

C#:   Task.Run(() => F());
来源：http://we.jctech888.com.cn

[O02] 使用线程池
来源：http://pe.bjjhwx.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://lj.nszjky.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hp.9csxet.cn

JS:   // worker_threads 线程池
来源：http://ej.szsharing.cn

TS:   // worker_threads 线程池
来源：http://fy.gzmigu.cn

Java: Executors.newFixedThreadPool(4)
来源：http://nf.jianghongdianzi.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ti.yuexingan06.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://qb.lnxyls.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://gv.hnjuh.cn

[O03] 加锁保护共享数据
来源：http://ne.nicolike.cn

Py:   with lock: shared += 1
来源：http://ut.szxytkj.cn

PHP:  // 用 flock() 做文件锁
来源：http://dg.nicolike.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://lo.haigaiapp.cn

TS:   // 同 JS
来源：http://th.wgjwhj.cn

Java: synchronized (this) { shared++; }
来源：http://es.huixiangedu.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ys.nszjky.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://vp.hnjuh.cn

C#:   lock (gate) { shared++; }
来源：http://yj.yuexingan06.cn

[O04] 定义异步函数并等待
来源：http://dt.jctech888.com.cn

Py:   async def f():⏎    await g()
来源：http://xg.shtwfgs.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://cm.szsharing.cn

JS:   async function f() { await g(); }
来源：http://xx.hnjuh.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://ht.haigaiapp.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ps.chemitech.net.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://cx.jctech888.com.cn

Ruby: # 用 Fiber 或 async gem
来源：http://nu.lnxyls.cn

C#:   async Task F() { await G(); }
来源：http://ld.huixinmuqiang.cn

[O05] 并发执行并等待全部完成
来源：http://vz.bookmarksfly.cn

Py:   asyncio.gather(*tasks)
来源：http://jn.bjjhwx.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://or.huixiangedu.cn

JS:   await Promise.all(tasks)
来源：http://al.lnxyls.cn

TS:   await Promise.all(tasks)
来源：http://un.nicolike.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://xg.chemitech.net.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://gw.gzmigu.cn

Ruby: threads.map(&:join)
来源：http://ql.yuexingan06.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://iz.yuexingan06.cn

[O06] 使用进程池
来源：http://zb.huanxung.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ue.jianghongdianzi.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://yc.muxihuayi.cn

JS:   // child_process / cluster 模块
来源：http://bv.gzmigu.cn

TS:   // child_process / cluster 模块
来源：http://vf.bjjhwx.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ih.bookmarksfly.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://yq.shxzukj.cn

Ruby: // fork 块
来源：http://du.huixinmuqiang.cn

C#:   Parallel.For
来源：http://ph.chemitech.net.cn

================================================================================
来源：http://my.asd995.cn

P. 常用工具函数
来源：http://lh.jianghongdianzi.cn

================================================================================
来源：http://xk.hahajie.cn

[P01] 生成 UUID
来源：http://hl.nszjky.cn

Py:   str(uuid.uuid4())
来源：http://ce.newstarts.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://va.yuntaijiaju.cn

JS:   crypto.randomUUID()
来源：http://td.bookmarksfly.cn

TS:   crypto.randomUUID()
来源：http://wq.hnjuh.cn

Java: UUID.randomUUID().toString()
来源：http://tz.huixinmuqiang.cn

Go:   // 用 github.com/google/uuid
来源：http://hy.huixinmuqiang.cn

Ruby: SecureRandom.uuid
来源：http://lr.szsharing.cn

C#:   Guid.NewGuid().ToString()
来源：http://tq.9csxet.cn

[P02] MD5 / SHA256 摘要
来源：http://bv.9csxet.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://vc.hnjuh.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://uw.haigaiapp.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://vl.haigaiapp.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://qn.lnxyls.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wn.muxihuayi.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://le.chemitech.net.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://eo.huixinmuqiang.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://gu.9csxet.cn

[P03] 生成短随机字符串
来源：http://jz.shxzskj.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hs.nicolike.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://rr.nszjky.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://um.szsharing.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ql.hnjuh.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ty.bjjhwx.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wu.nicolike.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://dt.jctech888.com.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://dh.nszjky.cn

[P04] 求长度
来源：http://qg.panjiajie.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://dg.bookmarksfly.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ot.bookmarksfly.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://fd.huixinmuqiang.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://zf.jianghongdianzi.cn

Java: list.size();  map.size();  s.length()
来源：http://de.nicolike.cn

Go:   len(arr);  len(m)
来源：http://mo.muxihuayi.cn

Ruby: x.length;  x.size
来源：http://ml.hnjuh.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://kl.yuntaijiaju.cn

[P05] 判断两个对象内容是否相等
来源：http://nk.szxytkj.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://ub.yuexingan06.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://fs.bookmarksfly.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://un.bjjhwx.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ja.shtwfgs.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://at.huixinmuqiang.cn

Go:   reflect.DeepEqual(a, b)
来源：http://aa.nicolike.cn

Ruby: a == b
来源：http://ff.huixiangedu.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://an.jctech888.com.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://pg.panjiajie.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ev.asd995.cn

PHP:  if (empty($x)) {}
来源：http://yz.9csxet.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://sv.colortex.cn

TS:   if (x == null) {}
来源：http://pk.panjiajie.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://ch.huanxung.cn

Go:   if x == nil {}
来源：http://um.huanxung.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hg.colortex.cn

C#:   if (x is null) {}
来源：http://hx.hahajie.cn

[P07] 防抖与节流
来源：http://xv.shxzskj.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://qb.9csxet.cn

PHP:  // 手写时间戳比较
来源：http://dk.colortex.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ib.nicolike.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://in.huixiangedu.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://xk.huixiangedu.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://cd.asd995.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://oy.wgjwhj.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://zw.nicolike.cn

[P08] 处理浮点精度问题
来源：http://xr.haigaiapp.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://qn.shtwfgs.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://fl.gzmigu.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://vp.521024.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://dc.jctech888.com.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://as.bookmarksfly.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://qa.asd995.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://fk.jctech888.com.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://xg.lnxyls.cn

================================================================================
来源：http://ip.nszjky.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://lr.szxytkj.cn

================================================================================
来源：http://ja.yuntaijiaju.cn

[Q01] 创建表
来源：http://aw.shtwfgs.cn

CREATE TABLE users (
来源：http://ix.shtwfgs.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://bz.gzmigu.cn

name VARCHAR(50) NOT NULL,
来源：http://bb.lnxyls.cn

email VARCHAR(100) UNIQUE,
来源：http://fe.colortex.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://rw.nszjky.cn

);
来源：http://sz.shxzskj.cn

[Q02] 创建带外键的表
来源：http://xy.muxihuayi.cn

CREATE TABLE orders (
来源：http://ao.lnxyls.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://nz.asd995.cn

user_id INT NOT NULL,
来源：http://sl.muxihuayi.cn

amount DECIMAL(10, 2),
来源：http://ii.bookmarksfly.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://lo.szsharing.cn

);
来源：http://ss.wgjwhj.cn

[Q03] 增加列
来源：http://do.yuntaijiaju.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hb.bjjhwx.cn

[Q04] 修改列类型
来源：http://ot.jctech888.com.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://rk.asd995.cn

[Q05] 重命名列
来源：http://qn.521024.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://jt.shtwfgs.cn

[Q06] 删除列
来源：http://kv.shxzukj.cn

ALTER TABLE users DROP COLUMN age;
来源：http://ui.haigaiapp.cn

[Q07] 删除表
来源：http://or.asd995.cn

DROP TABLE IF EXISTS orders;
来源：http://qo.nicolike.cn

[Q08] 创建普通索引
来源：http://xx.hahajie.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://og.szxytkj.cn

[Q09] 创建唯一索引
来源：http://bb.yuexingan06.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wy.huanxung.cn

[Q10] 插入单行
来源：http://qo.newstarts.cn


<!-- 参考信息 -->