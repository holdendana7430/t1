代发 wailian999

JS:   [...arr].sort((a, b) => a - b)
来源：http://sk.yuntaijiaju.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://qm.9csxet.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://dj.muxihuayi.cn

Go:   slices.Sort(arr)
来源：http://tu.chemitech.net.cn

Ruby: arr.sort
来源：http://si.huixiangedu.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://ry.newstarts.cn

[N03] 快速排序（分治示例）
来源：http://dc.lnxyls.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ew.lnxyls.cn

PHP:  // 递归实现，或用 usort
来源：http://ut.huixinmuqiang.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://fq.gzmigu.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://kc.hnjuh.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ei.szxytkj.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://yy.haigaiapp.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hb.yuntaijiaju.cn

C#:   // 手写递归，或 Array.Sort
来源：http://ex.huixinmuqiang.cn

[N04] 斐波那契数列
来源：http://sy.huixiangedu.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://uw.shxzukj.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://db.nszjky.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://iv.bjjhwx.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://dy.asd995.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ul.shtwfgs.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://lm.gzmigu.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ff.bookmarksfly.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://eo.bookmarksfly.cn

[N05] 最大公约数
来源：http://op.9csxet.cn

Py:   math.gcd(a, b)
来源：http://ju.jctech888.com.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mh.colortex.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://sd.szxytkj.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://jf.nicolike.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://zb.yuexingan06.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://so.lnxyls.cn

Ruby: a.gcd(b)
来源：http://oc.panjiajie.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ya.shxzskj.cn

[N06] 判断回文字符串
来源：http://bg.nszjky.cn

Py:   s == s[::-1]
来源：http://rs.jianghongdianzi.cn

PHP:  $s === strrev($s);
来源：http://kj.asd995.cn

JS:   s === [...s].reverse().join("")
来源：http://up.nicolike.cn

TS:   s === [...s].reverse().join("")
来源：http://kd.newstarts.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://lr.muxihuayi.cn

Go:   // 双指针从两端比较
来源：http://pb.muxihuayi.cn

Ruby: s == s.reverse
来源：http://qj.chemitech.net.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://md.jianghongdianzi.cn

[N07] 两数之和（返回下标）
来源：http://qw.jianghongdianzi.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://kp.huixiangedu.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://pz.colortex.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://nn.shxzskj.cn

TS:   // 手写 Map<string, number>
来源：http://mj.szxytkj.cn

Java: // 手写 HashMap
来源：http://os.yuexingan06.cn

Go:   // 手写 map[int]int
来源：http://tn.lnxyls.cn

Ruby: // 手写 Hash
来源：http://wn.nicolike.cn

C#:   // 手写 Dictionary<int, int>
来源：http://gc.bjjhwx.cn

[N08] 生成全排列
来源：http://xf.huixinmuqiang.cn

Py:   itertools.permutations(arr)
来源：http://it.asd995.cn

PHP:  // 手写递归交换
来源：http://zd.shxzskj.cn

JS:   // 手写回溯递归
来源：http://fu.nszjky.cn

TS:   // 手写回溯递归
来源：http://qb.asd995.cn

Java: // 手写回溯递归
来源：http://we.jctech888.com.cn

Go:   // 手写回溯递归
来源：http://mv.haigaiapp.cn

Ruby: arr.permutation.to_a
来源：http://wf.wgjwhj.cn

C#:   // 手写回溯递归
来源：http://yt.haigaiapp.cn

[N09] 栈与队列
来源：http://cm.panjiajie.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://nb.szsharing.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ha.shxzskj.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://qf.nszjky.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.wgjwhj.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ca.wgjwhj.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://vb.szsharing.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hs.newstarts.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://my.newstarts.cn

[N10] 链表节点定义
来源：http://bv.hahajie.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://pg.haigaiapp.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://sf.asd995.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://xn.asd995.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://yp.panjiajie.cn

Java: class Node { int v; Node next; }
来源：http://ab.nszjky.cn

Go:   type Node struct { V int; Next *Node }
来源：http://tf.muxihuayi.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://qv.szxytkj.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://um.bookmarksfly.cn

[N11] 二叉树中序遍历
来源：http://mc.yuntaijiaju.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hf.jctech888.com.cn

PHP:  // 手写递归函数
来源：http://gd.9csxet.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ch.yuntaijiaju.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ty.szxytkj.cn

Java: // 手写递归
来源：http://kp.521024.cn

Go:   // 手写递归
来源：http://du.colortex.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wm.yuntaijiaju.cn

C#:   // 手写递归
来源：http://gs.hnjuh.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://cq.bookmarksfly.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://vm.521024.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://kf.asd995.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hk.hnjuh.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://fc.nszjky.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mf.yuexingan06.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://kr.nszjky.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://dl.bookmarksfly.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://nm.shtwfgs.cn

================================================================================
来源：http://fq.jianghongdianzi.cn

O. 并发与异步
来源：http://oy.hnjuh.cn

================================================================================
来源：http://ek.haigaiapp.cn

[O01] 启动一个线程
来源：http://dx.colortex.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://dp.shtwfgs.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://aa.huixinmuqiang.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://xw.shxzukj.cn

TS:   // 同 JS
来源：http://hu.muxihuayi.cn

Java: new Thread(() -> f()).start()
来源：http://kq.nszjky.cn

Go:   go f()
来源：http://hh.asd995.cn

Ruby: Thread.new { f }
来源：http://lx.nszjky.cn

C#:   Task.Run(() => F());
来源：http://bx.9csxet.cn

[O02] 使用线程池
来源：http://sv.huanxung.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://sk.szxytkj.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://px.jianghongdianzi.cn

JS:   // worker_threads 线程池
来源：http://er.hnjuh.cn

TS:   // worker_threads 线程池
来源：http://is.colortex.cn

Java: Executors.newFixedThreadPool(4)
来源：http://xp.yuntaijiaju.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://gs.nszjky.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://jc.yuntaijiaju.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://uu.szxytkj.cn

[O03] 加锁保护共享数据
来源：http://pg.colortex.cn

Py:   with lock: shared += 1
来源：http://ir.nszjky.cn

PHP:  // 用 flock() 做文件锁
来源：http://ge.szxytkj.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://bc.panjiajie.cn

TS:   // 同 JS
来源：http://wz.yuntaijiaju.cn

Java: synchronized (this) { shared++; }
来源：http://to.shtwfgs.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://or.nicolike.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://mp.huixiangedu.cn

C#:   lock (gate) { shared++; }
来源：http://ks.muxihuayi.cn

[O04] 定义异步函数并等待
来源：http://qk.shxzukj.cn

Py:   async def f():⏎    await g()
来源：http://jk.yuexingan06.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://uu.huixiangedu.cn

JS:   async function f() { await g(); }
来源：http://qn.panjiajie.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://ct.521024.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://go.bookmarksfly.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ko.lnxyls.cn

Ruby: # 用 Fiber 或 async gem
来源：http://ui.colortex.cn

C#:   async Task F() { await G(); }
来源：http://sd.huixinmuqiang.cn

[O05] 并发执行并等待全部完成
来源：http://wz.muxihuayi.cn

Py:   asyncio.gather(*tasks)
来源：http://gh.huixiangedu.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://iy.yuntaijiaju.cn

JS:   await Promise.all(tasks)
来源：http://be.jctech888.com.cn

TS:   await Promise.all(tasks)
来源：http://we.yuntaijiaju.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hn.nszjky.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://fe.bjjhwx.cn

Ruby: threads.map(&:join)
来源：http://sm.hnjuh.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://xw.shtwfgs.cn

[O06] 使用进程池
来源：http://kn.gzmigu.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://zq.szsharing.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://fd.haigaiapp.cn

JS:   // child_process / cluster 模块
来源：http://jn.newstarts.cn

TS:   // child_process / cluster 模块
来源：http://fn.wgjwhj.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://tr.hnjuh.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://vq.chemitech.net.cn

Ruby: // fork 块
来源：http://ka.lnxyls.cn

C#:   Parallel.For
来源：http://tv.jianghongdianzi.cn

================================================================================
来源：http://bd.nicolike.cn

P. 常用工具函数
来源：http://fg.gzmigu.cn

================================================================================
来源：http://bq.lnxyls.cn

[P01] 生成 UUID
来源：http://ye.newstarts.cn

Py:   str(uuid.uuid4())
来源：http://ir.szsharing.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ny.newstarts.cn

JS:   crypto.randomUUID()
来源：http://ly.9csxet.cn

TS:   crypto.randomUUID()
来源：http://ei.nicolike.cn

Java: UUID.randomUUID().toString()
来源：http://pn.muxihuayi.cn

Go:   // 用 github.com/google/uuid
来源：http://is.hnjuh.cn

Ruby: SecureRandom.uuid
来源：http://ge.wgjwhj.cn

C#:   Guid.NewGuid().ToString()
来源：http://on.newstarts.cn

[P02] MD5 / SHA256 摘要
来源：http://ts.panjiajie.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wz.wgjwhj.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://ik.chemitech.net.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://cs.jctech888.com.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wd.521024.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://nz.bjjhwx.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://pi.jctech888.com.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ok.muxihuayi.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://uc.haigaiapp.cn

[P03] 生成短随机字符串
来源：http://rg.521024.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://gt.huixinmuqiang.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://gj.gzmigu.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://xz.szxytkj.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://na.bjjhwx.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wk.wgjwhj.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://sy.hahajie.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://yc.9csxet.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://nl.panjiajie.cn

[P04] 求长度
来源：http://lw.huixinmuqiang.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://nc.lnxyls.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://uf.szsharing.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://gi.colortex.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://dm.yuntaijiaju.cn

Java: list.size();  map.size();  s.length()
来源：http://xv.yuntaijiaju.cn

Go:   len(arr);  len(m)
来源：http://el.huixinmuqiang.cn

Ruby: x.length;  x.size
来源：http://wa.hnjuh.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://hc.huixinmuqiang.cn

[P05] 判断两个对象内容是否相等
来源：http://sy.muxihuayi.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://pq.huixiangedu.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://bo.szsharing.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://cg.shxzskj.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://xp.hahajie.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ty.colortex.cn

Go:   reflect.DeepEqual(a, b)
来源：http://cr.yuexingan06.cn

Ruby: a == b
来源：http://bh.bookmarksfly.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ur.newstarts.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://gj.nszjky.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://re.yuntaijiaju.cn

PHP:  if (empty($x)) {}
来源：http://aq.521024.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ix.jctech888.com.cn

TS:   if (x == null) {}
来源：http://oh.shxzukj.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://fg.yuexingan06.cn

Go:   if x == nil {}
来源：http://zw.szsharing.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://tg.wgjwhj.cn

C#:   if (x is null) {}
来源：http://pf.huanxung.cn

[P07] 防抖与节流
来源：http://mb.bookmarksfly.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://gi.jianghongdianzi.cn

PHP:  // 手写时间戳比较
来源：http://xg.muxihuayi.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://cm.colortex.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://cb.521024.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ik.nicolike.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://nb.bjjhwx.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://km.521024.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://nc.lnxyls.cn

[P08] 处理浮点精度问题
来源：http://jd.nicolike.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://vx.szxytkj.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://vo.huixiangedu.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://yy.muxihuayi.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://cr.huixiangedu.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://cg.nicolike.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://lx.panjiajie.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://fm.jianghongdianzi.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://xe.shxzskj.cn

================================================================================
来源：http://zj.szxytkj.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://yj.hnjuh.cn

================================================================================
来源：http://qe.bookmarksfly.cn

[Q01] 创建表
来源：http://dv.bookmarksfly.cn

CREATE TABLE users (
来源：http://cj.nicolike.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://va.yuntaijiaju.cn

name VARCHAR(50) NOT NULL,
来源：http://qv.chemitech.net.cn

email VARCHAR(100) UNIQUE,
来源：http://sh.wgjwhj.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://jl.huixiangedu.cn

);
来源：http://ba.yuntaijiaju.cn

[Q02] 创建带外键的表
来源：http://cx.huanxung.cn

CREATE TABLE orders (
来源：http://ru.bjjhwx.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://xz.gzmigu.cn

user_id INT NOT NULL,
来源：http://xf.chemitech.net.cn

amount DECIMAL(10, 2),
来源：http://cy.lnxyls.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://bc.haigaiapp.cn

);
来源：http://zz.chemitech.net.cn

[Q03] 增加列
来源：http://rv.hahajie.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://pc.hahajie.cn

[Q04] 修改列类型
来源：http://gv.shtwfgs.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://vw.jctech888.com.cn

[Q05] 重命名列
来源：http://sp.lnxyls.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://sk.hnjuh.cn

[Q06] 删除列
来源：http://uj.huanxung.cn

ALTER TABLE users DROP COLUMN age;
来源：http://rp.lnxyls.cn

[Q07] 删除表
来源：http://vt.huixinmuqiang.cn

DROP TABLE IF EXISTS orders;
来源：http://xh.newstarts.cn

[Q08] 创建普通索引
来源：http://ne.yuntaijiaju.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://vt.huixiangedu.cn

[Q09] 创建唯一索引
来源：http://gv.shxzukj.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://yn.huixiangedu.cn

[Q10] 插入单行
来源：http://hv.chemitech.net.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://br.huixinmuqiang.cn

[Q11] 一次插入多行
来源：http://rn.chemitech.net.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://it.colortex.cn

[Q12] 插入后取自增 ID
来源：http://mw.521024.cn

INSERT INTO users (name) VALUES ('C');
来源：http://jr.huixiangedu.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ep.bjjhwx.cn

[Q13] 忽略重复插入
来源：http://ug.bookmarksfly.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://is.huixiangedu.cn

[Q14] 存在则更新（upsert）
来源：http://mo.shxzskj.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://zc.huanxung.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://iy.gzmigu.cn

[Q15] 查询全部
来源：http://ug.lnxyls.cn

SELECT * FROM users;
来源：http://ln.lnxyls.cn

[Q16] 查询指定列
来源：http://mg.shxzskj.cn

SELECT id, name FROM users;
来源：http://sm.jianghongdianzi.cn

[Q17] 条件查询
来源：http://lo.huixinmuqiang.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://nu.szsharing.cn

[Q18] 模糊匹配
来源：http://qm.9csxet.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wg.shtwfgs.cn

[Q19] 范围查询
来源：http://oz.9csxet.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://rr.gzmigu.cn

[Q20] IN 列表
来源：http://mm.bookmarksfly.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://sx.wgjwhj.cn

[Q21] 空值判断
来源：http://qv.nszjky.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://is.yuexingan06.cn

[Q22] 排序
来源：http://ow.szxytkj.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://zx.yuexingan06.cn

[Q23] 分页
来源：http://eo.521024.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://pi.haigaiapp.cn

[Q24] 去重
来源：http://tw.jianghongdianzi.cn

SELECT DISTINCT city FROM users;
来源：http://yy.gzmigu.cn

[Q25] 只取前 N 条
来源：http://ey.huanxung.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://jd.hahajie.cn

[Q26] 计数
来源：http://vr.haigaiapp.cn

SELECT COUNT(*) FROM users;
来源：http://tz.hahajie.cn

[Q27] 条件计数
来源：http://gt.bookmarksfly.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://dc.shxzukj.cn

[Q28] 求和与平均
来源：http://zd.wgjwhj.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://qh.9csxet.cn

[Q29] 最大最小值
来源：http://sq.jctech888.com.cn


<!-- 参考信息 -->