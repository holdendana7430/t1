代发 wailian999

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hd.gzmigu.cn

Java: Arrays.binarySearch(arr, x)
来源：http://ra.yuntaijiaju.cn

Go:   sort.SearchInts(arr, x)
来源：http://jj.hahajie.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://px.chemitech.net.cn

C#:   Array.BinarySearch(arr, x)
来源：http://mj.muxihuayi.cn

[N02] 排序（工程实践用内置实现）
来源：http://bw.huixinmuqiang.cn

Py:   sorted(arr);  arr.sort()
来源：http://pr.szsharing.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://en.jctech888.com.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://gl.jianghongdianzi.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://ck.yuntaijiaju.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://qw.colortex.cn

Go:   slices.Sort(arr)
来源：http://rd.jianghongdianzi.cn

Ruby: arr.sort
来源：http://aa.colortex.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://lh.hahajie.cn

[N03] 快速排序（分治示例）
来源：http://qp.nszjky.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://yp.shtwfgs.cn

PHP:  // 递归实现，或用 usort
来源：http://zi.newstarts.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://km.521024.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ut.bjjhwx.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://jo.nszjky.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://cu.chemitech.net.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://lb.huanxung.cn

C#:   // 手写递归，或 Array.Sort
来源：http://jm.muxihuayi.cn

[N04] 斐波那契数列
来源：http://bh.chemitech.net.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://va.yuexingan06.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://bp.9csxet.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://il.chemitech.net.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://rq.yuexingan06.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://en.asd995.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wj.bjjhwx.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://qi.huixiangedu.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://uf.bookmarksfly.cn

[N05] 最大公约数
来源：http://cr.nszjky.cn

Py:   math.gcd(a, b)
来源：http://gu.yuexingan06.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://fq.szsharing.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://sy.szxytkj.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://on.yuexingan06.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://lq.szsharing.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://pn.hahajie.cn

Ruby: a.gcd(b)
来源：http://ot.szsharing.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ua.nicolike.cn

[N06] 判断回文字符串
来源：http://uf.colortex.cn

Py:   s == s[::-1]
来源：http://kf.newstarts.cn

PHP:  $s === strrev($s);
来源：http://or.hahajie.cn

JS:   s === [...s].reverse().join("")
来源：http://is.asd995.cn

TS:   s === [...s].reverse().join("")
来源：http://qr.jianghongdianzi.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://vy.newstarts.cn

Go:   // 双指针从两端比较
来源：http://fi.asd995.cn

Ruby: s == s.reverse
来源：http://hj.szxytkj.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://yf.521024.cn

[N07] 两数之和（返回下标）
来源：http://jo.szxytkj.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://is.gzmigu.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://xo.szxytkj.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://st.muxihuayi.cn

TS:   // 手写 Map<string, number>
来源：http://dj.521024.cn

Java: // 手写 HashMap
来源：http://tc.gzmigu.cn

Go:   // 手写 map[int]int
来源：http://yh.nszjky.cn

Ruby: // 手写 Hash
来源：http://es.nicolike.cn

C#:   // 手写 Dictionary<int, int>
来源：http://oa.szsharing.cn

[N08] 生成全排列
来源：http://ba.gzmigu.cn

Py:   itertools.permutations(arr)
来源：http://gm.lnxyls.cn

PHP:  // 手写递归交换
来源：http://xh.newstarts.cn

JS:   // 手写回溯递归
来源：http://kl.wgjwhj.cn

TS:   // 手写回溯递归
来源：http://xh.szsharing.cn

Java: // 手写回溯递归
来源：http://uq.gzmigu.cn

Go:   // 手写回溯递归
来源：http://kr.nszjky.cn

Ruby: arr.permutation.to_a
来源：http://qb.bjjhwx.cn

C#:   // 手写回溯递归
来源：http://wi.hahajie.cn

[N09] 栈与队列
来源：http://tr.chemitech.net.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://fw.muxihuayi.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://dw.gzmigu.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://bz.huixinmuqiang.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ns.colortex.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://sj.9csxet.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://we.huixiangedu.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://db.9csxet.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://zu.szxytkj.cn

[N10] 链表节点定义
来源：http://ha.bjjhwx.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://qn.haigaiapp.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://et.9csxet.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://nc.shxzukj.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hq.wgjwhj.cn

Java: class Node { int v; Node next; }
来源：http://mn.panjiajie.cn

Go:   type Node struct { V int; Next *Node }
来源：http://xt.gzmigu.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://dv.bookmarksfly.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://jg.haigaiapp.cn

[N11] 二叉树中序遍历
来源：http://iw.yuexingan06.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://zf.nicolike.cn

PHP:  // 手写递归函数
来源：http://bl.muxihuayi.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://sk.panjiajie.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://eb.chemitech.net.cn

Java: // 手写递归
来源：http://dx.wgjwhj.cn

Go:   // 手写递归
来源：http://rf.newstarts.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://jk.huixiangedu.cn

C#:   // 手写递归
来源：http://yr.jianghongdianzi.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://zn.nicolike.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://zz.nicolike.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ga.521024.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://iu.521024.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://yz.nicolike.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://iu.wgjwhj.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://rn.9csxet.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mk.szxytkj.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://vr.9csxet.cn

================================================================================
来源：http://wi.colortex.cn

O. 并发与异步
来源：http://av.panjiajie.cn

================================================================================
来源：http://nl.chemitech.net.cn

[O01] 启动一个线程
来源：http://vw.asd995.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ch.szxytkj.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://td.huanxung.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://rn.colortex.cn

TS:   // 同 JS
来源：http://ao.jctech888.com.cn

Java: new Thread(() -> f()).start()
来源：http://mn.shxzukj.cn

Go:   go f()
来源：http://mq.hahajie.cn

Ruby: Thread.new { f }
来源：http://wz.shtwfgs.cn

C#:   Task.Run(() => F());
来源：http://hz.huixinmuqiang.cn

[O02] 使用线程池
来源：http://kv.yuexingan06.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://fg.haigaiapp.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://xy.panjiajie.cn

JS:   // worker_threads 线程池
来源：http://dp.shxzukj.cn

TS:   // worker_threads 线程池
来源：http://rf.szsharing.cn

Java: Executors.newFixedThreadPool(4)
来源：http://ov.panjiajie.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://im.huanxung.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://bh.hahajie.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hy.shxzukj.cn

[O03] 加锁保护共享数据
来源：http://jx.yuexingan06.cn

Py:   with lock: shared += 1
来源：http://jd.colortex.cn

PHP:  // 用 flock() 做文件锁
来源：http://rt.9csxet.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://id.szsharing.cn

TS:   // 同 JS
来源：http://pz.9csxet.cn

Java: synchronized (this) { shared++; }
来源：http://as.shxzskj.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ws.shxzukj.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://tq.521024.cn

C#:   lock (gate) { shared++; }
来源：http://gs.bjjhwx.cn

[O04] 定义异步函数并等待
来源：http://em.lnxyls.cn

Py:   async def f():⏎    await g()
来源：http://bt.jianghongdianzi.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://fg.shxzukj.cn

JS:   async function f() { await g(); }
来源：http://xe.panjiajie.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://xy.wgjwhj.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://zf.haigaiapp.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ec.nicolike.cn

Ruby: # 用 Fiber 或 async gem
来源：http://gl.huixinmuqiang.cn

C#:   async Task F() { await G(); }
来源：http://ak.panjiajie.cn

[O05] 并发执行并等待全部完成
来源：http://pu.shxzskj.cn

Py:   asyncio.gather(*tasks)
来源：http://pg.shxzskj.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://rs.newstarts.cn

JS:   await Promise.all(tasks)
来源：http://mk.haigaiapp.cn

TS:   await Promise.all(tasks)
来源：http://gg.shxzskj.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://xe.hnjuh.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://kq.yuntaijiaju.cn

Ruby: threads.map(&:join)
来源：http://ll.yuntaijiaju.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://ej.szxytkj.cn

[O06] 使用进程池
来源：http://jr.shtwfgs.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://dx.jctech888.com.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://qi.shxzukj.cn

JS:   // child_process / cluster 模块
来源：http://ky.wgjwhj.cn

TS:   // child_process / cluster 模块
来源：http://is.nicolike.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ku.hahajie.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://pz.jctech888.com.cn

Ruby: // fork 块
来源：http://hd.yuexingan06.cn

C#:   Parallel.For
来源：http://in.szxytkj.cn

================================================================================
来源：http://ib.521024.cn

P. 常用工具函数
来源：http://rt.newstarts.cn

================================================================================
来源：http://yj.hahajie.cn

[P01] 生成 UUID
来源：http://gw.wgjwhj.cn

Py:   str(uuid.uuid4())
来源：http://mj.nicolike.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://eo.9csxet.cn

JS:   crypto.randomUUID()
来源：http://vi.jianghongdianzi.cn

TS:   crypto.randomUUID()
来源：http://jl.jctech888.com.cn

Java: UUID.randomUUID().toString()
来源：http://bb.hahajie.cn

Go:   // 用 github.com/google/uuid
来源：http://kb.haigaiapp.cn

Ruby: SecureRandom.uuid
来源：http://fv.hahajie.cn

C#:   Guid.NewGuid().ToString()
来源：http://vn.newstarts.cn

[P02] MD5 / SHA256 摘要
来源：http://ax.colortex.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://eo.shtwfgs.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://ac.hahajie.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://co.hahajie.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://yc.colortex.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://uc.colortex.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://pa.521024.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://du.shxzskj.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://jq.shxzskj.cn

[P03] 生成短随机字符串
来源：http://zm.bookmarksfly.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://lc.bookmarksfly.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://sx.chemitech.net.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://pn.bjjhwx.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ip.muxihuayi.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://dj.panjiajie.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://qm.panjiajie.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://qb.huanxung.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ke.huanxung.cn

[P04] 求长度
来源：http://am.jctech888.com.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ww.colortex.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ei.huixiangedu.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ls.szxytkj.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://qx.9csxet.cn

Java: list.size();  map.size();  s.length()
来源：http://fr.hnjuh.cn

Go:   len(arr);  len(m)
来源：http://fu.521024.cn

Ruby: x.length;  x.size
来源：http://kp.muxihuayi.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://ax.nszjky.cn

[P05] 判断两个对象内容是否相等
来源：http://ou.lnxyls.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://al.lnxyls.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://fi.colortex.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://cb.yuntaijiaju.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://nn.haigaiapp.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://tf.hnjuh.cn

Go:   reflect.DeepEqual(a, b)
来源：http://mw.yuexingan06.cn

Ruby: a == b
来源：http://tt.jctech888.com.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hr.asd995.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://st.muxihuayi.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://qm.9csxet.cn

PHP:  if (empty($x)) {}
来源：http://lx.asd995.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://cq.hahajie.cn

TS:   if (x == null) {}
来源：http://jy.shxzskj.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://so.chemitech.net.cn

Go:   if x == nil {}
来源：http://up.lnxyls.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://bu.jianghongdianzi.cn

C#:   if (x is null) {}
来源：http://yo.muxihuayi.cn

[P07] 防抖与节流
来源：http://yr.newstarts.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://vq.shtwfgs.cn

PHP:  // 手写时间戳比较
来源：http://ep.gzmigu.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://fk.huixinmuqiang.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://va.nszjky.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://in.szsharing.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://di.521024.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://eo.szsharing.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://eo.haigaiapp.cn

[P08] 处理浮点精度问题
来源：http://ui.jctech888.com.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://re.newstarts.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://jh.shxzskj.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://vk.haigaiapp.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://nm.shxzskj.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://fg.lnxyls.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://xa.yuntaijiaju.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://oo.gzmigu.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://is.shxzskj.cn

================================================================================
来源：http://gg.jianghongdianzi.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://xc.lnxyls.cn

================================================================================
来源：http://id.bjjhwx.cn

[Q01] 创建表
来源：http://ra.bookmarksfly.cn

CREATE TABLE users (
来源：http://uz.lnxyls.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ct.jctech888.com.cn

name VARCHAR(50) NOT NULL,
来源：http://dk.521024.cn

email VARCHAR(100) UNIQUE,
来源：http://vz.colortex.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ex.jctech888.com.cn

);
来源：http://zk.jctech888.com.cn

[Q02] 创建带外键的表
来源：http://kq.shxzskj.cn

CREATE TABLE orders (
来源：http://rc.huanxung.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://kc.wgjwhj.cn

user_id INT NOT NULL,
来源：http://mb.lnxyls.cn

amount DECIMAL(10, 2),
来源：http://ot.nicolike.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://sc.nicolike.cn

);
来源：http://ca.bookmarksfly.cn

[Q03] 增加列
来源：http://bc.lnxyls.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://fp.muxihuayi.cn

[Q04] 修改列类型
来源：http://wj.nicolike.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://qu.yuntaijiaju.cn

[Q05] 重命名列
来源：http://sj.hnjuh.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://se.9csxet.cn

[Q06] 删除列
来源：http://hh.gzmigu.cn

ALTER TABLE users DROP COLUMN age;
来源：http://jt.chemitech.net.cn

[Q07] 删除表
来源：http://kj.lnxyls.cn

DROP TABLE IF EXISTS orders;
来源：http://sg.nszjky.cn

[Q08] 创建普通索引
来源：http://ep.shxzskj.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://wa.gzmigu.cn

[Q09] 创建唯一索引
来源：http://ot.shxzskj.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ce.asd995.cn

[Q10] 插入单行
来源：http://mi.haigaiapp.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://bz.nicolike.cn

[Q11] 一次插入多行
来源：http://qz.newstarts.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://go.bookmarksfly.cn

[Q12] 插入后取自增 ID
来源：http://aq.yuexingan06.cn

INSERT INTO users (name) VALUES ('C');
来源：http://pc.muxihuayi.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ny.szxytkj.cn

[Q13] 忽略重复插入
来源：http://dv.shxzukj.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://dc.szxytkj.cn

[Q14] 存在则更新（upsert）
来源：http://je.jctech888.com.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://rf.nicolike.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://dy.huixinmuqiang.cn

[Q15] 查询全部
来源：http://zg.yuexingan06.cn

SELECT * FROM users;
来源：http://gf.shxzukj.cn

[Q16] 查询指定列
来源：http://uy.shxzskj.cn

SELECT id, name FROM users;
来源：http://wa.yuexingan06.cn

[Q17] 条件查询
来源：http://fc.newstarts.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://zd.haigaiapp.cn

[Q18] 模糊匹配
来源：http://wk.bjjhwx.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://xk.hahajie.cn

[Q19] 范围查询
来源：http://uz.jctech888.com.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ds.bjjhwx.cn

[Q20] IN 列表
来源：http://ke.huanxung.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://vm.shxzukj.cn

[Q21] 空值判断
来源：http://av.bookmarksfly.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://gr.jctech888.com.cn

[Q22] 排序
来源：http://jb.jianghongdianzi.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://rm.chemitech.net.cn

[Q23] 分页
来源：http://bh.lnxyls.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ab.shxzskj.cn

[Q24] 去重
来源：http://ff.colortex.cn

SELECT DISTINCT city FROM users;
来源：http://cv.huanxung.cn

[Q25] 只取前 N 条
来源：http://zj.asd995.cn


<!-- 参考信息 -->