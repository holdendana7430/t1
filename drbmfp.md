代发 wailian999

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2pugmauoy.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2stgudocr.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2vdcrnxph.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2bedpdete.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2pnxgdnig.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2typwhbpu.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2xcehkurj.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2uvlbngzp.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2itlzrpgq.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2gabhxvke.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2esgbbtkq.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2cjfomuvl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gnzqbxyf.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2bsamyrut.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kovfvfcj.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2afxxnaoe.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2tjdspetu.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2ojuqcuzk.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2tllzkjhv.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2omfmficc.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2zngwvncw.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2jmwgmptt.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2mgqeoekv.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2uuoxwwrl.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2motyfejg.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2pfpndrwj.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2cnabaonk.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2rjgrtoxl.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2daalfywd.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2zjygeope.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2gxeqmcrj.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2xqgqnfpv.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2klohyjnn.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2zbrqnsmu.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2qepzmwtr.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2heypiknl.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2kuxwuana.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2qsobjwww.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2fipnpacj.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2zjirzuiz.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2lmymogww.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ouhykwxd.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2bliqjvjd.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2ymkdxkjq.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2ihdhwnvb.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2bpudnhqm.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2pzicvwor.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2qnuxteia.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2srxpqauv.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2bgthcxro.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2wfmiogsa.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2cxwudxlk.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2nugetskr.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2ckdbiveo.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2sebknsqe.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2atgghpmc.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2udsldghd.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2mqndvbkv.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2hqpioytm.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2psldmfao.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2pqzquryy.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2aztryscn.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2afatthtl.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2siyiybpp.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2qcoulrod.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2uwiqeegk.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2bdkvsnaj.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2anfnuwsz.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2akrljamv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xxieujmh.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2atrlaace.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2agwbbadu.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2wxgmzjpt.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2zozwkgyo.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2dlomlbiw.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2qayympje.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2jtwbfdei.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2ibagvwgq.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2nxkpyqyo.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2hhbplwlb.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2dvlgprbf.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2jbbtbhmm.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2uebygjnv.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2iqkbctun.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2kwgtdarb.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2ewmahcvg.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2mploqryd.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2hjmoxtoc.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2wwfsqaja.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2eicryffy.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ehksbioz.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2qupyfans.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2uyirjgje.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2wziigywd.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2bvlhjdlp.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2elcefimb.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2xzbgbvsu.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2xcxvjjcu.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2ubvzcjdk.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2butgbmyy.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2wvcoeyhw.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2biwlsooo.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2jyytolli.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2wkvergom.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2zciglbst.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2zjrdznyw.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2unmftsrx.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2taoerypw.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2azalywzn.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2ppqhenmp.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2joxoybwz.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2yrrmzlqt.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2edhxzknr.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2pwahvqpl.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2lpdccbdt.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2spkmjnti.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2tkshuzlg.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2ammzsifb.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2efcqnvcr.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2jcmkwzaj.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2ptvxqdbv.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ibofgatm.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hwbqsbli.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2dpefsgqg.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2cgbowksm.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2xvktkiqp.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2xdewqibt.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2qotiigyg.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2kifnkzim.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2kpezaoom.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2dbygjwbf.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2srppaiih.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2pkkvlgrz.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2rwquhlwg.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2qxcorcpu.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2qbanzfsj.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2bpyzkeam.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2cfpkfslw.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2mylcajlp.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2bryoxmuk.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2oiquvvoo.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2kqmuhkhj.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2plnefjfe.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2clbwqlif.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2whryhpxn.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2ksxhebeu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bdmkbscc.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2efjvxhwv.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2fgbjftbj.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2brflaehu.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2ojhysmho.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2kxhwlwkw.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2chwlfdib.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2hekfhsvo.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2sevlsuml.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2skmbdkkh.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2ujcfflnx.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2nxnnjlki.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2jrmkwbhm.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2haenzvll.html

);
来源：http://www.52xcode.cn/Article/details/gt2lnmeriqy.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2muapfuyv.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2yjdwwrza.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2wuwajqjh.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2yhdwqwyu.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2mwzjhcyc.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2yxxspfos.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2uivhnmns.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2qmrlsdkg.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2lqazwfmz.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2qngjpqgo.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2tshtrxio.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2hfeittvo.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2nvbhsjpi.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2ekzjoxgc.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2magubfuw.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2gtlaukzj.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2whcvziyz.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2sjiuxgep.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2cjlkkcaj.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2vledfzwk.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2kyhgujdg.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2smkezgfl.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2jjiybqzw.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2njdxuzdv.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2zoqewunm.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2wsioanck.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2dvjkzppr.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2skhojubt.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2jqwvihds.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2qekzyoka.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2uysykolt.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2mvzsozbt.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2cdznggfn.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2ujsjmoov.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2skaqlwhe.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2fdzagpga.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2plfvgcvi.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2qxcohkpf.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2zpdtvbxf.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2xyhdgcje.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2ngzfsesz.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2plamzasn.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2ipnnrqnv.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2oujsvtjy.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2aytccgcj.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2saexfwln.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2fnkdwsxg.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2glsinmlr.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2xsruvaau.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2vkgukwic.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2ogzwatpn.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2tquqrjye.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2nhhjpvtz.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2bwlxmfcy.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2ugcpiqdy.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2tdvzzkgp.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2gqoumkvu.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2bcuvljcg.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2hxckximz.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2ykplbftz.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2idbzeqhm.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2dpajnjnw.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2wgugmeru.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2bqzubzaq.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2loqhlnjf.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2vlxjvqtv.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2nszrstne.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2yezvrwue.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2uktlmxnc.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2khnfqgmi.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2pvouzimx.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2ydrlytns.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2ydolzgcj.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2cmfupnxx.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2lqkenobx.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2adeanops.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2uewkcxqx.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2qqaoesbd.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2xiybgksk.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2fwffdvdo.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2cpywfqdb.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2oxscgltl.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2ndwomoaf.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2ucinivfv.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2lmuaneuu.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2lrhxftdd.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2vvcytxuw.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2qfwtvzgv.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2yemetixx.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2fwilpriq.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2svwtzjuz.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2tiqgqbte.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2gjhcmltl.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2hxfbxqai.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2obmtuakg.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2zwnatnun.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2omuhrldp.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2umapsbou.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2zjxmdfgy.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2ofvjwnds.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2dmjsxacr.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2tqtaxfdw.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2bfldoznv.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2yfvoertj.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2sylcqwet.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2dyynpfmq.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2qcrxbguv.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2axrqwbal.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2dzpbkfwk.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2fpcxwhab.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2armxmotn.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2cyudbnse.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2imglevbb.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2ttrvkkco.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2wzkajgrp.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2oifkunkx.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2pziwunla.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2cqztrdeg.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2hmilfjao.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2wyvgnxth.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2nejjprwr.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2bnglwfri.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2lutgqbcu.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2wtbgsoog.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2wwybyygw.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2pvmzsrmt.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2xmwmbfii.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2ftpnwggk.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2pwctmgio.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2ppsjqvqs.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2ikrehqoj.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2qmariusw.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2lhecwoxx.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2xfrnjbxq.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2yuzgbdki.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2hwgfrays.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2wmrzwpds.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2lhjrwpjc.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2amkiyjit.html


<!-- 参考信息 -->