代发 wailian999

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.m.share.hesvh.cn/Article/details/gtmgazqkp.sHtML

[O03] 加锁保护共享数据
来源：http://baike.zdbjq.cn/Article/details/gboowsvcp.sHtML

Py:   with lock: shared += 1
来源：http://m.share.fehbvm.com/Article/details/gzvkshrdo.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://wap.hesvh.cn/Article/details/gkdycypkv.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://blog.zdbjq.cn/Article/details/gvykhfxuk.sHtML

TS:   // 同 JS
来源：http://www.blog.hesvh.cn/Article/details/gcrtptclb.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.m.share.hesvh.cn/Article/details/gvtywgopg.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://m.share.fehbvm.com/Article/details/gpibmvvmu.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.m.share.hesvh.cn/Article/details/glxukztzt.sHtML

C#:   lock (gate) { shared++; }
来源：http://baike.fehbvm.com/Article/details/gbuklszte.sHtML

[O04] 定义异步函数并等待
来源：http://3g.hesvh.cn/Article/details/gfrsilfui.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.hesvh.cn/Article/details/gkqxxlkgv.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.hesvh.cn/Article/details/gdarfoxxl.sHtML

JS:   async function f() { await g(); }
来源：http://www.blog.zdbjq.cn/Article/details/gqvfakftb.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://wap.hesvh.cn/Article/details/gseetcvaa.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.zdbjq.cn/Article/details/gtctyerjh.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://read.share.hesvh.cn/Article/details/gwgnfhaeh.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.blog.zdbjq.cn/Article/details/ggykteewg.sHtML

C#:   async Task F() { await G(); }
来源：http://mobile.zdbjq.cn/Article/details/gcmfmnsph.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.hesvh.cn/Article/details/geruzljzq.sHtML

Py:   asyncio.gather(*tasks)
来源：http://read.share.fehbvm.com/Article/details/gurcpkwhx.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://m.share.fehbvm.com/Article/details/gvwujkcdq.sHtML

JS:   await Promise.all(tasks)
来源：http://www.m.share.fehbvm.com/Article/details/gsqghjuli.sHtML

TS:   await Promise.all(tasks)
来源：http://m.share.zdbjq.cn/Article/details/gkvclffqi.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.share.fehbvm.com/Article/details/gepctulgb.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://3g.fehbvm.com/Article/details/gtrbrnrxz.sHtML

Ruby: threads.map(&:join)
来源：http://www.blog.fehbvm.com/Article/details/gsfbiyygy.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.share.fehbvm.com/Article/details/ggvwhlmjf.sHtML

[O06] 使用进程池
来源：http://www.blog.hesvh.cn/Article/details/glurqhsqg.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://3g.fehbvm.com/Article/details/gfyrewfsb.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://read.share.zdbjq.cn/Article/details/gataqynby.sHtML

JS:   // child_process / cluster 模块
来源：http://baike.zdbjq.cn/Article/details/glkwziind.sHtML

TS:   // child_process / cluster 模块
来源：http://baike.fehbvm.com/Article/details/goafofifa.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://m.share.hesvh.cn/Article/details/geyhffage.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.m.share.zdbjq.cn/Article/details/glehepsbu.sHtML

Ruby: // fork 块
来源：http://www.m.share.hesvh.cn/Article/details/ggnqvjurd.sHtML

C#:   Parallel.For
来源：http://www.share.zdbjq.cn/Article/details/gzybbwyhi.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/ghgxnctto.sHtML

P. 常用工具函数
来源：http://www.m.share.hesvh.cn/Article/details/gljduysxi.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gpbbavize.sHtML

[P01] 生成 UUID
来源：http://baike.hesvh.cn/Article/details/gimyskbue.sHtML

Py:   str(uuid.uuid4())
来源：http://m.share.hesvh.cn/Article/details/gahchvfiq.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wap.hesvh.cn/Article/details/gjvczdhvn.sHtML

JS:   crypto.randomUUID()
来源：http://mobile.fehbvm.com/Article/details/gasnbkatq.sHtML

TS:   crypto.randomUUID()
来源：http://wap.hesvh.cn/Article/details/gpahlqghx.sHtML

Java: UUID.randomUUID().toString()
来源：http://m.share.hesvh.cn/Article/details/gfkgfjfqp.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.m.share.zdbjq.cn/Article/details/gogdlorfp.sHtML

Ruby: SecureRandom.uuid
来源：http://wap.hesvh.cn/Article/details/gexagafon.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://wap.zdbjq.cn/Article/details/gwdfykmma.sHtML

[P02] MD5 / SHA256 摘要
来源：http://read.share.hesvh.cn/Article/details/gkzdfcrux.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://3g.zdbjq.cn/Article/details/gchyazfdg.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://wap.hesvh.cn/Article/details/gtgftihzr.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://blog.fehbvm.com/Article/details/gamelomuy.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.fehbvm.com/Article/details/goxgaxxdx.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://baike.hesvh.cn/Article/details/grwzilooy.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.m.share.zdbjq.cn/Article/details/glyioykjx.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wap.hesvh.cn/Article/details/gmcvnexni.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://baike.zdbjq.cn/Article/details/giivklmux.sHtML

[P03] 生成短随机字符串
来源：http://www.blog.fehbvm.com/Article/details/ghnznqzfv.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.blog.fehbvm.com/Article/details/gpnufxwew.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.blog.hesvh.cn/Article/details/gxuwdfksm.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.zdbjq.cn/Article/details/gpeywrskr.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.hesvh.cn/Article/details/gbnmkemhe.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mobile.fehbvm.com/Article/details/gyrpboxqn.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://baike.zdbjq.cn/Article/details/gvjatrorb.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://wap.zdbjq.cn/Article/details/gxqtacacv.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.share.hesvh.cn/Article/details/gaucatklr.sHtML

[P04] 求长度
来源：http://wap.zdbjq.cn/Article/details/gampuxnlz.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://m.share.zdbjq.cn/Article/details/ggnbequij.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.hesvh.cn/Article/details/gkufanqcz.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.hesvh.cn/Article/details/gkyttkrfg.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.hesvh.cn/Article/details/gypkxsrzn.sHtML

Java: list.size();  map.size();  s.length()
来源：http://wap.hesvh.cn/Article/details/gcnckuwdc.sHtML

Go:   len(arr);  len(m)
来源：http://wap.fehbvm.com/Article/details/gerexfhvy.sHtML

Ruby: x.length;  x.size
来源：http://3g.zdbjq.cn/Article/details/gzuswzksq.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://m.share.hesvh.cn/Article/details/ggwksfrsn.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.blog.fehbvm.com/Article/details/gyaxzqyzn.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.blog.fehbvm.com/Article/details/gfvyzeysk.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://m.share.hesvh.cn/Article/details/gegrypxyq.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://blog.hesvh.cn/Article/details/gkazivpbp.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.hesvh.cn/Article/details/gogvhwggs.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://read.share.fehbvm.com/Article/details/gfftusdnv.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.share.fehbvm.com/Article/details/gqjndjrvu.sHtML

Ruby: a == b
来源：http://3g.fehbvm.com/Article/details/gkahlqmjf.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://read.share.hesvh.cn/Article/details/gjkykcvoj.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mobile.hesvh.cn/Article/details/gumarlows.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://baike.zdbjq.cn/Article/details/glyqemike.sHtML

PHP:  if (empty($x)) {}
来源：http://blog.fehbvm.com/Article/details/gwafuqabv.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://baike.zdbjq.cn/Article/details/gwduvtpal.sHtML

TS:   if (x == null) {}
来源：http://m.share.zdbjq.cn/Article/details/gqmsanzkj.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.blog.fehbvm.com/Article/details/gtreeddrx.sHtML

Go:   if x == nil {}
来源：http://read.share.hesvh.cn/Article/details/gopmtcjmt.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.share.zdbjq.cn/Article/details/glxegkznc.sHtML

C#:   if (x is null) {}
来源：http://m.share.hesvh.cn/Article/details/ghhtwokuv.sHtML

[P07] 防抖与节流
来源：http://baike.hesvh.cn/Article/details/goyavsdwe.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://m.share.hesvh.cn/Article/details/gjavvjwso.sHtML

PHP:  // 手写时间戳比较
来源：http://m.share.fehbvm.com/Article/details/gamtkaeva.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.fehbvm.com/Article/details/gbvhpppsf.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.zdbjq.cn/Article/details/gtlxxutuh.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://blog.fehbvm.com/Article/details/guryiwrml.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.zdbjq.cn/Article/details/gkqcfyzhf.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.m.share.fehbvm.com/Article/details/giewspyeo.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://baike.zdbjq.cn/Article/details/ghopsmpei.sHtML

[P08] 处理浮点精度问题
来源：http://read.share.fehbvm.com/Article/details/gwlhuzayk.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://baike.hesvh.cn/Article/details/gnrvnxrrw.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.share.fehbvm.com/Article/details/ghvumncft.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://m.share.zdbjq.cn/Article/details/gqnnpmbfn.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.blog.fehbvm.com/Article/details/ghfabznju.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://3g.fehbvm.com/Article/details/gtcrjimnv.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.blog.hesvh.cn/Article/details/gaxjnuifp.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mobile.fehbvm.com/Article/details/gnhqspawz.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://m.share.fehbvm.com/Article/details/gwllowckc.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gkkigbxff.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.share.hesvh.cn/Article/details/gmqsmzomm.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gkhiebdsh.sHtML

[Q01] 创建表
来源：http://www.m.share.zdbjq.cn/Article/details/glbyejomj.sHtML

CREATE TABLE users (
来源：http://wap.hesvh.cn/Article/details/gviyprdcb.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.hesvh.cn/Article/details/gggneglpd.sHtML

name VARCHAR(50) NOT NULL,
来源：http://wap.hesvh.cn/Article/details/gzicweebj.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.m.share.zdbjq.cn/Article/details/ggrhambqx.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://baike.zdbjq.cn/Article/details/gyiqlyinu.sHtML

);
来源：http://mobile.fehbvm.com/Article/details/gavsjeqlg.sHtML

[Q02] 创建带外键的表
来源：http://m.share.zdbjq.cn/Article/details/gifgsfuqx.sHtML

CREATE TABLE orders (
来源：http://www.share.hesvh.cn/Article/details/gqeghjmgy.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.zdbjq.cn/Article/details/gdedgsquh.sHtML

user_id INT NOT NULL,
来源：http://3g.hesvh.cn/Article/details/gecvleipq.sHtML

amount DECIMAL(10, 2),
来源：http://m.share.fehbvm.com/Article/details/gidsptmnb.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wap.zdbjq.cn/Article/details/gdnhnqqio.sHtML

);
来源：http://www.share.zdbjq.cn/Article/details/gryoqsgqx.sHtML

[Q03] 增加列
来源：http://3g.fehbvm.com/Article/details/gkdsrcxdn.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://read.share.zdbjq.cn/Article/details/gjqmconlq.sHtML

[Q04] 修改列类型
来源：http://www.share.fehbvm.com/Article/details/gobqkwgps.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mobile.zdbjq.cn/Article/details/gqsxcmezc.sHtML

[Q05] 重命名列
来源：http://baike.fehbvm.com/Article/details/gfwuujvma.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.blog.fehbvm.com/Article/details/gwbwcqgsw.sHtML

[Q06] 删除列
来源：http://www.m.share.fehbvm.com/Article/details/gacooinlx.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://m.share.zdbjq.cn/Article/details/gpjxejgec.sHtML

[Q07] 删除表
来源：http://www.share.hesvh.cn/Article/details/gjvbqbbyi.sHtML

DROP TABLE IF EXISTS orders;
来源：http://read.share.zdbjq.cn/Article/details/gjhqhgjmf.sHtML

[Q08] 创建普通索引
来源：http://mobile.fehbvm.com/Article/details/gvtkqqdrh.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://baike.zdbjq.cn/Article/details/gmecmnhcv.sHtML

[Q09] 创建唯一索引
来源：http://mobile.hesvh.cn/Article/details/gfulmasgf.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mobile.hesvh.cn/Article/details/gcjqmxkww.sHtML

[Q10] 插入单行
来源：http://3g.fehbvm.com/Article/details/gguczlres.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.share.hesvh.cn/Article/details/gizslenru.sHtML

[Q11] 一次插入多行
来源：http://www.share.zdbjq.cn/Article/details/gzoycsicb.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://read.share.fehbvm.com/Article/details/gwofyowrb.sHtML

[Q12] 插入后取自增 ID
来源：http://3g.hesvh.cn/Article/details/gkbyjkrcw.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://blog.hesvh.cn/Article/details/gznyfybgi.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.m.share.zdbjq.cn/Article/details/galnlopwx.sHtML

[Q13] 忽略重复插入
来源：http://read.share.hesvh.cn/Article/details/gifqgahps.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.fehbvm.com/Article/details/gjltgpydx.sHtML

[Q14] 存在则更新（upsert）
来源：http://wap.hesvh.cn/Article/details/gwmqzjgap.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.m.share.fehbvm.com/Article/details/gzuxkfobi.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.share.hesvh.cn/Article/details/gljwpqvlk.sHtML

[Q15] 查询全部
来源：http://www.blog.fehbvm.com/Article/details/gysplsmcw.sHtML

SELECT * FROM users;
来源：http://www.share.fehbvm.com/Article/details/gyyrivzcb.sHtML

[Q16] 查询指定列
来源：http://3g.fehbvm.com/Article/details/gyuzatzyv.sHtML

SELECT id, name FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gokmtaohi.sHtML

[Q17] 条件查询
来源：http://www.blog.fehbvm.com/Article/details/gapqdhvmh.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.fehbvm.com/Article/details/gxzjrejxj.sHtML

[Q18] 模糊匹配
来源：http://baike.zdbjq.cn/Article/details/gpwlamtmb.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.zdbjq.cn/Article/details/gscezzhdv.sHtML

[Q19] 范围查询
来源：http://www.blog.zdbjq.cn/Article/details/gfkyvagoh.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.blog.zdbjq.cn/Article/details/gvoyemlsi.sHtML

[Q20] IN 列表
来源：http://mobile.zdbjq.cn/Article/details/ghcsymgju.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://3g.hesvh.cn/Article/details/gfwdqzpvp.sHtML

[Q21] 空值判断
来源：http://3g.fehbvm.com/Article/details/gyldllzfq.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://baike.hesvh.cn/Article/details/gcovfdrmc.sHtML

[Q22] 排序
来源：http://www.blog.fehbvm.com/Article/details/ghmmanhde.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://m.share.zdbjq.cn/Article/details/gvmdivrvd.sHtML

[Q23] 分页
来源：http://m.share.zdbjq.cn/Article/details/gtclsjwvv.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://read.share.hesvh.cn/Article/details/gjhchsegc.sHtML

[Q24] 去重
来源：http://www.share.hesvh.cn/Article/details/gvzkpfkjz.sHtML

SELECT DISTINCT city FROM users;
来源：http://read.share.hesvh.cn/Article/details/gkocxuweq.sHtML

[Q25] 只取前 N 条
来源：http://3g.fehbvm.com/Article/details/goxnjasur.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wap.zdbjq.cn/Article/details/ghvpnhzsz.sHtML

[Q26] 计数
来源：http://www.m.share.hesvh.cn/Article/details/glwjsxiga.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gjfymqeun.sHtML

[Q27] 条件计数
来源：http://baike.hesvh.cn/Article/details/grgzaaotk.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gsnmqfcvo.sHtML

[Q28] 求和与平均
来源：http://read.share.zdbjq.cn/Article/details/gqcgonawk.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/gjhdczqmy.sHtML

[Q29] 最大最小值
来源：http://www.m.share.zdbjq.cn/Article/details/gwdrpnurz.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gowuchrqz.sHtML

[Q30] 分组统计
来源：http://www.blog.hesvh.cn/Article/details/gymnnvzpc.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.zdbjq.cn/Article/details/ghhdarjrl.sHtML

[Q31] 分组后过滤
来源：http://mobile.zdbjq.cn/Article/details/glnihvimu.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://read.share.hesvh.cn/Article/details/gfrldwdty.sHtML

[Q32] 分组拼接字符串
来源：http://baike.zdbjq.cn/Article/details/gzrhwbbck.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://3g.hesvh.cn/Article/details/ggnorsvbu.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://blog.zdbjq.cn/Article/details/gdktqxjdm.sHtML

[Q33] 多列分组
来源：http://wap.zdbjq.cn/Article/details/gwqtuqugq.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.share.fehbvm.com/Article/details/goiniybgj.sHtML

[Q34] 每组取第一条
来源：http://m.share.hesvh.cn/Article/details/ggtbozazo.sHtML

SELECT * FROM (
来源：http://baike.fehbvm.com/Article/details/gzwovfmke.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mobile.hesvh.cn/Article/details/gbjyrtnvl.sHtML

) t WHERE rn = 1;
来源：http://m.share.hesvh.cn/Article/details/gkyfwedwx.sHtML

[Q35] 内连接
来源：http://read.share.hesvh.cn/Article/details/gawktexul.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.hesvh.cn/Article/details/gvrphcqca.sHtML

[Q36] 左连接
来源：http://blog.fehbvm.com/Article/details/gxqlfdtuz.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mobile.fehbvm.com/Article/details/geyxskqru.sHtML

[Q37] 右连接
来源：http://baike.zdbjq.cn/Article/details/gnyppqtde.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.hesvh.cn/Article/details/gibaidrmt.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://baike.fehbvm.com/Article/details/geeuemzpc.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://baike.fehbvm.com/Article/details/gvsuqsoul.sHtML

[Q39] 自连接（查上下级）
来源：http://wap.zdbjq.cn/Article/details/gobdfcwwu.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.zdbjq.cn/Article/details/gztzyshnj.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.fehbvm.com/Article/details/gzkulrsvd.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.fehbvm.com/Article/details/gwijsjppb.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.fehbvm.com/Article/details/gyhfonsrf.sHtML

[Q41] 多表连接
来源：http://www.blog.hesvh.cn/Article/details/gzaqxritf.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.fehbvm.com/Article/details/gamkyibyx.sHtML

JOIN users u ON u.id = o.user_id
来源：http://read.share.hesvh.cn/Article/details/gdijmrfjo.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.zdbjq.cn/Article/details/gvvmsdlor.sHtML

[Q42] 连接条件附加过滤
来源：http://m.share.fehbvm.com/Article/details/gcsdffmrh.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.zdbjq.cn/Article/details/gmpcdmpat.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.m.share.hesvh.cn/Article/details/gddgdtgdg.sHtML

[Q43] 标量子查询
来源：http://www.share.fehbvm.com/Article/details/gltslwogt.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.blog.zdbjq.cn/Article/details/gowwnvhvl.sHtML

[Q44] IN 子查询
来源：http://m.share.hesvh.cn/Article/details/gpwgvqexx.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://m.share.fehbvm.com/Article/details/gosyeyuzk.sHtML

[Q45] EXISTS 判断存在
来源：http://mobile.hesvh.cn/Article/details/gnxfjdapy.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.fehbvm.com/Article/details/giflhusgr.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://wap.zdbjq.cn/Article/details/gahcbijwk.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.fehbvm.com/Article/details/glufzafjl.sHtML

[Q47] 与平均值比较
来源：http://m.share.zdbjq.cn/Article/details/ggmonfscr.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.zdbjq.cn/Article/details/gnldtvxfu.sHtML

[Q48] CTE 公用表表达式
来源：http://www.share.zdbjq.cn/Article/details/glpflzogt.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.m.share.zdbjq.cn/Article/details/gvdjymjxm.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://mobile.zdbjq.cn/Article/details/grdswjlht.sHtML

[Q49] 更新单行
来源：http://3g.hesvh.cn/Article/details/gwahtzbvt.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://m.share.fehbvm.com/Article/details/gtconusxl.sHtML

[Q50] 批量更新
来源：http://read.share.zdbjq.cn/Article/details/gnokgesgd.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://baike.fehbvm.com/Article/details/gudhmwduv.sHtML

[Q51] 用子查询更新
来源：http://wap.fehbvm.com/Article/details/gtpwxuwjk.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.hesvh.cn/Article/details/gcsqeusug.sHtML

[Q52] 删除指定行
来源：http://wap.hesvh.cn/Article/details/ghufnjvyi.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.fehbvm.com/Article/details/gkzkqemcg.sHtML

[Q53] 按条件删除
来源：http://read.share.fehbvm.com/Article/details/gywpvmdoj.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://m.share.hesvh.cn/Article/details/gxtwgwdwn.sHtML

[Q54] 清空表
来源：http://www.share.hesvh.cn/Article/details/guphoktpw.sHtML

TRUNCATE TABLE logs;
来源：http://m.share.hesvh.cn/Article/details/gjhkwrpfr.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.fehbvm.com/Article/details/govuizkdm.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.share.hesvh.cn/Article/details/gxnlmnpfa.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.m.share.zdbjq.cn/Article/details/gvmazgsep.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mobile.fehbvm.com/Article/details/glxpnkuvj.sHtML

[Q57] 行号
来源：http://www.m.share.hesvh.cn/Article/details/gfxfhmzxt.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gozsoqqsa.sHtML

[Q58] 累计求和
来源：http://read.share.hesvh.cn/Article/details/gdzjrngqt.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/glwuxpuea.sHtML

[Q59] 分组内累计
来源：http://www.blog.fehbvm.com/Article/details/gfydnfbqw.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://m.share.hesvh.cn/Article/details/getlsofas.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.zdbjq.cn/Article/details/gayremant.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.m.share.fehbvm.com/Article/details/gbzifuqxl.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/grcbcxmsh.sHtML

[Q61] 移动平均
来源：http://www.m.share.zdbjq.cn/Article/details/gfuupkqcd.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wap.fehbvm.com/Article/details/gpmzujsmo.sHtML

[Q62] 分组占比
来源：http://blog.zdbjq.cn/Article/details/gxgvlujze.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.fehbvm.com/Article/details/gexulqyzo.sHtML

[Q63] 开启事务
来源：http://www.blog.fehbvm.com/Article/details/gkpgallql.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.fehbvm.com/Article/details/gchbdjufd.sHtML

[Q64] 提交事务
来源：http://mobile.hesvh.cn/Article/details/gebncugde.sHtML

COMMIT;
来源：http://wap.hesvh.cn/Article/details/gwwnzvhwq.sHtML

[Q65] 回滚事务
来源：http://m.share.hesvh.cn/Article/details/ghkowbovr.sHtML

ROLLBACK;
来源：http://wap.hesvh.cn/Article/details/gepbtsfjh.sHtML

[Q66] 行锁查询
来源：http://www.share.fehbvm.com/Article/details/gbokbvyso.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.hesvh.cn/Article/details/gfzjzueel.sHtML

[Q67] 设置隔离级别
来源：http://3g.fehbvm.com/Article/details/gxljhuhfm.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.hesvh.cn/Article/details/givjdvgbz.sHtML

[Q68] 保存点
来源：http://baike.hesvh.cn/Article/details/gayrnemrd.sHtML

SAVEPOINT sp1;
来源：http://www.share.zdbjq.cn/Article/details/guircbzui.sHtML

ROLLBACK TO sp1;
来源：http://blog.zdbjq.cn/Article/details/gpuqxjquk.sHtML

[Q69] 查看执行计划
来源：http://read.share.hesvh.cn/Article/details/gqzofnhwy.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.fehbvm.com/Article/details/gsquzgcou.sHtML

[Q70] 更新统计信息
来源：http://www.blog.fehbvm.com/Article/details/grqfqqvng.sHtML

ANALYZE TABLE users;
来源：http://wap.zdbjq.cn/Article/details/gozsjxabx.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.zdbjq.cn/Article/details/gqgrsmgnw.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://blog.zdbjq.cn/Article/details/gfajxhaiy.sHtML

[Q72] 查看索引
来源：http://blog.hesvh.cn/Article/details/ghudpnpht.sHtML

SHOW INDEX FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gmmunlsko.sHtML

[Q73] 查看表状态
来源：http://baike.fehbvm.com/Article/details/gijfgqkhi.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.fehbvm.com/Article/details/gyzposhep.sHtML

[Q74] 强制使用索引
来源：http://www.blog.zdbjq.cn/Article/details/gydlaypog.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.zdbjq.cn/Article/details/gppzdxptn.sHtML

[Q75] 日期格式化
来源：http://read.share.zdbjq.cn/Article/details/gxvzedpib.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/ghqvzsuiv.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.zdbjq.cn/Article/details/ggifbdbdg.sHtML

[Q76] 按天统计
来源：http://www.m.share.fehbvm.com/Article/details/gisexpapp.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.fehbvm.com/Article/details/grchxnhxg.sHtML

[Q77] 时间加减
来源：http://mobile.zdbjq.cn/Article/details/gcegrhkdp.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://m.share.fehbvm.com/Article/details/gkmwjjaxy.sHtML

[Q78] 当前时间
来源：http://www.share.fehbvm.com/Article/details/gafcdsytl.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.zdbjq.cn/Article/details/gavzckmtw.sHtML

[Q79] 字符串拼接
来源：http://blog.hesvh.cn/Article/details/gzdvuvxog.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.zdbjq.cn/Article/details/grrnzzlvu.sHtML

[Q80] 字符串截取
来源：http://blog.hesvh.cn/Article/details/gsknslsyp.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.fehbvm.com/Article/details/gkbxixkib.sHtML

[Q81] 字符串替换
来源：http://www.blog.fehbvm.com/Article/details/gjldakdaf.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.hesvh.cn/Article/details/getrqtdca.sHtML


<!-- 参考信息 -->