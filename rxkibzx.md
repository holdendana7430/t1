代发 wailian999

[N05] 最大公约数
来源：http://pw.9csxet.cn

Py:   math.gcd(a, b)
来源：http://tw.bookmarksfly.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://tc.shxzukj.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://vy.9csxet.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://kj.bjjhwx.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://qa.shtwfgs.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ci.haigaiapp.cn

Ruby: a.gcd(b)
来源：http://qi.muxihuayi.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mz.wgjwhj.cn

[N06] 判断回文字符串
来源：http://pm.huanxung.cn

Py:   s == s[::-1]
来源：http://gg.lnxyls.cn

PHP:  $s === strrev($s);
来源：http://jp.shxzukj.cn

JS:   s === [...s].reverse().join("")
来源：http://in.huixiangedu.cn

TS:   s === [...s].reverse().join("")
来源：http://or.panjiajie.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hi.shtwfgs.cn

Go:   // 双指针从两端比较
来源：http://ag.shxzukj.cn

Ruby: s == s.reverse
来源：http://ic.yuntaijiaju.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://pr.huixiangedu.cn

[N07] 两数之和（返回下标）
来源：http://nz.bookmarksfly.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://jo.gzmigu.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://zv.colortex.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://in.newstarts.cn

TS:   // 手写 Map<string, number>
来源：http://zn.panjiajie.cn

Java: // 手写 HashMap
来源：http://pk.panjiajie.cn

Go:   // 手写 map[int]int
来源：http://di.nszjky.cn

Ruby: // 手写 Hash
来源：http://pg.huixiangedu.cn

C#:   // 手写 Dictionary<int, int>
来源：http://jt.szsharing.cn

[N08] 生成全排列
来源：http://ck.wgjwhj.cn

Py:   itertools.permutations(arr)
来源：http://nd.shxzskj.cn

PHP:  // 手写递归交换
来源：http://ng.haigaiapp.cn

JS:   // 手写回溯递归
来源：http://rg.panjiajie.cn

TS:   // 手写回溯递归
来源：http://kk.szxytkj.cn

Java: // 手写回溯递归
来源：http://kg.huanxung.cn

Go:   // 手写回溯递归
来源：http://hj.huixiangedu.cn

Ruby: arr.permutation.to_a
来源：http://mw.nicolike.cn

C#:   // 手写回溯递归
来源：http://jd.szsharing.cn

[N09] 栈与队列
来源：http://bq.shxzukj.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wf.nicolike.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ac.shtwfgs.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://fh.szxytkj.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://he.shxzukj.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ph.szxytkj.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://yb.bjjhwx.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://nz.gzmigu.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://iq.9csxet.cn

[N10] 链表节点定义
来源：http://pv.9csxet.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://up.521024.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://us.yuexingan06.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://rd.521024.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://sq.shxzskj.cn

Java: class Node { int v; Node next; }
来源：http://zt.chemitech.net.cn

Go:   type Node struct { V int; Next *Node }
来源：http://cu.lnxyls.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://hl.nszjky.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://mp.szxytkj.cn

[N11] 二叉树中序遍历
来源：http://ut.lnxyls.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ir.jianghongdianzi.cn

PHP:  // 手写递归函数
来源：http://yd.chemitech.net.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://rm.haigaiapp.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ru.lnxyls.cn

Java: // 手写递归
来源：http://hi.shtwfgs.cn

Go:   // 手写递归
来源：http://nw.huanxung.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://pf.yuntaijiaju.cn

C#:   // 手写递归
来源：http://sx.gzmigu.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://xh.asd995.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ol.yuexingan06.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://kh.jctech888.com.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://nq.szsharing.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://iv.huixiangedu.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://fs.nicolike.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://lm.haigaiapp.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://tz.hnjuh.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://lb.huixiangedu.cn

================================================================================
来源：http://ik.huixinmuqiang.cn

O. 并发与异步
来源：http://ts.jianghongdianzi.cn

================================================================================
来源：http://vc.muxihuayi.cn

[O01] 启动一个线程
来源：http://eu.hahajie.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://qs.szxytkj.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://fn.521024.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://jp.nszjky.cn

TS:   // 同 JS
来源：http://xy.szxytkj.cn

Java: new Thread(() -> f()).start()
来源：http://jg.nszjky.cn

Go:   go f()
来源：http://ji.9csxet.cn

Ruby: Thread.new { f }
来源：http://rm.hnjuh.cn

C#:   Task.Run(() => F());
来源：http://lf.szxytkj.cn

[O02] 使用线程池
来源：http://mv.jianghongdianzi.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://pk.shxzukj.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ry.szsharing.cn

JS:   // worker_threads 线程池
来源：http://jm.newstarts.cn

TS:   // worker_threads 线程池
来源：http://rh.shxzukj.cn

Java: Executors.newFixedThreadPool(4)
来源：http://oc.yuntaijiaju.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ci.haigaiapp.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ny.yuntaijiaju.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://sh.521024.cn

[O03] 加锁保护共享数据
来源：http://pn.szxytkj.cn

Py:   with lock: shared += 1
来源：http://wa.lnxyls.cn

PHP:  // 用 flock() 做文件锁
来源：http://cm.shxzukj.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://gg.lnxyls.cn

TS:   // 同 JS
来源：http://rh.lnxyls.cn

Java: synchronized (this) { shared++; }
来源：http://lb.9csxet.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://xx.yuntaijiaju.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://kl.muxihuayi.cn

C#:   lock (gate) { shared++; }
来源：http://us.huixinmuqiang.cn

[O04] 定义异步函数并等待
来源：http://zr.jianghongdianzi.cn

Py:   async def f():⏎    await g()
来源：http://on.chemitech.net.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ck.nszjky.cn

JS:   async function f() { await g(); }
来源：http://ar.huixiangedu.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://il.panjiajie.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mh.shxzukj.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://rc.gzmigu.cn

Ruby: # 用 Fiber 或 async gem
来源：http://mn.jctech888.com.cn

C#:   async Task F() { await G(); }
来源：http://yg.nszjky.cn

[O05] 并发执行并等待全部完成
来源：http://gq.chemitech.net.cn

Py:   asyncio.gather(*tasks)
来源：http://pb.jianghongdianzi.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mz.panjiajie.cn

JS:   await Promise.all(tasks)
来源：http://hy.panjiajie.cn

TS:   await Promise.all(tasks)
来源：http://tx.shxzukj.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://rp.yuexingan06.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://qj.huixinmuqiang.cn

Ruby: threads.map(&:join)
来源：http://qs.bjjhwx.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://dq.szxytkj.cn

[O06] 使用进程池
来源：http://vs.huixinmuqiang.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ui.yuntaijiaju.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://tv.szsharing.cn

JS:   // child_process / cluster 模块
来源：http://of.huanxung.cn

TS:   // child_process / cluster 模块
来源：http://xr.nicolike.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://eo.hnjuh.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://er.hahajie.cn

Ruby: // fork 块
来源：http://bl.gzmigu.cn

C#:   Parallel.For
来源：http://ba.chemitech.net.cn

================================================================================
来源：http://xs.huixiangedu.cn

P. 常用工具函数
来源：http://cq.shxzukj.cn

================================================================================
来源：http://bn.bookmarksfly.cn

[P01] 生成 UUID
来源：http://ro.szxytkj.cn

Py:   str(uuid.uuid4())
来源：http://zz.huanxung.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://vf.muxihuayi.cn

JS:   crypto.randomUUID()
来源：http://wk.szsharing.cn

TS:   crypto.randomUUID()
来源：http://qx.muxihuayi.cn

Java: UUID.randomUUID().toString()
来源：http://yc.huixinmuqiang.cn

Go:   // 用 github.com/google/uuid
来源：http://at.yuexingan06.cn

Ruby: SecureRandom.uuid
来源：http://tz.lnxyls.cn

C#:   Guid.NewGuid().ToString()
来源：http://hh.hnjuh.cn

[P02] MD5 / SHA256 摘要
来源：http://zx.bjjhwx.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://po.chemitech.net.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://ul.jctech888.com.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://kl.wgjwhj.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://pk.jianghongdianzi.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ei.huanxung.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ic.shxzskj.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://rs.bookmarksfly.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://vp.lnxyls.cn

[P03] 生成短随机字符串
来源：http://ki.haigaiapp.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://qu.hnjuh.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://lo.lnxyls.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://fk.yuntaijiaju.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ay.shxzukj.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://bn.521024.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ow.shxzukj.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://nr.haigaiapp.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://rv.hnjuh.cn

[P04] 求长度
来源：http://pt.hahajie.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://fy.nicolike.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://lr.muxihuayi.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hc.gzmigu.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mu.yuexingan06.cn

Java: list.size();  map.size();  s.length()
来源：http://kv.huixinmuqiang.cn

Go:   len(arr);  len(m)
来源：http://ss.bjjhwx.cn

Ruby: x.length;  x.size
来源：http://wm.yuexingan06.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://cu.jianghongdianzi.cn

[P05] 判断两个对象内容是否相等
来源：http://yq.nszjky.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://hw.szsharing.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mi.haigaiapp.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ww.huixinmuqiang.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ig.szxytkj.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://so.colortex.cn

Go:   reflect.DeepEqual(a, b)
来源：http://gu.muxihuayi.cn

Ruby: a == b
来源：http://sb.colortex.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://et.panjiajie.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://bn.yuexingan06.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://sm.shxzukj.cn

PHP:  if (empty($x)) {}
来源：http://dl.asd995.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://xl.colortex.cn

TS:   if (x == null) {}
来源：http://ay.shxzskj.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://ct.huixinmuqiang.cn

Go:   if x == nil {}
来源：http://rt.szsharing.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://py.lnxyls.cn

C#:   if (x is null) {}
来源：http://za.huixiangedu.cn

[P07] 防抖与节流
来源：http://am.bjjhwx.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://rc.hnjuh.cn

PHP:  // 手写时间戳比较
来源：http://rb.asd995.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://of.lnxyls.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://jg.yuexingan06.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mm.haigaiapp.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://vz.chemitech.net.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://qz.huanxung.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://gp.chemitech.net.cn

[P08] 处理浮点精度问题
来源：http://zp.huixinmuqiang.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://gx.muxihuayi.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://vo.shxzskj.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wz.wgjwhj.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://eq.shxzukj.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://sw.asd995.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ib.szxytkj.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wq.nszjky.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://zk.jctech888.com.cn

================================================================================
来源：http://vh.colortex.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://yr.shxzukj.cn

================================================================================
来源：http://ik.bookmarksfly.cn

[Q01] 创建表
来源：http://fs.huanxung.cn

CREATE TABLE users (
来源：http://yd.jctech888.com.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://fg.szsharing.cn

name VARCHAR(50) NOT NULL,
来源：http://ok.wgjwhj.cn

email VARCHAR(100) UNIQUE,
来源：http://jw.hnjuh.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://uv.nszjky.cn

);
来源：http://ix.nszjky.cn

[Q02] 创建带外键的表
来源：http://qn.chemitech.net.cn

CREATE TABLE orders (
来源：http://nz.yuntaijiaju.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ov.shxzskj.cn

user_id INT NOT NULL,
来源：http://vz.nicolike.cn

amount DECIMAL(10, 2),
来源：http://xm.nicolike.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://no.jianghongdianzi.cn

);
来源：http://sk.chemitech.net.cn

[Q03] 增加列
来源：http://ri.chemitech.net.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://sw.yuexingan06.cn

[Q04] 修改列类型
来源：http://lh.bookmarksfly.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://yu.shxzskj.cn

[Q05] 重命名列
来源：http://xa.jctech888.com.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://fj.hahajie.cn

[Q06] 删除列
来源：http://qb.shxzskj.cn

ALTER TABLE users DROP COLUMN age;
来源：http://gp.bookmarksfly.cn

[Q07] 删除表
来源：http://hx.yuntaijiaju.cn

DROP TABLE IF EXISTS orders;
来源：http://re.gzmigu.cn

[Q08] 创建普通索引
来源：http://zp.chemitech.net.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://vz.9csxet.cn

[Q09] 创建唯一索引
来源：http://ye.newstarts.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://il.huixiangedu.cn

[Q10] 插入单行
来源：http://ya.colortex.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://zt.lnxyls.cn

[Q11] 一次插入多行
来源：http://mr.chemitech.net.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://vd.huixiangedu.cn

[Q12] 插入后取自增 ID
来源：http://jc.huixiangedu.cn

INSERT INTO users (name) VALUES ('C');
来源：http://yz.bjjhwx.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://in.wgjwhj.cn

[Q13] 忽略重复插入
来源：http://ou.nszjky.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.szsharing.cn

[Q14] 存在则更新（upsert）
来源：http://af.szsharing.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://tf.huixiangedu.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://lq.hnjuh.cn

[Q15] 查询全部
来源：http://xe.panjiajie.cn

SELECT * FROM users;
来源：http://kb.521024.cn

[Q16] 查询指定列
来源：http://jb.jctech888.com.cn

SELECT id, name FROM users;
来源：http://yq.colortex.cn

[Q17] 条件查询
来源：http://fp.colortex.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ko.huanxung.cn

[Q18] 模糊匹配
来源：http://ij.hahajie.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://bc.haigaiapp.cn

[Q19] 范围查询
来源：http://rc.yuntaijiaju.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://bf.szxytkj.cn

[Q20] IN 列表
来源：http://oa.muxihuayi.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://al.shtwfgs.cn

[Q21] 空值判断
来源：http://fu.9csxet.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://ox.huixiangedu.cn

[Q22] 排序
来源：http://yr.panjiajie.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://cg.hahajie.cn

[Q23] 分页
来源：http://xe.colortex.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://eo.nicolike.cn

[Q24] 去重
来源：http://hc.bjjhwx.cn

SELECT DISTINCT city FROM users;
来源：http://vx.bjjhwx.cn

[Q25] 只取前 N 条
来源：http://dm.521024.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://kt.shxzskj.cn

[Q26] 计数
来源：http://mv.hnjuh.cn

SELECT COUNT(*) FROM users;
来源：http://xf.chemitech.net.cn

[Q27] 条件计数
来源：http://nc.hnjuh.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ue.huanxung.cn

[Q28] 求和与平均
来源：http://ga.bookmarksfly.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://rt.szsharing.cn

[Q29] 最大最小值
来源：http://wq.panjiajie.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://do.hahajie.cn

[Q30] 分组统计
来源：http://te.yuexingan06.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hq.nicolike.cn

[Q31] 分组后过滤
来源：http://si.colortex.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://eg.colortex.cn

[Q32] 分组拼接字符串
来源：http://el.chemitech.net.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://xi.shxzskj.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://vq.chemitech.net.cn

[Q33] 多列分组
来源：http://kz.9csxet.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ux.nszjky.cn

[Q34] 每组取第一条
来源：http://ga.huixinmuqiang.cn

SELECT * FROM (
来源：http://yr.shxzukj.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://uj.shxzukj.cn

) t WHERE rn = 1;
来源：http://ss.bookmarksfly.cn

[Q35] 内连接
来源：http://wr.shxzukj.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ua.hnjuh.cn

[Q36] 左连接
来源：http://cd.hnjuh.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hw.bookmarksfly.cn

[Q37] 右连接
来源：http://oe.haigaiapp.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://dp.shtwfgs.cn

[Q38] 全外连接（PostgreSQL）
来源：http://rz.asd995.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://yd.lnxyls.cn

[Q39] 自连接（查上下级）
来源：http://ud.9csxet.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://zw.huanxung.cn


<!-- 参考信息 -->