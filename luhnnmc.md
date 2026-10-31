代发 wailian999

JS:   [...arr].sort((a, b) => a - b)
来源：http://kr.chemitech.net.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://la.bjjhwx.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://xz.panjiajie.cn

Go:   slices.Sort(arr)
来源：http://yv.shxzskj.cn

Ruby: arr.sort
来源：http://rp.lnxyls.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://xm.panjiajie.cn

[N03] 快速排序（分治示例）
来源：http://pr.szsharing.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://xp.shxzskj.cn

PHP:  // 递归实现，或用 usort
来源：http://sf.bjjhwx.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mr.hahajie.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://dt.9csxet.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ag.haigaiapp.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hc.jianghongdianzi.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ne.shxzskj.cn

C#:   // 手写递归，或 Array.Sort
来源：http://un.huanxung.cn

[N04] 斐波那契数列
来源：http://ya.huixinmuqiang.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://lg.huixinmuqiang.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hl.bookmarksfly.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://qr.yuexingan06.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://vj.shxzukj.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://bw.9csxet.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wy.521024.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ao.szsharing.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://xs.jianghongdianzi.cn

[N05] 最大公约数
来源：http://jz.szxytkj.cn

Py:   math.gcd(a, b)
来源：http://sr.jctech888.com.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ny.9csxet.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://zf.chemitech.net.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://lb.jctech888.com.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ew.haigaiapp.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://cq.haigaiapp.cn

Ruby: a.gcd(b)
来源：http://pb.huanxung.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://id.jctech888.com.cn

[N06] 判断回文字符串
来源：http://hz.lnxyls.cn

Py:   s == s[::-1]
来源：http://di.jctech888.com.cn

PHP:  $s === strrev($s);
来源：http://jl.jctech888.com.cn

JS:   s === [...s].reverse().join("")
来源：http://ar.bookmarksfly.cn

TS:   s === [...s].reverse().join("")
来源：http://xp.huixiangedu.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://tp.jctech888.com.cn

Go:   // 双指针从两端比较
来源：http://xl.bjjhwx.cn

Ruby: s == s.reverse
来源：http://he.521024.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://wm.asd995.cn

[N07] 两数之和（返回下标）
来源：http://ki.chemitech.net.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ar.muxihuayi.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://os.colortex.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://wm.nszjky.cn

TS:   // 手写 Map<string, number>
来源：http://vf.newstarts.cn

Java: // 手写 HashMap
来源：http://gy.shxzukj.cn

Go:   // 手写 map[int]int
来源：http://jm.asd995.cn

Ruby: // 手写 Hash
来源：http://dh.hnjuh.cn

C#:   // 手写 Dictionary<int, int>
来源：http://oa.newstarts.cn

[N08] 生成全排列
来源：http://rs.shxzukj.cn

Py:   itertools.permutations(arr)
来源：http://tb.szxytkj.cn

PHP:  // 手写递归交换
来源：http://we.szsharing.cn

JS:   // 手写回溯递归
来源：http://nz.szsharing.cn

TS:   // 手写回溯递归
来源：http://iv.wgjwhj.cn

Java: // 手写回溯递归
来源：http://yu.jctech888.com.cn

Go:   // 手写回溯递归
来源：http://my.asd995.cn

Ruby: arr.permutation.to_a
来源：http://ji.521024.cn

C#:   // 手写回溯递归
来源：http://pj.nszjky.cn

[N09] 栈与队列
来源：http://ll.nicolike.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://an.wgjwhj.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://vy.521024.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://nw.panjiajie.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://nn.colortex.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://dc.huixiangedu.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ky.shxzukj.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://eo.shxzskj.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://tv.panjiajie.cn

[N10] 链表节点定义
来源：http://it.nszjky.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://zr.nicolike.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://cj.jianghongdianzi.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://vb.nicolike.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://zj.yuexingan06.cn

Java: class Node { int v; Node next; }
来源：http://ro.hnjuh.cn

Go:   type Node struct { V int; Next *Node }
来源：http://my.hnjuh.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://oq.shxzukj.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://tm.haigaiapp.cn

[N11] 二叉树中序遍历
来源：http://vo.wgjwhj.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://jm.colortex.cn

PHP:  // 手写递归函数
来源：http://ph.newstarts.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ta.szsharing.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://iw.muxihuayi.cn

Java: // 手写递归
来源：http://rq.panjiajie.cn

Go:   // 手写递归
来源：http://sw.yuntaijiaju.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ol.asd995.cn

C#:   // 手写递归
来源：http://ii.asd995.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://bx.jianghongdianzi.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://in.lnxyls.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://uy.huixinmuqiang.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://zz.gzmigu.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://gu.szxytkj.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://dl.shxzskj.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://vv.huixinmuqiang.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ou.lnxyls.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://qt.yuexingan06.cn

================================================================================
来源：http://am.nicolike.cn

O. 并发与异步
来源：http://kw.asd995.cn

================================================================================
来源：http://ge.yuntaijiaju.cn

[O01] 启动一个线程
来源：http://rj.hahajie.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ef.9csxet.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://vz.hnjuh.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://im.bookmarksfly.cn

TS:   // 同 JS
来源：http://rj.szsharing.cn

Java: new Thread(() -> f()).start()
来源：http://ab.newstarts.cn

Go:   go f()
来源：http://uh.521024.cn

Ruby: Thread.new { f }
来源：http://dc.bjjhwx.cn

C#:   Task.Run(() => F());
来源：http://zx.hahajie.cn

[O02] 使用线程池
来源：http://ed.9csxet.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.nicolike.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://md.huanxung.cn

JS:   // worker_threads 线程池
来源：http://ts.colortex.cn

TS:   // worker_threads 线程池
来源：http://kb.521024.cn

Java: Executors.newFixedThreadPool(4)
来源：http://tx.colortex.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://il.muxihuayi.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://tc.lnxyls.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ma.chemitech.net.cn

[O03] 加锁保护共享数据
来源：http://el.newstarts.cn

Py:   with lock: shared += 1
来源：http://bs.muxihuayi.cn

PHP:  // 用 flock() 做文件锁
来源：http://kf.bookmarksfly.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://zm.szsharing.cn

TS:   // 同 JS
来源：http://dz.haigaiapp.cn

Java: synchronized (this) { shared++; }
来源：http://st.521024.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ly.yuexingan06.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://wb.jianghongdianzi.cn

C#:   lock (gate) { shared++; }
来源：http://om.shtwfgs.cn

[O04] 定义异步函数并等待
来源：http://bq.huanxung.cn

Py:   async def f():⏎    await g()
来源：http://no.yuntaijiaju.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hg.haigaiapp.cn

JS:   async function f() { await g(); }
来源：http://vf.lnxyls.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://wj.nicolike.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://rw.hahajie.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://rr.jctech888.com.cn

Ruby: # 用 Fiber 或 async gem
来源：http://nn.shxzukj.cn

C#:   async Task F() { await G(); }
来源：http://sy.gzmigu.cn

[O05] 并发执行并等待全部完成
来源：http://xf.asd995.cn

Py:   asyncio.gather(*tasks)
来源：http://hu.jctech888.com.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://vp.haigaiapp.cn

JS:   await Promise.all(tasks)
来源：http://rl.jianghongdianzi.cn

TS:   await Promise.all(tasks)
来源：http://ba.bookmarksfly.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ij.huixiangedu.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://nk.chemitech.net.cn

Ruby: threads.map(&:join)
来源：http://ox.gzmigu.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://cg.hahajie.cn

[O06] 使用进程池
来源：http://zq.nszjky.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ef.huanxung.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://dj.bookmarksfly.cn

JS:   // child_process / cluster 模块
来源：http://sj.huixiangedu.cn

TS:   // child_process / cluster 模块
来源：http://qc.jctech888.com.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ve.szxytkj.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://gy.huanxung.cn

Ruby: // fork 块
来源：http://jj.shxzukj.cn

C#:   Parallel.For
来源：http://on.gzmigu.cn

================================================================================
来源：http://fm.szxytkj.cn

P. 常用工具函数
来源：http://bx.colortex.cn

================================================================================
来源：http://pu.nicolike.cn

[P01] 生成 UUID
来源：http://zx.jianghongdianzi.cn

Py:   str(uuid.uuid4())
来源：http://nb.hnjuh.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://js.521024.cn

JS:   crypto.randomUUID()
来源：http://ue.panjiajie.cn

TS:   crypto.randomUUID()
来源：http://jp.521024.cn

Java: UUID.randomUUID().toString()
来源：http://ye.hahajie.cn

Go:   // 用 github.com/google/uuid
来源：http://gn.bjjhwx.cn

Ruby: SecureRandom.uuid
来源：http://je.huanxung.cn

C#:   Guid.NewGuid().ToString()
来源：http://ay.huixinmuqiang.cn

[P02] MD5 / SHA256 摘要
来源：http://ee.asd995.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hg.asd995.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://ga.newstarts.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://me.jctech888.com.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://dw.hahajie.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ru.jctech888.com.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://xg.huanxung.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://pn.chemitech.net.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://df.szsharing.cn

[P03] 生成短随机字符串
来源：http://nd.nszjky.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://kr.wgjwhj.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://bk.newstarts.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://yq.chemitech.net.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://cu.chemitech.net.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://dp.huixiangedu.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://of.shxzskj.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://ls.colortex.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://tq.szsharing.cn

[P04] 求长度
来源：http://fm.521024.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hm.jianghongdianzi.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://vp.huixinmuqiang.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://yt.yuntaijiaju.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://br.colortex.cn

Java: list.size();  map.size();  s.length()
来源：http://th.shxzskj.cn

Go:   len(arr);  len(m)
来源：http://kv.shxzskj.cn

Ruby: x.length;  x.size
来源：http://rc.chemitech.net.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://iu.521024.cn

[P05] 判断两个对象内容是否相等
来源：http://gi.huanxung.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://tg.huixinmuqiang.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ib.wgjwhj.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wv.jianghongdianzi.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://pn.hahajie.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://gt.huixinmuqiang.cn

Go:   reflect.DeepEqual(a, b)
来源：http://qe.wgjwhj.cn

Ruby: a == b
来源：http://qv.muxihuayi.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://yc.lnxyls.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://vr.jianghongdianzi.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://gq.colortex.cn

PHP:  if (empty($x)) {}
来源：http://ip.shtwfgs.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://nd.shtwfgs.cn

TS:   if (x == null) {}
来源：http://lz.newstarts.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://je.yuntaijiaju.cn

Go:   if x == nil {}
来源：http://rh.muxihuayi.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://cx.szsharing.cn

C#:   if (x is null) {}
来源：http://tm.hahajie.cn

[P07] 防抖与节流
来源：http://cy.nszjky.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://fv.chemitech.net.cn

PHP:  // 手写时间戳比较
来源：http://yc.chemitech.net.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qr.yuexingan06.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://jf.huixinmuqiang.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hi.hahajie.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://bm.colortex.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://rs.bookmarksfly.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://la.jctech888.com.cn

[P08] 处理浮点精度问题
来源：http://ii.panjiajie.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ba.yuntaijiaju.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://cg.newstarts.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://fj.shxzukj.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://cp.newstarts.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://lz.521024.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ba.bjjhwx.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://vx.muxihuayi.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://bw.huanxung.cn

================================================================================
来源：http://vc.shtwfgs.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mq.bookmarksfly.cn

================================================================================
来源：http://th.hnjuh.cn

[Q01] 创建表
来源：http://wn.yuexingan06.cn

CREATE TABLE users (
来源：http://kd.szsharing.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mf.nicolike.cn

name VARCHAR(50) NOT NULL,
来源：http://ou.szxytkj.cn

email VARCHAR(100) UNIQUE,
来源：http://rr.yuntaijiaju.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ns.colortex.cn

);
来源：http://ce.haigaiapp.cn

[Q02] 创建带外键的表
来源：http://sf.bjjhwx.cn

CREATE TABLE orders (
来源：http://ml.bjjhwx.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ei.panjiajie.cn

user_id INT NOT NULL,
来源：http://ks.nicolike.cn

amount DECIMAL(10, 2),
来源：http://cv.shtwfgs.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://vd.bookmarksfly.cn

);
来源：http://gw.szsharing.cn

[Q03] 增加列
来源：http://wx.shxzskj.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://gj.nicolike.cn

[Q04] 修改列类型
来源：http://ad.szsharing.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://sm.nicolike.cn

[Q05] 重命名列
来源：http://uz.9csxet.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wb.hahajie.cn

[Q06] 删除列
来源：http://th.jctech888.com.cn

ALTER TABLE users DROP COLUMN age;
来源：http://ba.asd995.cn

[Q07] 删除表
来源：http://an.521024.cn

DROP TABLE IF EXISTS orders;
来源：http://ag.hnjuh.cn

[Q08] 创建普通索引
来源：http://zb.hnjuh.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://yx.lnxyls.cn

[Q09] 创建唯一索引
来源：http://mj.shxzukj.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://sa.jianghongdianzi.cn

[Q10] 插入单行
来源：http://rl.hahajie.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://aw.bookmarksfly.cn

[Q11] 一次插入多行
来源：http://qd.haigaiapp.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://fk.huixiangedu.cn

[Q12] 插入后取自增 ID
来源：http://ld.shtwfgs.cn

INSERT INTO users (name) VALUES ('C');
来源：http://ss.wgjwhj.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mk.newstarts.cn

[Q13] 忽略重复插入
来源：http://lp.bookmarksfly.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://oc.yuntaijiaju.cn

[Q14] 存在则更新（upsert）
来源：http://az.bjjhwx.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://sj.9csxet.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ln.szxytkj.cn

[Q15] 查询全部
来源：http://do.9csxet.cn

SELECT * FROM users;
来源：http://ey.huixinmuqiang.cn

[Q16] 查询指定列
来源：http://qq.yuexingan06.cn

SELECT id, name FROM users;
来源：http://tl.jianghongdianzi.cn

[Q17] 条件查询
来源：http://lt.asd995.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://uu.huanxung.cn

[Q18] 模糊匹配
来源：http://cd.shxzukj.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://xp.hahajie.cn

[Q19] 范围查询
来源：http://to.bjjhwx.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://pv.szxytkj.cn

[Q20] IN 列表
来源：http://bf.newstarts.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://xi.hnjuh.cn

[Q21] 空值判断
来源：http://px.hahajie.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://um.lnxyls.cn

[Q22] 排序
来源：http://jf.wgjwhj.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://zc.haigaiapp.cn

[Q23] 分页
来源：http://kb.jianghongdianzi.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://lm.shxzskj.cn

[Q24] 去重
来源：http://fl.9csxet.cn

SELECT DISTINCT city FROM users;
来源：http://lq.shxzukj.cn

[Q25] 只取前 N 条
来源：http://wj.panjiajie.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://lc.bookmarksfly.cn

[Q26] 计数
来源：http://fp.bookmarksfly.cn

SELECT COUNT(*) FROM users;
来源：http://aq.szsharing.cn

[Q27] 条件计数
来源：http://cq.haigaiapp.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ck.521024.cn

[Q28] 求和与平均
来源：http://wt.shxzukj.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wn.wgjwhj.cn

[Q29] 最大最小值
来源：http://ge.bookmarksfly.cn


<!-- 参考信息 -->