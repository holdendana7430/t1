代发 wailian999

Ruby: arr.sort
来源：http://pz.bjjhwx.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://dm.yuntaijiaju.cn

[N03] 快速排序（分治示例）
来源：http://od.colortex.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ks.chemitech.net.cn

PHP:  // 递归实现，或用 usort
来源：http://kr.shxzukj.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wj.huanxung.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://pc.huixinmuqiang.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://pa.nicolike.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://jy.shxzskj.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://lx.bjjhwx.cn

C#:   // 手写递归，或 Array.Sort
来源：http://vm.huixiangedu.cn

[N04] 斐波那契数列
来源：http://ec.newstarts.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://cz.huixinmuqiang.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://iq.shxzskj.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mq.521024.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ws.shxzukj.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hh.shtwfgs.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://dq.huixinmuqiang.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://de.szsharing.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://xq.huanxung.cn

[N05] 最大公约数
来源：http://qv.shxzukj.cn

Py:   math.gcd(a, b)
来源：http://cl.shxzukj.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ym.hnjuh.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://rf.shxzskj.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://io.huanxung.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://qi.wgjwhj.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://nx.huanxung.cn

Ruby: a.gcd(b)
来源：http://bo.hnjuh.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://bl.colortex.cn

[N06] 判断回文字符串
来源：http://cc.szsharing.cn

Py:   s == s[::-1]
来源：http://fl.huanxung.cn

PHP:  $s === strrev($s);
来源：http://mg.jctech888.com.cn

JS:   s === [...s].reverse().join("")
来源：http://jp.szsharing.cn

TS:   s === [...s].reverse().join("")
来源：http://xw.hnjuh.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://lw.szxytkj.cn

Go:   // 双指针从两端比较
来源：http://dp.yuexingan06.cn

Ruby: s == s.reverse
来源：http://ka.hnjuh.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://tp.jctech888.com.cn

[N07] 两数之和（返回下标）
来源：http://ac.jianghongdianzi.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mv.yuntaijiaju.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://dr.jianghongdianzi.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://dw.bjjhwx.cn

TS:   // 手写 Map<string, number>
来源：http://tm.9csxet.cn

Java: // 手写 HashMap
来源：http://vt.chemitech.net.cn

Go:   // 手写 map[int]int
来源：http://fz.newstarts.cn

Ruby: // 手写 Hash
来源：http://yi.yuntaijiaju.cn

C#:   // 手写 Dictionary<int, int>
来源：http://sl.huanxung.cn

[N08] 生成全排列
来源：http://vy.szsharing.cn

Py:   itertools.permutations(arr)
来源：http://tn.hnjuh.cn

PHP:  // 手写递归交换
来源：http://ok.bookmarksfly.cn

JS:   // 手写回溯递归
来源：http://jn.huixiangedu.cn

TS:   // 手写回溯递归
来源：http://yy.huixinmuqiang.cn

Java: // 手写回溯递归
来源：http://up.jctech888.com.cn

Go:   // 手写回溯递归
来源：http://cj.newstarts.cn

Ruby: arr.permutation.to_a
来源：http://lp.bookmarksfly.cn

C#:   // 手写回溯递归
来源：http://os.hahajie.cn

[N09] 栈与队列
来源：http://qh.gzmigu.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://lg.nicolike.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://xj.nicolike.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://dw.hahajie.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ha.jctech888.com.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://uc.chemitech.net.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://xv.wgjwhj.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://jd.jianghongdianzi.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://lq.chemitech.net.cn

[N10] 链表节点定义
来源：http://vh.lnxyls.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ej.gzmigu.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://lf.haigaiapp.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ov.yuntaijiaju.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://lg.shtwfgs.cn

Java: class Node { int v; Node next; }
来源：http://kl.szxytkj.cn

Go:   type Node struct { V int; Next *Node }
来源：http://io.521024.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://fi.shtwfgs.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://bw.bjjhwx.cn

[N11] 二叉树中序遍历
来源：http://cb.huanxung.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ui.nszjky.cn

PHP:  // 手写递归函数
来源：http://co.9csxet.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://tg.huixiangedu.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://oj.shtwfgs.cn

Java: // 手写递归
来源：http://bn.shxzskj.cn

Go:   // 手写递归
来源：http://at.huixinmuqiang.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wx.bookmarksfly.cn

C#:   // 手写递归
来源：http://gp.yuexingan06.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://yu.szsharing.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://lx.szxytkj.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://fw.shxzskj.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://jq.hnjuh.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://nn.colortex.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://vm.yuexingan06.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://uw.bookmarksfly.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ho.shtwfgs.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://if.huixinmuqiang.cn

================================================================================
来源：http://hk.shxzskj.cn

O. 并发与异步
来源：http://nc.shxzukj.cn

================================================================================
来源：http://wz.gzmigu.cn

[O01] 启动一个线程
来源：http://pp.gzmigu.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://pa.chemitech.net.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://rd.gzmigu.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hj.hnjuh.cn

TS:   // 同 JS
来源：http://io.huixinmuqiang.cn

Java: new Thread(() -> f()).start()
来源：http://ru.shxzskj.cn

Go:   go f()
来源：http://to.yuexingan06.cn

Ruby: Thread.new { f }
来源：http://fb.huixinmuqiang.cn

C#:   Task.Run(() => F());
来源：http://fn.szxytkj.cn

[O02] 使用线程池
来源：http://wb.jianghongdianzi.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://zf.shxzskj.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mn.wgjwhj.cn

JS:   // worker_threads 线程池
来源：http://be.9csxet.cn

TS:   // worker_threads 线程池
来源：http://ez.9csxet.cn

Java: Executors.newFixedThreadPool(4)
来源：http://bw.hnjuh.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://oo.chemitech.net.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://cd.chemitech.net.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://bc.nicolike.cn

[O03] 加锁保护共享数据
来源：http://za.shtwfgs.cn

Py:   with lock: shared += 1
来源：http://hm.shxzukj.cn

PHP:  // 用 flock() 做文件锁
来源：http://ff.lnxyls.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://pe.muxihuayi.cn

TS:   // 同 JS
来源：http://uy.haigaiapp.cn

Java: synchronized (this) { shared++; }
来源：http://tw.shtwfgs.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://um.jianghongdianzi.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://og.nszjky.cn

C#:   lock (gate) { shared++; }
来源：http://ri.yuexingan06.cn

[O04] 定义异步函数并等待
来源：http://mc.yuntaijiaju.cn

Py:   async def f():⏎    await g()
来源：http://zy.jctech888.com.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://au.jctech888.com.cn

JS:   async function f() { await g(); }
来源：http://zm.szsharing.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://pp.newstarts.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://gz.hnjuh.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://nw.nicolike.cn

Ruby: # 用 Fiber 或 async gem
来源：http://ho.521024.cn

C#:   async Task F() { await G(); }
来源：http://pf.shtwfgs.cn

[O05] 并发执行并等待全部完成
来源：http://ur.gzmigu.cn

Py:   asyncio.gather(*tasks)
来源：http://ww.haigaiapp.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://rk.521024.cn

JS:   await Promise.all(tasks)
来源：http://et.yuexingan06.cn

TS:   await Promise.all(tasks)
来源：http://ih.huixiangedu.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://be.szsharing.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://nx.nszjky.cn

Ruby: threads.map(&:join)
来源：http://yz.nszjky.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://mh.panjiajie.cn

[O06] 使用进程池
来源：http://cm.lnxyls.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://tc.colortex.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://cp.chemitech.net.cn

JS:   // child_process / cluster 模块
来源：http://cl.shxzskj.cn

TS:   // child_process / cluster 模块
来源：http://rz.huixinmuqiang.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://gx.szxytkj.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ix.colortex.cn

Ruby: // fork 块
来源：http://sz.asd995.cn

C#:   Parallel.For
来源：http://gm.huanxung.cn

================================================================================
来源：http://wm.szsharing.cn

P. 常用工具函数
来源：http://cw.huixinmuqiang.cn

================================================================================
来源：http://si.colortex.cn

[P01] 生成 UUID
来源：http://uj.hahajie.cn

Py:   str(uuid.uuid4())
来源：http://gt.nicolike.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://nw.9csxet.cn

JS:   crypto.randomUUID()
来源：http://ot.shxzskj.cn

TS:   crypto.randomUUID()
来源：http://ot.bookmarksfly.cn

Java: UUID.randomUUID().toString()
来源：http://dr.newstarts.cn

Go:   // 用 github.com/google/uuid
来源：http://pc.haigaiapp.cn

Ruby: SecureRandom.uuid
来源：http://cb.wgjwhj.cn

C#:   Guid.NewGuid().ToString()
来源：http://wl.nszjky.cn

[P02] MD5 / SHA256 摘要
来源：http://tu.haigaiapp.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://xt.jctech888.com.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://ob.shxzukj.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://em.haigaiapp.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://bz.jctech888.com.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ai.nicolike.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ku.hnjuh.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://xv.bjjhwx.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://nn.chemitech.net.cn

[P03] 生成短随机字符串
来源：http://lh.huanxung.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://di.jianghongdianzi.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://yl.huixiangedu.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://zr.shtwfgs.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://iv.szxytkj.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://xv.asd995.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://dj.chemitech.net.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://id.lnxyls.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://fo.newstarts.cn

[P04] 求长度
来源：http://in.haigaiapp.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://jh.szxytkj.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://lx.bjjhwx.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://kn.nszjky.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ty.huanxung.cn

Java: list.size();  map.size();  s.length()
来源：http://il.huanxung.cn

Go:   len(arr);  len(m)
来源：http://ty.jctech888.com.cn

Ruby: x.length;  x.size
来源：http://wz.shxzskj.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://cx.shxzukj.cn

[P05] 判断两个对象内容是否相等
来源：http://hk.panjiajie.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://ro.chemitech.net.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://su.haigaiapp.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://rm.shtwfgs.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mc.shtwfgs.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://jf.panjiajie.cn

Go:   reflect.DeepEqual(a, b)
来源：http://rs.wgjwhj.cn

Ruby: a == b
来源：http://pu.bjjhwx.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://lk.haigaiapp.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://dr.shxzukj.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://de.newstarts.cn

PHP:  if (empty($x)) {}
来源：http://gg.szxytkj.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ep.yuntaijiaju.cn

TS:   if (x == null) {}
来源：http://em.szsharing.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://go.wgjwhj.cn

Go:   if x == nil {}
来源：http://dr.nicolike.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://vj.wgjwhj.cn

C#:   if (x is null) {}
来源：http://tn.yuntaijiaju.cn

[P07] 防抖与节流
来源：http://ef.chemitech.net.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ya.huixiangedu.cn

PHP:  // 手写时间戳比较
来源：http://mz.haigaiapp.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ao.nszjky.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://go.nszjky.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://rh.asd995.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ui.panjiajie.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://id.huixinmuqiang.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ha.newstarts.cn

[P08] 处理浮点精度问题
来源：http://py.nszjky.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://jb.shtwfgs.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hv.shxzukj.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://uv.szxytkj.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://sf.9csxet.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://gc.szsharing.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://fz.szxytkj.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://lr.bjjhwx.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://kt.shxzskj.cn

================================================================================
来源：http://fm.jctech888.com.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ld.asd995.cn

================================================================================
来源：http://yr.colortex.cn

[Q01] 创建表
来源：http://gp.asd995.cn

CREATE TABLE users (
来源：http://up.shtwfgs.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ca.shtwfgs.cn

name VARCHAR(50) NOT NULL,
来源：http://fj.yuntaijiaju.cn

email VARCHAR(100) UNIQUE,
来源：http://pw.szsharing.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ev.jianghongdianzi.cn

);
来源：http://tt.521024.cn

[Q02] 创建带外键的表
来源：http://yy.nszjky.cn

CREATE TABLE orders (
来源：http://ah.521024.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://lu.521024.cn

user_id INT NOT NULL,
来源：http://jv.shxzukj.cn

amount DECIMAL(10, 2),
来源：http://jm.521024.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://fv.yuntaijiaju.cn

);
来源：http://lc.yuntaijiaju.cn

[Q03] 增加列
来源：http://zf.gzmigu.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://nn.haigaiapp.cn

[Q04] 修改列类型
来源：http://vf.colortex.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://qb.asd995.cn

[Q05] 重命名列
来源：http://kt.yuexingan06.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://uo.shtwfgs.cn

[Q06] 删除列
来源：http://lb.jianghongdianzi.cn

ALTER TABLE users DROP COLUMN age;
来源：http://lm.shtwfgs.cn

[Q07] 删除表
来源：http://yj.nszjky.cn

DROP TABLE IF EXISTS orders;
来源：http://vj.jianghongdianzi.cn

[Q08] 创建普通索引
来源：http://me.shxzskj.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://um.haigaiapp.cn

[Q09] 创建唯一索引
来源：http://ek.panjiajie.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wm.jianghongdianzi.cn

[Q10] 插入单行
来源：http://wa.nszjky.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hl.gzmigu.cn

[Q11] 一次插入多行
来源：http://ea.jianghongdianzi.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://av.shxzskj.cn

[Q12] 插入后取自增 ID
来源：http://mg.huixiangedu.cn

INSERT INTO users (name) VALUES ('C');
来源：http://rg.huixiangedu.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://eq.hnjuh.cn

[Q13] 忽略重复插入
来源：http://um.panjiajie.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://sm.bjjhwx.cn

[Q14] 存在则更新（upsert）
来源：http://vc.hahajie.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.bjjhwx.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hw.shxzskj.cn

[Q15] 查询全部
来源：http://xg.shxzukj.cn

SELECT * FROM users;
来源：http://zg.nicolike.cn

[Q16] 查询指定列
来源：http://rx.wgjwhj.cn

SELECT id, name FROM users;
来源：http://kd.huanxung.cn

[Q17] 条件查询
来源：http://lg.nszjky.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://sj.yuexingan06.cn

[Q18] 模糊匹配
来源：http://mn.panjiajie.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://dc.shxzskj.cn

[Q19] 范围查询
来源：http://lo.hahajie.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://zk.yuexingan06.cn

[Q20] IN 列表
来源：http://kg.yuexingan06.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://zh.colortex.cn

[Q21] 空值判断
来源：http://gq.haigaiapp.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://kq.shxzukj.cn

[Q22] 排序
来源：http://sa.szxytkj.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://bh.chemitech.net.cn

[Q23] 分页
来源：http://ct.chemitech.net.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://pw.chemitech.net.cn

[Q24] 去重
来源：http://bx.yuexingan06.cn

SELECT DISTINCT city FROM users;
来源：http://ur.jctech888.com.cn

[Q25] 只取前 N 条
来源：http://kn.nszjky.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://nv.panjiajie.cn

[Q26] 计数
来源：http://ye.huixinmuqiang.cn

SELECT COUNT(*) FROM users;
来源：http://da.chemitech.net.cn

[Q27] 条件计数
来源：http://zh.wgjwhj.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://vb.hahajie.cn

[Q28] 求和与平均
来源：http://iq.wgjwhj.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://sj.panjiajie.cn

[Q29] 最大最小值
来源：http://kj.yuntaijiaju.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://ab.lnxyls.cn

[Q30] 分组统计
来源：http://jd.shxzskj.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://yd.huanxung.cn

[Q31] 分组后过滤
来源：http://uz.newstarts.cn


<!-- 参考信息 -->