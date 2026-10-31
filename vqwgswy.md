代发 wailian999

C#:   Environment.OSVersion;  Environment.Version
来源：http://mk.nicolike.cn

================================================================================
来源：http://qk.nicolike.cn

N. 数据结构与算法
来源：http://ch.szxytkj.cn

================================================================================
来源：http://lw.jctech888.com.cn

[N01] 二分查找（有序数组）
来源：http://sb.wgjwhj.cn

Py:   bisect.bisect_left(arr, x)
来源：http://ac.newstarts.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://uw.newstarts.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://xo.szsharing.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://eq.huixinmuqiang.cn

Java: Arrays.binarySearch(arr, x)
来源：http://ll.muxihuayi.cn

Go:   sort.SearchInts(arr, x)
来源：http://gg.huixiangedu.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://ip.jctech888.com.cn

C#:   Array.BinarySearch(arr, x)
来源：http://sl.bjjhwx.cn

[N02] 排序（工程实践用内置实现）
来源：http://sj.9csxet.cn

Py:   sorted(arr);  arr.sort()
来源：http://tt.hnjuh.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://pv.muxihuayi.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://ma.colortex.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://dj.szxytkj.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ro.huanxung.cn

Go:   slices.Sort(arr)
来源：http://xg.521024.cn

Ruby: arr.sort
来源：http://sg.colortex.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://ah.nszjky.cn

[N03] 快速排序（分治示例）
来源：http://ep.panjiajie.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ny.hnjuh.cn

PHP:  // 递归实现，或用 usort
来源：http://bl.szxytkj.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ij.521024.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://bi.newstarts.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://fl.chemitech.net.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://iw.muxihuayi.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://kw.521024.cn

C#:   // 手写递归，或 Array.Sort
来源：http://us.muxihuayi.cn

[N04] 斐波那契数列
来源：http://db.colortex.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://bx.9csxet.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://kr.newstarts.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hr.huixiangedu.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ak.asd995.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://px.jctech888.com.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://qf.szsharing.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://vq.9csxet.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://zr.huixinmuqiang.cn

[N05] 最大公约数
来源：http://hv.jianghongdianzi.cn

Py:   math.gcd(a, b)
来源：http://kv.yuexingan06.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://cm.9csxet.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://md.hahajie.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://jj.521024.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://yd.panjiajie.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://vw.jctech888.com.cn

Ruby: a.gcd(b)
来源：http://or.bookmarksfly.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ad.nszjky.cn

[N06] 判断回文字符串
来源：http://dw.hahajie.cn

Py:   s == s[::-1]
来源：http://ri.bjjhwx.cn

PHP:  $s === strrev($s);
来源：http://ab.yuntaijiaju.cn

JS:   s === [...s].reverse().join("")
来源：http://om.shtwfgs.cn

TS:   s === [...s].reverse().join("")
来源：http://kf.jctech888.com.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ub.yuntaijiaju.cn

Go:   // 双指针从两端比较
来源：http://wr.colortex.cn

Ruby: s == s.reverse
来源：http://pp.haigaiapp.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://eb.yuntaijiaju.cn

[N07] 两数之和（返回下标）
来源：http://ht.hnjuh.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://zz.521024.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ip.chemitech.net.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://gz.jianghongdianzi.cn

TS:   // 手写 Map<string, number>
来源：http://db.colortex.cn

Java: // 手写 HashMap
来源：http://bo.shxzskj.cn

Go:   // 手写 map[int]int
来源：http://qp.9csxet.cn

Ruby: // 手写 Hash
来源：http://qt.asd995.cn

C#:   // 手写 Dictionary<int, int>
来源：http://gl.nicolike.cn

[N08] 生成全排列
来源：http://eu.huixinmuqiang.cn

Py:   itertools.permutations(arr)
来源：http://eb.chemitech.net.cn

PHP:  // 手写递归交换
来源：http://tj.haigaiapp.cn

JS:   // 手写回溯递归
来源：http://xb.haigaiapp.cn

TS:   // 手写回溯递归
来源：http://kd.huixinmuqiang.cn

Java: // 手写回溯递归
来源：http://dk.hahajie.cn

Go:   // 手写回溯递归
来源：http://zz.hnjuh.cn

Ruby: arr.permutation.to_a
来源：http://jr.huixinmuqiang.cn

C#:   // 手写回溯递归
来源：http://bb.huixiangedu.cn

[N09] 栈与队列
来源：http://mh.muxihuayi.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://qa.yuntaijiaju.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://lr.shxzskj.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mm.bookmarksfly.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://cu.newstarts.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://qs.shxzskj.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://cu.yuexingan06.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://yy.asd995.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ef.huixiangedu.cn

[N10] 链表节点定义
来源：http://cb.9csxet.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://eq.szsharing.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://to.newstarts.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://uw.bookmarksfly.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://eh.bookmarksfly.cn

Java: class Node { int v; Node next; }
来源：http://xq.haigaiapp.cn

Go:   type Node struct { V int; Next *Node }
来源：http://ba.jianghongdianzi.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://af.yuntaijiaju.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://rj.lnxyls.cn

[N11] 二叉树中序遍历
来源：http://vw.jctech888.com.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hp.gzmigu.cn

PHP:  // 手写递归函数
来源：http://ew.hahajie.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://cr.shtwfgs.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hb.nicolike.cn

Java: // 手写递归
来源：http://ug.hahajie.cn

Go:   // 手写递归
来源：http://dl.jctech888.com.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://gg.521024.cn

C#:   // 手写递归
来源：http://xm.yuexingan06.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://fr.huixinmuqiang.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://pp.jctech888.com.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://or.gzmigu.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://bs.lnxyls.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mb.bookmarksfly.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://kc.shxzskj.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://pp.wgjwhj.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ae.shxzskj.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://si.bjjhwx.cn

================================================================================
来源：http://rc.bookmarksfly.cn

O. 并发与异步
来源：http://wo.colortex.cn

================================================================================
来源：http://fi.yuexingan06.cn

[O01] 启动一个线程
来源：http://dg.521024.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://oi.bjjhwx.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mq.newstarts.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://th.haigaiapp.cn

TS:   // 同 JS
来源：http://bv.haigaiapp.cn

Java: new Thread(() -> f()).start()
来源：http://mq.yuntaijiaju.cn

Go:   go f()
来源：http://rh.shtwfgs.cn

Ruby: Thread.new { f }
来源：http://yz.jianghongdianzi.cn

C#:   Task.Run(() => F());
来源：http://zg.muxihuayi.cn

[O02] 使用线程池
来源：http://vk.newstarts.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://qo.newstarts.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://kf.huixinmuqiang.cn

JS:   // worker_threads 线程池
来源：http://mx.colortex.cn

TS:   // worker_threads 线程池
来源：http://iu.bookmarksfly.cn

Java: Executors.newFixedThreadPool(4)
来源：http://od.shtwfgs.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://rg.nszjky.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://co.newstarts.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://uz.newstarts.cn

[O03] 加锁保护共享数据
来源：http://qu.shtwfgs.cn

Py:   with lock: shared += 1
来源：http://nm.shxzskj.cn

PHP:  // 用 flock() 做文件锁
来源：http://up.asd995.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ok.panjiajie.cn

TS:   // 同 JS
来源：http://wz.521024.cn

Java: synchronized (this) { shared++; }
来源：http://mp.gzmigu.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://jb.shtwfgs.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://lr.shxzskj.cn

C#:   lock (gate) { shared++; }
来源：http://hd.521024.cn

[O04] 定义异步函数并等待
来源：http://zu.huixinmuqiang.cn

Py:   async def f():⏎    await g()
来源：http://mt.shxzskj.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://lv.shtwfgs.cn

JS:   async function f() { await g(); }
来源：http://gj.huixinmuqiang.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://jy.nszjky.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ar.asd995.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://rg.shxzskj.cn

Ruby: # 用 Fiber 或 async gem
来源：http://yn.hnjuh.cn

C#:   async Task F() { await G(); }
来源：http://ea.nicolike.cn

[O05] 并发执行并等待全部完成
来源：http://ho.gzmigu.cn

Py:   asyncio.gather(*tasks)
来源：http://tz.panjiajie.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://an.shxzskj.cn

JS:   await Promise.all(tasks)
来源：http://dw.521024.cn

TS:   await Promise.all(tasks)
来源：http://xb.9csxet.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://cz.nszjky.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ka.shxzukj.cn

Ruby: threads.map(&:join)
来源：http://tz.yuexingan06.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://mc.asd995.cn

[O06] 使用进程池
来源：http://pg.szsharing.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ro.huixinmuqiang.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://hk.colortex.cn

JS:   // child_process / cluster 模块
来源：http://ap.yuexingan06.cn

TS:   // child_process / cluster 模块
来源：http://dn.huixinmuqiang.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://dv.gzmigu.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://iw.nicolike.cn

Ruby: // fork 块
来源：http://cr.yuexingan06.cn

C#:   Parallel.For
来源：http://aw.hahajie.cn

================================================================================
来源：http://jj.yuexingan06.cn

P. 常用工具函数
来源：http://lw.hnjuh.cn

================================================================================
来源：http://aa.521024.cn

[P01] 生成 UUID
来源：http://kj.chemitech.net.cn

Py:   str(uuid.uuid4())
来源：http://rw.asd995.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://gc.hahajie.cn

JS:   crypto.randomUUID()
来源：http://vt.szxytkj.cn

TS:   crypto.randomUUID()
来源：http://ii.chemitech.net.cn

Java: UUID.randomUUID().toString()
来源：http://os.wgjwhj.cn

Go:   // 用 github.com/google/uuid
来源：http://ym.huixinmuqiang.cn

Ruby: SecureRandom.uuid
来源：http://hb.bjjhwx.cn

C#:   Guid.NewGuid().ToString()
来源：http://tt.bookmarksfly.cn

[P02] MD5 / SHA256 摘要
来源：http://rl.lnxyls.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://vd.521024.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://qg.hahajie.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://kl.hnjuh.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://dv.panjiajie.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mf.panjiajie.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://bw.newstarts.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://sw.newstarts.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://lz.9csxet.cn

[P03] 生成短随机字符串
来源：http://io.szxytkj.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://gu.yuexingan06.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://aj.chemitech.net.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://bz.jianghongdianzi.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://sd.shtwfgs.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://yi.haigaiapp.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://on.szsharing.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://aw.shxzskj.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wr.shxzukj.cn

[P04] 求长度
来源：http://sn.jianghongdianzi.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://vy.yuntaijiaju.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://aw.yuexingan06.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://yw.bjjhwx.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://xs.hnjuh.cn

Java: list.size();  map.size();  s.length()
来源：http://gt.yuntaijiaju.cn

Go:   len(arr);  len(m)
来源：http://mg.szsharing.cn

Ruby: x.length;  x.size
来源：http://bx.huixinmuqiang.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://sj.newstarts.cn

[P05] 判断两个对象内容是否相等
来源：http://pr.lnxyls.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://gm.huixinmuqiang.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wh.haigaiapp.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://cc.szsharing.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://st.nicolike.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ll.asd995.cn

Go:   reflect.DeepEqual(a, b)
来源：http://kd.jctech888.com.cn

Ruby: a == b
来源：http://xo.yuntaijiaju.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://xd.9csxet.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://gw.shxzukj.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://yc.lnxyls.cn

PHP:  if (empty($x)) {}
来源：http://zd.gzmigu.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ci.lnxyls.cn

TS:   if (x == null) {}
来源：http://pa.szsharing.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://ln.nicolike.cn

Go:   if x == nil {}
来源：http://rl.haigaiapp.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://af.asd995.cn

C#:   if (x is null) {}
来源：http://wr.521024.cn

[P07] 防抖与节流
来源：http://di.nszjky.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wb.hnjuh.cn

PHP:  // 手写时间戳比较
来源：http://ak.bjjhwx.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://rb.hahajie.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://te.huanxung.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://tt.huixinmuqiang.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://sf.shtwfgs.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://ta.lnxyls.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://jo.shxzskj.cn

[P08] 处理浮点精度问题
来源：http://zi.shxzskj.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://uw.muxihuayi.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://er.szxytkj.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://be.muxihuayi.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://eb.bookmarksfly.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://cb.bookmarksfly.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://tk.bookmarksfly.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hn.hahajie.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://sn.chemitech.net.cn

================================================================================
来源：http://pi.lnxyls.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://gs.nicolike.cn

================================================================================
来源：http://dm.hahajie.cn

[Q01] 创建表
来源：http://cd.lnxyls.cn

CREATE TABLE users (
来源：http://qs.shxzukj.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://jw.bjjhwx.cn

name VARCHAR(50) NOT NULL,
来源：http://iz.bjjhwx.cn

email VARCHAR(100) UNIQUE,
来源：http://ke.jianghongdianzi.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://pt.shxzskj.cn

);
来源：http://ly.asd995.cn

[Q02] 创建带外键的表
来源：http://mc.521024.cn

CREATE TABLE orders (
来源：http://dt.shxzskj.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://rc.hahajie.cn

user_id INT NOT NULL,
来源：http://yp.nicolike.cn

amount DECIMAL(10, 2),
来源：http://gi.9csxet.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://qm.huixiangedu.cn

);
来源：http://fr.yuexingan06.cn

[Q03] 增加列
来源：http://tv.szxytkj.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://pz.shxzskj.cn

[Q04] 修改列类型
来源：http://dd.nicolike.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://yx.szxytkj.cn

[Q05] 重命名列
来源：http://bz.huixinmuqiang.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://sk.9csxet.cn

[Q06] 删除列
来源：http://iq.asd995.cn

ALTER TABLE users DROP COLUMN age;
来源：http://za.asd995.cn

[Q07] 删除表
来源：http://yo.nicolike.cn

DROP TABLE IF EXISTS orders;
来源：http://jx.nszjky.cn

[Q08] 创建普通索引
来源：http://tv.bjjhwx.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://sf.jianghongdianzi.cn

[Q09] 创建唯一索引
来源：http://xi.hahajie.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://zi.huanxung.cn

[Q10] 插入单行
来源：http://yf.shtwfgs.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://at.9csxet.cn

[Q11] 一次插入多行
来源：http://qm.jianghongdianzi.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hw.panjiajie.cn

[Q12] 插入后取自增 ID
来源：http://ns.szsharing.cn

INSERT INTO users (name) VALUES ('C');
来源：http://tk.bookmarksfly.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://tz.hnjuh.cn

[Q13] 忽略重复插入
来源：http://md.bookmarksfly.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://es.nszjky.cn

[Q14] 存在则更新（upsert）
来源：http://bu.nicolike.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://dp.chemitech.net.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://fk.jctech888.com.cn

[Q15] 查询全部
来源：http://lp.yuntaijiaju.cn

SELECT * FROM users;
来源：http://jl.panjiajie.cn

[Q16] 查询指定列
来源：http://vk.asd995.cn

SELECT id, name FROM users;
来源：http://ew.huanxung.cn

[Q17] 条件查询
来源：http://hy.shxzukj.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ok.hahajie.cn

[Q18] 模糊匹配
来源：http://ks.hahajie.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://il.521024.cn

[Q19] 范围查询
来源：http://nd.szsharing.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ql.asd995.cn

[Q20] IN 列表
来源：http://ju.huixinmuqiang.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://jh.newstarts.cn

[Q21] 空值判断
来源：http://ww.521024.cn


<!-- 参考信息 -->