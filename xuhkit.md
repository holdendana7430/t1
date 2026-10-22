代发 wailian999

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2fsbdvkiu.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2jyhoqxsy.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ujlxqylk.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2dtxzxknr.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2edxkijyf.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2qofbpbko.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2cedtsdsz.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2zhvrlbqy.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2wksgxdzm.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2cucqshdw.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2tgvpgvnt.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2pupvujdk.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2ksdtqvzf.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2kqfgysci.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2lhiehvlz.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2hghvnnbk.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2irravpml.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2xevrjevl.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2zygxnmrt.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2dabwfldn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xuewopbb.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2uzattacv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yqaodevi.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2zhkzqnlq.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2seupfpdf.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2rnunvgul.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2hytoxbig.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2clufzxnx.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2xhmkyxqb.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2xrzwyunw.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2irsttaqo.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2zvzdgftr.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2wwicrtjj.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2emqzkrfy.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2iwkjhyjh.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2vswfqhsl.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2fgjmyyug.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2fjrlqmox.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2zirwevaw.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2acdnqath.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2itrmiupd.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2caialgrb.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2mebmraqz.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2glmtwxcd.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2qerssgbc.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2fokfgdtk.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2tixgkrfj.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2whuaxwlz.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2bsxkhbuv.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2sgrwjwfp.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2sndwpoct.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2anbkfscn.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2hgjmyumz.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2uagabann.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2tygapcrz.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2rvedmohz.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2qidjsvvn.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2sloernoj.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2tdbktsao.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2hwszdbyi.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2eaesaqeb.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2awufpdat.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2rmuxuqbr.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2yxjepaks.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2hixqdrzl.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2kwfheobh.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2jfhffqtz.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2edwnqnmt.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2qpurigbz.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2jivirtkz.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2abofqnqg.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2dfgbbblh.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2hdpsmplt.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2xnmppgvz.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2ctnitrxv.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2clrnsuaa.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2xposaicm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wfiqfzmm.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2nkdwapik.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mydrdplz.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2iurrmmkh.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2lqfbemzl.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2szqysgpc.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2aiqyntip.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2evmtjajl.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2mvmwobak.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2jbakqdwd.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2drjzltcb.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2lqmcphdx.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2fdjmyftf.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2xljqrnhz.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2nwvmsecm.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2rkqpuudy.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2iynwhxfs.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2ijgyfjks.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2tjiibuhd.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2ghdsbiib.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2wpqnlqcv.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2vvbadlzo.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2cqgglvcd.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2apfkrgan.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2rqvbplub.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2lqbjeiri.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2lfywpyjx.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2iyqrxhrt.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2bfjfjotw.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2tsphdoli.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2dagdhvll.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2suuybfld.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2cjescomr.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2mgoibzwo.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2jqfeclqr.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2zktanapi.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2lhhmbvub.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2nbxkcuzs.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2ambyopbj.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2audxmmqi.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2ekqvxdmu.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2wvigqgjn.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2xvhjbodk.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2hmcgpuak.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2usnyqbfl.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2kgfzptap.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2lgfmnpob.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2kshhnwqa.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2asugapsh.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2rrltdmgt.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xymfimbj.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2jkazmckn.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2weocnlfr.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2etbwktxs.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2mqvgnbmq.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2mktdsptg.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2lydmskne.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2yylrkxgp.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2yyydbhcn.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2eqjanlhx.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2vkzqybih.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2jkmtersi.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2vqipinnq.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2zvjvlmsh.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2cjdekssa.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2peqqymmp.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2ayidfrfj.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2dlcgysyh.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2cfnaeews.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2djgjkstz.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2aiaktwkt.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2gfsqaqsm.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2fpsejavg.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2alhxrhcj.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2jeemlqlu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hrskhidp.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2hvnqriyb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fcztbxqp.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2islcylwg.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2bebitukd.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2thhjuxjd.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2iacymnrc.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2gyrelspd.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2zpobzxto.html

);
来源：http://www.52xcode.cn/Article/details/gt2uouasnlk.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2wxywnuxr.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2idlwlkyf.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2nnbckgjz.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2owriqrnk.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2ruebfhkz.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2ssbrurus.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2vvdtmalt.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2mhmnmbkc.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2sfudddvw.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2nztrqemh.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2olyrqmbw.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2ujrbxlzr.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2pruqasly.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2uwfiumld.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2snltruxo.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2fiisrskn.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2yfhpzfic.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2ruwjfvmm.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2bgbygmgb.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2hcpuxjjb.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2qyrmayhw.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2zxkqtcrk.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2pkwpgqvo.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2imwnolnv.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2bnvzxssp.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2uwaasqiq.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2xftobbwb.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2mjcygjzn.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2ihvwseat.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2rauhrsuh.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2lrgttnjy.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2okugycar.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2wnagkuly.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2pmawkxde.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2uxzuehxt.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2cvrihudl.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ximwgodu.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2jdlidubo.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2pdcfsnhs.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2uwmpijzu.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2xmklvoyi.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2xjjassmu.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2nodbobsa.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2hnqjgiyw.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2gqkywvzm.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2djcfwrfe.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2sugqcicw.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2qvqljkjh.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2bomhnkoa.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2mlldflkm.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2bykqkjtw.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2tbxeqqwm.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ouvkczek.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2nxxrgskf.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2hquhjujp.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2eobyyuja.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2rmongwba.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2tidhbspt.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2gzrhamud.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2idylijyv.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2cnubcqyc.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2lqvjsynd.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2sbvviopf.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2ipwicwjf.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2ddlarixk.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2pespkwvu.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2nvyhukvc.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2ocozfyfm.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2rchutaur.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2tpoiggew.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2asywqjje.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2cabegnou.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2mysedytb.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2wkxdnssn.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2fupmekcs.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2xzcckbih.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2ontbgvxj.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2mloescst.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2cbutqldl.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2ivpvcqwt.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2xuxhovpr.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2tqceykty.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2yqxnyqbv.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2ochsfauo.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2uvbiantf.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2abrwxybn.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2eywhvibc.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2iukrfcvv.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2ngqcochn.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2oliaczzu.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2ovjmucpw.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2uhtxngkf.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2snqdtqfh.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2hlxciqmj.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2rdfhatdn.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2fxartvhz.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2uhjwoeli.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2vlrinyhd.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2teyavvbh.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2yjvaplzb.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2qbzxvtia.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2eokpweeg.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2bcqhczzr.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2fcawkvje.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2aizbaqkw.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2nfxvnbgd.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2ahtlkijj.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2qxhrfrwp.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2opqnitkz.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2mftsfxnt.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2mbbosrcw.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2fdhidbxi.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2htlhudbh.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2lpiusqlf.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2ajgfjfrh.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2dxrqwyxz.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2fpjjxovb.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2lzrygsyl.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2atyajefb.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2jhvlopsv.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2angrhpkz.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2xjmjeysa.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2vwklshou.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2eawydjwc.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2qicrftcv.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2rnwcxbjj.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ckeiqfwc.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2euaspnjz.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ycocyvpt.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2yvppmjbd.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2wyjebxgh.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2kfesyujv.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2vqqbmecu.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2gsigdsjc.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2nfrdatle.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2uyetbhoo.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2lphyidkn.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2nftuczmk.html


<!-- 参考信息 -->