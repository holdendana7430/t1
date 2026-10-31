代发 wailian999

C#:   Environment.OSVersion;  Environment.Version
来源：http://ih.hahajie.cn

================================================================================
来源：http://wd.nicolike.cn

N. 数据结构与算法
来源：http://su.szxytkj.cn

================================================================================
来源：http://hu.newstarts.cn

[N01] 二分查找（有序数组）
来源：http://yg.shxzukj.cn

Py:   bisect.bisect_left(arr, x)
来源：http://vk.lnxyls.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://rq.bjjhwx.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://nq.bookmarksfly.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ht.yuexingan06.cn

Java: Arrays.binarySearch(arr, x)
来源：http://op.szxytkj.cn

Go:   sort.SearchInts(arr, x)
来源：http://zw.colortex.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://za.bjjhwx.cn

C#:   Array.BinarySearch(arr, x)
来源：http://qy.huanxung.cn

[N02] 排序（工程实践用内置实现）
来源：http://fx.hnjuh.cn

Py:   sorted(arr);  arr.sort()
来源：http://fs.panjiajie.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://qk.huixiangedu.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://dr.shtwfgs.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://fx.jctech888.com.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://lj.haigaiapp.cn

Go:   slices.Sort(arr)
来源：http://cu.9csxet.cn

Ruby: arr.sort
来源：http://ro.lnxyls.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://kg.jctech888.com.cn

[N03] 快速排序（分治示例）
来源：http://ri.gzmigu.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://lx.9csxet.cn

PHP:  // 递归实现，或用 usort
来源：http://we.szsharing.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://go.9csxet.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://jp.yuntaijiaju.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://bm.yuexingan06.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://sh.bjjhwx.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://vr.jianghongdianzi.cn

C#:   // 手写递归，或 Array.Sort
来源：http://wp.lnxyls.cn

[N04] 斐波那契数列
来源：http://mp.chemitech.net.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://au.521024.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://my.shxzukj.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://oi.shxzskj.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ez.shxzukj.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://sk.wgjwhj.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://tm.bookmarksfly.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wn.huixiangedu.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://az.jctech888.com.cn

[N05] 最大公约数
来源：http://gt.hahajie.cn

Py:   math.gcd(a, b)
来源：http://wq.muxihuayi.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://pv.yuexingan06.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://sy.shtwfgs.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ph.bjjhwx.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://lz.huixinmuqiang.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://qo.yuntaijiaju.cn

Ruby: a.gcd(b)
来源：http://xa.bjjhwx.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://jm.hahajie.cn

[N06] 判断回文字符串
来源：http://bk.nicolike.cn

Py:   s == s[::-1]
来源：http://rq.bookmarksfly.cn

PHP:  $s === strrev($s);
来源：http://hm.szxytkj.cn

JS:   s === [...s].reverse().join("")
来源：http://li.gzmigu.cn

TS:   s === [...s].reverse().join("")
来源：http://jt.newstarts.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://nv.521024.cn

Go:   // 双指针从两端比较
来源：http://gz.newstarts.cn

Ruby: s == s.reverse
来源：http://rh.chemitech.net.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://vw.muxihuayi.cn

[N07] 两数之和（返回下标）
来源：http://pa.muxihuayi.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ev.panjiajie.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://lx.9csxet.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://ww.huanxung.cn

TS:   // 手写 Map<string, number>
来源：http://jz.huixiangedu.cn

Java: // 手写 HashMap
来源：http://pc.shxzukj.cn

Go:   // 手写 map[int]int
来源：http://xn.nicolike.cn

Ruby: // 手写 Hash
来源：http://yr.asd995.cn

C#:   // 手写 Dictionary<int, int>
来源：http://xd.hnjuh.cn

[N08] 生成全排列
来源：http://fa.shxzskj.cn

Py:   itertools.permutations(arr)
来源：http://qd.shxzukj.cn

PHP:  // 手写递归交换
来源：http://jp.jianghongdianzi.cn

JS:   // 手写回溯递归
来源：http://ug.shxzskj.cn

TS:   // 手写回溯递归
来源：http://ya.521024.cn

Java: // 手写回溯递归
来源：http://yh.huixinmuqiang.cn

Go:   // 手写回溯递归
来源：http://ik.shtwfgs.cn

Ruby: arr.permutation.to_a
来源：http://km.9csxet.cn

C#:   // 手写回溯递归
来源：http://tu.nicolike.cn

[N09] 栈与队列
来源：http://rj.colortex.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://uu.521024.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://zg.521024.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://gd.szxytkj.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://qz.huixinmuqiang.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ok.shxzskj.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://un.nicolike.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://lc.gzmigu.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://xy.hnjuh.cn

[N10] 链表节点定义
来源：http://yf.huixiangedu.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://tg.gzmigu.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://re.shxzukj.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://fm.haigaiapp.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://uw.huixiangedu.cn

Java: class Node { int v; Node next; }
来源：http://gg.gzmigu.cn

Go:   type Node struct { V int; Next *Node }
来源：http://ve.nszjky.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://mu.huixiangedu.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://dh.huixiangedu.cn

[N11] 二叉树中序遍历
来源：http://la.szsharing.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://fo.hnjuh.cn

PHP:  // 手写递归函数
来源：http://zt.nszjky.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ax.shxzskj.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://bx.bjjhwx.cn

Java: // 手写递归
来源：http://lk.jctech888.com.cn

Go:   // 手写递归
来源：http://ai.gzmigu.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://za.shxzskj.cn

C#:   // 手写递归
来源：http://uj.gzmigu.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://oj.colortex.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://cx.colortex.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://xe.yuexingan06.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://tq.colortex.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://bm.lnxyls.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ka.hahajie.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://xw.chemitech.net.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://yn.szxytkj.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://kc.chemitech.net.cn

================================================================================
来源：http://nv.jctech888.com.cn

O. 并发与异步
来源：http://jg.chemitech.net.cn

================================================================================
来源：http://ap.szsharing.cn

[O01] 启动一个线程
来源：http://cj.newstarts.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://qw.shtwfgs.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://fr.huanxung.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://qs.haigaiapp.cn

TS:   // 同 JS
来源：http://nc.bookmarksfly.cn

Java: new Thread(() -> f()).start()
来源：http://dh.muxihuayi.cn

Go:   go f()
来源：http://rs.asd995.cn

Ruby: Thread.new { f }
来源：http://mq.szsharing.cn

C#:   Task.Run(() => F());
来源：http://uc.hnjuh.cn

[O02] 使用线程池
来源：http://en.shtwfgs.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://uk.newstarts.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://eo.nszjky.cn

JS:   // worker_threads 线程池
来源：http://sc.nszjky.cn

TS:   // worker_threads 线程池
来源：http://iv.wgjwhj.cn

Java: Executors.newFixedThreadPool(4)
来源：http://dj.yuntaijiaju.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://cb.nicolike.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://me.nicolike.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://un.nszjky.cn

[O03] 加锁保护共享数据
来源：http://gq.huanxung.cn

Py:   with lock: shared += 1
来源：http://yp.jianghongdianzi.cn

PHP:  // 用 flock() 做文件锁
来源：http://rj.hnjuh.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ej.yuntaijiaju.cn

TS:   // 同 JS
来源：http://fs.panjiajie.cn

Java: synchronized (this) { shared++; }
来源：http://rx.shxzskj.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://rg.chemitech.net.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://bi.wgjwhj.cn

C#:   lock (gate) { shared++; }
来源：http://rx.hnjuh.cn

[O04] 定义异步函数并等待
来源：http://ar.shxzskj.cn

Py:   async def f():⏎    await g()
来源：http://na.haigaiapp.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://rw.lnxyls.cn

JS:   async function f() { await g(); }
来源：http://wh.jianghongdianzi.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://ab.gzmigu.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://qw.yuexingan06.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://cg.hnjuh.cn

Ruby: # 用 Fiber 或 async gem
来源：http://lj.colortex.cn

C#:   async Task F() { await G(); }
来源：http://in.shxzukj.cn

[O05] 并发执行并等待全部完成
来源：http://ep.jctech888.com.cn

Py:   asyncio.gather(*tasks)
来源：http://gj.colortex.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://yz.colortex.cn

JS:   await Promise.all(tasks)
来源：http://ii.huixiangedu.cn

TS:   await Promise.all(tasks)
来源：http://az.colortex.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://kk.nicolike.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://aq.9csxet.cn

Ruby: threads.map(&:join)
来源：http://vi.hahajie.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://yb.bookmarksfly.cn

[O06] 使用进程池
来源：http://qd.wgjwhj.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ge.hnjuh.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://xg.huixinmuqiang.cn

JS:   // child_process / cluster 模块
来源：http://eb.yuntaijiaju.cn

TS:   // child_process / cluster 模块
来源：http://xg.gzmigu.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://tj.9csxet.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ha.yuntaijiaju.cn

Ruby: // fork 块
来源：http://fv.gzmigu.cn

C#:   Parallel.For
来源：http://bj.hnjuh.cn

================================================================================
来源：http://rs.szxytkj.cn

P. 常用工具函数
来源：http://ln.huixiangedu.cn

================================================================================
来源：http://se.huixinmuqiang.cn

[P01] 生成 UUID
来源：http://db.chemitech.net.cn

Py:   str(uuid.uuid4())
来源：http://kt.hahajie.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://jk.yuntaijiaju.cn

JS:   crypto.randomUUID()
来源：http://gu.shxzukj.cn

TS:   crypto.randomUUID()
来源：http://si.shtwfgs.cn

Java: UUID.randomUUID().toString()
来源：http://gi.huanxung.cn

Go:   // 用 github.com/google/uuid
来源：http://ki.bookmarksfly.cn

Ruby: SecureRandom.uuid
来源：http://kr.colortex.cn

C#:   Guid.NewGuid().ToString()
来源：http://xc.jianghongdianzi.cn

[P02] MD5 / SHA256 摘要
来源：http://uk.gzmigu.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ir.nszjky.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://te.gzmigu.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://sw.panjiajie.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://qm.bookmarksfly.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://co.hahajie.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ix.huixiangedu.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ae.shtwfgs.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://gd.jctech888.com.cn

[P03] 生成短随机字符串
来源：http://nn.newstarts.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mk.shxzskj.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://uv.huixiangedu.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://zq.jctech888.com.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://lx.521024.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://xz.bjjhwx.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://nc.chemitech.net.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://sp.yuntaijiaju.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ru.nszjky.cn

[P04] 求长度
来源：http://nh.asd995.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://gh.521024.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://uq.nicolike.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ed.yuntaijiaju.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://rz.hnjuh.cn

Java: list.size();  map.size();  s.length()
来源：http://ti.chemitech.net.cn

Go:   len(arr);  len(m)
来源：http://ak.nicolike.cn

Ruby: x.length;  x.size
来源：http://jm.hahajie.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://qy.shtwfgs.cn

[P05] 判断两个对象内容是否相等
来源：http://ww.wgjwhj.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://rv.huixinmuqiang.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://zr.521024.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://xz.bjjhwx.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://qb.colortex.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://or.lnxyls.cn

Go:   reflect.DeepEqual(a, b)
来源：http://yw.huanxung.cn

Ruby: a == b
来源：http://jk.hnjuh.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://bw.haigaiapp.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://nu.jctech888.com.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://nj.shxzskj.cn

PHP:  if (empty($x)) {}
来源：http://wf.asd995.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://uk.hnjuh.cn

TS:   if (x == null) {}
来源：http://qv.huanxung.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://md.yuntaijiaju.cn

Go:   if x == nil {}
来源：http://jk.lnxyls.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://tc.shxzskj.cn

C#:   if (x is null) {}
来源：http://ra.jctech888.com.cn

[P07] 防抖与节流
来源：http://ad.shxzukj.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://kl.wgjwhj.cn

PHP:  // 手写时间戳比较
来源：http://tx.nszjky.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://yf.gzmigu.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://rd.chemitech.net.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hl.yuexingan06.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://on.yuexingan06.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://xy.colortex.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://rb.gzmigu.cn

[P08] 处理浮点精度问题
来源：http://ho.lnxyls.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://jw.asd995.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://tu.szxytkj.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://tp.szxytkj.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://qu.nicolike.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://in.shxzskj.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hd.panjiajie.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://lq.jctech888.com.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://te.szxytkj.cn

================================================================================
来源：http://ro.521024.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ju.asd995.cn

================================================================================
来源：http://ve.jianghongdianzi.cn

[Q01] 创建表
来源：http://ou.szxytkj.cn

CREATE TABLE users (
来源：http://im.huanxung.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://qr.jianghongdianzi.cn

name VARCHAR(50) NOT NULL,
来源：http://iw.huixinmuqiang.cn

email VARCHAR(100) UNIQUE,
来源：http://wp.huixiangedu.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://uq.yuntaijiaju.cn

);
来源：http://wz.huanxung.cn

[Q02] 创建带外键的表
来源：http://na.yuntaijiaju.cn

CREATE TABLE orders (
来源：http://kn.haigaiapp.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mn.521024.cn

user_id INT NOT NULL,
来源：http://yi.colortex.cn

amount DECIMAL(10, 2),
来源：http://xu.nszjky.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://gn.9csxet.cn

);
来源：http://iu.bjjhwx.cn

[Q03] 增加列
来源：http://no.yuntaijiaju.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hr.muxihuayi.cn

[Q04] 修改列类型
来源：http://vx.huixiangedu.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hq.9csxet.cn

[Q05] 重命名列
来源：http://zh.huanxung.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ax.hnjuh.cn

[Q06] 删除列
来源：http://aa.9csxet.cn

ALTER TABLE users DROP COLUMN age;
来源：http://fw.lnxyls.cn

[Q07] 删除表
来源：http://er.muxihuayi.cn

DROP TABLE IF EXISTS orders;
来源：http://ev.huixiangedu.cn

[Q08] 创建普通索引
来源：http://bv.shtwfgs.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://yl.huixiangedu.cn

[Q09] 创建唯一索引
来源：http://ud.bjjhwx.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://sx.hnjuh.cn

[Q10] 插入单行
来源：http://nl.asd995.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wa.asd995.cn

[Q11] 一次插入多行
来源：http://oi.nicolike.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://oa.bjjhwx.cn

[Q12] 插入后取自增 ID
来源：http://om.asd995.cn

INSERT INTO users (name) VALUES ('C');
来源：http://vk.colortex.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://vc.shxzskj.cn

[Q13] 忽略重复插入
来源：http://pg.nszjky.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://rj.521024.cn

[Q14] 存在则更新（upsert）
来源：http://dd.wgjwhj.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://vu.bookmarksfly.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://fb.haigaiapp.cn

[Q15] 查询全部
来源：http://jp.nszjky.cn

SELECT * FROM users;
来源：http://ou.muxihuayi.cn

[Q16] 查询指定列
来源：http://el.lnxyls.cn

SELECT id, name FROM users;
来源：http://jt.jianghongdianzi.cn

[Q17] 条件查询
来源：http://bt.haigaiapp.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hm.bookmarksfly.cn

[Q18] 模糊匹配
来源：http://is.shxzukj.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ke.wgjwhj.cn

[Q19] 范围查询
来源：http://ra.huixiangedu.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mr.lnxyls.cn

[Q20] IN 列表
来源：http://ho.asd995.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://at.hahajie.cn

[Q21] 空值判断
来源：http://ge.yuntaijiaju.cn


<!-- 参考信息 -->