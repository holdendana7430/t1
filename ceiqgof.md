代发 wailian999

JS:   [...arr].sort((a, b) => a - b)
来源：http://cg.muxihuayi.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://ui.muxihuayi.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://yp.jctech888.com.cn

Go:   slices.Sort(arr)
来源：http://fa.shxzskj.cn

Ruby: arr.sort
来源：http://ln.nszjky.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://af.hahajie.cn

[N03] 快速排序（分治示例）
来源：http://mj.huanxung.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://lu.panjiajie.cn

PHP:  // 递归实现，或用 usort
来源：http://em.asd995.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://rf.jctech888.com.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://vi.hahajie.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://cn.bjjhwx.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://pt.yuntaijiaju.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ab.hnjuh.cn

C#:   // 手写递归，或 Array.Sort
来源：http://sp.hnjuh.cn

[N04] 斐波那契数列
来源：http://jn.huanxung.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://yg.lnxyls.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://fb.jianghongdianzi.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://sj.bjjhwx.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://xb.gzmigu.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://dn.hahajie.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://qm.bjjhwx.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://jx.huixinmuqiang.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://dc.muxihuayi.cn

[N05] 最大公约数
来源：http://cy.huixinmuqiang.cn

Py:   math.gcd(a, b)
来源：http://rv.szxytkj.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://dw.szxytkj.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://dq.chemitech.net.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://vr.yuntaijiaju.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://cp.wgjwhj.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://nl.bookmarksfly.cn

Ruby: a.gcd(b)
来源：http://yy.gzmigu.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://fd.shxzukj.cn

[N06] 判断回文字符串
来源：http://ey.shxzskj.cn

Py:   s == s[::-1]
来源：http://wd.szsharing.cn

PHP:  $s === strrev($s);
来源：http://uj.chemitech.net.cn

JS:   s === [...s].reverse().join("")
来源：http://dx.bookmarksfly.cn

TS:   s === [...s].reverse().join("")
来源：http://hj.newstarts.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mz.shtwfgs.cn

Go:   // 双指针从两端比较
来源：http://bu.hahajie.cn

Ruby: s == s.reverse
来源：http://wy.nszjky.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://gq.nszjky.cn

[N07] 两数之和（返回下标）
来源：http://ri.asd995.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://nj.shxzskj.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ec.panjiajie.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://gy.wgjwhj.cn

TS:   // 手写 Map<string, number>
来源：http://jd.bookmarksfly.cn

Java: // 手写 HashMap
来源：http://rv.yuntaijiaju.cn

Go:   // 手写 map[int]int
来源：http://gi.panjiajie.cn

Ruby: // 手写 Hash
来源：http://ti.panjiajie.cn

C#:   // 手写 Dictionary<int, int>
来源：http://dn.huixiangedu.cn

[N08] 生成全排列
来源：http://wm.hnjuh.cn

Py:   itertools.permutations(arr)
来源：http://bf.shtwfgs.cn

PHP:  // 手写递归交换
来源：http://pg.lnxyls.cn

JS:   // 手写回溯递归
来源：http://mr.shxzukj.cn

TS:   // 手写回溯递归
来源：http://uc.shxzukj.cn

Java: // 手写回溯递归
来源：http://ew.lnxyls.cn

Go:   // 手写回溯递归
来源：http://oz.huixiangedu.cn

Ruby: arr.permutation.to_a
来源：http://kw.haigaiapp.cn

C#:   // 手写回溯递归
来源：http://rm.chemitech.net.cn

[N09] 栈与队列
来源：http://xn.9csxet.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wu.newstarts.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://oj.huanxung.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mu.bjjhwx.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ew.huixinmuqiang.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://pi.chemitech.net.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://gt.shtwfgs.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ca.shxzskj.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://fj.jianghongdianzi.cn

[N10] 链表节点定义
来源：http://uv.asd995.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ep.jctech888.com.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://yt.bookmarksfly.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://fm.haigaiapp.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://qn.panjiajie.cn

Java: class Node { int v; Node next; }
来源：http://jl.muxihuayi.cn

Go:   type Node struct { V int; Next *Node }
来源：http://xz.haigaiapp.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://hd.hahajie.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://ji.newstarts.cn

[N11] 二叉树中序遍历
来源：http://lo.muxihuayi.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://gn.hahajie.cn

PHP:  // 手写递归函数
来源：http://uy.jctech888.com.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ez.nszjky.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://pe.shtwfgs.cn

Java: // 手写递归
来源：http://yj.jianghongdianzi.cn

Go:   // 手写递归
来源：http://uw.muxihuayi.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://eu.gzmigu.cn

C#:   // 手写递归
来源：http://pb.yuexingan06.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://eo.newstarts.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://fg.newstarts.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://jl.huanxung.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://vm.chemitech.net.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://xe.yuntaijiaju.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://dh.gzmigu.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://jj.hahajie.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://cr.huanxung.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://zv.jctech888.com.cn

================================================================================
来源：http://um.shxzukj.cn

O. 并发与异步
来源：http://ma.jctech888.com.cn

================================================================================
来源：http://sz.521024.cn

[O01] 启动一个线程
来源：http://rc.huanxung.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://fy.szxytkj.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://zg.9csxet.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://yj.huanxung.cn

TS:   // 同 JS
来源：http://yp.muxihuayi.cn

Java: new Thread(() -> f()).start()
来源：http://ah.jctech888.com.cn

Go:   go f()
来源：http://ql.newstarts.cn

Ruby: Thread.new { f }
来源：http://nn.hnjuh.cn

C#:   Task.Run(() => F());
来源：http://db.colortex.cn

[O02] 使用线程池
来源：http://gz.asd995.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://bi.colortex.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://op.muxihuayi.cn

JS:   // worker_threads 线程池
来源：http://ll.wgjwhj.cn

TS:   // worker_threads 线程池
来源：http://ht.huanxung.cn

Java: Executors.newFixedThreadPool(4)
来源：http://zq.chemitech.net.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://bo.haigaiapp.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ru.bookmarksfly.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://qs.shtwfgs.cn

[O03] 加锁保护共享数据
来源：http://ta.chemitech.net.cn

Py:   with lock: shared += 1
来源：http://jg.yuntaijiaju.cn

PHP:  // 用 flock() 做文件锁
来源：http://rd.jctech888.com.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://oh.shxzskj.cn

TS:   // 同 JS
来源：http://yq.newstarts.cn

Java: synchronized (this) { shared++; }
来源：http://xq.jctech888.com.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://st.jianghongdianzi.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://td.jctech888.com.cn

C#:   lock (gate) { shared++; }
来源：http://kl.bjjhwx.cn

[O04] 定义异步函数并等待
来源：http://zb.wgjwhj.cn

Py:   async def f():⏎    await g()
来源：http://yy.szsharing.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://rd.nszjky.cn

JS:   async function f() { await g(); }
来源：http://ly.szsharing.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://hh.gzmigu.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://cs.colortex.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://sn.bookmarksfly.cn

Ruby: # 用 Fiber 或 async gem
来源：http://dv.muxihuayi.cn

C#:   async Task F() { await G(); }
来源：http://hn.jianghongdianzi.cn

[O05] 并发执行并等待全部完成
来源：http://rm.chemitech.net.cn

Py:   asyncio.gather(*tasks)
来源：http://nr.shxzukj.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://lh.yuexingan06.cn

JS:   await Promise.all(tasks)
来源：http://yw.bookmarksfly.cn

TS:   await Promise.all(tasks)
来源：http://mo.huanxung.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://bj.yuexingan06.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://bb.haigaiapp.cn

Ruby: threads.map(&:join)
来源：http://gd.chemitech.net.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://pz.lnxyls.cn

[O06] 使用进程池
来源：http://ev.huixiangedu.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://sv.huixiangedu.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://rx.yuntaijiaju.cn

JS:   // child_process / cluster 模块
来源：http://cl.szxytkj.cn

TS:   // child_process / cluster 模块
来源：http://zb.huixiangedu.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://pn.huanxung.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hk.haigaiapp.cn

Ruby: // fork 块
来源：http://nc.huixiangedu.cn

C#:   Parallel.For
来源：http://pt.asd995.cn

================================================================================
来源：http://ba.newstarts.cn

P. 常用工具函数
来源：http://qc.bookmarksfly.cn

================================================================================
来源：http://tp.521024.cn

[P01] 生成 UUID
来源：http://xr.521024.cn

Py:   str(uuid.uuid4())
来源：http://lj.panjiajie.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://vm.colortex.cn

JS:   crypto.randomUUID()
来源：http://pv.muxihuayi.cn

TS:   crypto.randomUUID()
来源：http://ex.huanxung.cn

Java: UUID.randomUUID().toString()
来源：http://gm.huanxung.cn

Go:   // 用 github.com/google/uuid
来源：http://dx.lnxyls.cn

Ruby: SecureRandom.uuid
来源：http://ud.newstarts.cn

C#:   Guid.NewGuid().ToString()
来源：http://at.huixiangedu.cn

[P02] MD5 / SHA256 摘要
来源：http://gd.newstarts.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://uy.521024.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://kj.hahajie.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mm.colortex.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://uv.jctech888.com.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ok.jctech888.com.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://kp.yuntaijiaju.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://xl.szxytkj.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://xy.gzmigu.cn

[P03] 生成短随机字符串
来源：http://nv.hnjuh.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://gh.newstarts.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hb.shxzskj.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://zm.haigaiapp.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://vr.asd995.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wr.bjjhwx.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://jo.haigaiapp.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://hx.shxzskj.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://zd.nicolike.cn

[P04] 求长度
来源：http://ck.panjiajie.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ii.9csxet.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://fk.wgjwhj.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ar.bjjhwx.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://un.asd995.cn

Java: list.size();  map.size();  s.length()
来源：http://ci.huixinmuqiang.cn

Go:   len(arr);  len(m)
来源：http://xb.huixiangedu.cn

Ruby: x.length;  x.size
来源：http://rm.asd995.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://ha.jianghongdianzi.cn

[P05] 判断两个对象内容是否相等
来源：http://jl.huixiangedu.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://vn.asd995.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mq.nicolike.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://vi.asd995.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://jn.hnjuh.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://pa.hnjuh.cn

Go:   reflect.DeepEqual(a, b)
来源：http://jo.bjjhwx.cn

Ruby: a == b
来源：http://vz.hnjuh.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ap.yuntaijiaju.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://pe.panjiajie.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wh.yuexingan06.cn

PHP:  if (empty($x)) {}
来源：http://ue.shxzukj.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://vc.asd995.cn

TS:   if (x == null) {}
来源：http://lb.wgjwhj.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://io.yuexingan06.cn

Go:   if x == nil {}
来源：http://bw.asd995.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wf.szxytkj.cn

C#:   if (x is null) {}
来源：http://jt.wgjwhj.cn

[P07] 防抖与节流
来源：http://ts.shtwfgs.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://dv.hnjuh.cn

PHP:  // 手写时间戳比较
来源：http://tu.jctech888.com.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://yh.bjjhwx.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mi.muxihuayi.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://dd.bjjhwx.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hl.chemitech.net.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://mu.shtwfgs.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://nd.hnjuh.cn

[P08] 处理浮点精度问题
来源：http://nt.shxzukj.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wl.nszjky.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ex.bjjhwx.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://et.chemitech.net.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wg.newstarts.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://xv.yuexingan06.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ae.newstarts.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://xr.chemitech.net.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://tj.jianghongdianzi.cn

================================================================================
来源：http://of.szsharing.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://rc.hnjuh.cn

================================================================================
来源：http://sj.huanxung.cn

[Q01] 创建表
来源：http://jh.huixinmuqiang.cn

CREATE TABLE users (
来源：http://dj.bjjhwx.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://gd.hahajie.cn

name VARCHAR(50) NOT NULL,
来源：http://ll.muxihuayi.cn

email VARCHAR(100) UNIQUE,
来源：http://uo.hahajie.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://rf.haigaiapp.cn

);
来源：http://uf.muxihuayi.cn

[Q02] 创建带外键的表
来源：http://hv.shxzukj.cn

CREATE TABLE orders (
来源：http://iu.yuexingan06.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://rx.shxzskj.cn

user_id INT NOT NULL,
来源：http://tk.szxytkj.cn

amount DECIMAL(10, 2),
来源：http://hu.colortex.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://et.huixinmuqiang.cn

);
来源：http://zy.wgjwhj.cn

[Q03] 增加列
来源：http://wq.newstarts.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://rh.chemitech.net.cn

[Q04] 修改列类型
来源：http://uf.bjjhwx.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://uv.yuntaijiaju.cn

[Q05] 重命名列
来源：http://dz.jctech888.com.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://fk.nicolike.cn

[Q06] 删除列
来源：http://ew.szsharing.cn

ALTER TABLE users DROP COLUMN age;
来源：http://sh.chemitech.net.cn

[Q07] 删除表
来源：http://oq.jctech888.com.cn

DROP TABLE IF EXISTS orders;
来源：http://no.newstarts.cn

[Q08] 创建普通索引
来源：http://hn.huanxung.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://xc.huixinmuqiang.cn

[Q09] 创建唯一索引
来源：http://pm.yuntaijiaju.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://qu.huixinmuqiang.cn

[Q10] 插入单行
来源：http://yp.shtwfgs.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ws.szxytkj.cn

[Q11] 一次插入多行
来源：http://ne.lnxyls.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://kb.shtwfgs.cn

[Q12] 插入后取自增 ID
来源：http://im.wgjwhj.cn

INSERT INTO users (name) VALUES ('C');
来源：http://it.shxzukj.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://cj.szxytkj.cn

[Q13] 忽略重复插入
来源：http://hw.haigaiapp.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://at.jianghongdianzi.cn

[Q14] 存在则更新（upsert）
来源：http://bh.muxihuayi.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://pv.panjiajie.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://re.hahajie.cn

[Q15] 查询全部
来源：http://nt.hahajie.cn

SELECT * FROM users;
来源：http://qe.szxytkj.cn

[Q16] 查询指定列
来源：http://hu.lnxyls.cn

SELECT id, name FROM users;
来源：http://re.bjjhwx.cn

[Q17] 条件查询
来源：http://qm.bookmarksfly.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://tz.yuntaijiaju.cn

[Q18] 模糊匹配
来源：http://ep.huanxung.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://gl.huixinmuqiang.cn

[Q19] 范围查询
来源：http://zt.colortex.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ed.colortex.cn

[Q20] IN 列表
来源：http://nn.colortex.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://fd.hahajie.cn

[Q21] 空值判断
来源：http://ml.huanxung.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://nh.asd995.cn

[Q22] 排序
来源：http://yh.muxihuayi.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://le.bjjhwx.cn

[Q23] 分页
来源：http://pt.yuexingan06.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://kq.szxytkj.cn

[Q24] 去重
来源：http://yl.lnxyls.cn

SELECT DISTINCT city FROM users;
来源：http://ux.hnjuh.cn

[Q25] 只取前 N 条
来源：http://xq.chemitech.net.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mh.huixinmuqiang.cn

[Q26] 计数
来源：http://fg.szxytkj.cn

SELECT COUNT(*) FROM users;
来源：http://og.yuexingan06.cn

[Q27] 条件计数
来源：http://yx.panjiajie.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://uy.shtwfgs.cn

[Q28] 求和与平均
来源：http://bd.yuexingan06.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://dw.szxytkj.cn

[Q29] 最大最小值
来源：http://ie.9csxet.cn


<!-- 参考信息 -->