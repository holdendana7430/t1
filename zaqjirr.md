代发 wailian999

Ruby: s == s.reverse
来源：http://kb.shxzskj.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://ia.yuntaijiaju.cn

[N07] 两数之和（返回下标）
来源：http://hn.jianghongdianzi.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ow.521024.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://sm.panjiajie.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://zf.yuntaijiaju.cn

TS:   // 手写 Map<string, number>
来源：http://oj.yuexingan06.cn

Java: // 手写 HashMap
来源：http://ng.chemitech.net.cn

Go:   // 手写 map[int]int
来源：http://np.haigaiapp.cn

Ruby: // 手写 Hash
来源：http://mx.huixinmuqiang.cn

C#:   // 手写 Dictionary<int, int>
来源：http://da.muxihuayi.cn

[N08] 生成全排列
来源：http://ra.shtwfgs.cn

Py:   itertools.permutations(arr)
来源：http://jw.521024.cn

PHP:  // 手写递归交换
来源：http://lo.yuntaijiaju.cn

JS:   // 手写回溯递归
来源：http://wq.lnxyls.cn

TS:   // 手写回溯递归
来源：http://da.muxihuayi.cn

Java: // 手写回溯递归
来源：http://yt.jctech888.com.cn

Go:   // 手写回溯递归
来源：http://sn.nszjky.cn

Ruby: arr.permutation.to_a
来源：http://px.hnjuh.cn

C#:   // 手写回溯递归
来源：http://az.521024.cn

[N09] 栈与队列
来源：http://ng.huixiangedu.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://jj.hnjuh.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://oi.yuexingan06.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://iy.9csxet.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://zp.shxzskj.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ki.shtwfgs.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://in.wgjwhj.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://yo.gzmigu.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://tn.asd995.cn

[N10] 链表节点定义
来源：http://zj.bookmarksfly.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ye.hnjuh.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://on.shtwfgs.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://fv.haigaiapp.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://zw.huanxung.cn

Java: class Node { int v; Node next; }
来源：http://bx.chemitech.net.cn

Go:   type Node struct { V int; Next *Node }
来源：http://vk.huanxung.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://bp.wgjwhj.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://sx.gzmigu.cn

[N11] 二叉树中序遍历
来源：http://ik.huixiangedu.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://rn.bookmarksfly.cn

PHP:  // 手写递归函数
来源：http://ad.haigaiapp.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://nt.panjiajie.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://im.huanxung.cn

Java: // 手写递归
来源：http://wj.chemitech.net.cn

Go:   // 手写递归
来源：http://kd.hnjuh.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ch.huixinmuqiang.cn

C#:   // 手写递归
来源：http://en.lnxyls.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://qy.asd995.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://jq.jianghongdianzi.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://rq.newstarts.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://jz.panjiajie.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ag.chemitech.net.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://dx.gzmigu.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://uv.asd995.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://rb.yuexingan06.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wg.gzmigu.cn

================================================================================
来源：http://xm.colortex.cn

O. 并发与异步
来源：http://ek.nicolike.cn

================================================================================
来源：http://em.newstarts.cn

[O01] 启动一个线程
来源：http://sn.shxzukj.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://qo.huixinmuqiang.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://zx.9csxet.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://yb.wgjwhj.cn

TS:   // 同 JS
来源：http://gm.nszjky.cn

Java: new Thread(() -> f()).start()
来源：http://lu.newstarts.cn

Go:   go f()
来源：http://lm.shtwfgs.cn

Ruby: Thread.new { f }
来源：http://av.jctech888.com.cn

C#:   Task.Run(() => F());
来源：http://zo.szsharing.cn

[O02] 使用线程池
来源：http://yc.shxzukj.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ep.nszjky.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://io.asd995.cn

JS:   // worker_threads 线程池
来源：http://jd.jianghongdianzi.cn

TS:   // worker_threads 线程池
来源：http://wg.hahajie.cn

Java: Executors.newFixedThreadPool(4)
来源：http://yk.panjiajie.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://aq.jctech888.com.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://au.521024.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://fw.szxytkj.cn

[O03] 加锁保护共享数据
来源：http://ko.haigaiapp.cn

Py:   with lock: shared += 1
来源：http://pe.jctech888.com.cn

PHP:  // 用 flock() 做文件锁
来源：http://dw.9csxet.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hj.newstarts.cn

TS:   // 同 JS
来源：http://kj.panjiajie.cn

Java: synchronized (this) { shared++; }
来源：http://di.9csxet.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mo.shtwfgs.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://br.shxzukj.cn

C#:   lock (gate) { shared++; }
来源：http://ut.bookmarksfly.cn

[O04] 定义异步函数并等待
来源：http://xz.lnxyls.cn

Py:   async def f():⏎    await g()
来源：http://om.szsharing.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ol.muxihuayi.cn

JS:   async function f() { await g(); }
来源：http://pt.jianghongdianzi.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://rq.nicolike.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://lc.huixinmuqiang.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ls.colortex.cn

Ruby: # 用 Fiber 或 async gem
来源：http://ji.9csxet.cn

C#:   async Task F() { await G(); }
来源：http://yw.hahajie.cn

[O05] 并发执行并等待全部完成
来源：http://jx.bjjhwx.cn

Py:   asyncio.gather(*tasks)
来源：http://dd.newstarts.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ax.9csxet.cn

JS:   await Promise.all(tasks)
来源：http://ft.jianghongdianzi.cn

TS:   await Promise.all(tasks)
来源：http://fg.wgjwhj.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://oy.newstarts.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ff.huixiangedu.cn

Ruby: threads.map(&:join)
来源：http://nv.shxzukj.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://bl.gzmigu.cn

[O06] 使用进程池
来源：http://ep.szxytkj.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://oq.521024.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://hb.asd995.cn

JS:   // child_process / cluster 模块
来源：http://ms.colortex.cn

TS:   // child_process / cluster 模块
来源：http://pq.chemitech.net.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ul.hahajie.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://qs.jianghongdianzi.cn

Ruby: // fork 块
来源：http://ip.panjiajie.cn

C#:   Parallel.For
来源：http://tt.nicolike.cn

================================================================================
来源：http://tl.jianghongdianzi.cn

P. 常用工具函数
来源：http://kr.chemitech.net.cn

================================================================================
来源：http://pz.lnxyls.cn

[P01] 生成 UUID
来源：http://kt.huanxung.cn

Py:   str(uuid.uuid4())
来源：http://ii.huanxung.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ym.huixiangedu.cn

JS:   crypto.randomUUID()
来源：http://vg.yuexingan06.cn

TS:   crypto.randomUUID()
来源：http://qj.yuntaijiaju.cn

Java: UUID.randomUUID().toString()
来源：http://lk.huixiangedu.cn

Go:   // 用 github.com/google/uuid
来源：http://dl.szxytkj.cn

Ruby: SecureRandom.uuid
来源：http://pb.asd995.cn

C#:   Guid.NewGuid().ToString()
来源：http://tk.huixinmuqiang.cn

[P02] MD5 / SHA256 摘要
来源：http://kr.colortex.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://io.szxytkj.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://ks.szxytkj.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mu.hnjuh.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://tf.asd995.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://uw.shtwfgs.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ov.bookmarksfly.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ps.jianghongdianzi.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://tk.shxzskj.cn

[P03] 生成短随机字符串
来源：http://fg.szxytkj.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://re.shxzukj.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://sg.bjjhwx.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://dr.bookmarksfly.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://kr.shxzukj.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://rp.nszjky.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ym.asd995.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://bt.haigaiapp.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://gh.asd995.cn

[P04] 求长度
来源：http://yu.shxzskj.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://be.szxytkj.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://pj.colortex.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ps.newstarts.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://sd.shxzukj.cn

Java: list.size();  map.size();  s.length()
来源：http://yu.muxihuayi.cn

Go:   len(arr);  len(m)
来源：http://ym.muxihuayi.cn

Ruby: x.length;  x.size
来源：http://wb.muxihuayi.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://yk.chemitech.net.cn

[P05] 判断两个对象内容是否相等
来源：http://ev.szxytkj.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://en.nszjky.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://em.gzmigu.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://zz.yuntaijiaju.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://oj.panjiajie.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://td.nicolike.cn

Go:   reflect.DeepEqual(a, b)
来源：http://hh.panjiajie.cn

Ruby: a == b
来源：http://mm.shxzukj.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://fw.huanxung.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://pg.shxzskj.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ho.nicolike.cn

PHP:  if (empty($x)) {}
来源：http://di.shxzskj.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hu.9csxet.cn

TS:   if (x == null) {}
来源：http://cf.521024.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://wm.nszjky.cn

Go:   if x == nil {}
来源：http://xq.panjiajie.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ef.asd995.cn

C#:   if (x is null) {}
来源：http://yb.bjjhwx.cn

[P07] 防抖与节流
来源：http://ze.szxytkj.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hl.bookmarksfly.cn

PHP:  // 手写时间戳比较
来源：http://zo.colortex.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hs.shxzukj.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ie.gzmigu.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ci.shtwfgs.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://lq.9csxet.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://jo.yuexingan06.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://as.asd995.cn

[P08] 处理浮点精度问题
来源：http://at.muxihuayi.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ei.huanxung.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://op.chemitech.net.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://tp.hnjuh.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://cj.lnxyls.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://qh.jianghongdianzi.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://kn.muxihuayi.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://lv.bookmarksfly.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://tw.nszjky.cn

================================================================================
来源：http://zo.hnjuh.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://fk.asd995.cn

================================================================================
来源：http://ks.hahajie.cn

[Q01] 创建表
来源：http://pp.huixiangedu.cn

CREATE TABLE users (
来源：http://tf.chemitech.net.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://af.huixiangedu.cn

name VARCHAR(50) NOT NULL,
来源：http://ma.wgjwhj.cn

email VARCHAR(100) UNIQUE,
来源：http://pv.shtwfgs.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://xa.haigaiapp.cn

);
来源：http://ho.huixiangedu.cn

[Q02] 创建带外键的表
来源：http://yz.panjiajie.cn

CREATE TABLE orders (
来源：http://ta.521024.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ch.9csxet.cn

user_id INT NOT NULL,
来源：http://wa.nicolike.cn

amount DECIMAL(10, 2),
来源：http://bl.gzmigu.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://rd.shtwfgs.cn

);
来源：http://jv.colortex.cn

[Q03] 增加列
来源：http://vd.szxytkj.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://yg.nszjky.cn

[Q04] 修改列类型
来源：http://wm.gzmigu.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://vv.panjiajie.cn

[Q05] 重命名列
来源：http://aj.521024.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ps.nszjky.cn

[Q06] 删除列
来源：http://ii.521024.cn

ALTER TABLE users DROP COLUMN age;
来源：http://yq.huanxung.cn

[Q07] 删除表
来源：http://tq.shxzukj.cn

DROP TABLE IF EXISTS orders;
来源：http://dj.hnjuh.cn

[Q08] 创建普通索引
来源：http://wg.521024.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://gp.chemitech.net.cn

[Q09] 创建唯一索引
来源：http://mv.9csxet.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ls.jctech888.com.cn

[Q10] 插入单行
来源：http://gt.shtwfgs.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://kz.haigaiapp.cn

[Q11] 一次插入多行
来源：http://oi.huixinmuqiang.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ry.szsharing.cn

[Q12] 插入后取自增 ID
来源：http://dm.hnjuh.cn

INSERT INTO users (name) VALUES ('C');
来源：http://hk.shxzukj.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://oe.jianghongdianzi.cn

[Q13] 忽略重复插入
来源：http://se.asd995.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ln.colortex.cn

[Q14] 存在则更新（upsert）
来源：http://es.shxzukj.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://dn.hnjuh.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ul.nszjky.cn

[Q15] 查询全部
来源：http://ow.shxzukj.cn

SELECT * FROM users;
来源：http://qs.nicolike.cn

[Q16] 查询指定列
来源：http://fe.asd995.cn

SELECT id, name FROM users;
来源：http://bc.hahajie.cn

[Q17] 条件查询
来源：http://fx.szxytkj.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://lq.jctech888.com.cn

[Q18] 模糊匹配
来源：http://ir.shtwfgs.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://yb.nicolike.cn

[Q19] 范围查询
来源：http://du.huanxung.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://zk.huanxung.cn

[Q20] IN 列表
来源：http://de.hahajie.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wp.newstarts.cn

[Q21] 空值判断
来源：http://cv.bookmarksfly.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://fi.nicolike.cn

[Q22] 排序
来源：http://hy.szsharing.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://gf.521024.cn

[Q23] 分页
来源：http://jo.shxzskj.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://kd.huixinmuqiang.cn

[Q24] 去重
来源：http://io.jianghongdianzi.cn

SELECT DISTINCT city FROM users;
来源：http://yr.haigaiapp.cn

[Q25] 只取前 N 条
来源：http://sh.szxytkj.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://nc.muxihuayi.cn

[Q26] 计数
来源：http://tj.szxytkj.cn

SELECT COUNT(*) FROM users;
来源：http://ff.yuntaijiaju.cn

[Q27] 条件计数
来源：http://nr.jctech888.com.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ao.yuntaijiaju.cn

[Q28] 求和与平均
来源：http://db.newstarts.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://rc.bookmarksfly.cn

[Q29] 最大最小值
来源：http://gk.gzmigu.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://qk.shxzukj.cn

[Q30] 分组统计
来源：http://rq.shtwfgs.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hf.szsharing.cn

[Q31] 分组后过滤
来源：http://gm.shtwfgs.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://rl.huanxung.cn

[Q32] 分组拼接字符串
来源：http://nb.lnxyls.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ah.shxzskj.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://sl.szsharing.cn

[Q33] 多列分组
来源：http://ub.jctech888.com.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ai.hnjuh.cn

[Q34] 每组取第一条
来源：http://rm.muxihuayi.cn

SELECT * FROM (
来源：http://oy.haigaiapp.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://cx.wgjwhj.cn

) t WHERE rn = 1;
来源：http://fv.colortex.cn

[Q35] 内连接
来源：http://mi.muxihuayi.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ac.newstarts.cn

[Q36] 左连接
来源：http://lm.haigaiapp.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://fp.yuexingan06.cn

[Q37] 右连接
来源：http://gf.huixinmuqiang.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://al.nszjky.cn

[Q38] 全外连接（PostgreSQL）
来源：http://mm.wgjwhj.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://fh.szxytkj.cn

[Q39] 自连接（查上下级）
来源：http://li.asd995.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://sj.bookmarksfly.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://fa.jianghongdianzi.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://xg.huixinmuqiang.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://bg.colortex.cn

[Q41] 多表连接
来源：http://xa.asd995.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://dz.haigaiapp.cn

JOIN users u ON u.id = o.user_id
来源：http://zs.haigaiapp.cn

JOIN products p ON p.id = o.product_id;
来源：http://bt.yuexingan06.cn

[Q42] 连接条件附加过滤
来源：http://rp.colortex.cn

SELECT u.name, o.amount FROM users u
来源：http://nq.muxihuayi.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mv.szxytkj.cn

[Q43] 标量子查询
来源：http://io.wgjwhj.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://tc.huixiangedu.cn

[Q44] IN 子查询
来源：http://cm.9csxet.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mw.hnjuh.cn

[Q45] EXISTS 判断存在
来源：http://mx.nszjky.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://og.shtwfgs.cn


<!-- 参考信息 -->