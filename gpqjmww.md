代发 wailian999

Ruby: s == s.reverse
来源：http://oy.yuntaijiaju.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://fy.hahajie.cn

[N07] 两数之和（返回下标）
来源：http://vt.lnxyls.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://jw.szsharing.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://do.bjjhwx.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://bv.wgjwhj.cn

TS:   // 手写 Map<string, number>
来源：http://gz.asd995.cn

Java: // 手写 HashMap
来源：http://xr.huanxung.cn

Go:   // 手写 map[int]int
来源：http://vd.newstarts.cn

Ruby: // 手写 Hash
来源：http://eh.gzmigu.cn

C#:   // 手写 Dictionary<int, int>
来源：http://pu.bookmarksfly.cn

[N08] 生成全排列
来源：http://up.hahajie.cn

Py:   itertools.permutations(arr)
来源：http://uj.521024.cn

PHP:  // 手写递归交换
来源：http://xc.shxzskj.cn

JS:   // 手写回溯递归
来源：http://fa.9csxet.cn

TS:   // 手写回溯递归
来源：http://vt.yuexingan06.cn

Java: // 手写回溯递归
来源：http://qj.colortex.cn

Go:   // 手写回溯递归
来源：http://gv.haigaiapp.cn

Ruby: arr.permutation.to_a
来源：http://gy.yuexingan06.cn

C#:   // 手写回溯递归
来源：http://at.panjiajie.cn

[N09] 栈与队列
来源：http://fl.szsharing.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://iw.asd995.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://sp.nicolike.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://bh.nicolike.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://eb.huanxung.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://tb.yuexingan06.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ca.521024.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://sy.huixiangedu.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://tl.huixinmuqiang.cn

[N10] 链表节点定义
来源：http://nh.muxihuayi.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://qp.huixiangedu.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://nj.nicolike.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://tk.jctech888.com.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://fl.9csxet.cn

Java: class Node { int v; Node next; }
来源：http://di.huixinmuqiang.cn

Go:   type Node struct { V int; Next *Node }
来源：http://kb.newstarts.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://rz.haigaiapp.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://gc.nicolike.cn

[N11] 二叉树中序遍历
来源：http://qf.colortex.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://zk.hahajie.cn

PHP:  // 手写递归函数
来源：http://ip.colortex.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ro.jianghongdianzi.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ri.szsharing.cn

Java: // 手写递归
来源：http://zt.muxihuayi.cn

Go:   // 手写递归
来源：http://mc.jctech888.com.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://xz.9csxet.cn

C#:   // 手写递归
来源：http://zx.jianghongdianzi.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ya.szxytkj.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ff.bookmarksfly.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://jf.shtwfgs.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://jv.bookmarksfly.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://xs.hahajie.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ue.bjjhwx.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://xj.huixiangedu.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ml.panjiajie.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://nx.jianghongdianzi.cn

================================================================================
来源：http://rm.shxzskj.cn

O. 并发与异步
来源：http://rf.szsharing.cn

================================================================================
来源：http://wk.bookmarksfly.cn

[O01] 启动一个线程
来源：http://eg.yuntaijiaju.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mo.muxihuayi.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://bw.hnjuh.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://iy.gzmigu.cn

TS:   // 同 JS
来源：http://qx.yuntaijiaju.cn

Java: new Thread(() -> f()).start()
来源：http://jg.asd995.cn

Go:   go f()
来源：http://fx.shxzskj.cn

Ruby: Thread.new { f }
来源：http://sb.muxihuayi.cn

C#:   Task.Run(() => F());
来源：http://wc.huixiangedu.cn

[O02] 使用线程池
来源：http://qx.szsharing.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://sn.haigaiapp.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://bv.nszjky.cn

JS:   // worker_threads 线程池
来源：http://xz.huanxung.cn

TS:   // worker_threads 线程池
来源：http://il.newstarts.cn

Java: Executors.newFixedThreadPool(4)
来源：http://dv.gzmigu.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ro.gzmigu.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://rw.9csxet.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wu.shtwfgs.cn

[O03] 加锁保护共享数据
来源：http://sd.bookmarksfly.cn

Py:   with lock: shared += 1
来源：http://ox.szsharing.cn

PHP:  // 用 flock() 做文件锁
来源：http://aq.lnxyls.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://gb.jctech888.com.cn

TS:   // 同 JS
来源：http://sg.huixiangedu.cn

Java: synchronized (this) { shared++; }
来源：http://to.9csxet.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mb.shtwfgs.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://rm.gzmigu.cn

C#:   lock (gate) { shared++; }
来源：http://bz.9csxet.cn

[O04] 定义异步函数并等待
来源：http://oh.shxzskj.cn

Py:   async def f():⏎    await g()
来源：http://di.shtwfgs.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://sw.newstarts.cn

JS:   async function f() { await g(); }
来源：http://ua.bookmarksfly.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://az.shtwfgs.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://yq.shxzukj.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://yi.shxzskj.cn

Ruby: # 用 Fiber 或 async gem
来源：http://ca.hahajie.cn

C#:   async Task F() { await G(); }
来源：http://pi.huixinmuqiang.cn

[O05] 并发执行并等待全部完成
来源：http://yq.gzmigu.cn

Py:   asyncio.gather(*tasks)
来源：http://or.bookmarksfly.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://xr.nicolike.cn

JS:   await Promise.all(tasks)
来源：http://oj.panjiajie.cn

TS:   await Promise.all(tasks)
来源：http://iz.yuntaijiaju.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://sr.9csxet.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ox.lnxyls.cn

Ruby: threads.map(&:join)
来源：http://aq.jianghongdianzi.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://fb.newstarts.cn

[O06] 使用进程池
来源：http://cr.colortex.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ks.huixinmuqiang.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://cc.panjiajie.cn

JS:   // child_process / cluster 模块
来源：http://as.jianghongdianzi.cn

TS:   // child_process / cluster 模块
来源：http://wb.521024.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://tu.bookmarksfly.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hl.shxzukj.cn

Ruby: // fork 块
来源：http://gx.jctech888.com.cn

C#:   Parallel.For
来源：http://dr.yuexingan06.cn

================================================================================
来源：http://as.szsharing.cn

P. 常用工具函数
来源：http://qj.huixiangedu.cn

================================================================================
来源：http://qq.9csxet.cn

[P01] 生成 UUID
来源：http://ho.nicolike.cn

Py:   str(uuid.uuid4())
来源：http://qa.shtwfgs.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://da.jianghongdianzi.cn

JS:   crypto.randomUUID()
来源：http://lo.yuntaijiaju.cn

TS:   crypto.randomUUID()
来源：http://to.chemitech.net.cn

Java: UUID.randomUUID().toString()
来源：http://cy.huixinmuqiang.cn

Go:   // 用 github.com/google/uuid
来源：http://vm.huixiangedu.cn

Ruby: SecureRandom.uuid
来源：http://ub.lnxyls.cn

C#:   Guid.NewGuid().ToString()
来源：http://io.yuntaijiaju.cn

[P02] MD5 / SHA256 摘要
来源：http://gv.colortex.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://qm.9csxet.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://yh.asd995.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://vd.asd995.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wn.asd995.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://bq.hahajie.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://nn.szsharing.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ao.9csxet.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://kn.huixiangedu.cn

[P03] 生成短随机字符串
来源：http://fl.yuexingan06.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://yz.nszjky.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://zn.szxytkj.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://oe.9csxet.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://uv.muxihuayi.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://eu.wgjwhj.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ov.yuntaijiaju.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://xd.muxihuayi.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://jh.huanxung.cn

[P04] 求长度
来源：http://wv.huanxung.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wy.newstarts.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://qe.bookmarksfly.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wk.asd995.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hh.haigaiapp.cn

Java: list.size();  map.size();  s.length()
来源：http://im.lnxyls.cn

Go:   len(arr);  len(m)
来源：http://nr.hahajie.cn

Ruby: x.length;  x.size
来源：http://zh.lnxyls.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://zz.shxzskj.cn

[P05] 判断两个对象内容是否相等
来源：http://fe.lnxyls.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://gm.jianghongdianzi.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://on.bjjhwx.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mx.panjiajie.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://fd.bookmarksfly.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://zc.huixiangedu.cn

Go:   reflect.DeepEqual(a, b)
来源：http://gl.nicolike.cn

Ruby: a == b
来源：http://xo.nicolike.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://dh.9csxet.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://vk.bjjhwx.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://uf.szxytkj.cn

PHP:  if (empty($x)) {}
来源：http://ob.shtwfgs.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hx.muxihuayi.cn

TS:   if (x == null) {}
来源：http://mq.bjjhwx.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://vl.szxytkj.cn

Go:   if x == nil {}
来源：http://xv.newstarts.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://fk.wgjwhj.cn

C#:   if (x is null) {}
来源：http://yk.szxytkj.cn

[P07] 防抖与节流
来源：http://si.shtwfgs.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://vo.muxihuayi.cn

PHP:  // 手写时间戳比较
来源：http://lz.lnxyls.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://kr.huanxung.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://id.jianghongdianzi.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ki.yuntaijiaju.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://lb.huixiangedu.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://xz.panjiajie.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://qo.bjjhwx.cn

[P08] 处理浮点精度问题
来源：http://mg.shxzskj.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://st.muxihuayi.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://jo.9csxet.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://co.jctech888.com.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ov.haigaiapp.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://dq.jctech888.com.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://nc.wgjwhj.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ih.colortex.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://cq.9csxet.cn

================================================================================
来源：http://hj.wgjwhj.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://yf.hnjuh.cn

================================================================================
来源：http://vp.nszjky.cn

[Q01] 创建表
来源：http://mr.hahajie.cn

CREATE TABLE users (
来源：http://qo.hnjuh.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ei.jianghongdianzi.cn

name VARCHAR(50) NOT NULL,
来源：http://mp.9csxet.cn

email VARCHAR(100) UNIQUE,
来源：http://am.szxytkj.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ui.shxzukj.cn

);
来源：http://pt.yuntaijiaju.cn

[Q02] 创建带外键的表
来源：http://nk.colortex.cn

CREATE TABLE orders (
来源：http://ez.haigaiapp.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://nn.yuexingan06.cn

user_id INT NOT NULL,
来源：http://ry.lnxyls.cn

amount DECIMAL(10, 2),
来源：http://ze.huixiangedu.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://tj.shtwfgs.cn

);
来源：http://nm.chemitech.net.cn

[Q03] 增加列
来源：http://dq.shxzukj.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ti.jctech888.com.cn

[Q04] 修改列类型
来源：http://kh.panjiajie.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://iu.newstarts.cn

[Q05] 重命名列
来源：http://qi.hahajie.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://dh.lnxyls.cn

[Q06] 删除列
来源：http://na.haigaiapp.cn

ALTER TABLE users DROP COLUMN age;
来源：http://rw.huanxung.cn

[Q07] 删除表
来源：http://yn.shtwfgs.cn

DROP TABLE IF EXISTS orders;
来源：http://ud.muxihuayi.cn

[Q08] 创建普通索引
来源：http://zh.huanxung.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://jj.9csxet.cn

[Q09] 创建唯一索引
来源：http://jd.asd995.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ip.huixiangedu.cn

[Q10] 插入单行
来源：http://ne.521024.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://tt.shtwfgs.cn

[Q11] 一次插入多行
来源：http://js.521024.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://zx.jianghongdianzi.cn

[Q12] 插入后取自增 ID
来源：http://ca.hahajie.cn

INSERT INTO users (name) VALUES ('C');
来源：http://ho.lnxyls.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ka.haigaiapp.cn

[Q13] 忽略重复插入
来源：http://bw.yuexingan06.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://un.yuexingan06.cn

[Q14] 存在则更新（upsert）
来源：http://zt.hnjuh.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ii.colortex.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://yb.jianghongdianzi.cn

[Q15] 查询全部
来源：http://zo.lnxyls.cn

SELECT * FROM users;
来源：http://li.yuexingan06.cn

[Q16] 查询指定列
来源：http://dh.jctech888.com.cn

SELECT id, name FROM users;
来源：http://er.shxzskj.cn

[Q17] 条件查询
来源：http://og.bookmarksfly.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://td.521024.cn

[Q18] 模糊匹配
来源：http://ev.nszjky.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://bn.shxzskj.cn

[Q19] 范围查询
来源：http://jo.colortex.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://kz.lnxyls.cn

[Q20] IN 列表
来源：http://tr.shxzukj.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://qg.hnjuh.cn

[Q21] 空值判断
来源：http://xz.wgjwhj.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://el.hnjuh.cn

[Q22] 排序
来源：http://do.521024.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://zk.muxihuayi.cn

[Q23] 分页
来源：http://so.wgjwhj.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://sp.wgjwhj.cn

[Q24] 去重
来源：http://vd.hnjuh.cn

SELECT DISTINCT city FROM users;
来源：http://di.gzmigu.cn

[Q25] 只取前 N 条
来源：http://ml.chemitech.net.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://uw.asd995.cn

[Q26] 计数
来源：http://ab.colortex.cn

SELECT COUNT(*) FROM users;
来源：http://gc.panjiajie.cn

[Q27] 条件计数
来源：http://ql.hnjuh.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://fx.yuexingan06.cn

[Q28] 求和与平均
来源：http://gj.newstarts.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hu.nszjky.cn

[Q29] 最大最小值
来源：http://yk.muxihuayi.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://ll.newstarts.cn

[Q30] 分组统计
来源：http://bc.hnjuh.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mv.nicolike.cn

[Q31] 分组后过滤
来源：http://ti.shxzskj.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://js.newstarts.cn

[Q32] 分组拼接字符串
来源：http://fb.lnxyls.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://vo.yuexingan06.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://eu.hnjuh.cn

[Q33] 多列分组
来源：http://ur.chemitech.net.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://yi.colortex.cn

[Q34] 每组取第一条
来源：http://wo.yuexingan06.cn

SELECT * FROM (
来源：http://qr.szxytkj.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mv.shtwfgs.cn

) t WHERE rn = 1;
来源：http://iy.muxihuayi.cn

[Q35] 内连接
来源：http://qh.9csxet.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://bm.huixinmuqiang.cn

[Q36] 左连接
来源：http://nf.yuntaijiaju.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://yz.shxzukj.cn

[Q37] 右连接
来源：http://zu.huanxung.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://nz.asd995.cn

[Q38] 全外连接（PostgreSQL）
来源：http://bh.huixiangedu.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://em.haigaiapp.cn

[Q39] 自连接（查上下级）
来源：http://nn.jianghongdianzi.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://kf.nicolike.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mc.bookmarksfly.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://tr.huixinmuqiang.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://cz.lnxyls.cn

[Q41] 多表连接
来源：http://ov.lnxyls.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://kt.huixinmuqiang.cn

JOIN users u ON u.id = o.user_id
来源：http://fz.hahajie.cn

JOIN products p ON p.id = o.product_id;
来源：http://tp.521024.cn

[Q42] 连接条件附加过滤
来源：http://kr.szsharing.cn

SELECT u.name, o.amount FROM users u
来源：http://im.shxzskj.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://jv.yuexingan06.cn

[Q43] 标量子查询
来源：http://ak.bjjhwx.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ky.chemitech.net.cn

[Q44] IN 子查询
来源：http://mt.nszjky.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://xo.jctech888.com.cn

[Q45] EXISTS 判断存在
来源：http://ug.bjjhwx.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mj.nszjky.cn


<!-- 参考信息 -->