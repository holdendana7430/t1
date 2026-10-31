代发 wailian999

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://pw.jianghongdianzi.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://la.yuntaijiaju.cn

TS:   // 手写 Map<string, number>
来源：http://kh.newstarts.cn

Java: // 手写 HashMap
来源：http://xp.yuexingan06.cn

Go:   // 手写 map[int]int
来源：http://qa.wgjwhj.cn

Ruby: // 手写 Hash
来源：http://jv.jianghongdianzi.cn

C#:   // 手写 Dictionary<int, int>
来源：http://db.yuexingan06.cn

[N08] 生成全排列
来源：http://me.nicolike.cn

Py:   itertools.permutations(arr)
来源：http://pq.lnxyls.cn

PHP:  // 手写递归交换
来源：http://ki.haigaiapp.cn

JS:   // 手写回溯递归
来源：http://te.yuntaijiaju.cn

TS:   // 手写回溯递归
来源：http://fr.shtwfgs.cn

Java: // 手写回溯递归
来源：http://wc.nszjky.cn

Go:   // 手写回溯递归
来源：http://wx.asd995.cn

Ruby: arr.permutation.to_a
来源：http://zl.haigaiapp.cn

C#:   // 手写回溯递归
来源：http://xq.yuexingan06.cn

[N09] 栈与队列
来源：http://nx.szxytkj.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ct.bjjhwx.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://fq.jianghongdianzi.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://if.bookmarksfly.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://na.muxihuayi.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wn.jianghongdianzi.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://om.newstarts.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://jy.haigaiapp.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://oh.huixiangedu.cn

[N10] 链表节点定义
来源：http://ss.huanxung.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://pw.yuntaijiaju.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://nn.hahajie.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://rx.newstarts.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://cz.yuexingan06.cn

Java: class Node { int v; Node next; }
来源：http://jj.panjiajie.cn

Go:   type Node struct { V int; Next *Node }
来源：http://hn.bookmarksfly.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://cw.yuntaijiaju.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://jf.lnxyls.cn

[N11] 二叉树中序遍历
来源：http://rc.yuntaijiaju.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://tw.shxzskj.cn

PHP:  // 手写递归函数
来源：http://uo.jianghongdianzi.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://vw.szxytkj.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://vk.yuntaijiaju.cn

Java: // 手写递归
来源：http://dh.huixiangedu.cn

Go:   // 手写递归
来源：http://mj.yuexingan06.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://dc.shxzskj.cn

C#:   // 手写递归
来源：http://mm.szxytkj.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://yi.chemitech.net.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://yz.bookmarksfly.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ec.lnxyls.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://zo.newstarts.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://cl.szxytkj.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://we.521024.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://cb.newstarts.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://yl.nszjky.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://yo.hnjuh.cn

================================================================================
来源：http://vg.huixiangedu.cn

O. 并发与异步
来源：http://sx.hnjuh.cn

================================================================================
来源：http://sr.muxihuayi.cn

[O01] 启动一个线程
来源：http://es.panjiajie.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://gg.nicolike.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wu.shxzskj.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://li.yuntaijiaju.cn

TS:   // 同 JS
来源：http://bp.huanxung.cn

Java: new Thread(() -> f()).start()
来源：http://he.colortex.cn

Go:   go f()
来源：http://ya.shxzskj.cn

Ruby: Thread.new { f }
来源：http://ry.huixiangedu.cn

C#:   Task.Run(() => F());
来源：http://sh.bookmarksfly.cn

[O02] 使用线程池
来源：http://cu.shxzskj.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://yn.nicolike.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://uc.wgjwhj.cn

JS:   // worker_threads 线程池
来源：http://xd.asd995.cn

TS:   // worker_threads 线程池
来源：http://ue.hnjuh.cn

Java: Executors.newFixedThreadPool(4)
来源：http://ai.szxytkj.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://tl.szxytkj.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://nx.gzmigu.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://xd.colortex.cn

[O03] 加锁保护共享数据
来源：http://bf.wgjwhj.cn

Py:   with lock: shared += 1
来源：http://md.bookmarksfly.cn

PHP:  // 用 flock() 做文件锁
来源：http://cv.asd995.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://uq.huixinmuqiang.cn

TS:   // 同 JS
来源：http://fz.bjjhwx.cn

Java: synchronized (this) { shared++; }
来源：http://ec.huixiangedu.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://pj.9csxet.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://ps.hnjuh.cn

C#:   lock (gate) { shared++; }
来源：http://ss.bjjhwx.cn

[O04] 定义异步函数并等待
来源：http://na.panjiajie.cn

Py:   async def f():⏎    await g()
来源：http://ge.wgjwhj.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://jr.lnxyls.cn

JS:   async function f() { await g(); }
来源：http://mw.yuntaijiaju.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://su.lnxyls.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mp.521024.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://vo.hahajie.cn

Ruby: # 用 Fiber 或 async gem
来源：http://tl.hnjuh.cn

C#:   async Task F() { await G(); }
来源：http://tz.lnxyls.cn

[O05] 并发执行并等待全部完成
来源：http://ls.chemitech.net.cn

Py:   asyncio.gather(*tasks)
来源：http://fv.huanxung.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://rm.newstarts.cn

JS:   await Promise.all(tasks)
来源：http://yg.colortex.cn

TS:   await Promise.all(tasks)
来源：http://oy.jctech888.com.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://jy.huanxung.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://cv.hnjuh.cn

Ruby: threads.map(&:join)
来源：http://ce.bookmarksfly.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://mk.szxytkj.cn

[O06] 使用进程池
来源：http://us.huanxung.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mw.521024.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://wu.szxytkj.cn

JS:   // child_process / cluster 模块
来源：http://wx.szsharing.cn

TS:   // child_process / cluster 模块
来源：http://ku.lnxyls.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://yg.9csxet.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ba.chemitech.net.cn

Ruby: // fork 块
来源：http://mb.haigaiapp.cn

C#:   Parallel.For
来源：http://eg.nszjky.cn

================================================================================
来源：http://ll.9csxet.cn

P. 常用工具函数
来源：http://xx.szxytkj.cn

================================================================================
来源：http://nl.gzmigu.cn

[P01] 生成 UUID
来源：http://tf.hahajie.cn

Py:   str(uuid.uuid4())
来源：http://ab.521024.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://xi.szsharing.cn

JS:   crypto.randomUUID()
来源：http://qc.colortex.cn

TS:   crypto.randomUUID()
来源：http://ux.szsharing.cn

Java: UUID.randomUUID().toString()
来源：http://pw.9csxet.cn

Go:   // 用 github.com/google/uuid
来源：http://uf.muxihuayi.cn

Ruby: SecureRandom.uuid
来源：http://gd.szsharing.cn

C#:   Guid.NewGuid().ToString()
来源：http://cf.panjiajie.cn

[P02] MD5 / SHA256 摘要
来源：http://dd.huixiangedu.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://vx.szsharing.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://km.gzmigu.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mc.muxihuayi.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ok.nicolike.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://uw.jctech888.com.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://fb.szxytkj.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://de.szsharing.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://oq.huanxung.cn

[P03] 生成短随机字符串
来源：http://si.newstarts.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://iv.huixiangedu.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://kq.panjiajie.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://pl.nicolike.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://jk.huixiangedu.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://qb.chemitech.net.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ml.asd995.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://gm.bjjhwx.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://gc.huixinmuqiang.cn

[P04] 求长度
来源：http://un.lnxyls.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://iw.jctech888.com.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hi.szxytkj.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wm.shxzskj.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://cl.shxzskj.cn

Java: list.size();  map.size();  s.length()
来源：http://jf.huanxung.cn

Go:   len(arr);  len(m)
来源：http://ma.colortex.cn

Ruby: x.length;  x.size
来源：http://zn.nicolike.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://ot.9csxet.cn

[P05] 判断两个对象内容是否相等
来源：http://cm.newstarts.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://yy.huixinmuqiang.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://bl.gzmigu.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://yl.shxzukj.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mc.yuexingan06.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ll.chemitech.net.cn

Go:   reflect.DeepEqual(a, b)
来源：http://zz.hnjuh.cn

Ruby: a == b
来源：http://il.shxzukj.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ac.huixinmuqiang.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ym.yuexingan06.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://dc.huixiangedu.cn

PHP:  if (empty($x)) {}
来源：http://xv.huixiangedu.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://kh.szsharing.cn

TS:   if (x == null) {}
来源：http://av.huixiangedu.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://bq.jctech888.com.cn

Go:   if x == nil {}
来源：http://oz.nszjky.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://qt.nszjky.cn

C#:   if (x is null) {}
来源：http://ih.yuntaijiaju.cn

[P07] 防抖与节流
来源：http://io.shxzskj.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://xm.jctech888.com.cn

PHP:  // 手写时间戳比较
来源：http://ib.lnxyls.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://po.bjjhwx.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://tr.colortex.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hn.huixinmuqiang.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://dy.nszjky.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://az.huixinmuqiang.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://lv.jctech888.com.cn

[P08] 处理浮点精度问题
来源：http://wz.521024.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://vk.haigaiapp.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://em.panjiajie.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ex.jianghongdianzi.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://gk.shxzskj.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://bk.shtwfgs.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://sk.yuexingan06.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mg.521024.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://fq.szxytkj.cn

================================================================================
来源：http://ts.muxihuayi.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://lt.huixiangedu.cn

================================================================================
来源：http://ic.hahajie.cn

[Q01] 创建表
来源：http://wm.muxihuayi.cn

CREATE TABLE users (
来源：http://un.huixiangedu.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://fs.jctech888.com.cn

name VARCHAR(50) NOT NULL,
来源：http://uv.asd995.cn

email VARCHAR(100) UNIQUE,
来源：http://we.huixinmuqiang.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://xj.shxzskj.cn

);
来源：http://hr.hnjuh.cn

[Q02] 创建带外键的表
来源：http://jh.bookmarksfly.cn

CREATE TABLE orders (
来源：http://qw.nszjky.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wc.haigaiapp.cn

user_id INT NOT NULL,
来源：http://th.muxihuayi.cn

amount DECIMAL(10, 2),
来源：http://df.nszjky.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://iz.szxytkj.cn

);
来源：http://tp.shxzskj.cn

[Q03] 增加列
来源：http://of.nicolike.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://zx.bjjhwx.cn

[Q04] 修改列类型
来源：http://ki.shtwfgs.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://jr.jianghongdianzi.cn

[Q05] 重命名列
来源：http://ct.yuexingan06.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://et.colortex.cn

[Q06] 删除列
来源：http://sm.chemitech.net.cn

ALTER TABLE users DROP COLUMN age;
来源：http://ef.hnjuh.cn

[Q07] 删除表
来源：http://wb.lnxyls.cn

DROP TABLE IF EXISTS orders;
来源：http://cv.asd995.cn

[Q08] 创建普通索引
来源：http://bp.colortex.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://fp.9csxet.cn

[Q09] 创建唯一索引
来源：http://gw.colortex.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ve.muxihuayi.cn

[Q10] 插入单行
来源：http://ep.yuntaijiaju.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://qg.521024.cn

[Q11] 一次插入多行
来源：http://ds.wgjwhj.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://eq.jianghongdianzi.cn

[Q12] 插入后取自增 ID
来源：http://gt.jctech888.com.cn

INSERT INTO users (name) VALUES ('C');
来源：http://gg.yuntaijiaju.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ir.jianghongdianzi.cn

[Q13] 忽略重复插入
来源：http://aj.shxzukj.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://dl.yuexingan06.cn

[Q14] 存在则更新（upsert）
来源：http://wi.shxzskj.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://td.bjjhwx.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://xk.haigaiapp.cn

[Q15] 查询全部
来源：http://wp.colortex.cn

SELECT * FROM users;
来源：http://zn.shxzskj.cn

[Q16] 查询指定列
来源：http://lq.newstarts.cn

SELECT id, name FROM users;
来源：http://el.chemitech.net.cn

[Q17] 条件查询
来源：http://ld.jianghongdianzi.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://fj.jctech888.com.cn

[Q18] 模糊匹配
来源：http://ks.asd995.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mp.bjjhwx.cn

[Q19] 范围查询
来源：http://jn.shxzskj.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://yd.szsharing.cn

[Q20] IN 列表
来源：http://pl.muxihuayi.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://nn.panjiajie.cn

[Q21] 空值判断
来源：http://as.huanxung.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://hh.huixinmuqiang.cn

[Q22] 排序
来源：http://ul.huixinmuqiang.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://sn.szsharing.cn

[Q23] 分页
来源：http://mk.muxihuayi.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ep.jctech888.com.cn

[Q24] 去重
来源：http://cx.wgjwhj.cn

SELECT DISTINCT city FROM users;
来源：http://md.shxzukj.cn

[Q25] 只取前 N 条
来源：http://oy.shtwfgs.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ia.hnjuh.cn

[Q26] 计数
来源：http://bp.jianghongdianzi.cn

SELECT COUNT(*) FROM users;
来源：http://vw.hahajie.cn

[Q27] 条件计数
来源：http://rl.jctech888.com.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ss.colortex.cn

[Q28] 求和与平均
来源：http://my.gzmigu.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://yr.shxzukj.cn

[Q29] 最大最小值
来源：http://od.yuexingan06.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://xa.hahajie.cn

[Q30] 分组统计
来源：http://iw.wgjwhj.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://qj.muxihuayi.cn

[Q31] 分组后过滤
来源：http://ag.huanxung.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://sx.bjjhwx.cn

[Q32] 分组拼接字符串
来源：http://dn.9csxet.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://da.gzmigu.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ka.huixinmuqiang.cn

[Q33] 多列分组
来源：http://ua.muxihuayi.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://gx.shtwfgs.cn

[Q34] 每组取第一条
来源：http://ix.szxytkj.cn

SELECT * FROM (
来源：http://kr.chemitech.net.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://gv.huanxung.cn

) t WHERE rn = 1;
来源：http://uc.asd995.cn

[Q35] 内连接
来源：http://ol.bookmarksfly.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ud.yuntaijiaju.cn

[Q36] 左连接
来源：http://hu.hahajie.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ap.hahajie.cn

[Q37] 右连接
来源：http://wj.jianghongdianzi.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mc.9csxet.cn

[Q38] 全外连接（PostgreSQL）
来源：http://ds.szxytkj.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://bf.huixiangedu.cn

[Q39] 自连接（查上下级）
来源：http://ub.yuexingan06.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://lw.gzmigu.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://vj.jianghongdianzi.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://dx.wgjwhj.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ce.jianghongdianzi.cn

[Q41] 多表连接
来源：http://vh.wgjwhj.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://hi.yuexingan06.cn

JOIN users u ON u.id = o.user_id
来源：http://sl.jianghongdianzi.cn

JOIN products p ON p.id = o.product_id;
来源：http://aj.shtwfgs.cn

[Q42] 连接条件附加过滤
来源：http://di.haigaiapp.cn

SELECT u.name, o.amount FROM users u
来源：http://gz.hnjuh.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ub.shxzukj.cn

[Q43] 标量子查询
来源：http://sa.huanxung.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://cq.shtwfgs.cn

[Q44] IN 子查询
来源：http://ex.haigaiapp.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://vq.colortex.cn

[Q45] EXISTS 判断存在
来源：http://ed.szsharing.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://yx.haigaiapp.cn

[Q46] NOT EXISTS 判断不存在
来源：http://im.yuexingan06.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wh.shxzskj.cn

[Q47] 与平均值比较
来源：http://he.jianghongdianzi.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://vw.shxzskj.cn


<!-- 参考信息 -->