代发 wailian999

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://li.panjiajie.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://yj.colortex.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://pm.lnxyls.cn

Ruby: a.gcd(b)
来源：http://fr.shxzskj.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://lq.lnxyls.cn

[N06] 判断回文字符串
来源：http://jt.jianghongdianzi.cn

Py:   s == s[::-1]
来源：http://gy.shxzskj.cn

PHP:  $s === strrev($s);
来源：http://pc.521024.cn

JS:   s === [...s].reverse().join("")
来源：http://rn.panjiajie.cn

TS:   s === [...s].reverse().join("")
来源：http://au.huanxung.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://dh.hnjuh.cn

Go:   // 双指针从两端比较
来源：http://hq.yuntaijiaju.cn

Ruby: s == s.reverse
来源：http://mx.nicolike.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://pe.huixinmuqiang.cn

[N07] 两数之和（返回下标）
来源：http://wr.asd995.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://fq.panjiajie.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://tj.jctech888.com.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://eg.bjjhwx.cn

TS:   // 手写 Map<string, number>
来源：http://ws.haigaiapp.cn

Java: // 手写 HashMap
来源：http://jb.nszjky.cn

Go:   // 手写 map[int]int
来源：http://og.bookmarksfly.cn

Ruby: // 手写 Hash
来源：http://pc.nszjky.cn

C#:   // 手写 Dictionary<int, int>
来源：http://pa.bookmarksfly.cn

[N08] 生成全排列
来源：http://zw.lnxyls.cn

Py:   itertools.permutations(arr)
来源：http://gr.wgjwhj.cn

PHP:  // 手写递归交换
来源：http://zf.haigaiapp.cn

JS:   // 手写回溯递归
来源：http://sv.chemitech.net.cn

TS:   // 手写回溯递归
来源：http://je.bjjhwx.cn

Java: // 手写回溯递归
来源：http://rg.jctech888.com.cn

Go:   // 手写回溯递归
来源：http://sf.nszjky.cn

Ruby: arr.permutation.to_a
来源：http://gp.bookmarksfly.cn

C#:   // 手写回溯递归
来源：http://dm.yuexingan06.cn

[N09] 栈与队列
来源：http://oy.shxzukj.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://gc.521024.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://uh.nicolike.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wl.szsharing.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ca.gzmigu.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://qf.521024.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wx.jctech888.com.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://zi.nszjky.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://kj.shxzukj.cn

[N10] 链表节点定义
来源：http://yj.hahajie.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://xv.panjiajie.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://rb.asd995.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ee.shtwfgs.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://sq.hahajie.cn

Java: class Node { int v; Node next; }
来源：http://ki.asd995.cn

Go:   type Node struct { V int; Next *Node }
来源：http://vp.hnjuh.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://uc.huixiangedu.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://qr.wgjwhj.cn

[N11] 二叉树中序遍历
来源：http://vy.huixiangedu.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://jv.nszjky.cn

PHP:  // 手写递归函数
来源：http://pp.panjiajie.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ow.bjjhwx.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://kp.hahajie.cn

Java: // 手写递归
来源：http://za.jianghongdianzi.cn

Go:   // 手写递归
来源：http://ou.nicolike.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://qc.nszjky.cn

C#:   // 手写递归
来源：http://fb.newstarts.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://bs.szxytkj.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://oo.muxihuayi.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ds.jianghongdianzi.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://pd.chemitech.net.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ew.shxzskj.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://pi.jctech888.com.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://rv.haigaiapp.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mu.szxytkj.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://vn.yuexingan06.cn

================================================================================
来源：http://is.521024.cn

O. 并发与异步
来源：http://xs.shxzskj.cn

================================================================================
来源：http://pz.jianghongdianzi.cn

[O01] 启动一个线程
来源：http://ek.asd995.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://bm.nszjky.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://jb.nicolike.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://se.chemitech.net.cn

TS:   // 同 JS
来源：http://hz.huanxung.cn

Java: new Thread(() -> f()).start()
来源：http://ku.bjjhwx.cn

Go:   go f()
来源：http://jj.shtwfgs.cn

Ruby: Thread.new { f }
来源：http://sd.shxzskj.cn

C#:   Task.Run(() => F());
来源：http://ee.hnjuh.cn

[O02] 使用线程池
来源：http://zm.yuntaijiaju.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://zt.panjiajie.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://an.521024.cn

JS:   // worker_threads 线程池
来源：http://st.shxzskj.cn

TS:   // worker_threads 线程池
来源：http://pn.szsharing.cn

Java: Executors.newFixedThreadPool(4)
来源：http://rd.szsharing.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://br.asd995.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://oo.shxzskj.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://va.wgjwhj.cn

[O03] 加锁保护共享数据
来源：http://tt.haigaiapp.cn

Py:   with lock: shared += 1
来源：http://pd.chemitech.net.cn

PHP:  // 用 flock() 做文件锁
来源：http://nx.gzmigu.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wb.muxihuayi.cn

TS:   // 同 JS
来源：http://uh.haigaiapp.cn

Java: synchronized (this) { shared++; }
来源：http://bv.haigaiapp.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://vt.yuntaijiaju.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://cf.gzmigu.cn

C#:   lock (gate) { shared++; }
来源：http://xj.chemitech.net.cn

[O04] 定义异步函数并等待
来源：http://ge.huixiangedu.cn

Py:   async def f():⏎    await g()
来源：http://qs.yuntaijiaju.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://kx.jianghongdianzi.cn

JS:   async function f() { await g(); }
来源：http://nk.yuexingan06.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://yq.lnxyls.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://iu.huanxung.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ck.chemitech.net.cn

Ruby: # 用 Fiber 或 async gem
来源：http://ve.shxzukj.cn

C#:   async Task F() { await G(); }
来源：http://gr.shxzukj.cn

[O05] 并发执行并等待全部完成
来源：http://hz.wgjwhj.cn

Py:   asyncio.gather(*tasks)
来源：http://hy.yuntaijiaju.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ut.yuexingan06.cn

JS:   await Promise.all(tasks)
来源：http://ob.szsharing.cn

TS:   await Promise.all(tasks)
来源：http://sh.gzmigu.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://vs.asd995.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://qn.huanxung.cn

Ruby: threads.map(&:join)
来源：http://bw.chemitech.net.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://wo.yuexingan06.cn

[O06] 使用进程池
来源：http://iz.jianghongdianzi.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://oe.9csxet.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://fe.shxzukj.cn

JS:   // child_process / cluster 模块
来源：http://jb.szxytkj.cn

TS:   // child_process / cluster 模块
来源：http://xy.szxytkj.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://yt.yuexingan06.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://zl.bjjhwx.cn

Ruby: // fork 块
来源：http://yt.nicolike.cn

C#:   Parallel.For
来源：http://je.szsharing.cn

================================================================================
来源：http://fp.asd995.cn

P. 常用工具函数
来源：http://kz.colortex.cn

================================================================================
来源：http://ui.nszjky.cn

[P01] 生成 UUID
来源：http://ic.hahajie.cn

Py:   str(uuid.uuid4())
来源：http://ex.shxzskj.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://xr.muxihuayi.cn

JS:   crypto.randomUUID()
来源：http://my.jianghongdianzi.cn

TS:   crypto.randomUUID()
来源：http://zm.jianghongdianzi.cn

Java: UUID.randomUUID().toString()
来源：http://wh.yuntaijiaju.cn

Go:   // 用 github.com/google/uuid
来源：http://ko.yuexingan06.cn

Ruby: SecureRandom.uuid
来源：http://km.colortex.cn

C#:   Guid.NewGuid().ToString()
来源：http://go.chemitech.net.cn

[P02] MD5 / SHA256 摘要
来源：http://gm.lnxyls.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://jq.yuexingan06.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://bx.jianghongdianzi.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://bv.bookmarksfly.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://rb.nszjky.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://as.521024.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://fg.huixinmuqiang.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wg.szsharing.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ig.szxytkj.cn

[P03] 生成短随机字符串
来源：http://cg.hahajie.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://uo.gzmigu.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://un.huixinmuqiang.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ga.shtwfgs.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://gp.bjjhwx.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://en.yuexingan06.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wp.jctech888.com.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://hl.shxzukj.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ui.jianghongdianzi.cn

[P04] 求长度
来源：http://wm.hahajie.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://uk.yuntaijiaju.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://qf.bookmarksfly.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://eg.yuntaijiaju.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mh.newstarts.cn

Java: list.size();  map.size();  s.length()
来源：http://vq.lnxyls.cn

Go:   len(arr);  len(m)
来源：http://ex.huanxung.cn

Ruby: x.length;  x.size
来源：http://er.bookmarksfly.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://wy.colortex.cn

[P05] 判断两个对象内容是否相等
来源：http://rd.huixiangedu.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://nt.yuntaijiaju.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://jq.yuntaijiaju.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://tv.hahajie.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://en.shxzskj.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ch.yuexingan06.cn

Go:   reflect.DeepEqual(a, b)
来源：http://ql.huanxung.cn

Ruby: a == b
来源：http://yt.bjjhwx.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://zi.szsharing.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ul.nszjky.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ym.9csxet.cn

PHP:  if (empty($x)) {}
来源：http://il.yuexingan06.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mg.hahajie.cn

TS:   if (x == null) {}
来源：http://vg.nszjky.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://bg.shxzskj.cn

Go:   if x == nil {}
来源：http://qt.bjjhwx.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ag.9csxet.cn

C#:   if (x is null) {}
来源：http://uk.nicolike.cn

[P07] 防抖与节流
来源：http://bt.9csxet.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ce.yuexingan06.cn

PHP:  // 手写时间戳比较
来源：http://ne.hnjuh.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wv.hnjuh.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qa.muxihuayi.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://jx.nicolike.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://kd.haigaiapp.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://te.shxzukj.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hc.521024.cn

[P08] 处理浮点精度问题
来源：http://yq.shtwfgs.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://lz.newstarts.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://js.hahajie.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://nz.wgjwhj.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://cc.nszjky.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ho.shxzskj.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://xc.szsharing.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wc.bookmarksfly.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://pc.jianghongdianzi.cn

================================================================================
来源：http://pz.szxytkj.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://tn.nszjky.cn

================================================================================
来源：http://ks.lnxyls.cn

[Q01] 创建表
来源：http://ct.yuexingan06.cn

CREATE TABLE users (
来源：http://yd.huanxung.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://kh.hnjuh.cn

name VARCHAR(50) NOT NULL,
来源：http://fd.jctech888.com.cn

email VARCHAR(100) UNIQUE,
来源：http://jl.newstarts.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://lv.nicolike.cn

);
来源：http://lk.yuexingan06.cn

[Q02] 创建带外键的表
来源：http://bl.hahajie.cn

CREATE TABLE orders (
来源：http://qe.newstarts.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ow.shxzskj.cn

user_id INT NOT NULL,
来源：http://wi.521024.cn

amount DECIMAL(10, 2),
来源：http://le.shxzukj.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://rl.hnjuh.cn

);
来源：http://jr.hnjuh.cn

[Q03] 增加列
来源：http://fy.huixiangedu.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://zx.szsharing.cn

[Q04] 修改列类型
来源：http://zj.asd995.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ky.bookmarksfly.cn

[Q05] 重命名列
来源：http://zh.shxzskj.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://cx.hnjuh.cn

[Q06] 删除列
来源：http://uw.jctech888.com.cn

ALTER TABLE users DROP COLUMN age;
来源：http://pe.jianghongdianzi.cn

[Q07] 删除表
来源：http://jw.jianghongdianzi.cn

DROP TABLE IF EXISTS orders;
来源：http://jg.chemitech.net.cn

[Q08] 创建普通索引
来源：http://ki.jianghongdianzi.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://qe.muxihuayi.cn

[Q09] 创建唯一索引
来源：http://ys.colortex.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ds.shxzskj.cn

[Q10] 插入单行
来源：http://lk.huixiangedu.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ef.jianghongdianzi.cn

[Q11] 一次插入多行
来源：http://gu.gzmigu.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://pb.wgjwhj.cn

[Q12] 插入后取自增 ID
来源：http://cc.panjiajie.cn

INSERT INTO users (name) VALUES ('C');
来源：http://rj.gzmigu.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hl.wgjwhj.cn

[Q13] 忽略重复插入
来源：http://tb.lnxyls.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://px.521024.cn

[Q14] 存在则更新（upsert）
来源：http://xo.szsharing.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hw.haigaiapp.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://vj.9csxet.cn

[Q15] 查询全部
来源：http://hm.haigaiapp.cn

SELECT * FROM users;
来源：http://cy.jianghongdianzi.cn

[Q16] 查询指定列
来源：http://ed.panjiajie.cn

SELECT id, name FROM users;
来源：http://xs.huixinmuqiang.cn

[Q17] 条件查询
来源：http://uy.hnjuh.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ge.bookmarksfly.cn

[Q18] 模糊匹配
来源：http://yj.hahajie.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://yt.huixinmuqiang.cn

[Q19] 范围查询
来源：http://ex.chemitech.net.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://fr.bookmarksfly.cn

[Q20] IN 列表
来源：http://cu.nszjky.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://eh.jctech888.com.cn

[Q21] 空值判断
来源：http://yt.gzmigu.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://aq.yuntaijiaju.cn

[Q22] 排序
来源：http://hv.szsharing.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://yx.shxzukj.cn

[Q23] 分页
来源：http://hp.hnjuh.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://bl.shxzukj.cn

[Q24] 去重
来源：http://nk.chemitech.net.cn

SELECT DISTINCT city FROM users;
来源：http://xi.shtwfgs.cn

[Q25] 只取前 N 条
来源：http://rp.yuntaijiaju.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ms.panjiajie.cn

[Q26] 计数
来源：http://ti.asd995.cn

SELECT COUNT(*) FROM users;
来源：http://wb.shxzukj.cn

[Q27] 条件计数
来源：http://tf.hahajie.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://yz.asd995.cn

[Q28] 求和与平均
来源：http://rr.shtwfgs.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://bm.jianghongdianzi.cn

[Q29] 最大最小值
来源：http://wo.hnjuh.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://wd.jctech888.com.cn

[Q30] 分组统计
来源：http://tu.9csxet.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://zj.shxzskj.cn

[Q31] 分组后过滤
来源：http://ig.jctech888.com.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ok.lnxyls.cn

[Q32] 分组拼接字符串
来源：http://mp.szxytkj.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ip.yuntaijiaju.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://xt.panjiajie.cn

[Q33] 多列分组
来源：http://hs.szsharing.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://zf.panjiajie.cn

[Q34] 每组取第一条
来源：http://ym.yuexingan06.cn

SELECT * FROM (
来源：http://wi.yuntaijiaju.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ta.huanxung.cn

) t WHERE rn = 1;
来源：http://kk.newstarts.cn

[Q35] 内连接
来源：http://yw.szxytkj.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://sx.9csxet.cn

[Q36] 左连接
来源：http://lv.shxzskj.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://dl.szsharing.cn

[Q37] 右连接
来源：http://qr.colortex.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ak.szxytkj.cn

[Q38] 全外连接（PostgreSQL）
来源：http://kn.nicolike.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://bd.hnjuh.cn

[Q39] 自连接（查上下级）
来源：http://gc.shxzukj.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://vl.shxzskj.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://bc.colortex.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://rk.hnjuh.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://pr.521024.cn

[Q41] 多表连接
来源：http://dj.yuexingan06.cn


<!-- 参考信息 -->