代发 wailian999

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3nsudvwuq.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3szywqsue.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3hokndfkp.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3ydlbhbur.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3jbvjfgyq.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3cuuizoep.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3jsxtssha.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3codhqlpx.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3kodvqorl.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3hqkulzsa.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3rsczdnvs.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3qowbkiek.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3cbyaenlb.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3feufmquu.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3iduhwwyi.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3aecmckps.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wjvlfhcw.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3xkdxpjvn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hcquramk.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3fnnegndk.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3cpldxxny.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3thqwlpub.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3bfawfmgw.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3rfdkzxwx.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3kwuibagq.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3usjbsqar.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3mkxdluzp.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3dugxkxot.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3mnshbtfh.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3wzwyvmbv.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3kmyfjghp.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3amvfywhz.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3qqbqkrsy.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3imkvcsuz.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3rsbanlsk.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3uvhlfnxn.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3gjxiefxu.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3aaluezwh.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3jcyvpskd.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3fuzzcxhs.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3optpmmlg.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3ivnlnczx.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3ihtatvdp.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3foeylagq.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3syjiduln.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3juikldwz.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3bzmpnljv.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3ziyalskp.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3nnvvtcwk.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ukscrywg.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3ssxxkyzu.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3jipicvpk.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3zsqcaqom.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3plgkkumo.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3qtuhdbje.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3fcvadzbg.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3vdvcvhja.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3hpuhqutp.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3qfuiwkqy.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3wyhzxyqk.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3liuerjqj.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3xmgvwhud.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3hxoofzwg.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3knqjqapz.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3grgdqrsy.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3kbteqzoo.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3ncttckqa.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3wcayxfya.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3eebscnib.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3alvlchmm.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3nubrruhf.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3uivfrqzs.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3qkmscvfu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3geabnsvr.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3lctlqdsz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lpuwifoc.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3ynrmrktg.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3fjgwmolq.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3tybewhta.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3qdxvppzo.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3enzkdtiz.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3tspqqinr.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3chatxbvw.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3gtdmazav.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3ipbdgyrc.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3tlmfdont.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3kbiyucwf.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3swgonnmo.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3suzjhzim.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3cfbwctjk.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3idrskmhv.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3bvebzolx.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3hthhwrye.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3mwgigkpd.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3uzxkswqg.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3mhslihfw.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3zijknagp.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ojfdeyhv.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3sszapvrp.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3ayqauytl.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3qumnokiq.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3hprzszdv.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3fousofej.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3omxsaoas.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3sfjkiwvp.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3kzkfhbry.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3enopkvjt.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3bpfqohra.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3qcukbwxm.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3lflardgh.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3nqpwaoef.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3lndaqzbj.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3ohaacgne.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3vsitnvaq.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3rpgkiynx.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3hzblxfpy.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3mmbpvmvs.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3qpiicrsb.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3nkmfefvj.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3ymxhxovy.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3tmiqdvzi.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3mfsnsbrn.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3aasbbxlv.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3oqhivbbh.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3ybflkcos.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3icyiuogm.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vrgvykpa.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3qtfgypnt.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3ijkuuljp.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3ftnqhqkk.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3tcnuzxbg.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3dlpybprc.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3ujthnjjd.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3hwowelwk.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3cabatibq.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3zqxvvrdt.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3mxmkkdlq.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3veowcygy.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3opzqjmcs.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3bixbnfwx.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3fhcdbjqm.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3maiaftia.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3lpmmeznb.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3hsvdbefc.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3bhvypsqs.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3usurhpgp.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3ublbjsfb.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3haopbpgo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ldqswmas.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3ngdxteco.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3eozwcemn.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3yhxrpjtg.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3ttbvurxx.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3xarahvmq.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3savphhaw.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3phborpow.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3hzryunav.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3yxgtgeiw.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3qlswkoto.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3abgchnfn.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3tiftxxix.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3arqgnsux.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3xpsjyibm.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3vwwjmwkw.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3yfmbahax.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3mauhwdwp.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3ubpvmtuh.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3rgqjqxha.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3dhstiwrl.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3pmdqfhym.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3errktdqd.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3lgvrgicu.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3rejbslky.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3ashglzum.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3lujnlpav.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3ajcedrau.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3ppflfovj.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3kdufquho.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3ejccrism.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3xbrsiwsi.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3lgaabope.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3fvucoswk.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3eaqjbdwy.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3ankyymcb.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3biorzero.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3nzfcxriy.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3xbawmnpq.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3dwmwzvby.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3cbwxdppl.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3hyinevkl.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3sshntucf.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3wtghoafw.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3fxbalsln.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3zmcjxnha.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ksnbzang.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3wovmjlnm.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3fcxuntgj.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3mbcmfqqv.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3nufbbgsm.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3tolzylwt.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3aujankjg.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3zwvuidre.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3qyqfrpeo.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3emtferux.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3slhtjuyj.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3jezpysem.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3zwzdvxjj.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3lwbsjblr.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3bthgvtpq.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3ldyrijnx.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3gaygaalv.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3ljagzeqe.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3bjzoezyk.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3kckgyxls.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ttuczfdn.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3flquqevh.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3jatawmxy.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3fmyywqhq.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3zperyqvj.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3zeafzbtx.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3vfwjjlsz.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3jovkhsfy.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3tzufrqtl.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3kifrdhko.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3tpfkggdt.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3gajgqmmh.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3okpymztt.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3abtgxhel.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3mwvvbdaj.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3zytxqxww.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3ofllwjkw.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3snopxdrh.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3xdlhjmds.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3xlfkepmp.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3xiwrtlbs.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3adgznaqx.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3rfstuisi.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3stccuxan.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3rojysgnm.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3unmxbvcp.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3qzvrngpz.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3qtachanu.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3twllhcec.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3ymfdgzbn.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3suoutbpg.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3bvwppjyi.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3ezvygbyh.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3jwzzsjpq.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3eyqwwpvf.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3sijsxpvb.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3yahbflyp.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3duzrmmrv.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3dxdnmbwc.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3wtfeztxp.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3oejqyrfn.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3rworsohv.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3zcurouka.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3orrjgrcs.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3fvutwewj.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3zeipkuca.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3watbqiue.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3spdpayyt.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3ozhdfeyu.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3pojnboyx.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3gepshobe.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3uvvsbqro.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3kyflmxlt.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3wyfmrkfp.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3tjgydvfj.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3klumdueq.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3kmbopybc.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3lzwnrart.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3rgbdlnsr.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3cnqgdtnq.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3iskmitmt.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3tpzqzicl.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3qcintepy.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3ajpchtqt.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3rnjrqeek.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3fkszarvi.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3lkpiccad.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3qqaylogf.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3ukgextix.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3mzqygewo.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3vdqpvpvi.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3jsbijzbp.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3qqzxlkes.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3vmviuedf.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ynakbker.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3lbanwfff.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3dugarchq.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3jctvvvaw.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3ddmctgdy.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3gwywanwm.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3yiyjtzbi.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3xqeoxqjb.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3dybflsrf.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3slyxeziu.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3pipfhkto.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3pwldqapq.html


<!-- 参考信息 -->