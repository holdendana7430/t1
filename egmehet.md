代发 wailian999

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ae.jianghongdianzi.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://ka.gzmigu.cn

TS:   // 手写 Map<string, number>
来源：http://tn.jianghongdianzi.cn

Java: // 手写 HashMap
来源：http://qi.nicolike.cn

Go:   // 手写 map[int]int
来源：http://iy.newstarts.cn

Ruby: // 手写 Hash
来源：http://ko.huanxung.cn

C#:   // 手写 Dictionary<int, int>
来源：http://qk.hahajie.cn

[N08] 生成全排列
来源：http://db.huanxung.cn

Py:   itertools.permutations(arr)
来源：http://kg.nicolike.cn

PHP:  // 手写递归交换
来源：http://rv.chemitech.net.cn

JS:   // 手写回溯递归
来源：http://es.asd995.cn

TS:   // 手写回溯递归
来源：http://pj.asd995.cn

Java: // 手写回溯递归
来源：http://kh.yuexingan06.cn

Go:   // 手写回溯递归
来源：http://rh.hahajie.cn

Ruby: arr.permutation.to_a
来源：http://rs.bookmarksfly.cn

C#:   // 手写回溯递归
来源：http://yx.asd995.cn

[N09] 栈与队列
来源：http://zq.shtwfgs.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ge.nszjky.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://xl.bookmarksfly.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://aa.colortex.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ng.wgjwhj.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://iv.panjiajie.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://nz.colortex.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://pl.newstarts.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://pn.shtwfgs.cn

[N10] 链表节点定义
来源：http://yq.hahajie.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://nj.wgjwhj.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://qd.yuntaijiaju.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://nm.nicolike.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://vk.hnjuh.cn

Java: class Node { int v; Node next; }
来源：http://lv.521024.cn

Go:   type Node struct { V int; Next *Node }
来源：http://mh.szxytkj.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://tg.szsharing.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://ak.muxihuayi.cn

[N11] 二叉树中序遍历
来源：http://ey.hahajie.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ls.jctech888.com.cn

PHP:  // 手写递归函数
来源：http://oi.bjjhwx.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://tk.gzmigu.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mi.hahajie.cn

Java: // 手写递归
来源：http://yk.gzmigu.cn

Go:   // 手写递归
来源：http://de.nicolike.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://fi.shtwfgs.cn

C#:   // 手写递归
来源：http://gd.bookmarksfly.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://aj.bookmarksfly.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://pc.hahajie.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://sw.bjjhwx.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://dq.szxytkj.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://nb.nszjky.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://et.szsharing.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ls.gzmigu.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://sq.wgjwhj.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hk.lnxyls.cn

================================================================================
来源：http://dj.panjiajie.cn

O. 并发与异步
来源：http://fr.asd995.cn

================================================================================
来源：http://vr.huixiangedu.cn

[O01] 启动一个线程
来源：http://bq.colortex.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://en.nicolike.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://td.wgjwhj.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ks.jianghongdianzi.cn

TS:   // 同 JS
来源：http://ri.bjjhwx.cn

Java: new Thread(() -> f()).start()
来源：http://ch.shxzukj.cn

Go:   go f()
来源：http://hh.yuexingan06.cn

Ruby: Thread.new { f }
来源：http://fa.asd995.cn

C#:   Task.Run(() => F());
来源：http://rn.shxzskj.cn

[O02] 使用线程池
来源：http://zk.521024.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://fn.gzmigu.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://dw.bookmarksfly.cn

JS:   // worker_threads 线程池
来源：http://kd.wgjwhj.cn

TS:   // worker_threads 线程池
来源：http://ln.colortex.cn

Java: Executors.newFixedThreadPool(4)
来源：http://my.muxihuayi.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ua.yuntaijiaju.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://em.huanxung.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mq.bookmarksfly.cn

[O03] 加锁保护共享数据
来源：http://pd.hnjuh.cn

Py:   with lock: shared += 1
来源：http://cn.bjjhwx.cn

PHP:  // 用 flock() 做文件锁
来源：http://om.yuntaijiaju.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://lp.hnjuh.cn

TS:   // 同 JS
来源：http://xi.shxzskj.cn

Java: synchronized (this) { shared++; }
来源：http://av.shxzukj.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mq.panjiajie.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://ei.9csxet.cn

C#:   lock (gate) { shared++; }
来源：http://ct.newstarts.cn

[O04] 定义异步函数并等待
来源：http://su.huixiangedu.cn

Py:   async def f():⏎    await g()
来源：http://xs.newstarts.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://gh.9csxet.cn

JS:   async function f() { await g(); }
来源：http://bf.jianghongdianzi.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://vh.yuntaijiaju.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://bm.asd995.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://jx.szxytkj.cn

Ruby: # 用 Fiber 或 async gem
来源：http://rp.yuntaijiaju.cn

C#:   async Task F() { await G(); }
来源：http://ui.nicolike.cn

[O05] 并发执行并等待全部完成
来源：http://nz.hnjuh.cn

Py:   asyncio.gather(*tasks)
来源：http://gv.jctech888.com.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ns.lnxyls.cn

JS:   await Promise.all(tasks)
来源：http://zh.jianghongdianzi.cn

TS:   await Promise.all(tasks)
来源：http://sj.huixinmuqiang.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://iw.newstarts.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://if.haigaiapp.cn

Ruby: threads.map(&:join)
来源：http://wp.521024.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://fm.asd995.cn

[O06] 使用进程池
来源：http://xg.hnjuh.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://yj.wgjwhj.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://vt.bjjhwx.cn

JS:   // child_process / cluster 模块
来源：http://ls.panjiajie.cn

TS:   // child_process / cluster 模块
来源：http://bc.shxzukj.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://jt.521024.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ti.bjjhwx.cn

Ruby: // fork 块
来源：http://ey.chemitech.net.cn

C#:   Parallel.For
来源：http://qe.shtwfgs.cn

================================================================================
来源：http://ip.muxihuayi.cn

P. 常用工具函数
来源：http://ft.huixiangedu.cn

================================================================================
来源：http://tb.9csxet.cn

[P01] 生成 UUID
来源：http://ut.hnjuh.cn

Py:   str(uuid.uuid4())
来源：http://vv.521024.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://yi.nicolike.cn

JS:   crypto.randomUUID()
来源：http://uv.szxytkj.cn

TS:   crypto.randomUUID()
来源：http://rw.szsharing.cn

Java: UUID.randomUUID().toString()
来源：http://ir.nszjky.cn

Go:   // 用 github.com/google/uuid
来源：http://xc.bjjhwx.cn

Ruby: SecureRandom.uuid
来源：http://ur.lnxyls.cn

C#:   Guid.NewGuid().ToString()
来源：http://yk.gzmigu.cn

[P02] MD5 / SHA256 摘要
来源：http://fc.nicolike.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://nq.jctech888.com.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://ak.huixiangedu.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://uw.nicolike.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://nf.wgjwhj.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://de.bjjhwx.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://dr.gzmigu.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://lh.shxzukj.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ru.hnjuh.cn

[P03] 生成短随机字符串
来源：http://bb.bookmarksfly.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ea.hnjuh.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://qs.shxzukj.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hh.huixinmuqiang.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://lu.chemitech.net.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://be.shxzukj.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://bi.nszjky.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://sz.huixiangedu.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://jo.panjiajie.cn

[P04] 求长度
来源：http://va.haigaiapp.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://bv.asd995.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://kg.hnjuh.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://yh.yuexingan06.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hu.nszjky.cn

Java: list.size();  map.size();  s.length()
来源：http://ri.lnxyls.cn

Go:   len(arr);  len(m)
来源：http://qb.asd995.cn

Ruby: x.length;  x.size
来源：http://ye.asd995.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://ep.newstarts.cn

[P05] 判断两个对象内容是否相等
来源：http://fe.colortex.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://vq.chemitech.net.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://cr.wgjwhj.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ul.muxihuayi.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://bx.szsharing.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://he.newstarts.cn

Go:   reflect.DeepEqual(a, b)
来源：http://ui.shxzukj.cn

Ruby: a == b
来源：http://ni.shtwfgs.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://cc.huixinmuqiang.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hv.nicolike.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://vy.huixinmuqiang.cn

PHP:  if (empty($x)) {}
来源：http://kj.lnxyls.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mv.colortex.cn

TS:   if (x == null) {}
来源：http://sk.9csxet.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://gv.jianghongdianzi.cn

Go:   if x == nil {}
来源：http://mh.chemitech.net.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hx.lnxyls.cn

C#:   if (x is null) {}
来源：http://ed.bookmarksfly.cn

[P07] 防抖与节流
来源：http://et.huanxung.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://qw.colortex.cn

PHP:  // 手写时间戳比较
来源：http://vq.nszjky.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://it.szxytkj.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://as.chemitech.net.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://pt.chemitech.net.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://sp.muxihuayi.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://gv.9csxet.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://lx.szsharing.cn

[P08] 处理浮点精度问题
来源：http://ne.chemitech.net.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mn.chemitech.net.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://zw.wgjwhj.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://bo.asd995.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mc.chemitech.net.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://yc.shxzukj.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://gj.huixiangedu.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://xd.haigaiapp.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://sf.bookmarksfly.cn

================================================================================
来源：http://uk.jctech888.com.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://gu.gzmigu.cn

================================================================================
来源：http://nd.huixinmuqiang.cn

[Q01] 创建表
来源：http://bn.chemitech.net.cn

CREATE TABLE users (
来源：http://bn.asd995.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://cu.panjiajie.cn

name VARCHAR(50) NOT NULL,
来源：http://me.huanxung.cn

email VARCHAR(100) UNIQUE,
来源：http://hf.huixinmuqiang.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hx.nicolike.cn

);
来源：http://ik.szsharing.cn

[Q02] 创建带外键的表
来源：http://lh.panjiajie.cn

CREATE TABLE orders (
来源：http://rl.9csxet.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://dw.jianghongdianzi.cn

user_id INT NOT NULL,
来源：http://dx.newstarts.cn

amount DECIMAL(10, 2),
来源：http://yr.newstarts.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://jw.shtwfgs.cn

);
来源：http://sw.chemitech.net.cn

[Q03] 增加列
来源：http://zd.gzmigu.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ww.bjjhwx.cn

[Q04] 修改列类型
来源：http://wm.szxytkj.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://vs.newstarts.cn

[Q05] 重命名列
来源：http://ms.nszjky.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://qg.shxzskj.cn

[Q06] 删除列
来源：http://iu.huanxung.cn

ALTER TABLE users DROP COLUMN age;
来源：http://fk.lnxyls.cn

[Q07] 删除表
来源：http://su.jctech888.com.cn

DROP TABLE IF EXISTS orders;
来源：http://ot.hahajie.cn

[Q08] 创建普通索引
来源：http://po.521024.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://je.chemitech.net.cn

[Q09] 创建唯一索引
来源：http://td.521024.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ob.wgjwhj.cn

[Q10] 插入单行
来源：http://hn.szsharing.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://sk.szxytkj.cn

[Q11] 一次插入多行
来源：http://hk.shtwfgs.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://pc.huixiangedu.cn

[Q12] 插入后取自增 ID
来源：http://dk.panjiajie.cn

INSERT INTO users (name) VALUES ('C');
来源：http://hf.yuexingan06.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://dm.huixiangedu.cn

[Q13] 忽略重复插入
来源：http://ob.szxytkj.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://qq.bookmarksfly.cn

[Q14] 存在则更新（upsert）
来源：http://ev.chemitech.net.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://nh.yuntaijiaju.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ix.panjiajie.cn

[Q15] 查询全部
来源：http://wo.shxzskj.cn

SELECT * FROM users;
来源：http://np.lnxyls.cn

[Q16] 查询指定列
来源：http://vt.bjjhwx.cn

SELECT id, name FROM users;
来源：http://ys.panjiajie.cn

[Q17] 条件查询
来源：http://aq.huixiangedu.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://xy.szsharing.cn

[Q18] 模糊匹配
来源：http://fz.9csxet.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://tq.huanxung.cn

[Q19] 范围查询
来源：http://rr.wgjwhj.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://lo.asd995.cn

[Q20] IN 列表
来源：http://zs.newstarts.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ub.shxzskj.cn

[Q21] 空值判断
来源：http://yn.wgjwhj.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://ks.jianghongdianzi.cn

[Q22] 排序
来源：http://zy.panjiajie.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ng.bjjhwx.cn

[Q23] 分页
来源：http://nq.szxytkj.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://pi.nszjky.cn

[Q24] 去重
来源：http://bq.colortex.cn

SELECT DISTINCT city FROM users;
来源：http://rg.jctech888.com.cn

[Q25] 只取前 N 条
来源：http://ct.lnxyls.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ue.muxihuayi.cn

[Q26] 计数
来源：http://tg.nszjky.cn

SELECT COUNT(*) FROM users;
来源：http://ao.chemitech.net.cn

[Q27] 条件计数
来源：http://py.hnjuh.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://tn.yuntaijiaju.cn

[Q28] 求和与平均
来源：http://yj.9csxet.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://xd.newstarts.cn

[Q29] 最大最小值
来源：http://hb.colortex.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://sf.wgjwhj.cn

[Q30] 分组统计
来源：http://eb.jianghongdianzi.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://zm.521024.cn

[Q31] 分组后过滤
来源：http://zv.9csxet.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://og.panjiajie.cn

[Q32] 分组拼接字符串
来源：http://qk.bookmarksfly.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://jq.haigaiapp.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wz.nszjky.cn

[Q33] 多列分组
来源：http://zv.shxzukj.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://fl.hnjuh.cn

[Q34] 每组取第一条
来源：http://ax.hahajie.cn

SELECT * FROM (
来源：http://mv.huanxung.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://gf.colortex.cn

) t WHERE rn = 1;
来源：http://vt.muxihuayi.cn

[Q35] 内连接
来源：http://rl.lnxyls.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mx.yuntaijiaju.cn

[Q36] 左连接
来源：http://cd.lnxyls.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ad.jianghongdianzi.cn

[Q37] 右连接
来源：http://oy.muxihuayi.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://iu.yuexingan06.cn

[Q38] 全外连接（PostgreSQL）
来源：http://bc.huanxung.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://sq.bookmarksfly.cn

[Q39] 自连接（查上下级）
来源：http://aw.yuexingan06.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://gd.panjiajie.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://rg.haigaiapp.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://vy.szxytkj.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://yy.bookmarksfly.cn

[Q41] 多表连接
来源：http://cw.newstarts.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://cn.colortex.cn

JOIN users u ON u.id = o.user_id
来源：http://fk.nszjky.cn

JOIN products p ON p.id = o.product_id;
来源：http://cv.wgjwhj.cn

[Q42] 连接条件附加过滤
来源：http://yg.huixinmuqiang.cn

SELECT u.name, o.amount FROM users u
来源：http://tb.521024.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://nm.nicolike.cn

[Q43] 标量子查询
来源：http://xa.huanxung.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://kd.yuexingan06.cn

[Q44] IN 子查询
来源：http://vi.panjiajie.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://dl.huixinmuqiang.cn

[Q45] EXISTS 判断存在
来源：http://yf.bjjhwx.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wu.panjiajie.cn

[Q46] NOT EXISTS 判断不存在
来源：http://zi.9csxet.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ig.panjiajie.cn

[Q47] 与平均值比较
来源：http://mj.hahajie.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://xs.hnjuh.cn


<!-- 参考信息 -->