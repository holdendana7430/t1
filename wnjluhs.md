代发 wailian999

C#:   Environment.OSVersion;  Environment.Version
来源：http://iz.szsharing.cn

================================================================================
来源：http://zy.shxzskj.cn

N. 数据结构与算法
来源：http://ze.wgjwhj.cn

================================================================================
来源：http://hm.wgjwhj.cn

[N01] 二分查找（有序数组）
来源：http://lv.521024.cn

Py:   bisect.bisect_left(arr, x)
来源：http://el.hnjuh.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wu.shxzskj.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ms.muxihuayi.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ms.shxzskj.cn

Java: Arrays.binarySearch(arr, x)
来源：http://zo.9csxet.cn

Go:   sort.SearchInts(arr, x)
来源：http://dx.colortex.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://kq.szsharing.cn

C#:   Array.BinarySearch(arr, x)
来源：http://oi.huanxung.cn

[N02] 排序（工程实践用内置实现）
来源：http://vc.huixinmuqiang.cn

Py:   sorted(arr);  arr.sort()
来源：http://il.chemitech.net.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://rd.yuntaijiaju.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://uh.panjiajie.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://wp.muxihuayi.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://kh.bjjhwx.cn

Go:   slices.Sort(arr)
来源：http://mb.huixiangedu.cn

Ruby: arr.sort
来源：http://ps.chemitech.net.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://ih.chemitech.net.cn

[N03] 快速排序（分治示例）
来源：http://my.gzmigu.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://kq.jianghongdianzi.cn

PHP:  // 递归实现，或用 usort
来源：http://vh.lnxyls.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://gd.haigaiapp.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://vw.asd995.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://bg.yuexingan06.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://oc.huixinmuqiang.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://pb.haigaiapp.cn

C#:   // 手写递归，或 Array.Sort
来源：http://kg.wgjwhj.cn

[N04] 斐波那契数列
来源：http://vm.jianghongdianzi.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://dm.yuexingan06.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ro.hnjuh.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://bi.shxzskj.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://bg.yuexingan06.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mq.jianghongdianzi.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://zc.wgjwhj.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://pg.haigaiapp.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hr.asd995.cn

[N05] 最大公约数
来源：http://qy.newstarts.cn

Py:   math.gcd(a, b)
来源：http://rt.gzmigu.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://io.newstarts.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://lu.haigaiapp.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ce.huanxung.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://cl.nicolike.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ww.shxzskj.cn

Ruby: a.gcd(b)
来源：http://gz.bjjhwx.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://eg.yuntaijiaju.cn

[N06] 判断回文字符串
来源：http://hr.nicolike.cn

Py:   s == s[::-1]
来源：http://xt.shxzukj.cn

PHP:  $s === strrev($s);
来源：http://rf.lnxyls.cn

JS:   s === [...s].reverse().join("")
来源：http://lg.gzmigu.cn

TS:   s === [...s].reverse().join("")
来源：http://fd.521024.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wb.haigaiapp.cn

Go:   // 双指针从两端比较
来源：http://wf.haigaiapp.cn

Ruby: s == s.reverse
来源：http://rd.szxytkj.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://nw.haigaiapp.cn

[N07] 两数之和（返回下标）
来源：http://yw.9csxet.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ap.szsharing.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://lv.hahajie.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://sx.hnjuh.cn

TS:   // 手写 Map<string, number>
来源：http://sa.szxytkj.cn

Java: // 手写 HashMap
来源：http://xi.chemitech.net.cn

Go:   // 手写 map[int]int
来源：http://ml.shtwfgs.cn

Ruby: // 手写 Hash
来源：http://st.yuntaijiaju.cn

C#:   // 手写 Dictionary<int, int>
来源：http://zi.bookmarksfly.cn

[N08] 生成全排列
来源：http://pt.chemitech.net.cn

Py:   itertools.permutations(arr)
来源：http://gc.lnxyls.cn

PHP:  // 手写递归交换
来源：http://ah.muxihuayi.cn

JS:   // 手写回溯递归
来源：http://ad.shtwfgs.cn

TS:   // 手写回溯递归
来源：http://hq.panjiajie.cn

Java: // 手写回溯递归
来源：http://uv.panjiajie.cn

Go:   // 手写回溯递归
来源：http://qr.hahajie.cn

Ruby: arr.permutation.to_a
来源：http://oy.chemitech.net.cn

C#:   // 手写回溯递归
来源：http://xn.asd995.cn

[N09] 栈与队列
来源：http://ob.asd995.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://eg.jctech888.com.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://lm.521024.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://dk.colortex.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ip.huixiangedu.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://vf.gzmigu.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://on.jctech888.com.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://rx.lnxyls.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ny.gzmigu.cn

[N10] 链表节点定义
来源：http://nm.szxytkj.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://er.huixinmuqiang.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://ge.yuntaijiaju.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ew.shxzskj.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ax.shxzukj.cn

Java: class Node { int v; Node next; }
来源：http://gw.jctech888.com.cn

Go:   type Node struct { V int; Next *Node }
来源：http://rf.shtwfgs.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://dq.chemitech.net.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://fv.szxytkj.cn

[N11] 二叉树中序遍历
来源：http://dx.bookmarksfly.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://du.chemitech.net.cn

PHP:  // 手写递归函数
来源：http://ey.asd995.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://sh.haigaiapp.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://rs.muxihuayi.cn

Java: // 手写递归
来源：http://zt.lnxyls.cn

Go:   // 手写递归
来源：http://st.huixinmuqiang.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://po.shxzukj.cn

C#:   // 手写递归
来源：http://tu.szsharing.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://sy.bookmarksfly.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://vn.bjjhwx.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wn.szxytkj.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ov.jctech888.com.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ex.jianghongdianzi.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://dd.shtwfgs.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://jv.panjiajie.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://sc.nszjky.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://il.lnxyls.cn

================================================================================
来源：http://bz.newstarts.cn

O. 并发与异步
来源：http://da.hahajie.cn

================================================================================
来源：http://pj.shxzskj.cn

[O01] 启动一个线程
来源：http://hk.nszjky.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://jk.szxytkj.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://sy.newstarts.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ik.newstarts.cn

TS:   // 同 JS
来源：http://ja.nszjky.cn

Java: new Thread(() -> f()).start()
来源：http://sq.shxzskj.cn

Go:   go f()
来源：http://dw.panjiajie.cn

Ruby: Thread.new { f }
来源：http://sy.hahajie.cn

C#:   Task.Run(() => F());
来源：http://pe.9csxet.cn

[O02] 使用线程池
来源：http://nx.bookmarksfly.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://of.jctech888.com.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://aa.nszjky.cn

JS:   // worker_threads 线程池
来源：http://hf.haigaiapp.cn

TS:   // worker_threads 线程池
来源：http://ih.shxzukj.cn

Java: Executors.newFixedThreadPool(4)
来源：http://iz.szxytkj.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://za.nicolike.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ot.nszjky.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hr.hnjuh.cn

[O03] 加锁保护共享数据
来源：http://nz.lnxyls.cn

Py:   with lock: shared += 1
来源：http://yi.panjiajie.cn

PHP:  // 用 flock() 做文件锁
来源：http://sx.shxzukj.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://kd.wgjwhj.cn

TS:   // 同 JS
来源：http://dw.521024.cn

Java: synchronized (this) { shared++; }
来源：http://pj.yuntaijiaju.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://lg.colortex.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://rn.bookmarksfly.cn

C#:   lock (gate) { shared++; }
来源：http://eb.asd995.cn

[O04] 定义异步函数并等待
来源：http://fm.bookmarksfly.cn

Py:   async def f():⏎    await g()
来源：http://cf.9csxet.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://zq.haigaiapp.cn

JS:   async function f() { await g(); }
来源：http://rv.lnxyls.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://ti.nszjky.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://eg.yuexingan06.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://sk.shtwfgs.cn

Ruby: # 用 Fiber 或 async gem
来源：http://cw.jianghongdianzi.cn

C#:   async Task F() { await G(); }
来源：http://yt.colortex.cn

[O05] 并发执行并等待全部完成
来源：http://dn.newstarts.cn

Py:   asyncio.gather(*tasks)
来源：http://zx.wgjwhj.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://cu.9csxet.cn

JS:   await Promise.all(tasks)
来源：http://ez.colortex.cn

TS:   await Promise.all(tasks)
来源：http://nr.jctech888.com.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://pe.lnxyls.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://qb.haigaiapp.cn

Ruby: threads.map(&:join)
来源：http://uj.haigaiapp.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://jn.yuntaijiaju.cn

[O06] 使用进程池
来源：http://lg.asd995.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://fu.huanxung.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://ma.huanxung.cn

JS:   // child_process / cluster 模块
来源：http://tw.shxzukj.cn

TS:   // child_process / cluster 模块
来源：http://ea.muxihuayi.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://lf.yuntaijiaju.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://qw.szsharing.cn

Ruby: // fork 块
来源：http://xp.bookmarksfly.cn

C#:   Parallel.For
来源：http://rk.szxytkj.cn

================================================================================
来源：http://gi.szxytkj.cn

P. 常用工具函数
来源：http://ni.szsharing.cn

================================================================================
来源：http://rb.panjiajie.cn

[P01] 生成 UUID
来源：http://ww.shtwfgs.cn

Py:   str(uuid.uuid4())
来源：http://yk.huanxung.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://se.bookmarksfly.cn

JS:   crypto.randomUUID()
来源：http://hl.hnjuh.cn

TS:   crypto.randomUUID()
来源：http://pd.shxzukj.cn

Java: UUID.randomUUID().toString()
来源：http://nk.gzmigu.cn

Go:   // 用 github.com/google/uuid
来源：http://oy.yuntaijiaju.cn

Ruby: SecureRandom.uuid
来源：http://af.chemitech.net.cn

C#:   Guid.NewGuid().ToString()
来源：http://cc.shtwfgs.cn

[P02] MD5 / SHA256 摘要
来源：http://yw.newstarts.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ww.hnjuh.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://nc.bookmarksfly.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://na.jctech888.com.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wj.hahajie.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ii.szxytkj.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ym.newstarts.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ey.huixinmuqiang.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mr.huixiangedu.cn

[P03] 生成短随机字符串
来源：http://nq.9csxet.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://qq.shxzskj.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://in.shtwfgs.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://yw.bookmarksfly.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://sc.lnxyls.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://pb.huixinmuqiang.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://rl.521024.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://yz.panjiajie.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://px.asd995.cn

[P04] 求长度
来源：http://qu.bookmarksfly.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://iq.jctech888.com.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://io.szsharing.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://tp.panjiajie.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://kx.chemitech.net.cn

Java: list.size();  map.size();  s.length()
来源：http://fd.9csxet.cn

Go:   len(arr);  len(m)
来源：http://kr.jianghongdianzi.cn

Ruby: x.length;  x.size
来源：http://il.jianghongdianzi.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://mp.nicolike.cn

[P05] 判断两个对象内容是否相等
来源：http://py.hahajie.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://hi.521024.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://xg.521024.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://qv.nszjky.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://io.jianghongdianzi.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://bw.shxzukj.cn

Go:   reflect.DeepEqual(a, b)
来源：http://hh.colortex.cn

Ruby: a == b
来源：http://qn.521024.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://st.muxihuayi.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://dq.asd995.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://xn.hnjuh.cn

PHP:  if (empty($x)) {}
来源：http://vg.yuntaijiaju.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://vi.colortex.cn

TS:   if (x == null) {}
来源：http://nj.gzmigu.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://um.szsharing.cn

Go:   if x == nil {}
来源：http://aq.hnjuh.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://qs.shxzukj.cn

C#:   if (x is null) {}
来源：http://kb.szsharing.cn

[P07] 防抖与节流
来源：http://ff.nszjky.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wj.panjiajie.cn

PHP:  // 手写时间戳比较
来源：http://hk.shxzukj.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://jc.huanxung.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://sz.shxzskj.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://my.panjiajie.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ey.asd995.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://vz.chemitech.net.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://om.hahajie.cn

[P08] 处理浮点精度问题
来源：http://zp.yuexingan06.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://dw.shxzskj.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://xm.huixiangedu.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://um.9csxet.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://zy.wgjwhj.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ja.muxihuayi.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://xf.hahajie.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ir.colortex.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://sv.yuexingan06.cn

================================================================================
来源：http://ew.huanxung.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://yc.gzmigu.cn

================================================================================
来源：http://ve.wgjwhj.cn

[Q01] 创建表
来源：http://qv.jctech888.com.cn

CREATE TABLE users (
来源：http://av.521024.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hd.hahajie.cn

name VARCHAR(50) NOT NULL,
来源：http://ln.shtwfgs.cn

email VARCHAR(100) UNIQUE,
来源：http://ai.asd995.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://zm.muxihuayi.cn

);
来源：http://pj.nicolike.cn

[Q02] 创建带外键的表
来源：http://hz.shtwfgs.cn

CREATE TABLE orders (
来源：http://yd.muxihuayi.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://rl.yuntaijiaju.cn

user_id INT NOT NULL,
来源：http://rb.jianghongdianzi.cn

amount DECIMAL(10, 2),
来源：http://zk.jctech888.com.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://nr.nszjky.cn

);
来源：http://hd.521024.cn

[Q03] 增加列
来源：http://bl.9csxet.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://my.nicolike.cn

[Q04] 修改列类型
来源：http://lp.szxytkj.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ic.huixiangedu.cn

[Q05] 重命名列
来源：http://gm.muxihuayi.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wq.huanxung.cn

[Q06] 删除列
来源：http://ru.haigaiapp.cn

ALTER TABLE users DROP COLUMN age;
来源：http://wa.huanxung.cn

[Q07] 删除表
来源：http://di.huixinmuqiang.cn

DROP TABLE IF EXISTS orders;
来源：http://jf.hnjuh.cn

[Q08] 创建普通索引
来源：http://dt.yuntaijiaju.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://ix.bookmarksfly.cn

[Q09] 创建唯一索引
来源：http://yh.wgjwhj.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://oe.haigaiapp.cn

[Q10] 插入单行
来源：http://al.lnxyls.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://kx.hnjuh.cn

[Q11] 一次插入多行
来源：http://nn.hahajie.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ho.asd995.cn

[Q12] 插入后取自增 ID
来源：http://gc.haigaiapp.cn

INSERT INTO users (name) VALUES ('C');
来源：http://tf.szsharing.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://xa.asd995.cn

[Q13] 忽略重复插入
来源：http://gl.gzmigu.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://cc.wgjwhj.cn

[Q14] 存在则更新（upsert）
来源：http://ql.panjiajie.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://sg.huixinmuqiang.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://uq.szsharing.cn

[Q15] 查询全部
来源：http://rf.szsharing.cn

SELECT * FROM users;
来源：http://tb.huanxung.cn

[Q16] 查询指定列
来源：http://of.newstarts.cn

SELECT id, name FROM users;
来源：http://wc.jianghongdianzi.cn

[Q17] 条件查询
来源：http://zp.szsharing.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://qh.nicolike.cn

[Q18] 模糊匹配
来源：http://mz.yuntaijiaju.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://jt.szsharing.cn

[Q19] 范围查询
来源：http://cq.asd995.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hx.hnjuh.cn

[Q20] IN 列表
来源：http://pl.yuntaijiaju.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://vu.shxzskj.cn

[Q21] 空值判断
来源：http://tv.szsharing.cn


<!-- 参考信息 -->