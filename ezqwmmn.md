代发 wailian999

C#:   Array.BinarySearch(arr, x)
来源：http://tj.shxzukj.cn

[N02] 排序（工程实践用内置实现）
来源：http://gp.shtwfgs.cn

Py:   sorted(arr);  arr.sort()
来源：http://nn.521024.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://lh.szsharing.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://ig.nszjky.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://gv.szsharing.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://gd.nicolike.cn

Go:   slices.Sort(arr)
来源：http://tm.gzmigu.cn

Ruby: arr.sort
来源：http://zq.panjiajie.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://eu.huixiangedu.cn

[N03] 快速排序（分治示例）
来源：http://yn.colortex.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://jp.huanxung.cn

PHP:  // 递归实现，或用 usort
来源：http://ma.szxytkj.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mt.szxytkj.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://gp.asd995.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://kj.lnxyls.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://oi.jctech888.com.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hm.gzmigu.cn

C#:   // 手写递归，或 Array.Sort
来源：http://xh.szsharing.cn

[N04] 斐波那契数列
来源：http://sq.yuntaijiaju.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://gl.muxihuayi.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://op.jctech888.com.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://sd.szxytkj.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ne.jctech888.com.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://lf.asd995.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://cm.gzmigu.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://xz.lnxyls.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ox.hnjuh.cn

[N05] 最大公约数
来源：http://bj.huixinmuqiang.cn

Py:   math.gcd(a, b)
来源：http://uf.huanxung.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hm.bjjhwx.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://yy.hnjuh.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://rq.shtwfgs.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://uv.szsharing.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mw.yuexingan06.cn

Ruby: a.gcd(b)
来源：http://fh.gzmigu.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://jd.jianghongdianzi.cn

[N06] 判断回文字符串
来源：http://yq.chemitech.net.cn

Py:   s == s[::-1]
来源：http://io.bookmarksfly.cn

PHP:  $s === strrev($s);
来源：http://yv.bookmarksfly.cn

JS:   s === [...s].reverse().join("")
来源：http://gx.hahajie.cn

TS:   s === [...s].reverse().join("")
来源：http://ih.bookmarksfly.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://dy.colortex.cn

Go:   // 双指针从两端比较
来源：http://sl.nicolike.cn

Ruby: s == s.reverse
来源：http://ny.szxytkj.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://wz.yuntaijiaju.cn

[N07] 两数之和（返回下标）
来源：http://gs.nicolike.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://kn.shtwfgs.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://fh.521024.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://ef.asd995.cn

TS:   // 手写 Map<string, number>
来源：http://vp.huixinmuqiang.cn

Java: // 手写 HashMap
来源：http://ck.bjjhwx.cn

Go:   // 手写 map[int]int
来源：http://et.szsharing.cn

Ruby: // 手写 Hash
来源：http://mr.colortex.cn

C#:   // 手写 Dictionary<int, int>
来源：http://zd.wgjwhj.cn

[N08] 生成全排列
来源：http://tg.szxytkj.cn

Py:   itertools.permutations(arr)
来源：http://dg.muxihuayi.cn

PHP:  // 手写递归交换
来源：http://fs.nicolike.cn

JS:   // 手写回溯递归
来源：http://jq.huixiangedu.cn

TS:   // 手写回溯递归
来源：http://hs.yuntaijiaju.cn

Java: // 手写回溯递归
来源：http://pt.shxzskj.cn

Go:   // 手写回溯递归
来源：http://mi.hahajie.cn

Ruby: arr.permutation.to_a
来源：http://zv.huixinmuqiang.cn

C#:   // 手写回溯递归
来源：http://ub.szsharing.cn

[N09] 栈与队列
来源：http://qr.nszjky.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://tz.9csxet.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://kv.shtwfgs.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://rd.jctech888.com.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://fe.gzmigu.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://xg.szxytkj.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hj.szsharing.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://pa.jctech888.com.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://um.colortex.cn

[N10] 链表节点定义
来源：http://eg.hnjuh.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://re.hnjuh.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://ku.nicolike.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://sn.jianghongdianzi.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mu.yuexingan06.cn

Java: class Node { int v; Node next; }
来源：http://mf.shxzukj.cn

Go:   type Node struct { V int; Next *Node }
来源：http://xv.nicolike.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://ih.yuexingan06.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://gq.hahajie.cn

[N11] 二叉树中序遍历
来源：http://kk.panjiajie.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://al.jctech888.com.cn

PHP:  // 手写递归函数
来源：http://sx.jianghongdianzi.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://px.huanxung.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://dv.jianghongdianzi.cn

Java: // 手写递归
来源：http://vs.wgjwhj.cn

Go:   // 手写递归
来源：http://kb.colortex.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://es.chemitech.net.cn

C#:   // 手写递归
来源：http://wj.bjjhwx.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://jk.gzmigu.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://zh.huanxung.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://va.hnjuh.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://vf.huanxung.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://kt.newstarts.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://bg.bookmarksfly.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mu.newstarts.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://no.szsharing.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wq.nszjky.cn

================================================================================
来源：http://kw.szsharing.cn

O. 并发与异步
来源：http://qa.shtwfgs.cn

================================================================================
来源：http://aw.nszjky.cn

[O01] 启动一个线程
来源：http://ba.bookmarksfly.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ge.szsharing.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://sr.lnxyls.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ya.bjjhwx.cn

TS:   // 同 JS
来源：http://lr.wgjwhj.cn

Java: new Thread(() -> f()).start()
来源：http://hc.huanxung.cn

Go:   go f()
来源：http://ni.nicolike.cn

Ruby: Thread.new { f }
来源：http://gh.asd995.cn

C#:   Task.Run(() => F());
来源：http://ho.chemitech.net.cn

[O02] 使用线程池
来源：http://dx.jianghongdianzi.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://em.shxzukj.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://xj.huixiangedu.cn

JS:   // worker_threads 线程池
来源：http://yb.newstarts.cn

TS:   // worker_threads 线程池
来源：http://rk.shxzukj.cn

Java: Executors.newFixedThreadPool(4)
来源：http://px.szxytkj.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ma.shtwfgs.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://tm.wgjwhj.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ql.521024.cn

[O03] 加锁保护共享数据
来源：http://ry.colortex.cn

Py:   with lock: shared += 1
来源：http://in.chemitech.net.cn

PHP:  // 用 flock() 做文件锁
来源：http://yz.asd995.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://tj.szxytkj.cn

TS:   // 同 JS
来源：http://ua.haigaiapp.cn

Java: synchronized (this) { shared++; }
来源：http://nl.muxihuayi.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://oj.asd995.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://gv.gzmigu.cn

C#:   lock (gate) { shared++; }
来源：http://ra.colortex.cn

[O04] 定义异步函数并等待
来源：http://ik.newstarts.cn

Py:   async def f():⏎    await g()
来源：http://yq.nszjky.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://tu.newstarts.cn

JS:   async function f() { await g(); }
来源：http://dz.wgjwhj.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://iz.huixinmuqiang.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://tt.huanxung.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://eo.bookmarksfly.cn

Ruby: # 用 Fiber 或 async gem
来源：http://nh.szsharing.cn

C#:   async Task F() { await G(); }
来源：http://yb.gzmigu.cn

[O05] 并发执行并等待全部完成
来源：http://yp.bjjhwx.cn

Py:   asyncio.gather(*tasks)
来源：http://lq.lnxyls.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://kz.szxytkj.cn

JS:   await Promise.all(tasks)
来源：http://no.asd995.cn

TS:   await Promise.all(tasks)
来源：http://bs.shxzskj.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://js.szsharing.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://at.colortex.cn

Ruby: threads.map(&:join)
来源：http://ym.jianghongdianzi.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://tj.lnxyls.cn

[O06] 使用进程池
来源：http://jt.shxzukj.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://my.shtwfgs.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://qm.chemitech.net.cn

JS:   // child_process / cluster 模块
来源：http://jn.shxzskj.cn

TS:   // child_process / cluster 模块
来源：http://te.yuexingan06.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hk.nszjky.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://kp.bookmarksfly.cn

Ruby: // fork 块
来源：http://fl.chemitech.net.cn

C#:   Parallel.For
来源：http://tq.hnjuh.cn

================================================================================
来源：http://pd.521024.cn

P. 常用工具函数
来源：http://wx.yuntaijiaju.cn

================================================================================
来源：http://eb.chemitech.net.cn

[P01] 生成 UUID
来源：http://po.shxzukj.cn

Py:   str(uuid.uuid4())
来源：http://qv.panjiajie.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://qd.shxzskj.cn

JS:   crypto.randomUUID()
来源：http://hf.shxzskj.cn

TS:   crypto.randomUUID()
来源：http://do.huanxung.cn

Java: UUID.randomUUID().toString()
来源：http://yr.hnjuh.cn

Go:   // 用 github.com/google/uuid
来源：http://yg.jctech888.com.cn

Ruby: SecureRandom.uuid
来源：http://ru.huixinmuqiang.cn

C#:   Guid.NewGuid().ToString()
来源：http://wq.panjiajie.cn

[P02] MD5 / SHA256 摘要
来源：http://gl.gzmigu.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ct.nszjky.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://uw.wgjwhj.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://zi.newstarts.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://aj.lnxyls.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://zl.haigaiapp.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://fg.huixiangedu.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ul.521024.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://uh.hahajie.cn

[P03] 生成短随机字符串
来源：http://xk.haigaiapp.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ji.9csxet.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://rz.huanxung.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://gd.huanxung.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://xx.nszjky.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://xq.nicolike.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://nq.muxihuayi.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://gr.wgjwhj.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://td.hnjuh.cn

[P04] 求长度
来源：http://gw.yuntaijiaju.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://dl.wgjwhj.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://pq.shtwfgs.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://bt.shxzukj.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://fc.szxytkj.cn

Java: list.size();  map.size();  s.length()
来源：http://ca.nicolike.cn

Go:   len(arr);  len(m)
来源：http://tt.szxytkj.cn

Ruby: x.length;  x.size
来源：http://eb.hnjuh.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://pz.szsharing.cn

[P05] 判断两个对象内容是否相等
来源：http://gn.colortex.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://dw.bjjhwx.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://xq.huixiangedu.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://na.yuntaijiaju.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://to.yuexingan06.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://rr.shxzskj.cn

Go:   reflect.DeepEqual(a, b)
来源：http://zl.huanxung.cn

Ruby: a == b
来源：http://xb.hahajie.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://rg.asd995.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://qg.bjjhwx.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://xb.huanxung.cn

PHP:  if (empty($x)) {}
来源：http://px.9csxet.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://rn.szxytkj.cn

TS:   if (x == null) {}
来源：http://dx.nicolike.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://tb.panjiajie.cn

Go:   if x == nil {}
来源：http://vh.bjjhwx.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ap.colortex.cn

C#:   if (x is null) {}
来源：http://xg.huixinmuqiang.cn

[P07] 防抖与节流
来源：http://wy.panjiajie.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mu.chemitech.net.cn

PHP:  // 手写时间戳比较
来源：http://zc.hnjuh.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xg.newstarts.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://bg.bjjhwx.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://kw.yuntaijiaju.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://tp.shxzskj.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://jg.huanxung.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://kx.nszjky.cn

[P08] 处理浮点精度问题
来源：http://mo.nicolike.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ch.lnxyls.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://el.nszjky.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://dq.wgjwhj.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://os.shtwfgs.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://xo.hnjuh.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://fm.huanxung.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ci.szxytkj.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://bt.huixiangedu.cn

================================================================================
来源：http://si.huixinmuqiang.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://eh.jianghongdianzi.cn

================================================================================
来源：http://pm.asd995.cn

[Q01] 创建表
来源：http://dr.szsharing.cn

CREATE TABLE users (
来源：http://en.jctech888.com.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ti.colortex.cn

name VARCHAR(50) NOT NULL,
来源：http://sx.colortex.cn

email VARCHAR(100) UNIQUE,
来源：http://xk.panjiajie.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://co.521024.cn

);
来源：http://dr.gzmigu.cn

[Q02] 创建带外键的表
来源：http://ce.colortex.cn

CREATE TABLE orders (
来源：http://jj.haigaiapp.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://nt.shxzukj.cn

user_id INT NOT NULL,
来源：http://zb.asd995.cn

amount DECIMAL(10, 2),
来源：http://wl.huixinmuqiang.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://qb.haigaiapp.cn

);
来源：http://ab.yuexingan06.cn

[Q03] 增加列
来源：http://jq.haigaiapp.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://cz.muxihuayi.cn

[Q04] 修改列类型
来源：http://ph.huixiangedu.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://jf.nicolike.cn

[Q05] 重命名列
来源：http://gf.szxytkj.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://br.jianghongdianzi.cn

[Q06] 删除列
来源：http://bs.huixiangedu.cn

ALTER TABLE users DROP COLUMN age;
来源：http://ev.jctech888.com.cn

[Q07] 删除表
来源：http://kc.huanxung.cn

DROP TABLE IF EXISTS orders;
来源：http://ev.muxihuayi.cn

[Q08] 创建普通索引
来源：http://pp.huanxung.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://bh.nszjky.cn

[Q09] 创建唯一索引
来源：http://xw.hnjuh.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ko.muxihuayi.cn

[Q10] 插入单行
来源：http://zg.nicolike.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://py.9csxet.cn

[Q11] 一次插入多行
来源：http://xw.huanxung.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wb.shxzskj.cn

[Q12] 插入后取自增 ID
来源：http://ya.chemitech.net.cn

INSERT INTO users (name) VALUES ('C');
来源：http://zm.panjiajie.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ce.panjiajie.cn

[Q13] 忽略重复插入
来源：http://og.shxzskj.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://oa.wgjwhj.cn

[Q14] 存在则更新（upsert）
来源：http://wh.nszjky.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ho.huixinmuqiang.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://xq.haigaiapp.cn

[Q15] 查询全部
来源：http://hk.bjjhwx.cn

SELECT * FROM users;
来源：http://os.huixiangedu.cn

[Q16] 查询指定列
来源：http://yp.9csxet.cn

SELECT id, name FROM users;
来源：http://qt.nicolike.cn

[Q17] 条件查询
来源：http://ui.hahajie.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://cv.huixiangedu.cn

[Q18] 模糊匹配
来源：http://dk.lnxyls.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ov.haigaiapp.cn

[Q19] 范围查询
来源：http://pa.nicolike.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://bi.chemitech.net.cn

[Q20] IN 列表
来源：http://xu.shtwfgs.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://rb.wgjwhj.cn

[Q21] 空值判断
来源：http://ag.bjjhwx.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://he.9csxet.cn

[Q22] 排序
来源：http://us.9csxet.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://fj.jianghongdianzi.cn

[Q23] 分页
来源：http://gi.haigaiapp.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ti.huixiangedu.cn

[Q24] 去重
来源：http://xo.asd995.cn

SELECT DISTINCT city FROM users;
来源：http://vg.panjiajie.cn

[Q25] 只取前 N 条
来源：http://tb.gzmigu.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://am.haigaiapp.cn

[Q26] 计数
来源：http://di.bjjhwx.cn

SELECT COUNT(*) FROM users;
来源：http://kt.shxzukj.cn

[Q27] 条件计数
来源：http://cq.haigaiapp.cn


<!-- 参考信息 -->