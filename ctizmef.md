代发 wailian999

TS:   process.platform;  process.version
来源：http://bx.szsharing.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://qy.wgjwhj.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://ol.panjiajie.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ap.jctech888.com.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://ud.bjjhwx.cn

================================================================================
来源：http://cx.colortex.cn

N. 数据结构与算法
来源：http://uj.9csxet.cn

================================================================================
来源：http://ke.asd995.cn

[N01] 二分查找（有序数组）
来源：http://tg.hahajie.cn

Py:   bisect.bisect_left(arr, x)
来源：http://dp.huanxung.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://fk.chemitech.net.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://sg.yuexingan06.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ur.muxihuayi.cn

Java: Arrays.binarySearch(arr, x)
来源：http://rq.haigaiapp.cn

Go:   sort.SearchInts(arr, x)
来源：http://ua.wgjwhj.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://cn.haigaiapp.cn

C#:   Array.BinarySearch(arr, x)
来源：http://ao.yuntaijiaju.cn

[N02] 排序（工程实践用内置实现）
来源：http://mw.nicolike.cn

Py:   sorted(arr);  arr.sort()
来源：http://bc.yuexingan06.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://yw.jctech888.com.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://wl.huixinmuqiang.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://bk.hahajie.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ze.bookmarksfly.cn

Go:   slices.Sort(arr)
来源：http://sa.muxihuayi.cn

Ruby: arr.sort
来源：http://xj.newstarts.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://gx.gzmigu.cn

[N03] 快速排序（分治示例）
来源：http://dg.bjjhwx.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://dz.jctech888.com.cn

PHP:  // 递归实现，或用 usort
来源：http://bz.gzmigu.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ik.521024.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://xc.asd995.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://qc.yuexingan06.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ht.shxzskj.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wn.hnjuh.cn

C#:   // 手写递归，或 Array.Sort
来源：http://fr.lnxyls.cn

[N04] 斐波那契数列
来源：http://wh.huixinmuqiang.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://to.huixiangedu.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://nw.huixiangedu.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://is.jianghongdianzi.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ph.jctech888.com.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ar.yuexingan06.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://bs.colortex.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://qm.shxzskj.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://we.asd995.cn

[N05] 最大公约数
来源：http://hg.hahajie.cn

Py:   math.gcd(a, b)
来源：http://op.colortex.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://pa.colortex.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://lg.gzmigu.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ug.9csxet.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://jy.hnjuh.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://pz.huixiangedu.cn

Ruby: a.gcd(b)
来源：http://tx.bookmarksfly.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ur.yuntaijiaju.cn

[N06] 判断回文字符串
来源：http://nw.gzmigu.cn

Py:   s == s[::-1]
来源：http://vk.9csxet.cn

PHP:  $s === strrev($s);
来源：http://ey.muxihuayi.cn

JS:   s === [...s].reverse().join("")
来源：http://rn.colortex.cn

TS:   s === [...s].reverse().join("")
来源：http://oh.shxzukj.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://id.huixiangedu.cn

Go:   // 双指针从两端比较
来源：http://fo.wgjwhj.cn

Ruby: s == s.reverse
来源：http://zd.shxzukj.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://cd.asd995.cn

[N07] 两数之和（返回下标）
来源：http://qe.gzmigu.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://eq.nszjky.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://bb.asd995.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://bp.hnjuh.cn

TS:   // 手写 Map<string, number>
来源：http://aw.shxzskj.cn

Java: // 手写 HashMap
来源：http://bg.jctech888.com.cn

Go:   // 手写 map[int]int
来源：http://jb.newstarts.cn

Ruby: // 手写 Hash
来源：http://ru.asd995.cn

C#:   // 手写 Dictionary<int, int>
来源：http://ux.shxzukj.cn

[N08] 生成全排列
来源：http://cq.hnjuh.cn

Py:   itertools.permutations(arr)
来源：http://rd.panjiajie.cn

PHP:  // 手写递归交换
来源：http://gn.haigaiapp.cn

JS:   // 手写回溯递归
来源：http://cq.9csxet.cn

TS:   // 手写回溯递归
来源：http://bu.bjjhwx.cn

Java: // 手写回溯递归
来源：http://yl.chemitech.net.cn

Go:   // 手写回溯递归
来源：http://lp.nicolike.cn

Ruby: arr.permutation.to_a
来源：http://ue.huixiangedu.cn

C#:   // 手写回溯递归
来源：http://do.huixiangedu.cn

[N09] 栈与队列
来源：http://nx.jianghongdianzi.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://fc.jianghongdianzi.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://jk.nicolike.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://jy.nicolike.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://fq.bookmarksfly.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://lu.huanxung.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://zz.lnxyls.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ga.wgjwhj.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ga.huixinmuqiang.cn

[N10] 链表节点定义
来源：http://rn.colortex.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://dh.shxzukj.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://br.chemitech.net.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://eu.yuexingan06.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://gw.lnxyls.cn

Java: class Node { int v; Node next; }
来源：http://hg.521024.cn

Go:   type Node struct { V int; Next *Node }
来源：http://vx.hahajie.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://oz.szsharing.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://lr.muxihuayi.cn

[N11] 二叉树中序遍历
来源：http://yr.colortex.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://yh.chemitech.net.cn

PHP:  // 手写递归函数
来源：http://am.9csxet.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://sl.colortex.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ed.newstarts.cn

Java: // 手写递归
来源：http://xx.muxihuayi.cn

Go:   // 手写递归
来源：http://bz.lnxyls.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://nx.huixinmuqiang.cn

C#:   // 手写递归
来源：http://uw.haigaiapp.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://kw.shtwfgs.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ui.shxzskj.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://tm.nszjky.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://iv.haigaiapp.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://kj.newstarts.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ez.muxihuayi.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ew.colortex.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://aw.bjjhwx.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://xm.521024.cn

================================================================================
来源：http://qu.asd995.cn

O. 并发与异步
来源：http://ml.jctech888.com.cn

================================================================================
来源：http://mj.chemitech.net.cn

[O01] 启动一个线程
来源：http://tt.nicolike.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://kk.hahajie.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://tk.jianghongdianzi.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://yd.bookmarksfly.cn

TS:   // 同 JS
来源：http://eh.huixinmuqiang.cn

Java: new Thread(() -> f()).start()
来源：http://og.asd995.cn

Go:   go f()
来源：http://sw.colortex.cn

Ruby: Thread.new { f }
来源：http://sn.wgjwhj.cn

C#:   Task.Run(() => F());
来源：http://vr.521024.cn

[O02] 使用线程池
来源：http://mf.hahajie.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://bo.szsharing.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ew.wgjwhj.cn

JS:   // worker_threads 线程池
来源：http://xf.muxihuayi.cn

TS:   // worker_threads 线程池
来源：http://nv.yuexingan06.cn

Java: Executors.newFixedThreadPool(4)
来源：http://sz.nicolike.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wm.colortex.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://lt.jctech888.com.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://yq.szxytkj.cn

[O03] 加锁保护共享数据
来源：http://ss.shxzukj.cn

Py:   with lock: shared += 1
来源：http://ur.huixiangedu.cn

PHP:  // 用 flock() 做文件锁
来源：http://ey.bookmarksfly.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://pa.gzmigu.cn

TS:   // 同 JS
来源：http://vn.chemitech.net.cn

Java: synchronized (this) { shared++; }
来源：http://ao.chemitech.net.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://qj.panjiajie.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://co.panjiajie.cn

C#:   lock (gate) { shared++; }
来源：http://uh.hnjuh.cn

[O04] 定义异步函数并等待
来源：http://aa.bjjhwx.cn

Py:   async def f():⏎    await g()
来源：http://hy.shtwfgs.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://fp.newstarts.cn

JS:   async function f() { await g(); }
来源：http://ja.hnjuh.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://ew.muxihuayi.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://dp.nszjky.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://dm.szxytkj.cn

Ruby: # 用 Fiber 或 async gem
来源：http://st.asd995.cn

C#:   async Task F() { await G(); }
来源：http://pw.panjiajie.cn

[O05] 并发执行并等待全部完成
来源：http://gh.haigaiapp.cn

Py:   asyncio.gather(*tasks)
来源：http://qj.jianghongdianzi.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://tx.jianghongdianzi.cn

JS:   await Promise.all(tasks)
来源：http://nu.wgjwhj.cn

TS:   await Promise.all(tasks)
来源：http://sx.521024.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://py.newstarts.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://oa.haigaiapp.cn

Ruby: threads.map(&:join)
来源：http://mg.muxihuayi.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://yf.shxzskj.cn

[O06] 使用进程池
来源：http://ty.shxzskj.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://dt.muxihuayi.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://tz.bookmarksfly.cn

JS:   // child_process / cluster 模块
来源：http://af.jianghongdianzi.cn

TS:   // child_process / cluster 模块
来源：http://zu.huixiangedu.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://aj.hahajie.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://tk.szsharing.cn

Ruby: // fork 块
来源：http://wt.szxytkj.cn

C#:   Parallel.For
来源：http://bu.panjiajie.cn

================================================================================
来源：http://rn.colortex.cn

P. 常用工具函数
来源：http://nf.panjiajie.cn

================================================================================
来源：http://gx.wgjwhj.cn

[P01] 生成 UUID
来源：http://uv.hahajie.cn

Py:   str(uuid.uuid4())
来源：http://wo.521024.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://bh.newstarts.cn

JS:   crypto.randomUUID()
来源：http://vn.huixiangedu.cn

TS:   crypto.randomUUID()
来源：http://ys.wgjwhj.cn

Java: UUID.randomUUID().toString()
来源：http://tp.szsharing.cn

Go:   // 用 github.com/google/uuid
来源：http://pj.shtwfgs.cn

Ruby: SecureRandom.uuid
来源：http://ai.haigaiapp.cn

C#:   Guid.NewGuid().ToString()
来源：http://vo.newstarts.cn

[P02] MD5 / SHA256 摘要
来源：http://ov.haigaiapp.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ga.szsharing.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://za.lnxyls.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://kg.nicolike.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://zf.wgjwhj.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ym.yuntaijiaju.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://jq.szsharing.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://bz.szxytkj.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://bh.bookmarksfly.cn

[P03] 生成短随机字符串
来源：http://vu.haigaiapp.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://he.newstarts.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://sf.521024.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://em.colortex.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wd.nicolike.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://uv.lnxyls.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ou.shtwfgs.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://rs.panjiajie.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ck.huixiangedu.cn

[P04] 求长度
来源：http://bu.huixiangedu.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://rg.521024.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://qd.jctech888.com.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://lt.9csxet.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://he.jianghongdianzi.cn

Java: list.size();  map.size();  s.length()
来源：http://sm.shtwfgs.cn

Go:   len(arr);  len(m)
来源：http://zh.yuexingan06.cn

Ruby: x.length;  x.size
来源：http://ng.panjiajie.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://pj.haigaiapp.cn

[P05] 判断两个对象内容是否相等
来源：http://hg.yuexingan06.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://wh.colortex.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ef.haigaiapp.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://sg.nicolike.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://fv.colortex.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wo.chemitech.net.cn

Go:   reflect.DeepEqual(a, b)
来源：http://dr.gzmigu.cn

Ruby: a == b
来源：http://vn.szsharing.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://cm.shxzskj.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://xh.521024.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mf.shtwfgs.cn

PHP:  if (empty($x)) {}
来源：http://ci.521024.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://il.bjjhwx.cn

TS:   if (x == null) {}
来源：http://dk.lnxyls.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://dc.panjiajie.cn

Go:   if x == nil {}
来源：http://tj.gzmigu.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ts.panjiajie.cn

C#:   if (x is null) {}
来源：http://mk.shxzskj.cn

[P07] 防抖与节流
来源：http://ed.newstarts.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://in.wgjwhj.cn

PHP:  // 手写时间戳比较
来源：http://sj.9csxet.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://sd.yuntaijiaju.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qp.chemitech.net.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://br.colortex.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ow.yuntaijiaju.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://ye.hahajie.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://gb.shxzskj.cn

[P08] 处理浮点精度问题
来源：http://uy.szsharing.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://md.newstarts.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://bc.gzmigu.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://xi.bjjhwx.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://dk.yuexingan06.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://pp.shxzskj.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://yj.hnjuh.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://oo.huixiangedu.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://uu.shtwfgs.cn

================================================================================
来源：http://ve.nszjky.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://qw.huixinmuqiang.cn

================================================================================
来源：http://zs.bjjhwx.cn

[Q01] 创建表
来源：http://vv.yuexingan06.cn

CREATE TABLE users (
来源：http://yl.shtwfgs.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ui.nszjky.cn

name VARCHAR(50) NOT NULL,
来源：http://ec.szxytkj.cn

email VARCHAR(100) UNIQUE,
来源：http://aj.jctech888.com.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://yc.haigaiapp.cn

);
来源：http://hj.huanxung.cn

[Q02] 创建带外键的表
来源：http://uy.bookmarksfly.cn

CREATE TABLE orders (
来源：http://tq.yuexingan06.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://oh.chemitech.net.cn

user_id INT NOT NULL,
来源：http://cd.gzmigu.cn

amount DECIMAL(10, 2),
来源：http://vp.haigaiapp.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://rz.shxzukj.cn

);
来源：http://zu.huanxung.cn

[Q03] 增加列
来源：http://wq.9csxet.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://de.colortex.cn

[Q04] 修改列类型
来源：http://js.huixinmuqiang.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://nh.wgjwhj.cn

[Q05] 重命名列
来源：http://ac.shxzskj.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ef.shxzukj.cn

[Q06] 删除列
来源：http://si.huixiangedu.cn

ALTER TABLE users DROP COLUMN age;
来源：http://mi.shxzukj.cn

[Q07] 删除表
来源：http://in.szxytkj.cn

DROP TABLE IF EXISTS orders;
来源：http://da.lnxyls.cn

[Q08] 创建普通索引
来源：http://be.nicolike.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://bw.yuexingan06.cn

[Q09] 创建唯一索引
来源：http://lz.huixiangedu.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://kn.yuntaijiaju.cn

[Q10] 插入单行
来源：http://wx.huixiangedu.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://xm.panjiajie.cn

[Q11] 一次插入多行
来源：http://gh.521024.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://qn.nicolike.cn

[Q12] 插入后取自增 ID
来源：http://wi.hahajie.cn

INSERT INTO users (name) VALUES ('C');
来源：http://fc.yuexingan06.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://qh.asd995.cn

[Q13] 忽略重复插入
来源：http://ab.huanxung.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hw.asd995.cn

[Q14] 存在则更新（upsert）
来源：http://kc.hnjuh.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mb.shtwfgs.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://if.haigaiapp.cn

[Q15] 查询全部
来源：http://ci.shxzskj.cn

SELECT * FROM users;
来源：http://ol.bookmarksfly.cn

[Q16] 查询指定列
来源：http://nr.gzmigu.cn

SELECT id, name FROM users;
来源：http://jg.szxytkj.cn

[Q17] 条件查询
来源：http://sj.szsharing.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://rd.shxzukj.cn

[Q18] 模糊匹配
来源：http://or.yuntaijiaju.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://qh.nicolike.cn

[Q19] 范围查询
来源：http://ba.jctech888.com.cn


<!-- 参考信息 -->