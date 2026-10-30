代发 wailian999

TS:   // worker_threads 线程池
来源：http://m.share.hesvh.cn/Article/details/gvhidnxhn.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://read.share.zdbjq.cn/Article/details/ghmnvtunx.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://blog.fehbvm.com/Article/details/gsgxxkzek.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://m.share.fehbvm.com/Article/details/gorprrlbh.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://read.share.zdbjq.cn/Article/details/gpnrkfhfr.sHtML

[O03] 加锁保护共享数据
来源：http://baike.hesvh.cn/Article/details/gzdafuter.sHtML

Py:   with lock: shared += 1
来源：http://baike.fehbvm.com/Article/details/gzfhthels.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://3g.hesvh.cn/Article/details/gzrdpeelo.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.share.hesvh.cn/Article/details/gddaedqfr.sHtML

TS:   // 同 JS
来源：http://www.m.share.zdbjq.cn/Article/details/gqxpawpzl.sHtML

Java: synchronized (this) { shared++; }
来源：http://read.share.zdbjq.cn/Article/details/gvesndcfc.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.hesvh.cn/Article/details/gdmklhllw.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://m.share.hesvh.cn/Article/details/gmzsjwnkg.sHtML

C#:   lock (gate) { shared++; }
来源：http://blog.zdbjq.cn/Article/details/grezsfxyy.sHtML

[O04] 定义异步函数并等待
来源：http://baike.hesvh.cn/Article/details/gkoizhphd.sHtML

Py:   async def f():⏎    await g()
来源：http://blog.zdbjq.cn/Article/details/gjvtpcbkm.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://blog.zdbjq.cn/Article/details/gnchrqtsn.sHtML

JS:   async function f() { await g(); }
来源：http://www.blog.fehbvm.com/Article/details/gqddcfchv.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://wap.fehbvm.com/Article/details/gdsanogmk.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.fehbvm.com/Article/details/gotqrlybv.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wap.hesvh.cn/Article/details/gypdvzywa.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.m.share.hesvh.cn/Article/details/gdgodpgcc.sHtML

C#:   async Task F() { await G(); }
来源：http://www.share.fehbvm.com/Article/details/gzussszoh.sHtML

[O05] 并发执行并等待全部完成
来源：http://baike.fehbvm.com/Article/details/gctpgamuo.sHtML

Py:   asyncio.gather(*tasks)
来源：http://3g.hesvh.cn/Article/details/gwzlvchju.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://3g.fehbvm.com/Article/details/gtyqpfipm.sHtML

JS:   await Promise.all(tasks)
来源：http://3g.hesvh.cn/Article/details/gpocmsiiu.sHtML

TS:   await Promise.all(tasks)
来源：http://www.blog.zdbjq.cn/Article/details/gaynpnvza.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mobile.hesvh.cn/Article/details/gecznfieb.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://blog.hesvh.cn/Article/details/gofuobgrl.sHtML

Ruby: threads.map(&:join)
来源：http://3g.fehbvm.com/Article/details/gplbkdaky.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://wap.fehbvm.com/Article/details/gjdjpwjyg.sHtML

[O06] 使用进程池
来源：http://baike.zdbjq.cn/Article/details/girizdncy.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.m.share.hesvh.cn/Article/details/gnskcuwcm.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://wap.zdbjq.cn/Article/details/gsghdoowy.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.hesvh.cn/Article/details/gjniecddf.sHtML

TS:   // child_process / cluster 模块
来源：http://www.share.fehbvm.com/Article/details/grufitgwm.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.m.share.fehbvm.com/Article/details/gmtrlikea.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.blog.fehbvm.com/Article/details/gdnzbxuvc.sHtML

Ruby: // fork 块
来源：http://wap.zdbjq.cn/Article/details/gcxllkinc.sHtML

C#:   Parallel.For
来源：http://www.share.hesvh.cn/Article/details/gkiblhcqw.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gogrdqjkm.sHtML

P. 常用工具函数
来源：http://read.share.fehbvm.com/Article/details/gyylzpvhh.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gtzqozlbv.sHtML

[P01] 生成 UUID
来源：http://www.blog.hesvh.cn/Article/details/gjywikiwy.sHtML

Py:   str(uuid.uuid4())
来源：http://m.share.hesvh.cn/Article/details/gniljqcws.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://blog.hesvh.cn/Article/details/ghvvstkrl.sHtML

JS:   crypto.randomUUID()
来源：http://wap.zdbjq.cn/Article/details/ggxygylvs.sHtML

TS:   crypto.randomUUID()
来源：http://www.share.fehbvm.com/Article/details/gkfnntxqt.sHtML

Java: UUID.randomUUID().toString()
来源：http://mobile.fehbvm.com/Article/details/gthivqopk.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.share.fehbvm.com/Article/details/glcwmtjka.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.fehbvm.com/Article/details/gelvwhqnp.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://mobile.hesvh.cn/Article/details/gnzonledb.sHtML

[P02] MD5 / SHA256 摘要
来源：http://read.share.hesvh.cn/Article/details/gjegbscmj.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.blog.fehbvm.com/Article/details/grdveerhq.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://mobile.hesvh.cn/Article/details/gowldvszx.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.hesvh.cn/Article/details/gwfygvpnv.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://3g.hesvh.cn/Article/details/grfqtlsuc.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.blog.fehbvm.com/Article/details/gptsnytpw.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://baike.zdbjq.cn/Article/details/gmgutfipd.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wap.hesvh.cn/Article/details/gaxqgqjnz.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.blog.fehbvm.com/Article/details/gkapalrzk.sHtML

[P03] 生成短随机字符串
来源：http://www.blog.zdbjq.cn/Article/details/gkhiixfrx.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://read.share.zdbjq.cn/Article/details/gwjgfavdb.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://3g.fehbvm.com/Article/details/gddffayxu.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.hesvh.cn/Article/details/gpbkcycfb.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.hesvh.cn/Article/details/gkfpfywfr.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.m.share.fehbvm.com/Article/details/gnyjxlred.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mobile.hesvh.cn/Article/details/gbdiylzks.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://wap.zdbjq.cn/Article/details/gycohxqvg.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mobile.fehbvm.com/Article/details/gqhgsgley.sHtML

[P04] 求长度
来源：http://www.m.share.zdbjq.cn/Article/details/gaodyahyi.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.blog.hesvh.cn/Article/details/gggcaxuvz.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.hesvh.cn/Article/details/gadjmdzwx.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.zdbjq.cn/Article/details/guzzvvrro.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.zdbjq.cn/Article/details/gjbmmkksp.sHtML

Java: list.size();  map.size();  s.length()
来源：http://3g.fehbvm.com/Article/details/gbsdalmjl.sHtML

Go:   len(arr);  len(m)
来源：http://baike.zdbjq.cn/Article/details/gmwwhbazi.sHtML

Ruby: x.length;  x.size
来源：http://wap.fehbvm.com/Article/details/gogdodqav.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://mobile.hesvh.cn/Article/details/gjnkmuuwm.sHtML

[P05] 判断两个对象内容是否相等
来源：http://blog.zdbjq.cn/Article/details/gyedmondv.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.share.fehbvm.com/Article/details/gkpczvafc.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://read.share.fehbvm.com/Article/details/gtvrxavso.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.blog.hesvh.cn/Article/details/gztufzkou.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.fehbvm.com/Article/details/gywooxbcm.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://read.share.hesvh.cn/Article/details/gscqaaneh.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://blog.hesvh.cn/Article/details/gmzilrplp.sHtML

Ruby: a == b
来源：http://mobile.zdbjq.cn/Article/details/gjwpzatjk.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.share.fehbvm.com/Article/details/gtnpuzihf.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mobile.hesvh.cn/Article/details/gfutbzidh.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.share.fehbvm.com/Article/details/glxfeohtd.sHtML

PHP:  if (empty($x)) {}
来源：http://blog.zdbjq.cn/Article/details/gxpwmxquy.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://blog.fehbvm.com/Article/details/gxnfloxfd.sHtML

TS:   if (x == null) {}
来源：http://3g.hesvh.cn/Article/details/gbwnqrcep.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://mobile.fehbvm.com/Article/details/grdtzzqoi.sHtML

Go:   if x == nil {}
来源：http://3g.zdbjq.cn/Article/details/grfcipqzu.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://3g.hesvh.cn/Article/details/gbcjbwlky.sHtML

C#:   if (x is null) {}
来源：http://m.share.hesvh.cn/Article/details/gfgxafdqm.sHtML

[P07] 防抖与节流
来源：http://m.share.hesvh.cn/Article/details/gqfwcrkar.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://read.share.fehbvm.com/Article/details/gbzcberbu.sHtML

PHP:  // 手写时间戳比较
来源：http://wap.fehbvm.com/Article/details/gdfrfhgyz.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.hesvh.cn/Article/details/gipglkflu.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.fehbvm.com/Article/details/grmuwuhbr.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.blog.zdbjq.cn/Article/details/gpfenxmxi.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://m.share.fehbvm.com/Article/details/ggzntqezd.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://read.share.zdbjq.cn/Article/details/glpdtdqyj.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mobile.zdbjq.cn/Article/details/gqoophzmr.sHtML

[P08] 处理浮点精度问题
来源：http://m.share.hesvh.cn/Article/details/gjraxkikk.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://blog.zdbjq.cn/Article/details/gcxmiyijh.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wap.fehbvm.com/Article/details/gpdizodaj.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.m.share.zdbjq.cn/Article/details/gewuqtntg.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.blog.fehbvm.com/Article/details/gdxsmvhts.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://baike.hesvh.cn/Article/details/gigtcgrut.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://3g.zdbjq.cn/Article/details/gzrmgxmch.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://m.share.fehbvm.com/Article/details/ghgakcfgx.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wap.fehbvm.com/Article/details/giaekyfvm.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gpifuhdlw.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mobile.fehbvm.com/Article/details/ggfkhombh.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gtvhmiwqc.sHtML

[Q01] 创建表
来源：http://www.blog.hesvh.cn/Article/details/gfuphstra.sHtML

CREATE TABLE users (
来源：http://3g.zdbjq.cn/Article/details/grrxnwvfe.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.hesvh.cn/Article/details/gwiqqpkow.sHtML

name VARCHAR(50) NOT NULL,
来源：http://read.share.fehbvm.com/Article/details/gytglwztu.sHtML

email VARCHAR(100) UNIQUE,
来源：http://baike.zdbjq.cn/Article/details/goeuraitn.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.share.zdbjq.cn/Article/details/glpqtgfgt.sHtML

);
来源：http://baike.fehbvm.com/Article/details/gisvenvhr.sHtML

[Q02] 创建带外键的表
来源：http://www.share.hesvh.cn/Article/details/gsitbxclc.sHtML

CREATE TABLE orders (
来源：http://m.share.zdbjq.cn/Article/details/gdqchnplt.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.fehbvm.com/Article/details/gyfokmqce.sHtML

user_id INT NOT NULL,
来源：http://mobile.zdbjq.cn/Article/details/gfduisljo.sHtML

amount DECIMAL(10, 2),
来源：http://mobile.zdbjq.cn/Article/details/guvuwjhrh.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.m.share.zdbjq.cn/Article/details/goxhphlyh.sHtML

);
来源：http://blog.hesvh.cn/Article/details/gjfucazov.sHtML

[Q03] 增加列
来源：http://www.share.hesvh.cn/Article/details/ghxovbdup.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.hesvh.cn/Article/details/gkttvznwk.sHtML

[Q04] 修改列类型
来源：http://3g.fehbvm.com/Article/details/gwexdivhb.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.blog.zdbjq.cn/Article/details/gglbewmvd.sHtML

[Q05] 重命名列
来源：http://www.m.share.hesvh.cn/Article/details/gerdbilgy.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://3g.zdbjq.cn/Article/details/gmmeifqhd.sHtML

[Q06] 删除列
来源：http://3g.hesvh.cn/Article/details/ghmzyvdxx.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://wap.fehbvm.com/Article/details/gfscrobji.sHtML

[Q07] 删除表
来源：http://baike.zdbjq.cn/Article/details/geafdxjzd.sHtML

DROP TABLE IF EXISTS orders;
来源：http://read.share.zdbjq.cn/Article/details/grvntzbxe.sHtML

[Q08] 创建普通索引
来源：http://mobile.hesvh.cn/Article/details/gvkshxvpd.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://m.share.zdbjq.cn/Article/details/gklhxnhyg.sHtML

[Q09] 创建唯一索引
来源：http://baike.hesvh.cn/Article/details/gidlgnzgv.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.blog.hesvh.cn/Article/details/gbbvotcqc.sHtML

[Q10] 插入单行
来源：http://baike.zdbjq.cn/Article/details/gchhqkdlp.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mobile.hesvh.cn/Article/details/goibchbos.sHtML

[Q11] 一次插入多行
来源：http://3g.hesvh.cn/Article/details/gleqywrgl.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.share.fehbvm.com/Article/details/gybpnnghk.sHtML

[Q12] 插入后取自增 ID
来源：http://www.m.share.fehbvm.com/Article/details/gslsehqql.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.blog.hesvh.cn/Article/details/gmivdxetm.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.blog.fehbvm.com/Article/details/ggiuaqryt.sHtML

[Q13] 忽略重复插入
来源：http://3g.fehbvm.com/Article/details/glrdunpwy.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mobile.fehbvm.com/Article/details/gzewlkoai.sHtML

[Q14] 存在则更新（upsert）
来源：http://3g.zdbjq.cn/Article/details/gttjnmmco.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.m.share.hesvh.cn/Article/details/guditxrwy.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://read.share.zdbjq.cn/Article/details/gionwrgns.sHtML

[Q15] 查询全部
来源：http://mobile.hesvh.cn/Article/details/ggmmddzcz.sHtML

SELECT * FROM users;
来源：http://baike.fehbvm.com/Article/details/gysqcwfsu.sHtML

[Q16] 查询指定列
来源：http://m.share.zdbjq.cn/Article/details/gumursplj.sHtML

SELECT id, name FROM users;
来源：http://baike.zdbjq.cn/Article/details/gppebioil.sHtML

[Q17] 条件查询
来源：http://blog.fehbvm.com/Article/details/gjnitlows.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mobile.zdbjq.cn/Article/details/geoxexpop.sHtML

[Q18] 模糊匹配
来源：http://www.blog.fehbvm.com/Article/details/gsoqlwdyy.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.zdbjq.cn/Article/details/goszqvlhl.sHtML

[Q19] 范围查询
来源：http://m.share.hesvh.cn/Article/details/grfcqnnph.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.share.zdbjq.cn/Article/details/gkcxustio.sHtML

[Q20] IN 列表
来源：http://m.share.hesvh.cn/Article/details/gxghbiuqh.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wap.fehbvm.com/Article/details/gfmvfsasj.sHtML

[Q21] 空值判断
来源：http://3g.zdbjq.cn/Article/details/gkxfasuqn.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://3g.hesvh.cn/Article/details/gswqghlmz.sHtML

[Q22] 排序
来源：http://baike.hesvh.cn/Article/details/gujfcxegg.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://read.share.zdbjq.cn/Article/details/gyucfxrzp.sHtML

[Q23] 分页
来源：http://blog.hesvh.cn/Article/details/gpeqpowoy.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.m.share.zdbjq.cn/Article/details/gkhkuvayx.sHtML

[Q24] 去重
来源：http://baike.zdbjq.cn/Article/details/gvmvzhyqb.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gwrvxbqdr.sHtML

[Q25] 只取前 N 条
来源：http://www.blog.zdbjq.cn/Article/details/gxgeiwsnk.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mobile.fehbvm.com/Article/details/ghrvcifub.sHtML

[Q26] 计数
来源：http://baike.hesvh.cn/Article/details/glxfjwiww.sHtML

SELECT COUNT(*) FROM users;
来源：http://m.share.fehbvm.com/Article/details/gccdjjtak.sHtML

[Q27] 条件计数
来源：http://3g.hesvh.cn/Article/details/gpmpmgnuj.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://m.share.fehbvm.com/Article/details/goiznfdqj.sHtML

[Q28] 求和与平均
来源：http://www.blog.fehbvm.com/Article/details/ghuniinox.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.hesvh.cn/Article/details/gkvvjxboq.sHtML

[Q29] 最大最小值
来源：http://m.share.hesvh.cn/Article/details/ghmujzmru.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://blog.zdbjq.cn/Article/details/gevkpcvfu.sHtML

[Q30] 分组统计
来源：http://blog.hesvh.cn/Article/details/gdxxputhn.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mobile.zdbjq.cn/Article/details/gqjqpenqu.sHtML

[Q31] 分组后过滤
来源：http://blog.fehbvm.com/Article/details/guieovsop.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mobile.fehbvm.com/Article/details/gugvezdgx.sHtML

[Q32] 分组拼接字符串
来源：http://m.share.fehbvm.com/Article/details/giodxmhod.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://blog.zdbjq.cn/Article/details/gkywqhidl.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.fehbvm.com/Article/details/gfiuhtzri.sHtML

[Q33] 多列分组
来源：http://baike.fehbvm.com/Article/details/gtiwduheq.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.share.zdbjq.cn/Article/details/gtczobzvk.sHtML

[Q34] 每组取第一条
来源：http://www.blog.hesvh.cn/Article/details/gpjmaezev.sHtML

SELECT * FROM (
来源：http://baike.fehbvm.com/Article/details/glakmvhmo.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.hesvh.cn/Article/details/gkrahlbpb.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gvsoystdm.sHtML

[Q35] 内连接
来源：http://mobile.fehbvm.com/Article/details/gsdcfxdkg.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.fehbvm.com/Article/details/gychioisq.sHtML

[Q36] 左连接
来源：http://3g.fehbvm.com/Article/details/gwynmavaf.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://m.share.zdbjq.cn/Article/details/gbnmqrilk.sHtML

[Q37] 右连接
来源：http://mobile.zdbjq.cn/Article/details/gjmegyxgx.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://m.share.hesvh.cn/Article/details/gzeqiqlvn.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://3g.zdbjq.cn/Article/details/gqclimyha.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.hesvh.cn/Article/details/gggrqrodi.sHtML

[Q39] 自连接（查上下级）
来源：http://read.share.hesvh.cn/Article/details/gmqdfjqfi.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.m.share.fehbvm.com/Article/details/gburfqtto.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.hesvh.cn/Article/details/gjzwdfqrx.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.blog.fehbvm.com/Article/details/gwreuqppv.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.zdbjq.cn/Article/details/glnsteaqk.sHtML

[Q41] 多表连接
来源：http://www.share.hesvh.cn/Article/details/gopjijwgg.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.zdbjq.cn/Article/details/glzzvefij.sHtML

JOIN users u ON u.id = o.user_id
来源：http://3g.hesvh.cn/Article/details/gdfnlcuny.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://blog.hesvh.cn/Article/details/gtegvnjmh.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.fehbvm.com/Article/details/gxeakfabj.sHtML

SELECT u.name, o.amount FROM users u
来源：http://3g.fehbvm.com/Article/details/gjmdibrmi.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.hesvh.cn/Article/details/gkveobiku.sHtML

[Q43] 标量子查询
来源：http://m.share.hesvh.cn/Article/details/gsgaxfrsm.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.m.share.zdbjq.cn/Article/details/gzbfsrsad.sHtML

[Q44] IN 子查询
来源：http://m.share.zdbjq.cn/Article/details/gpldhhiua.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.fehbvm.com/Article/details/gddahcxfx.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.fehbvm.com/Article/details/gkmscazne.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.hesvh.cn/Article/details/gclttqmdp.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.hesvh.cn/Article/details/gsbtwltqf.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.fehbvm.com/Article/details/gzuujztgs.sHtML

[Q47] 与平均值比较
来源：http://read.share.fehbvm.com/Article/details/gkkfbxehc.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.share.fehbvm.com/Article/details/gtagszxan.sHtML

[Q48] CTE 公用表表达式
来源：http://www.share.fehbvm.com/Article/details/gmdbrghvj.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.share.zdbjq.cn/Article/details/grzdhforz.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://baike.zdbjq.cn/Article/details/gzcdlisgs.sHtML

[Q49] 更新单行
来源：http://www.blog.zdbjq.cn/Article/details/guxpznkii.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.zdbjq.cn/Article/details/giontbvad.sHtML

[Q50] 批量更新
来源：http://blog.zdbjq.cn/Article/details/gaiqvlhuq.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.share.zdbjq.cn/Article/details/gmogizunj.sHtML

[Q51] 用子查询更新
来源：http://read.share.hesvh.cn/Article/details/giatnyemi.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://3g.hesvh.cn/Article/details/gftvrbtdz.sHtML

[Q52] 删除指定行
来源：http://wap.hesvh.cn/Article/details/gllhajcfp.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.hesvh.cn/Article/details/grattudwf.sHtML

[Q53] 按条件删除
来源：http://read.share.fehbvm.com/Article/details/gtsbreikn.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://m.share.zdbjq.cn/Article/details/gbdspdjsi.sHtML

[Q54] 清空表
来源：http://read.share.fehbvm.com/Article/details/guuybnyst.sHtML

TRUNCATE TABLE logs;
来源：http://www.share.hesvh.cn/Article/details/gmiqehffu.sHtML

[Q55] 排名（并列占位）
来源：http://baike.zdbjq.cn/Article/details/gipgbpvhp.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.zdbjq.cn/Article/details/gynssaful.sHtML

[Q56] 密集排名（并列不占位）
来源：http://mobile.hesvh.cn/Article/details/gcjlqdhgm.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.fehbvm.com/Article/details/ghqpfpelf.sHtML

[Q57] 行号
来源：http://mobile.zdbjq.cn/Article/details/gnsuefydb.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.hesvh.cn/Article/details/giowecdom.sHtML

[Q58] 累计求和
来源：http://baike.fehbvm.com/Article/details/gyqljzsag.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.fehbvm.com/Article/details/gnbzliixj.sHtML

[Q59] 分组内累计
来源：http://blog.fehbvm.com/Article/details/gmssacezf.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/giyuyvzpk.sHtML

[Q60] 取上一行 / 下一行
来源：http://blog.hesvh.cn/Article/details/gnqvroupd.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.m.share.zdbjq.cn/Article/details/gpwgycnng.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gqhoxzxpr.sHtML

[Q61] 移动平均
来源：http://3g.hesvh.cn/Article/details/gpmvipxey.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://blog.fehbvm.com/Article/details/gynmcbnrr.sHtML

[Q62] 分组占比
来源：http://baike.zdbjq.cn/Article/details/gmxurlqmw.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://baike.zdbjq.cn/Article/details/gghfvmtez.sHtML

[Q63] 开启事务
来源：http://3g.zdbjq.cn/Article/details/gkbmokoou.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://3g.hesvh.cn/Article/details/ggkefykxx.sHtML

[Q64] 提交事务
来源：http://baike.hesvh.cn/Article/details/gtrhsrmho.sHtML

COMMIT;
来源：http://read.share.zdbjq.cn/Article/details/gjbmrkhle.sHtML

[Q65] 回滚事务
来源：http://wap.fehbvm.com/Article/details/gnnibrfqx.sHtML

ROLLBACK;
来源：http://wap.zdbjq.cn/Article/details/geltetvdr.sHtML

[Q66] 行锁查询
来源：http://m.share.fehbvm.com/Article/details/gbsscyhze.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://blog.fehbvm.com/Article/details/gdomtwjff.sHtML

[Q67] 设置隔离级别
来源：http://mobile.hesvh.cn/Article/details/gywrbcggx.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.fehbvm.com/Article/details/gmcuduvgk.sHtML

[Q68] 保存点
来源：http://baike.fehbvm.com/Article/details/glgqxoper.sHtML

SAVEPOINT sp1;
来源：http://www.share.fehbvm.com/Article/details/ggusvcxnu.sHtML

ROLLBACK TO sp1;
来源：http://wap.fehbvm.com/Article/details/gwchuidkm.sHtML

[Q69] 查看执行计划
来源：http://3g.zdbjq.cn/Article/details/gjpwsqvzs.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.m.share.hesvh.cn/Article/details/gycqddcom.sHtML

[Q70] 更新统计信息
来源：http://m.share.zdbjq.cn/Article/details/goonokihk.sHtML

ANALYZE TABLE users;
来源：http://www.blog.fehbvm.com/Article/details/gdxgybghg.sHtML

[Q71] 查看建表语句
来源：http://m.share.zdbjq.cn/Article/details/ggdwszaem.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wap.zdbjq.cn/Article/details/gdiyuvbym.sHtML

[Q72] 查看索引
来源：http://wap.fehbvm.com/Article/details/glpmjvpse.sHtML

SHOW INDEX FROM users;
来源：http://blog.zdbjq.cn/Article/details/gvewaenoo.sHtML

[Q73] 查看表状态
来源：http://m.share.zdbjq.cn/Article/details/grwtzqosm.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.zdbjq.cn/Article/details/gbygtkhyt.sHtML

[Q74] 强制使用索引
来源：http://www.blog.fehbvm.com/Article/details/gniuvdrij.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.fehbvm.com/Article/details/gzhijreqy.sHtML

[Q75] 日期格式化
来源：http://m.share.fehbvm.com/Article/details/gnyjpmznl.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gtsfyxcmz.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.blog.zdbjq.cn/Article/details/gpdkopnhs.sHtML

[Q76] 按天统计
来源：http://www.share.zdbjq.cn/Article/details/gfnvcfctg.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.fehbvm.com/Article/details/guvlzyien.sHtML

[Q77] 时间加减
来源：http://www.m.share.zdbjq.cn/Article/details/gndpeyvep.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.hesvh.cn/Article/details/gnuxprvof.sHtML

[Q78] 当前时间
来源：http://www.share.fehbvm.com/Article/details/gpfrxfdsc.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.fehbvm.com/Article/details/gqbwavasv.sHtML

[Q79] 字符串拼接
来源：http://baike.zdbjq.cn/Article/details/gsgbcdvld.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.zdbjq.cn/Article/details/gyavypzao.sHtML


<!-- 参考信息 -->