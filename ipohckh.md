代发 wailian999

JS:   s === [...s].reverse().join("")
来源：http://mh.huixinmuqiang.cn

TS:   s === [...s].reverse().join("")
来源：http://zn.wgjwhj.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wo.lnxyls.cn

Go:   // 双指针从两端比较
来源：http://mi.yuntaijiaju.cn

Ruby: s == s.reverse
来源：http://gm.bookmarksfly.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://xd.bookmarksfly.cn

[N07] 两数之和（返回下标）
来源：http://bt.jctech888.com.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wn.lnxyls.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://uj.lnxyls.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://az.asd995.cn

TS:   // 手写 Map<string, number>
来源：http://la.bjjhwx.cn

Java: // 手写 HashMap
来源：http://nq.yuntaijiaju.cn

Go:   // 手写 map[int]int
来源：http://nx.gzmigu.cn

Ruby: // 手写 Hash
来源：http://jj.szxytkj.cn

C#:   // 手写 Dictionary<int, int>
来源：http://dx.jianghongdianzi.cn

[N08] 生成全排列
来源：http://iq.huixiangedu.cn

Py:   itertools.permutations(arr)
来源：http://de.haigaiapp.cn

PHP:  // 手写递归交换
来源：http://pj.huanxung.cn

JS:   // 手写回溯递归
来源：http://yt.muxihuayi.cn

TS:   // 手写回溯递归
来源：http://af.bookmarksfly.cn

Java: // 手写回溯递归
来源：http://va.huanxung.cn

Go:   // 手写回溯递归
来源：http://dv.nszjky.cn

Ruby: arr.permutation.to_a
来源：http://od.hnjuh.cn

C#:   // 手写回溯递归
来源：http://es.newstarts.cn

[N09] 栈与队列
来源：http://ld.wgjwhj.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://xx.yuntaijiaju.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wb.bookmarksfly.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ls.haigaiapp.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://qk.szsharing.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://or.521024.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ej.huixiangedu.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ft.szxytkj.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://bq.shxzskj.cn

[N10] 链表节点定义
来源：http://hm.haigaiapp.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://jw.bookmarksfly.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://jz.gzmigu.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://kv.shxzskj.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://pu.panjiajie.cn

Java: class Node { int v; Node next; }
来源：http://zt.szsharing.cn

Go:   type Node struct { V int; Next *Node }
来源：http://qq.jctech888.com.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://sj.shtwfgs.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://of.9csxet.cn

[N11] 二叉树中序遍历
来源：http://xu.lnxyls.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://xc.hnjuh.cn

PHP:  // 手写递归函数
来源：http://vq.hnjuh.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ha.yuexingan06.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://rk.nicolike.cn

Java: // 手写递归
来源：http://zd.wgjwhj.cn

Go:   // 手写递归
来源：http://zj.yuntaijiaju.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hj.asd995.cn

C#:   // 手写递归
来源：http://go.yuexingan06.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://vi.huixinmuqiang.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://pn.huanxung.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://kk.hnjuh.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://pe.shxzukj.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ug.bjjhwx.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://fr.szxytkj.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://yb.yuntaijiaju.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://no.wgjwhj.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://xl.9csxet.cn

================================================================================
来源：http://yx.asd995.cn

O. 并发与异步
来源：http://ji.bookmarksfly.cn

================================================================================
来源：http://ll.wgjwhj.cn

[O01] 启动一个线程
来源：http://vf.newstarts.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://no.jctech888.com.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://zz.yuntaijiaju.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://er.chemitech.net.cn

TS:   // 同 JS
来源：http://up.nicolike.cn

Java: new Thread(() -> f()).start()
来源：http://ns.lnxyls.cn

Go:   go f()
来源：http://cz.hnjuh.cn

Ruby: Thread.new { f }
来源：http://hb.jctech888.com.cn

C#:   Task.Run(() => F());
来源：http://ev.nszjky.cn

[O02] 使用线程池
来源：http://op.szxytkj.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://lc.bookmarksfly.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://jk.muxihuayi.cn

JS:   // worker_threads 线程池
来源：http://tv.huanxung.cn

TS:   // worker_threads 线程池
来源：http://oo.szsharing.cn

Java: Executors.newFixedThreadPool(4)
来源：http://le.jctech888.com.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://kw.521024.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://tt.shxzukj.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://xc.panjiajie.cn

[O03] 加锁保护共享数据
来源：http://bg.hnjuh.cn

Py:   with lock: shared += 1
来源：http://hp.hnjuh.cn

PHP:  // 用 flock() 做文件锁
来源：http://ai.gzmigu.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://fb.yuexingan06.cn

TS:   // 同 JS
来源：http://my.bookmarksfly.cn

Java: synchronized (this) { shared++; }
来源：http://hi.9csxet.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://af.bjjhwx.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://pa.shtwfgs.cn

C#:   lock (gate) { shared++; }
来源：http://os.shxzukj.cn

[O04] 定义异步函数并等待
来源：http://us.jianghongdianzi.cn

Py:   async def f():⏎    await g()
来源：http://xr.bjjhwx.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://jm.521024.cn

JS:   async function f() { await g(); }
来源：http://zr.huanxung.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://zf.huanxung.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://at.haigaiapp.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://yw.shtwfgs.cn

Ruby: # 用 Fiber 或 async gem
来源：http://sf.huixinmuqiang.cn

C#:   async Task F() { await G(); }
来源：http://jo.lnxyls.cn

[O05] 并发执行并等待全部完成
来源：http://au.hnjuh.cn

Py:   asyncio.gather(*tasks)
来源：http://ke.asd995.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://yh.colortex.cn

JS:   await Promise.all(tasks)
来源：http://iv.huanxung.cn

TS:   await Promise.all(tasks)
来源：http://xb.szxytkj.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hx.asd995.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://kx.wgjwhj.cn

Ruby: threads.map(&:join)
来源：http://yz.szsharing.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://mq.jianghongdianzi.cn

[O06] 使用进程池
来源：http://em.colortex.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://tb.yuexingan06.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://ur.haigaiapp.cn

JS:   // child_process / cluster 模块
来源：http://st.szxytkj.cn

TS:   // child_process / cluster 模块
来源：http://pv.huanxung.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ny.yuexingan06.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://db.jctech888.com.cn

Ruby: // fork 块
来源：http://gb.nicolike.cn

C#:   Parallel.For
来源：http://kj.nszjky.cn

================================================================================
来源：http://ki.panjiajie.cn

P. 常用工具函数
来源：http://bt.huixinmuqiang.cn

================================================================================
来源：http://nf.lnxyls.cn

[P01] 生成 UUID
来源：http://qq.shxzskj.cn

Py:   str(uuid.uuid4())
来源：http://tv.haigaiapp.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mp.nszjky.cn

JS:   crypto.randomUUID()
来源：http://zh.lnxyls.cn

TS:   crypto.randomUUID()
来源：http://wp.newstarts.cn

Java: UUID.randomUUID().toString()
来源：http://xl.chemitech.net.cn

Go:   // 用 github.com/google/uuid
来源：http://qz.szsharing.cn

Ruby: SecureRandom.uuid
来源：http://lb.shtwfgs.cn

C#:   Guid.NewGuid().ToString()
来源：http://kl.shxzskj.cn

[P02] MD5 / SHA256 摘要
来源：http://on.wgjwhj.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://sr.shxzskj.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://hk.bjjhwx.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://bt.bookmarksfly.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://te.521024.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://dm.newstarts.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://re.hahajie.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hh.asd995.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://me.asd995.cn

[P03] 生成短随机字符串
来源：http://qg.jianghongdianzi.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ps.newstarts.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://tk.hnjuh.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://au.gzmigu.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://tk.shtwfgs.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ny.huixiangedu.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://bc.huanxung.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://gi.521024.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ve.huixinmuqiang.cn

[P04] 求长度
来源：http://rh.szsharing.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://qz.szsharing.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://xz.yuexingan06.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://cx.jianghongdianzi.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://zm.muxihuayi.cn

Java: list.size();  map.size();  s.length()
来源：http://ce.huanxung.cn

Go:   len(arr);  len(m)
来源：http://pt.colortex.cn

Ruby: x.length;  x.size
来源：http://lz.bjjhwx.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://ir.chemitech.net.cn

[P05] 判断两个对象内容是否相等
来源：http://nj.haigaiapp.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://fc.huanxung.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://xn.jianghongdianzi.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://kj.bookmarksfly.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://in.shtwfgs.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://up.newstarts.cn

Go:   reflect.DeepEqual(a, b)
来源：http://xs.yuexingan06.cn

Ruby: a == b
来源：http://fd.lnxyls.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://uz.hnjuh.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://lm.nicolike.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ck.hahajie.cn

PHP:  if (empty($x)) {}
来源：http://qt.hnjuh.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://jg.yuntaijiaju.cn

TS:   if (x == null) {}
来源：http://ua.wgjwhj.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://ul.nszjky.cn

Go:   if x == nil {}
来源：http://se.hahajie.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://qw.bookmarksfly.cn

C#:   if (x is null) {}
来源：http://gk.muxihuayi.cn

[P07] 防抖与节流
来源：http://de.lnxyls.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://dt.huanxung.cn

PHP:  // 手写时间戳比较
来源：http://nt.shxzukj.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ty.huixinmuqiang.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://rz.muxihuayi.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://bf.szxytkj.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://bk.colortex.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://js.szsharing.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ru.chemitech.net.cn

[P08] 处理浮点精度问题
来源：http://bx.bookmarksfly.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://iq.hahajie.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://eq.shxzukj.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://zg.newstarts.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://kg.newstarts.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://cs.yuexingan06.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ms.wgjwhj.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://cy.haigaiapp.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://uj.huixinmuqiang.cn

================================================================================
来源：http://ms.szxytkj.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://qh.colortex.cn

================================================================================
来源：http://mz.lnxyls.cn

[Q01] 创建表
来源：http://oj.hahajie.cn

CREATE TABLE users (
来源：http://ti.colortex.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://us.jianghongdianzi.cn

name VARCHAR(50) NOT NULL,
来源：http://mz.szsharing.cn

email VARCHAR(100) UNIQUE,
来源：http://gm.chemitech.net.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ds.colortex.cn

);
来源：http://ql.muxihuayi.cn

[Q02] 创建带外键的表
来源：http://nc.muxihuayi.cn

CREATE TABLE orders (
来源：http://cq.yuntaijiaju.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://fb.szxytkj.cn

user_id INT NOT NULL,
来源：http://mi.huixiangedu.cn

amount DECIMAL(10, 2),
来源：http://bo.wgjwhj.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://qg.szxytkj.cn

);
来源：http://om.bjjhwx.cn

[Q03] 增加列
来源：http://qf.wgjwhj.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://bz.huanxung.cn

[Q04] 修改列类型
来源：http://np.shxzukj.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://kx.yuexingan06.cn

[Q05] 重命名列
来源：http://yl.szsharing.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://kr.nicolike.cn

[Q06] 删除列
来源：http://ew.shxzskj.cn

ALTER TABLE users DROP COLUMN age;
来源：http://jn.gzmigu.cn

[Q07] 删除表
来源：http://bz.yuexingan06.cn

DROP TABLE IF EXISTS orders;
来源：http://ie.szsharing.cn

[Q08] 创建普通索引
来源：http://zj.hnjuh.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://rt.shxzukj.cn

[Q09] 创建唯一索引
来源：http://fa.colortex.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://bx.hahajie.cn

[Q10] 插入单行
来源：http://sb.shxzskj.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://nb.bjjhwx.cn

[Q11] 一次插入多行
来源：http://uq.huixinmuqiang.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ud.colortex.cn

[Q12] 插入后取自增 ID
来源：http://hw.huixinmuqiang.cn

INSERT INTO users (name) VALUES ('C');
来源：http://fq.9csxet.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wn.huanxung.cn

[Q13] 忽略重复插入
来源：http://yu.hahajie.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://tb.shxzskj.cn

[Q14] 存在则更新（upsert）
来源：http://wd.huanxung.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://bv.szsharing.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wy.521024.cn

[Q15] 查询全部
来源：http://dg.haigaiapp.cn

SELECT * FROM users;
来源：http://rf.nicolike.cn

[Q16] 查询指定列
来源：http://db.huanxung.cn

SELECT id, name FROM users;
来源：http://nd.nszjky.cn

[Q17] 条件查询
来源：http://un.9csxet.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ju.haigaiapp.cn

[Q18] 模糊匹配
来源：http://zj.yuntaijiaju.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ra.hahajie.cn

[Q19] 范围查询
来源：http://sb.wgjwhj.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hs.asd995.cn

[Q20] IN 列表
来源：http://kz.jianghongdianzi.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://sr.jctech888.com.cn

[Q21] 空值判断
来源：http://pf.haigaiapp.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://yu.chemitech.net.cn

[Q22] 排序
来源：http://ud.muxihuayi.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://cz.521024.cn

[Q23] 分页
来源：http://fa.hnjuh.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://tm.szxytkj.cn

[Q24] 去重
来源：http://as.hnjuh.cn

SELECT DISTINCT city FROM users;
来源：http://pz.huanxung.cn

[Q25] 只取前 N 条
来源：http://dd.colortex.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://eu.jctech888.com.cn

[Q26] 计数
来源：http://kr.jianghongdianzi.cn

SELECT COUNT(*) FROM users;
来源：http://or.szsharing.cn

[Q27] 条件计数
来源：http://kn.huanxung.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hu.nszjky.cn

[Q28] 求和与平均
来源：http://yv.haigaiapp.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://jk.huixiangedu.cn

[Q29] 最大最小值
来源：http://wd.nicolike.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://dg.shxzskj.cn

[Q30] 分组统计
来源：http://ap.nszjky.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://su.huixinmuqiang.cn

[Q31] 分组后过滤
来源：http://ac.nicolike.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://eb.huixiangedu.cn

[Q32] 分组拼接字符串
来源：http://hh.nszjky.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ey.szsharing.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://xk.huixinmuqiang.cn

[Q33] 多列分组
来源：http://gu.muxihuayi.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wn.panjiajie.cn

[Q34] 每组取第一条
来源：http://xr.gzmigu.cn

SELECT * FROM (
来源：http://pb.jctech888.com.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://yd.hahajie.cn

) t WHERE rn = 1;
来源：http://vu.wgjwhj.cn

[Q35] 内连接
来源：http://rs.huixinmuqiang.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ni.colortex.cn

[Q36] 左连接
来源：http://dw.shxzskj.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://nj.hahajie.cn

[Q37] 右连接
来源：http://ep.9csxet.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://tq.shxzskj.cn

[Q38] 全外连接（PostgreSQL）
来源：http://tz.colortex.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ri.wgjwhj.cn

[Q39] 自连接（查上下级）
来源：http://nk.wgjwhj.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://xg.huanxung.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wa.nszjky.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://ym.9csxet.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://zv.hnjuh.cn

[Q41] 多表连接
来源：http://jj.hahajie.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://fh.hnjuh.cn

JOIN users u ON u.id = o.user_id
来源：http://or.asd995.cn

JOIN products p ON p.id = o.product_id;
来源：http://zw.haigaiapp.cn

[Q42] 连接条件附加过滤
来源：http://af.huixinmuqiang.cn

SELECT u.name, o.amount FROM users u
来源：http://yn.asd995.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://bx.lnxyls.cn

[Q43] 标量子查询
来源：http://bq.hahajie.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://vr.jctech888.com.cn


<!-- 参考信息 -->