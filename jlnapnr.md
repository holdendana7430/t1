代发 wailian999

[O02] 使用线程池
来源：http://3g.zdbjq.cn/Article/details/gwwhrkuql.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.hesvh.cn/Article/details/ggquwznoc.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mobile.zdbjq.cn/Article/details/gjhybxkpl.sHtML

JS:   // worker_threads 线程池
来源：http://baike.zdbjq.cn/Article/details/gwpdpkfzp.sHtML

TS:   // worker_threads 线程池
来源：http://baike.hesvh.cn/Article/details/gkktikjbj.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://blog.hesvh.cn/Article/details/gekjyfnsx.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://read.share.fehbvm.com/Article/details/gnaqljbyf.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.zdbjq.cn/Article/details/gmzdnwcdh.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://baike.hesvh.cn/Article/details/gigfbrdjh.sHtML

[O03] 加锁保护共享数据
来源：http://blog.fehbvm.com/Article/details/gvkpnvtcw.sHtML

Py:   with lock: shared += 1
来源：http://www.share.hesvh.cn/Article/details/gcqoiskxx.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.zdbjq.cn/Article/details/givqbbuti.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.share.fehbvm.com/Article/details/gojhplcdj.sHtML

TS:   // 同 JS
来源：http://www.m.share.zdbjq.cn/Article/details/guznpjkvy.sHtML

Java: synchronized (this) { shared++; }
来源：http://3g.zdbjq.cn/Article/details/gytyzutyo.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://blog.fehbvm.com/Article/details/gdhpfonzj.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://baike.zdbjq.cn/Article/details/gpmseyzxq.sHtML

C#:   lock (gate) { shared++; }
来源：http://wap.hesvh.cn/Article/details/gmnxdsqtu.sHtML

[O04] 定义异步函数并等待
来源：http://www.share.fehbvm.com/Article/details/ghqupwojt.sHtML

Py:   async def f():⏎    await g()
来源：http://www.m.share.fehbvm.com/Article/details/gthrfhhoh.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.blog.fehbvm.com/Article/details/gxnsmntdn.sHtML

JS:   async function f() { await g(); }
来源：http://m.share.fehbvm.com/Article/details/gjdkusnur.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://mobile.zdbjq.cn/Article/details/gvqcryvpi.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.zdbjq.cn/Article/details/gnxwtrilh.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://3g.zdbjq.cn/Article/details/gsjnhyyyz.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.hesvh.cn/Article/details/gralygozu.sHtML

C#:   async Task F() { await G(); }
来源：http://www.m.share.hesvh.cn/Article/details/gaaobgsfz.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.share.hesvh.cn/Article/details/gjcqvtifr.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.share.zdbjq.cn/Article/details/gxqxufyay.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://3g.zdbjq.cn/Article/details/gvnclonzy.sHtML

JS:   await Promise.all(tasks)
来源：http://www.blog.zdbjq.cn/Article/details/gjtahgcio.sHtML

TS:   await Promise.all(tasks)
来源：http://3g.zdbjq.cn/Article/details/gfdunetcj.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.blog.zdbjq.cn/Article/details/ghonvfbwn.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.share.hesvh.cn/Article/details/gvtyrayou.sHtML

Ruby: threads.map(&:join)
来源：http://baike.fehbvm.com/Article/details/gbrblyfcy.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://blog.hesvh.cn/Article/details/ggnbkoiip.sHtML

[O06] 使用进程池
来源：http://3g.hesvh.cn/Article/details/gkyiveqzw.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://3g.fehbvm.com/Article/details/gmbkapxky.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://mobile.zdbjq.cn/Article/details/gnkfxbgib.sHtML

JS:   // child_process / cluster 模块
来源：http://baike.fehbvm.com/Article/details/gcjrbgisw.sHtML

TS:   // child_process / cluster 模块
来源：http://baike.fehbvm.com/Article/details/gqsizddhu.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://blog.zdbjq.cn/Article/details/gphektpei.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://3g.fehbvm.com/Article/details/gdvajiplk.sHtML

Ruby: // fork 块
来源：http://3g.hesvh.cn/Article/details/gpihjrsfy.sHtML

C#:   Parallel.For
来源：http://www.blog.hesvh.cn/Article/details/glmadurwk.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gvbvunvko.sHtML

P. 常用工具函数
来源：http://read.share.zdbjq.cn/Article/details/gublcwoxs.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gvllqxpzh.sHtML

[P01] 生成 UUID
来源：http://www.share.hesvh.cn/Article/details/ghetrjxsk.sHtML

Py:   str(uuid.uuid4())
来源：http://mobile.fehbvm.com/Article/details/gfokblbrm.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mobile.hesvh.cn/Article/details/gtkirkznf.sHtML

JS:   crypto.randomUUID()
来源：http://mobile.hesvh.cn/Article/details/gvljjukei.sHtML

TS:   crypto.randomUUID()
来源：http://www.m.share.fehbvm.com/Article/details/gzzsbcbsz.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.m.share.zdbjq.cn/Article/details/ghikxukvn.sHtML

Go:   // 用 github.com/google/uuid
来源：http://blog.hesvh.cn/Article/details/gnvokzhsn.sHtML

Ruby: SecureRandom.uuid
来源：http://www.m.share.fehbvm.com/Article/details/gbaorogsh.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.blog.zdbjq.cn/Article/details/gwucidqod.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.m.share.zdbjq.cn/Article/details/goqgkwhnr.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://read.share.fehbvm.com/Article/details/gaztdmuxa.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://3g.fehbvm.com/Article/details/gnahbzpoi.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://blog.fehbvm.com/Article/details/gwufbhbtz.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://blog.hesvh.cn/Article/details/ggsupuvyn.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.blog.hesvh.cn/Article/details/gwpnovcjr.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mobile.zdbjq.cn/Article/details/gmqmslpdh.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://read.share.hesvh.cn/Article/details/gittcuxfk.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.blog.zdbjq.cn/Article/details/gtukaodew.sHtML

[P03] 生成短随机字符串
来源：http://www.blog.hesvh.cn/Article/details/gmoljgrur.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mobile.zdbjq.cn/Article/details/gpwbbywzl.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wap.zdbjq.cn/Article/details/gqbmvhjig.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.zdbjq.cn/Article/details/gtidigvpv.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.fehbvm.com/Article/details/gdimuskqo.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.share.fehbvm.com/Article/details/gpthuoybq.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://m.share.fehbvm.com/Article/details/gakbaqtwe.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.share.fehbvm.com/Article/details/gshwqcfwo.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.blog.hesvh.cn/Article/details/gjdqmfnoa.sHtML

[P04] 求长度
来源：http://mobile.fehbvm.com/Article/details/gnfspzaue.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://m.share.fehbvm.com/Article/details/gpsbxpsfv.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.fehbvm.com/Article/details/gjvktoabt.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.zdbjq.cn/Article/details/ginqkwfyn.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.fehbvm.com/Article/details/gkvvwbzzz.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.m.share.fehbvm.com/Article/details/guhkxxqpb.sHtML

Go:   len(arr);  len(m)
来源：http://www.m.share.fehbvm.com/Article/details/gairkxsvx.sHtML

Ruby: x.length;  x.size
来源：http://mobile.zdbjq.cn/Article/details/gnozuwqhx.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://m.share.hesvh.cn/Article/details/gclkdvrxn.sHtML

[P05] 判断两个对象内容是否相等
来源：http://m.share.fehbvm.com/Article/details/gfyaeinsc.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://wap.hesvh.cn/Article/details/gnqgckczr.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://baike.fehbvm.com/Article/details/gssyliqgf.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://m.share.hesvh.cn/Article/details/gebrevoqr.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.hesvh.cn/Article/details/gspwkivrb.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mobile.hesvh.cn/Article/details/gphdbirvw.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://3g.hesvh.cn/Article/details/gunfcbfql.sHtML

Ruby: a == b
来源：http://3g.hesvh.cn/Article/details/gjusbjeov.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.m.share.zdbjq.cn/Article/details/gmmffitkd.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://read.share.fehbvm.com/Article/details/ghvupchpc.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mobile.hesvh.cn/Article/details/golegpgub.sHtML

PHP:  if (empty($x)) {}
来源：http://mobile.hesvh.cn/Article/details/gmuaubqrv.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.m.share.hesvh.cn/Article/details/gysodpdxl.sHtML

TS:   if (x == null) {}
来源：http://wap.zdbjq.cn/Article/details/gahvduqra.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.m.share.zdbjq.cn/Article/details/ghnqtlcxe.sHtML

Go:   if x == nil {}
来源：http://read.share.hesvh.cn/Article/details/giazjnddy.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://m.share.fehbvm.com/Article/details/gpvqttgyn.sHtML

C#:   if (x is null) {}
来源：http://3g.zdbjq.cn/Article/details/gkfqdxevi.sHtML

[P07] 防抖与节流
来源：http://3g.fehbvm.com/Article/details/gvpzvcgdk.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.blog.zdbjq.cn/Article/details/ggumrezla.sHtML

PHP:  // 手写时间戳比较
来源：http://www.blog.zdbjq.cn/Article/details/gbvhrakbr.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.hesvh.cn/Article/details/gugcesise.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.zdbjq.cn/Article/details/gtwpptote.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://blog.hesvh.cn/Article/details/ghutoeqqd.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://read.share.zdbjq.cn/Article/details/gxwvvxttl.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.zdbjq.cn/Article/details/gihqprgiv.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.share.fehbvm.com/Article/details/gkvvlmywm.sHtML

[P08] 处理浮点精度问题
来源：http://blog.hesvh.cn/Article/details/gbvobvdze.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://m.share.fehbvm.com/Article/details/gybrifmrm.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://blog.fehbvm.com/Article/details/gblalvndg.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wap.zdbjq.cn/Article/details/gpwifzcgk.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mobile.hesvh.cn/Article/details/gihmxodbl.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://m.share.fehbvm.com/Article/details/gjenkedpt.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.share.hesvh.cn/Article/details/gnpuxdygz.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.share.zdbjq.cn/Article/details/gpglvdmob.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://3g.zdbjq.cn/Article/details/gnoyvwzpz.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/ghqfezojf.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.blog.hesvh.cn/Article/details/grctsuiuv.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/graphkqht.sHtML

[Q01] 创建表
来源：http://read.share.zdbjq.cn/Article/details/gqdmdgykx.sHtML

CREATE TABLE users (
来源：http://read.share.fehbvm.com/Article/details/gpiovqzvf.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.zdbjq.cn/Article/details/gvnpzokou.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.share.fehbvm.com/Article/details/gzabdwxjl.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.m.share.zdbjq.cn/Article/details/gbyjczobd.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.share.zdbjq.cn/Article/details/gsyvqgsjw.sHtML

);
来源：http://m.share.hesvh.cn/Article/details/gqnqvquch.sHtML

[Q02] 创建带外键的表
来源：http://www.blog.hesvh.cn/Article/details/gijbzvmzt.sHtML

CREATE TABLE orders (
来源：http://baike.fehbvm.com/Article/details/gwbdeodop.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.zdbjq.cn/Article/details/gfrkzsakq.sHtML

user_id INT NOT NULL,
来源：http://mobile.fehbvm.com/Article/details/guqlliqfa.sHtML

amount DECIMAL(10, 2),
来源：http://www.blog.hesvh.cn/Article/details/gioxichot.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.share.fehbvm.com/Article/details/gbdmiusky.sHtML

);
来源：http://blog.zdbjq.cn/Article/details/gufqvpryf.sHtML

[Q03] 增加列
来源：http://www.share.hesvh.cn/Article/details/gtuaiuieb.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.blog.zdbjq.cn/Article/details/gqwnremyv.sHtML

[Q04] 修改列类型
来源：http://blog.zdbjq.cn/Article/details/gmfhhawir.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://baike.fehbvm.com/Article/details/gbkjvsein.sHtML

[Q05] 重命名列
来源：http://3g.hesvh.cn/Article/details/gffmjykce.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.blog.hesvh.cn/Article/details/giylkitfu.sHtML

[Q06] 删除列
来源：http://mobile.hesvh.cn/Article/details/gcwnilldq.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.m.share.hesvh.cn/Article/details/gjscaiuys.sHtML

[Q07] 删除表
来源：http://wap.fehbvm.com/Article/details/gyglcupvh.sHtML

DROP TABLE IF EXISTS orders;
来源：http://baike.zdbjq.cn/Article/details/gdwgghrge.sHtML

[Q08] 创建普通索引
来源：http://www.blog.hesvh.cn/Article/details/grgmmxhov.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.m.share.zdbjq.cn/Article/details/gcasdpqvk.sHtML

[Q09] 创建唯一索引
来源：http://blog.fehbvm.com/Article/details/ggidgqyzl.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://baike.fehbvm.com/Article/details/gontsbpoe.sHtML

[Q10] 插入单行
来源：http://mobile.fehbvm.com/Article/details/gifmzbczi.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wap.hesvh.cn/Article/details/ghwukcgbq.sHtML

[Q11] 一次插入多行
来源：http://mobile.zdbjq.cn/Article/details/gnrghhabu.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.m.share.fehbvm.com/Article/details/giyxbofmq.sHtML

[Q12] 插入后取自增 ID
来源：http://www.share.hesvh.cn/Article/details/gcawgmkpc.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://wap.fehbvm.com/Article/details/ggdsgpynh.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.m.share.zdbjq.cn/Article/details/gavxmttcd.sHtML

[Q13] 忽略重复插入
来源：http://mobile.fehbvm.com/Article/details/geefonobb.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://baike.zdbjq.cn/Article/details/gosiaiebq.sHtML

[Q14] 存在则更新（upsert）
来源：http://wap.hesvh.cn/Article/details/gjsjyuxrr.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://3g.fehbvm.com/Article/details/gzfkqlpgd.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://blog.fehbvm.com/Article/details/gjhvaxocj.sHtML

[Q15] 查询全部
来源：http://www.share.fehbvm.com/Article/details/gywbcykzf.sHtML

SELECT * FROM users;
来源：http://mobile.fehbvm.com/Article/details/ghfvdkgqg.sHtML

[Q16] 查询指定列
来源：http://baike.zdbjq.cn/Article/details/ggxspcswt.sHtML

SELECT id, name FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gcpgcuvov.sHtML

[Q17] 条件查询
来源：http://blog.fehbvm.com/Article/details/gpztoqrpt.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://blog.zdbjq.cn/Article/details/gralvcfgt.sHtML

[Q18] 模糊匹配
来源：http://read.share.zdbjq.cn/Article/details/gbanxjkpj.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://m.share.fehbvm.com/Article/details/gbozrbkyy.sHtML

[Q19] 范围查询
来源：http://www.blog.zdbjq.cn/Article/details/gaaepylfl.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://read.share.fehbvm.com/Article/details/gimxuofgw.sHtML

[Q20] IN 列表
来源：http://www.m.share.hesvh.cn/Article/details/gpggjdsjh.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.zdbjq.cn/Article/details/gbegnyegs.sHtML

[Q21] 空值判断
来源：http://blog.zdbjq.cn/Article/details/gfotmszwi.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://mobile.zdbjq.cn/Article/details/gbibsurdy.sHtML

[Q22] 排序
来源：http://m.share.zdbjq.cn/Article/details/gtwpooshd.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://3g.fehbvm.com/Article/details/ggqrqkrga.sHtML

[Q23] 分页
来源：http://read.share.hesvh.cn/Article/details/gmmiukgkp.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://m.share.hesvh.cn/Article/details/goxbjydka.sHtML

[Q24] 去重
来源：http://read.share.zdbjq.cn/Article/details/glmitrast.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.share.fehbvm.com/Article/details/gqyytijhf.sHtML

[Q25] 只取前 N 条
来源：http://www.m.share.zdbjq.cn/Article/details/gvqesoyrf.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://blog.zdbjq.cn/Article/details/gdauthiqc.sHtML

[Q26] 计数
来源：http://blog.zdbjq.cn/Article/details/gxlewxmbf.sHtML

SELECT COUNT(*) FROM users;
来源：http://blog.hesvh.cn/Article/details/gqxldzueh.sHtML

[Q27] 条件计数
来源：http://m.share.fehbvm.com/Article/details/glvpmerde.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://baike.fehbvm.com/Article/details/glepienkw.sHtML

[Q28] 求和与平均
来源：http://www.m.share.fehbvm.com/Article/details/gvoscfjzf.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://read.share.fehbvm.com/Article/details/gcexpupyy.sHtML

[Q29] 最大最小值
来源：http://mobile.hesvh.cn/Article/details/ggpfoxzfg.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.fehbvm.com/Article/details/gpyyutmfv.sHtML

[Q30] 分组统计
来源：http://3g.fehbvm.com/Article/details/gcabwscgu.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mobile.fehbvm.com/Article/details/gchielmlx.sHtML

[Q31] 分组后过滤
来源：http://wap.zdbjq.cn/Article/details/gujpfszcg.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.hesvh.cn/Article/details/gddoxjfrk.sHtML

[Q32] 分组拼接字符串
来源：http://www.share.fehbvm.com/Article/details/grdeuaqvu.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.blog.zdbjq.cn/Article/details/gytyjjuhi.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.share.fehbvm.com/Article/details/gyhjoynql.sHtML

[Q33] 多列分组
来源：http://www.m.share.fehbvm.com/Article/details/ghwlorrin.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://blog.zdbjq.cn/Article/details/gkisjnfrh.sHtML

[Q34] 每组取第一条
来源：http://www.m.share.hesvh.cn/Article/details/ghauyunmq.sHtML

SELECT * FROM (
来源：http://www.m.share.fehbvm.com/Article/details/guayefzqa.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.share.hesvh.cn/Article/details/gchmrzzke.sHtML

) t WHERE rn = 1;
来源：http://baike.zdbjq.cn/Article/details/gtyavigmi.sHtML

[Q35] 内连接
来源：http://m.share.zdbjq.cn/Article/details/geefbcesg.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.zdbjq.cn/Article/details/gsvvaxave.sHtML

[Q36] 左连接
来源：http://blog.hesvh.cn/Article/details/gxnryhayr.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.fehbvm.com/Article/details/gezfjkzxu.sHtML

[Q37] 右连接
来源：http://www.blog.fehbvm.com/Article/details/gichonplb.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.fehbvm.com/Article/details/gnlduyvgh.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://wap.zdbjq.cn/Article/details/gulpflmod.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.hesvh.cn/Article/details/gmqenauzh.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.hesvh.cn/Article/details/gnffliquv.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.fehbvm.com/Article/details/gnuhrgcbm.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://baike.zdbjq.cn/Article/details/gdmxdapob.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://baike.hesvh.cn/Article/details/gtjqqwxzb.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://baike.fehbvm.com/Article/details/gzcdnrixv.sHtML

[Q41] 多表连接
来源：http://baike.hesvh.cn/Article/details/gbidmpjgb.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.fehbvm.com/Article/details/ghfkrdbof.sHtML

JOIN users u ON u.id = o.user_id
来源：http://blog.hesvh.cn/Article/details/gfvatkjun.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.fehbvm.com/Article/details/glmdibqsh.sHtML

[Q42] 连接条件附加过滤
来源：http://wap.zdbjq.cn/Article/details/gpsjatgta.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.blog.fehbvm.com/Article/details/gwxvorlze.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.hesvh.cn/Article/details/gfzmauwzz.sHtML

[Q43] 标量子查询
来源：http://wap.hesvh.cn/Article/details/gwngngfxt.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wap.fehbvm.com/Article/details/gylmbqebu.sHtML

[Q44] IN 子查询
来源：http://read.share.zdbjq.cn/Article/details/gfuecrjdz.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://blog.hesvh.cn/Article/details/gcpgkakqh.sHtML

[Q45] EXISTS 判断存在
来源：http://3g.zdbjq.cn/Article/details/gywgusbxs.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.zdbjq.cn/Article/details/gmzzbdnml.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.share.zdbjq.cn/Article/details/gtygygkaj.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.hesvh.cn/Article/details/gsgkdbrvk.sHtML

[Q47] 与平均值比较
来源：http://www.m.share.zdbjq.cn/Article/details/gbrelxyjg.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.fehbvm.com/Article/details/gtxybhjen.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.zdbjq.cn/Article/details/gpxauizhq.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://3g.zdbjq.cn/Article/details/gdwubxyqm.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://3g.hesvh.cn/Article/details/gtpbienkt.sHtML

[Q49] 更新单行
来源：http://baike.zdbjq.cn/Article/details/gqqwftrqi.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mobile.hesvh.cn/Article/details/gisilwsib.sHtML

[Q50] 批量更新
来源：http://baike.zdbjq.cn/Article/details/gxfnuornl.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.share.fehbvm.com/Article/details/gpvjmhtjp.sHtML

[Q51] 用子查询更新
来源：http://read.share.zdbjq.cn/Article/details/gptinpjcz.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blog.zdbjq.cn/Article/details/giqasvgem.sHtML

[Q52] 删除指定行
来源：http://read.share.fehbvm.com/Article/details/givkwqchs.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.hesvh.cn/Article/details/gwuhakcpt.sHtML

[Q53] 按条件删除
来源：http://m.share.zdbjq.cn/Article/details/gkroywwrx.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.share.hesvh.cn/Article/details/gkjjcrjlg.sHtML

[Q54] 清空表
来源：http://www.blog.hesvh.cn/Article/details/gnydojskz.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.hesvh.cn/Article/details/gisojqqps.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.zdbjq.cn/Article/details/ghfeafoti.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.zdbjq.cn/Article/details/gcclcmatm.sHtML

[Q56] 密集排名（并列不占位）
来源：http://mobile.hesvh.cn/Article/details/ggbppcvhp.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://read.share.zdbjq.cn/Article/details/gablvzhbc.sHtML

[Q57] 行号
来源：http://blog.fehbvm.com/Article/details/gkxrlibhq.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.fehbvm.com/Article/details/gtsfxponc.sHtML

[Q58] 累计求和
来源：http://www.share.fehbvm.com/Article/details/ggjgoqfqt.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.hesvh.cn/Article/details/gaygqlgqg.sHtML

[Q59] 分组内累计
来源：http://www.blog.zdbjq.cn/Article/details/gesdewybg.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/ghxykdvkp.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.fehbvm.com/Article/details/glzkqcuva.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.hesvh.cn/Article/details/gvtnpotgd.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/gjofnaumd.sHtML

[Q61] 移动平均
来源：http://baike.hesvh.cn/Article/details/gyjckeyiq.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/gnigzbyvz.sHtML

[Q62] 分组占比
来源：http://www.share.fehbvm.com/Article/details/goufmgriz.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://baike.hesvh.cn/Article/details/gqrwtsjjw.sHtML

[Q63] 开启事务
来源：http://mobile.fehbvm.com/Article/details/gyurnqyfc.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://mobile.fehbvm.com/Article/details/gedoyssti.sHtML

[Q64] 提交事务
来源：http://wap.fehbvm.com/Article/details/gvnpfchkj.sHtML

COMMIT;
来源：http://www.share.hesvh.cn/Article/details/gvparipex.sHtML

[Q65] 回滚事务
来源：http://www.share.zdbjq.cn/Article/details/gxuapoxqw.sHtML

ROLLBACK;
来源：http://wap.zdbjq.cn/Article/details/giqhnpbbu.sHtML

[Q66] 行锁查询
来源：http://www.share.fehbvm.com/Article/details/ggpixwzmc.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.fehbvm.com/Article/details/giznmrhdn.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.fehbvm.com/Article/details/gnwdtqvnq.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.fehbvm.com/Article/details/gsnzvpwny.sHtML

[Q68] 保存点
来源：http://3g.zdbjq.cn/Article/details/gpnowmeir.sHtML

SAVEPOINT sp1;
来源：http://www.share.hesvh.cn/Article/details/ghbcjxado.sHtML

ROLLBACK TO sp1;
来源：http://baike.hesvh.cn/Article/details/grhrbytut.sHtML

[Q69] 查看执行计划
来源：http://www.share.zdbjq.cn/Article/details/gnzirlpir.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.zdbjq.cn/Article/details/gxmnuvlve.sHtML

[Q70] 更新统计信息
来源：http://mobile.hesvh.cn/Article/details/gyuadupty.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.hesvh.cn/Article/details/gzfqjdfvv.sHtML

[Q71] 查看建表语句
来源：http://read.share.fehbvm.com/Article/details/guupptugs.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.fehbvm.com/Article/details/gooinfhhn.sHtML

[Q72] 查看索引
来源：http://www.m.share.hesvh.cn/Article/details/goyfbvvbo.sHtML

SHOW INDEX FROM users;
来源：http://www.share.fehbvm.com/Article/details/gxfecnkdb.sHtML

[Q73] 查看表状态
来源：http://baike.hesvh.cn/Article/details/gozqastdq.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.fehbvm.com/Article/details/gmgyzgqnu.sHtML

[Q74] 强制使用索引
来源：http://baike.fehbvm.com/Article/details/gemajnddz.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.fehbvm.com/Article/details/gzpejqzfu.sHtML

[Q75] 日期格式化
来源：http://mobile.hesvh.cn/Article/details/grnblyuzt.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.fehbvm.com/Article/details/gxuziunkg.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.zdbjq.cn/Article/details/giwhtpxof.sHtML

[Q76] 按天统计
来源：http://3g.zdbjq.cn/Article/details/gcthnhegu.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.hesvh.cn/Article/details/gcpwwwmmr.sHtML

[Q77] 时间加减
来源：http://www.blog.fehbvm.com/Article/details/gbwiauzhs.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.zdbjq.cn/Article/details/glmrmzslx.sHtML


<!-- 参考信息 -->