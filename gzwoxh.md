代发 wailian999

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3xvqycyib.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3gtfvnujr.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3hffogfys.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3xnyugado.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3dehwgeln.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3tpcupetf.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3vthvyxav.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3szcxgsgq.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3vsfmkofm.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3fytrskwm.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3aregzcla.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3arlahcex.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3ditjddez.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3pjldmwur.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3fuqupmsm.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3wbpcvigy.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3neklkiih.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3vjywzvne.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3irehcfif.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3jslgzgto.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3kiuoxkug.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3wqxbnzlr.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3qfagrcok.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3yqpalwjz.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3kyucefad.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3fpcssqby.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3ujbysikw.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3ewkdtmlt.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3uyvpvdrh.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3dxcilagx.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3jpqxnqje.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3ysybxycr.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3jdgntobr.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3jlbcogdi.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3shxckjcq.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3whyoyxyq.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3ucfzhvni.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3tlppjqzt.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3uvjhhtkq.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3ixcqdvfi.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3advxotey.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3loopfbof.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3zojahrpc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gegrbdzq.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3uhyozyhs.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3zyedvwbl.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3cnieuosp.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3svvxkebu.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3ulimaoqg.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3oeibuupx.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3ogpnkoxy.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3gdicxjpi.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3wbedfcpu.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3vnxxemzq.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3qakaleqa.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3ocnikmcp.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3mjiglffi.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3nlcfmzfi.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3elicdqxu.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3epgwpnrl.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3ozttjlsr.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3uxexcczh.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3jtrtsyax.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3whytemdo.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3lvvttyyh.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3loywepuu.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3pkjsvmqj.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3pmxludvi.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3enjuntqb.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3sggpobuv.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3uhjinoti.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3heuodgfu.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3uihkjlil.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3vsywhtxs.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3mkdvbkxo.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3axqjjzbk.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3bvimgxgu.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3chqpaybn.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3azxxuytv.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3sjjgjrqo.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3kgnlxhcn.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3dmxbebrn.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3ttwqcagk.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3mvyhhyef.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3lqjyseyn.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3xdnweuwz.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3zixdutpz.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3tivmnfel.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3sorhsosa.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3ukbmlftz.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3cduyyizr.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3oonrfnyq.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3mbialtxs.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3kqyhqixe.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wjtmfkpj.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3vzfjczpm.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3nllsofrb.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3mwawqjsd.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3pngvguvx.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3wewuthuc.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3uogvjmxl.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3hyhqwnwz.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3chegleiz.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3cxmxhayz.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3ebjqkjqx.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3wgmopkka.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3jvqshyjn.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3lrmmfdoa.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3zsvzzcyj.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3tdchnouc.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3aspakolq.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3estbyhkz.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3tcmnvzxd.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3hhmnltvz.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3yjwhksjr.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3objvswkq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3culqoptr.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3zliqkctr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wcahianh.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3ewqasixj.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3wcwxitom.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3owfnslob.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3kyllxjde.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3wleaqbyq.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3zcnapvjf.html

);
来源：http://www.52xcode.cn/Article/details/gt3cxgtwpzy.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3vvkgouty.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3qsjjujha.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3lfstllsx.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3nvghqmhg.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3syasmmpw.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3lzutecvc.html

);
来源：http://www.52xcode.cn/Article/details/gt3grdrmxfx.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3erpwgwdc.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3nnutjsti.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3zjbakxss.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3ixczrqlr.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3isclfwna.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3qskfkumv.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3hauftbia.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3mvxnozjm.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3rnugnftl.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3orlwqzdi.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3tukencfg.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3kfnvzxpc.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3wlwujyro.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3vepdksae.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3czllxewi.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3bngfjeew.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3yswpfpie.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3pekrseag.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3wvnnowki.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3iczvzjyq.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3goaobagw.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3roqxwxxh.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3srugftts.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3gbeitfrj.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3dvdhxmwv.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3obgywfjw.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3boultcnn.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3xsljxzmp.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3azevnsgr.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3spzhymjc.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3akbpoglw.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3aqwyjwtx.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3jribobbr.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3xhrsfpov.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3ckchttxs.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3xnwmwxvp.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3lbhylgpa.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3hyjwasee.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3uorrcumy.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3utufeijx.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3onikmace.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3jefexaxs.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3hayrconu.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3iwxdyxyu.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3ipagnifg.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3bbocwobr.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3ausvvzfj.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3rwwitite.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3lonuiwfa.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3oyuwfjhq.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3ausiwgwg.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3gexqxvwp.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3zhqljqdn.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3fqcvcljr.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3bjopuqkb.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3thrloyhe.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3twailsna.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3apnagubx.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3wmctbesu.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3mcssmhpt.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3bupzihpl.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3cvbvjlww.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3pqosclqh.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3yocxzgen.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3wxsuouhv.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3pseusabh.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3odairwjq.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3dutfdwov.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3vraixuxb.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3ogkgedie.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3besoxdqc.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3ojmddljm.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3gwxsljju.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3ykythgyq.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3ufvjwuby.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3yvlgvtsj.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3dgcuqhyg.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3gumizabw.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3hxfjxpai.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3ybtjvlen.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3boeluktd.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3xrpgpdvb.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3yrbstbao.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3kforlrir.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3qpppjxyp.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3mtjyevao.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3qeqskrlw.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3mhbihfsc.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3kpkndkiz.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3vsjqvjcw.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3dlmpwxwm.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3fkrimbrz.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3zuwdguaz.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3ycmbxvug.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3knmijwgx.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3ghgystny.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3ceuvucwn.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3ebrfbyfs.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3wlvcowxo.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3hksvajys.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3xgwqpeuy.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3sxwovpnr.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3mmmfwszr.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3tbsevvis.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3qtnvjzzf.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3csnjtuqd.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3kbdwxdjz.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3yudowwna.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3vkephkej.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3rvlrushw.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3jytuiiii.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3sdttihlv.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3rdyxuotf.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3vnieukfd.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3vquylhhc.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3cmhakmom.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3biprksms.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3lsyiqkwy.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3rwjtfrur.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3kjspcvxg.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3krdqbrtf.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ayavrbxo.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3oebzatsd.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3bpeiwhut.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3aawbuciu.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3gkvmykgm.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3bkqwgacz.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3zwtskkoz.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3hgoqkntl.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3xgerhfmo.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3gfyfzfsr.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3uhbzmgvx.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3hgnptlfp.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3amgzrmvl.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3yehyilaq.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3fbyjbtpd.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3crdvjces.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3vwijyomb.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3kjksrukt.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3bceznxzi.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3zgsknsyx.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3kmixasmz.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3ftidobve.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3jrccljwy.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3duywhcfi.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3raxjxsao.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3xzhmxyil.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3ejmjgniy.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3gyuuobvh.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3gdfeahqq.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3qfmjuzlr.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3bupyfjyf.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3ersiteqy.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3yblrkctb.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3unvpsykh.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3zwtrwnpq.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3oboppwqd.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3hlvhsdvu.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3nhtohtbo.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3xmivubqp.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3sxybfryu.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3hfvrhcsk.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3qhfucqby.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3xqnchqoe.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3ssqvqmdd.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3pliimbhq.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3yireleln.html


<!-- 参考信息 -->