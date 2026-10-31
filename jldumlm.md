代发 wailian999

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ir.shtwfgs.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://xa.shxzukj.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ew.nszjky.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://yw.shtwfgs.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://kv.haigaiapp.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wa.shxzskj.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://bc.bookmarksfly.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ls.panjiajie.cn

[N05] 最大公约数
来源：http://yp.jctech888.com.cn

Py:   math.gcd(a, b)
来源：http://fj.lnxyls.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://bo.nicolike.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://xd.colortex.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://lc.haigaiapp.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://du.hahajie.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ml.bookmarksfly.cn

Ruby: a.gcd(b)
来源：http://ts.shxzukj.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ei.colortex.cn

[N06] 判断回文字符串
来源：http://jr.jianghongdianzi.cn

Py:   s == s[::-1]
来源：http://ma.szxytkj.cn

PHP:  $s === strrev($s);
来源：http://wh.szsharing.cn

JS:   s === [...s].reverse().join("")
来源：http://vy.muxihuayi.cn

TS:   s === [...s].reverse().join("")
来源：http://xp.huixinmuqiang.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://bn.haigaiapp.cn

Go:   // 双指针从两端比较
来源：http://cz.huixiangedu.cn

Ruby: s == s.reverse
来源：http://jb.9csxet.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://sw.huanxung.cn

[N07] 两数之和（返回下标）
来源：http://tu.bookmarksfly.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://fv.colortex.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://yp.colortex.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://gr.bookmarksfly.cn

TS:   // 手写 Map<string, number>
来源：http://od.shxzukj.cn

Java: // 手写 HashMap
来源：http://xe.panjiajie.cn

Go:   // 手写 map[int]int
来源：http://ff.jctech888.com.cn

Ruby: // 手写 Hash
来源：http://vf.yuntaijiaju.cn

C#:   // 手写 Dictionary<int, int>
来源：http://dj.gzmigu.cn

[N08] 生成全排列
来源：http://yh.wgjwhj.cn

Py:   itertools.permutations(arr)
来源：http://fx.panjiajie.cn

PHP:  // 手写递归交换
来源：http://tm.lnxyls.cn

JS:   // 手写回溯递归
来源：http://or.huixinmuqiang.cn

TS:   // 手写回溯递归
来源：http://ug.shxzukj.cn

Java: // 手写回溯递归
来源：http://uq.chemitech.net.cn

Go:   // 手写回溯递归
来源：http://ys.nicolike.cn

Ruby: arr.permutation.to_a
来源：http://qn.shxzukj.cn

C#:   // 手写回溯递归
来源：http://bh.gzmigu.cn

[N09] 栈与队列
来源：http://jn.hnjuh.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://aa.jctech888.com.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://im.huixiangedu.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wk.panjiajie.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://fh.yuexingan06.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.hahajie.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://nz.colortex.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://km.yuntaijiaju.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://my.colortex.cn

[N10] 链表节点定义
来源：http://hr.jctech888.com.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ra.szsharing.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://qk.bjjhwx.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wc.szxytkj.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://zo.newstarts.cn

Java: class Node { int v; Node next; }
来源：http://qb.jctech888.com.cn

Go:   type Node struct { V int; Next *Node }
来源：http://jz.yuexingan06.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://xw.hahajie.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://yv.jianghongdianzi.cn

[N11] 二叉树中序遍历
来源：http://yq.shxzskj.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ct.shxzskj.cn

PHP:  // 手写递归函数
来源：http://tg.szxytkj.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://tw.gzmigu.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://zz.huixiangedu.cn

Java: // 手写递归
来源：http://fb.shxzukj.cn

Go:   // 手写递归
来源：http://pr.gzmigu.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ry.shxzukj.cn

C#:   // 手写递归
来源：http://jc.chemitech.net.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://er.colortex.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://fq.muxihuayi.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://yh.bookmarksfly.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://yf.jctech888.com.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://cd.szsharing.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://cc.nicolike.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://sp.huixiangedu.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://jj.521024.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://zj.nszjky.cn

================================================================================
来源：http://ay.521024.cn

O. 并发与异步
来源：http://vm.jianghongdianzi.cn

================================================================================
来源：http://ze.jianghongdianzi.cn

[O01] 启动一个线程
来源：http://ad.yuexingan06.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://jn.szsharing.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://nq.jctech888.com.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://rj.wgjwhj.cn

TS:   // 同 JS
来源：http://nn.gzmigu.cn

Java: new Thread(() -> f()).start()
来源：http://du.wgjwhj.cn

Go:   go f()
来源：http://di.bjjhwx.cn

Ruby: Thread.new { f }
来源：http://fs.panjiajie.cn

C#:   Task.Run(() => F());
来源：http://sz.nszjky.cn

[O02] 使用线程池
来源：http://qp.nicolike.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://sy.panjiajie.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://qu.asd995.cn

JS:   // worker_threads 线程池
来源：http://eo.colortex.cn

TS:   // worker_threads 线程池
来源：http://bo.huixiangedu.cn

Java: Executors.newFixedThreadPool(4)
来源：http://xy.bjjhwx.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://se.wgjwhj.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mm.nszjky.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://dd.szxytkj.cn

[O03] 加锁保护共享数据
来源：http://oq.huixinmuqiang.cn

Py:   with lock: shared += 1
来源：http://sp.colortex.cn

PHP:  // 用 flock() 做文件锁
来源：http://uh.hahajie.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ro.nicolike.cn

TS:   // 同 JS
来源：http://la.szxytkj.cn

Java: synchronized (this) { shared++; }
来源：http://jf.shtwfgs.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://eb.panjiajie.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://qh.colortex.cn

C#:   lock (gate) { shared++; }
来源：http://cp.521024.cn

[O04] 定义异步函数并等待
来源：http://op.jctech888.com.cn

Py:   async def f():⏎    await g()
来源：http://gm.nszjky.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://gl.lnxyls.cn

JS:   async function f() { await g(); }
来源：http://zl.nszjky.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://oz.shxzskj.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mg.bjjhwx.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://od.shtwfgs.cn

Ruby: # 用 Fiber 或 async gem
来源：http://tq.muxihuayi.cn

C#:   async Task F() { await G(); }
来源：http://hn.nszjky.cn

[O05] 并发执行并等待全部完成
来源：http://gc.haigaiapp.cn

Py:   asyncio.gather(*tasks)
来源：http://oy.panjiajie.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://bh.newstarts.cn

JS:   await Promise.all(tasks)
来源：http://yg.haigaiapp.cn

TS:   await Promise.all(tasks)
来源：http://jh.yuexingan06.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://pj.wgjwhj.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mn.shxzskj.cn

Ruby: threads.map(&:join)
来源：http://dd.haigaiapp.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://mh.bookmarksfly.cn

[O06] 使用进程池
来源：http://jy.lnxyls.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mu.szsharing.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://ho.asd995.cn

JS:   // child_process / cluster 模块
来源：http://li.bjjhwx.cn

TS:   // child_process / cluster 模块
来源：http://qc.shxzskj.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://nd.521024.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://qg.huixinmuqiang.cn

Ruby: // fork 块
来源：http://ri.hahajie.cn

C#:   Parallel.For
来源：http://zv.huanxung.cn

================================================================================
来源：http://uj.shtwfgs.cn

P. 常用工具函数
来源：http://bx.jctech888.com.cn

================================================================================
来源：http://ak.jianghongdianzi.cn

[P01] 生成 UUID
来源：http://ng.bookmarksfly.cn

Py:   str(uuid.uuid4())
来源：http://ky.huixiangedu.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://zu.huanxung.cn

JS:   crypto.randomUUID()
来源：http://ek.521024.cn

TS:   crypto.randomUUID()
来源：http://wh.yuntaijiaju.cn

Java: UUID.randomUUID().toString()
来源：http://at.bookmarksfly.cn

Go:   // 用 github.com/google/uuid
来源：http://fi.wgjwhj.cn

Ruby: SecureRandom.uuid
来源：http://nw.gzmigu.cn

C#:   Guid.NewGuid().ToString()
来源：http://uw.szxytkj.cn

[P02] MD5 / SHA256 摘要
来源：http://sf.colortex.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://zg.colortex.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://qr.newstarts.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ek.szsharing.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://lv.panjiajie.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://dm.szxytkj.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://lr.asd995.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://tw.shxzskj.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://rn.szxytkj.cn

[P03] 生成短随机字符串
来源：http://ez.yuexingan06.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mi.panjiajie.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://io.jianghongdianzi.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ja.colortex.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://su.huixinmuqiang.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://zb.hahajie.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ap.chemitech.net.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://ey.huanxung.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://bt.521024.cn

[P04] 求长度
来源：http://ej.shxzukj.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://tj.hnjuh.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://qt.szxytkj.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ii.muxihuayi.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://zs.muxihuayi.cn

Java: list.size();  map.size();  s.length()
来源：http://xb.nszjky.cn

Go:   len(arr);  len(m)
来源：http://rx.huixinmuqiang.cn

Ruby: x.length;  x.size
来源：http://ar.szxytkj.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://xy.yuntaijiaju.cn

[P05] 判断两个对象内容是否相等
来源：http://ui.nszjky.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://sm.9csxet.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://xs.9csxet.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ha.bjjhwx.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ih.jctech888.com.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://fj.panjiajie.cn

Go:   reflect.DeepEqual(a, b)
来源：http://sz.haigaiapp.cn

Ruby: a == b
来源：http://op.asd995.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://lz.huanxung.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://jg.colortex.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ja.szxytkj.cn

PHP:  if (empty($x)) {}
来源：http://tc.wgjwhj.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mn.panjiajie.cn

TS:   if (x == null) {}
来源：http://tp.huixinmuqiang.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://kj.nicolike.cn

Go:   if x == nil {}
来源：http://hg.huixiangedu.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mm.bookmarksfly.cn

C#:   if (x is null) {}
来源：http://fu.bjjhwx.cn

[P07] 防抖与节流
来源：http://ed.jctech888.com.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://pk.lnxyls.cn

PHP:  // 手写时间戳比较
来源：http://ag.nicolike.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://my.yuexingan06.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://vz.colortex.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://co.hnjuh.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://na.asd995.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://ec.muxihuayi.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://iv.yuexingan06.cn

[P08] 处理浮点精度问题
来源：http://tu.hahajie.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://jw.yuntaijiaju.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://cn.wgjwhj.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://tt.lnxyls.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://aa.huixinmuqiang.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://nx.bjjhwx.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ok.9csxet.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://is.jianghongdianzi.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://sy.521024.cn

================================================================================
来源：http://bx.asd995.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://rq.wgjwhj.cn

================================================================================
来源：http://ih.szxytkj.cn

[Q01] 创建表
来源：http://ip.colortex.cn

CREATE TABLE users (
来源：http://rl.lnxyls.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://if.asd995.cn

name VARCHAR(50) NOT NULL,
来源：http://nf.shxzskj.cn

email VARCHAR(100) UNIQUE,
来源：http://no.bookmarksfly.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://dg.muxihuayi.cn

);
来源：http://mk.huixiangedu.cn

[Q02] 创建带外键的表
来源：http://hn.szsharing.cn

CREATE TABLE orders (
来源：http://qh.nszjky.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://fy.nicolike.cn

user_id INT NOT NULL,
来源：http://ab.521024.cn

amount DECIMAL(10, 2),
来源：http://ot.panjiajie.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://um.muxihuayi.cn

);
来源：http://gj.bookmarksfly.cn

[Q03] 增加列
来源：http://dm.colortex.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mn.9csxet.cn

[Q04] 修改列类型
来源：http://lv.wgjwhj.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mh.9csxet.cn

[Q05] 重命名列
来源：http://fy.wgjwhj.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://xl.gzmigu.cn

[Q06] 删除列
来源：http://ni.hahajie.cn

ALTER TABLE users DROP COLUMN age;
来源：http://ei.szsharing.cn

[Q07] 删除表
来源：http://vp.shxzukj.cn

DROP TABLE IF EXISTS orders;
来源：http://hb.chemitech.net.cn

[Q08] 创建普通索引
来源：http://lb.jianghongdianzi.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://mg.shxzskj.cn

[Q09] 创建唯一索引
来源：http://og.hahajie.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ch.bjjhwx.cn

[Q10] 插入单行
来源：http://fn.shtwfgs.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wv.shxzukj.cn

[Q11] 一次插入多行
来源：http://zw.szxytkj.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://qe.asd995.cn

[Q12] 插入后取自增 ID
来源：http://dh.asd995.cn

INSERT INTO users (name) VALUES ('C');
来源：http://bv.lnxyls.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://zt.huanxung.cn

[Q13] 忽略重复插入
来源：http://pg.bookmarksfly.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://dj.yuexingan06.cn

[Q14] 存在则更新（upsert）
来源：http://eg.lnxyls.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://qz.muxihuayi.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://xm.huixinmuqiang.cn

[Q15] 查询全部
来源：http://qu.gzmigu.cn

SELECT * FROM users;
来源：http://de.muxihuayi.cn

[Q16] 查询指定列
来源：http://mk.hahajie.cn

SELECT id, name FROM users;
来源：http://rm.nicolike.cn

[Q17] 条件查询
来源：http://ki.nicolike.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wg.yuexingan06.cn

[Q18] 模糊匹配
来源：http://da.panjiajie.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ss.521024.cn

[Q19] 范围查询
来源：http://lp.bjjhwx.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hh.huanxung.cn

[Q20] IN 列表
来源：http://rg.bookmarksfly.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://br.huixinmuqiang.cn

[Q21] 空值判断
来源：http://ta.muxihuayi.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://be.nicolike.cn

[Q22] 排序
来源：http://pv.shxzukj.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wy.shxzskj.cn

[Q23] 分页
来源：http://tm.muxihuayi.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ci.nicolike.cn

[Q24] 去重
来源：http://bv.521024.cn

SELECT DISTINCT city FROM users;
来源：http://ia.muxihuayi.cn

[Q25] 只取前 N 条
来源：http://yo.panjiajie.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://uy.bookmarksfly.cn

[Q26] 计数
来源：http://ve.szxytkj.cn

SELECT COUNT(*) FROM users;
来源：http://nn.521024.cn

[Q27] 条件计数
来源：http://hn.newstarts.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://op.szxytkj.cn

[Q28] 求和与平均
来源：http://nn.szxytkj.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://st.hnjuh.cn

[Q29] 最大最小值
来源：http://bp.hahajie.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://pe.newstarts.cn

[Q30] 分组统计
来源：http://tz.521024.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hn.huanxung.cn

[Q31] 分组后过滤
来源：http://rz.yuexingan06.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ur.colortex.cn

[Q32] 分组拼接字符串
来源：http://cn.bookmarksfly.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://eb.bjjhwx.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://lw.jctech888.com.cn

[Q33] 多列分组
来源：http://zc.huixinmuqiang.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://jl.colortex.cn

[Q34] 每组取第一条
来源：http://vm.gzmigu.cn

SELECT * FROM (
来源：http://jk.lnxyls.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://lf.bjjhwx.cn

) t WHERE rn = 1;
来源：http://oh.chemitech.net.cn

[Q35] 内连接
来源：http://nx.colortex.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ko.nszjky.cn


<!-- 参考信息 -->