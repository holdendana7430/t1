代发 wailian999

[N01] 二分查找（有序数组）
来源：http://je.newstarts.cn

Py:   bisect.bisect_left(arr, x)
来源：http://cm.wgjwhj.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://me.nicolike.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://sf.szsharing.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://nb.nszjky.cn

Java: Arrays.binarySearch(arr, x)
来源：http://rg.nicolike.cn

Go:   sort.SearchInts(arr, x)
来源：http://ct.panjiajie.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://tc.huixiangedu.cn

C#:   Array.BinarySearch(arr, x)
来源：http://wg.lnxyls.cn

[N02] 排序（工程实践用内置实现）
来源：http://gp.shtwfgs.cn

Py:   sorted(arr);  arr.sort()
来源：http://kw.colortex.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wf.colortex.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://id.gzmigu.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://uw.521024.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://pp.yuntaijiaju.cn

Go:   slices.Sort(arr)
来源：http://jt.panjiajie.cn

Ruby: arr.sort
来源：http://oo.bjjhwx.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://rf.lnxyls.cn

[N03] 快速排序（分治示例）
来源：http://uv.9csxet.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://iw.yuexingan06.cn

PHP:  // 递归实现，或用 usort
来源：http://ho.newstarts.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://rd.bookmarksfly.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mu.huanxung.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://kk.chemitech.net.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wb.wgjwhj.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://bq.yuntaijiaju.cn

C#:   // 手写递归，或 Array.Sort
来源：http://ti.hahajie.cn

[N04] 斐波那契数列
来源：http://zx.521024.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://sc.shxzukj.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://vf.shxzukj.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://re.shxzukj.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://lt.haigaiapp.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://cg.yuexingan06.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://tl.lnxyls.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://pp.szxytkj.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://am.szsharing.cn

[N05] 最大公约数
来源：http://fo.huixiangedu.cn

Py:   math.gcd(a, b)
来源：http://gk.hahajie.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://tj.hahajie.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://np.szxytkj.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://dt.szsharing.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://vy.hnjuh.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://di.gzmigu.cn

Ruby: a.gcd(b)
来源：http://od.colortex.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://yu.yuntaijiaju.cn

[N06] 判断回文字符串
来源：http://jw.bookmarksfly.cn

Py:   s == s[::-1]
来源：http://cz.szsharing.cn

PHP:  $s === strrev($s);
来源：http://vb.521024.cn

JS:   s === [...s].reverse().join("")
来源：http://fx.shxzukj.cn

TS:   s === [...s].reverse().join("")
来源：http://vl.huanxung.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://js.szsharing.cn

Go:   // 双指针从两端比较
来源：http://dt.huixinmuqiang.cn

Ruby: s == s.reverse
来源：http://xs.bookmarksfly.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://bp.newstarts.cn

[N07] 两数之和（返回下标）
来源：http://ob.szsharing.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://lg.jctech888.com.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ib.huanxung.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://pr.521024.cn

TS:   // 手写 Map<string, number>
来源：http://fd.521024.cn

Java: // 手写 HashMap
来源：http://vh.huanxung.cn

Go:   // 手写 map[int]int
来源：http://ez.bjjhwx.cn

Ruby: // 手写 Hash
来源：http://si.gzmigu.cn

C#:   // 手写 Dictionary<int, int>
来源：http://hd.huixinmuqiang.cn

[N08] 生成全排列
来源：http://uh.muxihuayi.cn

Py:   itertools.permutations(arr)
来源：http://gn.nicolike.cn

PHP:  // 手写递归交换
来源：http://hq.huixiangedu.cn

JS:   // 手写回溯递归
来源：http://zd.yuntaijiaju.cn

TS:   // 手写回溯递归
来源：http://lg.wgjwhj.cn

Java: // 手写回溯递归
来源：http://ti.newstarts.cn

Go:   // 手写回溯递归
来源：http://nq.asd995.cn

Ruby: arr.permutation.to_a
来源：http://as.shxzskj.cn

C#:   // 手写回溯递归
来源：http://yu.shtwfgs.cn

[N09] 栈与队列
来源：http://kg.jianghongdianzi.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://nr.panjiajie.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://bp.wgjwhj.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hy.huanxung.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ty.521024.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://qe.shxzukj.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://jh.gzmigu.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://dk.huixinmuqiang.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wh.haigaiapp.cn

[N10] 链表节点定义
来源：http://gi.haigaiapp.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://au.wgjwhj.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://tz.nszjky.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://lr.newstarts.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://za.yuexingan06.cn

Java: class Node { int v; Node next; }
来源：http://ry.szxytkj.cn

Go:   type Node struct { V int; Next *Node }
来源：http://lx.gzmigu.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://xw.panjiajie.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://nc.newstarts.cn

[N11] 二叉树中序遍历
来源：http://sj.hnjuh.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ou.panjiajie.cn

PHP:  // 手写递归函数
来源：http://za.521024.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://xk.shxzskj.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://sm.panjiajie.cn

Java: // 手写递归
来源：http://vm.huanxung.cn

Go:   // 手写递归
来源：http://rf.lnxyls.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://fw.haigaiapp.cn

C#:   // 手写递归
来源：http://ur.bookmarksfly.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://so.muxihuayi.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mk.nszjky.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://xn.521024.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://bj.shtwfgs.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://sg.haigaiapp.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://lm.newstarts.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ae.haigaiapp.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://bb.bookmarksfly.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wh.nszjky.cn

================================================================================
来源：http://kp.jctech888.com.cn

O. 并发与异步
来源：http://iw.nszjky.cn

================================================================================
来源：http://sz.szsharing.cn

[O01] 启动一个线程
来源：http://jz.huanxung.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://we.szxytkj.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ud.yuntaijiaju.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://yo.panjiajie.cn

TS:   // 同 JS
来源：http://vq.muxihuayi.cn

Java: new Thread(() -> f()).start()
来源：http://aq.szxytkj.cn

Go:   go f()
来源：http://ig.lnxyls.cn

Ruby: Thread.new { f }
来源：http://tn.nszjky.cn

C#:   Task.Run(() => F());
来源：http://ei.asd995.cn

[O02] 使用线程池
来源：http://ae.wgjwhj.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://zd.yuntaijiaju.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://kz.szsharing.cn

JS:   // worker_threads 线程池
来源：http://lt.shtwfgs.cn

TS:   // worker_threads 线程池
来源：http://lv.bookmarksfly.cn

Java: Executors.newFixedThreadPool(4)
来源：http://jr.jctech888.com.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ls.colortex.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://sz.newstarts.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://sq.haigaiapp.cn

[O03] 加锁保护共享数据
来源：http://in.newstarts.cn

Py:   with lock: shared += 1
来源：http://jn.panjiajie.cn

PHP:  // 用 flock() 做文件锁
来源：http://kt.wgjwhj.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ju.chemitech.net.cn

TS:   // 同 JS
来源：http://ol.haigaiapp.cn

Java: synchronized (this) { shared++; }
来源：http://jc.521024.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://go.hnjuh.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://ss.huixinmuqiang.cn

C#:   lock (gate) { shared++; }
来源：http://sq.shxzukj.cn

[O04] 定义异步函数并等待
来源：http://jo.hnjuh.cn

Py:   async def f():⏎    await g()
来源：http://oz.colortex.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ey.shtwfgs.cn

JS:   async function f() { await g(); }
来源：http://pe.newstarts.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://nj.shtwfgs.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://yl.chemitech.net.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://qh.shxzskj.cn

Ruby: # 用 Fiber 或 async gem
来源：http://tr.lnxyls.cn

C#:   async Task F() { await G(); }
来源：http://bm.bjjhwx.cn

[O05] 并发执行并等待全部完成
来源：http://uq.yuntaijiaju.cn

Py:   asyncio.gather(*tasks)
来源：http://jd.newstarts.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wk.jianghongdianzi.cn

JS:   await Promise.all(tasks)
来源：http://dn.hnjuh.cn

TS:   await Promise.all(tasks)
来源：http://xj.chemitech.net.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mi.bjjhwx.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://gi.szsharing.cn

Ruby: threads.map(&:join)
来源：http://uw.gzmigu.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://ry.szsharing.cn

[O06] 使用进程池
来源：http://oc.shtwfgs.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://tk.nicolike.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://be.lnxyls.cn

JS:   // child_process / cluster 模块
来源：http://uc.colortex.cn

TS:   // child_process / cluster 模块
来源：http://cz.newstarts.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://cs.huixinmuqiang.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://uc.panjiajie.cn

Ruby: // fork 块
来源：http://yo.lnxyls.cn

C#:   Parallel.For
来源：http://sm.szxytkj.cn

================================================================================
来源：http://zf.colortex.cn

P. 常用工具函数
来源：http://zu.bjjhwx.cn

================================================================================
来源：http://xs.szsharing.cn

[P01] 生成 UUID
来源：http://ud.huixinmuqiang.cn

Py:   str(uuid.uuid4())
来源：http://ai.haigaiapp.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://fk.yuntaijiaju.cn

JS:   crypto.randomUUID()
来源：http://hh.chemitech.net.cn

TS:   crypto.randomUUID()
来源：http://ox.shxzskj.cn

Java: UUID.randomUUID().toString()
来源：http://lf.yuntaijiaju.cn

Go:   // 用 github.com/google/uuid
来源：http://fd.asd995.cn

Ruby: SecureRandom.uuid
来源：http://pj.shtwfgs.cn

C#:   Guid.NewGuid().ToString()
来源：http://ny.shxzukj.cn

[P02] MD5 / SHA256 摘要
来源：http://nn.huanxung.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://kl.shxzskj.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://vq.yuntaijiaju.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hq.chemitech.net.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ez.9csxet.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://yf.asd995.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://st.521024.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ts.huixinmuqiang.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://yq.wgjwhj.cn

[P03] 生成短随机字符串
来源：http://sm.521024.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://nj.jianghongdianzi.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wc.shtwfgs.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://yz.szxytkj.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://vc.colortex.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://qr.colortex.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hx.bookmarksfly.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://lk.muxihuayi.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ja.szxytkj.cn

[P04] 求长度
来源：http://bf.huixinmuqiang.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ob.hnjuh.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://kh.yuntaijiaju.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wd.yuexingan06.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://oe.521024.cn

Java: list.size();  map.size();  s.length()
来源：http://gv.shxzukj.cn

Go:   len(arr);  len(m)
来源：http://fi.huixinmuqiang.cn

Ruby: x.length;  x.size
来源：http://rx.jctech888.com.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://mv.shxzukj.cn

[P05] 判断两个对象内容是否相等
来源：http://fp.panjiajie.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://ru.haigaiapp.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hi.shtwfgs.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://xu.muxihuayi.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://vb.nicolike.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://yn.asd995.cn

Go:   reflect.DeepEqual(a, b)
来源：http://pu.muxihuayi.cn

Ruby: a == b
来源：http://mu.chemitech.net.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://vb.bjjhwx.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://pz.shxzskj.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://qh.bookmarksfly.cn

PHP:  if (empty($x)) {}
来源：http://lu.hnjuh.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://tg.yuntaijiaju.cn

TS:   if (x == null) {}
来源：http://ja.panjiajie.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://fs.nicolike.cn

Go:   if x == nil {}
来源：http://gt.hnjuh.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mc.lnxyls.cn

C#:   if (x is null) {}
来源：http://pl.wgjwhj.cn

[P07] 防抖与节流
来源：http://zi.huanxung.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://dd.szsharing.cn

PHP:  // 手写时间戳比较
来源：http://zb.huixiangedu.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://bf.jctech888.com.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://oc.shxzskj.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wy.nszjky.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ik.bookmarksfly.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://om.shxzskj.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://fc.bookmarksfly.cn

[P08] 处理浮点精度问题
来源：http://pk.haigaiapp.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://qk.huixiangedu.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hf.shtwfgs.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://fl.nicolike.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://rc.newstarts.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://nf.jianghongdianzi.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://qm.yuexingan06.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://jo.gzmigu.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://vy.nicolike.cn

================================================================================
来源：http://oh.huixiangedu.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://bj.yuexingan06.cn

================================================================================
来源：http://ng.wgjwhj.cn

[Q01] 创建表
来源：http://ap.nicolike.cn

CREATE TABLE users (
来源：http://aa.huixinmuqiang.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://fl.521024.cn

name VARCHAR(50) NOT NULL,
来源：http://ff.nicolike.cn

email VARCHAR(100) UNIQUE,
来源：http://ao.szsharing.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://gl.colortex.cn

);
来源：http://rs.bjjhwx.cn

[Q02] 创建带外键的表
来源：http://tr.bookmarksfly.cn

CREATE TABLE orders (
来源：http://qy.panjiajie.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://su.bookmarksfly.cn

user_id INT NOT NULL,
来源：http://pt.jctech888.com.cn

amount DECIMAL(10, 2),
来源：http://ms.haigaiapp.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://qu.huixiangedu.cn

);
来源：http://zr.shxzukj.cn

[Q03] 增加列
来源：http://vt.newstarts.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://kw.szsharing.cn

[Q04] 修改列类型
来源：http://ro.huixinmuqiang.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://kq.jctech888.com.cn

[Q05] 重命名列
来源：http://vr.szxytkj.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://gy.gzmigu.cn

[Q06] 删除列
来源：http://wq.huanxung.cn

ALTER TABLE users DROP COLUMN age;
来源：http://om.shtwfgs.cn

[Q07] 删除表
来源：http://ng.wgjwhj.cn

DROP TABLE IF EXISTS orders;
来源：http://bn.521024.cn

[Q08] 创建普通索引
来源：http://ap.hahajie.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://yi.wgjwhj.cn

[Q09] 创建唯一索引
来源：http://dx.chemitech.net.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://jj.wgjwhj.cn

[Q10] 插入单行
来源：http://ro.panjiajie.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ht.asd995.cn

[Q11] 一次插入多行
来源：http://eo.panjiajie.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mh.shxzukj.cn

[Q12] 插入后取自增 ID
来源：http://px.hahajie.cn

INSERT INTO users (name) VALUES ('C');
来源：http://wu.shxzskj.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://zw.bjjhwx.cn

[Q13] 忽略重复插入
来源：http://kg.colortex.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ol.nszjky.cn

[Q14] 存在则更新（upsert）
来源：http://rz.szxytkj.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://de.lnxyls.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://zh.hnjuh.cn

[Q15] 查询全部
来源：http://bb.9csxet.cn

SELECT * FROM users;
来源：http://ih.szxytkj.cn

[Q16] 查询指定列
来源：http://rx.nszjky.cn

SELECT id, name FROM users;
来源：http://oo.521024.cn

[Q17] 条件查询
来源：http://pi.chemitech.net.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://zf.shtwfgs.cn

[Q18] 模糊匹配
来源：http://rp.hahajie.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://xt.gzmigu.cn

[Q19] 范围查询
来源：http://af.huixinmuqiang.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://kj.asd995.cn

[Q20] IN 列表
来源：http://qh.huixinmuqiang.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://sj.yuntaijiaju.cn

[Q21] 空值判断
来源：http://zr.yuexingan06.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://au.gzmigu.cn

[Q22] 排序
来源：http://xh.szsharing.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://kw.wgjwhj.cn

[Q23] 分页
来源：http://hz.newstarts.cn


<!-- 参考信息 -->