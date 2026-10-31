代发 wailian999

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://tn.haigaiapp.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://gc.lnxyls.cn

TS:   // 手写 Map<string, number>
来源：http://ew.haigaiapp.cn

Java: // 手写 HashMap
来源：http://xb.muxihuayi.cn

Go:   // 手写 map[int]int
来源：http://gq.jctech888.com.cn

Ruby: // 手写 Hash
来源：http://jg.nszjky.cn

C#:   // 手写 Dictionary<int, int>
来源：http://hu.jianghongdianzi.cn

[N08] 生成全排列
来源：http://hx.nszjky.cn

Py:   itertools.permutations(arr)
来源：http://xw.huixinmuqiang.cn

PHP:  // 手写递归交换
来源：http://pe.lnxyls.cn

JS:   // 手写回溯递归
来源：http://bl.muxihuayi.cn

TS:   // 手写回溯递归
来源：http://rb.bookmarksfly.cn

Java: // 手写回溯递归
来源：http://uh.shxzskj.cn

Go:   // 手写回溯递归
来源：http://rx.shtwfgs.cn

Ruby: arr.permutation.to_a
来源：http://no.huixinmuqiang.cn

C#:   // 手写回溯递归
来源：http://oh.panjiajie.cn

[N09] 栈与队列
来源：http://md.jctech888.com.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ep.hahajie.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://yf.newstarts.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://oc.wgjwhj.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://dm.huixinmuqiang.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://uo.9csxet.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://zz.muxihuayi.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mw.panjiajie.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://yw.9csxet.cn

[N10] 链表节点定义
来源：http://cj.bookmarksfly.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://tu.521024.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://dm.huixiangedu.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mw.bjjhwx.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://xg.bjjhwx.cn

Java: class Node { int v; Node next; }
来源：http://io.shxzskj.cn

Go:   type Node struct { V int; Next *Node }
来源：http://nq.bjjhwx.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://xq.jianghongdianzi.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://in.jianghongdianzi.cn

[N11] 二叉树中序遍历
来源：http://wy.huanxung.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://cq.shxzukj.cn

PHP:  // 手写递归函数
来源：http://pm.colortex.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://vn.hahajie.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mp.hnjuh.cn

Java: // 手写递归
来源：http://km.yuntaijiaju.cn

Go:   // 手写递归
来源：http://im.huixiangedu.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://oc.bookmarksfly.cn

C#:   // 手写递归
来源：http://gz.lnxyls.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://vb.yuntaijiaju.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wd.bookmarksfly.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wt.szsharing.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://lt.bjjhwx.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wa.nicolike.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://po.huanxung.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ks.jctech888.com.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ia.9csxet.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://vp.shxzskj.cn

================================================================================
来源：http://gp.shxzskj.cn

O. 并发与异步
来源：http://tw.shtwfgs.cn

================================================================================
来源：http://ms.huanxung.cn

[O01] 启动一个线程
来源：http://sd.huanxung.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://vq.jianghongdianzi.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://rt.521024.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://eg.szxytkj.cn

TS:   // 同 JS
来源：http://wq.szxytkj.cn

Java: new Thread(() -> f()).start()
来源：http://gb.huixinmuqiang.cn

Go:   go f()
来源：http://qi.huanxung.cn

Ruby: Thread.new { f }
来源：http://qr.bjjhwx.cn

C#:   Task.Run(() => F());
来源：http://jp.hahajie.cn

[O02] 使用线程池
来源：http://ti.shxzukj.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mm.panjiajie.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://te.panjiajie.cn

JS:   // worker_threads 线程池
来源：http://ja.szsharing.cn

TS:   // worker_threads 线程池
来源：http://kw.shtwfgs.cn

Java: Executors.newFixedThreadPool(4)
来源：http://te.asd995.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://fw.huanxung.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://oz.bookmarksfly.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://oa.colortex.cn

[O03] 加锁保护共享数据
来源：http://db.colortex.cn

Py:   with lock: shared += 1
来源：http://aj.chemitech.net.cn

PHP:  // 用 flock() 做文件锁
来源：http://vs.shtwfgs.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://iy.huixiangedu.cn

TS:   // 同 JS
来源：http://qw.lnxyls.cn

Java: synchronized (this) { shared++; }
来源：http://gk.newstarts.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://gd.szxytkj.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://vm.szsharing.cn

C#:   lock (gate) { shared++; }
来源：http://sn.shxzskj.cn

[O04] 定义异步函数并等待
来源：http://my.panjiajie.cn

Py:   async def f():⏎    await g()
来源：http://by.szsharing.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ch.colortex.cn

JS:   async function f() { await g(); }
来源：http://jy.shxzskj.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://to.bjjhwx.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ns.muxihuayi.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hr.yuntaijiaju.cn

Ruby: # 用 Fiber 或 async gem
来源：http://mz.bookmarksfly.cn

C#:   async Task F() { await G(); }
来源：http://qn.yuexingan06.cn

[O05] 并发执行并等待全部完成
来源：http://up.hahajie.cn

Py:   asyncio.gather(*tasks)
来源：http://dx.gzmigu.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://fe.nszjky.cn

JS:   await Promise.all(tasks)
来源：http://tv.asd995.cn

TS:   await Promise.all(tasks)
来源：http://lo.521024.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://gj.haigaiapp.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://tp.nicolike.cn

Ruby: threads.map(&:join)
来源：http://nr.jctech888.com.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://je.9csxet.cn

[O06] 使用进程池
来源：http://tx.colortex.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ge.yuntaijiaju.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://go.bookmarksfly.cn

JS:   // child_process / cluster 模块
来源：http://sg.bjjhwx.cn

TS:   // child_process / cluster 模块
来源：http://nb.huixiangedu.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://tw.jctech888.com.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ax.jctech888.com.cn

Ruby: // fork 块
来源：http://ny.szxytkj.cn

C#:   Parallel.For
来源：http://zh.9csxet.cn

================================================================================
来源：http://if.jianghongdianzi.cn

P. 常用工具函数
来源：http://sb.huixinmuqiang.cn

================================================================================
来源：http://ji.huanxung.cn

[P01] 生成 UUID
来源：http://vk.521024.cn

Py:   str(uuid.uuid4())
来源：http://sm.jianghongdianzi.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://df.huixinmuqiang.cn

JS:   crypto.randomUUID()
来源：http://tt.huanxung.cn

TS:   crypto.randomUUID()
来源：http://al.bookmarksfly.cn

Java: UUID.randomUUID().toString()
来源：http://os.lnxyls.cn

Go:   // 用 github.com/google/uuid
来源：http://vq.yuexingan06.cn

Ruby: SecureRandom.uuid
来源：http://np.wgjwhj.cn

C#:   Guid.NewGuid().ToString()
来源：http://pe.szxytkj.cn

[P02] MD5 / SHA256 摘要
来源：http://nr.huanxung.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://jk.521024.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://hw.colortex.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hh.bjjhwx.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://sc.nszjky.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://xq.yuexingan06.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://up.asd995.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ib.yuexingan06.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://as.9csxet.cn

[P03] 生成短随机字符串
来源：http://xt.huanxung.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://dj.yuntaijiaju.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://vv.szxytkj.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://jl.shxzukj.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ko.newstarts.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://zi.newstarts.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ff.haigaiapp.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://oj.shtwfgs.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://bh.huixinmuqiang.cn

[P04] 求长度
来源：http://jl.bjjhwx.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://gu.gzmigu.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mv.521024.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://tx.nicolike.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ds.jianghongdianzi.cn

Java: list.size();  map.size();  s.length()
来源：http://uk.bjjhwx.cn

Go:   len(arr);  len(m)
来源：http://ge.nicolike.cn

Ruby: x.length;  x.size
来源：http://ao.jctech888.com.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://cr.9csxet.cn

[P05] 判断两个对象内容是否相等
来源：http://ec.shxzskj.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://jb.newstarts.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://pm.panjiajie.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://qr.hahajie.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://os.shtwfgs.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://rz.jianghongdianzi.cn

Go:   reflect.DeepEqual(a, b)
来源：http://po.521024.cn

Ruby: a == b
来源：http://ln.shtwfgs.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://es.shtwfgs.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://no.bookmarksfly.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://pu.chemitech.net.cn

PHP:  if (empty($x)) {}
来源：http://hl.lnxyls.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ss.panjiajie.cn

TS:   if (x == null) {}
来源：http://md.szxytkj.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://tl.szxytkj.cn

Go:   if x == nil {}
来源：http://sv.bjjhwx.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://gg.muxihuayi.cn

C#:   if (x is null) {}
来源：http://ed.lnxyls.cn

[P07] 防抖与节流
来源：http://rw.colortex.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://lu.yuntaijiaju.cn

PHP:  // 手写时间戳比较
来源：http://fa.szxytkj.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xd.muxihuayi.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://el.shtwfgs.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://xj.shxzukj.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://fi.hnjuh.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://of.jctech888.com.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ee.jctech888.com.cn

[P08] 处理浮点精度问题
来源：http://ps.haigaiapp.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://nn.gzmigu.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hr.haigaiapp.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://gm.muxihuayi.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://zm.shtwfgs.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://nm.gzmigu.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://er.chemitech.net.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://cp.newstarts.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://gb.9csxet.cn

================================================================================
来源：http://yi.yuexingan06.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://kz.hahajie.cn

================================================================================
来源：http://ji.asd995.cn

[Q01] 创建表
来源：http://xi.asd995.cn

CREATE TABLE users (
来源：http://vs.lnxyls.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://kt.jctech888.com.cn

name VARCHAR(50) NOT NULL,
来源：http://qt.jctech888.com.cn

email VARCHAR(100) UNIQUE,
来源：http://eo.muxihuayi.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://zg.szxytkj.cn

);
来源：http://rx.huixiangedu.cn

[Q02] 创建带外键的表
来源：http://ld.huixiangedu.cn

CREATE TABLE orders (
来源：http://hk.yuexingan06.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://dn.nszjky.cn

user_id INT NOT NULL,
来源：http://nb.huanxung.cn

amount DECIMAL(10, 2),
来源：http://nm.bjjhwx.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://uz.shxzskj.cn

);
来源：http://co.521024.cn

[Q03] 增加列
来源：http://vy.lnxyls.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ob.521024.cn

[Q04] 修改列类型
来源：http://bu.chemitech.net.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hw.chemitech.net.cn

[Q05] 重命名列
来源：http://wu.huixiangedu.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://cu.huanxung.cn

[Q06] 删除列
来源：http://he.huanxung.cn

ALTER TABLE users DROP COLUMN age;
来源：http://ax.shxzukj.cn

[Q07] 删除表
来源：http://py.szxytkj.cn

DROP TABLE IF EXISTS orders;
来源：http://eh.huixinmuqiang.cn

[Q08] 创建普通索引
来源：http://ec.hahajie.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://pk.521024.cn

[Q09] 创建唯一索引
来源：http://xi.szsharing.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wu.9csxet.cn

[Q10] 插入单行
来源：http://ek.chemitech.net.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://yj.jianghongdianzi.cn

[Q11] 一次插入多行
来源：http://fp.lnxyls.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://oi.shtwfgs.cn

[Q12] 插入后取自增 ID
来源：http://np.shtwfgs.cn

INSERT INTO users (name) VALUES ('C');
来源：http://sb.asd995.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://cv.jctech888.com.cn

[Q13] 忽略重复插入
来源：http://uc.jianghongdianzi.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://td.yuntaijiaju.cn

[Q14] 存在则更新（upsert）
来源：http://un.shtwfgs.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://om.haigaiapp.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://lc.newstarts.cn

[Q15] 查询全部
来源：http://ml.colortex.cn

SELECT * FROM users;
来源：http://og.szsharing.cn

[Q16] 查询指定列
来源：http://sh.nszjky.cn

SELECT id, name FROM users;
来源：http://ce.nicolike.cn

[Q17] 条件查询
来源：http://nf.asd995.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hv.muxihuayi.cn

[Q18] 模糊匹配
来源：http://xq.521024.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://vj.lnxyls.cn

[Q19] 范围查询
来源：http://fs.bjjhwx.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://yk.shxzukj.cn

[Q20] IN 列表
来源：http://ue.panjiajie.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://us.shxzukj.cn

[Q21] 空值判断
来源：http://hj.bookmarksfly.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://qu.yuntaijiaju.cn

[Q22] 排序
来源：http://rd.szsharing.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://jk.hahajie.cn

[Q23] 分页
来源：http://tt.nicolike.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://fl.huanxung.cn

[Q24] 去重
来源：http://rw.jianghongdianzi.cn

SELECT DISTINCT city FROM users;
来源：http://fk.bookmarksfly.cn

[Q25] 只取前 N 条
来源：http://ll.hnjuh.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://qg.panjiajie.cn

[Q26] 计数
来源：http://ri.asd995.cn

SELECT COUNT(*) FROM users;
来源：http://hw.yuntaijiaju.cn

[Q27] 条件计数
来源：http://si.newstarts.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ij.hnjuh.cn

[Q28] 求和与平均
来源：http://fv.yuexingan06.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://yq.yuntaijiaju.cn

[Q29] 最大最小值
来源：http://no.jianghongdianzi.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://zf.wgjwhj.cn

[Q30] 分组统计
来源：http://hi.nicolike.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://rh.wgjwhj.cn

[Q31] 分组后过滤
来源：http://nt.jctech888.com.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ru.asd995.cn

[Q32] 分组拼接字符串
来源：http://mv.huixiangedu.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://gf.shtwfgs.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://js.asd995.cn

[Q33] 多列分组
来源：http://pp.muxihuayi.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://cm.yuexingan06.cn

[Q34] 每组取第一条
来源：http://ph.wgjwhj.cn

SELECT * FROM (
来源：http://eo.bjjhwx.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://yg.lnxyls.cn

) t WHERE rn = 1;
来源：http://lb.hahajie.cn

[Q35] 内连接
来源：http://kf.521024.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://se.9csxet.cn

[Q36] 左连接
来源：http://fs.shtwfgs.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://cn.bookmarksfly.cn

[Q37] 右连接
来源：http://fh.yuntaijiaju.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://gq.shtwfgs.cn

[Q38] 全外连接（PostgreSQL）
来源：http://xv.hahajie.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://be.colortex.cn

[Q39] 自连接（查上下级）
来源：http://mn.bookmarksfly.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.asd995.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://oy.chemitech.net.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://ey.gzmigu.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://md.jianghongdianzi.cn

[Q41] 多表连接
来源：http://gr.nszjky.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://hf.nicolike.cn

JOIN users u ON u.id = o.user_id
来源：http://za.jctech888.com.cn

JOIN products p ON p.id = o.product_id;
来源：http://tc.lnxyls.cn

[Q42] 连接条件附加过滤
来源：http://ye.szxytkj.cn

SELECT u.name, o.amount FROM users u
来源：http://wi.chemitech.net.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://jx.bookmarksfly.cn

[Q43] 标量子查询
来源：http://qf.yuntaijiaju.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://al.asd995.cn

[Q44] IN 子查询
来源：http://cz.wgjwhj.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://pm.chemitech.net.cn

[Q45] EXISTS 判断存在
来源：http://lw.haigaiapp.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://sy.huanxung.cn

[Q46] NOT EXISTS 判断不存在
来源：http://ms.shtwfgs.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://fi.huanxung.cn

[Q47] 与平均值比较
来源：http://lq.panjiajie.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://xg.panjiajie.cn


<!-- 参考信息 -->