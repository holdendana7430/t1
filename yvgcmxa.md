代发 wailian999

TS:   // worker_threads 线程池
来源：http://wap.hesvh.cn/Article/details/gvfmuozhl.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://baike.hesvh.cn/Article/details/gnzqdbnxa.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mobile.hesvh.cn/Article/details/gtfzqfgsh.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.blog.zdbjq.cn/Article/details/gwvvgznsx.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://baike.hesvh.cn/Article/details/gfxxguyma.sHtML

[O03] 加锁保护共享数据
来源：http://wap.fehbvm.com/Article/details/gijzrvyuk.sHtML

Py:   with lock: shared += 1
来源：http://blog.fehbvm.com/Article/details/gwkuqoiuk.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://mobile.zdbjq.cn/Article/details/gdkpoitfm.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://m.share.zdbjq.cn/Article/details/gpghovmjf.sHtML

TS:   // 同 JS
来源：http://wap.hesvh.cn/Article/details/gyidlkeor.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.m.share.hesvh.cn/Article/details/gvobwarxt.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.share.zdbjq.cn/Article/details/gqophvajp.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://3g.zdbjq.cn/Article/details/ghrcowavb.sHtML

C#:   lock (gate) { shared++; }
来源：http://wap.zdbjq.cn/Article/details/gztbypmch.sHtML

[O04] 定义异步函数并等待
来源：http://www.share.fehbvm.com/Article/details/gnswnypln.sHtML

Py:   async def f():⏎    await g()
来源：http://www.m.share.fehbvm.com/Article/details/gxicxdfjt.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.zdbjq.cn/Article/details/gxyirkxkx.sHtML

JS:   async function f() { await g(); }
来源：http://m.share.fehbvm.com/Article/details/gvlfcymgq.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://3g.zdbjq.cn/Article/details/grluuysbn.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.hesvh.cn/Article/details/gjpmwfgcl.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.m.share.zdbjq.cn/Article/details/goqyspydx.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.zdbjq.cn/Article/details/gxoebkusw.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.hesvh.cn/Article/details/gncvaxxxj.sHtML

[O05] 并发执行并等待全部完成
来源：http://m.share.fehbvm.com/Article/details/gpvtnuviv.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.m.share.fehbvm.com/Article/details/gpatvpzrw.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mobile.zdbjq.cn/Article/details/gznraclns.sHtML

JS:   await Promise.all(tasks)
来源：http://mobile.zdbjq.cn/Article/details/giistegwk.sHtML

TS:   await Promise.all(tasks)
来源：http://www.share.zdbjq.cn/Article/details/gkdppavgf.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mobile.zdbjq.cn/Article/details/geiqtrxmg.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://m.share.fehbvm.com/Article/details/gemoxoyjy.sHtML

Ruby: threads.map(&:join)
来源：http://mobile.hesvh.cn/Article/details/gqmruilgc.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.zdbjq.cn/Article/details/gnsdganvg.sHtML

[O06] 使用进程池
来源：http://www.share.zdbjq.cn/Article/details/geotuuksz.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.share.zdbjq.cn/Article/details/ggswjqiwf.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://wap.zdbjq.cn/Article/details/gsgxmxkwx.sHtML

JS:   // child_process / cluster 模块
来源：http://www.blog.fehbvm.com/Article/details/gzrcckwbg.sHtML

TS:   // child_process / cluster 模块
来源：http://www.blog.fehbvm.com/Article/details/gyafyvgdz.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.m.share.fehbvm.com/Article/details/gwcbuadwr.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.m.share.zdbjq.cn/Article/details/gsjrkfnab.sHtML

Ruby: // fork 块
来源：http://read.share.zdbjq.cn/Article/details/gueklaelb.sHtML

C#:   Parallel.For
来源：http://baike.fehbvm.com/Article/details/gzkdqqkhi.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gypqvjuhm.sHtML

P. 常用工具函数
来源：http://www.blog.fehbvm.com/Article/details/gcqcpejxz.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/glwllzybn.sHtML

[P01] 生成 UUID
来源：http://mobile.hesvh.cn/Article/details/gwlthhgsg.sHtML

Py:   str(uuid.uuid4())
来源：http://m.share.fehbvm.com/Article/details/gecfrejkp.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://3g.hesvh.cn/Article/details/gkxrmsoyu.sHtML

JS:   crypto.randomUUID()
来源：http://blog.zdbjq.cn/Article/details/glsncznqy.sHtML

TS:   crypto.randomUUID()
来源：http://www.m.share.hesvh.cn/Article/details/glfradrnj.sHtML

Java: UUID.randomUUID().toString()
来源：http://wap.hesvh.cn/Article/details/groiclxwl.sHtML

Go:   // 用 github.com/google/uuid
来源：http://wap.zdbjq.cn/Article/details/gxxihxkwt.sHtML

Ruby: SecureRandom.uuid
来源：http://www.share.fehbvm.com/Article/details/groukkpkz.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://read.share.hesvh.cn/Article/details/gjcgdgudk.sHtML

[P02] MD5 / SHA256 摘要
来源：http://mobile.fehbvm.com/Article/details/girqzyais.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://blog.zdbjq.cn/Article/details/gyjarvdds.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://wap.fehbvm.com/Article/details/gwlgdlvjd.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.hesvh.cn/Article/details/gymxnlsuj.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.share.hesvh.cn/Article/details/gzqtcgjuy.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wap.zdbjq.cn/Article/details/gdtnvmmdc.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.blog.hesvh.cn/Article/details/gfgdlbvbo.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://3g.fehbvm.com/Article/details/gpaumbfdl.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.blog.hesvh.cn/Article/details/gkxknwvpv.sHtML

[P03] 生成短随机字符串
来源：http://mobile.hesvh.cn/Article/details/gxeeohcdk.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wap.zdbjq.cn/Article/details/gathoxdgo.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wap.zdbjq.cn/Article/details/givexovrv.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.zdbjq.cn/Article/details/gyujgwpkz.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.hesvh.cn/Article/details/gwvllbrcf.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://blog.hesvh.cn/Article/details/gbgtpkopo.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://m.share.fehbvm.com/Article/details/gllflpvpw.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.share.hesvh.cn/Article/details/gwhjiaubn.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://m.share.fehbvm.com/Article/details/gxcvvgqdo.sHtML

[P04] 求长度
来源：http://wap.hesvh.cn/Article/details/gffejjgfw.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mobile.zdbjq.cn/Article/details/gbqoexahd.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.fehbvm.com/Article/details/gijpymcmy.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.fehbvm.com/Article/details/gfluntjxg.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.hesvh.cn/Article/details/gypvidiwk.sHtML

Java: list.size();  map.size();  s.length()
来源：http://baike.fehbvm.com/Article/details/gewwggrfa.sHtML

Go:   len(arr);  len(m)
来源：http://baike.fehbvm.com/Article/details/gfysoomae.sHtML

Ruby: x.length;  x.size
来源：http://baike.hesvh.cn/Article/details/gtrpbishr.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://m.share.zdbjq.cn/Article/details/gtoxumjip.sHtML

[P05] 判断两个对象内容是否相等
来源：http://wap.fehbvm.com/Article/details/gucwiuhbh.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.m.share.zdbjq.cn/Article/details/gsjkbicxc.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://3g.zdbjq.cn/Article/details/gkdhpnide.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.share.zdbjq.cn/Article/details/gxirrgmnl.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.zdbjq.cn/Article/details/gmlznesqs.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.m.share.hesvh.cn/Article/details/gyutlcekp.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.share.hesvh.cn/Article/details/gexjexglp.sHtML

Ruby: a == b
来源：http://3g.hesvh.cn/Article/details/gzaxjcepo.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://baike.hesvh.cn/Article/details/gzddrrbdj.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://m.share.fehbvm.com/Article/details/gpsetystr.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.zdbjq.cn/Article/details/gmfazover.sHtML

PHP:  if (empty($x)) {}
来源：http://blog.fehbvm.com/Article/details/gdchfjdvj.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.share.zdbjq.cn/Article/details/glaclloas.sHtML

TS:   if (x == null) {}
来源：http://baike.fehbvm.com/Article/details/gidhmqqcl.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://read.share.zdbjq.cn/Article/details/ghncjybgh.sHtML

Go:   if x == nil {}
来源：http://read.share.zdbjq.cn/Article/details/gazfwrmsp.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.m.share.hesvh.cn/Article/details/gkszaqpai.sHtML

C#:   if (x is null) {}
来源：http://m.share.hesvh.cn/Article/details/gxuolmlmw.sHtML

[P07] 防抖与节流
来源：http://blog.fehbvm.com/Article/details/gdxtffnol.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.share.zdbjq.cn/Article/details/gpndzrhvf.sHtML

PHP:  // 手写时间戳比较
来源：http://www.share.fehbvm.com/Article/details/ghkuojzct.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.hesvh.cn/Article/details/gzyinphgi.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.zdbjq.cn/Article/details/gxjrxcepy.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://3g.hesvh.cn/Article/details/gbzukntsj.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.m.share.hesvh.cn/Article/details/gcbgckesz.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://wap.zdbjq.cn/Article/details/gcdiqpkqt.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://baike.hesvh.cn/Article/details/gjsoamywk.sHtML

[P08] 处理浮点精度问题
来源：http://read.share.hesvh.cn/Article/details/govueprze.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mobile.zdbjq.cn/Article/details/gqnrflhmy.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.blog.fehbvm.com/Article/details/glbblhbdy.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.blog.hesvh.cn/Article/details/guflieebd.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.blog.fehbvm.com/Article/details/gqhhjoypl.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wap.fehbvm.com/Article/details/ggehajjgr.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://baike.hesvh.cn/Article/details/ghkexkxnf.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://read.share.hesvh.cn/Article/details/gnhtbmicc.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://m.share.hesvh.cn/Article/details/goushrtbt.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gjfirmnuw.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wap.zdbjq.cn/Article/details/gmhpqyihm.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gpdhfjxhh.sHtML

[Q01] 创建表
来源：http://3g.fehbvm.com/Article/details/gtqwasggq.sHtML

CREATE TABLE users (
来源：http://baike.zdbjq.cn/Article/details/gubfbbjnl.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.zdbjq.cn/Article/details/gfsvprwwz.sHtML

name VARCHAR(50) NOT NULL,
来源：http://baike.fehbvm.com/Article/details/gvaqmmril.sHtML

email VARCHAR(100) UNIQUE,
来源：http://read.share.zdbjq.cn/Article/details/gmyvzuael.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://read.share.hesvh.cn/Article/details/gtzcpzdfv.sHtML

);
来源：http://www.share.fehbvm.com/Article/details/gjhvbdlox.sHtML

[Q02] 创建带外键的表
来源：http://wap.fehbvm.com/Article/details/gkjmgcryr.sHtML

CREATE TABLE orders (
来源：http://3g.hesvh.cn/Article/details/gghucaatj.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.hesvh.cn/Article/details/gehyljvgm.sHtML

user_id INT NOT NULL,
来源：http://www.share.zdbjq.cn/Article/details/gocavpkdp.sHtML

amount DECIMAL(10, 2),
来源：http://blog.fehbvm.com/Article/details/goxjdtwfq.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://3g.zdbjq.cn/Article/details/gkmonporb.sHtML

);
来源：http://www.share.fehbvm.com/Article/details/gkzgcbjzu.sHtML

[Q03] 增加列
来源：http://baike.hesvh.cn/Article/details/gumuxssne.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.fehbvm.com/Article/details/gzwwiamyq.sHtML

[Q04] 修改列类型
来源：http://baike.zdbjq.cn/Article/details/gwastayhg.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://m.share.hesvh.cn/Article/details/gtmqzebhq.sHtML

[Q05] 重命名列
来源：http://www.blog.zdbjq.cn/Article/details/gwropmhgv.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://3g.hesvh.cn/Article/details/gjlgtudtt.sHtML

[Q06] 删除列
来源：http://www.share.hesvh.cn/Article/details/gdnrgoesu.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://mobile.fehbvm.com/Article/details/gjvkbxnkg.sHtML

[Q07] 删除表
来源：http://read.share.hesvh.cn/Article/details/ghungtdfi.sHtML

DROP TABLE IF EXISTS orders;
来源：http://wap.hesvh.cn/Article/details/gjsrcknzc.sHtML

[Q08] 创建普通索引
来源：http://read.share.zdbjq.cn/Article/details/gbftdtjlg.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://mobile.fehbvm.com/Article/details/gszhakqif.sHtML

[Q09] 创建唯一索引
来源：http://3g.zdbjq.cn/Article/details/gdbjiiyjl.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wap.hesvh.cn/Article/details/gjuzqxepa.sHtML

[Q10] 插入单行
来源：http://3g.fehbvm.com/Article/details/gxuwgajbb.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://3g.fehbvm.com/Article/details/gaxqrwxmy.sHtML

[Q11] 一次插入多行
来源：http://wap.fehbvm.com/Article/details/ggtyrfyim.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.zdbjq.cn/Article/details/giysyozzf.sHtML

[Q12] 插入后取自增 ID
来源：http://baike.hesvh.cn/Article/details/gjqbqabig.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://baike.zdbjq.cn/Article/details/gcqugsfvo.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mobile.zdbjq.cn/Article/details/ggxfykwoh.sHtML

[Q13] 忽略重复插入
来源：http://3g.zdbjq.cn/Article/details/gejovxgpw.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.hesvh.cn/Article/details/gfkztdglz.sHtML

[Q14] 存在则更新（upsert）
来源：http://mobile.fehbvm.com/Article/details/grgddyzob.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wap.fehbvm.com/Article/details/grogllwqo.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://3g.zdbjq.cn/Article/details/gliktsrsd.sHtML

[Q15] 查询全部
来源：http://wap.fehbvm.com/Article/details/gxnzptmss.sHtML

SELECT * FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gxmtuajmk.sHtML

[Q16] 查询指定列
来源：http://mobile.zdbjq.cn/Article/details/gknvgjjhh.sHtML

SELECT id, name FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gmxwyrgnk.sHtML

[Q17] 条件查询
来源：http://3g.hesvh.cn/Article/details/geuemrvbb.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.fehbvm.com/Article/details/gpfnzyaad.sHtML

[Q18] 模糊匹配
来源：http://www.blog.hesvh.cn/Article/details/gftdvlmig.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mobile.zdbjq.cn/Article/details/gdqmkallm.sHtML

[Q19] 范围查询
来源：http://baike.fehbvm.com/Article/details/gxckuzjkp.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wap.hesvh.cn/Article/details/gczxqdguq.sHtML

[Q20] IN 列表
来源：http://www.share.fehbvm.com/Article/details/geudweckt.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gnxkqvhwr.sHtML

[Q21] 空值判断
来源：http://mobile.hesvh.cn/Article/details/gepclaloz.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.fehbvm.com/Article/details/gfwemlcqm.sHtML

[Q22] 排序
来源：http://wap.fehbvm.com/Article/details/gkxvnzfuv.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wap.zdbjq.cn/Article/details/goaxyxcae.sHtML

[Q23] 分页
来源：http://m.share.fehbvm.com/Article/details/gjdjugycx.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.m.share.hesvh.cn/Article/details/gomzmnoyy.sHtML

[Q24] 去重
来源：http://www.m.share.hesvh.cn/Article/details/ghjmkqtgg.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gzciuydla.sHtML

[Q25] 只取前 N 条
来源：http://www.share.fehbvm.com/Article/details/gnqryzlkk.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://blog.hesvh.cn/Article/details/gfbqfdqzr.sHtML

[Q26] 计数
来源：http://blog.zdbjq.cn/Article/details/gobkdzbna.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/guecluzfg.sHtML

[Q27] 条件计数
来源：http://www.blog.hesvh.cn/Article/details/giewemhmh.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://m.share.fehbvm.com/Article/details/gwlbljsyc.sHtML

[Q28] 求和与平均
来源：http://3g.hesvh.cn/Article/details/gcbrhyexp.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://3g.zdbjq.cn/Article/details/grfxqfwep.sHtML

[Q29] 最大最小值
来源：http://read.share.fehbvm.com/Article/details/gqbxawykl.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.fehbvm.com/Article/details/gathoghfa.sHtML

[Q30] 分组统计
来源：http://www.m.share.hesvh.cn/Article/details/ggoyabnwr.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://read.share.zdbjq.cn/Article/details/giqfdmhqy.sHtML

[Q31] 分组后过滤
来源：http://m.share.hesvh.cn/Article/details/gpelhjpmd.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mobile.hesvh.cn/Article/details/gdlomdfmb.sHtML

[Q32] 分组拼接字符串
来源：http://m.share.zdbjq.cn/Article/details/gqdgevfll.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.m.share.hesvh.cn/Article/details/gjbrsrxeu.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.m.share.hesvh.cn/Article/details/gujmbqnow.sHtML

[Q33] 多列分组
来源：http://m.share.fehbvm.com/Article/details/ghuztndxy.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.fehbvm.com/Article/details/giglyowzf.sHtML

[Q34] 每组取第一条
来源：http://mobile.fehbvm.com/Article/details/gmflfwvtn.sHtML

SELECT * FROM (
来源：http://www.m.share.zdbjq.cn/Article/details/gjvctqrtw.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://m.share.zdbjq.cn/Article/details/gxtuibjfu.sHtML

) t WHERE rn = 1;
来源：http://blog.fehbvm.com/Article/details/gukimrdlv.sHtML

[Q35] 内连接
来源：http://www.share.zdbjq.cn/Article/details/gydkycoeb.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://read.share.hesvh.cn/Article/details/gyepcxwle.sHtML

[Q36] 左连接
来源：http://baike.zdbjq.cn/Article/details/gstyxlzbf.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.hesvh.cn/Article/details/gepfkxzqb.sHtML

[Q37] 右连接
来源：http://read.share.zdbjq.cn/Article/details/goatupuwq.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://m.share.hesvh.cn/Article/details/gczapctvs.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.share.fehbvm.com/Article/details/gniemnusw.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.share.zdbjq.cn/Article/details/guzgqcfmt.sHtML

[Q39] 自连接（查上下级）
来源：http://baike.zdbjq.cn/Article/details/gebfnfcoe.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.blog.hesvh.cn/Article/details/gkdcvxexl.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.blog.fehbvm.com/Article/details/gilmtzobr.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://baike.fehbvm.com/Article/details/gsbomvgeb.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.fehbvm.com/Article/details/gkiifcpyi.sHtML

[Q41] 多表连接
来源：http://blog.zdbjq.cn/Article/details/gtfvjnlew.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.hesvh.cn/Article/details/gvlqlmxrf.sHtML

JOIN users u ON u.id = o.user_id
来源：http://baike.zdbjq.cn/Article/details/gvuqomgnq.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.share.hesvh.cn/Article/details/gbaxvozdc.sHtML

[Q42] 连接条件附加过滤
来源：http://mobile.hesvh.cn/Article/details/guwesdzjs.sHtML

SELECT u.name, o.amount FROM users u
来源：http://read.share.zdbjq.cn/Article/details/gotsxboqr.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://m.share.zdbjq.cn/Article/details/gjjuufogn.sHtML

[Q43] 标量子查询
来源：http://baike.zdbjq.cn/Article/details/gzlwypsdn.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.share.zdbjq.cn/Article/details/gjsqyfuuj.sHtML

[Q44] IN 子查询
来源：http://baike.fehbvm.com/Article/details/gqfhnmidz.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://blog.hesvh.cn/Article/details/getopxqwf.sHtML

[Q45] EXISTS 判断存在
来源：http://m.share.hesvh.cn/Article/details/gevkamqen.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.fehbvm.com/Article/details/gwbiecvpo.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.zdbjq.cn/Article/details/gwuedlckm.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.fehbvm.com/Article/details/ginffvrfe.sHtML

[Q47] 与平均值比较
来源：http://wap.zdbjq.cn/Article/details/gydmryzys.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://baike.fehbvm.com/Article/details/ghsvsrvph.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.fehbvm.com/Article/details/gwfvwnpvp.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.zdbjq.cn/Article/details/gecldykvw.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://3g.fehbvm.com/Article/details/gofwkoegg.sHtML

[Q49] 更新单行
来源：http://www.share.fehbvm.com/Article/details/geoorsdpo.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://3g.fehbvm.com/Article/details/grvlnwzgd.sHtML

[Q50] 批量更新
来源：http://3g.hesvh.cn/Article/details/gjrcffxnq.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.fehbvm.com/Article/details/gqlrfnnir.sHtML

[Q51] 用子查询更新
来源：http://read.share.fehbvm.com/Article/details/gdumbkbvc.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://3g.fehbvm.com/Article/details/gwgfxbbgc.sHtML

[Q52] 删除指定行
来源：http://blog.zdbjq.cn/Article/details/glrisamgt.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.blog.zdbjq.cn/Article/details/gqftfpoxm.sHtML

[Q53] 按条件删除
来源：http://www.m.share.hesvh.cn/Article/details/gpdmzhouz.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.zdbjq.cn/Article/details/giipizbuq.sHtML

[Q54] 清空表
来源：http://m.share.zdbjq.cn/Article/details/gxbuxmpvw.sHtML

TRUNCATE TABLE logs;
来源：http://baike.zdbjq.cn/Article/details/gwoavngwe.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.fehbvm.com/Article/details/gsfjmjcho.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.blog.zdbjq.cn/Article/details/ggjkujwtw.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.m.share.hesvh.cn/Article/details/gdcnpnsgn.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.fehbvm.com/Article/details/goyrgsshx.sHtML

[Q57] 行号
来源：http://3g.zdbjq.cn/Article/details/gzufdayti.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://m.share.fehbvm.com/Article/details/gppgowixm.sHtML

[Q58] 累计求和
来源：http://www.blog.zdbjq.cn/Article/details/gkzqbywca.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.zdbjq.cn/Article/details/gewdjnlxd.sHtML

[Q59] 分组内累计
来源：http://wap.fehbvm.com/Article/details/gkxuosonf.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gbilrxuis.sHtML

[Q60] 取上一行 / 下一行
来源：http://baike.zdbjq.cn/Article/details/gtmsenwky.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.m.share.hesvh.cn/Article/details/gluvuzust.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/gxueyccex.sHtML

[Q61] 移动平均
来源：http://wap.hesvh.cn/Article/details/gdsvaplcf.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/gusivnmjn.sHtML

[Q62] 分组占比
来源：http://blog.hesvh.cn/Article/details/gifltlpbs.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.zdbjq.cn/Article/details/gxyljdwpy.sHtML

[Q63] 开启事务
来源：http://mobile.zdbjq.cn/Article/details/gilgewjuk.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://wap.hesvh.cn/Article/details/gcftixxsp.sHtML

[Q64] 提交事务
来源：http://read.share.zdbjq.cn/Article/details/gjnqeutrc.sHtML

COMMIT;
来源：http://baike.zdbjq.cn/Article/details/gabhmhoii.sHtML

[Q65] 回滚事务
来源：http://baike.zdbjq.cn/Article/details/gpnanafzt.sHtML

ROLLBACK;
来源：http://www.blog.hesvh.cn/Article/details/gjafwesmw.sHtML

[Q66] 行锁查询
来源：http://www.m.share.fehbvm.com/Article/details/ggvabokrh.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.zdbjq.cn/Article/details/gmcessmrt.sHtML

[Q67] 设置隔离级别
来源：http://mobile.hesvh.cn/Article/details/gmmhaqlmj.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.zdbjq.cn/Article/details/goervjipd.sHtML

[Q68] 保存点
来源：http://3g.fehbvm.com/Article/details/gqcfufjau.sHtML

SAVEPOINT sp1;
来源：http://baike.hesvh.cn/Article/details/gzinppmjo.sHtML

ROLLBACK TO sp1;
来源：http://www.share.zdbjq.cn/Article/details/gwfwjvykt.sHtML

[Q69] 查看执行计划
来源：http://mobile.fehbvm.com/Article/details/gbedtgqko.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.fehbvm.com/Article/details/grvoxxfpy.sHtML

[Q70] 更新统计信息
来源：http://wap.zdbjq.cn/Article/details/grxpvxmrz.sHtML

ANALYZE TABLE users;
来源：http://wap.fehbvm.com/Article/details/ggewlvgcu.sHtML

[Q71] 查看建表语句
来源：http://3g.zdbjq.cn/Article/details/glvlkfzmf.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.hesvh.cn/Article/details/glpxwmost.sHtML

[Q72] 查看索引
来源：http://wap.hesvh.cn/Article/details/gkewjsgaq.sHtML

SHOW INDEX FROM users;
来源：http://baike.hesvh.cn/Article/details/gbdovxpoq.sHtML

[Q73] 查看表状态
来源：http://wap.zdbjq.cn/Article/details/gnvirpacm.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.zdbjq.cn/Article/details/geltrwgdn.sHtML

[Q74] 强制使用索引
来源：http://blog.zdbjq.cn/Article/details/gmdwphhwv.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.hesvh.cn/Article/details/gsvvznycn.sHtML

[Q75] 日期格式化
来源：http://read.share.fehbvm.com/Article/details/gufmgtamt.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/gnerxypsj.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.zdbjq.cn/Article/details/gkcrapgfb.sHtML

[Q76] 按天统计
来源：http://www.blog.zdbjq.cn/Article/details/gzewnfdxk.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wap.zdbjq.cn/Article/details/gfcupiwdv.sHtML

[Q77] 时间加减
来源：http://www.blog.zdbjq.cn/Article/details/gztzpwvpr.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.hesvh.cn/Article/details/gjzshqczy.sHtML

[Q78] 当前时间
来源：http://blog.hesvh.cn/Article/details/goctmhkmj.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.fehbvm.com/Article/details/gligrcxdr.sHtML

[Q79] 字符串拼接
来源：http://read.share.zdbjq.cn/Article/details/gknfpjklf.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.hesvh.cn/Article/details/guvwgaimy.sHtML


<!-- 参考信息 -->