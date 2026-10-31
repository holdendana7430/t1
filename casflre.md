代发 wailian999

Go:   // 手写 map[int]int
来源：http://bk.huixinmuqiang.cn

Ruby: // 手写 Hash
来源：http://od.wgjwhj.cn

C#:   // 手写 Dictionary<int, int>
来源：http://gp.9csxet.cn

[N08] 生成全排列
来源：http://xi.yuntaijiaju.cn

Py:   itertools.permutations(arr)
来源：http://gi.colortex.cn

PHP:  // 手写递归交换
来源：http://ql.yuexingan06.cn

JS:   // 手写回溯递归
来源：http://af.yuntaijiaju.cn

TS:   // 手写回溯递归
来源：http://np.newstarts.cn

Java: // 手写回溯递归
来源：http://bz.muxihuayi.cn

Go:   // 手写回溯递归
来源：http://hx.huanxung.cn

Ruby: arr.permutation.to_a
来源：http://ca.huanxung.cn

C#:   // 手写回溯递归
来源：http://ee.hnjuh.cn

[N09] 栈与队列
来源：http://jt.haigaiapp.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://py.shtwfgs.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://vm.newstarts.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ff.nicolike.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://xx.wgjwhj.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wa.nszjky.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wi.hnjuh.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ds.yuexingan06.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://kr.bjjhwx.cn

[N10] 链表节点定义
来源：http://lw.szsharing.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ta.muxihuayi.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://aa.shtwfgs.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://dh.jianghongdianzi.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mk.bookmarksfly.cn

Java: class Node { int v; Node next; }
来源：http://xf.lnxyls.cn

Go:   type Node struct { V int; Next *Node }
来源：http://zv.huixiangedu.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://px.chemitech.net.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://tc.szsharing.cn

[N11] 二叉树中序遍历
来源：http://yi.chemitech.net.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://rp.521024.cn

PHP:  // 手写递归函数
来源：http://ul.jctech888.com.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://tr.colortex.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://tp.shxzskj.cn

Java: // 手写递归
来源：http://su.jctech888.com.cn

Go:   // 手写递归
来源：http://on.huixinmuqiang.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://up.lnxyls.cn

C#:   // 手写递归
来源：http://ol.chemitech.net.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mt.bjjhwx.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ws.hnjuh.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://zj.shxzskj.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ws.huanxung.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ao.jianghongdianzi.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://vs.shxzukj.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ox.jctech888.com.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://oh.asd995.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wy.panjiajie.cn

================================================================================
来源：http://rq.shxzukj.cn

O. 并发与异步
来源：http://ez.shxzukj.cn

================================================================================
来源：http://rd.shtwfgs.cn

[O01] 启动一个线程
来源：http://sf.hnjuh.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mu.jctech888.com.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://he.huanxung.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://bl.yuntaijiaju.cn

TS:   // 同 JS
来源：http://iy.bookmarksfly.cn

Java: new Thread(() -> f()).start()
来源：http://fz.yuntaijiaju.cn

Go:   go f()
来源：http://sv.gzmigu.cn

Ruby: Thread.new { f }
来源：http://tm.9csxet.cn

C#:   Task.Run(() => F());
来源：http://ms.huixinmuqiang.cn

[O02] 使用线程池
来源：http://sr.nicolike.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://gm.521024.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://rp.shtwfgs.cn

JS:   // worker_threads 线程池
来源：http://fa.huixiangedu.cn

TS:   // worker_threads 线程池
来源：http://me.shxzukj.cn

Java: Executors.newFixedThreadPool(4)
来源：http://yo.lnxyls.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ok.yuntaijiaju.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hs.jctech888.com.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://qu.huanxung.cn

[O03] 加锁保护共享数据
来源：http://ch.9csxet.cn

Py:   with lock: shared += 1
来源：http://um.bjjhwx.cn

PHP:  // 用 flock() 做文件锁
来源：http://zv.huixinmuqiang.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://jc.lnxyls.cn

TS:   // 同 JS
来源：http://ss.shxzskj.cn

Java: synchronized (this) { shared++; }
来源：http://iw.haigaiapp.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://xs.shxzskj.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://pa.lnxyls.cn

C#:   lock (gate) { shared++; }
来源：http://xh.9csxet.cn

[O04] 定义异步函数并等待
来源：http://yz.jctech888.com.cn

Py:   async def f():⏎    await g()
来源：http://tx.huixinmuqiang.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wf.9csxet.cn

JS:   async function f() { await g(); }
来源：http://qk.jianghongdianzi.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://nj.nicolike.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://at.huanxung.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://qu.gzmigu.cn

Ruby: # 用 Fiber 或 async gem
来源：http://nq.wgjwhj.cn

C#:   async Task F() { await G(); }
来源：http://ov.gzmigu.cn

[O05] 并发执行并等待全部完成
来源：http://iq.lnxyls.cn

Py:   asyncio.gather(*tasks)
来源：http://do.chemitech.net.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://qg.jianghongdianzi.cn

JS:   await Promise.all(tasks)
来源：http://vc.huixiangedu.cn

TS:   await Promise.all(tasks)
来源：http://uq.asd995.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://zh.nicolike.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ty.bjjhwx.cn

Ruby: threads.map(&:join)
来源：http://zp.9csxet.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://es.bookmarksfly.cn

[O06] 使用进程池
来源：http://nq.szsharing.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://sy.yuexingan06.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://gw.szsharing.cn

JS:   // child_process / cluster 模块
来源：http://wq.bookmarksfly.cn

TS:   // child_process / cluster 模块
来源：http://po.asd995.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://tk.521024.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://kx.gzmigu.cn

Ruby: // fork 块
来源：http://kq.asd995.cn

C#:   Parallel.For
来源：http://en.chemitech.net.cn

================================================================================
来源：http://qi.shtwfgs.cn

P. 常用工具函数
来源：http://ee.shxzskj.cn

================================================================================
来源：http://up.panjiajie.cn

[P01] 生成 UUID
来源：http://sq.nszjky.cn

Py:   str(uuid.uuid4())
来源：http://kb.chemitech.net.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ke.wgjwhj.cn

JS:   crypto.randomUUID()
来源：http://mi.yuexingan06.cn

TS:   crypto.randomUUID()
来源：http://pp.521024.cn

Java: UUID.randomUUID().toString()
来源：http://zg.chemitech.net.cn

Go:   // 用 github.com/google/uuid
来源：http://bt.lnxyls.cn

Ruby: SecureRandom.uuid
来源：http://rt.wgjwhj.cn

C#:   Guid.NewGuid().ToString()
来源：http://tb.9csxet.cn

[P02] MD5 / SHA256 摘要
来源：http://rk.szxytkj.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://qs.szsharing.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://do.shxzskj.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wv.colortex.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://fi.521024.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://kp.bookmarksfly.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://dh.gzmigu.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://oq.shxzskj.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://sy.huanxung.cn

[P03] 生成短随机字符串
来源：http://vv.newstarts.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ho.newstarts.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://yp.9csxet.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ya.asd995.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ci.muxihuayi.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://sn.nszjky.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://xo.shtwfgs.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://tp.asd995.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ad.newstarts.cn

[P04] 求长度
来源：http://hp.bookmarksfly.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://qs.newstarts.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://al.nicolike.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://sw.nicolike.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://zi.521024.cn

Java: list.size();  map.size();  s.length()
来源：http://xg.szsharing.cn

Go:   len(arr);  len(m)
来源：http://le.521024.cn

Ruby: x.length;  x.size
来源：http://ld.huixinmuqiang.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://ua.shxzukj.cn

[P05] 判断两个对象内容是否相等
来源：http://ep.szsharing.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://wk.gzmigu.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://bn.huixiangedu.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://zz.chemitech.net.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://is.jctech888.com.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ef.huixiangedu.cn

Go:   reflect.DeepEqual(a, b)
来源：http://ed.yuntaijiaju.cn

Ruby: a == b
来源：http://qg.chemitech.net.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://cr.newstarts.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://iy.bookmarksfly.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://we.huixinmuqiang.cn

PHP:  if (empty($x)) {}
来源：http://ox.huixinmuqiang.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://fv.yuntaijiaju.cn

TS:   if (x == null) {}
来源：http://yw.hahajie.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://xd.bookmarksfly.cn

Go:   if x == nil {}
来源：http://yr.newstarts.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://tp.shxzukj.cn

C#:   if (x is null) {}
来源：http://xc.hahajie.cn

[P07] 防抖与节流
来源：http://xz.huixinmuqiang.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ny.szxytkj.cn

PHP:  // 手写时间戳比较
来源：http://hz.nszjky.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mh.huanxung.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mq.hahajie.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://dg.haigaiapp.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ix.szxytkj.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://ss.nicolike.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://bx.lnxyls.cn

[P08] 处理浮点精度问题
来源：http://kf.chemitech.net.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://gu.muxihuayi.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://vc.bjjhwx.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://qg.yuexingan06.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://xy.9csxet.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ed.yuntaijiaju.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://oh.szsharing.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://gr.shtwfgs.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://us.huanxung.cn

================================================================================
来源：http://fj.lnxyls.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://il.shxzskj.cn

================================================================================
来源：http://si.nicolike.cn

[Q01] 创建表
来源：http://si.nszjky.cn

CREATE TABLE users (
来源：http://to.asd995.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://im.szxytkj.cn

name VARCHAR(50) NOT NULL,
来源：http://uq.colortex.cn

email VARCHAR(100) UNIQUE,
来源：http://mf.jianghongdianzi.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://jl.newstarts.cn

);
来源：http://hc.muxihuayi.cn

[Q02] 创建带外键的表
来源：http://xb.lnxyls.cn

CREATE TABLE orders (
来源：http://un.panjiajie.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://vo.jctech888.com.cn

user_id INT NOT NULL,
来源：http://ct.gzmigu.cn

amount DECIMAL(10, 2),
来源：http://tv.newstarts.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://uf.bookmarksfly.cn

);
来源：http://md.wgjwhj.cn

[Q03] 增加列
来源：http://rc.newstarts.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://bu.nicolike.cn

[Q04] 修改列类型
来源：http://sl.jianghongdianzi.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://id.521024.cn

[Q05] 重命名列
来源：http://hc.haigaiapp.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mj.shxzskj.cn

[Q06] 删除列
来源：http://hn.nicolike.cn

ALTER TABLE users DROP COLUMN age;
来源：http://oi.yuexingan06.cn

[Q07] 删除表
来源：http://zd.szxytkj.cn

DROP TABLE IF EXISTS orders;
来源：http://qv.shxzukj.cn

[Q08] 创建普通索引
来源：http://ij.haigaiapp.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://hm.haigaiapp.cn

[Q09] 创建唯一索引
来源：http://gq.huanxung.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://xi.szxytkj.cn

[Q10] 插入单行
来源：http://sq.yuntaijiaju.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://rf.nicolike.cn

[Q11] 一次插入多行
来源：http://ni.yuntaijiaju.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://bd.huixinmuqiang.cn

[Q12] 插入后取自增 ID
来源：http://be.huixiangedu.cn

INSERT INTO users (name) VALUES ('C');
来源：http://rl.huixiangedu.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mp.asd995.cn

[Q13] 忽略重复插入
来源：http://xq.bjjhwx.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ac.shxzukj.cn

[Q14] 存在则更新（upsert）
来源：http://hs.asd995.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://dk.chemitech.net.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://zy.shtwfgs.cn

[Q15] 查询全部
来源：http://nn.panjiajie.cn

SELECT * FROM users;
来源：http://ls.nicolike.cn

[Q16] 查询指定列
来源：http://du.nicolike.cn

SELECT id, name FROM users;
来源：http://gx.yuexingan06.cn

[Q17] 条件查询
来源：http://ua.nszjky.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ep.huixinmuqiang.cn

[Q18] 模糊匹配
来源：http://hn.lnxyls.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://jl.huixiangedu.cn

[Q19] 范围查询
来源：http://xf.szxytkj.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://xx.jctech888.com.cn

[Q20] IN 列表
来源：http://sd.muxihuayi.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://rc.newstarts.cn

[Q21] 空值判断
来源：http://ho.muxihuayi.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://sd.9csxet.cn

[Q22] 排序
来源：http://gj.shxzskj.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://fw.bjjhwx.cn

[Q23] 分页
来源：http://vd.haigaiapp.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://do.haigaiapp.cn

[Q24] 去重
来源：http://uu.panjiajie.cn

SELECT DISTINCT city FROM users;
来源：http://ce.lnxyls.cn

[Q25] 只取前 N 条
来源：http://zz.szsharing.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://xe.jctech888.com.cn

[Q26] 计数
来源：http://jd.wgjwhj.cn

SELECT COUNT(*) FROM users;
来源：http://ym.newstarts.cn

[Q27] 条件计数
来源：http://rk.asd995.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://vg.bookmarksfly.cn

[Q28] 求和与平均
来源：http://xo.shtwfgs.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://dc.yuexingan06.cn

[Q29] 最大最小值
来源：http://ef.szxytkj.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://fk.shtwfgs.cn

[Q30] 分组统计
来源：http://di.hahajie.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://gv.lnxyls.cn

[Q31] 分组后过滤
来源：http://ts.nicolike.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://sy.521024.cn

[Q32] 分组拼接字符串
来源：http://zt.bookmarksfly.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ax.shtwfgs.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hc.szsharing.cn

[Q33] 多列分组
来源：http://uw.lnxyls.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://vq.szsharing.cn

[Q34] 每组取第一条
来源：http://kr.nicolike.cn

SELECT * FROM (
来源：http://cn.jianghongdianzi.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://du.szxytkj.cn

) t WHERE rn = 1;
来源：http://pk.shxzskj.cn

[Q35] 内连接
来源：http://ug.szxytkj.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mt.shxzukj.cn

[Q36] 左连接
来源：http://lg.nicolike.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://se.newstarts.cn

[Q37] 右连接
来源：http://dy.bookmarksfly.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ay.nicolike.cn

[Q38] 全外连接（PostgreSQL）
来源：http://mj.chemitech.net.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://qf.gzmigu.cn

[Q39] 自连接（查上下级）
来源：http://zs.yuexingan06.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://ac.521024.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://do.lnxyls.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://ko.hahajie.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://oz.huixinmuqiang.cn

[Q41] 多表连接
来源：http://lc.bjjhwx.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://uo.asd995.cn

JOIN users u ON u.id = o.user_id
来源：http://lf.haigaiapp.cn

JOIN products p ON p.id = o.product_id;
来源：http://qj.shtwfgs.cn

[Q42] 连接条件附加过滤
来源：http://tq.nicolike.cn

SELECT u.name, o.amount FROM users u
来源：http://cx.szxytkj.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ec.hahajie.cn

[Q43] 标量子查询
来源：http://bn.hahajie.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://vj.jctech888.com.cn

[Q44] IN 子查询
来源：http://gn.asd995.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://so.hahajie.cn

[Q45] EXISTS 判断存在
来源：http://uu.yuexingan06.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://gk.bjjhwx.cn

[Q46] NOT EXISTS 判断不存在
来源：http://bv.haigaiapp.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://nk.huixiangedu.cn

[Q47] 与平均值比较
来源：http://vg.nszjky.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://zo.hnjuh.cn

[Q48] CTE 公用表表达式
来源：http://ja.521024.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mu.szsharing.cn

SELECT * FROM t WHERE c > 5;
来源：http://iu.lnxyls.cn

[Q49] 更新单行
来源：http://ns.jctech888.com.cn


<!-- 参考信息 -->