代发 wailian999

Ruby: exit 1
来源：http://yk.hahajie.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://nr.shtwfgs.cn

[M06] 向标准错误输出
来源：http://bl.wgjwhj.cn

Py:   print("err", file=sys.stderr)
来源：http://ff.521024.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://vr.jianghongdianzi.cn

JS:   console.error("err")
来源：http://lm.colortex.cn

TS:   console.error("err")
来源：http://ms.panjiajie.cn

Java: System.err.println("err")
来源：http://rp.hahajie.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://nu.newstarts.cn

Ruby: warn "err"
来源：http://fa.muxihuayi.cn

C#:   Console.Error.WriteLine("err")
来源：http://ca.shxzukj.cn

[M07] 判断是否为主入口
来源：http://gw.haigaiapp.cn

Py:   if __name__ == "__main__":
来源：http://jy.bjjhwx.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://xj.muxihuayi.cn

JS:   require.main === module
来源：http://tu.muxihuayi.cn

TS:   require.main === module
来源：http://ek.hnjuh.cn

Java: public static void main(String[] args)
来源：http://tu.jctech888.com.cn

Go:   func main()
来源：http://ka.yuntaijiaju.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://sd.jctech888.com.cn

C#:   static void Main(string[] args)
来源：http://pg.yuexingan06.cn

[M08] 获取系统与运行时信息
来源：http://pq.huanxung.cn

Py:   platform.system();  platform.python_version()
来源：http://ck.huixiangedu.cn

PHP:  PHP_OS;  phpversion();
来源：http://sz.gzmigu.cn

JS:   process.platform;  process.version
来源：http://nu.shtwfgs.cn

TS:   process.platform;  process.version
来源：http://nj.huixiangedu.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ym.lnxyls.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://jv.9csxet.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ls.wgjwhj.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://uj.bookmarksfly.cn

================================================================================
来源：http://bx.wgjwhj.cn

N. 数据结构与算法
来源：http://ds.nszjky.cn

================================================================================
来源：http://ep.521024.cn

[N01] 二分查找（有序数组）
来源：http://lx.asd995.cn

Py:   bisect.bisect_left(arr, x)
来源：http://zk.huanxung.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hc.huanxung.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://va.shxzukj.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://to.521024.cn

Java: Arrays.binarySearch(arr, x)
来源：http://mx.shxzukj.cn

Go:   sort.SearchInts(arr, x)
来源：http://kt.yuntaijiaju.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://kz.nicolike.cn

C#:   Array.BinarySearch(arr, x)
来源：http://bq.nicolike.cn

[N02] 排序（工程实践用内置实现）
来源：http://oh.hnjuh.cn

Py:   sorted(arr);  arr.sort()
来源：http://xy.yuexingan06.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://dd.chemitech.net.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://bl.colortex.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://bd.yuexingan06.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://dm.wgjwhj.cn

Go:   slices.Sort(arr)
来源：http://re.jianghongdianzi.cn

Ruby: arr.sort
来源：http://ip.shxzukj.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://di.521024.cn

[N03] 快速排序（分治示例）
来源：http://jt.gzmigu.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://tj.muxihuayi.cn

PHP:  // 递归实现，或用 usort
来源：http://md.521024.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://pk.521024.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://nt.chemitech.net.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ai.chemitech.net.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ix.gzmigu.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://vl.huixiangedu.cn

C#:   // 手写递归，或 Array.Sort
来源：http://ki.colortex.cn

[N04] 斐波那契数列
来源：http://xv.yuexingan06.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://lg.nicolike.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ni.jianghongdianzi.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ej.shtwfgs.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://gc.bjjhwx.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://be.nszjky.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://cn.haigaiapp.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ef.newstarts.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wi.gzmigu.cn

[N05] 最大公约数
来源：http://wn.bjjhwx.cn

Py:   math.gcd(a, b)
来源：http://lc.huanxung.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://zp.shxzukj.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wv.yuexingan06.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://zj.nszjky.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mf.colortex.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ow.bookmarksfly.cn

Ruby: a.gcd(b)
来源：http://yf.panjiajie.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://gr.panjiajie.cn

[N06] 判断回文字符串
来源：http://lw.huanxung.cn

Py:   s == s[::-1]
来源：http://vs.lnxyls.cn

PHP:  $s === strrev($s);
来源：http://nh.haigaiapp.cn

JS:   s === [...s].reverse().join("")
来源：http://gg.lnxyls.cn

TS:   s === [...s].reverse().join("")
来源：http://pr.nszjky.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ly.nicolike.cn

Go:   // 双指针从两端比较
来源：http://wi.huixiangedu.cn

Ruby: s == s.reverse
来源：http://yw.lnxyls.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://jn.nszjky.cn

[N07] 两数之和（返回下标）
来源：http://df.chemitech.net.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://my.bjjhwx.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ef.shtwfgs.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://uu.shtwfgs.cn

TS:   // 手写 Map<string, number>
来源：http://dt.521024.cn

Java: // 手写 HashMap
来源：http://si.bookmarksfly.cn

Go:   // 手写 map[int]int
来源：http://vl.wgjwhj.cn

Ruby: // 手写 Hash
来源：http://zz.huanxung.cn

C#:   // 手写 Dictionary<int, int>
来源：http://cu.huixiangedu.cn

[N08] 生成全排列
来源：http://fg.521024.cn

Py:   itertools.permutations(arr)
来源：http://sj.szxytkj.cn

PHP:  // 手写递归交换
来源：http://tf.gzmigu.cn

JS:   // 手写回溯递归
来源：http://qa.huixiangedu.cn

TS:   // 手写回溯递归
来源：http://eh.shtwfgs.cn

Java: // 手写回溯递归
来源：http://cx.asd995.cn

Go:   // 手写回溯递归
来源：http://bq.muxihuayi.cn

Ruby: arr.permutation.to_a
来源：http://gq.jctech888.com.cn

C#:   // 手写回溯递归
来源：http://oa.lnxyls.cn

[N09] 栈与队列
来源：http://lq.hnjuh.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ae.nszjky.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://gl.shxzskj.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ea.521024.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://oy.yuntaijiaju.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://xy.nicolike.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hx.gzmigu.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://xb.shxzukj.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ew.jianghongdianzi.cn

[N10] 链表节点定义
来源：http://py.shtwfgs.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://my.9csxet.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://lr.muxihuayi.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://gn.yuexingan06.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://sx.panjiajie.cn

Java: class Node { int v; Node next; }
来源：http://pz.9csxet.cn

Go:   type Node struct { V int; Next *Node }
来源：http://it.nszjky.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://vt.chemitech.net.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://bc.9csxet.cn

[N11] 二叉树中序遍历
来源：http://pg.521024.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ve.yuexingan06.cn

PHP:  // 手写递归函数
来源：http://oz.nszjky.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://gl.chemitech.net.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://to.bjjhwx.cn

Java: // 手写递归
来源：http://av.gzmigu.cn

Go:   // 手写递归
来源：http://vy.chemitech.net.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://bs.wgjwhj.cn

C#:   // 手写递归
来源：http://xu.yuexingan06.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://nf.chemitech.net.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ut.yuexingan06.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ho.nicolike.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://av.huanxung.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ii.bjjhwx.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://gl.521024.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://nl.huixiangedu.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://al.huixinmuqiang.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://zb.bjjhwx.cn

================================================================================
来源：http://jt.bookmarksfly.cn

O. 并发与异步
来源：http://kf.hahajie.cn

================================================================================
来源：http://ap.huixinmuqiang.cn

[O01] 启动一个线程
来源：http://uh.szsharing.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://dh.yuntaijiaju.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://vk.huixiangedu.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://qd.yuntaijiaju.cn

TS:   // 同 JS
来源：http://bz.haigaiapp.cn

Java: new Thread(() -> f()).start()
来源：http://yk.asd995.cn

Go:   go f()
来源：http://fg.hahajie.cn

Ruby: Thread.new { f }
来源：http://mr.chemitech.net.cn

C#:   Task.Run(() => F());
来源：http://kx.shxzukj.cn

[O02] 使用线程池
来源：http://zt.9csxet.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://lo.huixinmuqiang.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://xe.newstarts.cn

JS:   // worker_threads 线程池
来源：http://zq.bjjhwx.cn

TS:   // worker_threads 线程池
来源：http://wa.huanxung.cn

Java: Executors.newFixedThreadPool(4)
来源：http://bf.bjjhwx.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://bi.newstarts.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://yz.bookmarksfly.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://kg.hahajie.cn

[O03] 加锁保护共享数据
来源：http://fb.huanxung.cn

Py:   with lock: shared += 1
来源：http://za.nicolike.cn

PHP:  // 用 flock() 做文件锁
来源：http://fp.lnxyls.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://bw.nicolike.cn

TS:   // 同 JS
来源：http://ep.shxzukj.cn

Java: synchronized (this) { shared++; }
来源：http://ed.gzmigu.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://iy.shxzukj.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://mj.huanxung.cn

C#:   lock (gate) { shared++; }
来源：http://yy.521024.cn

[O04] 定义异步函数并等待
来源：http://qn.jianghongdianzi.cn

Py:   async def f():⏎    await g()
来源：http://ll.jianghongdianzi.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://pd.nicolike.cn

JS:   async function f() { await g(); }
来源：http://tg.chemitech.net.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://vg.huanxung.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://cg.nszjky.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://er.yuntaijiaju.cn

Ruby: # 用 Fiber 或 async gem
来源：http://vl.gzmigu.cn

C#:   async Task F() { await G(); }
来源：http://nw.colortex.cn

[O05] 并发执行并等待全部完成
来源：http://yh.jianghongdianzi.cn

Py:   asyncio.gather(*tasks)
来源：http://vw.shxzukj.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://bi.bjjhwx.cn

JS:   await Promise.all(tasks)
来源：http://wi.huanxung.cn

TS:   await Promise.all(tasks)
来源：http://kr.bookmarksfly.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://rw.yuexingan06.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://lg.colortex.cn

Ruby: threads.map(&:join)
来源：http://sx.9csxet.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://hn.wgjwhj.cn

[O06] 使用进程池
来源：http://ao.szxytkj.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://vz.huixiangedu.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://vh.jctech888.com.cn

JS:   // child_process / cluster 模块
来源：http://nq.nszjky.cn

TS:   // child_process / cluster 模块
来源：http://jb.jctech888.com.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://bp.chemitech.net.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://pg.bookmarksfly.cn

Ruby: // fork 块
来源：http://gy.jianghongdianzi.cn

C#:   Parallel.For
来源：http://nd.asd995.cn

================================================================================
来源：http://vm.shtwfgs.cn

P. 常用工具函数
来源：http://kw.wgjwhj.cn

================================================================================
来源：http://ug.shtwfgs.cn

[P01] 生成 UUID
来源：http://lr.szsharing.cn

Py:   str(uuid.uuid4())
来源：http://pq.hnjuh.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wi.shxzukj.cn

JS:   crypto.randomUUID()
来源：http://oh.colortex.cn

TS:   crypto.randomUUID()
来源：http://sr.jianghongdianzi.cn

Java: UUID.randomUUID().toString()
来源：http://hy.shxzskj.cn

Go:   // 用 github.com/google/uuid
来源：http://cw.hahajie.cn

Ruby: SecureRandom.uuid
来源：http://uy.yuexingan06.cn

C#:   Guid.NewGuid().ToString()
来源：http://ob.hnjuh.cn

[P02] MD5 / SHA256 摘要
来源：http://co.shxzskj.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://jd.nszjky.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://ub.gzmigu.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ym.szxytkj.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://nf.chemitech.net.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://qo.asd995.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://qz.shxzskj.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hn.panjiajie.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://xg.yuntaijiaju.cn

[P03] 生成短随机字符串
来源：http://za.huixiangedu.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://cg.wgjwhj.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://dm.jctech888.com.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://cb.jctech888.com.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://vn.hnjuh.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://vt.asd995.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://tu.panjiajie.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://ut.haigaiapp.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://uo.nicolike.cn

[P04] 求长度
来源：http://mz.shxzskj.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://na.nicolike.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hd.colortex.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://fs.lnxyls.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://iv.gzmigu.cn

Java: list.size();  map.size();  s.length()
来源：http://tg.lnxyls.cn

Go:   len(arr);  len(m)
来源：http://gu.panjiajie.cn

Ruby: x.length;  x.size
来源：http://bm.huixiangedu.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://ac.huixinmuqiang.cn

[P05] 判断两个对象内容是否相等
来源：http://mi.jctech888.com.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://hc.shxzukj.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://dn.nicolike.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://kq.huixiangedu.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ox.huixiangedu.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ld.hahajie.cn

Go:   reflect.DeepEqual(a, b)
来源：http://xn.chemitech.net.cn

Ruby: a == b
来源：http://ev.hahajie.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://po.nszjky.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://zo.wgjwhj.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hc.haigaiapp.cn

PHP:  if (empty($x)) {}
来源：http://uk.wgjwhj.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://rg.szsharing.cn

TS:   if (x == null) {}
来源：http://qk.lnxyls.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://ic.huixiangedu.cn

Go:   if x == nil {}
来源：http://cj.lnxyls.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hu.muxihuayi.cn

C#:   if (x is null) {}
来源：http://au.nicolike.cn

[P07] 防抖与节流
来源：http://gf.colortex.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://zh.yuexingan06.cn

PHP:  // 手写时间戳比较
来源：http://fu.shxzskj.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://zt.szxytkj.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ul.newstarts.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://rh.haigaiapp.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://so.nszjky.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://ee.colortex.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hn.nszjky.cn

[P08] 处理浮点精度问题
来源：http://gb.shxzukj.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wk.shxzskj.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mt.jianghongdianzi.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://go.9csxet.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://jx.bjjhwx.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mk.bjjhwx.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mb.nszjky.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://rs.bjjhwx.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://km.yuexingan06.cn

================================================================================
来源：http://mz.nicolike.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://cm.panjiajie.cn

================================================================================
来源：http://uv.shtwfgs.cn

[Q01] 创建表
来源：http://kj.asd995.cn

CREATE TABLE users (
来源：http://zv.bjjhwx.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://xe.hahajie.cn

name VARCHAR(50) NOT NULL,
来源：http://ix.asd995.cn

email VARCHAR(100) UNIQUE,
来源：http://jc.yuexingan06.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://xi.yuexingan06.cn

);
来源：http://tf.lnxyls.cn

[Q02] 创建带外键的表
来源：http://ue.haigaiapp.cn

CREATE TABLE orders (
来源：http://rw.huixiangedu.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://jv.huixiangedu.cn

user_id INT NOT NULL,
来源：http://yx.jctech888.com.cn

amount DECIMAL(10, 2),
来源：http://zn.jctech888.com.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ub.hnjuh.cn

);
来源：http://ia.hahajie.cn

[Q03] 增加列
来源：http://wr.bjjhwx.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://re.shxzukj.cn

[Q04] 修改列类型
来源：http://gs.shxzskj.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ev.chemitech.net.cn

[Q05] 重命名列
来源：http://ho.haigaiapp.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ge.shtwfgs.cn

[Q06] 删除列
来源：http://sf.521024.cn

ALTER TABLE users DROP COLUMN age;
来源：http://pp.newstarts.cn

[Q07] 删除表
来源：http://xp.hahajie.cn

DROP TABLE IF EXISTS orders;
来源：http://ub.jctech888.com.cn

[Q08] 创建普通索引
来源：http://ih.yuexingan06.cn


<!-- 参考信息 -->