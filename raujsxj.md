代发 wailian999

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://rq.bjjhwx.cn

Ruby: warn "err"
来源：http://tj.szsharing.cn

C#:   Console.Error.WriteLine("err")
来源：http://bu.hnjuh.cn

[M07] 判断是否为主入口
来源：http://ow.muxihuayi.cn

Py:   if __name__ == "__main__":
来源：http://wn.yuexingan06.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://td.colortex.cn

JS:   require.main === module
来源：http://uo.bjjhwx.cn

TS:   require.main === module
来源：http://qm.lnxyls.cn

Java: public static void main(String[] args)
来源：http://kf.521024.cn

Go:   func main()
来源：http://jz.huixinmuqiang.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ll.gzmigu.cn

C#:   static void Main(string[] args)
来源：http://eo.shxzukj.cn

[M08] 获取系统与运行时信息
来源：http://jf.hnjuh.cn

Py:   platform.system();  platform.python_version()
来源：http://zs.haigaiapp.cn

PHP:  PHP_OS;  phpversion();
来源：http://wg.colortex.cn

JS:   process.platform;  process.version
来源：http://og.521024.cn

TS:   process.platform;  process.version
来源：http://pu.huanxung.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://bx.haigaiapp.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://sp.szxytkj.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://qs.yuntaijiaju.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://dr.hahajie.cn

================================================================================
来源：http://pk.gzmigu.cn

N. 数据结构与算法
来源：http://dx.bookmarksfly.cn

================================================================================
来源：http://km.huixinmuqiang.cn

[N01] 二分查找（有序数组）
来源：http://dv.huixiangedu.cn

Py:   bisect.bisect_left(arr, x)
来源：http://qa.bookmarksfly.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://fv.panjiajie.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ov.nicolike.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://jp.9csxet.cn

Java: Arrays.binarySearch(arr, x)
来源：http://be.nicolike.cn

Go:   sort.SearchInts(arr, x)
来源：http://ul.lnxyls.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://ce.hahajie.cn

C#:   Array.BinarySearch(arr, x)
来源：http://ja.shxzukj.cn

[N02] 排序（工程实践用内置实现）
来源：http://te.521024.cn

Py:   sorted(arr);  arr.sort()
来源：http://rl.muxihuayi.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ab.haigaiapp.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://qx.wgjwhj.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://gp.9csxet.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ti.asd995.cn

Go:   slices.Sort(arr)
来源：http://rj.bjjhwx.cn

Ruby: arr.sort
来源：http://im.colortex.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://np.chemitech.net.cn

[N03] 快速排序（分治示例）
来源：http://hz.hnjuh.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://uk.asd995.cn

PHP:  // 递归实现，或用 usort
来源：http://qh.nicolike.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://yl.haigaiapp.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://xf.hnjuh.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://zj.szxytkj.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://xt.bookmarksfly.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wy.newstarts.cn

C#:   // 手写递归，或 Array.Sort
来源：http://om.huixiangedu.cn

[N04] 斐波那契数列
来源：http://vn.nicolike.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://xs.huixinmuqiang.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://pp.bookmarksfly.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://yw.gzmigu.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ai.nicolike.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://xl.lnxyls.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ji.wgjwhj.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ip.jctech888.com.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mz.bjjhwx.cn

[N05] 最大公约数
来源：http://zt.szsharing.cn

Py:   math.gcd(a, b)
来源：http://am.jctech888.com.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hh.wgjwhj.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://cc.bjjhwx.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ub.panjiajie.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ga.shtwfgs.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://oy.panjiajie.cn

Ruby: a.gcd(b)
来源：http://zl.shtwfgs.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://um.bjjhwx.cn

[N06] 判断回文字符串
来源：http://nq.szxytkj.cn

Py:   s == s[::-1]
来源：http://ga.newstarts.cn

PHP:  $s === strrev($s);
来源：http://km.yuexingan06.cn

JS:   s === [...s].reverse().join("")
来源：http://oc.haigaiapp.cn

TS:   s === [...s].reverse().join("")
来源：http://vi.9csxet.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ts.colortex.cn

Go:   // 双指针从两端比较
来源：http://fk.colortex.cn

Ruby: s == s.reverse
来源：http://cf.jctech888.com.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://wo.muxihuayi.cn

[N07] 两数之和（返回下标）
来源：http://cg.huixinmuqiang.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://fr.jianghongdianzi.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ey.panjiajie.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://pa.nicolike.cn

TS:   // 手写 Map<string, number>
来源：http://ng.szxytkj.cn

Java: // 手写 HashMap
来源：http://xe.hahajie.cn

Go:   // 手写 map[int]int
来源：http://qa.haigaiapp.cn

Ruby: // 手写 Hash
来源：http://zl.jctech888.com.cn

C#:   // 手写 Dictionary<int, int>
来源：http://aw.huixinmuqiang.cn

[N08] 生成全排列
来源：http://ry.yuexingan06.cn

Py:   itertools.permutations(arr)
来源：http://jv.huanxung.cn

PHP:  // 手写递归交换
来源：http://qk.nszjky.cn

JS:   // 手写回溯递归
来源：http://mk.asd995.cn

TS:   // 手写回溯递归
来源：http://sy.yuntaijiaju.cn

Java: // 手写回溯递归
来源：http://qz.wgjwhj.cn

Go:   // 手写回溯递归
来源：http://ad.shxzskj.cn

Ruby: arr.permutation.to_a
来源：http://qn.huanxung.cn

C#:   // 手写回溯递归
来源：http://oe.521024.cn

[N09] 栈与队列
来源：http://tx.yuexingan06.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://fp.lnxyls.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hf.jianghongdianzi.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://dk.lnxyls.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://rf.haigaiapp.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://qh.shxzskj.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://oh.panjiajie.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://qr.huanxung.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://jj.hahajie.cn

[N10] 链表节点定义
来源：http://th.szxytkj.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ai.9csxet.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://vv.bookmarksfly.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://rx.asd995.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://px.shxzskj.cn

Java: class Node { int v; Node next; }
来源：http://mx.gzmigu.cn

Go:   type Node struct { V int; Next *Node }
来源：http://rg.haigaiapp.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://oq.shtwfgs.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://im.hnjuh.cn

[N11] 二叉树中序遍历
来源：http://sh.huanxung.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://om.huanxung.cn

PHP:  // 手写递归函数
来源：http://bx.nszjky.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://zq.haigaiapp.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ek.yuexingan06.cn

Java: // 手写递归
来源：http://cz.shxzukj.cn

Go:   // 手写递归
来源：http://dq.haigaiapp.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://qd.huixinmuqiang.cn

C#:   // 手写递归
来源：http://pa.jianghongdianzi.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hj.colortex.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ha.jctech888.com.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ao.hahajie.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ge.9csxet.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://vk.panjiajie.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://pj.lnxyls.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://rb.bjjhwx.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ql.9csxet.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://vw.chemitech.net.cn

================================================================================
来源：http://vz.yuexingan06.cn

O. 并发与异步
来源：http://vr.colortex.cn

================================================================================
来源：http://jo.hnjuh.cn

[O01] 启动一个线程
来源：http://qz.shtwfgs.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ne.bjjhwx.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://qj.521024.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://vj.panjiajie.cn

TS:   // 同 JS
来源：http://kr.bjjhwx.cn

Java: new Thread(() -> f()).start()
来源：http://bu.muxihuayi.cn

Go:   go f()
来源：http://lg.shtwfgs.cn

Ruby: Thread.new { f }
来源：http://rn.huanxung.cn

C#:   Task.Run(() => F());
来源：http://wb.gzmigu.cn

[O02] 使用线程池
来源：http://pr.colortex.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wu.huixinmuqiang.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://nw.nicolike.cn

JS:   // worker_threads 线程池
来源：http://fh.yuntaijiaju.cn

TS:   // worker_threads 线程池
来源：http://xc.jctech888.com.cn

Java: Executors.newFixedThreadPool(4)
来源：http://wl.huanxung.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://lq.yuntaijiaju.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://md.asd995.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ga.newstarts.cn

[O03] 加锁保护共享数据
来源：http://gj.jianghongdianzi.cn

Py:   with lock: shared += 1
来源：http://wa.wgjwhj.cn

PHP:  // 用 flock() 做文件锁
来源：http://ao.gzmigu.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://bu.huanxung.cn

TS:   // 同 JS
来源：http://zy.huixiangedu.cn

Java: synchronized (this) { shared++; }
来源：http://qq.hahajie.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://dn.hahajie.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://oy.lnxyls.cn

C#:   lock (gate) { shared++; }
来源：http://hx.asd995.cn

[O04] 定义异步函数并等待
来源：http://vo.yuexingan06.cn

Py:   async def f():⏎    await g()
来源：http://zg.shtwfgs.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://if.newstarts.cn

JS:   async function f() { await g(); }
来源：http://wn.shxzskj.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://ld.hnjuh.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://av.hahajie.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hk.hahajie.cn

Ruby: # 用 Fiber 或 async gem
来源：http://iu.haigaiapp.cn

C#:   async Task F() { await G(); }
来源：http://fw.huixinmuqiang.cn

[O05] 并发执行并等待全部完成
来源：http://ek.bookmarksfly.cn

Py:   asyncio.gather(*tasks)
来源：http://yv.huixiangedu.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hd.521024.cn

JS:   await Promise.all(tasks)
来源：http://ky.nicolike.cn

TS:   await Promise.all(tasks)
来源：http://sd.szxytkj.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hk.huanxung.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://nr.nicolike.cn

Ruby: threads.map(&:join)
来源：http://js.hnjuh.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://nc.gzmigu.cn

[O06] 使用进程池
来源：http://ux.521024.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://nl.bookmarksfly.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://qd.lnxyls.cn

JS:   // child_process / cluster 模块
来源：http://il.shxzukj.cn

TS:   // child_process / cluster 模块
来源：http://nm.lnxyls.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://qs.nicolike.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://sd.yuntaijiaju.cn

Ruby: // fork 块
来源：http://ho.gzmigu.cn

C#:   Parallel.For
来源：http://fg.asd995.cn

================================================================================
来源：http://xh.lnxyls.cn

P. 常用工具函数
来源：http://it.jianghongdianzi.cn

================================================================================
来源：http://ah.lnxyls.cn

[P01] 生成 UUID
来源：http://ep.wgjwhj.cn

Py:   str(uuid.uuid4())
来源：http://dj.nszjky.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://cy.asd995.cn

JS:   crypto.randomUUID()
来源：http://ba.lnxyls.cn

TS:   crypto.randomUUID()
来源：http://jy.nicolike.cn

Java: UUID.randomUUID().toString()
来源：http://yn.huixiangedu.cn

Go:   // 用 github.com/google/uuid
来源：http://mb.hnjuh.cn

Ruby: SecureRandom.uuid
来源：http://ug.hnjuh.cn

C#:   Guid.NewGuid().ToString()
来源：http://jh.yuntaijiaju.cn

[P02] MD5 / SHA256 摘要
来源：http://vg.chemitech.net.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ed.panjiajie.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://ja.jctech888.com.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://jo.yuexingan06.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://fc.gzmigu.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ci.bookmarksfly.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://zg.nicolike.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://sa.haigaiapp.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://yz.shxzskj.cn

[P03] 生成短随机字符串
来源：http://yu.shxzukj.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://nz.jianghongdianzi.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://io.shtwfgs.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://fj.521024.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://rx.muxihuayi.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wo.muxihuayi.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://tu.szxytkj.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://gg.newstarts.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hn.nicolike.cn

[P04] 求长度
来源：http://es.panjiajie.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ua.jctech888.com.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://il.haigaiapp.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://yl.shxzukj.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://bh.haigaiapp.cn

Java: list.size();  map.size();  s.length()
来源：http://ay.gzmigu.cn

Go:   len(arr);  len(m)
来源：http://qc.huanxung.cn

Ruby: x.length;  x.size
来源：http://bp.nszjky.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://qq.lnxyls.cn

[P05] 判断两个对象内容是否相等
来源：http://lu.haigaiapp.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://pg.gzmigu.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://su.hnjuh.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hk.hnjuh.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://dk.shtwfgs.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://cu.bjjhwx.cn

Go:   reflect.DeepEqual(a, b)
来源：http://tl.colortex.cn

Ruby: a == b
来源：http://mj.nicolike.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://bq.shxzskj.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hc.huixiangedu.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://zq.panjiajie.cn

PHP:  if (empty($x)) {}
来源：http://dg.hnjuh.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wa.nszjky.cn

TS:   if (x == null) {}
来源：http://de.nicolike.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://rj.huixinmuqiang.cn

Go:   if x == nil {}
来源：http://wd.huixinmuqiang.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://cr.szxytkj.cn

C#:   if (x is null) {}
来源：http://sl.shxzskj.cn

[P07] 防抖与节流
来源：http://dj.nszjky.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ai.yuexingan06.cn

PHP:  // 手写时间戳比较
来源：http://sy.gzmigu.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://pr.szxytkj.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://sq.bjjhwx.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ot.szsharing.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://or.szxytkj.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://vh.bookmarksfly.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://lh.shxzukj.cn

[P08] 处理浮点精度问题
来源：http://nf.shxzskj.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hn.panjiajie.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://oh.jianghongdianzi.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://uw.gzmigu.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://kj.colortex.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://dy.szsharing.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://dw.jctech888.com.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://fu.jctech888.com.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://qz.colortex.cn

================================================================================
来源：http://hn.szsharing.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ai.szxytkj.cn

================================================================================
来源：http://xe.nicolike.cn

[Q01] 创建表
来源：http://nr.jianghongdianzi.cn

CREATE TABLE users (
来源：http://uc.521024.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://rn.wgjwhj.cn

name VARCHAR(50) NOT NULL,
来源：http://xo.colortex.cn

email VARCHAR(100) UNIQUE,
来源：http://df.colortex.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://lf.nicolike.cn

);
来源：http://zh.gzmigu.cn

[Q02] 创建带外键的表
来源：http://xl.hahajie.cn

CREATE TABLE orders (
来源：http://in.gzmigu.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://xm.hahajie.cn

user_id INT NOT NULL,
来源：http://bq.nicolike.cn

amount DECIMAL(10, 2),
来源：http://yi.shxzukj.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://yz.bookmarksfly.cn

);
来源：http://tw.asd995.cn

[Q03] 增加列
来源：http://pz.jctech888.com.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mt.wgjwhj.cn

[Q04] 修改列类型
来源：http://hr.newstarts.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://rv.shtwfgs.cn

[Q05] 重命名列
来源：http://rj.wgjwhj.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://zs.huixiangedu.cn

[Q06] 删除列
来源：http://is.jianghongdianzi.cn

ALTER TABLE users DROP COLUMN age;
来源：http://em.huixiangedu.cn

[Q07] 删除表
来源：http://uj.jctech888.com.cn

DROP TABLE IF EXISTS orders;
来源：http://df.newstarts.cn

[Q08] 创建普通索引
来源：http://as.panjiajie.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://os.panjiajie.cn

[Q09] 创建唯一索引
来源：http://dw.muxihuayi.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://yg.nszjky.cn

[Q10] 插入单行
来源：http://uu.muxihuayi.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://vm.newstarts.cn

[Q11] 一次插入多行
来源：http://qm.jianghongdianzi.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://xx.nicolike.cn

[Q12] 插入后取自增 ID
来源：http://ef.chemitech.net.cn


<!-- 参考信息 -->