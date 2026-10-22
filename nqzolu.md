代发 wailian999

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2tzmtgfgk.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2esdmmvnm.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2fsapxfin.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2rslirixz.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2gsmufovl.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2numswpas.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2acmhshhl.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2bmvrqflv.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2dtqwygbp.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2bthrlsxw.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2zclkjpdj.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2unjqomwm.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2qrdxitnu.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2oswdusgv.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2cdnvmxck.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2jyuykfsq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2erjtyrbf.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2qmtekhmb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wzklfuus.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2qwgimxwh.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2asijfprp.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2jtdkwhbj.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2vwrfritc.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2brlssssq.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2paohbpld.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2wkginglb.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2tycjetyn.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2whxlwhjm.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2bfpsjlah.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2pyhdrfdp.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2ncegkgif.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2irzdpyvg.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2wpypjxpq.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2usunyhkn.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2glccwpms.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2gbfmhhgw.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2jnolsqrt.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2ggtvmlmu.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2uosjmgvx.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2hyhzzjix.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2czuwsrov.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2tvtqbere.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2quzraalb.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2ghkylqnr.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2mwfloiuy.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2dmhmxtod.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2aqoofxwl.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2assdmssl.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2ojnswkbf.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2kfzduuvy.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2javjtduf.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2cnmcqipv.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2cyzjpsnw.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2dkskjlaq.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2afajpwep.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2cwzfcgjl.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2kkhotoha.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2racgrvrv.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2mrnjgrps.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2puttlwtx.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2nvzlbxuz.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2xjebxjll.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2pvlyqfle.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2jdziyklw.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2ndolwwgq.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2dyoillad.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2rqkehpoh.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2ydowkoxw.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2tpnlgkrc.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2njtgravk.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2kkposmtq.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2vkpkckyx.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2urrkixel.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2commspqj.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2khcyvlmt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ahwvcaqo.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2tvkfmtoy.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2ffpobeht.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2cheqhzkt.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2fxzbpjwp.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2mscdjptz.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2jpluxpca.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2iqivonpm.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2vvcodeeq.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2jaanqzrl.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2ncyrcmjc.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2xogvwnre.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2fzhkmgdf.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2yycwaxwp.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2upvgctms.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2ebyquzoa.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2xqdwbvww.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2gyisdyvp.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2wtkypbnu.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2fsnjhbzm.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2zlijzndo.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2unoausrd.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2dkcmnfqu.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2xxplgiuh.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2mdxexcck.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2gzaequss.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2edzabacy.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2ycncvgny.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2dnbogiec.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2ughnpagi.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2zdoiovbp.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2dlvartls.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2csgyvkpi.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2ozaokgxf.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2jmwgfnrn.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2taslczff.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2udodfbmb.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2pkdoggih.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2ziwjjurr.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2ildrsjam.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2dtnkvtpl.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2utxtwjns.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2hndnbcrk.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2yrfqloyg.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2tazorqnb.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2czfxkfdv.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2hyaensgy.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2meskixpo.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2zgtgjxys.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2hkwggrel.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hivaqfns.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2qmslpxqw.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2cltmcmcs.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2fyhvayrt.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zsppapoj.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2qilchzwn.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2jgcswynu.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2qxskaczh.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2qblwtyqt.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2jcdzrjqz.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2piurpzdu.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2jxpyifmh.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2lhqkbakj.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2kcnteoem.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2abreqtsm.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2nwttgpkl.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2rjoqruka.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2izyueeza.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2wlrleltq.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2osviynjt.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2sebtfbkt.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2cqyirrgg.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2plitphdq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tpddrvsr.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2dhqylawn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jgtkeevu.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2rzgqrhhx.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2upotpwxs.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2nnzmlvko.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2jdngnwuj.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2psyspghz.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2zwiffjgm.html

);
来源：http://www.52xcode.cn/Article/details/gt2sikvvsim.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2ojtztzpt.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2dulmmxvv.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2huioqcsd.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2ojsgfjwy.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2gvhjczvb.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2hvxeizob.html

);
来源：http://www.52xcode.cn/Article/details/gt2jhvajnjm.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2pjyqhzyt.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2cnhjuogk.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2ejyunbkc.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2jinvtlsp.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2eiaftaym.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2sgbxlpeu.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2bjfgdyxo.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2ordefuop.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2zctpxgug.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2grprswex.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2mzgczblh.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2zbxtuxav.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2idnrgbzb.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2chswkudl.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2ejfymspq.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2qgtjojpi.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2uisqkqym.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2vhtvuygq.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2bxdkbake.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2aqhslnnw.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2shvmhgxu.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2dizixrad.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2ghlscgnf.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2fnmduxai.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2iwramxrc.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2lpuiykjq.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2poglhurs.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2hucdfhpy.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2oatjussp.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2zhshhnku.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2ftyqkaci.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2mlblqcej.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2lpdxpejf.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2krtmumiz.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2jjdgpabs.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2rqzyzimh.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2jfisxtlj.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2ukjikdek.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2hduxtkde.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2qiefnoww.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2pvhfkkai.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2fllkvngs.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2lrojdcqu.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2dzbelhej.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2ihqogqzp.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2huyfozdx.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2bwdpquqm.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2sbkzxktv.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2yiwhfgzy.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2sdqbwrmc.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2qgyxmmwm.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2wfirjgzc.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2qcxkojjd.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2rmiiudar.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2duknybbd.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2qxdslgbe.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2elecizxy.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2mtvqebdb.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2lroywwdw.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2ioohbwtr.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2qfrkijip.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2izzsnsnx.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2ikwyzcto.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2yzvqcexk.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2ommwgcap.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2uksvmoan.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2zwmbbdtg.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2eishrfcn.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2qbsfmngp.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2alztmxfs.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2ihkwqadw.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2pntblbkd.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2fmmckdnf.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2pfmxcxur.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2zgwxrnwc.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2zrsojbmr.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2evinmzrx.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2toriqupz.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2ugxwstuj.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2xrujkfvr.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2atbdxfot.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2gfkzfnnr.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2hwtnsquh.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2bebcfutx.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2orlbnaat.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2fqowhzgu.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2whsdzxgr.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2dqdmrxdb.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2rdlttovn.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2ryfqhrhx.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2obenjihf.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2rercwtgn.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2fkshhdmm.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2yvhgeobu.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2uxhiskzu.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2tywccdgz.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2rookeffv.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2pjrnwryh.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2iltphsdw.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2bnerwekj.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2lryryqoq.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2zwuxdmwa.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2lnktfgjj.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2jcjaqmzz.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2xohopyrz.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2duppobyd.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2tvljpiud.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2hfcplfna.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2cmbspqas.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2jzicrksu.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2mqctgqsh.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2mpsrxalw.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2dxokafly.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2ryerqivd.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2bctwyerx.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2zplnmhcd.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2gezlllfg.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2qiaculke.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2zegsttvo.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2jjfhtcgg.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2oneljuvi.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2rwxfsxvp.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2cewygxqr.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2opdhsfzy.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2rdakxpct.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2cphyjvlx.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2xertlvfj.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2ubghzjcx.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2rgrbmjip.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2vpxnzoqr.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2xaubmpdc.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2eazihskm.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2pqmznlic.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2ermuvgvf.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2hrvynhhq.html


<!-- 参考信息 -->