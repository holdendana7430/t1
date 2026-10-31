代发 wailian999

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://jw.jianghongdianzi.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://fr.shxzskj.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://eh.521024.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ip.bjjhwx.cn

[N05] 最大公约数
来源：http://kt.haigaiapp.cn

Py:   math.gcd(a, b)
来源：http://nu.nszjky.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://an.shtwfgs.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ds.panjiajie.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://sh.shxzskj.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hi.shtwfgs.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://vt.huixiangedu.cn

Ruby: a.gcd(b)
来源：http://tk.shtwfgs.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://zd.jctech888.com.cn

[N06] 判断回文字符串
来源：http://kk.shtwfgs.cn

Py:   s == s[::-1]
来源：http://qp.panjiajie.cn

PHP:  $s === strrev($s);
来源：http://ah.521024.cn

JS:   s === [...s].reverse().join("")
来源：http://vj.bjjhwx.cn

TS:   s === [...s].reverse().join("")
来源：http://ub.panjiajie.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ig.szsharing.cn

Go:   // 双指针从两端比较
来源：http://mr.huanxung.cn

Ruby: s == s.reverse
来源：http://sa.szsharing.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://ix.9csxet.cn

[N07] 两数之和（返回下标）
来源：http://xi.szxytkj.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://gg.jctech888.com.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://nt.colortex.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://zd.jctech888.com.cn

TS:   // 手写 Map<string, number>
来源：http://vz.wgjwhj.cn

Java: // 手写 HashMap
来源：http://he.muxihuayi.cn

Go:   // 手写 map[int]int
来源：http://rq.muxihuayi.cn

Ruby: // 手写 Hash
来源：http://ts.9csxet.cn

C#:   // 手写 Dictionary<int, int>
来源：http://zj.colortex.cn

[N08] 生成全排列
来源：http://xs.huixinmuqiang.cn

Py:   itertools.permutations(arr)
来源：http://qt.hahajie.cn

PHP:  // 手写递归交换
来源：http://qm.9csxet.cn

JS:   // 手写回溯递归
来源：http://ta.szxytkj.cn

TS:   // 手写回溯递归
来源：http://bm.haigaiapp.cn

Java: // 手写回溯递归
来源：http://dh.colortex.cn

Go:   // 手写回溯递归
来源：http://ku.asd995.cn

Ruby: arr.permutation.to_a
来源：http://ax.nszjky.cn

C#:   // 手写回溯递归
来源：http://ug.chemitech.net.cn

[N09] 栈与队列
来源：http://wq.shxzukj.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://yo.chemitech.net.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://cc.shxzukj.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://pt.shtwfgs.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ag.shxzskj.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://dc.chemitech.net.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://sa.hnjuh.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ll.jctech888.com.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://sw.shxzskj.cn

[N10] 链表节点定义
来源：http://oz.colortex.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mg.asd995.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://my.jctech888.com.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://dd.huixinmuqiang.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://pw.huixiangedu.cn

Java: class Node { int v; Node next; }
来源：http://dl.yuntaijiaju.cn

Go:   type Node struct { V int; Next *Node }
来源：http://lq.521024.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://ol.huanxung.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://uu.bjjhwx.cn

[N11] 二叉树中序遍历
来源：http://sa.szsharing.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://sr.colortex.cn

PHP:  // 手写递归函数
来源：http://wc.huixinmuqiang.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ld.bookmarksfly.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ik.jctech888.com.cn

Java: // 手写递归
来源：http://va.gzmigu.cn

Go:   // 手写递归
来源：http://gi.muxihuayi.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://fh.9csxet.cn

C#:   // 手写递归
来源：http://ee.shxzukj.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://rj.huanxung.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://nu.wgjwhj.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mr.huixinmuqiang.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wo.asd995.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ub.shxzukj.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://pm.nicolike.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://vg.haigaiapp.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://cv.wgjwhj.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://xd.newstarts.cn

================================================================================
来源：http://xc.bjjhwx.cn

O. 并发与异步
来源：http://cz.jctech888.com.cn

================================================================================
来源：http://bd.nszjky.cn

[O01] 启动一个线程
来源：http://uj.muxihuayi.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ia.hnjuh.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://bk.lnxyls.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://fn.bookmarksfly.cn

TS:   // 同 JS
来源：http://ck.newstarts.cn

Java: new Thread(() -> f()).start()
来源：http://vy.muxihuayi.cn

Go:   go f()
来源：http://on.colortex.cn

Ruby: Thread.new { f }
来源：http://vz.colortex.cn

C#:   Task.Run(() => F());
来源：http://iy.newstarts.cn

[O02] 使用线程池
来源：http://ky.shxzskj.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://pq.lnxyls.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wt.jianghongdianzi.cn

JS:   // worker_threads 线程池
来源：http://wk.colortex.cn

TS:   // worker_threads 线程池
来源：http://za.nicolike.cn

Java: Executors.newFixedThreadPool(4)
来源：http://sp.9csxet.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://zd.nszjky.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://da.shtwfgs.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://bi.yuntaijiaju.cn

[O03] 加锁保护共享数据
来源：http://wp.yuexingan06.cn

Py:   with lock: shared += 1
来源：http://np.asd995.cn

PHP:  // 用 flock() 做文件锁
来源：http://zm.bjjhwx.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://rh.panjiajie.cn

TS:   // 同 JS
来源：http://yr.newstarts.cn

Java: synchronized (this) { shared++; }
来源：http://ck.bookmarksfly.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://cm.9csxet.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://pt.shtwfgs.cn

C#:   lock (gate) { shared++; }
来源：http://no.haigaiapp.cn

[O04] 定义异步函数并等待
来源：http://cq.huixinmuqiang.cn

Py:   async def f():⏎    await g()
来源：http://ip.szxytkj.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ci.hahajie.cn

JS:   async function f() { await g(); }
来源：http://ci.nicolike.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://ri.yuexingan06.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wh.huixiangedu.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://au.9csxet.cn

Ruby: # 用 Fiber 或 async gem
来源：http://zs.panjiajie.cn

C#:   async Task F() { await G(); }
来源：http://km.szsharing.cn

[O05] 并发执行并等待全部完成
来源：http://wo.hnjuh.cn

Py:   asyncio.gather(*tasks)
来源：http://mu.szxytkj.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ks.szxytkj.cn

JS:   await Promise.all(tasks)
来源：http://bh.bjjhwx.cn

TS:   await Promise.all(tasks)
来源：http://sa.jianghongdianzi.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://zz.jianghongdianzi.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wq.bookmarksfly.cn

Ruby: threads.map(&:join)
来源：http://ob.chemitech.net.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://qt.huixinmuqiang.cn

[O06] 使用进程池
来源：http://ik.hnjuh.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://kb.haigaiapp.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://xa.colortex.cn

JS:   // child_process / cluster 模块
来源：http://hs.nszjky.cn

TS:   // child_process / cluster 模块
来源：http://dt.gzmigu.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://zd.jianghongdianzi.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ro.chemitech.net.cn

Ruby: // fork 块
来源：http://tl.shxzukj.cn

C#:   Parallel.For
来源：http://kc.jctech888.com.cn

================================================================================
来源：http://ug.gzmigu.cn

P. 常用工具函数
来源：http://mn.jianghongdianzi.cn

================================================================================
来源：http://wa.shtwfgs.cn

[P01] 生成 UUID
来源：http://bs.szsharing.cn

Py:   str(uuid.uuid4())
来源：http://ze.hahajie.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://nb.hnjuh.cn

JS:   crypto.randomUUID()
来源：http://ht.huixinmuqiang.cn

TS:   crypto.randomUUID()
来源：http://ox.nicolike.cn

Java: UUID.randomUUID().toString()
来源：http://mm.yuntaijiaju.cn

Go:   // 用 github.com/google/uuid
来源：http://ma.lnxyls.cn

Ruby: SecureRandom.uuid
来源：http://ew.hahajie.cn

C#:   Guid.NewGuid().ToString()
来源：http://vb.newstarts.cn

[P02] MD5 / SHA256 摘要
来源：http://xf.muxihuayi.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://xd.yuntaijiaju.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://js.shtwfgs.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://lq.asd995.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ek.newstarts.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://gw.haigaiapp.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://om.yuntaijiaju.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://en.szsharing.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ar.shxzskj.cn

[P03] 生成短随机字符串
来源：http://nx.jctech888.com.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://zt.huanxung.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://xa.shxzskj.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://kq.huixiangedu.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://gu.9csxet.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://lw.hnjuh.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://lz.shtwfgs.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.shxzskj.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ez.muxihuayi.cn

[P04] 求长度
来源：http://to.colortex.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://zq.asd995.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://sb.bjjhwx.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://qa.asd995.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://jy.huixinmuqiang.cn

Java: list.size();  map.size();  s.length()
来源：http://mf.shxzskj.cn

Go:   len(arr);  len(m)
来源：http://hv.shxzukj.cn

Ruby: x.length;  x.size
来源：http://oz.nicolike.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://jp.bjjhwx.cn

[P05] 判断两个对象内容是否相等
来源：http://ku.jianghongdianzi.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://tv.huixiangedu.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://yf.hnjuh.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://bf.newstarts.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://xl.jctech888.com.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://nw.huanxung.cn

Go:   reflect.DeepEqual(a, b)
来源：http://sv.nszjky.cn

Ruby: a == b
来源：http://op.bjjhwx.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://tj.hahajie.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://xi.521024.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://kr.hnjuh.cn

PHP:  if (empty($x)) {}
来源：http://np.szsharing.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://gy.shxzskj.cn

TS:   if (x == null) {}
来源：http://yd.9csxet.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://re.yuntaijiaju.cn

Go:   if x == nil {}
来源：http://ab.yuntaijiaju.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://tr.shtwfgs.cn

C#:   if (x is null) {}
来源：http://ik.bookmarksfly.cn

[P07] 防抖与节流
来源：http://hx.shxzukj.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://it.hnjuh.cn

PHP:  // 手写时间戳比较
来源：http://pf.huanxung.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://bq.wgjwhj.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://pu.huixinmuqiang.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://yh.bjjhwx.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://zi.huixiangedu.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://ve.hnjuh.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ch.nszjky.cn

[P08] 处理浮点精度问题
来源：http://be.521024.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://gr.hnjuh.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://pa.gzmigu.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://io.asd995.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://bp.shxzskj.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ew.szxytkj.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://zc.muxihuayi.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://rc.shxzukj.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://fg.newstarts.cn

================================================================================
来源：http://wb.lnxyls.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://rl.lnxyls.cn

================================================================================
来源：http://jv.panjiajie.cn

[Q01] 创建表
来源：http://re.521024.cn

CREATE TABLE users (
来源：http://wt.hnjuh.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://vk.newstarts.cn

name VARCHAR(50) NOT NULL,
来源：http://ka.huanxung.cn

email VARCHAR(100) UNIQUE,
来源：http://zw.szsharing.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://eh.jctech888.com.cn

);
来源：http://uu.wgjwhj.cn

[Q02] 创建带外键的表
来源：http://cl.9csxet.cn

CREATE TABLE orders (
来源：http://ew.shxzskj.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ra.shxzukj.cn

user_id INT NOT NULL,
来源：http://pq.jctech888.com.cn

amount DECIMAL(10, 2),
来源：http://yy.hnjuh.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ax.huixiangedu.cn

);
来源：http://rr.9csxet.cn

[Q03] 增加列
来源：http://ve.haigaiapp.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://in.yuexingan06.cn

[Q04] 修改列类型
来源：http://gn.9csxet.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://aq.yuexingan06.cn

[Q05] 重命名列
来源：http://ge.jianghongdianzi.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wl.9csxet.cn

[Q06] 删除列
来源：http://xs.shxzskj.cn

ALTER TABLE users DROP COLUMN age;
来源：http://nq.szxytkj.cn

[Q07] 删除表
来源：http://ww.jianghongdianzi.cn

DROP TABLE IF EXISTS orders;
来源：http://lb.chemitech.net.cn

[Q08] 创建普通索引
来源：http://xb.bjjhwx.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://wa.yuexingan06.cn

[Q09] 创建唯一索引
来源：http://ds.bjjhwx.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hb.szxytkj.cn

[Q10] 插入单行
来源：http://cp.hahajie.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://je.chemitech.net.cn

[Q11] 一次插入多行
来源：http://ba.gzmigu.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://fx.nicolike.cn

[Q12] 插入后取自增 ID
来源：http://zf.asd995.cn

INSERT INTO users (name) VALUES ('C');
来源：http://uy.yuexingan06.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://fh.chemitech.net.cn

[Q13] 忽略重复插入
来源：http://wh.bookmarksfly.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://dz.szsharing.cn

[Q14] 存在则更新（upsert）
来源：http://og.huixinmuqiang.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://vc.asd995.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ua.newstarts.cn

[Q15] 查询全部
来源：http://tm.haigaiapp.cn

SELECT * FROM users;
来源：http://jd.szsharing.cn

[Q16] 查询指定列
来源：http://ke.shtwfgs.cn

SELECT id, name FROM users;
来源：http://ib.huixiangedu.cn

[Q17] 条件查询
来源：http://xt.shxzskj.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://du.chemitech.net.cn

[Q18] 模糊匹配
来源：http://gd.huanxung.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://pw.huixiangedu.cn

[Q19] 范围查询
来源：http://ui.haigaiapp.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ak.asd995.cn

[Q20] IN 列表
来源：http://nx.asd995.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://nr.huixiangedu.cn

[Q21] 空值判断
来源：http://mj.szsharing.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://nx.szsharing.cn

[Q22] 排序
来源：http://on.shtwfgs.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://eu.jctech888.com.cn

[Q23] 分页
来源：http://il.nszjky.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ik.9csxet.cn

[Q24] 去重
来源：http://mj.newstarts.cn

SELECT DISTINCT city FROM users;
来源：http://qa.szxytkj.cn

[Q25] 只取前 N 条
来源：http://je.yuntaijiaju.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://bv.shxzskj.cn

[Q26] 计数
来源：http://ks.colortex.cn

SELECT COUNT(*) FROM users;
来源：http://yu.huanxung.cn

[Q27] 条件计数
来源：http://bs.yuexingan06.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://oz.huixiangedu.cn

[Q28] 求和与平均
来源：http://rq.huixinmuqiang.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://pj.asd995.cn

[Q29] 最大最小值
来源：http://sp.panjiajie.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://me.jianghongdianzi.cn

[Q30] 分组统计
来源：http://mh.shxzskj.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://me.wgjwhj.cn

[Q31] 分组后过滤
来源：http://gp.muxihuayi.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://sn.huanxung.cn

[Q32] 分组拼接字符串
来源：http://gx.newstarts.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://cp.bjjhwx.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://oy.nszjky.cn

[Q33] 多列分组
来源：http://so.muxihuayi.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://dt.huixinmuqiang.cn

[Q34] 每组取第一条
来源：http://pl.lnxyls.cn

SELECT * FROM (
来源：http://ee.shtwfgs.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://kx.huixinmuqiang.cn

) t WHERE rn = 1;
来源：http://xg.yuntaijiaju.cn

[Q35] 内连接
来源：http://px.chemitech.net.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ox.szxytkj.cn

[Q36] 左连接
来源：http://rq.521024.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://kr.szxytkj.cn

[Q37] 右连接
来源：http://qx.bjjhwx.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://aw.9csxet.cn


<!-- 参考信息 -->