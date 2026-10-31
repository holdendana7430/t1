代发 wailian999

JS:   [...arr].sort((a, b) => a - b)
来源：http://ej.huixinmuqiang.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://ty.szsharing.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://lm.szxytkj.cn

Go:   slices.Sort(arr)
来源：http://gy.521024.cn

Ruby: arr.sort
来源：http://id.nicolike.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://fm.shtwfgs.cn

[N03] 快速排序（分治示例）
来源：http://eb.jianghongdianzi.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ym.newstarts.cn

PHP:  // 递归实现，或用 usort
来源：http://ci.shxzskj.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://zi.szxytkj.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ng.jctech888.com.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ho.szsharing.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://bo.huanxung.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://bm.colortex.cn

C#:   // 手写递归，或 Array.Sort
来源：http://cw.asd995.cn

[N04] 斐波那契数列
来源：http://rw.bookmarksfly.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://qq.9csxet.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://sj.hnjuh.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://jj.bookmarksfly.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://gf.asd995.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://qg.szsharing.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ng.lnxyls.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://gp.huixiangedu.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ct.hnjuh.cn

[N05] 最大公约数
来源：http://sp.gzmigu.cn

Py:   math.gcd(a, b)
来源：http://bd.chemitech.net.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://il.huixiangedu.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://pw.wgjwhj.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://bc.gzmigu.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://rp.gzmigu.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://fz.shtwfgs.cn

Ruby: a.gcd(b)
来源：http://dc.yuntaijiaju.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wk.521024.cn

[N06] 判断回文字符串
来源：http://oz.haigaiapp.cn

Py:   s == s[::-1]
来源：http://re.colortex.cn

PHP:  $s === strrev($s);
来源：http://ng.lnxyls.cn

JS:   s === [...s].reverse().join("")
来源：http://aq.shxzskj.cn

TS:   s === [...s].reverse().join("")
来源：http://qw.colortex.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wf.szsharing.cn

Go:   // 双指针从两端比较
来源：http://os.huanxung.cn

Ruby: s == s.reverse
来源：http://sg.jianghongdianzi.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://rd.gzmigu.cn

[N07] 两数之和（返回下标）
来源：http://vk.haigaiapp.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://dt.lnxyls.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://qq.huanxung.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://ne.huanxung.cn

TS:   // 手写 Map<string, number>
来源：http://ql.gzmigu.cn

Java: // 手写 HashMap
来源：http://hd.yuexingan06.cn

Go:   // 手写 map[int]int
来源：http://le.newstarts.cn

Ruby: // 手写 Hash
来源：http://ri.521024.cn

C#:   // 手写 Dictionary<int, int>
来源：http://tj.wgjwhj.cn

[N08] 生成全排列
来源：http://cg.yuexingan06.cn

Py:   itertools.permutations(arr)
来源：http://xw.lnxyls.cn

PHP:  // 手写递归交换
来源：http://kj.haigaiapp.cn

JS:   // 手写回溯递归
来源：http://th.jctech888.com.cn

TS:   // 手写回溯递归
来源：http://xj.newstarts.cn

Java: // 手写回溯递归
来源：http://kw.newstarts.cn

Go:   // 手写回溯递归
来源：http://pe.muxihuayi.cn

Ruby: arr.permutation.to_a
来源：http://ye.panjiajie.cn

C#:   // 手写回溯递归
来源：http://uk.bookmarksfly.cn

[N09] 栈与队列
来源：http://xb.nicolike.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://yd.colortex.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://dr.muxihuayi.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://sx.hnjuh.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://of.bookmarksfly.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://jg.hahajie.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hm.hahajie.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://am.chemitech.net.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://qh.huixinmuqiang.cn

[N10] 链表节点定义
来源：http://ei.hahajie.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://pl.asd995.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://qw.chemitech.net.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://al.shxzukj.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://fp.yuntaijiaju.cn

Java: class Node { int v; Node next; }
来源：http://wp.bjjhwx.cn

Go:   type Node struct { V int; Next *Node }
来源：http://xu.hnjuh.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://bt.muxihuayi.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://yj.szxytkj.cn

[N11] 二叉树中序遍历
来源：http://tg.jianghongdianzi.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ke.nszjky.cn

PHP:  // 手写递归函数
来源：http://pz.colortex.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://av.lnxyls.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://zw.yuexingan06.cn

Java: // 手写递归
来源：http://rb.hahajie.cn

Go:   // 手写递归
来源：http://rx.shxzskj.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wd.newstarts.cn

C#:   // 手写递归
来源：http://oo.muxihuayi.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mt.huixiangedu.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mc.wgjwhj.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://bg.bookmarksfly.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://od.chemitech.net.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://lv.hahajie.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://zz.panjiajie.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://og.panjiajie.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://zf.huanxung.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ry.huixinmuqiang.cn

================================================================================
来源：http://pj.nszjky.cn

O. 并发与异步
来源：http://jw.yuntaijiaju.cn

================================================================================
来源：http://bx.nicolike.cn

[O01] 启动一个线程
来源：http://mb.nicolike.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ez.hnjuh.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ua.newstarts.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://cx.panjiajie.cn

TS:   // 同 JS
来源：http://ap.gzmigu.cn

Java: new Thread(() -> f()).start()
来源：http://xx.szxytkj.cn

Go:   go f()
来源：http://yd.newstarts.cn

Ruby: Thread.new { f }
来源：http://qb.lnxyls.cn

C#:   Task.Run(() => F());
来源：http://fj.wgjwhj.cn

[O02] 使用线程池
来源：http://fc.nicolike.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://oy.nszjky.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://eo.shxzskj.cn

JS:   // worker_threads 线程池
来源：http://ca.nicolike.cn

TS:   // worker_threads 线程池
来源：http://xd.szsharing.cn

Java: Executors.newFixedThreadPool(4)
来源：http://pt.huanxung.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ct.muxihuayi.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://tp.bookmarksfly.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://xq.bjjhwx.cn

[O03] 加锁保护共享数据
来源：http://ev.muxihuayi.cn

Py:   with lock: shared += 1
来源：http://cw.jctech888.com.cn

PHP:  // 用 flock() 做文件锁
来源：http://tl.yuexingan06.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://bl.muxihuayi.cn

TS:   // 同 JS
来源：http://ec.shtwfgs.cn

Java: synchronized (this) { shared++; }
来源：http://za.szxytkj.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wh.yuexingan06.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://kr.jctech888.com.cn

C#:   lock (gate) { shared++; }
来源：http://qz.huixinmuqiang.cn

[O04] 定义异步函数并等待
来源：http://si.bookmarksfly.cn

Py:   async def f():⏎    await g()
来源：http://hf.bjjhwx.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://eo.bookmarksfly.cn

JS:   async function f() { await g(); }
来源：http://wt.huixinmuqiang.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://en.haigaiapp.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://gk.521024.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ne.haigaiapp.cn

Ruby: # 用 Fiber 或 async gem
来源：http://se.huanxung.cn

C#:   async Task F() { await G(); }
来源：http://pg.huixinmuqiang.cn

[O05] 并发执行并等待全部完成
来源：http://wq.panjiajie.cn

Py:   asyncio.gather(*tasks)
来源：http://vn.shtwfgs.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://tl.hnjuh.cn

JS:   await Promise.all(tasks)
来源：http://jn.yuntaijiaju.cn

TS:   await Promise.all(tasks)
来源：http://ov.haigaiapp.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://fv.shxzukj.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://bp.bookmarksfly.cn

Ruby: threads.map(&:join)
来源：http://yn.yuexingan06.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://ep.jctech888.com.cn

[O06] 使用进程池
来源：http://nk.szxytkj.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://nc.shxzukj.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://jo.bookmarksfly.cn

JS:   // child_process / cluster 模块
来源：http://vo.huixiangedu.cn

TS:   // child_process / cluster 模块
来源：http://je.wgjwhj.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://pl.colortex.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://fx.huixiangedu.cn

Ruby: // fork 块
来源：http://ny.yuntaijiaju.cn

C#:   Parallel.For
来源：http://rn.jianghongdianzi.cn

================================================================================
来源：http://xk.muxihuayi.cn

P. 常用工具函数
来源：http://xk.yuexingan06.cn

================================================================================
来源：http://gy.nszjky.cn

[P01] 生成 UUID
来源：http://kq.lnxyls.cn

Py:   str(uuid.uuid4())
来源：http://fm.bjjhwx.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://qk.huanxung.cn

JS:   crypto.randomUUID()
来源：http://cu.haigaiapp.cn

TS:   crypto.randomUUID()
来源：http://ts.bookmarksfly.cn

Java: UUID.randomUUID().toString()
来源：http://es.huixiangedu.cn

Go:   // 用 github.com/google/uuid
来源：http://al.lnxyls.cn

Ruby: SecureRandom.uuid
来源：http://gu.szsharing.cn

C#:   Guid.NewGuid().ToString()
来源：http://hs.nszjky.cn

[P02] MD5 / SHA256 摘要
来源：http://ag.yuexingan06.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hj.521024.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://ux.huixinmuqiang.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://no.shtwfgs.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mg.jctech888.com.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://lu.9csxet.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ei.bjjhwx.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mq.muxihuayi.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ay.shxzukj.cn

[P03] 生成短随机字符串
来源：http://zn.szxytkj.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://cw.yuexingan06.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ww.chemitech.net.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://zc.jianghongdianzi.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://un.muxihuayi.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://rf.jianghongdianzi.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hj.nicolike.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://iy.9csxet.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://an.wgjwhj.cn

[P04] 求长度
来源：http://gn.shxzskj.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://fl.lnxyls.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ch.nszjky.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://pr.muxihuayi.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://np.huixinmuqiang.cn

Java: list.size();  map.size();  s.length()
来源：http://za.haigaiapp.cn

Go:   len(arr);  len(m)
来源：http://gi.jctech888.com.cn

Ruby: x.length;  x.size
来源：http://ns.muxihuayi.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://vd.shxzskj.cn

[P05] 判断两个对象内容是否相等
来源：http://mi.haigaiapp.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://kn.jianghongdianzi.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wy.shxzukj.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mt.colortex.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://rp.chemitech.net.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://sp.szsharing.cn

Go:   reflect.DeepEqual(a, b)
来源：http://pw.lnxyls.cn

Ruby: a == b
来源：http://ce.bjjhwx.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://fr.nszjky.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ii.shxzskj.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://vo.521024.cn

PHP:  if (empty($x)) {}
来源：http://pk.jctech888.com.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://rz.nszjky.cn

TS:   if (x == null) {}
来源：http://oj.huixiangedu.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://kp.wgjwhj.cn

Go:   if x == nil {}
来源：http://is.chemitech.net.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ku.yuexingan06.cn

C#:   if (x is null) {}
来源：http://it.nszjky.cn

[P07] 防抖与节流
来源：http://ak.bjjhwx.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mr.shtwfgs.cn

PHP:  // 手写时间戳比较
来源：http://ge.521024.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ue.bjjhwx.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://cs.chemitech.net.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://vd.jianghongdianzi.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://jq.muxihuayi.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://df.newstarts.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://by.newstarts.cn

[P08] 处理浮点精度问题
来源：http://bf.panjiajie.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ie.yuexingan06.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wv.muxihuayi.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://af.huixinmuqiang.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ml.hnjuh.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://xa.shxzskj.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://rb.chemitech.net.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://dy.shxzukj.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ej.9csxet.cn

================================================================================
来源：http://cm.nicolike.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://yn.hahajie.cn

================================================================================
来源：http://ud.newstarts.cn

[Q01] 创建表
来源：http://yl.bookmarksfly.cn

CREATE TABLE users (
来源：http://cj.huixinmuqiang.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ip.bookmarksfly.cn

name VARCHAR(50) NOT NULL,
来源：http://lw.9csxet.cn

email VARCHAR(100) UNIQUE,
来源：http://ed.gzmigu.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hk.newstarts.cn

);
来源：http://jm.haigaiapp.cn

[Q02] 创建带外键的表
来源：http://gw.shxzukj.cn

CREATE TABLE orders (
来源：http://ci.bookmarksfly.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://so.nszjky.cn

user_id INT NOT NULL,
来源：http://hw.muxihuayi.cn

amount DECIMAL(10, 2),
来源：http://ot.nicolike.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://xn.nszjky.cn

);
来源：http://vf.newstarts.cn

[Q03] 增加列
来源：http://ph.panjiajie.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mb.nicolike.cn

[Q04] 修改列类型
来源：http://up.gzmigu.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hg.asd995.cn

[Q05] 重命名列
来源：http://gv.jctech888.com.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://fm.nicolike.cn

[Q06] 删除列
来源：http://og.nszjky.cn

ALTER TABLE users DROP COLUMN age;
来源：http://qs.yuntaijiaju.cn

[Q07] 删除表
来源：http://wm.shtwfgs.cn

DROP TABLE IF EXISTS orders;
来源：http://id.newstarts.cn

[Q08] 创建普通索引
来源：http://np.muxihuayi.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://jf.9csxet.cn

[Q09] 创建唯一索引
来源：http://pq.521024.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://er.lnxyls.cn

[Q10] 插入单行
来源：http://rp.hnjuh.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://yb.huanxung.cn

[Q11] 一次插入多行
来源：http://ty.521024.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://sq.521024.cn

[Q12] 插入后取自增 ID
来源：http://fs.9csxet.cn

INSERT INTO users (name) VALUES ('C');
来源：http://jv.szsharing.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://jx.jianghongdianzi.cn

[Q13] 忽略重复插入
来源：http://mc.huixiangedu.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://pg.hnjuh.cn

[Q14] 存在则更新（upsert）
来源：http://rz.huixiangedu.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://bq.jctech888.com.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://lw.bookmarksfly.cn

[Q15] 查询全部
来源：http://fl.szxytkj.cn

SELECT * FROM users;
来源：http://nq.yuexingan06.cn

[Q16] 查询指定列
来源：http://su.yuexingan06.cn

SELECT id, name FROM users;
来源：http://xk.wgjwhj.cn

[Q17] 条件查询
来源：http://wm.521024.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://cv.muxihuayi.cn

[Q18] 模糊匹配
来源：http://cu.newstarts.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://yk.panjiajie.cn

[Q19] 范围查询
来源：http://vx.nszjky.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://kn.szsharing.cn

[Q20] IN 列表
来源：http://rd.panjiajie.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://in.hnjuh.cn

[Q21] 空值判断
来源：http://ov.panjiajie.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://dr.szxytkj.cn

[Q22] 排序
来源：http://dq.hahajie.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://lr.bookmarksfly.cn

[Q23] 分页
来源：http://kb.bjjhwx.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ea.lnxyls.cn

[Q24] 去重
来源：http://sb.muxihuayi.cn

SELECT DISTINCT city FROM users;
来源：http://gb.hahajie.cn

[Q25] 只取前 N 条
来源：http://uc.huanxung.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://zf.huanxung.cn

[Q26] 计数
来源：http://ch.szxytkj.cn

SELECT COUNT(*) FROM users;
来源：http://tz.9csxet.cn

[Q27] 条件计数
来源：http://ve.szxytkj.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://dp.shxzskj.cn

[Q28] 求和与平均
来源：http://us.9csxet.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://zb.hahajie.cn

[Q29] 最大最小值
来源：http://jl.colortex.cn


<!-- 参考信息 -->