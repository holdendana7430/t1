代发 wailian999

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2pbugjbpw.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2nwvbyttb.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2xyrugomp.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2yxnfkjxm.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2fselekjj.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2piakiwhp.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2jyooiwlk.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2jkileuya.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2wsrkwiui.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2ksaujkmh.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2zrffhvir.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2hjwtkwgg.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2hhtccszg.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2vikqrltq.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2tbnelilq.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2rvlnebot.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2cstdmlty.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2mwzrfkyn.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2vieepxcu.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2lbahkbuo.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2slkxlbfu.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2mwntbpxz.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2gpkdzndu.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2hlebhijz.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2vgphjwkx.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2mnyxtxpx.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2xergkwfv.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2jnibkkkk.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2tzosaxdj.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2uyiatgka.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2kfuucmmj.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2vwibrclg.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2uqhegitz.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2jcbzavxz.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2olnbofmo.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2lxgjprrl.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2mslhkibt.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2kozsbeiy.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2clqmoujj.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2nbwtrptv.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2rqpneloj.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2mpmdyufz.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2jgijvvrv.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2bznclxtx.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2cwnlfcak.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2kzriqnop.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2sjqecfww.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2kxuwoliy.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2vrnqgghf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2veocwhxo.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2uukjxfgw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ebtigmeh.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2iiezuygz.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2zrgtvxsu.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2avlcxwqn.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2ukyujoqj.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2ouwjoisc.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2ixqkwxdr.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2zkuawdkc.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2llgtdjgn.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2hjkqldgw.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2edsdvxjg.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2lbuorcws.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2thfhvqty.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2sfopoucl.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2grrorvnw.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2tflhzfsp.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2bqcqbokz.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2gyyxgmga.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2yholcyvh.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2eurzwwkg.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2frirddyf.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2ydztbryg.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2vksnyjra.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2zklhjwwp.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2psfdfcwx.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2mmnyvttd.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2zfdvfivq.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2fdcolknb.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2bwtqgxku.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2hedllaer.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2pdxssrlp.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2wilkfqwy.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2ymrcfmzi.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2rhxtarqq.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2wnkhtbtd.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2lmdegnnh.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2vzwvbdul.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2nfnznnvv.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2mwjgaxnw.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2rfawnmrw.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2todbntvq.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2rbqlsejx.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2ftoaimhe.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2ufwqpwek.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2tgmitpie.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2nslusjai.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2mmxykdrh.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2tryljtae.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2azcuquej.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2fvvszoxz.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2wlwrwrmx.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2tordhrzj.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2bzioayik.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2zbkmjlit.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2redsrmle.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2iptuwybk.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2boarxdtl.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2qkzamiwg.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2adtprnpk.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2xpxahqro.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2pdcbouww.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2loiaqeav.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2sacqwahc.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2aqdhkhfn.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2tchucdtb.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2lgwjkrwz.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2yfsdpekz.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2egpgkqzq.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2hlaxbmqw.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2vbzgoaeb.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2yfwfeutl.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2elspxmvj.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2fjscoibc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uacjaick.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2iupmsoah.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zckdgqxo.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2hjtoypaq.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2pdcntqtb.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2dpjfaelo.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2ekcoudyt.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2xvdjncqn.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2dyvmrxez.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2vcyqevvm.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2buvlifaf.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2hiruwgls.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2olaafkwf.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2nroagnub.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2dbmfhhbo.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2dzevpdus.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2utbxhayn.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2lhqdwbhu.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2dnxahkyp.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2elzfdhir.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2eyctleri.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2duxsfine.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2dblaxrte.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2vfnkdvpk.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2qoflpint.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2tinhsovp.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2nlsrqwou.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2agbsivko.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2iwwivvrj.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2hnuujvmg.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2umxblmff.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2aeihvyfr.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2rcjoqqsw.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2jtjovtli.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2yvywgiaj.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2dahtmzkt.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2ejdaeznt.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2wdjlauzj.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2wnfwtpqw.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2dteuqsow.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2npwtwubf.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2anlseeku.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2xzaopiir.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2fennchbx.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ycooluov.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2xklivpve.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2mcqjqvoz.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2eugekfot.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2mbayuiaz.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2onegnzpg.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2ueohgurj.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2aszqqohf.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2hbegcjii.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2topwogwp.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2jhkawrnn.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2fsolmjjs.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2gmwagojm.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2snixbqnt.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2lmnpfkmk.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2uuuqkszx.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2cchzkvnt.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2zkzzalel.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2raygntzx.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2tdebcjyl.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2drlxyjgz.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2hrtpqfrm.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2tnxonyut.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2udclriqm.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2hujlxtlo.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2ighpaxok.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2lxytpdry.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2yjcnungn.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2hwscfczr.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2mkafygra.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2fubblocp.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2yzkwspxb.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2rmqzpfkq.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2erkwgxrz.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2tqpphbtd.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2bgjfsoxn.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2lezlfqbb.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2qfrvwkdg.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2ufqehyvh.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2kzoatgsq.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2xheyhvuz.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2jnwogmlh.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2uuzfwnnd.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2kfmbijct.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2ojedfkti.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2xjcgciii.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2zbaqttvn.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2pjjboyit.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2ebvrufro.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2fuuzhvpd.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2czakuqzx.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2uwafegej.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2nowqvuaz.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2cfqrkfrr.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2jqgfxxbq.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2dwnjawen.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2bgdwmsrn.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2aummwhtf.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2ufeejkrf.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2nidtjvly.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2nncduveb.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2bodfqelm.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2ycmdwluf.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2pqwmxbpz.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2vdvrqsri.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2euvbrzzt.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2gttdpysd.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2qtgsytqh.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2gpjwyvdk.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2jvdktask.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2ctycpvei.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2yrbatusr.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2ieuzqcey.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2zccpmwgr.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2hvqdehdc.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2viuxujsw.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2ikxjqsay.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2ztsknhah.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2louqhqzv.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2foicxzrj.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ofikboei.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2oufzoggp.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2qlfdnqgf.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2fcbbildz.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2boinvsrd.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2ftmxvthe.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2ybkgvmmh.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2hnaztsrj.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2dcripopo.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2kdgnhlax.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2cfexvkoy.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2feseniaz.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2sdvhtkfg.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2ggihlvkt.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2laezrxea.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2asvpurcr.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2bfjdqtma.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2kswqqyhc.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2cjodzkvl.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2dczrfbar.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2qlnmrgmg.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2gazrainw.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2vchsueck.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2kmgszbwl.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2wwoyldou.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2jhuudjvv.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2mqliygll.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2jefjcznk.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2yxxfntmo.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2ycokrkcq.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2rpaqoanz.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2wskmagmh.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2dxkgxwin.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2plgncmrr.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2jgabcjfn.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2kizedjml.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2ngetkvxc.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2tusbciiv.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2aikyxdky.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2azcuxbhc.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2ffocdbxd.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2cndkifmc.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2bceufoay.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2pelqbfpu.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2dcwsnvkq.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2xhgfktez.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2bssuufdj.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2dlmqdpbk.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2gjnkvpzj.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2modqbugq.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2vocjcack.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2sedxbnbk.html


<!-- 参考信息 -->