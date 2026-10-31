代发 wailian999

C#:   Array.BinarySearch(arr, x)
来源：http://ex.hnjuh.cn

[N02] 排序（工程实践用内置实现）
来源：http://kk.521024.cn

Py:   sorted(arr);  arr.sort()
来源：http://hv.521024.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://cy.huixiangedu.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://wi.hahajie.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://om.bookmarksfly.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://dj.haigaiapp.cn

Go:   slices.Sort(arr)
来源：http://aw.yuexingan06.cn

Ruby: arr.sort
来源：http://qi.hahajie.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://se.hnjuh.cn

[N03] 快速排序（分治示例）
来源：http://ia.panjiajie.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://vu.yuexingan06.cn

PHP:  // 递归实现，或用 usort
来源：http://rv.newstarts.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://il.gzmigu.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://qe.haigaiapp.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://zz.jianghongdianzi.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ee.panjiajie.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://zd.wgjwhj.cn

C#:   // 手写递归，或 Array.Sort
来源：http://wi.szsharing.cn

[N04] 斐波那契数列
来源：http://jo.521024.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://uy.nszjky.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://pn.huanxung.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://cu.bjjhwx.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://cj.wgjwhj.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://sc.colortex.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://cf.521024.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ol.521024.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ai.jctech888.com.cn

[N05] 最大公约数
来源：http://dr.colortex.cn

Py:   math.gcd(a, b)
来源：http://ag.szxytkj.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ia.huixinmuqiang.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ed.chemitech.net.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://vd.nszjky.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://an.nicolike.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://pb.szxytkj.cn

Ruby: a.gcd(b)
来源：http://mz.asd995.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://rw.nicolike.cn

[N06] 判断回文字符串
来源：http://ct.colortex.cn

Py:   s == s[::-1]
来源：http://md.haigaiapp.cn

PHP:  $s === strrev($s);
来源：http://fk.nszjky.cn

JS:   s === [...s].reverse().join("")
来源：http://yg.nicolike.cn

TS:   s === [...s].reverse().join("")
来源：http://nh.huixiangedu.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://rt.colortex.cn

Go:   // 双指针从两端比较
来源：http://yc.9csxet.cn

Ruby: s == s.reverse
来源：http://pe.wgjwhj.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://yv.nicolike.cn

[N07] 两数之和（返回下标）
来源：http://rw.newstarts.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://aj.shxzskj.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://kw.newstarts.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://qc.haigaiapp.cn

TS:   // 手写 Map<string, number>
来源：http://gv.newstarts.cn

Java: // 手写 HashMap
来源：http://cv.wgjwhj.cn

Go:   // 手写 map[int]int
来源：http://un.521024.cn

Ruby: // 手写 Hash
来源：http://wa.bjjhwx.cn

C#:   // 手写 Dictionary<int, int>
来源：http://fo.shxzukj.cn

[N08] 生成全排列
来源：http://mx.chemitech.net.cn

Py:   itertools.permutations(arr)
来源：http://gs.jianghongdianzi.cn

PHP:  // 手写递归交换
来源：http://ur.huanxung.cn

JS:   // 手写回溯递归
来源：http://vq.bjjhwx.cn

TS:   // 手写回溯递归
来源：http://tx.nszjky.cn

Java: // 手写回溯递归
来源：http://wc.panjiajie.cn

Go:   // 手写回溯递归
来源：http://iw.9csxet.cn

Ruby: arr.permutation.to_a
来源：http://ln.shxzukj.cn

C#:   // 手写回溯递归
来源：http://nc.9csxet.cn

[N09] 栈与队列
来源：http://fd.panjiajie.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://go.panjiajie.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ha.521024.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wl.newstarts.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://yu.jctech888.com.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://dj.nicolike.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://qp.huanxung.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://xc.newstarts.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ag.newstarts.cn

[N10] 链表节点定义
来源：http://vh.asd995.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ko.panjiajie.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://je.szxytkj.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://fk.gzmigu.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://sv.huixiangedu.cn

Java: class Node { int v; Node next; }
来源：http://nk.muxihuayi.cn

Go:   type Node struct { V int; Next *Node }
来源：http://pi.nszjky.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://hp.bookmarksfly.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://rs.newstarts.cn

[N11] 二叉树中序遍历
来源：http://na.chemitech.net.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ln.hnjuh.cn

PHP:  // 手写递归函数
来源：http://tx.nicolike.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://dr.newstarts.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://dy.shtwfgs.cn

Java: // 手写递归
来源：http://ex.shtwfgs.cn

Go:   // 手写递归
来源：http://do.newstarts.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ns.chemitech.net.cn

C#:   // 手写递归
来源：http://kn.gzmigu.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://kt.lnxyls.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hp.nicolike.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://da.hnjuh.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://vh.chemitech.net.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://bq.szsharing.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://as.shtwfgs.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://md.bookmarksfly.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ao.shxzukj.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ji.shtwfgs.cn

================================================================================
来源：http://av.yuexingan06.cn

O. 并发与异步
来源：http://mp.lnxyls.cn

================================================================================
来源：http://xi.9csxet.cn

[O01] 启动一个线程
来源：http://kw.hnjuh.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://dg.shxzskj.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://jp.szxytkj.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://vm.newstarts.cn

TS:   // 同 JS
来源：http://gi.huixinmuqiang.cn

Java: new Thread(() -> f()).start()
来源：http://nm.panjiajie.cn

Go:   go f()
来源：http://nz.shxzukj.cn

Ruby: Thread.new { f }
来源：http://rj.9csxet.cn

C#:   Task.Run(() => F());
来源：http://oe.nszjky.cn

[O02] 使用线程池
来源：http://tp.hnjuh.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://vz.nicolike.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://de.asd995.cn

JS:   // worker_threads 线程池
来源：http://nx.colortex.cn

TS:   // worker_threads 线程池
来源：http://vo.jianghongdianzi.cn

Java: Executors.newFixedThreadPool(4)
来源：http://zu.haigaiapp.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hn.bjjhwx.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ta.521024.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://qt.yuntaijiaju.cn

[O03] 加锁保护共享数据
来源：http://dh.wgjwhj.cn

Py:   with lock: shared += 1
来源：http://at.shxzskj.cn

PHP:  // 用 flock() 做文件锁
来源：http://ae.shxzukj.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://lz.asd995.cn

TS:   // 同 JS
来源：http://bq.newstarts.cn

Java: synchronized (this) { shared++; }
来源：http://vp.shxzskj.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://sr.szxytkj.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://py.szsharing.cn

C#:   lock (gate) { shared++; }
来源：http://tj.lnxyls.cn

[O04] 定义异步函数并等待
来源：http://ae.jianghongdianzi.cn

Py:   async def f():⏎    await g()
来源：http://tx.gzmigu.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://gd.hahajie.cn

JS:   async function f() { await g(); }
来源：http://rq.huixiangedu.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://kf.szsharing.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wb.nszjky.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ba.bookmarksfly.cn

Ruby: # 用 Fiber 或 async gem
来源：http://uh.hahajie.cn

C#:   async Task F() { await G(); }
来源：http://wb.huixinmuqiang.cn

[O05] 并发执行并等待全部完成
来源：http://qu.jianghongdianzi.cn

Py:   asyncio.gather(*tasks)
来源：http://nr.colortex.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://vn.521024.cn

JS:   await Promise.all(tasks)
来源：http://cs.lnxyls.cn

TS:   await Promise.all(tasks)
来源：http://of.newstarts.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://gm.huixinmuqiang.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://oh.muxihuayi.cn

Ruby: threads.map(&:join)
来源：http://sa.asd995.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://va.nicolike.cn

[O06] 使用进程池
来源：http://xm.shtwfgs.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://bz.jctech888.com.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://zx.jianghongdianzi.cn

JS:   // child_process / cluster 模块
来源：http://dy.shxzskj.cn

TS:   // child_process / cluster 模块
来源：http://ag.jianghongdianzi.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ef.asd995.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://vj.shtwfgs.cn

Ruby: // fork 块
来源：http://cy.yuntaijiaju.cn

C#:   Parallel.For
来源：http://xe.haigaiapp.cn

================================================================================
来源：http://pt.nicolike.cn

P. 常用工具函数
来源：http://zi.muxihuayi.cn

================================================================================
来源：http://az.chemitech.net.cn

[P01] 生成 UUID
来源：http://pc.muxihuayi.cn

Py:   str(uuid.uuid4())
来源：http://os.huixiangedu.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ff.jianghongdianzi.cn

JS:   crypto.randomUUID()
来源：http://qe.9csxet.cn

TS:   crypto.randomUUID()
来源：http://nn.chemitech.net.cn

Java: UUID.randomUUID().toString()
来源：http://gw.jctech888.com.cn

Go:   // 用 github.com/google/uuid
来源：http://yi.lnxyls.cn

Ruby: SecureRandom.uuid
来源：http://zz.bjjhwx.cn

C#:   Guid.NewGuid().ToString()
来源：http://fv.asd995.cn

[P02] MD5 / SHA256 摘要
来源：http://wi.shxzskj.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hc.nszjky.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://jk.panjiajie.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://oq.colortex.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://tq.yuntaijiaju.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://vb.huixinmuqiang.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://im.yuntaijiaju.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ez.9csxet.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://po.huixiangedu.cn

[P03] 生成短随机字符串
来源：http://rh.yuntaijiaju.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ul.bookmarksfly.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://zb.wgjwhj.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ix.wgjwhj.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://eu.muxihuayi.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hn.hahajie.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://sl.521024.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://ey.shxzukj.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ox.hahajie.cn

[P04] 求长度
来源：http://oc.shxzukj.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://yj.jianghongdianzi.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://bi.haigaiapp.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://na.bookmarksfly.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://yk.muxihuayi.cn

Java: list.size();  map.size();  s.length()
来源：http://ov.hnjuh.cn

Go:   len(arr);  len(m)
来源：http://jg.jctech888.com.cn

Ruby: x.length;  x.size
来源：http://ib.colortex.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://om.jianghongdianzi.cn

[P05] 判断两个对象内容是否相等
来源：http://wq.bookmarksfly.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://cs.yuntaijiaju.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mb.asd995.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://tq.yuexingan06.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://dj.jctech888.com.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hu.9csxet.cn

Go:   reflect.DeepEqual(a, b)
来源：http://ds.jctech888.com.cn

Ruby: a == b
来源：http://gt.colortex.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ee.yuntaijiaju.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ik.colortex.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://gy.chemitech.net.cn

PHP:  if (empty($x)) {}
来源：http://wo.szxytkj.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wl.jianghongdianzi.cn

TS:   if (x == null) {}
来源：http://xm.hahajie.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://ij.huanxung.cn

Go:   if x == nil {}
来源：http://id.newstarts.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://om.shxzukj.cn

C#:   if (x is null) {}
来源：http://lr.huixiangedu.cn

[P07] 防抖与节流
来源：http://ww.jianghongdianzi.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://zb.bookmarksfly.cn

PHP:  // 手写时间戳比较
来源：http://zp.panjiajie.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xc.nszjky.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ql.jianghongdianzi.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://kd.shxzukj.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://vo.yuntaijiaju.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://gd.jianghongdianzi.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://sd.wgjwhj.cn

[P08] 处理浮点精度问题
来源：http://uh.bjjhwx.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://qf.jianghongdianzi.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wm.hnjuh.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://at.haigaiapp.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://fh.yuexingan06.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://kn.yuexingan06.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ba.haigaiapp.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://jm.haigaiapp.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://re.szxytkj.cn

================================================================================
来源：http://dy.huixinmuqiang.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://pu.lnxyls.cn

================================================================================
来源：http://pw.521024.cn

[Q01] 创建表
来源：http://an.huixiangedu.cn

CREATE TABLE users (
来源：http://ul.hahajie.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://qx.wgjwhj.cn

name VARCHAR(50) NOT NULL,
来源：http://zw.nszjky.cn

email VARCHAR(100) UNIQUE,
来源：http://ej.szxytkj.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://iw.jianghongdianzi.cn

);
来源：http://ox.yuexingan06.cn

[Q02] 创建带外键的表
来源：http://aq.jianghongdianzi.cn

CREATE TABLE orders (
来源：http://ut.lnxyls.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://em.hnjuh.cn

user_id INT NOT NULL,
来源：http://nb.shtwfgs.cn

amount DECIMAL(10, 2),
来源：http://rg.gzmigu.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ca.huanxung.cn

);
来源：http://fx.bookmarksfly.cn

[Q03] 增加列
来源：http://mm.jianghongdianzi.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://xf.yuexingan06.cn

[Q04] 修改列类型
来源：http://zx.colortex.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://na.huixiangedu.cn

[Q05] 重命名列
来源：http://ve.yuntaijiaju.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://cz.bjjhwx.cn

[Q06] 删除列
来源：http://ws.hahajie.cn

ALTER TABLE users DROP COLUMN age;
来源：http://zn.szxytkj.cn

[Q07] 删除表
来源：http://ch.szsharing.cn

DROP TABLE IF EXISTS orders;
来源：http://ut.jianghongdianzi.cn

[Q08] 创建普通索引
来源：http://uh.huixiangedu.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://nc.muxihuayi.cn

[Q09] 创建唯一索引
来源：http://ht.szsharing.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://yb.521024.cn

[Q10] 插入单行
来源：http://ms.huixinmuqiang.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hj.521024.cn

[Q11] 一次插入多行
来源：http://sk.hnjuh.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://oe.bjjhwx.cn

[Q12] 插入后取自增 ID
来源：http://cm.wgjwhj.cn

INSERT INTO users (name) VALUES ('C');
来源：http://ha.yuntaijiaju.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://if.lnxyls.cn

[Q13] 忽略重复插入
来源：http://xl.yuntaijiaju.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://fr.nicolike.cn

[Q14] 存在则更新（upsert）
来源：http://do.bookmarksfly.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://cx.jctech888.com.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://zj.shtwfgs.cn

[Q15] 查询全部
来源：http://ag.szxytkj.cn

SELECT * FROM users;
来源：http://vz.huanxung.cn

[Q16] 查询指定列
来源：http://kh.haigaiapp.cn

SELECT id, name FROM users;
来源：http://gt.jctech888.com.cn

[Q17] 条件查询
来源：http://dl.huanxung.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://db.lnxyls.cn

[Q18] 模糊匹配
来源：http://os.yuexingan06.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://dx.9csxet.cn

[Q19] 范围查询
来源：http://ok.yuexingan06.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://oz.szsharing.cn

[Q20] IN 列表
来源：http://xm.huixiangedu.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://jy.hahajie.cn

[Q21] 空值判断
来源：http://tj.yuexingan06.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://al.huixinmuqiang.cn

[Q22] 排序
来源：http://da.shtwfgs.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://lr.jianghongdianzi.cn

[Q23] 分页
来源：http://pn.jianghongdianzi.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mm.huixiangedu.cn

[Q24] 去重
来源：http://nu.jianghongdianzi.cn

SELECT DISTINCT city FROM users;
来源：http://vz.521024.cn

[Q25] 只取前 N 条
来源：http://ru.lnxyls.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mh.shtwfgs.cn

[Q26] 计数
来源：http://pe.521024.cn

SELECT COUNT(*) FROM users;
来源：http://yx.asd995.cn

[Q27] 条件计数
来源：http://ak.panjiajie.cn


<!-- 参考信息 -->