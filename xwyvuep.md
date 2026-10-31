代发 wailian999

[N05] 最大公约数
来源：http://dx.bjjhwx.cn

Py:   math.gcd(a, b)
来源：http://ae.yuntaijiaju.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://gi.haigaiapp.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://iy.panjiajie.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hj.jianghongdianzi.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://iz.yuntaijiaju.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://kr.colortex.cn

Ruby: a.gcd(b)
来源：http://oq.haigaiapp.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://gz.bjjhwx.cn

[N06] 判断回文字符串
来源：http://ys.muxihuayi.cn

Py:   s == s[::-1]
来源：http://rc.panjiajie.cn

PHP:  $s === strrev($s);
来源：http://qp.shxzskj.cn

JS:   s === [...s].reverse().join("")
来源：http://db.huanxung.cn

TS:   s === [...s].reverse().join("")
来源：http://kl.asd995.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://xf.521024.cn

Go:   // 双指针从两端比较
来源：http://if.colortex.cn

Ruby: s == s.reverse
来源：http://lm.huixinmuqiang.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://fp.chemitech.net.cn

[N07] 两数之和（返回下标）
来源：http://oz.nszjky.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ud.9csxet.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hc.bjjhwx.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://to.panjiajie.cn

TS:   // 手写 Map<string, number>
来源：http://jc.hnjuh.cn

Java: // 手写 HashMap
来源：http://vy.bjjhwx.cn

Go:   // 手写 map[int]int
来源：http://or.bookmarksfly.cn

Ruby: // 手写 Hash
来源：http://fj.yuntaijiaju.cn

C#:   // 手写 Dictionary<int, int>
来源：http://fa.jctech888.com.cn

[N08] 生成全排列
来源：http://vf.wgjwhj.cn

Py:   itertools.permutations(arr)
来源：http://xw.shxzskj.cn

PHP:  // 手写递归交换
来源：http://ti.hnjuh.cn

JS:   // 手写回溯递归
来源：http://fv.521024.cn

TS:   // 手写回溯递归
来源：http://nm.huanxung.cn

Java: // 手写回溯递归
来源：http://ri.szxytkj.cn

Go:   // 手写回溯递归
来源：http://fu.nszjky.cn

Ruby: arr.permutation.to_a
来源：http://yj.szxytkj.cn

C#:   // 手写回溯递归
来源：http://rb.jctech888.com.cn

[N09] 栈与队列
来源：http://fw.lnxyls.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://cd.521024.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://fx.huixiangedu.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wi.shxzukj.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://vf.muxihuayi.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://xc.bookmarksfly.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ll.shxzukj.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://py.haigaiapp.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://gj.nszjky.cn

[N10] 链表节点定义
来源：http://pc.nicolike.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://cp.newstarts.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://sn.bjjhwx.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://bh.szxytkj.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://qz.lnxyls.cn

Java: class Node { int v; Node next; }
来源：http://vk.521024.cn

Go:   type Node struct { V int; Next *Node }
来源：http://ut.szxytkj.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://us.9csxet.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://lv.shxzukj.cn

[N11] 二叉树中序遍历
来源：http://ao.yuntaijiaju.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ro.yuntaijiaju.cn

PHP:  // 手写递归函数
来源：http://oa.huixiangedu.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ok.newstarts.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://yd.hahajie.cn

Java: // 手写递归
来源：http://ak.bjjhwx.cn

Go:   // 手写递归
来源：http://wq.lnxyls.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://xb.bjjhwx.cn

C#:   // 手写递归
来源：http://ry.521024.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ej.gzmigu.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://zp.szxytkj.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://px.nszjky.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mv.521024.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://tv.bjjhwx.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://zq.bookmarksfly.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://fj.szxytkj.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ig.colortex.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ln.shxzskj.cn

================================================================================
来源：http://hz.yuexingan06.cn

O. 并发与异步
来源：http://mu.nicolike.cn

================================================================================
来源：http://te.shxzskj.cn

[O01] 启动一个线程
来源：http://th.bjjhwx.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://dn.asd995.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://oi.yuntaijiaju.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://le.hnjuh.cn

TS:   // 同 JS
来源：http://cs.huanxung.cn

Java: new Thread(() -> f()).start()
来源：http://cu.lnxyls.cn

Go:   go f()
来源：http://ot.hnjuh.cn

Ruby: Thread.new { f }
来源：http://uu.nszjky.cn

C#:   Task.Run(() => F());
来源：http://oh.huixiangedu.cn

[O02] 使用线程池
来源：http://of.shxzukj.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://sw.muxihuayi.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ov.shtwfgs.cn

JS:   // worker_threads 线程池
来源：http://xv.shxzukj.cn

TS:   // worker_threads 线程池
来源：http://cl.huixinmuqiang.cn

Java: Executors.newFixedThreadPool(4)
来源：http://wm.asd995.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://am.shxzukj.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://or.huixiangedu.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://pk.chemitech.net.cn

[O03] 加锁保护共享数据
来源：http://ni.hnjuh.cn

Py:   with lock: shared += 1
来源：http://rr.colortex.cn

PHP:  // 用 flock() 做文件锁
来源：http://kq.panjiajie.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ux.shxzukj.cn

TS:   // 同 JS
来源：http://ey.wgjwhj.cn

Java: synchronized (this) { shared++; }
来源：http://ig.szxytkj.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mu.panjiajie.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://if.521024.cn

C#:   lock (gate) { shared++; }
来源：http://xt.yuntaijiaju.cn

[O04] 定义异步函数并等待
来源：http://eb.jianghongdianzi.cn

Py:   async def f():⏎    await g()
来源：http://pl.shxzukj.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://uu.huixiangedu.cn

JS:   async function f() { await g(); }
来源：http://dj.newstarts.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://qe.haigaiapp.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://qf.gzmigu.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hs.9csxet.cn

Ruby: # 用 Fiber 或 async gem
来源：http://bw.yuntaijiaju.cn

C#:   async Task F() { await G(); }
来源：http://cc.nicolike.cn

[O05] 并发执行并等待全部完成
来源：http://mj.hnjuh.cn

Py:   asyncio.gather(*tasks)
来源：http://hc.wgjwhj.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://iw.shxzskj.cn

JS:   await Promise.all(tasks)
来源：http://ns.colortex.cn

TS:   await Promise.all(tasks)
来源：http://cq.wgjwhj.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://om.huixinmuqiang.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://xb.szsharing.cn

Ruby: threads.map(&:join)
来源：http://nr.hnjuh.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://wz.lnxyls.cn

[O06] 使用进程池
来源：http://vt.newstarts.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wn.bookmarksfly.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://mt.szxytkj.cn

JS:   // child_process / cluster 模块
来源：http://ty.wgjwhj.cn

TS:   // child_process / cluster 模块
来源：http://bi.colortex.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://xp.panjiajie.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ot.newstarts.cn

Ruby: // fork 块
来源：http://bi.huanxung.cn

C#:   Parallel.For
来源：http://qq.hnjuh.cn

================================================================================
来源：http://sz.jianghongdianzi.cn

P. 常用工具函数
来源：http://ni.asd995.cn

================================================================================
来源：http://ml.jianghongdianzi.cn

[P01] 生成 UUID
来源：http://bj.huixiangedu.cn

Py:   str(uuid.uuid4())
来源：http://nw.wgjwhj.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ru.hnjuh.cn

JS:   crypto.randomUUID()
来源：http://dl.newstarts.cn

TS:   crypto.randomUUID()
来源：http://ge.haigaiapp.cn

Java: UUID.randomUUID().toString()
来源：http://ck.yuexingan06.cn

Go:   // 用 github.com/google/uuid
来源：http://uo.wgjwhj.cn

Ruby: SecureRandom.uuid
来源：http://zr.shtwfgs.cn

C#:   Guid.NewGuid().ToString()
来源：http://hi.hnjuh.cn

[P02] MD5 / SHA256 摘要
来源：http://lt.gzmigu.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ow.hnjuh.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://rh.bjjhwx.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://je.huixiangedu.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ps.bjjhwx.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://zb.bjjhwx.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://so.huanxung.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://lj.chemitech.net.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://yl.chemitech.net.cn

[P03] 生成短随机字符串
来源：http://az.shtwfgs.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://vi.9csxet.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hc.jianghongdianzi.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ft.muxihuayi.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://rq.newstarts.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://dw.yuexingan06.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://zq.hahajie.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://jk.huixiangedu.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://jp.szxytkj.cn

[P04] 求长度
来源：http://rb.yuexingan06.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://sw.521024.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://vr.nicolike.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ul.nszjky.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://yj.newstarts.cn

Java: list.size();  map.size();  s.length()
来源：http://dd.nicolike.cn

Go:   len(arr);  len(m)
来源：http://up.haigaiapp.cn

Ruby: x.length;  x.size
来源：http://vj.yuexingan06.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://ep.newstarts.cn

[P05] 判断两个对象内容是否相等
来源：http://eo.chemitech.net.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://cd.gzmigu.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://rd.wgjwhj.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://gf.shxzskj.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ob.shtwfgs.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://dh.nicolike.cn

Go:   reflect.DeepEqual(a, b)
来源：http://na.szxytkj.cn

Ruby: a == b
来源：http://ug.wgjwhj.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ye.panjiajie.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ym.yuntaijiaju.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ec.huixiangedu.cn

PHP:  if (empty($x)) {}
来源：http://ce.newstarts.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://sy.nszjky.cn

TS:   if (x == null) {}
来源：http://jz.szsharing.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://zf.shxzukj.cn

Go:   if x == nil {}
来源：http://fv.lnxyls.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ai.bookmarksfly.cn

C#:   if (x is null) {}
来源：http://xq.yuntaijiaju.cn

[P07] 防抖与节流
来源：http://bw.jianghongdianzi.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ij.nicolike.cn

PHP:  // 手写时间戳比较
来源：http://cc.9csxet.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ab.hnjuh.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://jv.gzmigu.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://go.gzmigu.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://zj.lnxyls.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://dl.bjjhwx.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://vw.9csxet.cn

[P08] 处理浮点精度问题
来源：http://dv.hnjuh.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ay.yuntaijiaju.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ue.jianghongdianzi.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://zi.bookmarksfly.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://yu.gzmigu.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://rl.newstarts.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://yu.shxzukj.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://gh.bjjhwx.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://us.jianghongdianzi.cn

================================================================================
来源：http://zt.521024.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://oe.bjjhwx.cn

================================================================================
来源：http://nw.hahajie.cn

[Q01] 创建表
来源：http://fi.hahajie.cn

CREATE TABLE users (
来源：http://ho.9csxet.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://zx.nicolike.cn

name VARCHAR(50) NOT NULL,
来源：http://ke.jianghongdianzi.cn

email VARCHAR(100) UNIQUE,
来源：http://jz.shxzskj.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://gq.jctech888.com.cn

);
来源：http://hr.yuexingan06.cn

[Q02] 创建带外键的表
来源：http://ru.colortex.cn

CREATE TABLE orders (
来源：http://aj.shtwfgs.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://vt.asd995.cn

user_id INT NOT NULL,
来源：http://dt.muxihuayi.cn

amount DECIMAL(10, 2),
来源：http://ud.9csxet.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://th.muxihuayi.cn

);
来源：http://bm.newstarts.cn

[Q03] 增加列
来源：http://sn.nszjky.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://cx.nicolike.cn

[Q04] 修改列类型
来源：http://me.lnxyls.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://od.huixinmuqiang.cn

[Q05] 重命名列
来源：http://ba.9csxet.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://dv.lnxyls.cn

[Q06] 删除列
来源：http://hb.jianghongdianzi.cn

ALTER TABLE users DROP COLUMN age;
来源：http://ae.szsharing.cn

[Q07] 删除表
来源：http://qb.gzmigu.cn

DROP TABLE IF EXISTS orders;
来源：http://cc.shxzukj.cn

[Q08] 创建普通索引
来源：http://ou.hahajie.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://hf.shtwfgs.cn

[Q09] 创建唯一索引
来源：http://jz.huixinmuqiang.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://uc.newstarts.cn

[Q10] 插入单行
来源：http://mo.jctech888.com.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://nl.shtwfgs.cn

[Q11] 一次插入多行
来源：http://ed.lnxyls.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wf.szxytkj.cn

[Q12] 插入后取自增 ID
来源：http://iy.lnxyls.cn

INSERT INTO users (name) VALUES ('C');
来源：http://tz.jianghongdianzi.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://dk.jctech888.com.cn

[Q13] 忽略重复插入
来源：http://js.hnjuh.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://nf.szxytkj.cn

[Q14] 存在则更新（upsert）
来源：http://cj.9csxet.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ct.haigaiapp.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://cz.nicolike.cn

[Q15] 查询全部
来源：http://hu.bookmarksfly.cn

SELECT * FROM users;
来源：http://pb.huixiangedu.cn

[Q16] 查询指定列
来源：http://tt.bookmarksfly.cn

SELECT id, name FROM users;
来源：http://lw.asd995.cn

[Q17] 条件查询
来源：http://br.9csxet.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://lj.jianghongdianzi.cn

[Q18] 模糊匹配
来源：http://yi.yuexingan06.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://td.521024.cn

[Q19] 范围查询
来源：http://zk.newstarts.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://lm.szxytkj.cn

[Q20] IN 列表
来源：http://aw.9csxet.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://gq.yuntaijiaju.cn

[Q21] 空值判断
来源：http://ci.yuntaijiaju.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://ly.huanxung.cn

[Q22] 排序
来源：http://fr.asd995.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ik.yuntaijiaju.cn

[Q23] 分页
来源：http://js.gzmigu.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://at.lnxyls.cn

[Q24] 去重
来源：http://sn.521024.cn

SELECT DISTINCT city FROM users;
来源：http://bq.shxzukj.cn

[Q25] 只取前 N 条
来源：http://nj.wgjwhj.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://sl.panjiajie.cn

[Q26] 计数
来源：http://bv.chemitech.net.cn

SELECT COUNT(*) FROM users;
来源：http://gd.shxzukj.cn

[Q27] 条件计数
来源：http://mx.bjjhwx.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://vc.huixinmuqiang.cn

[Q28] 求和与平均
来源：http://ud.yuexingan06.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://dn.huanxung.cn

[Q29] 最大最小值
来源：http://ow.nicolike.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://bm.shtwfgs.cn

[Q30] 分组统计
来源：http://he.9csxet.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://no.shxzukj.cn

[Q31] 分组后过滤
来源：http://tn.9csxet.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wa.9csxet.cn

[Q32] 分组拼接字符串
来源：http://yc.jianghongdianzi.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://pl.muxihuayi.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://yb.szsharing.cn

[Q33] 多列分组
来源：http://fn.nicolike.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://kq.szxytkj.cn

[Q34] 每组取第一条
来源：http://fr.yuexingan06.cn

SELECT * FROM (
来源：http://cc.muxihuayi.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://fp.huixiangedu.cn

) t WHERE rn = 1;
来源：http://np.yuexingan06.cn

[Q35] 内连接
来源：http://fy.chemitech.net.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://fb.huixinmuqiang.cn

[Q36] 左连接
来源：http://us.jianghongdianzi.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ko.jctech888.com.cn

[Q37] 右连接
来源：http://nf.wgjwhj.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ge.521024.cn

[Q38] 全外连接（PostgreSQL）
来源：http://dj.colortex.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wa.521024.cn

[Q39] 自连接（查上下级）
来源：http://ok.szxytkj.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://sh.nicolike.cn


<!-- 参考信息 -->