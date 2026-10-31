代发 wailian999

Py:   itertools.permutations(arr)
来源：http://hm.wgjwhj.cn

PHP:  // 手写递归交换
来源：http://lb.colortex.cn

JS:   // 手写回溯递归
来源：http://jx.huixiangedu.cn

TS:   // 手写回溯递归
来源：http://oc.gzmigu.cn

Java: // 手写回溯递归
来源：http://jx.shtwfgs.cn

Go:   // 手写回溯递归
来源：http://rt.shxzskj.cn

Ruby: arr.permutation.to_a
来源：http://oa.521024.cn

C#:   // 手写回溯递归
来源：http://vr.huixiangedu.cn

[N09] 栈与队列
来源：http://zf.hahajie.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://qn.colortex.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://xx.shxzukj.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ph.haigaiapp.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://pm.wgjwhj.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ac.hahajie.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ne.wgjwhj.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://fi.bookmarksfly.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://tv.newstarts.cn

[N10] 链表节点定义
来源：http://gt.shxzukj.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ru.9csxet.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://du.asd995.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://dh.haigaiapp.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://yo.panjiajie.cn

Java: class Node { int v; Node next; }
来源：http://el.shtwfgs.cn

Go:   type Node struct { V int; Next *Node }
来源：http://it.panjiajie.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://gt.colortex.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://qg.shxzskj.cn

[N11] 二叉树中序遍历
来源：http://rr.lnxyls.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://vj.nicolike.cn

PHP:  // 手写递归函数
来源：http://do.hahajie.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://zp.hnjuh.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ho.jctech888.com.cn

Java: // 手写递归
来源：http://bb.bookmarksfly.cn

Go:   // 手写递归
来源：http://yf.muxihuayi.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ct.huanxung.cn

C#:   // 手写递归
来源：http://zh.newstarts.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://io.jianghongdianzi.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ls.shxzskj.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ex.colortex.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://er.shxzukj.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://pd.gzmigu.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://kg.szsharing.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://vp.jianghongdianzi.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ir.gzmigu.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://vg.jianghongdianzi.cn

================================================================================
来源：http://nx.yuexingan06.cn

O. 并发与异步
来源：http://sj.nicolike.cn

================================================================================
来源：http://sg.hnjuh.cn

[O01] 启动一个线程
来源：http://jf.asd995.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://cm.huixiangedu.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://qq.panjiajie.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://lz.shxzskj.cn

TS:   // 同 JS
来源：http://hh.bookmarksfly.cn

Java: new Thread(() -> f()).start()
来源：http://lc.nszjky.cn

Go:   go f()
来源：http://rf.muxihuayi.cn

Ruby: Thread.new { f }
来源：http://iu.jctech888.com.cn

C#:   Task.Run(() => F());
来源：http://bd.nszjky.cn

[O02] 使用线程池
来源：http://mk.9csxet.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://lv.nszjky.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ll.shxzskj.cn

JS:   // worker_threads 线程池
来源：http://zc.bjjhwx.cn

TS:   // worker_threads 线程池
来源：http://ek.haigaiapp.cn

Java: Executors.newFixedThreadPool(4)
来源：http://hf.gzmigu.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://va.huixinmuqiang.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://bi.muxihuayi.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://rg.haigaiapp.cn

[O03] 加锁保护共享数据
来源：http://ug.huanxung.cn

Py:   with lock: shared += 1
来源：http://ou.newstarts.cn

PHP:  // 用 flock() 做文件锁
来源：http://lf.colortex.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://am.huanxung.cn

TS:   // 同 JS
来源：http://mt.panjiajie.cn

Java: synchronized (this) { shared++; }
来源：http://fm.szxytkj.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://jh.gzmigu.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://wn.szsharing.cn

C#:   lock (gate) { shared++; }
来源：http://wd.huixiangedu.cn

[O04] 定义异步函数并等待
来源：http://ol.yuexingan06.cn

Py:   async def f():⏎    await g()
来源：http://fk.newstarts.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://lc.hnjuh.cn

JS:   async function f() { await g(); }
来源：http://sl.chemitech.net.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://qo.yuntaijiaju.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ar.huanxung.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://nl.nszjky.cn

Ruby: # 用 Fiber 或 async gem
来源：http://bg.hahajie.cn

C#:   async Task F() { await G(); }
来源：http://qm.jianghongdianzi.cn

[O05] 并发执行并等待全部完成
来源：http://dk.muxihuayi.cn

Py:   asyncio.gather(*tasks)
来源：http://zj.yuntaijiaju.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://al.chemitech.net.cn

JS:   await Promise.all(tasks)
来源：http://sc.shxzukj.cn

TS:   await Promise.all(tasks)
来源：http://us.yuexingan06.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://xq.gzmigu.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mf.521024.cn

Ruby: threads.map(&:join)
来源：http://pc.bookmarksfly.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://uu.nszjky.cn

[O06] 使用进程池
来源：http://hh.panjiajie.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://et.gzmigu.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://kp.asd995.cn

JS:   // child_process / cluster 模块
来源：http://aw.shtwfgs.cn

TS:   // child_process / cluster 模块
来源：http://me.9csxet.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://di.yuexingan06.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ql.shxzskj.cn

Ruby: // fork 块
来源：http://ql.haigaiapp.cn

C#:   Parallel.For
来源：http://yt.nicolike.cn

================================================================================
来源：http://zt.szsharing.cn

P. 常用工具函数
来源：http://pb.9csxet.cn

================================================================================
来源：http://ny.shxzukj.cn

[P01] 生成 UUID
来源：http://fh.jctech888.com.cn

Py:   str(uuid.uuid4())
来源：http://fl.huixinmuqiang.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://tn.haigaiapp.cn

JS:   crypto.randomUUID()
来源：http://cg.szsharing.cn

TS:   crypto.randomUUID()
来源：http://fq.wgjwhj.cn

Java: UUID.randomUUID().toString()
来源：http://vr.szsharing.cn

Go:   // 用 github.com/google/uuid
来源：http://qm.bjjhwx.cn

Ruby: SecureRandom.uuid
来源：http://rb.colortex.cn

C#:   Guid.NewGuid().ToString()
来源：http://tk.521024.cn

[P02] MD5 / SHA256 摘要
来源：http://dc.shxzskj.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ri.nicolike.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://uu.shtwfgs.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://yj.newstarts.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://re.huixinmuqiang.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://vx.huixiangedu.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ei.huanxung.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://qx.huanxung.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://dx.colortex.cn

[P03] 生成短随机字符串
来源：http://ol.shxzukj.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mk.huixiangedu.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://fx.hahajie.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hs.colortex.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://dr.lnxyls.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://na.chemitech.net.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ll.521024.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://dh.huanxung.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://jl.wgjwhj.cn

[P04] 求长度
来源：http://uo.colortex.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mq.hnjuh.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://gt.panjiajie.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://il.huixiangedu.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mq.hahajie.cn

Java: list.size();  map.size();  s.length()
来源：http://br.haigaiapp.cn

Go:   len(arr);  len(m)
来源：http://dc.jctech888.com.cn

Ruby: x.length;  x.size
来源：http://lt.shtwfgs.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://vp.shtwfgs.cn

[P05] 判断两个对象内容是否相等
来源：http://ea.jianghongdianzi.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://rr.521024.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://nt.panjiajie.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://se.bookmarksfly.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ff.bjjhwx.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://qx.asd995.cn

Go:   reflect.DeepEqual(a, b)
来源：http://pc.521024.cn

Ruby: a == b
来源：http://ea.szxytkj.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hx.yuntaijiaju.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hh.asd995.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://zb.shxzukj.cn

PHP:  if (empty($x)) {}
来源：http://gu.huanxung.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://gb.szsharing.cn

TS:   if (x == null) {}
来源：http://ns.bookmarksfly.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://so.chemitech.net.cn

Go:   if x == nil {}
来源：http://lz.shxzskj.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://dy.jctech888.com.cn

C#:   if (x is null) {}
来源：http://fu.jianghongdianzi.cn

[P07] 防抖与节流
来源：http://bc.huixinmuqiang.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://sh.colortex.cn

PHP:  // 手写时间戳比较
来源：http://rc.huixinmuqiang.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ly.bjjhwx.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://eu.yuntaijiaju.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://yb.yuexingan06.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://go.jianghongdianzi.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://wl.haigaiapp.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://tz.hnjuh.cn

[P08] 处理浮点精度问题
来源：http://nh.9csxet.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ze.nicolike.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://uw.huixiangedu.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ic.szxytkj.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ro.bookmarksfly.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://pq.521024.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://jr.colortex.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ah.wgjwhj.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://vf.chemitech.net.cn

================================================================================
来源：http://jz.yuexingan06.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://oz.lnxyls.cn

================================================================================
来源：http://fv.wgjwhj.cn

[Q01] 创建表
来源：http://pr.szsharing.cn

CREATE TABLE users (
来源：http://pi.521024.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://zz.szsharing.cn

name VARCHAR(50) NOT NULL,
来源：http://ca.nicolike.cn

email VARCHAR(100) UNIQUE,
来源：http://jx.haigaiapp.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://is.szxytkj.cn

);
来源：http://vv.shxzukj.cn

[Q02] 创建带外键的表
来源：http://sr.nszjky.cn

CREATE TABLE orders (
来源：http://rh.yuexingan06.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://rj.huixiangedu.cn

user_id INT NOT NULL,
来源：http://en.jianghongdianzi.cn

amount DECIMAL(10, 2),
来源：http://fo.shxzskj.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://rj.jctech888.com.cn

);
来源：http://hu.hnjuh.cn

[Q03] 增加列
来源：http://tf.yuntaijiaju.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://du.colortex.cn

[Q04] 修改列类型
来源：http://qy.szxytkj.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://rb.nicolike.cn

[Q05] 重命名列
来源：http://cc.szsharing.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://yq.gzmigu.cn

[Q06] 删除列
来源：http://wb.521024.cn

ALTER TABLE users DROP COLUMN age;
来源：http://zs.nicolike.cn

[Q07] 删除表
来源：http://pg.huixiangedu.cn

DROP TABLE IF EXISTS orders;
来源：http://gz.szxytkj.cn

[Q08] 创建普通索引
来源：http://xp.chemitech.net.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://cu.newstarts.cn

[Q09] 创建唯一索引
来源：http://op.jianghongdianzi.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://xa.muxihuayi.cn

[Q10] 插入单行
来源：http://rj.gzmigu.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://xo.panjiajie.cn

[Q11] 一次插入多行
来源：http://id.huanxung.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ci.bjjhwx.cn

[Q12] 插入后取自增 ID
来源：http://in.wgjwhj.cn

INSERT INTO users (name) VALUES ('C');
来源：http://cd.jctech888.com.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hv.nicolike.cn

[Q13] 忽略重复插入
来源：http://ug.yuntaijiaju.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ao.szsharing.cn

[Q14] 存在则更新（upsert）
来源：http://tt.9csxet.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ft.shxzskj.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://zt.lnxyls.cn

[Q15] 查询全部
来源：http://zk.hahajie.cn

SELECT * FROM users;
来源：http://la.huanxung.cn

[Q16] 查询指定列
来源：http://gs.huanxung.cn

SELECT id, name FROM users;
来源：http://sn.bookmarksfly.cn

[Q17] 条件查询
来源：http://iw.szxytkj.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wv.shxzukj.cn

[Q18] 模糊匹配
来源：http://mm.bookmarksfly.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ss.wgjwhj.cn

[Q19] 范围查询
来源：http://qb.yuntaijiaju.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://vm.colortex.cn

[Q20] IN 列表
来源：http://td.colortex.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://kp.wgjwhj.cn

[Q21] 空值判断
来源：http://lm.wgjwhj.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://wo.nicolike.cn

[Q22] 排序
来源：http://hb.huixiangedu.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://je.yuexingan06.cn

[Q23] 分页
来源：http://aa.lnxyls.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://nq.chemitech.net.cn

[Q24] 去重
来源：http://tw.szsharing.cn

SELECT DISTINCT city FROM users;
来源：http://xl.9csxet.cn

[Q25] 只取前 N 条
来源：http://vg.newstarts.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://dt.hnjuh.cn

[Q26] 计数
来源：http://fe.wgjwhj.cn

SELECT COUNT(*) FROM users;
来源：http://wo.yuntaijiaju.cn

[Q27] 条件计数
来源：http://zq.colortex.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://fe.hahajie.cn

[Q28] 求和与平均
来源：http://ao.lnxyls.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://gb.nszjky.cn

[Q29] 最大最小值
来源：http://bu.gzmigu.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://yh.nicolike.cn

[Q30] 分组统计
来源：http://sm.yuntaijiaju.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ej.shtwfgs.cn

[Q31] 分组后过滤
来源：http://ji.nszjky.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ga.wgjwhj.cn

[Q32] 分组拼接字符串
来源：http://vh.huixinmuqiang.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://cc.huanxung.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ti.shtwfgs.cn

[Q33] 多列分组
来源：http://fe.nicolike.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://zp.huixinmuqiang.cn

[Q34] 每组取第一条
来源：http://jq.yuntaijiaju.cn

SELECT * FROM (
来源：http://zz.hahajie.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://pf.yuntaijiaju.cn

) t WHERE rn = 1;
来源：http://rf.hahajie.cn

[Q35] 内连接
来源：http://dn.yuntaijiaju.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ec.nicolike.cn

[Q36] 左连接
来源：http://px.shtwfgs.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://yb.bookmarksfly.cn

[Q37] 右连接
来源：http://yo.nszjky.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://sm.lnxyls.cn

[Q38] 全外连接（PostgreSQL）
来源：http://lr.nszjky.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://pe.nszjky.cn

[Q39] 自连接（查上下级）
来源：http://cg.szxytkj.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://yb.yuntaijiaju.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://gb.9csxet.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://cf.muxihuayi.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://rq.9csxet.cn

[Q41] 多表连接
来源：http://ig.asd995.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://wt.hahajie.cn

JOIN users u ON u.id = o.user_id
来源：http://ag.shxzukj.cn

JOIN products p ON p.id = o.product_id;
来源：http://cn.bjjhwx.cn

[Q42] 连接条件附加过滤
来源：http://qu.shxzukj.cn

SELECT u.name, o.amount FROM users u
来源：http://ta.hnjuh.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://zg.shxzskj.cn

[Q43] 标量子查询
来源：http://aj.newstarts.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://bi.nicolike.cn

[Q44] IN 子查询
来源：http://wi.jianghongdianzi.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://fd.huixiangedu.cn

[Q45] EXISTS 判断存在
来源：http://wk.jianghongdianzi.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ip.nicolike.cn

[Q46] NOT EXISTS 判断不存在
来源：http://tj.nszjky.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ki.shtwfgs.cn

[Q47] 与平均值比较
来源：http://ny.shxzskj.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://xh.bookmarksfly.cn

[Q48] CTE 公用表表达式
来源：http://oz.bjjhwx.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://bz.shxzukj.cn

SELECT * FROM t WHERE c > 5;
来源：http://uy.wgjwhj.cn

[Q49] 更新单行
来源：http://mh.muxihuayi.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hy.shxzukj.cn

[Q50] 批量更新
来源：http://nl.haigaiapp.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://tz.bookmarksfly.cn

[Q51] 用子查询更新
来源：http://oo.nicolike.cn


<!-- 参考信息 -->