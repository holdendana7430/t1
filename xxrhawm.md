代发 wailian999

Java: new Thread(() -> f()).start()
来源：http://www.blog.fehbvm.com/Article/details/givppizbk.sHtML

Go:   go f()
来源：http://baike.fehbvm.com/Article/details/ggetdcfzt.sHtML

Ruby: Thread.new { f }
来源：http://read.share.fehbvm.com/Article/details/gnbxbcbvn.sHtML

C#:   Task.Run(() => F());
来源：http://www.m.share.hesvh.cn/Article/details/guvlirxms.sHtML

[O02] 使用线程池
来源：http://baike.zdbjq.cn/Article/details/gvngtmdyh.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.fehbvm.com/Article/details/gdkngmovh.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.blog.zdbjq.cn/Article/details/grkbjolkt.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.hesvh.cn/Article/details/gkizpmedb.sHtML

TS:   // worker_threads 线程池
来源：http://www.share.zdbjq.cn/Article/details/gatmitfkv.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://3g.fehbvm.com/Article/details/gmzuwmwfk.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://m.share.zdbjq.cn/Article/details/gfpjhjgeb.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mobile.zdbjq.cn/Article/details/gyyiursfx.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.m.share.fehbvm.com/Article/details/gshaihbbq.sHtML

[O03] 加锁保护共享数据
来源：http://www.share.fehbvm.com/Article/details/gpglrwgsa.sHtML

Py:   with lock: shared += 1
来源：http://mobile.zdbjq.cn/Article/details/gcexayxvu.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://m.share.zdbjq.cn/Article/details/gecqqfuth.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.fehbvm.com/Article/details/gjeurrnoc.sHtML

TS:   // 同 JS
来源：http://3g.zdbjq.cn/Article/details/gsimfcpjx.sHtML

Java: synchronized (this) { shared++; }
来源：http://mobile.hesvh.cn/Article/details/gbxhuhary.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.blog.fehbvm.com/Article/details/gdkeegpww.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://blog.hesvh.cn/Article/details/gjhxnqatq.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.hesvh.cn/Article/details/gnzrvchsa.sHtML

[O04] 定义异步函数并等待
来源：http://baike.hesvh.cn/Article/details/gwaeretas.sHtML

Py:   async def f():⏎    await g()
来源：http://www.m.share.fehbvm.com/Article/details/gtdvtgutk.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.hesvh.cn/Article/details/gtrkmugho.sHtML

JS:   async function f() { await g(); }
来源：http://mobile.fehbvm.com/Article/details/ggkkxrizq.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://blog.fehbvm.com/Article/details/gpdxwrpwz.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.zdbjq.cn/Article/details/gjexvhsrc.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://baike.fehbvm.com/Article/details/gwmkjlqsb.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://blog.zdbjq.cn/Article/details/gkkfzthhw.sHtML

C#:   async Task F() { await G(); }
来源：http://www.blog.hesvh.cn/Article/details/gxvfvfovh.sHtML

[O05] 并发执行并等待全部完成
来源：http://wap.zdbjq.cn/Article/details/gfyitnbfn.sHtML

Py:   asyncio.gather(*tasks)
来源：http://wap.zdbjq.cn/Article/details/ghbybxbmv.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://blog.fehbvm.com/Article/details/gssnyfcpf.sHtML

JS:   await Promise.all(tasks)
来源：http://wap.zdbjq.cn/Article/details/gfolxngtv.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.fehbvm.com/Article/details/gmomwgmsh.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mobile.fehbvm.com/Article/details/ggtxqzahh.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://read.share.zdbjq.cn/Article/details/gbfoigvsy.sHtML

Ruby: threads.map(&:join)
来源：http://wap.zdbjq.cn/Article/details/gftiajhld.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.fehbvm.com/Article/details/gmwbprrmt.sHtML

[O06] 使用进程池
来源：http://blog.hesvh.cn/Article/details/gwyrhdsik.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://blog.hesvh.cn/Article/details/gdbzzxjzj.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://baike.zdbjq.cn/Article/details/gyodqhbfc.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.zdbjq.cn/Article/details/gldiucdkr.sHtML

TS:   // child_process / cluster 模块
来源：http://baike.hesvh.cn/Article/details/gumhiklyx.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wap.hesvh.cn/Article/details/ggnzqphai.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.blog.zdbjq.cn/Article/details/glxizowyu.sHtML

Ruby: // fork 块
来源：http://m.share.zdbjq.cn/Article/details/gygwzccih.sHtML

C#:   Parallel.For
来源：http://read.share.fehbvm.com/Article/details/gzovfnzzf.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gocbgeldg.sHtML

P. 常用工具函数
来源：http://www.blog.fehbvm.com/Article/details/gxddatdbu.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gkmtgfjca.sHtML

[P01] 生成 UUID
来源：http://mobile.hesvh.cn/Article/details/gcbieptzq.sHtML

Py:   str(uuid.uuid4())
来源：http://wap.zdbjq.cn/Article/details/gecndlbfg.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://read.share.hesvh.cn/Article/details/gqcivbjft.sHtML

JS:   crypto.randomUUID()
来源：http://baike.fehbvm.com/Article/details/gryxwojmm.sHtML

TS:   crypto.randomUUID()
来源：http://www.m.share.hesvh.cn/Article/details/ghrkqsdkh.sHtML

Java: UUID.randomUUID().toString()
来源：http://mobile.fehbvm.com/Article/details/gmqcdymrj.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.blog.zdbjq.cn/Article/details/gnlvdvwfy.sHtML

Ruby: SecureRandom.uuid
来源：http://read.share.hesvh.cn/Article/details/ggdcsfsjc.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.share.hesvh.cn/Article/details/gakjxqhoa.sHtML

[P02] MD5 / SHA256 摘要
来源：http://blog.hesvh.cn/Article/details/gtsatjfsg.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://read.share.zdbjq.cn/Article/details/ggpywhekz.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.m.share.fehbvm.com/Article/details/gocohxhfm.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.fehbvm.com/Article/details/gdhpicvwz.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://baike.hesvh.cn/Article/details/gmtdjslwj.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://m.share.zdbjq.cn/Article/details/ginwbxeib.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://3g.hesvh.cn/Article/details/giijquqgg.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.m.share.zdbjq.cn/Article/details/grlrwthhx.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.share.fehbvm.com/Article/details/gijedgcqa.sHtML

[P03] 生成短随机字符串
来源：http://www.m.share.hesvh.cn/Article/details/gzdjqolkk.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.share.fehbvm.com/Article/details/grpdlzmrj.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mobile.fehbvm.com/Article/details/gtmfcxdug.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.fehbvm.com/Article/details/gfgopiwvz.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.fehbvm.com/Article/details/gepxgfzzh.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.hesvh.cn/Article/details/gzdjochyo.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.hesvh.cn/Article/details/gkyexdese.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://3g.hesvh.cn/Article/details/ggkjktmzd.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://3g.fehbvm.com/Article/details/gkllbprgk.sHtML

[P04] 求长度
来源：http://www.m.share.zdbjq.cn/Article/details/gpiaijdjf.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.share.fehbvm.com/Article/details/gfyafbkce.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.fehbvm.com/Article/details/gthrqefhd.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.hesvh.cn/Article/details/gorteblpm.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.fehbvm.com/Article/details/gazmehbjs.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.share.zdbjq.cn/Article/details/gdfacnhux.sHtML

Go:   len(arr);  len(m)
来源：http://wap.hesvh.cn/Article/details/gkoybwsif.sHtML

Ruby: x.length;  x.size
来源：http://3g.hesvh.cn/Article/details/gemtrbtko.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://baike.fehbvm.com/Article/details/gquplizyw.sHtML

[P05] 判断两个对象内容是否相等
来源：http://read.share.hesvh.cn/Article/details/gsmakpcjp.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://mobile.hesvh.cn/Article/details/ghwsfzmxr.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.m.share.hesvh.cn/Article/details/gfxoswwtu.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://baike.zdbjq.cn/Article/details/gewiqgouu.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.zdbjq.cn/Article/details/glrovegxk.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://3g.zdbjq.cn/Article/details/glofvolfb.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://baike.hesvh.cn/Article/details/gaozjcrti.sHtML

Ruby: a == b
来源：http://www.blog.zdbjq.cn/Article/details/glnqketxb.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://baike.fehbvm.com/Article/details/gbloapwev.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://blog.hesvh.cn/Article/details/gcbwdmnbv.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wap.hesvh.cn/Article/details/ghpcrhuoq.sHtML

PHP:  if (empty($x)) {}
来源：http://read.share.zdbjq.cn/Article/details/goyskwjgo.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mobile.zdbjq.cn/Article/details/gcgcfzojv.sHtML

TS:   if (x == null) {}
来源：http://www.blog.hesvh.cn/Article/details/gdmogjhey.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.share.hesvh.cn/Article/details/ghurpjfpu.sHtML

Go:   if x == nil {}
来源：http://www.blog.hesvh.cn/Article/details/geowhnwsy.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wap.fehbvm.com/Article/details/gppiykjbd.sHtML

C#:   if (x is null) {}
来源：http://wap.zdbjq.cn/Article/details/gtfntlwfg.sHtML

[P07] 防抖与节流
来源：http://wap.hesvh.cn/Article/details/gnfmqgzio.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mobile.hesvh.cn/Article/details/gifpufxpa.sHtML

PHP:  // 手写时间戳比较
来源：http://www.m.share.fehbvm.com/Article/details/gbypeaakm.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.hesvh.cn/Article/details/gqxmygaxp.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.fehbvm.com/Article/details/giiptvbim.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://m.share.fehbvm.com/Article/details/gqmxunwoa.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.fehbvm.com/Article/details/gxvdelpwj.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://read.share.hesvh.cn/Article/details/gmugsijjg.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://3g.fehbvm.com/Article/details/gvwqbwfxb.sHtML

[P08] 处理浮点精度问题
来源：http://www.share.zdbjq.cn/Article/details/gegdiwcra.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://read.share.fehbvm.com/Article/details/gaogqpnxq.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://3g.hesvh.cn/Article/details/gpykuydyc.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://3g.zdbjq.cn/Article/details/gbiyzqzxn.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.m.share.fehbvm.com/Article/details/gbtteavnw.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://baike.zdbjq.cn/Article/details/gknjegyta.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.blog.hesvh.cn/Article/details/gluccpnaz.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.blog.hesvh.cn/Article/details/gfvrdeezi.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mobile.zdbjq.cn/Article/details/gbfkqpdxz.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gyrpcxkgh.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://3g.fehbvm.com/Article/details/gwwkqgzel.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gwdccofov.sHtML

[Q01] 创建表
来源：http://wap.zdbjq.cn/Article/details/gisampxfx.sHtML

CREATE TABLE users (
来源：http://www.m.share.fehbvm.com/Article/details/gtdcloijz.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.hesvh.cn/Article/details/gnqupxqcz.sHtML

name VARCHAR(50) NOT NULL,
来源：http://m.share.zdbjq.cn/Article/details/grbxbfjrb.sHtML

email VARCHAR(100) UNIQUE,
来源：http://3g.zdbjq.cn/Article/details/gjltdfawz.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://3g.fehbvm.com/Article/details/giajnfbtw.sHtML

);
来源：http://blog.hesvh.cn/Article/details/gixfxnhrf.sHtML

[Q02] 创建带外键的表
来源：http://www.blog.zdbjq.cn/Article/details/gblckofpt.sHtML

CREATE TABLE orders (
来源：http://www.m.share.zdbjq.cn/Article/details/gbpdxrdwh.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.fehbvm.com/Article/details/gedmcwvop.sHtML

user_id INT NOT NULL,
来源：http://www.share.fehbvm.com/Article/details/guqszkmym.sHtML

amount DECIMAL(10, 2),
来源：http://www.m.share.hesvh.cn/Article/details/gzvdiclpi.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mobile.hesvh.cn/Article/details/gaozokuww.sHtML

);
来源：http://m.share.fehbvm.com/Article/details/gzepufzxn.sHtML

[Q03] 增加列
来源：http://baike.zdbjq.cn/Article/details/gsnkpvbjp.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://m.share.hesvh.cn/Article/details/gsyhpzjfo.sHtML

[Q04] 修改列类型
来源：http://m.share.hesvh.cn/Article/details/ghqymkabt.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://3g.fehbvm.com/Article/details/gkhgkshou.sHtML

[Q05] 重命名列
来源：http://baike.hesvh.cn/Article/details/gqcnwhxgb.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://m.share.hesvh.cn/Article/details/gvrwezaao.sHtML

[Q06] 删除列
来源：http://read.share.fehbvm.com/Article/details/guutzulvs.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://3g.hesvh.cn/Article/details/ghrkqnlvi.sHtML

[Q07] 删除表
来源：http://wap.hesvh.cn/Article/details/goncrbaje.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.share.hesvh.cn/Article/details/ginspdqsv.sHtML

[Q08] 创建普通索引
来源：http://blog.hesvh.cn/Article/details/gbzyktbbl.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.m.share.zdbjq.cn/Article/details/glwubwseb.sHtML

[Q09] 创建唯一索引
来源：http://mobile.hesvh.cn/Article/details/gswervbzc.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mobile.hesvh.cn/Article/details/gsbvjlqmt.sHtML

[Q10] 插入单行
来源：http://blog.hesvh.cn/Article/details/gbuhwagpk.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.zdbjq.cn/Article/details/ghmvlooyq.sHtML

[Q11] 一次插入多行
来源：http://3g.hesvh.cn/Article/details/giayzynqh.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.hesvh.cn/Article/details/gkjfpfaem.sHtML

[Q12] 插入后取自增 ID
来源：http://www.blog.hesvh.cn/Article/details/gkattdnec.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://read.share.fehbvm.com/Article/details/geuakxgog.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://blog.hesvh.cn/Article/details/gahyxypme.sHtML

[Q13] 忽略重复插入
来源：http://blog.fehbvm.com/Article/details/gbjpuaedu.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.share.zdbjq.cn/Article/details/gjbdmkery.sHtML

[Q14] 存在则更新（upsert）
来源：http://blog.fehbvm.com/Article/details/gowetrxdb.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mobile.fehbvm.com/Article/details/gfflocqlj.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.share.hesvh.cn/Article/details/ggyrrckqn.sHtML

[Q15] 查询全部
来源：http://www.blog.hesvh.cn/Article/details/glshyuszx.sHtML

SELECT * FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gfitahmwk.sHtML

[Q16] 查询指定列
来源：http://wap.fehbvm.com/Article/details/gjwhsayss.sHtML

SELECT id, name FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gcltumfco.sHtML

[Q17] 条件查询
来源：http://blog.zdbjq.cn/Article/details/goyfzgigq.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://3g.zdbjq.cn/Article/details/gcopqzrqm.sHtML

[Q18] 模糊匹配
来源：http://m.share.hesvh.cn/Article/details/gadlefejc.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wap.fehbvm.com/Article/details/gveewgfxd.sHtML

[Q19] 范围查询
来源：http://www.blog.hesvh.cn/Article/details/gdcrhumta.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://read.share.hesvh.cn/Article/details/goyccoajy.sHtML

[Q20] IN 列表
来源：http://3g.hesvh.cn/Article/details/gpzsjpyse.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://3g.hesvh.cn/Article/details/guzjxcnsh.sHtML

[Q21] 空值判断
来源：http://www.m.share.zdbjq.cn/Article/details/gcxlzatbs.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.fehbvm.com/Article/details/gvkyfphib.sHtML

[Q22] 排序
来源：http://wap.fehbvm.com/Article/details/gvekgeolt.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.zdbjq.cn/Article/details/gyovqyzfu.sHtML

[Q23] 分页
来源：http://m.share.zdbjq.cn/Article/details/gaccxhogq.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://blog.hesvh.cn/Article/details/gszbrcehh.sHtML

[Q24] 去重
来源：http://www.blog.zdbjq.cn/Article/details/gmgcoipiy.sHtML

SELECT DISTINCT city FROM users;
来源：http://baike.hesvh.cn/Article/details/geenoaigt.sHtML

[Q25] 只取前 N 条
来源：http://mobile.fehbvm.com/Article/details/gdycwtsuw.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://m.share.hesvh.cn/Article/details/goemzxhjt.sHtML

[Q26] 计数
来源：http://www.share.fehbvm.com/Article/details/godpsbimb.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.share.hesvh.cn/Article/details/geksfutwh.sHtML

[Q27] 条件计数
来源：http://3g.zdbjq.cn/Article/details/gnilcqyjb.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gwvznqfyv.sHtML

[Q28] 求和与平均
来源：http://blog.fehbvm.com/Article/details/gqlloyhem.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/goixxiyvy.sHtML

[Q29] 最大最小值
来源：http://m.share.zdbjq.cn/Article/details/goqefsgct.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gcdxssiyk.sHtML

[Q30] 分组统计
来源：http://www.blog.zdbjq.cn/Article/details/gxghdwhtl.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.blog.hesvh.cn/Article/details/gzuidkfxe.sHtML

[Q31] 分组后过滤
来源：http://www.m.share.hesvh.cn/Article/details/gqcgcgqcy.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wap.fehbvm.com/Article/details/gnjfmrdjm.sHtML

[Q32] 分组拼接字符串
来源：http://www.share.hesvh.cn/Article/details/gazjiylbl.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.zdbjq.cn/Article/details/gdusujcec.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.fehbvm.com/Article/details/gmgmgcgvm.sHtML

[Q33] 多列分组
来源：http://baike.fehbvm.com/Article/details/gnvglpxbf.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.hesvh.cn/Article/details/gxdksrcyb.sHtML

[Q34] 每组取第一条
来源：http://3g.fehbvm.com/Article/details/gdelopzpu.sHtML

SELECT * FROM (
来源：http://www.m.share.hesvh.cn/Article/details/gizobeyqy.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://read.share.fehbvm.com/Article/details/gkttbjrre.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gzsauntmy.sHtML

[Q35] 内连接
来源：http://wap.zdbjq.cn/Article/details/geyijxkwa.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://m.share.zdbjq.cn/Article/details/gstwllxaj.sHtML

[Q36] 左连接
来源：http://m.share.zdbjq.cn/Article/details/gxzbcgacn.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://m.share.hesvh.cn/Article/details/guikfyedt.sHtML

[Q37] 右连接
来源：http://mobile.zdbjq.cn/Article/details/gvtcluhze.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://blog.hesvh.cn/Article/details/ghncywzxa.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.share.hesvh.cn/Article/details/gmfymhckc.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://blog.zdbjq.cn/Article/details/gqisziqrz.sHtML

[Q39] 自连接（查上下级）
来源：http://3g.fehbvm.com/Article/details/ggtmggict.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://3g.fehbvm.com/Article/details/gwvewhtip.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.blog.hesvh.cn/Article/details/gkfjyvvob.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://m.share.zdbjq.cn/Article/details/gdfplvphc.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.blog.hesvh.cn/Article/details/gcbcgohsl.sHtML

[Q41] 多表连接
来源：http://3g.fehbvm.com/Article/details/gkiksfixd.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.fehbvm.com/Article/details/gmhtndzzy.sHtML

JOIN users u ON u.id = o.user_id
来源：http://mobile.hesvh.cn/Article/details/gaotclfzn.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.hesvh.cn/Article/details/greonmmxw.sHtML

[Q42] 连接条件附加过滤
来源：http://m.share.fehbvm.com/Article/details/gjeczmdrh.sHtML

SELECT u.name, o.amount FROM users u
来源：http://mobile.zdbjq.cn/Article/details/gjscyylxm.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.zdbjq.cn/Article/details/gykyczfrs.sHtML

[Q43] 标量子查询
来源：http://www.blog.fehbvm.com/Article/details/ginwdljwn.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.blog.fehbvm.com/Article/details/gvbnbiams.sHtML

[Q44] IN 子查询
来源：http://read.share.fehbvm.com/Article/details/gocbyvcer.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mobile.hesvh.cn/Article/details/gdcokajzy.sHtML

[Q45] EXISTS 判断存在
来源：http://blog.hesvh.cn/Article/details/galkyzhqb.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.fehbvm.com/Article/details/gavncvuhd.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.share.zdbjq.cn/Article/details/gbfhmynah.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.fehbvm.com/Article/details/gxsbkrjyl.sHtML

[Q47] 与平均值比较
来源：http://mobile.fehbvm.com/Article/details/gbuknubmd.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://m.share.hesvh.cn/Article/details/gusmbuyxm.sHtML

[Q48] CTE 公用表表达式
来源：http://baike.fehbvm.com/Article/details/grxqldehd.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://3g.fehbvm.com/Article/details/gtaodvfsc.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.hesvh.cn/Article/details/gajpivlar.sHtML

[Q49] 更新单行
来源：http://www.m.share.zdbjq.cn/Article/details/gizpxojwi.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.share.fehbvm.com/Article/details/gsrerxfqd.sHtML

[Q50] 批量更新
来源：http://3g.hesvh.cn/Article/details/gtbjzguxx.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://blog.hesvh.cn/Article/details/gsyfdakzx.sHtML

[Q51] 用子查询更新
来源：http://www.m.share.hesvh.cn/Article/details/ghvggketk.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wap.fehbvm.com/Article/details/gnfbtzcxw.sHtML

[Q52] 删除指定行
来源：http://baike.zdbjq.cn/Article/details/gfbjsrtsk.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.m.share.zdbjq.cn/Article/details/grzkujjmw.sHtML

[Q53] 按条件删除
来源：http://m.share.hesvh.cn/Article/details/gntwxmosk.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://3g.hesvh.cn/Article/details/ggkypclml.sHtML

[Q54] 清空表
来源：http://www.blog.fehbvm.com/Article/details/gfrdenskz.sHtML

TRUNCATE TABLE logs;
来源：http://baike.zdbjq.cn/Article/details/gmqeeuxxz.sHtML

[Q55] 排名（并列占位）
来源：http://www.share.hesvh.cn/Article/details/gtjyjdvxc.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.hesvh.cn/Article/details/gkhjudbuw.sHtML

[Q56] 密集排名（并列不占位）
来源：http://3g.zdbjq.cn/Article/details/gwroixalv.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.hesvh.cn/Article/details/gjchdegvl.sHtML

[Q57] 行号
来源：http://3g.zdbjq.cn/Article/details/gpacbyglr.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.zdbjq.cn/Article/details/gjtotezaa.sHtML

[Q58] 累计求和
来源：http://m.share.zdbjq.cn/Article/details/ggpsvmwra.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.fehbvm.com/Article/details/gbdygghfg.sHtML

[Q59] 分组内累计
来源：http://3g.hesvh.cn/Article/details/gaecpwyby.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.fehbvm.com/Article/details/gidgoorjg.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.zdbjq.cn/Article/details/gnnwmqkhk.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.hesvh.cn/Article/details/gmomptygb.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.hesvh.cn/Article/details/gfxcfnbzu.sHtML

[Q61] 移动平均
来源：http://read.share.zdbjq.cn/Article/details/gqaaprnxs.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.hesvh.cn/Article/details/ghhrdvrzj.sHtML

[Q62] 分组占比
来源：http://www.m.share.zdbjq.cn/Article/details/ghouzejsc.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://baike.hesvh.cn/Article/details/grbwnmqmx.sHtML

[Q63] 开启事务
来源：http://www.share.zdbjq.cn/Article/details/genipaubv.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.fehbvm.com/Article/details/gwgvqiwzc.sHtML

[Q64] 提交事务
来源：http://wap.hesvh.cn/Article/details/gwszlknze.sHtML

COMMIT;
来源：http://www.m.share.hesvh.cn/Article/details/govzdsjap.sHtML

[Q65] 回滚事务
来源：http://www.blog.zdbjq.cn/Article/details/gkblcsuom.sHtML

ROLLBACK;
来源：http://wap.zdbjq.cn/Article/details/gdztowkyy.sHtML

[Q66] 行锁查询
来源：http://mobile.zdbjq.cn/Article/details/guesmhucp.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.zdbjq.cn/Article/details/ghgqnusox.sHtML

[Q67] 设置隔离级别
来源：http://m.share.zdbjq.cn/Article/details/gvmpfschq.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.zdbjq.cn/Article/details/giqkoahci.sHtML

[Q68] 保存点
来源：http://www.blog.zdbjq.cn/Article/details/gkbozptyj.sHtML

SAVEPOINT sp1;
来源：http://www.share.zdbjq.cn/Article/details/gdlskbdcz.sHtML

ROLLBACK TO sp1;
来源：http://blog.zdbjq.cn/Article/details/gqaambgba.sHtML

[Q69] 查看执行计划
来源：http://www.share.hesvh.cn/Article/details/glxvurfea.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.hesvh.cn/Article/details/gqvkcpqno.sHtML

[Q70] 更新统计信息
来源：http://blog.fehbvm.com/Article/details/guixnhwgs.sHtML

ANALYZE TABLE users;
来源：http://www.share.hesvh.cn/Article/details/gqnwpqgln.sHtML

[Q71] 查看建表语句
来源：http://read.share.zdbjq.cn/Article/details/gmhlmhoaz.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.hesvh.cn/Article/details/gkqcundij.sHtML

[Q72] 查看索引
来源：http://baike.hesvh.cn/Article/details/grqxsxwxl.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gvlvizuhe.sHtML

[Q73] 查看表状态
来源：http://wap.hesvh.cn/Article/details/geihvbbpk.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.hesvh.cn/Article/details/gtrqaxbjw.sHtML

[Q74] 强制使用索引
来源：http://baike.zdbjq.cn/Article/details/gvjurhldc.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.zdbjq.cn/Article/details/glybatxjf.sHtML

[Q75] 日期格式化
来源：http://www.m.share.fehbvm.com/Article/details/gopgewonc.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/ghdqscwhw.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.hesvh.cn/Article/details/gwhafxajg.sHtML


<!-- 参考信息 -->