代发 wailian999

Ruby: s == s.reverse
来源：http://sw.jianghongdianzi.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://ew.hahajie.cn

[N07] 两数之和（返回下标）
来源：http://og.jianghongdianzi.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://qc.yuexingan06.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ln.panjiajie.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://kr.shxzskj.cn

TS:   // 手写 Map<string, number>
来源：http://ki.shtwfgs.cn

Java: // 手写 HashMap
来源：http://ja.9csxet.cn

Go:   // 手写 map[int]int
来源：http://wl.chemitech.net.cn

Ruby: // 手写 Hash
来源：http://iq.bjjhwx.cn

C#:   // 手写 Dictionary<int, int>
来源：http://nm.lnxyls.cn

[N08] 生成全排列
来源：http://go.yuexingan06.cn

Py:   itertools.permutations(arr)
来源：http://ba.bjjhwx.cn

PHP:  // 手写递归交换
来源：http://gw.panjiajie.cn

JS:   // 手写回溯递归
来源：http://wi.chemitech.net.cn

TS:   // 手写回溯递归
来源：http://km.bjjhwx.cn

Java: // 手写回溯递归
来源：http://qp.yuexingan06.cn

Go:   // 手写回溯递归
来源：http://wr.shtwfgs.cn

Ruby: arr.permutation.to_a
来源：http://to.yuntaijiaju.cn

C#:   // 手写回溯递归
来源：http://dw.lnxyls.cn

[N09] 栈与队列
来源：http://lk.hahajie.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://be.haigaiapp.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://bx.panjiajie.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://dd.muxihuayi.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://gb.jianghongdianzi.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://in.huanxung.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ps.521024.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ny.shxzukj.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ru.asd995.cn

[N10] 链表节点定义
来源：http://zz.lnxyls.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://sl.huixinmuqiang.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://yc.shxzskj.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://bf.jctech888.com.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://rg.szsharing.cn

Java: class Node { int v; Node next; }
来源：http://fm.huixinmuqiang.cn

Go:   type Node struct { V int; Next *Node }
来源：http://rv.jctech888.com.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://vp.hnjuh.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://gd.szxytkj.cn

[N11] 二叉树中序遍历
来源：http://yi.9csxet.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://qq.lnxyls.cn

PHP:  // 手写递归函数
来源：http://jv.gzmigu.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ys.hahajie.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://xf.hahajie.cn

Java: // 手写递归
来源：http://hp.jianghongdianzi.cn

Go:   // 手写递归
来源：http://qh.haigaiapp.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://zu.huanxung.cn

C#:   // 手写递归
来源：http://kk.hahajie.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://cg.szsharing.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://zd.521024.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://er.hnjuh.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://gu.newstarts.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://qs.hnjuh.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ts.yuexingan06.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://az.521024.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://rt.wgjwhj.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://zi.9csxet.cn

================================================================================
来源：http://ey.yuexingan06.cn

O. 并发与异步
来源：http://ez.lnxyls.cn

================================================================================
来源：http://kb.haigaiapp.cn

[O01] 启动一个线程
来源：http://vc.jctech888.com.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://rt.panjiajie.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://fr.hahajie.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://xs.jianghongdianzi.cn

TS:   // 同 JS
来源：http://eq.muxihuayi.cn

Java: new Thread(() -> f()).start()
来源：http://yz.jianghongdianzi.cn

Go:   go f()
来源：http://wv.chemitech.net.cn

Ruby: Thread.new { f }
来源：http://ev.jianghongdianzi.cn

C#:   Task.Run(() => F());
来源：http://kq.wgjwhj.cn

[O02] 使用线程池
来源：http://wn.lnxyls.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://as.huixiangedu.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://qy.hahajie.cn

JS:   // worker_threads 线程池
来源：http://fw.jianghongdianzi.cn

TS:   // worker_threads 线程池
来源：http://ys.yuntaijiaju.cn

Java: Executors.newFixedThreadPool(4)
来源：http://co.asd995.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://yi.huixinmuqiang.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ea.huixiangedu.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://xl.szxytkj.cn

[O03] 加锁保护共享数据
来源：http://sp.newstarts.cn

Py:   with lock: shared += 1
来源：http://be.nszjky.cn

PHP:  // 用 flock() 做文件锁
来源：http://em.shtwfgs.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://qo.nszjky.cn

TS:   // 同 JS
来源：http://qt.gzmigu.cn

Java: synchronized (this) { shared++; }
来源：http://ns.bookmarksfly.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://lz.yuexingan06.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://ji.nicolike.cn

C#:   lock (gate) { shared++; }
来源：http://az.yuexingan06.cn

[O04] 定义异步函数并等待
来源：http://ew.huanxung.cn

Py:   async def f():⏎    await g()
来源：http://rd.hnjuh.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://gi.shxzukj.cn

JS:   async function f() { await g(); }
来源：http://bu.haigaiapp.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://nc.szxytkj.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://xb.nszjky.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://iy.nszjky.cn

Ruby: # 用 Fiber 或 async gem
来源：http://fv.yuexingan06.cn

C#:   async Task F() { await G(); }
来源：http://ou.asd995.cn

[O05] 并发执行并等待全部完成
来源：http://gt.haigaiapp.cn

Py:   asyncio.gather(*tasks)
来源：http://gs.panjiajie.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://uq.szxytkj.cn

JS:   await Promise.all(tasks)
来源：http://fu.9csxet.cn

TS:   await Promise.all(tasks)
来源：http://xx.huixinmuqiang.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://kn.jctech888.com.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://di.wgjwhj.cn

Ruby: threads.map(&:join)
来源：http://uy.521024.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://be.shxzukj.cn

[O06] 使用进程池
来源：http://cw.bookmarksfly.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://te.gzmigu.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://tf.shtwfgs.cn

JS:   // child_process / cluster 模块
来源：http://bb.panjiajie.cn

TS:   // child_process / cluster 模块
来源：http://pi.nicolike.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ws.shxzukj.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://za.nszjky.cn

Ruby: // fork 块
来源：http://zz.asd995.cn

C#:   Parallel.For
来源：http://fm.hahajie.cn

================================================================================
来源：http://bi.jianghongdianzi.cn

P. 常用工具函数
来源：http://by.szsharing.cn

================================================================================
来源：http://mm.chemitech.net.cn

[P01] 生成 UUID
来源：http://nk.muxihuayi.cn

Py:   str(uuid.uuid4())
来源：http://px.huixinmuqiang.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://bx.9csxet.cn

JS:   crypto.randomUUID()
来源：http://gm.bjjhwx.cn

TS:   crypto.randomUUID()
来源：http://cy.asd995.cn

Java: UUID.randomUUID().toString()
来源：http://er.szsharing.cn

Go:   // 用 github.com/google/uuid
来源：http://oi.newstarts.cn

Ruby: SecureRandom.uuid
来源：http://fq.521024.cn

C#:   Guid.NewGuid().ToString()
来源：http://ql.yuexingan06.cn

[P02] MD5 / SHA256 摘要
来源：http://hp.bjjhwx.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://sd.yuntaijiaju.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://dc.muxihuayi.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://xx.nszjky.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://cq.hahajie.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ud.huixiangedu.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://af.chemitech.net.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ff.bjjhwx.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://tv.9csxet.cn

[P03] 生成短随机字符串
来源：http://eh.muxihuayi.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://yq.colortex.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wz.haigaiapp.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://za.521024.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://pz.huixiangedu.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://uc.bookmarksfly.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://rh.jctech888.com.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://jy.huanxung.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://gd.shxzskj.cn

[P04] 求长度
来源：http://rc.shxzukj.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wc.jctech888.com.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://rg.huanxung.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://tt.newstarts.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://re.chemitech.net.cn

Java: list.size();  map.size();  s.length()
来源：http://ob.huixinmuqiang.cn

Go:   len(arr);  len(m)
来源：http://nv.jctech888.com.cn

Ruby: x.length;  x.size
来源：http://rd.lnxyls.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://gu.hnjuh.cn

[P05] 判断两个对象内容是否相等
来源：http://oa.jianghongdianzi.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://yl.hnjuh.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hi.9csxet.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://cj.colortex.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://nw.jctech888.com.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ra.gzmigu.cn

Go:   reflect.DeepEqual(a, b)
来源：http://zl.jianghongdianzi.cn

Ruby: a == b
来源：http://al.bjjhwx.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://xv.yuntaijiaju.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://gm.yuexingan06.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ga.chemitech.net.cn

PHP:  if (empty($x)) {}
来源：http://de.shxzskj.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://fn.panjiajie.cn

TS:   if (x == null) {}
来源：http://rn.szsharing.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://nu.muxihuayi.cn

Go:   if x == nil {}
来源：http://gv.yuexingan06.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://tb.chemitech.net.cn

C#:   if (x is null) {}
来源：http://tw.haigaiapp.cn

[P07] 防抖与节流
来源：http://na.huanxung.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://pk.shxzskj.cn

PHP:  // 手写时间戳比较
来源：http://mr.wgjwhj.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ig.jianghongdianzi.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ia.shxzukj.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://rs.colortex.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wh.jianghongdianzi.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://dn.haigaiapp.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://nr.yuntaijiaju.cn

[P08] 处理浮点精度问题
来源：http://wc.9csxet.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ny.colortex.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://zd.hnjuh.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wi.shxzukj.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ah.huixinmuqiang.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hs.huixinmuqiang.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hr.huixinmuqiang.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://gy.shxzukj.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mr.shxzskj.cn

================================================================================
来源：http://dg.muxihuayi.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://fq.chemitech.net.cn

================================================================================
来源：http://tx.huixiangedu.cn

[Q01] 创建表
来源：http://ng.shxzukj.cn

CREATE TABLE users (
来源：http://gl.chemitech.net.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://zm.shtwfgs.cn

name VARCHAR(50) NOT NULL,
来源：http://gh.shtwfgs.cn

email VARCHAR(100) UNIQUE,
来源：http://wm.colortex.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://xi.huixinmuqiang.cn

);
来源：http://iq.shtwfgs.cn

[Q02] 创建带外键的表
来源：http://jy.wgjwhj.cn

CREATE TABLE orders (
来源：http://tq.newstarts.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://kb.panjiajie.cn

user_id INT NOT NULL,
来源：http://wj.gzmigu.cn

amount DECIMAL(10, 2),
来源：http://zh.nszjky.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://sv.9csxet.cn

);
来源：http://fo.haigaiapp.cn

[Q03] 增加列
来源：http://zm.chemitech.net.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://xo.lnxyls.cn

[Q04] 修改列类型
来源：http://rx.huixinmuqiang.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://uy.9csxet.cn

[Q05] 重命名列
来源：http://cp.shtwfgs.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ad.asd995.cn

[Q06] 删除列
来源：http://jn.colortex.cn

ALTER TABLE users DROP COLUMN age;
来源：http://ct.huixinmuqiang.cn

[Q07] 删除表
来源：http://ka.hahajie.cn

DROP TABLE IF EXISTS orders;
来源：http://qg.hahajie.cn

[Q08] 创建普通索引
来源：http://qd.shtwfgs.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://nm.lnxyls.cn

[Q09] 创建唯一索引
来源：http://oe.lnxyls.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://kj.szxytkj.cn

[Q10] 插入单行
来源：http://ad.nicolike.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://si.szxytkj.cn

[Q11] 一次插入多行
来源：http://qg.szsharing.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://qm.nicolike.cn

[Q12] 插入后取自增 ID
来源：http://bo.huixinmuqiang.cn

INSERT INTO users (name) VALUES ('C');
来源：http://pz.shtwfgs.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://sr.huanxung.cn

[Q13] 忽略重复插入
来源：http://jf.huixiangedu.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://yw.yuexingan06.cn

[Q14] 存在则更新（upsert）
来源：http://xm.yuexingan06.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mp.nszjky.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hy.nszjky.cn

[Q15] 查询全部
来源：http://zj.chemitech.net.cn

SELECT * FROM users;
来源：http://lu.shtwfgs.cn

[Q16] 查询指定列
来源：http://dg.nszjky.cn

SELECT id, name FROM users;
来源：http://tt.yuntaijiaju.cn

[Q17] 条件查询
来源：http://or.muxihuayi.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ip.huixinmuqiang.cn

[Q18] 模糊匹配
来源：http://lo.lnxyls.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://iz.muxihuayi.cn

[Q19] 范围查询
来源：http://ly.shxzukj.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://nc.szsharing.cn

[Q20] IN 列表
来源：http://wn.newstarts.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://px.szsharing.cn

[Q21] 空值判断
来源：http://av.newstarts.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://vu.colortex.cn

[Q22] 排序
来源：http://cr.huixiangedu.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://gp.szsharing.cn

[Q23] 分页
来源：http://if.panjiajie.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ib.jianghongdianzi.cn

[Q24] 去重
来源：http://sq.shxzskj.cn

SELECT DISTINCT city FROM users;
来源：http://ed.wgjwhj.cn

[Q25] 只取前 N 条
来源：http://an.hnjuh.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hd.panjiajie.cn

[Q26] 计数
来源：http://gn.hahajie.cn

SELECT COUNT(*) FROM users;
来源：http://cz.shxzukj.cn

[Q27] 条件计数
来源：http://ym.shxzskj.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://zw.nicolike.cn

[Q28] 求和与平均
来源：http://rl.9csxet.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://df.muxihuayi.cn

[Q29] 最大最小值
来源：http://jo.colortex.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://bi.haigaiapp.cn

[Q30] 分组统计
来源：http://xq.asd995.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://eu.bookmarksfly.cn

[Q31] 分组后过滤
来源：http://ej.nicolike.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://zx.jianghongdianzi.cn

[Q32] 分组拼接字符串
来源：http://fg.shxzukj.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wn.szsharing.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://om.521024.cn

[Q33] 多列分组
来源：http://di.hahajie.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ji.colortex.cn

[Q34] 每组取第一条
来源：http://lm.szxytkj.cn

SELECT * FROM (
来源：http://vd.hnjuh.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://tn.bjjhwx.cn

) t WHERE rn = 1;
来源：http://rr.wgjwhj.cn

[Q35] 内连接
来源：http://oj.hahajie.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ec.bookmarksfly.cn

[Q36] 左连接
来源：http://ob.shxzukj.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ej.asd995.cn

[Q37] 右连接
来源：http://ja.jianghongdianzi.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ec.521024.cn

[Q38] 全外连接（PostgreSQL）
来源：http://iy.nicolike.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://sk.gzmigu.cn

[Q39] 自连接（查上下级）
来源：http://zs.shtwfgs.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://nx.jctech888.com.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://rp.panjiajie.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://dd.jianghongdianzi.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://qk.shtwfgs.cn

[Q41] 多表连接
来源：http://wl.nicolike.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://bh.lnxyls.cn

JOIN users u ON u.id = o.user_id
来源：http://zp.wgjwhj.cn

JOIN products p ON p.id = o.product_id;
来源：http://hs.wgjwhj.cn

[Q42] 连接条件附加过滤
来源：http://sx.muxihuayi.cn

SELECT u.name, o.amount FROM users u
来源：http://ma.huixiangedu.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://vz.jctech888.com.cn

[Q43] 标量子查询
来源：http://yw.panjiajie.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://jy.shtwfgs.cn

[Q44] IN 子查询
来源：http://fe.colortex.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mq.szxytkj.cn

[Q45] EXISTS 判断存在
来源：http://bu.gzmigu.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://im.newstarts.cn


<!-- 参考信息 -->