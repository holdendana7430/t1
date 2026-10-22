代发 wailian999

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2legikbww.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2bmznokao.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2ukttlxvd.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2fiiqjnrj.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2mwasarfo.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2fedlerir.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2etiytmqx.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2zrpqjhwa.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2cxvxaeuq.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2lputbvlr.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2rsgqbgsc.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2qfjkwlsi.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2gurvrrio.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2robxtrmv.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2rqbjxkiy.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2ypllxfby.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2vgknhstw.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2vwolmbrz.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2dmiqemok.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2yupooobl.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2quspkech.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ydczksnm.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2fvxgrevm.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2wigllilm.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2fpxahupg.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2kqlkhmot.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2qrqohkmu.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2apbwoazh.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2syucjjjh.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2fjadqpxu.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2eiozswob.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2oyqhzdhu.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2zcmdmhfg.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2tovyzopb.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2ycvjazlf.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2tteiguyu.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2xstmvkok.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2kvviveql.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2gvotomyq.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2vkcnevlm.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2kyfvaktr.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2ynimntgo.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2owjjucjx.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2vsqteusg.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2ymuphfkg.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2itjdpiku.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2trxnrpno.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2jiuvinlg.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2tzlblarc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qkilnaxr.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2zgiuaqyl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vlrpxqra.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2heipcurn.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2eojyufjl.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2vbigqwzf.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2hgcuwnyf.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2nmmqmcdz.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2vgynlebg.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2bqlkuxea.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2ndqlboow.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2ecmfzluj.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2yvkcbcyp.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2kxamuksv.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2jsclzixd.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2mnnrjvcr.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2njvqqxef.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2wgiyjdqa.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2uwpezmli.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2rouzloxv.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2nlxbvfrf.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2afftvtjl.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2euwipryh.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2bofhdcgh.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2sklugyts.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2ytynmwnc.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2mciepnzh.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2lfoowupb.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2vmtflqua.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2iurolvdd.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2syzdadpa.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2tqouorlh.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2hwobafkf.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2wnxzijku.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2pyhymkrb.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2hguzscbg.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2tsjlkngu.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2enpoosjf.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2yazqroxv.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2qwlirdjz.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2fcdorvum.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2yhpvujrn.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2stomcgvt.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2ecikdozj.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2pqzxdnlf.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2nbziheet.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2uanrgrsv.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2lgwgusdo.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2vwcadrea.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2fhgfyicp.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2achgvolv.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2hhdjlueq.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2vvnfmhiu.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2chambktq.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2ifhadcjb.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2zmyydngr.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2kcxvunwe.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2fvchoyww.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2gohzzwno.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2maiisgjb.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2noxxqtlv.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2fsrnwmii.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2jjtvzieh.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2omsgugmk.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2zipxegpm.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2tfkklphw.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2qrkdbuph.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2jquenpto.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2aemhnjqu.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2jxomraew.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2oqcqjibe.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2rlmacvhh.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2tapmavgc.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2lgnmnohi.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2tfosnlix.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uqkoxixd.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2vqktlpio.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ibsuqpdp.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2debqpjzu.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2qvpwnkai.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2xquzhqpg.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2qpnnowqu.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2ivodkhmq.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2nyyevgjr.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2lpowipke.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2rctyocjv.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2udswbkhv.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2spmbkahw.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2jdprcqrs.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2cvvhcimc.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2dgkvwvuf.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2ctlhohjd.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2odjwkwph.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2vecjgvfj.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2cfmwsckx.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2wqylugqj.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2gxzhxdrk.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2agpqoihn.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2hjbwihdg.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2xwjawrlh.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2ckbfmyez.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ajimbhqv.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2jhcsikci.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2dgywgoxw.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2cldjiwat.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2guvuiyrw.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2qiakzztb.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2zxhxoszh.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2ubhmwuuv.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2axmiccsz.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2iwltdrko.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2klokijun.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2xwbotlpe.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2ghifzivb.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2frpzznzy.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2ompxogvu.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2oejledkp.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2gnvrjker.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2tkyxtiry.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2tpjpkqyp.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2kejgkiqq.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2yamitvol.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2wxzskcej.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2wroegjwt.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2mqfpyemw.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2otkikfxv.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2acbtivda.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2jrveykdt.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2cjgcofjv.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ygarfebf.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2yjticbgi.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2zphuubpb.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2msspffto.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2ceptbsei.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2qatherfy.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2bhzvtamy.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2lsjebjax.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2duwyurkd.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2dfhjtdjw.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2fxxmdtln.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2hxyfefnh.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2cgwbyuxq.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2tfzancty.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2qiqmxmpu.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2gawcsdhv.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2gsqbkawx.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2dduqzocu.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2wvkerpbw.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2yxrwrlsn.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2muuivrll.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2irhyufam.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2pqualfdz.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2waliawzr.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2kvpqbuch.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2kuiqesti.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2kerkrssw.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2zdzwsctn.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2dexlvjyx.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2afbtqrsc.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2otoismui.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2foignict.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2ytgllsym.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2yjohsggh.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2bjuuxwpz.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2uitnxuch.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2zxjwixkx.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2pdrchefu.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2ueeffloh.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2wczfqoww.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2cafprzgk.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2olpufsuw.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2mewgewvr.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2nhoqcsnd.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2dtsdglmx.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2vulyreqa.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2yqwzagaz.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2helfmzjw.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2chtfnwij.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2zebnukmg.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2xkcburgt.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2dibdicum.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2tokwrcwg.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2ljatkoyw.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2dqaekrgg.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2hteenznv.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2yrumunnl.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2ypzedsnv.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2kmehrlss.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2rhrrosse.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2joowhpar.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2ldcbgzeb.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2lcjdjivk.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2ijkmmprl.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2twronmge.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2hrmeowry.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2naaqptzs.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2fvzhigoy.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2esmgqmiw.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2bbuvlget.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2libvbdrv.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2blskixki.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2hmjkiymx.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2tadiqvhb.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2qjjrfgye.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2fftsellb.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2ydbvuyum.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2hoxvzibm.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2fyrjhmrp.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2vllztmjq.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2lvekqziy.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2pjufrwie.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2zdbhlngy.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2ubucjgdt.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2xpwqrayk.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2egtvrdrn.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2zojbflyw.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2evsvrnxu.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2ddjzideq.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2zrhedszr.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2fkvhbivx.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2bjbyoqqp.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2vrjfqlyg.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2uhknluul.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2mmuofozk.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2jmqyzykj.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2rtzoasjw.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2ckmylluj.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2plrnowar.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2wixpksdr.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2zlsmnpti.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2mpftcyhs.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2qdbmdkub.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2ekwsvibd.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2yyixiahk.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2lwzkndww.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2tnblpsaf.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2gvnfoyxn.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2oqiyyqdp.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2vobynujx.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2simwvomt.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2eqddntzm.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2tqzpvgnz.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2ynggnssn.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2qgmrrneb.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2udpfvetq.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2wbbyetuy.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2weqnsrkw.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2wmqlmjiy.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2janpwfdm.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2awwzzrvu.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2eoqdbicg.html


<!-- 参考信息 -->