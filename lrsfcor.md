代发 wailian999

JS:   s === [...s].reverse().join("")
来源：http://tc.yuntaijiaju.cn

TS:   s === [...s].reverse().join("")
来源：http://kj.bookmarksfly.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://pp.521024.cn

Go:   // 双指针从两端比较
来源：http://jr.hnjuh.cn

Ruby: s == s.reverse
来源：http://ms.szxytkj.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://dc.newstarts.cn

[N07] 两数之和（返回下标）
来源：http://bo.yuntaijiaju.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://oy.chemitech.net.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://lq.jctech888.com.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://he.colortex.cn

TS:   // 手写 Map<string, number>
来源：http://nq.jctech888.com.cn

Java: // 手写 HashMap
来源：http://ok.gzmigu.cn

Go:   // 手写 map[int]int
来源：http://ck.huanxung.cn

Ruby: // 手写 Hash
来源：http://kv.shxzukj.cn

C#:   // 手写 Dictionary<int, int>
来源：http://dc.haigaiapp.cn

[N08] 生成全排列
来源：http://wu.521024.cn

Py:   itertools.permutations(arr)
来源：http://vv.colortex.cn

PHP:  // 手写递归交换
来源：http://kq.jianghongdianzi.cn

JS:   // 手写回溯递归
来源：http://qn.hahajie.cn

TS:   // 手写回溯递归
来源：http://ft.wgjwhj.cn

Java: // 手写回溯递归
来源：http://pm.yuntaijiaju.cn

Go:   // 手写回溯递归
来源：http://jr.nicolike.cn

Ruby: arr.permutation.to_a
来源：http://rr.szsharing.cn

C#:   // 手写回溯递归
来源：http://sf.hahajie.cn

[N09] 栈与队列
来源：http://hz.hnjuh.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wi.colortex.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://cb.bookmarksfly.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://qj.colortex.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://nx.szsharing.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://bk.szxytkj.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://xn.haigaiapp.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ky.shtwfgs.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://gx.bookmarksfly.cn

[N10] 链表节点定义
来源：http://xj.haigaiapp.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mo.huixiangedu.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://cg.muxihuayi.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ve.szxytkj.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://bl.shxzukj.cn

Java: class Node { int v; Node next; }
来源：http://ae.wgjwhj.cn

Go:   type Node struct { V int; Next *Node }
来源：http://qj.9csxet.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://ao.jianghongdianzi.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://eb.huixinmuqiang.cn

[N11] 二叉树中序遍历
来源：http://ny.chemitech.net.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://nq.huanxung.cn

PHP:  // 手写递归函数
来源：http://qu.jianghongdianzi.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wg.yuexingan06.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://dt.huixiangedu.cn

Java: // 手写递归
来源：http://in.szxytkj.cn

Go:   // 手写递归
来源：http://ah.bjjhwx.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://dg.colortex.cn

C#:   // 手写递归
来源：http://tw.521024.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ag.newstarts.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://jn.yuexingan06.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://nk.nszjky.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://xu.jianghongdianzi.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://jf.shtwfgs.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://jj.shtwfgs.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ow.jctech888.com.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://bu.shxzskj.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://pa.chemitech.net.cn

================================================================================
来源：http://qi.shxzskj.cn

O. 并发与异步
来源：http://gw.9csxet.cn

================================================================================
来源：http://yc.bjjhwx.cn

[O01] 启动一个线程
来源：http://ns.huixinmuqiang.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://sb.shxzukj.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ip.newstarts.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ua.gzmigu.cn

TS:   // 同 JS
来源：http://cl.panjiajie.cn

Java: new Thread(() -> f()).start()
来源：http://fm.bjjhwx.cn

Go:   go f()
来源：http://ba.chemitech.net.cn

Ruby: Thread.new { f }
来源：http://sk.newstarts.cn

C#:   Task.Run(() => F());
来源：http://kv.huanxung.cn

[O02] 使用线程池
来源：http://xv.haigaiapp.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ge.yuntaijiaju.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://zn.yuexingan06.cn

JS:   // worker_threads 线程池
来源：http://dw.newstarts.cn

TS:   // worker_threads 线程池
来源：http://qs.bjjhwx.cn

Java: Executors.newFixedThreadPool(4)
来源：http://jy.szxytkj.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://lp.newstarts.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://sp.hahajie.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://op.chemitech.net.cn

[O03] 加锁保护共享数据
来源：http://fs.bjjhwx.cn

Py:   with lock: shared += 1
来源：http://ud.jctech888.com.cn

PHP:  // 用 flock() 做文件锁
来源：http://dr.shxzskj.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://nr.521024.cn

TS:   // 同 JS
来源：http://fc.bookmarksfly.cn

Java: synchronized (this) { shared++; }
来源：http://hl.shtwfgs.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ca.huixinmuqiang.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://mc.bookmarksfly.cn

C#:   lock (gate) { shared++; }
来源：http://qj.haigaiapp.cn

[O04] 定义异步函数并等待
来源：http://mp.nszjky.cn

Py:   async def f():⏎    await g()
来源：http://te.muxihuayi.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://vl.hahajie.cn

JS:   async function f() { await g(); }
来源：http://eg.szxytkj.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://zx.huixinmuqiang.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://se.asd995.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://lc.lnxyls.cn

Ruby: # 用 Fiber 或 async gem
来源：http://hv.muxihuayi.cn

C#:   async Task F() { await G(); }
来源：http://qi.chemitech.net.cn

[O05] 并发执行并等待全部完成
来源：http://ek.szxytkj.cn

Py:   asyncio.gather(*tasks)
来源：http://sz.haigaiapp.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://tq.gzmigu.cn

JS:   await Promise.all(tasks)
来源：http://lt.yuexingan06.cn

TS:   await Promise.all(tasks)
来源：http://sw.huixinmuqiang.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://lr.bookmarksfly.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://bz.jctech888.com.cn

Ruby: threads.map(&:join)
来源：http://zh.shxzskj.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://zo.muxihuayi.cn

[O06] 使用进程池
来源：http://cp.newstarts.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://pv.nszjky.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://en.wgjwhj.cn

JS:   // child_process / cluster 模块
来源：http://kp.newstarts.cn

TS:   // child_process / cluster 模块
来源：http://tw.521024.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://su.wgjwhj.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ek.asd995.cn

Ruby: // fork 块
来源：http://pq.szxytkj.cn

C#:   Parallel.For
来源：http://fx.jianghongdianzi.cn

================================================================================
来源：http://ov.huixiangedu.cn

P. 常用工具函数
来源：http://rn.bookmarksfly.cn

================================================================================
来源：http://cb.hahajie.cn

[P01] 生成 UUID
来源：http://ai.shxzskj.cn

Py:   str(uuid.uuid4())
来源：http://au.huanxung.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://nw.hahajie.cn

JS:   crypto.randomUUID()
来源：http://zc.bookmarksfly.cn

TS:   crypto.randomUUID()
来源：http://zy.chemitech.net.cn

Java: UUID.randomUUID().toString()
来源：http://ee.huanxung.cn

Go:   // 用 github.com/google/uuid
来源：http://xh.huixiangedu.cn

Ruby: SecureRandom.uuid
来源：http://lm.panjiajie.cn

C#:   Guid.NewGuid().ToString()
来源：http://sn.muxihuayi.cn

[P02] MD5 / SHA256 摘要
来源：http://lc.szsharing.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://cm.hnjuh.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://cs.yuexingan06.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://kg.shtwfgs.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://db.panjiajie.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wf.521024.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mk.nicolike.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://bw.huanxung.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://bt.muxihuayi.cn

[P03] 生成短随机字符串
来源：http://tn.hahajie.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://qh.jianghongdianzi.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://fp.bookmarksfly.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://zv.jianghongdianzi.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ms.huixinmuqiang.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://yr.shtwfgs.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://rz.gzmigu.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://wb.yuntaijiaju.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://xz.shtwfgs.cn

[P04] 求长度
来源：http://hj.panjiajie.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ss.yuexingan06.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://kp.yuntaijiaju.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://iu.asd995.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wt.huanxung.cn

Java: list.size();  map.size();  s.length()
来源：http://kz.521024.cn

Go:   len(arr);  len(m)
来源：http://wq.nicolike.cn

Ruby: x.length;  x.size
来源：http://eh.wgjwhj.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://hd.bjjhwx.cn

[P05] 判断两个对象内容是否相等
来源：http://rs.yuntaijiaju.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://ly.jctech888.com.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://va.huixinmuqiang.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://qp.szxytkj.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://nh.bookmarksfly.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://vi.hnjuh.cn

Go:   reflect.DeepEqual(a, b)
来源：http://js.huixiangedu.cn

Ruby: a == b
来源：http://ja.wgjwhj.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://et.shxzskj.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ym.szsharing.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://zy.muxihuayi.cn

PHP:  if (empty($x)) {}
来源：http://dy.bookmarksfly.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mc.colortex.cn

TS:   if (x == null) {}
来源：http://qn.huixinmuqiang.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://ew.lnxyls.cn

Go:   if x == nil {}
来源：http://ng.lnxyls.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://co.wgjwhj.cn

C#:   if (x is null) {}
来源：http://om.huixiangedu.cn

[P07] 防抖与节流
来源：http://lw.wgjwhj.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://sj.yuntaijiaju.cn

PHP:  // 手写时间戳比较
来源：http://ua.wgjwhj.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ae.szsharing.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ld.wgjwhj.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ln.jctech888.com.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://tn.bookmarksfly.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://am.lnxyls.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://an.bjjhwx.cn

[P08] 处理浮点精度问题
来源：http://zu.nszjky.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ox.chemitech.net.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://cg.chemitech.net.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mp.huanxung.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://lm.yuexingan06.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://sl.bjjhwx.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://dg.chemitech.net.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://dz.chemitech.net.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://pt.szxytkj.cn

================================================================================
来源：http://cl.newstarts.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://oe.bookmarksfly.cn

================================================================================
来源：http://or.9csxet.cn

[Q01] 创建表
来源：http://nq.colortex.cn

CREATE TABLE users (
来源：http://td.lnxyls.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://lf.bjjhwx.cn

name VARCHAR(50) NOT NULL,
来源：http://al.szsharing.cn

email VARCHAR(100) UNIQUE,
来源：http://xm.chemitech.net.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://gi.bookmarksfly.cn

);
来源：http://na.jctech888.com.cn

[Q02] 创建带外键的表
来源：http://yp.chemitech.net.cn

CREATE TABLE orders (
来源：http://jd.huixiangedu.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://eo.jianghongdianzi.cn

user_id INT NOT NULL,
来源：http://df.9csxet.cn

amount DECIMAL(10, 2),
来源：http://nx.wgjwhj.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://nm.szxytkj.cn

);
来源：http://iq.shtwfgs.cn

[Q03] 增加列
来源：http://zm.hnjuh.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ih.haigaiapp.cn

[Q04] 修改列类型
来源：http://mq.newstarts.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://nv.yuntaijiaju.cn

[Q05] 重命名列
来源：http://hy.huanxung.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hm.bjjhwx.cn

[Q06] 删除列
来源：http://ls.haigaiapp.cn

ALTER TABLE users DROP COLUMN age;
来源：http://wq.muxihuayi.cn

[Q07] 删除表
来源：http://mq.wgjwhj.cn

DROP TABLE IF EXISTS orders;
来源：http://zk.huixinmuqiang.cn

[Q08] 创建普通索引
来源：http://zo.haigaiapp.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://ng.shxzskj.cn

[Q09] 创建唯一索引
来源：http://ri.bookmarksfly.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://zk.shxzskj.cn

[Q10] 插入单行
来源：http://sx.gzmigu.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://zm.asd995.cn

[Q11] 一次插入多行
来源：http://qj.shtwfgs.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://tx.nicolike.cn

[Q12] 插入后取自增 ID
来源：http://lo.gzmigu.cn

INSERT INTO users (name) VALUES ('C');
来源：http://iu.lnxyls.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wl.panjiajie.cn

[Q13] 忽略重复插入
来源：http://kb.huixiangedu.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://fn.bookmarksfly.cn

[Q14] 存在则更新（upsert）
来源：http://el.jianghongdianzi.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ep.muxihuayi.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ek.bjjhwx.cn

[Q15] 查询全部
来源：http://zh.gzmigu.cn

SELECT * FROM users;
来源：http://wm.bookmarksfly.cn

[Q16] 查询指定列
来源：http://jb.521024.cn

SELECT id, name FROM users;
来源：http://iy.szxytkj.cn

[Q17] 条件查询
来源：http://tx.yuexingan06.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://kw.szsharing.cn

[Q18] 模糊匹配
来源：http://ps.jctech888.com.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wz.yuntaijiaju.cn

[Q19] 范围查询
来源：http://mp.hnjuh.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://rp.szxytkj.cn

[Q20] IN 列表
来源：http://ym.hahajie.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://yq.shxzskj.cn

[Q21] 空值判断
来源：http://xw.nicolike.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://fq.szxytkj.cn

[Q22] 排序
来源：http://xh.huixinmuqiang.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://eu.szxytkj.cn

[Q23] 分页
来源：http://fs.nicolike.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://gl.hahajie.cn

[Q24] 去重
来源：http://ty.jianghongdianzi.cn

SELECT DISTINCT city FROM users;
来源：http://lb.newstarts.cn

[Q25] 只取前 N 条
来源：http://na.lnxyls.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://gb.colortex.cn

[Q26] 计数
来源：http://vv.szsharing.cn

SELECT COUNT(*) FROM users;
来源：http://kk.muxihuayi.cn

[Q27] 条件计数
来源：http://ew.yuexingan06.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://gg.nszjky.cn

[Q28] 求和与平均
来源：http://jr.9csxet.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://vx.szxytkj.cn

[Q29] 最大最小值
来源：http://gp.9csxet.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://ot.hnjuh.cn

[Q30] 分组统计
来源：http://yc.szxytkj.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://dw.huixinmuqiang.cn

[Q31] 分组后过滤
来源：http://ux.chemitech.net.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://vb.huanxung.cn

[Q32] 分组拼接字符串
来源：http://gx.yuexingan06.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://qv.wgjwhj.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://rq.huanxung.cn

[Q33] 多列分组
来源：http://xp.gzmigu.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://py.hahajie.cn

[Q34] 每组取第一条
来源：http://ar.huixinmuqiang.cn

SELECT * FROM (
来源：http://ms.muxihuayi.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://xq.wgjwhj.cn

) t WHERE rn = 1;
来源：http://ws.lnxyls.cn

[Q35] 内连接
来源：http://dy.muxihuayi.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://gf.huixinmuqiang.cn

[Q36] 左连接
来源：http://kz.yuexingan06.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://kv.hnjuh.cn

[Q37] 右连接
来源：http://tr.haigaiapp.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://gl.yuexingan06.cn

[Q38] 全外连接（PostgreSQL）
来源：http://gv.521024.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://sr.huanxung.cn

[Q39] 自连接（查上下级）
来源：http://qp.newstarts.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://gt.9csxet.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://bc.bookmarksfly.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://fr.huixiangedu.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ye.yuntaijiaju.cn

[Q41] 多表连接
来源：http://ea.9csxet.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://zh.bookmarksfly.cn

JOIN users u ON u.id = o.user_id
来源：http://tc.bjjhwx.cn

JOIN products p ON p.id = o.product_id;
来源：http://ff.colortex.cn

[Q42] 连接条件附加过滤
来源：http://rx.hnjuh.cn

SELECT u.name, o.amount FROM users u
来源：http://ew.wgjwhj.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://xo.9csxet.cn

[Q43] 标量子查询
来源：http://ej.lnxyls.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://qn.shtwfgs.cn


<!-- 参考信息 -->