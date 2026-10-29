代发 wailian999

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://read.share.fehbvm.com/Article/details/gwzdwozjm.sHtML

[O03] 加锁保护共享数据
来源：http://3g.hesvh.cn/Article/details/gxumjobse.sHtML

Py:   with lock: shared += 1
来源：http://www.share.hesvh.cn/Article/details/gvclhmpbu.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.share.hesvh.cn/Article/details/gzdgdfbnn.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mobile.hesvh.cn/Article/details/gmhcmmbfu.sHtML

TS:   // 同 JS
来源：http://baike.zdbjq.cn/Article/details/gpzxvzskf.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.share.fehbvm.com/Article/details/gvjbopeqh.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.zdbjq.cn/Article/details/gjtrihmha.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://blog.hesvh.cn/Article/details/gcdcaajvf.sHtML

C#:   lock (gate) { shared++; }
来源：http://blog.zdbjq.cn/Article/details/gttureeai.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.hesvh.cn/Article/details/gkgwaigtp.sHtML

Py:   async def f():⏎    await g()
来源：http://3g.hesvh.cn/Article/details/giuvkafpc.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.hesvh.cn/Article/details/gvbssiksz.sHtML

JS:   async function f() { await g(); }
来源：http://blog.zdbjq.cn/Article/details/gwfxcyavt.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.m.share.fehbvm.com/Article/details/gulfwlaft.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://baike.fehbvm.com/Article/details/gkbojnpat.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://3g.hesvh.cn/Article/details/gsmrqrbst.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.zdbjq.cn/Article/details/gnzdtwzad.sHtML

C#:   async Task F() { await G(); }
来源：http://baike.zdbjq.cn/Article/details/gytxuqakc.sHtML

[O05] 并发执行并等待全部完成
来源：http://blog.fehbvm.com/Article/details/ggrwcascn.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.fehbvm.com/Article/details/gnatbzvdl.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mobile.fehbvm.com/Article/details/gairpuxle.sHtML

JS:   await Promise.all(tasks)
来源：http://read.share.fehbvm.com/Article/details/gnfinxwzi.sHtML

TS:   await Promise.all(tasks)
来源：http://baike.zdbjq.cn/Article/details/gcojybalg.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://blog.zdbjq.cn/Article/details/gujynwqtd.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wap.hesvh.cn/Article/details/gmqztmola.sHtML

Ruby: threads.map(&:join)
来源：http://mobile.fehbvm.com/Article/details/gnfpvrgub.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.blog.hesvh.cn/Article/details/gtutushlg.sHtML

[O06] 使用进程池
来源：http://wap.fehbvm.com/Article/details/gcmivrftn.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://read.share.zdbjq.cn/Article/details/gmnrfqfbg.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://read.share.fehbvm.com/Article/details/gvgzxnahk.sHtML

JS:   // child_process / cluster 模块
来源：http://wap.hesvh.cn/Article/details/goysqvltq.sHtML

TS:   // child_process / cluster 模块
来源：http://www.blog.fehbvm.com/Article/details/gkqymwcah.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mobile.fehbvm.com/Article/details/gmjinodfw.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://read.share.fehbvm.com/Article/details/gmelnzbik.sHtML

Ruby: // fork 块
来源：http://m.share.zdbjq.cn/Article/details/gossaoxue.sHtML

C#:   Parallel.For
来源：http://wap.zdbjq.cn/Article/details/gxbnjhods.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gyfgmnafj.sHtML

P. 常用工具函数
来源：http://3g.zdbjq.cn/Article/details/gpumfuppn.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gfwwcmpiy.sHtML

[P01] 生成 UUID
来源：http://blog.hesvh.cn/Article/details/gzhwfoypo.sHtML

Py:   str(uuid.uuid4())
来源：http://read.share.zdbjq.cn/Article/details/gkhvqskof.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://3g.fehbvm.com/Article/details/gqdpbbfuw.sHtML

JS:   crypto.randomUUID()
来源：http://blog.hesvh.cn/Article/details/ggjfgtrrj.sHtML

TS:   crypto.randomUUID()
来源：http://read.share.zdbjq.cn/Article/details/gegsbcqwu.sHtML

Java: UUID.randomUUID().toString()
来源：http://blog.fehbvm.com/Article/details/gfwmtwrxz.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.hesvh.cn/Article/details/giptxlahd.sHtML

Ruby: SecureRandom.uuid
来源：http://mobile.hesvh.cn/Article/details/gxorkouve.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://read.share.zdbjq.cn/Article/details/gmxdacnbj.sHtML

[P02] MD5 / SHA256 摘要
来源：http://blog.zdbjq.cn/Article/details/grtwfcppx.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://blog.hesvh.cn/Article/details/gqrjyrdgi.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://3g.hesvh.cn/Article/details/gziugqesq.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://3g.hesvh.cn/Article/details/gfkbnqyor.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://blog.hesvh.cn/Article/details/ghnpsghze.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mobile.fehbvm.com/Article/details/gssjfszuu.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.share.zdbjq.cn/Article/details/ginoxdaog.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gzmbkuksg.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.share.hesvh.cn/Article/details/gcuafnuxl.sHtML

[P03] 生成短随机字符串
来源：http://www.blog.zdbjq.cn/Article/details/geroqttpr.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.share.hesvh.cn/Article/details/gwrhsyzjq.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://m.share.fehbvm.com/Article/details/gfzbdpaub.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.fehbvm.com/Article/details/gciyacslf.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.hesvh.cn/Article/details/ggjnvugim.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mobile.fehbvm.com/Article/details/glftygwva.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mobile.zdbjq.cn/Article/details/gptuntkmu.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://baike.zdbjq.cn/Article/details/gcsseeggh.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.blog.zdbjq.cn/Article/details/gfclkrzni.sHtML

[P04] 求长度
来源：http://mobile.fehbvm.com/Article/details/ghkiotsab.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wap.zdbjq.cn/Article/details/gcoxbucwt.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.zdbjq.cn/Article/details/gxdtrogzy.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.fehbvm.com/Article/details/gqxawiedz.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.hesvh.cn/Article/details/gaylqbdgd.sHtML

Java: list.size();  map.size();  s.length()
来源：http://baike.hesvh.cn/Article/details/gjgftonaq.sHtML

Go:   len(arr);  len(m)
来源：http://blog.hesvh.cn/Article/details/gfjclvuun.sHtML

Ruby: x.length;  x.size
来源：http://www.blog.zdbjq.cn/Article/details/gwijdlket.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.m.share.fehbvm.com/Article/details/gdxxiaynx.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.m.share.hesvh.cn/Article/details/giaoprltr.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://3g.fehbvm.com/Article/details/gggqvyakh.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wap.hesvh.cn/Article/details/gkrbhldzc.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://read.share.fehbvm.com/Article/details/gatydduud.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.hesvh.cn/Article/details/gbkcvrydf.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.m.share.fehbvm.com/Article/details/gusxchauk.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.zdbjq.cn/Article/details/gorwgpfza.sHtML

Ruby: a == b
来源：http://read.share.fehbvm.com/Article/details/gjhnbulaf.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://m.share.fehbvm.com/Article/details/gjvuywgtp.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://blog.hesvh.cn/Article/details/geyjjcwhg.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://3g.fehbvm.com/Article/details/gtfwxfmpn.sHtML

PHP:  if (empty($x)) {}
来源：http://3g.zdbjq.cn/Article/details/gtxpfnrqb.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.share.fehbvm.com/Article/details/ghjznsmzf.sHtML

TS:   if (x == null) {}
来源：http://read.share.zdbjq.cn/Article/details/glrmycnom.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://m.share.zdbjq.cn/Article/details/gyxwuxfpc.sHtML

Go:   if x == nil {}
来源：http://blog.fehbvm.com/Article/details/goedzwfgq.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.m.share.hesvh.cn/Article/details/gbueqtlis.sHtML

C#:   if (x is null) {}
来源：http://blog.hesvh.cn/Article/details/gsdbiaoit.sHtML

[P07] 防抖与节流
来源：http://baike.zdbjq.cn/Article/details/gmgefjcno.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.share.fehbvm.com/Article/details/gaeozawtw.sHtML

PHP:  // 手写时间戳比较
来源：http://read.share.hesvh.cn/Article/details/gmmayggfn.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.zdbjq.cn/Article/details/gtkzomzwf.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.hesvh.cn/Article/details/gizsztqjo.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.share.hesvh.cn/Article/details/gszxxaxqq.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wap.zdbjq.cn/Article/details/gmminklob.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://baike.zdbjq.cn/Article/details/gphldwffp.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://read.share.hesvh.cn/Article/details/gztyneulo.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.hesvh.cn/Article/details/gasppzabf.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://read.share.zdbjq.cn/Article/details/goyuwnopt.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.fehbvm.com/Article/details/glaczemfv.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.hesvh.cn/Article/details/gmqhcpvoi.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.m.share.zdbjq.cn/Article/details/gmboanwbj.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://blog.fehbvm.com/Article/details/gscqyeiqv.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.share.zdbjq.cn/Article/details/gfmnfegep.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://m.share.hesvh.cn/Article/details/gjhahiapa.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wap.zdbjq.cn/Article/details/gcygyxksc.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gginbufak.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://baike.zdbjq.cn/Article/details/ghswwhzch.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gzlnxfead.sHtML

[Q01] 创建表
来源：http://www.blog.hesvh.cn/Article/details/gmalzjqyi.sHtML

CREATE TABLE users (
来源：http://blog.hesvh.cn/Article/details/gntskthmy.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.hesvh.cn/Article/details/gzaxxibjf.sHtML

name VARCHAR(50) NOT NULL,
来源：http://3g.hesvh.cn/Article/details/giukkjhmc.sHtML

email VARCHAR(100) UNIQUE,
来源：http://3g.fehbvm.com/Article/details/gohwgjhux.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wap.fehbvm.com/Article/details/gvnqlwobv.sHtML

);
来源：http://www.m.share.hesvh.cn/Article/details/gocmtnbau.sHtML

[Q02] 创建带外键的表
来源：http://wap.hesvh.cn/Article/details/gytddpemp.sHtML

CREATE TABLE orders (
来源：http://www.blog.fehbvm.com/Article/details/gmsblkwht.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.zdbjq.cn/Article/details/gynkyfxiw.sHtML

user_id INT NOT NULL,
来源：http://baike.fehbvm.com/Article/details/gaqmivamj.sHtML

amount DECIMAL(10, 2),
来源：http://3g.zdbjq.cn/Article/details/gtdqlupvo.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.blog.zdbjq.cn/Article/details/gukojdqkn.sHtML

);
来源：http://m.share.zdbjq.cn/Article/details/ggkxrkjtr.sHtML

[Q03] 增加列
来源：http://3g.fehbvm.com/Article/details/gkmofndut.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://read.share.fehbvm.com/Article/details/gzaqcqftu.sHtML

[Q04] 修改列类型
来源：http://blog.zdbjq.cn/Article/details/gbrvydtln.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://m.share.hesvh.cn/Article/details/gvrsdvdjv.sHtML

[Q05] 重命名列
来源：http://www.share.zdbjq.cn/Article/details/gviqihprd.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://m.share.zdbjq.cn/Article/details/gjfrzcpya.sHtML

[Q06] 删除列
来源：http://mobile.zdbjq.cn/Article/details/gzyfpxiyc.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://3g.zdbjq.cn/Article/details/gkrflvsql.sHtML

[Q07] 删除表
来源：http://www.m.share.zdbjq.cn/Article/details/gwdlagojs.sHtML

DROP TABLE IF EXISTS orders;
来源：http://m.share.zdbjq.cn/Article/details/gdmizdaii.sHtML

[Q08] 创建普通索引
来源：http://read.share.zdbjq.cn/Article/details/gvcyofpun.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.blog.zdbjq.cn/Article/details/gaxxrvwqv.sHtML

[Q09] 创建唯一索引
来源：http://www.share.hesvh.cn/Article/details/gyxtdphvc.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://read.share.fehbvm.com/Article/details/gffslbxyi.sHtML

[Q10] 插入单行
来源：http://www.m.share.zdbjq.cn/Article/details/ggbrojopz.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.share.fehbvm.com/Article/details/gdkbyfhoc.sHtML

[Q11] 一次插入多行
来源：http://wap.hesvh.cn/Article/details/gtdirssxr.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wap.hesvh.cn/Article/details/gwyrexwlg.sHtML

[Q12] 插入后取自增 ID
来源：http://3g.zdbjq.cn/Article/details/gnrzfrjya.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://wap.fehbvm.com/Article/details/gkaemikam.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.m.share.zdbjq.cn/Article/details/gkkmujnvd.sHtML

[Q13] 忽略重复插入
来源：http://www.m.share.hesvh.cn/Article/details/gcaagqroa.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://read.share.fehbvm.com/Article/details/gpccusflc.sHtML

[Q14] 存在则更新（upsert）
来源：http://3g.fehbvm.com/Article/details/gvgvyxtwe.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://blog.zdbjq.cn/Article/details/gzdqacjgj.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://baike.fehbvm.com/Article/details/girlqfkyc.sHtML

[Q15] 查询全部
来源：http://baike.fehbvm.com/Article/details/godobsrnr.sHtML

SELECT * FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gbcsodowt.sHtML

[Q16] 查询指定列
来源：http://blog.hesvh.cn/Article/details/gailvaqsb.sHtML

SELECT id, name FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gazielbfr.sHtML

[Q17] 条件查询
来源：http://www.blog.fehbvm.com/Article/details/gtafvixlo.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://3g.fehbvm.com/Article/details/gsnptqnqg.sHtML

[Q18] 模糊匹配
来源：http://blog.fehbvm.com/Article/details/gpankiyrq.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wap.hesvh.cn/Article/details/gkpuzbksm.sHtML

[Q19] 范围查询
来源：http://www.blog.hesvh.cn/Article/details/gaumxqhqa.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.share.fehbvm.com/Article/details/gxytirerr.sHtML

[Q20] IN 列表
来源：http://baike.hesvh.cn/Article/details/gnplgmypj.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://baike.hesvh.cn/Article/details/ggumlcvou.sHtML

[Q21] 空值判断
来源：http://mobile.zdbjq.cn/Article/details/gpnnntabw.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.share.zdbjq.cn/Article/details/gaumredth.sHtML

[Q22] 排序
来源：http://blog.zdbjq.cn/Article/details/gkuzvrutq.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.blog.hesvh.cn/Article/details/gmpiijbup.sHtML

[Q23] 分页
来源：http://baike.hesvh.cn/Article/details/gpnancwlt.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mobile.fehbvm.com/Article/details/gisncodzq.sHtML

[Q24] 去重
来源：http://mobile.fehbvm.com/Article/details/gjgyobjew.sHtML

SELECT DISTINCT city FROM users;
来源：http://wap.hesvh.cn/Article/details/gxyciezcw.sHtML

[Q25] 只取前 N 条
来源：http://www.blog.hesvh.cn/Article/details/gzjadgtlp.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.fehbvm.com/Article/details/gwszqoyyn.sHtML

[Q26] 计数
来源：http://m.share.hesvh.cn/Article/details/gvhhpdgwh.sHtML

SELECT COUNT(*) FROM users;
来源：http://3g.hesvh.cn/Article/details/gtdrskacc.sHtML

[Q27] 条件计数
来源：http://www.share.zdbjq.cn/Article/details/gszdieclu.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gbownqlah.sHtML

[Q28] 求和与平均
来源：http://baike.fehbvm.com/Article/details/ghrugevfc.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://3g.hesvh.cn/Article/details/gunvbrnyc.sHtML

[Q29] 最大最小值
来源：http://read.share.zdbjq.cn/Article/details/ghlvgwipy.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gnbtafczg.sHtML

[Q30] 分组统计
来源：http://baike.fehbvm.com/Article/details/ghgelsczd.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.blog.zdbjq.cn/Article/details/glvgsbmjr.sHtML

[Q31] 分组后过滤
来源：http://www.blog.zdbjq.cn/Article/details/grgjbaspz.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wap.fehbvm.com/Article/details/geqxntnuf.sHtML

[Q32] 分组拼接字符串
来源：http://blog.fehbvm.com/Article/details/gabchxcye.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://blog.hesvh.cn/Article/details/gxrzzpbyj.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://baike.hesvh.cn/Article/details/gpcrspzgs.sHtML

[Q33] 多列分组
来源：http://mobile.hesvh.cn/Article/details/gawggqfok.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://blog.hesvh.cn/Article/details/gpkboyezw.sHtML

[Q34] 每组取第一条
来源：http://www.m.share.fehbvm.com/Article/details/gnoftofov.sHtML

SELECT * FROM (
来源：http://www.m.share.hesvh.cn/Article/details/gynhbycfw.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://baike.hesvh.cn/Article/details/gepfzpwds.sHtML

) t WHERE rn = 1;
来源：http://www.blog.zdbjq.cn/Article/details/gcyseexxt.sHtML

[Q35] 内连接
来源：http://blog.fehbvm.com/Article/details/gvnwkpboq.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.zdbjq.cn/Article/details/gpddlivsc.sHtML

[Q36] 左连接
来源：http://read.share.hesvh.cn/Article/details/gevswoowz.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://read.share.hesvh.cn/Article/details/gujgiubbd.sHtML

[Q37] 右连接
来源：http://wap.fehbvm.com/Article/details/ghsktoewj.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.share.fehbvm.com/Article/details/gyivhexev.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://wap.fehbvm.com/Article/details/ghvciiefc.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mobile.hesvh.cn/Article/details/gosswkank.sHtML

[Q39] 自连接（查上下级）
来源：http://baike.zdbjq.cn/Article/details/gnyydocym.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.fehbvm.com/Article/details/gjnrgavzt.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://baike.hesvh.cn/Article/details/gqcvoxjkz.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.hesvh.cn/Article/details/gcwtqmhoi.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://3g.fehbvm.com/Article/details/gesgpjhwy.sHtML

[Q41] 多表连接
来源：http://wap.fehbvm.com/Article/details/gvjyywixj.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.hesvh.cn/Article/details/gfgusmumt.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.share.hesvh.cn/Article/details/gzafqaovz.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://blog.fehbvm.com/Article/details/gpgtbepdk.sHtML

[Q42] 连接条件附加过滤
来源：http://wap.hesvh.cn/Article/details/gscemdnfw.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.zdbjq.cn/Article/details/gcjvpwrnh.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.hesvh.cn/Article/details/gqemlseah.sHtML

[Q43] 标量子查询
来源：http://3g.fehbvm.com/Article/details/ggqumyjzv.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.blog.fehbvm.com/Article/details/ggnabsruq.sHtML

[Q44] IN 子查询
来源：http://3g.zdbjq.cn/Article/details/gpmrlbxgb.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mobile.hesvh.cn/Article/details/gkmmfrooc.sHtML

[Q45] EXISTS 判断存在
来源：http://wap.zdbjq.cn/Article/details/gptuncfrr.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.fehbvm.com/Article/details/gwgvlmdiu.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.m.share.zdbjq.cn/Article/details/gjzabxskw.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.hesvh.cn/Article/details/gcohwvthl.sHtML

[Q47] 与平均值比较
来源：http://baike.hesvh.cn/Article/details/gkzzqooye.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.share.hesvh.cn/Article/details/ghyhtjmlx.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.fehbvm.com/Article/details/gviacpqjr.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.blog.zdbjq.cn/Article/details/ghikgullm.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://wap.hesvh.cn/Article/details/gwjcrvvlx.sHtML

[Q49] 更新单行
来源：http://wap.fehbvm.com/Article/details/gqgejptoq.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://3g.zdbjq.cn/Article/details/gqcqpowzs.sHtML

[Q50] 批量更新
来源：http://read.share.fehbvm.com/Article/details/grzzuzceq.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.m.share.zdbjq.cn/Article/details/ghatdvumw.sHtML

[Q51] 用子查询更新
来源：http://www.share.hesvh.cn/Article/details/gdgtxfayw.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.share.hesvh.cn/Article/details/gspeyvcyr.sHtML

[Q52] 删除指定行
来源：http://www.share.zdbjq.cn/Article/details/gvuvqagvm.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.hesvh.cn/Article/details/ggbtkusut.sHtML

[Q53] 按条件删除
来源：http://read.share.hesvh.cn/Article/details/guukczygx.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.fehbvm.com/Article/details/ghrpmdupb.sHtML

[Q54] 清空表
来源：http://www.share.zdbjq.cn/Article/details/gozizldda.sHtML

TRUNCATE TABLE logs;
来源：http://www.blog.zdbjq.cn/Article/details/gragexzmv.sHtML

[Q55] 排名（并列占位）
来源：http://www.m.share.fehbvm.com/Article/details/gdokrfcts.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.share.zdbjq.cn/Article/details/gyvpqgqlc.sHtML

[Q56] 密集排名（并列不占位）
来源：http://3g.zdbjq.cn/Article/details/ghyhcztyl.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.fehbvm.com/Article/details/gjdbgipme.sHtML

[Q57] 行号
来源：http://3g.zdbjq.cn/Article/details/gwxshplpf.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.hesvh.cn/Article/details/gvqwqkzfn.sHtML

[Q58] 累计求和
来源：http://www.blog.hesvh.cn/Article/details/gylcpwlyn.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/gecxcfnna.sHtML

[Q59] 分组内累计
来源：http://blog.fehbvm.com/Article/details/gbmibswnc.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://blog.zdbjq.cn/Article/details/gxylkuduq.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.hesvh.cn/Article/details/gvtxymwzs.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.fehbvm.com/Article/details/gwiwgyisp.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.zdbjq.cn/Article/details/ghhglrqlj.sHtML

[Q61] 移动平均
来源：http://3g.zdbjq.cn/Article/details/gjydpbtzs.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/goqssrqlt.sHtML

[Q62] 分组占比
来源：http://read.share.zdbjq.cn/Article/details/gqewzgqto.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.zdbjq.cn/Article/details/gwkysprdb.sHtML

[Q63] 开启事务
来源：http://3g.zdbjq.cn/Article/details/gampzsxoj.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://3g.zdbjq.cn/Article/details/gkekkpdhd.sHtML

[Q64] 提交事务
来源：http://m.share.fehbvm.com/Article/details/gioidhsqd.sHtML

COMMIT;
来源：http://baike.zdbjq.cn/Article/details/gotvapapp.sHtML

[Q65] 回滚事务
来源：http://mobile.fehbvm.com/Article/details/gfaxbwarw.sHtML

ROLLBACK;
来源：http://www.m.share.zdbjq.cn/Article/details/gmynxttuc.sHtML

[Q66] 行锁查询
来源：http://read.share.zdbjq.cn/Article/details/gsudmoirr.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wap.zdbjq.cn/Article/details/gzuwiaktl.sHtML

[Q67] 设置隔离级别
来源：http://wap.hesvh.cn/Article/details/gzifbnkaf.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.fehbvm.com/Article/details/gjwdlfxoe.sHtML

[Q68] 保存点
来源：http://3g.hesvh.cn/Article/details/guxcsyege.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.zdbjq.cn/Article/details/gcazltzpq.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.hesvh.cn/Article/details/gordgxifp.sHtML

[Q69] 查看执行计划
来源：http://read.share.hesvh.cn/Article/details/gkcddqjor.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.zdbjq.cn/Article/details/gsllsabix.sHtML

[Q70] 更新统计信息
来源：http://baike.fehbvm.com/Article/details/gnkkpcjap.sHtML

ANALYZE TABLE users;
来源：http://www.blog.fehbvm.com/Article/details/gmlrqbnod.sHtML

[Q71] 查看建表语句
来源：http://read.share.zdbjq.cn/Article/details/goawwknbo.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.fehbvm.com/Article/details/gyqimheiz.sHtML

[Q72] 查看索引
来源：http://3g.zdbjq.cn/Article/details/guqbwkfaz.sHtML

SHOW INDEX FROM users;
来源：http://blog.zdbjq.cn/Article/details/gldeplwkn.sHtML

[Q73] 查看表状态
来源：http://www.blog.hesvh.cn/Article/details/glqxjtfrq.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.hesvh.cn/Article/details/ghhnytjez.sHtML

[Q74] 强制使用索引
来源：http://read.share.hesvh.cn/Article/details/gwgmlwpvq.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.fehbvm.com/Article/details/gnyoftqkc.sHtML

[Q75] 日期格式化
来源：http://read.share.zdbjq.cn/Article/details/gfqzegmnc.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.hesvh.cn/Article/details/gfpsvbktd.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.zdbjq.cn/Article/details/gvsvrhgts.sHtML

[Q76] 按天统计
来源：http://baike.hesvh.cn/Article/details/gsrbbirkw.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.hesvh.cn/Article/details/gygelidlx.sHtML

[Q77] 时间加减
来源：http://mobile.fehbvm.com/Article/details/gzaerbhzh.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.hesvh.cn/Article/details/ghcrcqmwy.sHtML

[Q78] 当前时间
来源：http://baike.fehbvm.com/Article/details/gbylmwbsn.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.hesvh.cn/Article/details/gqrpowwfv.sHtML

[Q79] 字符串拼接
来源：http://read.share.zdbjq.cn/Article/details/gdlhwxojq.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.hesvh.cn/Article/details/ggdzmkxtn.sHtML

[Q80] 字符串截取
来源：http://3g.hesvh.cn/Article/details/gjxsodyms.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.hesvh.cn/Article/details/gkvdxtxpg.sHtML

[Q81] 字符串替换
来源：http://baike.zdbjq.cn/Article/details/gwycjttrc.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.hesvh.cn/Article/details/gebkautao.sHtML


<!-- 参考信息 -->