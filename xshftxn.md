代发 wailian999

Ruby: exit 1
来源：http://ck.hahajie.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://gm.shxzskj.cn

[M06] 向标准错误输出
来源：http://gg.shxzskj.cn

Py:   print("err", file=sys.stderr)
来源：http://hn.chemitech.net.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://bc.9csxet.cn

JS:   console.error("err")
来源：http://vn.szsharing.cn

TS:   console.error("err")
来源：http://zq.lnxyls.cn

Java: System.err.println("err")
来源：http://yn.gzmigu.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://gq.asd995.cn

Ruby: warn "err"
来源：http://kv.haigaiapp.cn

C#:   Console.Error.WriteLine("err")
来源：http://oq.haigaiapp.cn

[M07] 判断是否为主入口
来源：http://mi.bookmarksfly.cn

Py:   if __name__ == "__main__":
来源：http://dw.nszjky.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://fh.gzmigu.cn

JS:   require.main === module
来源：http://sh.haigaiapp.cn

TS:   require.main === module
来源：http://xb.szsharing.cn

Java: public static void main(String[] args)
来源：http://ea.shxzskj.cn

Go:   func main()
来源：http://st.huixiangedu.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://zs.shtwfgs.cn

C#:   static void Main(string[] args)
来源：http://nh.szsharing.cn

[M08] 获取系统与运行时信息
来源：http://yx.bjjhwx.cn

Py:   platform.system();  platform.python_version()
来源：http://ed.hnjuh.cn

PHP:  PHP_OS;  phpversion();
来源：http://ey.nicolike.cn

JS:   process.platform;  process.version
来源：http://ru.huixiangedu.cn

TS:   process.platform;  process.version
来源：http://gt.hahajie.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ca.bookmarksfly.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://uz.lnxyls.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ve.panjiajie.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://lv.lnxyls.cn

================================================================================
来源：http://ws.shxzukj.cn

N. 数据结构与算法
来源：http://rb.colortex.cn

================================================================================
来源：http://td.yuntaijiaju.cn

[N01] 二分查找（有序数组）
来源：http://lf.panjiajie.cn

Py:   bisect.bisect_left(arr, x)
来源：http://go.bjjhwx.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://jq.hnjuh.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://qz.shxzukj.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hh.nszjky.cn

Java: Arrays.binarySearch(arr, x)
来源：http://iq.huixinmuqiang.cn

Go:   sort.SearchInts(arr, x)
来源：http://rb.jianghongdianzi.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://jh.wgjwhj.cn

C#:   Array.BinarySearch(arr, x)
来源：http://vv.bjjhwx.cn

[N02] 排序（工程实践用内置实现）
来源：http://nd.shxzukj.cn

Py:   sorted(arr);  arr.sort()
来源：http://ui.shxzukj.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://pm.gzmigu.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://li.shxzukj.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://gz.jianghongdianzi.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://bq.muxihuayi.cn

Go:   slices.Sort(arr)
来源：http://ed.bookmarksfly.cn

Ruby: arr.sort
来源：http://zv.wgjwhj.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://py.hnjuh.cn

[N03] 快速排序（分治示例）
来源：http://kb.huanxung.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wb.nszjky.cn

PHP:  // 递归实现，或用 usort
来源：http://ni.asd995.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wu.521024.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://xs.yuntaijiaju.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://gq.wgjwhj.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://gf.jianghongdianzi.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://yt.huixiangedu.cn

C#:   // 手写递归，或 Array.Sort
来源：http://yq.szxytkj.cn

[N04] 斐波那契数列
来源：http://jp.shxzskj.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://yv.colortex.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://rk.shxzskj.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ks.9csxet.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://su.huixinmuqiang.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://cw.gzmigu.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://cf.chemitech.net.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://dg.nszjky.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://uw.9csxet.cn

[N05] 最大公约数
来源：http://du.colortex.cn

Py:   math.gcd(a, b)
来源：http://ir.jctech888.com.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://sw.hahajie.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://bw.huanxung.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ee.asd995.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://up.bjjhwx.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://st.asd995.cn

Ruby: a.gcd(b)
来源：http://pd.wgjwhj.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://qe.jianghongdianzi.cn

[N06] 判断回文字符串
来源：http://jt.gzmigu.cn

Py:   s == s[::-1]
来源：http://ez.muxihuayi.cn

PHP:  $s === strrev($s);
来源：http://qi.asd995.cn

JS:   s === [...s].reverse().join("")
来源：http://ow.szxytkj.cn

TS:   s === [...s].reverse().join("")
来源：http://uy.521024.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://cz.hahajie.cn

Go:   // 双指针从两端比较
来源：http://ri.nicolike.cn

Ruby: s == s.reverse
来源：http://qv.lnxyls.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://eg.huixinmuqiang.cn

[N07] 两数之和（返回下标）
来源：http://ab.yuntaijiaju.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://nk.jianghongdianzi.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://bk.hahajie.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://lb.shtwfgs.cn

TS:   // 手写 Map<string, number>
来源：http://cl.huixinmuqiang.cn

Java: // 手写 HashMap
来源：http://tc.hnjuh.cn

Go:   // 手写 map[int]int
来源：http://yg.colortex.cn

Ruby: // 手写 Hash
来源：http://hz.bjjhwx.cn

C#:   // 手写 Dictionary<int, int>
来源：http://ds.huixinmuqiang.cn

[N08] 生成全排列
来源：http://uv.wgjwhj.cn

Py:   itertools.permutations(arr)
来源：http://ov.jianghongdianzi.cn

PHP:  // 手写递归交换
来源：http://ah.yuexingan06.cn

JS:   // 手写回溯递归
来源：http://uo.nicolike.cn

TS:   // 手写回溯递归
来源：http://ts.huanxung.cn

Java: // 手写回溯递归
来源：http://yh.bookmarksfly.cn

Go:   // 手写回溯递归
来源：http://ch.nszjky.cn

Ruby: arr.permutation.to_a
来源：http://bm.jianghongdianzi.cn

C#:   // 手写回溯递归
来源：http://ge.lnxyls.cn

[N09] 栈与队列
来源：http://fk.szxytkj.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://on.bookmarksfly.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://vj.hahajie.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://pj.muxihuayi.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ru.bookmarksfly.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ms.shtwfgs.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://rz.muxihuayi.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ix.bookmarksfly.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mj.shtwfgs.cn

[N10] 链表节点定义
来源：http://eb.jianghongdianzi.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://jp.521024.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://nd.huanxung.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://vi.jianghongdianzi.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://xs.nszjky.cn

Java: class Node { int v; Node next; }
来源：http://va.yuntaijiaju.cn

Go:   type Node struct { V int; Next *Node }
来源：http://to.jianghongdianzi.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://cv.lnxyls.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://zu.nicolike.cn

[N11] 二叉树中序遍历
来源：http://ru.jianghongdianzi.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://nn.shtwfgs.cn

PHP:  // 手写递归函数
来源：http://ku.muxihuayi.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ak.huixiangedu.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://lc.9csxet.cn

Java: // 手写递归
来源：http://fz.colortex.cn

Go:   // 手写递归
来源：http://tq.hnjuh.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://tj.bookmarksfly.cn

C#:   // 手写递归
来源：http://lr.hahajie.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://xv.bookmarksfly.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://qm.yuexingan06.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://bw.shtwfgs.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://my.jianghongdianzi.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://dp.huanxung.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ms.nicolike.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://zd.shxzskj.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ta.shxzukj.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://xa.shxzukj.cn

================================================================================
来源：http://fc.shxzskj.cn

O. 并发与异步
来源：http://tq.hnjuh.cn

================================================================================
来源：http://ca.hahajie.cn

[O01] 启动一个线程
来源：http://my.gzmigu.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://gq.chemitech.net.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://nq.jctech888.com.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://yw.shtwfgs.cn

TS:   // 同 JS
来源：http://ez.shxzukj.cn

Java: new Thread(() -> f()).start()
来源：http://pv.yuexingan06.cn

Go:   go f()
来源：http://zr.huixinmuqiang.cn

Ruby: Thread.new { f }
来源：http://dx.jctech888.com.cn

C#:   Task.Run(() => F());
来源：http://qg.gzmigu.cn

[O02] 使用线程池
来源：http://ea.bjjhwx.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://go.szxytkj.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://si.jctech888.com.cn

JS:   // worker_threads 线程池
来源：http://xg.huanxung.cn

TS:   // worker_threads 线程池
来源：http://hy.shtwfgs.cn

Java: Executors.newFixedThreadPool(4)
来源：http://qq.9csxet.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://xd.jctech888.com.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://nb.bookmarksfly.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://bl.wgjwhj.cn

[O03] 加锁保护共享数据
来源：http://lh.panjiajie.cn

Py:   with lock: shared += 1
来源：http://qg.gzmigu.cn

PHP:  // 用 flock() 做文件锁
来源：http://zd.shtwfgs.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://do.jctech888.com.cn

TS:   // 同 JS
来源：http://gs.bookmarksfly.cn

Java: synchronized (this) { shared++; }
来源：http://uj.hahajie.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ey.gzmigu.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://qn.colortex.cn

C#:   lock (gate) { shared++; }
来源：http://jv.shtwfgs.cn

[O04] 定义异步函数并等待
来源：http://hu.colortex.cn

Py:   async def f():⏎    await g()
来源：http://gw.huixinmuqiang.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://jh.chemitech.net.cn

JS:   async function f() { await g(); }
来源：http://xr.nicolike.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://le.asd995.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://xn.shxzskj.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://eu.szxytkj.cn

Ruby: # 用 Fiber 或 async gem
来源：http://gz.szsharing.cn

C#:   async Task F() { await G(); }
来源：http://xc.huixiangedu.cn

[O05] 并发执行并等待全部完成
来源：http://bs.huixiangedu.cn

Py:   asyncio.gather(*tasks)
来源：http://pd.huanxung.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ke.hnjuh.cn

JS:   await Promise.all(tasks)
来源：http://os.lnxyls.cn

TS:   await Promise.all(tasks)
来源：http://zl.huixinmuqiang.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://gp.huanxung.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://vk.szsharing.cn

Ruby: threads.map(&:join)
来源：http://sp.szsharing.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://vq.521024.cn

[O06] 使用进程池
来源：http://lm.hnjuh.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wg.yuexingan06.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://ve.haigaiapp.cn

JS:   // child_process / cluster 模块
来源：http://fd.huixinmuqiang.cn

TS:   // child_process / cluster 模块
来源：http://mh.colortex.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://gr.muxihuayi.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://et.asd995.cn

Ruby: // fork 块
来源：http://rz.jianghongdianzi.cn

C#:   Parallel.For
来源：http://gd.nszjky.cn

================================================================================
来源：http://lb.nszjky.cn

P. 常用工具函数
来源：http://nt.hnjuh.cn

================================================================================
来源：http://jc.jctech888.com.cn

[P01] 生成 UUID
来源：http://ry.jctech888.com.cn

Py:   str(uuid.uuid4())
来源：http://kn.bookmarksfly.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://nl.shtwfgs.cn

JS:   crypto.randomUUID()
来源：http://va.shtwfgs.cn

TS:   crypto.randomUUID()
来源：http://xo.szxytkj.cn

Java: UUID.randomUUID().toString()
来源：http://up.asd995.cn

Go:   // 用 github.com/google/uuid
来源：http://rs.huixinmuqiang.cn

Ruby: SecureRandom.uuid
来源：http://ou.hnjuh.cn

C#:   Guid.NewGuid().ToString()
来源：http://xn.yuexingan06.cn

[P02] MD5 / SHA256 摘要
来源：http://bd.hahajie.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ns.hahajie.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://dx.asd995.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://go.huanxung.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://oy.wgjwhj.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://gp.521024.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wm.hnjuh.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wf.chemitech.net.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://nr.newstarts.cn

[P03] 生成短随机字符串
来源：http://cw.asd995.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://pa.hnjuh.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ly.nicolike.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ic.nszjky.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://af.wgjwhj.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://yn.shxzskj.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://gu.bookmarksfly.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://fl.nszjky.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://li.yuntaijiaju.cn

[P04] 求长度
来源：http://pq.lnxyls.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://gu.jctech888.com.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://rk.asd995.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://zo.gzmigu.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://dx.nszjky.cn

Java: list.size();  map.size();  s.length()
来源：http://iw.nszjky.cn

Go:   len(arr);  len(m)
来源：http://cs.shxzukj.cn

Ruby: x.length;  x.size
来源：http://us.szxytkj.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://oz.jctech888.com.cn

[P05] 判断两个对象内容是否相等
来源：http://bi.lnxyls.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://xz.colortex.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ex.wgjwhj.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://la.nszjky.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://jn.shtwfgs.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://xp.haigaiapp.cn

Go:   reflect.DeepEqual(a, b)
来源：http://ni.521024.cn

Ruby: a == b
来源：http://bx.szxytkj.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ge.szsharing.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://xd.bjjhwx.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://el.bjjhwx.cn

PHP:  if (empty($x)) {}
来源：http://vb.yuexingan06.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://bj.shtwfgs.cn

TS:   if (x == null) {}
来源：http://ei.gzmigu.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://mj.nicolike.cn

Go:   if x == nil {}
来源：http://sw.hnjuh.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://xe.lnxyls.cn

C#:   if (x is null) {}
来源：http://lq.chemitech.net.cn

[P07] 防抖与节流
来源：http://hh.nicolike.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://vo.nicolike.cn

PHP:  // 手写时间戳比较
来源：http://yh.gzmigu.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://nc.colortex.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://bd.haigaiapp.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ll.colortex.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://kt.shtwfgs.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://sf.huixiangedu.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://db.huixinmuqiang.cn

[P08] 处理浮点精度问题
来源：http://ik.9csxet.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://cu.bookmarksfly.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://qg.521024.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://di.yuexingan06.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://an.panjiajie.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://lb.bookmarksfly.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://gd.bjjhwx.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://sq.newstarts.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://xt.wgjwhj.cn

================================================================================
来源：http://vx.521024.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://nw.asd995.cn

================================================================================
来源：http://zj.jianghongdianzi.cn

[Q01] 创建表
来源：http://jd.521024.cn

CREATE TABLE users (
来源：http://da.jctech888.com.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://cz.szsharing.cn

name VARCHAR(50) NOT NULL,
来源：http://dq.nicolike.cn

email VARCHAR(100) UNIQUE,
来源：http://ox.nicolike.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://es.huixiangedu.cn

);
来源：http://pj.jctech888.com.cn

[Q02] 创建带外键的表
来源：http://ae.9csxet.cn

CREATE TABLE orders (
来源：http://au.jctech888.com.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ee.shxzukj.cn

user_id INT NOT NULL,
来源：http://uy.gzmigu.cn

amount DECIMAL(10, 2),
来源：http://mp.nszjky.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://rw.9csxet.cn

);
来源：http://ib.panjiajie.cn

[Q03] 增加列
来源：http://pe.asd995.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ce.asd995.cn

[Q04] 修改列类型
来源：http://we.jianghongdianzi.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://yt.wgjwhj.cn

[Q05] 重命名列
来源：http://dt.yuexingan06.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://sz.gzmigu.cn

[Q06] 删除列
来源：http://mq.521024.cn

ALTER TABLE users DROP COLUMN age;
来源：http://td.haigaiapp.cn

[Q07] 删除表
来源：http://pt.bjjhwx.cn

DROP TABLE IF EXISTS orders;
来源：http://lc.shxzukj.cn

[Q08] 创建普通索引
来源：http://ly.huixinmuqiang.cn


<!-- 参考信息 -->