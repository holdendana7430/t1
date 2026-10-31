代发 wailian999

[N01] 二分查找（有序数组）
来源：http://ja.nszjky.cn

Py:   bisect.bisect_left(arr, x)
来源：http://kv.shxzskj.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://qu.wgjwhj.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://nf.panjiajie.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ny.shxzskj.cn

Java: Arrays.binarySearch(arr, x)
来源：http://dg.newstarts.cn

Go:   sort.SearchInts(arr, x)
来源：http://sf.shtwfgs.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://it.haigaiapp.cn

C#:   Array.BinarySearch(arr, x)
来源：http://uz.hnjuh.cn

[N02] 排序（工程实践用内置实现）
来源：http://ur.colortex.cn

Py:   sorted(arr);  arr.sort()
来源：http://ww.huixinmuqiang.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://my.521024.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://hg.asd995.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://ov.nicolike.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://cx.huixinmuqiang.cn

Go:   slices.Sort(arr)
来源：http://dq.jctech888.com.cn

Ruby: arr.sort
来源：http://pk.asd995.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://oz.yuexingan06.cn

[N03] 快速排序（分治示例）
来源：http://ti.haigaiapp.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://xy.szsharing.cn

PHP:  // 递归实现，或用 usort
来源：http://re.gzmigu.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://gm.shtwfgs.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://jf.jianghongdianzi.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://th.muxihuayi.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://km.asd995.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://jy.szsharing.cn

C#:   // 手写递归，或 Array.Sort
来源：http://ph.huixiangedu.cn

[N04] 斐波那契数列
来源：http://mc.shtwfgs.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://dx.shxzukj.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://fd.huanxung.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://vq.gzmigu.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://pg.lnxyls.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.hahajie.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://lp.nicolike.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://su.szsharing.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://yw.521024.cn

[N05] 最大公约数
来源：http://nm.newstarts.cn

Py:   math.gcd(a, b)
来源：http://bc.9csxet.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ap.shxzukj.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://gt.9csxet.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://cd.colortex.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ao.bookmarksfly.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.huixinmuqiang.cn

Ruby: a.gcd(b)
来源：http://hq.lnxyls.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://yb.bookmarksfly.cn

[N06] 判断回文字符串
来源：http://fg.szsharing.cn

Py:   s == s[::-1]
来源：http://qb.nicolike.cn

PHP:  $s === strrev($s);
来源：http://ht.521024.cn

JS:   s === [...s].reverse().join("")
来源：http://fx.bookmarksfly.cn

TS:   s === [...s].reverse().join("")
来源：http://qw.gzmigu.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://pu.521024.cn

Go:   // 双指针从两端比较
来源：http://oi.muxihuayi.cn

Ruby: s == s.reverse
来源：http://kl.szxytkj.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://hp.szxytkj.cn

[N07] 两数之和（返回下标）
来源：http://rl.newstarts.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://tr.szxytkj.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://dg.haigaiapp.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://zh.nicolike.cn

TS:   // 手写 Map<string, number>
来源：http://kz.huixinmuqiang.cn

Java: // 手写 HashMap
来源：http://jy.nszjky.cn

Go:   // 手写 map[int]int
来源：http://yk.colortex.cn

Ruby: // 手写 Hash
来源：http://ug.jianghongdianzi.cn

C#:   // 手写 Dictionary<int, int>
来源：http://bx.shxzukj.cn

[N08] 生成全排列
来源：http://wz.gzmigu.cn

Py:   itertools.permutations(arr)
来源：http://cr.jctech888.com.cn

PHP:  // 手写递归交换
来源：http://od.szsharing.cn

JS:   // 手写回溯递归
来源：http://kc.haigaiapp.cn

TS:   // 手写回溯递归
来源：http://oq.yuntaijiaju.cn

Java: // 手写回溯递归
来源：http://em.bjjhwx.cn

Go:   // 手写回溯递归
来源：http://ie.huixinmuqiang.cn

Ruby: arr.permutation.to_a
来源：http://sr.lnxyls.cn

C#:   // 手写回溯递归
来源：http://fj.nicolike.cn

[N09] 栈与队列
来源：http://rn.nicolike.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://sg.asd995.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://bf.jctech888.com.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://tg.asd995.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ab.szsharing.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://pp.szxytkj.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ci.nicolike.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://co.bookmarksfly.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://dk.huanxung.cn

[N10] 链表节点定义
来源：http://ys.muxihuayi.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ky.jianghongdianzi.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://ku.jianghongdianzi.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://vl.nszjky.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ii.muxihuayi.cn

Java: class Node { int v; Node next; }
来源：http://ji.lnxyls.cn

Go:   type Node struct { V int; Next *Node }
来源：http://rn.huanxung.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://fe.muxihuayi.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://wq.chemitech.net.cn

[N11] 二叉树中序遍历
来源：http://ac.newstarts.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://fh.shtwfgs.cn

PHP:  // 手写递归函数
来源：http://yy.nicolike.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ra.colortex.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mj.hnjuh.cn

Java: // 手写递归
来源：http://ye.bjjhwx.cn

Go:   // 手写递归
来源：http://af.huanxung.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://et.huanxung.cn

C#:   // 手写递归
来源：http://ia.szxytkj.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://zn.yuntaijiaju.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hu.shtwfgs.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://rp.gzmigu.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ml.huixinmuqiang.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://qd.yuntaijiaju.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://jx.nicolike.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://rl.asd995.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://zi.huixiangedu.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ey.huixinmuqiang.cn

================================================================================
来源：http://fe.muxihuayi.cn

O. 并发与异步
来源：http://sf.shxzskj.cn

================================================================================
来源：http://st.bjjhwx.cn

[O01] 启动一个线程
来源：http://kt.521024.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://jq.nszjky.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://if.haigaiapp.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ag.lnxyls.cn

TS:   // 同 JS
来源：http://qn.nszjky.cn

Java: new Thread(() -> f()).start()
来源：http://ev.jianghongdianzi.cn

Go:   go f()
来源：http://kv.panjiajie.cn

Ruby: Thread.new { f }
来源：http://kv.colortex.cn

C#:   Task.Run(() => F());
来源：http://dh.yuntaijiaju.cn

[O02] 使用线程池
来源：http://zp.yuntaijiaju.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://cd.yuexingan06.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://np.muxihuayi.cn

JS:   // worker_threads 线程池
来源：http://eh.yuexingan06.cn

TS:   // worker_threads 线程池
来源：http://ca.haigaiapp.cn

Java: Executors.newFixedThreadPool(4)
来源：http://hd.521024.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://au.shtwfgs.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://rj.haigaiapp.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ze.szxytkj.cn

[O03] 加锁保护共享数据
来源：http://gj.bookmarksfly.cn

Py:   with lock: shared += 1
来源：http://ej.shxzukj.cn

PHP:  // 用 flock() 做文件锁
来源：http://hr.yuexingan06.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://pd.lnxyls.cn

TS:   // 同 JS
来源：http://rx.haigaiapp.cn

Java: synchronized (this) { shared++; }
来源：http://dg.yuntaijiaju.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://sj.asd995.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://sf.huanxung.cn

C#:   lock (gate) { shared++; }
来源：http://jt.huixinmuqiang.cn

[O04] 定义异步函数并等待
来源：http://pn.bookmarksfly.cn

Py:   async def f():⏎    await g()
来源：http://em.hahajie.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://bj.colortex.cn

JS:   async function f() { await g(); }
来源：http://pp.muxihuayi.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://py.hahajie.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://uv.newstarts.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ok.yuntaijiaju.cn

Ruby: # 用 Fiber 或 async gem
来源：http://sw.haigaiapp.cn

C#:   async Task F() { await G(); }
来源：http://sh.521024.cn

[O05] 并发执行并等待全部完成
来源：http://qt.9csxet.cn

Py:   asyncio.gather(*tasks)
来源：http://sf.wgjwhj.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://qe.jctech888.com.cn

JS:   await Promise.all(tasks)
来源：http://la.asd995.cn

TS:   await Promise.all(tasks)
来源：http://im.wgjwhj.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://dw.jianghongdianzi.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://rb.szxytkj.cn

Ruby: threads.map(&:join)
来源：http://dy.nicolike.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://ns.lnxyls.cn

[O06] 使用进程池
来源：http://li.hnjuh.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://pc.yuexingan06.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://py.hahajie.cn

JS:   // child_process / cluster 模块
来源：http://kx.nszjky.cn

TS:   // child_process / cluster 模块
来源：http://hc.nszjky.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://zq.nszjky.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://jv.shtwfgs.cn

Ruby: // fork 块
来源：http://pe.yuexingan06.cn

C#:   Parallel.For
来源：http://de.szxytkj.cn

================================================================================
来源：http://yb.lnxyls.cn

P. 常用工具函数
来源：http://ku.jianghongdianzi.cn

================================================================================
来源：http://nl.shxzukj.cn

[P01] 生成 UUID
来源：http://ok.huixinmuqiang.cn

Py:   str(uuid.uuid4())
来源：http://nx.521024.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://vv.9csxet.cn

JS:   crypto.randomUUID()
来源：http://tv.9csxet.cn

TS:   crypto.randomUUID()
来源：http://md.nicolike.cn

Java: UUID.randomUUID().toString()
来源：http://uw.jctech888.com.cn

Go:   // 用 github.com/google/uuid
来源：http://nt.huixinmuqiang.cn

Ruby: SecureRandom.uuid
来源：http://hk.shxzukj.cn

C#:   Guid.NewGuid().ToString()
来源：http://jy.shtwfgs.cn

[P02] MD5 / SHA256 摘要
来源：http://os.yuexingan06.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mf.haigaiapp.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://fp.bjjhwx.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ks.newstarts.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mt.chemitech.net.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://fv.lnxyls.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://jq.huixiangedu.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ck.bjjhwx.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://lk.nszjky.cn

[P03] 生成短随机字符串
来源：http://ru.nszjky.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://is.jianghongdianzi.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://lx.haigaiapp.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://eh.muxihuayi.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://pk.haigaiapp.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://qe.haigaiapp.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://if.colortex.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://ko.szxytkj.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://gc.bookmarksfly.cn

[P04] 求长度
来源：http://kc.9csxet.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://re.huanxung.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://np.yuexingan06.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ft.shtwfgs.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://lx.huixiangedu.cn

Java: list.size();  map.size();  s.length()
来源：http://fg.bjjhwx.cn

Go:   len(arr);  len(m)
来源：http://zd.jctech888.com.cn

Ruby: x.length;  x.size
来源：http://ab.colortex.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://ba.bookmarksfly.cn

[P05] 判断两个对象内容是否相等
来源：http://qx.muxihuayi.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://bl.jctech888.com.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://yh.shxzskj.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://sr.newstarts.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ku.muxihuayi.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://es.huixinmuqiang.cn

Go:   reflect.DeepEqual(a, b)
来源：http://pw.szxytkj.cn

Ruby: a == b
来源：http://gp.shxzukj.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ho.yuntaijiaju.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://co.shxzskj.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://jt.lnxyls.cn

PHP:  if (empty($x)) {}
来源：http://ar.jianghongdianzi.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://di.shxzskj.cn

TS:   if (x == null) {}
来源：http://eb.yuexingan06.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://ya.jianghongdianzi.cn

Go:   if x == nil {}
来源：http://vu.muxihuayi.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://lb.colortex.cn

C#:   if (x is null) {}
来源：http://ab.huanxung.cn

[P07] 防抖与节流
来源：http://mf.huanxung.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://gr.wgjwhj.cn

PHP:  // 手写时间戳比较
来源：http://fc.newstarts.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://go.huixinmuqiang.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://jf.nicolike.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://to.panjiajie.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://lg.shtwfgs.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://ik.nszjky.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ac.yuntaijiaju.cn

[P08] 处理浮点精度问题
来源：http://ao.asd995.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://br.szxytkj.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://qc.haigaiapp.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://pt.shtwfgs.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://iu.shxzukj.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://di.huanxung.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hy.gzmigu.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://tf.muxihuayi.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://nr.lnxyls.cn

================================================================================
来源：http://zp.nszjky.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://so.9csxet.cn

================================================================================
来源：http://ct.newstarts.cn

[Q01] 创建表
来源：http://zn.chemitech.net.cn

CREATE TABLE users (
来源：http://nh.gzmigu.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wu.yuexingan06.cn

name VARCHAR(50) NOT NULL,
来源：http://eh.shxzukj.cn

email VARCHAR(100) UNIQUE,
来源：http://hj.yuexingan06.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://fk.huanxung.cn

);
来源：http://qz.nicolike.cn

[Q02] 创建带外键的表
来源：http://ht.wgjwhj.cn

CREATE TABLE orders (
来源：http://fz.muxihuayi.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wm.9csxet.cn

user_id INT NOT NULL,
来源：http://bo.panjiajie.cn

amount DECIMAL(10, 2),
来源：http://mb.lnxyls.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://lf.newstarts.cn

);
来源：http://mc.szsharing.cn

[Q03] 增加列
来源：http://oi.szsharing.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://dc.panjiajie.cn

[Q04] 修改列类型
来源：http://hy.haigaiapp.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://na.jianghongdianzi.cn

[Q05] 重命名列
来源：http://mg.colortex.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://aa.shxzskj.cn

[Q06] 删除列
来源：http://nn.yuexingan06.cn

ALTER TABLE users DROP COLUMN age;
来源：http://zd.shxzukj.cn

[Q07] 删除表
来源：http://zz.huixinmuqiang.cn

DROP TABLE IF EXISTS orders;
来源：http://sa.haigaiapp.cn

[Q08] 创建普通索引
来源：http://kl.yuexingan06.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://lz.gzmigu.cn

[Q09] 创建唯一索引
来源：http://pa.shxzukj.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://xs.yuntaijiaju.cn

[Q10] 插入单行
来源：http://ze.wgjwhj.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://sm.yuntaijiaju.cn

[Q11] 一次插入多行
来源：http://rb.yuntaijiaju.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://yz.huixinmuqiang.cn

[Q12] 插入后取自增 ID
来源：http://jl.nszjky.cn

INSERT INTO users (name) VALUES ('C');
来源：http://ru.jctech888.com.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://pj.chemitech.net.cn

[Q13] 忽略重复插入
来源：http://hl.huixiangedu.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://fc.hnjuh.cn

[Q14] 存在则更新（upsert）
来源：http://dm.521024.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://zj.newstarts.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://nb.jctech888.com.cn

[Q15] 查询全部
来源：http://ym.bookmarksfly.cn

SELECT * FROM users;
来源：http://kt.yuntaijiaju.cn

[Q16] 查询指定列
来源：http://cu.huixiangedu.cn

SELECT id, name FROM users;
来源：http://rn.bookmarksfly.cn

[Q17] 条件查询
来源：http://gp.haigaiapp.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://kj.jctech888.com.cn

[Q18] 模糊匹配
来源：http://mb.colortex.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ei.colortex.cn

[Q19] 范围查询
来源：http://ex.bjjhwx.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mj.lnxyls.cn

[Q20] IN 列表
来源：http://nc.huanxung.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://qz.shxzskj.cn

[Q21] 空值判断
来源：http://cs.huixinmuqiang.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://zd.wgjwhj.cn

[Q22] 排序
来源：http://qc.newstarts.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ka.shxzskj.cn

[Q23] 分页
来源：http://hp.haigaiapp.cn


<!-- 参考信息 -->