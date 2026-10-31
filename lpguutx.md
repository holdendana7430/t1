代发 wailian999

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://qm.lnxyls.cn

[N06] 判断回文字符串
来源：http://ha.hnjuh.cn

Py:   s == s[::-1]
来源：http://ww.lnxyls.cn

PHP:  $s === strrev($s);
来源：http://lk.521024.cn

JS:   s === [...s].reverse().join("")
来源：http://hb.huixinmuqiang.cn

TS:   s === [...s].reverse().join("")
来源：http://gq.hahajie.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ct.bookmarksfly.cn

Go:   // 双指针从两端比较
来源：http://ev.bookmarksfly.cn

Ruby: s == s.reverse
来源：http://og.lnxyls.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://cx.gzmigu.cn

[N07] 两数之和（返回下标）
来源：http://fl.szsharing.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://dv.wgjwhj.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://xk.shxzskj.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://yi.9csxet.cn

TS:   // 手写 Map<string, number>
来源：http://yz.huanxung.cn

Java: // 手写 HashMap
来源：http://xa.asd995.cn

Go:   // 手写 map[int]int
来源：http://dt.colortex.cn

Ruby: // 手写 Hash
来源：http://gk.haigaiapp.cn

C#:   // 手写 Dictionary<int, int>
来源：http://to.huixinmuqiang.cn

[N08] 生成全排列
来源：http://it.chemitech.net.cn

Py:   itertools.permutations(arr)
来源：http://wv.wgjwhj.cn

PHP:  // 手写递归交换
来源：http://cr.521024.cn

JS:   // 手写回溯递归
来源：http://bi.jianghongdianzi.cn

TS:   // 手写回溯递归
来源：http://fv.9csxet.cn

Java: // 手写回溯递归
来源：http://uu.huanxung.cn

Go:   // 手写回溯递归
来源：http://pc.shxzukj.cn

Ruby: arr.permutation.to_a
来源：http://kt.chemitech.net.cn

C#:   // 手写回溯递归
来源：http://lc.bookmarksfly.cn

[N09] 栈与队列
来源：http://jg.shtwfgs.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wb.shxzskj.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://dt.jctech888.com.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://nq.chemitech.net.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ju.shtwfgs.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://zh.lnxyls.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ot.huixinmuqiang.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://jd.szxytkj.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://vw.haigaiapp.cn

[N10] 链表节点定义
来源：http://yo.szsharing.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://yr.panjiajie.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://kf.haigaiapp.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://pv.shxzskj.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ok.jianghongdianzi.cn

Java: class Node { int v; Node next; }
来源：http://bb.yuntaijiaju.cn

Go:   type Node struct { V int; Next *Node }
来源：http://xc.hnjuh.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://fg.huanxung.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://ek.hahajie.cn

[N11] 二叉树中序遍历
来源：http://gz.chemitech.net.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://dk.lnxyls.cn

PHP:  // 手写递归函数
来源：http://fq.muxihuayi.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://fn.newstarts.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://oh.asd995.cn

Java: // 手写递归
来源：http://ai.wgjwhj.cn

Go:   // 手写递归
来源：http://wb.9csxet.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ht.bjjhwx.cn

C#:   // 手写递归
来源：http://vr.haigaiapp.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://rs.huixiangedu.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://fu.hnjuh.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://kb.chemitech.net.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://jy.yuntaijiaju.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wo.jianghongdianzi.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ht.szsharing.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://bb.hnjuh.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://xm.szxytkj.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://sr.521024.cn

================================================================================
来源：http://iw.yuntaijiaju.cn

O. 并发与异步
来源：http://nn.chemitech.net.cn

================================================================================
来源：http://nn.chemitech.net.cn

[O01] 启动一个线程
来源：http://ww.9csxet.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://cs.asd995.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://np.yuexingan06.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wb.yuntaijiaju.cn

TS:   // 同 JS
来源：http://fg.jctech888.com.cn

Java: new Thread(() -> f()).start()
来源：http://pl.bjjhwx.cn

Go:   go f()
来源：http://kf.shxzukj.cn

Ruby: Thread.new { f }
来源：http://tw.hahajie.cn

C#:   Task.Run(() => F());
来源：http://fc.yuexingan06.cn

[O02] 使用线程池
来源：http://yq.lnxyls.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ev.haigaiapp.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://fb.huixinmuqiang.cn

JS:   // worker_threads 线程池
来源：http://xy.colortex.cn

TS:   // worker_threads 线程池
来源：http://lg.shxzukj.cn

Java: Executors.newFixedThreadPool(4)
来源：http://nh.bjjhwx.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://kg.bookmarksfly.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mx.shxzukj.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://gg.newstarts.cn

[O03] 加锁保护共享数据
来源：http://mg.huanxung.cn

Py:   with lock: shared += 1
来源：http://lv.huixinmuqiang.cn

PHP:  // 用 flock() 做文件锁
来源：http://ad.shtwfgs.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://rc.chemitech.net.cn

TS:   // 同 JS
来源：http://nk.nszjky.cn

Java: synchronized (this) { shared++; }
来源：http://bk.9csxet.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ex.hahajie.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://xs.haigaiapp.cn

C#:   lock (gate) { shared++; }
来源：http://yf.muxihuayi.cn

[O04] 定义异步函数并等待
来源：http://nv.panjiajie.cn

Py:   async def f():⏎    await g()
来源：http://sn.bookmarksfly.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://zu.yuntaijiaju.cn

JS:   async function f() { await g(); }
来源：http://ms.huixiangedu.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://hs.muxihuayi.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://az.jctech888.com.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://se.hahajie.cn

Ruby: # 用 Fiber 或 async gem
来源：http://qi.jctech888.com.cn

C#:   async Task F() { await G(); }
来源：http://qg.shxzukj.cn

[O05] 并发执行并等待全部完成
来源：http://xj.bjjhwx.cn

Py:   asyncio.gather(*tasks)
来源：http://gx.huixiangedu.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hg.lnxyls.cn

JS:   await Promise.all(tasks)
来源：http://bq.nicolike.cn

TS:   await Promise.all(tasks)
来源：http://ly.huixiangedu.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://pk.muxihuayi.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://do.yuntaijiaju.cn

Ruby: threads.map(&:join)
来源：http://lk.jianghongdianzi.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://ig.nicolike.cn

[O06] 使用进程池
来源：http://ck.muxihuayi.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ru.wgjwhj.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://pe.szxytkj.cn

JS:   // child_process / cluster 模块
来源：http://qj.huixinmuqiang.cn

TS:   // child_process / cluster 模块
来源：http://xk.bjjhwx.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hn.huanxung.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mn.gzmigu.cn

Ruby: // fork 块
来源：http://py.yuntaijiaju.cn

C#:   Parallel.For
来源：http://qa.521024.cn

================================================================================
来源：http://yw.shxzskj.cn

P. 常用工具函数
来源：http://vq.gzmigu.cn

================================================================================
来源：http://ix.colortex.cn

[P01] 生成 UUID
来源：http://qd.nicolike.cn

Py:   str(uuid.uuid4())
来源：http://yd.huanxung.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ya.bookmarksfly.cn

JS:   crypto.randomUUID()
来源：http://it.lnxyls.cn

TS:   crypto.randomUUID()
来源：http://mp.yuexingan06.cn

Java: UUID.randomUUID().toString()
来源：http://vg.lnxyls.cn

Go:   // 用 github.com/google/uuid
来源：http://kr.bjjhwx.cn

Ruby: SecureRandom.uuid
来源：http://tt.lnxyls.cn

C#:   Guid.NewGuid().ToString()
来源：http://oc.shxzukj.cn

[P02] MD5 / SHA256 摘要
来源：http://cz.szxytkj.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://uq.hahajie.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://zu.jianghongdianzi.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://qx.jctech888.com.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://rs.szsharing.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://kv.haigaiapp.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ug.gzmigu.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://sx.asd995.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://yd.chemitech.net.cn

[P03] 生成短随机字符串
来源：http://wp.yuexingan06.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://xy.nicolike.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://xm.colortex.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hi.jianghongdianzi.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://yo.hahajie.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://bn.nicolike.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://yx.jianghongdianzi.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://zq.newstarts.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wo.nicolike.cn

[P04] 求长度
来源：http://ye.shtwfgs.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://tk.nicolike.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://sk.colortex.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://jh.yuntaijiaju.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://kc.nszjky.cn

Java: list.size();  map.size();  s.length()
来源：http://qi.panjiajie.cn

Go:   len(arr);  len(m)
来源：http://jx.nszjky.cn

Ruby: x.length;  x.size
来源：http://nr.huixinmuqiang.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://ng.hnjuh.cn

[P05] 判断两个对象内容是否相等
来源：http://oc.jianghongdianzi.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://zs.shxzukj.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://pp.haigaiapp.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hx.jianghongdianzi.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://no.szsharing.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://yb.jianghongdianzi.cn

Go:   reflect.DeepEqual(a, b)
来源：http://zz.haigaiapp.cn

Ruby: a == b
来源：http://bj.jianghongdianzi.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://su.nicolike.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://la.shxzukj.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://pj.9csxet.cn

PHP:  if (empty($x)) {}
来源：http://jd.huanxung.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ud.wgjwhj.cn

TS:   if (x == null) {}
来源：http://em.hnjuh.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://pn.hahajie.cn

Go:   if x == nil {}
来源：http://vy.asd995.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hf.panjiajie.cn

C#:   if (x is null) {}
来源：http://cl.hahajie.cn

[P07] 防抖与节流
来源：http://ad.lnxyls.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://zf.521024.cn

PHP:  // 手写时间戳比较
来源：http://tb.521024.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://op.szxytkj.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://fw.colortex.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ws.panjiajie.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://qw.hahajie.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://tb.jctech888.com.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mc.asd995.cn

[P08] 处理浮点精度问题
来源：http://id.huixiangedu.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ox.bjjhwx.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ll.jianghongdianzi.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://gy.huanxung.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ox.lnxyls.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ql.muxihuayi.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://yy.colortex.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://yy.chemitech.net.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://pd.newstarts.cn

================================================================================
来源：http://fn.huanxung.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ln.haigaiapp.cn

================================================================================
来源：http://rm.nicolike.cn

[Q01] 创建表
来源：http://xu.521024.cn

CREATE TABLE users (
来源：http://pu.jctech888.com.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://qe.shtwfgs.cn

name VARCHAR(50) NOT NULL,
来源：http://fi.huanxung.cn

email VARCHAR(100) UNIQUE,
来源：http://qj.hnjuh.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mj.nszjky.cn

);
来源：http://oi.jianghongdianzi.cn

[Q02] 创建带外键的表
来源：http://sg.huanxung.cn

CREATE TABLE orders (
来源：http://mi.szxytkj.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hc.muxihuayi.cn

user_id INT NOT NULL,
来源：http://cl.shxzukj.cn

amount DECIMAL(10, 2),
来源：http://dg.huanxung.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://lf.hnjuh.cn

);
来源：http://hn.nszjky.cn

[Q03] 增加列
来源：http://qd.nicolike.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://kf.9csxet.cn

[Q04] 修改列类型
来源：http://fm.bjjhwx.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://cg.chemitech.net.cn

[Q05] 重命名列
来源：http://ay.szsharing.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mw.521024.cn

[Q06] 删除列
来源：http://mb.szxytkj.cn

ALTER TABLE users DROP COLUMN age;
来源：http://tz.yuntaijiaju.cn

[Q07] 删除表
来源：http://er.huixinmuqiang.cn

DROP TABLE IF EXISTS orders;
来源：http://aa.yuntaijiaju.cn

[Q08] 创建普通索引
来源：http://nj.hahajie.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://rc.shxzskj.cn

[Q09] 创建唯一索引
来源：http://rb.szxytkj.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://cv.nszjky.cn

[Q10] 插入单行
来源：http://bl.chemitech.net.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ji.huixinmuqiang.cn

[Q11] 一次插入多行
来源：http://sd.newstarts.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://da.haigaiapp.cn

[Q12] 插入后取自增 ID
来源：http://oh.huixinmuqiang.cn

INSERT INTO users (name) VALUES ('C');
来源：http://op.chemitech.net.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://vw.panjiajie.cn

[Q13] 忽略重复插入
来源：http://hp.jctech888.com.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://yi.szxytkj.cn

[Q14] 存在则更新（upsert）
来源：http://sx.colortex.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://rj.newstarts.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wm.szsharing.cn

[Q15] 查询全部
来源：http://ds.shxzukj.cn

SELECT * FROM users;
来源：http://vh.colortex.cn

[Q16] 查询指定列
来源：http://mf.521024.cn

SELECT id, name FROM users;
来源：http://yv.gzmigu.cn

[Q17] 条件查询
来源：http://ws.bjjhwx.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://dg.huixiangedu.cn

[Q18] 模糊匹配
来源：http://bl.shxzskj.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://kc.9csxet.cn

[Q19] 范围查询
来源：http://xi.hnjuh.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://er.huixiangedu.cn

[Q20] IN 列表
来源：http://yw.bjjhwx.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://yf.szxytkj.cn

[Q21] 空值判断
来源：http://ig.jianghongdianzi.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://lp.huanxung.cn

[Q22] 排序
来源：http://tt.huixiangedu.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://kl.521024.cn

[Q23] 分页
来源：http://up.shtwfgs.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://vk.jctech888.com.cn

[Q24] 去重
来源：http://lj.bookmarksfly.cn

SELECT DISTINCT city FROM users;
来源：http://nr.chemitech.net.cn

[Q25] 只取前 N 条
来源：http://xd.gzmigu.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ej.chemitech.net.cn

[Q26] 计数
来源：http://th.asd995.cn

SELECT COUNT(*) FROM users;
来源：http://am.huixiangedu.cn

[Q27] 条件计数
来源：http://ts.nszjky.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://na.szsharing.cn

[Q28] 求和与平均
来源：http://qt.yuntaijiaju.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://jv.lnxyls.cn

[Q29] 最大最小值
来源：http://kc.hahajie.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://bx.shxzskj.cn

[Q30] 分组统计
来源：http://xo.521024.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://jh.gzmigu.cn

[Q31] 分组后过滤
来源：http://ab.gzmigu.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://am.yuexingan06.cn

[Q32] 分组拼接字符串
来源：http://us.huixinmuqiang.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://yq.szxytkj.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://qt.szxytkj.cn

[Q33] 多列分组
来源：http://zi.nicolike.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wu.yuntaijiaju.cn

[Q34] 每组取第一条
来源：http://uu.huixiangedu.cn

SELECT * FROM (
来源：http://du.yuntaijiaju.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://xb.gzmigu.cn

) t WHERE rn = 1;
来源：http://mb.szsharing.cn

[Q35] 内连接
来源：http://qc.huixiangedu.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://rx.szsharing.cn

[Q36] 左连接
来源：http://uc.gzmigu.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://me.shtwfgs.cn

[Q37] 右连接
来源：http://nc.gzmigu.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hg.szsharing.cn

[Q38] 全外连接（PostgreSQL）
来源：http://sm.521024.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://fk.lnxyls.cn

[Q39] 自连接（查上下级）
来源：http://ek.asd995.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://zh.jianghongdianzi.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://nk.hnjuh.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://gd.jianghongdianzi.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://je.colortex.cn

[Q41] 多表连接
来源：http://xn.yuntaijiaju.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://jn.colortex.cn

JOIN users u ON u.id = o.user_id
来源：http://kt.shtwfgs.cn

JOIN products p ON p.id = o.product_id;
来源：http://tg.szxytkj.cn

[Q42] 连接条件附加过滤
来源：http://fv.jianghongdianzi.cn


<!-- 参考信息 -->