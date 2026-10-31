代发 wailian999

C#:   Environment.OSVersion;  Environment.Version
来源：http://lc.szxytkj.cn

================================================================================
来源：http://sd.gzmigu.cn

N. 数据结构与算法
来源：http://mb.asd995.cn

================================================================================
来源：http://qo.hnjuh.cn

[N01] 二分查找（有序数组）
来源：http://jj.shtwfgs.cn

Py:   bisect.bisect_left(arr, x)
来源：http://ol.nicolike.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://oc.huixinmuqiang.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ki.yuntaijiaju.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://gl.newstarts.cn

Java: Arrays.binarySearch(arr, x)
来源：http://po.9csxet.cn

Go:   sort.SearchInts(arr, x)
来源：http://ib.jctech888.com.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://zr.newstarts.cn

C#:   Array.BinarySearch(arr, x)
来源：http://ag.shxzukj.cn

[N02] 排序（工程实践用内置实现）
来源：http://nd.huixiangedu.cn

Py:   sorted(arr);  arr.sort()
来源：http://qw.yuexingan06.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://qy.hahajie.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://bd.gzmigu.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://gv.lnxyls.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://kp.shxzskj.cn

Go:   slices.Sort(arr)
来源：http://sg.colortex.cn

Ruby: arr.sort
来源：http://md.521024.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://bz.colortex.cn

[N03] 快速排序（分治示例）
来源：http://fv.chemitech.net.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mi.muxihuayi.cn

PHP:  // 递归实现，或用 usort
来源：http://sc.huixinmuqiang.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ek.huanxung.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wy.yuexingan06.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hk.yuexingan06.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://lb.haigaiapp.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://jy.newstarts.cn

C#:   // 手写递归，或 Array.Sort
来源：http://wk.colortex.cn

[N04] 斐波那契数列
来源：http://ng.bjjhwx.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://bf.panjiajie.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wa.nszjky.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://tk.yuntaijiaju.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://uc.nicolike.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://zg.9csxet.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://xe.jctech888.com.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ch.szxytkj.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://fr.shtwfgs.cn

[N05] 最大公约数
来源：http://zi.haigaiapp.cn

Py:   math.gcd(a, b)
来源：http://gz.chemitech.net.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://xu.bookmarksfly.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://gv.szsharing.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://lh.wgjwhj.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://bv.jctech888.com.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://lk.wgjwhj.cn

Ruby: a.gcd(b)
来源：http://si.yuexingan06.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://gw.muxihuayi.cn

[N06] 判断回文字符串
来源：http://dr.huixiangedu.cn

Py:   s == s[::-1]
来源：http://ny.jctech888.com.cn

PHP:  $s === strrev($s);
来源：http://kt.yuntaijiaju.cn

JS:   s === [...s].reverse().join("")
来源：http://qq.jctech888.com.cn

TS:   s === [...s].reverse().join("")
来源：http://zh.9csxet.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://dy.9csxet.cn

Go:   // 双指针从两端比较
来源：http://rq.lnxyls.cn

Ruby: s == s.reverse
来源：http://nz.szsharing.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://ov.huixiangedu.cn

[N07] 两数之和（返回下标）
来源：http://od.huanxung.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://kz.nszjky.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ep.shxzskj.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://gj.lnxyls.cn

TS:   // 手写 Map<string, number>
来源：http://tp.yuexingan06.cn

Java: // 手写 HashMap
来源：http://ze.shtwfgs.cn

Go:   // 手写 map[int]int
来源：http://aq.bjjhwx.cn

Ruby: // 手写 Hash
来源：http://vx.wgjwhj.cn

C#:   // 手写 Dictionary<int, int>
来源：http://jz.haigaiapp.cn

[N08] 生成全排列
来源：http://js.jianghongdianzi.cn

Py:   itertools.permutations(arr)
来源：http://vc.szxytkj.cn

PHP:  // 手写递归交换
来源：http://uj.bjjhwx.cn

JS:   // 手写回溯递归
来源：http://pv.szxytkj.cn

TS:   // 手写回溯递归
来源：http://ex.hnjuh.cn

Java: // 手写回溯递归
来源：http://ck.gzmigu.cn

Go:   // 手写回溯递归
来源：http://ed.szsharing.cn

Ruby: arr.permutation.to_a
来源：http://yx.newstarts.cn

C#:   // 手写回溯递归
来源：http://mh.huanxung.cn

[N09] 栈与队列
来源：http://wy.huanxung.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://lb.shtwfgs.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://gm.newstarts.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://tu.huanxung.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://om.chemitech.net.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://pq.shxzskj.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ny.jianghongdianzi.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://iq.hahajie.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://la.chemitech.net.cn

[N10] 链表节点定义
来源：http://rz.nicolike.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://sc.yuexingan06.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://sf.hnjuh.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://eg.bjjhwx.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://rx.szsharing.cn

Java: class Node { int v; Node next; }
来源：http://jo.wgjwhj.cn

Go:   type Node struct { V int; Next *Node }
来源：http://zp.wgjwhj.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://hy.nicolike.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://xm.shxzskj.cn

[N11] 二叉树中序遍历
来源：http://qb.yuexingan06.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://bi.yuexingan06.cn

PHP:  // 手写递归函数
来源：http://wj.newstarts.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://jk.yuexingan06.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://nr.521024.cn

Java: // 手写递归
来源：http://vb.9csxet.cn

Go:   // 手写递归
来源：http://dw.haigaiapp.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ds.gzmigu.cn

C#:   // 手写递归
来源：http://ho.jianghongdianzi.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://xe.hnjuh.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://eq.jctech888.com.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://qc.muxihuayi.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://yy.nszjky.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://tj.newstarts.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://iu.bookmarksfly.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://yk.jctech888.com.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://bi.nszjky.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://dz.jctech888.com.cn

================================================================================
来源：http://lt.gzmigu.cn

O. 并发与异步
来源：http://is.muxihuayi.cn

================================================================================
来源：http://vr.hahajie.cn

[O01] 启动一个线程
来源：http://qq.bjjhwx.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://he.hahajie.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://xc.gzmigu.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://uj.gzmigu.cn

TS:   // 同 JS
来源：http://or.wgjwhj.cn

Java: new Thread(() -> f()).start()
来源：http://gf.521024.cn

Go:   go f()
来源：http://wf.nszjky.cn

Ruby: Thread.new { f }
来源：http://gi.szsharing.cn

C#:   Task.Run(() => F());
来源：http://jb.panjiajie.cn

[O02] 使用线程池
来源：http://gh.shtwfgs.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://vn.shtwfgs.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hd.shtwfgs.cn

JS:   // worker_threads 线程池
来源：http://fz.hahajie.cn

TS:   // worker_threads 线程池
来源：http://kj.nszjky.cn

Java: Executors.newFixedThreadPool(4)
来源：http://cy.huixinmuqiang.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://rc.chemitech.net.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://pb.yuexingan06.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://zv.hnjuh.cn

[O03] 加锁保护共享数据
来源：http://lr.chemitech.net.cn

Py:   with lock: shared += 1
来源：http://nn.lnxyls.cn

PHP:  // 用 flock() 做文件锁
来源：http://hc.shxzukj.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ja.521024.cn

TS:   // 同 JS
来源：http://yr.521024.cn

Java: synchronized (this) { shared++; }
来源：http://ko.shxzskj.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://yn.colortex.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://ds.panjiajie.cn

C#:   lock (gate) { shared++; }
来源：http://yx.lnxyls.cn

[O04] 定义异步函数并等待
来源：http://eh.hahajie.cn

Py:   async def f():⏎    await g()
来源：http://tn.bjjhwx.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wb.jianghongdianzi.cn

JS:   async function f() { await g(); }
来源：http://nq.chemitech.net.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://np.wgjwhj.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://gz.gzmigu.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://pz.9csxet.cn

Ruby: # 用 Fiber 或 async gem
来源：http://ot.gzmigu.cn

C#:   async Task F() { await G(); }
来源：http://kl.newstarts.cn

[O05] 并发执行并等待全部完成
来源：http://ni.newstarts.cn

Py:   asyncio.gather(*tasks)
来源：http://gh.newstarts.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://jv.jianghongdianzi.cn

JS:   await Promise.all(tasks)
来源：http://jp.nszjky.cn

TS:   await Promise.all(tasks)
来源：http://wq.hahajie.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ya.nicolike.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mx.nicolike.cn

Ruby: threads.map(&:join)
来源：http://gk.huixiangedu.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://ye.wgjwhj.cn

[O06] 使用进程池
来源：http://yx.bookmarksfly.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://kf.haigaiapp.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://gs.huixiangedu.cn

JS:   // child_process / cluster 模块
来源：http://yc.haigaiapp.cn

TS:   // child_process / cluster 模块
来源：http://vr.bookmarksfly.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://vc.nszjky.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://zh.jianghongdianzi.cn

Ruby: // fork 块
来源：http://oz.newstarts.cn

C#:   Parallel.For
来源：http://dz.szxytkj.cn

================================================================================
来源：http://xu.panjiajie.cn

P. 常用工具函数
来源：http://in.yuntaijiaju.cn

================================================================================
来源：http://rf.chemitech.net.cn

[P01] 生成 UUID
来源：http://dr.szxytkj.cn

Py:   str(uuid.uuid4())
来源：http://dt.nszjky.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://dq.lnxyls.cn

JS:   crypto.randomUUID()
来源：http://wk.szsharing.cn

TS:   crypto.randomUUID()
来源：http://qz.bjjhwx.cn

Java: UUID.randomUUID().toString()
来源：http://iq.szxytkj.cn

Go:   // 用 github.com/google/uuid
来源：http://ew.haigaiapp.cn

Ruby: SecureRandom.uuid
来源：http://vi.9csxet.cn

C#:   Guid.NewGuid().ToString()
来源：http://ek.shxzskj.cn

[P02] MD5 / SHA256 摘要
来源：http://xu.muxihuayi.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://oo.colortex.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.jianghongdianzi.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://gb.hahajie.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hc.haigaiapp.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wm.newstarts.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://xk.521024.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://pg.newstarts.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://yh.nszjky.cn

[P03] 生成短随机字符串
来源：http://qh.hnjuh.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://yy.szxytkj.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ec.huanxung.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ej.shxzskj.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://vb.asd995.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://rs.nszjky.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://zy.huixiangedu.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://hj.521024.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://zc.nszjky.cn

[P04] 求长度
来源：http://ih.huixiangedu.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mw.huanxung.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://gz.szxytkj.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://dj.haigaiapp.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://en.jctech888.com.cn

Java: list.size();  map.size();  s.length()
来源：http://ar.hahajie.cn

Go:   len(arr);  len(m)
来源：http://sy.asd995.cn

Ruby: x.length;  x.size
来源：http://bb.hnjuh.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://yz.gzmigu.cn

[P05] 判断两个对象内容是否相等
来源：http://hf.nszjky.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://zd.colortex.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://bj.asd995.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ft.szsharing.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ix.521024.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://yn.muxihuayi.cn

Go:   reflect.DeepEqual(a, b)
来源：http://zo.jianghongdianzi.cn

Ruby: a == b
来源：http://ki.gzmigu.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://df.shxzskj.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://zz.hnjuh.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://tv.huixinmuqiang.cn

PHP:  if (empty($x)) {}
来源：http://ce.nszjky.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://lz.haigaiapp.cn

TS:   if (x == null) {}
来源：http://jt.shxzskj.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://je.9csxet.cn

Go:   if x == nil {}
来源：http://sm.shtwfgs.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://lg.asd995.cn

C#:   if (x is null) {}
来源：http://yd.bookmarksfly.cn

[P07] 防抖与节流
来源：http://pa.huanxung.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://cp.huanxung.cn

PHP:  // 手写时间戳比较
来源：http://ie.huixinmuqiang.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://kw.bjjhwx.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://fm.hahajie.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://uh.hnjuh.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://nx.bookmarksfly.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://dm.huixiangedu.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://pa.nszjky.cn

[P08] 处理浮点精度问题
来源：http://ps.huanxung.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://vc.wgjwhj.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ql.newstarts.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://eb.yuexingan06.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://pl.bjjhwx.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://qs.521024.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://iu.hnjuh.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://aj.shxzskj.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://qu.chemitech.net.cn

================================================================================
来源：http://tc.jianghongdianzi.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://pp.shtwfgs.cn

================================================================================
来源：http://uf.jianghongdianzi.cn

[Q01] 创建表
来源：http://uo.szsharing.cn

CREATE TABLE users (
来源：http://ze.shxzukj.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://lg.yuntaijiaju.cn

name VARCHAR(50) NOT NULL,
来源：http://bt.shxzskj.cn

email VARCHAR(100) UNIQUE,
来源：http://dp.shxzskj.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://yd.asd995.cn

);
来源：http://nz.asd995.cn

[Q02] 创建带外键的表
来源：http://dd.colortex.cn

CREATE TABLE orders (
来源：http://bl.lnxyls.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://un.yuntaijiaju.cn

user_id INT NOT NULL,
来源：http://tb.bookmarksfly.cn

amount DECIMAL(10, 2),
来源：http://fu.huixinmuqiang.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ns.yuntaijiaju.cn

);
来源：http://rc.9csxet.cn

[Q03] 增加列
来源：http://ha.wgjwhj.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://en.bookmarksfly.cn

[Q04] 修改列类型
来源：http://fs.521024.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://tb.yuexingan06.cn

[Q05] 重命名列
来源：http://go.nszjky.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://aj.asd995.cn

[Q06] 删除列
来源：http://nj.nicolike.cn

ALTER TABLE users DROP COLUMN age;
来源：http://kr.9csxet.cn

[Q07] 删除表
来源：http://fe.newstarts.cn

DROP TABLE IF EXISTS orders;
来源：http://fi.shtwfgs.cn

[Q08] 创建普通索引
来源：http://xf.muxihuayi.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://pg.bjjhwx.cn

[Q09] 创建唯一索引
来源：http://wo.bjjhwx.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://br.szsharing.cn

[Q10] 插入单行
来源：http://vh.huanxung.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ce.jianghongdianzi.cn

[Q11] 一次插入多行
来源：http://ht.wgjwhj.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://qz.szxytkj.cn

[Q12] 插入后取自增 ID
来源：http://hq.9csxet.cn

INSERT INTO users (name) VALUES ('C');
来源：http://qw.shxzskj.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://fl.huixinmuqiang.cn

[Q13] 忽略重复插入
来源：http://qp.asd995.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://qv.panjiajie.cn

[Q14] 存在则更新（upsert）
来源：http://tl.chemitech.net.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://fd.nicolike.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ek.colortex.cn

[Q15] 查询全部
来源：http://eq.521024.cn

SELECT * FROM users;
来源：http://ot.haigaiapp.cn

[Q16] 查询指定列
来源：http://ro.jianghongdianzi.cn

SELECT id, name FROM users;
来源：http://cg.wgjwhj.cn

[Q17] 条件查询
来源：http://vn.bookmarksfly.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://jy.lnxyls.cn

[Q18] 模糊匹配
来源：http://cf.shtwfgs.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://oa.colortex.cn

[Q19] 范围查询
来源：http://ah.gzmigu.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://so.bjjhwx.cn

[Q20] IN 列表
来源：http://js.yuntaijiaju.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://lb.muxihuayi.cn

[Q21] 空值判断
来源：http://jw.muxihuayi.cn


<!-- 参考信息 -->