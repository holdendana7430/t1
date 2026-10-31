代发 wailian999

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://kw.shtwfgs.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wj.shxzukj.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://xe.shtwfgs.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://py.szsharing.cn

[N05] 最大公约数
来源：http://dr.gzmigu.cn

Py:   math.gcd(a, b)
来源：http://wd.newstarts.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://km.chemitech.net.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://bp.shtwfgs.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://aq.jianghongdianzi.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://uz.huixinmuqiang.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://zi.shxzskj.cn

Ruby: a.gcd(b)
来源：http://ik.gzmigu.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://fh.asd995.cn

[N06] 判断回文字符串
来源：http://pp.nszjky.cn

Py:   s == s[::-1]
来源：http://yy.muxihuayi.cn

PHP:  $s === strrev($s);
来源：http://dc.asd995.cn

JS:   s === [...s].reverse().join("")
来源：http://ax.haigaiapp.cn

TS:   s === [...s].reverse().join("")
来源：http://ez.muxihuayi.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://fi.bookmarksfly.cn

Go:   // 双指针从两端比较
来源：http://gr.9csxet.cn

Ruby: s == s.reverse
来源：http://wh.szxytkj.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://bc.huixiangedu.cn

[N07] 两数之和（返回下标）
来源：http://lz.bjjhwx.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://rj.jctech888.com.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://kt.yuexingan06.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://bp.gzmigu.cn

TS:   // 手写 Map<string, number>
来源：http://wt.nicolike.cn

Java: // 手写 HashMap
来源：http://vi.wgjwhj.cn

Go:   // 手写 map[int]int
来源：http://lg.jctech888.com.cn

Ruby: // 手写 Hash
来源：http://fl.nszjky.cn

C#:   // 手写 Dictionary<int, int>
来源：http://nk.muxihuayi.cn

[N08] 生成全排列
来源：http://uj.gzmigu.cn

Py:   itertools.permutations(arr)
来源：http://ep.jianghongdianzi.cn

PHP:  // 手写递归交换
来源：http://el.chemitech.net.cn

JS:   // 手写回溯递归
来源：http://ql.huixiangedu.cn

TS:   // 手写回溯递归
来源：http://qt.shtwfgs.cn

Java: // 手写回溯递归
来源：http://lf.gzmigu.cn

Go:   // 手写回溯递归
来源：http://zd.bjjhwx.cn

Ruby: arr.permutation.to_a
来源：http://ph.colortex.cn

C#:   // 手写回溯递归
来源：http://tv.haigaiapp.cn

[N09] 栈与队列
来源：http://bn.jctech888.com.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ni.lnxyls.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ox.bookmarksfly.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://fw.jctech888.com.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mq.yuntaijiaju.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://kc.newstarts.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://to.hahajie.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hn.newstarts.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://oq.shtwfgs.cn

[N10] 链表节点定义
来源：http://yl.newstarts.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://bm.wgjwhj.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://wc.521024.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://rr.hahajie.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://nq.bookmarksfly.cn

Java: class Node { int v; Node next; }
来源：http://gg.lnxyls.cn

Go:   type Node struct { V int; Next *Node }
来源：http://by.jianghongdianzi.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://ao.szxytkj.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://hb.asd995.cn

[N11] 二叉树中序遍历
来源：http://yh.521024.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://fs.bjjhwx.cn

PHP:  // 手写递归函数
来源：http://go.panjiajie.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ix.bookmarksfly.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ys.szsharing.cn

Java: // 手写递归
来源：http://wf.wgjwhj.cn

Go:   // 手写递归
来源：http://nh.yuexingan06.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ee.nicolike.cn

C#:   // 手写递归
来源：http://qx.yuntaijiaju.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://vz.colortex.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://zh.shtwfgs.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://qq.huixiangedu.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://oi.panjiajie.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://uk.jctech888.com.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://yj.shtwfgs.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ji.szsharing.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://fu.jctech888.com.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://tb.panjiajie.cn

================================================================================
来源：http://ed.nszjky.cn

O. 并发与异步
来源：http://uu.szsharing.cn

================================================================================
来源：http://dy.asd995.cn

[O01] 启动一个线程
来源：http://xg.9csxet.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mj.asd995.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://le.huixinmuqiang.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wz.nicolike.cn

TS:   // 同 JS
来源：http://jd.chemitech.net.cn

Java: new Thread(() -> f()).start()
来源：http://wd.yuexingan06.cn

Go:   go f()
来源：http://kn.shtwfgs.cn

Ruby: Thread.new { f }
来源：http://pu.wgjwhj.cn

C#:   Task.Run(() => F());
来源：http://ty.haigaiapp.cn

[O02] 使用线程池
来源：http://qb.haigaiapp.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wa.szxytkj.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wn.nszjky.cn

JS:   // worker_threads 线程池
来源：http://si.chemitech.net.cn

TS:   // worker_threads 线程池
来源：http://mo.shtwfgs.cn

Java: Executors.newFixedThreadPool(4)
来源：http://hz.lnxyls.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://iq.wgjwhj.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://up.wgjwhj.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wb.hnjuh.cn

[O03] 加锁保护共享数据
来源：http://ji.shxzukj.cn

Py:   with lock: shared += 1
来源：http://ia.jctech888.com.cn

PHP:  // 用 flock() 做文件锁
来源：http://bt.hnjuh.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://fq.asd995.cn

TS:   // 同 JS
来源：http://rb.521024.cn

Java: synchronized (this) { shared++; }
来源：http://of.szxytkj.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://co.lnxyls.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://oz.jianghongdianzi.cn

C#:   lock (gate) { shared++; }
来源：http://tn.asd995.cn

[O04] 定义异步函数并等待
来源：http://ff.chemitech.net.cn

Py:   async def f():⏎    await g()
来源：http://hh.bookmarksfly.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://bu.wgjwhj.cn

JS:   async function f() { await g(); }
来源：http://ly.jctech888.com.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://ca.shxzskj.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://cg.bjjhwx.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://td.hnjuh.cn

Ruby: # 用 Fiber 或 async gem
来源：http://ko.huixinmuqiang.cn

C#:   async Task F() { await G(); }
来源：http://fo.wgjwhj.cn

[O05] 并发执行并等待全部完成
来源：http://kp.shxzskj.cn

Py:   asyncio.gather(*tasks)
来源：http://mk.yuexingan06.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://rf.gzmigu.cn

JS:   await Promise.all(tasks)
来源：http://yi.jctech888.com.cn

TS:   await Promise.all(tasks)
来源：http://rz.huanxung.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://yp.yuntaijiaju.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mm.muxihuayi.cn

Ruby: threads.map(&:join)
来源：http://ac.lnxyls.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://qv.gzmigu.cn

[O06] 使用进程池
来源：http://tw.bjjhwx.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://jx.panjiajie.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://vi.wgjwhj.cn

JS:   // child_process / cluster 模块
来源：http://uu.nicolike.cn

TS:   // child_process / cluster 模块
来源：http://ed.haigaiapp.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://km.521024.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://qy.nicolike.cn

Ruby: // fork 块
来源：http://qf.521024.cn

C#:   Parallel.For
来源：http://vt.panjiajie.cn

================================================================================
来源：http://qp.bjjhwx.cn

P. 常用工具函数
来源：http://vc.huanxung.cn

================================================================================
来源：http://rl.hnjuh.cn

[P01] 生成 UUID
来源：http://st.gzmigu.cn

Py:   str(uuid.uuid4())
来源：http://jc.colortex.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://nr.colortex.cn

JS:   crypto.randomUUID()
来源：http://ua.muxihuayi.cn

TS:   crypto.randomUUID()
来源：http://bw.huixiangedu.cn

Java: UUID.randomUUID().toString()
来源：http://po.gzmigu.cn

Go:   // 用 github.com/google/uuid
来源：http://ha.muxihuayi.cn

Ruby: SecureRandom.uuid
来源：http://ci.colortex.cn

C#:   Guid.NewGuid().ToString()
来源：http://js.muxihuayi.cn

[P02] MD5 / SHA256 摘要
来源：http://bs.lnxyls.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://vz.szsharing.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://dd.szxytkj.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ai.newstarts.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://nk.hnjuh.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://rd.haigaiapp.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://rn.huixinmuqiang.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://cs.muxihuayi.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ox.muxihuayi.cn

[P03] 生成短随机字符串
来源：http://yg.bjjhwx.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://fh.bookmarksfly.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://kj.yuexingan06.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://oi.jctech888.com.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://sy.shxzskj.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://bq.colortex.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://fv.521024.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://xh.bookmarksfly.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://gw.szsharing.cn

[P04] 求长度
来源：http://ma.hnjuh.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wj.hnjuh.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://pl.9csxet.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ng.szsharing.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wz.yuexingan06.cn

Java: list.size();  map.size();  s.length()
来源：http://ah.huixinmuqiang.cn

Go:   len(arr);  len(m)
来源：http://xn.colortex.cn

Ruby: x.length;  x.size
来源：http://sz.bjjhwx.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://ca.hahajie.cn

[P05] 判断两个对象内容是否相等
来源：http://zh.shxzskj.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://tq.yuntaijiaju.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://jt.muxihuayi.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://zr.haigaiapp.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ks.gzmigu.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://kk.shtwfgs.cn

Go:   reflect.DeepEqual(a, b)
来源：http://xw.jctech888.com.cn

Ruby: a == b
来源：http://ks.wgjwhj.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://cn.shtwfgs.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mm.521024.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://tq.szxytkj.cn

PHP:  if (empty($x)) {}
来源：http://xb.bookmarksfly.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ax.shtwfgs.cn

TS:   if (x == null) {}
来源：http://mt.gzmigu.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://ju.lnxyls.cn

Go:   if x == nil {}
来源：http://fr.hahajie.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://rr.521024.cn

C#:   if (x is null) {}
来源：http://em.haigaiapp.cn

[P07] 防抖与节流
来源：http://jr.huanxung.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://sb.yuexingan06.cn

PHP:  // 手写时间戳比较
来源：http://ex.newstarts.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://tc.szxytkj.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://nl.szsharing.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://bi.szxytkj.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://tq.newstarts.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://rl.szxytkj.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ui.jianghongdianzi.cn

[P08] 处理浮点精度问题
来源：http://re.colortex.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://lw.szxytkj.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ed.jianghongdianzi.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://uq.huanxung.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://yk.shxzukj.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://kc.hahajie.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://by.nicolike.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://pm.wgjwhj.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://gv.panjiajie.cn

================================================================================
来源：http://tf.wgjwhj.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://gl.chemitech.net.cn

================================================================================
来源：http://sb.yuexingan06.cn

[Q01] 创建表
来源：http://lg.panjiajie.cn

CREATE TABLE users (
来源：http://jz.521024.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://zj.jianghongdianzi.cn

name VARCHAR(50) NOT NULL,
来源：http://jp.shtwfgs.cn

email VARCHAR(100) UNIQUE,
来源：http://qu.shxzukj.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://dc.panjiajie.cn

);
来源：http://tb.9csxet.cn

[Q02] 创建带外键的表
来源：http://hy.hahajie.cn

CREATE TABLE orders (
来源：http://kp.gzmigu.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ck.chemitech.net.cn

user_id INT NOT NULL,
来源：http://ch.hahajie.cn

amount DECIMAL(10, 2),
来源：http://pf.bookmarksfly.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://as.newstarts.cn

);
来源：http://oz.chemitech.net.cn

[Q03] 增加列
来源：http://fe.szsharing.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ip.hnjuh.cn

[Q04] 修改列类型
来源：http://ea.huixinmuqiang.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://tc.yuntaijiaju.cn

[Q05] 重命名列
来源：http://sp.panjiajie.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://fi.muxihuayi.cn

[Q06] 删除列
来源：http://cf.yuntaijiaju.cn

ALTER TABLE users DROP COLUMN age;
来源：http://fm.shxzskj.cn

[Q07] 删除表
来源：http://qs.nszjky.cn

DROP TABLE IF EXISTS orders;
来源：http://wo.jctech888.com.cn

[Q08] 创建普通索引
来源：http://ra.shxzukj.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://dr.shxzukj.cn

[Q09] 创建唯一索引
来源：http://se.nszjky.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://sc.colortex.cn

[Q10] 插入单行
来源：http://eb.nicolike.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://nt.jianghongdianzi.cn

[Q11] 一次插入多行
来源：http://me.chemitech.net.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://sg.jianghongdianzi.cn

[Q12] 插入后取自增 ID
来源：http://yb.panjiajie.cn

INSERT INTO users (name) VALUES ('C');
来源：http://yr.lnxyls.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://cm.shtwfgs.cn

[Q13] 忽略重复插入
来源：http://fx.huanxung.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ae.hnjuh.cn

[Q14] 存在则更新（upsert）
来源：http://kk.9csxet.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://tn.colortex.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://kt.yuexingan06.cn

[Q15] 查询全部
来源：http://jn.huixinmuqiang.cn

SELECT * FROM users;
来源：http://fc.shxzukj.cn

[Q16] 查询指定列
来源：http://hk.lnxyls.cn

SELECT id, name FROM users;
来源：http://sn.lnxyls.cn

[Q17] 条件查询
来源：http://vy.bjjhwx.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://yu.wgjwhj.cn

[Q18] 模糊匹配
来源：http://dw.bjjhwx.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://se.asd995.cn

[Q19] 范围查询
来源：http://fi.szsharing.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://fu.yuexingan06.cn

[Q20] IN 列表
来源：http://pn.colortex.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://bc.huixiangedu.cn

[Q21] 空值判断
来源：http://zx.colortex.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://mj.jianghongdianzi.cn

[Q22] 排序
来源：http://gf.wgjwhj.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://xz.521024.cn

[Q23] 分页
来源：http://eb.9csxet.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://op.bjjhwx.cn

[Q24] 去重
来源：http://iy.shxzukj.cn

SELECT DISTINCT city FROM users;
来源：http://pv.shxzskj.cn

[Q25] 只取前 N 条
来源：http://ed.szsharing.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://cb.haigaiapp.cn

[Q26] 计数
来源：http://yz.bjjhwx.cn

SELECT COUNT(*) FROM users;
来源：http://yo.panjiajie.cn

[Q27] 条件计数
来源：http://to.hahajie.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://px.haigaiapp.cn

[Q28] 求和与平均
来源：http://vc.panjiajie.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://qx.bookmarksfly.cn

[Q29] 最大最小值
来源：http://xv.szxytkj.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://au.chemitech.net.cn

[Q30] 分组统计
来源：http://dr.haigaiapp.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hg.jctech888.com.cn

[Q31] 分组后过滤
来源：http://mh.haigaiapp.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://iw.gzmigu.cn

[Q32] 分组拼接字符串
来源：http://vg.huixiangedu.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://np.yuntaijiaju.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ur.huixiangedu.cn

[Q33] 多列分组
来源：http://jk.jianghongdianzi.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://qk.yuntaijiaju.cn

[Q34] 每组取第一条
来源：http://eo.huixinmuqiang.cn

SELECT * FROM (
来源：http://kq.lnxyls.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://me.nicolike.cn

) t WHERE rn = 1;
来源：http://ly.wgjwhj.cn

[Q35] 内连接
来源：http://jh.asd995.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://va.gzmigu.cn

[Q36] 左连接
来源：http://bn.shtwfgs.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://uj.shtwfgs.cn

[Q37] 右连接
来源：http://of.huanxung.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://iy.hnjuh.cn


<!-- 参考信息 -->