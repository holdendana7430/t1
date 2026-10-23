代发 wailian999

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cwzfmjed.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3oxjqdefg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yevkgxwa.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3tromtloj.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3gnvptvtb.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3tlofmmrc.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3hxxwymbx.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3bbbeoxbm.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3fhesajcd.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3hhvwzbha.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3jsieapja.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3ammafify.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3vdicnfnr.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3ddvymbhw.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3sloefmsy.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3jhsojdvm.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3acaxoofa.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3jeupuzgu.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3ngczmghh.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3lzozkxsb.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3hlanouhr.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3gskehtxn.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3mrylzvur.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3jnmfnkvl.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3atnivrte.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3qvxwseqz.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3ledojlkk.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3kugeyapm.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3pplmbjea.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3drhlayqw.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3kafuegxl.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3zkofiiki.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3owwjxpqq.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3uloshhmo.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3bgendzhs.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3bkexqyxm.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3dvmftzai.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3dfxmspkc.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3ywydutvh.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3etyowvex.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3qiriiiyv.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3oslnppnf.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3cmdmcahm.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3leuezwdu.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3gprmcsvf.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3ncyudkoi.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3tyqcuijd.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3onuxzlcx.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3qcegsjmw.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3vmxdxobz.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3zkgdddue.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3juerqsqt.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3fxwfolkf.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3yywarygy.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3hwwhieyi.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3uqjynrzq.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3tjejmhzt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zxqtpwvc.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3wluxgvfc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tjhwggog.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3iyohshka.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3ypwcjqzn.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3vfdgbxaq.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3fxrhwfuj.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3welzdhgz.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3udyomyoe.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3dcupwmeq.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3vlpvgryf.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3oacyycpa.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3yebtiicl.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3hfygfkiq.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3mrbycjff.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3hctdwdbt.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3ypgpnyxn.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3kqfbdvka.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3rynwuxev.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3iyfshgmf.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3ivmsvqem.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3rhlmehfs.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3vfvfjugm.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3wwvwdmeu.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3prztafhc.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3itvetomn.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3ueecfqaw.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3mrfguaav.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3dzexhgwm.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3nccwfsbf.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3vamuesrf.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3soqxwzkp.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3ddkeejlr.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3dgsxceok.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3hyicmpap.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3taxrvtnm.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3nesgthux.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3ydwhqyjr.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3wqqmzbes.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3qovolxzu.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3yomsyspc.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3cdcbwyht.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3ulmustpi.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3mcobcvis.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3zciziioz.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3absoliok.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3tzrapnqd.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3yrzqvxgv.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3yggihzyi.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3uncstvcy.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bnxgjgte.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3mvrkegau.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3icvpfnqw.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3orkylohb.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3gfuofzjh.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3qcpxsakj.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vegshzpl.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3rriohxwp.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3djpweoef.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3wcvvidtn.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3ufmzhent.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3ivacnnnq.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3qlmkiuty.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3xtigubsi.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3cyspmtac.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3zqwtripm.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3fwvtfyog.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3grjkimhk.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ceogkdnp.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3lyhuigpn.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3bcbrectg.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3xcdamatp.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3jlqwdxpk.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3bajnxefb.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3ftankxpg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gqtilstx.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3dztyvcnr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wcriqooz.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3dxuvjlzm.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3lpycoecf.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3nfvfykzt.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3blqiajya.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3onwwlnaj.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3tmmplnsf.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3vuobwbwl.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3uftlqlgd.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3ursiqhdc.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3icmwveba.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3vpvhgyfu.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3cxckgzax.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3rctzkfje.html

);
来源：http://www.52xcode.cn/Article/details/gt3amxpommc.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3sqhrpbql.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3flrcoujj.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3appdrwbv.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3ubfszylb.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3byjrbqdm.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3ptrfsnyf.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3zeuvovtp.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3vsbbzvkh.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3hylibnpm.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3asrgtrcf.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3fkponeey.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3bqxfxcne.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3boulhexk.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3mibrjqhf.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3ufqknscc.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3rvzdvbol.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3jzevgwwh.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3oxlfwrbt.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3bohtocug.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3bereibwn.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3wkbdovus.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3pjjntapi.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3copwplof.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3xevwofrg.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3zjvtftco.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3eyeflcof.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3zqmmdmdq.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3aguxjsmr.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3szrzzere.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3powyubxj.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3acslixnb.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3bncpoirl.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3rvqcezij.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3rhuczetw.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3rqputphb.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3uxkqduis.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3paposdzw.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3oizcttsd.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3yslerelc.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3vweyhrkf.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3mjlwzwdy.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3qtynqbjw.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3vzussuvh.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3kbyqqcaa.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3ebhzgcro.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3jsebyqin.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3ommuvubn.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3svskpqsb.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3uvgrehzl.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3lxbsvuqy.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3ajwdfzyf.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3qovvirsw.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3fkwbrpyq.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3xkjarrmy.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3wpyfkwlo.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3aixclrmf.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3lhmjkfub.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3hmdwzmoq.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3dwtenxtr.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3rjqrtoys.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3rrfpoqod.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3feypjnsn.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3ywowoplr.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3lncjzgtm.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3pllbbxec.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3ypyfdtbt.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3ftnfqasl.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3iqiqirdy.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3srnfkkqt.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3avpgajev.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3oftidqjw.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3xbpfqoyi.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3uklladtj.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3ftrzcadg.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3mrtjvcdh.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3fcqejmqx.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3liwcvxys.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3hpvzjlkb.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3mqkeykgi.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3oarvztjp.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3cihgmepb.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3uupilhys.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3abxmpnzz.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3rmjugrio.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3jufblpys.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3hpaycedi.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3vqtygvlp.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3esdgtsuj.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3jogmwxbm.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3zzpmowzi.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3ffwurnwy.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3vzwabkgc.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3wkpkgjan.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3gcdzmqgr.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3zutuutxd.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3iucfqiic.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3dvowubkz.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3znircqlk.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3kkadejjq.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3uvqfqalx.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3juzhsacb.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3cnffynnx.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3bniqamlp.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3frjebqwe.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3nkbevkmp.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3fymjzlyl.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3hkgklrum.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3vaafavgg.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3mldzioxh.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3kevdnxnr.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3zszevnuo.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3rlyraosh.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3cdjpywud.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3hgeohkdh.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3nsnjzznu.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3fqtcrsxy.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3tfgwqjzx.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3etyntidx.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3bqqfjdsp.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ebzosjun.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3cscqbnlw.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3lceztcvc.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3mpwckwco.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3ybsifgpi.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3lqrvlgwt.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3akkmwflh.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3jckmmcnv.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3kpgyngga.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3wyqtotds.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3phzqzoel.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3lmvtfniw.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3jcanzlyz.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3cxbzqada.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3xbwouhar.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3woizxwgl.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3afutcnbj.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3zrhanrad.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3mksamasi.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3zolmnmph.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3clxezird.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3gysbngjw.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3cnewvumq.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3zvykombz.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3rhlvxoay.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3sqvbunau.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3txunlesd.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3mylcrjgd.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3cykmyikr.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3nxkkwihn.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3rycohpml.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3ofppvivv.html


<!-- 参考信息 -->