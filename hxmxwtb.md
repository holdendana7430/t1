代发 wailian999

PHP:  fwrite(STDERR, "err\n");
来源：http://on.jianghongdianzi.cn

JS:   console.error("err")
来源：http://yj.haigaiapp.cn

TS:   console.error("err")
来源：http://hq.shtwfgs.cn

Java: System.err.println("err")
来源：http://yh.nicolike.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hk.haigaiapp.cn

Ruby: warn "err"
来源：http://ah.9csxet.cn

C#:   Console.Error.WriteLine("err")
来源：http://yg.yuexingan06.cn

[M07] 判断是否为主入口
来源：http://dk.colortex.cn

Py:   if __name__ == "__main__":
来源：http://er.colortex.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ml.jianghongdianzi.cn

JS:   require.main === module
来源：http://yh.bookmarksfly.cn

TS:   require.main === module
来源：http://il.huanxung.cn

Java: public static void main(String[] args)
来源：http://gn.gzmigu.cn

Go:   func main()
来源：http://nr.huanxung.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://fd.jctech888.com.cn

C#:   static void Main(string[] args)
来源：http://is.newstarts.cn

[M08] 获取系统与运行时信息
来源：http://ta.muxihuayi.cn

Py:   platform.system();  platform.python_version()
来源：http://em.muxihuayi.cn

PHP:  PHP_OS;  phpversion();
来源：http://km.chemitech.net.cn

JS:   process.platform;  process.version
来源：http://jn.shxzskj.cn

TS:   process.platform;  process.version
来源：http://ji.panjiajie.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ez.lnxyls.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://uk.jctech888.com.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://nk.shxzskj.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://se.yuntaijiaju.cn

================================================================================
来源：http://kr.nszjky.cn

N. 数据结构与算法
来源：http://zf.huixiangedu.cn

================================================================================
来源：http://zx.gzmigu.cn

[N01] 二分查找（有序数组）
来源：http://sb.yuntaijiaju.cn

Py:   bisect.bisect_left(arr, x)
来源：http://mz.chemitech.net.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://gl.haigaiapp.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://gc.bjjhwx.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://fc.jctech888.com.cn

Java: Arrays.binarySearch(arr, x)
来源：http://yu.huixinmuqiang.cn

Go:   sort.SearchInts(arr, x)
来源：http://cw.szsharing.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://kj.wgjwhj.cn

C#:   Array.BinarySearch(arr, x)
来源：http://av.wgjwhj.cn

[N02] 排序（工程实践用内置实现）
来源：http://ad.haigaiapp.cn

Py:   sorted(arr);  arr.sort()
来源：http://no.9csxet.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://py.521024.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://ct.lnxyls.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://sv.szxytkj.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://dp.nicolike.cn

Go:   slices.Sort(arr)
来源：http://ob.jctech888.com.cn

Ruby: arr.sort
来源：http://qt.colortex.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://st.huixinmuqiang.cn

[N03] 快速排序（分治示例）
来源：http://ow.panjiajie.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://il.panjiajie.cn

PHP:  // 递归实现，或用 usort
来源：http://vk.szsharing.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://vi.haigaiapp.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ma.521024.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://rj.yuntaijiaju.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://oi.shxzskj.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ma.9csxet.cn

C#:   // 手写递归，或 Array.Sort
来源：http://ud.wgjwhj.cn

[N04] 斐波那契数列
来源：http://oo.panjiajie.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://cs.huixinmuqiang.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://df.panjiajie.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://kr.huanxung.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wq.nszjky.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://yr.wgjwhj.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://dr.lnxyls.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://nu.yuntaijiaju.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://au.bookmarksfly.cn

[N05] 最大公约数
来源：http://gy.muxihuayi.cn

Py:   math.gcd(a, b)
来源：http://is.huixiangedu.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ew.colortex.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://uv.yuexingan06.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://uc.chemitech.net.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://rx.shtwfgs.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://zr.szxytkj.cn

Ruby: a.gcd(b)
来源：http://bt.jianghongdianzi.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://kb.shtwfgs.cn

[N06] 判断回文字符串
来源：http://pu.huixinmuqiang.cn

Py:   s == s[::-1]
来源：http://fk.newstarts.cn

PHP:  $s === strrev($s);
来源：http://qu.nicolike.cn

JS:   s === [...s].reverse().join("")
来源：http://ms.chemitech.net.cn

TS:   s === [...s].reverse().join("")
来源：http://tr.shxzskj.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://dy.yuexingan06.cn

Go:   // 双指针从两端比较
来源：http://ja.huixinmuqiang.cn

Ruby: s == s.reverse
来源：http://js.huanxung.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://vm.9csxet.cn

[N07] 两数之和（返回下标）
来源：http://id.hahajie.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://jr.hnjuh.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ev.yuntaijiaju.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://fs.shxzukj.cn

TS:   // 手写 Map<string, number>
来源：http://po.panjiajie.cn

Java: // 手写 HashMap
来源：http://wy.huixiangedu.cn

Go:   // 手写 map[int]int
来源：http://mv.shxzukj.cn

Ruby: // 手写 Hash
来源：http://co.hahajie.cn

C#:   // 手写 Dictionary<int, int>
来源：http://ut.colortex.cn

[N08] 生成全排列
来源：http://gr.hahajie.cn

Py:   itertools.permutations(arr)
来源：http://sg.asd995.cn

PHP:  // 手写递归交换
来源：http://av.lnxyls.cn

JS:   // 手写回溯递归
来源：http://wu.yuexingan06.cn

TS:   // 手写回溯递归
来源：http://xm.huixiangedu.cn

Java: // 手写回溯递归
来源：http://rf.bookmarksfly.cn

Go:   // 手写回溯递归
来源：http://qo.panjiajie.cn

Ruby: arr.permutation.to_a
来源：http://kk.muxihuayi.cn

C#:   // 手写回溯递归
来源：http://cx.hnjuh.cn

[N09] 栈与队列
来源：http://sc.huanxung.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://tu.szsharing.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://cp.bookmarksfly.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://le.muxihuayi.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://da.huanxung.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://xs.panjiajie.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://qq.yuntaijiaju.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ep.szxytkj.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://lx.nszjky.cn

[N10] 链表节点定义
来源：http://uk.nszjky.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://pd.bjjhwx.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://qu.nszjky.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://le.jctech888.com.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ke.wgjwhj.cn

Java: class Node { int v; Node next; }
来源：http://pb.bjjhwx.cn

Go:   type Node struct { V int; Next *Node }
来源：http://ft.colortex.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://ji.muxihuayi.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://pc.nicolike.cn

[N11] 二叉树中序遍历
来源：http://nt.chemitech.net.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://uy.wgjwhj.cn

PHP:  // 手写递归函数
来源：http://dw.hahajie.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://da.shtwfgs.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://rf.chemitech.net.cn

Java: // 手写递归
来源：http://rx.shxzukj.cn

Go:   // 手写递归
来源：http://yz.asd995.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hj.bookmarksfly.cn

C#:   // 手写递归
来源：http://xm.colortex.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ba.szsharing.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://cn.9csxet.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ae.huixinmuqiang.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ta.chemitech.net.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wb.shxzukj.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://up.gzmigu.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://qu.huixinmuqiang.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ay.yuexingan06.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ku.bookmarksfly.cn

================================================================================
来源：http://dm.hnjuh.cn

O. 并发与异步
来源：http://jf.huanxung.cn

================================================================================
来源：http://ix.huixiangedu.cn

[O01] 启动一个线程
来源：http://mz.jctech888.com.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://uv.hnjuh.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://bo.panjiajie.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://dz.huixinmuqiang.cn

TS:   // 同 JS
来源：http://fl.muxihuayi.cn

Java: new Thread(() -> f()).start()
来源：http://me.9csxet.cn

Go:   go f()
来源：http://li.shtwfgs.cn

Ruby: Thread.new { f }
来源：http://xi.colortex.cn

C#:   Task.Run(() => F());
来源：http://tc.szsharing.cn

[O02] 使用线程池
来源：http://fg.huanxung.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://yr.9csxet.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://qk.nszjky.cn

JS:   // worker_threads 线程池
来源：http://pt.panjiajie.cn

TS:   // worker_threads 线程池
来源：http://jd.lnxyls.cn

Java: Executors.newFixedThreadPool(4)
来源：http://ig.hahajie.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://nl.lnxyls.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://kr.haigaiapp.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wr.wgjwhj.cn

[O03] 加锁保护共享数据
来源：http://db.shtwfgs.cn

Py:   with lock: shared += 1
来源：http://np.huixiangedu.cn

PHP:  // 用 flock() 做文件锁
来源：http://hb.jianghongdianzi.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://rh.9csxet.cn

TS:   // 同 JS
来源：http://oi.shxzukj.cn

Java: synchronized (this) { shared++; }
来源：http://ei.bookmarksfly.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ij.hahajie.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://tv.muxihuayi.cn

C#:   lock (gate) { shared++; }
来源：http://jh.nicolike.cn

[O04] 定义异步函数并等待
来源：http://bp.colortex.cn

Py:   async def f():⏎    await g()
来源：http://pf.jianghongdianzi.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ws.hnjuh.cn

JS:   async function f() { await g(); }
来源：http://er.gzmigu.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://yw.wgjwhj.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://zw.shtwfgs.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://xr.huixinmuqiang.cn

Ruby: # 用 Fiber 或 async gem
来源：http://hv.hahajie.cn

C#:   async Task F() { await G(); }
来源：http://ag.hahajie.cn

[O05] 并发执行并等待全部完成
来源：http://uq.asd995.cn

Py:   asyncio.gather(*tasks)
来源：http://nd.huixiangedu.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://pa.chemitech.net.cn

JS:   await Promise.all(tasks)
来源：http://px.shxzukj.cn

TS:   await Promise.all(tasks)
来源：http://pt.asd995.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ft.9csxet.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://um.hahajie.cn

Ruby: threads.map(&:join)
来源：http://ld.521024.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://ke.szxytkj.cn

[O06] 使用进程池
来源：http://qj.colortex.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ul.nicolike.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://zu.yuexingan06.cn

JS:   // child_process / cluster 模块
来源：http://po.521024.cn

TS:   // child_process / cluster 模块
来源：http://wb.bookmarksfly.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ic.gzmigu.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ac.colortex.cn

Ruby: // fork 块
来源：http://ur.bookmarksfly.cn

C#:   Parallel.For
来源：http://cd.nicolike.cn

================================================================================
来源：http://tu.hnjuh.cn

P. 常用工具函数
来源：http://zr.hahajie.cn

================================================================================
来源：http://ub.nszjky.cn

[P01] 生成 UUID
来源：http://ed.shxzskj.cn

Py:   str(uuid.uuid4())
来源：http://ei.yuntaijiaju.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://oy.newstarts.cn

JS:   crypto.randomUUID()
来源：http://gg.hnjuh.cn

TS:   crypto.randomUUID()
来源：http://fb.chemitech.net.cn

Java: UUID.randomUUID().toString()
来源：http://gt.jctech888.com.cn

Go:   // 用 github.com/google/uuid
来源：http://xx.jctech888.com.cn

Ruby: SecureRandom.uuid
来源：http://zv.9csxet.cn

C#:   Guid.NewGuid().ToString()
来源：http://fa.yuexingan06.cn

[P02] MD5 / SHA256 摘要
来源：http://ms.szxytkj.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ab.521024.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://tl.jianghongdianzi.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ik.shtwfgs.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://zb.gzmigu.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ft.wgjwhj.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wu.9csxet.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://nq.newstarts.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://lz.shxzukj.cn

[P03] 生成短随机字符串
来源：http://il.bjjhwx.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ws.wgjwhj.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://go.shxzskj.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://fz.nicolike.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://yx.lnxyls.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mj.colortex.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://uw.nicolike.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://ea.szxytkj.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ef.yuexingan06.cn

[P04] 求长度
来源：http://vx.shxzukj.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ov.hahajie.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mk.shxzukj.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://he.nszjky.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://jl.nszjky.cn

Java: list.size();  map.size();  s.length()
来源：http://xu.chemitech.net.cn

Go:   len(arr);  len(m)
来源：http://ga.nszjky.cn

Ruby: x.length;  x.size
来源：http://we.haigaiapp.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://sr.colortex.cn

[P05] 判断两个对象内容是否相等
来源：http://gt.haigaiapp.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://sw.521024.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ke.wgjwhj.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://eg.bjjhwx.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://bw.lnxyls.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ma.haigaiapp.cn

Go:   reflect.DeepEqual(a, b)
来源：http://bm.nicolike.cn

Ruby: a == b
来源：http://lf.wgjwhj.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ri.szxytkj.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://km.gzmigu.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://nd.wgjwhj.cn

PHP:  if (empty($x)) {}
来源：http://lh.wgjwhj.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://es.bjjhwx.cn

TS:   if (x == null) {}
来源：http://ra.huixinmuqiang.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://ub.521024.cn

Go:   if x == nil {}
来源：http://li.9csxet.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://yc.szxytkj.cn

C#:   if (x is null) {}
来源：http://hb.asd995.cn

[P07] 防抖与节流
来源：http://ns.shtwfgs.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://cj.shxzukj.cn

PHP:  // 手写时间戳比较
来源：http://xp.newstarts.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://gl.yuntaijiaju.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://nm.jianghongdianzi.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://vm.muxihuayi.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://pp.shxzskj.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://nk.colortex.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://zp.hahajie.cn

[P08] 处理浮点精度问题
来源：http://qt.nszjky.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://xr.colortex.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ks.shxzukj.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://vt.panjiajie.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://dr.bjjhwx.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://lf.yuexingan06.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mx.lnxyls.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://fr.yuntaijiaju.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://uf.nszjky.cn

================================================================================
来源：http://ez.panjiajie.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://nd.colortex.cn

================================================================================
来源：http://ik.colortex.cn

[Q01] 创建表
来源：http://ts.colortex.cn

CREATE TABLE users (
来源：http://jx.521024.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://qq.szxytkj.cn

name VARCHAR(50) NOT NULL,
来源：http://xu.huanxung.cn

email VARCHAR(100) UNIQUE,
来源：http://ie.gzmigu.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://df.gzmigu.cn

);
来源：http://py.huixiangedu.cn

[Q02] 创建带外键的表
来源：http://kk.szxytkj.cn

CREATE TABLE orders (
来源：http://ec.hnjuh.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://vs.521024.cn

user_id INT NOT NULL,
来源：http://ww.bookmarksfly.cn

amount DECIMAL(10, 2),
来源：http://dm.haigaiapp.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://zs.huixiangedu.cn

);
来源：http://ph.lnxyls.cn

[Q03] 增加列
来源：http://vg.colortex.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ut.hnjuh.cn

[Q04] 修改列类型
来源：http://yh.huixiangedu.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://vh.newstarts.cn

[Q05] 重命名列
来源：http://tm.521024.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://di.lnxyls.cn

[Q06] 删除列
来源：http://rk.yuntaijiaju.cn

ALTER TABLE users DROP COLUMN age;
来源：http://th.huixinmuqiang.cn

[Q07] 删除表
来源：http://bi.chemitech.net.cn

DROP TABLE IF EXISTS orders;
来源：http://az.panjiajie.cn

[Q08] 创建普通索引
来源：http://kc.shtwfgs.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://qk.haigaiapp.cn

[Q09] 创建唯一索引
来源：http://yn.muxihuayi.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ns.wgjwhj.cn

[Q10] 插入单行
来源：http://mv.muxihuayi.cn


<!-- 参考信息 -->