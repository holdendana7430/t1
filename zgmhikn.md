代发 wailian999

JS:   [...arr].sort((a, b) => a - b)
来源：http://qr.9csxet.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://pz.haigaiapp.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://fy.jctech888.com.cn

Go:   slices.Sort(arr)
来源：http://az.muxihuayi.cn

Ruby: arr.sort
来源：http://xp.gzmigu.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://od.szsharing.cn

[N03] 快速排序（分治示例）
来源：http://dg.huixinmuqiang.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://cd.wgjwhj.cn

PHP:  // 递归实现，或用 usort
来源：http://zt.jctech888.com.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ek.huixinmuqiang.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://vn.jctech888.com.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://fg.yuexingan06.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ol.bookmarksfly.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ux.jianghongdianzi.cn

C#:   // 手写递归，或 Array.Sort
来源：http://sk.huixinmuqiang.cn

[N04] 斐波那契数列
来源：http://bj.521024.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://yz.colortex.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://gl.shtwfgs.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://qy.huanxung.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://eq.jianghongdianzi.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://jf.lnxyls.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ux.huanxung.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ae.shtwfgs.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hr.521024.cn

[N05] 最大公约数
来源：http://sp.asd995.cn

Py:   math.gcd(a, b)
来源：http://xh.shxzukj.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://dm.gzmigu.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://kz.lnxyls.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://pn.szsharing.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://by.jctech888.com.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ed.asd995.cn

Ruby: a.gcd(b)
来源：http://kv.shtwfgs.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wz.asd995.cn

[N06] 判断回文字符串
来源：http://xx.bookmarksfly.cn

Py:   s == s[::-1]
来源：http://io.colortex.cn

PHP:  $s === strrev($s);
来源：http://hi.muxihuayi.cn

JS:   s === [...s].reverse().join("")
来源：http://sg.9csxet.cn

TS:   s === [...s].reverse().join("")
来源：http://nj.newstarts.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ym.shtwfgs.cn

Go:   // 双指针从两端比较
来源：http://tk.yuntaijiaju.cn

Ruby: s == s.reverse
来源：http://kw.shxzukj.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://rs.nicolike.cn

[N07] 两数之和（返回下标）
来源：http://sx.szxytkj.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://sx.wgjwhj.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://lr.jianghongdianzi.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://qm.shtwfgs.cn

TS:   // 手写 Map<string, number>
来源：http://aq.szsharing.cn

Java: // 手写 HashMap
来源：http://or.huixiangedu.cn

Go:   // 手写 map[int]int
来源：http://gw.szxytkj.cn

Ruby: // 手写 Hash
来源：http://hc.9csxet.cn

C#:   // 手写 Dictionary<int, int>
来源：http://jb.huanxung.cn

[N08] 生成全排列
来源：http://da.bjjhwx.cn

Py:   itertools.permutations(arr)
来源：http://pd.muxihuayi.cn

PHP:  // 手写递归交换
来源：http://cc.haigaiapp.cn

JS:   // 手写回溯递归
来源：http://jl.nszjky.cn

TS:   // 手写回溯递归
来源：http://xj.panjiajie.cn

Java: // 手写回溯递归
来源：http://fv.shtwfgs.cn

Go:   // 手写回溯递归
来源：http://mt.szxytkj.cn

Ruby: arr.permutation.to_a
来源：http://qb.hnjuh.cn

C#:   // 手写回溯递归
来源：http://yy.huixiangedu.cn

[N09] 栈与队列
来源：http://tx.bjjhwx.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hg.huanxung.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://lb.panjiajie.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://nf.huixiangedu.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://zq.panjiajie.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://az.panjiajie.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ez.bookmarksfly.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://cm.nicolike.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ts.bookmarksfly.cn

[N10] 链表节点定义
来源：http://rt.hnjuh.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://yx.shtwfgs.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://mq.szsharing.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://eo.jianghongdianzi.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://qa.shxzskj.cn

Java: class Node { int v; Node next; }
来源：http://vc.gzmigu.cn

Go:   type Node struct { V int; Next *Node }
来源：http://qy.gzmigu.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://ao.hahajie.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://nk.jianghongdianzi.cn

[N11] 二叉树中序遍历
来源：http://jj.panjiajie.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ma.jianghongdianzi.cn

PHP:  // 手写递归函数
来源：http://tq.nszjky.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wy.gzmigu.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://tg.muxihuayi.cn

Java: // 手写递归
来源：http://zg.panjiajie.cn

Go:   // 手写递归
来源：http://qn.haigaiapp.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://cx.hnjuh.cn

C#:   // 手写递归
来源：http://xy.haigaiapp.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wk.9csxet.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://yy.nszjky.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://oq.colortex.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hd.bookmarksfly.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://uw.521024.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://it.shxzskj.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://fe.yuntaijiaju.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://pu.521024.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://nn.wgjwhj.cn

================================================================================
来源：http://qh.521024.cn

O. 并发与异步
来源：http://fb.muxihuayi.cn

================================================================================
来源：http://fo.panjiajie.cn

[O01] 启动一个线程
来源：http://jl.jianghongdianzi.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://fj.521024.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://rh.newstarts.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://tz.yuexingan06.cn

TS:   // 同 JS
来源：http://eh.asd995.cn

Java: new Thread(() -> f()).start()
来源：http://nt.haigaiapp.cn

Go:   go f()
来源：http://tw.521024.cn

Ruby: Thread.new { f }
来源：http://xj.szxytkj.cn

C#:   Task.Run(() => F());
来源：http://jy.jianghongdianzi.cn

[O02] 使用线程池
来源：http://fv.szsharing.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://oo.jianghongdianzi.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://fy.jianghongdianzi.cn

JS:   // worker_threads 线程池
来源：http://qw.wgjwhj.cn

TS:   // worker_threads 线程池
来源：http://vg.huixiangedu.cn

Java: Executors.newFixedThreadPool(4)
来源：http://jl.9csxet.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://tt.hahajie.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ls.nszjky.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://xv.szxytkj.cn

[O03] 加锁保护共享数据
来源：http://zg.szxytkj.cn

Py:   with lock: shared += 1
来源：http://zl.9csxet.cn

PHP:  // 用 flock() 做文件锁
来源：http://rg.muxihuayi.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://rr.hahajie.cn

TS:   // 同 JS
来源：http://sd.lnxyls.cn

Java: synchronized (this) { shared++; }
来源：http://lq.huixinmuqiang.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://zv.yuntaijiaju.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://kt.yuexingan06.cn

C#:   lock (gate) { shared++; }
来源：http://ru.yuexingan06.cn

[O04] 定义异步函数并等待
来源：http://ul.yuexingan06.cn

Py:   async def f():⏎    await g()
来源：http://kc.bjjhwx.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://nf.huanxung.cn

JS:   async function f() { await g(); }
来源：http://mn.chemitech.net.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://kv.shtwfgs.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://aj.colortex.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://nh.asd995.cn

Ruby: # 用 Fiber 或 async gem
来源：http://bg.panjiajie.cn

C#:   async Task F() { await G(); }
来源：http://ur.colortex.cn

[O05] 并发执行并等待全部完成
来源：http://wd.9csxet.cn

Py:   asyncio.gather(*tasks)
来源：http://cd.chemitech.net.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://qr.huixiangedu.cn

JS:   await Promise.all(tasks)
来源：http://ub.bookmarksfly.cn

TS:   await Promise.all(tasks)
来源：http://yy.colortex.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ph.hnjuh.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wj.wgjwhj.cn

Ruby: threads.map(&:join)
来源：http://gn.colortex.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://ti.huanxung.cn

[O06] 使用进程池
来源：http://ft.haigaiapp.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://kp.colortex.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://ud.nszjky.cn

JS:   // child_process / cluster 模块
来源：http://zx.chemitech.net.cn

TS:   // child_process / cluster 模块
来源：http://ay.huixinmuqiang.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://uw.jianghongdianzi.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://sh.asd995.cn

Ruby: // fork 块
来源：http://zu.huanxung.cn

C#:   Parallel.For
来源：http://tz.bjjhwx.cn

================================================================================
来源：http://aj.shxzukj.cn

P. 常用工具函数
来源：http://mq.muxihuayi.cn

================================================================================
来源：http://gc.yuntaijiaju.cn

[P01] 生成 UUID
来源：http://ln.chemitech.net.cn

Py:   str(uuid.uuid4())
来源：http://kq.hnjuh.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://dx.lnxyls.cn

JS:   crypto.randomUUID()
来源：http://dj.jianghongdianzi.cn

TS:   crypto.randomUUID()
来源：http://zg.yuntaijiaju.cn

Java: UUID.randomUUID().toString()
来源：http://ly.panjiajie.cn

Go:   // 用 github.com/google/uuid
来源：http://yc.gzmigu.cn

Ruby: SecureRandom.uuid
来源：http://sb.jianghongdianzi.cn

C#:   Guid.NewGuid().ToString()
来源：http://bk.shtwfgs.cn

[P02] MD5 / SHA256 摘要
来源：http://lx.huixiangedu.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://oy.nicolike.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://gu.panjiajie.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://dx.nicolike.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://he.jctech888.com.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://es.szxytkj.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mf.jianghongdianzi.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://yd.gzmigu.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hi.jianghongdianzi.cn

[P03] 生成短随机字符串
来源：http://ph.bjjhwx.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://tk.gzmigu.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wk.huixiangedu.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://nk.bjjhwx.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ea.haigaiapp.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://vf.yuntaijiaju.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ul.nszjky.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://lb.hnjuh.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://uu.521024.cn

[P04] 求长度
来源：http://or.wgjwhj.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://zc.bjjhwx.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://jv.hnjuh.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://vz.shxzukj.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://fx.521024.cn

Java: list.size();  map.size();  s.length()
来源：http://uf.huanxung.cn

Go:   len(arr);  len(m)
来源：http://ab.yuntaijiaju.cn

Ruby: x.length;  x.size
来源：http://fl.colortex.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://uh.bookmarksfly.cn

[P05] 判断两个对象内容是否相等
来源：http://ye.hahajie.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://kh.hnjuh.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://bd.jctech888.com.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://np.nicolike.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://al.yuexingan06.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://fp.gzmigu.cn

Go:   reflect.DeepEqual(a, b)
来源：http://cl.jianghongdianzi.cn

Ruby: a == b
来源：http://ca.haigaiapp.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://lk.521024.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://bb.nszjky.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://uu.wgjwhj.cn

PHP:  if (empty($x)) {}
来源：http://hm.jianghongdianzi.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://me.muxihuayi.cn

TS:   if (x == null) {}
来源：http://vp.asd995.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://it.jianghongdianzi.cn

Go:   if x == nil {}
来源：http://au.muxihuayi.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://uc.gzmigu.cn

C#:   if (x is null) {}
来源：http://dn.panjiajie.cn

[P07] 防抖与节流
来源：http://kv.huixinmuqiang.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://qh.shtwfgs.cn

PHP:  // 手写时间戳比较
来源：http://ew.521024.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ml.gzmigu.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mc.bjjhwx.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://rh.huanxung.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://lc.9csxet.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://as.jianghongdianzi.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://og.hahajie.cn

[P08] 处理浮点精度问题
来源：http://xc.521024.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://lb.yuntaijiaju.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://vx.shtwfgs.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://bj.521024.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://pu.nszjky.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://nr.huixiangedu.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://iq.panjiajie.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mq.9csxet.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ep.jianghongdianzi.cn

================================================================================
来源：http://ut.panjiajie.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://jr.hnjuh.cn

================================================================================
来源：http://eu.asd995.cn

[Q01] 创建表
来源：http://st.hnjuh.cn

CREATE TABLE users (
来源：http://nf.shxzukj.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://px.newstarts.cn

name VARCHAR(50) NOT NULL,
来源：http://ro.shtwfgs.cn

email VARCHAR(100) UNIQUE,
来源：http://ws.shxzskj.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ca.hnjuh.cn

);
来源：http://eh.nszjky.cn

[Q02] 创建带外键的表
来源：http://du.jianghongdianzi.cn

CREATE TABLE orders (
来源：http://qq.lnxyls.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://zg.huixiangedu.cn

user_id INT NOT NULL,
来源：http://gn.szxytkj.cn

amount DECIMAL(10, 2),
来源：http://gh.9csxet.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://zz.gzmigu.cn

);
来源：http://sh.yuexingan06.cn

[Q03] 增加列
来源：http://og.asd995.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://js.jctech888.com.cn

[Q04] 修改列类型
来源：http://bi.9csxet.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mf.colortex.cn

[Q05] 重命名列
来源：http://ow.bjjhwx.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ee.muxihuayi.cn

[Q06] 删除列
来源：http://nx.panjiajie.cn

ALTER TABLE users DROP COLUMN age;
来源：http://wg.wgjwhj.cn

[Q07] 删除表
来源：http://yp.bookmarksfly.cn

DROP TABLE IF EXISTS orders;
来源：http://na.bjjhwx.cn

[Q08] 创建普通索引
来源：http://rp.bookmarksfly.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://xr.gzmigu.cn

[Q09] 创建唯一索引
来源：http://is.bookmarksfly.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://we.bjjhwx.cn

[Q10] 插入单行
来源：http://ah.521024.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://su.huixiangedu.cn

[Q11] 一次插入多行
来源：http://kb.chemitech.net.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://aq.huixiangedu.cn

[Q12] 插入后取自增 ID
来源：http://xl.521024.cn

INSERT INTO users (name) VALUES ('C');
来源：http://uh.9csxet.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://uj.jctech888.com.cn

[Q13] 忽略重复插入
来源：http://pq.panjiajie.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://um.hnjuh.cn

[Q14] 存在则更新（upsert）
来源：http://qv.yuexingan06.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://fs.yuntaijiaju.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://nb.huanxung.cn

[Q15] 查询全部
来源：http://xw.521024.cn

SELECT * FROM users;
来源：http://pz.hahajie.cn

[Q16] 查询指定列
来源：http://yg.jianghongdianzi.cn

SELECT id, name FROM users;
来源：http://kw.nicolike.cn

[Q17] 条件查询
来源：http://st.colortex.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ew.shxzukj.cn

[Q18] 模糊匹配
来源：http://fg.shtwfgs.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ax.gzmigu.cn

[Q19] 范围查询
来源：http://tn.gzmigu.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ge.haigaiapp.cn

[Q20] IN 列表
来源：http://zb.huixiangedu.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://yp.shtwfgs.cn

[Q21] 空值判断
来源：http://ph.hahajie.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://ou.bookmarksfly.cn

[Q22] 排序
来源：http://vk.shtwfgs.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://yj.shxzukj.cn

[Q23] 分页
来源：http://qr.jianghongdianzi.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://rp.huixinmuqiang.cn

[Q24] 去重
来源：http://sv.521024.cn

SELECT DISTINCT city FROM users;
来源：http://ea.panjiajie.cn

[Q25] 只取前 N 条
来源：http://lc.hahajie.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://gc.szsharing.cn

[Q26] 计数
来源：http://uj.huanxung.cn

SELECT COUNT(*) FROM users;
来源：http://dh.szxytkj.cn

[Q27] 条件计数
来源：http://fm.jctech888.com.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ow.huanxung.cn

[Q28] 求和与平均
来源：http://op.asd995.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://uq.wgjwhj.cn

[Q29] 最大最小值
来源：http://dj.nicolike.cn


<!-- 参考信息 -->