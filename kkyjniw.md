代发 wailian999

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://er.hahajie.cn

Ruby: warn "err"
来源：http://zp.nszjky.cn

C#:   Console.Error.WriteLine("err")
来源：http://iz.9csxet.cn

[M07] 判断是否为主入口
来源：http://dd.9csxet.cn

Py:   if __name__ == "__main__":
来源：http://vm.szxytkj.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://jw.bjjhwx.cn

JS:   require.main === module
来源：http://ef.jctech888.com.cn

TS:   require.main === module
来源：http://ml.huanxung.cn

Java: public static void main(String[] args)
来源：http://fw.haigaiapp.cn

Go:   func main()
来源：http://mb.yuntaijiaju.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://pm.huanxung.cn

C#:   static void Main(string[] args)
来源：http://xa.muxihuayi.cn

[M08] 获取系统与运行时信息
来源：http://ms.9csxet.cn

Py:   platform.system();  platform.python_version()
来源：http://yn.521024.cn

PHP:  PHP_OS;  phpversion();
来源：http://ob.jctech888.com.cn

JS:   process.platform;  process.version
来源：http://nc.gzmigu.cn

TS:   process.platform;  process.version
来源：http://mo.wgjwhj.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://pl.huixinmuqiang.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://qu.521024.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://lx.nicolike.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://yd.yuntaijiaju.cn

================================================================================
来源：http://co.shtwfgs.cn

N. 数据结构与算法
来源：http://sc.hnjuh.cn

================================================================================
来源：http://fv.bookmarksfly.cn

[N01] 二分查找（有序数组）
来源：http://kn.jianghongdianzi.cn

Py:   bisect.bisect_left(arr, x)
来源：http://rq.muxihuayi.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ez.bjjhwx.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://oj.huixinmuqiang.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://uk.haigaiapp.cn

Java: Arrays.binarySearch(arr, x)
来源：http://yu.huixinmuqiang.cn

Go:   sort.SearchInts(arr, x)
来源：http://cd.521024.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://vv.colortex.cn

C#:   Array.BinarySearch(arr, x)
来源：http://pm.nicolike.cn

[N02] 排序（工程实践用内置实现）
来源：http://zo.newstarts.cn

Py:   sorted(arr);  arr.sort()
来源：http://dl.asd995.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ut.shtwfgs.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://zm.muxihuayi.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://eq.newstarts.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://an.huanxung.cn

Go:   slices.Sort(arr)
来源：http://sy.colortex.cn

Ruby: arr.sort
来源：http://up.szsharing.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://jn.wgjwhj.cn

[N03] 快速排序（分治示例）
来源：http://cn.huanxung.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ou.shxzukj.cn

PHP:  // 递归实现，或用 usort
来源：http://br.jianghongdianzi.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://pz.asd995.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ss.newstarts.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ux.panjiajie.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://uh.bookmarksfly.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://sv.huixinmuqiang.cn

C#:   // 手写递归，或 Array.Sort
来源：http://ap.wgjwhj.cn

[N04] 斐波那契数列
来源：http://rw.haigaiapp.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://lj.gzmigu.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ce.521024.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://nk.nicolike.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ow.muxihuayi.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://tr.bjjhwx.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://zd.521024.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://eg.asd995.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://qt.521024.cn

[N05] 最大公约数
来源：http://et.huixinmuqiang.cn

Py:   math.gcd(a, b)
来源：http://gf.szsharing.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://gp.gzmigu.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://qs.nicolike.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://bh.muxihuayi.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://oz.panjiajie.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ki.chemitech.net.cn

Ruby: a.gcd(b)
来源：http://kp.hnjuh.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://tk.yuntaijiaju.cn

[N06] 判断回文字符串
来源：http://ln.haigaiapp.cn

Py:   s == s[::-1]
来源：http://iz.panjiajie.cn

PHP:  $s === strrev($s);
来源：http://tv.gzmigu.cn

JS:   s === [...s].reverse().join("")
来源：http://lj.szsharing.cn

TS:   s === [...s].reverse().join("")
来源：http://bl.yuexingan06.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ze.yuntaijiaju.cn

Go:   // 双指针从两端比较
来源：http://sa.yuntaijiaju.cn

Ruby: s == s.reverse
来源：http://sc.szxytkj.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://od.lnxyls.cn

[N07] 两数之和（返回下标）
来源：http://ub.gzmigu.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://lz.bookmarksfly.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://oo.yuexingan06.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://ra.huanxung.cn

TS:   // 手写 Map<string, number>
来源：http://en.yuntaijiaju.cn

Java: // 手写 HashMap
来源：http://js.huanxung.cn

Go:   // 手写 map[int]int
来源：http://pd.chemitech.net.cn

Ruby: // 手写 Hash
来源：http://jx.gzmigu.cn

C#:   // 手写 Dictionary<int, int>
来源：http://wb.szxytkj.cn

[N08] 生成全排列
来源：http://aw.huixinmuqiang.cn

Py:   itertools.permutations(arr)
来源：http://ka.shxzukj.cn

PHP:  // 手写递归交换
来源：http://vl.nszjky.cn

JS:   // 手写回溯递归
来源：http://it.colortex.cn

TS:   // 手写回溯递归
来源：http://ca.hahajie.cn

Java: // 手写回溯递归
来源：http://jz.gzmigu.cn

Go:   // 手写回溯递归
来源：http://fz.gzmigu.cn

Ruby: arr.permutation.to_a
来源：http://co.shxzskj.cn

C#:   // 手写回溯递归
来源：http://nj.szsharing.cn

[N09] 栈与队列
来源：http://wc.521024.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://bi.nszjky.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://li.huixiangedu.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://dh.colortex.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://sd.huixiangedu.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://fr.panjiajie.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://sm.shxzukj.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://bv.huanxung.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://bu.newstarts.cn

[N10] 链表节点定义
来源：http://ti.szxytkj.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://vh.jianghongdianzi.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://ex.yuntaijiaju.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ea.nicolike.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://on.chemitech.net.cn

Java: class Node { int v; Node next; }
来源：http://cj.521024.cn

Go:   type Node struct { V int; Next *Node }
来源：http://yp.chemitech.net.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://iv.gzmigu.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://df.yuexingan06.cn

[N11] 二叉树中序遍历
来源：http://cx.shxzukj.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://sh.szsharing.cn

PHP:  // 手写递归函数
来源：http://yt.hnjuh.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://rn.bookmarksfly.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://nk.szsharing.cn

Java: // 手写递归
来源：http://no.huixinmuqiang.cn

Go:   // 手写递归
来源：http://ry.nicolike.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://jz.jianghongdianzi.cn

C#:   // 手写递归
来源：http://vv.yuntaijiaju.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://nq.huixinmuqiang.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ji.chemitech.net.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://kv.yuntaijiaju.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://am.shxzukj.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://uj.huanxung.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ni.szsharing.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://sg.haigaiapp.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://nc.newstarts.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://gm.huixiangedu.cn

================================================================================
来源：http://aq.panjiajie.cn

O. 并发与异步
来源：http://vp.huanxung.cn

================================================================================
来源：http://zx.jctech888.com.cn

[O01] 启动一个线程
来源：http://jh.lnxyls.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://co.yuntaijiaju.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ox.shxzukj.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://dv.yuntaijiaju.cn

TS:   // 同 JS
来源：http://jr.huixiangedu.cn

Java: new Thread(() -> f()).start()
来源：http://sd.haigaiapp.cn

Go:   go f()
来源：http://ku.gzmigu.cn

Ruby: Thread.new { f }
来源：http://to.gzmigu.cn

C#:   Task.Run(() => F());
来源：http://tn.panjiajie.cn

[O02] 使用线程池
来源：http://my.huanxung.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://vn.yuexingan06.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://tu.521024.cn

JS:   // worker_threads 线程池
来源：http://ye.chemitech.net.cn

TS:   // worker_threads 线程池
来源：http://mp.nszjky.cn

Java: Executors.newFixedThreadPool(4)
来源：http://oc.szxytkj.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://xv.nicolike.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mr.shxzukj.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://xi.yuexingan06.cn

[O03] 加锁保护共享数据
来源：http://kc.bookmarksfly.cn

Py:   with lock: shared += 1
来源：http://hl.yuexingan06.cn

PHP:  // 用 flock() 做文件锁
来源：http://dt.yuntaijiaju.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ru.haigaiapp.cn

TS:   // 同 JS
来源：http://rn.panjiajie.cn

Java: synchronized (this) { shared++; }
来源：http://bf.szxytkj.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hk.jianghongdianzi.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://ng.szsharing.cn

C#:   lock (gate) { shared++; }
来源：http://vk.gzmigu.cn

[O04] 定义异步函数并等待
来源：http://gb.yuexingan06.cn

Py:   async def f():⏎    await g()
来源：http://ft.hnjuh.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://oi.huanxung.cn

JS:   async function f() { await g(); }
来源：http://gz.szxytkj.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://aa.jianghongdianzi.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mt.bookmarksfly.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://fs.colortex.cn

Ruby: # 用 Fiber 或 async gem
来源：http://db.gzmigu.cn

C#:   async Task F() { await G(); }
来源：http://dt.colortex.cn

[O05] 并发执行并等待全部完成
来源：http://zc.jianghongdianzi.cn

Py:   asyncio.gather(*tasks)
来源：http://ez.huanxung.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ja.muxihuayi.cn

JS:   await Promise.all(tasks)
来源：http://os.521024.cn

TS:   await Promise.all(tasks)
来源：http://ba.521024.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://nj.hnjuh.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ro.shxzskj.cn

Ruby: threads.map(&:join)
来源：http://tj.szsharing.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://qb.wgjwhj.cn

[O06] 使用进程池
来源：http://vj.bookmarksfly.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://fg.huixiangedu.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://yj.hnjuh.cn

JS:   // child_process / cluster 模块
来源：http://fq.9csxet.cn

TS:   // child_process / cluster 模块
来源：http://ht.gzmigu.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://kc.bookmarksfly.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://gg.jctech888.com.cn

Ruby: // fork 块
来源：http://yi.szxytkj.cn

C#:   Parallel.For
来源：http://dm.huanxung.cn

================================================================================
来源：http://ig.yuntaijiaju.cn

P. 常用工具函数
来源：http://zl.szxytkj.cn

================================================================================
来源：http://go.hahajie.cn

[P01] 生成 UUID
来源：http://wb.lnxyls.cn

Py:   str(uuid.uuid4())
来源：http://fh.huixiangedu.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://lp.hahajie.cn

JS:   crypto.randomUUID()
来源：http://pr.wgjwhj.cn

TS:   crypto.randomUUID()
来源：http://hw.yuexingan06.cn

Java: UUID.randomUUID().toString()
来源：http://sh.wgjwhj.cn

Go:   // 用 github.com/google/uuid
来源：http://hh.shxzukj.cn

Ruby: SecureRandom.uuid
来源：http://zn.huixiangedu.cn

C#:   Guid.NewGuid().ToString()
来源：http://aw.asd995.cn

[P02] MD5 / SHA256 摘要
来源：http://st.huixiangedu.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://jr.bookmarksfly.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://rz.jianghongdianzi.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://gi.wgjwhj.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://uj.shxzukj.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hm.hnjuh.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://id.lnxyls.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ud.szxytkj.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ms.panjiajie.cn

[P03] 生成短随机字符串
来源：http://lr.muxihuayi.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://di.9csxet.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ul.nszjky.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://yu.muxihuayi.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ei.shxzukj.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://gw.szsharing.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://gk.haigaiapp.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://zg.hahajie.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://to.huanxung.cn

[P04] 求长度
来源：http://bn.huanxung.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://qh.bookmarksfly.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ae.szsharing.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://uy.shxzukj.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wj.colortex.cn

Java: list.size();  map.size();  s.length()
来源：http://et.szxytkj.cn

Go:   len(arr);  len(m)
来源：http://tj.9csxet.cn

Ruby: x.length;  x.size
来源：http://qj.panjiajie.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://hh.nicolike.cn

[P05] 判断两个对象内容是否相等
来源：http://cc.nszjky.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://gp.bookmarksfly.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://cw.newstarts.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://gw.szxytkj.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://qc.bjjhwx.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://fd.panjiajie.cn

Go:   reflect.DeepEqual(a, b)
来源：http://pw.wgjwhj.cn

Ruby: a == b
来源：http://hi.yuntaijiaju.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://vv.nszjky.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wp.chemitech.net.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://fw.haigaiapp.cn

PHP:  if (empty($x)) {}
来源：http://pu.asd995.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ox.wgjwhj.cn

TS:   if (x == null) {}
来源：http://zd.newstarts.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://lj.yuntaijiaju.cn

Go:   if x == nil {}
来源：http://rl.jianghongdianzi.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://pm.bookmarksfly.cn

C#:   if (x is null) {}
来源：http://zs.colortex.cn

[P07] 防抖与节流
来源：http://vm.9csxet.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://rc.shxzukj.cn

PHP:  // 手写时间戳比较
来源：http://fl.hahajie.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ju.shtwfgs.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://gy.szxytkj.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://sb.bookmarksfly.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ss.jianghongdianzi.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://mp.muxihuayi.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mz.muxihuayi.cn

[P08] 处理浮点精度问题
来源：http://hx.lnxyls.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ga.panjiajie.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ra.chemitech.net.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://xy.asd995.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://fc.szsharing.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://qa.521024.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://kp.newstarts.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ak.szxytkj.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://tx.wgjwhj.cn

================================================================================
来源：http://qe.yuntaijiaju.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ys.szsharing.cn

================================================================================
来源：http://dz.9csxet.cn

[Q01] 创建表
来源：http://sw.hahajie.cn

CREATE TABLE users (
来源：http://lv.9csxet.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://yz.nicolike.cn

name VARCHAR(50) NOT NULL,
来源：http://pm.yuexingan06.cn

email VARCHAR(100) UNIQUE,
来源：http://jx.9csxet.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mi.yuntaijiaju.cn

);
来源：http://mq.bookmarksfly.cn

[Q02] 创建带外键的表
来源：http://dm.jctech888.com.cn

CREATE TABLE orders (
来源：http://ox.lnxyls.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://uv.yuntaijiaju.cn

user_id INT NOT NULL,
来源：http://ey.gzmigu.cn

amount DECIMAL(10, 2),
来源：http://pg.asd995.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://fm.szsharing.cn

);
来源：http://aj.nicolike.cn

[Q03] 增加列
来源：http://pp.bookmarksfly.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://te.gzmigu.cn

[Q04] 修改列类型
来源：http://yg.newstarts.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wv.szxytkj.cn

[Q05] 重命名列
来源：http://hp.jianghongdianzi.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://er.szxytkj.cn

[Q06] 删除列
来源：http://mt.9csxet.cn

ALTER TABLE users DROP COLUMN age;
来源：http://mm.panjiajie.cn

[Q07] 删除表
来源：http://wq.huixinmuqiang.cn

DROP TABLE IF EXISTS orders;
来源：http://uc.jctech888.com.cn

[Q08] 创建普通索引
来源：http://if.muxihuayi.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://am.jianghongdianzi.cn

[Q09] 创建唯一索引
来源：http://uh.nszjky.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ku.huixiangedu.cn

[Q10] 插入单行
来源：http://nt.szxytkj.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://pv.panjiajie.cn

[Q11] 一次插入多行
来源：http://dl.hahajie.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://je.yuexingan06.cn

[Q12] 插入后取自增 ID
来源：http://iq.nszjky.cn


<!-- 参考信息 -->