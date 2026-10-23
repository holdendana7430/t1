代发 wailian999

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3cwknxlct.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3llnuwydu.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3pfupykhp.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3acieifej.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3yngwnwbx.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3ybekfnmy.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3rmwdckqf.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3kvrcqyls.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3gklekjys.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3skqkerrf.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3hulurgpl.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3ptwefbge.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3snoxudfi.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3mufsfvyc.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3bvedvjyz.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3ipqxmrms.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3otwuhljv.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3dmcyjscy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qhruneos.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3hijchqrp.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3pqodkuov.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3peldqtbj.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3cefozvfk.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3serduonw.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3gfjlqoqf.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3mvhkdrcz.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3lgylcyav.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3gfllrjho.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3xmfsoiju.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3xccfchjt.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3mdetpeuz.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3ihlwnpts.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3arecwgxj.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3wvgrbkct.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3fimnkwkm.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3bgpoxpej.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3oicreiun.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3smgcciqk.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3qctjmpkn.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3biufehta.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3meooocqm.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3nnzydcve.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3luyrqsxx.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3vsymdxmo.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3vmkpbzhs.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3tnpmkerz.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3mogkrkug.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3uxjmhklo.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3knsfvrmx.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3sfvgdyhh.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3wbdyylsh.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3lvkskfsj.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3qgcmtsjp.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3dxdnwxvq.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3wvgotioj.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3lrrjrhch.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3vlcdqvyb.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3lwmnuswi.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3fzvsnzgt.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3kkvwyjao.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3qtblgsoi.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3mrzzhdqg.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3lsufgpjc.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3nwqnfxwa.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3lwkaukag.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3trsjccux.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3kfoggvxd.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3hekdiaiq.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3kxzmjzkg.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3nuuqyfju.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3wrmtrrgj.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3hbfvebrr.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3moyiqxxy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kbprbfmz.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3yuwtkqcq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qrbkjbeo.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3zxucqjxr.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3pjcrewzv.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3hvzdpbii.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3ednntgzm.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3uoryulsr.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3jqdmwase.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3wlzcmebw.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3herbiutl.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3vzbttwwv.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3ybrhjaeb.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3pzunxcnc.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3iaqxvoja.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3cenbuuhf.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3crzjtqkd.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3ecofftre.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3lxzkrqlv.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3oihrkbjl.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3otoenheo.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3lgywgkcm.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3opaujrlx.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3wovzdvjf.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3goldjsvc.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3zkefhrpq.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3jsbuxonn.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3bmfmercn.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3wpjanplb.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3xxvuljpc.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3vpwimmxp.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3mgcylyge.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3slifwzdj.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3lckrjpri.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3pkacpprs.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3fnfkxuin.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3iupsdstk.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3ibmsbjsd.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3vxquzbxn.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3anvpwdic.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3ejokjuqh.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3kpqnfaij.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3wumhgono.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3zgauonxx.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3rnewhnyl.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3aorlofjs.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3thgdrugt.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3eklariyg.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3hrflbagf.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3mmcbalgu.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3blimxwvq.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3xaifdpic.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3wlguczon.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bglermnh.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3ncipfvie.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3kvapjpbb.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3migrchxe.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3scaqjrmj.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3yjbsyqkx.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3azcixpaa.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3mpwtecjk.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3mxgzefmg.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3domthzrm.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3duxaapdf.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3orisbuag.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3nxdmqwae.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3eyficlbd.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3kkoviyvs.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3swmxgkgq.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3nyyvzdrz.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3rkaxgdrp.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3zuiusrvq.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3ffzodgro.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3dzcjkssp.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3mcseqppy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3etxrchrx.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3zpgrooom.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cbcggeyi.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3ynyrcmao.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3rqvttvxd.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3grjfohqp.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3cujjkkaz.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3hzxcjsmh.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3ovkldlik.html

);
来源：http://www.52xcode.cn/Article/details/gt3nyofornx.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3xegjrkkk.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3jwfdkeat.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3oiqykmyg.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3rvrldyge.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3tdookwge.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3rmimtwco.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3mwoizoqg.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3ipofyvmi.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3bkwfglph.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3gfixfzwr.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3bbynskbr.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3xjeiazxp.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3xzkzwtmx.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3rlkxzupk.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3yptextxd.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3tkinflrk.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3giljnbad.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3blxgkjmo.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3aujmuman.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3ffikprqw.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3omfasekk.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3ththglgy.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3albnbyag.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3yxgivour.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3fpjecesu.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3voopusnh.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3yelrqbtz.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3mprgqadf.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3tpoqzrdi.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3meybhcia.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3jmzvmtoq.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3wgziysxz.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3epalmfsd.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3wcpefpik.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ayuccbty.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3ucuzqslh.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3nwtqblds.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3avoiogtf.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3sjuolbpq.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3sunwjvwp.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3rvaumgeh.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3ozjlbdkm.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3bpqrzabe.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3fhvsplqr.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3ngnwnlou.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3rasnxkph.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3obsqqveq.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3qtbsitrl.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3pmxiaczm.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3ymdjvsug.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3heiyblfi.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3sonsprbb.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3saxlnaea.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3wmzcquqq.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3xjpmamkj.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3brbgdqww.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3yzregxdp.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3wztyxtbn.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3dcgznlid.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3xjyusvda.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3fqhffsls.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3tpbbcucw.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3rcacqcjb.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3pglgykrq.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3bhonvduo.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3waurfssa.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3acmnoinj.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3vygzxypm.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3jyaujekc.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3zqsdpxug.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3rlkufprw.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3mralubqc.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3srfeccue.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3thcfwlgf.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3gxrmrrbg.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3efojwrgh.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3hfypcfuh.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3dqnujosl.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3yzlsyifk.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3srcuxxoq.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3suskaeqd.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3evmbarmf.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3vbirbvxl.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3ltdigfao.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3ioyheewb.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3tchduxlj.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3vebcdckj.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3pbgbobgl.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3mrjturen.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3truscxhg.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3ykxtmnnw.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3curbresc.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3qvwwihaf.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3wihegmiv.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3inayjpzx.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3rfnymubd.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3sekcwqrt.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3ojngobhl.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3aahyrjja.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3fofqwzrb.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3dnvrgirh.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3grlpfvok.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3xydpexao.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3nzhrtgpk.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3glpbdukl.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3cfirimry.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3jitjlnoe.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3ndertuod.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3ztjujvnq.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3emjqpyap.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3npmqbnul.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3mfncyuqu.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3ngnvcizt.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3pcbwzsdq.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3kmjjmxci.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3ydyjgxlq.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3xcqqyqpk.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3zwnxtimv.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3nrgzebkw.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3hvlaakxx.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3xtlapjtt.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3ehjkenkq.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3bszrogkt.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3mdnadcfh.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3ttczuhzb.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3dhqwdkcy.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3vqtrlrwe.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3bgyuycji.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3wabfwbux.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3wsvnxlas.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3ufmovqdt.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3rnwhujqx.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3spxhkilb.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3viyrppbk.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3oglacuea.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3fhvkyywa.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3lsjbiadg.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3liadiyhw.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3hglyayyi.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3yzwmenjv.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3orepyhje.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3qbjhuqea.html


<!-- 参考信息 -->