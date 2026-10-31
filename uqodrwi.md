代发 wailian999

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://jc.gzmigu.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://yq.nicolike.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ku.szxytkj.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://kc.hnjuh.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://iy.haigaiapp.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://lj.yuexingan06.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://kf.wgjwhj.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://xk.shxzukj.cn

[N05] 最大公约数
来源：http://is.huanxung.cn

Py:   math.gcd(a, b)
来源：http://ih.shxzskj.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://jq.hnjuh.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://fg.wgjwhj.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://bb.yuntaijiaju.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://lg.huanxung.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://rd.yuexingan06.cn

Ruby: a.gcd(b)
来源：http://jw.yuntaijiaju.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wo.hnjuh.cn

[N06] 判断回文字符串
来源：http://iz.huixiangedu.cn

Py:   s == s[::-1]
来源：http://yz.bjjhwx.cn

PHP:  $s === strrev($s);
来源：http://ux.gzmigu.cn

JS:   s === [...s].reverse().join("")
来源：http://lv.nicolike.cn

TS:   s === [...s].reverse().join("")
来源：http://rn.huixiangedu.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://lc.hnjuh.cn

Go:   // 双指针从两端比较
来源：http://pf.colortex.cn

Ruby: s == s.reverse
来源：http://ns.colortex.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://zo.asd995.cn

[N07] 两数之和（返回下标）
来源：http://tp.huixinmuqiang.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://sh.muxihuayi.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://de.wgjwhj.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://sy.hnjuh.cn

TS:   // 手写 Map<string, number>
来源：http://xp.jianghongdianzi.cn

Java: // 手写 HashMap
来源：http://lq.jianghongdianzi.cn

Go:   // 手写 map[int]int
来源：http://zn.bookmarksfly.cn

Ruby: // 手写 Hash
来源：http://tn.colortex.cn

C#:   // 手写 Dictionary<int, int>
来源：http://bl.huixiangedu.cn

[N08] 生成全排列
来源：http://ue.szxytkj.cn

Py:   itertools.permutations(arr)
来源：http://pi.huixiangedu.cn

PHP:  // 手写递归交换
来源：http://pz.wgjwhj.cn

JS:   // 手写回溯递归
来源：http://yw.nszjky.cn

TS:   // 手写回溯递归
来源：http://ai.hnjuh.cn

Java: // 手写回溯递归
来源：http://ac.colortex.cn

Go:   // 手写回溯递归
来源：http://rd.jctech888.com.cn

Ruby: arr.permutation.to_a
来源：http://qw.wgjwhj.cn

C#:   // 手写回溯递归
来源：http://ul.bjjhwx.cn

[N09] 栈与队列
来源：http://hj.szsharing.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://da.szsharing.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://xc.szsharing.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://qj.chemitech.net.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wm.panjiajie.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mf.bjjhwx.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://vm.yuntaijiaju.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://qo.szxytkj.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://fo.huixinmuqiang.cn

[N10] 链表节点定义
来源：http://zx.huixiangedu.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://vr.colortex.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://tf.shxzskj.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://oq.haigaiapp.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ia.gzmigu.cn

Java: class Node { int v; Node next; }
来源：http://lh.shxzukj.cn

Go:   type Node struct { V int; Next *Node }
来源：http://xc.yuexingan06.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://yq.9csxet.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://rg.yuntaijiaju.cn

[N11] 二叉树中序遍历
来源：http://yl.muxihuayi.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://gc.chemitech.net.cn

PHP:  // 手写递归函数
来源：http://rp.9csxet.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://tt.bjjhwx.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://sr.shxzskj.cn

Java: // 手写递归
来源：http://pz.nicolike.cn

Go:   // 手写递归
来源：http://ct.521024.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://py.szxytkj.cn

C#:   // 手写递归
来源：http://mw.haigaiapp.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://rk.yuntaijiaju.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://uh.nszjky.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ud.huixinmuqiang.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://om.colortex.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://zc.huanxung.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://cx.9csxet.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://cb.colortex.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://vu.jianghongdianzi.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://xh.shxzskj.cn

================================================================================
来源：http://ev.newstarts.cn

O. 并发与异步
来源：http://kv.hahajie.cn

================================================================================
来源：http://yp.jianghongdianzi.cn

[O01] 启动一个线程
来源：http://nw.gzmigu.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://np.bjjhwx.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://xn.shxzukj.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ik.bookmarksfly.cn

TS:   // 同 JS
来源：http://vr.jianghongdianzi.cn

Java: new Thread(() -> f()).start()
来源：http://ek.szxytkj.cn

Go:   go f()
来源：http://ky.yuntaijiaju.cn

Ruby: Thread.new { f }
来源：http://si.muxihuayi.cn

C#:   Task.Run(() => F());
来源：http://xm.huanxung.cn

[O02] 使用线程池
来源：http://ud.9csxet.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://bs.asd995.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://lx.shxzukj.cn

JS:   // worker_threads 线程池
来源：http://jm.bjjhwx.cn

TS:   // worker_threads 线程池
来源：http://ps.gzmigu.cn

Java: Executors.newFixedThreadPool(4)
来源：http://mi.huixiangedu.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://cf.shtwfgs.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://fd.yuntaijiaju.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://gx.colortex.cn

[O03] 加锁保护共享数据
来源：http://wc.haigaiapp.cn

Py:   with lock: shared += 1
来源：http://vg.asd995.cn

PHP:  // 用 flock() 做文件锁
来源：http://ua.szsharing.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ar.haigaiapp.cn

TS:   // 同 JS
来源：http://wc.shxzukj.cn

Java: synchronized (this) { shared++; }
来源：http://kc.shxzukj.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://rc.panjiajie.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://hd.9csxet.cn

C#:   lock (gate) { shared++; }
来源：http://ux.shxzskj.cn

[O04] 定义异步函数并等待
来源：http://xr.lnxyls.cn

Py:   async def f():⏎    await g()
来源：http://ju.szxytkj.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://bh.szsharing.cn

JS:   async function f() { await g(); }
来源：http://ll.panjiajie.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://mr.jianghongdianzi.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://eb.shxzukj.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://lz.hnjuh.cn

Ruby: # 用 Fiber 或 async gem
来源：http://hp.shxzukj.cn

C#:   async Task F() { await G(); }
来源：http://om.bjjhwx.cn

[O05] 并发执行并等待全部完成
来源：http://rw.jctech888.com.cn

Py:   asyncio.gather(*tasks)
来源：http://yg.nszjky.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://sn.hahajie.cn

JS:   await Promise.all(tasks)
来源：http://ny.521024.cn

TS:   await Promise.all(tasks)
来源：http://go.wgjwhj.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ii.colortex.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://tn.shxzskj.cn

Ruby: threads.map(&:join)
来源：http://lr.panjiajie.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://pd.hahajie.cn

[O06] 使用进程池
来源：http://xb.bjjhwx.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://yw.jianghongdianzi.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://uh.shxzukj.cn

JS:   // child_process / cluster 模块
来源：http://rl.shxzukj.cn

TS:   // child_process / cluster 模块
来源：http://mw.haigaiapp.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ql.newstarts.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ff.chemitech.net.cn

Ruby: // fork 块
来源：http://vq.yuntaijiaju.cn

C#:   Parallel.For
来源：http://ef.9csxet.cn

================================================================================
来源：http://gd.bjjhwx.cn

P. 常用工具函数
来源：http://wi.yuntaijiaju.cn

================================================================================
来源：http://it.haigaiapp.cn

[P01] 生成 UUID
来源：http://gp.asd995.cn

Py:   str(uuid.uuid4())
来源：http://hd.wgjwhj.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://tj.szxytkj.cn

JS:   crypto.randomUUID()
来源：http://xh.hahajie.cn

TS:   crypto.randomUUID()
来源：http://wn.nicolike.cn

Java: UUID.randomUUID().toString()
来源：http://gs.huanxung.cn

Go:   // 用 github.com/google/uuid
来源：http://ji.lnxyls.cn

Ruby: SecureRandom.uuid
来源：http://or.jctech888.com.cn

C#:   Guid.NewGuid().ToString()
来源：http://xl.yuexingan06.cn

[P02] MD5 / SHA256 摘要
来源：http://ok.shxzskj.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://sf.szxytkj.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://yg.shxzskj.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ou.haigaiapp.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mi.bjjhwx.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://tg.hahajie.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://od.bookmarksfly.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://gz.haigaiapp.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hr.9csxet.cn

[P03] 生成短随机字符串
来源：http://rj.huanxung.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://iz.haigaiapp.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://lt.asd995.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://im.lnxyls.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ll.jctech888.com.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://de.jctech888.com.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://pz.huixinmuqiang.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://mw.szxytkj.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mv.9csxet.cn

[P04] 求长度
来源：http://mo.hnjuh.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://cj.haigaiapp.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://xx.nszjky.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://yj.huixinmuqiang.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://lb.huixiangedu.cn

Java: list.size();  map.size();  s.length()
来源：http://zz.huanxung.cn

Go:   len(arr);  len(m)
来源：http://eo.haigaiapp.cn

Ruby: x.length;  x.size
来源：http://ff.szsharing.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://sz.bookmarksfly.cn

[P05] 判断两个对象内容是否相等
来源：http://wk.shxzukj.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://ix.bookmarksfly.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ee.yuexingan06.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://fn.shtwfgs.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ch.newstarts.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://na.jctech888.com.cn

Go:   reflect.DeepEqual(a, b)
来源：http://xq.lnxyls.cn

Ruby: a == b
来源：http://au.panjiajie.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://xf.huixinmuqiang.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hy.haigaiapp.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://gk.9csxet.cn

PHP:  if (empty($x)) {}
来源：http://vg.asd995.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://dx.huanxung.cn

TS:   if (x == null) {}
来源：http://hp.jctech888.com.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://ao.lnxyls.cn

Go:   if x == nil {}
来源：http://pe.bookmarksfly.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mh.hnjuh.cn

C#:   if (x is null) {}
来源：http://yn.nicolike.cn

[P07] 防抖与节流
来源：http://ix.9csxet.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ho.haigaiapp.cn

PHP:  // 手写时间戳比较
来源：http://hq.huixiangedu.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ri.jianghongdianzi.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://vc.yuexingan06.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ba.nicolike.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://oz.shxzskj.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://db.521024.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://bf.huixinmuqiang.cn

[P08] 处理浮点精度问题
来源：http://es.bjjhwx.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://pn.bjjhwx.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ax.yuexingan06.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://qj.bjjhwx.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://gn.wgjwhj.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://rk.hahajie.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://vy.chemitech.net.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://xx.hahajie.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ci.jianghongdianzi.cn

================================================================================
来源：http://mn.nicolike.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ob.521024.cn

================================================================================
来源：http://zu.yuntaijiaju.cn

[Q01] 创建表
来源：http://gf.szxytkj.cn

CREATE TABLE users (
来源：http://pp.bjjhwx.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://dz.9csxet.cn

name VARCHAR(50) NOT NULL,
来源：http://aa.521024.cn

email VARCHAR(100) UNIQUE,
来源：http://tv.szxytkj.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://xe.gzmigu.cn

);
来源：http://nj.chemitech.net.cn

[Q02] 创建带外键的表
来源：http://yv.colortex.cn

CREATE TABLE orders (
来源：http://fg.gzmigu.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mj.nszjky.cn

user_id INT NOT NULL,
来源：http://vj.haigaiapp.cn

amount DECIMAL(10, 2),
来源：http://ux.panjiajie.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mi.lnxyls.cn

);
来源：http://nl.panjiajie.cn

[Q03] 增加列
来源：http://nj.521024.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://fi.shxzskj.cn

[Q04] 修改列类型
来源：http://bl.9csxet.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://yo.asd995.cn

[Q05] 重命名列
来源：http://ll.yuexingan06.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mz.bookmarksfly.cn

[Q06] 删除列
来源：http://qg.shxzukj.cn

ALTER TABLE users DROP COLUMN age;
来源：http://uk.szsharing.cn

[Q07] 删除表
来源：http://at.asd995.cn

DROP TABLE IF EXISTS orders;
来源：http://dx.jctech888.com.cn

[Q08] 创建普通索引
来源：http://re.521024.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://rk.huixinmuqiang.cn

[Q09] 创建唯一索引
来源：http://mn.shtwfgs.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://qc.lnxyls.cn

[Q10] 插入单行
来源：http://zl.szsharing.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://rc.gzmigu.cn

[Q11] 一次插入多行
来源：http://ld.9csxet.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://gi.jianghongdianzi.cn

[Q12] 插入后取自增 ID
来源：http://wy.panjiajie.cn

INSERT INTO users (name) VALUES ('C');
来源：http://ia.chemitech.net.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ju.haigaiapp.cn

[Q13] 忽略重复插入
来源：http://pp.shxzukj.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://vv.nicolike.cn

[Q14] 存在则更新（upsert）
来源：http://ii.jianghongdianzi.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://dn.hnjuh.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ll.panjiajie.cn

[Q15] 查询全部
来源：http://la.asd995.cn

SELECT * FROM users;
来源：http://kf.szsharing.cn

[Q16] 查询指定列
来源：http://pz.huixiangedu.cn

SELECT id, name FROM users;
来源：http://uz.yuexingan06.cn

[Q17] 条件查询
来源：http://kq.muxihuayi.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://jn.newstarts.cn

[Q18] 模糊匹配
来源：http://gp.yuntaijiaju.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://fb.huixinmuqiang.cn

[Q19] 范围查询
来源：http://me.yuntaijiaju.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://yx.huixiangedu.cn

[Q20] IN 列表
来源：http://ul.szsharing.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://nq.yuntaijiaju.cn

[Q21] 空值判断
来源：http://bi.szxytkj.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://ac.shtwfgs.cn

[Q22] 排序
来源：http://ka.9csxet.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://tr.jianghongdianzi.cn

[Q23] 分页
来源：http://hd.bjjhwx.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wl.huanxung.cn

[Q24] 去重
来源：http://dk.yuexingan06.cn

SELECT DISTINCT city FROM users;
来源：http://at.lnxyls.cn

[Q25] 只取前 N 条
来源：http://cu.nicolike.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://um.jctech888.com.cn

[Q26] 计数
来源：http://tx.wgjwhj.cn

SELECT COUNT(*) FROM users;
来源：http://yy.yuexingan06.cn

[Q27] 条件计数
来源：http://oc.huixiangedu.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://dp.chemitech.net.cn

[Q28] 求和与平均
来源：http://vk.jianghongdianzi.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://zy.asd995.cn

[Q29] 最大最小值
来源：http://fz.jianghongdianzi.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://zc.bookmarksfly.cn

[Q30] 分组统计
来源：http://im.asd995.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://rj.haigaiapp.cn

[Q31] 分组后过滤
来源：http://li.huixinmuqiang.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://zm.szxytkj.cn

[Q32] 分组拼接字符串
来源：http://ka.jianghongdianzi.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://gx.lnxyls.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://nu.asd995.cn

[Q33] 多列分组
来源：http://kw.jianghongdianzi.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://xx.chemitech.net.cn

[Q34] 每组取第一条
来源：http://ou.muxihuayi.cn

SELECT * FROM (
来源：http://kd.shxzskj.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wm.bookmarksfly.cn

) t WHERE rn = 1;
来源：http://jj.huanxung.cn

[Q35] 内连接
来源：http://tp.panjiajie.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ma.huanxung.cn


<!-- 参考信息 -->