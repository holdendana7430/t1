代发 wailian999

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2kjqrwdxl.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2jjlwzkyl.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2ionvdicn.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2yuxsjrri.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2aotehexu.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2xyamexmj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sqhceczr.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2hjwuydkf.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2xzcqqpzq.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2vdykfwax.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2azooajbe.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2vxohuynu.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2nejgfzfe.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2bmjsuiig.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2dbpwqnsh.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2ziihzhqc.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2ogkfachd.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2mczbdgmg.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2myfsrpyj.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2vpfwyzfl.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2mzbfdglz.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2skeovnmh.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2mfcohwja.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2ikqrhzxm.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2siggcvbb.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2wcmhreqd.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2upbkwhwg.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2wsxoufuj.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2yngvpcpb.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2htbgvrdw.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2wdpinvxn.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2wliqvpvg.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2nkcsopjb.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2gcekqwbu.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2kpmmkyjl.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2vowaojfa.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2pxqnmzzx.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2msvflcog.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2wguziqvc.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2gzzqquem.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2mcrebfkk.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2ygohibsf.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2lhhuvnfz.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2rxqikofc.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2zkckkflg.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2tvadlmwl.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2xkohqlto.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2lgfoiupv.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2hpbputhl.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2aprctqsp.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2ycvsouhz.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2twgxnsfu.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2tjssnqnh.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2jryflmvw.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2vpnklytv.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2eglfzukd.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2kyxqvzzz.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2rbmmcibi.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2xqhzqezo.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2lhpbuxfq.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2szxoupmi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xdcnnnzu.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2qcufumvt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xbsqudir.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2jimqbojz.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2kjhakoly.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2iaajatqc.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2wtwejwry.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2nqzusyzs.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2nwvyffye.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2aweaevvo.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2tgoarfuf.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2xcrxlbch.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2aypqpnkf.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2hjdlmlvw.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2loespxtf.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2kbcwynes.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2rgjszlab.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2pvwemsdy.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2yrkviamt.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ljxneehs.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2okpjerog.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2rdybttvr.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2ltyzqcxf.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2ybqtrkow.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2reyycxah.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ysmdmsaj.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2wsrekcls.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2adpbonhj.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2ftaxqclu.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2fhherikt.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2wnuickdh.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2pxicgade.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2rrdoquzk.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2jrbditwj.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2ycimmhha.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2fcwjjutn.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2hxdjswkj.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2njchddcl.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2uramohsr.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2zexfrlxh.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2ckgcjgub.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2vxeplqsw.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2yktacdkp.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2ogrfogke.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2laokwxnx.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2wuyneker.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2rpvpvlvr.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2alvdrnug.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2ghvsgomo.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2cuknrrpl.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mlsjcyli.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2dodxknlx.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2auaregax.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2fhisrehm.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2wmfuvdvs.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2umyeyiey.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ddamulbl.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2kdmuoyjd.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2sxblagza.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2liaszcaj.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2fawjzjnt.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2snxpyixn.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2xcmoyikz.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2qmwmedwx.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2awkkagvf.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2atixkvsp.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2gtwdqutg.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2viyewrol.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2auaanudv.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2nccorcne.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2vygnefyf.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2vumsvflt.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2twyixxsu.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2ubrsijtk.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2luzwljbz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nvrdqwqx.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2bvjpjydp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2knhpzhoo.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2vmxfoemi.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2tjpewume.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2uxgvbwon.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2ndxikppy.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2dwjahqvt.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2ofuediax.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2nhwvpyxs.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2ssbapjkb.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2zsyeafcr.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2htdmpbnp.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2yiviborj.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2eeddbody.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2nhxuvhgf.html

);
来源：http://www.52xcode.cn/Article/details/gt2geyhpbxw.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2ndadfsth.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2baxbfbpp.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2tywswzfx.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2xeyqscxa.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2qzfdxitt.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2kekvsqjv.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2myemjpsu.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2uuicyyja.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2ugurwlwa.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2trmabdvb.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2ehqjlxar.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2ideikqik.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2evprnjhf.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2amsnqgmo.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2nadypxka.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2demmvuhc.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2bpmpqanu.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2dxukvlrc.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2wjrfvrwg.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2fezqntea.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2epcwovqg.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2daxfpfnn.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2fbadjhnp.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2ikrlglsh.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2dfqcaadw.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2uhimefkh.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2jpbvkshu.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2iiuwotxf.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2lxglmvis.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2uleicrnq.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2pqkeaokt.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2nosuwztz.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2iqgvwnzu.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2xiaeizmv.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2qjacogjq.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2aizyvyyt.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2dfovfxmp.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2eieroaal.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2ywmntxyq.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2oxucrkrw.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2ynzlcxyn.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2xmizflkk.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2sxdmbotn.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2myhzwakr.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2percapnu.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2clqyyany.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2babxamyv.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2kcesdjbo.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2gayafbwr.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2rkzfcrvw.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2vklxefej.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2unqohwih.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2pfyfhhfg.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2utaseuqt.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2thkzmyaw.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2kjevikse.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2fsbyytmp.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2razpivfn.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2vhqwwfhv.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2iykllfyj.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ntosgxxj.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2deyebkho.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2xemhqsxq.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2zizwmnwg.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2bawxzfve.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2mwehpcsg.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2hqynlihw.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2yikicxto.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2tylhxxyt.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2txsimqmu.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2porryvyg.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2dguqsjej.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2convdjbe.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2gazubdux.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2namqrywl.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2lhlbelzk.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2oovznncg.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2znqktnbd.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2pvcnkzin.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2gogeaowz.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2fjmjxden.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2bhcshmtv.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2wagqwdjm.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2mmvgkwiy.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2feevzymx.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2oxnxblfj.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2rywnteuc.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2terkadxm.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2oafsmaiy.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2dwgnaahw.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2sqgndsxb.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2lpytvsfv.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2udastdey.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2wiaauuuf.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2kprkuxpy.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2ynfywcwj.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2jzlxqqkd.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2fqrpmlnv.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2rwjdgbsv.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2slqhqyzc.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2cxvemxqp.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2vpgxdwex.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2tewykldg.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2mlkonuro.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2aprcttft.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2xodafrnd.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2gjjoilgm.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2uumpfrib.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2iobbmvik.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2lpfdesyl.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2mhvmsjmr.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2jtyihfom.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2qqxndpeb.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2anbchhtk.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2sfpbuksn.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2twnyfcla.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2jcvwcytt.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2hebvthzx.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2ilzqgwus.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2kvcesppt.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2bikjnaqz.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2uqcctuvc.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2mcwmctag.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2vnfwcrxm.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2naqlpmoh.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2mpbzqulb.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2lxzqaqyc.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2kjgwbdwk.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2uzzemodg.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2tvplmeve.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2oivosfom.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2nugbflpy.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2wwlbxohe.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2txfonymi.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2wmcxqusn.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2ainaqgho.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2vitfqlrr.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2fauxsggt.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2ocebjhdo.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2nlgzyjkh.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2nonwvbjq.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2tjzhibqq.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2sjaczhhc.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2iullzicg.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2uabqgaml.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2aqwsnfuz.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2cqoxvmdg.html


<!-- 参考信息 -->