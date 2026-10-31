代发 wailian999

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://df.haigaiapp.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://co.asd995.cn

TS:   // 手写 Map<string, number>
来源：http://jz.huixiangedu.cn

Java: // 手写 HashMap
来源：http://db.9csxet.cn

Go:   // 手写 map[int]int
来源：http://sj.newstarts.cn

Ruby: // 手写 Hash
来源：http://im.muxihuayi.cn

C#:   // 手写 Dictionary<int, int>
来源：http://jl.hnjuh.cn

[N08] 生成全排列
来源：http://ym.jctech888.com.cn

Py:   itertools.permutations(arr)
来源：http://fy.shtwfgs.cn

PHP:  // 手写递归交换
来源：http://ob.asd995.cn

JS:   // 手写回溯递归
来源：http://sy.jianghongdianzi.cn

TS:   // 手写回溯递归
来源：http://ft.szsharing.cn

Java: // 手写回溯递归
来源：http://wv.huixinmuqiang.cn

Go:   // 手写回溯递归
来源：http://fi.yuntaijiaju.cn

Ruby: arr.permutation.to_a
来源：http://pe.panjiajie.cn

C#:   // 手写回溯递归
来源：http://et.bjjhwx.cn

[N09] 栈与队列
来源：http://pr.9csxet.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://zk.colortex.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://al.haigaiapp.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://re.gzmigu.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://he.lnxyls.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://xd.newstarts.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://yt.shtwfgs.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://fl.haigaiapp.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://so.lnxyls.cn

[N10] 链表节点定义
来源：http://uv.lnxyls.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://uv.shtwfgs.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://rk.gzmigu.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://oy.521024.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://bj.hnjuh.cn

Java: class Node { int v; Node next; }
来源：http://kq.panjiajie.cn

Go:   type Node struct { V int; Next *Node }
来源：http://zv.szsharing.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://rk.wgjwhj.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://vy.shxzskj.cn

[N11] 二叉树中序遍历
来源：http://iu.asd995.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://bh.szsharing.cn

PHP:  // 手写递归函数
来源：http://lv.muxihuayi.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://gm.wgjwhj.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://rb.bjjhwx.cn

Java: // 手写递归
来源：http://in.huixinmuqiang.cn

Go:   // 手写递归
来源：http://ln.hahajie.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://jm.huanxung.cn

C#:   // 手写递归
来源：http://tt.haigaiapp.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://uu.yuntaijiaju.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://qk.chemitech.net.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hs.szxytkj.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://xy.szxytkj.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ew.yuexingan06.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mi.muxihuayi.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://dt.szxytkj.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://pn.521024.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://gk.jctech888.com.cn

================================================================================
来源：http://eo.szxytkj.cn

O. 并发与异步
来源：http://cb.huixinmuqiang.cn

================================================================================
来源：http://zu.colortex.cn

[O01] 启动一个线程
来源：http://td.chemitech.net.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://dq.yuntaijiaju.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://cd.shxzukj.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://gb.jctech888.com.cn

TS:   // 同 JS
来源：http://ty.colortex.cn

Java: new Thread(() -> f()).start()
来源：http://vm.huixiangedu.cn

Go:   go f()
来源：http://qd.shtwfgs.cn

Ruby: Thread.new { f }
来源：http://fk.jianghongdianzi.cn

C#:   Task.Run(() => F());
来源：http://fw.wgjwhj.cn

[O02] 使用线程池
来源：http://bb.colortex.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://lp.muxihuayi.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hl.yuexingan06.cn

JS:   // worker_threads 线程池
来源：http://eo.521024.cn

TS:   // worker_threads 线程池
来源：http://gx.bookmarksfly.cn

Java: Executors.newFixedThreadPool(4)
来源：http://ty.huanxung.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://sf.huanxung.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://si.yuexingan06.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://rx.hahajie.cn

[O03] 加锁保护共享数据
来源：http://sq.panjiajie.cn

Py:   with lock: shared += 1
来源：http://cb.wgjwhj.cn

PHP:  // 用 flock() 做文件锁
来源：http://ut.gzmigu.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://js.muxihuayi.cn

TS:   // 同 JS
来源：http://oy.nszjky.cn

Java: synchronized (this) { shared++; }
来源：http://gb.shxzskj.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://yf.yuexingan06.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://vo.huixiangedu.cn

C#:   lock (gate) { shared++; }
来源：http://ky.haigaiapp.cn

[O04] 定义异步函数并等待
来源：http://km.hnjuh.cn

Py:   async def f():⏎    await g()
来源：http://zo.szxytkj.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ls.bjjhwx.cn

JS:   async function f() { await g(); }
来源：http://ws.nszjky.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://ae.huixinmuqiang.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ge.szsharing.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ov.huixinmuqiang.cn

Ruby: # 用 Fiber 或 async gem
来源：http://vm.shxzskj.cn

C#:   async Task F() { await G(); }
来源：http://ix.nszjky.cn

[O05] 并发执行并等待全部完成
来源：http://jo.521024.cn

Py:   asyncio.gather(*tasks)
来源：http://vt.szxytkj.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ix.huanxung.cn

JS:   await Promise.all(tasks)
来源：http://gl.huanxung.cn

TS:   await Promise.all(tasks)
来源：http://cw.huixinmuqiang.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://yj.huixinmuqiang.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://lp.nicolike.cn

Ruby: threads.map(&:join)
来源：http://ui.nszjky.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://ey.hnjuh.cn

[O06] 使用进程池
来源：http://xp.9csxet.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ly.hahajie.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://lw.hahajie.cn

JS:   // child_process / cluster 模块
来源：http://xv.gzmigu.cn

TS:   // child_process / cluster 模块
来源：http://cw.huixinmuqiang.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://op.lnxyls.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://jj.wgjwhj.cn

Ruby: // fork 块
来源：http://ky.szxytkj.cn

C#:   Parallel.For
来源：http://uz.shxzskj.cn

================================================================================
来源：http://vy.asd995.cn

P. 常用工具函数
来源：http://yg.bookmarksfly.cn

================================================================================
来源：http://an.newstarts.cn

[P01] 生成 UUID
来源：http://me.huixinmuqiang.cn

Py:   str(uuid.uuid4())
来源：http://ul.huixinmuqiang.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wl.shxzskj.cn

JS:   crypto.randomUUID()
来源：http://mb.huixiangedu.cn

TS:   crypto.randomUUID()
来源：http://ya.hnjuh.cn

Java: UUID.randomUUID().toString()
来源：http://gr.muxihuayi.cn

Go:   // 用 github.com/google/uuid
来源：http://wg.colortex.cn

Ruby: SecureRandom.uuid
来源：http://zd.yuntaijiaju.cn

C#:   Guid.NewGuid().ToString()
来源：http://nf.newstarts.cn

[P02] MD5 / SHA256 摘要
来源：http://av.jctech888.com.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://jl.bookmarksfly.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://gc.jianghongdianzi.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ig.panjiajie.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://er.huixinmuqiang.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ui.bjjhwx.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ch.huanxung.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://rp.gzmigu.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://lt.lnxyls.cn

[P03] 生成短随机字符串
来源：http://wf.bjjhwx.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://he.asd995.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://cu.shtwfgs.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://tb.asd995.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://qr.panjiajie.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://uj.colortex.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://cb.shtwfgs.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://jb.muxihuayi.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://df.szxytkj.cn

[P04] 求长度
来源：http://bd.jianghongdianzi.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://db.yuexingan06.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ka.colortex.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ge.newstarts.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wr.muxihuayi.cn

Java: list.size();  map.size();  s.length()
来源：http://cr.shxzskj.cn

Go:   len(arr);  len(m)
来源：http://yh.shtwfgs.cn

Ruby: x.length;  x.size
来源：http://hh.shtwfgs.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://lr.asd995.cn

[P05] 判断两个对象内容是否相等
来源：http://ws.hahajie.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://dt.wgjwhj.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ks.bjjhwx.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ot.huanxung.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://nz.521024.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://da.asd995.cn

Go:   reflect.DeepEqual(a, b)
来源：http://sf.wgjwhj.cn

Ruby: a == b
来源：http://hk.colortex.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ac.lnxyls.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://bx.panjiajie.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://md.haigaiapp.cn

PHP:  if (empty($x)) {}
来源：http://ph.huixinmuqiang.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://qz.huixiangedu.cn

TS:   if (x == null) {}
来源：http://ml.9csxet.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://aq.szxytkj.cn

Go:   if x == nil {}
来源：http://jo.shxzskj.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://qw.szsharing.cn

C#:   if (x is null) {}
来源：http://ha.shxzukj.cn

[P07] 防抖与节流
来源：http://fs.shtwfgs.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://jo.wgjwhj.cn

PHP:  // 手写时间戳比较
来源：http://jz.hnjuh.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://pg.bjjhwx.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://zr.jctech888.com.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://fl.yuexingan06.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://az.bjjhwx.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://vn.huanxung.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://kz.yuexingan06.cn

[P08] 处理浮点精度问题
来源：http://lr.nszjky.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://uf.hahajie.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://pt.asd995.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://oj.bjjhwx.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ba.hnjuh.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://yj.szxytkj.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://zy.haigaiapp.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://yb.521024.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wr.lnxyls.cn

================================================================================
来源：http://xv.newstarts.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://oi.szxytkj.cn

================================================================================
来源：http://gl.wgjwhj.cn

[Q01] 创建表
来源：http://mg.newstarts.cn

CREATE TABLE users (
来源：http://uh.huanxung.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wr.bookmarksfly.cn

name VARCHAR(50) NOT NULL,
来源：http://vv.nszjky.cn

email VARCHAR(100) UNIQUE,
来源：http://jz.hahajie.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ux.shtwfgs.cn

);
来源：http://li.jianghongdianzi.cn

[Q02] 创建带外键的表
来源：http://ym.haigaiapp.cn

CREATE TABLE orders (
来源：http://au.szxytkj.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://oo.gzmigu.cn

user_id INT NOT NULL,
来源：http://mb.jianghongdianzi.cn

amount DECIMAL(10, 2),
来源：http://qw.jctech888.com.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://fn.nicolike.cn

);
来源：http://yi.yuexingan06.cn

[Q03] 增加列
来源：http://mj.jctech888.com.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://cj.chemitech.net.cn

[Q04] 修改列类型
来源：http://ts.yuexingan06.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hg.chemitech.net.cn

[Q05] 重命名列
来源：http://lu.newstarts.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://qm.haigaiapp.cn

[Q06] 删除列
来源：http://rq.huixinmuqiang.cn

ALTER TABLE users DROP COLUMN age;
来源：http://fl.huanxung.cn

[Q07] 删除表
来源：http://zq.szsharing.cn

DROP TABLE IF EXISTS orders;
来源：http://xr.9csxet.cn

[Q08] 创建普通索引
来源：http://fn.panjiajie.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://ru.hnjuh.cn

[Q09] 创建唯一索引
来源：http://mg.panjiajie.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://tl.panjiajie.cn

[Q10] 插入单行
来源：http://jx.shxzskj.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://qc.nicolike.cn

[Q11] 一次插入多行
来源：http://km.wgjwhj.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ms.panjiajie.cn

[Q12] 插入后取自增 ID
来源：http://ux.yuexingan06.cn

INSERT INTO users (name) VALUES ('C');
来源：http://fl.haigaiapp.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://cq.nicolike.cn

[Q13] 忽略重复插入
来源：http://pv.hahajie.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://yz.jctech888.com.cn

[Q14] 存在则更新（upsert）
来源：http://mg.szxytkj.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://on.lnxyls.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ah.shtwfgs.cn

[Q15] 查询全部
来源：http://wx.bjjhwx.cn

SELECT * FROM users;
来源：http://to.shxzukj.cn

[Q16] 查询指定列
来源：http://bg.newstarts.cn

SELECT id, name FROM users;
来源：http://ft.asd995.cn

[Q17] 条件查询
来源：http://oe.huixiangedu.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wd.szsharing.cn

[Q18] 模糊匹配
来源：http://nd.bjjhwx.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hw.huixinmuqiang.cn

[Q19] 范围查询
来源：http://wg.panjiajie.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://pw.shtwfgs.cn

[Q20] IN 列表
来源：http://uu.muxihuayi.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wc.huixinmuqiang.cn

[Q21] 空值判断
来源：http://po.hahajie.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://wv.lnxyls.cn

[Q22] 排序
来源：http://mu.nicolike.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://xp.wgjwhj.cn

[Q23] 分页
来源：http://hd.jianghongdianzi.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://gr.asd995.cn

[Q24] 去重
来源：http://ez.haigaiapp.cn

SELECT DISTINCT city FROM users;
来源：http://qo.huixiangedu.cn

[Q25] 只取前 N 条
来源：http://ol.shxzukj.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ym.jianghongdianzi.cn

[Q26] 计数
来源：http://rf.hnjuh.cn

SELECT COUNT(*) FROM users;
来源：http://to.shxzukj.cn

[Q27] 条件计数
来源：http://pk.nicolike.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://dn.yuntaijiaju.cn

[Q28] 求和与平均
来源：http://av.521024.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://cw.hnjuh.cn

[Q29] 最大最小值
来源：http://wb.521024.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://kx.bookmarksfly.cn

[Q30] 分组统计
来源：http://zd.huixinmuqiang.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://vw.bookmarksfly.cn

[Q31] 分组后过滤
来源：http://fn.wgjwhj.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://vk.szxytkj.cn

[Q32] 分组拼接字符串
来源：http://ao.muxihuayi.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://uv.shxzskj.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://kw.huanxung.cn

[Q33] 多列分组
来源：http://hb.szsharing.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://vq.bookmarksfly.cn

[Q34] 每组取第一条
来源：http://aj.huixinmuqiang.cn

SELECT * FROM (
来源：http://yp.newstarts.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ok.haigaiapp.cn

) t WHERE rn = 1;
来源：http://fz.shxzukj.cn

[Q35] 内连接
来源：http://ss.9csxet.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://xs.jianghongdianzi.cn

[Q36] 左连接
来源：http://ph.huixinmuqiang.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://lu.newstarts.cn

[Q37] 右连接
来源：http://qh.yuntaijiaju.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://nz.newstarts.cn

[Q38] 全外连接（PostgreSQL）
来源：http://lb.hahajie.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://dx.yuexingan06.cn

[Q39] 自连接（查上下级）
来源：http://ua.haigaiapp.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://ni.yuntaijiaju.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://df.chemitech.net.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://lk.huixinmuqiang.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://je.huixinmuqiang.cn

[Q41] 多表连接
来源：http://fj.jctech888.com.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://zk.huanxung.cn

JOIN users u ON u.id = o.user_id
来源：http://et.szxytkj.cn

JOIN products p ON p.id = o.product_id;
来源：http://do.muxihuayi.cn

[Q42] 连接条件附加过滤
来源：http://gd.haigaiapp.cn

SELECT u.name, o.amount FROM users u
来源：http://pe.nicolike.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://cp.yuntaijiaju.cn

[Q43] 标量子查询
来源：http://gr.shxzukj.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ms.haigaiapp.cn

[Q44] IN 子查询
来源：http://gz.nicolike.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hf.huanxung.cn

[Q45] EXISTS 判断存在
来源：http://yc.huixiangedu.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mb.newstarts.cn

[Q46] NOT EXISTS 判断不存在
来源：http://hf.haigaiapp.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://jc.yuexingan06.cn

[Q47] 与平均值比较
来源：http://qc.szsharing.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://qw.haigaiapp.cn


<!-- 参考信息 -->