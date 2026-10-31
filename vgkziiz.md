代发 wailian999

Py:   itertools.permutations(arr)
来源：http://vb.gzmigu.cn

PHP:  // 手写递归交换
来源：http://ma.shtwfgs.cn

JS:   // 手写回溯递归
来源：http://cs.lnxyls.cn

TS:   // 手写回溯递归
来源：http://aj.nicolike.cn

Java: // 手写回溯递归
来源：http://yv.szxytkj.cn

Go:   // 手写回溯递归
来源：http://vx.hnjuh.cn

Ruby: arr.permutation.to_a
来源：http://hv.9csxet.cn

C#:   // 手写回溯递归
来源：http://gu.wgjwhj.cn

[N09] 栈与队列
来源：http://ke.hahajie.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://fv.shxzskj.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://zv.bookmarksfly.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://nx.shtwfgs.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://xj.bjjhwx.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://qc.wgjwhj.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ba.gzmigu.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://nb.yuntaijiaju.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://zv.wgjwhj.cn

[N10] 链表节点定义
来源：http://nn.huixiangedu.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wn.shxzukj.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://os.hahajie.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ho.colortex.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://qj.jctech888.com.cn

Java: class Node { int v; Node next; }
来源：http://vx.asd995.cn

Go:   type Node struct { V int; Next *Node }
来源：http://rz.shxzskj.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://xn.colortex.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://by.gzmigu.cn

[N11] 二叉树中序遍历
来源：http://ed.haigaiapp.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ix.huixinmuqiang.cn

PHP:  // 手写递归函数
来源：http://vu.asd995.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ba.shxzskj.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://el.jianghongdianzi.cn

Java: // 手写递归
来源：http://eb.newstarts.cn

Go:   // 手写递归
来源：http://zg.panjiajie.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://yf.huixiangedu.cn

C#:   // 手写递归
来源：http://bu.hnjuh.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://si.huixiangedu.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://pv.yuntaijiaju.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ft.yuntaijiaju.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://eg.huanxung.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://gw.huixiangedu.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ig.jianghongdianzi.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://qh.szxytkj.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://yq.bjjhwx.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://fw.521024.cn

================================================================================
来源：http://hd.shxzukj.cn

O. 并发与异步
来源：http://ay.wgjwhj.cn

================================================================================
来源：http://ng.huanxung.cn

[O01] 启动一个线程
来源：http://xz.gzmigu.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://at.gzmigu.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://tt.nicolike.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://aj.shxzukj.cn

TS:   // 同 JS
来源：http://so.shxzukj.cn

Java: new Thread(() -> f()).start()
来源：http://dm.9csxet.cn

Go:   go f()
来源：http://rx.hahajie.cn

Ruby: Thread.new { f }
来源：http://km.haigaiapp.cn

C#:   Task.Run(() => F());
来源：http://ig.yuexingan06.cn

[O02] 使用线程池
来源：http://ix.9csxet.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://oy.huanxung.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://kt.jctech888.com.cn

JS:   // worker_threads 线程池
来源：http://wp.colortex.cn

TS:   // worker_threads 线程池
来源：http://ad.huixinmuqiang.cn

Java: Executors.newFixedThreadPool(4)
来源：http://kj.bookmarksfly.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://kp.shtwfgs.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://fz.gzmigu.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://gg.9csxet.cn

[O03] 加锁保护共享数据
来源：http://fz.muxihuayi.cn

Py:   with lock: shared += 1
来源：http://ku.jianghongdianzi.cn

PHP:  // 用 flock() 做文件锁
来源：http://hq.nicolike.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ai.9csxet.cn

TS:   // 同 JS
来源：http://dy.hahajie.cn

Java: synchronized (this) { shared++; }
来源：http://ix.szxytkj.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://lv.huixinmuqiang.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://bp.asd995.cn

C#:   lock (gate) { shared++; }
来源：http://ze.jianghongdianzi.cn

[O04] 定义异步函数并等待
来源：http://yc.nszjky.cn

Py:   async def f():⏎    await g()
来源：http://sa.bookmarksfly.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mw.jctech888.com.cn

JS:   async function f() { await g(); }
来源：http://ng.asd995.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://se.shtwfgs.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://qz.muxihuayi.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://bp.gzmigu.cn

Ruby: # 用 Fiber 或 async gem
来源：http://kr.huanxung.cn

C#:   async Task F() { await G(); }
来源：http://ok.huixiangedu.cn

[O05] 并发执行并等待全部完成
来源：http://fp.colortex.cn

Py:   asyncio.gather(*tasks)
来源：http://re.szsharing.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://jk.jianghongdianzi.cn

JS:   await Promise.all(tasks)
来源：http://sp.szsharing.cn

TS:   await Promise.all(tasks)
来源：http://ao.panjiajie.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://dk.9csxet.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ey.panjiajie.cn

Ruby: threads.map(&:join)
来源：http://cn.jianghongdianzi.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://el.bjjhwx.cn

[O06] 使用进程池
来源：http://fo.muxihuayi.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://yy.yuntaijiaju.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://le.shtwfgs.cn

JS:   // child_process / cluster 模块
来源：http://wc.shxzskj.cn

TS:   // child_process / cluster 模块
来源：http://qg.colortex.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ks.huixiangedu.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://bj.lnxyls.cn

Ruby: // fork 块
来源：http://lw.huanxung.cn

C#:   Parallel.For
来源：http://ie.521024.cn

================================================================================
来源：http://ex.shxzukj.cn

P. 常用工具函数
来源：http://tv.521024.cn

================================================================================
来源：http://ml.bookmarksfly.cn

[P01] 生成 UUID
来源：http://lt.asd995.cn

Py:   str(uuid.uuid4())
来源：http://bo.shxzskj.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://kb.muxihuayi.cn

JS:   crypto.randomUUID()
来源：http://ah.szsharing.cn

TS:   crypto.randomUUID()
来源：http://rf.asd995.cn

Java: UUID.randomUUID().toString()
来源：http://sc.yuntaijiaju.cn

Go:   // 用 github.com/google/uuid
来源：http://bc.huanxung.cn

Ruby: SecureRandom.uuid
来源：http://rr.shxzukj.cn

C#:   Guid.NewGuid().ToString()
来源：http://wb.shxzskj.cn

[P02] MD5 / SHA256 摘要
来源：http://uo.wgjwhj.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ei.nicolike.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://ml.521024.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hw.jianghongdianzi.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ha.yuntaijiaju.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://up.panjiajie.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://oh.chemitech.net.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://dr.bjjhwx.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://dx.colortex.cn

[P03] 生成短随机字符串
来源：http://rq.jctech888.com.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ez.huixiangedu.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://li.haigaiapp.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://cg.lnxyls.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mb.huixinmuqiang.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://av.bjjhwx.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://km.colortex.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://zc.hahajie.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://tv.szxytkj.cn

[P04] 求长度
来源：http://zc.asd995.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wy.shxzukj.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://kf.muxihuayi.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://dm.szsharing.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://qn.huanxung.cn

Java: list.size();  map.size();  s.length()
来源：http://cm.yuntaijiaju.cn

Go:   len(arr);  len(m)
来源：http://ea.chemitech.net.cn

Ruby: x.length;  x.size
来源：http://pc.huanxung.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://ad.muxihuayi.cn

[P05] 判断两个对象内容是否相等
来源：http://jb.chemitech.net.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://ay.chemitech.net.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://or.shxzukj.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ez.muxihuayi.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ul.shxzskj.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://yt.shxzskj.cn

Go:   reflect.DeepEqual(a, b)
来源：http://ur.gzmigu.cn

Ruby: a == b
来源：http://gs.huixiangedu.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://sc.asd995.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ra.jianghongdianzi.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://xf.yuexingan06.cn

PHP:  if (empty($x)) {}
来源：http://so.gzmigu.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://yd.asd995.cn

TS:   if (x == null) {}
来源：http://yi.shxzskj.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://jd.yuexingan06.cn

Go:   if x == nil {}
来源：http://sq.hahajie.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://tf.shxzukj.cn

C#:   if (x is null) {}
来源：http://hr.bookmarksfly.cn

[P07] 防抖与节流
来源：http://ps.haigaiapp.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ju.yuexingan06.cn

PHP:  // 手写时间戳比较
来源：http://en.shxzukj.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://lo.yuntaijiaju.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://vs.bjjhwx.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://gb.gzmigu.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://vv.haigaiapp.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://rg.newstarts.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://kj.jianghongdianzi.cn

[P08] 处理浮点精度问题
来源：http://ts.gzmigu.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://uu.szsharing.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ij.nszjky.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://lo.521024.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://kl.shxzskj.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ow.szxytkj.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wk.jianghongdianzi.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://fo.newstarts.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://zb.asd995.cn

================================================================================
来源：http://ns.521024.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://np.muxihuayi.cn

================================================================================
来源：http://kr.9csxet.cn

[Q01] 创建表
来源：http://ea.shtwfgs.cn

CREATE TABLE users (
来源：http://ea.bookmarksfly.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://pt.huixinmuqiang.cn

name VARCHAR(50) NOT NULL,
来源：http://mn.szxytkj.cn

email VARCHAR(100) UNIQUE,
来源：http://vs.9csxet.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ee.asd995.cn

);
来源：http://hv.bookmarksfly.cn

[Q02] 创建带外键的表
来源：http://wy.521024.cn

CREATE TABLE orders (
来源：http://nm.521024.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://th.haigaiapp.cn

user_id INT NOT NULL,
来源：http://ix.colortex.cn

amount DECIMAL(10, 2),
来源：http://ux.colortex.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://rw.colortex.cn

);
来源：http://jg.lnxyls.cn

[Q03] 增加列
来源：http://gt.9csxet.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://du.muxihuayi.cn

[Q04] 修改列类型
来源：http://dg.gzmigu.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ye.shtwfgs.cn

[Q05] 重命名列
来源：http://pp.szxytkj.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://yf.huanxung.cn

[Q06] 删除列
来源：http://qy.asd995.cn

ALTER TABLE users DROP COLUMN age;
来源：http://qv.lnxyls.cn

[Q07] 删除表
来源：http://iu.huixiangedu.cn

DROP TABLE IF EXISTS orders;
来源：http://yq.chemitech.net.cn

[Q08] 创建普通索引
来源：http://bg.huixiangedu.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://ff.jctech888.com.cn

[Q09] 创建唯一索引
来源：http://rc.lnxyls.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ov.newstarts.cn

[Q10] 插入单行
来源：http://wl.hnjuh.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://br.shxzukj.cn

[Q11] 一次插入多行
来源：http://ft.huixinmuqiang.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://fk.hnjuh.cn

[Q12] 插入后取自增 ID
来源：http://bz.9csxet.cn

INSERT INTO users (name) VALUES ('C');
来源：http://ps.newstarts.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://uc.jianghongdianzi.cn

[Q13] 忽略重复插入
来源：http://wa.colortex.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://oj.chemitech.net.cn

[Q14] 存在则更新（upsert）
来源：http://ow.yuexingan06.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ns.jctech888.com.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://nt.huanxung.cn

[Q15] 查询全部
来源：http://cr.lnxyls.cn

SELECT * FROM users;
来源：http://bn.shtwfgs.cn

[Q16] 查询指定列
来源：http://vo.gzmigu.cn

SELECT id, name FROM users;
来源：http://ps.nicolike.cn

[Q17] 条件查询
来源：http://mc.chemitech.net.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://qm.9csxet.cn

[Q18] 模糊匹配
来源：http://kp.chemitech.net.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://yk.yuntaijiaju.cn

[Q19] 范围查询
来源：http://ft.chemitech.net.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://po.newstarts.cn

[Q20] IN 列表
来源：http://cr.wgjwhj.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://xq.yuntaijiaju.cn

[Q21] 空值判断
来源：http://sa.521024.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://cp.shxzukj.cn

[Q22] 排序
来源：http://fi.lnxyls.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ss.jctech888.com.cn

[Q23] 分页
来源：http://ob.chemitech.net.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://oh.muxihuayi.cn

[Q24] 去重
来源：http://zs.haigaiapp.cn

SELECT DISTINCT city FROM users;
来源：http://jk.haigaiapp.cn

[Q25] 只取前 N 条
来源：http://pl.gzmigu.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ng.shtwfgs.cn

[Q26] 计数
来源：http://rr.bjjhwx.cn

SELECT COUNT(*) FROM users;
来源：http://eb.nicolike.cn

[Q27] 条件计数
来源：http://ud.nszjky.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://yg.szxytkj.cn

[Q28] 求和与平均
来源：http://ys.shxzskj.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.nszjky.cn

[Q29] 最大最小值
来源：http://ee.jctech888.com.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://kk.hnjuh.cn

[Q30] 分组统计
来源：http://ie.gzmigu.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://uh.lnxyls.cn

[Q31] 分组后过滤
来源：http://eo.asd995.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ec.521024.cn

[Q32] 分组拼接字符串
来源：http://gf.huixinmuqiang.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://kj.jianghongdianzi.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://xp.shtwfgs.cn

[Q33] 多列分组
来源：http://fg.9csxet.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ew.panjiajie.cn

[Q34] 每组取第一条
来源：http://jt.haigaiapp.cn

SELECT * FROM (
来源：http://ak.hnjuh.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ou.panjiajie.cn

) t WHERE rn = 1;
来源：http://mo.haigaiapp.cn

[Q35] 内连接
来源：http://yn.bjjhwx.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://if.colortex.cn

[Q36] 左连接
来源：http://ow.nicolike.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://cu.szsharing.cn

[Q37] 右连接
来源：http://ld.jianghongdianzi.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://gr.shtwfgs.cn

[Q38] 全外连接（PostgreSQL）
来源：http://mi.jctech888.com.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wy.huixiangedu.cn

[Q39] 自连接（查上下级）
来源：http://mb.shxzukj.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://rn.shtwfgs.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://cs.huanxung.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://gu.bjjhwx.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://nv.panjiajie.cn

[Q41] 多表连接
来源：http://nu.gzmigu.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://xr.shtwfgs.cn

JOIN users u ON u.id = o.user_id
来源：http://db.huixinmuqiang.cn

JOIN products p ON p.id = o.product_id;
来源：http://bg.asd995.cn

[Q42] 连接条件附加过滤
来源：http://ex.haigaiapp.cn

SELECT u.name, o.amount FROM users u
来源：http://sp.bjjhwx.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://zn.asd995.cn

[Q43] 标量子查询
来源：http://ia.colortex.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.jctech888.com.cn

[Q44] IN 子查询
来源：http://jl.shtwfgs.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://jm.chemitech.net.cn

[Q45] EXISTS 判断存在
来源：http://zg.haigaiapp.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://zk.bjjhwx.cn

[Q46] NOT EXISTS 判断不存在
来源：http://vp.nicolike.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://si.wgjwhj.cn

[Q47] 与平均值比较
来源：http://an.9csxet.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://tb.haigaiapp.cn

[Q48] CTE 公用表表达式
来源：http://mx.wgjwhj.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://rl.9csxet.cn

SELECT * FROM t WHERE c > 5;
来源：http://wc.haigaiapp.cn

[Q49] 更新单行
来源：http://fe.nszjky.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://lg.jctech888.com.cn

[Q50] 批量更新
来源：http://as.shxzskj.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://yw.szsharing.cn

[Q51] 用子查询更新
来源：http://uy.bjjhwx.cn


<!-- 参考信息 -->