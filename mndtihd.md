代发 wailian999

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.hesvh.cn/Article/details/gezvkkkuq.sHtML

[O03] 加锁保护共享数据
来源：http://m.share.zdbjq.cn/Article/details/gkkbzgwxp.sHtML

Py:   with lock: shared += 1
来源：http://m.share.hesvh.cn/Article/details/gtieuxhuq.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://3g.zdbjq.cn/Article/details/gcmatkywn.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://read.share.zdbjq.cn/Article/details/gblepjvaq.sHtML

TS:   // 同 JS
来源：http://www.share.hesvh.cn/Article/details/ghcdhcvnd.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.blog.fehbvm.com/Article/details/gtikjhgmb.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.blog.zdbjq.cn/Article/details/ghtnrsxne.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.share.zdbjq.cn/Article/details/gesdflbap.sHtML

C#:   lock (gate) { shared++; }
来源：http://wap.zdbjq.cn/Article/details/gvqctkloa.sHtML

[O04] 定义异步函数并等待
来源：http://blog.fehbvm.com/Article/details/gstzcicyw.sHtML

Py:   async def f():⏎    await g()
来源：http://read.share.hesvh.cn/Article/details/gxapkvrmv.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mobile.fehbvm.com/Article/details/gtunxgvfo.sHtML

JS:   async function f() { await g(); }
来源：http://www.share.hesvh.cn/Article/details/guizycztc.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://m.share.fehbvm.com/Article/details/gqpdsjbyb.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://read.share.fehbvm.com/Article/details/gpuwxihdt.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://blog.fehbvm.com/Article/details/ghovxfpsy.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.share.hesvh.cn/Article/details/gznkoavgg.sHtML

C#:   async Task F() { await G(); }
来源：http://m.share.zdbjq.cn/Article/details/gxfgywpkb.sHtML

[O05] 并发执行并等待全部完成
来源：http://mobile.zdbjq.cn/Article/details/gidgdzbqb.sHtML

Py:   asyncio.gather(*tasks)
来源：http://blog.hesvh.cn/Article/details/gthtfxsxy.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.blog.fehbvm.com/Article/details/gsmbyipuo.sHtML

JS:   await Promise.all(tasks)
来源：http://www.m.share.zdbjq.cn/Article/details/gjfakukbi.sHtML

TS:   await Promise.all(tasks)
来源：http://m.share.zdbjq.cn/Article/details/gkuzsoclj.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.m.share.hesvh.cn/Article/details/gwotajnza.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.m.share.zdbjq.cn/Article/details/ghykethza.sHtML

Ruby: threads.map(&:join)
来源：http://blog.hesvh.cn/Article/details/gwighfmie.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://blog.hesvh.cn/Article/details/ghdnsvvcq.sHtML

[O06] 使用进程池
来源：http://baike.hesvh.cn/Article/details/ggmisfspp.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://m.share.fehbvm.com/Article/details/gqxvpddpm.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.m.share.zdbjq.cn/Article/details/gttqeyzkn.sHtML

JS:   // child_process / cluster 模块
来源：http://baike.hesvh.cn/Article/details/gcekjwcuz.sHtML

TS:   // child_process / cluster 模块
来源：http://read.share.fehbvm.com/Article/details/gabuhunwl.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.share.zdbjq.cn/Article/details/gdsnawsgg.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://3g.fehbvm.com/Article/details/gsbbuycir.sHtML

Ruby: // fork 块
来源：http://3g.zdbjq.cn/Article/details/gwihtxybm.sHtML

C#:   Parallel.For
来源：http://www.share.zdbjq.cn/Article/details/gbyszaykr.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/goqxdrqlt.sHtML

P. 常用工具函数
来源：http://m.share.hesvh.cn/Article/details/gdkllzfbz.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gwhuwsolw.sHtML

[P01] 生成 UUID
来源：http://read.share.zdbjq.cn/Article/details/gntzrfxmn.sHtML

Py:   str(uuid.uuid4())
来源：http://www.share.zdbjq.cn/Article/details/grjvitwrm.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://baike.fehbvm.com/Article/details/gdecyqraw.sHtML

JS:   crypto.randomUUID()
来源：http://blog.zdbjq.cn/Article/details/gqpkplywb.sHtML

TS:   crypto.randomUUID()
来源：http://www.blog.zdbjq.cn/Article/details/gxjydfdxm.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.share.hesvh.cn/Article/details/gwlukzrio.sHtML

Go:   // 用 github.com/google/uuid
来源：http://read.share.fehbvm.com/Article/details/gqrdbdziu.sHtML

Ruby: SecureRandom.uuid
来源：http://baike.hesvh.cn/Article/details/gziczlsvc.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.blog.zdbjq.cn/Article/details/getelwexn.sHtML

[P02] MD5 / SHA256 摘要
来源：http://m.share.zdbjq.cn/Article/details/gvvhdfesu.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://3g.fehbvm.com/Article/details/gypfzxrbk.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://wap.hesvh.cn/Article/details/goxwfynox.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.m.share.hesvh.cn/Article/details/gmawlyhix.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.share.hesvh.cn/Article/details/gdvqnhurc.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://3g.hesvh.cn/Article/details/gnzcgmwdm.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://m.share.hesvh.cn/Article/details/gijdrvosx.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://3g.hesvh.cn/Article/details/gvorreyfz.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mobile.fehbvm.com/Article/details/gilrmghbm.sHtML

[P03] 生成短随机字符串
来源：http://mobile.zdbjq.cn/Article/details/gtemzhtjo.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://baike.fehbvm.com/Article/details/gdadcexup.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mobile.zdbjq.cn/Article/details/gcijhojns.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.hesvh.cn/Article/details/ghwtalafe.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.hesvh.cn/Article/details/gcequxcxg.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://baike.hesvh.cn/Article/details/gvalbhjrh.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.zdbjq.cn/Article/details/gjzuikrxt.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.share.hesvh.cn/Article/details/gmtnnjcyw.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.share.zdbjq.cn/Article/details/gxipgvabu.sHtML

[P04] 求长度
来源：http://blog.zdbjq.cn/Article/details/gnrvxsmah.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://m.share.zdbjq.cn/Article/details/gfkoxiiaq.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.zdbjq.cn/Article/details/grcheurbw.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.zdbjq.cn/Article/details/gscydgafd.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.fehbvm.com/Article/details/glmfuhfhn.sHtML

Java: list.size();  map.size();  s.length()
来源：http://mobile.hesvh.cn/Article/details/gbxefsuzr.sHtML

Go:   len(arr);  len(m)
来源：http://wap.fehbvm.com/Article/details/glqxvvjok.sHtML

Ruby: x.length;  x.size
来源：http://mobile.fehbvm.com/Article/details/gfmadrewh.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://read.share.hesvh.cn/Article/details/gbvbpoyxw.sHtML

[P05] 判断两个对象内容是否相等
来源：http://wap.zdbjq.cn/Article/details/gsfskpxpu.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://wap.hesvh.cn/Article/details/gznrhoqzv.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://read.share.zdbjq.cn/Article/details/gblpcriax.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.blog.fehbvm.com/Article/details/gojbanlfk.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.zdbjq.cn/Article/details/gtnpbdebe.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.blog.zdbjq.cn/Article/details/gwfcwqcsc.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://baike.zdbjq.cn/Article/details/gjsvxdyyj.sHtML

Ruby: a == b
来源：http://www.m.share.fehbvm.com/Article/details/gtoqvsiyy.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.blog.hesvh.cn/Article/details/guaoxtfot.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://baike.fehbvm.com/Article/details/gtwzfmdvj.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://3g.zdbjq.cn/Article/details/glbajrnkg.sHtML

PHP:  if (empty($x)) {}
来源：http://mobile.fehbvm.com/Article/details/ghjigotjm.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://blog.hesvh.cn/Article/details/gtjgagnks.sHtML

TS:   if (x == null) {}
来源：http://www.blog.zdbjq.cn/Article/details/ghnujnfvp.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://blog.hesvh.cn/Article/details/gjdqqdebk.sHtML

Go:   if x == nil {}
来源：http://mobile.zdbjq.cn/Article/details/ghozktikk.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.blog.zdbjq.cn/Article/details/glbwvnvfn.sHtML

C#:   if (x is null) {}
来源：http://www.share.zdbjq.cn/Article/details/gglyddstn.sHtML

[P07] 防抖与节流
来源：http://www.blog.zdbjq.cn/Article/details/guzrvjlxq.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://read.share.zdbjq.cn/Article/details/glqgsdmte.sHtML

PHP:  // 手写时间戳比较
来源：http://read.share.fehbvm.com/Article/details/ggtyhwwvy.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.hesvh.cn/Article/details/gtaghypmc.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.zdbjq.cn/Article/details/grslujyok.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.share.hesvh.cn/Article/details/gbdyvdywk.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.share.fehbvm.com/Article/details/grdtibyvb.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.blog.zdbjq.cn/Article/details/gmbysjjry.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.share.fehbvm.com/Article/details/geyghkuyb.sHtML

[P08] 处理浮点精度问题
来源：http://m.share.zdbjq.cn/Article/details/gehjbhdge.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://baike.zdbjq.cn/Article/details/gqcjpfcps.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://3g.fehbvm.com/Article/details/gnjevmrch.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.hesvh.cn/Article/details/gwztqzsak.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.m.share.fehbvm.com/Article/details/glnpsrhbz.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://read.share.zdbjq.cn/Article/details/geomtswnx.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://read.share.zdbjq.cn/Article/details/gybzveccg.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://read.share.hesvh.cn/Article/details/gsecxzrqd.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://3g.hesvh.cn/Article/details/gbwcmswit.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gcqtuujlz.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://3g.zdbjq.cn/Article/details/gqltnbaki.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gwldenvhc.sHtML

[Q01] 创建表
来源：http://blog.zdbjq.cn/Article/details/gvfkahedo.sHtML

CREATE TABLE users (
来源：http://blog.hesvh.cn/Article/details/gdytmyadu.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.hesvh.cn/Article/details/gpwaxmvrt.sHtML

name VARCHAR(50) NOT NULL,
来源：http://baike.hesvh.cn/Article/details/glzcfbbmp.sHtML

email VARCHAR(100) UNIQUE,
来源：http://3g.zdbjq.cn/Article/details/gxuvdcqaa.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.share.fehbvm.com/Article/details/gpikdrycx.sHtML

);
来源：http://wap.fehbvm.com/Article/details/gvyqroyuw.sHtML

[Q02] 创建带外键的表
来源：http://www.blog.zdbjq.cn/Article/details/gjrdanlzf.sHtML

CREATE TABLE orders (
来源：http://www.m.share.fehbvm.com/Article/details/gwnvahsoi.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.hesvh.cn/Article/details/gyxwitxmd.sHtML

user_id INT NOT NULL,
来源：http://mobile.hesvh.cn/Article/details/gfdygjabl.sHtML

amount DECIMAL(10, 2),
来源：http://www.m.share.fehbvm.com/Article/details/gefnndgkh.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.share.hesvh.cn/Article/details/gfthdetuj.sHtML

);
来源：http://read.share.hesvh.cn/Article/details/galkybufx.sHtML

[Q03] 增加列
来源：http://www.share.hesvh.cn/Article/details/gsmgwmfut.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.m.share.hesvh.cn/Article/details/gvbmrpnpe.sHtML

[Q04] 修改列类型
来源：http://blog.hesvh.cn/Article/details/ggyykvcan.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.share.hesvh.cn/Article/details/gkfswipfq.sHtML

[Q05] 重命名列
来源：http://www.share.zdbjq.cn/Article/details/gnoorsmvq.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://baike.zdbjq.cn/Article/details/grxtwtncy.sHtML

[Q06] 删除列
来源：http://blog.hesvh.cn/Article/details/gytzebwxk.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.m.share.hesvh.cn/Article/details/gkliyggec.sHtML

[Q07] 删除表
来源：http://wap.hesvh.cn/Article/details/glbbbrzsq.sHtML

DROP TABLE IF EXISTS orders;
来源：http://wap.fehbvm.com/Article/details/geegftxwn.sHtML

[Q08] 创建普通索引
来源：http://www.m.share.zdbjq.cn/Article/details/gwecodaem.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://mobile.hesvh.cn/Article/details/gthxnqwpn.sHtML

[Q09] 创建唯一索引
来源：http://blog.zdbjq.cn/Article/details/guavcfwal.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://3g.hesvh.cn/Article/details/gxflicqoy.sHtML

[Q10] 插入单行
来源：http://3g.zdbjq.cn/Article/details/gfpzvzvpm.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.blog.zdbjq.cn/Article/details/gvraxkihl.sHtML

[Q11] 一次插入多行
来源：http://mobile.hesvh.cn/Article/details/gwqrpmmeo.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.hesvh.cn/Article/details/gujkeqxmg.sHtML

[Q12] 插入后取自增 ID
来源：http://mobile.fehbvm.com/Article/details/glpsysday.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.m.share.fehbvm.com/Article/details/gxwtvpwmh.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.m.share.hesvh.cn/Article/details/gogdasfxk.sHtML

[Q13] 忽略重复插入
来源：http://3g.hesvh.cn/Article/details/gokdqmzhs.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.hesvh.cn/Article/details/gnannajoo.sHtML

[Q14] 存在则更新（upsert）
来源：http://baike.hesvh.cn/Article/details/gesyktzmd.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mobile.zdbjq.cn/Article/details/gbbmbzpep.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.fehbvm.com/Article/details/gehthtipy.sHtML

[Q15] 查询全部
来源：http://read.share.zdbjq.cn/Article/details/gotekqkce.sHtML

SELECT * FROM users;
来源：http://baike.zdbjq.cn/Article/details/gkzltpeol.sHtML

[Q16] 查询指定列
来源：http://3g.zdbjq.cn/Article/details/gxhpdeydi.sHtML

SELECT id, name FROM users;
来源：http://baike.hesvh.cn/Article/details/gjsaqizgp.sHtML

[Q17] 条件查询
来源：http://www.blog.zdbjq.cn/Article/details/gejsbvhmv.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.hesvh.cn/Article/details/gdtrhikzg.sHtML

[Q18] 模糊匹配
来源：http://mobile.hesvh.cn/Article/details/gljkmtovm.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://m.share.zdbjq.cn/Article/details/guvmcxgvr.sHtML

[Q19] 范围查询
来源：http://wap.zdbjq.cn/Article/details/gdscpkhjh.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://3g.fehbvm.com/Article/details/ggzzhfetz.sHtML

[Q20] IN 列表
来源：http://m.share.hesvh.cn/Article/details/gzxlmjtuh.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.blog.hesvh.cn/Article/details/gqyvtuxsx.sHtML

[Q21] 空值判断
来源：http://baike.fehbvm.com/Article/details/gvcocycsn.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.m.share.fehbvm.com/Article/details/gywkycqjn.sHtML

[Q22] 排序
来源：http://www.m.share.fehbvm.com/Article/details/ggijbomhk.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://blog.zdbjq.cn/Article/details/gmkgnwqtn.sHtML

[Q23] 分页
来源：http://baike.hesvh.cn/Article/details/grtwmbznl.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://m.share.zdbjq.cn/Article/details/gzblamcps.sHtML

[Q24] 去重
来源：http://www.blog.zdbjq.cn/Article/details/gnejodzie.sHtML

SELECT DISTINCT city FROM users;
来源：http://read.share.zdbjq.cn/Article/details/giqqddikn.sHtML

[Q25] 只取前 N 条
来源：http://mobile.fehbvm.com/Article/details/ggjczvixr.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://read.share.hesvh.cn/Article/details/gyofmgeea.sHtML

[Q26] 计数
来源：http://3g.fehbvm.com/Article/details/gajlybpsu.sHtML

SELECT COUNT(*) FROM users;
来源：http://wap.hesvh.cn/Article/details/grfvcfujy.sHtML

[Q27] 条件计数
来源：http://wap.hesvh.cn/Article/details/gjvvgkjdv.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://m.share.fehbvm.com/Article/details/gfbajnztd.sHtML

[Q28] 求和与平均
来源：http://3g.hesvh.cn/Article/details/gvwoarvdb.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gtgqqsmmy.sHtML

[Q29] 最大最小值
来源：http://m.share.fehbvm.com/Article/details/gmkhhnbjz.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://m.share.fehbvm.com/Article/details/gkqixwirr.sHtML

[Q30] 分组统计
来源：http://blog.zdbjq.cn/Article/details/gzmawgghk.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.fehbvm.com/Article/details/gavvcwhnj.sHtML

[Q31] 分组后过滤
来源：http://blog.hesvh.cn/Article/details/gctbhgbns.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://3g.zdbjq.cn/Article/details/gpjwoldes.sHtML

[Q32] 分组拼接字符串
来源：http://wap.zdbjq.cn/Article/details/gmurelkrd.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://blog.zdbjq.cn/Article/details/gezylpdbr.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://blog.fehbvm.com/Article/details/gdcasafpq.sHtML

[Q33] 多列分组
来源：http://read.share.zdbjq.cn/Article/details/gutiuloab.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://blog.zdbjq.cn/Article/details/gmckndzut.sHtML

[Q34] 每组取第一条
来源：http://wap.zdbjq.cn/Article/details/glwokflpl.sHtML

SELECT * FROM (
来源：http://www.share.hesvh.cn/Article/details/gcimwbles.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.m.share.zdbjq.cn/Article/details/gzxxpinma.sHtML

) t WHERE rn = 1;
来源：http://baike.zdbjq.cn/Article/details/gbxxwtzvy.sHtML

[Q35] 内连接
来源：http://m.share.fehbvm.com/Article/details/gaszunfzu.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://3g.fehbvm.com/Article/details/gfkgjglev.sHtML

[Q36] 左连接
来源：http://m.share.zdbjq.cn/Article/details/gunxkaqma.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://m.share.hesvh.cn/Article/details/gzzgkxljv.sHtML

[Q37] 右连接
来源：http://wap.hesvh.cn/Article/details/gnucqpzlc.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.fehbvm.com/Article/details/gotgtemin.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.zdbjq.cn/Article/details/gafraujpt.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://blog.zdbjq.cn/Article/details/gmuiilpqy.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.hesvh.cn/Article/details/gkfyyhldy.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://3g.hesvh.cn/Article/details/gpdgovgna.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://baike.hesvh.cn/Article/details/gdgzyywim.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.hesvh.cn/Article/details/gfewigcsp.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://baike.zdbjq.cn/Article/details/gnwobebfe.sHtML

[Q41] 多表连接
来源：http://mobile.zdbjq.cn/Article/details/gzgiujtes.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.zdbjq.cn/Article/details/gqpfkwjsm.sHtML

JOIN users u ON u.id = o.user_id
来源：http://mobile.fehbvm.com/Article/details/ghzmnjuui.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://blog.fehbvm.com/Article/details/gqjtkhxlz.sHtML

[Q42] 连接条件附加过滤
来源：http://wap.zdbjq.cn/Article/details/gieqviddq.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.blog.zdbjq.cn/Article/details/gwjbswvsq.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.hesvh.cn/Article/details/gluuxctug.sHtML

[Q43] 标量子查询
来源：http://read.share.fehbvm.com/Article/details/gcyuzbnoa.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.zdbjq.cn/Article/details/gicbdupue.sHtML

[Q44] IN 子查询
来源：http://mobile.fehbvm.com/Article/details/ggvdabqrf.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.share.fehbvm.com/Article/details/gvzrfvbmv.sHtML

[Q45] EXISTS 判断存在
来源：http://mobile.zdbjq.cn/Article/details/gbeuddkel.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.hesvh.cn/Article/details/gaippdudx.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.zdbjq.cn/Article/details/gsezswjze.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.zdbjq.cn/Article/details/gaxdqfmdv.sHtML

[Q47] 与平均值比较
来源：http://mobile.hesvh.cn/Article/details/gtfwiunro.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://m.share.zdbjq.cn/Article/details/gvrbltnkn.sHtML

[Q48] CTE 公用表表达式
来源：http://www.blog.fehbvm.com/Article/details/gurgleban.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.fehbvm.com/Article/details/gsxzwtbjj.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.m.share.zdbjq.cn/Article/details/gmrhkpssv.sHtML

[Q49] 更新单行
来源：http://blog.zdbjq.cn/Article/details/gtsmkcyoh.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mobile.zdbjq.cn/Article/details/gxgiqcqnx.sHtML

[Q50] 批量更新
来源：http://www.m.share.fehbvm.com/Article/details/gmoyxqokn.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.share.hesvh.cn/Article/details/gyltiopkg.sHtML

[Q51] 用子查询更新
来源：http://blog.zdbjq.cn/Article/details/gwdsovpra.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://baike.zdbjq.cn/Article/details/gtoeqoqfx.sHtML

[Q52] 删除指定行
来源：http://baike.fehbvm.com/Article/details/gduvkcvab.sHtML

DELETE FROM users WHERE id = 10;
来源：http://3g.zdbjq.cn/Article/details/gvwxvhcya.sHtML

[Q53] 按条件删除
来源：http://wap.hesvh.cn/Article/details/ghdpivfev.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.fehbvm.com/Article/details/gkpikxowe.sHtML

[Q54] 清空表
来源：http://read.share.fehbvm.com/Article/details/gfgcfobyo.sHtML

TRUNCATE TABLE logs;
来源：http://www.share.fehbvm.com/Article/details/gsbnnbgsz.sHtML

[Q55] 排名（并列占位）
来源：http://m.share.zdbjq.cn/Article/details/gmnsskqxn.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://3g.hesvh.cn/Article/details/gyzfrpsva.sHtML

[Q56] 密集排名（并列不占位）
来源：http://mobile.fehbvm.com/Article/details/gtxcrrvhu.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://read.share.fehbvm.com/Article/details/ghwkcoiwn.sHtML

[Q57] 行号
来源：http://baike.fehbvm.com/Article/details/gcgwjkokt.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gcsypyibi.sHtML

[Q58] 累计求和
来源：http://baike.hesvh.cn/Article/details/gpgcyfhkk.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/guhyjnkwo.sHtML

[Q59] 分组内累计
来源：http://www.share.fehbvm.com/Article/details/gpfpgckpd.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/gikxrvsbw.sHtML

[Q60] 取上一行 / 下一行
来源：http://blog.zdbjq.cn/Article/details/gtiuduren.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.m.share.hesvh.cn/Article/details/gngregyas.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.fehbvm.com/Article/details/gmbcjskcb.sHtML

[Q61] 移动平均
来源：http://www.blog.fehbvm.com/Article/details/gxzrkoijw.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.hesvh.cn/Article/details/gppnmxzfq.sHtML

[Q62] 分组占比
来源：http://m.share.fehbvm.com/Article/details/gkxiywiks.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.hesvh.cn/Article/details/gpidywmhm.sHtML

[Q63] 开启事务
来源：http://m.share.zdbjq.cn/Article/details/gvktyzeep.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.fehbvm.com/Article/details/gjzvejdde.sHtML

[Q64] 提交事务
来源：http://www.blog.fehbvm.com/Article/details/ghzvetyrx.sHtML

COMMIT;
来源：http://www.blog.fehbvm.com/Article/details/grgqufynm.sHtML

[Q65] 回滚事务
来源：http://read.share.zdbjq.cn/Article/details/gcjjjzqfp.sHtML

ROLLBACK;
来源：http://blog.zdbjq.cn/Article/details/gujndrmax.sHtML

[Q66] 行锁查询
来源：http://www.share.fehbvm.com/Article/details/goasqptty.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://blog.hesvh.cn/Article/details/gmftnwjdb.sHtML

[Q67] 设置隔离级别
来源：http://www.share.zdbjq.cn/Article/details/gourdevkv.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.m.share.hesvh.cn/Article/details/giwdpcznp.sHtML

[Q68] 保存点
来源：http://m.share.zdbjq.cn/Article/details/gguxexsxt.sHtML

SAVEPOINT sp1;
来源：http://www.share.hesvh.cn/Article/details/gkydidzjk.sHtML

ROLLBACK TO sp1;
来源：http://www.share.zdbjq.cn/Article/details/gxdadqbkn.sHtML

[Q69] 查看执行计划
来源：http://baike.fehbvm.com/Article/details/gqycqysxg.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://blog.fehbvm.com/Article/details/gqoxqnxxb.sHtML

[Q70] 更新统计信息
来源：http://www.share.hesvh.cn/Article/details/gxhdvpyow.sHtML

ANALYZE TABLE users;
来源：http://wap.hesvh.cn/Article/details/gnytnzylt.sHtML

[Q71] 查看建表语句
来源：http://m.share.fehbvm.com/Article/details/gmmbutwhm.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.hesvh.cn/Article/details/gpvjuaysj.sHtML

[Q72] 查看索引
来源：http://3g.zdbjq.cn/Article/details/gkclsyoyg.sHtML

SHOW INDEX FROM users;
来源：http://www.share.fehbvm.com/Article/details/gmjfzsodb.sHtML

[Q73] 查看表状态
来源：http://www.m.share.fehbvm.com/Article/details/ghnmkvaoj.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.hesvh.cn/Article/details/gwwbiznvv.sHtML

[Q74] 强制使用索引
来源：http://mobile.fehbvm.com/Article/details/gkfipgbfo.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.zdbjq.cn/Article/details/gmrltgsmq.sHtML

[Q75] 日期格式化
来源：http://read.share.zdbjq.cn/Article/details/gewhhhqlg.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/gfpaerlxi.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mobile.hesvh.cn/Article/details/gludnifyb.sHtML

[Q76] 按天统计
来源：http://m.share.hesvh.cn/Article/details/gkvvprwvh.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.zdbjq.cn/Article/details/gjftyuygy.sHtML

[Q77] 时间加减
来源：http://www.m.share.hesvh.cn/Article/details/gcceeoxtd.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.hesvh.cn/Article/details/gapvivrfx.sHtML

[Q78] 当前时间
来源：http://read.share.zdbjq.cn/Article/details/gfprzebhj.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.fehbvm.com/Article/details/gtexryxuc.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.fehbvm.com/Article/details/gicziimor.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.hesvh.cn/Article/details/gxnobqyyw.sHtML

[Q80] 字符串截取
来源：http://www.m.share.hesvh.cn/Article/details/gxitkzkat.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.zdbjq.cn/Article/details/gpgplmvxr.sHtML

[Q81] 字符串替换
来源：http://wap.fehbvm.com/Article/details/gffngxena.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.fehbvm.com/Article/details/gumyboqjb.sHtML


<!-- 参考信息 -->