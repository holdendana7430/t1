代发 wailian999

JS:   [...arr].sort((a, b) => a - b)
来源：http://za.jianghongdianzi.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://kz.lnxyls.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://de.newstarts.cn

Go:   slices.Sort(arr)
来源：http://oj.jianghongdianzi.cn

Ruby: arr.sort
来源：http://qh.colortex.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://af.asd995.cn

[N03] 快速排序（分治示例）
来源：http://oh.wgjwhj.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://xm.huanxung.cn

PHP:  // 递归实现，或用 usort
来源：http://xk.haigaiapp.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://zc.jctech888.com.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ua.shxzskj.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://of.shxzukj.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://uk.newstarts.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://lq.huixinmuqiang.cn

C#:   // 手写递归，或 Array.Sort
来源：http://ca.yuexingan06.cn

[N04] 斐波那契数列
来源：http://xb.szxytkj.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://px.bookmarksfly.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ab.shxzskj.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://qg.szsharing.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://fw.haigaiapp.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://lu.wgjwhj.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://eu.huixinmuqiang.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ya.asd995.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://tg.jctech888.com.cn

[N05] 最大公约数
来源：http://se.shtwfgs.cn

Py:   math.gcd(a, b)
来源：http://ek.szxytkj.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://qe.yuntaijiaju.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://te.nicolike.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://am.newstarts.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hn.9csxet.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ik.colortex.cn

Ruby: a.gcd(b)
来源：http://zy.shxzskj.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://yu.gzmigu.cn

[N06] 判断回文字符串
来源：http://pv.asd995.cn

Py:   s == s[::-1]
来源：http://ea.jianghongdianzi.cn

PHP:  $s === strrev($s);
来源：http://cr.hahajie.cn

JS:   s === [...s].reverse().join("")
来源：http://xv.hnjuh.cn

TS:   s === [...s].reverse().join("")
来源：http://rg.bjjhwx.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://sb.shxzskj.cn

Go:   // 双指针从两端比较
来源：http://ni.muxihuayi.cn

Ruby: s == s.reverse
来源：http://ci.hahajie.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://zs.panjiajie.cn

[N07] 两数之和（返回下标）
来源：http://sm.shxzskj.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://so.haigaiapp.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://jr.hnjuh.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://da.huixinmuqiang.cn

TS:   // 手写 Map<string, number>
来源：http://jy.nicolike.cn

Java: // 手写 HashMap
来源：http://ot.gzmigu.cn

Go:   // 手写 map[int]int
来源：http://ty.wgjwhj.cn

Ruby: // 手写 Hash
来源：http://su.huixiangedu.cn

C#:   // 手写 Dictionary<int, int>
来源：http://jb.nszjky.cn

[N08] 生成全排列
来源：http://ju.huixiangedu.cn

Py:   itertools.permutations(arr)
来源：http://ba.jctech888.com.cn

PHP:  // 手写递归交换
来源：http://ad.9csxet.cn

JS:   // 手写回溯递归
来源：http://ep.jctech888.com.cn

TS:   // 手写回溯递归
来源：http://cn.muxihuayi.cn

Java: // 手写回溯递归
来源：http://ys.nicolike.cn

Go:   // 手写回溯递归
来源：http://pw.huanxung.cn

Ruby: arr.permutation.to_a
来源：http://hg.yuntaijiaju.cn

C#:   // 手写回溯递归
来源：http://bh.9csxet.cn

[N09] 栈与队列
来源：http://gw.jianghongdianzi.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://up.yuexingan06.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://pa.yuexingan06.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://un.huixinmuqiang.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://sw.bjjhwx.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://zj.muxihuayi.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://zd.9csxet.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://sn.huixinmuqiang.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://zt.szsharing.cn

[N10] 链表节点定义
来源：http://mc.521024.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://nc.muxihuayi.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://wn.9csxet.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wv.gzmigu.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ll.jctech888.com.cn

Java: class Node { int v; Node next; }
来源：http://sq.muxihuayi.cn

Go:   type Node struct { V int; Next *Node }
来源：http://im.shxzukj.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://rr.hnjuh.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://es.jianghongdianzi.cn

[N11] 二叉树中序遍历
来源：http://ed.wgjwhj.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://si.chemitech.net.cn

PHP:  // 手写递归函数
来源：http://qo.shxzukj.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://zj.bookmarksfly.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ay.colortex.cn

Java: // 手写递归
来源：http://ox.szxytkj.cn

Go:   // 手写递归
来源：http://qt.gzmigu.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://fv.colortex.cn

C#:   // 手写递归
来源：http://kz.yuntaijiaju.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://eu.huanxung.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://qx.shxzskj.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://sv.jianghongdianzi.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://aj.lnxyls.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ds.yuntaijiaju.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://zv.yuntaijiaju.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://iv.asd995.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ie.asd995.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://af.yuexingan06.cn

================================================================================
来源：http://om.shxzskj.cn

O. 并发与异步
来源：http://gu.yuexingan06.cn

================================================================================
来源：http://wz.yuntaijiaju.cn

[O01] 启动一个线程
来源：http://rx.szsharing.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://kv.jianghongdianzi.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ac.muxihuayi.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ke.szxytkj.cn

TS:   // 同 JS
来源：http://uh.yuexingan06.cn

Java: new Thread(() -> f()).start()
来源：http://ko.szsharing.cn

Go:   go f()
来源：http://ge.yuexingan06.cn

Ruby: Thread.new { f }
来源：http://hy.huixiangedu.cn

C#:   Task.Run(() => F());
来源：http://ig.9csxet.cn

[O02] 使用线程池
来源：http://it.szsharing.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://fg.huanxung.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://vz.szxytkj.cn

JS:   // worker_threads 线程池
来源：http://ld.muxihuayi.cn

TS:   // worker_threads 线程池
来源：http://cl.hnjuh.cn

Java: Executors.newFixedThreadPool(4)
来源：http://fi.521024.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://xx.shxzukj.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://fh.521024.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://zy.colortex.cn

[O03] 加锁保护共享数据
来源：http://ae.yuexingan06.cn

Py:   with lock: shared += 1
来源：http://xp.hnjuh.cn

PHP:  // 用 flock() 做文件锁
来源：http://vg.szsharing.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://nh.wgjwhj.cn

TS:   // 同 JS
来源：http://tx.nszjky.cn

Java: synchronized (this) { shared++; }
来源：http://va.wgjwhj.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://kc.wgjwhj.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://ld.panjiajie.cn

C#:   lock (gate) { shared++; }
来源：http://aq.wgjwhj.cn

[O04] 定义异步函数并等待
来源：http://bq.yuntaijiaju.cn

Py:   async def f():⏎    await g()
来源：http://yj.nicolike.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://nh.szsharing.cn

JS:   async function f() { await g(); }
来源：http://mc.jctech888.com.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://pe.chemitech.net.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://cd.szsharing.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://qr.bookmarksfly.cn

Ruby: # 用 Fiber 或 async gem
来源：http://rk.yuexingan06.cn

C#:   async Task F() { await G(); }
来源：http://bp.hahajie.cn

[O05] 并发执行并等待全部完成
来源：http://zu.asd995.cn

Py:   asyncio.gather(*tasks)
来源：http://ui.szxytkj.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ct.asd995.cn

JS:   await Promise.all(tasks)
来源：http://ih.wgjwhj.cn

TS:   await Promise.all(tasks)
来源：http://dh.chemitech.net.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://sz.yuntaijiaju.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://bb.panjiajie.cn

Ruby: threads.map(&:join)
来源：http://ao.yuntaijiaju.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://tf.yuntaijiaju.cn

[O06] 使用进程池
来源：http://jo.haigaiapp.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://av.nicolike.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://mg.bookmarksfly.cn

JS:   // child_process / cluster 模块
来源：http://oc.521024.cn

TS:   // child_process / cluster 模块
来源：http://ed.hahajie.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://zk.huixiangedu.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://uv.bjjhwx.cn

Ruby: // fork 块
来源：http://ar.hahajie.cn

C#:   Parallel.For
来源：http://vx.jianghongdianzi.cn

================================================================================
来源：http://pg.muxihuayi.cn

P. 常用工具函数
来源：http://lo.muxihuayi.cn

================================================================================
来源：http://du.nicolike.cn

[P01] 生成 UUID
来源：http://rm.jctech888.com.cn

Py:   str(uuid.uuid4())
来源：http://ff.shxzskj.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://dq.jctech888.com.cn

JS:   crypto.randomUUID()
来源：http://my.bjjhwx.cn

TS:   crypto.randomUUID()
来源：http://zg.asd995.cn

Java: UUID.randomUUID().toString()
来源：http://qd.szxytkj.cn

Go:   // 用 github.com/google/uuid
来源：http://ls.bjjhwx.cn

Ruby: SecureRandom.uuid
来源：http://mf.yuntaijiaju.cn

C#:   Guid.NewGuid().ToString()
来源：http://za.hnjuh.cn

[P02] MD5 / SHA256 摘要
来源：http://ed.huixinmuqiang.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hb.9csxet.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://ho.yuntaijiaju.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ks.hahajie.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://gb.muxihuayi.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://yw.yuntaijiaju.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mr.asd995.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ck.nszjky.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://fo.hnjuh.cn

[P03] 生成短随机字符串
来源：http://nx.shxzukj.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://tt.haigaiapp.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ts.jctech888.com.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://pj.hnjuh.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://rs.lnxyls.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ub.hahajie.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mu.colortex.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://ko.hahajie.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ec.chemitech.net.cn

[P04] 求长度
来源：http://iu.gzmigu.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://vy.colortex.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://dx.shxzskj.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://nn.chemitech.net.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://fa.bookmarksfly.cn

Java: list.size();  map.size();  s.length()
来源：http://mw.huixiangedu.cn

Go:   len(arr);  len(m)
来源：http://ql.newstarts.cn

Ruby: x.length;  x.size
来源：http://op.szxytkj.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://rc.colortex.cn

[P05] 判断两个对象内容是否相等
来源：http://dz.asd995.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://id.9csxet.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ld.panjiajie.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://jn.nicolike.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://tn.bjjhwx.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mh.haigaiapp.cn

Go:   reflect.DeepEqual(a, b)
来源：http://jh.huixinmuqiang.cn

Ruby: a == b
来源：http://sv.bjjhwx.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://sn.wgjwhj.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mz.hahajie.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://qt.521024.cn

PHP:  if (empty($x)) {}
来源：http://of.szsharing.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://td.jctech888.com.cn

TS:   if (x == null) {}
来源：http://tm.szxytkj.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://rb.shxzukj.cn

Go:   if x == nil {}
来源：http://cn.huixinmuqiang.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://np.panjiajie.cn

C#:   if (x is null) {}
来源：http://jt.521024.cn

[P07] 防抖与节流
来源：http://pg.chemitech.net.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wj.szxytkj.cn

PHP:  // 手写时间戳比较
来源：http://lj.yuexingan06.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ih.newstarts.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qn.nicolike.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://au.bjjhwx.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://vk.szxytkj.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://sb.9csxet.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://kv.jianghongdianzi.cn

[P08] 处理浮点精度问题
来源：http://mn.jctech888.com.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://um.shxzskj.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://gk.huanxung.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://dk.shxzukj.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://zu.9csxet.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://bt.newstarts.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wx.nicolike.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ea.huixinmuqiang.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://qt.nicolike.cn

================================================================================
来源：http://fu.bjjhwx.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wy.muxihuayi.cn

================================================================================
来源：http://cp.colortex.cn

[Q01] 创建表
来源：http://hg.hnjuh.cn

CREATE TABLE users (
来源：http://zc.bjjhwx.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://up.gzmigu.cn

name VARCHAR(50) NOT NULL,
来源：http://ls.nszjky.cn

email VARCHAR(100) UNIQUE,
来源：http://ks.nicolike.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://li.nszjky.cn

);
来源：http://jy.bjjhwx.cn

[Q02] 创建带外键的表
来源：http://uz.lnxyls.cn

CREATE TABLE orders (
来源：http://op.chemitech.net.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ld.haigaiapp.cn

user_id INT NOT NULL,
来源：http://bd.huixinmuqiang.cn

amount DECIMAL(10, 2),
来源：http://sa.hnjuh.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ct.newstarts.cn

);
来源：http://yz.haigaiapp.cn

[Q03] 增加列
来源：http://ms.shxzskj.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://pn.shxzskj.cn

[Q04] 修改列类型
来源：http://hg.lnxyls.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://xy.huixiangedu.cn

[Q05] 重命名列
来源：http://du.colortex.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://jo.panjiajie.cn

[Q06] 删除列
来源：http://um.huixiangedu.cn

ALTER TABLE users DROP COLUMN age;
来源：http://za.hnjuh.cn

[Q07] 删除表
来源：http://fr.jianghongdianzi.cn

DROP TABLE IF EXISTS orders;
来源：http://vh.huixinmuqiang.cn

[Q08] 创建普通索引
来源：http://gj.bjjhwx.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://ao.jctech888.com.cn

[Q09] 创建唯一索引
来源：http://an.asd995.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://pq.chemitech.net.cn

[Q10] 插入单行
来源：http://jk.nicolike.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ey.shxzskj.cn

[Q11] 一次插入多行
来源：http://pe.yuexingan06.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://eq.hahajie.cn

[Q12] 插入后取自增 ID
来源：http://ri.haigaiapp.cn

INSERT INTO users (name) VALUES ('C');
来源：http://dj.panjiajie.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://nz.haigaiapp.cn

[Q13] 忽略重复插入
来源：http://qy.colortex.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://us.haigaiapp.cn

[Q14] 存在则更新（upsert）
来源：http://ow.newstarts.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://bq.nicolike.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://xz.colortex.cn

[Q15] 查询全部
来源：http://rt.jctech888.com.cn

SELECT * FROM users;
来源：http://su.panjiajie.cn

[Q16] 查询指定列
来源：http://hn.hahajie.cn

SELECT id, name FROM users;
来源：http://so.gzmigu.cn

[Q17] 条件查询
来源：http://qi.shtwfgs.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://la.hahajie.cn

[Q18] 模糊匹配
来源：http://ny.bookmarksfly.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://jh.jctech888.com.cn

[Q19] 范围查询
来源：http://xw.hahajie.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://fk.huanxung.cn

[Q20] IN 列表
来源：http://nf.bookmarksfly.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://pb.lnxyls.cn

[Q21] 空值判断
来源：http://bv.yuexingan06.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://kx.yuexingan06.cn

[Q22] 排序
来源：http://cc.colortex.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ec.shtwfgs.cn

[Q23] 分页
来源：http://yc.szsharing.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://sa.huanxung.cn

[Q24] 去重
来源：http://ip.szxytkj.cn

SELECT DISTINCT city FROM users;
来源：http://zb.shxzskj.cn

[Q25] 只取前 N 条
来源：http://rr.muxihuayi.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://jb.szxytkj.cn

[Q26] 计数
来源：http://zo.jctech888.com.cn

SELECT COUNT(*) FROM users;
来源：http://jv.jctech888.com.cn

[Q27] 条件计数
来源：http://fr.huixiangedu.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ze.chemitech.net.cn

[Q28] 求和与平均
来源：http://vx.shxzskj.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://lt.yuntaijiaju.cn

[Q29] 最大最小值
来源：http://fs.bjjhwx.cn


<!-- 参考信息 -->