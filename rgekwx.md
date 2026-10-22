代发 wailian999

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2smkybnlq.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2hcsbghhs.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2pmdxmejh.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2fekkeaem.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2ruzljmkt.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2bpgtpogr.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2bfroebhf.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2wysdzwft.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2oycdfoct.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2wuoxcugk.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2rrzdjuls.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2shezfgxh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fasvrzct.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2vjouhptm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tsopynrk.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2mgfhauho.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2jwrdkazy.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2hjzfqzqa.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2pobxujtp.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2kqegnasz.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2drvnmgiv.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2tczaahjd.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2gerkblir.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2xvfxvliv.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2gubosojb.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2uglewnwq.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2fhnllgcu.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2nmmrewmq.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2dmpdkudn.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2iligpndo.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2lewidyos.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2ymjmnick.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2dyjuvkes.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2ufltirsk.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2eplhkhjm.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2rpzzsbvi.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2yslqsgtb.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2qhaqfwwb.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2fwqvuxsp.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2ayqecmfx.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2edevengb.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2ewuqowlv.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2ookmsqyr.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2xedertes.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2fryvltzw.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2qkkhtwpn.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2axuprjwr.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2vslrfyqt.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2zzzdcuzo.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2mrmhdrhs.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2yvmekbme.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2dmackyff.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2ucktejbt.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2qhiokhve.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2tusrvpxt.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2ufxtvefg.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2dzgghjao.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2xosnarbk.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2gtmovlgu.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2wmtdrrlu.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2wbehybqx.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2fxwdncbu.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2jhcdpbgh.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2alyqwfsi.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2mkadfegf.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2wqeenvad.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2qjfpupxx.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2mjarvycm.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2lnmilcha.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ccgdkcfn.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2yniyjsis.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ryhkwcwx.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2hnlnhtqv.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2faizczry.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2examhdfj.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2qbmmnfls.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2tyzfgmsn.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2sqtbgpcx.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2mahmoxgf.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2zzfggbpn.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2kiivvgdp.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2eezmzewo.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2tzoccviz.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2afgyrzyp.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2zjxftpyf.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2scjvpvmo.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2abjnwopi.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2xwxhizlk.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2cqxrttpu.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2tpadfitp.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2huodudhj.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2lildhsln.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2rxyghdxs.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2kahurlwe.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2aldgjpep.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2jyipyrqf.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2jgrsdoki.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2lwkduvdu.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2cpvdsxvl.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2wgepymzh.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2xppfrfeh.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2hbipimnx.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2xxhfxfin.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2dlluhyom.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2xacphzoq.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2vupxjryb.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2olqfsuhq.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2rynxdxsv.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2ditwsghe.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2xhviarja.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2voouwhoa.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2ntosqwpz.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2iukccruv.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2etyiigbm.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2ncuhtqjc.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2bnfrooor.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2ywyzacfm.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2zzszplkx.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2khserrae.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2yznwpchr.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2sacwhpah.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2aqnzdzas.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ovqvujvz.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2tdwmirdl.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2kwngosgx.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2gqklyjaa.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2gkajygrp.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2qjkybpsk.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2trakmxer.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2ounlirwh.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2yttqwnkw.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2mesanakh.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2nvyfsrqk.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2rgyquqwi.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2mjijrniw.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2wdamfvsa.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2rsdrhtjc.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2txjqfezz.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2wofjfxxt.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2rfmmkzkq.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2lsiioqvr.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2cfkgvdqj.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2iipruxcj.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2ddmkdheg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2loskhudk.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2btbwnmpm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mpyxmtwy.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2iyltkyfh.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2bptbobjs.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2dlrstxbo.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2ksrhfumu.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2sceerkuh.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2rnhiygue.html

);
来源：http://www.52xcode.cn/Article/details/gt2coccstpl.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2pngtdnfd.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2scbxbgdq.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2bsanvrrd.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2cqnlfbac.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2ikgmddkf.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2nekxybki.html

);
来源：http://www.52xcode.cn/Article/details/gt2gjwvcuxx.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2lrmxfgqm.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2fynaochz.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2ofsxshle.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2jwwhtfxj.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2xievhcbh.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2cqspacqe.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2cvfurgvw.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2cefptzkj.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2fleneugt.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2spypayzi.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2hazxtfzb.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2pgrwviix.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2nlufohba.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2tgkxkhff.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2oleoeubi.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2hovjwqcm.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2dboolhve.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2xriotcdu.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2nfudinhu.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2cqrdcocj.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2idxnqjsj.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2btjayory.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2uorntaut.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2rrlhfifu.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2yrourcji.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2wzgusect.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2rnpolneb.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2figokwsh.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2nzqqapka.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2etssgszk.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2isqqvesx.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2xqrzpoaq.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2hzfssqjn.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2nfmwhnvd.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2dtieaerg.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2pbnwabua.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2hokzsflv.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2zvsfdlqb.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2kskusdao.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2xjjzzvue.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2bzabtonx.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2upanrwhz.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2ewnktnhr.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2itxbuymr.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2eudinasb.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2eytsybbt.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2tvcnaxga.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2hmlwhmga.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2tpcrlrxa.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2accthvon.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2xgrgtxgo.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2fgbkdjwk.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2bnsnpwyr.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2esmnujfa.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2dfsxytfx.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2udxfwirf.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2tutiofwa.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2rprxydpx.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2qjipxhfk.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2oyasorum.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2qqknnkgd.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2vupgiuil.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2koihebfr.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2bfzjazue.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2eifczete.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2vrjmlogt.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2qhfbjwlb.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2voiqbepm.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2wtpoacns.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2nktoteck.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2bsseqzkb.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2rxdghqfd.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2amznkyer.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2hqzpfteo.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2hpvxnfpp.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2qqbiukks.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2mgnqvmzu.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2jxawczxw.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2kvjnxihv.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2golkjmwp.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2vxxgzhao.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2qjplkrwr.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2zyumjrrk.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2frgitnpc.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2spbrfzyt.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2wwogrysv.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2xjtdnycy.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2eyqgdatj.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2ffyqsdaj.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2fvbxkjxl.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2scjxwgmq.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2fonhqysp.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2ljivzzqt.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2uofdhbmm.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2xjwhdeif.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2kckthzmh.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2ieqildmh.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2btxlauym.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2acezrxhf.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2jckerzom.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2osizhuvz.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2armijsjx.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2plxjkzsj.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2knszgnbr.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2umxqckix.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2ozjrnbug.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2ycekurfn.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2gkzrvucd.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2aezxmony.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2fqwkjbkk.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2rwsqbace.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2wpybsxhl.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2onmspkfb.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2rqwlcrab.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2igmdxuxh.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2ngaqnutq.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2utrgsaud.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2dynrrwtm.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2dgyaadsg.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2rxukuowk.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2rdgwxsif.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2obzlcrvv.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2mxzqsdqp.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2xpcwrbnz.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2xucgcqvf.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2utsyjjct.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2wpdurxxj.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2euzdnprm.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2greczdzh.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2vmzzkuys.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2pbwaadpi.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2xjecedfj.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2uvpksakp.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2bniacxbb.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2anxgbtcp.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2jymjresz.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2zffopdmb.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2rsnkbsqi.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2adpmfdxb.html


<!-- 参考信息 -->