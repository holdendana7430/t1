代发 wailian999

JS:   s === [...s].reverse().join("")
来源：http://ja.colortex.cn

TS:   s === [...s].reverse().join("")
来源：http://ow.huixiangedu.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://xg.shxzskj.cn

Go:   // 双指针从两端比较
来源：http://om.szxytkj.cn

Ruby: s == s.reverse
来源：http://cq.nicolike.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://gk.newstarts.cn

[N07] 两数之和（返回下标）
来源：http://bs.shxzukj.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://as.gzmigu.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://pl.chemitech.net.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://nm.huanxung.cn

TS:   // 手写 Map<string, number>
来源：http://tc.shxzskj.cn

Java: // 手写 HashMap
来源：http://xp.shxzukj.cn

Go:   // 手写 map[int]int
来源：http://pl.wgjwhj.cn

Ruby: // 手写 Hash
来源：http://cp.asd995.cn

C#:   // 手写 Dictionary<int, int>
来源：http://as.wgjwhj.cn

[N08] 生成全排列
来源：http://fl.bjjhwx.cn

Py:   itertools.permutations(arr)
来源：http://as.muxihuayi.cn

PHP:  // 手写递归交换
来源：http://gy.huixiangedu.cn

JS:   // 手写回溯递归
来源：http://tw.huixiangedu.cn

TS:   // 手写回溯递归
来源：http://jc.nicolike.cn

Java: // 手写回溯递归
来源：http://xu.muxihuayi.cn

Go:   // 手写回溯递归
来源：http://lg.nszjky.cn

Ruby: arr.permutation.to_a
来源：http://lk.shtwfgs.cn

C#:   // 手写回溯递归
来源：http://cv.hnjuh.cn

[N09] 栈与队列
来源：http://jz.hahajie.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://gz.nszjky.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://rx.gzmigu.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://cu.lnxyls.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://td.yuexingan06.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://bc.muxihuayi.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://sh.hnjuh.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ir.huixinmuqiang.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://cu.huanxung.cn

[N10] 链表节点定义
来源：http://ay.shxzukj.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://nb.huanxung.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://cp.muxihuayi.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://la.muxihuayi.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://lu.newstarts.cn

Java: class Node { int v; Node next; }
来源：http://xk.521024.cn

Go:   type Node struct { V int; Next *Node }
来源：http://oo.bookmarksfly.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://fj.hnjuh.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://lq.nszjky.cn

[N11] 二叉树中序遍历
来源：http://sn.9csxet.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://um.haigaiapp.cn

PHP:  // 手写递归函数
来源：http://dr.9csxet.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://qr.wgjwhj.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://kv.9csxet.cn

Java: // 手写递归
来源：http://ou.bookmarksfly.cn

Go:   // 手写递归
来源：http://tk.yuntaijiaju.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://pm.nszjky.cn

C#:   // 手写递归
来源：http://ic.chemitech.net.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ds.szxytkj.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://xd.colortex.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ie.asd995.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://gv.jctech888.com.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://rp.yuexingan06.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://rg.colortex.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://lh.gzmigu.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://qx.jianghongdianzi.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://aw.muxihuayi.cn

================================================================================
来源：http://zt.huixinmuqiang.cn

O. 并发与异步
来源：http://el.hahajie.cn

================================================================================
来源：http://qz.szsharing.cn

[O01] 启动一个线程
来源：http://aq.panjiajie.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://lj.521024.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hm.bookmarksfly.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ki.shtwfgs.cn

TS:   // 同 JS
来源：http://pd.colortex.cn

Java: new Thread(() -> f()).start()
来源：http://le.bookmarksfly.cn

Go:   go f()
来源：http://um.newstarts.cn

Ruby: Thread.new { f }
来源：http://zh.gzmigu.cn

C#:   Task.Run(() => F());
来源：http://in.jctech888.com.cn

[O02] 使用线程池
来源：http://so.shxzskj.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://nm.yuexingan06.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://uy.hnjuh.cn

JS:   // worker_threads 线程池
来源：http://hz.huixinmuqiang.cn

TS:   // worker_threads 线程池
来源：http://zg.nicolike.cn

Java: Executors.newFixedThreadPool(4)
来源：http://nw.hahajie.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://yo.shtwfgs.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ch.lnxyls.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ny.yuntaijiaju.cn

[O03] 加锁保护共享数据
来源：http://vv.lnxyls.cn

Py:   with lock: shared += 1
来源：http://rb.jianghongdianzi.cn

PHP:  // 用 flock() 做文件锁
来源：http://xz.nicolike.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://rn.shxzukj.cn

TS:   // 同 JS
来源：http://ea.colortex.cn

Java: synchronized (this) { shared++; }
来源：http://wm.9csxet.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://fw.huanxung.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://bk.yuntaijiaju.cn

C#:   lock (gate) { shared++; }
来源：http://vv.szsharing.cn

[O04] 定义异步函数并等待
来源：http://su.bjjhwx.cn

Py:   async def f():⏎    await g()
来源：http://sg.yuexingan06.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://bo.yuexingan06.cn

JS:   async function f() { await g(); }
来源：http://aq.jianghongdianzi.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://ii.haigaiapp.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://kw.bjjhwx.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://if.chemitech.net.cn

Ruby: # 用 Fiber 或 async gem
来源：http://py.huixiangedu.cn

C#:   async Task F() { await G(); }
来源：http://ep.chemitech.net.cn

[O05] 并发执行并等待全部完成
来源：http://fl.szxytkj.cn

Py:   asyncio.gather(*tasks)
来源：http://gn.jianghongdianzi.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://iy.szxytkj.cn

JS:   await Promise.all(tasks)
来源：http://sn.panjiajie.cn

TS:   await Promise.all(tasks)
来源：http://lx.hnjuh.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hp.shxzukj.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://vy.haigaiapp.cn

Ruby: threads.map(&:join)
来源：http://xt.szsharing.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://fs.bjjhwx.cn

[O06] 使用进程池
来源：http://jj.shxzukj.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://uz.jianghongdianzi.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://dg.szxytkj.cn

JS:   // child_process / cluster 模块
来源：http://kg.lnxyls.cn

TS:   // child_process / cluster 模块
来源：http://hl.hnjuh.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://eo.asd995.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ky.shtwfgs.cn

Ruby: // fork 块
来源：http://ty.haigaiapp.cn

C#:   Parallel.For
来源：http://di.hahajie.cn

================================================================================
来源：http://pa.gzmigu.cn

P. 常用工具函数
来源：http://bh.szxytkj.cn

================================================================================
来源：http://hb.jianghongdianzi.cn

[P01] 生成 UUID
来源：http://om.szsharing.cn

Py:   str(uuid.uuid4())
来源：http://wl.huanxung.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://bz.haigaiapp.cn

JS:   crypto.randomUUID()
来源：http://dw.yuntaijiaju.cn

TS:   crypto.randomUUID()
来源：http://fo.huixiangedu.cn

Java: UUID.randomUUID().toString()
来源：http://yz.haigaiapp.cn

Go:   // 用 github.com/google/uuid
来源：http://ej.wgjwhj.cn

Ruby: SecureRandom.uuid
来源：http://ct.hnjuh.cn

C#:   Guid.NewGuid().ToString()
来源：http://xp.bookmarksfly.cn

[P02] MD5 / SHA256 摘要
来源：http://hr.shtwfgs.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://rg.nszjky.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://zh.huixinmuqiang.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://if.nszjky.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://vo.yuntaijiaju.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://vd.wgjwhj.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ds.yuntaijiaju.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://zz.muxihuayi.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://yn.newstarts.cn

[P03] 生成短随机字符串
来源：http://xj.lnxyls.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ki.wgjwhj.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://qq.hahajie.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ie.asd995.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ns.asd995.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://rq.huixiangedu.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://nn.shxzskj.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://qy.wgjwhj.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://gy.nszjky.cn

[P04] 求长度
来源：http://sj.shtwfgs.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://vs.yuexingan06.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hr.lnxyls.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ee.huanxung.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://xe.shxzukj.cn

Java: list.size();  map.size();  s.length()
来源：http://bd.9csxet.cn

Go:   len(arr);  len(m)
来源：http://cn.gzmigu.cn

Ruby: x.length;  x.size
来源：http://qk.jctech888.com.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://cn.bjjhwx.cn

[P05] 判断两个对象内容是否相等
来源：http://fs.hnjuh.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://qr.chemitech.net.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://jl.newstarts.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ob.bookmarksfly.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://yp.shxzskj.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ib.bookmarksfly.cn

Go:   reflect.DeepEqual(a, b)
来源：http://ld.yuexingan06.cn

Ruby: a == b
来源：http://jx.shxzskj.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hv.haigaiapp.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://qf.9csxet.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://nj.wgjwhj.cn

PHP:  if (empty($x)) {}
来源：http://qe.lnxyls.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://qk.szxytkj.cn

TS:   if (x == null) {}
来源：http://sv.521024.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://vy.chemitech.net.cn

Go:   if x == nil {}
来源：http://rj.huixiangedu.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://nq.asd995.cn

C#:   if (x is null) {}
来源：http://xk.yuntaijiaju.cn

[P07] 防抖与节流
来源：http://yj.haigaiapp.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://kb.lnxyls.cn

PHP:  // 手写时间戳比较
来源：http://aq.bjjhwx.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wv.bjjhwx.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://gi.panjiajie.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wv.shxzukj.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://zn.jctech888.com.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://md.panjiajie.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://yz.jianghongdianzi.cn

[P08] 处理浮点精度问题
来源：http://ox.szxytkj.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://jl.jianghongdianzi.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ax.muxihuayi.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://qd.huixiangedu.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://js.panjiajie.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://yz.yuntaijiaju.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://xi.shxzukj.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://qd.huixiangedu.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://id.asd995.cn

================================================================================
来源：http://ym.haigaiapp.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://gc.szsharing.cn

================================================================================
来源：http://mu.panjiajie.cn

[Q01] 创建表
来源：http://ln.shtwfgs.cn

CREATE TABLE users (
来源：http://jz.shxzskj.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://bc.panjiajie.cn

name VARCHAR(50) NOT NULL,
来源：http://tu.yuntaijiaju.cn

email VARCHAR(100) UNIQUE,
来源：http://nh.huixinmuqiang.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://gi.nicolike.cn

);
来源：http://kj.yuexingan06.cn

[Q02] 创建带外键的表
来源：http://mo.shxzukj.cn

CREATE TABLE orders (
来源：http://vt.521024.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://qr.newstarts.cn

user_id INT NOT NULL,
来源：http://an.haigaiapp.cn

amount DECIMAL(10, 2),
来源：http://uz.shxzskj.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ip.colortex.cn

);
来源：http://zl.szxytkj.cn

[Q03] 增加列
来源：http://wc.szxytkj.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://go.wgjwhj.cn

[Q04] 修改列类型
来源：http://sy.wgjwhj.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://yg.jctech888.com.cn

[Q05] 重命名列
来源：http://om.newstarts.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://nq.gzmigu.cn

[Q06] 删除列
来源：http://qs.shxzskj.cn

ALTER TABLE users DROP COLUMN age;
来源：http://uu.jctech888.com.cn

[Q07] 删除表
来源：http://bu.gzmigu.cn

DROP TABLE IF EXISTS orders;
来源：http://nm.asd995.cn

[Q08] 创建普通索引
来源：http://nu.nicolike.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://sz.jianghongdianzi.cn

[Q09] 创建唯一索引
来源：http://rz.panjiajie.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://zv.shxzukj.cn

[Q10] 插入单行
来源：http://hd.9csxet.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://qw.gzmigu.cn

[Q11] 一次插入多行
来源：http://gp.haigaiapp.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://rl.nicolike.cn

[Q12] 插入后取自增 ID
来源：http://fk.chemitech.net.cn

INSERT INTO users (name) VALUES ('C');
来源：http://vh.jctech888.com.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://pc.newstarts.cn

[Q13] 忽略重复插入
来源：http://ba.yuntaijiaju.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://eq.yuntaijiaju.cn

[Q14] 存在则更新（upsert）
来源：http://an.9csxet.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://qs.newstarts.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://sd.9csxet.cn

[Q15] 查询全部
来源：http://hf.gzmigu.cn

SELECT * FROM users;
来源：http://cu.panjiajie.cn

[Q16] 查询指定列
来源：http://wq.bookmarksfly.cn

SELECT id, name FROM users;
来源：http://be.huixinmuqiang.cn

[Q17] 条件查询
来源：http://wm.szsharing.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://bx.yuntaijiaju.cn

[Q18] 模糊匹配
来源：http://vq.newstarts.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://lu.panjiajie.cn

[Q19] 范围查询
来源：http://hk.shxzukj.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ew.shxzskj.cn

[Q20] IN 列表
来源：http://ia.bjjhwx.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://be.muxihuayi.cn

[Q21] 空值判断
来源：http://px.panjiajie.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://nw.szsharing.cn

[Q22] 排序
来源：http://yb.huanxung.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://jt.haigaiapp.cn

[Q23] 分页
来源：http://zr.nicolike.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://rr.shxzukj.cn

[Q24] 去重
来源：http://kt.521024.cn

SELECT DISTINCT city FROM users;
来源：http://fl.nicolike.cn

[Q25] 只取前 N 条
来源：http://of.nicolike.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ch.asd995.cn

[Q26] 计数
来源：http://jk.muxihuayi.cn

SELECT COUNT(*) FROM users;
来源：http://lp.wgjwhj.cn

[Q27] 条件计数
来源：http://pv.huanxung.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://qy.shtwfgs.cn

[Q28] 求和与平均
来源：http://uf.szsharing.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://en.huixiangedu.cn

[Q29] 最大最小值
来源：http://zw.nicolike.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://td.shxzskj.cn

[Q30] 分组统计
来源：http://qu.huixiangedu.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://tg.huixiangedu.cn

[Q31] 分组后过滤
来源：http://li.bookmarksfly.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://bh.lnxyls.cn

[Q32] 分组拼接字符串
来源：http://hv.huixiangedu.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://pv.gzmigu.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://uz.huanxung.cn

[Q33] 多列分组
来源：http://ac.colortex.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://gc.521024.cn

[Q34] 每组取第一条
来源：http://uo.gzmigu.cn

SELECT * FROM (
来源：http://ae.yuntaijiaju.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://xm.9csxet.cn

) t WHERE rn = 1;
来源：http://wi.gzmigu.cn

[Q35] 内连接
来源：http://gy.9csxet.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://yz.shtwfgs.cn

[Q36] 左连接
来源：http://wp.newstarts.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://xn.hahajie.cn

[Q37] 右连接
来源：http://zw.jianghongdianzi.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ja.gzmigu.cn

[Q38] 全外连接（PostgreSQL）
来源：http://hw.muxihuayi.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wz.chemitech.net.cn

[Q39] 自连接（查上下级）
来源：http://ye.wgjwhj.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://kz.jianghongdianzi.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://al.muxihuayi.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://xf.szsharing.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://dx.shxzukj.cn

[Q41] 多表连接
来源：http://nx.bjjhwx.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://xg.muxihuayi.cn

JOIN users u ON u.id = o.user_id
来源：http://an.huanxung.cn

JOIN products p ON p.id = o.product_id;
来源：http://wi.jctech888.com.cn

[Q42] 连接条件附加过滤
来源：http://yl.yuexingan06.cn

SELECT u.name, o.amount FROM users u
来源：http://kw.shxzskj.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://lr.szxytkj.cn

[Q43] 标量子查询
来源：http://wv.hahajie.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://jy.shxzukj.cn


<!-- 参考信息 -->