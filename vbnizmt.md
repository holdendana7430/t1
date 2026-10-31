代发 wailian999

C#:   Array.BinarySearch(arr, x)
来源：http://hz.nszjky.cn

[N02] 排序（工程实践用内置实现）
来源：http://si.gzmigu.cn

Py:   sorted(arr);  arr.sort()
来源：http://ke.wgjwhj.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://xp.9csxet.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://wo.newstarts.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://cu.wgjwhj.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ze.szxytkj.cn

Go:   slices.Sort(arr)
来源：http://ov.newstarts.cn

Ruby: arr.sort
来源：http://wl.jctech888.com.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://nr.jctech888.com.cn

[N03] 快速排序（分治示例）
来源：http://vw.shtwfgs.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://qq.521024.cn

PHP:  // 递归实现，或用 usort
来源：http://ir.jctech888.com.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hq.gzmigu.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://rh.bookmarksfly.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://cg.colortex.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://em.huanxung.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://dp.haigaiapp.cn

C#:   // 手写递归，或 Array.Sort
来源：http://lf.colortex.cn

[N04] 斐波那契数列
来源：http://pe.bjjhwx.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://xv.newstarts.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://kg.huixinmuqiang.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://co.asd995.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ej.colortex.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://vk.nszjky.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ew.gzmigu.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://cy.9csxet.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ud.yuexingan06.cn

[N05] 最大公约数
来源：http://ug.wgjwhj.cn

Py:   math.gcd(a, b)
来源：http://ex.hahajie.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://gv.jctech888.com.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ji.szsharing.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ex.521024.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://zk.chemitech.net.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://eh.shxzukj.cn

Ruby: a.gcd(b)
来源：http://lb.shxzukj.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://fo.521024.cn

[N06] 判断回文字符串
来源：http://lb.shxzukj.cn

Py:   s == s[::-1]
来源：http://rj.lnxyls.cn

PHP:  $s === strrev($s);
来源：http://hy.jctech888.com.cn

JS:   s === [...s].reverse().join("")
来源：http://uu.huixinmuqiang.cn

TS:   s === [...s].reverse().join("")
来源：http://na.521024.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://zj.nszjky.cn

Go:   // 双指针从两端比较
来源：http://ar.hnjuh.cn

Ruby: s == s.reverse
来源：http://kb.9csxet.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://pp.shtwfgs.cn

[N07] 两数之和（返回下标）
来源：http://mx.colortex.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://az.chemitech.net.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://da.yuntaijiaju.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://ny.newstarts.cn

TS:   // 手写 Map<string, number>
来源：http://sg.colortex.cn

Java: // 手写 HashMap
来源：http://ip.lnxyls.cn

Go:   // 手写 map[int]int
来源：http://pp.wgjwhj.cn

Ruby: // 手写 Hash
来源：http://du.bjjhwx.cn

C#:   // 手写 Dictionary<int, int>
来源：http://oz.bookmarksfly.cn

[N08] 生成全排列
来源：http://wd.jctech888.com.cn

Py:   itertools.permutations(arr)
来源：http://bd.bjjhwx.cn

PHP:  // 手写递归交换
来源：http://ee.521024.cn

JS:   // 手写回溯递归
来源：http://iu.hnjuh.cn

TS:   // 手写回溯递归
来源：http://cg.newstarts.cn

Java: // 手写回溯递归
来源：http://ph.huanxung.cn

Go:   // 手写回溯递归
来源：http://kq.panjiajie.cn

Ruby: arr.permutation.to_a
来源：http://qi.gzmigu.cn

C#:   // 手写回溯递归
来源：http://fk.shxzskj.cn

[N09] 栈与队列
来源：http://bv.szxytkj.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://zg.huanxung.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mq.shxzskj.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ux.nicolike.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://td.nicolike.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://di.nicolike.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ie.gzmigu.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://so.lnxyls.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hd.huixinmuqiang.cn

[N10] 链表节点定义
来源：http://tb.panjiajie.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://fk.shxzskj.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://qe.huixinmuqiang.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://bf.bjjhwx.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://dz.muxihuayi.cn

Java: class Node { int v; Node next; }
来源：http://xt.colortex.cn

Go:   type Node struct { V int; Next *Node }
来源：http://hc.nicolike.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://pv.nszjky.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://fb.gzmigu.cn

[N11] 二叉树中序遍历
来源：http://zc.shtwfgs.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ie.yuntaijiaju.cn

PHP:  // 手写递归函数
来源：http://nj.chemitech.net.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hh.shxzskj.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ar.bookmarksfly.cn

Java: // 手写递归
来源：http://is.asd995.cn

Go:   // 手写递归
来源：http://ek.yuexingan06.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ra.asd995.cn

C#:   // 手写递归
来源：http://jp.szxytkj.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ac.shxzukj.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://qj.huixiangedu.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ux.wgjwhj.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://vo.shtwfgs.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ny.nszjky.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://vd.jianghongdianzi.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://qe.jctech888.com.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://tt.colortex.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ie.bookmarksfly.cn

================================================================================
来源：http://ov.shxzskj.cn

O. 并发与异步
来源：http://za.szxytkj.cn

================================================================================
来源：http://xq.nszjky.cn

[O01] 启动一个线程
来源：http://jy.huixinmuqiang.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://pg.huixinmuqiang.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://rp.szxytkj.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://sg.shxzukj.cn

TS:   // 同 JS
来源：http://dd.hnjuh.cn

Java: new Thread(() -> f()).start()
来源：http://il.gzmigu.cn

Go:   go f()
来源：http://ln.gzmigu.cn

Ruby: Thread.new { f }
来源：http://te.szsharing.cn

C#:   Task.Run(() => F());
来源：http://qi.9csxet.cn

[O02] 使用线程池
来源：http://om.lnxyls.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mr.shtwfgs.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wp.huixiangedu.cn

JS:   // worker_threads 线程池
来源：http://es.haigaiapp.cn

TS:   // worker_threads 线程池
来源：http://wo.9csxet.cn

Java: Executors.newFixedThreadPool(4)
来源：http://st.szsharing.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ui.yuntaijiaju.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://qx.521024.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://lv.nszjky.cn

[O03] 加锁保护共享数据
来源：http://cp.521024.cn

Py:   with lock: shared += 1
来源：http://vw.haigaiapp.cn

PHP:  // 用 flock() 做文件锁
来源：http://rm.asd995.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ml.muxihuayi.cn

TS:   // 同 JS
来源：http://hu.szsharing.cn

Java: synchronized (this) { shared++; }
来源：http://bh.9csxet.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://tz.shxzukj.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://uk.yuntaijiaju.cn

C#:   lock (gate) { shared++; }
来源：http://pp.gzmigu.cn

[O04] 定义异步函数并等待
来源：http://ar.bjjhwx.cn

Py:   async def f():⏎    await g()
来源：http://zx.colortex.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ht.szxytkj.cn

JS:   async function f() { await g(); }
来源：http://gz.asd995.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://fi.asd995.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://dy.gzmigu.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://rx.shxzskj.cn

Ruby: # 用 Fiber 或 async gem
来源：http://he.yuexingan06.cn

C#:   async Task F() { await G(); }
来源：http://xx.gzmigu.cn

[O05] 并发执行并等待全部完成
来源：http://mp.hahajie.cn

Py:   asyncio.gather(*tasks)
来源：http://nz.hahajie.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://jc.panjiajie.cn

JS:   await Promise.all(tasks)
来源：http://ov.gzmigu.cn

TS:   await Promise.all(tasks)
来源：http://vi.yuntaijiaju.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://zc.yuexingan06.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://dr.panjiajie.cn

Ruby: threads.map(&:join)
来源：http://nz.nicolike.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://yf.nszjky.cn

[O06] 使用进程池
来源：http://bm.huanxung.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://nq.521024.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://hk.colortex.cn

JS:   // child_process / cluster 模块
来源：http://gh.nicolike.cn

TS:   // child_process / cluster 模块
来源：http://sq.lnxyls.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://bw.bookmarksfly.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://sa.wgjwhj.cn

Ruby: // fork 块
来源：http://ke.gzmigu.cn

C#:   Parallel.For
来源：http://rz.huanxung.cn

================================================================================
来源：http://sa.gzmigu.cn

P. 常用工具函数
来源：http://zl.jianghongdianzi.cn

================================================================================
来源：http://dc.haigaiapp.cn

[P01] 生成 UUID
来源：http://vb.hnjuh.cn

Py:   str(uuid.uuid4())
来源：http://ub.huixiangedu.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://tt.huanxung.cn

JS:   crypto.randomUUID()
来源：http://hl.gzmigu.cn

TS:   crypto.randomUUID()
来源：http://tm.521024.cn

Java: UUID.randomUUID().toString()
来源：http://sg.panjiajie.cn

Go:   // 用 github.com/google/uuid
来源：http://ch.521024.cn

Ruby: SecureRandom.uuid
来源：http://sv.hnjuh.cn

C#:   Guid.NewGuid().ToString()
来源：http://dn.yuntaijiaju.cn

[P02] MD5 / SHA256 摘要
来源：http://uk.hnjuh.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://jp.jctech888.com.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://wf.shxzukj.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://jd.haigaiapp.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://dl.chemitech.net.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://tq.bookmarksfly.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://vk.muxihuayi.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://bj.haigaiapp.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://zn.yuexingan06.cn

[P03] 生成短随机字符串
来源：http://os.haigaiapp.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://di.szxytkj.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mc.huanxung.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://gq.shxzukj.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ba.asd995.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mj.szxytkj.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://qu.wgjwhj.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://uw.shxzukj.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://dc.nicolike.cn

[P04] 求长度
来源：http://lk.jianghongdianzi.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://vk.colortex.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://un.bookmarksfly.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://yc.huanxung.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://iu.hahajie.cn

Java: list.size();  map.size();  s.length()
来源：http://ii.bookmarksfly.cn

Go:   len(arr);  len(m)
来源：http://fh.huixiangedu.cn

Ruby: x.length;  x.size
来源：http://vr.szsharing.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://wi.nicolike.cn

[P05] 判断两个对象内容是否相等
来源：http://jr.newstarts.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://lr.jctech888.com.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://nk.521024.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://yy.szxytkj.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://id.shtwfgs.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ks.shtwfgs.cn

Go:   reflect.DeepEqual(a, b)
来源：http://pr.521024.cn

Ruby: a == b
来源：http://il.nicolike.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://og.hnjuh.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ci.szxytkj.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://sy.asd995.cn

PHP:  if (empty($x)) {}
来源：http://wh.shxzskj.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://zv.asd995.cn

TS:   if (x == null) {}
来源：http://nw.yuexingan06.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://dw.jctech888.com.cn

Go:   if x == nil {}
来源：http://tr.huixinmuqiang.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://gv.yuexingan06.cn

C#:   if (x is null) {}
来源：http://ul.shtwfgs.cn

[P07] 防抖与节流
来源：http://tt.asd995.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://pb.hahajie.cn

PHP:  // 手写时间戳比较
来源：http://xk.hahajie.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://as.hahajie.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://il.yuntaijiaju.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://kx.shxzskj.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://nt.bookmarksfly.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://mi.shtwfgs.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hm.lnxyls.cn

[P08] 处理浮点精度问题
来源：http://je.szxytkj.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://rm.yuexingan06.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://rg.nszjky.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ub.nicolike.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wg.huanxung.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ux.muxihuayi.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://rt.huixiangedu.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://pq.newstarts.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://zg.colortex.cn

================================================================================
来源：http://kj.newstarts.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ks.colortex.cn

================================================================================
来源：http://ns.jctech888.com.cn

[Q01] 创建表
来源：http://xb.huanxung.cn

CREATE TABLE users (
来源：http://ri.muxihuayi.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wq.bookmarksfly.cn

name VARCHAR(50) NOT NULL,
来源：http://mv.szxytkj.cn

email VARCHAR(100) UNIQUE,
来源：http://ai.yuntaijiaju.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://iy.asd995.cn

);
来源：http://tl.shtwfgs.cn

[Q02] 创建带外键的表
来源：http://gv.bjjhwx.cn

CREATE TABLE orders (
来源：http://aj.haigaiapp.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ir.nszjky.cn

user_id INT NOT NULL,
来源：http://ym.521024.cn

amount DECIMAL(10, 2),
来源：http://xg.colortex.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://fh.huanxung.cn

);
来源：http://na.colortex.cn

[Q03] 增加列
来源：http://sp.lnxyls.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://rs.muxihuayi.cn

[Q04] 修改列类型
来源：http://ct.9csxet.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ix.newstarts.cn

[Q05] 重命名列
来源：http://cc.521024.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://zh.shxzukj.cn

[Q06] 删除列
来源：http://sw.shxzskj.cn

ALTER TABLE users DROP COLUMN age;
来源：http://os.chemitech.net.cn

[Q07] 删除表
来源：http://jp.panjiajie.cn

DROP TABLE IF EXISTS orders;
来源：http://hs.muxihuayi.cn

[Q08] 创建普通索引
来源：http://cy.yuntaijiaju.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://gw.yuntaijiaju.cn

[Q09] 创建唯一索引
来源：http://hl.lnxyls.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://jq.szsharing.cn

[Q10] 插入单行
来源：http://ob.yuexingan06.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://yc.jctech888.com.cn

[Q11] 一次插入多行
来源：http://so.huanxung.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://lz.chemitech.net.cn

[Q12] 插入后取自增 ID
来源：http://wk.9csxet.cn

INSERT INTO users (name) VALUES ('C');
来源：http://fo.shtwfgs.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ij.szsharing.cn

[Q13] 忽略重复插入
来源：http://zm.yuexingan06.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://cq.shxzskj.cn

[Q14] 存在则更新（upsert）
来源：http://uy.wgjwhj.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://pt.nszjky.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://fk.9csxet.cn

[Q15] 查询全部
来源：http://xp.panjiajie.cn

SELECT * FROM users;
来源：http://pv.nszjky.cn

[Q16] 查询指定列
来源：http://ly.shtwfgs.cn

SELECT id, name FROM users;
来源：http://ys.yuntaijiaju.cn

[Q17] 条件查询
来源：http://wl.hnjuh.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://cq.yuexingan06.cn

[Q18] 模糊匹配
来源：http://oy.colortex.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://jr.yuntaijiaju.cn

[Q19] 范围查询
来源：http://nx.hnjuh.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://gp.shtwfgs.cn

[Q20] IN 列表
来源：http://qt.haigaiapp.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://rj.bjjhwx.cn

[Q21] 空值判断
来源：http://ls.hahajie.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://by.yuntaijiaju.cn

[Q22] 排序
来源：http://bw.colortex.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://zq.hnjuh.cn

[Q23] 分页
来源：http://zu.shtwfgs.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://vx.shxzukj.cn

[Q24] 去重
来源：http://um.panjiajie.cn

SELECT DISTINCT city FROM users;
来源：http://hc.newstarts.cn

[Q25] 只取前 N 条
来源：http://ax.jianghongdianzi.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://av.shtwfgs.cn

[Q26] 计数
来源：http://js.haigaiapp.cn

SELECT COUNT(*) FROM users;
来源：http://rv.hahajie.cn

[Q27] 条件计数
来源：http://hq.9csxet.cn


<!-- 参考信息 -->