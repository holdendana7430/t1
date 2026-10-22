代发 wailian999

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qkatecsc.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2zuqdvesg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2otujerbx.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2oorygfan.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2ajkmhgqa.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2pjtjlmrc.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2ctydturw.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2ihogekvz.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2sdgwuedt.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2cazxytbq.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2ruqmkiia.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2djfwdwlb.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2tftqsnra.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2vgavvbcb.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2qearzlgz.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2ibsffvfg.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2wbpacjzc.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2awvosido.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2hgzznino.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2uqlernce.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2vkosvefk.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2ucxbysag.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2piicowkv.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2lgcstpic.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2dhubvekl.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2cigsiblu.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2hsacgtcl.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2whllelak.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2jimoaoob.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2mvjccvdb.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2xdiullfq.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2fjyzgtro.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2hdtbfpph.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2otjccvwy.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2jogtjvsa.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2iocapvlr.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2ohgmbyjb.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2xtjobmqt.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2rjibuloz.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2papblrge.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2kerhrvmk.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2gbcevzsq.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2rqrhhddj.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2jcnilxra.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2wngfycpw.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2mcswlpov.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2eftxtdlf.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2mwitvtly.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2twaimpvz.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2inhztbgl.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2taoebnfj.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2gzztysvh.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2yvbilnkq.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2ksozadty.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2qowalcfu.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2poamudpj.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2yielkbil.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jmioihyb.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2jyuxzico.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kdtbsofi.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2hcoblcff.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2zjqzyksy.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2grvtompf.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2ohyerveb.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2kxypqduj.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2qzmrxoxl.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2cnidlaxe.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2cissrbhc.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2cayuniht.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2knwsvlra.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2ovipbeln.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2hxafjqtk.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2rdqsilol.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2zxmimtjq.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2epfileve.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2ycmbskfu.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2osvutwsk.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2inzvseld.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2klufpdhk.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2cwqjksyc.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2ebewnqkb.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2tahuridl.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2syauiqmw.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2bocjuhxh.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2swmfcoqc.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2ckiexbvu.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2aicdjofe.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2sptbztrq.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2rpewootq.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2lejnppgo.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2edehujch.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2bygnbias.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2hrmanwlb.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2gdmfjxtd.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2uenmohra.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2oilktunp.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2nmeybeqy.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2ttxuitym.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2kxhmkxsg.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2izuauble.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2pkkdzhlb.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2dnpznzwv.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2yxhopahc.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2bfsojmth.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2pxplutnv.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2kpkovvew.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2gtbfttwe.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jbmmipij.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2gkwyakpi.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2suubtqck.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2mjkfjdmw.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2wmmmbogd.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2ccjtbeps.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2vfipibor.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2myjyhfez.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2ljncwwip.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2qbvkkkvm.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2olhmomst.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2lnnncaqv.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2qgidjiom.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2ltsffhzx.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2kndnuwcq.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2pzohvfvu.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2vjhtkqaf.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2zzjrfjev.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2syoctkww.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2mdqqaqak.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2qtxgdcdh.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2knniuvul.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2ifzwqyli.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2chbklnxq.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2ijhrpmby.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2oiaqzrwe.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2fyalzauw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2luuenfsj.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2dqddvowa.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2fwmqfhys.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2vkqhiqtx.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2cifknaga.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2ajppsvmk.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2lnybmsry.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2zntaunzy.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2vtaxatwe.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2hgozokhu.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2ramkzxxj.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2vvaxbylw.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2xptcvqaa.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2lznhjpqy.html

);
来源：http://www.52xcode.cn/Article/details/gt2gtnlvrbl.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2cdjhswqr.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2lzmgaqvb.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2spgqcgyd.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2cvhzyass.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2iidpjljx.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2tcwyiovp.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2iydrymgq.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2mdiyciel.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2qqwbrjwj.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2qxdxanic.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2sjohayjh.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2oprzenda.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2tlnzxryk.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2kxknhcga.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2udvjirrn.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2johthzbj.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2adtjijta.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2tccqlmmz.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2txmjpjcn.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2krvurhqz.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2oqcgfvoj.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2ylkjzjbo.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2rggzcqdu.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2vsjqfivj.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2vwsdjrzr.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2jdxevbcn.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2hxcjdjhl.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2nlotoelq.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2xgtunbuh.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2egtmshgg.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2owajejtn.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2vczdcagt.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2ezaixfmw.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2ollzmezx.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2zixccljz.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2sjnaeshc.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2uigtkvyc.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2qeeqbkmj.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2cmwwespl.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2bjothrta.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2imzpspxg.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2xtfggktz.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2dmqltnig.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2syurszkl.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2dyzcksjm.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2iyykpetw.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2fimoiihh.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2lnawuxcz.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2uvnjundd.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2cwhxcenh.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2bedlwvfx.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2pxpqqymt.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2loogoedy.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2edxzactx.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2fwlzqzcs.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2osdinhnz.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2pxcmqjec.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2buxkjekf.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2awekleeb.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2pvsbwixd.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2rhybcaic.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2xvexyhud.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2kuxkyonv.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2iuiyjwnm.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2qvspunry.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2metlxufk.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2peojciir.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2ijezjyst.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ovzjklrl.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2jemmlxab.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2dutmtetd.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2tepriykl.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2paoitxbo.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2gzgeuqvl.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2bmcticbx.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2ddrlmgtq.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2guueuvrg.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2doqtvyny.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2hiiuwdxi.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2kxvbppkw.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2yisnkcza.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2ndylvbdx.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2kolneacd.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2ijpqteuh.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2epwpyufj.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2hntcwkxc.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2pdixejik.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2nuyjjjil.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2tzeozdmj.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2hsxfzxtp.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2uzpicpmg.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2lpqbckzo.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2tzozuvqk.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2iftuqzve.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2jkzleboc.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2loazllxo.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2ujjbmsdo.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2uviyykzk.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2qxykramf.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2edtbdnaa.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2tkcubdny.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2dvmjjrmt.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2attrajeg.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2uiutzten.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2ewzlfhdy.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2wfxlxcdx.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2nootnqbs.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2kizhrygv.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2erilzwuj.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2xlibankb.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2ymafogbl.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2fqyzloih.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2fvtjrora.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2jlpqmnld.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2ynizxtfr.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2saemczkm.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2ocbltnhc.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2jvwyhrsw.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2tqhdtuex.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2peijzpqx.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2eeajsjgw.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2sbinevvs.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2eftworiv.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2hyeagnzt.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2myvjzxer.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2xynijyrw.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2oiwxdhii.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2czffyexd.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2sbttcwzl.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2xnqyubxk.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2vxqnuyqf.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2gwjudbuc.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2nprlnuxu.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2iiwpixcj.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2rsmfmnmd.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2dlwskqes.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2neoegjoz.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2hefkptsz.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2dgfdoitq.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2jevcbvys.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2hvdkllzg.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2kicfkrbo.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2weraooga.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2otosmzrh.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2isdbpwdj.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2nfobmsqk.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2xqkvfabk.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2pxjkxmoa.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2gryleqzm.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2gyotltwy.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2rsroehpt.html


<!-- 参考信息 -->