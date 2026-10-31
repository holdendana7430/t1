代发 wailian999

JS:   s === [...s].reverse().join("")
来源：http://pn.newstarts.cn

TS:   s === [...s].reverse().join("")
来源：http://yy.panjiajie.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://lx.521024.cn

Go:   // 双指针从两端比较
来源：http://zt.nicolike.cn

Ruby: s == s.reverse
来源：http://gf.huixinmuqiang.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://qw.yuntaijiaju.cn

[N07] 两数之和（返回下标）
来源：http://mb.bookmarksfly.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://vh.asd995.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://pn.jianghongdianzi.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://ab.lnxyls.cn

TS:   // 手写 Map<string, number>
来源：http://ke.wgjwhj.cn

Java: // 手写 HashMap
来源：http://hj.bookmarksfly.cn

Go:   // 手写 map[int]int
来源：http://wo.szxytkj.cn

Ruby: // 手写 Hash
来源：http://ip.bjjhwx.cn

C#:   // 手写 Dictionary<int, int>
来源：http://tb.yuexingan06.cn

[N08] 生成全排列
来源：http://eg.huanxung.cn

Py:   itertools.permutations(arr)
来源：http://yr.wgjwhj.cn

PHP:  // 手写递归交换
来源：http://ak.szxytkj.cn

JS:   // 手写回溯递归
来源：http://bh.yuexingan06.cn

TS:   // 手写回溯递归
来源：http://pb.jctech888.com.cn

Java: // 手写回溯递归
来源：http://tw.huanxung.cn

Go:   // 手写回溯递归
来源：http://ce.jianghongdianzi.cn

Ruby: arr.permutation.to_a
来源：http://xh.9csxet.cn

C#:   // 手写回溯递归
来源：http://zc.szxytkj.cn

[N09] 栈与队列
来源：http://bf.jctech888.com.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://py.hahajie.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://zp.panjiajie.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://xi.yuexingan06.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ly.shxzukj.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ro.gzmigu.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://on.jctech888.com.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://da.huanxung.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://cr.9csxet.cn

[N10] 链表节点定义
来源：http://pa.9csxet.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://kw.shxzukj.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://te.9csxet.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://yu.newstarts.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wh.colortex.cn

Java: class Node { int v; Node next; }
来源：http://oi.panjiajie.cn

Go:   type Node struct { V int; Next *Node }
来源：http://nz.shxzukj.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://cd.bookmarksfly.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://wp.bookmarksfly.cn

[N11] 二叉树中序遍历
来源：http://ey.panjiajie.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://uv.bookmarksfly.cn

PHP:  // 手写递归函数
来源：http://sb.szxytkj.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://yu.yuexingan06.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://lk.haigaiapp.cn

Java: // 手写递归
来源：http://le.yuexingan06.cn

Go:   // 手写递归
来源：http://qn.bjjhwx.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://iy.jctech888.com.cn

C#:   // 手写递归
来源：http://ku.9csxet.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://uu.521024.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://id.gzmigu.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://du.yuexingan06.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://jq.shtwfgs.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ah.yuntaijiaju.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hs.huixinmuqiang.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hh.521024.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://bn.gzmigu.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ip.chemitech.net.cn

================================================================================
来源：http://ui.521024.cn

O. 并发与异步
来源：http://ws.haigaiapp.cn

================================================================================
来源：http://cl.9csxet.cn

[O01] 启动一个线程
来源：http://xa.huixiangedu.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://dz.shtwfgs.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://lk.lnxyls.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://jn.huanxung.cn

TS:   // 同 JS
来源：http://tw.hnjuh.cn

Java: new Thread(() -> f()).start()
来源：http://fd.huanxung.cn

Go:   go f()
来源：http://ix.huixiangedu.cn

Ruby: Thread.new { f }
来源：http://yd.jianghongdianzi.cn

C#:   Task.Run(() => F());
来源：http://xg.asd995.cn

[O02] 使用线程池
来源：http://nx.jianghongdianzi.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ht.yuexingan06.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://vt.shxzskj.cn

JS:   // worker_threads 线程池
来源：http://sn.haigaiapp.cn

TS:   // worker_threads 线程池
来源：http://po.bookmarksfly.cn

Java: Executors.newFixedThreadPool(4)
来源：http://xo.szsharing.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hn.bjjhwx.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://cx.nicolike.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://dk.jianghongdianzi.cn

[O03] 加锁保护共享数据
来源：http://gq.asd995.cn

Py:   with lock: shared += 1
来源：http://dc.bjjhwx.cn

PHP:  // 用 flock() 做文件锁
来源：http://af.shxzukj.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://xi.shxzskj.cn

TS:   // 同 JS
来源：http://tr.nicolike.cn

Java: synchronized (this) { shared++; }
来源：http://yc.huixiangedu.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://gn.shtwfgs.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://eb.wgjwhj.cn

C#:   lock (gate) { shared++; }
来源：http://oq.gzmigu.cn

[O04] 定义异步函数并等待
来源：http://vm.yuntaijiaju.cn

Py:   async def f():⏎    await g()
来源：http://fx.lnxyls.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hs.huixiangedu.cn

JS:   async function f() { await g(); }
来源：http://dh.shxzukj.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://it.wgjwhj.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://kf.huixinmuqiang.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://nd.huixiangedu.cn

Ruby: # 用 Fiber 或 async gem
来源：http://fp.szsharing.cn

C#:   async Task F() { await G(); }
来源：http://qi.asd995.cn

[O05] 并发执行并等待全部完成
来源：http://gt.bookmarksfly.cn

Py:   asyncio.gather(*tasks)
来源：http://tl.huanxung.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://dx.huixiangedu.cn

JS:   await Promise.all(tasks)
来源：http://dr.hahajie.cn

TS:   await Promise.all(tasks)
来源：http://ac.wgjwhj.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://dz.bookmarksfly.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://rp.jctech888.com.cn

Ruby: threads.map(&:join)
来源：http://cn.wgjwhj.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://aj.nicolike.cn

[O06] 使用进程池
来源：http://cw.shxzskj.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://cs.jctech888.com.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://hs.szxytkj.cn

JS:   // child_process / cluster 模块
来源：http://cn.521024.cn

TS:   // child_process / cluster 模块
来源：http://mz.shxzskj.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ge.colortex.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://dp.colortex.cn

Ruby: // fork 块
来源：http://ji.bjjhwx.cn

C#:   Parallel.For
来源：http://ye.huanxung.cn

================================================================================
来源：http://xq.panjiajie.cn

P. 常用工具函数
来源：http://sz.9csxet.cn

================================================================================
来源：http://tp.szxytkj.cn

[P01] 生成 UUID
来源：http://kd.bookmarksfly.cn

Py:   str(uuid.uuid4())
来源：http://ae.jianghongdianzi.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://xg.newstarts.cn

JS:   crypto.randomUUID()
来源：http://cw.hnjuh.cn

TS:   crypto.randomUUID()
来源：http://bv.bjjhwx.cn

Java: UUID.randomUUID().toString()
来源：http://yb.huixiangedu.cn

Go:   // 用 github.com/google/uuid
来源：http://xw.haigaiapp.cn

Ruby: SecureRandom.uuid
来源：http://yq.521024.cn

C#:   Guid.NewGuid().ToString()
来源：http://si.jianghongdianzi.cn

[P02] MD5 / SHA256 摘要
来源：http://xt.nszjky.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://cl.panjiajie.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://wd.yuexingan06.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://vq.huixiangedu.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://qr.nicolike.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://jt.hahajie.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wl.asd995.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://kp.huanxung.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://yk.newstarts.cn

[P03] 生成短随机字符串
来源：http://gl.521024.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://jt.shxzskj.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://eb.521024.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://es.9csxet.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hy.huixinmuqiang.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://dr.wgjwhj.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://oj.lnxyls.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://gg.muxihuayi.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://uu.asd995.cn

[P04] 求长度
来源：http://op.panjiajie.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://dt.hnjuh.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mu.asd995.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://om.szxytkj.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ou.nicolike.cn

Java: list.size();  map.size();  s.length()
来源：http://lc.shxzukj.cn

Go:   len(arr);  len(m)
来源：http://om.wgjwhj.cn

Ruby: x.length;  x.size
来源：http://lz.hahajie.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://pc.nszjky.cn

[P05] 判断两个对象内容是否相等
来源：http://wk.shtwfgs.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://tp.gzmigu.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://qo.nicolike.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://cp.jctech888.com.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://fa.szxytkj.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://uh.panjiajie.cn

Go:   reflect.DeepEqual(a, b)
来源：http://tb.bookmarksfly.cn

Ruby: a == b
来源：http://ce.nszjky.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://xy.nszjky.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://zc.521024.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://yp.shxzskj.cn

PHP:  if (empty($x)) {}
来源：http://un.huanxung.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://fm.panjiajie.cn

TS:   if (x == null) {}
来源：http://tq.nszjky.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://zi.lnxyls.cn

Go:   if x == nil {}
来源：http://vn.huixiangedu.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://va.huanxung.cn

C#:   if (x is null) {}
来源：http://hy.gzmigu.cn

[P07] 防抖与节流
来源：http://zx.shtwfgs.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://pt.jctech888.com.cn

PHP:  // 手写时间戳比较
来源：http://td.nicolike.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://bk.bookmarksfly.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ha.yuntaijiaju.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://gu.chemitech.net.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://qw.newstarts.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://hp.panjiajie.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://vh.szxytkj.cn

[P08] 处理浮点精度问题
来源：http://gr.chemitech.net.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://lq.yuntaijiaju.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://qa.huixiangedu.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ze.asd995.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://oo.bjjhwx.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://xc.yuexingan06.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://dl.yuntaijiaju.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://rl.wgjwhj.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://yn.chemitech.net.cn

================================================================================
来源：http://jp.szsharing.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://nx.shtwfgs.cn

================================================================================
来源：http://gb.hnjuh.cn

[Q01] 创建表
来源：http://tl.521024.cn

CREATE TABLE users (
来源：http://ni.wgjwhj.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ab.yuntaijiaju.cn

name VARCHAR(50) NOT NULL,
来源：http://uw.szxytkj.cn

email VARCHAR(100) UNIQUE,
来源：http://tb.shtwfgs.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://nq.yuexingan06.cn

);
来源：http://nb.colortex.cn

[Q02] 创建带外键的表
来源：http://cb.newstarts.cn

CREATE TABLE orders (
来源：http://pi.wgjwhj.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://jb.panjiajie.cn

user_id INT NOT NULL,
来源：http://ta.shxzskj.cn

amount DECIMAL(10, 2),
来源：http://ju.yuntaijiaju.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ps.muxihuayi.cn

);
来源：http://hg.lnxyls.cn

[Q03] 增加列
来源：http://yy.panjiajie.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://zi.colortex.cn

[Q04] 修改列类型
来源：http://wp.huixiangedu.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://tk.shtwfgs.cn

[Q05] 重命名列
来源：http://iq.colortex.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ga.jctech888.com.cn

[Q06] 删除列
来源：http://dc.nszjky.cn

ALTER TABLE users DROP COLUMN age;
来源：http://za.hnjuh.cn

[Q07] 删除表
来源：http://tr.9csxet.cn

DROP TABLE IF EXISTS orders;
来源：http://ql.hnjuh.cn

[Q08] 创建普通索引
来源：http://fg.shxzskj.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://eh.hahajie.cn

[Q09] 创建唯一索引
来源：http://pm.lnxyls.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wg.szxytkj.cn

[Q10] 插入单行
来源：http://nc.haigaiapp.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://fr.yuntaijiaju.cn

[Q11] 一次插入多行
来源：http://tz.hahajie.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://cf.bjjhwx.cn

[Q12] 插入后取自增 ID
来源：http://hc.hahajie.cn

INSERT INTO users (name) VALUES ('C');
来源：http://es.shxzskj.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://kz.huixinmuqiang.cn

[Q13] 忽略重复插入
来源：http://ab.szsharing.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://zx.chemitech.net.cn

[Q14] 存在则更新（upsert）
来源：http://rt.nszjky.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://tt.chemitech.net.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://nf.lnxyls.cn

[Q15] 查询全部
来源：http://tw.haigaiapp.cn

SELECT * FROM users;
来源：http://ct.yuntaijiaju.cn

[Q16] 查询指定列
来源：http://fe.hnjuh.cn

SELECT id, name FROM users;
来源：http://qs.hnjuh.cn

[Q17] 条件查询
来源：http://pr.colortex.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://bb.wgjwhj.cn

[Q18] 模糊匹配
来源：http://li.muxihuayi.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ow.jctech888.com.cn

[Q19] 范围查询
来源：http://zl.panjiajie.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://gs.huixiangedu.cn

[Q20] IN 列表
来源：http://mb.newstarts.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ah.haigaiapp.cn

[Q21] 空值判断
来源：http://vh.huixinmuqiang.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://ok.9csxet.cn

[Q22] 排序
来源：http://os.lnxyls.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://td.shxzukj.cn

[Q23] 分页
来源：http://cu.chemitech.net.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://em.hahajie.cn

[Q24] 去重
来源：http://fa.wgjwhj.cn

SELECT DISTINCT city FROM users;
来源：http://je.newstarts.cn

[Q25] 只取前 N 条
来源：http://jw.szxytkj.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://oz.shxzskj.cn

[Q26] 计数
来源：http://fv.asd995.cn

SELECT COUNT(*) FROM users;
来源：http://xl.panjiajie.cn

[Q27] 条件计数
来源：http://ya.hahajie.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://qs.hahajie.cn

[Q28] 求和与平均
来源：http://lj.bjjhwx.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://ay.gzmigu.cn

[Q29] 最大最小值
来源：http://mw.gzmigu.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://kk.wgjwhj.cn

[Q30] 分组统计
来源：http://la.huixinmuqiang.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wr.gzmigu.cn

[Q31] 分组后过滤
来源：http://wr.hahajie.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wb.9csxet.cn

[Q32] 分组拼接字符串
来源：http://vz.wgjwhj.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://lb.wgjwhj.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wh.shtwfgs.cn

[Q33] 多列分组
来源：http://ei.newstarts.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://jp.shxzukj.cn

[Q34] 每组取第一条
来源：http://gh.haigaiapp.cn

SELECT * FROM (
来源：http://ae.shxzskj.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://tr.szxytkj.cn

) t WHERE rn = 1;
来源：http://zi.jianghongdianzi.cn

[Q35] 内连接
来源：http://fi.panjiajie.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://le.muxihuayi.cn

[Q36] 左连接
来源：http://cq.yuntaijiaju.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ds.lnxyls.cn

[Q37] 右连接
来源：http://mk.muxihuayi.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://rn.huixiangedu.cn

[Q38] 全外连接（PostgreSQL）
来源：http://rw.yuexingan06.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://tg.9csxet.cn

[Q39] 自连接（查上下级）
来源：http://pd.bookmarksfly.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://fd.nicolike.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://tt.yuntaijiaju.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://dr.jctech888.com.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://fu.shxzukj.cn

[Q41] 多表连接
来源：http://zc.huixiangedu.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://pd.colortex.cn

JOIN users u ON u.id = o.user_id
来源：http://wo.hahajie.cn

JOIN products p ON p.id = o.product_id;
来源：http://cx.haigaiapp.cn

[Q42] 连接条件附加过滤
来源：http://rc.gzmigu.cn

SELECT u.name, o.amount FROM users u
来源：http://yc.hahajie.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://kq.muxihuayi.cn

[Q43] 标量子查询
来源：http://jw.szxytkj.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://bf.szsharing.cn


<!-- 参考信息 -->