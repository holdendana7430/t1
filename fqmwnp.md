代发 wailian999

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2jqlbwlsm.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2lqatcjyi.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2buoqlaru.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2vnqmoihx.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2cgpfrjdl.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2lhzaqped.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2ktwbmmco.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2uhuoglet.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2xohnqosw.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2hotaftqx.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2knqltwke.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2rnrfawbk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2esmdcyeu.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2bxjahvyq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cxtrwtkv.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2dxlmxocn.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2ujwavoch.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2qmlmmgrz.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2pboqnkur.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2kohjinog.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2ljhxqjvf.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2heszjqel.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2adftbdzx.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2eiimlnol.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2lreulvsl.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2ykyjztza.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2zjbsndfr.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2nawcwved.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2slahfpea.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2nvpgaeuj.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2tvfqltny.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2lljxnksa.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2oymhsdej.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2njhwjidm.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2xfynyajg.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2srjshhww.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2pspfcisq.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2ogoqzngg.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2jmzugvch.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2etiyfgya.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2iphiwrqk.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2monzlbjj.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2mwohuush.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2bmcuvpty.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2tdshbomk.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2yxpdwrcj.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2hsbfdxlq.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2fktyayqe.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2nxsvtiis.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2hxgdlkjk.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2hmcxogak.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2qkzrpugn.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2jotgwqwo.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2fstvymvy.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2hvbcmrbl.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2amxazriz.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2lazueqvc.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2gepngynz.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2dbrrgtkm.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2ohrtthmw.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2bssxxbhn.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2iwxylzeu.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2rxdxnvql.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2rthtmrlc.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2cryextan.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2wltdspta.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2xbzglndm.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2weyzwvfs.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2swzurbzx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rsbryeyw.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2bdnltbor.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vxkcyupj.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2hfrlrcbv.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2dcyqclsj.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2gyirhzwd.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2inpgnuuq.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2wuyxohsy.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2vhxqsytp.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2rfzzvole.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2ndstavma.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2jnronccj.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2hxbuvhxs.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2llstzrkk.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2kibanqle.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2dpjspzgo.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2zquwdryh.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2fsfgsexw.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2kjvnkvox.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2obynwbhx.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2nhgxqjgh.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2kbdomqqo.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2cgvldmfv.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2yysjxckq.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2tlffkuxp.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2qpclfbrb.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2dsurbiam.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2svnzcspi.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2tclqguaq.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2wxzdijzj.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2biazsdsy.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2phqueflq.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2htzurnfj.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2gxihpxze.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2phbmycmo.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2gqeyjhdv.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2gyplatlq.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2bsavcsge.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2ypsxoaoh.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2jpclvtsx.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2kjjmfsrd.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2unoxdmmf.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2egkznmkm.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2jloowfdg.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2jydfjwbp.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2ndwxexih.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2hrbypmav.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2grrcpbwu.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2lhdbskjy.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2tcnhbtpl.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2gpdbmowg.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2eldtidqr.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gcuttmyf.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2utzsezwj.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2vxjysxbk.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2cynllnez.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2czmdwvak.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2tdjnplmb.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2riuuevfo.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2koswdtrm.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2flxsysvz.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2kwvakldo.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2ptueswyb.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2elnnjofh.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2efwzmekm.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2wapbsque.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2bgohuqxp.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2nmwrdxxe.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2dgcekuam.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2elnoreha.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2tzwugxdo.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2xucpejrm.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2aaymtudm.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2kogfeijz.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2vopummiq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2swihkpus.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2saibikeo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uymvokwm.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2jmauvate.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2xiapnnty.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2pcldfjlx.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2valqcpkp.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2dbxzmimp.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2dtprutmz.html

);
来源：http://www.52xcode.cn/Article/details/gt2osffwugf.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2kxbbwdtr.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2edygsope.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2qjggopbn.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2vxbzvkiw.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2vbnesovk.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2wngantde.html

);
来源：http://www.52xcode.cn/Article/details/gt2afqoiozf.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2criwukia.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2eqoipgzw.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2frpessfm.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2ztyhcllt.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2fbmuvsqg.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2yybsuayt.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2avmoelre.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2smzhefgg.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2vibbcqjx.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2zwnpdmjc.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2vuqkdrli.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2wvhmiaks.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2xkkygslr.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2tfafuhaa.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2rqwehmuo.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2iyfssvkv.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2qshoyauy.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2odtibksd.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2dbujoqpd.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2qpvoxmid.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2zfnyhlsm.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2fitljvgr.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2yjvvspgb.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2otmtxlkg.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2fsjdtcgx.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2rmzargdp.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2aerkvizr.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2mojkrnsp.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2zbuvmbxc.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2uvmsfcre.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2qtatuxql.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2jyyrljad.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2vglukadm.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2rtlybpxi.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2vfgisdjc.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2zfhrrhaz.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2bxldwvyt.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2yxaiazqe.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2rnxogspl.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2ralctuzm.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2pzeoukvs.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2ftpuvqig.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2nperjqai.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2vvtljifg.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2xqqgifpn.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2kwwsnizx.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2kbantzfq.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2fvnzbbfs.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2obxqwfox.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2togkumiw.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2qxgllxnb.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ftlgnmjw.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2jcuysftp.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2iyvbirtq.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2eassxssa.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2buwbflkv.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2jzrwnpur.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2ttjhckdc.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2siaxnbom.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2cktsugar.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2xfoiwonq.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2xnuqtybb.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2mabcmjtb.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2mkjvnkbx.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2qwixpxav.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2nktzeuia.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2pniforfl.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2ksoliizx.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2fasaflic.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2odslsdej.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2ebuvewlp.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2rilshgcp.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2cfroxuzw.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2eolgnwjh.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2gnxyugig.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2ncasuvle.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2ytrpnenb.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2atfvrgaa.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2eailtigi.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2jzftkndu.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2tomtwyur.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2rvcfmnmx.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2bhlfcczb.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2ibwujfig.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2bsypydta.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2cwncalvi.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2uvsbodmn.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2umkjcwze.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2quztzous.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2gvswjjtf.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2zspvqaoe.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2shicejco.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2lpbzajhz.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2grhyvklw.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2wjhlaooc.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2fgxzdagm.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2nnibrczk.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2hoxtoxxz.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2nxmxdwrg.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2slgetdzy.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2ikvymhkq.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2orvlayqu.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2pjxmyifw.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2fjtcgtuf.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2luzcsczw.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2ntxqrzni.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2zvgaekkb.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2lmnxtohu.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2cvzhwwmx.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2wnytzlmk.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2csapzuac.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2kcbuwpjx.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2fokowkny.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2mgsdsuzo.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2foioezsc.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2ypxhfpmy.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2luizkauf.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2uietwehc.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2akfgylin.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2xgynephy.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2ligwqmco.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2rpequoeu.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2fqiplhzg.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2osrtxobp.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2neukepup.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2rljmrrrb.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2woszkrng.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2udhhxzrx.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2snrzfvwl.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2wbhdzicv.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2wdqolxma.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2bcxilpmy.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2xfdnehjr.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2vjvefuew.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2tuybzxoc.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2aftidwen.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2dmdsrpph.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2fiwfmbys.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2wyjfmcyh.html


<!-- 参考信息 -->