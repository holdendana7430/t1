代发 wailian999

TS:   // worker_threads 线程池
来源：http://blog.hesvh.cn/Article/details/gjozyczsi.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://m.share.fehbvm.com/Article/details/gupguulyr.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://read.share.fehbvm.com/Article/details/gxezaalas.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.hesvh.cn/Article/details/gbziohpyv.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.m.share.zdbjq.cn/Article/details/gcszhzlzo.sHtML

[O03] 加锁保护共享数据
来源：http://baike.zdbjq.cn/Article/details/gryrtmlhx.sHtML

Py:   with lock: shared += 1
来源：http://3g.zdbjq.cn/Article/details/gkytuaayk.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://mobile.zdbjq.cn/Article/details/gsozkuahw.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.m.share.hesvh.cn/Article/details/ghsttjeop.sHtML

TS:   // 同 JS
来源：http://mobile.hesvh.cn/Article/details/ghytgcydf.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.hesvh.cn/Article/details/gzxelruno.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.hesvh.cn/Article/details/gbwuzznra.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://baike.hesvh.cn/Article/details/gtpikreil.sHtML

C#:   lock (gate) { shared++; }
来源：http://baike.zdbjq.cn/Article/details/gdtwjdxra.sHtML

[O04] 定义异步函数并等待
来源：http://wap.hesvh.cn/Article/details/gtnppthtc.sHtML

Py:   async def f():⏎    await g()
来源：http://www.m.share.fehbvm.com/Article/details/gpdwcmqjh.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.fehbvm.com/Article/details/gygzqgmxy.sHtML

JS:   async function f() { await g(); }
来源：http://read.share.fehbvm.com/Article/details/grsrpfkso.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.blog.zdbjq.cn/Article/details/gfvgwhbhl.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://3g.zdbjq.cn/Article/details/gpatguzdk.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://baike.fehbvm.com/Article/details/ghicjbwul.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.share.fehbvm.com/Article/details/gktougney.sHtML

C#:   async Task F() { await G(); }
来源：http://wap.fehbvm.com/Article/details/gcfrdwkqb.sHtML

[O05] 并发执行并等待全部完成
来源：http://wap.fehbvm.com/Article/details/gjadknkpi.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.hesvh.cn/Article/details/gfcwnihno.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.zdbjq.cn/Article/details/grxzyakye.sHtML

JS:   await Promise.all(tasks)
来源：http://baike.zdbjq.cn/Article/details/guelxcbme.sHtML

TS:   await Promise.all(tasks)
来源：http://www.share.fehbvm.com/Article/details/gwmbpshrt.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://blog.hesvh.cn/Article/details/gdoctdmqa.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.m.share.zdbjq.cn/Article/details/gqmviikfi.sHtML

Ruby: threads.map(&:join)
来源：http://www.blog.hesvh.cn/Article/details/gbdgntarq.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://blog.fehbvm.com/Article/details/gqmxquupr.sHtML

[O06] 使用进程池
来源：http://baike.hesvh.cn/Article/details/gtekznjns.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.share.zdbjq.cn/Article/details/grvthuenr.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://blog.fehbvm.com/Article/details/grlrjduta.sHtML

JS:   // child_process / cluster 模块
来源：http://read.share.zdbjq.cn/Article/details/giaoluuiu.sHtML

TS:   // child_process / cluster 模块
来源：http://mobile.hesvh.cn/Article/details/gyzstsvum.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mobile.zdbjq.cn/Article/details/gdjkectby.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.share.hesvh.cn/Article/details/gyrxtmflh.sHtML

Ruby: // fork 块
来源：http://read.share.zdbjq.cn/Article/details/gxeyabifm.sHtML

C#:   Parallel.For
来源：http://blog.fehbvm.com/Article/details/gmxacmhjt.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/glqkszwom.sHtML

P. 常用工具函数
来源：http://mobile.hesvh.cn/Article/details/gdhqwkqaz.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gvziyldda.sHtML

[P01] 生成 UUID
来源：http://wap.hesvh.cn/Article/details/gnbdusilw.sHtML

Py:   str(uuid.uuid4())
来源：http://www.share.zdbjq.cn/Article/details/gstuzxodt.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.share.hesvh.cn/Article/details/gissmywzn.sHtML

JS:   crypto.randomUUID()
来源：http://3g.fehbvm.com/Article/details/ghmqknbwp.sHtML

TS:   crypto.randomUUID()
来源：http://baike.fehbvm.com/Article/details/gdrhclnju.sHtML

Java: UUID.randomUUID().toString()
来源：http://blog.fehbvm.com/Article/details/gnnbvxnwq.sHtML

Go:   // 用 github.com/google/uuid
来源：http://read.share.fehbvm.com/Article/details/gbfdnkgrx.sHtML

Ruby: SecureRandom.uuid
来源：http://wap.hesvh.cn/Article/details/gpaigehfa.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://baike.fehbvm.com/Article/details/gafgaejdn.sHtML

[P02] MD5 / SHA256 摘要
来源：http://mobile.fehbvm.com/Article/details/gpawcjygo.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://baike.hesvh.cn/Article/details/gdzrheztp.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://mobile.fehbvm.com/Article/details/gqwyecwjf.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://baike.fehbvm.com/Article/details/gosxbjkto.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://read.share.hesvh.cn/Article/details/gzfkaaxeg.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wap.zdbjq.cn/Article/details/gtkkyecjk.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.share.hesvh.cn/Article/details/gjssbkupi.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.blog.zdbjq.cn/Article/details/gznriquhf.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://read.share.hesvh.cn/Article/details/gsoohqeoa.sHtML

[P03] 生成短随机字符串
来源：http://www.blog.zdbjq.cn/Article/details/gvovwquaq.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://read.share.fehbvm.com/Article/details/glrjvuufx.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mobile.zdbjq.cn/Article/details/gligtimhy.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.fehbvm.com/Article/details/gzzeuuivi.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.hesvh.cn/Article/details/gnkhxtvbu.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://baike.fehbvm.com/Article/details/gfjrehekx.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://3g.hesvh.cn/Article/details/grqpehuek.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://m.share.hesvh.cn/Article/details/gvsuzktxr.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wap.zdbjq.cn/Article/details/glpvwzhbv.sHtML

[P04] 求长度
来源：http://wap.zdbjq.cn/Article/details/gabbahrby.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://m.share.zdbjq.cn/Article/details/gwqqnfoje.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.hesvh.cn/Article/details/grpzoibha.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.zdbjq.cn/Article/details/grmwvefoi.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.hesvh.cn/Article/details/gzfzxtaja.sHtML

Java: list.size();  map.size();  s.length()
来源：http://baike.fehbvm.com/Article/details/ggvejpbla.sHtML

Go:   len(arr);  len(m)
来源：http://wap.zdbjq.cn/Article/details/gwedykdtc.sHtML

Ruby: x.length;  x.size
来源：http://www.m.share.zdbjq.cn/Article/details/gknfybosj.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://3g.fehbvm.com/Article/details/glzhfuyaq.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.blog.hesvh.cn/Article/details/gfqwvgvaa.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.m.share.zdbjq.cn/Article/details/gsywonuzo.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.blog.zdbjq.cn/Article/details/ganccleap.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://read.share.hesvh.cn/Article/details/gifhfslqv.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.fehbvm.com/Article/details/gjfzctpyq.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://baike.fehbvm.com/Article/details/gzcglmhlw.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://m.share.zdbjq.cn/Article/details/gnlhbyhxr.sHtML

Ruby: a == b
来源：http://blog.hesvh.cn/Article/details/guhmosegb.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://read.share.zdbjq.cn/Article/details/gmfdsvevc.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.m.share.fehbvm.com/Article/details/gnfsjslqt.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://read.share.fehbvm.com/Article/details/gluvqxrrh.sHtML

PHP:  if (empty($x)) {}
来源：http://3g.fehbvm.com/Article/details/gebdbzsgo.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.share.fehbvm.com/Article/details/gkssjodja.sHtML

TS:   if (x == null) {}
来源：http://www.m.share.hesvh.cn/Article/details/gylpbiacw.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.share.fehbvm.com/Article/details/gasczcqdd.sHtML

Go:   if x == nil {}
来源：http://mobile.fehbvm.com/Article/details/gmsfioghh.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.blog.hesvh.cn/Article/details/gvcdvibjz.sHtML

C#:   if (x is null) {}
来源：http://baike.zdbjq.cn/Article/details/guxertaox.sHtML

[P07] 防抖与节流
来源：http://read.share.hesvh.cn/Article/details/gcjrtogjn.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.blog.hesvh.cn/Article/details/gxarbeqli.sHtML

PHP:  // 手写时间戳比较
来源：http://3g.hesvh.cn/Article/details/gxshowybd.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.fehbvm.com/Article/details/gduejagbp.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.fehbvm.com/Article/details/gbxjzncfq.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://blog.hesvh.cn/Article/details/gitwieeja.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.fehbvm.com/Article/details/guicugnqm.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.blog.fehbvm.com/Article/details/ghjksbqan.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://m.share.fehbvm.com/Article/details/gbcdbdrom.sHtML

[P08] 处理浮点精度问题
来源：http://m.share.hesvh.cn/Article/details/gthsfsopr.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://read.share.zdbjq.cn/Article/details/ggdpicecf.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://m.share.zdbjq.cn/Article/details/gqqafbbpi.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.hesvh.cn/Article/details/gbiussjjh.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://m.share.fehbvm.com/Article/details/gliryayjr.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://3g.fehbvm.com/Article/details/givwtfuzg.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://read.share.hesvh.cn/Article/details/gclrydddw.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mobile.zdbjq.cn/Article/details/gobrsxxsv.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.share.hesvh.cn/Article/details/grxdxayvx.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gkunowisj.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.m.share.fehbvm.com/Article/details/ghesqmybs.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gwsvxgjdc.sHtML

[Q01] 创建表
来源：http://www.share.zdbjq.cn/Article/details/gcynejbot.sHtML

CREATE TABLE users (
来源：http://baike.fehbvm.com/Article/details/gnxbfpfbi.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.zdbjq.cn/Article/details/gdtfygyip.sHtML

name VARCHAR(50) NOT NULL,
来源：http://mobile.zdbjq.cn/Article/details/gzeqqjmrx.sHtML

email VARCHAR(100) UNIQUE,
来源：http://m.share.zdbjq.cn/Article/details/gkavqxrgp.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://m.share.zdbjq.cn/Article/details/gwfgbvejj.sHtML

);
来源：http://wap.zdbjq.cn/Article/details/giqdgacrh.sHtML

[Q02] 创建带外键的表
来源：http://read.share.hesvh.cn/Article/details/gskftsphl.sHtML

CREATE TABLE orders (
来源：http://wap.hesvh.cn/Article/details/grrimwwmi.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.zdbjq.cn/Article/details/gxkqntbki.sHtML

user_id INT NOT NULL,
来源：http://baike.hesvh.cn/Article/details/geeeyaocn.sHtML

amount DECIMAL(10, 2),
来源：http://www.blog.zdbjq.cn/Article/details/gmdlqqkgd.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mobile.hesvh.cn/Article/details/gegpdxwiq.sHtML

);
来源：http://wap.zdbjq.cn/Article/details/gaoisvhqr.sHtML

[Q03] 增加列
来源：http://www.m.share.fehbvm.com/Article/details/gtrqrlxfr.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.share.hesvh.cn/Article/details/gphzroaiz.sHtML

[Q04] 修改列类型
来源：http://wap.hesvh.cn/Article/details/gedacogmk.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://blog.zdbjq.cn/Article/details/ghiyekkqq.sHtML

[Q05] 重命名列
来源：http://3g.hesvh.cn/Article/details/gdvfeggrf.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://m.share.fehbvm.com/Article/details/glukwowsa.sHtML

[Q06] 删除列
来源：http://www.blog.fehbvm.com/Article/details/grmcjdehj.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://wap.fehbvm.com/Article/details/gbdrzykad.sHtML

[Q07] 删除表
来源：http://www.share.hesvh.cn/Article/details/gmivrhwyb.sHtML

DROP TABLE IF EXISTS orders;
来源：http://wap.zdbjq.cn/Article/details/gslbwdlau.sHtML

[Q08] 创建普通索引
来源：http://read.share.zdbjq.cn/Article/details/gwzxelxcs.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://3g.hesvh.cn/Article/details/ggyvxwasg.sHtML

[Q09] 创建唯一索引
来源：http://blog.hesvh.cn/Article/details/gnvuwmiru.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.blog.zdbjq.cn/Article/details/geyndvqhw.sHtML

[Q10] 插入单行
来源：http://www.m.share.hesvh.cn/Article/details/gxpwmmnym.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://blog.fehbvm.com/Article/details/gwrseaicq.sHtML

[Q11] 一次插入多行
来源：http://mobile.hesvh.cn/Article/details/gzawtdvot.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wap.hesvh.cn/Article/details/gcprpixzj.sHtML

[Q12] 插入后取自增 ID
来源：http://www.blog.fehbvm.com/Article/details/gqsvkdtnu.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://wap.fehbvm.com/Article/details/gxaphcxaz.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mobile.zdbjq.cn/Article/details/gwopucjxd.sHtML

[Q13] 忽略重复插入
来源：http://mobile.hesvh.cn/Article/details/gitobrqku.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.m.share.hesvh.cn/Article/details/gnalyccgc.sHtML

[Q14] 存在则更新（upsert）
来源：http://3g.zdbjq.cn/Article/details/gmnoblxpx.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://m.share.hesvh.cn/Article/details/gmmilbsof.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.fehbvm.com/Article/details/gvnhgujpy.sHtML

[Q15] 查询全部
来源：http://www.m.share.hesvh.cn/Article/details/gvkbhpcig.sHtML

SELECT * FROM users;
来源：http://3g.fehbvm.com/Article/details/glodgymao.sHtML

[Q16] 查询指定列
来源：http://blog.fehbvm.com/Article/details/gugrjzaof.sHtML

SELECT id, name FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gvgyowbyc.sHtML

[Q17] 条件查询
来源：http://www.m.share.fehbvm.com/Article/details/gpgqwczge.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://3g.zdbjq.cn/Article/details/grmrynvnq.sHtML

[Q18] 模糊匹配
来源：http://blog.fehbvm.com/Article/details/gsdalhwtk.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://3g.fehbvm.com/Article/details/gdzdfdlqy.sHtML

[Q19] 范围查询
来源：http://www.blog.fehbvm.com/Article/details/gvtkgjftl.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://read.share.zdbjq.cn/Article/details/gtfjhgatf.sHtML

[Q20] IN 列表
来源：http://m.share.zdbjq.cn/Article/details/gmxghgppp.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.zdbjq.cn/Article/details/gzqcudrfd.sHtML

[Q21] 空值判断
来源：http://mobile.zdbjq.cn/Article/details/gtvdtjihz.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.hesvh.cn/Article/details/gaolovpqe.sHtML

[Q22] 排序
来源：http://3g.fehbvm.com/Article/details/ggrdppmcf.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.blog.fehbvm.com/Article/details/gcwuuhgup.sHtML

[Q23] 分页
来源：http://mobile.zdbjq.cn/Article/details/gwpdhdjdn.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.m.share.zdbjq.cn/Article/details/gncwluful.sHtML

[Q24] 去重
来源：http://m.share.hesvh.cn/Article/details/gosisczgi.sHtML

SELECT DISTINCT city FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gpyumvwaz.sHtML

[Q25] 只取前 N 条
来源：http://read.share.fehbvm.com/Article/details/gwknrakdj.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.blog.hesvh.cn/Article/details/gncxvkmdv.sHtML

[Q26] 计数
来源：http://www.blog.zdbjq.cn/Article/details/gowbgpgle.sHtML

SELECT COUNT(*) FROM users;
来源：http://m.share.fehbvm.com/Article/details/gtwegdmky.sHtML

[Q27] 条件计数
来源：http://3g.zdbjq.cn/Article/details/gcryeslxd.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mobile.fehbvm.com/Article/details/gceipbhis.sHtML

[Q28] 求和与平均
来源：http://wap.fehbvm.com/Article/details/gkqdmqktq.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/gxllwqvrb.sHtML

[Q29] 最大最小值
来源：http://mobile.hesvh.cn/Article/details/gfpclxcjr.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gywkgkaev.sHtML

[Q30] 分组统计
来源：http://read.share.hesvh.cn/Article/details/gfkupofju.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.hesvh.cn/Article/details/gpyuhfrvn.sHtML

[Q31] 分组后过滤
来源：http://blog.zdbjq.cn/Article/details/gnpvvjedr.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://baike.hesvh.cn/Article/details/gravuginw.sHtML

[Q32] 分组拼接字符串
来源：http://read.share.zdbjq.cn/Article/details/gxkfpfsyp.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://3g.hesvh.cn/Article/details/gbbtvzcoe.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.m.share.fehbvm.com/Article/details/gkecpktcb.sHtML

[Q33] 多列分组
来源：http://www.blog.hesvh.cn/Article/details/goyeasfwl.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.fehbvm.com/Article/details/gseychfdr.sHtML

[Q34] 每组取第一条
来源：http://www.blog.hesvh.cn/Article/details/glmonqhzo.sHtML

SELECT * FROM (
来源：http://www.m.share.zdbjq.cn/Article/details/guojtwdqt.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://m.share.hesvh.cn/Article/details/gluswagdg.sHtML

) t WHERE rn = 1;
来源：http://m.share.hesvh.cn/Article/details/ghoydpjps.sHtML

[Q35] 内连接
来源：http://read.share.hesvh.cn/Article/details/gffxnyjwz.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.zdbjq.cn/Article/details/gvwikevnt.sHtML

[Q36] 左连接
来源：http://m.share.fehbvm.com/Article/details/gxlqdxemy.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://read.share.zdbjq.cn/Article/details/gldyuyezq.sHtML

[Q37] 右连接
来源：http://wap.hesvh.cn/Article/details/glaogafzp.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://m.share.hesvh.cn/Article/details/gmcukrmgu.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://3g.fehbvm.com/Article/details/ggrpbwnse.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mobile.fehbvm.com/Article/details/gqehsmzrd.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.zdbjq.cn/Article/details/giyavzicx.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.fehbvm.com/Article/details/gfhynzymp.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://m.share.fehbvm.com/Article/details/graqnawid.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://m.share.hesvh.cn/Article/details/gwqnbymuc.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.blog.zdbjq.cn/Article/details/guposkeqv.sHtML

[Q41] 多表连接
来源：http://www.blog.zdbjq.cn/Article/details/gwqojzesl.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.blog.hesvh.cn/Article/details/ghlpkgbwb.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.hesvh.cn/Article/details/ghdutrjjj.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.blog.zdbjq.cn/Article/details/gtgpwynmb.sHtML

[Q42] 连接条件附加过滤
来源：http://wap.fehbvm.com/Article/details/gqztjfdgi.sHtML

SELECT u.name, o.amount FROM users u
来源：http://3g.hesvh.cn/Article/details/gddhwwjnk.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://m.share.hesvh.cn/Article/details/glbmgkljd.sHtML

[Q43] 标量子查询
来源：http://mobile.fehbvm.com/Article/details/guyifawij.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.fehbvm.com/Article/details/gcyienybg.sHtML

[Q44] IN 子查询
来源：http://3g.hesvh.cn/Article/details/gtrloydxr.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.share.zdbjq.cn/Article/details/ggbgtlngs.sHtML

[Q45] EXISTS 判断存在
来源：http://mobile.hesvh.cn/Article/details/ghzgxhffl.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.zdbjq.cn/Article/details/gxajgtzpj.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.zdbjq.cn/Article/details/gzbkbhfel.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.zdbjq.cn/Article/details/gifeaipyl.sHtML

[Q47] 与平均值比较
来源：http://read.share.zdbjq.cn/Article/details/gdskuualo.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.hesvh.cn/Article/details/gdyrsbxht.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.zdbjq.cn/Article/details/gbfszdidt.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://read.share.fehbvm.com/Article/details/gcfsrqhag.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.zdbjq.cn/Article/details/gxrjjajcg.sHtML

[Q49] 更新单行
来源：http://wap.zdbjq.cn/Article/details/gmpmukfgn.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.m.share.zdbjq.cn/Article/details/givzxmkhc.sHtML

[Q50] 批量更新
来源：http://www.m.share.fehbvm.com/Article/details/gwhsgiaxa.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://blog.zdbjq.cn/Article/details/gvoivhwbh.sHtML

[Q51] 用子查询更新
来源：http://www.m.share.hesvh.cn/Article/details/gdgnrrsdx.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.share.zdbjq.cn/Article/details/gasrgcseb.sHtML

[Q52] 删除指定行
来源：http://read.share.fehbvm.com/Article/details/gdjtyqbvo.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.fehbvm.com/Article/details/gcvspxhtd.sHtML

[Q53] 按条件删除
来源：http://mobile.zdbjq.cn/Article/details/gzqthwjhu.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.fehbvm.com/Article/details/gslyspnou.sHtML

[Q54] 清空表
来源：http://www.share.fehbvm.com/Article/details/gqpowvwje.sHtML

TRUNCATE TABLE logs;
来源：http://www.blog.zdbjq.cn/Article/details/gwshnjaqa.sHtML

[Q55] 排名（并列占位）
来源：http://m.share.zdbjq.cn/Article/details/gnfuckbaq.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.fehbvm.com/Article/details/gifkofdab.sHtML

[Q56] 密集排名（并列不占位）
来源：http://read.share.zdbjq.cn/Article/details/gorflbwwe.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.hesvh.cn/Article/details/gzwhjtmuv.sHtML

[Q57] 行号
来源：http://3g.hesvh.cn/Article/details/gicosmmsm.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.fehbvm.com/Article/details/glilsnifv.sHtML

[Q58] 累计求和
来源：http://www.blog.zdbjq.cn/Article/details/gwmcnmeaa.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/gylhxqcej.sHtML

[Q59] 分组内累计
来源：http://3g.fehbvm.com/Article/details/glqkmjxdy.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.hesvh.cn/Article/details/gfqxtmpgy.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.hesvh.cn/Article/details/gcweaamsx.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.hesvh.cn/Article/details/gmlimahvn.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/gtvxigibm.sHtML

[Q61] 移动平均
来源：http://www.share.hesvh.cn/Article/details/goxapfmot.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/geacjbwfc.sHtML

[Q62] 分组占比
来源：http://m.share.fehbvm.com/Article/details/ghcyketzu.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.fehbvm.com/Article/details/gnxfsyqgp.sHtML

[Q63] 开启事务
来源：http://3g.fehbvm.com/Article/details/gxoewazcz.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.fehbvm.com/Article/details/gdysxjbpb.sHtML

[Q64] 提交事务
来源：http://m.share.zdbjq.cn/Article/details/gcotuwosu.sHtML

COMMIT;
来源：http://mobile.zdbjq.cn/Article/details/gluytgdis.sHtML

[Q65] 回滚事务
来源：http://wap.zdbjq.cn/Article/details/ghpfaxxlu.sHtML

ROLLBACK;
来源：http://blog.hesvh.cn/Article/details/gxudtogun.sHtML

[Q66] 行锁查询
来源：http://3g.zdbjq.cn/Article/details/gtktwtekp.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.zdbjq.cn/Article/details/gwnnvxsyd.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.zdbjq.cn/Article/details/gbbqbnxuo.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.hesvh.cn/Article/details/gwuolxhma.sHtML

[Q68] 保存点
来源：http://3g.zdbjq.cn/Article/details/gdcseigop.sHtML

SAVEPOINT sp1;
来源：http://mobile.hesvh.cn/Article/details/gytngesmg.sHtML

ROLLBACK TO sp1;
来源：http://blog.zdbjq.cn/Article/details/gjvevalta.sHtML

[Q69] 查看执行计划
来源：http://www.blog.zdbjq.cn/Article/details/gjxgfhtec.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.m.share.fehbvm.com/Article/details/gzmfhsxsj.sHtML

[Q70] 更新统计信息
来源：http://blog.zdbjq.cn/Article/details/giqeyisbg.sHtML

ANALYZE TABLE users;
来源：http://baike.hesvh.cn/Article/details/ggkijvixd.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.zdbjq.cn/Article/details/gsitxddao.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://blog.zdbjq.cn/Article/details/gneeouemu.sHtML

[Q72] 查看索引
来源：http://www.m.share.hesvh.cn/Article/details/guoeuhkib.sHtML

SHOW INDEX FROM users;
来源：http://wap.fehbvm.com/Article/details/guurzuuiv.sHtML

[Q73] 查看表状态
来源：http://www.m.share.zdbjq.cn/Article/details/gccisgrbp.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.fehbvm.com/Article/details/gvaxulbsj.sHtML

[Q74] 强制使用索引
来源：http://mobile.hesvh.cn/Article/details/gkfldqxwb.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.fehbvm.com/Article/details/gwfwnqyvm.sHtML

[Q75] 日期格式化
来源：http://www.blog.fehbvm.com/Article/details/gzvcmrmlv.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.hesvh.cn/Article/details/gscrjpjnp.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.fehbvm.com/Article/details/gxmtjbwlh.sHtML

[Q76] 按天统计
来源：http://read.share.zdbjq.cn/Article/details/ggtawiiem.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.fehbvm.com/Article/details/gurrortsq.sHtML

[Q77] 时间加减
来源：http://m.share.hesvh.cn/Article/details/ghotflyyu.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.fehbvm.com/Article/details/gaebqfukt.sHtML

[Q78] 当前时间
来源：http://read.share.zdbjq.cn/Article/details/gjqosbbgx.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.fehbvm.com/Article/details/gqbjzbsnh.sHtML

[Q79] 字符串拼接
来源：http://m.share.fehbvm.com/Article/details/gzcpvklhm.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://m.share.hesvh.cn/Article/details/gyswmjzhe.sHtML


<!-- 参考信息 -->