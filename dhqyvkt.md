代发 wailian999

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://gq.lnxyls.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://en.hnjuh.cn

TS:   // 手写 Map<string, number>
来源：http://cb.haigaiapp.cn

Java: // 手写 HashMap
来源：http://sa.huixinmuqiang.cn

Go:   // 手写 map[int]int
来源：http://ks.yuntaijiaju.cn

Ruby: // 手写 Hash
来源：http://sj.chemitech.net.cn

C#:   // 手写 Dictionary<int, int>
来源：http://yf.bjjhwx.cn

[N08] 生成全排列
来源：http://mn.bjjhwx.cn

Py:   itertools.permutations(arr)
来源：http://ds.hahajie.cn

PHP:  // 手写递归交换
来源：http://qb.colortex.cn

JS:   // 手写回溯递归
来源：http://ua.shxzskj.cn

TS:   // 手写回溯递归
来源：http://yn.szxytkj.cn

Java: // 手写回溯递归
来源：http://tc.shxzukj.cn

Go:   // 手写回溯递归
来源：http://ly.yuexingan06.cn

Ruby: arr.permutation.to_a
来源：http://sb.panjiajie.cn

C#:   // 手写回溯递归
来源：http://lp.chemitech.net.cn

[N09] 栈与队列
来源：http://qz.yuntaijiaju.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://fm.shxzukj.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://jh.wgjwhj.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://kd.shxzskj.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://we.asd995.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://lk.shxzskj.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://bx.huixiangedu.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://nq.shxzukj.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://yq.jianghongdianzi.cn

[N10] 链表节点定义
来源：http://dy.muxihuayi.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mv.shxzskj.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://xt.yuntaijiaju.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://yr.hnjuh.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://vf.panjiajie.cn

Java: class Node { int v; Node next; }
来源：http://fo.shxzukj.cn

Go:   type Node struct { V int; Next *Node }
来源：http://na.hnjuh.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://do.asd995.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://na.szsharing.cn

[N11] 二叉树中序遍历
来源：http://kt.huanxung.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://pk.gzmigu.cn

PHP:  // 手写递归函数
来源：http://yj.wgjwhj.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://vo.shxzskj.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://zg.shxzskj.cn

Java: // 手写递归
来源：http://ak.asd995.cn

Go:   // 手写递归
来源：http://uo.jianghongdianzi.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hb.yuexingan06.cn

C#:   // 手写递归
来源：http://ed.shxzukj.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://jt.lnxyls.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://oi.huanxung.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ol.asd995.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ex.yuexingan06.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ep.yuexingan06.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://jn.szsharing.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://qx.colortex.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://tk.huanxung.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ac.9csxet.cn

================================================================================
来源：http://md.colortex.cn

O. 并发与异步
来源：http://ld.shtwfgs.cn

================================================================================
来源：http://zc.haigaiapp.cn

[O01] 启动一个线程
来源：http://ry.yuntaijiaju.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://rl.muxihuayi.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wf.nicolike.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wa.bookmarksfly.cn

TS:   // 同 JS
来源：http://aj.newstarts.cn

Java: new Thread(() -> f()).start()
来源：http://dp.wgjwhj.cn

Go:   go f()
来源：http://iy.wgjwhj.cn

Ruby: Thread.new { f }
来源：http://ql.huixinmuqiang.cn

C#:   Task.Run(() => F());
来源：http://jy.wgjwhj.cn

[O02] 使用线程池
来源：http://kp.shxzukj.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ug.jianghongdianzi.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ob.nszjky.cn

JS:   // worker_threads 线程池
来源：http://de.gzmigu.cn

TS:   // worker_threads 线程池
来源：http://hf.panjiajie.cn

Java: Executors.newFixedThreadPool(4)
来源：http://ko.nicolike.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://iw.chemitech.net.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://oc.jianghongdianzi.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://io.jianghongdianzi.cn

[O03] 加锁保护共享数据
来源：http://sj.huixinmuqiang.cn

Py:   with lock: shared += 1
来源：http://nv.chemitech.net.cn

PHP:  // 用 flock() 做文件锁
来源：http://pv.shxzukj.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://zr.huixiangedu.cn

TS:   // 同 JS
来源：http://vz.colortex.cn

Java: synchronized (this) { shared++; }
来源：http://hh.chemitech.net.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://lm.chemitech.net.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://wf.nicolike.cn

C#:   lock (gate) { shared++; }
来源：http://ae.521024.cn

[O04] 定义异步函数并等待
来源：http://qe.chemitech.net.cn

Py:   async def f():⏎    await g()
来源：http://bg.jianghongdianzi.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hi.nszjky.cn

JS:   async function f() { await g(); }
来源：http://jn.nszjky.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://rp.jianghongdianzi.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://xd.lnxyls.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://cu.bjjhwx.cn

Ruby: # 用 Fiber 或 async gem
来源：http://gm.bookmarksfly.cn

C#:   async Task F() { await G(); }
来源：http://vj.jctech888.com.cn

[O05] 并发执行并等待全部完成
来源：http://sn.jctech888.com.cn

Py:   asyncio.gather(*tasks)
来源：http://zl.huanxung.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://fp.yuexingan06.cn

JS:   await Promise.all(tasks)
来源：http://tp.yuexingan06.cn

TS:   await Promise.all(tasks)
来源：http://rn.bjjhwx.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://cb.bookmarksfly.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://lj.huixiangedu.cn

Ruby: threads.map(&:join)
来源：http://pp.yuntaijiaju.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://pt.nszjky.cn

[O06] 使用进程池
来源：http://it.jianghongdianzi.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ri.panjiajie.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://hs.yuntaijiaju.cn

JS:   // child_process / cluster 模块
来源：http://ex.asd995.cn

TS:   // child_process / cluster 模块
来源：http://ai.asd995.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://qr.yuntaijiaju.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hy.haigaiapp.cn

Ruby: // fork 块
来源：http://gf.yuntaijiaju.cn

C#:   Parallel.For
来源：http://op.colortex.cn

================================================================================
来源：http://en.bjjhwx.cn

P. 常用工具函数
来源：http://ak.shtwfgs.cn

================================================================================
来源：http://af.jctech888.com.cn

[P01] 生成 UUID
来源：http://ae.gzmigu.cn

Py:   str(uuid.uuid4())
来源：http://cz.huanxung.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://lr.9csxet.cn

JS:   crypto.randomUUID()
来源：http://ku.szxytkj.cn

TS:   crypto.randomUUID()
来源：http://tn.shtwfgs.cn

Java: UUID.randomUUID().toString()
来源：http://cz.szsharing.cn

Go:   // 用 github.com/google/uuid
来源：http://bn.jianghongdianzi.cn

Ruby: SecureRandom.uuid
来源：http://hs.huanxung.cn

C#:   Guid.NewGuid().ToString()
来源：http://yt.haigaiapp.cn

[P02] MD5 / SHA256 摘要
来源：http://bb.shtwfgs.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://il.9csxet.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://sn.colortex.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ny.huixiangedu.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://py.wgjwhj.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ym.nicolike.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://xc.jianghongdianzi.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://fe.hahajie.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ze.huixinmuqiang.cn

[P03] 生成短随机字符串
来源：http://fp.nicolike.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://jr.shtwfgs.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ei.jianghongdianzi.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://tr.panjiajie.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://lr.chemitech.net.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://lv.gzmigu.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://fg.shxzskj.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://gv.shxzskj.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://it.muxihuayi.cn

[P04] 求长度
来源：http://cs.bjjhwx.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://bh.lnxyls.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ar.szxytkj.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ca.huixinmuqiang.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://tn.panjiajie.cn

Java: list.size();  map.size();  s.length()
来源：http://ww.521024.cn

Go:   len(arr);  len(m)
来源：http://tk.yuexingan06.cn

Ruby: x.length;  x.size
来源：http://vn.bookmarksfly.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://bs.muxihuayi.cn

[P05] 判断两个对象内容是否相等
来源：http://ve.yuntaijiaju.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://lb.shxzukj.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://oo.nicolike.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://rn.muxihuayi.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://af.yuntaijiaju.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://dq.bookmarksfly.cn

Go:   reflect.DeepEqual(a, b)
来源：http://wo.szsharing.cn

Ruby: a == b
来源：http://xz.9csxet.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://tw.yuntaijiaju.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://er.hahajie.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://nl.huixiangedu.cn

PHP:  if (empty($x)) {}
来源：http://lt.yuntaijiaju.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://rt.huanxung.cn

TS:   if (x == null) {}
来源：http://gt.yuntaijiaju.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://le.huixinmuqiang.cn

Go:   if x == nil {}
来源：http://fn.shxzukj.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://xn.newstarts.cn

C#:   if (x is null) {}
来源：http://ip.bjjhwx.cn

[P07] 防抖与节流
来源：http://sr.yuexingan06.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://cd.chemitech.net.cn

PHP:  // 手写时间戳比较
来源：http://og.wgjwhj.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://dp.panjiajie.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://tw.yuntaijiaju.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://pi.9csxet.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://nu.huixiangedu.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://pa.szxytkj.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://bl.colortex.cn

[P08] 处理浮点精度问题
来源：http://fr.9csxet.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://rq.huanxung.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ql.hahajie.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://nh.gzmigu.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://dh.haigaiapp.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://nr.9csxet.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://iq.yuntaijiaju.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://qf.huanxung.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://gx.haigaiapp.cn

================================================================================
来源：http://yv.yuntaijiaju.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ux.jctech888.com.cn

================================================================================
来源：http://sb.panjiajie.cn

[Q01] 创建表
来源：http://af.nszjky.cn

CREATE TABLE users (
来源：http://hi.asd995.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://xa.yuexingan06.cn

name VARCHAR(50) NOT NULL,
来源：http://xg.gzmigu.cn

email VARCHAR(100) UNIQUE,
来源：http://sn.colortex.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ct.shtwfgs.cn

);
来源：http://ty.9csxet.cn

[Q02] 创建带外键的表
来源：http://rh.muxihuayi.cn

CREATE TABLE orders (
来源：http://nz.jctech888.com.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ag.shxzskj.cn

user_id INT NOT NULL,
来源：http://tl.521024.cn

amount DECIMAL(10, 2),
来源：http://nl.huanxung.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://xl.521024.cn

);
来源：http://tn.huixiangedu.cn

[Q03] 增加列
来源：http://gt.jctech888.com.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://cp.shxzukj.cn

[Q04] 修改列类型
来源：http://jb.muxihuayi.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ue.shxzskj.cn

[Q05] 重命名列
来源：http://sv.yuntaijiaju.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://lx.shxzskj.cn

[Q06] 删除列
来源：http://xh.yuntaijiaju.cn

ALTER TABLE users DROP COLUMN age;
来源：http://ih.hahajie.cn

[Q07] 删除表
来源：http://bh.9csxet.cn

DROP TABLE IF EXISTS orders;
来源：http://pz.szxytkj.cn

[Q08] 创建普通索引
来源：http://hd.huixinmuqiang.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://zn.wgjwhj.cn

[Q09] 创建唯一索引
来源：http://yk.shxzskj.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://bq.bjjhwx.cn

[Q10] 插入单行
来源：http://ub.muxihuayi.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://sx.chemitech.net.cn

[Q11] 一次插入多行
来源：http://sy.szxytkj.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://xg.huanxung.cn

[Q12] 插入后取自增 ID
来源：http://mw.jianghongdianzi.cn

INSERT INTO users (name) VALUES ('C');
来源：http://dy.szxytkj.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://en.shxzukj.cn

[Q13] 忽略重复插入
来源：http://ji.yuntaijiaju.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ne.haigaiapp.cn

[Q14] 存在则更新（upsert）
来源：http://bz.hahajie.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ma.asd995.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://nj.jianghongdianzi.cn

[Q15] 查询全部
来源：http://xm.nszjky.cn

SELECT * FROM users;
来源：http://el.yuexingan06.cn

[Q16] 查询指定列
来源：http://ks.nicolike.cn

SELECT id, name FROM users;
来源：http://px.asd995.cn

[Q17] 条件查询
来源：http://yr.haigaiapp.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://zb.shxzskj.cn

[Q18] 模糊匹配
来源：http://go.jctech888.com.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://rx.shxzskj.cn

[Q19] 范围查询
来源：http://pq.521024.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wf.jctech888.com.cn

[Q20] IN 列表
来源：http://ab.shxzskj.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mi.shtwfgs.cn

[Q21] 空值判断
来源：http://vm.521024.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://hn.jianghongdianzi.cn

[Q22] 排序
来源：http://lx.lnxyls.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://bm.9csxet.cn

[Q23] 分页
来源：http://wp.lnxyls.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://kd.chemitech.net.cn

[Q24] 去重
来源：http://lu.huixiangedu.cn

SELECT DISTINCT city FROM users;
来源：http://ze.lnxyls.cn

[Q25] 只取前 N 条
来源：http://yq.yuntaijiaju.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://bj.newstarts.cn

[Q26] 计数
来源：http://ge.huixinmuqiang.cn

SELECT COUNT(*) FROM users;
来源：http://mt.panjiajie.cn

[Q27] 条件计数
来源：http://nl.jianghongdianzi.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mk.huixinmuqiang.cn

[Q28] 求和与平均
来源：http://ha.panjiajie.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://nl.wgjwhj.cn

[Q29] 最大最小值
来源：http://rk.jctech888.com.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://ga.szsharing.cn

[Q30] 分组统计
来源：http://lb.521024.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://sy.hahajie.cn

[Q31] 分组后过滤
来源：http://ak.gzmigu.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://rm.haigaiapp.cn

[Q32] 分组拼接字符串
来源：http://xu.shtwfgs.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ga.huanxung.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://cu.jianghongdianzi.cn

[Q33] 多列分组
来源：http://ky.szxytkj.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://gn.shxzskj.cn

[Q34] 每组取第一条
来源：http://us.colortex.cn

SELECT * FROM (
来源：http://cq.shtwfgs.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://en.9csxet.cn

) t WHERE rn = 1;
来源：http://gq.jctech888.com.cn

[Q35] 内连接
来源：http://kz.yuexingan06.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://kn.haigaiapp.cn

[Q36] 左连接
来源：http://ba.521024.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://fi.szsharing.cn

[Q37] 右连接
来源：http://ch.muxihuayi.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ks.szsharing.cn

[Q38] 全外连接（PostgreSQL）
来源：http://po.wgjwhj.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ge.huixiangedu.cn

[Q39] 自连接（查上下级）
来源：http://sw.gzmigu.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://jb.wgjwhj.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ie.jctech888.com.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://ti.9csxet.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://gd.lnxyls.cn

[Q41] 多表连接
来源：http://vs.9csxet.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://yl.bookmarksfly.cn

JOIN users u ON u.id = o.user_id
来源：http://be.yuntaijiaju.cn

JOIN products p ON p.id = o.product_id;
来源：http://gh.yuntaijiaju.cn

[Q42] 连接条件附加过滤
来源：http://sp.gzmigu.cn

SELECT u.name, o.amount FROM users u
来源：http://hq.szsharing.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://gd.wgjwhj.cn

[Q43] 标量子查询
来源：http://qw.shxzskj.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://lv.shxzukj.cn

[Q44] IN 子查询
来源：http://ua.jctech888.com.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hl.nszjky.cn

[Q45] EXISTS 判断存在
来源：http://kx.asd995.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ur.9csxet.cn

[Q46] NOT EXISTS 判断不存在
来源：http://si.shxzskj.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://kw.huixinmuqiang.cn

[Q47] 与平均值比较
来源：http://rg.bjjhwx.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ka.szxytkj.cn


<!-- 参考信息 -->