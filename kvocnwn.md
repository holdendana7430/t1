代发 wailian999

JS:   s === [...s].reverse().join("")
来源：http://rc.gzmigu.cn

TS:   s === [...s].reverse().join("")
来源：http://vn.wgjwhj.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ob.nicolike.cn

Go:   // 双指针从两端比较
来源：http://lp.gzmigu.cn

Ruby: s == s.reverse
来源：http://mz.521024.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://uu.bjjhwx.cn

[N07] 两数之和（返回下标）
来源：http://ai.newstarts.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ew.muxihuayi.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hr.hnjuh.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://gc.hahajie.cn

TS:   // 手写 Map<string, number>
来源：http://ac.huixiangedu.cn

Java: // 手写 HashMap
来源：http://my.jianghongdianzi.cn

Go:   // 手写 map[int]int
来源：http://pi.jianghongdianzi.cn

Ruby: // 手写 Hash
来源：http://kw.521024.cn

C#:   // 手写 Dictionary<int, int>
来源：http://ki.yuexingan06.cn

[N08] 生成全排列
来源：http://ly.lnxyls.cn

Py:   itertools.permutations(arr)
来源：http://px.shxzskj.cn

PHP:  // 手写递归交换
来源：http://bh.szxytkj.cn

JS:   // 手写回溯递归
来源：http://kj.9csxet.cn

TS:   // 手写回溯递归
来源：http://rk.yuexingan06.cn

Java: // 手写回溯递归
来源：http://qd.hnjuh.cn

Go:   // 手写回溯递归
来源：http://qw.huixiangedu.cn

Ruby: arr.permutation.to_a
来源：http://zg.nicolike.cn

C#:   // 手写回溯递归
来源：http://hd.panjiajie.cn

[N09] 栈与队列
来源：http://km.panjiajie.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://zo.bookmarksfly.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://nk.muxihuayi.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://oi.huixinmuqiang.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://lu.huixinmuqiang.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://cy.bjjhwx.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://fd.hnjuh.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://av.huanxung.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://fa.panjiajie.cn

[N10] 链表节点定义
来源：http://fh.shxzukj.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ho.bookmarksfly.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://cd.bjjhwx.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ho.szsharing.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://vt.shxzskj.cn

Java: class Node { int v; Node next; }
来源：http://cw.huanxung.cn

Go:   type Node struct { V int; Next *Node }
来源：http://nx.wgjwhj.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://zt.nicolike.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://ni.lnxyls.cn

[N11] 二叉树中序遍历
来源：http://yq.huixinmuqiang.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://jw.huixinmuqiang.cn

PHP:  // 手写递归函数
来源：http://hu.huanxung.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://zm.bjjhwx.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://uo.muxihuayi.cn

Java: // 手写递归
来源：http://fm.nicolike.cn

Go:   // 手写递归
来源：http://vk.yuexingan06.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://pl.huixinmuqiang.cn

C#:   // 手写递归
来源：http://li.hahajie.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://lc.huixiangedu.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://kw.521024.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ih.jianghongdianzi.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://lt.szsharing.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://bf.huanxung.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hv.yuntaijiaju.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ig.asd995.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ad.521024.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://yr.newstarts.cn

================================================================================
来源：http://rq.asd995.cn

O. 并发与异步
来源：http://xc.yuexingan06.cn

================================================================================
来源：http://us.szsharing.cn

[O01] 启动一个线程
来源：http://vl.asd995.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://if.bookmarksfly.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://uo.nicolike.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://gj.wgjwhj.cn

TS:   // 同 JS
来源：http://zr.bjjhwx.cn

Java: new Thread(() -> f()).start()
来源：http://sd.szsharing.cn

Go:   go f()
来源：http://zy.huixiangedu.cn

Ruby: Thread.new { f }
来源：http://te.lnxyls.cn

C#:   Task.Run(() => F());
来源：http://fb.lnxyls.cn

[O02] 使用线程池
来源：http://pu.bookmarksfly.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://xf.huanxung.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://rk.muxihuayi.cn

JS:   // worker_threads 线程池
来源：http://di.hnjuh.cn

TS:   // worker_threads 线程池
来源：http://wt.wgjwhj.cn

Java: Executors.newFixedThreadPool(4)
来源：http://nf.bookmarksfly.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ak.muxihuayi.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://eq.hahajie.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mp.colortex.cn

[O03] 加锁保护共享数据
来源：http://gw.9csxet.cn

Py:   with lock: shared += 1
来源：http://cj.bookmarksfly.cn

PHP:  // 用 flock() 做文件锁
来源：http://fr.bookmarksfly.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://sr.shtwfgs.cn

TS:   // 同 JS
来源：http://pw.asd995.cn

Java: synchronized (this) { shared++; }
来源：http://pp.yuexingan06.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://rp.shxzskj.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://es.szxytkj.cn

C#:   lock (gate) { shared++; }
来源：http://zm.521024.cn

[O04] 定义异步函数并等待
来源：http://ws.yuntaijiaju.cn

Py:   async def f():⏎    await g()
来源：http://is.gzmigu.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://bi.yuexingan06.cn

JS:   async function f() { await g(); }
来源：http://vg.gzmigu.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://cu.wgjwhj.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://zm.shxzskj.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://iz.yuexingan06.cn

Ruby: # 用 Fiber 或 async gem
来源：http://iz.asd995.cn

C#:   async Task F() { await G(); }
来源：http://jp.9csxet.cn

[O05] 并发执行并等待全部完成
来源：http://pz.nicolike.cn

Py:   asyncio.gather(*tasks)
来源：http://mq.521024.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://qf.shxzskj.cn

JS:   await Promise.all(tasks)
来源：http://wt.shtwfgs.cn

TS:   await Promise.all(tasks)
来源：http://oq.huixiangedu.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://rf.chemitech.net.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://it.huixiangedu.cn

Ruby: threads.map(&:join)
来源：http://we.nicolike.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://ht.nszjky.cn

[O06] 使用进程池
来源：http://rj.jctech888.com.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mo.shxzskj.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://pi.hnjuh.cn

JS:   // child_process / cluster 模块
来源：http://ys.chemitech.net.cn

TS:   // child_process / cluster 模块
来源：http://dh.huanxung.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://uh.shtwfgs.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://kl.huixiangedu.cn

Ruby: // fork 块
来源：http://mg.muxihuayi.cn

C#:   Parallel.For
来源：http://tp.521024.cn

================================================================================
来源：http://ig.szsharing.cn

P. 常用工具函数
来源：http://cw.panjiajie.cn

================================================================================
来源：http://zc.chemitech.net.cn

[P01] 生成 UUID
来源：http://bw.hnjuh.cn

Py:   str(uuid.uuid4())
来源：http://dh.muxihuayi.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://od.yuexingan06.cn

JS:   crypto.randomUUID()
来源：http://dv.huixiangedu.cn

TS:   crypto.randomUUID()
来源：http://oo.haigaiapp.cn

Java: UUID.randomUUID().toString()
来源：http://gn.chemitech.net.cn

Go:   // 用 github.com/google/uuid
来源：http://in.jctech888.com.cn

Ruby: SecureRandom.uuid
来源：http://af.lnxyls.cn

C#:   Guid.NewGuid().ToString()
来源：http://wf.panjiajie.cn

[P02] MD5 / SHA256 摘要
来源：http://bd.szsharing.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://gu.gzmigu.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://zu.huixinmuqiang.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mm.gzmigu.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ua.chemitech.net.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://bl.gzmigu.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://xq.nszjky.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://cc.nszjky.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://uv.shtwfgs.cn

[P03] 生成短随机字符串
来源：http://cp.jctech888.com.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://su.colortex.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://xv.jctech888.com.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://fv.lnxyls.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://jg.jianghongdianzi.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mo.gzmigu.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ct.shxzskj.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://un.hahajie.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ma.bookmarksfly.cn

[P04] 求长度
来源：http://qs.bjjhwx.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://zy.bjjhwx.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://od.nszjky.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://gw.lnxyls.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://qx.wgjwhj.cn

Java: list.size();  map.size();  s.length()
来源：http://vr.yuexingan06.cn

Go:   len(arr);  len(m)
来源：http://yh.shxzskj.cn

Ruby: x.length;  x.size
来源：http://es.chemitech.net.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://ax.yuexingan06.cn

[P05] 判断两个对象内容是否相等
来源：http://zs.huixiangedu.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://gs.bjjhwx.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://jj.wgjwhj.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://za.panjiajie.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://rz.9csxet.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://iq.9csxet.cn

Go:   reflect.DeepEqual(a, b)
来源：http://wy.colortex.cn

Ruby: a == b
来源：http://dl.lnxyls.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://un.hahajie.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://dx.nszjky.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ng.yuexingan06.cn

PHP:  if (empty($x)) {}
来源：http://si.szsharing.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://es.muxihuayi.cn

TS:   if (x == null) {}
来源：http://xp.yuexingan06.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://fd.bookmarksfly.cn

Go:   if x == nil {}
来源：http://sb.muxihuayi.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://xm.newstarts.cn

C#:   if (x is null) {}
来源：http://lu.shxzukj.cn

[P07] 防抖与节流
来源：http://xt.nszjky.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://nk.asd995.cn

PHP:  // 手写时间戳比较
来源：http://wi.lnxyls.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://nu.gzmigu.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://yu.shxzskj.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://rf.shxzukj.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://lt.shxzukj.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://zw.panjiajie.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hb.yuexingan06.cn

[P08] 处理浮点精度问题
来源：http://jw.newstarts.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://nl.lnxyls.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://zh.colortex.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://gh.huixinmuqiang.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://dw.chemitech.net.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://cj.huixiangedu.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wy.shxzukj.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://pg.yuntaijiaju.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://fw.hahajie.cn

================================================================================
来源：http://dt.jianghongdianzi.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hh.shxzskj.cn

================================================================================
来源：http://mx.nicolike.cn

[Q01] 创建表
来源：http://dv.chemitech.net.cn

CREATE TABLE users (
来源：http://wr.chemitech.net.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://qn.szxytkj.cn

name VARCHAR(50) NOT NULL,
来源：http://io.jctech888.com.cn

email VARCHAR(100) UNIQUE,
来源：http://hx.shtwfgs.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ry.chemitech.net.cn

);
来源：http://ut.bookmarksfly.cn

[Q02] 创建带外键的表
来源：http://aw.gzmigu.cn

CREATE TABLE orders (
来源：http://pg.9csxet.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mv.gzmigu.cn

user_id INT NOT NULL,
来源：http://wd.lnxyls.cn

amount DECIMAL(10, 2),
来源：http://hy.bjjhwx.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://lu.9csxet.cn

);
来源：http://fj.muxihuayi.cn

[Q03] 增加列
来源：http://mw.nszjky.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://gt.shtwfgs.cn

[Q04] 修改列类型
来源：http://fl.yuntaijiaju.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://bx.bookmarksfly.cn

[Q05] 重命名列
来源：http://ac.colortex.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://fu.chemitech.net.cn

[Q06] 删除列
来源：http://qc.9csxet.cn

ALTER TABLE users DROP COLUMN age;
来源：http://sb.colortex.cn

[Q07] 删除表
来源：http://vy.521024.cn

DROP TABLE IF EXISTS orders;
来源：http://uy.shxzukj.cn

[Q08] 创建普通索引
来源：http://kr.hahajie.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://zy.hahajie.cn

[Q09] 创建唯一索引
来源：http://zx.9csxet.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ko.nszjky.cn

[Q10] 插入单行
来源：http://fe.nicolike.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://bi.asd995.cn

[Q11] 一次插入多行
来源：http://ys.asd995.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ev.muxihuayi.cn

[Q12] 插入后取自增 ID
来源：http://ky.shtwfgs.cn

INSERT INTO users (name) VALUES ('C');
来源：http://sg.huixiangedu.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wx.asd995.cn

[Q13] 忽略重复插入
来源：http://df.bjjhwx.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://lg.lnxyls.cn

[Q14] 存在则更新（upsert）
来源：http://fu.muxihuayi.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ak.yuexingan06.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://vi.muxihuayi.cn

[Q15] 查询全部
来源：http://yf.jianghongdianzi.cn

SELECT * FROM users;
来源：http://xc.haigaiapp.cn

[Q16] 查询指定列
来源：http://aw.szxytkj.cn

SELECT id, name FROM users;
来源：http://jb.yuexingan06.cn

[Q17] 条件查询
来源：http://nj.shtwfgs.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://zd.9csxet.cn

[Q18] 模糊匹配
来源：http://re.chemitech.net.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://yo.asd995.cn

[Q19] 范围查询
来源：http://qn.asd995.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hl.nicolike.cn

[Q20] IN 列表
来源：http://on.9csxet.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://sl.szxytkj.cn

[Q21] 空值判断
来源：http://gz.jianghongdianzi.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://su.yuntaijiaju.cn

[Q22] 排序
来源：http://hq.yuntaijiaju.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ot.bookmarksfly.cn

[Q23] 分页
来源：http://ss.yuntaijiaju.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mc.yuexingan06.cn

[Q24] 去重
来源：http://pa.wgjwhj.cn

SELECT DISTINCT city FROM users;
来源：http://qm.shtwfgs.cn

[Q25] 只取前 N 条
来源：http://sa.chemitech.net.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ey.shxzukj.cn

[Q26] 计数
来源：http://fd.521024.cn

SELECT COUNT(*) FROM users;
来源：http://ki.haigaiapp.cn

[Q27] 条件计数
来源：http://yv.colortex.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://eg.yuexingan06.cn

[Q28] 求和与平均
来源：http://ep.muxihuayi.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://jq.bookmarksfly.cn

[Q29] 最大最小值
来源：http://pu.shxzukj.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://lc.szxytkj.cn

[Q30] 分组统计
来源：http://ve.bjjhwx.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://tb.haigaiapp.cn

[Q31] 分组后过滤
来源：http://us.yuntaijiaju.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ld.chemitech.net.cn

[Q32] 分组拼接字符串
来源：http://be.lnxyls.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://lv.huixiangedu.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://tu.huanxung.cn

[Q33] 多列分组
来源：http://wg.asd995.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://zt.bookmarksfly.cn

[Q34] 每组取第一条
来源：http://uy.yuexingan06.cn

SELECT * FROM (
来源：http://xw.huanxung.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://xe.hnjuh.cn

) t WHERE rn = 1;
来源：http://kz.huixiangedu.cn

[Q35] 内连接
来源：http://km.nszjky.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://qh.haigaiapp.cn

[Q36] 左连接
来源：http://ka.shxzskj.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://nz.hahajie.cn

[Q37] 右连接
来源：http://zz.szsharing.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://fd.szxytkj.cn

[Q38] 全外连接（PostgreSQL）
来源：http://do.colortex.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://bf.shxzskj.cn

[Q39] 自连接（查上下级）
来源：http://qw.bjjhwx.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://cq.huixinmuqiang.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://qq.jctech888.com.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://hb.yuexingan06.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ef.wgjwhj.cn

[Q41] 多表连接
来源：http://bm.chemitech.net.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://gy.huixinmuqiang.cn

JOIN users u ON u.id = o.user_id
来源：http://kj.huanxung.cn

JOIN products p ON p.id = o.product_id;
来源：http://ym.bookmarksfly.cn

[Q42] 连接条件附加过滤
来源：http://qb.yuntaijiaju.cn

SELECT u.name, o.amount FROM users u
来源：http://ix.huanxung.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://tp.shtwfgs.cn

[Q43] 标量子查询
来源：http://mi.nicolike.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://yh.newstarts.cn


<!-- 参考信息 -->