代发 wailian999

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://qa.yuexingan06.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://lp.muxihuayi.cn

C#:   // 手写递归，或 Array.Sort
来源：http://yb.lnxyls.cn

[N04] 斐波那契数列
来源：http://mx.nszjky.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://qo.huixiangedu.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mh.asd995.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://sc.huanxung.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://bp.yuntaijiaju.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://tj.jctech888.com.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://bq.wgjwhj.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://bv.newstarts.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://nn.nicolike.cn

[N05] 最大公约数
来源：http://mc.chemitech.net.cn

Py:   math.gcd(a, b)
来源：http://kq.shxzskj.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://fc.newstarts.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://pj.bookmarksfly.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://oy.521024.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ua.bookmarksfly.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ty.shxzskj.cn

Ruby: a.gcd(b)
来源：http://ex.szxytkj.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://qh.jianghongdianzi.cn

[N06] 判断回文字符串
来源：http://fn.shxzukj.cn

Py:   s == s[::-1]
来源：http://ut.szxytkj.cn

PHP:  $s === strrev($s);
来源：http://jc.newstarts.cn

JS:   s === [...s].reverse().join("")
来源：http://ez.newstarts.cn

TS:   s === [...s].reverse().join("")
来源：http://mi.bjjhwx.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://pq.521024.cn

Go:   // 双指针从两端比较
来源：http://lk.yuntaijiaju.cn

Ruby: s == s.reverse
来源：http://oq.newstarts.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://xf.huixiangedu.cn

[N07] 两数之和（返回下标）
来源：http://qy.panjiajie.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://fo.shtwfgs.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://lf.szxytkj.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://ju.panjiajie.cn

TS:   // 手写 Map<string, number>
来源：http://ki.szxytkj.cn

Java: // 手写 HashMap
来源：http://mh.shxzukj.cn

Go:   // 手写 map[int]int
来源：http://ww.asd995.cn

Ruby: // 手写 Hash
来源：http://vd.asd995.cn

C#:   // 手写 Dictionary<int, int>
来源：http://jg.asd995.cn

[N08] 生成全排列
来源：http://nw.newstarts.cn

Py:   itertools.permutations(arr)
来源：http://rm.shtwfgs.cn

PHP:  // 手写递归交换
来源：http://jy.chemitech.net.cn

JS:   // 手写回溯递归
来源：http://ss.panjiajie.cn

TS:   // 手写回溯递归
来源：http://kb.gzmigu.cn

Java: // 手写回溯递归
来源：http://ab.asd995.cn

Go:   // 手写回溯递归
来源：http://bx.9csxet.cn

Ruby: arr.permutation.to_a
来源：http://iz.hahajie.cn

C#:   // 手写回溯递归
来源：http://rw.hahajie.cn

[N09] 栈与队列
来源：http://ew.jctech888.com.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://dr.bookmarksfly.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://fk.chemitech.net.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://cj.szxytkj.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://fo.hnjuh.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://qb.wgjwhj.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://xl.chemitech.net.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ep.szsharing.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://pk.shxzskj.cn

[N10] 链表节点定义
来源：http://by.panjiajie.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://nc.shxzskj.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://zu.szsharing.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ji.bookmarksfly.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mw.hahajie.cn

Java: class Node { int v; Node next; }
来源：http://ol.chemitech.net.cn

Go:   type Node struct { V int; Next *Node }
来源：http://gp.chemitech.net.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://og.lnxyls.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://lx.huanxung.cn

[N11] 二叉树中序遍历
来源：http://ea.szxytkj.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://om.hnjuh.cn

PHP:  // 手写递归函数
来源：http://al.newstarts.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ao.yuntaijiaju.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://bu.szxytkj.cn

Java: // 手写递归
来源：http://qb.nicolike.cn

Go:   // 手写递归
来源：http://fc.nicolike.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://td.panjiajie.cn

C#:   // 手写递归
来源：http://kw.wgjwhj.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wk.gzmigu.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://qe.hnjuh.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://zy.521024.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wd.jctech888.com.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ks.shxzukj.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://dj.muxihuayi.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://xd.yuntaijiaju.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://yq.colortex.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wl.shxzskj.cn

================================================================================
来源：http://cq.haigaiapp.cn

O. 并发与异步
来源：http://sz.nicolike.cn

================================================================================
来源：http://hf.hnjuh.cn

[O01] 启动一个线程
来源：http://ol.huixiangedu.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hj.szxytkj.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://fh.chemitech.net.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://rz.szsharing.cn

TS:   // 同 JS
来源：http://fw.huanxung.cn

Java: new Thread(() -> f()).start()
来源：http://my.shxzskj.cn

Go:   go f()
来源：http://nt.asd995.cn

Ruby: Thread.new { f }
来源：http://xl.hnjuh.cn

C#:   Task.Run(() => F());
来源：http://wr.521024.cn

[O02] 使用线程池
来源：http://qq.huanxung.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://pn.jctech888.com.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wq.521024.cn

JS:   // worker_threads 线程池
来源：http://mz.yuntaijiaju.cn

TS:   // worker_threads 线程池
来源：http://tw.yuntaijiaju.cn

Java: Executors.newFixedThreadPool(4)
来源：http://ss.shxzskj.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://zw.yuntaijiaju.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wo.9csxet.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://jp.nicolike.cn

[O03] 加锁保护共享数据
来源：http://oe.huanxung.cn

Py:   with lock: shared += 1
来源：http://xh.huixinmuqiang.cn

PHP:  // 用 flock() 做文件锁
来源：http://ex.colortex.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hs.muxihuayi.cn

TS:   // 同 JS
来源：http://dq.yuexingan06.cn

Java: synchronized (this) { shared++; }
来源：http://xi.hnjuh.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://kt.bookmarksfly.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://ha.gzmigu.cn

C#:   lock (gate) { shared++; }
来源：http://go.wgjwhj.cn

[O04] 定义异步函数并等待
来源：http://ld.9csxet.cn

Py:   async def f():⏎    await g()
来源：http://yg.hnjuh.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://pg.521024.cn

JS:   async function f() { await g(); }
来源：http://vr.shxzskj.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://qq.9csxet.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://pp.huanxung.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://jt.huixinmuqiang.cn

Ruby: # 用 Fiber 或 async gem
来源：http://zr.panjiajie.cn

C#:   async Task F() { await G(); }
来源：http://zm.shxzskj.cn

[O05] 并发执行并等待全部完成
来源：http://wp.yuntaijiaju.cn

Py:   asyncio.gather(*tasks)
来源：http://vo.szxytkj.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ut.lnxyls.cn

JS:   await Promise.all(tasks)
来源：http://lr.huixinmuqiang.cn

TS:   await Promise.all(tasks)
来源：http://el.chemitech.net.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://jf.lnxyls.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ce.yuntaijiaju.cn

Ruby: threads.map(&:join)
来源：http://qx.nicolike.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://rq.haigaiapp.cn

[O06] 使用进程池
来源：http://vf.chemitech.net.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://qu.shxzskj.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://ad.bjjhwx.cn

JS:   // child_process / cluster 模块
来源：http://jf.szxytkj.cn

TS:   // child_process / cluster 模块
来源：http://kv.asd995.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://za.hahajie.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://re.bjjhwx.cn

Ruby: // fork 块
来源：http://ap.muxihuayi.cn

C#:   Parallel.For
来源：http://xc.gzmigu.cn

================================================================================
来源：http://jw.szsharing.cn

P. 常用工具函数
来源：http://fe.shxzukj.cn

================================================================================
来源：http://lj.shxzukj.cn

[P01] 生成 UUID
来源：http://xl.yuexingan06.cn

Py:   str(uuid.uuid4())
来源：http://rq.szxytkj.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://vq.bjjhwx.cn

JS:   crypto.randomUUID()
来源：http://qb.panjiajie.cn

TS:   crypto.randomUUID()
来源：http://wm.lnxyls.cn

Java: UUID.randomUUID().toString()
来源：http://lq.nszjky.cn

Go:   // 用 github.com/google/uuid
来源：http://az.chemitech.net.cn

Ruby: SecureRandom.uuid
来源：http://gv.haigaiapp.cn

C#:   Guid.NewGuid().ToString()
来源：http://qx.shxzukj.cn

[P02] MD5 / SHA256 摘要
来源：http://av.jctech888.com.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://xg.hnjuh.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://jc.shtwfgs.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://tt.huanxung.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wt.jctech888.com.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wf.nszjky.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://tv.panjiajie.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://tj.chemitech.net.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://qu.nicolike.cn

[P03] 生成短随机字符串
来源：http://si.yuntaijiaju.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://dl.haigaiapp.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://bx.jianghongdianzi.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://dp.asd995.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://sz.jctech888.com.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://eo.yuntaijiaju.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://tr.huixinmuqiang.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://vl.shxzukj.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://fn.huanxung.cn

[P04] 求长度
来源：http://kn.bookmarksfly.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://jf.haigaiapp.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ph.yuexingan06.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://pz.hahajie.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://df.huixiangedu.cn

Java: list.size();  map.size();  s.length()
来源：http://gx.bjjhwx.cn

Go:   len(arr);  len(m)
来源：http://wp.jctech888.com.cn

Ruby: x.length;  x.size
来源：http://sf.huixinmuqiang.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://tx.szsharing.cn

[P05] 判断两个对象内容是否相等
来源：http://rt.huixiangedu.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://kb.bjjhwx.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://vj.yuexingan06.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://jh.huixinmuqiang.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ik.bookmarksfly.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ij.chemitech.net.cn

Go:   reflect.DeepEqual(a, b)
来源：http://ri.521024.cn

Ruby: a == b
来源：http://zn.bjjhwx.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hy.shxzskj.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://qd.lnxyls.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://pn.9csxet.cn

PHP:  if (empty($x)) {}
来源：http://gw.colortex.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://kj.bookmarksfly.cn

TS:   if (x == null) {}
来源：http://vb.huixiangedu.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://wq.bjjhwx.cn

Go:   if x == nil {}
来源：http://rk.yuntaijiaju.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://jg.panjiajie.cn

C#:   if (x is null) {}
来源：http://gv.jctech888.com.cn

[P07] 防抖与节流
来源：http://pi.colortex.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://qs.huanxung.cn

PHP:  // 手写时间戳比较
来源：http://us.wgjwhj.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://bo.asd995.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://cl.hahajie.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ok.yuntaijiaju.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://cl.shxzukj.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://cz.hnjuh.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://rx.szxytkj.cn

[P08] 处理浮点精度问题
来源：http://kf.nicolike.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://xb.chemitech.net.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://qq.huixiangedu.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://na.huixinmuqiang.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ru.huixiangedu.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://uk.521024.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://pw.huixiangedu.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://vk.newstarts.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://jd.muxihuayi.cn

================================================================================
来源：http://wx.chemitech.net.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://dg.shxzskj.cn

================================================================================
来源：http://ir.newstarts.cn

[Q01] 创建表
来源：http://ks.asd995.cn

CREATE TABLE users (
来源：http://gy.hahajie.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://al.haigaiapp.cn

name VARCHAR(50) NOT NULL,
来源：http://rq.9csxet.cn

email VARCHAR(100) UNIQUE,
来源：http://mc.muxihuayi.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://jb.colortex.cn

);
来源：http://gj.colortex.cn

[Q02] 创建带外键的表
来源：http://uc.szsharing.cn

CREATE TABLE orders (
来源：http://qm.gzmigu.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://po.muxihuayi.cn

user_id INT NOT NULL,
来源：http://nl.yuexingan06.cn

amount DECIMAL(10, 2),
来源：http://pd.shtwfgs.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://vz.shxzukj.cn

);
来源：http://kg.shtwfgs.cn

[Q03] 增加列
来源：http://qy.gzmigu.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://sf.asd995.cn

[Q04] 修改列类型
来源：http://kz.yuntaijiaju.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://dr.huixinmuqiang.cn

[Q05] 重命名列
来源：http://ls.hnjuh.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://lw.bjjhwx.cn

[Q06] 删除列
来源：http://rd.gzmigu.cn

ALTER TABLE users DROP COLUMN age;
来源：http://rq.haigaiapp.cn

[Q07] 删除表
来源：http://uz.huixinmuqiang.cn

DROP TABLE IF EXISTS orders;
来源：http://ei.bjjhwx.cn

[Q08] 创建普通索引
来源：http://gm.asd995.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://eq.jctech888.com.cn

[Q09] 创建唯一索引
来源：http://nj.shxzukj.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://vv.lnxyls.cn

[Q10] 插入单行
来源：http://ud.panjiajie.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://aa.bjjhwx.cn

[Q11] 一次插入多行
来源：http://jr.huixinmuqiang.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://sb.hnjuh.cn

[Q12] 插入后取自增 ID
来源：http://ri.yuntaijiaju.cn

INSERT INTO users (name) VALUES ('C');
来源：http://lk.jctech888.com.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://uy.yuexingan06.cn

[Q13] 忽略重复插入
来源：http://lr.chemitech.net.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://uz.bjjhwx.cn

[Q14] 存在则更新（upsert）
来源：http://gd.521024.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://dl.lnxyls.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://et.hnjuh.cn

[Q15] 查询全部
来源：http://uf.nicolike.cn

SELECT * FROM users;
来源：http://mb.colortex.cn

[Q16] 查询指定列
来源：http://yl.szxytkj.cn

SELECT id, name FROM users;
来源：http://hz.yuntaijiaju.cn

[Q17] 条件查询
来源：http://kz.szxytkj.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://vt.bookmarksfly.cn

[Q18] 模糊匹配
来源：http://om.panjiajie.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://cc.gzmigu.cn

[Q19] 范围查询
来源：http://tk.szxytkj.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://av.huixiangedu.cn

[Q20] IN 列表
来源：http://yh.jctech888.com.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wu.hnjuh.cn

[Q21] 空值判断
来源：http://uj.shxzukj.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://fw.shxzskj.cn

[Q22] 排序
来源：http://av.wgjwhj.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wr.nicolike.cn

[Q23] 分页
来源：http://cy.521024.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://js.asd995.cn

[Q24] 去重
来源：http://wc.9csxet.cn

SELECT DISTINCT city FROM users;
来源：http://wp.colortex.cn

[Q25] 只取前 N 条
来源：http://mm.yuntaijiaju.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://gd.colortex.cn

[Q26] 计数
来源：http://te.lnxyls.cn

SELECT COUNT(*) FROM users;
来源：http://lu.panjiajie.cn

[Q27] 条件计数
来源：http://eo.huixiangedu.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ft.huixinmuqiang.cn

[Q28] 求和与平均
来源：http://qr.gzmigu.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://lf.shtwfgs.cn

[Q29] 最大最小值
来源：http://pp.huanxung.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://oi.huixinmuqiang.cn

[Q30] 分组统计
来源：http://zd.bjjhwx.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://og.newstarts.cn

[Q31] 分组后过滤
来源：http://ut.szxytkj.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://zd.jianghongdianzi.cn

[Q32] 分组拼接字符串
来源：http://xj.newstarts.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://am.szsharing.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wq.shxzskj.cn

[Q33] 多列分组
来源：http://jr.gzmigu.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://er.gzmigu.cn

[Q34] 每组取第一条
来源：http://ju.muxihuayi.cn

SELECT * FROM (
来源：http://pj.haigaiapp.cn


<!-- 参考信息 -->