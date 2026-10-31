代发 wailian999

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://cg.9csxet.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://zr.colortex.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://fj.asd995.cn

Ruby: a.gcd(b)
来源：http://rn.panjiajie.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://gu.shtwfgs.cn

[N06] 判断回文字符串
来源：http://ke.521024.cn

Py:   s == s[::-1]
来源：http://be.huixinmuqiang.cn

PHP:  $s === strrev($s);
来源：http://nn.szxytkj.cn

JS:   s === [...s].reverse().join("")
来源：http://ck.panjiajie.cn

TS:   s === [...s].reverse().join("")
来源：http://nh.lnxyls.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mz.shtwfgs.cn

Go:   // 双指针从两端比较
来源：http://yr.muxihuayi.cn

Ruby: s == s.reverse
来源：http://rp.nicolike.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://sp.huixiangedu.cn

[N07] 两数之和（返回下标）
来源：http://lb.lnxyls.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://oy.lnxyls.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://kd.newstarts.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://iv.haigaiapp.cn

TS:   // 手写 Map<string, number>
来源：http://cm.gzmigu.cn

Java: // 手写 HashMap
来源：http://is.chemitech.net.cn

Go:   // 手写 map[int]int
来源：http://hg.wgjwhj.cn

Ruby: // 手写 Hash
来源：http://br.hnjuh.cn

C#:   // 手写 Dictionary<int, int>
来源：http://qa.panjiajie.cn

[N08] 生成全排列
来源：http://fv.wgjwhj.cn

Py:   itertools.permutations(arr)
来源：http://ml.panjiajie.cn

PHP:  // 手写递归交换
来源：http://lh.yuntaijiaju.cn

JS:   // 手写回溯递归
来源：http://ru.bookmarksfly.cn

TS:   // 手写回溯递归
来源：http://yh.lnxyls.cn

Java: // 手写回溯递归
来源：http://zr.shxzskj.cn

Go:   // 手写回溯递归
来源：http://yx.gzmigu.cn

Ruby: arr.permutation.to_a
来源：http://us.szsharing.cn

C#:   // 手写回溯递归
来源：http://om.gzmigu.cn

[N09] 栈与队列
来源：http://wf.chemitech.net.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://nz.shxzukj.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://tm.jctech888.com.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://zt.colortex.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mj.nicolike.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://qs.yuntaijiaju.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://rn.521024.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://jw.lnxyls.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mr.haigaiapp.cn

[N10] 链表节点定义
来源：http://fi.shxzskj.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ej.shxzukj.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://mk.nszjky.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://qm.huixinmuqiang.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://fz.huixiangedu.cn

Java: class Node { int v; Node next; }
来源：http://ev.gzmigu.cn

Go:   type Node struct { V int; Next *Node }
来源：http://vg.9csxet.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://by.chemitech.net.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://ee.bookmarksfly.cn

[N11] 二叉树中序遍历
来源：http://gx.szsharing.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://eu.shtwfgs.cn

PHP:  // 手写递归函数
来源：http://gv.nicolike.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://dn.jianghongdianzi.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://qg.huixinmuqiang.cn

Java: // 手写递归
来源：http://zi.colortex.cn

Go:   // 手写递归
来源：http://ip.shxzskj.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://br.newstarts.cn

C#:   // 手写递归
来源：http://rl.asd995.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://dd.haigaiapp.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://td.szsharing.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://gp.muxihuayi.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://bc.szxytkj.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://yq.hahajie.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://js.huixiangedu.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://su.lnxyls.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://se.chemitech.net.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://tv.lnxyls.cn

================================================================================
来源：http://ul.huanxung.cn

O. 并发与异步
来源：http://ja.muxihuayi.cn

================================================================================
来源：http://ps.yuntaijiaju.cn

[O01] 启动一个线程
来源：http://bi.shtwfgs.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ce.haigaiapp.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ow.bookmarksfly.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hg.asd995.cn

TS:   // 同 JS
来源：http://yz.szxytkj.cn

Java: new Thread(() -> f()).start()
来源：http://rj.szxytkj.cn

Go:   go f()
来源：http://yv.panjiajie.cn

Ruby: Thread.new { f }
来源：http://lg.panjiajie.cn

C#:   Task.Run(() => F());
来源：http://yi.bjjhwx.cn

[O02] 使用线程池
来源：http://qd.bjjhwx.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://su.bjjhwx.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://kz.521024.cn

JS:   // worker_threads 线程池
来源：http://nj.szxytkj.cn

TS:   // worker_threads 线程池
来源：http://ma.newstarts.cn

Java: Executors.newFixedThreadPool(4)
来源：http://lj.lnxyls.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://rp.asd995.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://du.jianghongdianzi.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://zs.bjjhwx.cn

[O03] 加锁保护共享数据
来源：http://za.muxihuayi.cn

Py:   with lock: shared += 1
来源：http://vg.521024.cn

PHP:  // 用 flock() 做文件锁
来源：http://zz.szxytkj.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://vs.gzmigu.cn

TS:   // 同 JS
来源：http://as.asd995.cn

Java: synchronized (this) { shared++; }
来源：http://nm.521024.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hc.9csxet.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://eu.yuexingan06.cn

C#:   lock (gate) { shared++; }
来源：http://jo.szsharing.cn

[O04] 定义异步函数并等待
来源：http://od.szsharing.cn

Py:   async def f():⏎    await g()
来源：http://yw.lnxyls.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://bx.huixiangedu.cn

JS:   async function f() { await g(); }
来源：http://xa.yuexingan06.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://uh.huixinmuqiang.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ht.bookmarksfly.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://td.huixiangedu.cn

Ruby: # 用 Fiber 或 async gem
来源：http://fr.shxzskj.cn

C#:   async Task F() { await G(); }
来源：http://cm.haigaiapp.cn

[O05] 并发执行并等待全部完成
来源：http://lf.chemitech.net.cn

Py:   asyncio.gather(*tasks)
来源：http://uk.nszjky.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://zx.szxytkj.cn

JS:   await Promise.all(tasks)
来源：http://pv.jctech888.com.cn

TS:   await Promise.all(tasks)
来源：http://hc.bjjhwx.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://rj.nicolike.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://rd.shxzukj.cn

Ruby: threads.map(&:join)
来源：http://uu.hnjuh.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://eg.muxihuayi.cn

[O06] 使用进程池
来源：http://je.huixinmuqiang.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://gm.bookmarksfly.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://kt.newstarts.cn

JS:   // child_process / cluster 模块
来源：http://dk.yuntaijiaju.cn

TS:   // child_process / cluster 模块
来源：http://tg.shxzukj.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://nm.shtwfgs.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://al.asd995.cn

Ruby: // fork 块
来源：http://qe.colortex.cn

C#:   Parallel.For
来源：http://cm.hahajie.cn

================================================================================
来源：http://xc.szxytkj.cn

P. 常用工具函数
来源：http://fl.9csxet.cn

================================================================================
来源：http://ef.9csxet.cn

[P01] 生成 UUID
来源：http://pc.bjjhwx.cn

Py:   str(uuid.uuid4())
来源：http://qs.shtwfgs.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://oj.hahajie.cn

JS:   crypto.randomUUID()
来源：http://af.hnjuh.cn

TS:   crypto.randomUUID()
来源：http://ae.hahajie.cn

Java: UUID.randomUUID().toString()
来源：http://mo.colortex.cn

Go:   // 用 github.com/google/uuid
来源：http://vz.nicolike.cn

Ruby: SecureRandom.uuid
来源：http://yk.muxihuayi.cn

C#:   Guid.NewGuid().ToString()
来源：http://xd.521024.cn

[P02] MD5 / SHA256 摘要
来源：http://kb.newstarts.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ix.wgjwhj.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://eq.yuntaijiaju.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://qi.hahajie.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ku.huanxung.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://zm.lnxyls.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://zc.wgjwhj.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://tq.bjjhwx.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://uc.yuexingan06.cn

[P03] 生成短随机字符串
来源：http://wf.lnxyls.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ev.huixinmuqiang.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://im.chemitech.net.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://kg.newstarts.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://cm.newstarts.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://we.nszjky.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://no.shxzskj.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://rb.szsharing.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://tq.hnjuh.cn

[P04] 求长度
来源：http://zs.yuexingan06.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://vg.szsharing.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hp.bjjhwx.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://bs.colortex.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://gq.colortex.cn

Java: list.size();  map.size();  s.length()
来源：http://cy.lnxyls.cn

Go:   len(arr);  len(m)
来源：http://ba.huixiangedu.cn

Ruby: x.length;  x.size
来源：http://hl.huixiangedu.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://ao.chemitech.net.cn

[P05] 判断两个对象内容是否相等
来源：http://rn.nszjky.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://ze.521024.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://cm.haigaiapp.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://so.shxzukj.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ti.bjjhwx.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ap.chemitech.net.cn

Go:   reflect.DeepEqual(a, b)
来源：http://jg.muxihuayi.cn

Ruby: a == b
来源：http://vj.lnxyls.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://gt.hnjuh.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://lz.huixiangedu.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://an.bjjhwx.cn

PHP:  if (empty($x)) {}
来源：http://ck.9csxet.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://eo.huixiangedu.cn

TS:   if (x == null) {}
来源：http://lk.nszjky.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://mb.hahajie.cn

Go:   if x == nil {}
来源：http://ra.jianghongdianzi.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wq.haigaiapp.cn

C#:   if (x is null) {}
来源：http://gr.jianghongdianzi.cn

[P07] 防抖与节流
来源：http://vu.colortex.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://zb.nicolike.cn

PHP:  // 手写时间戳比较
来源：http://ia.colortex.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://kj.jianghongdianzi.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://fo.wgjwhj.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://vr.nszjky.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://zg.szsharing.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://mk.newstarts.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://qz.huixiangedu.cn

[P08] 处理浮点精度问题
来源：http://ey.huixinmuqiang.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ut.lnxyls.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://rf.hahajie.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://qh.gzmigu.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://jt.haigaiapp.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://bh.wgjwhj.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://tl.huanxung.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://oh.nszjky.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://aw.szxytkj.cn

================================================================================
来源：http://td.shtwfgs.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://pm.asd995.cn

================================================================================
来源：http://yr.hahajie.cn

[Q01] 创建表
来源：http://dk.hahajie.cn

CREATE TABLE users (
来源：http://sf.jianghongdianzi.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://zx.huanxung.cn

name VARCHAR(50) NOT NULL,
来源：http://kr.jianghongdianzi.cn

email VARCHAR(100) UNIQUE,
来源：http://fr.panjiajie.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ay.hahajie.cn

);
来源：http://ur.shtwfgs.cn

[Q02] 创建带外键的表
来源：http://th.521024.cn

CREATE TABLE orders (
来源：http://zm.jianghongdianzi.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://dt.9csxet.cn

user_id INT NOT NULL,
来源：http://lb.haigaiapp.cn

amount DECIMAL(10, 2),
来源：http://jm.panjiajie.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://cw.nicolike.cn

);
来源：http://pm.huixiangedu.cn

[Q03] 增加列
来源：http://ed.bookmarksfly.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://gn.nicolike.cn

[Q04] 修改列类型
来源：http://xj.szsharing.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://so.huixinmuqiang.cn

[Q05] 重命名列
来源：http://ms.asd995.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://zt.bookmarksfly.cn

[Q06] 删除列
来源：http://am.chemitech.net.cn

ALTER TABLE users DROP COLUMN age;
来源：http://ab.shtwfgs.cn

[Q07] 删除表
来源：http://sh.yuexingan06.cn

DROP TABLE IF EXISTS orders;
来源：http://yf.hahajie.cn

[Q08] 创建普通索引
来源：http://lx.bjjhwx.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://xk.lnxyls.cn

[Q09] 创建唯一索引
来源：http://rg.hahajie.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://qj.szxytkj.cn

[Q10] 插入单行
来源：http://uj.colortex.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://vg.szxytkj.cn

[Q11] 一次插入多行
来源：http://sb.gzmigu.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://jg.nicolike.cn

[Q12] 插入后取自增 ID
来源：http://hx.hahajie.cn

INSERT INTO users (name) VALUES ('C');
来源：http://ww.haigaiapp.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://rt.nicolike.cn

[Q13] 忽略重复插入
来源：http://sc.521024.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ge.asd995.cn

[Q14] 存在则更新（upsert）
来源：http://id.nszjky.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://zv.huixiangedu.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://zd.gzmigu.cn

[Q15] 查询全部
来源：http://ap.hnjuh.cn

SELECT * FROM users;
来源：http://ji.wgjwhj.cn

[Q16] 查询指定列
来源：http://dk.jianghongdianzi.cn

SELECT id, name FROM users;
来源：http://wx.haigaiapp.cn

[Q17] 条件查询
来源：http://cj.521024.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://zy.huixinmuqiang.cn

[Q18] 模糊匹配
来源：http://pd.colortex.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://iv.nszjky.cn

[Q19] 范围查询
来源：http://zn.jianghongdianzi.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mi.newstarts.cn

[Q20] IN 列表
来源：http://lb.szsharing.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://lv.panjiajie.cn

[Q21] 空值判断
来源：http://ad.nszjky.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://md.newstarts.cn

[Q22] 排序
来源：http://vo.9csxet.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ua.haigaiapp.cn

[Q23] 分页
来源：http://wx.9csxet.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://kw.wgjwhj.cn

[Q24] 去重
来源：http://wy.shxzskj.cn

SELECT DISTINCT city FROM users;
来源：http://mn.wgjwhj.cn

[Q25] 只取前 N 条
来源：http://zw.wgjwhj.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wz.jctech888.com.cn

[Q26] 计数
来源：http://xq.yuexingan06.cn

SELECT COUNT(*) FROM users;
来源：http://ub.chemitech.net.cn

[Q27] 条件计数
来源：http://di.nicolike.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wa.bjjhwx.cn

[Q28] 求和与平均
来源：http://sz.nszjky.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://jj.shxzskj.cn

[Q29] 最大最小值
来源：http://bi.asd995.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://sx.jianghongdianzi.cn

[Q30] 分组统计
来源：http://si.nszjky.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hh.yuexingan06.cn

[Q31] 分组后过滤
来源：http://ap.asd995.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://lk.hahajie.cn

[Q32] 分组拼接字符串
来源：http://rd.jianghongdianzi.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://rp.nicolike.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mm.newstarts.cn

[Q33] 多列分组
来源：http://to.bookmarksfly.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://vh.gzmigu.cn

[Q34] 每组取第一条
来源：http://uv.haigaiapp.cn

SELECT * FROM (
来源：http://yb.chemitech.net.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://vk.yuexingan06.cn

) t WHERE rn = 1;
来源：http://ab.chemitech.net.cn

[Q35] 内连接
来源：http://ke.chemitech.net.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://oc.huixiangedu.cn

[Q36] 左连接
来源：http://zl.huixinmuqiang.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://el.bookmarksfly.cn

[Q37] 右连接
来源：http://eh.jianghongdianzi.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hm.yuexingan06.cn

[Q38] 全外连接（PostgreSQL）
来源：http://pa.gzmigu.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://tg.bookmarksfly.cn

[Q39] 自连接（查上下级）
来源：http://fg.huixiangedu.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://pt.521024.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://nq.nicolike.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://nf.huanxung.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://gb.gzmigu.cn

[Q41] 多表连接
来源：http://em.bjjhwx.cn


<!-- 参考信息 -->