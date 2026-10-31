代发 wailian999

JS:   [...arr].sort((a, b) => a - b)
来源：http://wy.haigaiapp.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://lt.9csxet.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://jr.panjiajie.cn

Go:   slices.Sort(arr)
来源：http://eh.newstarts.cn

Ruby: arr.sort
来源：http://qq.shxzukj.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://yw.nicolike.cn

[N03] 快速排序（分治示例）
来源：http://fx.521024.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://on.shxzukj.cn

PHP:  // 递归实现，或用 usort
来源：http://fl.yuexingan06.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://zl.asd995.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://tv.szsharing.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://tf.nicolike.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://zy.bookmarksfly.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://gg.panjiajie.cn

C#:   // 手写递归，或 Array.Sort
来源：http://wg.asd995.cn

[N04] 斐波那契数列
来源：http://hl.jianghongdianzi.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://pd.shtwfgs.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://vp.huixinmuqiang.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://fk.shxzukj.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://oo.wgjwhj.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ud.gzmigu.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://rz.shtwfgs.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://bb.gzmigu.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://kk.jianghongdianzi.cn

[N05] 最大公约数
来源：http://ol.jctech888.com.cn

Py:   math.gcd(a, b)
来源：http://ww.yuexingan06.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://gz.yuexingan06.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://vs.shxzskj.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://yy.colortex.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mh.bookmarksfly.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://rv.huanxung.cn

Ruby: a.gcd(b)
来源：http://kq.gzmigu.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://rn.wgjwhj.cn

[N06] 判断回文字符串
来源：http://zs.huixinmuqiang.cn

Py:   s == s[::-1]
来源：http://fu.yuntaijiaju.cn

PHP:  $s === strrev($s);
来源：http://qr.shxzskj.cn

JS:   s === [...s].reverse().join("")
来源：http://ey.9csxet.cn

TS:   s === [...s].reverse().join("")
来源：http://id.nicolike.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://vi.asd995.cn

Go:   // 双指针从两端比较
来源：http://qb.gzmigu.cn

Ruby: s == s.reverse
来源：http://un.huixiangedu.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://fj.wgjwhj.cn

[N07] 两数之和（返回下标）
来源：http://nh.jianghongdianzi.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://vc.nicolike.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://kg.shtwfgs.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://rb.wgjwhj.cn

TS:   // 手写 Map<string, number>
来源：http://mr.nicolike.cn

Java: // 手写 HashMap
来源：http://hb.panjiajie.cn

Go:   // 手写 map[int]int
来源：http://ac.yuexingan06.cn

Ruby: // 手写 Hash
来源：http://wf.bookmarksfly.cn

C#:   // 手写 Dictionary<int, int>
来源：http://ur.jctech888.com.cn

[N08] 生成全排列
来源：http://mg.yuexingan06.cn

Py:   itertools.permutations(arr)
来源：http://yk.chemitech.net.cn

PHP:  // 手写递归交换
来源：http://uh.wgjwhj.cn

JS:   // 手写回溯递归
来源：http://rp.szsharing.cn

TS:   // 手写回溯递归
来源：http://dz.chemitech.net.cn

Java: // 手写回溯递归
来源：http://eg.hnjuh.cn

Go:   // 手写回溯递归
来源：http://lq.nszjky.cn

Ruby: arr.permutation.to_a
来源：http://bw.lnxyls.cn

C#:   // 手写回溯递归
来源：http://ml.szsharing.cn

[N09] 栈与队列
来源：http://og.gzmigu.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://xp.bjjhwx.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://dx.szsharing.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://fq.yuntaijiaju.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://fi.newstarts.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://xr.lnxyls.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://yb.szsharing.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://nl.bjjhwx.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wi.colortex.cn

[N10] 链表节点定义
来源：http://mh.gzmigu.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ce.muxihuayi.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://jf.shxzukj.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://vt.wgjwhj.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://fg.huixiangedu.cn

Java: class Node { int v; Node next; }
来源：http://xr.bookmarksfly.cn

Go:   type Node struct { V int; Next *Node }
来源：http://os.gzmigu.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://vk.521024.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://ww.chemitech.net.cn

[N11] 二叉树中序遍历
来源：http://rk.asd995.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ps.wgjwhj.cn

PHP:  // 手写递归函数
来源：http://ab.panjiajie.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://tt.haigaiapp.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://yt.yuexingan06.cn

Java: // 手写递归
来源：http://mf.huixiangedu.cn

Go:   // 手写递归
来源：http://ok.szxytkj.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://oq.shxzukj.cn

C#:   // 手写递归
来源：http://jr.panjiajie.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://fh.hahajie.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mk.bookmarksfly.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://lt.hnjuh.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mp.panjiajie.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://nt.nszjky.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://sc.nszjky.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://yy.yuexingan06.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://en.huixinmuqiang.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://go.shtwfgs.cn

================================================================================
来源：http://gy.jctech888.com.cn

O. 并发与异步
来源：http://dq.szsharing.cn

================================================================================
来源：http://oh.gzmigu.cn

[O01] 启动一个线程
来源：http://sz.jctech888.com.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://oz.wgjwhj.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://dr.haigaiapp.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ld.colortex.cn

TS:   // 同 JS
来源：http://nl.shxzukj.cn

Java: new Thread(() -> f()).start()
来源：http://ck.yuexingan06.cn

Go:   go f()
来源：http://ws.szxytkj.cn

Ruby: Thread.new { f }
来源：http://re.muxihuayi.cn

C#:   Task.Run(() => F());
来源：http://ao.szsharing.cn

[O02] 使用线程池
来源：http://eh.szxytkj.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://fn.asd995.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://xl.huixiangedu.cn

JS:   // worker_threads 线程池
来源：http://lf.colortex.cn

TS:   // worker_threads 线程池
来源：http://ke.colortex.cn

Java: Executors.newFixedThreadPool(4)
来源：http://sm.wgjwhj.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://yw.panjiajie.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://bf.nicolike.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://le.hnjuh.cn

[O03] 加锁保护共享数据
来源：http://lz.bjjhwx.cn

Py:   with lock: shared += 1
来源：http://ar.haigaiapp.cn

PHP:  // 用 flock() 做文件锁
来源：http://gf.gzmigu.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://yf.hahajie.cn

TS:   // 同 JS
来源：http://ye.nicolike.cn

Java: synchronized (this) { shared++; }
来源：http://lp.bjjhwx.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://iq.yuntaijiaju.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://fp.haigaiapp.cn

C#:   lock (gate) { shared++; }
来源：http://qt.newstarts.cn

[O04] 定义异步函数并等待
来源：http://yt.hahajie.cn

Py:   async def f():⏎    await g()
来源：http://mu.521024.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://vo.bookmarksfly.cn

JS:   async function f() { await g(); }
来源：http://jg.bjjhwx.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://yw.huixiangedu.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://sf.szsharing.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ux.asd995.cn

Ruby: # 用 Fiber 或 async gem
来源：http://wo.wgjwhj.cn

C#:   async Task F() { await G(); }
来源：http://yg.gzmigu.cn

[O05] 并发执行并等待全部完成
来源：http://qm.hnjuh.cn

Py:   asyncio.gather(*tasks)
来源：http://sp.huixiangedu.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ba.9csxet.cn

JS:   await Promise.all(tasks)
来源：http://cn.asd995.cn

TS:   await Promise.all(tasks)
来源：http://iv.lnxyls.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://bn.yuexingan06.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ys.yuntaijiaju.cn

Ruby: threads.map(&:join)
来源：http://yh.9csxet.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://zj.haigaiapp.cn

[O06] 使用进程池
来源：http://vj.muxihuayi.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ph.colortex.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://xh.hnjuh.cn

JS:   // child_process / cluster 模块
来源：http://wv.shxzukj.cn

TS:   // child_process / cluster 模块
来源：http://zz.huanxung.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://uk.wgjwhj.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://dn.newstarts.cn

Ruby: // fork 块
来源：http://bj.haigaiapp.cn

C#:   Parallel.For
来源：http://lm.shtwfgs.cn

================================================================================
来源：http://xg.shxzukj.cn

P. 常用工具函数
来源：http://ph.panjiajie.cn

================================================================================
来源：http://lk.bookmarksfly.cn

[P01] 生成 UUID
来源：http://ek.haigaiapp.cn

Py:   str(uuid.uuid4())
来源：http://jo.9csxet.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://lc.lnxyls.cn

JS:   crypto.randomUUID()
来源：http://ht.hahajie.cn

TS:   crypto.randomUUID()
来源：http://bg.huixinmuqiang.cn

Java: UUID.randomUUID().toString()
来源：http://iv.szxytkj.cn

Go:   // 用 github.com/google/uuid
来源：http://ix.newstarts.cn

Ruby: SecureRandom.uuid
来源：http://uo.wgjwhj.cn

C#:   Guid.NewGuid().ToString()
来源：http://sf.nszjky.cn

[P02] MD5 / SHA256 摘要
来源：http://jz.bjjhwx.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://bo.yuexingan06.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://qn.bookmarksfly.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ev.panjiajie.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://gm.shxzskj.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://gb.szsharing.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://gs.muxihuayi.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hh.huixiangedu.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://pi.haigaiapp.cn

[P03] 生成短随机字符串
来源：http://st.chemitech.net.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://dd.jianghongdianzi.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ar.chemitech.net.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://jk.gzmigu.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://gi.jctech888.com.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://fp.chemitech.net.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://yr.huixinmuqiang.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://va.jianghongdianzi.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://zt.nicolike.cn

[P04] 求长度
来源：http://el.newstarts.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://or.haigaiapp.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://lz.521024.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wk.gzmigu.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://fj.jianghongdianzi.cn

Java: list.size();  map.size();  s.length()
来源：http://jm.muxihuayi.cn

Go:   len(arr);  len(m)
来源：http://iz.huanxung.cn

Ruby: x.length;  x.size
来源：http://ai.szxytkj.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://gu.jctech888.com.cn

[P05] 判断两个对象内容是否相等
来源：http://xx.colortex.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://gq.9csxet.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://lu.gzmigu.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://he.huixinmuqiang.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mm.shtwfgs.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://qg.shxzukj.cn

Go:   reflect.DeepEqual(a, b)
来源：http://xx.colortex.cn

Ruby: a == b
来源：http://ll.haigaiapp.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://yy.chemitech.net.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://vk.chemitech.net.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://fa.nicolike.cn

PHP:  if (empty($x)) {}
来源：http://nj.jctech888.com.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ba.bjjhwx.cn

TS:   if (x == null) {}
来源：http://ue.bookmarksfly.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://cn.jctech888.com.cn

Go:   if x == nil {}
来源：http://en.jianghongdianzi.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ui.9csxet.cn

C#:   if (x is null) {}
来源：http://tb.bjjhwx.cn

[P07] 防抖与节流
来源：http://fm.huixinmuqiang.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://pa.jctech888.com.cn

PHP:  // 手写时间戳比较
来源：http://kd.521024.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hx.haigaiapp.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ye.shxzukj.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hs.hnjuh.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://cx.jctech888.com.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://ue.nszjky.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://bv.yuntaijiaju.cn

[P08] 处理浮点精度问题
来源：http://vv.jctech888.com.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://pp.lnxyls.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://kw.wgjwhj.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://kh.hnjuh.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://zu.huanxung.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://rl.muxihuayi.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://si.bjjhwx.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://cf.521024.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://rd.bookmarksfly.cn

================================================================================
来源：http://lr.shtwfgs.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://dk.jctech888.com.cn

================================================================================
来源：http://yh.huixiangedu.cn

[Q01] 创建表
来源：http://se.9csxet.cn

CREATE TABLE users (
来源：http://ff.jianghongdianzi.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ad.szxytkj.cn

name VARCHAR(50) NOT NULL,
来源：http://wh.jctech888.com.cn

email VARCHAR(100) UNIQUE,
来源：http://qd.hnjuh.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://qt.hahajie.cn

);
来源：http://jd.huanxung.cn

[Q02] 创建带外键的表
来源：http://js.muxihuayi.cn

CREATE TABLE orders (
来源：http://hh.huixiangedu.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://do.shxzskj.cn

user_id INT NOT NULL,
来源：http://zn.wgjwhj.cn

amount DECIMAL(10, 2),
来源：http://cm.asd995.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://fn.asd995.cn

);
来源：http://zl.shtwfgs.cn

[Q03] 增加列
来源：http://ze.szxytkj.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://gr.521024.cn

[Q04] 修改列类型
来源：http://ax.521024.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://al.muxihuayi.cn

[Q05] 重命名列
来源：http://rq.asd995.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://dc.nszjky.cn

[Q06] 删除列
来源：http://gk.hahajie.cn

ALTER TABLE users DROP COLUMN age;
来源：http://pp.nszjky.cn

[Q07] 删除表
来源：http://oo.shxzukj.cn

DROP TABLE IF EXISTS orders;
来源：http://di.hahajie.cn

[Q08] 创建普通索引
来源：http://li.lnxyls.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://hy.gzmigu.cn

[Q09] 创建唯一索引
来源：http://xc.shxzskj.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ve.jctech888.com.cn

[Q10] 插入单行
来源：http://hh.nszjky.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ge.chemitech.net.cn

[Q11] 一次插入多行
来源：http://li.asd995.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://yh.huixiangedu.cn

[Q12] 插入后取自增 ID
来源：http://hv.asd995.cn

INSERT INTO users (name) VALUES ('C');
来源：http://nw.newstarts.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://rq.bjjhwx.cn

[Q13] 忽略重复插入
来源：http://lb.nszjky.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://vi.hahajie.cn

[Q14] 存在则更新（upsert）
来源：http://yj.szxytkj.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ew.huanxung.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://by.shxzukj.cn

[Q15] 查询全部
来源：http://wj.nszjky.cn

SELECT * FROM users;
来源：http://ow.yuntaijiaju.cn

[Q16] 查询指定列
来源：http://sh.jianghongdianzi.cn

SELECT id, name FROM users;
来源：http://jr.9csxet.cn

[Q17] 条件查询
来源：http://vd.nszjky.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://tg.521024.cn

[Q18] 模糊匹配
来源：http://kb.yuexingan06.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://de.wgjwhj.cn

[Q19] 范围查询
来源：http://hb.szxytkj.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://tc.chemitech.net.cn

[Q20] IN 列表
来源：http://bd.shxzukj.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mb.newstarts.cn

[Q21] 空值判断
来源：http://sc.huixinmuqiang.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://jo.hahajie.cn

[Q22] 排序
来源：http://dk.nicolike.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://lw.bjjhwx.cn

[Q23] 分页
来源：http://vo.wgjwhj.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://gd.shtwfgs.cn

[Q24] 去重
来源：http://tn.jianghongdianzi.cn

SELECT DISTINCT city FROM users;
来源：http://cv.haigaiapp.cn

[Q25] 只取前 N 条
来源：http://vu.huanxung.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ui.huixiangedu.cn

[Q26] 计数
来源：http://ht.huixiangedu.cn

SELECT COUNT(*) FROM users;
来源：http://io.jctech888.com.cn

[Q27] 条件计数
来源：http://jd.9csxet.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://rq.shxzukj.cn

[Q28] 求和与平均
来源：http://og.gzmigu.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://qg.newstarts.cn

[Q29] 最大最小值
来源：http://fc.wgjwhj.cn


<!-- 参考信息 -->