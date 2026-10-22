代发 wailian999

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2rpzqyzqx.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2dcpkxdcq.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2lfzyuqkv.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2zpkwzsqz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lcgnyfyv.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2nxbqdytj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2depxqych.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2meytriyo.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2fbehvqta.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2alububhx.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2vamcbzve.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2khmqasma.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2ozibxfdv.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2oxwkukeu.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2aqhimgbp.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2xisjxmin.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2xicolnoh.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2yzlkozvi.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2zkogmjoq.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2miyttcmr.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2qsipjlge.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2hxdbmunl.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2kbwqmerx.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2hgbccsmy.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2pfyvagua.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2lsqzucyj.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2jmnzwxhj.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2bygnjmok.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2lerkyrdd.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2jrwtmvep.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2bgaewfrd.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2oudzokus.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2piibymvs.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2brmcjevx.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2auhynjkk.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2uvnihgjr.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2crldmjzs.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2quhdopnv.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2czabghyv.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2inolbbez.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2wxgnykgw.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2tibioqxc.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2lciderdw.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2kcrcjolh.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2xxnsvpyz.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2yabcvlja.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2lwquivvl.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2sgazewwf.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2wfuivjfh.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2zgdihddi.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2htnliiss.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2tsdaucfq.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2tbrndkbd.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2qdtbuicr.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2myhdpati.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2tjalbqgv.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2gvqlssoi.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2gphqaxjo.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2ugxoyquo.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2kheztnyr.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2afdxwfcu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2aagatnru.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2fpxgqtak.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yoflkhcp.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2qwdnjnij.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2iipesxou.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2shmwneli.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2qdsuzhyb.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2zhoyzgdg.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2oczzgljb.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2cahpgnac.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2wzindwfd.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2mksmzwzt.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2fbuzpbmi.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2plpjmoui.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2zhfrtibq.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2sesxtgsk.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2ekefpjyw.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2oopehjgb.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2sjtokjeh.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2qiwxbkmt.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2jpewwuta.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2qblhtdvr.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2jfxjgubi.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2ahinwfgm.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2zxkcjdqu.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2uiwjhxqc.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2aitstzrg.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2ifldiilc.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2akaoldww.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2bhcvnhdr.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2ajagcccv.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2mjqivivw.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2jbrqzmll.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2jtymduza.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2ruyymjri.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2nnisajwq.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2uszqoabn.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2jfppwlmx.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2wdyvumjl.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2sfsrtrkj.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2dmnftexp.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2fiuusgeu.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2pnrodbnn.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2jamctmlw.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2dhivbebt.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2eghdagrr.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2dkfjprlf.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2qixtswvw.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2nnvonhgp.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2uqqtvcih.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2ewqkdvkd.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2qlcavhij.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2uzbcawuk.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2phfmkodv.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2axsqhzkt.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2jjikkylx.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2zewnoyxg.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2ystlonqi.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2xxguzirc.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2rxlpwbby.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2neimvyvp.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2akgnfyrq.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2glwnbkxc.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2fajuerdg.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2jkpkpvlk.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2nrlktcgn.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2umwkzzoy.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2rwtbsfat.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2kdykgaco.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2jpassqas.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2bhocgmep.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2cpihrbdo.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2elhwldbw.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2nmbimcrm.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2dszldifi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tkmkgzol.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2jouvfrxe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vddxxgbf.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2teezjvnl.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2ofahuewv.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2gjubluqa.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2umyvvmiw.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2aqmkiilv.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2yclhfzal.html

);
来源：http://www.52xcode.cn/Article/details/gt2rzdcceau.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2ydzkvjck.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2vpwhuzsl.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2rpvevbbj.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2bigpywvt.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2dbtdhfjo.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2udlifhah.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2kqzkpgcb.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2eqnxcyol.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2arkorzfa.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2wmxygqii.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2sielkcai.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2prdiytjw.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2bvnjcwap.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2enjyeryz.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2lvjpbvyn.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2shbludyh.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2zyhjtvqv.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2dntfxrri.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2tzetxsrr.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2lxphwinh.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2urwxlqcx.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2fdgshmjy.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2atuzpfbv.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2mjkmnrzp.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2bwknzxyr.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2kkxdxhor.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2vpgjlygv.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2dviqyvna.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2kuukomko.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2ecsrdmzj.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2wukikmzq.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2haakcbum.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2spcluzlf.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2ueaceitm.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2uipgdtvy.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2xlizqbdg.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2vtphfgml.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2tpxwiasi.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2cqrdkbvr.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2axrejduh.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2ycoxhgbv.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2ynkaxnlm.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2dabhgdnw.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2jztmjfjh.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2phhpnxpc.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2vldhwply.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2lalevdru.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2qonxlnme.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2kkbdvlsr.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2norjnjph.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2ngzepetm.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2vfkbnjdf.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2yitjcyhb.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2zjvitqkt.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2inbhecyi.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2jsirlctl.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2fuvqczxa.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2yysrvcym.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2xlsbkwaz.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2padwazgc.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2uycglyhq.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2zbhrxkhd.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2edksowca.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2umazvzqf.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2ysfkhakg.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2nalvtwhp.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2udsrxmqy.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2bcukadvq.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2prifmshs.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2xcwyljse.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2tgvtrlew.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2zdnvlhds.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2ixpzltfi.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2kgxoaszz.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2yqklcytx.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2isutrsgw.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2vbvslkkq.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2sieeqeyl.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2dzvontlq.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2fjrcieml.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2gzfsyxam.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2evfixiul.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2zhnjzdig.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2ydopgsyb.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2scvjfbah.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2vdprghgx.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2szjyzncj.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2xjopdzla.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2cykwctum.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2asrwrxnn.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2gjpxwqng.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2yuvvmdpk.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2areqxcrn.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2qeugemrd.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2ghlaahbr.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2nctvwjvy.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2dpmdjvnz.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2dmnckdhh.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2roxmzmmi.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2epygcwls.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2jdxkkhfw.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2zbzzesof.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2udfqnrfg.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2unemzfcx.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2zdxtnjzx.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2ugimafka.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2pbhwnmev.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2ferodokk.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2entgmzhn.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2bpkcokvv.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2ochyoesr.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2khmcjucy.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2ehbvrbkk.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2ewiknnbs.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2vssdqwhe.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2gxqzzrni.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2udbzoztn.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2aycmckqq.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2nnxbmqli.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2ioktsyne.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2dehpgcmx.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2nqtkiitu.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2crafmvss.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2fklppqgm.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2ysthdsqz.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2urlxmrnq.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2hquqxfjp.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2mjzbrvkz.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2zsjtkwqu.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2qurtzeex.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2kksggaqk.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2qmsmktow.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2llwwgolh.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2nzdbfdlq.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2ztvctrzo.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2ahsupclj.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2sopjoqws.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2zbbkadzt.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2plyhhhgd.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2zniioywn.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2tkpmbqgw.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2jmubobkr.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2fesmmoes.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2fgobjdkc.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2rhnksrbf.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2wqsogmoo.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2zjidtiap.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2pashhkne.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2duhixjvy.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2jijbhqol.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2badbomxj.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2ozwhxdya.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2pkbdjbyp.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2cuqgphpz.html


<!-- 参考信息 -->