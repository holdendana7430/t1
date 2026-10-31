代发 wailian999

Go:   // 手写 map[int]int
来源：http://vi.lnxyls.cn

Ruby: // 手写 Hash
来源：http://dc.panjiajie.cn

C#:   // 手写 Dictionary<int, int>
来源：http://fd.lnxyls.cn

[N08] 生成全排列
来源：http://nt.asd995.cn

Py:   itertools.permutations(arr)
来源：http://ot.hahajie.cn

PHP:  // 手写递归交换
来源：http://se.521024.cn

JS:   // 手写回溯递归
来源：http://vi.huixinmuqiang.cn

TS:   // 手写回溯递归
来源：http://ck.asd995.cn

Java: // 手写回溯递归
来源：http://xh.lnxyls.cn

Go:   // 手写回溯递归
来源：http://pq.huixiangedu.cn

Ruby: arr.permutation.to_a
来源：http://gi.szxytkj.cn

C#:   // 手写回溯递归
来源：http://jc.nszjky.cn

[N09] 栈与队列
来源：http://oy.hnjuh.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://fn.hnjuh.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://nj.shxzukj.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://qo.nszjky.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://yn.muxihuayi.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://fr.newstarts.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://tx.haigaiapp.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://po.huixiangedu.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://rs.muxihuayi.cn

[N10] 链表节点定义
来源：http://ss.haigaiapp.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://kq.nszjky.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://df.shxzukj.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://xz.szsharing.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://uk.521024.cn

Java: class Node { int v; Node next; }
来源：http://to.nszjky.cn

Go:   type Node struct { V int; Next *Node }
来源：http://rf.muxihuayi.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://ih.bookmarksfly.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://zo.chemitech.net.cn

[N11] 二叉树中序遍历
来源：http://ce.hahajie.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mf.asd995.cn

PHP:  // 手写递归函数
来源：http://ee.lnxyls.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://aj.huixinmuqiang.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://aj.colortex.cn

Java: // 手写递归
来源：http://vk.muxihuayi.cn

Go:   // 手写递归
来源：http://fl.huixiangedu.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://kl.bookmarksfly.cn

C#:   // 手写递归
来源：http://qw.bjjhwx.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ln.jianghongdianzi.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://er.muxihuayi.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://qt.shtwfgs.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://qi.shtwfgs.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://rx.panjiajie.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ui.haigaiapp.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://cz.huanxung.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://xk.colortex.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ti.nszjky.cn

================================================================================
来源：http://rj.bookmarksfly.cn

O. 并发与异步
来源：http://fo.shtwfgs.cn

================================================================================
来源：http://hy.nicolike.cn

[O01] 启动一个线程
来源：http://rz.lnxyls.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://nw.newstarts.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://rc.szxytkj.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://md.shtwfgs.cn

TS:   // 同 JS
来源：http://ys.shxzskj.cn

Java: new Thread(() -> f()).start()
来源：http://kt.nszjky.cn

Go:   go f()
来源：http://df.szxytkj.cn

Ruby: Thread.new { f }
来源：http://om.hnjuh.cn

C#:   Task.Run(() => F());
来源：http://yn.9csxet.cn

[O02] 使用线程池
来源：http://kr.asd995.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://oi.huixinmuqiang.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://cu.nszjky.cn

JS:   // worker_threads 线程池
来源：http://dc.newstarts.cn

TS:   // worker_threads 线程池
来源：http://ie.haigaiapp.cn

Java: Executors.newFixedThreadPool(4)
来源：http://cq.colortex.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ej.jianghongdianzi.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://xq.hahajie.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://nm.shtwfgs.cn

[O03] 加锁保护共享数据
来源：http://lj.nszjky.cn

Py:   with lock: shared += 1
来源：http://zg.gzmigu.cn

PHP:  // 用 flock() 做文件锁
来源：http://sv.muxihuayi.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://qc.bjjhwx.cn

TS:   // 同 JS
来源：http://ko.yuntaijiaju.cn

Java: synchronized (this) { shared++; }
来源：http://lz.shxzskj.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://av.yuexingan06.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://aa.521024.cn

C#:   lock (gate) { shared++; }
来源：http://lu.chemitech.net.cn

[O04] 定义异步函数并等待
来源：http://yh.hnjuh.cn

Py:   async def f():⏎    await g()
来源：http://zm.szxytkj.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ps.szxytkj.cn

JS:   async function f() { await g(); }
来源：http://zp.hahajie.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://nb.nszjky.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hv.bookmarksfly.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://gc.huixiangedu.cn

Ruby: # 用 Fiber 或 async gem
来源：http://cm.yuntaijiaju.cn

C#:   async Task F() { await G(); }
来源：http://vp.gzmigu.cn

[O05] 并发执行并等待全部完成
来源：http://zb.gzmigu.cn

Py:   asyncio.gather(*tasks)
来源：http://ps.newstarts.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://yi.haigaiapp.cn

JS:   await Promise.all(tasks)
来源：http://pp.hnjuh.cn

TS:   await Promise.all(tasks)
来源：http://cq.bjjhwx.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://rf.szxytkj.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hp.panjiajie.cn

Ruby: threads.map(&:join)
来源：http://mz.haigaiapp.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://zq.hahajie.cn

[O06] 使用进程池
来源：http://da.chemitech.net.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://fk.gzmigu.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://en.asd995.cn

JS:   // child_process / cluster 模块
来源：http://lx.gzmigu.cn

TS:   // child_process / cluster 模块
来源：http://lf.shxzskj.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://cu.shtwfgs.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://tq.nszjky.cn

Ruby: // fork 块
来源：http://aa.shxzskj.cn

C#:   Parallel.For
来源：http://mk.chemitech.net.cn

================================================================================
来源：http://bd.yuntaijiaju.cn

P. 常用工具函数
来源：http://lm.yuntaijiaju.cn

================================================================================
来源：http://lg.hnjuh.cn

[P01] 生成 UUID
来源：http://sj.asd995.cn

Py:   str(uuid.uuid4())
来源：http://jb.hnjuh.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ub.521024.cn

JS:   crypto.randomUUID()
来源：http://lx.asd995.cn

TS:   crypto.randomUUID()
来源：http://kx.9csxet.cn

Java: UUID.randomUUID().toString()
来源：http://zy.hnjuh.cn

Go:   // 用 github.com/google/uuid
来源：http://uu.nicolike.cn

Ruby: SecureRandom.uuid
来源：http://ij.shxzskj.cn

C#:   Guid.NewGuid().ToString()
来源：http://vv.shxzukj.cn

[P02] MD5 / SHA256 摘要
来源：http://gy.huixinmuqiang.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://fo.huixiangedu.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://vl.lnxyls.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://tz.panjiajie.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ed.wgjwhj.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://pr.nszjky.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://lh.nicolike.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ou.gzmigu.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://jb.huixiangedu.cn

[P03] 生成短随机字符串
来源：http://ai.huixinmuqiang.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ge.yuexingan06.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wk.haigaiapp.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://zl.yuexingan06.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://un.asd995.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://bt.colortex.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://os.huixiangedu.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://iu.jctech888.com.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://yz.jianghongdianzi.cn

[P04] 求长度
来源：http://nc.yuexingan06.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://uu.huixiangedu.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://yi.bookmarksfly.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://tc.wgjwhj.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ut.newstarts.cn

Java: list.size();  map.size();  s.length()
来源：http://dw.yuntaijiaju.cn

Go:   len(arr);  len(m)
来源：http://hv.chemitech.net.cn

Ruby: x.length;  x.size
来源：http://cs.jctech888.com.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://xy.panjiajie.cn

[P05] 判断两个对象内容是否相等
来源：http://bo.shxzskj.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://gy.521024.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wb.nszjky.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://cd.shtwfgs.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://sc.jctech888.com.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://rm.shxzukj.cn

Go:   reflect.DeepEqual(a, b)
来源：http://tg.9csxet.cn

Ruby: a == b
来源：http://he.9csxet.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://dq.colortex.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://uc.9csxet.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ua.asd995.cn

PHP:  if (empty($x)) {}
来源：http://lu.haigaiapp.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://vq.panjiajie.cn

TS:   if (x == null) {}
来源：http://dg.szsharing.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://mk.panjiajie.cn

Go:   if x == nil {}
来源：http://xp.muxihuayi.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ud.521024.cn

C#:   if (x is null) {}
来源：http://gq.yuntaijiaju.cn

[P07] 防抖与节流
来源：http://fn.chemitech.net.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://zt.jianghongdianzi.cn

PHP:  // 手写时间戳比较
来源：http://sn.jianghongdianzi.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://bn.bjjhwx.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ac.hnjuh.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://qc.asd995.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://fb.newstarts.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://kr.colortex.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wn.panjiajie.cn

[P08] 处理浮点精度问题
来源：http://rt.lnxyls.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://kk.shtwfgs.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://dc.521024.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://nn.colortex.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://cz.hahajie.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ay.colortex.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://jm.nszjky.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://vj.jctech888.com.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://or.chemitech.net.cn

================================================================================
来源：http://zb.bjjhwx.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://rs.wgjwhj.cn

================================================================================
来源：http://xq.hnjuh.cn

[Q01] 创建表
来源：http://nv.nszjky.cn

CREATE TABLE users (
来源：http://rn.panjiajie.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://si.yuntaijiaju.cn

name VARCHAR(50) NOT NULL,
来源：http://mj.jianghongdianzi.cn

email VARCHAR(100) UNIQUE,
来源：http://ns.yuntaijiaju.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://rn.chemitech.net.cn

);
来源：http://ps.szsharing.cn

[Q02] 创建带外键的表
来源：http://ql.nicolike.cn

CREATE TABLE orders (
来源：http://fw.yuexingan06.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://jk.bjjhwx.cn

user_id INT NOT NULL,
来源：http://di.huixinmuqiang.cn

amount DECIMAL(10, 2),
来源：http://mr.gzmigu.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://lb.shtwfgs.cn

);
来源：http://fq.521024.cn

[Q03] 增加列
来源：http://vl.521024.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ej.bookmarksfly.cn

[Q04] 修改列类型
来源：http://fn.shxzukj.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://po.shtwfgs.cn

[Q05] 重命名列
来源：http://ze.colortex.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ha.yuexingan06.cn

[Q06] 删除列
来源：http://la.haigaiapp.cn

ALTER TABLE users DROP COLUMN age;
来源：http://xi.chemitech.net.cn

[Q07] 删除表
来源：http://el.shxzukj.cn

DROP TABLE IF EXISTS orders;
来源：http://er.chemitech.net.cn

[Q08] 创建普通索引
来源：http://ub.shtwfgs.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://yx.chemitech.net.cn

[Q09] 创建唯一索引
来源：http://jq.asd995.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://aw.asd995.cn

[Q10] 插入单行
来源：http://vk.chemitech.net.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://op.shxzskj.cn

[Q11] 一次插入多行
来源：http://fb.hnjuh.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://pl.muxihuayi.cn

[Q12] 插入后取自增 ID
来源：http://nt.wgjwhj.cn

INSERT INTO users (name) VALUES ('C');
来源：http://if.nicolike.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://lq.asd995.cn

[Q13] 忽略重复插入
来源：http://by.nszjky.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mu.bjjhwx.cn

[Q14] 存在则更新（upsert）
来源：http://hy.521024.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ez.jianghongdianzi.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ed.colortex.cn

[Q15] 查询全部
来源：http://sn.huixiangedu.cn

SELECT * FROM users;
来源：http://sy.nszjky.cn

[Q16] 查询指定列
来源：http://fy.nszjky.cn

SELECT id, name FROM users;
来源：http://dj.huanxung.cn

[Q17] 条件查询
来源：http://gq.shxzskj.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://qz.shxzskj.cn

[Q18] 模糊匹配
来源：http://vz.9csxet.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wd.panjiajie.cn

[Q19] 范围查询
来源：http://ck.bjjhwx.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://vo.yuntaijiaju.cn

[Q20] IN 列表
来源：http://zr.muxihuayi.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ia.huanxung.cn

[Q21] 空值判断
来源：http://al.chemitech.net.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://zs.panjiajie.cn

[Q22] 排序
来源：http://ik.lnxyls.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://bg.bjjhwx.cn

[Q23] 分页
来源：http://mx.yuexingan06.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://aj.shxzukj.cn

[Q24] 去重
来源：http://sb.shxzukj.cn

SELECT DISTINCT city FROM users;
来源：http://wc.gzmigu.cn

[Q25] 只取前 N 条
来源：http://xp.huixiangedu.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ba.9csxet.cn

[Q26] 计数
来源：http://jl.newstarts.cn

SELECT COUNT(*) FROM users;
来源：http://jj.szxytkj.cn

[Q27] 条件计数
来源：http://zj.bookmarksfly.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://kp.bjjhwx.cn

[Q28] 求和与平均
来源：http://uv.huixinmuqiang.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://dn.jianghongdianzi.cn

[Q29] 最大最小值
来源：http://el.huixinmuqiang.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://do.nicolike.cn

[Q30] 分组统计
来源：http://ow.shtwfgs.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://sj.huanxung.cn

[Q31] 分组后过滤
来源：http://ff.bjjhwx.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ks.yuexingan06.cn

[Q32] 分组拼接字符串
来源：http://ip.szsharing.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://qn.jianghongdianzi.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://va.bookmarksfly.cn

[Q33] 多列分组
来源：http://qt.shxzukj.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://vv.szsharing.cn

[Q34] 每组取第一条
来源：http://aj.yuntaijiaju.cn

SELECT * FROM (
来源：http://xz.shxzskj.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ga.yuexingan06.cn

) t WHERE rn = 1;
来源：http://kh.shxzukj.cn

[Q35] 内连接
来源：http://ip.yuexingan06.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://dg.chemitech.net.cn

[Q36] 左连接
来源：http://wd.huixiangedu.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://xd.shxzukj.cn

[Q37] 右连接
来源：http://bf.nszjky.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ym.wgjwhj.cn

[Q38] 全外连接（PostgreSQL）
来源：http://tw.9csxet.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hu.gzmigu.cn

[Q39] 自连接（查上下级）
来源：http://wx.muxihuayi.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://my.shtwfgs.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://st.9csxet.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://bv.hahajie.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wm.asd995.cn

[Q41] 多表连接
来源：http://wh.yuexingan06.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://jp.shxzukj.cn

JOIN users u ON u.id = o.user_id
来源：http://kj.nicolike.cn

JOIN products p ON p.id = o.product_id;
来源：http://gq.colortex.cn

[Q42] 连接条件附加过滤
来源：http://fh.nicolike.cn

SELECT u.name, o.amount FROM users u
来源：http://lv.jctech888.com.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ul.huanxung.cn

[Q43] 标量子查询
来源：http://so.bjjhwx.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mj.521024.cn

[Q44] IN 子查询
来源：http://bf.yuexingan06.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://av.panjiajie.cn

[Q45] EXISTS 判断存在
来源：http://cj.hnjuh.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://vh.newstarts.cn

[Q46] NOT EXISTS 判断不存在
来源：http://du.newstarts.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://fn.wgjwhj.cn

[Q47] 与平均值比较
来源：http://hx.huanxung.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://rq.521024.cn

[Q48] CTE 公用表表达式
来源：http://fj.wgjwhj.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://jq.hnjuh.cn

SELECT * FROM t WHERE c > 5;
来源：http://lz.huixiangedu.cn

[Q49] 更新单行
来源：http://lw.9csxet.cn


<!-- 参考信息 -->