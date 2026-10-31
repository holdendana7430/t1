代发 wailian999

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://cf.shxzskj.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://fp.lnxyls.cn

TS:   // 手写 Map<string, number>
来源：http://li.huixinmuqiang.cn

Java: // 手写 HashMap
来源：http://hl.yuexingan06.cn

Go:   // 手写 map[int]int
来源：http://oh.nicolike.cn

Ruby: // 手写 Hash
来源：http://wb.nicolike.cn

C#:   // 手写 Dictionary<int, int>
来源：http://mp.muxihuayi.cn

[N08] 生成全排列
来源：http://qe.panjiajie.cn

Py:   itertools.permutations(arr)
来源：http://co.nicolike.cn

PHP:  // 手写递归交换
来源：http://gs.asd995.cn

JS:   // 手写回溯递归
来源：http://vi.yuntaijiaju.cn

TS:   // 手写回溯递归
来源：http://tj.asd995.cn

Java: // 手写回溯递归
来源：http://fi.bookmarksfly.cn

Go:   // 手写回溯递归
来源：http://lx.shxzukj.cn

Ruby: arr.permutation.to_a
来源：http://op.haigaiapp.cn

C#:   // 手写回溯递归
来源：http://ak.haigaiapp.cn

[N09] 栈与队列
来源：http://qw.huixiangedu.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://at.lnxyls.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://yc.wgjwhj.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ia.asd995.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://rs.huixiangedu.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ad.bookmarksfly.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://fe.muxihuayi.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://rb.huixiangedu.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://vn.yuntaijiaju.cn

[N10] 链表节点定义
来源：http://fo.shxzukj.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://qq.chemitech.net.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://ya.shxzukj.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://gb.yuexingan06.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://rk.huixinmuqiang.cn

Java: class Node { int v; Node next; }
来源：http://gl.521024.cn

Go:   type Node struct { V int; Next *Node }
来源：http://hb.shxzskj.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://xr.9csxet.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://ce.shxzukj.cn

[N11] 二叉树中序遍历
来源：http://ik.yuntaijiaju.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://bw.jctech888.com.cn

PHP:  // 手写递归函数
来源：http://em.asd995.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ft.haigaiapp.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://kp.yuexingan06.cn

Java: // 手写递归
来源：http://hp.shtwfgs.cn

Go:   // 手写递归
来源：http://lw.newstarts.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://gm.jctech888.com.cn

C#:   // 手写递归
来源：http://ns.huixiangedu.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://uz.colortex.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hl.hnjuh.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://jj.szsharing.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://tu.lnxyls.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ub.asd995.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://vb.yuntaijiaju.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mq.bjjhwx.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://rz.shxzukj.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://df.yuexingan06.cn

================================================================================
来源：http://tn.huixiangedu.cn

O. 并发与异步
来源：http://fx.shxzskj.cn

================================================================================
来源：http://im.wgjwhj.cn

[O01] 启动一个线程
来源：http://nu.hahajie.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://qw.asd995.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://xb.colortex.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://cv.panjiajie.cn

TS:   // 同 JS
来源：http://vq.hnjuh.cn

Java: new Thread(() -> f()).start()
来源：http://xx.521024.cn

Go:   go f()
来源：http://ny.bjjhwx.cn

Ruby: Thread.new { f }
来源：http://nj.yuntaijiaju.cn

C#:   Task.Run(() => F());
来源：http://iu.shxzskj.cn

[O02] 使用线程池
来源：http://xy.huixinmuqiang.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://fq.521024.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wr.hahajie.cn

JS:   // worker_threads 线程池
来源：http://la.huanxung.cn

TS:   // worker_threads 线程池
来源：http://di.shxzskj.cn

Java: Executors.newFixedThreadPool(4)
来源：http://fv.hahajie.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://bk.lnxyls.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://np.huixinmuqiang.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://qx.huixiangedu.cn

[O03] 加锁保护共享数据
来源：http://jz.nszjky.cn

Py:   with lock: shared += 1
来源：http://sa.hnjuh.cn

PHP:  // 用 flock() 做文件锁
来源：http://bd.szsharing.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://dq.asd995.cn

TS:   // 同 JS
来源：http://dc.hnjuh.cn

Java: synchronized (this) { shared++; }
来源：http://sf.bookmarksfly.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://he.521024.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://nk.nicolike.cn

C#:   lock (gate) { shared++; }
来源：http://pr.9csxet.cn

[O04] 定义异步函数并等待
来源：http://jn.wgjwhj.cn

Py:   async def f():⏎    await g()
来源：http://xr.shtwfgs.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://kl.gzmigu.cn

JS:   async function f() { await g(); }
来源：http://mm.newstarts.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://it.huanxung.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://cv.jctech888.com.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://xv.9csxet.cn

Ruby: # 用 Fiber 或 async gem
来源：http://ny.jianghongdianzi.cn

C#:   async Task F() { await G(); }
来源：http://lv.yuntaijiaju.cn

[O05] 并发执行并等待全部完成
来源：http://ze.jctech888.com.cn

Py:   asyncio.gather(*tasks)
来源：http://ub.shxzskj.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://iw.lnxyls.cn

JS:   await Promise.all(tasks)
来源：http://nh.szxytkj.cn

TS:   await Promise.all(tasks)
来源：http://lo.hahajie.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://oq.shxzskj.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hn.newstarts.cn

Ruby: threads.map(&:join)
来源：http://cr.huixinmuqiang.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://dy.chemitech.net.cn

[O06] 使用进程池
来源：http://rm.9csxet.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ii.shxzukj.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://lt.hahajie.cn

JS:   // child_process / cluster 模块
来源：http://ft.haigaiapp.cn

TS:   // child_process / cluster 模块
来源：http://zd.shxzukj.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://oj.wgjwhj.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ja.colortex.cn

Ruby: // fork 块
来源：http://ae.muxihuayi.cn

C#:   Parallel.For
来源：http://eg.wgjwhj.cn

================================================================================
来源：http://cc.bookmarksfly.cn

P. 常用工具函数
来源：http://at.shxzskj.cn

================================================================================
来源：http://rf.jctech888.com.cn

[P01] 生成 UUID
来源：http://cb.lnxyls.cn

Py:   str(uuid.uuid4())
来源：http://yn.nszjky.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://jm.wgjwhj.cn

JS:   crypto.randomUUID()
来源：http://nn.szsharing.cn

TS:   crypto.randomUUID()
来源：http://um.hnjuh.cn

Java: UUID.randomUUID().toString()
来源：http://uk.huixinmuqiang.cn

Go:   // 用 github.com/google/uuid
来源：http://od.muxihuayi.cn

Ruby: SecureRandom.uuid
来源：http://iu.nszjky.cn

C#:   Guid.NewGuid().ToString()
来源：http://ga.bjjhwx.cn

[P02] MD5 / SHA256 摘要
来源：http://wf.521024.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://uu.colortex.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://wr.haigaiapp.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://sn.shxzukj.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://fx.szxytkj.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://pd.newstarts.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://oj.szxytkj.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://fg.huixinmuqiang.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://yd.yuexingan06.cn

[P03] 生成短随机字符串
来源：http://wv.huixiangedu.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://tn.chemitech.net.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://iq.bookmarksfly.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ji.jianghongdianzi.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ir.shxzskj.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hy.jianghongdianzi.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://rs.newstarts.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://zv.szxytkj.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://su.bjjhwx.cn

[P04] 求长度
来源：http://ft.newstarts.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://vj.jctech888.com.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ek.wgjwhj.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://kj.haigaiapp.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ma.huanxung.cn

Java: list.size();  map.size();  s.length()
来源：http://yp.521024.cn

Go:   len(arr);  len(m)
来源：http://dr.huixinmuqiang.cn

Ruby: x.length;  x.size
来源：http://hc.newstarts.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://sg.nicolike.cn

[P05] 判断两个对象内容是否相等
来源：http://hj.asd995.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://ri.shtwfgs.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ab.huixinmuqiang.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://tq.yuexingan06.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://sr.521024.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wa.shxzukj.cn

Go:   reflect.DeepEqual(a, b)
来源：http://gy.9csxet.cn

Ruby: a == b
来源：http://ec.wgjwhj.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ix.yuntaijiaju.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ql.huixinmuqiang.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://sc.asd995.cn

PHP:  if (empty($x)) {}
来源：http://qj.yuntaijiaju.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ri.9csxet.cn

TS:   if (x == null) {}
来源：http://zq.521024.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://xt.521024.cn

Go:   if x == nil {}
来源：http://kl.szsharing.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://df.wgjwhj.cn

C#:   if (x is null) {}
来源：http://hi.hnjuh.cn

[P07] 防抖与节流
来源：http://ko.521024.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ux.nszjky.cn

PHP:  // 手写时间戳比较
来源：http://pr.shxzskj.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://gk.jctech888.com.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hk.huixinmuqiang.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://og.jianghongdianzi.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ug.jctech888.com.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://md.jctech888.com.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ub.lnxyls.cn

[P08] 处理浮点精度问题
来源：http://ij.yuexingan06.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://qr.panjiajie.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://bd.huanxung.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ii.panjiajie.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://tt.panjiajie.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://gy.wgjwhj.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ds.lnxyls.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ra.shtwfgs.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://xd.nszjky.cn

================================================================================
来源：http://tz.shxzskj.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hk.colortex.cn

================================================================================
来源：http://op.wgjwhj.cn

[Q01] 创建表
来源：http://qq.bookmarksfly.cn

CREATE TABLE users (
来源：http://jn.lnxyls.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://oz.huixinmuqiang.cn

name VARCHAR(50) NOT NULL,
来源：http://iv.panjiajie.cn

email VARCHAR(100) UNIQUE,
来源：http://br.szxytkj.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://cz.jianghongdianzi.cn

);
来源：http://wd.521024.cn

[Q02] 创建带外键的表
来源：http://qz.colortex.cn

CREATE TABLE orders (
来源：http://bm.gzmigu.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://pd.shtwfgs.cn

user_id INT NOT NULL,
来源：http://cp.nicolike.cn

amount DECIMAL(10, 2),
来源：http://yj.bjjhwx.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://pk.shxzukj.cn

);
来源：http://fm.muxihuayi.cn

[Q03] 增加列
来源：http://si.yuntaijiaju.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ji.shxzskj.cn

[Q04] 修改列类型
来源：http://fu.shxzskj.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hv.gzmigu.cn

[Q05] 重命名列
来源：http://av.gzmigu.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://yc.nicolike.cn

[Q06] 删除列
来源：http://gz.haigaiapp.cn

ALTER TABLE users DROP COLUMN age;
来源：http://pw.shxzskj.cn

[Q07] 删除表
来源：http://is.newstarts.cn

DROP TABLE IF EXISTS orders;
来源：http://dr.yuntaijiaju.cn

[Q08] 创建普通索引
来源：http://sh.jctech888.com.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://sb.haigaiapp.cn

[Q09] 创建唯一索引
来源：http://jj.colortex.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ik.hahajie.cn

[Q10] 插入单行
来源：http://gz.jctech888.com.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://fb.521024.cn

[Q11] 一次插入多行
来源：http://rv.yuexingan06.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://yo.yuntaijiaju.cn

[Q12] 插入后取自增 ID
来源：http://ed.hahajie.cn

INSERT INTO users (name) VALUES ('C');
来源：http://ft.panjiajie.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ea.nicolike.cn

[Q13] 忽略重复插入
来源：http://xm.szxytkj.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wj.bookmarksfly.cn

[Q14] 存在则更新（upsert）
来源：http://ag.jctech888.com.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mg.yuexingan06.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mh.bookmarksfly.cn

[Q15] 查询全部
来源：http://hn.shtwfgs.cn

SELECT * FROM users;
来源：http://ym.9csxet.cn

[Q16] 查询指定列
来源：http://ds.newstarts.cn

SELECT id, name FROM users;
来源：http://kd.521024.cn

[Q17] 条件查询
来源：http://lh.jianghongdianzi.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ai.lnxyls.cn

[Q18] 模糊匹配
来源：http://mo.bookmarksfly.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://pi.muxihuayi.cn

[Q19] 范围查询
来源：http://ah.newstarts.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://dm.bookmarksfly.cn

[Q20] IN 列表
来源：http://pc.521024.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://yg.gzmigu.cn

[Q21] 空值判断
来源：http://ds.chemitech.net.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://kl.gzmigu.cn

[Q22] 排序
来源：http://gq.gzmigu.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://xn.hnjuh.cn

[Q23] 分页
来源：http://pm.szsharing.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ot.newstarts.cn

[Q24] 去重
来源：http://bg.bjjhwx.cn

SELECT DISTINCT city FROM users;
来源：http://jg.shxzukj.cn

[Q25] 只取前 N 条
来源：http://rm.hnjuh.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ko.jianghongdianzi.cn

[Q26] 计数
来源：http://zf.huixinmuqiang.cn

SELECT COUNT(*) FROM users;
来源：http://ov.bookmarksfly.cn

[Q27] 条件计数
来源：http://rn.jianghongdianzi.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://qe.shxzskj.cn

[Q28] 求和与平均
来源：http://ce.hahajie.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://at.wgjwhj.cn

[Q29] 最大最小值
来源：http://ts.muxihuayi.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://ng.huixiangedu.cn

[Q30] 分组统计
来源：http://ek.shtwfgs.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://vt.chemitech.net.cn

[Q31] 分组后过滤
来源：http://bs.muxihuayi.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://cb.hnjuh.cn

[Q32] 分组拼接字符串
来源：http://rv.gzmigu.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://fl.bjjhwx.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ih.gzmigu.cn

[Q33] 多列分组
来源：http://sq.muxihuayi.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://sh.shtwfgs.cn

[Q34] 每组取第一条
来源：http://si.nicolike.cn

SELECT * FROM (
来源：http://da.huixiangedu.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://py.szxytkj.cn

) t WHERE rn = 1;
来源：http://ri.newstarts.cn

[Q35] 内连接
来源：http://jo.521024.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://lr.szsharing.cn

[Q36] 左连接
来源：http://lu.hnjuh.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://jb.9csxet.cn

[Q37] 右连接
来源：http://kr.muxihuayi.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://gw.szxytkj.cn

[Q38] 全外连接（PostgreSQL）
来源：http://rn.shxzukj.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://rx.jianghongdianzi.cn

[Q39] 自连接（查上下级）
来源：http://lh.haigaiapp.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://jr.huixiangedu.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://jl.lnxyls.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://ue.jianghongdianzi.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://xi.huixinmuqiang.cn

[Q41] 多表连接
来源：http://mk.gzmigu.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://ha.gzmigu.cn

JOIN users u ON u.id = o.user_id
来源：http://bv.szsharing.cn

JOIN products p ON p.id = o.product_id;
来源：http://ts.lnxyls.cn

[Q42] 连接条件附加过滤
来源：http://kk.jianghongdianzi.cn

SELECT u.name, o.amount FROM users u
来源：http://cu.haigaiapp.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://we.hnjuh.cn

[Q43] 标量子查询
来源：http://hj.lnxyls.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://xf.newstarts.cn

[Q44] IN 子查询
来源：http://nc.shxzukj.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://zw.szxytkj.cn

[Q45] EXISTS 判断存在
来源：http://jo.wgjwhj.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://bh.shtwfgs.cn

[Q46] NOT EXISTS 判断不存在
来源：http://ud.shtwfgs.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://gp.wgjwhj.cn

[Q47] 与平均值比较
来源：http://nc.newstarts.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://re.shtwfgs.cn


<!-- 参考信息 -->