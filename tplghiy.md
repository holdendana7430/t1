代发 wailian999

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.hahajie.cn

Ruby: warn "err"
来源：http://dw.muxihuayi.cn

C#:   Console.Error.WriteLine("err")
来源：http://ay.chemitech.net.cn

[M07] 判断是否为主入口
来源：http://re.panjiajie.cn

Py:   if __name__ == "__main__":
来源：http://it.yuntaijiaju.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ta.shxzskj.cn

JS:   require.main === module
来源：http://gj.panjiajie.cn

TS:   require.main === module
来源：http://pi.yuexingan06.cn

Java: public static void main(String[] args)
来源：http://nq.muxihuayi.cn

Go:   func main()
来源：http://hk.asd995.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://cu.gzmigu.cn

C#:   static void Main(string[] args)
来源：http://wc.wgjwhj.cn

[M08] 获取系统与运行时信息
来源：http://zh.yuntaijiaju.cn

Py:   platform.system();  platform.python_version()
来源：http://ai.yuntaijiaju.cn

PHP:  PHP_OS;  phpversion();
来源：http://oa.9csxet.cn

JS:   process.platform;  process.version
来源：http://er.wgjwhj.cn

TS:   process.platform;  process.version
来源：http://bi.jianghongdianzi.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://xz.haigaiapp.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://qy.shtwfgs.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://li.521024.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://jz.jctech888.com.cn

================================================================================
来源：http://te.9csxet.cn

N. 数据结构与算法
来源：http://ci.nicolike.cn

================================================================================
来源：http://vu.huixiangedu.cn

[N01] 二分查找（有序数组）
来源：http://ra.gzmigu.cn

Py:   bisect.bisect_left(arr, x)
来源：http://ji.bookmarksfly.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://dj.yuntaijiaju.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://vz.yuntaijiaju.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hb.shxzskj.cn

Java: Arrays.binarySearch(arr, x)
来源：http://fm.shxzukj.cn

Go:   sort.SearchInts(arr, x)
来源：http://cj.nicolike.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://af.nszjky.cn

C#:   Array.BinarySearch(arr, x)
来源：http://ue.shxzskj.cn

[N02] 排序（工程实践用内置实现）
来源：http://as.newstarts.cn

Py:   sorted(arr);  arr.sort()
来源：http://sj.colortex.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://oi.huanxung.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://ti.jianghongdianzi.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://rt.hahajie.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wy.szxytkj.cn

Go:   slices.Sort(arr)
来源：http://ml.shxzskj.cn

Ruby: arr.sort
来源：http://vn.newstarts.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://tl.jianghongdianzi.cn

[N03] 快速排序（分治示例）
来源：http://vu.nicolike.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://tp.colortex.cn

PHP:  // 递归实现，或用 usort
来源：http://vh.szsharing.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://js.lnxyls.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://jb.521024.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://xb.szxytkj.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ux.szxytkj.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://xr.wgjwhj.cn

C#:   // 手写递归，或 Array.Sort
来源：http://nn.muxihuayi.cn

[N04] 斐波那契数列
来源：http://go.szxytkj.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://gg.huanxung.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mt.shxzukj.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://cf.panjiajie.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://uj.szxytkj.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://oe.huixiangedu.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ny.asd995.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://aa.jctech888.com.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wh.shtwfgs.cn

[N05] 最大公约数
来源：http://hc.huixiangedu.cn

Py:   math.gcd(a, b)
来源：http://um.shtwfgs.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hk.szsharing.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ag.asd995.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://cu.hnjuh.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://zo.bookmarksfly.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://tl.huixiangedu.cn

Ruby: a.gcd(b)
来源：http://nc.huanxung.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mg.shxzskj.cn

[N06] 判断回文字符串
来源：http://qx.asd995.cn

Py:   s == s[::-1]
来源：http://az.shxzskj.cn

PHP:  $s === strrev($s);
来源：http://aj.nicolike.cn

JS:   s === [...s].reverse().join("")
来源：http://ju.szxytkj.cn

TS:   s === [...s].reverse().join("")
来源：http://cq.szsharing.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://qb.huixinmuqiang.cn

Go:   // 双指针从两端比较
来源：http://tv.nicolike.cn

Ruby: s == s.reverse
来源：http://zk.asd995.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://rl.chemitech.net.cn

[N07] 两数之和（返回下标）
来源：http://rl.shxzskj.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://zj.bjjhwx.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ts.shxzukj.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://ff.jctech888.com.cn

TS:   // 手写 Map<string, number>
来源：http://ch.nszjky.cn

Java: // 手写 HashMap
来源：http://xp.jianghongdianzi.cn

Go:   // 手写 map[int]int
来源：http://pg.521024.cn

Ruby: // 手写 Hash
来源：http://nn.huixiangedu.cn

C#:   // 手写 Dictionary<int, int>
来源：http://ve.szsharing.cn

[N08] 生成全排列
来源：http://om.muxihuayi.cn

Py:   itertools.permutations(arr)
来源：http://ok.chemitech.net.cn

PHP:  // 手写递归交换
来源：http://we.asd995.cn

JS:   // 手写回溯递归
来源：http://lp.jianghongdianzi.cn

TS:   // 手写回溯递归
来源：http://az.bjjhwx.cn

Java: // 手写回溯递归
来源：http://rh.yuntaijiaju.cn

Go:   // 手写回溯递归
来源：http://gw.szsharing.cn

Ruby: arr.permutation.to_a
来源：http://id.asd995.cn

C#:   // 手写回溯递归
来源：http://rb.szsharing.cn

[N09] 栈与队列
来源：http://er.bookmarksfly.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://nn.gzmigu.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://jy.asd995.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://zl.nicolike.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://an.nszjky.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://gb.521024.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ut.huanxung.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://li.szxytkj.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://tf.521024.cn

[N10] 链表节点定义
来源：http://yf.yuexingan06.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ik.nicolike.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://aj.shtwfgs.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://gf.wgjwhj.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://qk.hnjuh.cn

Java: class Node { int v; Node next; }
来源：http://xh.muxihuayi.cn

Go:   type Node struct { V int; Next *Node }
来源：http://iu.gzmigu.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://ty.bookmarksfly.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://dq.lnxyls.cn

[N11] 二叉树中序遍历
来源：http://mw.shtwfgs.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://rd.haigaiapp.cn

PHP:  // 手写递归函数
来源：http://ve.bjjhwx.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://aw.panjiajie.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://zd.chemitech.net.cn

Java: // 手写递归
来源：http://oz.yuntaijiaju.cn

Go:   // 手写递归
来源：http://le.chemitech.net.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://qz.bookmarksfly.cn

C#:   // 手写递归
来源：http://nu.hnjuh.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://es.hahajie.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ni.shxzskj.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://la.hahajie.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wk.nicolike.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://gx.huanxung.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ac.colortex.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://om.bookmarksfly.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://yh.shxzskj.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hi.panjiajie.cn

================================================================================
来源：http://ra.huixiangedu.cn

O. 并发与异步
来源：http://mm.9csxet.cn

================================================================================
来源：http://nu.panjiajie.cn

[O01] 启动一个线程
来源：http://pp.huanxung.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://gq.nicolike.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ch.szxytkj.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ee.asd995.cn

TS:   // 同 JS
来源：http://tz.yuntaijiaju.cn

Java: new Thread(() -> f()).start()
来源：http://oi.haigaiapp.cn

Go:   go f()
来源：http://fw.gzmigu.cn

Ruby: Thread.new { f }
来源：http://cw.yuntaijiaju.cn

C#:   Task.Run(() => F());
来源：http://qm.huixiangedu.cn

[O02] 使用线程池
来源：http://fp.huixinmuqiang.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://kn.nicolike.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://cq.yuexingan06.cn

JS:   // worker_threads 线程池
来源：http://yn.asd995.cn

TS:   // worker_threads 线程池
来源：http://pr.asd995.cn

Java: Executors.newFixedThreadPool(4)
来源：http://kn.newstarts.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://na.jctech888.com.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://of.bookmarksfly.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://oo.9csxet.cn

[O03] 加锁保护共享数据
来源：http://md.hahajie.cn

Py:   with lock: shared += 1
来源：http://qm.521024.cn

PHP:  // 用 flock() 做文件锁
来源：http://hc.hnjuh.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://yd.huixiangedu.cn

TS:   // 同 JS
来源：http://fe.huixiangedu.cn

Java: synchronized (this) { shared++; }
来源：http://fe.muxihuayi.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ag.szsharing.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://th.521024.cn

C#:   lock (gate) { shared++; }
来源：http://nk.bjjhwx.cn

[O04] 定义异步函数并等待
来源：http://sz.szxytkj.cn

Py:   async def f():⏎    await g()
来源：http://sp.521024.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://vp.hahajie.cn

JS:   async function f() { await g(); }
来源：http://vq.bookmarksfly.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://sb.shxzukj.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ky.huanxung.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://gq.yuexingan06.cn

Ruby: # 用 Fiber 或 async gem
来源：http://oj.muxihuayi.cn

C#:   async Task F() { await G(); }
来源：http://tn.yuntaijiaju.cn

[O05] 并发执行并等待全部完成
来源：http://ds.jianghongdianzi.cn

Py:   asyncio.gather(*tasks)
来源：http://sm.bookmarksfly.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://yk.szxytkj.cn

JS:   await Promise.all(tasks)
来源：http://ng.newstarts.cn

TS:   await Promise.all(tasks)
来源：http://jv.gzmigu.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://db.yuntaijiaju.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hh.bjjhwx.cn

Ruby: threads.map(&:join)
来源：http://vr.huixinmuqiang.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://if.szsharing.cn

[O06] 使用进程池
来源：http://ut.hahajie.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://zz.nicolike.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://zi.panjiajie.cn

JS:   // child_process / cluster 模块
来源：http://xo.gzmigu.cn

TS:   // child_process / cluster 模块
来源：http://wh.nszjky.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://yq.gzmigu.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://jy.bjjhwx.cn

Ruby: // fork 块
来源：http://sc.hnjuh.cn

C#:   Parallel.For
来源：http://rk.hnjuh.cn

================================================================================
来源：http://fs.gzmigu.cn

P. 常用工具函数
来源：http://nr.bjjhwx.cn

================================================================================
来源：http://km.panjiajie.cn

[P01] 生成 UUID
来源：http://wu.nszjky.cn

Py:   str(uuid.uuid4())
来源：http://gl.chemitech.net.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://kr.hnjuh.cn

JS:   crypto.randomUUID()
来源：http://nc.huanxung.cn

TS:   crypto.randomUUID()
来源：http://vw.newstarts.cn

Java: UUID.randomUUID().toString()
来源：http://ns.521024.cn

Go:   // 用 github.com/google/uuid
来源：http://zr.gzmigu.cn

Ruby: SecureRandom.uuid
来源：http://wb.wgjwhj.cn

C#:   Guid.NewGuid().ToString()
来源：http://yd.nicolike.cn

[P02] MD5 / SHA256 摘要
来源：http://zi.huixinmuqiang.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ci.9csxet.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://nf.hahajie.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mc.shxzskj.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ru.shtwfgs.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://sl.jctech888.com.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://sz.bookmarksfly.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://vx.wgjwhj.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ap.chemitech.net.cn

[P03] 生成短随机字符串
来源：http://sr.bookmarksfly.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://cm.lnxyls.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://go.9csxet.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ub.shxzskj.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://aj.hahajie.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://up.huixinmuqiang.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ti.yuntaijiaju.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://od.newstarts.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://dq.bookmarksfly.cn

[P04] 求长度
来源：http://gl.szsharing.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ib.shxzskj.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wr.huanxung.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://gv.nicolike.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://or.chemitech.net.cn

Java: list.size();  map.size();  s.length()
来源：http://wy.shtwfgs.cn

Go:   len(arr);  len(m)
来源：http://vf.shtwfgs.cn

Ruby: x.length;  x.size
来源：http://ht.hnjuh.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://ur.panjiajie.cn

[P05] 判断两个对象内容是否相等
来源：http://gc.shxzukj.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://hi.jctech888.com.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://bj.gzmigu.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ol.521024.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hf.shtwfgs.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://rk.nszjky.cn

Go:   reflect.DeepEqual(a, b)
来源：http://dh.nicolike.cn

Ruby: a == b
来源：http://qs.nszjky.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ir.haigaiapp.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://sl.huixinmuqiang.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://gw.muxihuayi.cn

PHP:  if (empty($x)) {}
来源：http://jc.jctech888.com.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hy.szxytkj.cn

TS:   if (x == null) {}
来源：http://pf.shxzskj.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://bd.shtwfgs.cn

Go:   if x == nil {}
来源：http://xs.chemitech.net.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ra.huixiangedu.cn

C#:   if (x is null) {}
来源：http://tq.huixinmuqiang.cn

[P07] 防抖与节流
来源：http://tz.huixiangedu.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ds.hahajie.cn

PHP:  // 手写时间戳比较
来源：http://aj.nszjky.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ox.hnjuh.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ec.521024.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://kl.gzmigu.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mj.yuntaijiaju.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://yj.nszjky.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://qi.huixinmuqiang.cn

[P08] 处理浮点精度问题
来源：http://cm.hahajie.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://nv.nicolike.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://gt.muxihuayi.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ws.jctech888.com.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://cc.nicolike.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://zn.shxzskj.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://vs.szxytkj.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://qm.muxihuayi.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://kj.yuexingan06.cn

================================================================================
来源：http://gh.chemitech.net.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://db.nszjky.cn

================================================================================
来源：http://vf.haigaiapp.cn

[Q01] 创建表
来源：http://lr.colortex.cn

CREATE TABLE users (
来源：http://dq.521024.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ti.yuntaijiaju.cn

name VARCHAR(50) NOT NULL,
来源：http://kc.jctech888.com.cn

email VARCHAR(100) UNIQUE,
来源：http://rd.haigaiapp.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wi.shtwfgs.cn

);
来源：http://cp.jctech888.com.cn

[Q02] 创建带外键的表
来源：http://aa.nszjky.cn

CREATE TABLE orders (
来源：http://fv.521024.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://kb.huixiangedu.cn

user_id INT NOT NULL,
来源：http://pw.jctech888.com.cn

amount DECIMAL(10, 2),
来源：http://ea.bjjhwx.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://nu.huanxung.cn

);
来源：http://ej.lnxyls.cn

[Q03] 增加列
来源：http://aw.hahajie.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://kl.colortex.cn

[Q04] 修改列类型
来源：http://eh.jianghongdianzi.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://qz.wgjwhj.cn

[Q05] 重命名列
来源：http://az.colortex.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://fo.shxzukj.cn

[Q06] 删除列
来源：http://gn.nszjky.cn

ALTER TABLE users DROP COLUMN age;
来源：http://pv.hnjuh.cn

[Q07] 删除表
来源：http://di.yuntaijiaju.cn

DROP TABLE IF EXISTS orders;
来源：http://xm.lnxyls.cn

[Q08] 创建普通索引
来源：http://aw.nszjky.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://bn.yuntaijiaju.cn

[Q09] 创建唯一索引
来源：http://ho.muxihuayi.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mb.shtwfgs.cn

[Q10] 插入单行
来源：http://uc.hahajie.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://lx.huixiangedu.cn

[Q11] 一次插入多行
来源：http://hj.gzmigu.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://zr.nszjky.cn

[Q12] 插入后取自增 ID
来源：http://vh.huixinmuqiang.cn


<!-- 参考信息 -->