代发 wailian999

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://rn.jctech888.com.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://sv.wgjwhj.cn

C#:   // 手写递归，或 Array.Sort
来源：http://gh.gzmigu.cn

[N04] 斐波那契数列
来源：http://nn.haigaiapp.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://jc.lnxyls.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://vk.chemitech.net.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://lt.shtwfgs.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://bx.521024.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://pp.asd995.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://tf.yuexingan06.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://xz.huanxung.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://pk.shtwfgs.cn

[N05] 最大公约数
来源：http://ck.yuntaijiaju.cn

Py:   math.gcd(a, b)
来源：http://io.yuntaijiaju.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hq.newstarts.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://gp.bookmarksfly.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://bi.chemitech.net.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://qo.huanxung.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://pt.panjiajie.cn

Ruby: a.gcd(b)
来源：http://vm.newstarts.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://cn.shxzskj.cn

[N06] 判断回文字符串
来源：http://bw.muxihuayi.cn

Py:   s == s[::-1]
来源：http://fn.colortex.cn

PHP:  $s === strrev($s);
来源：http://xw.huanxung.cn

JS:   s === [...s].reverse().join("")
来源：http://qu.jctech888.com.cn

TS:   s === [...s].reverse().join("")
来源：http://kb.hahajie.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://kn.szxytkj.cn

Go:   // 双指针从两端比较
来源：http://td.shxzskj.cn

Ruby: s == s.reverse
来源：http://md.521024.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://za.521024.cn

[N07] 两数之和（返回下标）
来源：http://fz.colortex.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://pe.wgjwhj.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://vm.lnxyls.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://tx.newstarts.cn

TS:   // 手写 Map<string, number>
来源：http://xy.szsharing.cn

Java: // 手写 HashMap
来源：http://ye.huanxung.cn

Go:   // 手写 map[int]int
来源：http://jy.shxzskj.cn

Ruby: // 手写 Hash
来源：http://py.asd995.cn

C#:   // 手写 Dictionary<int, int>
来源：http://bh.huixiangedu.cn

[N08] 生成全排列
来源：http://vp.newstarts.cn

Py:   itertools.permutations(arr)
来源：http://xp.szxytkj.cn

PHP:  // 手写递归交换
来源：http://cz.9csxet.cn

JS:   // 手写回溯递归
来源：http://oj.yuntaijiaju.cn

TS:   // 手写回溯递归
来源：http://yy.nicolike.cn

Java: // 手写回溯递归
来源：http://ri.521024.cn

Go:   // 手写回溯递归
来源：http://qf.hahajie.cn

Ruby: arr.permutation.to_a
来源：http://ru.yuntaijiaju.cn

C#:   // 手写回溯递归
来源：http://gw.huanxung.cn

[N09] 栈与队列
来源：http://gw.bjjhwx.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://dh.9csxet.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://st.521024.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://by.bookmarksfly.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://kw.haigaiapp.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://vu.szxytkj.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://nb.wgjwhj.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://en.colortex.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ij.gzmigu.cn

[N10] 链表节点定义
来源：http://au.haigaiapp.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://tf.hnjuh.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://wm.lnxyls.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://vh.colortex.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://rx.lnxyls.cn

Java: class Node { int v; Node next; }
来源：http://zd.gzmigu.cn

Go:   type Node struct { V int; Next *Node }
来源：http://jp.huixiangedu.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://bo.szxytkj.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://pn.newstarts.cn

[N11] 二叉树中序遍历
来源：http://cx.szsharing.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://jz.bookmarksfly.cn

PHP:  // 手写递归函数
来源：http://jk.bjjhwx.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wv.wgjwhj.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mz.newstarts.cn

Java: // 手写递归
来源：http://kp.muxihuayi.cn

Go:   // 手写递归
来源：http://vl.szxytkj.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://iq.nicolike.cn

C#:   // 手写递归
来源：http://sh.9csxet.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://sl.shxzskj.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://lm.muxihuayi.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://pz.wgjwhj.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://sc.gzmigu.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ni.huixiangedu.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://na.9csxet.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ey.shxzukj.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://xa.yuexingan06.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://by.huanxung.cn

================================================================================
来源：http://gv.yuexingan06.cn

O. 并发与异步
来源：http://zv.huixiangedu.cn

================================================================================
来源：http://fc.gzmigu.cn

[O01] 启动一个线程
来源：http://gi.shxzukj.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://zl.shxzukj.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ht.szxytkj.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://tg.jianghongdianzi.cn

TS:   // 同 JS
来源：http://ce.huanxung.cn

Java: new Thread(() -> f()).start()
来源：http://jq.lnxyls.cn

Go:   go f()
来源：http://ek.szxytkj.cn

Ruby: Thread.new { f }
来源：http://xj.521024.cn

C#:   Task.Run(() => F());
来源：http://jv.asd995.cn

[O02] 使用线程池
来源：http://kj.szxytkj.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ww.jianghongdianzi.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://cr.wgjwhj.cn

JS:   // worker_threads 线程池
来源：http://da.521024.cn

TS:   // worker_threads 线程池
来源：http://qf.muxihuayi.cn

Java: Executors.newFixedThreadPool(4)
来源：http://yj.shxzukj.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ua.huixiangedu.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://og.521024.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://za.nszjky.cn

[O03] 加锁保护共享数据
来源：http://iz.nicolike.cn

Py:   with lock: shared += 1
来源：http://id.szxytkj.cn

PHP:  // 用 flock() 做文件锁
来源：http://rt.haigaiapp.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://zx.shxzskj.cn

TS:   // 同 JS
来源：http://gb.521024.cn

Java: synchronized (this) { shared++; }
来源：http://wq.szxytkj.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://gx.huixinmuqiang.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://wo.nszjky.cn

C#:   lock (gate) { shared++; }
来源：http://jw.huixinmuqiang.cn

[O04] 定义异步函数并等待
来源：http://ek.nicolike.cn

Py:   async def f():⏎    await g()
来源：http://mp.gzmigu.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://jk.colortex.cn

JS:   async function f() { await g(); }
来源：http://nl.huanxung.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://bq.szsharing.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://kl.521024.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ym.huanxung.cn

Ruby: # 用 Fiber 或 async gem
来源：http://gj.shxzukj.cn

C#:   async Task F() { await G(); }
来源：http://il.muxihuayi.cn

[O05] 并发执行并等待全部完成
来源：http://nv.huixinmuqiang.cn

Py:   asyncio.gather(*tasks)
来源：http://ws.shtwfgs.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ip.wgjwhj.cn

JS:   await Promise.all(tasks)
来源：http://bf.lnxyls.cn

TS:   await Promise.all(tasks)
来源：http://uo.jctech888.com.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://zh.wgjwhj.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://cp.521024.cn

Ruby: threads.map(&:join)
来源：http://fh.asd995.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://uc.hahajie.cn

[O06] 使用进程池
来源：http://pp.yuntaijiaju.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://iy.521024.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://fs.yuntaijiaju.cn

JS:   // child_process / cluster 模块
来源：http://kg.nicolike.cn

TS:   // child_process / cluster 模块
来源：http://tz.nicolike.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://be.chemitech.net.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://cu.haigaiapp.cn

Ruby: // fork 块
来源：http://bc.nicolike.cn

C#:   Parallel.For
来源：http://hd.9csxet.cn

================================================================================
来源：http://ze.shxzukj.cn

P. 常用工具函数
来源：http://rx.panjiajie.cn

================================================================================
来源：http://dj.shxzskj.cn

[P01] 生成 UUID
来源：http://qr.szxytkj.cn

Py:   str(uuid.uuid4())
来源：http://bw.jianghongdianzi.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ha.shxzukj.cn

JS:   crypto.randomUUID()
来源：http://yt.huixinmuqiang.cn

TS:   crypto.randomUUID()
来源：http://ts.muxihuayi.cn

Java: UUID.randomUUID().toString()
来源：http://ok.yuexingan06.cn

Go:   // 用 github.com/google/uuid
来源：http://tj.shxzukj.cn

Ruby: SecureRandom.uuid
来源：http://ld.haigaiapp.cn

C#:   Guid.NewGuid().ToString()
来源：http://wx.nszjky.cn

[P02] MD5 / SHA256 摘要
来源：http://ky.huixinmuqiang.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://gu.chemitech.net.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://jv.huixinmuqiang.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://cc.jctech888.com.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://zi.wgjwhj.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://fd.shtwfgs.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wm.szxytkj.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://xf.jianghongdianzi.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ah.yuntaijiaju.cn

[P03] 生成短随机字符串
来源：http://do.asd995.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://xf.colortex.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://rj.haigaiapp.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ok.newstarts.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://af.nszjky.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wb.hnjuh.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wz.huixiangedu.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://gl.huixiangedu.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://qo.newstarts.cn

[P04] 求长度
来源：http://lk.9csxet.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://fl.jctech888.com.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://gv.nicolike.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://kd.jctech888.com.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://nl.szsharing.cn

Java: list.size();  map.size();  s.length()
来源：http://ex.nszjky.cn

Go:   len(arr);  len(m)
来源：http://aj.jianghongdianzi.cn

Ruby: x.length;  x.size
来源：http://ka.bookmarksfly.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://dd.panjiajie.cn

[P05] 判断两个对象内容是否相等
来源：http://fw.lnxyls.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://br.nszjky.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://tf.muxihuayi.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://rm.521024.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://dw.hnjuh.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://so.huixinmuqiang.cn

Go:   reflect.DeepEqual(a, b)
来源：http://xs.huixiangedu.cn

Ruby: a == b
来源：http://ow.muxihuayi.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://rs.muxihuayi.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ll.521024.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://kb.huixinmuqiang.cn

PHP:  if (empty($x)) {}
来源：http://ug.hnjuh.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://lf.chemitech.net.cn

TS:   if (x == null) {}
来源：http://xh.hahajie.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://ra.wgjwhj.cn

Go:   if x == nil {}
来源：http://eh.bookmarksfly.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://pz.chemitech.net.cn

C#:   if (x is null) {}
来源：http://qe.9csxet.cn

[P07] 防抖与节流
来源：http://jq.jianghongdianzi.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://nq.gzmigu.cn

PHP:  // 手写时间戳比较
来源：http://lg.shxzukj.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://px.jctech888.com.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ws.hahajie.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://qg.hnjuh.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wu.huixinmuqiang.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://pm.hnjuh.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://we.jctech888.com.cn

[P08] 处理浮点精度问题
来源：http://ah.szsharing.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://si.panjiajie.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://zq.nszjky.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ss.szsharing.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://cv.wgjwhj.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://fk.szxytkj.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://sb.colortex.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://qp.jianghongdianzi.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ui.9csxet.cn

================================================================================
来源：http://si.szxytkj.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://xu.shxzskj.cn

================================================================================
来源：http://od.panjiajie.cn

[Q01] 创建表
来源：http://ls.bjjhwx.cn

CREATE TABLE users (
来源：http://pv.asd995.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://sw.yuexingan06.cn

name VARCHAR(50) NOT NULL,
来源：http://vt.hnjuh.cn

email VARCHAR(100) UNIQUE,
来源：http://yl.haigaiapp.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://oc.shxzskj.cn

);
来源：http://tb.huanxung.cn

[Q02] 创建带外键的表
来源：http://lj.shtwfgs.cn

CREATE TABLE orders (
来源：http://cd.bjjhwx.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ve.lnxyls.cn

user_id INT NOT NULL,
来源：http://fk.9csxet.cn

amount DECIMAL(10, 2),
来源：http://ru.huixinmuqiang.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://pd.wgjwhj.cn

);
来源：http://fb.bjjhwx.cn

[Q03] 增加列
来源：http://uf.shtwfgs.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hx.newstarts.cn

[Q04] 修改列类型
来源：http://du.shxzskj.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://nr.newstarts.cn

[Q05] 重命名列
来源：http://bq.yuntaijiaju.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://rr.jianghongdianzi.cn

[Q06] 删除列
来源：http://vg.shxzukj.cn

ALTER TABLE users DROP COLUMN age;
来源：http://vs.wgjwhj.cn

[Q07] 删除表
来源：http://rm.bjjhwx.cn

DROP TABLE IF EXISTS orders;
来源：http://fy.panjiajie.cn

[Q08] 创建普通索引
来源：http://ew.hahajie.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://mu.shxzskj.cn

[Q09] 创建唯一索引
来源：http://li.chemitech.net.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://xf.shxzskj.cn

[Q10] 插入单行
来源：http://ol.9csxet.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wo.wgjwhj.cn

[Q11] 一次插入多行
来源：http://gu.colortex.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://cp.huanxung.cn

[Q12] 插入后取自增 ID
来源：http://yr.bjjhwx.cn

INSERT INTO users (name) VALUES ('C');
来源：http://yc.colortex.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://us.yuntaijiaju.cn

[Q13] 忽略重复插入
来源：http://hu.hnjuh.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://fm.bjjhwx.cn

[Q14] 存在则更新（upsert）
来源：http://gg.szsharing.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://od.yuexingan06.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://sg.lnxyls.cn

[Q15] 查询全部
来源：http://kb.9csxet.cn

SELECT * FROM users;
来源：http://yx.9csxet.cn

[Q16] 查询指定列
来源：http://mv.lnxyls.cn

SELECT id, name FROM users;
来源：http://qj.9csxet.cn

[Q17] 条件查询
来源：http://bk.shxzukj.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://jo.huanxung.cn

[Q18] 模糊匹配
来源：http://mg.gzmigu.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://nn.bookmarksfly.cn

[Q19] 范围查询
来源：http://tg.lnxyls.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://an.bjjhwx.cn

[Q20] IN 列表
来源：http://ck.chemitech.net.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://lk.yuntaijiaju.cn

[Q21] 空值判断
来源：http://gh.jianghongdianzi.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://tu.szsharing.cn

[Q22] 排序
来源：http://sl.bookmarksfly.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wa.yuexingan06.cn

[Q23] 分页
来源：http://ih.chemitech.net.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://zm.muxihuayi.cn

[Q24] 去重
来源：http://ke.panjiajie.cn

SELECT DISTINCT city FROM users;
来源：http://ve.colortex.cn

[Q25] 只取前 N 条
来源：http://ps.shxzukj.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://yo.wgjwhj.cn

[Q26] 计数
来源：http://ft.nszjky.cn

SELECT COUNT(*) FROM users;
来源：http://ht.huanxung.cn

[Q27] 条件计数
来源：http://ib.szsharing.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ui.szxytkj.cn

[Q28] 求和与平均
来源：http://eb.haigaiapp.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://oi.szsharing.cn

[Q29] 最大最小值
来源：http://zd.szxytkj.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://vv.huixinmuqiang.cn

[Q30] 分组统计
来源：http://ct.szxytkj.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://fk.colortex.cn

[Q31] 分组后过滤
来源：http://mu.yuexingan06.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://em.bjjhwx.cn

[Q32] 分组拼接字符串
来源：http://ra.jianghongdianzi.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mw.jctech888.com.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://eg.521024.cn

[Q33] 多列分组
来源：http://ie.huanxung.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ph.huanxung.cn

[Q34] 每组取第一条
来源：http://xw.shxzskj.cn

SELECT * FROM (
来源：http://vb.521024.cn


<!-- 参考信息 -->