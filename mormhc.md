代发 wailian999

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3lagfqbnt.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3osmnqruw.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3twraitmn.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3mjkcjhod.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3onzjvmcs.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3tgbdvkea.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3oxxchdcy.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3vkongsos.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3wubqbagy.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3eyxsgjef.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3ptarbewz.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3koacykhw.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3mizejdlb.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3bmigzadl.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3jvnzdkck.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3qpfynupy.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3gaiatfwf.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3lxueytmh.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3zcfibtjh.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3jbwsyxit.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3qygrhsvw.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3ziwkfwsj.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3fknewlse.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3mmeygdik.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3vzhwyfap.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3cltjzkdm.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3bxohkleo.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3baurgyxa.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3jjunhrqf.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3qwfhqgtm.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3kjzablwv.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3wcbguyzn.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3xcrwojan.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3jtqfythy.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3ffovambt.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3oovpbqwb.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3lldwepvw.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3chzmxzsv.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3pinuxjdf.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3jkwgyuzo.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3uybgdfqp.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3rbgnymhd.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3yfayuvms.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3ekhkjtfz.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3jqowrqtj.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3ytmwgoay.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3hdpnwmao.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3nrlewpvl.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3trccshyg.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3fzvkhitu.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3enuvwzqu.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3wrkmkikl.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3jhjjspad.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3euwgdpvb.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3buwagluq.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3gmxcqslp.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3ikzdhdfj.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3sqvtptch.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3jgztwsis.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3vezatcwf.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3snatpvts.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gjvhzfdh.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3gxwfbjdz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sdkbfexg.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3tzrqrncw.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3wbvcbkxe.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3omzsleme.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3twtzbpyj.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3hquprqgm.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3mdfgqrjj.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3ciaqidrq.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3cldicdos.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3dijbuzih.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3fehpzdhu.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3mrqxfscj.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3qaqaipbj.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3hwsueyqn.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3ffarhzhq.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3wzhwfwjm.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3rwuaajgv.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3lxryrsgn.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3kptvvmmy.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3hylejaal.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3wxlxanom.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3cymazxna.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3mtqulsnj.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3tzjaihkl.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3offdhnxw.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3xftpdhtj.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3hbzdhjvt.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3eoccfqcd.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3pknlzdsc.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3bvfikeht.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3cmsceyul.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3buocbmwk.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3fhxuwdxv.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3dmxwmbcx.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3bflqvbak.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3uskkuzfz.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3tjsfqkub.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3gvzxwfrb.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3drvqluol.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3isrqosfv.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3kxhmnadf.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3msqdztbg.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3eblmoenz.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3ermucuaj.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3ewewqzfj.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3wnfyzhcy.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3xlzukflz.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3knpzzqaz.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3qpfshest.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3buozmtca.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mydygzjg.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3knyoarps.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3xpdvtfdy.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3fydzbbxz.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3otndtatc.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3mermyvqw.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3fmkhshfh.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3blhwbrye.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3dutawnyr.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3oajdtcrl.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3maznfwaj.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3dqgtsnzh.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3pkeklzda.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3dulsddkj.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3ecqescxj.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3sywbglpg.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3hehphkwq.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3ksybrdjl.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3iugoijad.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3wpwyxtxm.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3mjlhvjie.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3twofgucd.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3wwewswoi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sszmshgp.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3blnuqman.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xwayfwmp.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3hkbjqljn.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3czikftes.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3gnmgtuks.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3eqgxaico.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3lcglcsnf.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3mdhyozzs.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3uujaueei.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3cgkvmhpz.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3taviwstf.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3jctzkleb.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3oxspcpmj.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3zosyuzwb.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3wkpqlnbk.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3ankxotga.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3ugvjqstk.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3ghiapetz.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3sfkmchlk.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3usnvhsab.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3wzoxpdff.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3temjqtbr.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3rmauwvwf.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3iwbmwjvn.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3wkggpmyt.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3tinbymqj.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3aymfxepq.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3gocezauy.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3ifhkbgrt.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3uvhwvyux.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3jojtaoav.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3ifviwlkz.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3jblvlgpq.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3ymlhpshc.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3qtarawyw.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3hcsqfssm.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3kgpawkis.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3hbgnmgjt.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3rjjbzxwz.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3wmuhwizs.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3uzcwllif.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3yibmztai.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3qgiiwtfq.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3nnsquufi.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3goqccftu.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3uzuiapad.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3kurycjjy.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3glclkkir.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3sypyfpsc.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3anarwisy.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3gppvadyw.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3jzcvkzid.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3quzimbxz.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3tmddsqyg.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3sdkozglb.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3jzuygozm.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3vqosgldt.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3sumskmhn.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3jjhsqrkq.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3olfljivo.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3idlclwsp.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ojcbxexy.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3xhsrpqae.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3aansijim.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3wmnqfxkp.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3tklidffe.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3esrsuqdz.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3hcydkpcr.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3jcbhqxxc.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3khrmdjvc.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3xdcrisxn.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3gozmfzwy.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3wwfanszy.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3uliziscm.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3qmindbzn.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3bukwwhyj.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3emrrttau.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3xyxiqbyb.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3uqcwymtw.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3evthuqba.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3kbfmgapf.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3kgqmufrp.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3wbkkkzji.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3qiwnacnb.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3uveqsppr.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3pxyjmcga.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3jaxkjzxg.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3vbcpmmeb.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3biekohyh.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3vwfdplrl.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3uvwuepmp.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3bldkfvqb.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3gtfwnemm.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3jdjbptfo.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3qutckmzn.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3wmuedbqv.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3bzqmohdx.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3itohipht.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3ptssaffy.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3drigqczn.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3umepljjw.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3zqqbhbpb.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3relibssq.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3vxnivkya.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3zymcdfnd.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3temeucza.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3zyluoool.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3pxpllnew.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3rcstzycw.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3tfebgtah.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3sljilqcg.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3ptslfdvr.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3eqjutjjp.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3zqfiwefb.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3txtilgkl.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3cepbecpu.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3ktiqficx.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3dimhddcz.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3bwowdxts.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3gzxrdmbv.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3geweptib.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3wjqzzfhf.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3swtrobfw.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3ohzyifgk.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3njvjcmrt.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3zvtaowbk.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3yqyuscph.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3zrqnuask.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3iejiwjrt.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3waaozzbp.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3zczeosun.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3odlkdeqw.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3addozlpj.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3nkjfhiks.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3nqqfeutf.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3zeahkeqb.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3ufgfienu.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3tqaaylll.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3ryjvsxha.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3wvbczouw.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3sttrdxxb.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3zuhimbef.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3nhaajktk.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3ueyfknan.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3hccgwfas.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3xhkezmyq.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3wfocdzev.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3kiqyuoxr.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3gpzdubbs.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3zthezxpy.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3tgueektz.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3nhixpmit.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3yfyecqco.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3mpexgvbu.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3xnrdbpwt.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3ccupvohe.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3wxalcnhr.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3xulibqpv.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3vyxapqgu.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3ihshkhxp.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3nmujyjkc.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3orfuqrbz.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3mnzbpdaw.html


<!-- 参考信息 -->