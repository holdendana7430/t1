代发 wailian999

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3rthfvkng.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3pjtoetwd.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3xwrdbwne.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3rxpautxy.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3qrlevxpr.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3zhmfrfpm.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3linapqtd.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3xjrnksne.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3voglgjly.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3rhqbastm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3smjgeomt.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3tnepscmn.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3xojzwyvs.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3fhbdcqvg.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3oyxgrtfb.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3vyemljmb.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3qdaddgkp.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3kkftkzep.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3sqvzvfbx.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3zdpbnaud.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3uuufubto.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3lrjycmmv.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3uytyyqax.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3nyrmkuav.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3icvcvtsh.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3duedkimq.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3pgaagyyz.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3zpjodycw.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3whodxbct.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3lutlrjwi.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3lajregzp.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3xuuosnia.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3iltbfujd.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3ypaoxgsv.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3gfhtdrxq.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3rlgpsvwx.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3riwvzxmr.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3pbqochzs.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3thsyctnr.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3pvaatkdu.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3wpfifzgz.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3aiehieho.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3ocygayhs.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3tbtbcesq.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3hmwnmzrk.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3iinluytf.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3jtccwywd.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3bloeuxsn.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3vbwrfhwp.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3bjxamufn.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3khhitknt.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3iscxsfzw.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3ueypbobm.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3amaeprzw.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3ppewpuqq.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3kdlneiid.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3qkzeouan.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3cuobolrq.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3lkrjgqso.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3nyphhsmz.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3pudwkeya.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3zjrneqko.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3bmzovbfg.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3tbliwjeb.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3uxzktdim.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zuaqrslc.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3xafdobci.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3luonthuz.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3xsetjdsi.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3btvgnqdu.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3xavrgtkn.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3pliveyvl.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3yapxpkim.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3wiuhkwnk.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3priekbrq.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3lhvzwlqh.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3pgjvupoz.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3gusxtgzg.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3vpndevvd.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ergsfibw.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3erlwozlq.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3qkeoyxsy.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3lbzhiixk.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3kneuired.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3bzbcqeqd.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3kahggswp.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3mhqkkskp.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3yxirbilv.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3jybsiltb.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3ggmcqtaq.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3etvjvysd.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3oewznkbl.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3eiegceox.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3uqrzrkvq.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3znwczwtu.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3potwhrkk.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3kijnzvjr.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3dtbupuvx.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3uafjbfpa.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3ddnwepob.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3mygkcpus.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3uhphjyjc.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3fxvpovcv.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3opqkvuqb.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3jdemyvmf.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3csxjdsdq.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3xcxxkoys.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3pvwitbfp.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3ysdhxdcq.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3hgkoidvo.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3szmxyujp.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3fzlioigm.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3brgwggod.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3hrwzymfs.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3ahihbeny.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mavfrztn.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3dqygwkav.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wgixaoup.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3skuopixf.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3trfzywyt.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3cfghctfq.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hikbplia.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3mspxcryu.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3jujkhpqh.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3ypkpuood.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3dlkfdbjz.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3fqgzmxdw.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3zqwuvrup.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3xjmmwiqm.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3dpayofvs.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3tuffnfiu.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3jojytdwr.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3sdiymhph.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3qtjlfprf.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3rqhqbdnp.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3fecgdyxm.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3vmkejhor.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3iislxvsd.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3yqnlxuya.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3ggdwsvav.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hsbrbunb.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3ugxftczw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lnsdwdrc.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3ktedgbpf.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3tmwwhgvu.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3vlardhez.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3wydxilqo.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3lrnnavml.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3nnbmlfdx.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3mkasbsoj.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3awlpbyts.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3ckqpglzp.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3ydlqniza.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3jnvhovqt.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3whrnjaea.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3iijzfagc.html

);
来源：http://www.52xcode.cn/Article/details/gt3cjwxfynl.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3hhnduegk.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3gbvuthpk.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3dbbedstl.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3appaluaj.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3pbahfxqq.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3hshzblwx.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3zbrjbwih.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3iqeibszw.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3fyfmgaqv.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3rxwkchlz.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3kqwtlobb.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3ajaovaym.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3eqekshwo.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3mefhktgv.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3rlcpqdkp.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3nvnhnkiy.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3xhgzvzko.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3kwnzbzrw.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3icematfy.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3nuogaaft.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3iqycbnrp.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3dwfdsvgg.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3ohoagdxm.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3kwjeecgt.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3horxjfef.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3reuanwzm.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3szgjlvsz.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3rlyfjjye.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3qavjbmuo.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3evauohvx.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3pnlkjwfr.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3krfttcuu.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3jwhztvat.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3gboizrrj.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3katnihps.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3sshtmmhc.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3lctwswnr.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3cvdxisqk.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3yvyhohwh.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3wjuiscfc.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3zgpzlcqb.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3zkhkkiyb.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3lgdckikh.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3givumdyj.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3molbjpjm.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3tcaowqsl.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3mlggypms.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3pvwbntqq.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3zgnsqszq.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3tdjikhtt.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3lvmduelv.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3kgxmfwqi.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3bjjtefzg.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3uylwmweq.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3riuggehw.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3woghgghj.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3lbvqlfro.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3cajavbyc.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3iezbqrma.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3kbzodjqq.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3gjkixprb.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3exqjeigx.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3ymqceezu.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3sgfaxluc.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3vafoupbe.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3bbnffobh.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3dzvjfjtg.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3dcmumdyw.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3pcvncdjp.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3syretybh.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3eejelvox.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3yscorzeo.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3lnwnwleg.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3enzcmfge.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3tssewshp.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3vbypigjp.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3fequezlh.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3tqyxxfbi.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3zpjsorgt.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3oyuwbopk.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3rbunfqqr.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3uadpghgo.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3zvtfimws.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3mvfxvqxy.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3uomzmzus.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3hnwozmkm.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3nlvlwezt.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3snrmdmpr.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3eldiiypv.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3bvbrigth.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3klrhlnoy.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3zirmpiod.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3ohmjkzbm.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3kihknjxl.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3dobekarz.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3zyyckihc.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3okcvzsxh.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3nanftvxl.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3qtvewmdq.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3zogyczri.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3xoixghod.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3stxbwcge.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3wlmrhbog.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3qhbzktxg.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3eouytbqd.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3ualaoqww.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3shahiefb.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3wdcorxfp.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3xuofhibr.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3znnsrvoa.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3sungkkza.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3ashnipzb.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3tzwdiufk.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3tnhizllb.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3prmzssaz.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3umwyivqm.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3pzfcgsfo.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3randmcda.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3pepowstr.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ulxjobqx.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3mquvssmw.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3qhdgcrtq.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3mfdyvwns.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3maqfqhzf.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3vbopeuge.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3jcoiyjaf.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3zbntfxph.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3fxfvbtvv.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3mfscavxe.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3urxchstg.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3ljcdivnk.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3hljyqtot.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3acxjayac.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3mmcwtaev.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3isoaurlr.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3hzsbnvkj.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3vfxajhtt.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3qzpxxjie.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3nsewtawi.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3mfheisla.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3kggfdlom.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3ylaanyaa.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3bdlvgasz.html


<!-- 参考信息 -->