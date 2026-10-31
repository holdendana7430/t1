代发 wailian999

C#:   Array.BinarySearch(arr, x)
来源：http://fv.szsharing.cn

[N02] 排序（工程实践用内置实现）
来源：http://lq.hnjuh.cn

Py:   sorted(arr);  arr.sort()
来源：http://cd.panjiajie.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://xy.huanxung.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://yw.huanxung.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://ul.newstarts.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://rb.lnxyls.cn

Go:   slices.Sort(arr)
来源：http://pn.huixiangedu.cn

Ruby: arr.sort
来源：http://sa.jctech888.com.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://oz.hahajie.cn

[N03] 快速排序（分治示例）
来源：http://ou.hahajie.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://qb.nszjky.cn

PHP:  // 递归实现，或用 usort
来源：http://yj.yuntaijiaju.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://lo.chemitech.net.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://tc.jctech888.com.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://bh.hnjuh.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://av.asd995.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://fp.szxytkj.cn

C#:   // 手写递归，或 Array.Sort
来源：http://ky.shtwfgs.cn

[N04] 斐波那契数列
来源：http://kt.jianghongdianzi.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ck.panjiajie.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ic.gzmigu.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://xe.colortex.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://pl.hnjuh.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://uo.hnjuh.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://jr.shxzskj.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://zy.haigaiapp.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://rh.huixinmuqiang.cn

[N05] 最大公约数
来源：http://sb.huixiangedu.cn

Py:   math.gcd(a, b)
来源：http://ez.shxzukj.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ko.huanxung.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://kt.yuexingan06.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://bm.gzmigu.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ky.szsharing.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ld.huanxung.cn

Ruby: a.gcd(b)
来源：http://lq.asd995.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://vm.bjjhwx.cn

[N06] 判断回文字符串
来源：http://gm.newstarts.cn

Py:   s == s[::-1]
来源：http://hh.9csxet.cn

PHP:  $s === strrev($s);
来源：http://su.nszjky.cn

JS:   s === [...s].reverse().join("")
来源：http://cq.shxzskj.cn

TS:   s === [...s].reverse().join("")
来源：http://gy.szsharing.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://da.hnjuh.cn

Go:   // 双指针从两端比较
来源：http://mu.jianghongdianzi.cn

Ruby: s == s.reverse
来源：http://ma.wgjwhj.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://jk.szxytkj.cn

[N07] 两数之和（返回下标）
来源：http://co.huanxung.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://rg.jctech888.com.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wp.huixinmuqiang.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://jn.haigaiapp.cn

TS:   // 手写 Map<string, number>
来源：http://nd.huixinmuqiang.cn

Java: // 手写 HashMap
来源：http://qv.shxzskj.cn

Go:   // 手写 map[int]int
来源：http://lj.lnxyls.cn

Ruby: // 手写 Hash
来源：http://mm.shxzukj.cn

C#:   // 手写 Dictionary<int, int>
来源：http://xy.newstarts.cn

[N08] 生成全排列
来源：http://hq.chemitech.net.cn

Py:   itertools.permutations(arr)
来源：http://do.hnjuh.cn

PHP:  // 手写递归交换
来源：http://hx.muxihuayi.cn

JS:   // 手写回溯递归
来源：http://so.wgjwhj.cn

TS:   // 手写回溯递归
来源：http://yu.szsharing.cn

Java: // 手写回溯递归
来源：http://ii.yuntaijiaju.cn

Go:   // 手写回溯递归
来源：http://fg.jctech888.com.cn

Ruby: arr.permutation.to_a
来源：http://sc.gzmigu.cn

C#:   // 手写回溯递归
来源：http://th.9csxet.cn

[N09] 栈与队列
来源：http://mj.colortex.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://pl.yuexingan06.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://vb.521024.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ha.bookmarksfly.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://df.nszjky.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://en.colortex.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://lq.shtwfgs.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://kp.bookmarksfly.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://il.hnjuh.cn

[N10] 链表节点定义
来源：http://ub.colortex.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://pr.lnxyls.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://pl.szxytkj.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://lu.huanxung.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://sf.shxzskj.cn

Java: class Node { int v; Node next; }
来源：http://hc.huixinmuqiang.cn

Go:   type Node struct { V int; Next *Node }
来源：http://uv.bookmarksfly.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://wo.521024.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://ni.hnjuh.cn

[N11] 二叉树中序遍历
来源：http://re.wgjwhj.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://lf.huixiangedu.cn

PHP:  // 手写递归函数
来源：http://xp.shxzukj.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://rf.yuexingan06.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://zs.9csxet.cn

Java: // 手写递归
来源：http://xn.lnxyls.cn

Go:   // 手写递归
来源：http://jo.hnjuh.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://tj.muxihuayi.cn

C#:   // 手写递归
来源：http://gp.hahajie.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://uf.chemitech.net.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://oi.bookmarksfly.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://db.9csxet.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://qc.wgjwhj.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://dh.newstarts.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://of.muxihuayi.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://cc.huixinmuqiang.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ji.9csxet.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://rd.shtwfgs.cn

================================================================================
来源：http://wd.muxihuayi.cn

O. 并发与异步
来源：http://ai.szxytkj.cn

================================================================================
来源：http://hz.jianghongdianzi.cn

[O01] 启动一个线程
来源：http://bd.colortex.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://qf.panjiajie.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://bj.newstarts.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://bn.gzmigu.cn

TS:   // 同 JS
来源：http://wy.jctech888.com.cn

Java: new Thread(() -> f()).start()
来源：http://ak.szsharing.cn

Go:   go f()
来源：http://lt.hahajie.cn

Ruby: Thread.new { f }
来源：http://tj.nicolike.cn

C#:   Task.Run(() => F());
来源：http://fl.szsharing.cn

[O02] 使用线程池
来源：http://fo.nicolike.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ar.wgjwhj.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ov.yuntaijiaju.cn

JS:   // worker_threads 线程池
来源：http://mk.nszjky.cn

TS:   // worker_threads 线程池
来源：http://nc.szsharing.cn

Java: Executors.newFixedThreadPool(4)
来源：http://mu.jianghongdianzi.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ir.haigaiapp.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://vp.shxzskj.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://kg.hnjuh.cn

[O03] 加锁保护共享数据
来源：http://cd.521024.cn

Py:   with lock: shared += 1
来源：http://zc.panjiajie.cn

PHP:  // 用 flock() 做文件锁
来源：http://gs.haigaiapp.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://gv.521024.cn

TS:   // 同 JS
来源：http://ke.bjjhwx.cn

Java: synchronized (this) { shared++; }
来源：http://lk.nicolike.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://xh.chemitech.net.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://kg.bjjhwx.cn

C#:   lock (gate) { shared++; }
来源：http://aw.wgjwhj.cn

[O04] 定义异步函数并等待
来源：http://dp.haigaiapp.cn

Py:   async def f():⏎    await g()
来源：http://tb.colortex.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://nd.bookmarksfly.cn

JS:   async function f() { await g(); }
来源：http://ja.hnjuh.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://rd.9csxet.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://od.bookmarksfly.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://tk.yuexingan06.cn

Ruby: # 用 Fiber 或 async gem
来源：http://we.lnxyls.cn

C#:   async Task F() { await G(); }
来源：http://xv.muxihuayi.cn

[O05] 并发执行并等待全部完成
来源：http://qx.nszjky.cn

Py:   asyncio.gather(*tasks)
来源：http://qa.shxzukj.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://dh.colortex.cn

JS:   await Promise.all(tasks)
来源：http://qw.hahajie.cn

TS:   await Promise.all(tasks)
来源：http://hh.hnjuh.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://sq.lnxyls.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://rr.szxytkj.cn

Ruby: threads.map(&:join)
来源：http://dk.huixinmuqiang.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://yc.hnjuh.cn

[O06] 使用进程池
来源：http://wh.wgjwhj.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://gd.521024.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://av.bjjhwx.cn

JS:   // child_process / cluster 模块
来源：http://dy.newstarts.cn

TS:   // child_process / cluster 模块
来源：http://pk.muxihuayi.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://fh.lnxyls.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://eh.szxytkj.cn

Ruby: // fork 块
来源：http://ci.9csxet.cn

C#:   Parallel.For
来源：http://nv.muxihuayi.cn

================================================================================
来源：http://ke.yuexingan06.cn

P. 常用工具函数
来源：http://iz.jctech888.com.cn

================================================================================
来源：http://xp.lnxyls.cn

[P01] 生成 UUID
来源：http://qz.shxzukj.cn

Py:   str(uuid.uuid4())
来源：http://uk.asd995.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://da.huixiangedu.cn

JS:   crypto.randomUUID()
来源：http://dy.521024.cn

TS:   crypto.randomUUID()
来源：http://wl.bjjhwx.cn

Java: UUID.randomUUID().toString()
来源：http://rb.colortex.cn

Go:   // 用 github.com/google/uuid
来源：http://uy.haigaiapp.cn

Ruby: SecureRandom.uuid
来源：http://kk.szsharing.cn

C#:   Guid.NewGuid().ToString()
来源：http://md.jctech888.com.cn

[P02] MD5 / SHA256 摘要
来源：http://xu.haigaiapp.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://vn.szsharing.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://ou.chemitech.net.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://yn.shxzukj.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wy.huixiangedu.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://pq.521024.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://jp.shtwfgs.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://rz.huixinmuqiang.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://sf.huixiangedu.cn

[P03] 生成短随机字符串
来源：http://bg.yuexingan06.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://gt.lnxyls.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://uy.colortex.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://tn.lnxyls.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://st.huixiangedu.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ft.9csxet.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://yg.newstarts.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://mt.gzmigu.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://uu.shxzskj.cn

[P04] 求长度
来源：http://rp.yuexingan06.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://dx.shxzskj.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://zz.nszjky.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://da.szxytkj.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://lh.bookmarksfly.cn

Java: list.size();  map.size();  s.length()
来源：http://cx.shxzskj.cn

Go:   len(arr);  len(m)
来源：http://mp.9csxet.cn

Ruby: x.length;  x.size
来源：http://bd.hahajie.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://qy.huanxung.cn

[P05] 判断两个对象内容是否相等
来源：http://nb.nicolike.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://sn.huanxung.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wj.newstarts.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://vm.bjjhwx.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://bt.shxzukj.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wu.hnjuh.cn

Go:   reflect.DeepEqual(a, b)
来源：http://ha.panjiajie.cn

Ruby: a == b
来源：http://he.szxytkj.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://pg.shtwfgs.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://cz.yuntaijiaju.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://or.asd995.cn

PHP:  if (empty($x)) {}
来源：http://rs.hahajie.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://zy.yuntaijiaju.cn

TS:   if (x == null) {}
来源：http://oz.lnxyls.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://fv.gzmigu.cn

Go:   if x == nil {}
来源：http://aq.hahajie.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://tf.panjiajie.cn

C#:   if (x is null) {}
来源：http://wl.huixiangedu.cn

[P07] 防抖与节流
来源：http://zr.gzmigu.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://dp.shxzukj.cn

PHP:  // 手写时间戳比较
来源：http://yf.shxzskj.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://px.yuexingan06.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://to.colortex.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://yy.gzmigu.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://sa.nicolike.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://lx.huanxung.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wz.jianghongdianzi.cn

[P08] 处理浮点精度问题
来源：http://rj.newstarts.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ij.jctech888.com.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://zl.huixinmuqiang.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://cq.nszjky.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://aw.shtwfgs.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ao.haigaiapp.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://qp.hnjuh.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ht.panjiajie.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://zl.lnxyls.cn

================================================================================
来源：http://vw.wgjwhj.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ox.szxytkj.cn

================================================================================
来源：http://if.bookmarksfly.cn

[Q01] 创建表
来源：http://gq.muxihuayi.cn

CREATE TABLE users (
来源：http://xm.panjiajie.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ro.bookmarksfly.cn

name VARCHAR(50) NOT NULL,
来源：http://eu.hahajie.cn

email VARCHAR(100) UNIQUE,
来源：http://gs.hnjuh.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ph.bookmarksfly.cn

);
来源：http://bo.bjjhwx.cn

[Q02] 创建带外键的表
来源：http://dc.szsharing.cn

CREATE TABLE orders (
来源：http://mc.521024.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://aw.shtwfgs.cn

user_id INT NOT NULL,
来源：http://qh.yuntaijiaju.cn

amount DECIMAL(10, 2),
来源：http://lx.521024.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://rm.bookmarksfly.cn

);
来源：http://wp.shxzskj.cn

[Q03] 增加列
来源：http://rw.newstarts.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://nw.shtwfgs.cn

[Q04] 修改列类型
来源：http://lf.asd995.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://fv.shtwfgs.cn

[Q05] 重命名列
来源：http://ym.hahajie.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://nz.nszjky.cn

[Q06] 删除列
来源：http://yy.szsharing.cn

ALTER TABLE users DROP COLUMN age;
来源：http://mi.newstarts.cn

[Q07] 删除表
来源：http://zn.panjiajie.cn

DROP TABLE IF EXISTS orders;
来源：http://jd.jctech888.com.cn

[Q08] 创建普通索引
来源：http://co.bjjhwx.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://qa.colortex.cn

[Q09] 创建唯一索引
来源：http://qk.bookmarksfly.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ec.szxytkj.cn

[Q10] 插入单行
来源：http://mg.szsharing.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://jc.colortex.cn

[Q11] 一次插入多行
来源：http://se.521024.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://iq.chemitech.net.cn

[Q12] 插入后取自增 ID
来源：http://wd.colortex.cn

INSERT INTO users (name) VALUES ('C');
来源：http://ah.huixiangedu.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ie.jctech888.com.cn

[Q13] 忽略重复插入
来源：http://jr.shxzukj.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://pc.nicolike.cn

[Q14] 存在则更新（upsert）
来源：http://ei.huixinmuqiang.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ae.shxzskj.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://iy.szxytkj.cn

[Q15] 查询全部
来源：http://qb.haigaiapp.cn

SELECT * FROM users;
来源：http://he.lnxyls.cn

[Q16] 查询指定列
来源：http://ah.nszjky.cn

SELECT id, name FROM users;
来源：http://pp.shtwfgs.cn

[Q17] 条件查询
来源：http://np.panjiajie.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://gk.asd995.cn

[Q18] 模糊匹配
来源：http://ls.newstarts.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ak.yuntaijiaju.cn

[Q19] 范围查询
来源：http://ih.haigaiapp.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://cb.huixinmuqiang.cn

[Q20] IN 列表
来源：http://ys.szxytkj.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://al.shxzukj.cn

[Q21] 空值判断
来源：http://qg.colortex.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://is.hahajie.cn

[Q22] 排序
来源：http://sn.panjiajie.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://eg.wgjwhj.cn

[Q23] 分页
来源：http://mo.huanxung.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://kp.szsharing.cn

[Q24] 去重
来源：http://oe.colortex.cn

SELECT DISTINCT city FROM users;
来源：http://dv.huanxung.cn

[Q25] 只取前 N 条
来源：http://vi.hnjuh.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://er.521024.cn

[Q26] 计数
来源：http://ud.muxihuayi.cn

SELECT COUNT(*) FROM users;
来源：http://zw.shtwfgs.cn

[Q27] 条件计数
来源：http://ow.bjjhwx.cn


<!-- 参考信息 -->