代发 wailian999

C#:   Environment.OSVersion;  Environment.Version
来源：http://im.huixinmuqiang.cn

================================================================================
来源：http://zv.szsharing.cn

N. 数据结构与算法
来源：http://gh.yuntaijiaju.cn

================================================================================
来源：http://kc.huixinmuqiang.cn

[N01] 二分查找（有序数组）
来源：http://pn.hahajie.cn

Py:   bisect.bisect_left(arr, x)
来源：http://kt.huixinmuqiang.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://sy.9csxet.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://xy.521024.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ez.hahajie.cn

Java: Arrays.binarySearch(arr, x)
来源：http://pe.huanxung.cn

Go:   sort.SearchInts(arr, x)
来源：http://hj.szsharing.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://ju.gzmigu.cn

C#:   Array.BinarySearch(arr, x)
来源：http://qa.yuexingan06.cn

[N02] 排序（工程实践用内置实现）
来源：http://lg.huanxung.cn

Py:   sorted(arr);  arr.sort()
来源：http://ev.asd995.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://eb.521024.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://pk.asd995.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://jk.nicolike.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://us.wgjwhj.cn

Go:   slices.Sort(arr)
来源：http://hl.szsharing.cn

Ruby: arr.sort
来源：http://ac.9csxet.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://xa.huixiangedu.cn

[N03] 快速排序（分治示例）
来源：http://tw.shxzskj.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://uw.nszjky.cn

PHP:  // 递归实现，或用 usort
来源：http://ar.yuntaijiaju.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://av.jctech888.com.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mt.szxytkj.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://zo.huanxung.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://lg.bookmarksfly.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://en.jianghongdianzi.cn

C#:   // 手写递归，或 Array.Sort
来源：http://oo.jianghongdianzi.cn

[N04] 斐波那契数列
来源：http://nk.szsharing.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://iu.shtwfgs.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ll.huixiangedu.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mw.yuntaijiaju.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://gw.shtwfgs.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://xq.gzmigu.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ff.szxytkj.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://br.szsharing.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://th.yuntaijiaju.cn

[N05] 最大公约数
来源：http://ve.shxzukj.cn

Py:   math.gcd(a, b)
来源：http://qh.colortex.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ev.bjjhwx.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://zu.chemitech.net.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://gi.nicolike.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://oa.colortex.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://uf.lnxyls.cn

Ruby: a.gcd(b)
来源：http://dk.yuexingan06.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hf.nicolike.cn

[N06] 判断回文字符串
来源：http://ay.shxzskj.cn

Py:   s == s[::-1]
来源：http://id.huixinmuqiang.cn

PHP:  $s === strrev($s);
来源：http://rp.huixiangedu.cn

JS:   s === [...s].reverse().join("")
来源：http://ee.muxihuayi.cn

TS:   s === [...s].reverse().join("")
来源：http://is.szxytkj.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://he.9csxet.cn

Go:   // 双指针从两端比较
来源：http://an.hnjuh.cn

Ruby: s == s.reverse
来源：http://pt.haigaiapp.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://sj.nszjky.cn

[N07] 两数之和（返回下标）
来源：http://au.colortex.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wr.jianghongdianzi.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://yi.hahajie.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://hh.shxzskj.cn

TS:   // 手写 Map<string, number>
来源：http://ry.chemitech.net.cn

Java: // 手写 HashMap
来源：http://ft.yuntaijiaju.cn

Go:   // 手写 map[int]int
来源：http://wy.huixiangedu.cn

Ruby: // 手写 Hash
来源：http://od.bookmarksfly.cn

C#:   // 手写 Dictionary<int, int>
来源：http://yg.szsharing.cn

[N08] 生成全排列
来源：http://ht.yuntaijiaju.cn

Py:   itertools.permutations(arr)
来源：http://vp.jianghongdianzi.cn

PHP:  // 手写递归交换
来源：http://hw.hahajie.cn

JS:   // 手写回溯递归
来源：http://lb.wgjwhj.cn

TS:   // 手写回溯递归
来源：http://jt.hnjuh.cn

Java: // 手写回溯递归
来源：http://rz.shxzskj.cn

Go:   // 手写回溯递归
来源：http://lk.hnjuh.cn

Ruby: arr.permutation.to_a
来源：http://if.shtwfgs.cn

C#:   // 手写回溯递归
来源：http://xx.bjjhwx.cn

[N09] 栈与队列
来源：http://gp.szxytkj.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mt.jianghongdianzi.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ed.hahajie.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://qm.huixiangedu.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://qn.gzmigu.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://bp.nszjky.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ti.chemitech.net.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ez.wgjwhj.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://kk.nicolike.cn

[N10] 链表节点定义
来源：http://ih.szxytkj.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://dt.wgjwhj.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://mb.nszjky.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wq.huixinmuqiang.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://xy.bookmarksfly.cn

Java: class Node { int v; Node next; }
来源：http://oi.haigaiapp.cn

Go:   type Node struct { V int; Next *Node }
来源：http://tj.gzmigu.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://eh.szxytkj.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://ll.asd995.cn

[N11] 二叉树中序遍历
来源：http://dv.9csxet.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://tp.newstarts.cn

PHP:  // 手写递归函数
来源：http://om.gzmigu.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ze.521024.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://as.wgjwhj.cn

Java: // 手写递归
来源：http://wt.lnxyls.cn

Go:   // 手写递归
来源：http://al.panjiajie.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://km.9csxet.cn

C#:   // 手写递归
来源：http://tt.panjiajie.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://nh.huixiangedu.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://rn.chemitech.net.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://db.muxihuayi.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://gu.shxzskj.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hh.haigaiapp.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mo.huixiangedu.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ai.nszjky.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wb.jianghongdianzi.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://zt.hahajie.cn

================================================================================
来源：http://nt.9csxet.cn

O. 并发与异步
来源：http://kj.asd995.cn

================================================================================
来源：http://un.lnxyls.cn

[O01] 启动一个线程
来源：http://mq.bookmarksfly.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://cg.hnjuh.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://rg.jctech888.com.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://rq.lnxyls.cn

TS:   // 同 JS
来源：http://vs.huanxung.cn

Java: new Thread(() -> f()).start()
来源：http://eo.huanxung.cn

Go:   go f()
来源：http://mw.muxihuayi.cn

Ruby: Thread.new { f }
来源：http://qn.gzmigu.cn

C#:   Task.Run(() => F());
来源：http://te.colortex.cn

[O02] 使用线程池
来源：http://gi.yuntaijiaju.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://dj.shxzukj.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://tj.szsharing.cn

JS:   // worker_threads 线程池
来源：http://ie.huanxung.cn

TS:   // worker_threads 线程池
来源：http://ik.shxzskj.cn

Java: Executors.newFixedThreadPool(4)
来源：http://kq.newstarts.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://rj.nszjky.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ho.panjiajie.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://qq.hnjuh.cn

[O03] 加锁保护共享数据
来源：http://lg.huixinmuqiang.cn

Py:   with lock: shared += 1
来源：http://oy.asd995.cn

PHP:  // 用 flock() 做文件锁
来源：http://lr.hahajie.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://uy.shxzukj.cn

TS:   // 同 JS
来源：http://yv.huixiangedu.cn

Java: synchronized (this) { shared++; }
来源：http://mv.szsharing.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://qp.szsharing.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://vr.huixiangedu.cn

C#:   lock (gate) { shared++; }
来源：http://bg.wgjwhj.cn

[O04] 定义异步函数并等待
来源：http://oi.szxytkj.cn

Py:   async def f():⏎    await g()
来源：http://df.shxzukj.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://og.jianghongdianzi.cn

JS:   async function f() { await g(); }
来源：http://yh.521024.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://be.lnxyls.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://bg.shxzskj.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://bb.jianghongdianzi.cn

Ruby: # 用 Fiber 或 async gem
来源：http://au.nszjky.cn

C#:   async Task F() { await G(); }
来源：http://ti.szsharing.cn

[O05] 并发执行并等待全部完成
来源：http://bo.yuexingan06.cn

Py:   asyncio.gather(*tasks)
来源：http://ff.yuexingan06.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://vr.lnxyls.cn

JS:   await Promise.all(tasks)
来源：http://ix.huixinmuqiang.cn

TS:   await Promise.all(tasks)
来源：http://sk.shxzskj.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ph.muxihuayi.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://gf.shxzukj.cn

Ruby: threads.map(&:join)
来源：http://yw.lnxyls.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://fd.yuntaijiaju.cn

[O06] 使用进程池
来源：http://tr.muxihuayi.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ma.huixiangedu.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://cc.nicolike.cn

JS:   // child_process / cluster 模块
来源：http://vo.lnxyls.cn

TS:   // child_process / cluster 模块
来源：http://am.wgjwhj.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://in.hnjuh.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://jp.newstarts.cn

Ruby: // fork 块
来源：http://an.asd995.cn

C#:   Parallel.For
来源：http://jz.shxzskj.cn

================================================================================
来源：http://he.chemitech.net.cn

P. 常用工具函数
来源：http://qe.huanxung.cn

================================================================================
来源：http://ii.shxzskj.cn

[P01] 生成 UUID
来源：http://bj.szsharing.cn

Py:   str(uuid.uuid4())
来源：http://bg.huixiangedu.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://km.yuexingan06.cn

JS:   crypto.randomUUID()
来源：http://gm.gzmigu.cn

TS:   crypto.randomUUID()
来源：http://ip.huixiangedu.cn

Java: UUID.randomUUID().toString()
来源：http://nv.shxzukj.cn

Go:   // 用 github.com/google/uuid
来源：http://ay.muxihuayi.cn

Ruby: SecureRandom.uuid
来源：http://ka.muxihuayi.cn

C#:   Guid.NewGuid().ToString()
来源：http://gy.huanxung.cn

[P02] MD5 / SHA256 摘要
来源：http://jb.jctech888.com.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://sb.nszjky.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://yl.huixiangedu.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ol.muxihuayi.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://oj.jianghongdianzi.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://xq.asd995.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://oq.newstarts.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://lj.yuexingan06.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://tg.huixinmuqiang.cn

[P03] 生成短随机字符串
来源：http://pa.haigaiapp.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ee.521024.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://pl.9csxet.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://bq.lnxyls.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://qg.9csxet.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://tr.shxzukj.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://cq.muxihuayi.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://hq.nicolike.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ak.asd995.cn

[P04] 求长度
来源：http://kz.gzmigu.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://zc.lnxyls.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://zo.huixiangedu.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ij.asd995.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://nt.lnxyls.cn

Java: list.size();  map.size();  s.length()
来源：http://ku.9csxet.cn

Go:   len(arr);  len(m)
来源：http://bi.521024.cn

Ruby: x.length;  x.size
来源：http://hq.asd995.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://lv.szsharing.cn

[P05] 判断两个对象内容是否相等
来源：http://sb.asd995.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://iu.521024.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://il.huixinmuqiang.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://gk.lnxyls.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ug.nszjky.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ue.muxihuayi.cn

Go:   reflect.DeepEqual(a, b)
来源：http://yb.gzmigu.cn

Ruby: a == b
来源：http://js.shxzskj.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://vn.szxytkj.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://id.muxihuayi.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://yl.lnxyls.cn

PHP:  if (empty($x)) {}
来源：http://zr.panjiajie.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://yh.wgjwhj.cn

TS:   if (x == null) {}
来源：http://zv.shtwfgs.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://am.huixiangedu.cn

Go:   if x == nil {}
来源：http://wk.nicolike.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://pw.chemitech.net.cn

C#:   if (x is null) {}
来源：http://or.huixinmuqiang.cn

[P07] 防抖与节流
来源：http://ye.bjjhwx.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://cj.colortex.cn

PHP:  // 手写时间戳比较
来源：http://nr.colortex.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://oj.szxytkj.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ma.bookmarksfly.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wh.bjjhwx.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://lc.lnxyls.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://mq.bookmarksfly.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wg.lnxyls.cn

[P08] 处理浮点精度问题
来源：http://ug.chemitech.net.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://rd.hnjuh.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://se.nicolike.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://qz.shxzukj.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://yt.chemitech.net.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://zn.nszjky.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://js.huanxung.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://yh.nszjky.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ai.521024.cn

================================================================================
来源：http://wn.newstarts.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://my.huixinmuqiang.cn

================================================================================
来源：http://id.huanxung.cn

[Q01] 创建表
来源：http://ns.chemitech.net.cn

CREATE TABLE users (
来源：http://pd.hahajie.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ol.wgjwhj.cn

name VARCHAR(50) NOT NULL,
来源：http://rq.szxytkj.cn

email VARCHAR(100) UNIQUE,
来源：http://pr.asd995.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://sz.yuntaijiaju.cn

);
来源：http://fq.yuntaijiaju.cn

[Q02] 创建带外键的表
来源：http://ex.bookmarksfly.cn

CREATE TABLE orders (
来源：http://ur.wgjwhj.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://xm.bjjhwx.cn

user_id INT NOT NULL,
来源：http://sx.haigaiapp.cn

amount DECIMAL(10, 2),
来源：http://io.szxytkj.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://lv.yuexingan06.cn

);
来源：http://mv.shxzskj.cn

[Q03] 增加列
来源：http://eg.hahajie.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://xr.shtwfgs.cn

[Q04] 修改列类型
来源：http://pn.nszjky.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://cf.hahajie.cn

[Q05] 重命名列
来源：http://zh.9csxet.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://um.colortex.cn

[Q06] 删除列
来源：http://fg.hnjuh.cn

ALTER TABLE users DROP COLUMN age;
来源：http://er.newstarts.cn

[Q07] 删除表
来源：http://sg.colortex.cn

DROP TABLE IF EXISTS orders;
来源：http://jb.bjjhwx.cn

[Q08] 创建普通索引
来源：http://qq.panjiajie.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://xr.jianghongdianzi.cn

[Q09] 创建唯一索引
来源：http://vz.jianghongdianzi.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://vz.szsharing.cn

[Q10] 插入单行
来源：http://nn.shxzskj.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://bt.huixiangedu.cn

[Q11] 一次插入多行
来源：http://bt.shxzskj.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://qy.huixiangedu.cn

[Q12] 插入后取自增 ID
来源：http://en.jctech888.com.cn

INSERT INTO users (name) VALUES ('C');
来源：http://mz.huanxung.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://zz.shxzskj.cn

[Q13] 忽略重复插入
来源：http://uf.haigaiapp.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://fv.asd995.cn

[Q14] 存在则更新（upsert）
来源：http://sr.chemitech.net.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://te.colortex.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://pd.haigaiapp.cn

[Q15] 查询全部
来源：http://lm.shxzukj.cn

SELECT * FROM users;
来源：http://jy.521024.cn

[Q16] 查询指定列
来源：http://mx.gzmigu.cn

SELECT id, name FROM users;
来源：http://gf.hnjuh.cn

[Q17] 条件查询
来源：http://rh.huixiangedu.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ts.shxzskj.cn

[Q18] 模糊匹配
来源：http://wn.colortex.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://po.wgjwhj.cn

[Q19] 范围查询
来源：http://ew.hnjuh.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://cs.9csxet.cn

[Q20] IN 列表
来源：http://kd.shxzukj.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://uq.lnxyls.cn

[Q21] 空值判断
来源：http://by.newstarts.cn


<!-- 参考信息 -->