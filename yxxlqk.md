代发 wailian999

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2mzsikwks.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2uferheds.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2yybgorps.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2iqsjkddf.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2gslthutt.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2bmdscrjm.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2rnnckrnj.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2obboxwbz.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2rbegdmfm.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2udllnioy.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2qmohqujc.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2wsjjqwhx.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2kwtfmrku.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2brahbyod.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2dlvrefpd.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2qmgnsuct.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ufydoucs.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2bzlonjmn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2oacqeipe.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2fsizlljf.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2baozpvow.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2nqaefhpz.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2sxkjeebr.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2vcczerbk.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2foztskdw.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2qnxfndbi.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2pjjttvjy.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2wadamzmp.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2fpxbcrkd.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2qsxfghlp.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2qoplxsqg.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2zrzcrvqc.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2jqxsvhjx.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2uzutorhc.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2jtrjoqjd.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2kkuoxvwg.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2aiykrusi.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2strtqobz.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2vmzzvral.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2ejgrmqdy.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2wepkjbrj.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2qrpafjyg.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2xyfycckd.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2oapvehhi.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2eycqiqvv.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2ciwdlodm.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2qvnkbacu.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2fomrkuai.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2brwehctc.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2htmlfaig.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2muflpnij.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2cnxzwuje.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2qydgrbhl.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2lhnpmpde.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2jcqrngmf.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2nytrfswo.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2yygtlrmc.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2ojevqyuu.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2nsjtvbdm.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2ftjqmvue.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2cnviqtdj.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2mhachyim.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2lguhdlox.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2qwtjmvyn.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2zjqxdiqo.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2vbtucikx.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2tyhjdsbv.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2eddvskri.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2ovdzulvw.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2lscmswhp.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2emcvjxqd.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2ywguojpt.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2srjhelrt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bycigpez.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2vsjsadmy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ohqwmkuj.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2wyfzanqt.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2taalkfxg.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2zkaormsb.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2vomryfcc.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2aqeqpggr.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2vkrjfzgh.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2wqvjzexj.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2bbcmeqlb.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2qgasdpmi.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2jqkjplqh.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2sikhrzsw.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2etbdgimv.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2udibsifu.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2zgaiinwx.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2oxmruurj.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2qgnigkkf.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2hwuscqui.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2imvssegp.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2ujpgqfcp.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2jkkioyyi.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2mwknbjeq.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2mloamxjy.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2dbkyepyt.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2okoflwxa.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2abznxjnn.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2nfczqmrp.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2kktuujka.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2xhdokroy.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2kapsdbde.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2rtheflxn.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2cooryxcl.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2fskzogfq.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2bwgldddz.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2kpvyykrm.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2pbucuucp.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2wawcpjtz.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2tevffkiv.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2uhgrjskj.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2uemelobs.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2hsvervrr.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2nzllimpx.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2lqfanyfk.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2taeruasj.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2sgziuoqk.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2tuafkyqo.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2asrttnmy.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2xdrfrljo.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2qzujjhor.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2jvtcvwsw.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2sayjvjzn.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2onaqlvhx.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2lywvgprq.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2avymxhpx.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qzqbntbk.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2mbyvldrw.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2xxcxfliw.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2zofzadrg.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2hkujfycs.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2ozosunjg.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ewgvrsmy.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2oipivkel.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2rxtclqcx.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2usmqyjcq.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2mcfomktw.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2wvtpkmtv.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2xzuhygaw.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2gzvsgbva.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2qvehridq.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2sagkbqht.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2kaonaulu.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2iajppexo.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2xiongdhz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dwjmsztp.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2glfwamsp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dhijpbwo.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2dlvtauwu.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2mcmbeina.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2mtnthbtt.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2iobtrojx.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2iiqfykfi.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2dhcuezjs.html

);
来源：http://www.52xcode.cn/Article/details/gt2vegizdjd.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2zhryjktz.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2vaadrfos.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2yycwzaye.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2onkowuuu.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2wigsasyp.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2uocjtcyk.html

);
来源：http://www.52xcode.cn/Article/details/gt2rhuifxnz.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2codvpddz.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2fjbxkjde.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2uuqpozac.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2bjvudrdl.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2istobzkc.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2fhofeqqg.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2urwhtsvu.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2yopfegdj.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2buqamibt.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2tyufjnae.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2jcdtuwvj.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2cqqohiie.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2zldblguu.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2esqfxgsy.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2aespepkb.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2wnhkahrn.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2wkkzcvas.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2shkehauv.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2mkixvwhi.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2vjljqqfx.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2obosoufg.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2wzgkdrun.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2pqevlwuz.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2aqhrmlif.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2vcrlefzt.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2dwclzneq.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2pzvvhmct.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2xdhrklmn.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2legqsvsd.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2jecmurqy.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2kgmpwpuv.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2tvmaydhr.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2xubikgms.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2lezucpoi.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2hsszoefe.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2agyuyjzl.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2twzkdgyg.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2yzbplhsg.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2ktpgxqhb.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2wkcexeet.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2lvmfgmxk.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2lfdisfvk.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2gbuuvkkc.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2hnxhicfc.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2yoamlmaw.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2hswiqhjj.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2jmmfmsca.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2dytlppxd.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2jaglcugw.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ovsvwwpy.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2fpehmmog.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2jxyamoyf.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2lphzrbxe.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2prbjqiwt.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2bsxlqxlz.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ilqxdrmn.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2qodwartp.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2jaofctgl.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2mdwgqrxv.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2cjnwvtlf.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2gdltfbaq.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2bmvqoczj.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2dcykhztr.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2uuvskcqm.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2fzrwnefd.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2ttsqbslc.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2ptctubag.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2bfesrcng.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2fsajlegd.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2wyqskcpq.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2dmqyggat.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2jjdqerlw.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2tnimrqor.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2hnfbhdem.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2qhamugvx.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2khazmprk.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2utfqjwmi.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2nxnuefug.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2bpqdpopr.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2rkcceilm.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2btnlogcu.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2emlqgnmt.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2nddnlrjn.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2avsfvuka.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2ftguomzi.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2qtdlpguw.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2fypwflib.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2klhduotz.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2abyywjwd.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2xfbwpnwu.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2ebkffmsc.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2xigernsw.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2qbeponvg.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2ltutycxq.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2njvtvwqh.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2ozoxmchj.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2hjcdgpar.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2lsgzyzlz.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2uopwiaqa.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2yovessak.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2uzeuvabj.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2gabecwka.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2effkfiuc.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2wbzykecr.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2ajizofcu.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2dzhessug.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2amqkapln.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2zsvndfzc.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2libbglrf.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2ztlfnwwe.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2pquwdnbn.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2kllqanyn.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2duqvjdxu.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2busixdqf.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2mmbxzcma.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2ougvvnel.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2pgsfcqab.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2legmyzrz.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2uyqipeyr.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2jehsaywv.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2bngroluo.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2jlvcotyq.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2ylcislqm.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2ifrynnnb.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2qfgxfgnn.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2rkguotxk.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ldcuswqa.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2xedrwqxz.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2hckrgore.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2anqjnnkh.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2zlbdolir.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2xzmwygko.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2pfyrhsvl.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2pworrznq.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2paheqpjt.html


<!-- 参考信息 -->