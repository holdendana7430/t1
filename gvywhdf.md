代发 wailian999

[N05] 最大公约数
来源：http://rm.huixinmuqiang.cn

Py:   math.gcd(a, b)
来源：http://pm.huanxung.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://tf.nicolike.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://xb.asd995.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://xm.hahajie.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wi.haigaiapp.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://re.nszjky.cn

Ruby: a.gcd(b)
来源：http://du.gzmigu.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://cx.nszjky.cn

[N06] 判断回文字符串
来源：http://ez.jianghongdianzi.cn

Py:   s == s[::-1]
来源：http://pb.jianghongdianzi.cn

PHP:  $s === strrev($s);
来源：http://yl.muxihuayi.cn

JS:   s === [...s].reverse().join("")
来源：http://ne.huixinmuqiang.cn

TS:   s === [...s].reverse().join("")
来源：http://vf.9csxet.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://yb.asd995.cn

Go:   // 双指针从两端比较
来源：http://he.shtwfgs.cn

Ruby: s == s.reverse
来源：http://hx.yuntaijiaju.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://yv.9csxet.cn

[N07] 两数之和（返回下标）
来源：http://tq.colortex.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://xd.jctech888.com.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://lz.huixinmuqiang.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://mo.yuexingan06.cn

TS:   // 手写 Map<string, number>
来源：http://lf.newstarts.cn

Java: // 手写 HashMap
来源：http://im.9csxet.cn

Go:   // 手写 map[int]int
来源：http://zb.jctech888.com.cn

Ruby: // 手写 Hash
来源：http://fm.chemitech.net.cn

C#:   // 手写 Dictionary<int, int>
来源：http://cp.haigaiapp.cn

[N08] 生成全排列
来源：http://vd.hahajie.cn

Py:   itertools.permutations(arr)
来源：http://qz.hahajie.cn

PHP:  // 手写递归交换
来源：http://vc.chemitech.net.cn

JS:   // 手写回溯递归
来源：http://ku.huanxung.cn

TS:   // 手写回溯递归
来源：http://xj.lnxyls.cn

Java: // 手写回溯递归
来源：http://ve.panjiajie.cn

Go:   // 手写回溯递归
来源：http://yo.colortex.cn

Ruby: arr.permutation.to_a
来源：http://aw.yuexingan06.cn

C#:   // 手写回溯递归
来源：http://zk.szsharing.cn

[N09] 栈与队列
来源：http://dj.huanxung.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ht.asd995.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ri.huixiangedu.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://rm.shxzukj.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://bg.gzmigu.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://lv.chemitech.net.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://cy.asd995.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://sk.yuexingan06.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://qo.shxzukj.cn

[N10] 链表节点定义
来源：http://bt.nszjky.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ox.wgjwhj.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://bp.bjjhwx.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://cf.hahajie.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hb.521024.cn

Java: class Node { int v; Node next; }
来源：http://yk.shtwfgs.cn

Go:   type Node struct { V int; Next *Node }
来源：http://gv.lnxyls.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://jo.panjiajie.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://ch.newstarts.cn

[N11] 二叉树中序遍历
来源：http://xo.wgjwhj.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://nx.shxzukj.cn

PHP:  // 手写递归函数
来源：http://dz.yuntaijiaju.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://rh.9csxet.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ut.jctech888.com.cn

Java: // 手写递归
来源：http://sc.huixinmuqiang.cn

Go:   // 手写递归
来源：http://fp.521024.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://vq.haigaiapp.cn

C#:   // 手写递归
来源：http://io.asd995.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://oe.huixinmuqiang.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ax.521024.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wo.newstarts.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://bt.wgjwhj.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://rt.9csxet.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://kg.jianghongdianzi.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://nd.yuexingan06.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ge.huixiangedu.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://sm.asd995.cn

================================================================================
来源：http://nn.nicolike.cn

O. 并发与异步
来源：http://wv.yuntaijiaju.cn

================================================================================
来源：http://sg.hahajie.cn

[O01] 启动一个线程
来源：http://vc.hnjuh.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ga.jctech888.com.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mr.newstarts.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ti.jctech888.com.cn

TS:   // 同 JS
来源：http://ak.colortex.cn

Java: new Thread(() -> f()).start()
来源：http://ed.panjiajie.cn

Go:   go f()
来源：http://on.jctech888.com.cn

Ruby: Thread.new { f }
来源：http://nq.521024.cn

C#:   Task.Run(() => F());
来源：http://fx.9csxet.cn

[O02] 使用线程池
来源：http://xg.chemitech.net.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ah.chemitech.net.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://qm.9csxet.cn

JS:   // worker_threads 线程池
来源：http://xv.yuntaijiaju.cn

TS:   // worker_threads 线程池
来源：http://oy.nszjky.cn

Java: Executors.newFixedThreadPool(4)
来源：http://zk.haigaiapp.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://jw.szsharing.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ko.nicolike.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://kl.521024.cn

[O03] 加锁保护共享数据
来源：http://bb.yuntaijiaju.cn

Py:   with lock: shared += 1
来源：http://xb.jianghongdianzi.cn

PHP:  // 用 flock() 做文件锁
来源：http://fc.jctech888.com.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://yw.9csxet.cn

TS:   // 同 JS
来源：http://yx.colortex.cn

Java: synchronized (this) { shared++; }
来源：http://ug.shxzskj.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://pn.nicolike.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://th.chemitech.net.cn

C#:   lock (gate) { shared++; }
来源：http://fj.521024.cn

[O04] 定义异步函数并等待
来源：http://ai.huixiangedu.cn

Py:   async def f():⏎    await g()
来源：http://iv.huanxung.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://va.haigaiapp.cn

JS:   async function f() { await g(); }
来源：http://zu.szxytkj.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://fw.yuntaijiaju.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hv.shxzukj.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://cx.yuntaijiaju.cn

Ruby: # 用 Fiber 或 async gem
来源：http://bx.wgjwhj.cn

C#:   async Task F() { await G(); }
来源：http://jk.hnjuh.cn

[O05] 并发执行并等待全部完成
来源：http://zl.wgjwhj.cn

Py:   asyncio.gather(*tasks)
来源：http://if.huanxung.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://gi.hahajie.cn

JS:   await Promise.all(tasks)
来源：http://hm.nicolike.cn

TS:   await Promise.all(tasks)
来源：http://wh.yuexingan06.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://yd.hnjuh.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://vk.yuexingan06.cn

Ruby: threads.map(&:join)
来源：http://nc.lnxyls.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://hx.huanxung.cn

[O06] 使用进程池
来源：http://ch.yuntaijiaju.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ti.hahajie.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://xw.colortex.cn

JS:   // child_process / cluster 模块
来源：http://vi.asd995.cn

TS:   // child_process / cluster 模块
来源：http://dz.szxytkj.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://yu.newstarts.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hp.shxzukj.cn

Ruby: // fork 块
来源：http://ky.shtwfgs.cn

C#:   Parallel.For
来源：http://ns.huanxung.cn

================================================================================
来源：http://xh.nszjky.cn

P. 常用工具函数
来源：http://pp.bookmarksfly.cn

================================================================================
来源：http://wo.muxihuayi.cn

[P01] 生成 UUID
来源：http://pr.nszjky.cn

Py:   str(uuid.uuid4())
来源：http://xo.bjjhwx.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://um.huanxung.cn

JS:   crypto.randomUUID()
来源：http://fp.hnjuh.cn

TS:   crypto.randomUUID()
来源：http://gt.haigaiapp.cn

Java: UUID.randomUUID().toString()
来源：http://tu.szsharing.cn

Go:   // 用 github.com/google/uuid
来源：http://zo.jctech888.com.cn

Ruby: SecureRandom.uuid
来源：http://xi.jctech888.com.cn

C#:   Guid.NewGuid().ToString()
来源：http://hm.huixiangedu.cn

[P02] MD5 / SHA256 摘要
来源：http://qj.muxihuayi.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://dy.colortex.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://pg.muxihuayi.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://fo.newstarts.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://jp.asd995.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://qf.haigaiapp.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ea.szxytkj.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://lj.hnjuh.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://tf.shtwfgs.cn

[P03] 生成短随机字符串
来源：http://uz.panjiajie.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://xg.gzmigu.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ma.haigaiapp.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ue.huixiangedu.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://pm.nszjky.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://zi.nszjky.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://if.9csxet.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://ct.hahajie.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ft.bookmarksfly.cn

[P04] 求长度
来源：http://cb.wgjwhj.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://nh.szsharing.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://az.bjjhwx.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mq.panjiajie.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://as.jctech888.com.cn

Java: list.size();  map.size();  s.length()
来源：http://rs.hnjuh.cn

Go:   len(arr);  len(m)
来源：http://hk.bjjhwx.cn

Ruby: x.length;  x.size
来源：http://lj.521024.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://xg.jianghongdianzi.cn

[P05] 判断两个对象内容是否相等
来源：http://ll.nszjky.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://pm.shxzskj.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://pn.lnxyls.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://vj.nszjky.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://tt.huanxung.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://sr.newstarts.cn

Go:   reflect.DeepEqual(a, b)
来源：http://ht.gzmigu.cn

Ruby: a == b
来源：http://aw.panjiajie.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://vh.hahajie.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://qb.huixinmuqiang.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://dw.521024.cn

PHP:  if (empty($x)) {}
来源：http://ei.9csxet.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ad.panjiajie.cn

TS:   if (x == null) {}
来源：http://mv.yuntaijiaju.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://wj.asd995.cn

Go:   if x == nil {}
来源：http://zj.haigaiapp.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://yw.shtwfgs.cn

C#:   if (x is null) {}
来源：http://gi.wgjwhj.cn

[P07] 防抖与节流
来源：http://wt.wgjwhj.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://vm.nszjky.cn

PHP:  // 手写时间戳比较
来源：http://na.muxihuayi.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ko.asd995.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://js.shxzskj.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://iu.newstarts.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://nw.panjiajie.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://ry.szxytkj.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://eu.colortex.cn

[P08] 处理浮点精度问题
来源：http://mv.jctech888.com.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ny.lnxyls.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://om.hnjuh.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://gq.huixiangedu.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://gi.yuexingan06.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ae.colortex.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://kt.panjiajie.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://qi.jctech888.com.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://er.nicolike.cn

================================================================================
来源：http://qt.hahajie.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://le.szxytkj.cn

================================================================================
来源：http://fq.colortex.cn

[Q01] 创建表
来源：http://ky.yuntaijiaju.cn

CREATE TABLE users (
来源：http://mz.szsharing.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://jz.yuexingan06.cn

name VARCHAR(50) NOT NULL,
来源：http://ej.hahajie.cn

email VARCHAR(100) UNIQUE,
来源：http://hy.panjiajie.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://oe.jianghongdianzi.cn

);
来源：http://xe.521024.cn

[Q02] 创建带外键的表
来源：http://xw.asd995.cn

CREATE TABLE orders (
来源：http://le.hahajie.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://rq.hahajie.cn

user_id INT NOT NULL,
来源：http://cu.shxzukj.cn

amount DECIMAL(10, 2),
来源：http://ww.yuntaijiaju.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://qi.yuntaijiaju.cn

);
来源：http://xc.shxzukj.cn

[Q03] 增加列
来源：http://zf.bookmarksfly.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://yg.wgjwhj.cn

[Q04] 修改列类型
来源：http://nw.jianghongdianzi.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://gt.nszjky.cn

[Q05] 重命名列
来源：http://qd.huixiangedu.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ki.yuexingan06.cn

[Q06] 删除列
来源：http://cx.jianghongdianzi.cn

ALTER TABLE users DROP COLUMN age;
来源：http://su.jctech888.com.cn

[Q07] 删除表
来源：http://ag.newstarts.cn

DROP TABLE IF EXISTS orders;
来源：http://nb.jianghongdianzi.cn

[Q08] 创建普通索引
来源：http://pz.521024.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://ns.yuexingan06.cn

[Q09] 创建唯一索引
来源：http://bp.muxihuayi.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ka.huixiangedu.cn

[Q10] 插入单行
来源：http://hx.shtwfgs.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://lt.yuntaijiaju.cn

[Q11] 一次插入多行
来源：http://ve.colortex.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://qt.jctech888.com.cn

[Q12] 插入后取自增 ID
来源：http://fm.haigaiapp.cn

INSERT INTO users (name) VALUES ('C');
来源：http://qu.nicolike.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://qe.huixiangedu.cn

[Q13] 忽略重复插入
来源：http://sd.nicolike.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://qt.9csxet.cn

[Q14] 存在则更新（upsert）
来源：http://sl.bjjhwx.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://vt.hnjuh.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://nj.yuexingan06.cn

[Q15] 查询全部
来源：http://ia.jianghongdianzi.cn

SELECT * FROM users;
来源：http://du.nicolike.cn

[Q16] 查询指定列
来源：http://sy.shxzskj.cn

SELECT id, name FROM users;
来源：http://vo.szxytkj.cn

[Q17] 条件查询
来源：http://bz.lnxyls.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://qp.521024.cn

[Q18] 模糊匹配
来源：http://wl.haigaiapp.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://pa.huixiangedu.cn

[Q19] 范围查询
来源：http://ha.huixinmuqiang.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://zt.jianghongdianzi.cn

[Q20] IN 列表
来源：http://ka.haigaiapp.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wa.huixinmuqiang.cn

[Q21] 空值判断
来源：http://lc.hahajie.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://if.521024.cn

[Q22] 排序
来源：http://la.huixiangedu.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ya.chemitech.net.cn

[Q23] 分页
来源：http://lv.huixinmuqiang.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://va.chemitech.net.cn

[Q24] 去重
来源：http://is.bookmarksfly.cn

SELECT DISTINCT city FROM users;
来源：http://ql.chemitech.net.cn

[Q25] 只取前 N 条
来源：http://wx.bjjhwx.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://el.chemitech.net.cn

[Q26] 计数
来源：http://er.gzmigu.cn

SELECT COUNT(*) FROM users;
来源：http://fc.huixiangedu.cn

[Q27] 条件计数
来源：http://ky.asd995.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://fk.hnjuh.cn

[Q28] 求和与平均
来源：http://oq.huanxung.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://ms.9csxet.cn

[Q29] 最大最小值
来源：http://kj.huanxung.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://kp.chemitech.net.cn

[Q30] 分组统计
来源：http://fm.haigaiapp.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://rz.nszjky.cn

[Q31] 分组后过滤
来源：http://do.asd995.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ej.huixiangedu.cn

[Q32] 分组拼接字符串
来源：http://iy.asd995.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://jp.newstarts.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://vi.szsharing.cn

[Q33] 多列分组
来源：http://ki.shxzukj.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ti.shxzskj.cn

[Q34] 每组取第一条
来源：http://wi.shxzukj.cn

SELECT * FROM (
来源：http://np.wgjwhj.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ac.huixinmuqiang.cn

) t WHERE rn = 1;
来源：http://zy.hahajie.cn

[Q35] 内连接
来源：http://iy.nicolike.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wg.huixiangedu.cn

[Q36] 左连接
来源：http://dd.bjjhwx.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://db.gzmigu.cn

[Q37] 右连接
来源：http://fp.wgjwhj.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://qh.521024.cn

[Q38] 全外连接（PostgreSQL）
来源：http://ls.huanxung.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hn.jianghongdianzi.cn

[Q39] 自连接（查上下级）
来源：http://wn.panjiajie.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://tf.shxzukj.cn


<!-- 参考信息 -->