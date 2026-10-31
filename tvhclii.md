代发 wailian999

Go:   // 手写 map[int]int
来源：http://tj.huixiangedu.cn

Ruby: // 手写 Hash
来源：http://va.szxytkj.cn

C#:   // 手写 Dictionary<int, int>
来源：http://ek.shxzukj.cn

[N08] 生成全排列
来源：http://rv.chemitech.net.cn

Py:   itertools.permutations(arr)
来源：http://oi.shtwfgs.cn

PHP:  // 手写递归交换
来源：http://iv.chemitech.net.cn

JS:   // 手写回溯递归
来源：http://mf.huixiangedu.cn

TS:   // 手写回溯递归
来源：http://mx.yuexingan06.cn

Java: // 手写回溯递归
来源：http://ev.lnxyls.cn

Go:   // 手写回溯递归
来源：http://fj.szsharing.cn

Ruby: arr.permutation.to_a
来源：http://ni.lnxyls.cn

C#:   // 手写回溯递归
来源：http://da.hnjuh.cn

[N09] 栈与队列
来源：http://cn.521024.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ev.muxihuayi.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://vm.lnxyls.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://vq.yuexingan06.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://sh.bookmarksfly.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://lz.muxihuayi.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://la.wgjwhj.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://cr.yuexingan06.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://cy.nicolike.cn

[N10] 链表节点定义
来源：http://vh.szsharing.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://yc.shxzskj.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://zw.521024.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://xc.shtwfgs.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://dp.szsharing.cn

Java: class Node { int v; Node next; }
来源：http://gy.wgjwhj.cn

Go:   type Node struct { V int; Next *Node }
来源：http://ej.gzmigu.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://cv.newstarts.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://id.gzmigu.cn

[N11] 二叉树中序遍历
来源：http://pg.shtwfgs.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ey.huixiangedu.cn

PHP:  // 手写递归函数
来源：http://sc.huixiangedu.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://jq.9csxet.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://tv.lnxyls.cn

Java: // 手写递归
来源：http://bm.jctech888.com.cn

Go:   // 手写递归
来源：http://ut.521024.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ui.muxihuayi.cn

C#:   // 手写递归
来源：http://in.lnxyls.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://os.huixiangedu.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://bs.yuntaijiaju.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://qb.shtwfgs.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mu.muxihuayi.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ph.muxihuayi.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://im.muxihuayi.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://is.gzmigu.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ja.muxihuayi.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ow.jctech888.com.cn

================================================================================
来源：http://rb.chemitech.net.cn

O. 并发与异步
来源：http://sh.yuntaijiaju.cn

================================================================================
来源：http://gs.szsharing.cn

[O01] 启动一个线程
来源：http://ga.chemitech.net.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://sa.haigaiapp.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ae.haigaiapp.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://kx.521024.cn

TS:   // 同 JS
来源：http://wo.hnjuh.cn

Java: new Thread(() -> f()).start()
来源：http://wf.9csxet.cn

Go:   go f()
来源：http://zj.huixiangedu.cn

Ruby: Thread.new { f }
来源：http://rh.shxzskj.cn

C#:   Task.Run(() => F());
来源：http://ab.szxytkj.cn

[O02] 使用线程池
来源：http://yl.shxzskj.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hk.bookmarksfly.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://gw.huixinmuqiang.cn

JS:   // worker_threads 线程池
来源：http://oc.gzmigu.cn

TS:   // worker_threads 线程池
来源：http://bn.shtwfgs.cn

Java: Executors.newFixedThreadPool(4)
来源：http://je.521024.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://lz.chemitech.net.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://fs.jctech888.com.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://tj.nicolike.cn

[O03] 加锁保护共享数据
来源：http://iu.bjjhwx.cn

Py:   with lock: shared += 1
来源：http://qj.panjiajie.cn

PHP:  // 用 flock() 做文件锁
来源：http://ow.gzmigu.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://or.nicolike.cn

TS:   // 同 JS
来源：http://xb.yuexingan06.cn

Java: synchronized (this) { shared++; }
来源：http://rw.jianghongdianzi.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://qi.nszjky.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://cp.jianghongdianzi.cn

C#:   lock (gate) { shared++; }
来源：http://kd.bookmarksfly.cn

[O04] 定义异步函数并等待
来源：http://kv.haigaiapp.cn

Py:   async def f():⏎    await g()
来源：http://ky.asd995.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wm.bookmarksfly.cn

JS:   async function f() { await g(); }
来源：http://ix.szxytkj.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://ue.huanxung.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://cl.huixiangedu.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ql.gzmigu.cn

Ruby: # 用 Fiber 或 async gem
来源：http://ge.chemitech.net.cn

C#:   async Task F() { await G(); }
来源：http://ri.bookmarksfly.cn

[O05] 并发执行并等待全部完成
来源：http://wg.yuexingan06.cn

Py:   asyncio.gather(*tasks)
来源：http://nh.asd995.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://uy.bookmarksfly.cn

JS:   await Promise.all(tasks)
来源：http://dd.newstarts.cn

TS:   await Promise.all(tasks)
来源：http://gp.panjiajie.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://tq.newstarts.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://db.yuexingan06.cn

Ruby: threads.map(&:join)
来源：http://jn.huanxung.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://jv.huixinmuqiang.cn

[O06] 使用进程池
来源：http://df.lnxyls.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://da.yuntaijiaju.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://fe.jianghongdianzi.cn

JS:   // child_process / cluster 模块
来源：http://yt.bjjhwx.cn

TS:   // child_process / cluster 模块
来源：http://yg.shxzukj.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://tx.asd995.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ch.jianghongdianzi.cn

Ruby: // fork 块
来源：http://il.huanxung.cn

C#:   Parallel.For
来源：http://is.bookmarksfly.cn

================================================================================
来源：http://hj.shxzskj.cn

P. 常用工具函数
来源：http://gv.jctech888.com.cn

================================================================================
来源：http://pa.szxytkj.cn

[P01] 生成 UUID
来源：http://jw.huixinmuqiang.cn

Py:   str(uuid.uuid4())
来源：http://ud.yuexingan06.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hn.jianghongdianzi.cn

JS:   crypto.randomUUID()
来源：http://il.muxihuayi.cn

TS:   crypto.randomUUID()
来源：http://wh.jianghongdianzi.cn

Java: UUID.randomUUID().toString()
来源：http://hl.lnxyls.cn

Go:   // 用 github.com/google/uuid
来源：http://rf.bookmarksfly.cn

Ruby: SecureRandom.uuid
来源：http://jg.haigaiapp.cn

C#:   Guid.NewGuid().ToString()
来源：http://wq.521024.cn

[P02] MD5 / SHA256 摘要
来源：http://cy.wgjwhj.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://vk.nicolike.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://kw.muxihuayi.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ma.panjiajie.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mu.colortex.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://om.huixiangedu.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ba.huixinmuqiang.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://eb.wgjwhj.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://da.shxzskj.cn

[P03] 生成短随机字符串
来源：http://xn.nszjky.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://tb.nszjky.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://aa.haigaiapp.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://fi.huixinmuqiang.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://xw.hnjuh.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://yl.panjiajie.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://sm.nszjky.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://ia.nszjky.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://qp.szxytkj.cn

[P04] 求长度
来源：http://jo.chemitech.net.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://zi.colortex.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://bn.muxihuayi.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://iu.szxytkj.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wk.jianghongdianzi.cn

Java: list.size();  map.size();  s.length()
来源：http://uu.muxihuayi.cn

Go:   len(arr);  len(m)
来源：http://mw.shtwfgs.cn

Ruby: x.length;  x.size
来源：http://cq.huixinmuqiang.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://ri.9csxet.cn

[P05] 判断两个对象内容是否相等
来源：http://ty.yuntaijiaju.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://nk.bookmarksfly.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://dp.haigaiapp.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://iu.yuexingan06.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://sh.yuexingan06.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ox.nszjky.cn

Go:   reflect.DeepEqual(a, b)
来源：http://sl.haigaiapp.cn

Ruby: a == b
来源：http://cc.jctech888.com.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://nu.chemitech.net.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://oi.shxzukj.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hw.huixinmuqiang.cn

PHP:  if (empty($x)) {}
来源：http://gq.gzmigu.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wx.jctech888.com.cn

TS:   if (x == null) {}
来源：http://wp.bjjhwx.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://yb.szsharing.cn

Go:   if x == nil {}
来源：http://cn.szxytkj.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://bk.9csxet.cn

C#:   if (x is null) {}
来源：http://lx.lnxyls.cn

[P07] 防抖与节流
来源：http://qt.colortex.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ui.wgjwhj.cn

PHP:  // 手写时间戳比较
来源：http://fu.hahajie.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://en.huixinmuqiang.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hp.huixiangedu.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://jv.wgjwhj.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ft.hnjuh.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://fr.huixinmuqiang.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://go.colortex.cn

[P08] 处理浮点精度问题
来源：http://fw.asd995.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ss.9csxet.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hf.shxzukj.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://bt.yuntaijiaju.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://qf.shxzskj.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ib.lnxyls.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://lw.szsharing.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://id.shtwfgs.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ip.szsharing.cn

================================================================================
来源：http://gc.haigaiapp.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ui.panjiajie.cn

================================================================================
来源：http://ir.yuexingan06.cn

[Q01] 创建表
来源：http://te.chemitech.net.cn

CREATE TABLE users (
来源：http://ww.jianghongdianzi.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://vd.gzmigu.cn

name VARCHAR(50) NOT NULL,
来源：http://qd.9csxet.cn

email VARCHAR(100) UNIQUE,
来源：http://al.bjjhwx.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://kn.lnxyls.cn

);
来源：http://cd.jianghongdianzi.cn

[Q02] 创建带外键的表
来源：http://gk.9csxet.cn

CREATE TABLE orders (
来源：http://xr.jctech888.com.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://yx.chemitech.net.cn

user_id INT NOT NULL,
来源：http://wz.muxihuayi.cn

amount DECIMAL(10, 2),
来源：http://pv.nszjky.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://jx.521024.cn

);
来源：http://cv.huanxung.cn

[Q03] 增加列
来源：http://kw.wgjwhj.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://vz.shxzukj.cn

[Q04] 修改列类型
来源：http://tb.muxihuayi.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://el.muxihuayi.cn

[Q05] 重命名列
来源：http://ih.yuntaijiaju.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://zo.nszjky.cn

[Q06] 删除列
来源：http://oe.chemitech.net.cn

ALTER TABLE users DROP COLUMN age;
来源：http://is.jctech888.com.cn

[Q07] 删除表
来源：http://ph.bookmarksfly.cn

DROP TABLE IF EXISTS orders;
来源：http://ok.huixinmuqiang.cn

[Q08] 创建普通索引
来源：http://ug.nicolike.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://pw.panjiajie.cn

[Q09] 创建唯一索引
来源：http://ei.lnxyls.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wx.lnxyls.cn

[Q10] 插入单行
来源：http://qv.bookmarksfly.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://zy.szsharing.cn

[Q11] 一次插入多行
来源：http://zp.chemitech.net.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://jp.panjiajie.cn

[Q12] 插入后取自增 ID
来源：http://tr.muxihuayi.cn

INSERT INTO users (name) VALUES ('C');
来源：http://ym.shxzskj.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://tq.huixiangedu.cn

[Q13] 忽略重复插入
来源：http://au.haigaiapp.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://jo.asd995.cn

[Q14] 存在则更新（upsert）
来源：http://gm.huixinmuqiang.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://db.huanxung.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://nx.jianghongdianzi.cn

[Q15] 查询全部
来源：http://va.colortex.cn

SELECT * FROM users;
来源：http://it.jianghongdianzi.cn

[Q16] 查询指定列
来源：http://lr.haigaiapp.cn

SELECT id, name FROM users;
来源：http://pi.hahajie.cn

[Q17] 条件查询
来源：http://oa.colortex.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://fr.nszjky.cn

[Q18] 模糊匹配
来源：http://yy.hnjuh.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://rr.hnjuh.cn

[Q19] 范围查询
来源：http://ra.shtwfgs.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://rz.bookmarksfly.cn

[Q20] IN 列表
来源：http://jb.asd995.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://lp.jctech888.com.cn

[Q21] 空值判断
来源：http://bt.nicolike.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://uy.szsharing.cn

[Q22] 排序
来源：http://hc.gzmigu.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ib.bjjhwx.cn

[Q23] 分页
来源：http://fk.colortex.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://qq.521024.cn

[Q24] 去重
来源：http://rn.yuexingan06.cn

SELECT DISTINCT city FROM users;
来源：http://sf.yuexingan06.cn

[Q25] 只取前 N 条
来源：http://kd.szxytkj.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wr.panjiajie.cn

[Q26] 计数
来源：http://oa.jctech888.com.cn

SELECT COUNT(*) FROM users;
来源：http://wc.nicolike.cn

[Q27] 条件计数
来源：http://jm.9csxet.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ng.nicolike.cn

[Q28] 求和与平均
来源：http://on.panjiajie.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://gv.gzmigu.cn

[Q29] 最大最小值
来源：http://yi.panjiajie.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://im.huixinmuqiang.cn

[Q30] 分组统计
来源：http://vy.gzmigu.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://aq.yuexingan06.cn

[Q31] 分组后过滤
来源：http://rj.9csxet.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://pt.hnjuh.cn

[Q32] 分组拼接字符串
来源：http://qr.yuntaijiaju.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://xk.bjjhwx.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://vj.jctech888.com.cn

[Q33] 多列分组
来源：http://qg.panjiajie.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wc.hahajie.cn

[Q34] 每组取第一条
来源：http://tz.hahajie.cn

SELECT * FROM (
来源：http://lw.wgjwhj.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ko.gzmigu.cn

) t WHERE rn = 1;
来源：http://tl.panjiajie.cn

[Q35] 内连接
来源：http://pz.yuexingan06.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://eo.gzmigu.cn

[Q36] 左连接
来源：http://ba.bookmarksfly.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://qy.hnjuh.cn

[Q37] 右连接
来源：http://im.wgjwhj.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://au.nszjky.cn

[Q38] 全外连接（PostgreSQL）
来源：http://zj.shtwfgs.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://nk.huanxung.cn

[Q39] 自连接（查上下级）
来源：http://wg.chemitech.net.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://tw.yuntaijiaju.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://iz.bjjhwx.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://ih.bookmarksfly.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://bj.szxytkj.cn

[Q41] 多表连接
来源：http://nm.yuexingan06.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://ho.panjiajie.cn

JOIN users u ON u.id = o.user_id
来源：http://ik.hahajie.cn

JOIN products p ON p.id = o.product_id;
来源：http://io.haigaiapp.cn

[Q42] 连接条件附加过滤
来源：http://kv.huixiangedu.cn

SELECT u.name, o.amount FROM users u
来源：http://cz.muxihuayi.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://fl.huixinmuqiang.cn

[Q43] 标量子查询
来源：http://ul.gzmigu.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hx.shtwfgs.cn

[Q44] IN 子查询
来源：http://qj.huixinmuqiang.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://jk.panjiajie.cn

[Q45] EXISTS 判断存在
来源：http://fi.szsharing.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wh.asd995.cn

[Q46] NOT EXISTS 判断不存在
来源：http://tg.521024.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://is.gzmigu.cn

[Q47] 与平均值比较
来源：http://hl.yuntaijiaju.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://nx.9csxet.cn

[Q48] CTE 公用表表达式
来源：http://hb.nszjky.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://sp.colortex.cn

SELECT * FROM t WHERE c > 5;
来源：http://ae.haigaiapp.cn

[Q49] 更新单行
来源：http://sx.shtwfgs.cn


<!-- 参考信息 -->