代发 wailian999

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://bx.shxzskj.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://lq.hahajie.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://op.panjiajie.cn

Ruby: a.gcd(b)
来源：http://yb.hnjuh.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://if.newstarts.cn

[N06] 判断回文字符串
来源：http://uz.nszjky.cn

Py:   s == s[::-1]
来源：http://xk.szxytkj.cn

PHP:  $s === strrev($s);
来源：http://kg.asd995.cn

JS:   s === [...s].reverse().join("")
来源：http://vi.haigaiapp.cn

TS:   s === [...s].reverse().join("")
来源：http://zp.asd995.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://nh.jianghongdianzi.cn

Go:   // 双指针从两端比较
来源：http://iz.nicolike.cn

Ruby: s == s.reverse
来源：http://qz.wgjwhj.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://zd.panjiajie.cn

[N07] 两数之和（返回下标）
来源：http://un.shtwfgs.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://qu.asd995.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wh.nszjky.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://xo.yuntaijiaju.cn

TS:   // 手写 Map<string, number>
来源：http://fd.9csxet.cn

Java: // 手写 HashMap
来源：http://es.gzmigu.cn

Go:   // 手写 map[int]int
来源：http://cw.shxzskj.cn

Ruby: // 手写 Hash
来源：http://hg.wgjwhj.cn

C#:   // 手写 Dictionary<int, int>
来源：http://zs.huixiangedu.cn

[N08] 生成全排列
来源：http://md.lnxyls.cn

Py:   itertools.permutations(arr)
来源：http://jc.nicolike.cn

PHP:  // 手写递归交换
来源：http://ng.asd995.cn

JS:   // 手写回溯递归
来源：http://fz.9csxet.cn

TS:   // 手写回溯递归
来源：http://hp.colortex.cn

Java: // 手写回溯递归
来源：http://px.colortex.cn

Go:   // 手写回溯递归
来源：http://ec.nszjky.cn

Ruby: arr.permutation.to_a
来源：http://vr.haigaiapp.cn

C#:   // 手写回溯递归
来源：http://cr.shxzskj.cn

[N09] 栈与队列
来源：http://qt.shxzskj.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://kx.huanxung.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://dk.hahajie.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ug.jctech888.com.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ze.yuexingan06.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://yn.shtwfgs.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://pm.huanxung.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://rg.9csxet.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://qr.muxihuayi.cn

[N10] 链表节点定义
来源：http://gc.lnxyls.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ff.bookmarksfly.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://jv.yuexingan06.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://yb.newstarts.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://gc.yuntaijiaju.cn

Java: class Node { int v; Node next; }
来源：http://xo.nicolike.cn

Go:   type Node struct { V int; Next *Node }
来源：http://mj.jianghongdianzi.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://ci.521024.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://is.colortex.cn

[N11] 二叉树中序遍历
来源：http://kw.bjjhwx.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://rf.huixiangedu.cn

PHP:  // 手写递归函数
来源：http://dt.wgjwhj.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://pd.hnjuh.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://uq.hahajie.cn

Java: // 手写递归
来源：http://tn.gzmigu.cn

Go:   // 手写递归
来源：http://ng.yuexingan06.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://qu.huanxung.cn

C#:   // 手写递归
来源：http://gj.hnjuh.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ez.bookmarksfly.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://df.shxzukj.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://rx.huanxung.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://rg.newstarts.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://gg.nicolike.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://rc.newstarts.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mg.asd995.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://xl.nicolike.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://pw.lnxyls.cn

================================================================================
来源：http://hw.jianghongdianzi.cn

O. 并发与异步
来源：http://pc.panjiajie.cn

================================================================================
来源：http://fi.colortex.cn

[O01] 启动一个线程
来源：http://yw.9csxet.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://oa.lnxyls.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://es.521024.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hp.wgjwhj.cn

TS:   // 同 JS
来源：http://dx.gzmigu.cn

Java: new Thread(() -> f()).start()
来源：http://nx.shxzskj.cn

Go:   go f()
来源：http://cg.shxzukj.cn

Ruby: Thread.new { f }
来源：http://fc.shxzskj.cn

C#:   Task.Run(() => F());
来源：http://ot.muxihuayi.cn

[O02] 使用线程池
来源：http://xm.huanxung.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://dv.jianghongdianzi.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://na.wgjwhj.cn

JS:   // worker_threads 线程池
来源：http://qs.nicolike.cn

TS:   // worker_threads 线程池
来源：http://qc.yuntaijiaju.cn

Java: Executors.newFixedThreadPool(4)
来源：http://vm.haigaiapp.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://xr.gzmigu.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://nt.shtwfgs.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://um.huanxung.cn

[O03] 加锁保护共享数据
来源：http://ag.panjiajie.cn

Py:   with lock: shared += 1
来源：http://jh.huixinmuqiang.cn

PHP:  // 用 flock() 做文件锁
来源：http://jr.newstarts.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://aw.asd995.cn

TS:   // 同 JS
来源：http://cy.yuexingan06.cn

Java: synchronized (this) { shared++; }
来源：http://we.chemitech.net.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ck.panjiajie.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://sw.szxytkj.cn

C#:   lock (gate) { shared++; }
来源：http://ye.jianghongdianzi.cn

[O04] 定义异步函数并等待
来源：http://qi.jianghongdianzi.cn

Py:   async def f():⏎    await g()
来源：http://dt.colortex.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://kt.muxihuayi.cn

JS:   async function f() { await g(); }
来源：http://bf.asd995.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://tk.hnjuh.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://qu.szsharing.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://nf.jctech888.com.cn

Ruby: # 用 Fiber 或 async gem
来源：http://pu.huixiangedu.cn

C#:   async Task F() { await G(); }
来源：http://yg.huanxung.cn

[O05] 并发执行并等待全部完成
来源：http://mz.huixinmuqiang.cn

Py:   asyncio.gather(*tasks)
来源：http://au.gzmigu.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://sg.yuntaijiaju.cn

JS:   await Promise.all(tasks)
来源：http://zy.huixinmuqiang.cn

TS:   await Promise.all(tasks)
来源：http://nz.bjjhwx.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://sn.nicolike.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wc.521024.cn

Ruby: threads.map(&:join)
来源：http://ji.asd995.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://ah.shxzukj.cn

[O06] 使用进程池
来源：http://ec.bjjhwx.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://lk.shxzskj.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://vm.nszjky.cn

JS:   // child_process / cluster 模块
来源：http://tl.huixinmuqiang.cn

TS:   // child_process / cluster 模块
来源：http://zr.shtwfgs.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://gh.9csxet.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://jj.chemitech.net.cn

Ruby: // fork 块
来源：http://ze.jctech888.com.cn

C#:   Parallel.For
来源：http://xs.nszjky.cn

================================================================================
来源：http://fh.muxihuayi.cn

P. 常用工具函数
来源：http://bo.wgjwhj.cn

================================================================================
来源：http://nr.muxihuayi.cn

[P01] 生成 UUID
来源：http://sb.shtwfgs.cn

Py:   str(uuid.uuid4())
来源：http://yy.bjjhwx.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ve.szxytkj.cn

JS:   crypto.randomUUID()
来源：http://ks.muxihuayi.cn

TS:   crypto.randomUUID()
来源：http://pw.shtwfgs.cn

Java: UUID.randomUUID().toString()
来源：http://eb.panjiajie.cn

Go:   // 用 github.com/google/uuid
来源：http://sd.yuntaijiaju.cn

Ruby: SecureRandom.uuid
来源：http://zc.lnxyls.cn

C#:   Guid.NewGuid().ToString()
来源：http://ap.szsharing.cn

[P02] MD5 / SHA256 摘要
来源：http://sr.shxzskj.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://gu.newstarts.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://ex.521024.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://dt.nszjky.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://fw.yuntaijiaju.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://dz.chemitech.net.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://dk.wgjwhj.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hh.lnxyls.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://dd.lnxyls.cn

[P03] 生成短随机字符串
来源：http://df.asd995.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://kp.chemitech.net.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://as.wgjwhj.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wz.huixinmuqiang.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ps.shxzskj.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://zf.huanxung.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://at.shxzukj.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://hn.wgjwhj.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://la.nicolike.cn

[P04] 求长度
来源：http://jh.lnxyls.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://tr.shxzukj.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://rf.huanxung.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hm.hahajie.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://bc.shxzskj.cn

Java: list.size();  map.size();  s.length()
来源：http://jd.hnjuh.cn

Go:   len(arr);  len(m)
来源：http://gm.shtwfgs.cn

Ruby: x.length;  x.size
来源：http://mx.hahajie.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://xd.yuexingan06.cn

[P05] 判断两个对象内容是否相等
来源：http://hk.haigaiapp.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://ak.bookmarksfly.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ed.bjjhwx.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://uy.9csxet.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ie.wgjwhj.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://vk.bjjhwx.cn

Go:   reflect.DeepEqual(a, b)
来源：http://wm.bookmarksfly.cn

Ruby: a == b
来源：http://pv.yuexingan06.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://fb.chemitech.net.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mn.szsharing.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://sa.lnxyls.cn

PHP:  if (empty($x)) {}
来源：http://pn.bookmarksfly.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://bl.huixiangedu.cn

TS:   if (x == null) {}
来源：http://qh.huanxung.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://hl.shtwfgs.cn

Go:   if x == nil {}
来源：http://ya.bjjhwx.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://rl.yuexingan06.cn

C#:   if (x is null) {}
来源：http://hh.panjiajie.cn

[P07] 防抖与节流
来源：http://bb.yuntaijiaju.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://fe.nszjky.cn

PHP:  // 手写时间戳比较
来源：http://dz.jianghongdianzi.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://fy.huixiangedu.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ti.muxihuayi.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://rb.nszjky.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://jh.jctech888.com.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://my.wgjwhj.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://nn.muxihuayi.cn

[P08] 处理浮点精度问题
来源：http://fm.521024.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mn.shtwfgs.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://zp.chemitech.net.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://lz.shxzukj.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://zy.hahajie.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://qg.nszjky.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://rr.shxzukj.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://dk.colortex.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://we.shxzukj.cn

================================================================================
来源：http://ig.bjjhwx.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://tq.chemitech.net.cn

================================================================================
来源：http://ds.gzmigu.cn

[Q01] 创建表
来源：http://td.9csxet.cn

CREATE TABLE users (
来源：http://xy.newstarts.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://vk.newstarts.cn

name VARCHAR(50) NOT NULL,
来源：http://ep.shxzukj.cn

email VARCHAR(100) UNIQUE,
来源：http://vq.huixinmuqiang.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wx.muxihuayi.cn

);
来源：http://ju.haigaiapp.cn

[Q02] 创建带外键的表
来源：http://yd.gzmigu.cn

CREATE TABLE orders (
来源：http://ak.hnjuh.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://bq.muxihuayi.cn

user_id INT NOT NULL,
来源：http://cq.hahajie.cn

amount DECIMAL(10, 2),
来源：http://gn.gzmigu.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ev.colortex.cn

);
来源：http://dc.shxzukj.cn

[Q03] 增加列
来源：http://fv.huixinmuqiang.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://xr.jctech888.com.cn

[Q04] 修改列类型
来源：http://xh.szsharing.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://do.huanxung.cn

[Q05] 重命名列
来源：http://wj.521024.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://dw.yuntaijiaju.cn

[Q06] 删除列
来源：http://ks.muxihuayi.cn

ALTER TABLE users DROP COLUMN age;
来源：http://ie.nszjky.cn

[Q07] 删除表
来源：http://qs.szxytkj.cn

DROP TABLE IF EXISTS orders;
来源：http://rv.nicolike.cn

[Q08] 创建普通索引
来源：http://yo.bjjhwx.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://bx.shxzukj.cn

[Q09] 创建唯一索引
来源：http://dv.bjjhwx.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ix.yuntaijiaju.cn

[Q10] 插入单行
来源：http://er.nszjky.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mj.shxzukj.cn

[Q11] 一次插入多行
来源：http://rf.bjjhwx.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://no.bjjhwx.cn

[Q12] 插入后取自增 ID
来源：http://sp.9csxet.cn

INSERT INTO users (name) VALUES ('C');
来源：http://fk.shtwfgs.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://nu.asd995.cn

[Q13] 忽略重复插入
来源：http://fq.panjiajie.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://rs.haigaiapp.cn

[Q14] 存在则更新（upsert）
来源：http://ff.hahajie.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ti.newstarts.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://qv.shxzskj.cn

[Q15] 查询全部
来源：http://ml.szsharing.cn

SELECT * FROM users;
来源：http://gm.lnxyls.cn

[Q16] 查询指定列
来源：http://hv.haigaiapp.cn

SELECT id, name FROM users;
来源：http://jx.hahajie.cn

[Q17] 条件查询
来源：http://qi.colortex.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://tl.wgjwhj.cn

[Q18] 模糊匹配
来源：http://bo.jianghongdianzi.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://rf.muxihuayi.cn

[Q19] 范围查询
来源：http://pc.haigaiapp.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ba.huanxung.cn

[Q20] IN 列表
来源：http://qj.jctech888.com.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://lp.yuntaijiaju.cn

[Q21] 空值判断
来源：http://uj.jctech888.com.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://yt.nicolike.cn

[Q22] 排序
来源：http://vw.szxytkj.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://sn.newstarts.cn

[Q23] 分页
来源：http://yd.shtwfgs.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://qf.panjiajie.cn

[Q24] 去重
来源：http://rz.huixiangedu.cn

SELECT DISTINCT city FROM users;
来源：http://rt.jctech888.com.cn

[Q25] 只取前 N 条
来源：http://hl.colortex.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ah.gzmigu.cn

[Q26] 计数
来源：http://if.chemitech.net.cn

SELECT COUNT(*) FROM users;
来源：http://dq.hahajie.cn

[Q27] 条件计数
来源：http://ak.muxihuayi.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://fh.jianghongdianzi.cn

[Q28] 求和与平均
来源：http://oo.panjiajie.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wd.panjiajie.cn

[Q29] 最大最小值
来源：http://xj.bookmarksfly.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://yz.yuexingan06.cn

[Q30] 分组统计
来源：http://jc.szxytkj.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://fj.9csxet.cn

[Q31] 分组后过滤
来源：http://hv.lnxyls.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://vn.huanxung.cn

[Q32] 分组拼接字符串
来源：http://fo.colortex.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://lu.huixinmuqiang.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://br.muxihuayi.cn

[Q33] 多列分组
来源：http://al.panjiajie.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://sj.haigaiapp.cn

[Q34] 每组取第一条
来源：http://jn.huanxung.cn

SELECT * FROM (
来源：http://uc.shxzukj.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://fc.yuexingan06.cn

) t WHERE rn = 1;
来源：http://sn.nicolike.cn

[Q35] 内连接
来源：http://sd.panjiajie.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://qe.panjiajie.cn

[Q36] 左连接
来源：http://qj.huixinmuqiang.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://so.asd995.cn

[Q37] 右连接
来源：http://bk.chemitech.net.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ad.shxzskj.cn

[Q38] 全外连接（PostgreSQL）
来源：http://va.panjiajie.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ud.jianghongdianzi.cn

[Q39] 自连接（查上下级）
来源：http://rl.gzmigu.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://ty.hahajie.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://pp.newstarts.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://hi.newstarts.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://nz.gzmigu.cn

[Q41] 多表连接
来源：http://jw.yuexingan06.cn


<!-- 参考信息 -->