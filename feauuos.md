代发 wailian999

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://gu.szxytkj.cn

Java: Arrays.binarySearch(arr, x)
来源：http://eg.nicolike.cn

Go:   sort.SearchInts(arr, x)
来源：http://nm.bookmarksfly.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://xf.shxzskj.cn

C#:   Array.BinarySearch(arr, x)
来源：http://ks.huixiangedu.cn

[N02] 排序（工程实践用内置实现）
来源：http://wq.nszjky.cn

Py:   sorted(arr);  arr.sort()
来源：http://av.hnjuh.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://uv.hahajie.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://vl.huixiangedu.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://hn.hahajie.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://si.asd995.cn

Go:   slices.Sort(arr)
来源：http://vj.bookmarksfly.cn

Ruby: arr.sort
来源：http://lk.shxzukj.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://ld.jianghongdianzi.cn

[N03] 快速排序（分治示例）
来源：http://jt.hahajie.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ud.wgjwhj.cn

PHP:  // 递归实现，或用 usort
来源：http://hl.yuntaijiaju.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://qg.bookmarksfly.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://sn.newstarts.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://fl.521024.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ub.lnxyls.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ce.szsharing.cn

C#:   // 手写递归，或 Array.Sort
来源：http://vp.hnjuh.cn

[N04] 斐波那契数列
来源：http://ir.haigaiapp.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://lz.haigaiapp.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ef.szsharing.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ta.haigaiapp.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ov.hnjuh.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mk.huixiangedu.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mj.gzmigu.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ys.huixiangedu.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://om.9csxet.cn

[N05] 最大公约数
来源：http://gc.hahajie.cn

Py:   math.gcd(a, b)
来源：http://ck.szsharing.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hb.huixiangedu.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://je.wgjwhj.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ol.haigaiapp.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://qb.shtwfgs.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ei.bjjhwx.cn

Ruby: a.gcd(b)
来源：http://qj.nszjky.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://xd.nicolike.cn

[N06] 判断回文字符串
来源：http://iv.yuexingan06.cn

Py:   s == s[::-1]
来源：http://th.9csxet.cn

PHP:  $s === strrev($s);
来源：http://th.haigaiapp.cn

JS:   s === [...s].reverse().join("")
来源：http://ct.gzmigu.cn

TS:   s === [...s].reverse().join("")
来源：http://fm.newstarts.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://qy.nicolike.cn

Go:   // 双指针从两端比较
来源：http://ba.huanxung.cn

Ruby: s == s.reverse
来源：http://ed.szsharing.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://ur.jianghongdianzi.cn

[N07] 两数之和（返回下标）
来源：http://ap.lnxyls.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://jq.jctech888.com.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://fx.panjiajie.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://oo.huixiangedu.cn

TS:   // 手写 Map<string, number>
来源：http://pt.haigaiapp.cn

Java: // 手写 HashMap
来源：http://gj.shtwfgs.cn

Go:   // 手写 map[int]int
来源：http://ew.lnxyls.cn

Ruby: // 手写 Hash
来源：http://ab.haigaiapp.cn

C#:   // 手写 Dictionary<int, int>
来源：http://xi.panjiajie.cn

[N08] 生成全排列
来源：http://kb.muxihuayi.cn

Py:   itertools.permutations(arr)
来源：http://sl.521024.cn

PHP:  // 手写递归交换
来源：http://bw.bjjhwx.cn

JS:   // 手写回溯递归
来源：http://ux.asd995.cn

TS:   // 手写回溯递归
来源：http://fa.bookmarksfly.cn

Java: // 手写回溯递归
来源：http://yo.yuntaijiaju.cn

Go:   // 手写回溯递归
来源：http://hp.newstarts.cn

Ruby: arr.permutation.to_a
来源：http://zg.yuntaijiaju.cn

C#:   // 手写回溯递归
来源：http://ls.huixinmuqiang.cn

[N09] 栈与队列
来源：http://mm.shxzskj.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://pe.shxzukj.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://lx.colortex.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://jd.colortex.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mh.chemitech.net.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://kh.nicolike.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://cp.huixiangedu.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://gg.9csxet.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://jg.bjjhwx.cn

[N10] 链表节点定义
来源：http://xs.nicolike.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ww.9csxet.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://xi.huanxung.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://sz.shtwfgs.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://pk.wgjwhj.cn

Java: class Node { int v; Node next; }
来源：http://cy.colortex.cn

Go:   type Node struct { V int; Next *Node }
来源：http://kv.jctech888.com.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://hq.yuexingan06.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://qv.nszjky.cn

[N11] 二叉树中序遍历
来源：http://mc.wgjwhj.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://rz.nicolike.cn

PHP:  // 手写递归函数
来源：http://bx.shtwfgs.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://cf.shxzukj.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ie.jianghongdianzi.cn

Java: // 手写递归
来源：http://hs.hahajie.cn

Go:   // 手写递归
来源：http://so.huanxung.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://zk.521024.cn

C#:   // 手写递归
来源：http://qc.panjiajie.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://pn.newstarts.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://zr.jianghongdianzi.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://so.9csxet.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://gx.9csxet.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://jv.nszjky.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wh.bjjhwx.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ea.panjiajie.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://gi.haigaiapp.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://tn.hahajie.cn

================================================================================
来源：http://lp.521024.cn

O. 并发与异步
来源：http://aq.huixiangedu.cn

================================================================================
来源：http://rg.huixinmuqiang.cn

[O01] 启动一个线程
来源：http://zv.hahajie.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://be.nicolike.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://pg.newstarts.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://zt.nicolike.cn

TS:   // 同 JS
来源：http://ra.panjiajie.cn

Java: new Thread(() -> f()).start()
来源：http://uc.asd995.cn

Go:   go f()
来源：http://qu.yuntaijiaju.cn

Ruby: Thread.new { f }
来源：http://kc.jctech888.com.cn

C#:   Task.Run(() => F());
来源：http://ge.gzmigu.cn

[O02] 使用线程池
来源：http://qv.521024.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://jy.szsharing.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ui.chemitech.net.cn

JS:   // worker_threads 线程池
来源：http://cb.521024.cn

TS:   // worker_threads 线程池
来源：http://cr.nszjky.cn

Java: Executors.newFixedThreadPool(4)
来源：http://bx.shxzukj.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://qu.nszjky.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://fa.521024.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://cs.asd995.cn

[O03] 加锁保护共享数据
来源：http://xf.nicolike.cn

Py:   with lock: shared += 1
来源：http://ai.haigaiapp.cn

PHP:  // 用 flock() 做文件锁
来源：http://hl.521024.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://jm.jianghongdianzi.cn

TS:   // 同 JS
来源：http://pr.jianghongdianzi.cn

Java: synchronized (this) { shared++; }
来源：http://qw.shxzskj.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://eb.shxzskj.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://uq.muxihuayi.cn

C#:   lock (gate) { shared++; }
来源：http://cf.hnjuh.cn

[O04] 定义异步函数并等待
来源：http://xr.nszjky.cn

Py:   async def f():⏎    await g()
来源：http://xm.nszjky.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://nk.szsharing.cn

JS:   async function f() { await g(); }
来源：http://fl.shxzukj.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://wf.bjjhwx.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://fj.jianghongdianzi.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://tu.gzmigu.cn

Ruby: # 用 Fiber 或 async gem
来源：http://nh.jianghongdianzi.cn

C#:   async Task F() { await G(); }
来源：http://jz.jianghongdianzi.cn

[O05] 并发执行并等待全部完成
来源：http://tm.nicolike.cn

Py:   asyncio.gather(*tasks)
来源：http://ix.chemitech.net.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ua.haigaiapp.cn

JS:   await Promise.all(tasks)
来源：http://tm.lnxyls.cn

TS:   await Promise.all(tasks)
来源：http://aw.bjjhwx.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://qf.shxzskj.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://oi.haigaiapp.cn

Ruby: threads.map(&:join)
来源：http://xy.panjiajie.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://zy.huixinmuqiang.cn

[O06] 使用进程池
来源：http://gf.shxzskj.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ob.szxytkj.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://jw.shxzukj.cn

JS:   // child_process / cluster 模块
来源：http://qo.huixiangedu.cn

TS:   // child_process / cluster 模块
来源：http://ag.asd995.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://fq.muxihuayi.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://xf.nicolike.cn

Ruby: // fork 块
来源：http://nt.szxytkj.cn

C#:   Parallel.For
来源：http://px.newstarts.cn

================================================================================
来源：http://mk.colortex.cn

P. 常用工具函数
来源：http://bh.szxytkj.cn

================================================================================
来源：http://qz.shxzukj.cn

[P01] 生成 UUID
来源：http://mr.asd995.cn

Py:   str(uuid.uuid4())
来源：http://lz.szsharing.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://rv.chemitech.net.cn

JS:   crypto.randomUUID()
来源：http://js.shxzukj.cn

TS:   crypto.randomUUID()
来源：http://ln.hahajie.cn

Java: UUID.randomUUID().toString()
来源：http://ta.huixiangedu.cn

Go:   // 用 github.com/google/uuid
来源：http://aw.hnjuh.cn

Ruby: SecureRandom.uuid
来源：http://ec.shxzukj.cn

C#:   Guid.NewGuid().ToString()
来源：http://tc.asd995.cn

[P02] MD5 / SHA256 摘要
来源：http://qa.muxihuayi.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://te.chemitech.net.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://qt.lnxyls.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://cs.9csxet.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://pe.wgjwhj.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hr.huanxung.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://le.521024.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://yx.haigaiapp.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://oz.huixiangedu.cn

[P03] 生成短随机字符串
来源：http://yf.chemitech.net.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://nk.nszjky.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://by.bjjhwx.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://pu.521024.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://pj.yuntaijiaju.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://gm.huixiangedu.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://sj.huixiangedu.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://xb.nicolike.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wy.nicolike.cn

[P04] 求长度
来源：http://ea.shtwfgs.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ei.yuntaijiaju.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://bs.bookmarksfly.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://zs.newstarts.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://cb.gzmigu.cn

Java: list.size();  map.size();  s.length()
来源：http://ri.gzmigu.cn

Go:   len(arr);  len(m)
来源：http://tc.shxzskj.cn

Ruby: x.length;  x.size
来源：http://uw.shtwfgs.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://jq.jctech888.com.cn

[P05] 判断两个对象内容是否相等
来源：http://mk.bjjhwx.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://cy.colortex.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://gb.9csxet.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://bq.hahajie.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://xa.hahajie.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://qa.9csxet.cn

Go:   reflect.DeepEqual(a, b)
来源：http://il.9csxet.cn

Ruby: a == b
来源：http://bq.shxzukj.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://nw.nszjky.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://sq.yuntaijiaju.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://dy.haigaiapp.cn

PHP:  if (empty($x)) {}
来源：http://wm.panjiajie.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ut.chemitech.net.cn

TS:   if (x == null) {}
来源：http://uu.shxzukj.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://nn.huixinmuqiang.cn

Go:   if x == nil {}
来源：http://rh.bjjhwx.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://re.szxytkj.cn

C#:   if (x is null) {}
来源：http://co.bjjhwx.cn

[P07] 防抖与节流
来源：http://yf.asd995.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://zw.muxihuayi.cn

PHP:  // 手写时间戳比较
来源：http://mu.muxihuayi.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wp.shtwfgs.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://bg.hahajie.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://fx.chemitech.net.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://jh.yuntaijiaju.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://pb.yuntaijiaju.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://yz.shtwfgs.cn

[P08] 处理浮点精度问题
来源：http://mi.nszjky.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://qv.bookmarksfly.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://pk.yuexingan06.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://vh.szsharing.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mp.jctech888.com.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://xc.521024.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://zw.szsharing.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mu.jctech888.com.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://fx.yuexingan06.cn

================================================================================
来源：http://ne.jctech888.com.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ep.521024.cn

================================================================================
来源：http://uk.jctech888.com.cn

[Q01] 创建表
来源：http://dd.yuexingan06.cn

CREATE TABLE users (
来源：http://xk.521024.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://fp.huixiangedu.cn

name VARCHAR(50) NOT NULL,
来源：http://cj.lnxyls.cn

email VARCHAR(100) UNIQUE,
来源：http://sf.newstarts.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hs.shtwfgs.cn

);
来源：http://vv.shxzukj.cn

[Q02] 创建带外键的表
来源：http://jd.panjiajie.cn

CREATE TABLE orders (
来源：http://vz.bookmarksfly.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ue.chemitech.net.cn

user_id INT NOT NULL,
来源：http://lu.lnxyls.cn

amount DECIMAL(10, 2),
来源：http://vw.shxzukj.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ax.jctech888.com.cn

);
来源：http://iu.gzmigu.cn

[Q03] 增加列
来源：http://wl.shtwfgs.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ho.szsharing.cn

[Q04] 修改列类型
来源：http://bj.yuntaijiaju.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://xa.asd995.cn

[Q05] 重命名列
来源：http://hn.yuntaijiaju.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://sr.yuexingan06.cn

[Q06] 删除列
来源：http://fq.shxzskj.cn

ALTER TABLE users DROP COLUMN age;
来源：http://ff.szsharing.cn

[Q07] 删除表
来源：http://ev.wgjwhj.cn

DROP TABLE IF EXISTS orders;
来源：http://tg.muxihuayi.cn

[Q08] 创建普通索引
来源：http://zh.bookmarksfly.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://cv.huanxung.cn

[Q09] 创建唯一索引
来源：http://bp.newstarts.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://xe.jctech888.com.cn

[Q10] 插入单行
来源：http://ft.huanxung.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://iw.chemitech.net.cn

[Q11] 一次插入多行
来源：http://wh.hahajie.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wl.shxzskj.cn

[Q12] 插入后取自增 ID
来源：http://vk.shxzukj.cn

INSERT INTO users (name) VALUES ('C');
来源：http://qq.hnjuh.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://sv.nszjky.cn

[Q13] 忽略重复插入
来源：http://dj.yuntaijiaju.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ge.shxzskj.cn

[Q14] 存在则更新（upsert）
来源：http://el.jctech888.com.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://vv.wgjwhj.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://jh.shxzskj.cn

[Q15] 查询全部
来源：http://kb.yuexingan06.cn

SELECT * FROM users;
来源：http://vj.haigaiapp.cn

[Q16] 查询指定列
来源：http://ce.szsharing.cn

SELECT id, name FROM users;
来源：http://cc.hnjuh.cn

[Q17] 条件查询
来源：http://wx.colortex.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ow.yuexingan06.cn

[Q18] 模糊匹配
来源：http://ss.shtwfgs.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://pc.wgjwhj.cn

[Q19] 范围查询
来源：http://xa.huanxung.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ye.shxzskj.cn

[Q20] IN 列表
来源：http://dl.521024.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://fl.huixiangedu.cn

[Q21] 空值判断
来源：http://rk.shxzukj.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://we.bjjhwx.cn

[Q22] 排序
来源：http://ss.bjjhwx.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ab.szxytkj.cn

[Q23] 分页
来源：http://at.jianghongdianzi.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://xu.gzmigu.cn

[Q24] 去重
来源：http://nl.muxihuayi.cn

SELECT DISTINCT city FROM users;
来源：http://lp.szsharing.cn

[Q25] 只取前 N 条
来源：http://ts.huixiangedu.cn


<!-- 参考信息 -->