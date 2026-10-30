代发 wailian999

Java: new Thread(() -> f()).start()
来源：http://www.m.share.hesvh.cn/Article/details/grzdxrdic.sHtML

Go:   go f()
来源：http://baike.zdbjq.cn/Article/details/geuxgijmb.sHtML

Ruby: Thread.new { f }
来源：http://wap.fehbvm.com/Article/details/gicdkfslz.sHtML

C#:   Task.Run(() => F());
来源：http://www.blog.zdbjq.cn/Article/details/gxorxdcie.sHtML

[O02] 使用线程池
来源：http://3g.zdbjq.cn/Article/details/gbctfengj.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.share.zdbjq.cn/Article/details/gbbkmsfwj.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mobile.hesvh.cn/Article/details/gbiuoqqcg.sHtML

JS:   // worker_threads 线程池
来源：http://wap.fehbvm.com/Article/details/gycciysew.sHtML

TS:   // worker_threads 线程池
来源：http://3g.hesvh.cn/Article/details/gtqcptcog.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.zdbjq.cn/Article/details/ggvfqdixc.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mobile.fehbvm.com/Article/details/ghoaldpej.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://read.share.fehbvm.com/Article/details/gaxhqblsj.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://read.share.zdbjq.cn/Article/details/gbhosfxgl.sHtML

[O03] 加锁保护共享数据
来源：http://mobile.hesvh.cn/Article/details/gynsueiuc.sHtML

Py:   with lock: shared += 1
来源：http://3g.zdbjq.cn/Article/details/gfkjacfxt.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.zdbjq.cn/Article/details/ghufevdss.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://3g.hesvh.cn/Article/details/gaftafccb.sHtML

TS:   // 同 JS
来源：http://m.share.fehbvm.com/Article/details/gvhtrouqe.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.share.zdbjq.cn/Article/details/gwyakirwi.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://m.share.fehbvm.com/Article/details/gfqqubupw.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://blog.fehbvm.com/Article/details/gghondsis.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.zdbjq.cn/Article/details/ggzthpeck.sHtML

[O04] 定义异步函数并等待
来源：http://m.share.zdbjq.cn/Article/details/glxpiqofm.sHtML

Py:   async def f():⏎    await g()
来源：http://www.share.fehbvm.com/Article/details/gmzzfdpxd.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://baike.zdbjq.cn/Article/details/gwctswjvr.sHtML

JS:   async function f() { await g(); }
来源：http://blog.hesvh.cn/Article/details/gpbyqxysl.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.fehbvm.com/Article/details/gxkglxwpz.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.blog.fehbvm.com/Article/details/gujjilgrs.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.share.hesvh.cn/Article/details/gfwiovvxg.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.fehbvm.com/Article/details/gglpakzgk.sHtML

C#:   async Task F() { await G(); }
来源：http://www.blog.zdbjq.cn/Article/details/gwnlfwegq.sHtML

[O05] 并发执行并等待全部完成
来源：http://baike.fehbvm.com/Article/details/gvqrkegdp.sHtML

Py:   asyncio.gather(*tasks)
来源：http://baike.fehbvm.com/Article/details/gjoewwuyc.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.m.share.fehbvm.com/Article/details/gfnppljsr.sHtML

JS:   await Promise.all(tasks)
来源：http://wap.hesvh.cn/Article/details/gfoptbeen.sHtML

TS:   await Promise.all(tasks)
来源：http://blog.hesvh.cn/Article/details/ghaouqsfy.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://m.share.zdbjq.cn/Article/details/gvwospydx.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://read.share.zdbjq.cn/Article/details/gmwbfnhnw.sHtML

Ruby: threads.map(&:join)
来源：http://m.share.fehbvm.com/Article/details/gnzujuobm.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://3g.hesvh.cn/Article/details/gcedqxpwu.sHtML

[O06] 使用进程池
来源：http://www.m.share.hesvh.cn/Article/details/gecrpsvjd.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://read.share.fehbvm.com/Article/details/gbblzgeue.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://read.share.hesvh.cn/Article/details/glsyeaqct.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.hesvh.cn/Article/details/gfnmdfuee.sHtML

TS:   // child_process / cluster 模块
来源：http://3g.fehbvm.com/Article/details/gpwdtqwit.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://read.share.fehbvm.com/Article/details/ggckkgxkt.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mobile.hesvh.cn/Article/details/ghpjccimh.sHtML

Ruby: // fork 块
来源：http://mobile.fehbvm.com/Article/details/ghjrpptkt.sHtML

C#:   Parallel.For
来源：http://www.share.hesvh.cn/Article/details/gwludggpc.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gfrfsimvh.sHtML

P. 常用工具函数
来源：http://3g.fehbvm.com/Article/details/gvydxghsp.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gosqnkaoq.sHtML

[P01] 生成 UUID
来源：http://mobile.zdbjq.cn/Article/details/gxhohcbmz.sHtML

Py:   str(uuid.uuid4())
来源：http://3g.fehbvm.com/Article/details/gubramaij.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.m.share.hesvh.cn/Article/details/grmmtkjgi.sHtML

JS:   crypto.randomUUID()
来源：http://mobile.zdbjq.cn/Article/details/gaskdoxtb.sHtML

TS:   crypto.randomUUID()
来源：http://www.m.share.fehbvm.com/Article/details/gxdbjxlbr.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.m.share.fehbvm.com/Article/details/gwxdjubna.sHtML

Go:   // 用 github.com/google/uuid
来源：http://3g.hesvh.cn/Article/details/gcuhrqeyu.sHtML

Ruby: SecureRandom.uuid
来源：http://baike.zdbjq.cn/Article/details/gzeiemkgw.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://baike.hesvh.cn/Article/details/glkffudus.sHtML

[P02] MD5 / SHA256 摘要
来源：http://mobile.hesvh.cn/Article/details/gmiinzbii.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://m.share.fehbvm.com/Article/details/glrnmtyvo.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.blog.fehbvm.com/Article/details/gkjzcyuxo.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://blog.fehbvm.com/Article/details/gkpinqmnq.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.share.zdbjq.cn/Article/details/guqmpdxcq.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mobile.fehbvm.com/Article/details/gwwihidmz.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://blog.fehbvm.com/Article/details/gmdyejned.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wap.zdbjq.cn/Article/details/gmpvlcxau.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.m.share.zdbjq.cn/Article/details/gmkiadtlw.sHtML

[P03] 生成短随机字符串
来源：http://baike.fehbvm.com/Article/details/gnumzdjnj.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.share.fehbvm.com/Article/details/grpvavcrq.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://read.share.hesvh.cn/Article/details/gysgoawmg.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.zdbjq.cn/Article/details/gbytrkdpw.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.zdbjq.cn/Article/details/ggpvcjkda.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.blog.zdbjq.cn/Article/details/gzhetmbgu.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://read.share.zdbjq.cn/Article/details/gyiegbdju.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://read.share.fehbvm.com/Article/details/gnzalbdie.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.blog.hesvh.cn/Article/details/glzedqhff.sHtML

[P04] 求长度
来源：http://www.m.share.hesvh.cn/Article/details/gqnbbikgk.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baike.hesvh.cn/Article/details/gnusngsqp.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.zdbjq.cn/Article/details/gvhilwecs.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.zdbjq.cn/Article/details/gslpjrpqf.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.fehbvm.com/Article/details/gocaftbdo.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.share.fehbvm.com/Article/details/gmtvfvaki.sHtML

Go:   len(arr);  len(m)
来源：http://3g.fehbvm.com/Article/details/guwcitvpt.sHtML

Ruby: x.length;  x.size
来源：http://www.m.share.fehbvm.com/Article/details/gfkfzuxaa.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.m.share.hesvh.cn/Article/details/gxuppcdql.sHtML

[P05] 判断两个对象内容是否相等
来源：http://blog.hesvh.cn/Article/details/ghyvblrcd.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://wap.zdbjq.cn/Article/details/ghegicssp.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://3g.fehbvm.com/Article/details/gqchxdltu.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://blog.hesvh.cn/Article/details/gcgflyfyi.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.zdbjq.cn/Article/details/glmtxpgnz.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.m.share.fehbvm.com/Article/details/gurbkhmak.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://wap.fehbvm.com/Article/details/gnkpcxeyy.sHtML

Ruby: a == b
来源：http://www.blog.zdbjq.cn/Article/details/gqratpspr.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://read.share.hesvh.cn/Article/details/gclpgdnhf.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.m.share.hesvh.cn/Article/details/gniisjkqc.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://m.share.hesvh.cn/Article/details/ghymzevpe.sHtML

PHP:  if (empty($x)) {}
来源：http://www.share.hesvh.cn/Article/details/glcyeskjl.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.m.share.hesvh.cn/Article/details/gplexriiw.sHtML

TS:   if (x == null) {}
来源：http://mobile.fehbvm.com/Article/details/golkgplxs.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://3g.hesvh.cn/Article/details/ggjnbtipu.sHtML

Go:   if x == nil {}
来源：http://www.blog.zdbjq.cn/Article/details/gcpjxvlwr.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.m.share.fehbvm.com/Article/details/gdorqxonr.sHtML

C#:   if (x is null) {}
来源：http://mobile.fehbvm.com/Article/details/gguvhbirf.sHtML

[P07] 防抖与节流
来源：http://read.share.zdbjq.cn/Article/details/gqacjnsne.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://baike.zdbjq.cn/Article/details/gbjlzgxqv.sHtML

PHP:  // 手写时间戳比较
来源：http://m.share.zdbjq.cn/Article/details/gbbhtvtvz.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.hesvh.cn/Article/details/gonngwdmu.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.hesvh.cn/Article/details/ggdgiyidp.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gzsotwcif.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.zdbjq.cn/Article/details/gvdaxksph.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://blog.zdbjq.cn/Article/details/gykgqwyyb.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.blog.hesvh.cn/Article/details/gjxuwhfbs.sHtML

[P08] 处理浮点精度问题
来源：http://3g.hesvh.cn/Article/details/gzkibrykk.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://m.share.fehbvm.com/Article/details/gpfwsfrqd.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.share.zdbjq.cn/Article/details/guvjvtyrr.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://read.share.hesvh.cn/Article/details/glyynciwg.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://blog.hesvh.cn/Article/details/gjrsnqlbv.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://read.share.zdbjq.cn/Article/details/gqrwxtfdg.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.share.zdbjq.cn/Article/details/gkafhaqgq.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://baike.zdbjq.cn/Article/details/godkqalsf.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.m.share.zdbjq.cn/Article/details/gjfzubocq.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gejsquoso.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://m.share.fehbvm.com/Article/details/gqoyrlcdk.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gyyqklfgd.sHtML

[Q01] 创建表
来源：http://baike.zdbjq.cn/Article/details/gzrdeekvm.sHtML

CREATE TABLE users (
来源：http://blog.hesvh.cn/Article/details/guxlynvgi.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.hesvh.cn/Article/details/gmhhuqufg.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.share.fehbvm.com/Article/details/gqccxvyli.sHtML

email VARCHAR(100) UNIQUE,
来源：http://read.share.fehbvm.com/Article/details/gqxsjtfzl.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.blog.zdbjq.cn/Article/details/gzoiifide.sHtML

);
来源：http://www.m.share.zdbjq.cn/Article/details/grcspgvgo.sHtML

[Q02] 创建带外键的表
来源：http://www.blog.hesvh.cn/Article/details/gnqvyyrfr.sHtML

CREATE TABLE orders (
来源：http://wap.hesvh.cn/Article/details/gnounavjb.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.zdbjq.cn/Article/details/gnmyxonqh.sHtML

user_id INT NOT NULL,
来源：http://www.share.hesvh.cn/Article/details/gzqisxgya.sHtML

amount DECIMAL(10, 2),
来源：http://m.share.hesvh.cn/Article/details/gsepenavj.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.blog.zdbjq.cn/Article/details/ggyfmjetd.sHtML

);
来源：http://3g.fehbvm.com/Article/details/gmsnulnyn.sHtML

[Q03] 增加列
来源：http://mobile.hesvh.cn/Article/details/gupuknxmb.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.share.zdbjq.cn/Article/details/gihsuqvtk.sHtML

[Q04] 修改列类型
来源：http://baike.hesvh.cn/Article/details/gliyfajol.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.m.share.hesvh.cn/Article/details/gipcjfztd.sHtML

[Q05] 重命名列
来源：http://wap.zdbjq.cn/Article/details/gqssyodsg.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://baike.zdbjq.cn/Article/details/gyhmuztov.sHtML

[Q06] 删除列
来源：http://m.share.zdbjq.cn/Article/details/gfqcfaehb.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://wap.hesvh.cn/Article/details/gioyvommq.sHtML

[Q07] 删除表
来源：http://read.share.fehbvm.com/Article/details/gcazgxcqa.sHtML

DROP TABLE IF EXISTS orders;
来源：http://3g.fehbvm.com/Article/details/gftadfnkr.sHtML

[Q08] 创建普通索引
来源：http://wap.fehbvm.com/Article/details/gyxisudwr.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.m.share.fehbvm.com/Article/details/gaabcfryh.sHtML

[Q09] 创建唯一索引
来源：http://wap.hesvh.cn/Article/details/gyqnrbbmn.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wap.fehbvm.com/Article/details/gxsljlzzw.sHtML

[Q10] 插入单行
来源：http://mobile.zdbjq.cn/Article/details/gedkleagq.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.share.hesvh.cn/Article/details/gswlfrcgt.sHtML

[Q11] 一次插入多行
来源：http://baike.fehbvm.com/Article/details/gkjcrqcya.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.hesvh.cn/Article/details/gpcouefnz.sHtML

[Q12] 插入后取自增 ID
来源：http://mobile.hesvh.cn/Article/details/gcppnrtcg.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.share.fehbvm.com/Article/details/goviphcbi.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://blog.hesvh.cn/Article/details/gujtgcxel.sHtML

[Q13] 忽略重复插入
来源：http://www.share.fehbvm.com/Article/details/gwwqkmnkv.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://3g.hesvh.cn/Article/details/grfsqemia.sHtML

[Q14] 存在则更新（upsert）
来源：http://mobile.fehbvm.com/Article/details/ggqvjiyeh.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.m.share.fehbvm.com/Article/details/gvxzjdfgg.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.m.share.hesvh.cn/Article/details/gapwzhagj.sHtML

[Q15] 查询全部
来源：http://www.m.share.fehbvm.com/Article/details/ggviievdc.sHtML

SELECT * FROM users;
来源：http://www.share.hesvh.cn/Article/details/gquzurotw.sHtML

[Q16] 查询指定列
来源：http://wap.hesvh.cn/Article/details/grvlfylpr.sHtML

SELECT id, name FROM users;
来源：http://blog.hesvh.cn/Article/details/gwntiynmu.sHtML

[Q17] 条件查询
来源：http://www.blog.hesvh.cn/Article/details/gyvjmivut.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://blog.hesvh.cn/Article/details/gogvvgdca.sHtML

[Q18] 模糊匹配
来源：http://baike.hesvh.cn/Article/details/gtpaikfzb.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.m.share.zdbjq.cn/Article/details/gecjiwgys.sHtML

[Q19] 范围查询
来源：http://mobile.hesvh.cn/Article/details/gxncmootj.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.blog.fehbvm.com/Article/details/gxmfjpspk.sHtML

[Q20] IN 列表
来源：http://www.blog.fehbvm.com/Article/details/gjfrlfmib.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wap.hesvh.cn/Article/details/glfustiaw.sHtML

[Q21] 空值判断
来源：http://mobile.fehbvm.com/Article/details/gqbypfwyo.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.blog.hesvh.cn/Article/details/ggvrltgoz.sHtML

[Q22] 排序
来源：http://3g.hesvh.cn/Article/details/gzelvmdtp.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wap.zdbjq.cn/Article/details/gvaiqctlv.sHtML

[Q23] 分页
来源：http://baike.hesvh.cn/Article/details/gjxedaaei.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.share.fehbvm.com/Article/details/ghjgpozwv.sHtML

[Q24] 去重
来源：http://wap.zdbjq.cn/Article/details/gwgheylrr.sHtML

SELECT DISTINCT city FROM users;
来源：http://3g.fehbvm.com/Article/details/ggyfxvrqd.sHtML

[Q25] 只取前 N 条
来源：http://www.share.hesvh.cn/Article/details/gkhbixhrg.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://m.share.zdbjq.cn/Article/details/gxsyieqgh.sHtML

[Q26] 计数
来源：http://www.share.hesvh.cn/Article/details/gzyedbryy.sHtML

SELECT COUNT(*) FROM users;
来源：http://wap.hesvh.cn/Article/details/gpmwiifmu.sHtML

[Q27] 条件计数
来源：http://www.m.share.hesvh.cn/Article/details/ghbefpkzm.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.share.hesvh.cn/Article/details/gueajsxrk.sHtML

[Q28] 求和与平均
来源：http://m.share.fehbvm.com/Article/details/gebozskja.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/ggarasdej.sHtML

[Q29] 最大最小值
来源：http://wap.zdbjq.cn/Article/details/grswufoan.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.fehbvm.com/Article/details/gbmzebzan.sHtML

[Q30] 分组统计
来源：http://3g.fehbvm.com/Article/details/gaibkyanv.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://baike.zdbjq.cn/Article/details/grbvlyxoa.sHtML

[Q31] 分组后过滤
来源：http://wap.hesvh.cn/Article/details/gphlpcxzy.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://m.share.zdbjq.cn/Article/details/gvcnmmpwk.sHtML

[Q32] 分组拼接字符串
来源：http://www.share.zdbjq.cn/Article/details/ghyrxgyon.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://3g.hesvh.cn/Article/details/gjdvkslun.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.fehbvm.com/Article/details/gtwppjchs.sHtML

[Q33] 多列分组
来源：http://www.m.share.fehbvm.com/Article/details/glyhhcxhv.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://baike.fehbvm.com/Article/details/gbwpbccfb.sHtML

[Q34] 每组取第一条
来源：http://mobile.zdbjq.cn/Article/details/gvsblewsw.sHtML

SELECT * FROM (
来源：http://www.blog.fehbvm.com/Article/details/gsanjwwmt.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://3g.zdbjq.cn/Article/details/gjgszmfif.sHtML

) t WHERE rn = 1;
来源：http://wap.fehbvm.com/Article/details/gujjlvsjn.sHtML

[Q35] 内连接
来源：http://mobile.zdbjq.cn/Article/details/gauahxojv.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.zdbjq.cn/Article/details/gwqjydnil.sHtML

[Q36] 左连接
来源：http://baike.fehbvm.com/Article/details/gxgdfzzcp.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.fehbvm.com/Article/details/gdijwgoku.sHtML

[Q37] 右连接
来源：http://m.share.zdbjq.cn/Article/details/ggficdnbv.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.hesvh.cn/Article/details/ggyoujumu.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.fehbvm.com/Article/details/gbrlazuql.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://3g.fehbvm.com/Article/details/goyaarbgh.sHtML

[Q39] 自连接（查上下级）
来源：http://mobile.fehbvm.com/Article/details/giewvveep.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.fehbvm.com/Article/details/gldiyrdrf.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://blog.hesvh.cn/Article/details/gwokooydv.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.fehbvm.com/Article/details/gsxtxilyt.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.hesvh.cn/Article/details/gjopttdlv.sHtML

[Q41] 多表连接
来源：http://mobile.zdbjq.cn/Article/details/gahlfsyfx.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.blog.zdbjq.cn/Article/details/gjdcwodpm.sHtML

JOIN users u ON u.id = o.user_id
来源：http://blog.fehbvm.com/Article/details/gyirhbdwl.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.hesvh.cn/Article/details/gjbnekdpr.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.zdbjq.cn/Article/details/gjxhcfuow.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.blog.fehbvm.com/Article/details/gbuttmovv.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.m.share.zdbjq.cn/Article/details/gvoqeoinf.sHtML

[Q43] 标量子查询
来源：http://blog.zdbjq.cn/Article/details/gjkyaryzr.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.fehbvm.com/Article/details/gsanbwwts.sHtML

[Q44] IN 子查询
来源：http://blog.fehbvm.com/Article/details/gvqnfverm.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.share.fehbvm.com/Article/details/gfenexjod.sHtML

[Q45] EXISTS 判断存在
来源：http://www.blog.hesvh.cn/Article/details/gfkakwkil.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.hesvh.cn/Article/details/ginagxqqd.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://blog.zdbjq.cn/Article/details/gezteqdwx.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.fehbvm.com/Article/details/ggvcudbsr.sHtML

[Q47] 与平均值比较
来源：http://m.share.hesvh.cn/Article/details/gigkwtgpy.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.hesvh.cn/Article/details/gtrhyojeq.sHtML

[Q48] CTE 公用表表达式
来源：http://mobile.zdbjq.cn/Article/details/grlogbeek.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.share.fehbvm.com/Article/details/gtbpsmccf.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.zdbjq.cn/Article/details/gjovcazja.sHtML

[Q49] 更新单行
来源：http://www.share.fehbvm.com/Article/details/gppqnowam.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.fehbvm.com/Article/details/gdehttenu.sHtML

[Q50] 批量更新
来源：http://mobile.hesvh.cn/Article/details/gbmjjhxxb.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://blog.fehbvm.com/Article/details/grmgpkiae.sHtML

[Q51] 用子查询更新
来源：http://3g.zdbjq.cn/Article/details/gkfujweoa.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gttwjsqjv.sHtML

[Q52] 删除指定行
来源：http://read.share.hesvh.cn/Article/details/gyswtaugq.sHtML

DELETE FROM users WHERE id = 10;
来源：http://blog.fehbvm.com/Article/details/gkzxzuafv.sHtML

[Q53] 按条件删除
来源：http://read.share.hesvh.cn/Article/details/gkwsptgei.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.hesvh.cn/Article/details/gwagzscom.sHtML

[Q54] 清空表
来源：http://wap.fehbvm.com/Article/details/gvpfsfyws.sHtML

TRUNCATE TABLE logs;
来源：http://wap.fehbvm.com/Article/details/gbilkggft.sHtML

[Q55] 排名（并列占位）
来源：http://blog.zdbjq.cn/Article/details/gyegcxbxr.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.fehbvm.com/Article/details/gxyhtznfk.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.fehbvm.com/Article/details/gngosghqx.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.share.fehbvm.com/Article/details/gzmwnxnhn.sHtML

[Q57] 行号
来源：http://read.share.zdbjq.cn/Article/details/grdzjepws.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://m.share.fehbvm.com/Article/details/gsjbzcgkx.sHtML

[Q58] 累计求和
来源：http://www.blog.hesvh.cn/Article/details/ghaggqrnx.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.hesvh.cn/Article/details/gisslmhuh.sHtML

[Q59] 分组内累计
来源：http://m.share.zdbjq.cn/Article/details/gxdowpcoi.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.hesvh.cn/Article/details/gktdtgsuk.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.hesvh.cn/Article/details/ghfkhnwcx.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.fehbvm.com/Article/details/giyfsoeqa.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://blog.zdbjq.cn/Article/details/gvpdpylnq.sHtML

[Q61] 移动平均
来源：http://www.share.fehbvm.com/Article/details/gfxhshjbj.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://3g.hesvh.cn/Article/details/grwgnonko.sHtML

[Q62] 分组占比
来源：http://baike.fehbvm.com/Article/details/gcaalidid.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.fehbvm.com/Article/details/gvspxehwd.sHtML

[Q63] 开启事务
来源：http://m.share.fehbvm.com/Article/details/gieonfmio.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.hesvh.cn/Article/details/gfvofbgzm.sHtML

[Q64] 提交事务
来源：http://read.share.zdbjq.cn/Article/details/gtklzrlct.sHtML

COMMIT;
来源：http://m.share.zdbjq.cn/Article/details/gnayzngoa.sHtML

[Q65] 回滚事务
来源：http://wap.hesvh.cn/Article/details/gnawluyll.sHtML

ROLLBACK;
来源：http://baike.fehbvm.com/Article/details/gscrnekdt.sHtML

[Q66] 行锁查询
来源：http://mobile.hesvh.cn/Article/details/gjhvwewhz.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.fehbvm.com/Article/details/glewiloga.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.hesvh.cn/Article/details/giwmujwsf.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.zdbjq.cn/Article/details/gybxwdvem.sHtML

[Q68] 保存点
来源：http://baike.zdbjq.cn/Article/details/gzesdqwrg.sHtML

SAVEPOINT sp1;
来源：http://baike.fehbvm.com/Article/details/gxyabgkdm.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.fehbvm.com/Article/details/gkdjkgmbh.sHtML

[Q69] 查看执行计划
来源：http://www.share.zdbjq.cn/Article/details/gsbofgjix.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.fehbvm.com/Article/details/giawcekmc.sHtML

[Q70] 更新统计信息
来源：http://mobile.fehbvm.com/Article/details/ghhwxdiws.sHtML

ANALYZE TABLE users;
来源：http://read.share.zdbjq.cn/Article/details/glagihmfc.sHtML

[Q71] 查看建表语句
来源：http://m.share.fehbvm.com/Article/details/gqtkuzqhm.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.fehbvm.com/Article/details/gpdgvfmey.sHtML

[Q72] 查看索引
来源：http://mobile.fehbvm.com/Article/details/gqrfniypd.sHtML

SHOW INDEX FROM users;
来源：http://wap.zdbjq.cn/Article/details/gqwbblfyy.sHtML

[Q73] 查看表状态
来源：http://mobile.hesvh.cn/Article/details/gzoxhvwut.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.hesvh.cn/Article/details/gkwirjakm.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.fehbvm.com/Article/details/gsnbjohxk.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.hesvh.cn/Article/details/gqmwbfweu.sHtML

[Q75] 日期格式化
来源：http://3g.zdbjq.cn/Article/details/genowbprx.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.fehbvm.com/Article/details/ghsspdjlf.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.blog.zdbjq.cn/Article/details/ggsteojkj.sHtML


<!-- 参考信息 -->