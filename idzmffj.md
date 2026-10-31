代发 wailian999

C#:   Environment.OSVersion;  Environment.Version
来源：http://cj.hnjuh.cn

================================================================================
来源：http://zr.jctech888.com.cn

N. 数据结构与算法
来源：http://yx.hahajie.cn

================================================================================
来源：http://fm.jctech888.com.cn

[N01] 二分查找（有序数组）
来源：http://fm.hnjuh.cn

Py:   bisect.bisect_left(arr, x)
来源：http://cu.9csxet.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://nx.521024.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://pg.521024.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://bw.asd995.cn

Java: Arrays.binarySearch(arr, x)
来源：http://ki.shxzukj.cn

Go:   sort.SearchInts(arr, x)
来源：http://nx.szxytkj.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://qv.shxzukj.cn

C#:   Array.BinarySearch(arr, x)
来源：http://hg.muxihuayi.cn

[N02] 排序（工程实践用内置实现）
来源：http://me.lnxyls.cn

Py:   sorted(arr);  arr.sort()
来源：http://mj.bjjhwx.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://nw.huixiangedu.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://am.hahajie.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://wq.nicolike.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://pb.szsharing.cn

Go:   slices.Sort(arr)
来源：http://gj.chemitech.net.cn

Ruby: arr.sort
来源：http://ew.shxzskj.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://iu.521024.cn

[N03] 快速排序（分治示例）
来源：http://te.9csxet.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mc.shxzukj.cn

PHP:  // 递归实现，或用 usort
来源：http://ji.bjjhwx.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://br.huanxung.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://pj.szxytkj.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://nm.hahajie.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://by.colortex.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://fp.haigaiapp.cn

C#:   // 手写递归，或 Array.Sort
来源：http://lm.huanxung.cn

[N04] 斐波那契数列
来源：http://fx.panjiajie.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ab.bjjhwx.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://xr.yuntaijiaju.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://rd.newstarts.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wj.haigaiapp.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://jz.lnxyls.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://kd.szsharing.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://fr.jctech888.com.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://vz.nicolike.cn

[N05] 最大公约数
来源：http://my.521024.cn

Py:   math.gcd(a, b)
来源：http://sj.colortex.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://yc.lnxyls.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mr.haigaiapp.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://lw.huixinmuqiang.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://br.asd995.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://da.hahajie.cn

Ruby: a.gcd(b)
来源：http://xz.lnxyls.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://au.huanxung.cn

[N06] 判断回文字符串
来源：http://xf.hnjuh.cn

Py:   s == s[::-1]
来源：http://kq.9csxet.cn

PHP:  $s === strrev($s);
来源：http://tc.muxihuayi.cn

JS:   s === [...s].reverse().join("")
来源：http://nm.9csxet.cn

TS:   s === [...s].reverse().join("")
来源：http://gf.colortex.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ic.wgjwhj.cn

Go:   // 双指针从两端比较
来源：http://go.nszjky.cn

Ruby: s == s.reverse
来源：http://bk.shxzukj.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://zp.gzmigu.cn

[N07] 两数之和（返回下标）
来源：http://bj.jianghongdianzi.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://dw.chemitech.net.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://cs.huixinmuqiang.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://db.521024.cn

TS:   // 手写 Map<string, number>
来源：http://du.521024.cn

Java: // 手写 HashMap
来源：http://mb.521024.cn

Go:   // 手写 map[int]int
来源：http://pu.newstarts.cn

Ruby: // 手写 Hash
来源：http://nn.hahajie.cn

C#:   // 手写 Dictionary<int, int>
来源：http://nb.huanxung.cn

[N08] 生成全排列
来源：http://to.jctech888.com.cn

Py:   itertools.permutations(arr)
来源：http://hw.bjjhwx.cn

PHP:  // 手写递归交换
来源：http://ik.newstarts.cn

JS:   // 手写回溯递归
来源：http://cv.shxzukj.cn

TS:   // 手写回溯递归
来源：http://ui.bookmarksfly.cn

Java: // 手写回溯递归
来源：http://me.wgjwhj.cn

Go:   // 手写回溯递归
来源：http://wi.hnjuh.cn

Ruby: arr.permutation.to_a
来源：http://rk.chemitech.net.cn

C#:   // 手写回溯递归
来源：http://oq.jctech888.com.cn

[N09] 栈与队列
来源：http://ps.lnxyls.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://xq.newstarts.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://sy.haigaiapp.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://oc.nszjky.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://pw.bjjhwx.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ya.szsharing.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ul.colortex.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://fj.panjiajie.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ni.nicolike.cn

[N10] 链表节点定义
来源：http://yx.szxytkj.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://nz.shxzukj.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://tj.szxytkj.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ty.jctech888.com.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://cw.szsharing.cn

Java: class Node { int v; Node next; }
来源：http://mk.muxihuayi.cn

Go:   type Node struct { V int; Next *Node }
来源：http://yx.bookmarksfly.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://cr.wgjwhj.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://uz.jctech888.com.cn

[N11] 二叉树中序遍历
来源：http://pw.bjjhwx.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://io.huanxung.cn

PHP:  // 手写递归函数
来源：http://xl.bookmarksfly.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://bt.chemitech.net.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mv.shxzskj.cn

Java: // 手写递归
来源：http://au.nszjky.cn

Go:   // 手写递归
来源：http://qf.lnxyls.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://md.jctech888.com.cn

C#:   // 手写递归
来源：http://gv.haigaiapp.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://rj.huanxung.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://fy.huanxung.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://yl.bjjhwx.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://xd.huanxung.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ra.asd995.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://th.shxzukj.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://cq.9csxet.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://kb.hahajie.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://vb.szxytkj.cn

================================================================================
来源：http://vf.bookmarksfly.cn

O. 并发与异步
来源：http://qe.yuexingan06.cn

================================================================================
来源：http://wy.asd995.cn

[O01] 启动一个线程
来源：http://ll.hahajie.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://cl.huanxung.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://zf.9csxet.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mo.colortex.cn

TS:   // 同 JS
来源：http://nv.shtwfgs.cn

Java: new Thread(() -> f()).start()
来源：http://uo.bookmarksfly.cn

Go:   go f()
来源：http://iy.shtwfgs.cn

Ruby: Thread.new { f }
来源：http://zk.nszjky.cn

C#:   Task.Run(() => F());
来源：http://rn.muxihuayi.cn

[O02] 使用线程池
来源：http://kz.nszjky.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://az.colortex.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://sv.panjiajie.cn

JS:   // worker_threads 线程池
来源：http://uq.jctech888.com.cn

TS:   // worker_threads 线程池
来源：http://jt.9csxet.cn

Java: Executors.newFixedThreadPool(4)
来源：http://xv.muxihuayi.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://qh.asd995.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://lg.wgjwhj.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://fv.wgjwhj.cn

[O03] 加锁保护共享数据
来源：http://xs.jctech888.com.cn

Py:   with lock: shared += 1
来源：http://vc.bookmarksfly.cn

PHP:  // 用 flock() 做文件锁
来源：http://jx.nszjky.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ef.yuexingan06.cn

TS:   // 同 JS
来源：http://rq.jianghongdianzi.cn

Java: synchronized (this) { shared++; }
来源：http://kc.bookmarksfly.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://om.newstarts.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://zs.shxzukj.cn

C#:   lock (gate) { shared++; }
来源：http://qw.huixiangedu.cn

[O04] 定义异步函数并等待
来源：http://hz.521024.cn

Py:   async def f():⏎    await g()
来源：http://ki.shxzukj.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ok.hnjuh.cn

JS:   async function f() { await g(); }
来源：http://hd.9csxet.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://cf.jianghongdianzi.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mc.nszjky.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://jq.newstarts.cn

Ruby: # 用 Fiber 或 async gem
来源：http://kv.nszjky.cn

C#:   async Task F() { await G(); }
来源：http://xx.wgjwhj.cn

[O05] 并发执行并等待全部完成
来源：http://ul.shtwfgs.cn

Py:   asyncio.gather(*tasks)
来源：http://lj.shtwfgs.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://po.521024.cn

JS:   await Promise.all(tasks)
来源：http://us.yuexingan06.cn

TS:   await Promise.all(tasks)
来源：http://mo.shxzskj.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://kh.nicolike.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://xw.colortex.cn

Ruby: threads.map(&:join)
来源：http://gd.huixinmuqiang.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://oi.szsharing.cn

[O06] 使用进程池
来源：http://ea.jianghongdianzi.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://gx.haigaiapp.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://po.521024.cn

JS:   // child_process / cluster 模块
来源：http://ql.huixiangedu.cn

TS:   // child_process / cluster 模块
来源：http://yn.lnxyls.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://za.hahajie.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://zd.panjiajie.cn

Ruby: // fork 块
来源：http://yg.nicolike.cn

C#:   Parallel.For
来源：http://vv.huixinmuqiang.cn

================================================================================
来源：http://jc.huixinmuqiang.cn

P. 常用工具函数
来源：http://ye.bjjhwx.cn

================================================================================
来源：http://vd.hahajie.cn

[P01] 生成 UUID
来源：http://qk.asd995.cn

Py:   str(uuid.uuid4())
来源：http://uh.gzmigu.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://gh.nszjky.cn

JS:   crypto.randomUUID()
来源：http://xw.chemitech.net.cn

TS:   crypto.randomUUID()
来源：http://iu.yuntaijiaju.cn

Java: UUID.randomUUID().toString()
来源：http://yc.nszjky.cn

Go:   // 用 github.com/google/uuid
来源：http://hx.haigaiapp.cn

Ruby: SecureRandom.uuid
来源：http://gm.haigaiapp.cn

C#:   Guid.NewGuid().ToString()
来源：http://hj.hnjuh.cn

[P02] MD5 / SHA256 摘要
来源：http://di.nszjky.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://lw.9csxet.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://zc.chemitech.net.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://nc.shtwfgs.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://vz.newstarts.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://uc.yuntaijiaju.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://cy.huixiangedu.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://nv.huixiangedu.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://of.yuntaijiaju.cn

[P03] 生成短随机字符串
来源：http://hm.shxzukj.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://rz.huanxung.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://fu.hnjuh.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://dh.jianghongdianzi.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://iv.wgjwhj.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ht.521024.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://to.yuexingan06.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://iz.huanxung.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://vb.nszjky.cn

[P04] 求长度
来源：http://np.muxihuayi.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://xf.hahajie.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ad.hnjuh.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://yg.bookmarksfly.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ov.hnjuh.cn

Java: list.size();  map.size();  s.length()
来源：http://ai.szxytkj.cn

Go:   len(arr);  len(m)
来源：http://ml.shtwfgs.cn

Ruby: x.length;  x.size
来源：http://qz.bjjhwx.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://ym.9csxet.cn

[P05] 判断两个对象内容是否相等
来源：http://kp.huixiangedu.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://se.muxihuayi.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wk.yuexingan06.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://px.panjiajie.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ub.jianghongdianzi.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://bs.jctech888.com.cn

Go:   reflect.DeepEqual(a, b)
来源：http://mp.haigaiapp.cn

Ruby: a == b
来源：http://cf.szxytkj.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://xq.yuntaijiaju.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://iw.panjiajie.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://pz.shxzukj.cn

PHP:  if (empty($x)) {}
来源：http://cu.shtwfgs.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://gi.haigaiapp.cn

TS:   if (x == null) {}
来源：http://zt.asd995.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://uf.chemitech.net.cn

Go:   if x == nil {}
来源：http://cy.chemitech.net.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ag.haigaiapp.cn

C#:   if (x is null) {}
来源：http://fp.jctech888.com.cn

[P07] 防抖与节流
来源：http://ps.haigaiapp.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ij.muxihuayi.cn

PHP:  // 手写时间戳比较
来源：http://ec.newstarts.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://yz.panjiajie.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://dp.panjiajie.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://rh.bookmarksfly.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ud.hahajie.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://gw.shxzukj.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://qt.yuexingan06.cn

[P08] 处理浮点精度问题
来源：http://uo.gzmigu.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://vj.wgjwhj.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://dn.chemitech.net.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hy.szsharing.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://pi.huixiangedu.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://um.yuntaijiaju.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ki.muxihuayi.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://jb.gzmigu.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://xc.bjjhwx.cn

================================================================================
来源：http://lr.shxzukj.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://sd.hnjuh.cn

================================================================================
来源：http://uu.521024.cn

[Q01] 创建表
来源：http://oh.colortex.cn

CREATE TABLE users (
来源：http://jc.colortex.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://xi.muxihuayi.cn

name VARCHAR(50) NOT NULL,
来源：http://br.hnjuh.cn

email VARCHAR(100) UNIQUE,
来源：http://oc.shxzukj.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://dd.muxihuayi.cn

);
来源：http://wl.szsharing.cn

[Q02] 创建带外键的表
来源：http://ua.huixinmuqiang.cn

CREATE TABLE orders (
来源：http://rp.huixinmuqiang.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ye.haigaiapp.cn

user_id INT NOT NULL,
来源：http://ym.jctech888.com.cn

amount DECIMAL(10, 2),
来源：http://an.yuntaijiaju.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wc.9csxet.cn

);
来源：http://uf.haigaiapp.cn

[Q03] 增加列
来源：http://wv.gzmigu.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://bv.nicolike.cn

[Q04] 修改列类型
来源：http://mn.lnxyls.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://in.521024.cn

[Q05] 重命名列
来源：http://wo.9csxet.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://vy.shxzukj.cn

[Q06] 删除列
来源：http://at.shtwfgs.cn

ALTER TABLE users DROP COLUMN age;
来源：http://ug.9csxet.cn

[Q07] 删除表
来源：http://mt.jianghongdianzi.cn

DROP TABLE IF EXISTS orders;
来源：http://qy.newstarts.cn

[Q08] 创建普通索引
来源：http://po.lnxyls.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://jg.shxzukj.cn

[Q09] 创建唯一索引
来源：http://ic.hahajie.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://jf.hahajie.cn

[Q10] 插入单行
来源：http://bu.nicolike.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://gc.huixiangedu.cn

[Q11] 一次插入多行
来源：http://ns.jctech888.com.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://xg.newstarts.cn

[Q12] 插入后取自增 ID
来源：http://vo.huixinmuqiang.cn

INSERT INTO users (name) VALUES ('C');
来源：http://ew.shxzskj.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://fi.huixiangedu.cn

[Q13] 忽略重复插入
来源：http://ph.bookmarksfly.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://gp.shtwfgs.cn

[Q14] 存在则更新（upsert）
来源：http://ji.asd995.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://as.colortex.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://yg.shtwfgs.cn

[Q15] 查询全部
来源：http://te.wgjwhj.cn

SELECT * FROM users;
来源：http://nw.nicolike.cn

[Q16] 查询指定列
来源：http://rs.shxzukj.cn

SELECT id, name FROM users;
来源：http://hp.muxihuayi.cn

[Q17] 条件查询
来源：http://mx.muxihuayi.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://gu.9csxet.cn

[Q18] 模糊匹配
来源：http://sb.jianghongdianzi.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://sh.bjjhwx.cn

[Q19] 范围查询
来源：http://bs.yuntaijiaju.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://pk.panjiajie.cn

[Q20] IN 列表
来源：http://fu.bookmarksfly.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://xv.szsharing.cn

[Q21] 空值判断
来源：http://nt.szsharing.cn


<!-- 参考信息 -->