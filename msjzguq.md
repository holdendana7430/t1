代发 wailian999

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://lx.yuexingan06.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ft.panjiajie.cn

C#:   // 手写递归，或 Array.Sort
来源：http://rw.hnjuh.cn

[N04] 斐波那契数列
来源：http://bd.nicolike.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://fd.nicolike.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://px.huanxung.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ex.newstarts.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://yc.521024.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://fr.9csxet.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ra.asd995.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://uu.hahajie.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://pl.chemitech.net.cn

[N05] 最大公约数
来源：http://rt.newstarts.cn

Py:   math.gcd(a, b)
来源：http://oz.panjiajie.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wo.yuexingan06.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ia.9csxet.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wz.huixinmuqiang.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://bn.bookmarksfly.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://vo.chemitech.net.cn

Ruby: a.gcd(b)
来源：http://ws.huanxung.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://br.chemitech.net.cn

[N06] 判断回文字符串
来源：http://gr.huixiangedu.cn

Py:   s == s[::-1]
来源：http://oj.521024.cn

PHP:  $s === strrev($s);
来源：http://ym.hnjuh.cn

JS:   s === [...s].reverse().join("")
来源：http://np.hahajie.cn

TS:   s === [...s].reverse().join("")
来源：http://fr.yuntaijiaju.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://vb.wgjwhj.cn

Go:   // 双指针从两端比较
来源：http://ok.gzmigu.cn

Ruby: s == s.reverse
来源：http://im.colortex.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://jk.521024.cn

[N07] 两数之和（返回下标）
来源：http://uj.bookmarksfly.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wh.szxytkj.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ca.huixiangedu.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://fb.huixiangedu.cn

TS:   // 手写 Map<string, number>
来源：http://rg.haigaiapp.cn

Java: // 手写 HashMap
来源：http://qw.gzmigu.cn

Go:   // 手写 map[int]int
来源：http://qn.szsharing.cn

Ruby: // 手写 Hash
来源：http://dv.hahajie.cn

C#:   // 手写 Dictionary<int, int>
来源：http://ri.szxytkj.cn

[N08] 生成全排列
来源：http://nx.colortex.cn

Py:   itertools.permutations(arr)
来源：http://ae.szxytkj.cn

PHP:  // 手写递归交换
来源：http://ys.hnjuh.cn

JS:   // 手写回溯递归
来源：http://ue.asd995.cn

TS:   // 手写回溯递归
来源：http://tq.bookmarksfly.cn

Java: // 手写回溯递归
来源：http://rz.bjjhwx.cn

Go:   // 手写回溯递归
来源：http://pg.gzmigu.cn

Ruby: arr.permutation.to_a
来源：http://ho.gzmigu.cn

C#:   // 手写回溯递归
来源：http://fq.yuexingan06.cn

[N09] 栈与队列
来源：http://fm.szxytkj.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://yi.shxzukj.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://gl.shxzukj.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://aw.jianghongdianzi.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mg.hahajie.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://cz.huixiangedu.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://de.lnxyls.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://qu.hnjuh.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://rt.nicolike.cn

[N10] 链表节点定义
来源：http://dy.nicolike.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://bu.asd995.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://ba.colortex.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://uz.muxihuayi.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://dz.szxytkj.cn

Java: class Node { int v; Node next; }
来源：http://rz.yuntaijiaju.cn

Go:   type Node struct { V int; Next *Node }
来源：http://bz.bookmarksfly.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://et.colortex.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://mq.szsharing.cn

[N11] 二叉树中序遍历
来源：http://sa.panjiajie.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://pj.szxytkj.cn

PHP:  // 手写递归函数
来源：http://yd.bjjhwx.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://yw.colortex.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://cv.shxzskj.cn

Java: // 手写递归
来源：http://tf.9csxet.cn

Go:   // 手写递归
来源：http://zt.haigaiapp.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ji.colortex.cn

C#:   // 手写递归
来源：http://ts.panjiajie.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://fv.yuntaijiaju.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://yf.colortex.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://nr.9csxet.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://my.asd995.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://me.chemitech.net.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://nd.nicolike.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mo.huanxung.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://kp.hahajie.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://bf.newstarts.cn

================================================================================
来源：http://ho.gzmigu.cn

O. 并发与异步
来源：http://ab.asd995.cn

================================================================================
来源：http://nl.newstarts.cn

[O01] 启动一个线程
来源：http://bn.szsharing.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wi.yuntaijiaju.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ma.asd995.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://yy.jianghongdianzi.cn

TS:   // 同 JS
来源：http://lr.lnxyls.cn

Java: new Thread(() -> f()).start()
来源：http://aj.szxytkj.cn

Go:   go f()
来源：http://wd.szxytkj.cn

Ruby: Thread.new { f }
来源：http://se.nszjky.cn

C#:   Task.Run(() => F());
来源：http://ki.9csxet.cn

[O02] 使用线程池
来源：http://fv.asd995.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://cy.huixiangedu.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://iq.huixinmuqiang.cn

JS:   // worker_threads 线程池
来源：http://ve.haigaiapp.cn

TS:   // worker_threads 线程池
来源：http://zs.hahajie.cn

Java: Executors.newFixedThreadPool(4)
来源：http://qd.huixinmuqiang.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://xf.hahajie.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wc.muxihuayi.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://kt.jctech888.com.cn

[O03] 加锁保护共享数据
来源：http://fp.haigaiapp.cn

Py:   with lock: shared += 1
来源：http://qf.panjiajie.cn

PHP:  // 用 flock() 做文件锁
来源：http://er.asd995.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://xo.panjiajie.cn

TS:   // 同 JS
来源：http://nr.shtwfgs.cn

Java: synchronized (this) { shared++; }
来源：http://ii.huixiangedu.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://fm.huixiangedu.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://yf.shxzskj.cn

C#:   lock (gate) { shared++; }
来源：http://pr.521024.cn

[O04] 定义异步函数并等待
来源：http://dz.asd995.cn

Py:   async def f():⏎    await g()
来源：http://lz.szsharing.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://av.shtwfgs.cn

JS:   async function f() { await g(); }
来源：http://xx.bookmarksfly.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://jn.shxzukj.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://uu.wgjwhj.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://js.shxzskj.cn

Ruby: # 用 Fiber 或 async gem
来源：http://rd.haigaiapp.cn

C#:   async Task F() { await G(); }
来源：http://jc.gzmigu.cn

[O05] 并发执行并等待全部完成
来源：http://pc.nszjky.cn

Py:   asyncio.gather(*tasks)
来源：http://dl.bookmarksfly.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://si.muxihuayi.cn

JS:   await Promise.all(tasks)
来源：http://ly.panjiajie.cn

TS:   await Promise.all(tasks)
来源：http://tp.9csxet.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wd.bookmarksfly.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://qc.huanxung.cn

Ruby: threads.map(&:join)
来源：http://am.nszjky.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://jt.huixinmuqiang.cn

[O06] 使用进程池
来源：http://tu.szxytkj.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://lm.bjjhwx.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://zr.yuntaijiaju.cn

JS:   // child_process / cluster 模块
来源：http://zo.hahajie.cn

TS:   // child_process / cluster 模块
来源：http://ex.newstarts.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://dl.shxzskj.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://uv.panjiajie.cn

Ruby: // fork 块
来源：http://up.jctech888.com.cn

C#:   Parallel.For
来源：http://pz.haigaiapp.cn

================================================================================
来源：http://og.gzmigu.cn

P. 常用工具函数
来源：http://hc.9csxet.cn

================================================================================
来源：http://nq.521024.cn

[P01] 生成 UUID
来源：http://ac.bjjhwx.cn

Py:   str(uuid.uuid4())
来源：http://rt.521024.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://jd.nicolike.cn

JS:   crypto.randomUUID()
来源：http://at.bjjhwx.cn

TS:   crypto.randomUUID()
来源：http://de.nicolike.cn

Java: UUID.randomUUID().toString()
来源：http://np.hnjuh.cn

Go:   // 用 github.com/google/uuid
来源：http://bq.hahajie.cn

Ruby: SecureRandom.uuid
来源：http://kl.yuexingan06.cn

C#:   Guid.NewGuid().ToString()
来源：http://mj.haigaiapp.cn

[P02] MD5 / SHA256 摘要
来源：http://qd.yuexingan06.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://fx.bookmarksfly.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://ar.shxzukj.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://it.wgjwhj.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://dt.panjiajie.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://yf.jctech888.com.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://za.wgjwhj.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://vr.nicolike.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://za.gzmigu.cn

[P03] 生成短随机字符串
来源：http://zn.shxzskj.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://qv.newstarts.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://oj.szxytkj.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://oi.newstarts.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://er.muxihuayi.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://zp.yuexingan06.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://jt.gzmigu.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://pc.szxytkj.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://bn.521024.cn

[P04] 求长度
来源：http://qw.521024.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://kj.yuexingan06.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ao.shxzskj.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hu.shtwfgs.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ja.yuntaijiaju.cn

Java: list.size();  map.size();  s.length()
来源：http://rk.huixinmuqiang.cn

Go:   len(arr);  len(m)
来源：http://pc.hnjuh.cn

Ruby: x.length;  x.size
来源：http://vo.bjjhwx.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://kl.wgjwhj.cn

[P05] 判断两个对象内容是否相等
来源：http://vy.shxzukj.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://ck.jianghongdianzi.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://kk.jctech888.com.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://my.shxzukj.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mc.nicolike.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ti.huixinmuqiang.cn

Go:   reflect.DeepEqual(a, b)
来源：http://yo.shxzskj.cn

Ruby: a == b
来源：http://cb.521024.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://kn.shxzskj.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://zc.lnxyls.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://km.huanxung.cn

PHP:  if (empty($x)) {}
来源：http://ra.asd995.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wd.newstarts.cn

TS:   if (x == null) {}
来源：http://xd.huanxung.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://xu.hahajie.cn

Go:   if x == nil {}
来源：http://hc.hnjuh.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://nu.lnxyls.cn

C#:   if (x is null) {}
来源：http://um.yuntaijiaju.cn

[P07] 防抖与节流
来源：http://tc.newstarts.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://az.szxytkj.cn

PHP:  // 手写时间戳比较
来源：http://oj.asd995.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://aa.shxzukj.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qy.panjiajie.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://jw.hnjuh.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://cd.yuntaijiaju.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://oe.szxytkj.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hl.huixiangedu.cn

[P08] 处理浮点精度问题
来源：http://pd.hnjuh.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://nj.jctech888.com.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://gw.wgjwhj.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://tx.shxzskj.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://fe.szsharing.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://fc.haigaiapp.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ov.huixinmuqiang.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://gc.huixiangedu.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://bt.nszjky.cn

================================================================================
来源：http://rj.gzmigu.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ss.nszjky.cn

================================================================================
来源：http://gi.yuexingan06.cn

[Q01] 创建表
来源：http://dq.haigaiapp.cn

CREATE TABLE users (
来源：http://md.szsharing.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://sp.shxzukj.cn

name VARCHAR(50) NOT NULL,
来源：http://au.huixinmuqiang.cn

email VARCHAR(100) UNIQUE,
来源：http://zy.hnjuh.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://vy.muxihuayi.cn

);
来源：http://hd.shxzskj.cn

[Q02] 创建带外键的表
来源：http://tt.jianghongdianzi.cn

CREATE TABLE orders (
来源：http://ug.nicolike.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ub.szxytkj.cn

user_id INT NOT NULL,
来源：http://ib.shxzskj.cn

amount DECIMAL(10, 2),
来源：http://ge.jctech888.com.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://jv.521024.cn

);
来源：http://xi.yuntaijiaju.cn

[Q03] 增加列
来源：http://oc.bjjhwx.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://fg.muxihuayi.cn

[Q04] 修改列类型
来源：http://yq.hahajie.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://nw.shxzskj.cn

[Q05] 重命名列
来源：http://qq.huanxung.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://pk.shtwfgs.cn

[Q06] 删除列
来源：http://qk.panjiajie.cn

ALTER TABLE users DROP COLUMN age;
来源：http://lt.shtwfgs.cn

[Q07] 删除表
来源：http://cp.panjiajie.cn

DROP TABLE IF EXISTS orders;
来源：http://jd.shtwfgs.cn

[Q08] 创建普通索引
来源：http://fl.newstarts.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://vw.gzmigu.cn

[Q09] 创建唯一索引
来源：http://gk.newstarts.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://za.jianghongdianzi.cn

[Q10] 插入单行
来源：http://xc.yuexingan06.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://rm.shxzskj.cn

[Q11] 一次插入多行
来源：http://ct.shxzukj.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://qj.huanxung.cn

[Q12] 插入后取自增 ID
来源：http://dw.chemitech.net.cn

INSERT INTO users (name) VALUES ('C');
来源：http://ml.shxzskj.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://fu.huixiangedu.cn

[Q13] 忽略重复插入
来源：http://lq.asd995.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://vm.chemitech.net.cn

[Q14] 存在则更新（upsert）
来源：http://vo.haigaiapp.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://bk.521024.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ig.shxzukj.cn

[Q15] 查询全部
来源：http://rw.colortex.cn

SELECT * FROM users;
来源：http://pk.muxihuayi.cn

[Q16] 查询指定列
来源：http://ax.nszjky.cn

SELECT id, name FROM users;
来源：http://nk.huanxung.cn

[Q17] 条件查询
来源：http://nn.gzmigu.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://fx.nicolike.cn

[Q18] 模糊匹配
来源：http://ht.haigaiapp.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://gt.yuexingan06.cn

[Q19] 范围查询
来源：http://mw.bjjhwx.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ue.shxzskj.cn

[Q20] IN 列表
来源：http://rx.chemitech.net.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://jp.wgjwhj.cn

[Q21] 空值判断
来源：http://bu.szxytkj.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://hb.huanxung.cn

[Q22] 排序
来源：http://ur.9csxet.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://xl.newstarts.cn

[Q23] 分页
来源：http://sh.asd995.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://oa.nszjky.cn

[Q24] 去重
来源：http://tu.yuexingan06.cn

SELECT DISTINCT city FROM users;
来源：http://uj.chemitech.net.cn

[Q25] 只取前 N 条
来源：http://yv.wgjwhj.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://qt.chemitech.net.cn

[Q26] 计数
来源：http://ri.nszjky.cn

SELECT COUNT(*) FROM users;
来源：http://ny.521024.cn

[Q27] 条件计数
来源：http://xs.521024.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://cy.colortex.cn

[Q28] 求和与平均
来源：http://wc.gzmigu.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://ye.lnxyls.cn

[Q29] 最大最小值
来源：http://ii.bookmarksfly.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://fl.yuntaijiaju.cn

[Q30] 分组统计
来源：http://kl.muxihuayi.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://bm.9csxet.cn

[Q31] 分组后过滤
来源：http://pk.szxytkj.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://cj.nszjky.cn

[Q32] 分组拼接字符串
来源：http://jg.nicolike.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wk.wgjwhj.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://lp.hahajie.cn

[Q33] 多列分组
来源：http://bc.huanxung.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mo.yuexingan06.cn

[Q34] 每组取第一条
来源：http://ey.bookmarksfly.cn

SELECT * FROM (
来源：http://ua.yuntaijiaju.cn


<!-- 参考信息 -->