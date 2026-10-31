代发 wailian999

Go:   // 手写 map[int]int
来源：http://fq.bookmarksfly.cn

Ruby: // 手写 Hash
来源：http://so.521024.cn

C#:   // 手写 Dictionary<int, int>
来源：http://ol.muxihuayi.cn

[N08] 生成全排列
来源：http://xm.shtwfgs.cn

Py:   itertools.permutations(arr)
来源：http://fw.lnxyls.cn

PHP:  // 手写递归交换
来源：http://vr.yuexingan06.cn

JS:   // 手写回溯递归
来源：http://ij.chemitech.net.cn

TS:   // 手写回溯递归
来源：http://vn.chemitech.net.cn

Java: // 手写回溯递归
来源：http://do.lnxyls.cn

Go:   // 手写回溯递归
来源：http://fc.lnxyls.cn

Ruby: arr.permutation.to_a
来源：http://nr.szxytkj.cn

C#:   // 手写回溯递归
来源：http://hk.jianghongdianzi.cn

[N09] 栈与队列
来源：http://xr.colortex.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://dq.huanxung.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://qa.muxihuayi.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ic.wgjwhj.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mh.huixinmuqiang.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://rk.huixiangedu.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://kg.yuntaijiaju.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://zz.bookmarksfly.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://cm.shxzskj.cn

[N10] 链表节点定义
来源：http://kg.nszjky.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://od.asd995.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://fg.jctech888.com.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://gm.hnjuh.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ng.szsharing.cn

Java: class Node { int v; Node next; }
来源：http://vq.huixinmuqiang.cn

Go:   type Node struct { V int; Next *Node }
来源：http://cu.newstarts.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://av.shtwfgs.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://vb.shtwfgs.cn

[N11] 二叉树中序遍历
来源：http://qb.hahajie.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ng.shtwfgs.cn

PHP:  // 手写递归函数
来源：http://sr.shtwfgs.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://vw.haigaiapp.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://fd.panjiajie.cn

Java: // 手写递归
来源：http://zt.chemitech.net.cn

Go:   // 手写递归
来源：http://gq.521024.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ol.huixinmuqiang.cn

C#:   // 手写递归
来源：http://hd.chemitech.net.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hh.yuntaijiaju.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://se.jctech888.com.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://st.521024.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wn.shtwfgs.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://nv.hahajie.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://nc.9csxet.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://bv.jctech888.com.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ps.huixiangedu.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ur.yuexingan06.cn

================================================================================
来源：http://xj.chemitech.net.cn

O. 并发与异步
来源：http://ie.bjjhwx.cn

================================================================================
来源：http://rp.haigaiapp.cn

[O01] 启动一个线程
来源：http://kj.chemitech.net.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://rm.shxzskj.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ba.panjiajie.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ce.huixinmuqiang.cn

TS:   // 同 JS
来源：http://ox.bjjhwx.cn

Java: new Thread(() -> f()).start()
来源：http://xt.521024.cn

Go:   go f()
来源：http://bo.bjjhwx.cn

Ruby: Thread.new { f }
来源：http://ul.lnxyls.cn

C#:   Task.Run(() => F());
来源：http://ca.shxzukj.cn

[O02] 使用线程池
来源：http://wb.szsharing.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://oz.yuntaijiaju.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://oh.bjjhwx.cn

JS:   // worker_threads 线程池
来源：http://me.nicolike.cn

TS:   // worker_threads 线程池
来源：http://nq.nszjky.cn

Java: Executors.newFixedThreadPool(4)
来源：http://ys.lnxyls.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://yw.colortex.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ph.521024.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://bg.gzmigu.cn

[O03] 加锁保护共享数据
来源：http://rw.521024.cn

Py:   with lock: shared += 1
来源：http://vc.chemitech.net.cn

PHP:  // 用 flock() 做文件锁
来源：http://zo.9csxet.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://re.lnxyls.cn

TS:   // 同 JS
来源：http://bg.shtwfgs.cn

Java: synchronized (this) { shared++; }
来源：http://yv.nszjky.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://cc.haigaiapp.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://bz.huanxung.cn

C#:   lock (gate) { shared++; }
来源：http://hu.colortex.cn

[O04] 定义异步函数并等待
来源：http://km.chemitech.net.cn

Py:   async def f():⏎    await g()
来源：http://tq.shtwfgs.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ch.lnxyls.cn

JS:   async function f() { await g(); }
来源：http://lx.szxytkj.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://eh.newstarts.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://xy.panjiajie.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://jn.hahajie.cn

Ruby: # 用 Fiber 或 async gem
来源：http://rh.wgjwhj.cn

C#:   async Task F() { await G(); }
来源：http://zw.nszjky.cn

[O05] 并发执行并等待全部完成
来源：http://ld.shxzskj.cn

Py:   asyncio.gather(*tasks)
来源：http://zf.panjiajie.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://yv.newstarts.cn

JS:   await Promise.all(tasks)
来源：http://kp.nszjky.cn

TS:   await Promise.all(tasks)
来源：http://uy.szxytkj.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://gu.nszjky.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://qg.yuexingan06.cn

Ruby: threads.map(&:join)
来源：http://ow.chemitech.net.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://fh.nicolike.cn

[O06] 使用进程池
来源：http://cm.huixiangedu.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wc.lnxyls.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://pi.hahajie.cn

JS:   // child_process / cluster 模块
来源：http://iw.yuexingan06.cn

TS:   // child_process / cluster 模块
来源：http://ah.szsharing.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ja.huanxung.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ca.jctech888.com.cn

Ruby: // fork 块
来源：http://xj.gzmigu.cn

C#:   Parallel.For
来源：http://qs.521024.cn

================================================================================
来源：http://nw.colortex.cn

P. 常用工具函数
来源：http://ge.yuexingan06.cn

================================================================================
来源：http://ng.shxzukj.cn

[P01] 生成 UUID
来源：http://zf.yuexingan06.cn

Py:   str(uuid.uuid4())
来源：http://jt.nicolike.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://rg.jctech888.com.cn

JS:   crypto.randomUUID()
来源：http://rw.newstarts.cn

TS:   crypto.randomUUID()
来源：http://up.jianghongdianzi.cn

Java: UUID.randomUUID().toString()
来源：http://hj.521024.cn

Go:   // 用 github.com/google/uuid
来源：http://jb.huixinmuqiang.cn

Ruby: SecureRandom.uuid
来源：http://zt.haigaiapp.cn

C#:   Guid.NewGuid().ToString()
来源：http://rv.szsharing.cn

[P02] MD5 / SHA256 摘要
来源：http://ep.yuexingan06.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://fx.yuexingan06.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://eh.jctech888.com.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://sf.bjjhwx.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://yw.nicolike.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ci.huixinmuqiang.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://fv.yuntaijiaju.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://bw.bjjhwx.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://cb.wgjwhj.cn

[P03] 生成短随机字符串
来源：http://vb.lnxyls.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://kw.huixinmuqiang.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://it.shxzukj.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://qt.huixinmuqiang.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://fv.asd995.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://rt.hahajie.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://qg.bookmarksfly.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://jf.szxytkj.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://jn.newstarts.cn

[P04] 求长度
来源：http://bi.huanxung.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://qo.bookmarksfly.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://et.haigaiapp.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://de.hahajie.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://rc.nszjky.cn

Java: list.size();  map.size();  s.length()
来源：http://ba.huixinmuqiang.cn

Go:   len(arr);  len(m)
来源：http://bn.521024.cn

Ruby: x.length;  x.size
来源：http://pg.muxihuayi.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://fy.wgjwhj.cn

[P05] 判断两个对象内容是否相等
来源：http://vd.hnjuh.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://lq.yuntaijiaju.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://cp.9csxet.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://un.haigaiapp.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://oz.szxytkj.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://sg.yuexingan06.cn

Go:   reflect.DeepEqual(a, b)
来源：http://lq.huixiangedu.cn

Ruby: a == b
来源：http://ni.yuexingan06.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://fs.bookmarksfly.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://sn.bookmarksfly.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://zo.521024.cn

PHP:  if (empty($x)) {}
来源：http://jx.szsharing.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://up.chemitech.net.cn

TS:   if (x == null) {}
来源：http://bh.521024.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://xw.521024.cn

Go:   if x == nil {}
来源：http://xd.asd995.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://dx.nszjky.cn

C#:   if (x is null) {}
来源：http://xb.asd995.cn

[P07] 防抖与节流
来源：http://gy.szxytkj.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://qe.9csxet.cn

PHP:  // 手写时间戳比较
来源：http://yp.haigaiapp.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://yz.nszjky.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://nf.hnjuh.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://xw.bookmarksfly.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ja.huixinmuqiang.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://zx.chemitech.net.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://kj.huixinmuqiang.cn

[P08] 处理浮点精度问题
来源：http://vl.asd995.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ty.nicolike.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ot.wgjwhj.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://qc.521024.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ei.chemitech.net.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://vu.asd995.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://vl.9csxet.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://xy.yuexingan06.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://uj.huixiangedu.cn

================================================================================
来源：http://dx.huixiangedu.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://rm.jctech888.com.cn

================================================================================
来源：http://bd.9csxet.cn

[Q01] 创建表
来源：http://zq.lnxyls.cn

CREATE TABLE users (
来源：http://yu.bjjhwx.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://zo.bjjhwx.cn

name VARCHAR(50) NOT NULL,
来源：http://xj.nszjky.cn

email VARCHAR(100) UNIQUE,
来源：http://bh.hahajie.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://or.bookmarksfly.cn

);
来源：http://vv.lnxyls.cn

[Q02] 创建带外键的表
来源：http://rd.panjiajie.cn

CREATE TABLE orders (
来源：http://pm.shtwfgs.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://jg.hnjuh.cn

user_id INT NOT NULL,
来源：http://lw.muxihuayi.cn

amount DECIMAL(10, 2),
来源：http://pv.gzmigu.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://md.shxzukj.cn

);
来源：http://jm.jctech888.com.cn

[Q03] 增加列
来源：http://rf.huixiangedu.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ts.chemitech.net.cn

[Q04] 修改列类型
来源：http://ib.colortex.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://tn.shxzukj.cn

[Q05] 重命名列
来源：http://vn.shxzskj.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://pw.huixiangedu.cn

[Q06] 删除列
来源：http://tb.asd995.cn

ALTER TABLE users DROP COLUMN age;
来源：http://dh.panjiajie.cn

[Q07] 删除表
来源：http://ao.huixinmuqiang.cn

DROP TABLE IF EXISTS orders;
来源：http://is.haigaiapp.cn

[Q08] 创建普通索引
来源：http://yy.bjjhwx.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://ip.shtwfgs.cn

[Q09] 创建唯一索引
来源：http://om.9csxet.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://tc.wgjwhj.cn

[Q10] 插入单行
来源：http://pn.colortex.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://kv.jctech888.com.cn

[Q11] 一次插入多行
来源：http://xp.bookmarksfly.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://qn.hnjuh.cn

[Q12] 插入后取自增 ID
来源：http://md.jianghongdianzi.cn

INSERT INTO users (name) VALUES ('C');
来源：http://zt.huixinmuqiang.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://kg.521024.cn

[Q13] 忽略重复插入
来源：http://ap.jctech888.com.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wm.hnjuh.cn

[Q14] 存在则更新（upsert）
来源：http://cr.shxzukj.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://vc.521024.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://bm.jianghongdianzi.cn

[Q15] 查询全部
来源：http://ot.yuexingan06.cn

SELECT * FROM users;
来源：http://jm.muxihuayi.cn

[Q16] 查询指定列
来源：http://ng.yuntaijiaju.cn

SELECT id, name FROM users;
来源：http://wv.jctech888.com.cn

[Q17] 条件查询
来源：http://dv.9csxet.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mq.shtwfgs.cn

[Q18] 模糊匹配
来源：http://dd.shxzukj.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://yl.szxytkj.cn

[Q19] 范围查询
来源：http://nc.lnxyls.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://sg.hahajie.cn

[Q20] IN 列表
来源：http://hz.huixinmuqiang.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://rb.panjiajie.cn

[Q21] 空值判断
来源：http://sy.newstarts.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://nq.yuexingan06.cn

[Q22] 排序
来源：http://ds.newstarts.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://zd.shxzskj.cn

[Q23] 分页
来源：http://uc.shtwfgs.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ax.shxzskj.cn

[Q24] 去重
来源：http://de.huixinmuqiang.cn

SELECT DISTINCT city FROM users;
来源：http://vd.shxzskj.cn

[Q25] 只取前 N 条
来源：http://iq.shtwfgs.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://qe.lnxyls.cn

[Q26] 计数
来源：http://rl.shtwfgs.cn

SELECT COUNT(*) FROM users;
来源：http://jv.shtwfgs.cn

[Q27] 条件计数
来源：http://dt.bjjhwx.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://qa.jianghongdianzi.cn

[Q28] 求和与平均
来源：http://cd.colortex.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://li.chemitech.net.cn

[Q29] 最大最小值
来源：http://pe.newstarts.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://oy.shtwfgs.cn

[Q30] 分组统计
来源：http://cy.haigaiapp.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://pa.bookmarksfly.cn

[Q31] 分组后过滤
来源：http://xh.newstarts.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://sy.gzmigu.cn

[Q32] 分组拼接字符串
来源：http://wb.jianghongdianzi.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wl.shxzskj.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://xw.szsharing.cn

[Q33] 多列分组
来源：http://em.bjjhwx.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://bk.huanxung.cn

[Q34] 每组取第一条
来源：http://rn.gzmigu.cn

SELECT * FROM (
来源：http://tm.bookmarksfly.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://sj.huixiangedu.cn

) t WHERE rn = 1;
来源：http://oq.huixiangedu.cn

[Q35] 内连接
来源：http://oz.521024.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://bt.521024.cn

[Q36] 左连接
来源：http://kv.nicolike.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ys.haigaiapp.cn

[Q37] 右连接
来源：http://mx.jctech888.com.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://gs.szsharing.cn

[Q38] 全外连接（PostgreSQL）
来源：http://ra.shxzskj.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ef.asd995.cn

[Q39] 自连接（查上下级）
来源：http://yq.huanxung.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://qo.haigaiapp.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://pe.hnjuh.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://je.gzmigu.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://rg.jianghongdianzi.cn

[Q41] 多表连接
来源：http://zs.panjiajie.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://hw.panjiajie.cn

JOIN users u ON u.id = o.user_id
来源：http://pq.wgjwhj.cn

JOIN products p ON p.id = o.product_id;
来源：http://ga.nszjky.cn

[Q42] 连接条件附加过滤
来源：http://cm.9csxet.cn

SELECT u.name, o.amount FROM users u
来源：http://wv.yuexingan06.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://rl.haigaiapp.cn

[Q43] 标量子查询
来源：http://qr.panjiajie.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://nq.chemitech.net.cn

[Q44] IN 子查询
来源：http://bh.nicolike.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://jn.hnjuh.cn

[Q45] EXISTS 判断存在
来源：http://os.huixiangedu.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ca.hnjuh.cn

[Q46] NOT EXISTS 判断不存在
来源：http://wb.newstarts.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://aw.huanxung.cn

[Q47] 与平均值比较
来源：http://rw.nicolike.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://fa.huixinmuqiang.cn

[Q48] CTE 公用表表达式
来源：http://gr.panjiajie.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ga.newstarts.cn

SELECT * FROM t WHERE c > 5;
来源：http://kb.9csxet.cn

[Q49] 更新单行
来源：http://xw.bookmarksfly.cn


<!-- 参考信息 -->