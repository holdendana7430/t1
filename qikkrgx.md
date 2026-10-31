代发 wailian999

Ruby: s == s.reverse
来源：http://gj.wgjwhj.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://sr.yuexingan06.cn

[N07] 两数之和（返回下标）
来源：http://iy.hahajie.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ex.asd995.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://dr.nszjky.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://xl.muxihuayi.cn

TS:   // 手写 Map<string, number>
来源：http://qm.yuntaijiaju.cn

Java: // 手写 HashMap
来源：http://xm.9csxet.cn

Go:   // 手写 map[int]int
来源：http://iz.9csxet.cn

Ruby: // 手写 Hash
来源：http://sp.haigaiapp.cn

C#:   // 手写 Dictionary<int, int>
来源：http://gd.colortex.cn

[N08] 生成全排列
来源：http://eg.521024.cn

Py:   itertools.permutations(arr)
来源：http://cz.muxihuayi.cn

PHP:  // 手写递归交换
来源：http://mn.lnxyls.cn

JS:   // 手写回溯递归
来源：http://dw.szsharing.cn

TS:   // 手写回溯递归
来源：http://ri.shtwfgs.cn

Java: // 手写回溯递归
来源：http://lt.gzmigu.cn

Go:   // 手写回溯递归
来源：http://dp.asd995.cn

Ruby: arr.permutation.to_a
来源：http://ug.yuntaijiaju.cn

C#:   // 手写回溯递归
来源：http://qd.9csxet.cn

[N09] 栈与队列
来源：http://hf.huanxung.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://fm.huixinmuqiang.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://zt.jianghongdianzi.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://vr.yuntaijiaju.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://pp.nszjky.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://xo.gzmigu.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://uh.9csxet.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://lo.521024.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ot.hahajie.cn

[N10] 链表节点定义
来源：http://qv.asd995.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://eq.jctech888.com.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://io.gzmigu.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://my.gzmigu.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://bs.nicolike.cn

Java: class Node { int v; Node next; }
来源：http://mn.hahajie.cn

Go:   type Node struct { V int; Next *Node }
来源：http://ll.bookmarksfly.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://ee.szxytkj.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://fx.wgjwhj.cn

[N11] 二叉树中序遍历
来源：http://gt.muxihuayi.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://vj.huanxung.cn

PHP:  // 手写递归函数
来源：http://ex.shtwfgs.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://id.asd995.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://vc.chemitech.net.cn

Java: // 手写递归
来源：http://pr.szxytkj.cn

Go:   // 手写递归
来源：http://ns.jianghongdianzi.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://jg.jianghongdianzi.cn

C#:   // 手写递归
来源：http://ex.shxzukj.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://fh.shtwfgs.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://sr.asd995.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://nu.muxihuayi.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mh.shxzukj.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://gn.jianghongdianzi.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://cu.lnxyls.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://te.yuntaijiaju.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://sv.shxzukj.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ua.lnxyls.cn

================================================================================
来源：http://nh.yuntaijiaju.cn

O. 并发与异步
来源：http://wd.gzmigu.cn

================================================================================
来源：http://ra.lnxyls.cn

[O01] 启动一个线程
来源：http://ch.jctech888.com.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://dg.yuexingan06.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ql.jianghongdianzi.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://io.huixiangedu.cn

TS:   // 同 JS
来源：http://di.newstarts.cn

Java: new Thread(() -> f()).start()
来源：http://gs.nicolike.cn

Go:   go f()
来源：http://pw.yuexingan06.cn

Ruby: Thread.new { f }
来源：http://gc.521024.cn

C#:   Task.Run(() => F());
来源：http://rq.gzmigu.cn

[O02] 使用线程池
来源：http://jq.newstarts.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ua.szsharing.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wk.newstarts.cn

JS:   // worker_threads 线程池
来源：http://ih.wgjwhj.cn

TS:   // worker_threads 线程池
来源：http://yw.bookmarksfly.cn

Java: Executors.newFixedThreadPool(4)
来源：http://dd.gzmigu.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://sx.haigaiapp.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://cc.panjiajie.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://nf.newstarts.cn

[O03] 加锁保护共享数据
来源：http://co.bookmarksfly.cn

Py:   with lock: shared += 1
来源：http://tq.wgjwhj.cn

PHP:  // 用 flock() 做文件锁
来源：http://it.szsharing.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://gi.muxihuayi.cn

TS:   // 同 JS
来源：http://qa.nszjky.cn

Java: synchronized (this) { shared++; }
来源：http://bu.newstarts.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://yt.shtwfgs.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://ub.haigaiapp.cn

C#:   lock (gate) { shared++; }
来源：http://ut.newstarts.cn

[O04] 定义异步函数并等待
来源：http://sy.nicolike.cn

Py:   async def f():⏎    await g()
来源：http://at.szsharing.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://zg.shtwfgs.cn

JS:   async function f() { await g(); }
来源：http://ul.haigaiapp.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://bv.szxytkj.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://il.yuexingan06.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://kt.gzmigu.cn

Ruby: # 用 Fiber 或 async gem
来源：http://eu.shtwfgs.cn

C#:   async Task F() { await G(); }
来源：http://bz.yuntaijiaju.cn

[O05] 并发执行并等待全部完成
来源：http://vc.bookmarksfly.cn

Py:   asyncio.gather(*tasks)
来源：http://uy.huixiangedu.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ly.muxihuayi.cn

JS:   await Promise.all(tasks)
来源：http://mb.yuntaijiaju.cn

TS:   await Promise.all(tasks)
来源：http://ld.jctech888.com.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://pj.nicolike.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://zf.yuexingan06.cn

Ruby: threads.map(&:join)
来源：http://qx.nicolike.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://cd.shxzukj.cn

[O06] 使用进程池
来源：http://ty.jianghongdianzi.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hr.huixinmuqiang.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://ye.bjjhwx.cn

JS:   // child_process / cluster 模块
来源：http://zf.huanxung.cn

TS:   // child_process / cluster 模块
来源：http://yq.haigaiapp.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://jf.huixinmuqiang.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://pf.wgjwhj.cn

Ruby: // fork 块
来源：http://hz.huixinmuqiang.cn

C#:   Parallel.For
来源：http://st.bookmarksfly.cn

================================================================================
来源：http://yz.521024.cn

P. 常用工具函数
来源：http://uf.bjjhwx.cn

================================================================================
来源：http://gv.newstarts.cn

[P01] 生成 UUID
来源：http://yu.huixiangedu.cn

Py:   str(uuid.uuid4())
来源：http://xq.asd995.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://bp.asd995.cn

JS:   crypto.randomUUID()
来源：http://gs.shxzskj.cn

TS:   crypto.randomUUID()
来源：http://mo.nicolike.cn

Java: UUID.randomUUID().toString()
来源：http://tj.szsharing.cn

Go:   // 用 github.com/google/uuid
来源：http://uq.jctech888.com.cn

Ruby: SecureRandom.uuid
来源：http://xn.521024.cn

C#:   Guid.NewGuid().ToString()
来源：http://zb.521024.cn

[P02] MD5 / SHA256 摘要
来源：http://qy.hahajie.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://sn.hahajie.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://zn.shtwfgs.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://az.bjjhwx.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://pd.shxzskj.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://dr.panjiajie.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://jn.hahajie.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://tu.hahajie.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ez.jianghongdianzi.cn

[P03] 生成短随机字符串
来源：http://ol.shxzskj.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mp.jctech888.com.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ag.hnjuh.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://xo.huixinmuqiang.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://yh.bookmarksfly.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://js.9csxet.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://us.shtwfgs.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://ww.colortex.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://jj.nszjky.cn

[P04] 求长度
来源：http://wy.chemitech.net.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://yt.haigaiapp.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://pd.shxzskj.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hj.haigaiapp.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://kp.huanxung.cn

Java: list.size();  map.size();  s.length()
来源：http://ie.colortex.cn

Go:   len(arr);  len(m)
来源：http://qm.colortex.cn

Ruby: x.length;  x.size
来源：http://wl.nszjky.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://ub.muxihuayi.cn

[P05] 判断两个对象内容是否相等
来源：http://dd.muxihuayi.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://wg.nszjky.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://si.nicolike.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://gm.newstarts.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://dg.yuexingan06.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://jd.haigaiapp.cn

Go:   reflect.DeepEqual(a, b)
来源：http://gm.yuntaijiaju.cn

Ruby: a == b
来源：http://nk.hnjuh.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://yp.jctech888.com.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ve.panjiajie.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://xn.shxzskj.cn

PHP:  if (empty($x)) {}
来源：http://pn.bookmarksfly.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://pp.bjjhwx.cn

TS:   if (x == null) {}
来源：http://ea.jctech888.com.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://ni.shxzukj.cn

Go:   if x == nil {}
来源：http://jg.huixinmuqiang.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://qr.yuntaijiaju.cn

C#:   if (x is null) {}
来源：http://uj.szxytkj.cn

[P07] 防抖与节流
来源：http://gr.muxihuayi.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ph.jianghongdianzi.cn

PHP:  // 手写时间戳比较
来源：http://mm.colortex.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://zr.nszjky.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://yl.newstarts.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wt.huixinmuqiang.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://gu.bookmarksfly.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://ya.shxzskj.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wg.huixiangedu.cn

[P08] 处理浮点精度问题
来源：http://rg.hnjuh.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://tc.newstarts.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://tq.asd995.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://dk.chemitech.net.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hx.bjjhwx.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mn.bookmarksfly.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hd.jianghongdianzi.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://vx.haigaiapp.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ww.bjjhwx.cn

================================================================================
来源：http://qy.bjjhwx.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://vn.bookmarksfly.cn

================================================================================
来源：http://sy.shxzukj.cn

[Q01] 创建表
来源：http://mh.jianghongdianzi.cn

CREATE TABLE users (
来源：http://wr.huixinmuqiang.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://zl.shxzskj.cn

name VARCHAR(50) NOT NULL,
来源：http://bf.muxihuayi.cn

email VARCHAR(100) UNIQUE,
来源：http://kq.panjiajie.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://jl.szxytkj.cn

);
来源：http://ro.chemitech.net.cn

[Q02] 创建带外键的表
来源：http://oq.huanxung.cn

CREATE TABLE orders (
来源：http://ky.newstarts.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ck.asd995.cn

user_id INT NOT NULL,
来源：http://qs.jctech888.com.cn

amount DECIMAL(10, 2),
来源：http://fh.huixiangedu.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://iw.shtwfgs.cn

);
来源：http://xn.wgjwhj.cn

[Q03] 增加列
来源：http://pk.szsharing.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mr.shxzukj.cn

[Q04] 修改列类型
来源：http://hz.huixiangedu.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mj.muxihuayi.cn

[Q05] 重命名列
来源：http://fe.colortex.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://zj.shxzukj.cn

[Q06] 删除列
来源：http://xk.wgjwhj.cn

ALTER TABLE users DROP COLUMN age;
来源：http://ft.shtwfgs.cn

[Q07] 删除表
来源：http://jd.szsharing.cn

DROP TABLE IF EXISTS orders;
来源：http://nt.nszjky.cn

[Q08] 创建普通索引
来源：http://xy.szxytkj.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://gd.chemitech.net.cn

[Q09] 创建唯一索引
来源：http://lq.huixinmuqiang.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://lw.panjiajie.cn

[Q10] 插入单行
来源：http://dm.bookmarksfly.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ek.asd995.cn

[Q11] 一次插入多行
来源：http://xw.huanxung.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://xy.colortex.cn

[Q12] 插入后取自增 ID
来源：http://vg.colortex.cn

INSERT INTO users (name) VALUES ('C');
来源：http://cg.muxihuayi.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ou.wgjwhj.cn

[Q13] 忽略重复插入
来源：http://yw.9csxet.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mr.bookmarksfly.cn

[Q14] 存在则更新（upsert）
来源：http://la.szxytkj.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ch.nszjky.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hs.wgjwhj.cn

[Q15] 查询全部
来源：http://kk.jianghongdianzi.cn

SELECT * FROM users;
来源：http://gn.hnjuh.cn

[Q16] 查询指定列
来源：http://sh.nszjky.cn

SELECT id, name FROM users;
来源：http://rj.yuntaijiaju.cn

[Q17] 条件查询
来源：http://wa.lnxyls.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://yj.yuntaijiaju.cn

[Q18] 模糊匹配
来源：http://lx.shtwfgs.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://jy.muxihuayi.cn

[Q19] 范围查询
来源：http://cr.hahajie.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.asd995.cn

[Q20] IN 列表
来源：http://sp.huanxung.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://xb.shtwfgs.cn

[Q21] 空值判断
来源：http://le.521024.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://vz.shxzukj.cn

[Q22] 排序
来源：http://tt.muxihuayi.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://sl.colortex.cn

[Q23] 分页
来源：http://hg.wgjwhj.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mm.szsharing.cn

[Q24] 去重
来源：http://ji.hahajie.cn

SELECT DISTINCT city FROM users;
来源：http://ff.panjiajie.cn

[Q25] 只取前 N 条
来源：http://xm.shxzukj.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://tr.shtwfgs.cn

[Q26] 计数
来源：http://lb.nszjky.cn

SELECT COUNT(*) FROM users;
来源：http://gn.muxihuayi.cn

[Q27] 条件计数
来源：http://yc.asd995.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ts.shtwfgs.cn

[Q28] 求和与平均
来源：http://zf.bjjhwx.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wj.521024.cn

[Q29] 最大最小值
来源：http://ws.huanxung.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://vj.yuntaijiaju.cn

[Q30] 分组统计
来源：http://sz.szsharing.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://lw.nicolike.cn

[Q31] 分组后过滤
来源：http://ri.newstarts.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://dd.huanxung.cn

[Q32] 分组拼接字符串
来源：http://xa.huixiangedu.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ve.shtwfgs.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://bh.shtwfgs.cn

[Q33] 多列分组
来源：http://tx.shxzskj.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://gr.huanxung.cn

[Q34] 每组取第一条
来源：http://cw.nszjky.cn

SELECT * FROM (
来源：http://fn.huanxung.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://yl.shxzskj.cn

) t WHERE rn = 1;
来源：http://hl.lnxyls.cn

[Q35] 内连接
来源：http://mr.shxzskj.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://js.bookmarksfly.cn

[Q36] 左连接
来源：http://du.muxihuayi.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://gs.muxihuayi.cn

[Q37] 右连接
来源：http://mk.szsharing.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://pp.huixiangedu.cn

[Q38] 全外连接（PostgreSQL）
来源：http://fy.yuexingan06.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://rx.chemitech.net.cn

[Q39] 自连接（查上下级）
来源：http://fk.yuntaijiaju.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://yg.nszjky.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hp.szsharing.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://al.chemitech.net.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ey.huixiangedu.cn

[Q41] 多表连接
来源：http://cg.newstarts.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://rk.jctech888.com.cn

JOIN users u ON u.id = o.user_id
来源：http://zu.szxytkj.cn

JOIN products p ON p.id = o.product_id;
来源：http://js.szsharing.cn

[Q42] 连接条件附加过滤
来源：http://av.haigaiapp.cn

SELECT u.name, o.amount FROM users u
来源：http://mw.shtwfgs.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ov.haigaiapp.cn

[Q43] 标量子查询
来源：http://nn.chemitech.net.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://rx.huanxung.cn

[Q44] IN 子查询
来源：http://uq.muxihuayi.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ms.huanxung.cn

[Q45] EXISTS 判断存在
来源：http://pi.jctech888.com.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://yy.huixinmuqiang.cn


<!-- 参考信息 -->