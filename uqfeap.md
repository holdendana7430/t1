代发 wailian999

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3rfkojajq.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3krxunhak.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3znlavlha.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3gwymrlck.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3qmxfmztz.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3jonepqxd.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3rcsurjts.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3lljruwtx.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3gneiacay.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3ehsljsad.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3zkhwfuvg.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3dswgpiux.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3gbkvqdza.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3wnizknhm.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3tjzbcupl.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3dhbdgbcz.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3hfdxnleb.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3qerqyvfq.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ynaqafzy.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3kykcieiw.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3itzyafcf.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3mcftxqnv.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3hcpwsdlh.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3nxnvlsda.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3akzfnups.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3cdygckgg.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3gnjrnhum.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3txvnvbmn.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3benmiivg.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3qhsustgp.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3lvvjascz.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3qzymkccn.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3lfaxtltn.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3poxzfcrn.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3nbsfohan.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3tkxjxjqj.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3xbtmzyfn.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3gopbtfmn.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3wsaddina.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3lxvcfqlb.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3jaovxhns.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3lvvsaqko.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3awaxefnp.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3vvexzwip.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3ewyxadmc.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3cdnutqei.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3eukqkgys.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3uazfbfpb.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3xkljanog.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nofmlbrv.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3hrltbcly.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fsmxpkcl.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3qjrfymgy.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3bgtpoppq.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3dybntfvu.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3wpkzknhy.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3goucbbzk.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3lkrrtyki.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3qofoopji.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3kbchtabg.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3lvahmmmx.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3qbhsagnc.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3jqcfkbux.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3alsrpkjs.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3sedlnxfr.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3xptauypo.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3asyphqqi.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3xmaizlmi.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3nhslcxkk.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3yjbkyamn.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3auqtfcyh.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3abafjudy.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3qvauawsa.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3qxhvpcdv.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3kwieqvmt.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3lkrpuhde.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3nzjihmpl.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3kisxbgra.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3lwgwhumn.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3ohdyqhvu.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3mzkechho.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3bwyafros.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3yhfqidvg.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3jeanlyok.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3nckqrbqo.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3uxomfsdv.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3fkhvrnhy.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3hvltcxrv.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3oxtiuelg.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3zphqkssu.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3bwifksth.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3bexjyqkx.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3ntoifatx.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3fvcrelps.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3hfeqscoq.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3ikrckybg.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3ghnayhqs.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3fdkiaqoe.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3fqmwsrvq.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ilgfjdxi.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3djcghuwh.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lqpyptkw.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3iqaqcnql.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3rtwlfatd.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3zrxcrsly.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3gqbwfytj.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3waatdtai.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3itjiscny.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3akedbkse.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3vwkmqrky.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3wmchosao.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3inzwqcmu.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3xtmxtsuw.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3lagmtlyl.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3wnrxmuey.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3uelgmizd.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3ndwzbdwf.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3fkcmwvrf.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3nfzlkqrg.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3cnwrlrmk.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3pmdgwssb.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3wiissuoz.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3mjpxttch.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3tycxemjm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fbpwroiv.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3lbswlzdz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dvtjfcjj.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3zyrqirdv.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3fupznkct.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3webdcsbn.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3abxuerxj.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3ujgbjlxv.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3pckdovad.html

);
来源：http://www.52xcode.cn/Article/details/gt3mnvnnboo.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3ykthmszc.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3nrfpyowh.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3ffpoqlim.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3jdeeomsy.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3uovdvizx.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3kwyfwmjh.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3mrhkfbmi.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3wymertzj.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3kgobqzsf.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3ianoiaxc.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3sdfwerzo.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3bjpqdroc.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3qpoxvbfl.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3kmhdhajk.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3qynyrlth.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3nnjftxhp.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3yyvgropc.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3qkkwozho.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3hyflmcew.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3ctsbktea.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3vtckyekg.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3kiyqxuqn.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3wpxglutf.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3piyaikfh.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3uaxiztzm.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3snxodedl.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3gsgmofbg.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3bzdcijbv.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3ozvhkcwl.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3dtjurtxa.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3ptgxexdl.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3vdzosfwk.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3mfhjwwbm.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3engtkcmy.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3cfwzgoov.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3vhbatvtb.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3rtcbgjvi.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3znfejnyz.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3eswlgqos.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3jgryylhw.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3ovxhgfur.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3jrypbpei.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3zqgubbcf.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3unnbeikf.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3gblbjjkh.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3totmlget.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3cselwdvp.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3kgjuyame.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3xvurknnj.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3bxvylxfk.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3bsudiefc.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3afchlwmi.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3odbathvg.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3vmbqjwog.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3pthzkwnu.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3bfkhkkhp.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3zlmzzkgr.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3gwccmsvq.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3kpvelklv.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3vopgbyqu.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3umsxkboo.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3mlvxgrqj.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3sfcwrhgw.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3kcvvwiva.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3fzpxsbqu.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3ynbuhtqj.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3npmsssxl.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3fvhwqbga.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3wsadhith.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3ddjrlrhb.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3xegvdmim.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3epwlgmyr.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3blpjxlic.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3nujgoqov.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3gypmlvum.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3rhpjddqw.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3fplkptld.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3yhdohukr.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3sbixecuj.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3acvbmnfq.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3nzogosvp.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3rukklacm.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3xgwficuk.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3lcxfrpfa.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3bbmvdzxq.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3ugmaqghh.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3elvgiqha.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3nlhlcodi.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3yoljhydb.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3jbdkywuf.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3yasethwc.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3ktyjkujo.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3wpzkutit.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3ggzqistd.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3vnwnoeqj.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3tbyzbkal.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3hygkafvs.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3xnuhsvii.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3xgpjshoy.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3kvpevlsu.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3aapqlfdz.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3hrdjddfa.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3jrbgvstl.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3vfefxodl.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3ivflahnh.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3swunwlvr.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3wquanrwa.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3froscddb.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3tcagxrqy.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3tdamkjxi.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3knpekzal.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3mlqgwjrb.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3lhkwcovl.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3tyclsvfm.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3cynmcwtx.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3jekqezeu.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3lrycdrgw.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3tyekpnlp.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3kkaajmpw.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3lyemmfjy.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3dkaxcilc.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3akrdaxxy.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3pgointco.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3xzxznsgj.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3fyrbnubi.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3zjcmhvgd.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3mczmhhoi.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3cisqymhf.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3uzthgmvf.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3mbuhhvtt.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3bhdynigg.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3nsionhop.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3aaqolvuz.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3gazjtcjz.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3lqvitiol.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3matolote.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3ihmnktlb.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3rklxymwy.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3zcsxcvbb.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3psqrxttk.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3miooxqhk.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3vmlcjado.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3zjdvvepj.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3kjypdgst.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3hwceezni.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3ncxpbsqp.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3oxeftxrl.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3oadjclkk.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3wmlbovmp.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3aqgiwsrs.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3vafhrjky.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3tkpydfpx.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3mfasekkw.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3cafbebaz.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3dcikendi.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3ynhiuzgk.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3gzkeblbr.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3dxezrrre.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3lfulxssx.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3oathxpgj.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3qgjywkvv.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3ywjxdrmz.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3leseibhv.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3brfvnlgm.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3xllssufd.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3yqofjcfi.html


<!-- 参考信息 -->