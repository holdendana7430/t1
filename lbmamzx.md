代发 wailian999

JS:   s === [...s].reverse().join("")
来源：http://wj.gzmigu.cn

TS:   s === [...s].reverse().join("")
来源：http://jz.nicolike.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://uu.yuntaijiaju.cn

Go:   // 双指针从两端比较
来源：http://yo.shxzskj.cn

Ruby: s == s.reverse
来源：http://my.wgjwhj.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://vf.wgjwhj.cn

[N07] 两数之和（返回下标）
来源：http://jx.9csxet.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wv.yuexingan06.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://oc.9csxet.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://oa.huanxung.cn

TS:   // 手写 Map<string, number>
来源：http://zf.lnxyls.cn

Java: // 手写 HashMap
来源：http://gm.hnjuh.cn

Go:   // 手写 map[int]int
来源：http://zz.huixiangedu.cn

Ruby: // 手写 Hash
来源：http://qa.hnjuh.cn

C#:   // 手写 Dictionary<int, int>
来源：http://wy.nicolike.cn

[N08] 生成全排列
来源：http://bz.yuntaijiaju.cn

Py:   itertools.permutations(arr)
来源：http://yn.gzmigu.cn

PHP:  // 手写递归交换
来源：http://df.colortex.cn

JS:   // 手写回溯递归
来源：http://rt.wgjwhj.cn

TS:   // 手写回溯递归
来源：http://mn.shtwfgs.cn

Java: // 手写回溯递归
来源：http://cv.huanxung.cn

Go:   // 手写回溯递归
来源：http://xi.colortex.cn

Ruby: arr.permutation.to_a
来源：http://az.szsharing.cn

C#:   // 手写回溯递归
来源：http://aa.shxzukj.cn

[N09] 栈与队列
来源：http://pf.colortex.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://gv.wgjwhj.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ga.shxzskj.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://jz.hnjuh.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://dm.chemitech.net.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wd.panjiajie.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://rv.colortex.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://sj.huixinmuqiang.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://xz.huixiangedu.cn

[N10] 链表节点定义
来源：http://oj.huixiangedu.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://pe.colortex.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://cn.huixiangedu.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://pe.huixinmuqiang.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://sw.szsharing.cn

Java: class Node { int v; Node next; }
来源：http://ue.lnxyls.cn

Go:   type Node struct { V int; Next *Node }
来源：http://gx.szsharing.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://lq.jctech888.com.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://sg.colortex.cn

[N11] 二叉树中序遍历
来源：http://eg.szsharing.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://it.haigaiapp.cn

PHP:  // 手写递归函数
来源：http://rs.chemitech.net.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://dc.colortex.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://qg.shxzukj.cn

Java: // 手写递归
来源：http://oz.shxzskj.cn

Go:   // 手写递归
来源：http://li.huixinmuqiang.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://rj.szxytkj.cn

C#:   // 手写递归
来源：http://ai.lnxyls.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://aa.bookmarksfly.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://on.huixiangedu.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://dl.muxihuayi.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://as.bookmarksfly.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://qu.gzmigu.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://kc.huixiangedu.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://sf.gzmigu.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.521024.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://pc.chemitech.net.cn

================================================================================
来源：http://ta.yuntaijiaju.cn

O. 并发与异步
来源：http://zr.nszjky.cn

================================================================================
来源：http://jf.9csxet.cn

[O01] 启动一个线程
来源：http://uz.chemitech.net.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://po.nszjky.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ko.yuntaijiaju.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://tv.gzmigu.cn

TS:   // 同 JS
来源：http://vm.colortex.cn

Java: new Thread(() -> f()).start()
来源：http://ku.asd995.cn

Go:   go f()
来源：http://wj.shxzukj.cn

Ruby: Thread.new { f }
来源：http://zy.szxytkj.cn

C#:   Task.Run(() => F());
来源：http://as.muxihuayi.cn

[O02] 使用线程池
来源：http://ji.asd995.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://xd.hnjuh.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://fx.bookmarksfly.cn

JS:   // worker_threads 线程池
来源：http://yu.yuexingan06.cn

TS:   // worker_threads 线程池
来源：http://eh.shxzukj.cn

Java: Executors.newFixedThreadPool(4)
来源：http://zx.colortex.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://xm.bookmarksfly.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ut.shxzskj.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://lu.gzmigu.cn

[O03] 加锁保护共享数据
来源：http://ln.9csxet.cn

Py:   with lock: shared += 1
来源：http://qn.huixinmuqiang.cn

PHP:  // 用 flock() 做文件锁
来源：http://nb.newstarts.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ur.szsharing.cn

TS:   // 同 JS
来源：http://by.nszjky.cn

Java: synchronized (this) { shared++; }
来源：http://ac.colortex.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ad.chemitech.net.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://bh.colortex.cn

C#:   lock (gate) { shared++; }
来源：http://mp.panjiajie.cn

[O04] 定义异步函数并等待
来源：http://sq.wgjwhj.cn

Py:   async def f():⏎    await g()
来源：http://xj.bookmarksfly.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://qp.lnxyls.cn

JS:   async function f() { await g(); }
来源：http://me.haigaiapp.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.yuexingan06.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://en.chemitech.net.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://nz.nszjky.cn

Ruby: # 用 Fiber 或 async gem
来源：http://qz.asd995.cn

C#:   async Task F() { await G(); }
来源：http://kp.lnxyls.cn

[O05] 并发执行并等待全部完成
来源：http://ya.lnxyls.cn

Py:   asyncio.gather(*tasks)
来源：http://kw.jianghongdianzi.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://el.jctech888.com.cn

JS:   await Promise.all(tasks)
来源：http://kw.szsharing.cn

TS:   await Promise.all(tasks)
来源：http://qs.9csxet.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://bh.9csxet.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wl.bookmarksfly.cn

Ruby: threads.map(&:join)
来源：http://qv.huanxung.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://ps.szxytkj.cn

[O06] 使用进程池
来源：http://ez.bookmarksfly.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hq.szxytkj.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://kn.jctech888.com.cn

JS:   // child_process / cluster 模块
来源：http://au.yuntaijiaju.cn

TS:   // child_process / cluster 模块
来源：http://mb.panjiajie.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://cz.bjjhwx.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://kp.szsharing.cn

Ruby: // fork 块
来源：http://jg.huixiangedu.cn

C#:   Parallel.For
来源：http://dt.yuexingan06.cn

================================================================================
来源：http://tv.muxihuayi.cn

P. 常用工具函数
来源：http://ad.nszjky.cn

================================================================================
来源：http://lb.huixiangedu.cn

[P01] 生成 UUID
来源：http://tz.lnxyls.cn

Py:   str(uuid.uuid4())
来源：http://zt.jctech888.com.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://sp.asd995.cn

JS:   crypto.randomUUID()
来源：http://pd.9csxet.cn

TS:   crypto.randomUUID()
来源：http://xn.panjiajie.cn

Java: UUID.randomUUID().toString()
来源：http://ny.szxytkj.cn

Go:   // 用 github.com/google/uuid
来源：http://ag.shxzukj.cn

Ruby: SecureRandom.uuid
来源：http://rw.hnjuh.cn

C#:   Guid.NewGuid().ToString()
来源：http://xh.jctech888.com.cn

[P02] MD5 / SHA256 摘要
来源：http://om.jctech888.com.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://jm.lnxyls.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://gk.jianghongdianzi.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://uv.9csxet.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hh.muxihuayi.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ks.huixinmuqiang.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ji.jctech888.com.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://za.wgjwhj.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://nj.hnjuh.cn

[P03] 生成短随机字符串
来源：http://qh.gzmigu.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://cu.panjiajie.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wl.szxytkj.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://uf.huixiangedu.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wk.521024.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ym.hnjuh.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://gp.wgjwhj.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://ty.szxytkj.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://dx.shtwfgs.cn

[P04] 求长度
来源：http://hm.jctech888.com.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://rx.jianghongdianzi.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://et.nszjky.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://lg.szsharing.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://il.huixiangedu.cn

Java: list.size();  map.size();  s.length()
来源：http://aa.haigaiapp.cn

Go:   len(arr);  len(m)
来源：http://wk.huixinmuqiang.cn

Ruby: x.length;  x.size
来源：http://nz.huixinmuqiang.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://ln.nszjky.cn

[P05] 判断两个对象内容是否相等
来源：http://zl.shtwfgs.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://fr.yuexingan06.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ne.wgjwhj.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ri.asd995.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://xv.wgjwhj.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://cy.asd995.cn

Go:   reflect.DeepEqual(a, b)
来源：http://cg.shxzukj.cn

Ruby: a == b
来源：http://yi.newstarts.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://bi.asd995.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ye.shtwfgs.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ty.hahajie.cn

PHP:  if (empty($x)) {}
来源：http://cq.9csxet.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://fh.hahajie.cn

TS:   if (x == null) {}
来源：http://gz.9csxet.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://cu.huixiangedu.cn

Go:   if x == nil {}
来源：http://jw.huixinmuqiang.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://kv.521024.cn

C#:   if (x is null) {}
来源：http://wl.szxytkj.cn

[P07] 防抖与节流
来源：http://es.muxihuayi.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://sl.panjiajie.cn

PHP:  // 手写时间戳比较
来源：http://lk.colortex.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://md.gzmigu.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://jc.newstarts.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://vw.bjjhwx.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://lh.hahajie.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://xx.yuexingan06.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://bm.yuntaijiaju.cn

[P08] 处理浮点精度问题
来源：http://hy.newstarts.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://bk.newstarts.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://lw.bookmarksfly.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://qv.huixinmuqiang.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://jy.jctech888.com.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://xs.shtwfgs.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://en.huixinmuqiang.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://lf.newstarts.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ut.521024.cn

================================================================================
来源：http://pp.gzmigu.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://jg.szsharing.cn

================================================================================
来源：http://cu.asd995.cn

[Q01] 创建表
来源：http://jq.muxihuayi.cn

CREATE TABLE users (
来源：http://tn.shxzukj.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://nz.yuexingan06.cn

name VARCHAR(50) NOT NULL,
来源：http://ns.huixiangedu.cn

email VARCHAR(100) UNIQUE,
来源：http://nd.yuexingan06.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://dx.gzmigu.cn

);
来源：http://rf.nszjky.cn

[Q02] 创建带外键的表
来源：http://pt.gzmigu.cn

CREATE TABLE orders (
来源：http://ep.colortex.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wm.huanxung.cn

user_id INT NOT NULL,
来源：http://mw.jianghongdianzi.cn

amount DECIMAL(10, 2),
来源：http://au.hahajie.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://jm.huixiangedu.cn

);
来源：http://pt.huanxung.cn

[Q03] 增加列
来源：http://hj.haigaiapp.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://iz.yuntaijiaju.cn

[Q04] 修改列类型
来源：http://lz.nszjky.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://tu.bookmarksfly.cn

[Q05] 重命名列
来源：http://jf.szxytkj.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://sq.yuexingan06.cn

[Q06] 删除列
来源：http://fl.newstarts.cn

ALTER TABLE users DROP COLUMN age;
来源：http://qc.szsharing.cn

[Q07] 删除表
来源：http://aq.wgjwhj.cn

DROP TABLE IF EXISTS orders;
来源：http://dd.huanxung.cn

[Q08] 创建普通索引
来源：http://cb.jctech888.com.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://ho.nicolike.cn

[Q09] 创建唯一索引
来源：http://zx.shxzskj.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hb.chemitech.net.cn

[Q10] 插入单行
来源：http://le.521024.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://iz.gzmigu.cn

[Q11] 一次插入多行
来源：http://qy.asd995.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ra.lnxyls.cn

[Q12] 插入后取自增 ID
来源：http://xs.521024.cn

INSERT INTO users (name) VALUES ('C');
来源：http://sm.yuexingan06.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://dz.chemitech.net.cn

[Q13] 忽略重复插入
来源：http://gm.panjiajie.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://oh.hahajie.cn

[Q14] 存在则更新（upsert）
来源：http://zx.shtwfgs.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ea.haigaiapp.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://kb.nszjky.cn

[Q15] 查询全部
来源：http://ch.gzmigu.cn

SELECT * FROM users;
来源：http://tm.szsharing.cn

[Q16] 查询指定列
来源：http://sv.nicolike.cn

SELECT id, name FROM users;
来源：http://if.huixiangedu.cn

[Q17] 条件查询
来源：http://yh.shxzskj.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://om.bjjhwx.cn

[Q18] 模糊匹配
来源：http://sz.yuexingan06.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ub.panjiajie.cn

[Q19] 范围查询
来源：http://cx.lnxyls.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://av.newstarts.cn

[Q20] IN 列表
来源：http://xt.hnjuh.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://gw.nszjky.cn

[Q21] 空值判断
来源：http://gn.yuexingan06.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://bv.shtwfgs.cn

[Q22] 排序
来源：http://fj.szsharing.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.haigaiapp.cn

[Q23] 分页
来源：http://gd.shtwfgs.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://oq.chemitech.net.cn

[Q24] 去重
来源：http://en.bjjhwx.cn

SELECT DISTINCT city FROM users;
来源：http://ok.muxihuayi.cn

[Q25] 只取前 N 条
来源：http://ry.bookmarksfly.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://tl.wgjwhj.cn

[Q26] 计数
来源：http://wd.yuexingan06.cn

SELECT COUNT(*) FROM users;
来源：http://rb.shxzskj.cn

[Q27] 条件计数
来源：http://qk.hahajie.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://gf.szxytkj.cn

[Q28] 求和与平均
来源：http://tn.yuexingan06.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://jm.huixinmuqiang.cn

[Q29] 最大最小值
来源：http://vn.wgjwhj.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://ps.jctech888.com.cn

[Q30] 分组统计
来源：http://tq.muxihuayi.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://nx.shxzukj.cn

[Q31] 分组后过滤
来源：http://in.huixiangedu.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://bu.huixinmuqiang.cn

[Q32] 分组拼接字符串
来源：http://sl.nicolike.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://jq.muxihuayi.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://or.asd995.cn

[Q33] 多列分组
来源：http://gz.yuexingan06.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://my.szsharing.cn

[Q34] 每组取第一条
来源：http://gw.haigaiapp.cn

SELECT * FROM (
来源：http://nn.nszjky.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://yl.9csxet.cn

) t WHERE rn = 1;
来源：http://vv.huixiangedu.cn

[Q35] 内连接
来源：http://oo.gzmigu.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://yy.hahajie.cn

[Q36] 左连接
来源：http://dh.shxzukj.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://uu.colortex.cn

[Q37] 右连接
来源：http://js.shxzukj.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://sh.9csxet.cn

[Q38] 全外连接（PostgreSQL）
来源：http://pa.yuexingan06.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ke.bjjhwx.cn

[Q39] 自连接（查上下级）
来源：http://qa.colortex.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://jl.hnjuh.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hk.shxzskj.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://hb.huixiangedu.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ey.yuexingan06.cn

[Q41] 多表连接
来源：http://jf.panjiajie.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://uf.huixiangedu.cn

JOIN users u ON u.id = o.user_id
来源：http://ug.shtwfgs.cn

JOIN products p ON p.id = o.product_id;
来源：http://ea.hahajie.cn

[Q42] 连接条件附加过滤
来源：http://cm.haigaiapp.cn

SELECT u.name, o.amount FROM users u
来源：http://te.huixinmuqiang.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://cb.shxzskj.cn

[Q43] 标量子查询
来源：http://et.muxihuayi.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mk.chemitech.net.cn


<!-- 参考信息 -->