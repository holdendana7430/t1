代发 wailian999

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://gp.bjjhwx.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://sv.gzmigu.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://rb.huixinmuqiang.cn

Ruby: a.gcd(b)
来源：http://ki.yuexingan06.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://bw.asd995.cn

[N06] 判断回文字符串
来源：http://fd.huixinmuqiang.cn

Py:   s == s[::-1]
来源：http://ui.nszjky.cn

PHP:  $s === strrev($s);
来源：http://nw.yuntaijiaju.cn

JS:   s === [...s].reverse().join("")
来源：http://xd.haigaiapp.cn

TS:   s === [...s].reverse().join("")
来源：http://mx.521024.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://xw.shxzskj.cn

Go:   // 双指针从两端比较
来源：http://fm.huanxung.cn

Ruby: s == s.reverse
来源：http://ez.shtwfgs.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://cm.9csxet.cn

[N07] 两数之和（返回下标）
来源：http://wv.shxzukj.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://xm.colortex.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://uf.jctech888.com.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://fn.shxzskj.cn

TS:   // 手写 Map<string, number>
来源：http://yi.huanxung.cn

Java: // 手写 HashMap
来源：http://qj.yuntaijiaju.cn

Go:   // 手写 map[int]int
来源：http://fe.hnjuh.cn

Ruby: // 手写 Hash
来源：http://vt.521024.cn

C#:   // 手写 Dictionary<int, int>
来源：http://wr.huanxung.cn

[N08] 生成全排列
来源：http://la.nszjky.cn

Py:   itertools.permutations(arr)
来源：http://th.hahajie.cn

PHP:  // 手写递归交换
来源：http://pe.wgjwhj.cn

JS:   // 手写回溯递归
来源：http://ir.yuexingan06.cn

TS:   // 手写回溯递归
来源：http://wq.jianghongdianzi.cn

Java: // 手写回溯递归
来源：http://cc.yuexingan06.cn

Go:   // 手写回溯递归
来源：http://cl.bjjhwx.cn

Ruby: arr.permutation.to_a
来源：http://uk.shxzskj.cn

C#:   // 手写回溯递归
来源：http://de.521024.cn

[N09] 栈与队列
来源：http://zt.hahajie.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://en.huixiangedu.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://na.chemitech.net.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://kv.hahajie.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://cp.yuexingan06.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://gj.bjjhwx.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://no.nszjky.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mm.szsharing.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://le.muxihuayi.cn

[N10] 链表节点定义
来源：http://fs.shtwfgs.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wo.huixinmuqiang.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://rq.shxzskj.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ir.hahajie.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://qw.newstarts.cn

Java: class Node { int v; Node next; }
来源：http://ea.bjjhwx.cn

Go:   type Node struct { V int; Next *Node }
来源：http://nb.chemitech.net.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://lm.lnxyls.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://ug.chemitech.net.cn

[N11] 二叉树中序遍历
来源：http://vf.nszjky.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://kz.newstarts.cn

PHP:  // 手写递归函数
来源：http://xv.gzmigu.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://iz.521024.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://he.huanxung.cn

Java: // 手写递归
来源：http://de.yuntaijiaju.cn

Go:   // 手写递归
来源：http://av.lnxyls.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ve.shxzskj.cn

C#:   // 手写递归
来源：http://ux.wgjwhj.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://md.lnxyls.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://na.huixinmuqiang.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ac.nicolike.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://he.asd995.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://vl.szsharing.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hd.521024.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://cj.nszjky.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://sv.bjjhwx.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://aq.lnxyls.cn

================================================================================
来源：http://qb.nicolike.cn

O. 并发与异步
来源：http://ks.chemitech.net.cn

================================================================================
来源：http://kw.szxytkj.cn

[O01] 启动一个线程
来源：http://pp.yuexingan06.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://fk.shxzskj.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ax.huanxung.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://xv.nicolike.cn

TS:   // 同 JS
来源：http://we.colortex.cn

Java: new Thread(() -> f()).start()
来源：http://kl.hahajie.cn

Go:   go f()
来源：http://yj.nszjky.cn

Ruby: Thread.new { f }
来源：http://mm.nicolike.cn

C#:   Task.Run(() => F());
来源：http://og.gzmigu.cn

[O02] 使用线程池
来源：http://bn.nszjky.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://kp.lnxyls.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://qc.nszjky.cn

JS:   // worker_threads 线程池
来源：http://cy.panjiajie.cn

TS:   // worker_threads 线程池
来源：http://zn.wgjwhj.cn

Java: Executors.newFixedThreadPool(4)
来源：http://uk.chemitech.net.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://eg.shxzskj.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ib.panjiajie.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://oj.szxytkj.cn

[O03] 加锁保护共享数据
来源：http://dg.asd995.cn

Py:   with lock: shared += 1
来源：http://nk.muxihuayi.cn

PHP:  // 用 flock() 做文件锁
来源：http://xn.szsharing.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://yp.asd995.cn

TS:   // 同 JS
来源：http://yv.haigaiapp.cn

Java: synchronized (this) { shared++; }
来源：http://rs.huanxung.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://fq.asd995.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://yz.panjiajie.cn

C#:   lock (gate) { shared++; }
来源：http://pn.shtwfgs.cn

[O04] 定义异步函数并等待
来源：http://vz.lnxyls.cn

Py:   async def f():⏎    await g()
来源：http://ys.huixinmuqiang.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://pz.panjiajie.cn

JS:   async function f() { await g(); }
来源：http://om.hnjuh.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://vl.lnxyls.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ff.jianghongdianzi.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://zn.nszjky.cn

Ruby: # 用 Fiber 或 async gem
来源：http://eq.chemitech.net.cn

C#:   async Task F() { await G(); }
来源：http://fi.jctech888.com.cn

[O05] 并发执行并等待全部完成
来源：http://cf.521024.cn

Py:   asyncio.gather(*tasks)
来源：http://ot.asd995.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://lt.yuntaijiaju.cn

JS:   await Promise.all(tasks)
来源：http://yh.huixiangedu.cn

TS:   await Promise.all(tasks)
来源：http://li.newstarts.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ny.jianghongdianzi.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://rs.521024.cn

Ruby: threads.map(&:join)
来源：http://ta.shxzukj.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://fd.hnjuh.cn

[O06] 使用进程池
来源：http://fk.hnjuh.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://nr.newstarts.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://rr.wgjwhj.cn

JS:   // child_process / cluster 模块
来源：http://ni.bjjhwx.cn

TS:   // child_process / cluster 模块
来源：http://so.gzmigu.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://zp.lnxyls.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://fj.hahajie.cn

Ruby: // fork 块
来源：http://sy.hahajie.cn

C#:   Parallel.For
来源：http://vl.bookmarksfly.cn

================================================================================
来源：http://oj.chemitech.net.cn

P. 常用工具函数
来源：http://mo.nszjky.cn

================================================================================
来源：http://eq.shtwfgs.cn

[P01] 生成 UUID
来源：http://qh.muxihuayi.cn

Py:   str(uuid.uuid4())
来源：http://mw.szxytkj.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://vw.haigaiapp.cn

JS:   crypto.randomUUID()
来源：http://io.bjjhwx.cn

TS:   crypto.randomUUID()
来源：http://rq.chemitech.net.cn

Java: UUID.randomUUID().toString()
来源：http://gf.yuntaijiaju.cn

Go:   // 用 github.com/google/uuid
来源：http://ii.nicolike.cn

Ruby: SecureRandom.uuid
来源：http://jt.hahajie.cn

C#:   Guid.NewGuid().ToString()
来源：http://zw.nicolike.cn

[P02] MD5 / SHA256 摘要
来源：http://pz.shxzskj.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://oc.chemitech.net.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://ti.shxzukj.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://xx.colortex.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://tm.muxihuayi.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://xj.panjiajie.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://pu.asd995.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://nf.newstarts.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://qh.panjiajie.cn

[P03] 生成短随机字符串
来源：http://ja.nszjky.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://fj.shxzskj.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://aw.newstarts.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://cv.9csxet.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://xj.shxzukj.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ki.asd995.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ce.muxihuayi.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://xg.jianghongdianzi.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://nc.yuexingan06.cn

[P04] 求长度
来源：http://kt.shxzskj.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wn.shxzukj.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://rv.szxytkj.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://xc.yuexingan06.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ec.gzmigu.cn

Java: list.size();  map.size();  s.length()
来源：http://ow.szsharing.cn

Go:   len(arr);  len(m)
来源：http://zd.yuntaijiaju.cn

Ruby: x.length;  x.size
来源：http://mb.jctech888.com.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://ad.jctech888.com.cn

[P05] 判断两个对象内容是否相等
来源：http://ty.panjiajie.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://qv.szsharing.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://pe.lnxyls.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://co.gzmigu.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://gr.bookmarksfly.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://tv.521024.cn

Go:   reflect.DeepEqual(a, b)
来源：http://uc.nicolike.cn

Ruby: a == b
来源：http://vt.bookmarksfly.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://lc.yuexingan06.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ay.hahajie.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://qi.muxihuayi.cn

PHP:  if (empty($x)) {}
来源：http://wd.huanxung.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ka.hahajie.cn

TS:   if (x == null) {}
来源：http://tr.yuntaijiaju.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://mh.yuntaijiaju.cn

Go:   if x == nil {}
来源：http://cj.lnxyls.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://nu.9csxet.cn

C#:   if (x is null) {}
来源：http://tv.haigaiapp.cn

[P07] 防抖与节流
来源：http://tf.521024.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://gk.hahajie.cn

PHP:  // 手写时间戳比较
来源：http://oi.wgjwhj.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://sj.bjjhwx.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mh.lnxyls.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ix.yuntaijiaju.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ji.huanxung.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://sa.bookmarksfly.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hf.newstarts.cn

[P08] 处理浮点精度问题
来源：http://iy.szsharing.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://yd.gzmigu.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://po.muxihuayi.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://kt.jctech888.com.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://bc.jctech888.com.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://jk.nszjky.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://if.huixinmuqiang.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ce.chemitech.net.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://tc.shxzukj.cn

================================================================================
来源：http://pj.jctech888.com.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://go.nicolike.cn

================================================================================
来源：http://bo.bjjhwx.cn

[Q01] 创建表
来源：http://ng.nicolike.cn

CREATE TABLE users (
来源：http://ot.szsharing.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://sv.huanxung.cn

name VARCHAR(50) NOT NULL,
来源：http://bc.chemitech.net.cn

email VARCHAR(100) UNIQUE,
来源：http://ej.jctech888.com.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://qk.huanxung.cn

);
来源：http://un.521024.cn

[Q02] 创建带外键的表
来源：http://ev.521024.cn

CREATE TABLE orders (
来源：http://sw.nszjky.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://xx.jianghongdianzi.cn

user_id INT NOT NULL,
来源：http://zn.nicolike.cn

amount DECIMAL(10, 2),
来源：http://vm.panjiajie.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mw.huixiangedu.cn

);
来源：http://vu.jianghongdianzi.cn

[Q03] 增加列
来源：http://wx.shxzskj.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://qb.huixiangedu.cn

[Q04] 修改列类型
来源：http://ng.newstarts.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://kt.wgjwhj.cn

[Q05] 重命名列
来源：http://km.hnjuh.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://uk.shtwfgs.cn

[Q06] 删除列
来源：http://rc.yuexingan06.cn

ALTER TABLE users DROP COLUMN age;
来源：http://jr.newstarts.cn

[Q07] 删除表
来源：http://yz.colortex.cn

DROP TABLE IF EXISTS orders;
来源：http://xt.jianghongdianzi.cn

[Q08] 创建普通索引
来源：http://qm.shxzukj.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://iu.gzmigu.cn

[Q09] 创建唯一索引
来源：http://ty.szsharing.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://se.jianghongdianzi.cn

[Q10] 插入单行
来源：http://ko.hahajie.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mz.szxytkj.cn

[Q11] 一次插入多行
来源：http://ix.bookmarksfly.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://gk.shxzskj.cn

[Q12] 插入后取自增 ID
来源：http://re.gzmigu.cn

INSERT INTO users (name) VALUES ('C');
来源：http://ft.chemitech.net.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://fo.521024.cn

[Q13] 忽略重复插入
来源：http://hk.521024.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://jd.hahajie.cn

[Q14] 存在则更新（upsert）
来源：http://nk.newstarts.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hg.bjjhwx.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ej.huixiangedu.cn

[Q15] 查询全部
来源：http://dl.hahajie.cn

SELECT * FROM users;
来源：http://dp.shtwfgs.cn

[Q16] 查询指定列
来源：http://os.jctech888.com.cn

SELECT id, name FROM users;
来源：http://hk.hnjuh.cn

[Q17] 条件查询
来源：http://cc.huanxung.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ta.huixinmuqiang.cn

[Q18] 模糊匹配
来源：http://bm.chemitech.net.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://uc.muxihuayi.cn

[Q19] 范围查询
来源：http://pf.521024.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ts.jctech888.com.cn

[Q20] IN 列表
来源：http://sg.huixiangedu.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ar.huixiangedu.cn

[Q21] 空值判断
来源：http://dj.colortex.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://lb.chemitech.net.cn

[Q22] 排序
来源：http://xg.bookmarksfly.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ju.muxihuayi.cn

[Q23] 分页
来源：http://mq.nicolike.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://li.huixinmuqiang.cn

[Q24] 去重
来源：http://jm.521024.cn

SELECT DISTINCT city FROM users;
来源：http://hv.muxihuayi.cn

[Q25] 只取前 N 条
来源：http://aq.9csxet.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://qw.newstarts.cn

[Q26] 计数
来源：http://dz.hnjuh.cn

SELECT COUNT(*) FROM users;
来源：http://mc.panjiajie.cn

[Q27] 条件计数
来源：http://pm.huixinmuqiang.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wc.shxzukj.cn

[Q28] 求和与平均
来源：http://iu.jianghongdianzi.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://fz.bookmarksfly.cn

[Q29] 最大最小值
来源：http://lj.shxzskj.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://cq.9csxet.cn

[Q30] 分组统计
来源：http://zf.lnxyls.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ai.nicolike.cn

[Q31] 分组后过滤
来源：http://ot.huanxung.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://sh.szxytkj.cn

[Q32] 分组拼接字符串
来源：http://ca.huixiangedu.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://yl.shtwfgs.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://zi.lnxyls.cn

[Q33] 多列分组
来源：http://pv.nszjky.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://kr.shtwfgs.cn

[Q34] 每组取第一条
来源：http://vj.newstarts.cn

SELECT * FROM (
来源：http://zn.yuntaijiaju.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://qk.shxzukj.cn

) t WHERE rn = 1;
来源：http://br.nicolike.cn

[Q35] 内连接
来源：http://it.521024.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://dy.hnjuh.cn

[Q36] 左连接
来源：http://iy.9csxet.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://sn.hnjuh.cn

[Q37] 右连接
来源：http://ot.shtwfgs.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://jr.lnxyls.cn

[Q38] 全外连接（PostgreSQL）
来源：http://xn.huanxung.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wi.haigaiapp.cn

[Q39] 自连接（查上下级）
来源：http://do.haigaiapp.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://tv.colortex.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hr.asd995.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://az.huanxung.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ab.huixiangedu.cn

[Q41] 多表连接
来源：http://fh.szsharing.cn


<!-- 参考信息 -->