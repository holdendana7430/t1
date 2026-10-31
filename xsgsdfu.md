代发 wailian999

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://to.hahajie.cn

Ruby: warn "err"
来源：http://pp.bookmarksfly.cn

C#:   Console.Error.WriteLine("err")
来源：http://pu.hnjuh.cn

[M07] 判断是否为主入口
来源：http://wm.gzmigu.cn

Py:   if __name__ == "__main__":
来源：http://ya.lnxyls.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ta.shtwfgs.cn

JS:   require.main === module
来源：http://gq.bookmarksfly.cn

TS:   require.main === module
来源：http://gh.jctech888.com.cn

Java: public static void main(String[] args)
来源：http://uk.szsharing.cn

Go:   func main()
来源：http://le.shxzukj.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://aj.hnjuh.cn

C#:   static void Main(string[] args)
来源：http://sl.521024.cn

[M08] 获取系统与运行时信息
来源：http://su.jianghongdianzi.cn

Py:   platform.system();  platform.python_version()
来源：http://qn.shtwfgs.cn

PHP:  PHP_OS;  phpversion();
来源：http://rr.bookmarksfly.cn

JS:   process.platform;  process.version
来源：http://hi.shxzskj.cn

TS:   process.platform;  process.version
来源：http://hs.huanxung.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mn.huanxung.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://fk.newstarts.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hq.huixinmuqiang.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://sq.panjiajie.cn

================================================================================
来源：http://yc.bookmarksfly.cn

N. 数据结构与算法
来源：http://zi.bookmarksfly.cn

================================================================================
来源：http://wi.szxytkj.cn

[N01] 二分查找（有序数组）
来源：http://cv.yuexingan06.cn

Py:   bisect.bisect_left(arr, x)
来源：http://uo.huixiangedu.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://jo.nicolike.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://bp.hahajie.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ir.jianghongdianzi.cn

Java: Arrays.binarySearch(arr, x)
来源：http://kb.wgjwhj.cn

Go:   sort.SearchInts(arr, x)
来源：http://sq.bjjhwx.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://hm.bookmarksfly.cn

C#:   Array.BinarySearch(arr, x)
来源：http://dn.wgjwhj.cn

[N02] 排序（工程实践用内置实现）
来源：http://kg.szsharing.cn

Py:   sorted(arr);  arr.sort()
来源：http://nk.shxzskj.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://qk.shxzukj.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://bk.colortex.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://ke.nszjky.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://xo.yuexingan06.cn

Go:   slices.Sort(arr)
来源：http://rf.chemitech.net.cn

Ruby: arr.sort
来源：http://mg.nszjky.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://zx.shxzukj.cn

[N03] 快速排序（分治示例）
来源：http://qf.gzmigu.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://fa.wgjwhj.cn

PHP:  // 递归实现，或用 usort
来源：http://ui.jctech888.com.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://dz.wgjwhj.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ha.jianghongdianzi.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://zx.nicolike.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://qs.huixinmuqiang.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://uu.jianghongdianzi.cn

C#:   // 手写递归，或 Array.Sort
来源：http://sw.colortex.cn

[N04] 斐波那契数列
来源：http://pa.huixiangedu.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hd.asd995.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://tu.lnxyls.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://og.asd995.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://af.yuntaijiaju.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mq.jianghongdianzi.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://zv.asd995.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://nu.newstarts.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://dz.nszjky.cn

[N05] 最大公约数
来源：http://zp.9csxet.cn

Py:   math.gcd(a, b)
来源：http://xx.nszjky.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://vc.chemitech.net.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://av.wgjwhj.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://zx.asd995.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://bg.huanxung.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://pv.bjjhwx.cn

Ruby: a.gcd(b)
来源：http://jv.gzmigu.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://fm.hahajie.cn

[N06] 判断回文字符串
来源：http://uj.bjjhwx.cn

Py:   s == s[::-1]
来源：http://my.asd995.cn

PHP:  $s === strrev($s);
来源：http://cd.bookmarksfly.cn

JS:   s === [...s].reverse().join("")
来源：http://rw.shxzskj.cn

TS:   s === [...s].reverse().join("")
来源：http://tt.hnjuh.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://jz.shxzukj.cn

Go:   // 双指针从两端比较
来源：http://mp.chemitech.net.cn

Ruby: s == s.reverse
来源：http://ku.shxzukj.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://bp.chemitech.net.cn

[N07] 两数之和（返回下标）
来源：http://oq.chemitech.net.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ds.muxihuayi.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://im.gzmigu.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://wb.521024.cn

TS:   // 手写 Map<string, number>
来源：http://qp.yuexingan06.cn

Java: // 手写 HashMap
来源：http://uf.bookmarksfly.cn

Go:   // 手写 map[int]int
来源：http://cz.chemitech.net.cn

Ruby: // 手写 Hash
来源：http://ls.huixiangedu.cn

C#:   // 手写 Dictionary<int, int>
来源：http://ho.haigaiapp.cn

[N08] 生成全排列
来源：http://sp.bjjhwx.cn

Py:   itertools.permutations(arr)
来源：http://xq.nszjky.cn

PHP:  // 手写递归交换
来源：http://nc.huanxung.cn

JS:   // 手写回溯递归
来源：http://af.yuntaijiaju.cn

TS:   // 手写回溯递归
来源：http://ok.521024.cn

Java: // 手写回溯递归
来源：http://bq.colortex.cn

Go:   // 手写回溯递归
来源：http://xe.nicolike.cn

Ruby: arr.permutation.to_a
来源：http://wt.yuexingan06.cn

C#:   // 手写回溯递归
来源：http://qq.szxytkj.cn

[N09] 栈与队列
来源：http://lt.colortex.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://jx.huanxung.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://jf.bookmarksfly.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ol.yuntaijiaju.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://go.jctech888.com.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://nt.521024.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://fh.jctech888.com.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ph.jctech888.com.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://kj.yuntaijiaju.cn

[N10] 链表节点定义
来源：http://cx.asd995.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://zf.9csxet.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://ma.gzmigu.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://bd.wgjwhj.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://zs.nicolike.cn

Java: class Node { int v; Node next; }
来源：http://js.wgjwhj.cn

Go:   type Node struct { V int; Next *Node }
来源：http://cy.gzmigu.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://us.jctech888.com.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://hd.muxihuayi.cn

[N11] 二叉树中序遍历
来源：http://wu.muxihuayi.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://td.lnxyls.cn

PHP:  // 手写递归函数
来源：http://er.nicolike.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://di.jianghongdianzi.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://kx.newstarts.cn

Java: // 手写递归
来源：http://tb.colortex.cn

Go:   // 手写递归
来源：http://ea.szxytkj.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wo.yuntaijiaju.cn

C#:   // 手写递归
来源：http://gf.asd995.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ij.shxzukj.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://fi.nszjky.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ek.szsharing.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://at.szsharing.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://kt.lnxyls.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://kz.asd995.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://im.chemitech.net.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://df.bjjhwx.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://gr.gzmigu.cn

================================================================================
来源：http://yz.szsharing.cn

O. 并发与异步
来源：http://tc.bjjhwx.cn

================================================================================
来源：http://sk.szsharing.cn

[O01] 启动一个线程
来源：http://ze.jctech888.com.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://im.521024.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://xv.szsharing.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://uc.hahajie.cn

TS:   // 同 JS
来源：http://ow.szsharing.cn

Java: new Thread(() -> f()).start()
来源：http://uf.bjjhwx.cn

Go:   go f()
来源：http://aj.nszjky.cn

Ruby: Thread.new { f }
来源：http://wv.lnxyls.cn

C#:   Task.Run(() => F());
来源：http://ro.gzmigu.cn

[O02] 使用线程池
来源：http://oe.yuntaijiaju.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://fl.nszjky.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://kx.muxihuayi.cn

JS:   // worker_threads 线程池
来源：http://bw.jctech888.com.cn

TS:   // worker_threads 线程池
来源：http://ze.lnxyls.cn

Java: Executors.newFixedThreadPool(4)
来源：http://wn.yuntaijiaju.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://gl.yuexingan06.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://rl.chemitech.net.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://qx.huanxung.cn

[O03] 加锁保护共享数据
来源：http://ie.yuntaijiaju.cn

Py:   with lock: shared += 1
来源：http://lz.hahajie.cn

PHP:  // 用 flock() 做文件锁
来源：http://sv.bookmarksfly.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://dt.nszjky.cn

TS:   // 同 JS
来源：http://ap.panjiajie.cn

Java: synchronized (this) { shared++; }
来源：http://yd.nszjky.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://xf.lnxyls.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://fu.huixiangedu.cn

C#:   lock (gate) { shared++; }
来源：http://xw.asd995.cn

[O04] 定义异步函数并等待
来源：http://qs.nszjky.cn

Py:   async def f():⏎    await g()
来源：http://gj.nszjky.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://cx.hahajie.cn

JS:   async function f() { await g(); }
来源：http://oh.nszjky.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://iw.asd995.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ii.shxzukj.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://en.9csxet.cn

Ruby: # 用 Fiber 或 async gem
来源：http://wv.szsharing.cn

C#:   async Task F() { await G(); }
来源：http://aq.shxzukj.cn

[O05] 并发执行并等待全部完成
来源：http://pl.asd995.cn

Py:   asyncio.gather(*tasks)
来源：http://ga.9csxet.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://to.yuexingan06.cn

JS:   await Promise.all(tasks)
来源：http://zz.9csxet.cn

TS:   await Promise.all(tasks)
来源：http://dm.lnxyls.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wk.shtwfgs.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ho.huixinmuqiang.cn

Ruby: threads.map(&:join)
来源：http://vn.jctech888.com.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://ku.panjiajie.cn

[O06] 使用进程池
来源：http://nc.newstarts.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ly.szxytkj.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://fi.yuntaijiaju.cn

JS:   // child_process / cluster 模块
来源：http://wy.newstarts.cn

TS:   // child_process / cluster 模块
来源：http://tn.9csxet.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://rw.bookmarksfly.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://br.szxytkj.cn

Ruby: // fork 块
来源：http://ry.colortex.cn

C#:   Parallel.For
来源：http://jz.9csxet.cn

================================================================================
来源：http://ky.nszjky.cn

P. 常用工具函数
来源：http://xf.521024.cn

================================================================================
来源：http://nf.haigaiapp.cn

[P01] 生成 UUID
来源：http://rz.yuexingan06.cn

Py:   str(uuid.uuid4())
来源：http://ym.newstarts.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://xv.jianghongdianzi.cn

JS:   crypto.randomUUID()
来源：http://jl.bookmarksfly.cn

TS:   crypto.randomUUID()
来源：http://cc.newstarts.cn

Java: UUID.randomUUID().toString()
来源：http://vk.hnjuh.cn

Go:   // 用 github.com/google/uuid
来源：http://hd.szsharing.cn

Ruby: SecureRandom.uuid
来源：http://bk.newstarts.cn

C#:   Guid.NewGuid().ToString()
来源：http://sz.hahajie.cn

[P02] MD5 / SHA256 摘要
来源：http://eb.bookmarksfly.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://oi.yuexingan06.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://pr.huixinmuqiang.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ds.nszjky.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://gt.shtwfgs.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://qq.nicolike.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ck.521024.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://nj.wgjwhj.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://rq.szxytkj.cn

[P03] 生成短随机字符串
来源：http://hf.hnjuh.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ee.shtwfgs.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://gs.muxihuayi.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wz.521024.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://kh.szsharing.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://bg.shxzukj.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://xr.bookmarksfly.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://eg.lnxyls.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ki.hahajie.cn

[P04] 求长度
来源：http://kt.bookmarksfly.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ds.jianghongdianzi.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://bp.huixiangedu.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://qd.bjjhwx.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://rm.huanxung.cn

Java: list.size();  map.size();  s.length()
来源：http://rv.asd995.cn

Go:   len(arr);  len(m)
来源：http://yj.panjiajie.cn

Ruby: x.length;  x.size
来源：http://eu.nicolike.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://lo.huanxung.cn

[P05] 判断两个对象内容是否相等
来源：http://lw.nicolike.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://td.9csxet.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wy.521024.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://qp.gzmigu.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://fs.panjiajie.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wr.huanxung.cn

Go:   reflect.DeepEqual(a, b)
来源：http://yr.asd995.cn

Ruby: a == b
来源：http://cl.shtwfgs.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wp.chemitech.net.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://un.chemitech.net.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://vn.hahajie.cn

PHP:  if (empty($x)) {}
来源：http://wo.hahajie.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://fw.szsharing.cn

TS:   if (x == null) {}
来源：http://zu.szsharing.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://kw.panjiajie.cn

Go:   if x == nil {}
来源：http://qx.haigaiapp.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://rp.521024.cn

C#:   if (x is null) {}
来源：http://ok.szxytkj.cn

[P07] 防抖与节流
来源：http://sk.yuntaijiaju.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://zc.colortex.cn

PHP:  // 手写时间戳比较
来源：http://au.yuexingan06.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://br.hahajie.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ch.jctech888.com.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://zm.huixinmuqiang.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://uz.lnxyls.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://ap.jctech888.com.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ng.yuntaijiaju.cn

[P08] 处理浮点精度问题
来源：http://rr.jctech888.com.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://yf.haigaiapp.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ni.hahajie.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wm.jianghongdianzi.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wf.panjiajie.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://yf.huanxung.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://nr.nicolike.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://da.haigaiapp.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://sh.bookmarksfly.cn

================================================================================
来源：http://ed.newstarts.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://fo.jctech888.com.cn

================================================================================
来源：http://ha.bjjhwx.cn

[Q01] 创建表
来源：http://gh.shtwfgs.cn

CREATE TABLE users (
来源：http://uo.nicolike.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ml.huixiangedu.cn

name VARCHAR(50) NOT NULL,
来源：http://et.huixiangedu.cn

email VARCHAR(100) UNIQUE,
来源：http://fd.newstarts.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://oh.yuntaijiaju.cn

);
来源：http://zo.nicolike.cn

[Q02] 创建带外键的表
来源：http://ks.jctech888.com.cn

CREATE TABLE orders (
来源：http://un.hnjuh.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://vv.colortex.cn

user_id INT NOT NULL,
来源：http://xa.yuexingan06.cn

amount DECIMAL(10, 2),
来源：http://qb.521024.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://dm.newstarts.cn

);
来源：http://ub.yuntaijiaju.cn

[Q03] 增加列
来源：http://of.huixinmuqiang.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://fe.bookmarksfly.cn

[Q04] 修改列类型
来源：http://yo.haigaiapp.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://vu.shxzskj.cn

[Q05] 重命名列
来源：http://om.bjjhwx.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://bz.asd995.cn

[Q06] 删除列
来源：http://oh.huixiangedu.cn

ALTER TABLE users DROP COLUMN age;
来源：http://jj.asd995.cn

[Q07] 删除表
来源：http://yz.shxzukj.cn

DROP TABLE IF EXISTS orders;
来源：http://yr.521024.cn

[Q08] 创建普通索引
来源：http://tn.gzmigu.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://lf.huanxung.cn

[Q09] 创建唯一索引
来源：http://vy.hahajie.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://tk.huixinmuqiang.cn

[Q10] 插入单行
来源：http://ub.9csxet.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hp.nszjky.cn

[Q11] 一次插入多行
来源：http://ks.shtwfgs.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://dv.asd995.cn

[Q12] 插入后取自增 ID
来源：http://sj.521024.cn


<!-- 参考信息 -->