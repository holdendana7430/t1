代发 wailian999

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://xx.colortex.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://yf.shxzskj.cn

TS:   // 手写 Map<string, number>
来源：http://mn.nszjky.cn

Java: // 手写 HashMap
来源：http://ac.wgjwhj.cn

Go:   // 手写 map[int]int
来源：http://cw.huanxung.cn

Ruby: // 手写 Hash
来源：http://am.hahajie.cn

C#:   // 手写 Dictionary<int, int>
来源：http://ky.bookmarksfly.cn

[N08] 生成全排列
来源：http://pp.bjjhwx.cn

Py:   itertools.permutations(arr)
来源：http://iq.521024.cn

PHP:  // 手写递归交换
来源：http://ds.newstarts.cn

JS:   // 手写回溯递归
来源：http://io.521024.cn

TS:   // 手写回溯递归
来源：http://zc.yuntaijiaju.cn

Java: // 手写回溯递归
来源：http://iy.huixiangedu.cn

Go:   // 手写回溯递归
来源：http://kp.hahajie.cn

Ruby: arr.permutation.to_a
来源：http://tn.huixinmuqiang.cn

C#:   // 手写回溯递归
来源：http://ta.szxytkj.cn

[N09] 栈与队列
来源：http://am.521024.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://zt.wgjwhj.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://cm.huixinmuqiang.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://zn.huixinmuqiang.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hi.lnxyls.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://yz.nszjky.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://pv.panjiajie.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://cz.colortex.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://va.chemitech.net.cn

[N10] 链表节点定义
来源：http://bw.yuntaijiaju.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://tk.shtwfgs.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://fe.muxihuayi.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ru.lnxyls.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://du.huixinmuqiang.cn

Java: class Node { int v; Node next; }
来源：http://fw.bookmarksfly.cn

Go:   type Node struct { V int; Next *Node }
来源：http://nj.huixinmuqiang.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://et.wgjwhj.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://mg.yuntaijiaju.cn

[N11] 二叉树中序遍历
来源：http://gb.shxzukj.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://cw.szsharing.cn

PHP:  // 手写递归函数
来源：http://tl.gzmigu.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://gs.shxzskj.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://gd.colortex.cn

Java: // 手写递归
来源：http://ur.jctech888.com.cn

Go:   // 手写递归
来源：http://of.haigaiapp.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://re.lnxyls.cn

C#:   // 手写递归
来源：http://nd.huixiangedu.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://tr.yuntaijiaju.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://iu.huixiangedu.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://fm.shxzskj.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://xw.yuexingan06.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://fe.bookmarksfly.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://dk.colortex.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://gd.szsharing.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://my.jianghongdianzi.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://yv.nicolike.cn

================================================================================
来源：http://rm.yuntaijiaju.cn

O. 并发与异步
来源：http://ql.bookmarksfly.cn

================================================================================
来源：http://wc.bjjhwx.cn

[O01] 启动一个线程
来源：http://pa.yuntaijiaju.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://nm.9csxet.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://dg.nszjky.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://df.newstarts.cn

TS:   // 同 JS
来源：http://fe.szxytkj.cn

Java: new Thread(() -> f()).start()
来源：http://nn.yuexingan06.cn

Go:   go f()
来源：http://id.jctech888.com.cn

Ruby: Thread.new { f }
来源：http://zf.szxytkj.cn

C#:   Task.Run(() => F());
来源：http://nu.yuntaijiaju.cn

[O02] 使用线程池
来源：http://dn.panjiajie.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://lm.shxzukj.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://av.hahajie.cn

JS:   // worker_threads 线程池
来源：http://cx.yuntaijiaju.cn

TS:   // worker_threads 线程池
来源：http://nj.wgjwhj.cn

Java: Executors.newFixedThreadPool(4)
来源：http://ls.bjjhwx.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hq.hahajie.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mh.chemitech.net.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://dn.szxytkj.cn

[O03] 加锁保护共享数据
来源：http://hx.shtwfgs.cn

Py:   with lock: shared += 1
来源：http://kp.nszjky.cn

PHP:  // 用 flock() 做文件锁
来源：http://cg.hnjuh.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://nr.shxzukj.cn

TS:   // 同 JS
来源：http://fv.asd995.cn

Java: synchronized (this) { shared++; }
来源：http://mi.muxihuayi.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://gh.huixinmuqiang.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://ik.9csxet.cn

C#:   lock (gate) { shared++; }
来源：http://cx.gzmigu.cn

[O04] 定义异步函数并等待
来源：http://ge.chemitech.net.cn

Py:   async def f():⏎    await g()
来源：http://uu.hahajie.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ar.jctech888.com.cn

JS:   async function f() { await g(); }
来源：http://zd.521024.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.huixiangedu.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ct.nszjky.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hr.newstarts.cn

Ruby: # 用 Fiber 或 async gem
来源：http://bx.bjjhwx.cn

C#:   async Task F() { await G(); }
来源：http://nl.chemitech.net.cn

[O05] 并发执行并等待全部完成
来源：http://ja.9csxet.cn

Py:   asyncio.gather(*tasks)
来源：http://mm.bjjhwx.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://zl.newstarts.cn

JS:   await Promise.all(tasks)
来源：http://ig.muxihuayi.cn

TS:   await Promise.all(tasks)
来源：http://me.gzmigu.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://yf.chemitech.net.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://sj.newstarts.cn

Ruby: threads.map(&:join)
来源：http://cf.szsharing.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://bk.bjjhwx.cn

[O06] 使用进程池
来源：http://jo.shtwfgs.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://yc.szxytkj.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://sp.newstarts.cn

JS:   // child_process / cluster 模块
来源：http://nh.jctech888.com.cn

TS:   // child_process / cluster 模块
来源：http://kh.chemitech.net.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://rk.nszjky.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://aj.hnjuh.cn

Ruby: // fork 块
来源：http://ip.shtwfgs.cn

C#:   Parallel.For
来源：http://qh.asd995.cn

================================================================================
来源：http://bu.huixinmuqiang.cn

P. 常用工具函数
来源：http://un.chemitech.net.cn

================================================================================
来源：http://lp.shxzskj.cn

[P01] 生成 UUID
来源：http://cq.huixiangedu.cn

Py:   str(uuid.uuid4())
来源：http://ds.huixinmuqiang.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://gb.yuexingan06.cn

JS:   crypto.randomUUID()
来源：http://nh.bjjhwx.cn

TS:   crypto.randomUUID()
来源：http://sa.yuntaijiaju.cn

Java: UUID.randomUUID().toString()
来源：http://ov.jctech888.com.cn

Go:   // 用 github.com/google/uuid
来源：http://bs.jctech888.com.cn

Ruby: SecureRandom.uuid
来源：http://oq.panjiajie.cn

C#:   Guid.NewGuid().ToString()
来源：http://zy.jctech888.com.cn

[P02] MD5 / SHA256 摘要
来源：http://yk.shxzskj.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ce.nicolike.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://ol.bookmarksfly.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mu.szxytkj.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ot.jianghongdianzi.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ko.hahajie.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://vw.yuntaijiaju.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ny.bookmarksfly.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://te.jctech888.com.cn

[P03] 生成短随机字符串
来源：http://lj.bjjhwx.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://xr.bjjhwx.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://xg.newstarts.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://aq.szsharing.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://bh.shxzskj.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://fw.gzmigu.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ab.huixiangedu.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://ft.chemitech.net.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://uf.9csxet.cn

[P04] 求长度
来源：http://cg.lnxyls.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wg.colortex.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://uw.colortex.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ju.newstarts.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ch.bookmarksfly.cn

Java: list.size();  map.size();  s.length()
来源：http://fs.huixiangedu.cn

Go:   len(arr);  len(m)
来源：http://vg.lnxyls.cn

Ruby: x.length;  x.size
来源：http://tx.shxzskj.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://ui.muxihuayi.cn

[P05] 判断两个对象内容是否相等
来源：http://bl.gzmigu.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://br.yuexingan06.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://sw.szxytkj.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://jy.muxihuayi.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://bz.chemitech.net.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://bh.huixiangedu.cn

Go:   reflect.DeepEqual(a, b)
来源：http://qf.lnxyls.cn

Ruby: a == b
来源：http://ga.huanxung.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://qb.nszjky.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ka.yuexingan06.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://qf.hnjuh.cn

PHP:  if (empty($x)) {}
来源：http://vi.panjiajie.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wl.bjjhwx.cn

TS:   if (x == null) {}
来源：http://xs.lnxyls.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://fa.yuexingan06.cn

Go:   if x == nil {}
来源：http://ex.chemitech.net.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://xx.bookmarksfly.cn

C#:   if (x is null) {}
来源：http://rp.szsharing.cn

[P07] 防抖与节流
来源：http://bl.bookmarksfly.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://tk.shtwfgs.cn

PHP:  // 手写时间戳比较
来源：http://hb.szxytkj.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mu.bookmarksfly.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://dw.gzmigu.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ss.chemitech.net.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://dy.nszjky.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://in.bookmarksfly.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ul.wgjwhj.cn

[P08] 处理浮点精度问题
来源：http://cx.gzmigu.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://yy.colortex.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ei.shxzukj.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://bh.nicolike.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://pg.shxzukj.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://av.szxytkj.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ky.chemitech.net.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wn.wgjwhj.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://sk.huixiangedu.cn

================================================================================
来源：http://ur.nicolike.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hk.nicolike.cn

================================================================================
来源：http://is.colortex.cn

[Q01] 创建表
来源：http://po.asd995.cn

CREATE TABLE users (
来源：http://oo.yuntaijiaju.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wl.nszjky.cn

name VARCHAR(50) NOT NULL,
来源：http://ry.wgjwhj.cn

email VARCHAR(100) UNIQUE,
来源：http://dw.wgjwhj.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ls.nicolike.cn

);
来源：http://if.9csxet.cn

[Q02] 创建带外键的表
来源：http://co.szsharing.cn

CREATE TABLE orders (
来源：http://hn.asd995.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://im.asd995.cn

user_id INT NOT NULL,
来源：http://fj.chemitech.net.cn

amount DECIMAL(10, 2),
来源：http://eh.9csxet.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hg.bjjhwx.cn

);
来源：http://nh.colortex.cn

[Q03] 增加列
来源：http://hh.shtwfgs.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://tx.asd995.cn

[Q04] 修改列类型
来源：http://df.bookmarksfly.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mw.huixinmuqiang.cn

[Q05] 重命名列
来源：http://no.hahajie.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://lq.nicolike.cn

[Q06] 删除列
来源：http://rb.bjjhwx.cn

ALTER TABLE users DROP COLUMN age;
来源：http://qu.nszjky.cn

[Q07] 删除表
来源：http://sj.shxzukj.cn

DROP TABLE IF EXISTS orders;
来源：http://sl.shxzukj.cn

[Q08] 创建普通索引
来源：http://rk.panjiajie.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://qh.nicolike.cn

[Q09] 创建唯一索引
来源：http://ir.panjiajie.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://kv.yuntaijiaju.cn

[Q10] 插入单行
来源：http://vh.jctech888.com.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://pi.yuntaijiaju.cn

[Q11] 一次插入多行
来源：http://yb.9csxet.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://lo.hahajie.cn

[Q12] 插入后取自增 ID
来源：http://fn.9csxet.cn

INSERT INTO users (name) VALUES ('C');
来源：http://si.colortex.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://zb.bjjhwx.cn

[Q13] 忽略重复插入
来源：http://vd.colortex.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ky.bjjhwx.cn

[Q14] 存在则更新（upsert）
来源：http://ye.gzmigu.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ay.521024.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ur.asd995.cn

[Q15] 查询全部
来源：http://xl.jctech888.com.cn

SELECT * FROM users;
来源：http://vb.hahajie.cn

[Q16] 查询指定列
来源：http://ib.shxzskj.cn

SELECT id, name FROM users;
来源：http://zy.szsharing.cn

[Q17] 条件查询
来源：http://oq.szxytkj.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://dt.szxytkj.cn

[Q18] 模糊匹配
来源：http://gl.huanxung.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://fu.nicolike.cn

[Q19] 范围查询
来源：http://yi.yuexingan06.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://np.wgjwhj.cn

[Q20] IN 列表
来源：http://xi.9csxet.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://vv.huixiangedu.cn

[Q21] 空值判断
来源：http://vl.huixiangedu.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://xb.yuntaijiaju.cn

[Q22] 排序
来源：http://ed.hahajie.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://vy.gzmigu.cn

[Q23] 分页
来源：http://ge.nszjky.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://vm.jianghongdianzi.cn

[Q24] 去重
来源：http://gd.521024.cn

SELECT DISTINCT city FROM users;
来源：http://rl.hnjuh.cn

[Q25] 只取前 N 条
来源：http://lr.newstarts.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ar.newstarts.cn

[Q26] 计数
来源：http://ea.nszjky.cn

SELECT COUNT(*) FROM users;
来源：http://wl.panjiajie.cn

[Q27] 条件计数
来源：http://la.yuntaijiaju.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://tj.huixinmuqiang.cn

[Q28] 求和与平均
来源：http://os.9csxet.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://lw.asd995.cn

[Q29] 最大最小值
来源：http://kj.shxzukj.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://pe.colortex.cn

[Q30] 分组统计
来源：http://tw.nszjky.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://se.9csxet.cn

[Q31] 分组后过滤
来源：http://uo.lnxyls.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://md.colortex.cn

[Q32] 分组拼接字符串
来源：http://qt.shxzskj.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://xt.jianghongdianzi.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://dk.szxytkj.cn

[Q33] 多列分组
来源：http://ts.shxzukj.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://uu.yuexingan06.cn

[Q34] 每组取第一条
来源：http://vs.9csxet.cn

SELECT * FROM (
来源：http://mu.huanxung.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://xa.wgjwhj.cn

) t WHERE rn = 1;
来源：http://nq.bjjhwx.cn

[Q35] 内连接
来源：http://av.asd995.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://az.newstarts.cn

[Q36] 左连接
来源：http://sp.gzmigu.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://em.colortex.cn

[Q37] 右连接
来源：http://jb.huixinmuqiang.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ej.huixiangedu.cn

[Q38] 全外连接（PostgreSQL）
来源：http://wt.521024.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://fi.huixinmuqiang.cn

[Q39] 自连接（查上下级）
来源：http://xr.hahajie.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://hu.muxihuayi.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://kg.shtwfgs.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://si.shtwfgs.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://gj.shtwfgs.cn

[Q41] 多表连接
来源：http://wq.newstarts.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://gn.haigaiapp.cn

JOIN users u ON u.id = o.user_id
来源：http://av.hahajie.cn

JOIN products p ON p.id = o.product_id;
来源：http://ot.bjjhwx.cn

[Q42] 连接条件附加过滤
来源：http://cg.shtwfgs.cn

SELECT u.name, o.amount FROM users u
来源：http://xb.521024.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://jc.szxytkj.cn

[Q43] 标量子查询
来源：http://xn.huanxung.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://il.yuntaijiaju.cn

[Q44] IN 子查询
来源：http://cv.newstarts.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://pl.nicolike.cn

[Q45] EXISTS 判断存在
来源：http://bl.jianghongdianzi.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://gp.panjiajie.cn

[Q46] NOT EXISTS 判断不存在
来源：http://mw.newstarts.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://zw.chemitech.net.cn

[Q47] 与平均值比较
来源：http://vx.jianghongdianzi.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mj.wgjwhj.cn


<!-- 参考信息 -->