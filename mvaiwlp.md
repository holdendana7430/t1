代发 wailian999

[N05] 最大公约数
来源：http://fb.panjiajie.cn

Py:   math.gcd(a, b)
来源：http://gm.asd995.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://bw.shxzskj.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mq.jianghongdianzi.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://fp.jctech888.com.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mw.9csxet.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://lv.lnxyls.cn

Ruby: a.gcd(b)
来源：http://hh.9csxet.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://zv.haigaiapp.cn

[N06] 判断回文字符串
来源：http://hr.haigaiapp.cn

Py:   s == s[::-1]
来源：http://jv.haigaiapp.cn

PHP:  $s === strrev($s);
来源：http://yt.hahajie.cn

JS:   s === [...s].reverse().join("")
来源：http://fv.newstarts.cn

TS:   s === [...s].reverse().join("")
来源：http://ew.szsharing.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://uz.chemitech.net.cn

Go:   // 双指针从两端比较
来源：http://tm.nicolike.cn

Ruby: s == s.reverse
来源：http://aw.nszjky.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://gd.jctech888.com.cn

[N07] 两数之和（返回下标）
来源：http://iz.szxytkj.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ho.yuexingan06.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://yk.huanxung.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://dk.9csxet.cn

TS:   // 手写 Map<string, number>
来源：http://vn.huixiangedu.cn

Java: // 手写 HashMap
来源：http://ub.huixinmuqiang.cn

Go:   // 手写 map[int]int
来源：http://dp.huixinmuqiang.cn

Ruby: // 手写 Hash
来源：http://gz.newstarts.cn

C#:   // 手写 Dictionary<int, int>
来源：http://wx.colortex.cn

[N08] 生成全排列
来源：http://hb.hahajie.cn

Py:   itertools.permutations(arr)
来源：http://dn.yuexingan06.cn

PHP:  // 手写递归交换
来源：http://be.gzmigu.cn

JS:   // 手写回溯递归
来源：http://kn.lnxyls.cn

TS:   // 手写回溯递归
来源：http://vj.asd995.cn

Java: // 手写回溯递归
来源：http://ov.hnjuh.cn

Go:   // 手写回溯递归
来源：http://sr.newstarts.cn

Ruby: arr.permutation.to_a
来源：http://fj.jianghongdianzi.cn

C#:   // 手写回溯递归
来源：http://lh.bookmarksfly.cn

[N09] 栈与队列
来源：http://jt.hnjuh.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://fb.gzmigu.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://di.gzmigu.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mg.gzmigu.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://bm.lnxyls.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://kt.newstarts.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://xq.szsharing.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://qo.haigaiapp.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://nu.shxzskj.cn

[N10] 链表节点定义
来源：http://rs.lnxyls.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://oi.jianghongdianzi.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://xl.huanxung.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://je.panjiajie.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://eh.bookmarksfly.cn

Java: class Node { int v; Node next; }
来源：http://ru.colortex.cn

Go:   type Node struct { V int; Next *Node }
来源：http://yb.nszjky.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://el.bjjhwx.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://rp.9csxet.cn

[N11] 二叉树中序遍历
来源：http://zo.huixiangedu.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ks.huixiangedu.cn

PHP:  // 手写递归函数
来源：http://qh.bjjhwx.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://nv.huixinmuqiang.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://eh.huanxung.cn

Java: // 手写递归
来源：http://ox.shxzskj.cn

Go:   // 手写递归
来源：http://xf.colortex.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://sk.huixinmuqiang.cn

C#:   // 手写递归
来源：http://ua.lnxyls.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://pq.nicolike.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ox.asd995.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://kd.shxzskj.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://kz.lnxyls.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://jw.muxihuayi.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://xt.yuntaijiaju.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ke.newstarts.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://qe.shtwfgs.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://qc.gzmigu.cn

================================================================================
来源：http://re.huixinmuqiang.cn

O. 并发与异步
来源：http://xg.haigaiapp.cn

================================================================================
来源：http://yj.shxzskj.cn

[O01] 启动一个线程
来源：http://by.muxihuayi.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://sg.shtwfgs.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mb.lnxyls.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://lk.shtwfgs.cn

TS:   // 同 JS
来源：http://wj.panjiajie.cn

Java: new Thread(() -> f()).start()
来源：http://vg.shxzukj.cn

Go:   go f()
来源：http://ht.lnxyls.cn

Ruby: Thread.new { f }
来源：http://jm.bookmarksfly.cn

C#:   Task.Run(() => F());
来源：http://nk.szsharing.cn

[O02] 使用线程池
来源：http://qx.huanxung.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://az.shxzukj.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://zj.yuexingan06.cn

JS:   // worker_threads 线程池
来源：http://dt.szxytkj.cn

TS:   // worker_threads 线程池
来源：http://wc.nicolike.cn

Java: Executors.newFixedThreadPool(4)
来源：http://vt.nicolike.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://cj.huanxung.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://lb.asd995.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://aq.nicolike.cn

[O03] 加锁保护共享数据
来源：http://xv.lnxyls.cn

Py:   with lock: shared += 1
来源：http://qc.nszjky.cn

PHP:  // 用 flock() 做文件锁
来源：http://hr.asd995.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://kt.huixinmuqiang.cn

TS:   // 同 JS
来源：http://cv.shxzskj.cn

Java: synchronized (this) { shared++; }
来源：http://mh.shtwfgs.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://pt.shxzukj.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://pl.szxytkj.cn

C#:   lock (gate) { shared++; }
来源：http://nu.haigaiapp.cn

[O04] 定义异步函数并等待
来源：http://gx.hnjuh.cn

Py:   async def f():⏎    await g()
来源：http://lh.shtwfgs.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ng.asd995.cn

JS:   async function f() { await g(); }
来源：http://ih.hnjuh.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://dw.nicolike.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://vr.newstarts.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://jv.nicolike.cn

Ruby: # 用 Fiber 或 async gem
来源：http://rr.hahajie.cn

C#:   async Task F() { await G(); }
来源：http://gs.szsharing.cn

[O05] 并发执行并等待全部完成
来源：http://yd.gzmigu.cn

Py:   asyncio.gather(*tasks)
来源：http://jl.yuntaijiaju.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mv.jctech888.com.cn

JS:   await Promise.all(tasks)
来源：http://vj.jctech888.com.cn

TS:   await Promise.all(tasks)
来源：http://cw.9csxet.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://gl.shtwfgs.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://xx.chemitech.net.cn

Ruby: threads.map(&:join)
来源：http://mb.asd995.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://lp.521024.cn

[O06] 使用进程池
来源：http://nu.huixiangedu.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://fx.jctech888.com.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://gq.521024.cn

JS:   // child_process / cluster 模块
来源：http://fs.hahajie.cn

TS:   // child_process / cluster 模块
来源：http://pe.shtwfgs.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://gy.huixinmuqiang.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wv.bookmarksfly.cn

Ruby: // fork 块
来源：http://xw.lnxyls.cn

C#:   Parallel.For
来源：http://bw.newstarts.cn

================================================================================
来源：http://tf.nszjky.cn

P. 常用工具函数
来源：http://pn.newstarts.cn

================================================================================
来源：http://jo.newstarts.cn

[P01] 生成 UUID
来源：http://mf.newstarts.cn

Py:   str(uuid.uuid4())
来源：http://xi.yuntaijiaju.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://nm.szsharing.cn

JS:   crypto.randomUUID()
来源：http://zw.lnxyls.cn

TS:   crypto.randomUUID()
来源：http://ev.521024.cn

Java: UUID.randomUUID().toString()
来源：http://pr.hahajie.cn

Go:   // 用 github.com/google/uuid
来源：http://fc.9csxet.cn

Ruby: SecureRandom.uuid
来源：http://fj.521024.cn

C#:   Guid.NewGuid().ToString()
来源：http://oz.panjiajie.cn

[P02] MD5 / SHA256 摘要
来源：http://uy.chemitech.net.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://qs.wgjwhj.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://lp.szsharing.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://jt.shtwfgs.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://kz.chemitech.net.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://qe.bookmarksfly.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://im.jianghongdianzi.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://er.newstarts.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://bm.gzmigu.cn

[P03] 生成短随机字符串
来源：http://nx.shxzskj.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://od.chemitech.net.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://sh.nicolike.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://lx.szxytkj.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://rk.yuexingan06.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://rj.newstarts.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://pp.shxzskj.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://ry.gzmigu.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ja.huixinmuqiang.cn

[P04] 求长度
来源：http://pg.huixinmuqiang.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://bz.chemitech.net.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://qt.shtwfgs.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://im.szsharing.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ue.jianghongdianzi.cn

Java: list.size();  map.size();  s.length()
来源：http://pe.521024.cn

Go:   len(arr);  len(m)
来源：http://st.hnjuh.cn

Ruby: x.length;  x.size
来源：http://cl.nicolike.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://yd.yuexingan06.cn

[P05] 判断两个对象内容是否相等
来源：http://xq.bookmarksfly.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://ob.9csxet.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://sr.bookmarksfly.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://tc.jctech888.com.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://kg.hahajie.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://as.haigaiapp.cn

Go:   reflect.DeepEqual(a, b)
来源：http://yv.hahajie.cn

Ruby: a == b
来源：http://lj.bjjhwx.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://nf.asd995.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://xt.haigaiapp.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://le.jctech888.com.cn

PHP:  if (empty($x)) {}
来源：http://tk.jianghongdianzi.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://es.lnxyls.cn

TS:   if (x == null) {}
来源：http://gj.shxzukj.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://to.huixiangedu.cn

Go:   if x == nil {}
来源：http://ab.lnxyls.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hd.szxytkj.cn

C#:   if (x is null) {}
来源：http://rx.hnjuh.cn

[P07] 防抖与节流
来源：http://pw.szxytkj.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://xv.newstarts.cn

PHP:  // 手写时间戳比较
来源：http://mg.szsharing.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xc.huixiangedu.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://uc.hnjuh.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ua.jianghongdianzi.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ki.yuntaijiaju.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://on.jianghongdianzi.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://qv.521024.cn

[P08] 处理浮点精度问题
来源：http://ig.yuntaijiaju.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mi.newstarts.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ea.chemitech.net.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://fx.nicolike.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ou.asd995.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://pj.nicolike.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://df.jianghongdianzi.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://vj.9csxet.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://kp.huanxung.cn

================================================================================
来源：http://wb.shxzukj.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://uz.yuntaijiaju.cn

================================================================================
来源：http://tm.haigaiapp.cn

[Q01] 创建表
来源：http://wv.nszjky.cn

CREATE TABLE users (
来源：http://bv.szxytkj.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://jc.bjjhwx.cn

name VARCHAR(50) NOT NULL,
来源：http://rz.wgjwhj.cn

email VARCHAR(100) UNIQUE,
来源：http://nn.muxihuayi.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://te.yuexingan06.cn

);
来源：http://hv.newstarts.cn

[Q02] 创建带外键的表
来源：http://mx.hnjuh.cn

CREATE TABLE orders (
来源：http://uy.huixinmuqiang.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://vi.shxzukj.cn

user_id INT NOT NULL,
来源：http://zb.haigaiapp.cn

amount DECIMAL(10, 2),
来源：http://om.lnxyls.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wr.huanxung.cn

);
来源：http://lc.haigaiapp.cn

[Q03] 增加列
来源：http://hf.newstarts.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://on.huanxung.cn

[Q04] 修改列类型
来源：http://ai.szsharing.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://cm.9csxet.cn

[Q05] 重命名列
来源：http://vt.9csxet.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://zg.bookmarksfly.cn

[Q06] 删除列
来源：http://fl.huixiangedu.cn

ALTER TABLE users DROP COLUMN age;
来源：http://yt.newstarts.cn

[Q07] 删除表
来源：http://uj.chemitech.net.cn

DROP TABLE IF EXISTS orders;
来源：http://gg.huixinmuqiang.cn

[Q08] 创建普通索引
来源：http://we.hahajie.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://pc.yuexingan06.cn

[Q09] 创建唯一索引
来源：http://qn.bookmarksfly.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://re.muxihuayi.cn

[Q10] 插入单行
来源：http://ii.bookmarksfly.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://di.shxzskj.cn

[Q11] 一次插入多行
来源：http://qb.yuexingan06.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://dm.muxihuayi.cn

[Q12] 插入后取自增 ID
来源：http://ow.hahajie.cn

INSERT INTO users (name) VALUES ('C');
来源：http://ci.hnjuh.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://eb.szxytkj.cn

[Q13] 忽略重复插入
来源：http://dp.9csxet.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://gs.shxzskj.cn

[Q14] 存在则更新（upsert）
来源：http://si.szxytkj.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://pj.jianghongdianzi.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://nj.9csxet.cn

[Q15] 查询全部
来源：http://vh.hahajie.cn

SELECT * FROM users;
来源：http://fj.521024.cn

[Q16] 查询指定列
来源：http://ww.haigaiapp.cn

SELECT id, name FROM users;
来源：http://hq.panjiajie.cn

[Q17] 条件查询
来源：http://qa.shxzukj.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://nw.newstarts.cn

[Q18] 模糊匹配
来源：http://ff.nszjky.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://re.haigaiapp.cn

[Q19] 范围查询
来源：http://dx.panjiajie.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://kn.jctech888.com.cn

[Q20] IN 列表
来源：http://xi.shxzskj.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hb.gzmigu.cn

[Q21] 空值判断
来源：http://ub.huixiangedu.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://ta.huanxung.cn

[Q22] 排序
来源：http://lw.huixiangedu.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://km.asd995.cn

[Q23] 分页
来源：http://sf.chemitech.net.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://po.chemitech.net.cn

[Q24] 去重
来源：http://gn.wgjwhj.cn

SELECT DISTINCT city FROM users;
来源：http://oj.jianghongdianzi.cn

[Q25] 只取前 N 条
来源：http://do.asd995.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://at.newstarts.cn

[Q26] 计数
来源：http://lv.szxytkj.cn

SELECT COUNT(*) FROM users;
来源：http://do.bookmarksfly.cn

[Q27] 条件计数
来源：http://th.bookmarksfly.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://yc.hahajie.cn

[Q28] 求和与平均
来源：http://mo.jianghongdianzi.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://vw.newstarts.cn

[Q29] 最大最小值
来源：http://en.nszjky.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.huixinmuqiang.cn

[Q30] 分组统计
来源：http://kf.shxzukj.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ms.asd995.cn

[Q31] 分组后过滤
来源：http://hi.hahajie.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://cy.muxihuayi.cn

[Q32] 分组拼接字符串
来源：http://dv.nicolike.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://qh.panjiajie.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://fc.colortex.cn

[Q33] 多列分组
来源：http://ry.gzmigu.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://rt.huixiangedu.cn

[Q34] 每组取第一条
来源：http://xr.nszjky.cn

SELECT * FROM (
来源：http://gj.yuntaijiaju.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://iz.hahajie.cn

) t WHERE rn = 1;
来源：http://vk.gzmigu.cn

[Q35] 内连接
来源：http://wv.shxzskj.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://vm.bookmarksfly.cn

[Q36] 左连接
来源：http://ph.bjjhwx.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://bn.yuntaijiaju.cn

[Q37] 右连接
来源：http://qa.nicolike.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://jq.hahajie.cn

[Q38] 全外连接（PostgreSQL）
来源：http://df.asd995.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://bm.chemitech.net.cn

[Q39] 自连接（查上下级）
来源：http://zy.hnjuh.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://kt.hahajie.cn


<!-- 参考信息 -->