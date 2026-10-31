代发 wailian999

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://jh.shxzukj.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wx.panjiajie.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://fi.hahajie.cn

Ruby: a.gcd(b)
来源：http://fk.muxihuayi.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://bv.shxzskj.cn

[N06] 判断回文字符串
来源：http://ms.chemitech.net.cn

Py:   s == s[::-1]
来源：http://ui.nicolike.cn

PHP:  $s === strrev($s);
来源：http://bv.huixinmuqiang.cn

JS:   s === [...s].reverse().join("")
来源：http://my.hahajie.cn

TS:   s === [...s].reverse().join("")
来源：http://cy.9csxet.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://oo.bjjhwx.cn

Go:   // 双指针从两端比较
来源：http://hm.asd995.cn

Ruby: s == s.reverse
来源：http://we.bookmarksfly.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://cm.huixiangedu.cn

[N07] 两数之和（返回下标）
来源：http://nr.jianghongdianzi.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://vj.asd995.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://nz.wgjwhj.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://ct.shxzukj.cn

TS:   // 手写 Map<string, number>
来源：http://ar.panjiajie.cn

Java: // 手写 HashMap
来源：http://vi.shxzskj.cn

Go:   // 手写 map[int]int
来源：http://my.huanxung.cn

Ruby: // 手写 Hash
来源：http://zr.9csxet.cn

C#:   // 手写 Dictionary<int, int>
来源：http://ge.nszjky.cn

[N08] 生成全排列
来源：http://te.521024.cn

Py:   itertools.permutations(arr)
来源：http://yo.jctech888.com.cn

PHP:  // 手写递归交换
来源：http://zz.wgjwhj.cn

JS:   // 手写回溯递归
来源：http://gj.bookmarksfly.cn

TS:   // 手写回溯递归
来源：http://ia.muxihuayi.cn

Java: // 手写回溯递归
来源：http://kv.panjiajie.cn

Go:   // 手写回溯递归
来源：http://jd.yuexingan06.cn

Ruby: arr.permutation.to_a
来源：http://zp.szxytkj.cn

C#:   // 手写回溯递归
来源：http://ar.huixiangedu.cn

[N09] 栈与队列
来源：http://og.bookmarksfly.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ah.nszjky.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://pr.huixinmuqiang.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wn.gzmigu.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://rh.bookmarksfly.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://db.bookmarksfly.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ap.nicolike.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ei.huanxung.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://tn.huanxung.cn

[N10] 链表节点定义
来源：http://mf.szxytkj.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://br.jianghongdianzi.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://mh.shxzskj.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://bd.yuntaijiaju.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://nv.gzmigu.cn

Java: class Node { int v; Node next; }
来源：http://ea.9csxet.cn

Go:   type Node struct { V int; Next *Node }
来源：http://ow.lnxyls.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://ru.colortex.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://cm.yuexingan06.cn

[N11] 二叉树中序遍历
来源：http://su.huanxung.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hk.chemitech.net.cn

PHP:  // 手写递归函数
来源：http://fd.bookmarksfly.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://cs.huixiangedu.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://eo.9csxet.cn

Java: // 手写递归
来源：http://qk.panjiajie.cn

Go:   // 手写递归
来源：http://bv.hahajie.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://xv.panjiajie.cn

C#:   // 手写递归
来源：http://bb.szxytkj.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ee.asd995.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://qo.newstarts.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://xn.shxzukj.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://uk.shxzskj.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ef.nicolike.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://bt.szsharing.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://th.521024.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://im.chemitech.net.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://cq.hahajie.cn

================================================================================
来源：http://te.haigaiapp.cn

O. 并发与异步
来源：http://vf.jianghongdianzi.cn

================================================================================
来源：http://sp.huanxung.cn

[O01] 启动一个线程
来源：http://ul.newstarts.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://jw.bookmarksfly.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://dc.asd995.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://bq.chemitech.net.cn

TS:   // 同 JS
来源：http://eb.asd995.cn

Java: new Thread(() -> f()).start()
来源：http://fj.jianghongdianzi.cn

Go:   go f()
来源：http://ah.huixinmuqiang.cn

Ruby: Thread.new { f }
来源：http://ss.shxzukj.cn

C#:   Task.Run(() => F());
来源：http://mp.muxihuayi.cn

[O02] 使用线程池
来源：http://be.9csxet.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://rq.lnxyls.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://kz.hahajie.cn

JS:   // worker_threads 线程池
来源：http://ne.nszjky.cn

TS:   // worker_threads 线程池
来源：http://bt.nszjky.cn

Java: Executors.newFixedThreadPool(4)
来源：http://ow.yuexingan06.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://zg.bjjhwx.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://dl.szxytkj.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://vc.wgjwhj.cn

[O03] 加锁保护共享数据
来源：http://wc.shtwfgs.cn

Py:   with lock: shared += 1
来源：http://sa.lnxyls.cn

PHP:  // 用 flock() 做文件锁
来源：http://ss.yuexingan06.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ob.muxihuayi.cn

TS:   // 同 JS
来源：http://jl.lnxyls.cn

Java: synchronized (this) { shared++; }
来源：http://kd.newstarts.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://pk.hahajie.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://lw.jianghongdianzi.cn

C#:   lock (gate) { shared++; }
来源：http://pt.9csxet.cn

[O04] 定义异步函数并等待
来源：http://nl.bjjhwx.cn

Py:   async def f():⏎    await g()
来源：http://ku.jianghongdianzi.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://yp.gzmigu.cn

JS:   async function f() { await g(); }
来源：http://ue.yuntaijiaju.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://qn.huixiangedu.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://nu.bookmarksfly.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ji.lnxyls.cn

Ruby: # 用 Fiber 或 async gem
来源：http://jn.nicolike.cn

C#:   async Task F() { await G(); }
来源：http://ir.yuntaijiaju.cn

[O05] 并发执行并等待全部完成
来源：http://tp.9csxet.cn

Py:   asyncio.gather(*tasks)
来源：http://sd.hahajie.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://dw.jianghongdianzi.cn

JS:   await Promise.all(tasks)
来源：http://ar.wgjwhj.cn

TS:   await Promise.all(tasks)
来源：http://io.yuntaijiaju.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ms.yuexingan06.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://yl.bjjhwx.cn

Ruby: threads.map(&:join)
来源：http://kq.hahajie.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://ui.huanxung.cn

[O06] 使用进程池
来源：http://bj.asd995.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://jo.colortex.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://ty.jctech888.com.cn

JS:   // child_process / cluster 模块
来源：http://vs.9csxet.cn

TS:   // child_process / cluster 模块
来源：http://jo.shxzukj.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://sz.wgjwhj.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://nm.hahajie.cn

Ruby: // fork 块
来源：http://li.shxzukj.cn

C#:   Parallel.For
来源：http://kt.shxzskj.cn

================================================================================
来源：http://mb.huanxung.cn

P. 常用工具函数
来源：http://dg.nszjky.cn

================================================================================
来源：http://ma.newstarts.cn

[P01] 生成 UUID
来源：http://pk.hahajie.cn

Py:   str(uuid.uuid4())
来源：http://yl.nicolike.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://cp.nicolike.cn

JS:   crypto.randomUUID()
来源：http://se.yuntaijiaju.cn

TS:   crypto.randomUUID()
来源：http://ry.newstarts.cn

Java: UUID.randomUUID().toString()
来源：http://ma.yuexingan06.cn

Go:   // 用 github.com/google/uuid
来源：http://ms.bjjhwx.cn

Ruby: SecureRandom.uuid
来源：http://bv.wgjwhj.cn

C#:   Guid.NewGuid().ToString()
来源：http://pt.shxzskj.cn

[P02] MD5 / SHA256 摘要
来源：http://zt.shxzskj.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://im.haigaiapp.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://pg.chemitech.net.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://je.521024.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://af.jctech888.com.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://rx.colortex.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://zh.wgjwhj.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://vn.9csxet.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://an.huixinmuqiang.cn

[P03] 生成短随机字符串
来源：http://zy.bjjhwx.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://im.bookmarksfly.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://df.shxzukj.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://tz.jianghongdianzi.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://bf.colortex.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ge.haigaiapp.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://jw.shxzukj.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://jp.shxzukj.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://sq.lnxyls.cn

[P04] 求长度
来源：http://mg.hnjuh.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://qs.chemitech.net.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://qe.bjjhwx.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://vy.szxytkj.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ro.shxzukj.cn

Java: list.size();  map.size();  s.length()
来源：http://mr.bjjhwx.cn

Go:   len(arr);  len(m)
来源：http://qn.huixinmuqiang.cn

Ruby: x.length;  x.size
来源：http://ui.bjjhwx.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://ji.shxzskj.cn

[P05] 判断两个对象内容是否相等
来源：http://tv.huixinmuqiang.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://em.colortex.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://me.huixiangedu.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://uf.shxzukj.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://zr.huixiangedu.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ol.huanxung.cn

Go:   reflect.DeepEqual(a, b)
来源：http://hm.9csxet.cn

Ruby: a == b
来源：http://ai.bjjhwx.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://qg.shxzskj.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://bm.bookmarksfly.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://uu.yuexingan06.cn

PHP:  if (empty($x)) {}
来源：http://cb.asd995.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://gh.gzmigu.cn

TS:   if (x == null) {}
来源：http://dm.szxytkj.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://hh.huixiangedu.cn

Go:   if x == nil {}
来源：http://bp.jctech888.com.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://oe.hnjuh.cn

C#:   if (x is null) {}
来源：http://lz.shtwfgs.cn

[P07] 防抖与节流
来源：http://iu.hnjuh.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://yf.huixiangedu.cn

PHP:  // 手写时间戳比较
来源：http://gx.shtwfgs.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://db.lnxyls.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wx.nicolike.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wi.9csxet.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hc.huixinmuqiang.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://hx.shxzskj.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://gq.hnjuh.cn

[P08] 处理浮点精度问题
来源：http://ov.shtwfgs.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://kn.szxytkj.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://xe.nszjky.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://de.huanxung.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://fl.jctech888.com.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://fj.nszjky.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://fr.asd995.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wh.haigaiapp.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://yo.szxytkj.cn

================================================================================
来源：http://wv.haigaiapp.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://yq.lnxyls.cn

================================================================================
来源：http://yp.521024.cn

[Q01] 创建表
来源：http://hc.haigaiapp.cn

CREATE TABLE users (
来源：http://wa.szsharing.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ns.bjjhwx.cn

name VARCHAR(50) NOT NULL,
来源：http://sq.9csxet.cn

email VARCHAR(100) UNIQUE,
来源：http://ez.panjiajie.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://um.yuexingan06.cn

);
来源：http://rp.jctech888.com.cn

[Q02] 创建带外键的表
来源：http://aa.asd995.cn

CREATE TABLE orders (
来源：http://wv.huixinmuqiang.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://cu.521024.cn

user_id INT NOT NULL,
来源：http://ie.wgjwhj.cn

amount DECIMAL(10, 2),
来源：http://do.bookmarksfly.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://yn.hnjuh.cn

);
来源：http://ly.muxihuayi.cn

[Q03] 增加列
来源：http://ee.szsharing.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://rm.gzmigu.cn

[Q04] 修改列类型
来源：http://xq.huanxung.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://yy.hahajie.cn

[Q05] 重命名列
来源：http://eu.panjiajie.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://li.wgjwhj.cn

[Q06] 删除列
来源：http://ce.shxzskj.cn

ALTER TABLE users DROP COLUMN age;
来源：http://ak.jianghongdianzi.cn

[Q07] 删除表
来源：http://zj.yuntaijiaju.cn

DROP TABLE IF EXISTS orders;
来源：http://fm.newstarts.cn

[Q08] 创建普通索引
来源：http://it.nicolike.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://nu.huixinmuqiang.cn

[Q09] 创建唯一索引
来源：http://zv.bjjhwx.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://bd.shtwfgs.cn

[Q10] 插入单行
来源：http://ll.shxzukj.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ms.szsharing.cn

[Q11] 一次插入多行
来源：http://ko.lnxyls.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://fh.huixiangedu.cn

[Q12] 插入后取自增 ID
来源：http://tb.muxihuayi.cn

INSERT INTO users (name) VALUES ('C');
来源：http://js.hahajie.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://gb.huanxung.cn

[Q13] 忽略重复插入
来源：http://oz.haigaiapp.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://tr.jianghongdianzi.cn

[Q14] 存在则更新（upsert）
来源：http://sk.colortex.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://br.bjjhwx.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://fl.9csxet.cn

[Q15] 查询全部
来源：http://bs.nszjky.cn

SELECT * FROM users;
来源：http://uq.gzmigu.cn

[Q16] 查询指定列
来源：http://ro.muxihuayi.cn

SELECT id, name FROM users;
来源：http://jg.lnxyls.cn

[Q17] 条件查询
来源：http://co.hahajie.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ug.colortex.cn

[Q18] 模糊匹配
来源：http://ab.huixiangedu.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://cl.asd995.cn

[Q19] 范围查询
来源：http://bd.bookmarksfly.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://nd.muxihuayi.cn

[Q20] IN 列表
来源：http://im.szxytkj.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://nj.shxzskj.cn

[Q21] 空值判断
来源：http://fe.huixinmuqiang.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://jq.nicolike.cn

[Q22] 排序
来源：http://cs.yuntaijiaju.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://nr.nicolike.cn

[Q23] 分页
来源：http://yk.chemitech.net.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://er.hnjuh.cn

[Q24] 去重
来源：http://ox.szsharing.cn

SELECT DISTINCT city FROM users;
来源：http://re.panjiajie.cn

[Q25] 只取前 N 条
来源：http://oy.panjiajie.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://yw.shtwfgs.cn

[Q26] 计数
来源：http://mu.nicolike.cn

SELECT COUNT(*) FROM users;
来源：http://ic.nszjky.cn

[Q27] 条件计数
来源：http://ok.huixinmuqiang.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ri.shxzskj.cn

[Q28] 求和与平均
来源：http://bl.huixinmuqiang.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://gg.muxihuayi.cn

[Q29] 最大最小值
来源：http://fv.huixinmuqiang.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://tt.jctech888.com.cn

[Q30] 分组统计
来源：http://ql.huixiangedu.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://xi.shxzskj.cn

[Q31] 分组后过滤
来源：http://kf.bookmarksfly.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ud.muxihuayi.cn

[Q32] 分组拼接字符串
来源：http://ds.jctech888.com.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://tt.newstarts.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://gy.haigaiapp.cn

[Q33] 多列分组
来源：http://gc.bookmarksfly.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://le.hahajie.cn

[Q34] 每组取第一条
来源：http://ko.haigaiapp.cn

SELECT * FROM (
来源：http://rq.colortex.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ur.wgjwhj.cn

) t WHERE rn = 1;
来源：http://eb.muxihuayi.cn

[Q35] 内连接
来源：http://mz.muxihuayi.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://gy.wgjwhj.cn

[Q36] 左连接
来源：http://la.jctech888.com.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://yc.shxzukj.cn

[Q37] 右连接
来源：http://ay.hahajie.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://kc.lnxyls.cn

[Q38] 全外连接（PostgreSQL）
来源：http://zb.hahajie.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://gp.nszjky.cn

[Q39] 自连接（查上下级）
来源：http://yc.nicolike.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://rq.colortex.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ew.shtwfgs.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://td.szsharing.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://xi.9csxet.cn

[Q41] 多表连接
来源：http://jr.lnxyls.cn


<!-- 参考信息 -->