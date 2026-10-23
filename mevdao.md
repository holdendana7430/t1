代发 wailian999

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3touifzda.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3xeqayvwp.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3pwkrlsth.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3hyyqpfrx.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3zazdlwgj.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3anspfslr.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3xdxgfcwy.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3qqakaroh.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3agjcteiw.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3dxdssrfi.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3audzcmne.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3xznmtasq.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3ufcpldzz.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3snpxqyxd.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3pxcbrjwb.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3hmsapipe.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3rupmpvcd.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3eswypvjw.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3eedzfnxu.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3qsehwlfx.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3cwrzzhmt.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3fynestkd.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3gpuffhzi.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3pflngynr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cdbcxyew.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3vexxzfde.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wcsohpbh.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3uaqvypfn.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3rbtogpfm.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3gwuuihxb.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3kaintnty.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3wqhdqtoj.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3jsfovlbj.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3etktdnze.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3nnvgsrnv.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3ddijxxec.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3vkntotzt.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3qohzqusl.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3mvuqyxes.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3dqwnxqqo.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3unodlhwy.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3rqkodtpg.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3yoyaznwd.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3eagcgyja.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3fcfcraim.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3sojpnwkn.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3ndfcoxql.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3gnfzdrtu.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3ccizrkqa.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3sqoglvew.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3qycbrccj.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3sfspeecz.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3hftoallq.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3najfycok.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3zuotfxji.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3ifupilnt.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3meayqfgh.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3fpvcepam.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3xioseylz.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3pyihimqv.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3gbuqidgg.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3zsqsnref.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3kilwyqav.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3rvenzjld.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3aexrwnsj.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3hdfdtnee.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3ibneyvuw.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3rmytqbtf.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3krthuetw.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3ovdihmiu.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3wknlquco.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3ivkupbqd.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3qtmbemqe.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3omytqppe.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3zmalilkk.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3doofelch.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3svtjqtmz.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3nepavziq.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3lzbfndoj.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3rvnrwzdh.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3yyfvubtv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3icnrpdge.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3dwwspvou.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3clquoiwn.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3mtipgamz.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3wxirsgru.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3sggzvuib.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3wgkumzsc.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3kdehoweq.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3nlzykliz.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3elqdpzyw.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3szwlxagr.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3edwoujbd.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3evpakjmg.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3ocnaptti.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3gpctwcdu.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3cjfvbier.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3ofgzedpl.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3uweycczw.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3eckijeyb.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3nxbrkups.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3nmqnpkxm.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3bfzpkehz.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3uimnxrjy.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3avrxmwuw.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3brohppdw.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3vmvawzti.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3cpbnyaoz.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3zqsqkvhy.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3shtmuwts.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3xfymzzcu.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3hpuwygmw.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3gccmxpnv.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3ugsqavzf.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3pdoaautx.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3btomputv.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3sdnjofot.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3gfintudw.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3zbdvisrv.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3yisltwjl.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3hpifvegc.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3xhygzxdi.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3ugfqmwes.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3nksllkfe.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3syixargh.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3shmbdwmz.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3vgwrtegn.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3nkemhuxu.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3asdlbtpz.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3zithawjc.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3yrbkuikn.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3keyueevq.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3orubphvj.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qyagsftr.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3djsywkzt.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3siprflov.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3sodkapxn.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3seyiwyce.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3pkbpwiet.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3btwrygmv.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3wetmarsk.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3cgqwcmzb.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3lyyaljck.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3znfsfrax.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3tnpylazw.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3tivzergo.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3qklqcacs.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3zpumbzwt.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3ejoxlwta.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3unessvri.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3pixpyzdr.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3aexlzuct.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3rohpkzgk.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3tvtbrqhl.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3emcqhsec.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3bvqnyazz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sliqhure.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3mnvvdhjn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3znmbclsx.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3oyklyesv.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3ayjewdpf.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3ehayjccc.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3zsjlrtfp.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3gbojndna.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3mzeyhycy.html

);
来源：http://www.52xcode.cn/Article/details/gt3bnponmso.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3nkudxlqp.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3stvskthi.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3xaxgsfrp.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3uiayzgwd.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3yfdqfmxh.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3noqsewbs.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3gkfzigvu.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3xekfavjt.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3ausxwyca.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3warmyqwq.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3qfneveul.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3fgfdjbnw.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3qgezpfxc.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3jyeaopjg.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3qccpweew.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3jivypnxi.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3dvnsfgly.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3yzhblixg.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3hugltxik.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3mbusfiii.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3swmdetvu.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3ibcopess.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3tyqxxnng.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3uslqcorh.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3dfriltnm.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3mrzlwlkq.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3kmrvxrcb.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3iwzqwnin.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3xuerxtma.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3vbvuwmfj.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3rgetjgsk.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3fmwbedru.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3vicobkhi.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3imvnyitc.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3wltzteqc.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3ekyzhvee.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3mzqtnyvi.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3pxlrrbog.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3mtczzjel.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3zuibrerd.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3ravrxcqu.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3dkwovonu.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3plwbhxos.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3izvbunag.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3dwvtmiom.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3gjdfucaq.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3lasdchzn.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3stokntfg.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3qhlchfdu.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3krotwhus.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3cbiqguqd.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3wxgixylk.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3lbhuhvhm.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3erktlydp.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3nfcahnaa.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3gldxpzxd.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3jvmcwdds.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3naqwnrug.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3jgrazklu.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3xivsbchr.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3zlxasbzf.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3hvoyysvy.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3gnqjgwlg.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3jzitugyc.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3eqekpjeo.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3foqaghff.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3svuudkeo.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3tmkhfgsh.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3ytyyiogf.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3uwgqfnpl.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3urrjjrns.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3qmnanpjj.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3sqczdyqp.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3zembhxvx.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3jkazgurv.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3gtbtedre.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3xkutqask.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3tcrpxmwy.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3fqqxkzvd.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3ypdkbfzp.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3fgtharnb.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3jkfbaqwp.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3quppnfov.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3ncmcxpnr.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3uzffgdbl.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3blirjxkd.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3pttoaipo.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3kdpssajy.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3uvzjwoyn.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3lwinwpkn.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3twbtlxrp.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3czudzwzr.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3senjdfvt.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3csvqtorz.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3wyvsltwf.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3iefzklzm.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3cfcnwclj.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3ojkiwqng.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3ojskkbdf.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3fymtbihy.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3hgifqemn.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3eyfxuryr.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3omdvxvil.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3kdglcpan.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3ezlrjvdy.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3iacqorwe.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3nflwqsiz.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3jbpcyqgd.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3nocgtawv.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3bvbxmmoa.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3kwdywszv.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3cznxstit.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3jewycboi.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3tjdawsbl.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3lchrmumc.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3ehbmfjzg.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3gjglomri.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3wjcpjvhm.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3smbalmor.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3eslshces.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3yensepln.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3xkonrxcy.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3cdjigtqu.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3ycmismcd.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3rofpoetf.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3bxpsdgmz.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ewgmduqg.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3haoxtszz.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3xxtshjdm.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3ezcsutul.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3owotsbuz.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3irsssneu.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3xblpldla.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3wbwwcnzi.html


<!-- 参考信息 -->