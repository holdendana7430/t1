代发 wailian999

PHP:  fwrite(STDERR, "err\n");
来源：http://wj.hahajie.cn

JS:   console.error("err")
来源：http://zf.yuexingan06.cn

TS:   console.error("err")
来源：http://zm.asd995.cn

Java: System.err.println("err")
来源：http://yg.lnxyls.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ob.shxzukj.cn

Ruby: warn "err"
来源：http://hh.huanxung.cn

C#:   Console.Error.WriteLine("err")
来源：http://ao.huanxung.cn

[M07] 判断是否为主入口
来源：http://kb.haigaiapp.cn

Py:   if __name__ == "__main__":
来源：http://ef.nszjky.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://jy.yuexingan06.cn

JS:   require.main === module
来源：http://gv.shtwfgs.cn

TS:   require.main === module
来源：http://lf.huanxung.cn

Java: public static void main(String[] args)
来源：http://tw.9csxet.cn

Go:   func main()
来源：http://xa.lnxyls.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ml.haigaiapp.cn

C#:   static void Main(string[] args)
来源：http://vi.shxzukj.cn

[M08] 获取系统与运行时信息
来源：http://kx.shxzukj.cn

Py:   platform.system();  platform.python_version()
来源：http://ep.yuntaijiaju.cn

PHP:  PHP_OS;  phpversion();
来源：http://mn.shxzukj.cn

JS:   process.platform;  process.version
来源：http://qn.gzmigu.cn

TS:   process.platform;  process.version
来源：http://sr.shxzukj.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://fp.wgjwhj.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://ia.nszjky.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wh.asd995.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://qn.yuntaijiaju.cn

================================================================================
来源：http://cf.newstarts.cn

N. 数据结构与算法
来源：http://ye.bookmarksfly.cn

================================================================================
来源：http://ch.bookmarksfly.cn

[N01] 二分查找（有序数组）
来源：http://zn.521024.cn

Py:   bisect.bisect_left(arr, x)
来源：http://ud.szsharing.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ef.chemitech.net.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://zy.wgjwhj.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://el.haigaiapp.cn

Java: Arrays.binarySearch(arr, x)
来源：http://sd.chemitech.net.cn

Go:   sort.SearchInts(arr, x)
来源：http://gu.asd995.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://sq.hahajie.cn

C#:   Array.BinarySearch(arr, x)
来源：http://iv.yuexingan06.cn

[N02] 排序（工程实践用内置实现）
来源：http://yj.shxzskj.cn

Py:   sorted(arr);  arr.sort()
来源：http://wv.muxihuayi.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://er.huixinmuqiang.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://xq.jianghongdianzi.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://pu.hahajie.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ti.yuexingan06.cn

Go:   slices.Sort(arr)
来源：http://wk.wgjwhj.cn

Ruby: arr.sort
来源：http://ml.bookmarksfly.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://tm.yuntaijiaju.cn

[N03] 快速排序（分治示例）
来源：http://xx.huixiangedu.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://sd.szsharing.cn

PHP:  // 递归实现，或用 usort
来源：http://mi.huixiangedu.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://no.panjiajie.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://eu.huixiangedu.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ic.shtwfgs.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://oe.szxytkj.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://dd.521024.cn

C#:   // 手写递归，或 Array.Sort
来源：http://sm.nicolike.cn

[N04] 斐波那契数列
来源：http://fe.chemitech.net.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://eb.yuexingan06.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ko.shxzukj.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://pa.hahajie.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://qg.hnjuh.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://nx.9csxet.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ef.szxytkj.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://sn.lnxyls.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://vb.wgjwhj.cn

[N05] 最大公约数
来源：http://sb.huixinmuqiang.cn

Py:   math.gcd(a, b)
来源：http://zg.9csxet.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ab.nszjky.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ir.shxzukj.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://tl.colortex.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://we.lnxyls.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://fm.bjjhwx.cn

Ruby: a.gcd(b)
来源：http://bh.wgjwhj.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://nv.bjjhwx.cn

[N06] 判断回文字符串
来源：http://wh.bookmarksfly.cn

Py:   s == s[::-1]
来源：http://ei.hnjuh.cn

PHP:  $s === strrev($s);
来源：http://nm.wgjwhj.cn

JS:   s === [...s].reverse().join("")
来源：http://yj.muxihuayi.cn

TS:   s === [...s].reverse().join("")
来源：http://hl.hnjuh.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ql.lnxyls.cn

Go:   // 双指针从两端比较
来源：http://qd.panjiajie.cn

Ruby: s == s.reverse
来源：http://ux.shxzskj.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://as.yuntaijiaju.cn

[N07] 两数之和（返回下标）
来源：http://vi.wgjwhj.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ly.huanxung.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://yo.521024.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://ke.yuexingan06.cn

TS:   // 手写 Map<string, number>
来源：http://ej.hnjuh.cn

Java: // 手写 HashMap
来源：http://np.huixiangedu.cn

Go:   // 手写 map[int]int
来源：http://ru.hnjuh.cn

Ruby: // 手写 Hash
来源：http://ps.nicolike.cn

C#:   // 手写 Dictionary<int, int>
来源：http://he.nicolike.cn

[N08] 生成全排列
来源：http://qc.szsharing.cn

Py:   itertools.permutations(arr)
来源：http://rk.shxzukj.cn

PHP:  // 手写递归交换
来源：http://ft.hahajie.cn

JS:   // 手写回溯递归
来源：http://ek.panjiajie.cn

TS:   // 手写回溯递归
来源：http://zv.panjiajie.cn

Java: // 手写回溯递归
来源：http://co.nszjky.cn

Go:   // 手写回溯递归
来源：http://id.yuntaijiaju.cn

Ruby: arr.permutation.to_a
来源：http://od.szxytkj.cn

C#:   // 手写回溯递归
来源：http://aq.bookmarksfly.cn

[N09] 栈与队列
来源：http://hz.chemitech.net.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://kj.huixinmuqiang.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://co.panjiajie.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://yy.asd995.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ku.muxihuayi.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hi.muxihuayi.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://sn.haigaiapp.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ot.newstarts.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://nd.wgjwhj.cn

[N10] 链表节点定义
来源：http://ma.szxytkj.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hu.shxzukj.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://hf.yuexingan06.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ta.huixiangedu.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wf.shtwfgs.cn

Java: class Node { int v; Node next; }
来源：http://mk.9csxet.cn

Go:   type Node struct { V int; Next *Node }
来源：http://nj.nszjky.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://nz.shxzskj.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://qd.9csxet.cn

[N11] 二叉树中序遍历
来源：http://vb.bjjhwx.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://es.jctech888.com.cn

PHP:  // 手写递归函数
来源：http://tx.9csxet.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://nj.9csxet.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://gg.jctech888.com.cn

Java: // 手写递归
来源：http://vj.9csxet.cn

Go:   // 手写递归
来源：http://ij.colortex.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://vy.lnxyls.cn

C#:   // 手写递归
来源：http://rm.yuntaijiaju.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://xa.lnxyls.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://qq.9csxet.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://co.bookmarksfly.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://un.nicolike.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://fy.chemitech.net.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hi.jctech888.com.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://za.wgjwhj.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://py.huixinmuqiang.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://no.bookmarksfly.cn

================================================================================
来源：http://aj.jctech888.com.cn

O. 并发与异步
来源：http://cg.wgjwhj.cn

================================================================================
来源：http://up.bjjhwx.cn

[O01] 启动一个线程
来源：http://mx.521024.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ye.panjiajie.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://te.jctech888.com.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://bt.muxihuayi.cn

TS:   // 同 JS
来源：http://yv.nszjky.cn

Java: new Thread(() -> f()).start()
来源：http://zu.huixiangedu.cn

Go:   go f()
来源：http://ie.wgjwhj.cn

Ruby: Thread.new { f }
来源：http://br.nszjky.cn

C#:   Task.Run(() => F());
来源：http://er.lnxyls.cn

[O02] 使用线程池
来源：http://ue.bjjhwx.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://xk.shxzskj.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://rc.jctech888.com.cn

JS:   // worker_threads 线程池
来源：http://sq.gzmigu.cn

TS:   // worker_threads 线程池
来源：http://lj.wgjwhj.cn

Java: Executors.newFixedThreadPool(4)
来源：http://dj.huanxung.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://tj.nszjky.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://cu.asd995.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://of.huixiangedu.cn

[O03] 加锁保护共享数据
来源：http://et.bookmarksfly.cn

Py:   with lock: shared += 1
来源：http://jw.panjiajie.cn

PHP:  // 用 flock() 做文件锁
来源：http://gh.chemitech.net.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://dp.szsharing.cn

TS:   // 同 JS
来源：http://nk.shxzukj.cn

Java: synchronized (this) { shared++; }
来源：http://dz.nszjky.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://sh.bookmarksfly.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://an.bookmarksfly.cn

C#:   lock (gate) { shared++; }
来源：http://bh.jianghongdianzi.cn

[O04] 定义异步函数并等待
来源：http://hm.nicolike.cn

Py:   async def f():⏎    await g()
来源：http://tv.bookmarksfly.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hd.wgjwhj.cn

JS:   async function f() { await g(); }
来源：http://ad.bookmarksfly.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://yc.9csxet.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://lj.jctech888.com.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://pd.huixinmuqiang.cn

Ruby: # 用 Fiber 或 async gem
来源：http://iw.shxzukj.cn

C#:   async Task F() { await G(); }
来源：http://kr.asd995.cn

[O05] 并发执行并等待全部完成
来源：http://zn.huixinmuqiang.cn

Py:   asyncio.gather(*tasks)
来源：http://qf.newstarts.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://fr.hnjuh.cn

JS:   await Promise.all(tasks)
来源：http://tw.shxzukj.cn

TS:   await Promise.all(tasks)
来源：http://ho.huixiangedu.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://jq.huixiangedu.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://rg.huixinmuqiang.cn

Ruby: threads.map(&:join)
来源：http://tm.jianghongdianzi.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://va.colortex.cn

[O06] 使用进程池
来源：http://qv.bookmarksfly.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://bz.newstarts.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://vt.muxihuayi.cn

JS:   // child_process / cluster 模块
来源：http://ea.szxytkj.cn

TS:   // child_process / cluster 模块
来源：http://mg.yuexingan06.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://vk.hahajie.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ix.chemitech.net.cn

Ruby: // fork 块
来源：http://ui.jianghongdianzi.cn

C#:   Parallel.For
来源：http://ui.jianghongdianzi.cn

================================================================================
来源：http://kh.yuntaijiaju.cn

P. 常用工具函数
来源：http://ny.bjjhwx.cn

================================================================================
来源：http://jv.chemitech.net.cn

[P01] 生成 UUID
来源：http://zc.asd995.cn

Py:   str(uuid.uuid4())
来源：http://bj.521024.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://jv.9csxet.cn

JS:   crypto.randomUUID()
来源：http://ht.hahajie.cn

TS:   crypto.randomUUID()
来源：http://we.bookmarksfly.cn

Java: UUID.randomUUID().toString()
来源：http://wf.9csxet.cn

Go:   // 用 github.com/google/uuid
来源：http://jw.wgjwhj.cn

Ruby: SecureRandom.uuid
来源：http://ze.521024.cn

C#:   Guid.NewGuid().ToString()
来源：http://oy.newstarts.cn

[P02] MD5 / SHA256 摘要
来源：http://pc.wgjwhj.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://tb.shxzskj.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://ft.szsharing.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://at.wgjwhj.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ew.9csxet.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://qe.yuntaijiaju.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://fl.bjjhwx.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://kp.szsharing.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://qx.gzmigu.cn

[P03] 生成短随机字符串
来源：http://xo.colortex.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://pn.colortex.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ux.huixiangedu.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://gh.jctech888.com.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://dq.colortex.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://lh.jianghongdianzi.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://re.szsharing.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://xx.colortex.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://vw.bjjhwx.cn

[P04] 求长度
来源：http://yq.shxzukj.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ib.colortex.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://lk.9csxet.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ji.szsharing.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://zu.shxzskj.cn

Java: list.size();  map.size();  s.length()
来源：http://sc.wgjwhj.cn

Go:   len(arr);  len(m)
来源：http://xb.szsharing.cn

Ruby: x.length;  x.size
来源：http://bo.yuexingan06.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://cx.yuexingan06.cn

[P05] 判断两个对象内容是否相等
来源：http://sb.chemitech.net.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://cn.szxytkj.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://el.wgjwhj.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://iu.chemitech.net.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hj.jctech888.com.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://gm.hnjuh.cn

Go:   reflect.DeepEqual(a, b)
来源：http://lt.hnjuh.cn

Ruby: a == b
来源：http://dg.jctech888.com.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://vn.huixinmuqiang.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://zi.9csxet.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ua.chemitech.net.cn

PHP:  if (empty($x)) {}
来源：http://vv.panjiajie.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://dj.yuntaijiaju.cn

TS:   if (x == null) {}
来源：http://xl.szxytkj.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://wi.panjiajie.cn

Go:   if x == nil {}
来源：http://le.huixiangedu.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://fc.newstarts.cn

C#:   if (x is null) {}
来源：http://up.huanxung.cn

[P07] 防抖与节流
来源：http://lt.muxihuayi.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hw.gzmigu.cn

PHP:  // 手写时间戳比较
来源：http://ti.wgjwhj.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://kf.huanxung.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wb.colortex.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://du.jctech888.com.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://nf.nszjky.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://zf.bjjhwx.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://qe.huanxung.cn

[P08] 处理浮点精度问题
来源：http://dl.hnjuh.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ph.yuntaijiaju.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ht.shxzukj.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://kb.jianghongdianzi.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ep.bjjhwx.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ai.jctech888.com.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ev.asd995.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hw.9csxet.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wd.huixinmuqiang.cn

================================================================================
来源：http://vp.haigaiapp.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://sm.521024.cn

================================================================================
来源：http://zi.szsharing.cn

[Q01] 创建表
来源：http://th.colortex.cn

CREATE TABLE users (
来源：http://zk.wgjwhj.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://yl.newstarts.cn

name VARCHAR(50) NOT NULL,
来源：http://bk.huanxung.cn

email VARCHAR(100) UNIQUE,
来源：http://ns.szsharing.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ji.panjiajie.cn

);
来源：http://sz.asd995.cn

[Q02] 创建带外键的表
来源：http://vp.yuntaijiaju.cn

CREATE TABLE orders (
来源：http://kx.nszjky.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://vg.huanxung.cn

user_id INT NOT NULL,
来源：http://kj.panjiajie.cn

amount DECIMAL(10, 2),
来源：http://li.521024.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://db.bookmarksfly.cn

);
来源：http://gv.jctech888.com.cn

[Q03] 增加列
来源：http://yf.szsharing.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ds.yuexingan06.cn

[Q04] 修改列类型
来源：http://vr.hahajie.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ll.shxzukj.cn

[Q05] 重命名列
来源：http://bi.gzmigu.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ht.szxytkj.cn

[Q06] 删除列
来源：http://ab.huixinmuqiang.cn

ALTER TABLE users DROP COLUMN age;
来源：http://mi.muxihuayi.cn

[Q07] 删除表
来源：http://jp.szxytkj.cn

DROP TABLE IF EXISTS orders;
来源：http://gy.haigaiapp.cn

[Q08] 创建普通索引
来源：http://ha.jianghongdianzi.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://pc.jctech888.com.cn

[Q09] 创建唯一索引
来源：http://ml.newstarts.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://xi.wgjwhj.cn

[Q10] 插入单行
来源：http://tf.wgjwhj.cn


<!-- 参考信息 -->