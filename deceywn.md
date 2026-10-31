代发 wailian999

C#:   Environment.OSVersion;  Environment.Version
来源：http://pj.yuntaijiaju.cn

================================================================================
来源：http://si.9csxet.cn

N. 数据结构与算法
来源：http://ij.asd995.cn

================================================================================
来源：http://oj.chemitech.net.cn

[N01] 二分查找（有序数组）
来源：http://hn.huanxung.cn

Py:   bisect.bisect_left(arr, x)
来源：http://ac.nicolike.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://gy.yuntaijiaju.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://tz.wgjwhj.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://bd.shxzskj.cn

Java: Arrays.binarySearch(arr, x)
来源：http://ob.huixinmuqiang.cn

Go:   sort.SearchInts(arr, x)
来源：http://kx.521024.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://pu.colortex.cn

C#:   Array.BinarySearch(arr, x)
来源：http://kq.muxihuayi.cn

[N02] 排序（工程实践用内置实现）
来源：http://wp.yuexingan06.cn

Py:   sorted(arr);  arr.sort()
来源：http://xs.bookmarksfly.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wa.haigaiapp.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://iy.szxytkj.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://fe.szxytkj.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://vk.haigaiapp.cn

Go:   slices.Sort(arr)
来源：http://ks.panjiajie.cn

Ruby: arr.sort
来源：http://qq.szxytkj.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://qb.jianghongdianzi.cn

[N03] 快速排序（分治示例）
来源：http://li.521024.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://os.newstarts.cn

PHP:  // 递归实现，或用 usort
来源：http://db.colortex.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ye.shxzskj.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wp.shxzskj.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ro.huanxung.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://xv.yuexingan06.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://bc.bjjhwx.cn

C#:   // 手写递归，或 Array.Sort
来源：http://kw.wgjwhj.cn

[N04] 斐波那契数列
来源：http://hd.haigaiapp.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://cn.huixinmuqiang.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hk.shxzukj.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://oo.yuntaijiaju.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ja.jianghongdianzi.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ea.gzmigu.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wd.bookmarksfly.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://rd.shtwfgs.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ku.shxzskj.cn

[N05] 最大公约数
来源：http://zr.yuntaijiaju.cn

Py:   math.gcd(a, b)
来源：http://xn.asd995.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wz.nicolike.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ki.jianghongdianzi.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ym.shxzukj.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://nn.jianghongdianzi.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://xa.nszjky.cn

Ruby: a.gcd(b)
来源：http://qr.huixiangedu.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://jr.szxytkj.cn

[N06] 判断回文字符串
来源：http://lh.asd995.cn

Py:   s == s[::-1]
来源：http://ca.szxytkj.cn

PHP:  $s === strrev($s);
来源：http://kt.colortex.cn

JS:   s === [...s].reverse().join("")
来源：http://jz.muxihuayi.cn

TS:   s === [...s].reverse().join("")
来源：http://ws.shtwfgs.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ui.gzmigu.cn

Go:   // 双指针从两端比较
来源：http://wz.szxytkj.cn

Ruby: s == s.reverse
来源：http://sw.521024.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://cx.lnxyls.cn

[N07] 两数之和（返回下标）
来源：http://bl.jctech888.com.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://uj.yuexingan06.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ng.szxytkj.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://gt.chemitech.net.cn

TS:   // 手写 Map<string, number>
来源：http://ln.shxzskj.cn

Java: // 手写 HashMap
来源：http://er.gzmigu.cn

Go:   // 手写 map[int]int
来源：http://tt.huixinmuqiang.cn

Ruby: // 手写 Hash
来源：http://nx.wgjwhj.cn

C#:   // 手写 Dictionary<int, int>
来源：http://bl.nszjky.cn

[N08] 生成全排列
来源：http://rp.colortex.cn

Py:   itertools.permutations(arr)
来源：http://df.jctech888.com.cn

PHP:  // 手写递归交换
来源：http://jx.chemitech.net.cn

JS:   // 手写回溯递归
来源：http://nl.szxytkj.cn

TS:   // 手写回溯递归
来源：http://zt.gzmigu.cn

Java: // 手写回溯递归
来源：http://pc.shxzskj.cn

Go:   // 手写回溯递归
来源：http://tn.yuntaijiaju.cn

Ruby: arr.permutation.to_a
来源：http://an.huanxung.cn

C#:   // 手写回溯递归
来源：http://gq.bookmarksfly.cn

[N09] 栈与队列
来源：http://vf.yuexingan06.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ku.muxihuayi.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://qv.panjiajie.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://jo.asd995.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://qa.szxytkj.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://lk.yuexingan06.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://kg.gzmigu.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://cu.szsharing.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mc.jianghongdianzi.cn

[N10] 链表节点定义
来源：http://fr.9csxet.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://gn.nszjky.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://wz.huixiangedu.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://at.nszjky.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://nu.bjjhwx.cn

Java: class Node { int v; Node next; }
来源：http://ny.huixinmuqiang.cn

Go:   type Node struct { V int; Next *Node }
来源：http://pr.szxytkj.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://oc.szsharing.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://sc.lnxyls.cn

[N11] 二叉树中序遍历
来源：http://xg.gzmigu.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://pa.huixiangedu.cn

PHP:  // 手写递归函数
来源：http://ry.szsharing.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://vd.lnxyls.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://bo.jianghongdianzi.cn

Java: // 手写递归
来源：http://kv.huanxung.cn

Go:   // 手写递归
来源：http://wo.haigaiapp.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://tp.shtwfgs.cn

C#:   // 手写递归
来源：http://gd.szxytkj.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://zd.panjiajie.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://rc.yuntaijiaju.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://xo.huixiangedu.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://yk.hahajie.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://lt.lnxyls.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wa.wgjwhj.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://nr.9csxet.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ey.szsharing.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://lb.bjjhwx.cn

================================================================================
来源：http://gi.panjiajie.cn

O. 并发与异步
来源：http://nn.nszjky.cn

================================================================================
来源：http://jj.muxihuayi.cn

[O01] 启动一个线程
来源：http://ys.shxzskj.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://vk.wgjwhj.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ut.szsharing.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://zd.bjjhwx.cn

TS:   // 同 JS
来源：http://lm.huixinmuqiang.cn

Java: new Thread(() -> f()).start()
来源：http://vt.nicolike.cn

Go:   go f()
来源：http://og.hnjuh.cn

Ruby: Thread.new { f }
来源：http://ua.nszjky.cn

C#:   Task.Run(() => F());
来源：http://ul.huanxung.cn

[O02] 使用线程池
来源：http://ua.panjiajie.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://dc.9csxet.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mk.521024.cn

JS:   // worker_threads 线程池
来源：http://tb.yuexingan06.cn

TS:   // worker_threads 线程池
来源：http://fn.wgjwhj.cn

Java: Executors.newFixedThreadPool(4)
来源：http://bk.haigaiapp.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://el.wgjwhj.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://eg.yuntaijiaju.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://sg.bjjhwx.cn

[O03] 加锁保护共享数据
来源：http://kd.shtwfgs.cn

Py:   with lock: shared += 1
来源：http://yk.panjiajie.cn

PHP:  // 用 flock() 做文件锁
来源：http://xo.hahajie.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ji.huixiangedu.cn

TS:   // 同 JS
来源：http://tj.szsharing.cn

Java: synchronized (this) { shared++; }
来源：http://ip.huanxung.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ih.szsharing.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.colortex.cn

C#:   lock (gate) { shared++; }
来源：http://fx.yuexingan06.cn

[O04] 定义异步函数并等待
来源：http://bo.newstarts.cn

Py:   async def f():⏎    await g()
来源：http://sj.yuexingan06.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ha.yuexingan06.cn

JS:   async function f() { await g(); }
来源：http://rg.jctech888.com.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://jw.nszjky.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://xf.hnjuh.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://id.nszjky.cn

Ruby: # 用 Fiber 或 async gem
来源：http://gw.haigaiapp.cn

C#:   async Task F() { await G(); }
来源：http://tt.521024.cn

[O05] 并发执行并等待全部完成
来源：http://zf.nszjky.cn

Py:   asyncio.gather(*tasks)
来源：http://yu.shtwfgs.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hu.panjiajie.cn

JS:   await Promise.all(tasks)
来源：http://zm.gzmigu.cn

TS:   await Promise.all(tasks)
来源：http://vm.newstarts.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://if.shtwfgs.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://gb.chemitech.net.cn

Ruby: threads.map(&:join)
来源：http://rn.shxzskj.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://wf.asd995.cn

[O06] 使用进程池
来源：http://od.shtwfgs.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://da.colortex.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://jg.newstarts.cn

JS:   // child_process / cluster 模块
来源：http://xr.haigaiapp.cn

TS:   // child_process / cluster 模块
来源：http://ac.jctech888.com.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mp.521024.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://gc.shxzskj.cn

Ruby: // fork 块
来源：http://if.bjjhwx.cn

C#:   Parallel.For
来源：http://oy.yuntaijiaju.cn

================================================================================
来源：http://rx.chemitech.net.cn

P. 常用工具函数
来源：http://zz.huixinmuqiang.cn

================================================================================
来源：http://fd.shxzukj.cn

[P01] 生成 UUID
来源：http://yg.hahajie.cn

Py:   str(uuid.uuid4())
来源：http://kd.bookmarksfly.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://yl.9csxet.cn

JS:   crypto.randomUUID()
来源：http://de.bookmarksfly.cn

TS:   crypto.randomUUID()
来源：http://fi.yuntaijiaju.cn

Java: UUID.randomUUID().toString()
来源：http://hj.huixinmuqiang.cn

Go:   // 用 github.com/google/uuid
来源：http://ck.hnjuh.cn

Ruby: SecureRandom.uuid
来源：http://zr.haigaiapp.cn

C#:   Guid.NewGuid().ToString()
来源：http://vh.hahajie.cn

[P02] MD5 / SHA256 摘要
来源：http://ip.bjjhwx.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://gk.haigaiapp.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://em.muxihuayi.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://bf.hahajie.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://fb.haigaiapp.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://rf.bookmarksfly.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wr.panjiajie.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://qu.gzmigu.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://is.shtwfgs.cn

[P03] 生成短随机字符串
来源：http://re.hnjuh.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://de.nicolike.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://bl.haigaiapp.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ye.521024.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://un.bjjhwx.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://rs.nszjky.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://dx.jianghongdianzi.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://qi.yuntaijiaju.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://xr.szxytkj.cn

[P04] 求长度
来源：http://vc.9csxet.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://xw.9csxet.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://fo.lnxyls.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://lw.haigaiapp.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ux.wgjwhj.cn

Java: list.size();  map.size();  s.length()
来源：http://ek.asd995.cn

Go:   len(arr);  len(m)
来源：http://li.haigaiapp.cn

Ruby: x.length;  x.size
来源：http://ba.asd995.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://xy.yuexingan06.cn

[P05] 判断两个对象内容是否相等
来源：http://lu.521024.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://ku.haigaiapp.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://nk.wgjwhj.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://zs.huixiangedu.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mt.hahajie.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://jn.haigaiapp.cn

Go:   reflect.DeepEqual(a, b)
来源：http://vj.shxzskj.cn

Ruby: a == b
来源：http://tq.shxzskj.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://an.shxzskj.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://pw.bookmarksfly.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://kw.asd995.cn

PHP:  if (empty($x)) {}
来源：http://ve.jctech888.com.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://tv.chemitech.net.cn

TS:   if (x == null) {}
来源：http://zp.huixinmuqiang.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://vy.lnxyls.cn

Go:   if x == nil {}
来源：http://gz.muxihuayi.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://gt.521024.cn

C#:   if (x is null) {}
来源：http://ol.newstarts.cn

[P07] 防抖与节流
来源：http://to.huixiangedu.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ar.gzmigu.cn

PHP:  // 手写时间戳比较
来源：http://li.szsharing.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ah.chemitech.net.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qr.bookmarksfly.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hf.muxihuayi.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://fq.haigaiapp.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://go.shxzukj.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://vm.wgjwhj.cn

[P08] 处理浮点精度问题
来源：http://nc.9csxet.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://vu.yuexingan06.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://od.huixiangedu.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://bo.shtwfgs.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://dy.gzmigu.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://pp.haigaiapp.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wz.asd995.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://oy.lnxyls.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://dj.muxihuayi.cn

================================================================================
来源：http://pd.huanxung.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ja.521024.cn

================================================================================
来源：http://jn.nicolike.cn

[Q01] 创建表
来源：http://qx.asd995.cn

CREATE TABLE users (
来源：http://hz.shtwfgs.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://bi.huanxung.cn

name VARCHAR(50) NOT NULL,
来源：http://kg.jctech888.com.cn

email VARCHAR(100) UNIQUE,
来源：http://yr.shxzukj.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wp.colortex.cn

);
来源：http://je.yuexingan06.cn

[Q02] 创建带外键的表
来源：http://vo.shxzukj.cn

CREATE TABLE orders (
来源：http://oc.hahajie.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://rk.hnjuh.cn

user_id INT NOT NULL,
来源：http://fu.wgjwhj.cn

amount DECIMAL(10, 2),
来源：http://kz.wgjwhj.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mq.huanxung.cn

);
来源：http://tc.asd995.cn

[Q03] 增加列
来源：http://pg.colortex.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ei.huixinmuqiang.cn

[Q04] 修改列类型
来源：http://ed.jianghongdianzi.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ow.bjjhwx.cn

[Q05] 重命名列
来源：http://pm.yuntaijiaju.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ft.yuexingan06.cn

[Q06] 删除列
来源：http://lu.521024.cn

ALTER TABLE users DROP COLUMN age;
来源：http://jw.nszjky.cn

[Q07] 删除表
来源：http://lv.hahajie.cn

DROP TABLE IF EXISTS orders;
来源：http://oj.newstarts.cn

[Q08] 创建普通索引
来源：http://ms.asd995.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://zw.bookmarksfly.cn

[Q09] 创建唯一索引
来源：http://gf.newstarts.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://vy.panjiajie.cn

[Q10] 插入单行
来源：http://ft.hnjuh.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://cb.shtwfgs.cn

[Q11] 一次插入多行
来源：http://uy.jianghongdianzi.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://du.muxihuayi.cn

[Q12] 插入后取自增 ID
来源：http://yk.9csxet.cn

INSERT INTO users (name) VALUES ('C');
来源：http://pw.yuntaijiaju.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://gy.bookmarksfly.cn

[Q13] 忽略重复插入
来源：http://hp.hnjuh.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wa.huanxung.cn

[Q14] 存在则更新（upsert）
来源：http://ms.panjiajie.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://bs.yuexingan06.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ko.lnxyls.cn

[Q15] 查询全部
来源：http://wl.haigaiapp.cn

SELECT * FROM users;
来源：http://er.yuexingan06.cn

[Q16] 查询指定列
来源：http://xg.wgjwhj.cn

SELECT id, name FROM users;
来源：http://fy.hahajie.cn

[Q17] 条件查询
来源：http://oh.newstarts.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://cy.nicolike.cn

[Q18] 模糊匹配
来源：http://zu.huixiangedu.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://jg.shxzskj.cn

[Q19] 范围查询
来源：http://yr.nicolike.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://nx.bookmarksfly.cn

[Q20] IN 列表
来源：http://se.hnjuh.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://zf.9csxet.cn

[Q21] 空值判断
来源：http://qh.newstarts.cn


<!-- 参考信息 -->