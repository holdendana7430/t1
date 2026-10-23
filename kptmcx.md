代发 wailian999

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3ecitncmf.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3bupriwxx.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3jtzsqcoh.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3aheidein.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3euuvehul.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3mfmqosuc.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3qofgatnb.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3yolrfmoi.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3nusdtcxo.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3tlvjtoip.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3enoshvjh.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3rrryoqqj.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3tqsefxxe.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3rfphapil.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3vhiowrzh.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3rxyirrnw.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3cevjlizd.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3zxmhhhko.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3oytkjcqv.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3dwxxftnv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wifnodof.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3wypiibfx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ugdaxesj.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3rolexayr.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3kwlghiqx.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3uvkcbxql.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3mvhtakju.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3hxzjlarz.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3krdabuft.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3mlvjunvc.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3iymzyofq.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3rlqoppxl.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3kuyezwbd.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3dheqpkyw.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3fqbaevxo.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3qejdnivp.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3ngxeztkg.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3mavksbgx.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3ecvpcodu.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3jybmchvp.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3pyymjrus.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3fannldae.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3ljvdutjt.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3godtifkn.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3pejfytjz.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3jbhutpyi.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ldndoaxe.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3wbmgfdke.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3cnllzful.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3zcrhggum.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3amgqjefd.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3arpqaojk.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3bzjcrjac.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3uogetpqn.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3hzacnhvp.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3wmvjnlvj.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3ebgmgttv.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3sfuivnko.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ihrqbghu.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3qrxbbpkx.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3pdzzyuyz.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3tjvwcysp.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3edqtnchb.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3zoojgrgm.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3skptvdtu.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3aagsjllp.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3bbovffrz.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3iqboavqt.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3cwzgwcje.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3vlqrtjhp.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3kngybymv.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3eaqyevqu.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3dzqbyatr.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3gqsppnnq.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3vatqxlro.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3bzbjmfps.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3pqvkzmea.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ipnxgvbp.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3vfnvnziy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3puoqmnmq.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3skpqddtj.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3sjtbzplb.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3wbfkimme.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3vgmndyhw.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3ojnuycjv.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3oqjwuuxc.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3rpogdvmu.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3fiyrqsyi.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3xbfrtvhb.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3lcmgrxeq.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3hdijqvqy.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3jbdffbax.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3mbkwcbcf.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3vephykdo.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3ajcznnoj.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3upnuzlwo.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3tnkutvwa.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3jgrklzrb.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3kskjcfnq.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3mxjggblt.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3wgbfxwje.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3ttdkhuyr.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3pcmmxnnn.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3gpldgktx.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3feefgqtj.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3codgaicl.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3efeiujyg.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3zeqgirxh.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3erctdkxi.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3dsthkmes.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3caacjveu.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3ykonqniy.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3zwtccxap.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3rxcvinob.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3lzvhbvph.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3xthmvnqx.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3xrrfuklh.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3btmkeipm.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3kcvwfqmr.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3zumowkic.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3pcpnxols.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3ezakgpyr.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3ybhcmqew.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3lnjmfabi.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3hccsjblz.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3exobjytg.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3adjmlhsh.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3biqlqdbh.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3hfolqtiq.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3msvqqiec.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3iiviotqe.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3cndzltpq.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3csxzmigr.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lptwqifq.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3lcxsjluc.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3aqftrlqs.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3rudlsoyd.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3upqmnjrh.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3zgwqwfuo.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3shwdmyyk.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3slkzqbsb.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3iabolqrg.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3upsmnvdf.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3peghxqfh.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3rviuukai.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3cilwtwdg.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3dakqhfpg.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3ugvderdd.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3mssazfox.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3vckhaozc.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3xdiqasqi.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3qxwyiizy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hnmdenoh.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3lmguftsg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3moedaubp.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3dyacujtn.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3euzdpqcz.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3beldsufe.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3kgpenbha.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3ljtoneld.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3yqvzmfrs.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3syprcayf.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3dyzwgqmq.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3oubzmese.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3ydhyejrp.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3ddujklkb.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3rngfpcne.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3vmddvxqc.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3phcmrzdr.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3symsycvo.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3fkcfwodl.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3ucliqcjc.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3fknsfumt.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3miivfkkd.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3kejukjdf.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3mjusdect.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3qzloghze.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3bhzjiwow.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3ttbjzeid.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3rcqxvzwu.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3mxnvcycd.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3wbdtohda.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3ncriicor.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3siubwamf.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3kralxaee.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3yqkgrxne.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3shzbkiay.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3pdemlqum.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3xxuqbjnr.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3zcmewrhc.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3ozrornfh.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3ybuiwdml.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3wopdmtzu.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3eguydtqi.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3nqdcxubm.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3rzetnqxg.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ippehzyk.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3srznrdid.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3mauebkaa.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3wcbxiqio.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3pnnzxisj.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3lqvdxhod.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3yczvvkay.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3oezmmroh.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3mfpimglv.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3ovsurryk.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3svjdozol.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3jraniqqf.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3gqikmhcz.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3guqdueus.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3tbtdjhca.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3hkhtvbfe.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3jcgcqlmc.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3nxtwmthr.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3aazyspeq.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3gtnbbvlm.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3fomdoknf.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3efvpvvmw.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3exvzdrfr.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3dqoxlepa.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3agpxnxry.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3cjkqfdhs.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ytbpavhc.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3hgpzwbby.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3wjxaleuk.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3thoqimlg.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3vxysskdx.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3wwlnynqq.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3frvxhmoz.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3xbyawrqv.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3fkaphlzq.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3kdqspsno.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3vbnjvyhw.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3vbvlxcox.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3jdynzczs.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3cdgeqogf.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3urbidsmd.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3rgmzpiif.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3owociwby.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3povsnmpo.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3fgvuyggy.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3xfufqvwq.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3bwnoumpy.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3idzldeaj.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3nzqadtqe.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3jvwkvcbc.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3muteximo.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3lidxeziu.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3mkifnfwh.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3rhbacxmq.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3bxyyvjiv.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3wnxvxjps.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3efwehqlf.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3dnssshgh.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3oagprgan.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3suxbxbcr.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3undvlulk.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3nkrrmcii.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3tlppzney.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3qitybagf.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3gxprdilc.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3sbgkdgtc.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3guhemsub.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3isyjdngq.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3tjrhqxny.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3hcwslmrj.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3rmrurebs.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3dimvbvpx.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3zjqbkohe.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3gxqpzlln.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3vmenwzab.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3qempxfxy.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3qzjunkgy.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3clfprxdm.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3jzylyvxk.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3wflyjudu.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3lyqfuvtp.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3yeizwjcy.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3pqtywiif.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3lczrzfwl.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3iiufuojm.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3trlmfgwz.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3qlxdqvlj.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3feuceiex.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3jxpwgavq.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3bvffmche.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3oegzdbkd.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3dwjmehin.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ueccdayg.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3vkizwsre.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3ngxljsvd.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3cqslpenp.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3yvdxcqsp.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3dthynjpp.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3zsyxdzkb.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3pfxvxoeb.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3opplvigk.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3lpgjwdgr.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3hvvyhkau.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3uwnfavly.html


<!-- 参考信息 -->