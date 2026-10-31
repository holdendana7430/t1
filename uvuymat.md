代发 wailian999

JS:   s === [...s].reverse().join("")
来源：http://hm.nszjky.cn

TS:   s === [...s].reverse().join("")
来源：http://fe.hnjuh.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://as.shxzukj.cn

Go:   // 双指针从两端比较
来源：http://yw.huanxung.cn

Ruby: s == s.reverse
来源：http://mv.huanxung.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://ii.nszjky.cn

[N07] 两数之和（返回下标）
来源：http://bl.newstarts.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://uc.yuntaijiaju.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ly.szsharing.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://wr.szxytkj.cn

TS:   // 手写 Map<string, number>
来源：http://zg.hnjuh.cn

Java: // 手写 HashMap
来源：http://ar.hnjuh.cn

Go:   // 手写 map[int]int
来源：http://qp.wgjwhj.cn

Ruby: // 手写 Hash
来源：http://kh.bjjhwx.cn

C#:   // 手写 Dictionary<int, int>
来源：http://wm.yuntaijiaju.cn

[N08] 生成全排列
来源：http://eb.szxytkj.cn

Py:   itertools.permutations(arr)
来源：http://bn.shxzukj.cn

PHP:  // 手写递归交换
来源：http://fi.521024.cn

JS:   // 手写回溯递归
来源：http://ur.nicolike.cn

TS:   // 手写回溯递归
来源：http://lv.lnxyls.cn

Java: // 手写回溯递归
来源：http://ay.shxzukj.cn

Go:   // 手写回溯递归
来源：http://ve.haigaiapp.cn

Ruby: arr.permutation.to_a
来源：http://tj.hnjuh.cn

C#:   // 手写回溯递归
来源：http://zk.colortex.cn

[N09] 栈与队列
来源：http://ys.bookmarksfly.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://iw.bjjhwx.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://pg.newstarts.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ad.asd995.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://bd.lnxyls.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://pg.newstarts.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://vw.9csxet.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ag.szxytkj.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hg.hahajie.cn

[N10] 链表节点定义
来源：http://uc.jianghongdianzi.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ur.huanxung.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://ls.9csxet.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://re.bookmarksfly.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://qw.521024.cn

Java: class Node { int v; Node next; }
来源：http://vi.gzmigu.cn

Go:   type Node struct { V int; Next *Node }
来源：http://kj.shxzskj.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://je.haigaiapp.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://ol.shtwfgs.cn

[N11] 二叉树中序遍历
来源：http://do.jctech888.com.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://bo.hahajie.cn

PHP:  // 手写递归函数
来源：http://da.newstarts.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://jy.huixinmuqiang.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://vf.521024.cn

Java: // 手写递归
来源：http://bd.bjjhwx.cn

Go:   // 手写递归
来源：http://ob.szxytkj.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ue.yuexingan06.cn

C#:   // 手写递归
来源：http://mt.521024.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://it.yuntaijiaju.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://cp.huixinmuqiang.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://fs.asd995.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://kc.shxzskj.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://kv.asd995.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://xl.szxytkj.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ac.szsharing.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://cc.bookmarksfly.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mb.muxihuayi.cn

================================================================================
来源：http://rz.colortex.cn

O. 并发与异步
来源：http://ym.shxzukj.cn

================================================================================
来源：http://id.asd995.cn

[O01] 启动一个线程
来源：http://tu.shxzskj.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hd.muxihuayi.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hp.colortex.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://fg.hnjuh.cn

TS:   // 同 JS
来源：http://nc.yuntaijiaju.cn

Java: new Thread(() -> f()).start()
来源：http://nd.bookmarksfly.cn

Go:   go f()
来源：http://dz.asd995.cn

Ruby: Thread.new { f }
来源：http://wo.521024.cn

C#:   Task.Run(() => F());
来源：http://ko.hnjuh.cn

[O02] 使用线程池
来源：http://rg.newstarts.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://bk.521024.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://vn.newstarts.cn

JS:   // worker_threads 线程池
来源：http://jr.shxzukj.cn

TS:   // worker_threads 线程池
来源：http://jr.hnjuh.cn

Java: Executors.newFixedThreadPool(4)
来源：http://pn.bookmarksfly.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://lh.colortex.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://tb.colortex.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://bn.hnjuh.cn

[O03] 加锁保护共享数据
来源：http://ea.521024.cn

Py:   with lock: shared += 1
来源：http://am.wgjwhj.cn

PHP:  // 用 flock() 做文件锁
来源：http://vz.shxzukj.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://jx.yuexingan06.cn

TS:   // 同 JS
来源：http://yb.szxytkj.cn

Java: synchronized (this) { shared++; }
来源：http://ak.huixiangedu.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wo.lnxyls.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://ue.asd995.cn

C#:   lock (gate) { shared++; }
来源：http://il.muxihuayi.cn

[O04] 定义异步函数并等待
来源：http://at.hahajie.cn

Py:   async def f():⏎    await g()
来源：http://pa.9csxet.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://rp.yuntaijiaju.cn

JS:   async function f() { await g(); }
来源：http://aj.shtwfgs.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://yg.asd995.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://de.shxzskj.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://uj.521024.cn

Ruby: # 用 Fiber 或 async gem
来源：http://vm.yuexingan06.cn

C#:   async Task F() { await G(); }
来源：http://rw.jianghongdianzi.cn

[O05] 并发执行并等待全部完成
来源：http://ue.yuexingan06.cn

Py:   asyncio.gather(*tasks)
来源：http://sb.huixinmuqiang.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://pa.shxzskj.cn

JS:   await Promise.all(tasks)
来源：http://co.gzmigu.cn

TS:   await Promise.all(tasks)
来源：http://tb.wgjwhj.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ed.haigaiapp.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://we.haigaiapp.cn

Ruby: threads.map(&:join)
来源：http://qx.hnjuh.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://dj.asd995.cn

[O06] 使用进程池
来源：http://ji.newstarts.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://nw.gzmigu.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://fb.gzmigu.cn

JS:   // child_process / cluster 模块
来源：http://ja.hnjuh.cn

TS:   // child_process / cluster 模块
来源：http://lq.bookmarksfly.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wb.shxzukj.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://yd.yuexingan06.cn

Ruby: // fork 块
来源：http://dq.nszjky.cn

C#:   Parallel.For
来源：http://hr.shxzskj.cn

================================================================================
来源：http://no.yuexingan06.cn

P. 常用工具函数
来源：http://ub.bjjhwx.cn

================================================================================
来源：http://uw.yuexingan06.cn

[P01] 生成 UUID
来源：http://ah.huixinmuqiang.cn

Py:   str(uuid.uuid4())
来源：http://ng.shxzskj.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://pq.jctech888.com.cn

JS:   crypto.randomUUID()
来源：http://qa.bjjhwx.cn

TS:   crypto.randomUUID()
来源：http://kf.colortex.cn

Java: UUID.randomUUID().toString()
来源：http://ab.hahajie.cn

Go:   // 用 github.com/google/uuid
来源：http://wi.shxzukj.cn

Ruby: SecureRandom.uuid
来源：http://zk.haigaiapp.cn

C#:   Guid.NewGuid().ToString()
来源：http://ml.hahajie.cn

[P02] MD5 / SHA256 摘要
来源：http://yq.hahajie.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ny.wgjwhj.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://uj.nszjky.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://rk.szxytkj.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mq.muxihuayi.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://pk.szsharing.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ts.shxzukj.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://yi.nszjky.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ng.muxihuayi.cn

[P03] 生成短随机字符串
来源：http://bs.chemitech.net.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://gj.yuexingan06.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ds.haigaiapp.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://cy.huanxung.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://db.nszjky.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wa.shxzukj.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://zr.shxzskj.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://qu.nszjky.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://qf.huixinmuqiang.cn

[P04] 求长度
来源：http://dg.lnxyls.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://tc.bjjhwx.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ef.chemitech.net.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://qx.lnxyls.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://og.nicolike.cn

Java: list.size();  map.size();  s.length()
来源：http://kw.colortex.cn

Go:   len(arr);  len(m)
来源：http://pa.chemitech.net.cn

Ruby: x.length;  x.size
来源：http://ms.shxzukj.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://xc.shxzukj.cn

[P05] 判断两个对象内容是否相等
来源：http://vp.jianghongdianzi.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://oi.yuntaijiaju.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://yq.hahajie.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://sg.huanxung.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://xz.muxihuayi.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://qq.szsharing.cn

Go:   reflect.DeepEqual(a, b)
来源：http://kd.panjiajie.cn

Ruby: a == b
来源：http://rn.bookmarksfly.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://rw.yuexingan06.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ae.bookmarksfly.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://md.muxihuayi.cn

PHP:  if (empty($x)) {}
来源：http://rj.shxzskj.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://gi.wgjwhj.cn

TS:   if (x == null) {}
来源：http://cm.huixiangedu.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://mi.chemitech.net.cn

Go:   if x == nil {}
来源：http://pr.chemitech.net.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ue.hahajie.cn

C#:   if (x is null) {}
来源：http://mu.jianghongdianzi.cn

[P07] 防抖与节流
来源：http://da.newstarts.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ne.jctech888.com.cn

PHP:  // 手写时间戳比较
来源：http://ig.yuntaijiaju.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ux.9csxet.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://uv.shtwfgs.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://so.asd995.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://lu.huixinmuqiang.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://yz.jctech888.com.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://oz.bjjhwx.cn

[P08] 处理浮点精度问题
来源：http://xf.gzmigu.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://oe.shtwfgs.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://bb.jctech888.com.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://kk.shtwfgs.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://pw.bjjhwx.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://br.9csxet.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://nx.szxytkj.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://sx.chemitech.net.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ev.yuexingan06.cn

================================================================================
来源：http://mu.yuexingan06.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ye.huixiangedu.cn

================================================================================
来源：http://lm.bjjhwx.cn

[Q01] 创建表
来源：http://lq.yuntaijiaju.cn

CREATE TABLE users (
来源：http://kj.newstarts.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://vq.colortex.cn

name VARCHAR(50) NOT NULL,
来源：http://jj.jctech888.com.cn

email VARCHAR(100) UNIQUE,
来源：http://gl.bjjhwx.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://us.szxytkj.cn

);
来源：http://yr.shxzskj.cn

[Q02] 创建带外键的表
来源：http://ua.muxihuayi.cn

CREATE TABLE orders (
来源：http://nc.colortex.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ry.newstarts.cn

user_id INT NOT NULL,
来源：http://ic.nszjky.cn

amount DECIMAL(10, 2),
来源：http://qg.shtwfgs.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ox.huixiangedu.cn

);
来源：http://zv.wgjwhj.cn

[Q03] 增加列
来源：http://hh.panjiajie.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://sh.gzmigu.cn

[Q04] 修改列类型
来源：http://oi.jianghongdianzi.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://jk.chemitech.net.cn

[Q05] 重命名列
来源：http://ux.muxihuayi.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wi.gzmigu.cn

[Q06] 删除列
来源：http://qt.huixiangedu.cn

ALTER TABLE users DROP COLUMN age;
来源：http://xb.shtwfgs.cn

[Q07] 删除表
来源：http://hv.yuntaijiaju.cn

DROP TABLE IF EXISTS orders;
来源：http://kj.newstarts.cn

[Q08] 创建普通索引
来源：http://xx.wgjwhj.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://zn.shtwfgs.cn

[Q09] 创建唯一索引
来源：http://fp.jianghongdianzi.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://vq.521024.cn

[Q10] 插入单行
来源：http://go.shxzukj.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://kt.hnjuh.cn

[Q11] 一次插入多行
来源：http://vl.wgjwhj.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wc.jianghongdianzi.cn

[Q12] 插入后取自增 ID
来源：http://fe.hnjuh.cn

INSERT INTO users (name) VALUES ('C');
来源：http://vp.shxzskj.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ok.lnxyls.cn

[Q13] 忽略重复插入
来源：http://ng.wgjwhj.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://pw.muxihuayi.cn

[Q14] 存在则更新（upsert）
来源：http://bj.szxytkj.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ky.yuexingan06.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wd.lnxyls.cn

[Q15] 查询全部
来源：http://jl.shxzskj.cn

SELECT * FROM users;
来源：http://dt.jctech888.com.cn

[Q16] 查询指定列
来源：http://ra.muxihuayi.cn

SELECT id, name FROM users;
来源：http://yq.haigaiapp.cn

[Q17] 条件查询
来源：http://xz.jianghongdianzi.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://lh.szxytkj.cn

[Q18] 模糊匹配
来源：http://de.nicolike.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://vj.chemitech.net.cn

[Q19] 范围查询
来源：http://zt.yuexingan06.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://cf.szxytkj.cn

[Q20] IN 列表
来源：http://os.huixinmuqiang.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://jp.panjiajie.cn

[Q21] 空值判断
来源：http://pz.jianghongdianzi.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://di.jianghongdianzi.cn

[Q22] 排序
来源：http://tt.shxzukj.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://tm.colortex.cn

[Q23] 分页
来源：http://jc.hahajie.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://qz.huixinmuqiang.cn

[Q24] 去重
来源：http://vw.shxzskj.cn

SELECT DISTINCT city FROM users;
来源：http://ux.nszjky.cn

[Q25] 只取前 N 条
来源：http://ny.gzmigu.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://dq.muxihuayi.cn

[Q26] 计数
来源：http://bx.shxzukj.cn

SELECT COUNT(*) FROM users;
来源：http://lw.haigaiapp.cn

[Q27] 条件计数
来源：http://ju.szxytkj.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://jr.yuntaijiaju.cn

[Q28] 求和与平均
来源：http://su.jianghongdianzi.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://lt.shxzskj.cn

[Q29] 最大最小值
来源：http://ay.colortex.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://wz.jctech888.com.cn

[Q30] 分组统计
来源：http://nd.hahajie.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://yy.jctech888.com.cn

[Q31] 分组后过滤
来源：http://zh.yuexingan06.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://su.bjjhwx.cn

[Q32] 分组拼接字符串
来源：http://ky.yuntaijiaju.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://lb.panjiajie.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://oi.hahajie.cn

[Q33] 多列分组
来源：http://zt.chemitech.net.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ap.colortex.cn

[Q34] 每组取第一条
来源：http://kz.huixiangedu.cn

SELECT * FROM (
来源：http://oh.shxzukj.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://fb.huixiangedu.cn

) t WHERE rn = 1;
来源：http://xc.gzmigu.cn

[Q35] 内连接
来源：http://te.panjiajie.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://xr.nszjky.cn

[Q36] 左连接
来源：http://tu.shtwfgs.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ko.szsharing.cn

[Q37] 右连接
来源：http://ez.bjjhwx.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://rn.bjjhwx.cn

[Q38] 全外连接（PostgreSQL）
来源：http://lt.nicolike.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://nx.colortex.cn

[Q39] 自连接（查上下级）
来源：http://su.wgjwhj.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://ma.shxzukj.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://gj.haigaiapp.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://ky.asd995.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wu.nicolike.cn

[Q41] 多表连接
来源：http://td.huixiangedu.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://ed.jianghongdianzi.cn

JOIN users u ON u.id = o.user_id
来源：http://xx.shxzukj.cn

JOIN products p ON p.id = o.product_id;
来源：http://hz.szxytkj.cn

[Q42] 连接条件附加过滤
来源：http://sp.hnjuh.cn

SELECT u.name, o.amount FROM users u
来源：http://mh.huixiangedu.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mo.yuexingan06.cn

[Q43] 标量子查询
来源：http://ra.panjiajie.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://md.haigaiapp.cn


<!-- 参考信息 -->