代发 wailian999

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wap.fanxiaobao.xyz/Article/details/gpceobhfx.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://3g.fanxiaobao.xyz/Article/details/glwitpgbs.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mobile.fanxiaobao.xyz/Article/details/gcekrcfre.sHtML

TS:   // 同 JS
来源：http://wap.fanxiaobao.xyz/Article/details/ghmgatqpi.sHtML

Java: new Thread(() -> f()).start()
来源：http://3g.fanxiaobao.xyz/Article/details/gbalaeidj.sHtML

Go:   go f()
来源：http://m.share.fanxiaobao.xyz/Article/details/grnfovbxc.sHtML

Ruby: Thread.new { f }
来源：http://www.share.fanxiaobao.xyz/Article/details/gquafzzsu.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.fanxiaobao.xyz/Article/details/gutvmfxwb.sHtML

[O02] 使用线程池
来源：http://baike.fanxiaobao.xyz/Article/details/gyaeazzcc.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.share.fanxiaobao.xyz/Article/details/gmwngyotj.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blog.fanxiaobao.xyz/Article/details/gdfazkwhr.sHtML

JS:   // worker_threads 线程池
来源：http://read.share.fanxiaobao.xyz/Article/details/ghsxchkmz.sHtML

TS:   // worker_threads 线程池
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gghofidpb.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://baike.fanxiaobao.xyz/Article/details/gjofeghmz.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wap.fanxiaobao.xyz/Article/details/grcthtkyq.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://read.share.fanxiaobao.xyz/Article/details/gyikntxvj.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://baike.fanxiaobao.xyz/Article/details/gicyzrnwx.sHtML

[O03] 加锁保护共享数据
来源：http://wap.fanxiaobao.xyz/Article/details/gehuncfif.sHtML

Py:   with lock: shared += 1
来源：http://read.share.fanxiaobao.xyz/Article/details/gcfnwqbak.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.fanxiaobao.xyz/Article/details/gugtmgqzb.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://baike.fanxiaobao.xyz/Article/details/gbtjstard.sHtML

TS:   // 同 JS
来源：http://m.share.fanxiaobao.xyz/Article/details/gsieypmwt.sHtML

Java: synchronized (this) { shared++; }
来源：http://baike.fanxiaobao.xyz/Article/details/gutzvpajc.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://blog.fanxiaobao.xyz/Article/details/gduiswpxx.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://baike.fanxiaobao.xyz/Article/details/gberiuwwt.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxynuletn.sHtML

[O04] 定义异步函数并等待
来源：http://www.share.fanxiaobao.xyz/Article/details/gxjljkkgw.sHtML

Py:   async def f():⏎    await g()
来源：http://m.share.fanxiaobao.xyz/Article/details/gcfuzxcwp.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.share.fanxiaobao.xyz/Article/details/grdqgilmq.sHtML

JS:   async function f() { await g(); }
来源：http://3g.fanxiaobao.xyz/Article/details/gklkotkxo.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsxoulrch.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.fanxiaobao.xyz/Article/details/gozeuhqth.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.share.fanxiaobao.xyz/Article/details/gweyjdime.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://mobile.fanxiaobao.xyz/Article/details/gtcdtjpot.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.fanxiaobao.xyz/Article/details/gegrvwgwe.sHtML

[O05] 并发执行并等待全部完成
来源：http://read.share.fanxiaobao.xyz/Article/details/gblixqkee.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxkoyhfww.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkcjijlan.sHtML

JS:   await Promise.all(tasks)
来源：http://baike.fanxiaobao.xyz/Article/details/gtcunpkio.sHtML

TS:   await Promise.all(tasks)
来源：http://baike.fanxiaobao.xyz/Article/details/gxkjpsxkj.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wap.fanxiaobao.xyz/Article/details/gmxtunmqc.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpnkieggm.sHtML

Ruby: threads.map(&:join)
来源：http://baike.fanxiaobao.xyz/Article/details/gvzgzaddq.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gxuelkguq.sHtML

[O06] 使用进程池
来源：http://baike.fanxiaobao.xyz/Article/details/gythsujsd.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gezkgkuvt.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gguerhhhj.sHtML

JS:   // child_process / cluster 模块
来源：http://baike.fanxiaobao.xyz/Article/details/grmnjtjby.sHtML

TS:   // child_process / cluster 模块
来源：http://read.share.fanxiaobao.xyz/Article/details/givoedoza.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://m.share.fanxiaobao.xyz/Article/details/gintfpfja.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mobile.fanxiaobao.xyz/Article/details/grflqfnho.sHtML

Ruby: // fork 块
来源：http://baike.fanxiaobao.xyz/Article/details/ggdsratbx.sHtML

C#:   Parallel.For
来源：http://baike.fanxiaobao.xyz/Article/details/gtjfuhxyf.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gtmfrhunl.sHtML

P. 常用工具函数
来源：http://wap.fanxiaobao.xyz/Article/details/gczohdvqu.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gwwqfxznp.sHtML

[P01] 生成 UUID
来源：http://mobile.fanxiaobao.xyz/Article/details/gnmdnyoxf.sHtML

Py:   str(uuid.uuid4())
来源：http://3g.fanxiaobao.xyz/Article/details/gvjrdblub.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wap.fanxiaobao.xyz/Article/details/gbraozrjz.sHtML

JS:   crypto.randomUUID()
来源：http://3g.fanxiaobao.xyz/Article/details/gvpriftef.sHtML

TS:   crypto.randomUUID()
来源：http://baike.fanxiaobao.xyz/Article/details/gmjvrwpzk.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqacvmbzm.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gggajwdys.sHtML

Ruby: SecureRandom.uuid
来源：http://blog.fanxiaobao.xyz/Article/details/gxxaszjai.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.blog.fanxiaobao.xyz/Article/details/glbxtijsj.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnbyujiqz.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://baike.fanxiaobao.xyz/Article/details/gypksoqyd.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://wap.fanxiaobao.xyz/Article/details/gtqgrnpox.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://baike.fanxiaobao.xyz/Article/details/gwkoxfalb.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://baike.fanxiaobao.xyz/Article/details/gahogciva.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wap.fanxiaobao.xyz/Article/details/gfigctxax.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.share.fanxiaobao.xyz/Article/details/gxkawzerv.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grodpkwal.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvupgzyvn.sHtML

[P03] 生成短随机字符串
来源：http://baike.fanxiaobao.xyz/Article/details/gipaqklem.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://m.share.fanxiaobao.xyz/Article/details/geymvpvls.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghtlndtyn.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.fanxiaobao.xyz/Article/details/giwlfvjry.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.fanxiaobao.xyz/Article/details/ggtbrtmyi.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqzspokrv.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://baike.fanxiaobao.xyz/Article/details/gkvfphxqb.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://m.share.fanxiaobao.xyz/Article/details/gfrtmnpiv.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://blog.fanxiaobao.xyz/Article/details/gmbeopfcd.sHtML

[P04] 求长度
来源：http://baike.fanxiaobao.xyz/Article/details/grynrdnpm.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbktgnlbm.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.fanxiaobao.xyz/Article/details/gghfhrscf.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.fanxiaobao.xyz/Article/details/gpwmhgtoe.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giunbqhmm.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpfatspft.sHtML

Go:   len(arr);  len(m)
来源：http://mobile.fanxiaobao.xyz/Article/details/guwturheh.sHtML

Ruby: x.length;  x.size
来源：http://3g.fanxiaobao.xyz/Article/details/ghytlqxhp.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://m.share.fanxiaobao.xyz/Article/details/gflklpodq.sHtML

[P05] 判断两个对象内容是否相等
来源：http://wap.fanxiaobao.xyz/Article/details/gdotcqhhe.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://mobile.fanxiaobao.xyz/Article/details/gxjmzhjha.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://m.share.fanxiaobao.xyz/Article/details/gpuqbgqbh.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://3g.fanxiaobao.xyz/Article/details/gugbrofub.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.fanxiaobao.xyz/Article/details/goxnqvpwe.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://3g.fanxiaobao.xyz/Article/details/guoilhpnc.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://wap.fanxiaobao.xyz/Article/details/gumqbgvti.sHtML

Ruby: a == b
来源：http://www.share.fanxiaobao.xyz/Article/details/gupdkuewd.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://3g.fanxiaobao.xyz/Article/details/glpyjirzn.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://m.share.fanxiaobao.xyz/Article/details/ghagbveql.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://m.share.fanxiaobao.xyz/Article/details/gtbbvjadc.sHtML

PHP:  if (empty($x)) {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gcyrnuucm.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzwzguorz.sHtML

TS:   if (x == null) {}
来源：http://baike.fanxiaobao.xyz/Article/details/gozxztwml.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://wap.fanxiaobao.xyz/Article/details/gzmaaadwu.sHtML

Go:   if x == nil {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gulzmzdoo.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.share.fanxiaobao.xyz/Article/details/goigiiash.sHtML

C#:   if (x is null) {}
来源：http://baike.fanxiaobao.xyz/Article/details/gbxrkbqmc.sHtML

[P07] 防抖与节流
来源：http://www.share.fanxiaobao.xyz/Article/details/glazenaxm.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.share.fanxiaobao.xyz/Article/details/gihfvnqeh.sHtML

PHP:  // 手写时间戳比较
来源：http://baike.fanxiaobao.xyz/Article/details/gmnplbboe.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.fanxiaobao.xyz/Article/details/gtlgjzjgp.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmrjdjphp.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glnkzpsrz.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.fanxiaobao.xyz/Article/details/grmjmttdg.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://wap.fanxiaobao.xyz/Article/details/guqtqomfq.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://baike.fanxiaobao.xyz/Article/details/gkmcfpdie.sHtML

[P08] 处理浮点精度问题
来源：http://wap.fanxiaobao.xyz/Article/details/gzghatdkk.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.share.fanxiaobao.xyz/Article/details/gszyqqnuo.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.share.fanxiaobao.xyz/Article/details/gdjemwnjk.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://m.share.fanxiaobao.xyz/Article/details/gzftmzrug.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gksgumygp.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzwocvbxd.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://baike.fanxiaobao.xyz/Article/details/gsdhzvzup.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://m.share.fanxiaobao.xyz/Article/details/ggbsiqzpz.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmrjpruec.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnhdtssdn.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://m.share.fanxiaobao.xyz/Article/details/gjsiffrid.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjxkjkiha.sHtML

[Q01] 创建表
来源：http://blog.fanxiaobao.xyz/Article/details/gisgrbffn.sHtML

CREATE TABLE users (
来源：http://www.share.fanxiaobao.xyz/Article/details/ggzunivra.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.fanxiaobao.xyz/Article/details/gosbqlsfu.sHtML

name VARCHAR(50) NOT NULL,
来源：http://baike.fanxiaobao.xyz/Article/details/gjnsybtka.sHtML

email VARCHAR(100) UNIQUE,
来源：http://baike.fanxiaobao.xyz/Article/details/gzmnhqcef.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://3g.fanxiaobao.xyz/Article/details/gxiocjqby.sHtML

);
来源：http://baike.fanxiaobao.xyz/Article/details/gazxwityc.sHtML

[Q02] 创建带外键的表
来源：http://baike.fanxiaobao.xyz/Article/details/gcamjfbci.sHtML

CREATE TABLE orders (
来源：http://www.blog.fanxiaobao.xyz/Article/details/gatrrriwu.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdnsmqhfw.sHtML

user_id INT NOT NULL,
来源：http://mobile.fanxiaobao.xyz/Article/details/gspqkffob.sHtML

amount DECIMAL(10, 2),
来源：http://blog.fanxiaobao.xyz/Article/details/gndrwwcds.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.share.fanxiaobao.xyz/Article/details/gwmhvfdhe.sHtML

);
来源：http://read.share.fanxiaobao.xyz/Article/details/gipkklozd.sHtML

[Q03] 增加列
来源：http://blog.fanxiaobao.xyz/Article/details/glvcrvzmj.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mobile.fanxiaobao.xyz/Article/details/gtbortraq.sHtML

[Q04] 修改列类型
来源：http://read.share.fanxiaobao.xyz/Article/details/gatoqompx.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wap.fanxiaobao.xyz/Article/details/gcomgixop.sHtML

[Q05] 重命名列
来源：http://www.share.fanxiaobao.xyz/Article/details/gjhtvfsvt.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wap.fanxiaobao.xyz/Article/details/gmqfnmwwf.sHtML

[Q06] 删除列
来源：http://3g.fanxiaobao.xyz/Article/details/gpwngncdu.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtruksfds.sHtML

[Q07] 删除表
来源：http://www.share.fanxiaobao.xyz/Article/details/gqttyrxmb.sHtML

DROP TABLE IF EXISTS orders;
来源：http://blog.fanxiaobao.xyz/Article/details/gzelkkmjx.sHtML

[Q08] 创建普通索引
来源：http://m.share.fanxiaobao.xyz/Article/details/guyuavcbk.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsplkitjj.sHtML

[Q09] 创建唯一索引
来源：http://baike.fanxiaobao.xyz/Article/details/gmigfmpin.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghsyeldyu.sHtML

[Q10] 插入单行
来源：http://m.share.fanxiaobao.xyz/Article/details/gmwekvagc.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.fanxiaobao.xyz/Article/details/gpjntldgr.sHtML

[Q11] 一次插入多行
来源：http://baike.fanxiaobao.xyz/Article/details/getmrctjv.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://3g.fanxiaobao.xyz/Article/details/gixjgrwsr.sHtML

[Q12] 插入后取自增 ID
来源：http://m.share.fanxiaobao.xyz/Article/details/gnboxttdd.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghkqpjgzk.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wap.fanxiaobao.xyz/Article/details/gvtvughoo.sHtML

[Q13] 忽略重复插入
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcapprfaq.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://read.share.fanxiaobao.xyz/Article/details/gqjczckps.sHtML

[Q14] 存在则更新（upsert）
来源：http://3g.fanxiaobao.xyz/Article/details/gfulpdpkq.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wap.fanxiaobao.xyz/Article/details/ghuyvlxfx.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://read.share.fanxiaobao.xyz/Article/details/gbtpfqdli.sHtML

[Q15] 查询全部
来源：http://mobile.fanxiaobao.xyz/Article/details/gmrenjygx.sHtML

SELECT * FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmhlgbfrq.sHtML

[Q16] 查询指定列
来源：http://m.share.fanxiaobao.xyz/Article/details/garvybcns.sHtML

SELECT id, name FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/ghgwtekhk.sHtML

[Q17] 条件查询
来源：http://m.share.fanxiaobao.xyz/Article/details/gqnqodvwv.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/glbcagcyv.sHtML

[Q18] 模糊匹配
来源：http://baike.fanxiaobao.xyz/Article/details/godqnghbb.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.share.fanxiaobao.xyz/Article/details/goxxvbokx.sHtML

[Q19] 范围查询
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guiixjgoe.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://3g.fanxiaobao.xyz/Article/details/gknmphyor.sHtML

[Q20] IN 列表
来源：http://blog.fanxiaobao.xyz/Article/details/ggrtuhgny.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://baike.fanxiaobao.xyz/Article/details/gebwxovur.sHtML

[Q21] 空值判断
来源：http://blog.fanxiaobao.xyz/Article/details/gfjnyobln.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://wap.fanxiaobao.xyz/Article/details/gxplpumod.sHtML

[Q22] 排序
来源：http://m.share.fanxiaobao.xyz/Article/details/gmzkmexxe.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.share.fanxiaobao.xyz/Article/details/gmqjbjolo.sHtML

[Q23] 分页
来源：http://www.share.fanxiaobao.xyz/Article/details/gsoqypxmz.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://read.share.fanxiaobao.xyz/Article/details/giebfncag.sHtML

[Q24] 去重
来源：http://blog.fanxiaobao.xyz/Article/details/ghlnraxmn.sHtML

SELECT DISTINCT city FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gyefycjmf.sHtML

[Q25] 只取前 N 条
来源：http://m.share.fanxiaobao.xyz/Article/details/gcgxvmlrc.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://3g.fanxiaobao.xyz/Article/details/gvjbmfmun.sHtML

[Q26] 计数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goudqzwxu.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grgtkygbk.sHtML

[Q27] 条件计数
来源：http://read.share.fanxiaobao.xyz/Article/details/gmnxwyhfe.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gbwufhayk.sHtML

[Q28] 求和与平均
来源：http://m.share.fanxiaobao.xyz/Article/details/gybqbfnao.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wap.fanxiaobao.xyz/Article/details/gbokdvufk.sHtML

[Q29] 最大最小值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzjivriif.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gfebxcxep.sHtML

[Q30] 分组统计
来源：http://3g.fanxiaobao.xyz/Article/details/gvnckiivl.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://baike.fanxiaobao.xyz/Article/details/glvttrvlf.sHtML

[Q31] 分组后过滤
来源：http://m.share.fanxiaobao.xyz/Article/details/gudlbwnfa.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mobile.fanxiaobao.xyz/Article/details/gulvqnati.sHtML

[Q32] 分组拼接字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/gmeoyudnz.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wap.fanxiaobao.xyz/Article/details/goekmaugx.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.fanxiaobao.xyz/Article/details/goajkxneb.sHtML

[Q33] 多列分组
来源：http://read.share.fanxiaobao.xyz/Article/details/gwsyuyoln.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gifvdhond.sHtML

[Q34] 每组取第一条
来源：http://m.share.fanxiaobao.xyz/Article/details/gizriheog.sHtML

SELECT * FROM (
来源：http://www.share.fanxiaobao.xyz/Article/details/gokwqqhpb.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://baike.fanxiaobao.xyz/Article/details/ghotvqygk.sHtML

) t WHERE rn = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gzbnhbeoi.sHtML

[Q35] 内连接
来源：http://3g.fanxiaobao.xyz/Article/details/grepljuey.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wap.fanxiaobao.xyz/Article/details/gbkjotjbz.sHtML

[Q36] 左连接
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gweaasgla.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpsfkvsdo.sHtML

[Q37] 右连接
来源：http://m.share.fanxiaobao.xyz/Article/details/gxzhnntvk.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.fanxiaobao.xyz/Article/details/gbbbcetsp.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://baike.fanxiaobao.xyz/Article/details/gojjusfaw.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://blog.fanxiaobao.xyz/Article/details/gbccuiuho.sHtML

[Q39] 自连接（查上下级）
来源：http://baike.fanxiaobao.xyz/Article/details/gvlaczotc.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.fanxiaobao.xyz/Article/details/grhwvyuom.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://m.share.fanxiaobao.xyz/Article/details/gusrelfvg.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.fanxiaobao.xyz/Article/details/gzmyyfban.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkahfqhyu.sHtML

[Q41] 多表连接
来源：http://mobile.fanxiaobao.xyz/Article/details/gkaaqexdl.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.fanxiaobao.xyz/Article/details/gthhtsltz.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaayfllny.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghmmenyfh.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.fanxiaobao.xyz/Article/details/ggnjghsgw.sHtML

SELECT u.name, o.amount FROM users u
来源：http://wap.fanxiaobao.xyz/Article/details/gbstdcjuu.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gumlqhufd.sHtML

[Q43] 标量子查询
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvritrqmj.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvavdwkim.sHtML

[Q44] IN 子查询
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqwiccdhr.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://m.share.fanxiaobao.xyz/Article/details/gkuzahshz.sHtML

[Q45] EXISTS 判断存在
来源：http://blog.fanxiaobao.xyz/Article/details/gvtpxogqf.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.fanxiaobao.xyz/Article/details/gpmcrzmwl.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://m.share.fanxiaobao.xyz/Article/details/gqvtkbupo.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjerzlvme.sHtML

[Q47] 与平均值比较
来源：http://www.share.fanxiaobao.xyz/Article/details/gqihkrszz.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://m.share.fanxiaobao.xyz/Article/details/grlmuqvjw.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.fanxiaobao.xyz/Article/details/gvyalriuz.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.fanxiaobao.xyz/Article/details/gdzselxii.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://baike.fanxiaobao.xyz/Article/details/gvdwemwhg.sHtML

[Q49] 更新单行
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpnjucxxi.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.fanxiaobao.xyz/Article/details/gkwwqyhbw.sHtML

[Q50] 批量更新
来源：http://3g.fanxiaobao.xyz/Article/details/gglpvsdcc.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://baike.fanxiaobao.xyz/Article/details/gpfwtmrdo.sHtML

[Q51] 用子查询更新
来源：http://3g.fanxiaobao.xyz/Article/details/giexzspbf.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gqxqhiipo.sHtML

[Q52] 删除指定行
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzfkgocxa.sHtML

DELETE FROM users WHERE id = 10;
来源：http://blog.fanxiaobao.xyz/Article/details/gvmzsaquv.sHtML

[Q53] 按条件删除
来源：http://read.share.fanxiaobao.xyz/Article/details/gqadlqzlh.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.fanxiaobao.xyz/Article/details/gwdtzwavf.sHtML

[Q54] 清空表
来源：http://wap.fanxiaobao.xyz/Article/details/grhaiowtd.sHtML

TRUNCATE TABLE logs;
来源：http://mobile.fanxiaobao.xyz/Article/details/gwjitotng.sHtML

[Q55] 排名（并列占位）
来源：http://3g.fanxiaobao.xyz/Article/details/gshhgszok.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.fanxiaobao.xyz/Article/details/giobftfsk.sHtML

[Q56] 密集排名（并列不占位）
来源：http://wap.fanxiaobao.xyz/Article/details/gqzjdhyfe.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.fanxiaobao.xyz/Article/details/ggvxwpaoc.sHtML

[Q57] 行号
来源：http://3g.fanxiaobao.xyz/Article/details/gwtnaxppm.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gixcxiryz.sHtML

[Q58] 累计求和
来源：http://wap.fanxiaobao.xyz/Article/details/gzqvbpadb.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghvqbgesa.sHtML

[Q59] 分组内累计
来源：http://www.share.fanxiaobao.xyz/Article/details/gymtuthcq.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/gmfeumqsj.sHtML

[Q60] 取上一行 / 下一行
来源：http://wap.fanxiaobao.xyz/Article/details/gjlientaf.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wap.fanxiaobao.xyz/Article/details/gtgmjgdjk.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/gyucpwrgd.sHtML

[Q61] 移动平均
来源：http://read.share.fanxiaobao.xyz/Article/details/grnpbzwsb.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.fanxiaobao.xyz/Article/details/gcbydbvcr.sHtML

[Q62] 分组占比
来源：http://m.share.fanxiaobao.xyz/Article/details/gmjhxmxca.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvbbdprde.sHtML

[Q63] 开启事务
来源：http://blog.fanxiaobao.xyz/Article/details/gbwvgjixq.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://blog.fanxiaobao.xyz/Article/details/griaukrzi.sHtML

[Q64] 提交事务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdkxvokix.sHtML

COMMIT;
来源：http://m.share.fanxiaobao.xyz/Article/details/gzxrnappi.sHtML

[Q65] 回滚事务
来源：http://3g.fanxiaobao.xyz/Article/details/goufhxltv.sHtML

ROLLBACK;
来源：http://www.share.fanxiaobao.xyz/Article/details/gsycxtqvu.sHtML

[Q66] 行锁查询
来源：http://read.share.fanxiaobao.xyz/Article/details/gwqmpjsoe.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.fanxiaobao.xyz/Article/details/gvcwwxvtr.sHtML

[Q67] 设置隔离级别
来源：http://read.share.fanxiaobao.xyz/Article/details/gopzistgl.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.fanxiaobao.xyz/Article/details/ggaujfiza.sHtML

[Q68] 保存点
来源：http://m.share.fanxiaobao.xyz/Article/details/gjeppanrj.sHtML

SAVEPOINT sp1;
来源：http://3g.fanxiaobao.xyz/Article/details/gozvfajam.sHtML

ROLLBACK TO sp1;
来源：http://wap.fanxiaobao.xyz/Article/details/gudjhjptp.sHtML

[Q69] 查看执行计划
来源：http://baike.fanxiaobao.xyz/Article/details/gxhtkefit.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.fanxiaobao.xyz/Article/details/glsljydzg.sHtML

[Q70] 更新统计信息
来源：http://m.share.fanxiaobao.xyz/Article/details/grejlryqq.sHtML

ANALYZE TABLE users;
来源：http://wap.fanxiaobao.xyz/Article/details/gtwhggjcc.sHtML

[Q71] 查看建表语句
来源：http://wap.fanxiaobao.xyz/Article/details/gpvzdcsnp.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.fanxiaobao.xyz/Article/details/gkmwyeoki.sHtML

[Q72] 查看索引
来源：http://3g.fanxiaobao.xyz/Article/details/gqsljxmqv.sHtML

SHOW INDEX FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/grlpxhzua.sHtML

[Q73] 查看表状态
来源：http://read.share.fanxiaobao.xyz/Article/details/godvevtkn.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.fanxiaobao.xyz/Article/details/geyudvofv.sHtML

[Q74] 强制使用索引
来源：http://wap.fanxiaobao.xyz/Article/details/gvvwilxaf.sHtML


<!-- 参考信息 -->