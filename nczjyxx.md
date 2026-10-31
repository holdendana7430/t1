代发 wailian999

JS:   [...arr].sort((a, b) => a - b)
来源：http://af.lnxyls.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://cc.9csxet.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://la.gzmigu.cn

Go:   slices.Sort(arr)
来源：http://nl.szxytkj.cn

Ruby: arr.sort
来源：http://av.bjjhwx.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://ka.chemitech.net.cn

[N03] 快速排序（分治示例）
来源：http://gy.huixinmuqiang.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://jh.muxihuayi.cn

PHP:  // 递归实现，或用 usort
来源：http://ar.huanxung.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://xf.jctech888.com.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ue.yuexingan06.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://fv.hnjuh.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://oo.panjiajie.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://qg.panjiajie.cn

C#:   // 手写递归，或 Array.Sort
来源：http://xz.jctech888.com.cn

[N04] 斐波那契数列
来源：http://qy.huanxung.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://zy.bookmarksfly.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ep.shtwfgs.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://gi.huixiangedu.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://pc.shxzskj.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://cs.gzmigu.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://sq.hahajie.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ql.szsharing.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://gg.huanxung.cn

[N05] 最大公约数
来源：http://gj.huanxung.cn

Py:   math.gcd(a, b)
来源：http://zw.panjiajie.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://sm.asd995.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://op.asd995.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://yx.huixinmuqiang.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://fq.jctech888.com.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://em.yuntaijiaju.cn

Ruby: a.gcd(b)
来源：http://kl.gzmigu.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://rl.shtwfgs.cn

[N06] 判断回文字符串
来源：http://nj.bookmarksfly.cn

Py:   s == s[::-1]
来源：http://qh.huanxung.cn

PHP:  $s === strrev($s);
来源：http://dq.bookmarksfly.cn

JS:   s === [...s].reverse().join("")
来源：http://kh.9csxet.cn

TS:   s === [...s].reverse().join("")
来源：http://dj.nicolike.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://bh.muxihuayi.cn

Go:   // 双指针从两端比较
来源：http://gt.bookmarksfly.cn

Ruby: s == s.reverse
来源：http://lj.newstarts.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://xi.521024.cn

[N07] 两数之和（返回下标）
来源：http://ts.newstarts.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://kl.huixiangedu.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://fx.bookmarksfly.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://bl.lnxyls.cn

TS:   // 手写 Map<string, number>
来源：http://oh.szxytkj.cn

Java: // 手写 HashMap
来源：http://cz.huixiangedu.cn

Go:   // 手写 map[int]int
来源：http://ph.szxytkj.cn

Ruby: // 手写 Hash
来源：http://zw.jctech888.com.cn

C#:   // 手写 Dictionary<int, int>
来源：http://of.bookmarksfly.cn

[N08] 生成全排列
来源：http://dw.bjjhwx.cn

Py:   itertools.permutations(arr)
来源：http://cr.nicolike.cn

PHP:  // 手写递归交换
来源：http://xf.gzmigu.cn

JS:   // 手写回溯递归
来源：http://lv.asd995.cn

TS:   // 手写回溯递归
来源：http://vo.jctech888.com.cn

Java: // 手写回溯递归
来源：http://xu.yuntaijiaju.cn

Go:   // 手写回溯递归
来源：http://tq.bjjhwx.cn

Ruby: arr.permutation.to_a
来源：http://li.asd995.cn

C#:   // 手写回溯递归
来源：http://yk.yuntaijiaju.cn

[N09] 栈与队列
来源：http://xg.yuntaijiaju.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://yd.shxzukj.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mh.shxzukj.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ny.chemitech.net.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ah.gzmigu.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://bs.wgjwhj.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://im.hnjuh.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://gr.huanxung.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://za.nicolike.cn

[N10] 链表节点定义
来源：http://dw.nszjky.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wt.lnxyls.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://xn.nszjky.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ub.bookmarksfly.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ny.huixiangedu.cn

Java: class Node { int v; Node next; }
来源：http://qa.nszjky.cn

Go:   type Node struct { V int; Next *Node }
来源：http://xf.asd995.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://vx.asd995.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://qw.szsharing.cn

[N11] 二叉树中序遍历
来源：http://jo.wgjwhj.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://io.9csxet.cn

PHP:  // 手写递归函数
来源：http://pl.shxzskj.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://eh.szsharing.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://uh.nszjky.cn

Java: // 手写递归
来源：http://fn.muxihuayi.cn

Go:   // 手写递归
来源：http://qo.huixiangedu.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://dm.huixiangedu.cn

C#:   // 手写递归
来源：http://is.muxihuayi.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://jv.bjjhwx.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wx.9csxet.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ip.asd995.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ln.gzmigu.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://sd.gzmigu.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://px.szxytkj.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://vm.huixinmuqiang.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://vv.hnjuh.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://xl.yuexingan06.cn

================================================================================
来源：http://wm.shxzskj.cn

O. 并发与异步
来源：http://wi.shtwfgs.cn

================================================================================
来源：http://zn.huanxung.cn

[O01] 启动一个线程
来源：http://ha.nicolike.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://dv.colortex.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://rh.szsharing.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://yx.szsharing.cn

TS:   // 同 JS
来源：http://ns.wgjwhj.cn

Java: new Thread(() -> f()).start()
来源：http://do.huixinmuqiang.cn

Go:   go f()
来源：http://bt.muxihuayi.cn

Ruby: Thread.new { f }
来源：http://un.szxytkj.cn

C#:   Task.Run(() => F());
来源：http://im.huixinmuqiang.cn

[O02] 使用线程池
来源：http://re.huixiangedu.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://bt.colortex.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://in.shtwfgs.cn

JS:   // worker_threads 线程池
来源：http://en.huixinmuqiang.cn

TS:   // worker_threads 线程池
来源：http://fx.9csxet.cn

Java: Executors.newFixedThreadPool(4)
来源：http://at.shtwfgs.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://we.hnjuh.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://yc.bjjhwx.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://cn.muxihuayi.cn

[O03] 加锁保护共享数据
来源：http://na.chemitech.net.cn

Py:   with lock: shared += 1
来源：http://wj.shtwfgs.cn

PHP:  // 用 flock() 做文件锁
来源：http://jt.chemitech.net.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://tp.wgjwhj.cn

TS:   // 同 JS
来源：http://sk.jianghongdianzi.cn

Java: synchronized (this) { shared++; }
来源：http://bw.bookmarksfly.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://dl.521024.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://oa.shxzukj.cn

C#:   lock (gate) { shared++; }
来源：http://ar.szxytkj.cn

[O04] 定义异步函数并等待
来源：http://rf.bjjhwx.cn

Py:   async def f():⏎    await g()
来源：http://hm.lnxyls.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://fc.huanxung.cn

JS:   async function f() { await g(); }
来源：http://kb.nszjky.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://va.hahajie.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://rt.hnjuh.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://gr.panjiajie.cn

Ruby: # 用 Fiber 或 async gem
来源：http://wu.wgjwhj.cn

C#:   async Task F() { await G(); }
来源：http://fe.muxihuayi.cn

[O05] 并发执行并等待全部完成
来源：http://lz.szxytkj.cn

Py:   asyncio.gather(*tasks)
来源：http://zz.nicolike.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://va.huixinmuqiang.cn

JS:   await Promise.all(tasks)
来源：http://hx.newstarts.cn

TS:   await Promise.all(tasks)
来源：http://tr.shxzskj.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://az.muxihuayi.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://zg.hnjuh.cn

Ruby: threads.map(&:join)
来源：http://zw.haigaiapp.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://zd.lnxyls.cn

[O06] 使用进程池
来源：http://zz.yuntaijiaju.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://rk.shtwfgs.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://wk.huixinmuqiang.cn

JS:   // child_process / cluster 模块
来源：http://ma.jctech888.com.cn

TS:   // child_process / cluster 模块
来源：http://mn.hnjuh.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://jz.asd995.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://te.chemitech.net.cn

Ruby: // fork 块
来源：http://ro.huixinmuqiang.cn

C#:   Parallel.For
来源：http://ff.colortex.cn

================================================================================
来源：http://cj.bookmarksfly.cn

P. 常用工具函数
来源：http://nq.yuexingan06.cn

================================================================================
来源：http://sh.huixinmuqiang.cn

[P01] 生成 UUID
来源：http://rd.shxzskj.cn

Py:   str(uuid.uuid4())
来源：http://en.jctech888.com.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://jv.huixinmuqiang.cn

JS:   crypto.randomUUID()
来源：http://my.gzmigu.cn

TS:   crypto.randomUUID()
来源：http://vc.asd995.cn

Java: UUID.randomUUID().toString()
来源：http://yw.muxihuayi.cn

Go:   // 用 github.com/google/uuid
来源：http://yl.hahajie.cn

Ruby: SecureRandom.uuid
来源：http://tz.nicolike.cn

C#:   Guid.NewGuid().ToString()
来源：http://yg.gzmigu.cn

[P02] MD5 / SHA256 摘要
来源：http://gt.9csxet.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://gp.haigaiapp.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://ve.lnxyls.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://cm.hahajie.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://cs.huixinmuqiang.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ys.huixiangedu.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://di.yuntaijiaju.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://dg.colortex.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://kz.bjjhwx.cn

[P03] 生成短随机字符串
来源：http://kd.nicolike.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://eo.shtwfgs.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://fd.shxzukj.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ix.haigaiapp.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://kx.huixiangedu.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://bc.panjiajie.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ce.jianghongdianzi.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://du.chemitech.net.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://sv.shtwfgs.cn

[P04] 求长度
来源：http://sn.huanxung.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://iz.huixiangedu.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mc.nszjky.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://rd.lnxyls.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://zt.yuexingan06.cn

Java: list.size();  map.size();  s.length()
来源：http://hc.colortex.cn

Go:   len(arr);  len(m)
来源：http://ui.chemitech.net.cn

Ruby: x.length;  x.size
来源：http://im.bjjhwx.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://cj.newstarts.cn

[P05] 判断两个对象内容是否相等
来源：http://hb.asd995.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://qc.bookmarksfly.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://dy.wgjwhj.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wq.shtwfgs.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://bp.521024.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://vf.haigaiapp.cn

Go:   reflect.DeepEqual(a, b)
来源：http://lv.yuexingan06.cn

Ruby: a == b
来源：http://tg.colortex.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://qr.szsharing.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://zg.shxzskj.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://bo.newstarts.cn

PHP:  if (empty($x)) {}
来源：http://tj.chemitech.net.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://qs.shtwfgs.cn

TS:   if (x == null) {}
来源：http://xr.colortex.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://oh.gzmigu.cn

Go:   if x == nil {}
来源：http://fm.colortex.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ru.jianghongdianzi.cn

C#:   if (x is null) {}
来源：http://ij.lnxyls.cn

[P07] 防抖与节流
来源：http://nr.nszjky.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://zg.521024.cn

PHP:  // 手写时间戳比较
来源：http://hc.bookmarksfly.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://vk.colortex.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qq.yuexingan06.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hv.newstarts.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ea.szsharing.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://tu.huixiangedu.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://cy.yuexingan06.cn

[P08] 处理浮点精度问题
来源：http://jj.colortex.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ei.shxzukj.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://jm.haigaiapp.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wf.bookmarksfly.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://tn.asd995.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://gf.newstarts.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://sh.nicolike.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://lq.shxzukj.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://fo.shxzukj.cn

================================================================================
来源：http://zk.shxzukj.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://bx.shtwfgs.cn

================================================================================
来源：http://kx.hnjuh.cn

[Q01] 创建表
来源：http://uj.yuexingan06.cn

CREATE TABLE users (
来源：http://ap.yuexingan06.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://qa.hahajie.cn

name VARCHAR(50) NOT NULL,
来源：http://hu.huixinmuqiang.cn

email VARCHAR(100) UNIQUE,
来源：http://fz.yuexingan06.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://sd.jianghongdianzi.cn

);
来源：http://mr.szsharing.cn

[Q02] 创建带外键的表
来源：http://yt.hnjuh.cn

CREATE TABLE orders (
来源：http://ju.shxzskj.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://om.wgjwhj.cn

user_id INT NOT NULL,
来源：http://lv.jianghongdianzi.cn

amount DECIMAL(10, 2),
来源：http://mo.colortex.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://vd.yuexingan06.cn

);
来源：http://wo.huixinmuqiang.cn

[Q03] 增加列
来源：http://ch.wgjwhj.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://be.shtwfgs.cn

[Q04] 修改列类型
来源：http://cm.huanxung.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ay.szxytkj.cn

[Q05] 重命名列
来源：http://ui.colortex.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://fb.shxzskj.cn

[Q06] 删除列
来源：http://sw.521024.cn

ALTER TABLE users DROP COLUMN age;
来源：http://se.lnxyls.cn

[Q07] 删除表
来源：http://tk.yuntaijiaju.cn

DROP TABLE IF EXISTS orders;
来源：http://of.shxzukj.cn

[Q08] 创建普通索引
来源：http://zr.haigaiapp.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://gh.gzmigu.cn

[Q09] 创建唯一索引
来源：http://ll.521024.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://qy.jctech888.com.cn

[Q10] 插入单行
来源：http://zw.yuntaijiaju.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://gn.szsharing.cn

[Q11] 一次插入多行
来源：http://bh.asd995.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ei.huanxung.cn

[Q12] 插入后取自增 ID
来源：http://no.szsharing.cn

INSERT INTO users (name) VALUES ('C');
来源：http://us.hahajie.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://kv.jianghongdianzi.cn

[Q13] 忽略重复插入
来源：http://yw.huixiangedu.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://qu.huixiangedu.cn

[Q14] 存在则更新（upsert）
来源：http://ra.haigaiapp.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://bb.gzmigu.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://gp.yuexingan06.cn

[Q15] 查询全部
来源：http://vb.gzmigu.cn

SELECT * FROM users;
来源：http://uy.jctech888.com.cn

[Q16] 查询指定列
来源：http://el.jianghongdianzi.cn

SELECT id, name FROM users;
来源：http://bn.nicolike.cn

[Q17] 条件查询
来源：http://fn.huanxung.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ma.521024.cn

[Q18] 模糊匹配
来源：http://me.yuexingan06.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://xc.lnxyls.cn

[Q19] 范围查询
来源：http://nb.huanxung.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://pu.huixinmuqiang.cn

[Q20] IN 列表
来源：http://rx.hnjuh.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ii.huixinmuqiang.cn

[Q21] 空值判断
来源：http://er.huanxung.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://ak.asd995.cn

[Q22] 排序
来源：http://yk.gzmigu.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://qc.huixinmuqiang.cn

[Q23] 分页
来源：http://ur.haigaiapp.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://zd.huixinmuqiang.cn

[Q24] 去重
来源：http://rg.nszjky.cn

SELECT DISTINCT city FROM users;
来源：http://kf.shtwfgs.cn

[Q25] 只取前 N 条
来源：http://og.shxzskj.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://vl.jctech888.com.cn

[Q26] 计数
来源：http://ro.chemitech.net.cn

SELECT COUNT(*) FROM users;
来源：http://vc.gzmigu.cn

[Q27] 条件计数
来源：http://rf.szxytkj.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://np.huanxung.cn

[Q28] 求和与平均
来源：http://ru.szsharing.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://cl.huixiangedu.cn

[Q29] 最大最小值
来源：http://qa.colortex.cn


<!-- 参考信息 -->