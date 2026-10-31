代发 wailian999

Ruby: s == s.reverse
来源：http://aj.yuntaijiaju.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://qj.shxzskj.cn

[N07] 两数之和（返回下标）
来源：http://qs.yuexingan06.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://gq.szsharing.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://rk.9csxet.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://bf.shtwfgs.cn

TS:   // 手写 Map<string, number>
来源：http://jw.szsharing.cn

Java: // 手写 HashMap
来源：http://gn.hahajie.cn

Go:   // 手写 map[int]int
来源：http://le.jianghongdianzi.cn

Ruby: // 手写 Hash
来源：http://bp.shxzskj.cn

C#:   // 手写 Dictionary<int, int>
来源：http://cx.521024.cn

[N08] 生成全排列
来源：http://mg.panjiajie.cn

Py:   itertools.permutations(arr)
来源：http://tj.wgjwhj.cn

PHP:  // 手写递归交换
来源：http://qr.bjjhwx.cn

JS:   // 手写回溯递归
来源：http://jl.9csxet.cn

TS:   // 手写回溯递归
来源：http://qs.szxytkj.cn

Java: // 手写回溯递归
来源：http://gf.colortex.cn

Go:   // 手写回溯递归
来源：http://ia.hahajie.cn

Ruby: arr.permutation.to_a
来源：http://ox.jctech888.com.cn

C#:   // 手写回溯递归
来源：http://wx.haigaiapp.cn

[N09] 栈与队列
来源：http://qj.jianghongdianzi.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://zj.yuntaijiaju.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://fr.newstarts.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://au.muxihuayi.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://gs.gzmigu.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hb.9csxet.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ev.huixinmuqiang.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://bk.jianghongdianzi.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://iu.9csxet.cn

[N10] 链表节点定义
来源：http://no.shxzskj.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://rt.huixiangedu.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://lm.yuexingan06.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://bg.nszjky.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://gi.shxzskj.cn

Java: class Node { int v; Node next; }
来源：http://vn.huixinmuqiang.cn

Go:   type Node struct { V int; Next *Node }
来源：http://vl.colortex.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://ij.shxzukj.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://sd.muxihuayi.cn

[N11] 二叉树中序遍历
来源：http://yj.wgjwhj.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://jm.nszjky.cn

PHP:  // 手写递归函数
来源：http://og.yuexingan06.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://zz.bookmarksfly.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://zv.jctech888.com.cn

Java: // 手写递归
来源：http://bz.jctech888.com.cn

Go:   // 手写递归
来源：http://ml.asd995.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mi.jctech888.com.cn

C#:   // 手写递归
来源：http://yy.huanxung.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://gv.9csxet.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://lu.9csxet.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wq.yuexingan06.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://zp.chemitech.net.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ac.bookmarksfly.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://qf.yuntaijiaju.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://jq.chemitech.net.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://it.9csxet.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hn.bjjhwx.cn

================================================================================
来源：http://kw.9csxet.cn

O. 并发与异步
来源：http://jn.szsharing.cn

================================================================================
来源：http://ah.chemitech.net.cn

[O01] 启动一个线程
来源：http://iq.shxzskj.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ag.521024.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://zh.nszjky.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hj.huixinmuqiang.cn

TS:   // 同 JS
来源：http://fw.gzmigu.cn

Java: new Thread(() -> f()).start()
来源：http://fg.bookmarksfly.cn

Go:   go f()
来源：http://sg.jianghongdianzi.cn

Ruby: Thread.new { f }
来源：http://bj.yuexingan06.cn

C#:   Task.Run(() => F());
来源：http://ll.shxzskj.cn

[O02] 使用线程池
来源：http://co.panjiajie.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://vd.shxzukj.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://jr.haigaiapp.cn

JS:   // worker_threads 线程池
来源：http://aw.bookmarksfly.cn

TS:   // worker_threads 线程池
来源：http://mm.bookmarksfly.cn

Java: Executors.newFixedThreadPool(4)
来源：http://qq.wgjwhj.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://fz.huixiangedu.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ro.haigaiapp.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://io.jianghongdianzi.cn

[O03] 加锁保护共享数据
来源：http://la.nszjky.cn

Py:   with lock: shared += 1
来源：http://qi.yuexingan06.cn

PHP:  // 用 flock() 做文件锁
来源：http://wv.9csxet.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://kf.nicolike.cn

TS:   // 同 JS
来源：http://mt.nszjky.cn

Java: synchronized (this) { shared++; }
来源：http://oz.lnxyls.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://yk.muxihuayi.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://fn.bjjhwx.cn

C#:   lock (gate) { shared++; }
来源：http://wk.colortex.cn

[O04] 定义异步函数并等待
来源：http://ok.jianghongdianzi.cn

Py:   async def f():⏎    await g()
来源：http://zw.shxzskj.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://al.9csxet.cn

JS:   async function f() { await g(); }
来源：http://wa.huanxung.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://lc.shtwfgs.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://vw.colortex.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ud.szxytkj.cn

Ruby: # 用 Fiber 或 async gem
来源：http://vx.jianghongdianzi.cn

C#:   async Task F() { await G(); }
来源：http://ro.9csxet.cn

[O05] 并发执行并等待全部完成
来源：http://sw.szxytkj.cn

Py:   asyncio.gather(*tasks)
来源：http://gh.shtwfgs.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://oq.jctech888.com.cn

JS:   await Promise.all(tasks)
来源：http://rc.nszjky.cn

TS:   await Promise.all(tasks)
来源：http://sc.newstarts.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://qg.haigaiapp.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hv.huixiangedu.cn

Ruby: threads.map(&:join)
来源：http://fe.haigaiapp.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://hb.panjiajie.cn

[O06] 使用进程池
来源：http://ew.hnjuh.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://qb.chemitech.net.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://bv.huanxung.cn

JS:   // child_process / cluster 模块
来源：http://bd.szxytkj.cn

TS:   // child_process / cluster 模块
来源：http://pq.asd995.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://cm.nicolike.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://dq.jctech888.com.cn

Ruby: // fork 块
来源：http://la.shxzskj.cn

C#:   Parallel.For
来源：http://jy.bookmarksfly.cn

================================================================================
来源：http://re.huixiangedu.cn

P. 常用工具函数
来源：http://ma.bookmarksfly.cn

================================================================================
来源：http://iu.shxzskj.cn

[P01] 生成 UUID
来源：http://fa.chemitech.net.cn

Py:   str(uuid.uuid4())
来源：http://ps.huixiangedu.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://cy.bookmarksfly.cn

JS:   crypto.randomUUID()
来源：http://oq.bjjhwx.cn

TS:   crypto.randomUUID()
来源：http://jv.chemitech.net.cn

Java: UUID.randomUUID().toString()
来源：http://hs.shxzskj.cn

Go:   // 用 github.com/google/uuid
来源：http://ub.hnjuh.cn

Ruby: SecureRandom.uuid
来源：http://ri.szsharing.cn

C#:   Guid.NewGuid().ToString()
来源：http://do.szsharing.cn

[P02] MD5 / SHA256 摘要
来源：http://up.bookmarksfly.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://rr.muxihuayi.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://vq.bookmarksfly.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ua.colortex.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ld.bjjhwx.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://cf.yuntaijiaju.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ly.jctech888.com.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://jf.nszjky.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ok.muxihuayi.cn

[P03] 生成短随机字符串
来源：http://uh.huixiangedu.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://cs.huixinmuqiang.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://se.newstarts.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wg.chemitech.net.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://dr.szsharing.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://to.chemitech.net.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://dx.szsharing.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://xx.jctech888.com.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://bt.huixinmuqiang.cn

[P04] 求长度
来源：http://bg.521024.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://vi.shtwfgs.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ga.yuexingan06.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://vn.szxytkj.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hy.nszjky.cn

Java: list.size();  map.size();  s.length()
来源：http://xw.gzmigu.cn

Go:   len(arr);  len(m)
来源：http://gs.chemitech.net.cn

Ruby: x.length;  x.size
来源：http://rd.jianghongdianzi.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://gl.jctech888.com.cn

[P05] 判断两个对象内容是否相等
来源：http://ge.shxzukj.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://wo.huixinmuqiang.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mx.hahajie.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://if.szxytkj.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://nz.gzmigu.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://im.szxytkj.cn

Go:   reflect.DeepEqual(a, b)
来源：http://py.jctech888.com.cn

Ruby: a == b
来源：http://zs.wgjwhj.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mz.hahajie.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://fd.jianghongdianzi.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://lo.huixiangedu.cn

PHP:  if (empty($x)) {}
来源：http://ho.lnxyls.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://oa.colortex.cn

TS:   if (x == null) {}
来源：http://kr.521024.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://pu.wgjwhj.cn

Go:   if x == nil {}
来源：http://ah.nszjky.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://tt.hnjuh.cn

C#:   if (x is null) {}
来源：http://fk.nicolike.cn

[P07] 防抖与节流
来源：http://me.panjiajie.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://km.bjjhwx.cn

PHP:  // 手写时间戳比较
来源：http://se.newstarts.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://si.yuexingan06.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ta.gzmigu.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://xi.chemitech.net.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ce.newstarts.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://py.asd995.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://my.shtwfgs.cn

[P08] 处理浮点精度问题
来源：http://vp.nicolike.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://fu.huixiangedu.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://bj.huixinmuqiang.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://sa.hahajie.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://co.huanxung.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wh.wgjwhj.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ac.shxzskj.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://qh.huixinmuqiang.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://jt.shxzukj.cn

================================================================================
来源：http://bz.nicolike.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://xy.szsharing.cn

================================================================================
来源：http://ds.huanxung.cn

[Q01] 创建表
来源：http://ft.haigaiapp.cn

CREATE TABLE users (
来源：http://in.muxihuayi.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://qw.szxytkj.cn

name VARCHAR(50) NOT NULL,
来源：http://ar.haigaiapp.cn

email VARCHAR(100) UNIQUE,
来源：http://mu.lnxyls.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://kh.gzmigu.cn

);
来源：http://cf.lnxyls.cn

[Q02] 创建带外键的表
来源：http://te.shtwfgs.cn

CREATE TABLE orders (
来源：http://jr.wgjwhj.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://oy.huixiangedu.cn

user_id INT NOT NULL,
来源：http://av.hahajie.cn

amount DECIMAL(10, 2),
来源：http://am.panjiajie.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://or.muxihuayi.cn

);
来源：http://pd.szxytkj.cn

[Q03] 增加列
来源：http://ki.jianghongdianzi.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://lq.asd995.cn

[Q04] 修改列类型
来源：http://jb.shtwfgs.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://do.hnjuh.cn

[Q05] 重命名列
来源：http://dq.nicolike.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://tu.hahajie.cn

[Q06] 删除列
来源：http://aq.yuntaijiaju.cn

ALTER TABLE users DROP COLUMN age;
来源：http://bq.gzmigu.cn

[Q07] 删除表
来源：http://hz.huixiangedu.cn

DROP TABLE IF EXISTS orders;
来源：http://uv.gzmigu.cn

[Q08] 创建普通索引
来源：http://si.nszjky.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://ms.szxytkj.cn

[Q09] 创建唯一索引
来源：http://rs.szxytkj.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ze.panjiajie.cn

[Q10] 插入单行
来源：http://mt.colortex.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://zy.newstarts.cn

[Q11] 一次插入多行
来源：http://zb.9csxet.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ls.521024.cn

[Q12] 插入后取自增 ID
来源：http://fn.jctech888.com.cn

INSERT INTO users (name) VALUES ('C');
来源：http://dz.jianghongdianzi.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ti.yuexingan06.cn

[Q13] 忽略重复插入
来源：http://zk.haigaiapp.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mm.nicolike.cn

[Q14] 存在则更新（upsert）
来源：http://fw.gzmigu.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://dv.shxzskj.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mh.gzmigu.cn

[Q15] 查询全部
来源：http://yt.hnjuh.cn

SELECT * FROM users;
来源：http://qj.jianghongdianzi.cn

[Q16] 查询指定列
来源：http://di.jctech888.com.cn

SELECT id, name FROM users;
来源：http://sp.huanxung.cn

[Q17] 条件查询
来源：http://qw.nicolike.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ya.nszjky.cn

[Q18] 模糊匹配
来源：http://nv.521024.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mu.szsharing.cn

[Q19] 范围查询
来源：http://pr.bookmarksfly.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://rk.nicolike.cn

[Q20] IN 列表
来源：http://qn.shxzukj.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ka.panjiajie.cn

[Q21] 空值判断
来源：http://ez.jianghongdianzi.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://vb.haigaiapp.cn

[Q22] 排序
来源：http://rf.szxytkj.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://cy.9csxet.cn

[Q23] 分页
来源：http://ew.wgjwhj.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ml.shtwfgs.cn

[Q24] 去重
来源：http://yq.hnjuh.cn

SELECT DISTINCT city FROM users;
来源：http://nw.bookmarksfly.cn

[Q25] 只取前 N 条
来源：http://or.jianghongdianzi.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://nc.bjjhwx.cn

[Q26] 计数
来源：http://ag.lnxyls.cn

SELECT COUNT(*) FROM users;
来源：http://bs.muxihuayi.cn

[Q27] 条件计数
来源：http://me.chemitech.net.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://df.chemitech.net.cn

[Q28] 求和与平均
来源：http://pb.hahajie.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://xr.szxytkj.cn

[Q29] 最大最小值
来源：http://cg.hahajie.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://uj.lnxyls.cn

[Q30] 分组统计
来源：http://vx.newstarts.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://qr.bjjhwx.cn

[Q31] 分组后过滤
来源：http://mx.colortex.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://nu.jianghongdianzi.cn

[Q32] 分组拼接字符串
来源：http://gn.yuexingan06.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://li.yuntaijiaju.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wq.haigaiapp.cn

[Q33] 多列分组
来源：http://mw.shxzukj.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://bh.szxytkj.cn

[Q34] 每组取第一条
来源：http://ez.muxihuayi.cn

SELECT * FROM (
来源：http://nf.yuexingan06.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://vd.bookmarksfly.cn

) t WHERE rn = 1;
来源：http://fj.haigaiapp.cn

[Q35] 内连接
来源：http://lq.szsharing.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://eq.jctech888.com.cn

[Q36] 左连接
来源：http://km.yuexingan06.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ot.newstarts.cn

[Q37] 右连接
来源：http://bh.hnjuh.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://qn.yuexingan06.cn

[Q38] 全外连接（PostgreSQL）
来源：http://do.nicolike.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://de.huixinmuqiang.cn

[Q39] 自连接（查上下级）
来源：http://wp.yuexingan06.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://as.shtwfgs.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://xw.yuntaijiaju.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://sk.chemitech.net.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://zz.shxzskj.cn

[Q41] 多表连接
来源：http://io.haigaiapp.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://pr.wgjwhj.cn

JOIN users u ON u.id = o.user_id
来源：http://nl.wgjwhj.cn

JOIN products p ON p.id = o.product_id;
来源：http://vg.bookmarksfly.cn

[Q42] 连接条件附加过滤
来源：http://ue.chemitech.net.cn

SELECT u.name, o.amount FROM users u
来源：http://ot.haigaiapp.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://if.9csxet.cn

[Q43] 标量子查询
来源：http://pa.jctech888.com.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://sm.huixinmuqiang.cn

[Q44] IN 子查询
来源：http://hw.yuexingan06.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://gg.gzmigu.cn

[Q45] EXISTS 判断存在
来源：http://xa.panjiajie.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hf.jctech888.com.cn


<!-- 参考信息 -->