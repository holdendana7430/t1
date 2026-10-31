代发 wailian999

[N05] 最大公约数
来源：http://ae.lnxyls.cn

Py:   math.gcd(a, b)
来源：http://cn.shxzskj.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://kl.szsharing.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://lu.521024.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://dj.colortex.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://pz.huanxung.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://eh.hahajie.cn

Ruby: a.gcd(b)
来源：http://dg.shtwfgs.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ph.jianghongdianzi.cn

[N06] 判断回文字符串
来源：http://ov.shtwfgs.cn

Py:   s == s[::-1]
来源：http://ok.nicolike.cn

PHP:  $s === strrev($s);
来源：http://ni.hnjuh.cn

JS:   s === [...s].reverse().join("")
来源：http://zi.panjiajie.cn

TS:   s === [...s].reverse().join("")
来源：http://fi.wgjwhj.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://yx.panjiajie.cn

Go:   // 双指针从两端比较
来源：http://br.521024.cn

Ruby: s == s.reverse
来源：http://nx.nszjky.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://lw.yuexingan06.cn

[N07] 两数之和（返回下标）
来源：http://ti.bookmarksfly.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ev.nicolike.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://pb.haigaiapp.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://qz.yuexingan06.cn

TS:   // 手写 Map<string, number>
来源：http://gp.huixinmuqiang.cn

Java: // 手写 HashMap
来源：http://ot.colortex.cn

Go:   // 手写 map[int]int
来源：http://wv.asd995.cn

Ruby: // 手写 Hash
来源：http://rl.panjiajie.cn

C#:   // 手写 Dictionary<int, int>
来源：http://fd.shxzskj.cn

[N08] 生成全排列
来源：http://jh.bookmarksfly.cn

Py:   itertools.permutations(arr)
来源：http://si.wgjwhj.cn

PHP:  // 手写递归交换
来源：http://mm.gzmigu.cn

JS:   // 手写回溯递归
来源：http://bh.gzmigu.cn

TS:   // 手写回溯递归
来源：http://oy.huanxung.cn

Java: // 手写回溯递归
来源：http://zd.muxihuayi.cn

Go:   // 手写回溯递归
来源：http://fn.jctech888.com.cn

Ruby: arr.permutation.to_a
来源：http://pp.shxzukj.cn

C#:   // 手写回溯递归
来源：http://ca.hahajie.cn

[N09] 栈与队列
来源：http://ge.521024.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://kn.lnxyls.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ua.gzmigu.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://bf.chemitech.net.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://dx.huixinmuqiang.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://vs.haigaiapp.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wk.9csxet.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://qw.gzmigu.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ig.haigaiapp.cn

[N10] 链表节点定义
来源：http://em.asd995.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://zc.shxzskj.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://ai.gzmigu.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://qs.szxytkj.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://sz.newstarts.cn

Java: class Node { int v; Node next; }
来源：http://ra.newstarts.cn

Go:   type Node struct { V int; Next *Node }
来源：http://oe.shxzukj.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://ku.colortex.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://sy.lnxyls.cn

[N11] 二叉树中序遍历
来源：http://ad.muxihuayi.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://oj.asd995.cn

PHP:  // 手写递归函数
来源：http://if.wgjwhj.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hf.yuexingan06.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://da.nicolike.cn

Java: // 手写递归
来源：http://uc.asd995.cn

Go:   // 手写递归
来源：http://en.lnxyls.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://qw.newstarts.cn

C#:   // 手写递归
来源：http://bv.huixinmuqiang.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://cb.nicolike.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://fp.521024.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wd.newstarts.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://vq.nicolike.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://fp.shxzukj.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://gp.muxihuayi.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://op.9csxet.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ae.lnxyls.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://la.szsharing.cn

================================================================================
来源：http://is.wgjwhj.cn

O. 并发与异步
来源：http://og.jianghongdianzi.cn

================================================================================
来源：http://eg.huixiangedu.cn

[O01] 启动一个线程
来源：http://tc.bookmarksfly.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://fa.szxytkj.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mn.yuexingan06.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://xi.huanxung.cn

TS:   // 同 JS
来源：http://cg.chemitech.net.cn

Java: new Thread(() -> f()).start()
来源：http://ca.nszjky.cn

Go:   go f()
来源：http://du.muxihuayi.cn

Ruby: Thread.new { f }
来源：http://ko.hnjuh.cn

C#:   Task.Run(() => F());
来源：http://wb.huixinmuqiang.cn

[O02] 使用线程池
来源：http://sk.gzmigu.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://uq.newstarts.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://sa.muxihuayi.cn

JS:   // worker_threads 线程池
来源：http://ax.lnxyls.cn

TS:   // worker_threads 线程池
来源：http://ac.nicolike.cn

Java: Executors.newFixedThreadPool(4)
来源：http://bm.shxzskj.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://zd.lnxyls.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wu.muxihuayi.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://qd.bjjhwx.cn

[O03] 加锁保护共享数据
来源：http://ap.chemitech.net.cn

Py:   with lock: shared += 1
来源：http://pm.hnjuh.cn

PHP:  // 用 flock() 做文件锁
来源：http://cj.hnjuh.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://iz.huixinmuqiang.cn

TS:   // 同 JS
来源：http://so.yuexingan06.cn

Java: synchronized (this) { shared++; }
来源：http://mr.chemitech.net.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://fj.nicolike.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://hr.nszjky.cn

C#:   lock (gate) { shared++; }
来源：http://mq.nicolike.cn

[O04] 定义异步函数并等待
来源：http://aa.nicolike.cn

Py:   async def f():⏎    await g()
来源：http://pk.asd995.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://rl.jianghongdianzi.cn

JS:   async function f() { await g(); }
来源：http://pt.shxzskj.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://ko.jianghongdianzi.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ao.huixiangedu.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://tr.newstarts.cn

Ruby: # 用 Fiber 或 async gem
来源：http://sh.521024.cn

C#:   async Task F() { await G(); }
来源：http://wv.521024.cn

[O05] 并发执行并等待全部完成
来源：http://kg.colortex.cn

Py:   asyncio.gather(*tasks)
来源：http://ub.hnjuh.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://qx.chemitech.net.cn

JS:   await Promise.all(tasks)
来源：http://ps.muxihuayi.cn

TS:   await Promise.all(tasks)
来源：http://qg.huixiangedu.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://gq.szsharing.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://cj.lnxyls.cn

Ruby: threads.map(&:join)
来源：http://ba.chemitech.net.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://yu.lnxyls.cn

[O06] 使用进程池
来源：http://do.bjjhwx.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://si.newstarts.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://qy.521024.cn

JS:   // child_process / cluster 模块
来源：http://sr.521024.cn

TS:   // child_process / cluster 模块
来源：http://wj.nicolike.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://is.yuexingan06.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://nh.muxihuayi.cn

Ruby: // fork 块
来源：http://sv.asd995.cn

C#:   Parallel.For
来源：http://hr.gzmigu.cn

================================================================================
来源：http://nj.huanxung.cn

P. 常用工具函数
来源：http://py.asd995.cn

================================================================================
来源：http://oy.huixinmuqiang.cn

[P01] 生成 UUID
来源：http://ky.lnxyls.cn

Py:   str(uuid.uuid4())
来源：http://ul.jctech888.com.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ba.yuexingan06.cn

JS:   crypto.randomUUID()
来源：http://ct.newstarts.cn

TS:   crypto.randomUUID()
来源：http://kn.huixiangedu.cn

Java: UUID.randomUUID().toString()
来源：http://au.hahajie.cn

Go:   // 用 github.com/google/uuid
来源：http://hw.shtwfgs.cn

Ruby: SecureRandom.uuid
来源：http://wc.hahajie.cn

C#:   Guid.NewGuid().ToString()
来源：http://pz.gzmigu.cn

[P02] MD5 / SHA256 摘要
来源：http://nx.asd995.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://fl.hahajie.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://xk.yuntaijiaju.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://qw.newstarts.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://du.haigaiapp.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://lt.szsharing.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ms.hahajie.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://vl.nszjky.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://yf.szxytkj.cn

[P03] 生成短随机字符串
来源：http://tn.jctech888.com.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://np.huixiangedu.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://je.colortex.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://px.nicolike.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://kp.jctech888.com.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://nd.huanxung.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hv.hnjuh.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://mu.haigaiapp.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://pa.jctech888.com.cn

[P04] 求长度
来源：http://nm.panjiajie.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://st.newstarts.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://qf.muxihuayi.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://qf.asd995.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://cb.hnjuh.cn

Java: list.size();  map.size();  s.length()
来源：http://jf.wgjwhj.cn

Go:   len(arr);  len(m)
来源：http://ya.yuexingan06.cn

Ruby: x.length;  x.size
来源：http://eh.muxihuayi.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://zh.colortex.cn

[P05] 判断两个对象内容是否相等
来源：http://em.szxytkj.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://qa.newstarts.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://gx.huixinmuqiang.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://np.newstarts.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hv.chemitech.net.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mt.lnxyls.cn

Go:   reflect.DeepEqual(a, b)
来源：http://hw.bookmarksfly.cn

Ruby: a == b
来源：http://ds.nicolike.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mk.shtwfgs.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://sc.hnjuh.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://xb.huanxung.cn

PHP:  if (empty($x)) {}
来源：http://zs.jianghongdianzi.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://qz.jctech888.com.cn

TS:   if (x == null) {}
来源：http://nr.lnxyls.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://wt.yuexingan06.cn

Go:   if x == nil {}
来源：http://pf.bookmarksfly.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://rx.asd995.cn

C#:   if (x is null) {}
来源：http://xr.bjjhwx.cn

[P07] 防抖与节流
来源：http://mt.szxytkj.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://gw.nszjky.cn

PHP:  // 手写时间戳比较
来源：http://ah.szxytkj.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ao.yuntaijiaju.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://lo.nicolike.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://in.nszjky.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://iq.bookmarksfly.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://pm.asd995.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ij.nicolike.cn

[P08] 处理浮点精度问题
来源：http://lv.muxihuayi.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://as.shxzukj.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://nn.lnxyls.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://pf.gzmigu.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://pn.wgjwhj.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://iz.haigaiapp.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ki.9csxet.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://fk.szxytkj.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hg.nicolike.cn

================================================================================
来源：http://zs.huanxung.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ox.muxihuayi.cn

================================================================================
来源：http://rg.jianghongdianzi.cn

[Q01] 创建表
来源：http://jm.huixinmuqiang.cn

CREATE TABLE users (
来源：http://gx.9csxet.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ev.yuexingan06.cn

name VARCHAR(50) NOT NULL,
来源：http://vd.colortex.cn

email VARCHAR(100) UNIQUE,
来源：http://rs.nszjky.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://uh.szxytkj.cn

);
来源：http://xk.yuntaijiaju.cn

[Q02] 创建带外键的表
来源：http://xp.szsharing.cn

CREATE TABLE orders (
来源：http://om.hnjuh.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ql.huixiangedu.cn

user_id INT NOT NULL,
来源：http://dn.bjjhwx.cn

amount DECIMAL(10, 2),
来源：http://mh.nszjky.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://po.shxzskj.cn

);
来源：http://hs.nszjky.cn

[Q03] 增加列
来源：http://kx.521024.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ic.bjjhwx.cn

[Q04] 修改列类型
来源：http://ct.yuntaijiaju.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wk.panjiajie.cn

[Q05] 重命名列
来源：http://pq.lnxyls.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://jp.asd995.cn

[Q06] 删除列
来源：http://cf.huixiangedu.cn

ALTER TABLE users DROP COLUMN age;
来源：http://ud.gzmigu.cn

[Q07] 删除表
来源：http://de.haigaiapp.cn

DROP TABLE IF EXISTS orders;
来源：http://bg.gzmigu.cn

[Q08] 创建普通索引
来源：http://ew.szxytkj.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://pa.yuntaijiaju.cn

[Q09] 创建唯一索引
来源：http://jj.jianghongdianzi.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://iu.hnjuh.cn

[Q10] 插入单行
来源：http://ah.wgjwhj.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://qv.jctech888.com.cn

[Q11] 一次插入多行
来源：http://uy.colortex.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wq.huixiangedu.cn

[Q12] 插入后取自增 ID
来源：http://og.jctech888.com.cn

INSERT INTO users (name) VALUES ('C');
来源：http://pi.9csxet.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ug.9csxet.cn

[Q13] 忽略重复插入
来源：http://ll.yuntaijiaju.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://pt.bookmarksfly.cn

[Q14] 存在则更新（upsert）
来源：http://za.colortex.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ie.panjiajie.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://xv.asd995.cn

[Q15] 查询全部
来源：http://wh.nszjky.cn

SELECT * FROM users;
来源：http://xi.hnjuh.cn

[Q16] 查询指定列
来源：http://nd.szxytkj.cn

SELECT id, name FROM users;
来源：http://hg.hnjuh.cn

[Q17] 条件查询
来源：http://ja.bjjhwx.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ae.shxzskj.cn

[Q18] 模糊匹配
来源：http://if.nicolike.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ro.colortex.cn

[Q19] 范围查询
来源：http://dv.newstarts.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://dc.shtwfgs.cn

[Q20] IN 列表
来源：http://jz.szxytkj.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://om.jianghongdianzi.cn

[Q21] 空值判断
来源：http://pu.hahajie.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://lo.shtwfgs.cn

[Q22] 排序
来源：http://yd.jctech888.com.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ao.521024.cn

[Q23] 分页
来源：http://df.asd995.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://gb.521024.cn

[Q24] 去重
来源：http://gf.szsharing.cn

SELECT DISTINCT city FROM users;
来源：http://is.chemitech.net.cn

[Q25] 只取前 N 条
来源：http://jy.shxzskj.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ss.haigaiapp.cn

[Q26] 计数
来源：http://ry.jianghongdianzi.cn

SELECT COUNT(*) FROM users;
来源：http://gm.jianghongdianzi.cn

[Q27] 条件计数
来源：http://eg.huanxung.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://gk.gzmigu.cn

[Q28] 求和与平均
来源：http://fz.colortex.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wh.hnjuh.cn

[Q29] 最大最小值
来源：http://om.hahajie.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://to.yuntaijiaju.cn

[Q30] 分组统计
来源：http://gv.panjiajie.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://lr.haigaiapp.cn

[Q31] 分组后过滤
来源：http://vj.gzmigu.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://nv.asd995.cn

[Q32] 分组拼接字符串
来源：http://mu.muxihuayi.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ew.nszjky.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://cb.lnxyls.cn

[Q33] 多列分组
来源：http://ys.asd995.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://fz.szsharing.cn

[Q34] 每组取第一条
来源：http://zk.colortex.cn

SELECT * FROM (
来源：http://fg.9csxet.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://sf.chemitech.net.cn

) t WHERE rn = 1;
来源：http://pf.szxytkj.cn

[Q35] 内连接
来源：http://mq.panjiajie.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ie.hahajie.cn

[Q36] 左连接
来源：http://xx.gzmigu.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://om.panjiajie.cn

[Q37] 右连接
来源：http://dc.szsharing.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://dm.521024.cn

[Q38] 全外连接（PostgreSQL）
来源：http://dq.shtwfgs.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://or.yuexingan06.cn

[Q39] 自连接（查上下级）
来源：http://mz.jctech888.com.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://on.muxihuayi.cn


<!-- 参考信息 -->