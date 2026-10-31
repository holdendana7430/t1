代发 wailian999

Ruby: s == s.reverse
来源：http://vd.gzmigu.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://lo.haigaiapp.cn

[N07] 两数之和（返回下标）
来源：http://hn.hahajie.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ag.huanxung.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://vz.szsharing.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://ve.yuntaijiaju.cn

TS:   // 手写 Map<string, number>
来源：http://qa.shtwfgs.cn

Java: // 手写 HashMap
来源：http://db.haigaiapp.cn

Go:   // 手写 map[int]int
来源：http://jt.huixiangedu.cn

Ruby: // 手写 Hash
来源：http://wc.hnjuh.cn

C#:   // 手写 Dictionary<int, int>
来源：http://zl.huixinmuqiang.cn

[N08] 生成全排列
来源：http://iv.huixinmuqiang.cn

Py:   itertools.permutations(arr)
来源：http://ce.yuntaijiaju.cn

PHP:  // 手写递归交换
来源：http://uv.9csxet.cn

JS:   // 手写回溯递归
来源：http://fl.shtwfgs.cn

TS:   // 手写回溯递归
来源：http://fo.jctech888.com.cn

Java: // 手写回溯递归
来源：http://af.panjiajie.cn

Go:   // 手写回溯递归
来源：http://jo.szxytkj.cn

Ruby: arr.permutation.to_a
来源：http://om.9csxet.cn

C#:   // 手写回溯递归
来源：http://gd.asd995.cn

[N09] 栈与队列
来源：http://nx.asd995.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://su.chemitech.net.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mt.huixinmuqiang.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://fc.shtwfgs.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://kk.muxihuayi.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ei.hnjuh.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ze.colortex.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://dv.bjjhwx.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://zh.yuntaijiaju.cn

[N10] 链表节点定义
来源：http://vv.szxytkj.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://re.colortex.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://gv.shtwfgs.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ou.jctech888.com.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://tv.bookmarksfly.cn

Java: class Node { int v; Node next; }
来源：http://nm.asd995.cn

Go:   type Node struct { V int; Next *Node }
来源：http://bj.szxytkj.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://ob.huixinmuqiang.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://ld.szxytkj.cn

[N11] 二叉树中序遍历
来源：http://om.shxzskj.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://vn.haigaiapp.cn

PHP:  // 手写递归函数
来源：http://po.jctech888.com.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://my.panjiajie.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://bl.gzmigu.cn

Java: // 手写递归
来源：http://ye.hahajie.cn

Go:   // 手写递归
来源：http://wm.haigaiapp.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://kv.bookmarksfly.cn

C#:   // 手写递归
来源：http://rm.chemitech.net.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://lo.huixiangedu.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wt.shxzskj.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://kh.wgjwhj.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ff.bookmarksfly.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://zm.jctech888.com.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ck.shtwfgs.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://iz.9csxet.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://nk.muxihuayi.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://lt.bjjhwx.cn

================================================================================
来源：http://sl.jctech888.com.cn

O. 并发与异步
来源：http://hy.asd995.cn

================================================================================
来源：http://xa.huixiangedu.cn

[O01] 启动一个线程
来源：http://ww.asd995.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://za.shtwfgs.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://qz.muxihuayi.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ab.haigaiapp.cn

TS:   // 同 JS
来源：http://au.hnjuh.cn

Java: new Thread(() -> f()).start()
来源：http://ei.panjiajie.cn

Go:   go f()
来源：http://hv.szxytkj.cn

Ruby: Thread.new { f }
来源：http://ko.shxzukj.cn

C#:   Task.Run(() => F());
来源：http://mn.hnjuh.cn

[O02] 使用线程池
来源：http://vb.bjjhwx.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://bq.wgjwhj.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ez.haigaiapp.cn

JS:   // worker_threads 线程池
来源：http://mt.hnjuh.cn

TS:   // worker_threads 线程池
来源：http://zs.muxihuayi.cn

Java: Executors.newFixedThreadPool(4)
来源：http://be.newstarts.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://sn.jctech888.com.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ky.521024.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hq.521024.cn

[O03] 加锁保护共享数据
来源：http://ep.yuexingan06.cn

Py:   with lock: shared += 1
来源：http://mf.yuexingan06.cn

PHP:  // 用 flock() 做文件锁
来源：http://tg.huixiangedu.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://zr.9csxet.cn

TS:   // 同 JS
来源：http://bx.gzmigu.cn

Java: synchronized (this) { shared++; }
来源：http://mm.colortex.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://lh.nicolike.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://ed.wgjwhj.cn

C#:   lock (gate) { shared++; }
来源：http://vq.shtwfgs.cn

[O04] 定义异步函数并等待
来源：http://vm.huanxung.cn

Py:   async def f():⏎    await g()
来源：http://bs.huanxung.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://en.yuntaijiaju.cn

JS:   async function f() { await g(); }
来源：http://ga.bookmarksfly.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://ey.huixinmuqiang.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://rq.asd995.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ay.szxytkj.cn

Ruby: # 用 Fiber 或 async gem
来源：http://vu.hnjuh.cn

C#:   async Task F() { await G(); }
来源：http://xa.panjiajie.cn

[O05] 并发执行并等待全部完成
来源：http://wf.gzmigu.cn

Py:   asyncio.gather(*tasks)
来源：http://wd.colortex.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ii.shxzskj.cn

JS:   await Promise.all(tasks)
来源：http://mu.hnjuh.cn

TS:   await Promise.all(tasks)
来源：http://op.chemitech.net.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ci.gzmigu.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://cy.huixinmuqiang.cn

Ruby: threads.map(&:join)
来源：http://dh.lnxyls.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://gq.bookmarksfly.cn

[O06] 使用进程池
来源：http://li.huixiangedu.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://su.newstarts.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://uq.nszjky.cn

JS:   // child_process / cluster 模块
来源：http://ux.hnjuh.cn

TS:   // child_process / cluster 模块
来源：http://vt.bjjhwx.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://dr.lnxyls.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://sr.hahajie.cn

Ruby: // fork 块
来源：http://kf.nszjky.cn

C#:   Parallel.For
来源：http://im.muxihuayi.cn

================================================================================
来源：http://ge.asd995.cn

P. 常用工具函数
来源：http://ba.huanxung.cn

================================================================================
来源：http://ej.panjiajie.cn

[P01] 生成 UUID
来源：http://sw.shxzskj.cn

Py:   str(uuid.uuid4())
来源：http://qr.yuntaijiaju.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ou.lnxyls.cn

JS:   crypto.randomUUID()
来源：http://yu.wgjwhj.cn

TS:   crypto.randomUUID()
来源：http://ou.chemitech.net.cn

Java: UUID.randomUUID().toString()
来源：http://fv.9csxet.cn

Go:   // 用 github.com/google/uuid
来源：http://lc.hnjuh.cn

Ruby: SecureRandom.uuid
来源：http://ea.shxzskj.cn

C#:   Guid.NewGuid().ToString()
来源：http://wx.huanxung.cn

[P02] MD5 / SHA256 摘要
来源：http://dr.nicolike.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://jx.yuntaijiaju.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://tr.nszjky.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ew.gzmigu.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ga.huanxung.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://qx.colortex.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://qj.muxihuayi.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wv.szsharing.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://pz.muxihuayi.cn

[P03] 生成短随机字符串
来源：http://le.nszjky.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://lz.shxzskj.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://yh.szxytkj.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://my.colortex.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://gp.521024.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://rz.wgjwhj.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ur.chemitech.net.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://gn.yuexingan06.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://xe.colortex.cn

[P04] 求长度
来源：http://tt.hahajie.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://rl.newstarts.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://cp.szxytkj.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://qh.gzmigu.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://xk.panjiajie.cn

Java: list.size();  map.size();  s.length()
来源：http://tu.gzmigu.cn

Go:   len(arr);  len(m)
来源：http://aj.yuntaijiaju.cn

Ruby: x.length;  x.size
来源：http://ha.huanxung.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://rs.bjjhwx.cn

[P05] 判断两个对象内容是否相等
来源：http://uu.colortex.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://td.nicolike.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://zw.muxihuayi.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://kp.yuexingan06.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://vt.szsharing.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://vt.shxzukj.cn

Go:   reflect.DeepEqual(a, b)
来源：http://eq.bjjhwx.cn

Ruby: a == b
来源：http://oz.panjiajie.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://gm.9csxet.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://jf.hahajie.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://km.nicolike.cn

PHP:  if (empty($x)) {}
来源：http://ye.huixiangedu.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://xe.huanxung.cn

TS:   if (x == null) {}
来源：http://xy.jianghongdianzi.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://ih.bjjhwx.cn

Go:   if x == nil {}
来源：http://dg.lnxyls.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://zw.yuntaijiaju.cn

C#:   if (x is null) {}
来源：http://nu.szsharing.cn

[P07] 防抖与节流
来源：http://wd.gzmigu.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://jv.shtwfgs.cn

PHP:  // 手写时间戳比较
来源：http://ob.haigaiapp.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ps.szxytkj.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://uv.bookmarksfly.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mj.asd995.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://qu.bookmarksfly.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://fb.yuexingan06.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://nq.szxytkj.cn

[P08] 处理浮点精度问题
来源：http://yh.jctech888.com.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://bo.haigaiapp.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://tu.521024.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://bf.nszjky.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://na.huixinmuqiang.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://po.colortex.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://xi.shtwfgs.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ez.panjiajie.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://gk.yuntaijiaju.cn

================================================================================
来源：http://lg.gzmigu.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ji.huixinmuqiang.cn

================================================================================
来源：http://pb.nszjky.cn

[Q01] 创建表
来源：http://kk.newstarts.cn

CREATE TABLE users (
来源：http://sl.haigaiapp.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://fu.muxihuayi.cn

name VARCHAR(50) NOT NULL,
来源：http://xm.muxihuayi.cn

email VARCHAR(100) UNIQUE,
来源：http://tt.huixinmuqiang.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ug.shxzskj.cn

);
来源：http://pl.nszjky.cn

[Q02] 创建带外键的表
来源：http://ff.bookmarksfly.cn

CREATE TABLE orders (
来源：http://lc.muxihuayi.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ki.shxzukj.cn

user_id INT NOT NULL,
来源：http://uk.shxzukj.cn

amount DECIMAL(10, 2),
来源：http://ir.muxihuayi.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://xk.asd995.cn

);
来源：http://fk.gzmigu.cn

[Q03] 增加列
来源：http://pp.muxihuayi.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://yb.nicolike.cn

[Q04] 修改列类型
来源：http://bp.hnjuh.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://cv.huixinmuqiang.cn

[Q05] 重命名列
来源：http://da.jctech888.com.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ul.muxihuayi.cn

[Q06] 删除列
来源：http://fq.szxytkj.cn

ALTER TABLE users DROP COLUMN age;
来源：http://my.szsharing.cn

[Q07] 删除表
来源：http://po.newstarts.cn

DROP TABLE IF EXISTS orders;
来源：http://cx.jctech888.com.cn

[Q08] 创建普通索引
来源：http://rh.nszjky.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://fe.chemitech.net.cn

[Q09] 创建唯一索引
来源：http://uj.chemitech.net.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ro.huanxung.cn

[Q10] 插入单行
来源：http://jy.colortex.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ph.nicolike.cn

[Q11] 一次插入多行
来源：http://bz.wgjwhj.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ad.shxzskj.cn

[Q12] 插入后取自增 ID
来源：http://tt.colortex.cn

INSERT INTO users (name) VALUES ('C');
来源：http://bn.chemitech.net.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://yd.huixinmuqiang.cn

[Q13] 忽略重复插入
来源：http://lj.asd995.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://qb.panjiajie.cn

[Q14] 存在则更新（upsert）
来源：http://ph.yuntaijiaju.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://zz.muxihuayi.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://rs.gzmigu.cn

[Q15] 查询全部
来源：http://mv.gzmigu.cn

SELECT * FROM users;
来源：http://if.asd995.cn

[Q16] 查询指定列
来源：http://lk.jctech888.com.cn

SELECT id, name FROM users;
来源：http://hz.panjiajie.cn

[Q17] 条件查询
来源：http://fh.colortex.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://er.shxzukj.cn

[Q18] 模糊匹配
来源：http://me.shtwfgs.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://we.chemitech.net.cn

[Q19] 范围查询
来源：http://qw.szxytkj.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ln.szxytkj.cn

[Q20] IN 列表
来源：http://cz.haigaiapp.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://od.asd995.cn

[Q21] 空值判断
来源：http://dy.nicolike.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://ri.hnjuh.cn

[Q22] 排序
来源：http://hc.szsharing.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://de.jctech888.com.cn

[Q23] 分页
来源：http://md.nicolike.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://zb.huixinmuqiang.cn

[Q24] 去重
来源：http://ho.shxzskj.cn

SELECT DISTINCT city FROM users;
来源：http://ft.bookmarksfly.cn

[Q25] 只取前 N 条
来源：http://nj.muxihuayi.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://tc.jctech888.com.cn

[Q26] 计数
来源：http://zk.9csxet.cn

SELECT COUNT(*) FROM users;
来源：http://px.yuexingan06.cn

[Q27] 条件计数
来源：http://iv.panjiajie.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://iu.muxihuayi.cn

[Q28] 求和与平均
来源：http://li.huanxung.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://rf.bjjhwx.cn

[Q29] 最大最小值
来源：http://qw.huixiangedu.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://jp.hnjuh.cn

[Q30] 分组统计
来源：http://hf.yuexingan06.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://pe.muxihuayi.cn

[Q31] 分组后过滤
来源：http://ov.yuexingan06.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://vz.gzmigu.cn

[Q32] 分组拼接字符串
来源：http://oc.muxihuayi.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mj.szsharing.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hv.bjjhwx.cn

[Q33] 多列分组
来源：http://wy.bookmarksfly.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://cd.yuntaijiaju.cn

[Q34] 每组取第一条
来源：http://cm.szxytkj.cn

SELECT * FROM (
来源：http://to.chemitech.net.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ny.newstarts.cn

) t WHERE rn = 1;
来源：http://ua.lnxyls.cn

[Q35] 内连接
来源：http://gu.hahajie.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ag.muxihuayi.cn

[Q36] 左连接
来源：http://bc.521024.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://vl.hnjuh.cn

[Q37] 右连接
来源：http://ok.shxzskj.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://nk.hnjuh.cn

[Q38] 全外连接（PostgreSQL）
来源：http://ov.jianghongdianzi.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ws.chemitech.net.cn

[Q39] 自连接（查上下级）
来源：http://pa.nicolike.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://bv.newstarts.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://yk.newstarts.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://nd.panjiajie.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://uw.nicolike.cn

[Q41] 多表连接
来源：http://dz.jianghongdianzi.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://hm.colortex.cn

JOIN users u ON u.id = o.user_id
来源：http://tm.shxzskj.cn

JOIN products p ON p.id = o.product_id;
来源：http://so.wgjwhj.cn

[Q42] 连接条件附加过滤
来源：http://af.nszjky.cn

SELECT u.name, o.amount FROM users u
来源：http://ke.gzmigu.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://id.bjjhwx.cn

[Q43] 标量子查询
来源：http://bn.muxihuayi.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://xl.haigaiapp.cn

[Q44] IN 子查询
来源：http://ib.gzmigu.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mw.gzmigu.cn

[Q45] EXISTS 判断存在
来源：http://qk.chemitech.net.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ms.huixinmuqiang.cn


<!-- 参考信息 -->