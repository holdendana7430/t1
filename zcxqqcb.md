代发 wailian999

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://blog.zdbjq.cn/Article/details/gftlheojx.sHtML

TS:   // 同 JS
来源：http://mobile.zdbjq.cn/Article/details/gefnbmnhb.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.m.share.fehbvm.com/Article/details/gcasxfiwo.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.fehbvm.com/Article/details/gpbzfelkt.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://wap.hesvh.cn/Article/details/gtfeqnomu.sHtML

C#:   lock (gate) { shared++; }
来源：http://read.share.fehbvm.com/Article/details/gkreoakih.sHtML

[O04] 定义异步函数并等待
来源：http://wap.hesvh.cn/Article/details/gszwkyauu.sHtML

Py:   async def f():⏎    await g()
来源：http://www.m.share.hesvh.cn/Article/details/ghaffxoph.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.fehbvm.com/Article/details/gjxcucuil.sHtML

JS:   async function f() { await g(); }
来源：http://baike.hesvh.cn/Article/details/gvdxrdplm.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.share.zdbjq.cn/Article/details/gvduxwclj.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.share.hesvh.cn/Article/details/gwaxtjoho.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wap.hesvh.cn/Article/details/gozrnihkm.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://baike.fehbvm.com/Article/details/gaihfzjfp.sHtML

C#:   async Task F() { await G(); }
来源：http://www.m.share.hesvh.cn/Article/details/gwyghqwat.sHtML

[O05] 并发执行并等待全部完成
来源：http://blog.fehbvm.com/Article/details/gifkzbghy.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.fehbvm.com/Article/details/gsdsojqkd.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://blog.zdbjq.cn/Article/details/gtlfqomrb.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.hesvh.cn/Article/details/gwmuxlccm.sHtML

TS:   await Promise.all(tasks)
来源：http://baike.zdbjq.cn/Article/details/gfoojenhy.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://blog.hesvh.cn/Article/details/ggkrytrwq.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mobile.zdbjq.cn/Article/details/gtdorgkji.sHtML

Ruby: threads.map(&:join)
来源：http://baike.fehbvm.com/Article/details/guomfdovg.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://m.share.fehbvm.com/Article/details/galeqfceg.sHtML

[O06] 使用进程池
来源：http://m.share.zdbjq.cn/Article/details/gaxtbfylh.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wap.hesvh.cn/Article/details/gbsdzxfll.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://read.share.fehbvm.com/Article/details/ghllhrlbb.sHtML

JS:   // child_process / cluster 模块
来源：http://3g.fehbvm.com/Article/details/gyduowsfm.sHtML

TS:   // child_process / cluster 模块
来源：http://www.m.share.zdbjq.cn/Article/details/graqdfyqo.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wap.fehbvm.com/Article/details/gjtmhaqrc.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.m.share.fehbvm.com/Article/details/gmlryscwr.sHtML

Ruby: // fork 块
来源：http://wap.fehbvm.com/Article/details/gxcfvfqem.sHtML

C#:   Parallel.For
来源：http://blog.hesvh.cn/Article/details/gpevdrtrn.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gclgexscw.sHtML

P. 常用工具函数
来源：http://www.m.share.zdbjq.cn/Article/details/gpmrzhzcj.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gqvsnjzuo.sHtML

[P01] 生成 UUID
来源：http://wap.fehbvm.com/Article/details/gywjftdbv.sHtML

Py:   str(uuid.uuid4())
来源：http://baike.hesvh.cn/Article/details/gohbepngc.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.blog.hesvh.cn/Article/details/gfgodjibp.sHtML

JS:   crypto.randomUUID()
来源：http://baike.zdbjq.cn/Article/details/gsobwvwmn.sHtML

TS:   crypto.randomUUID()
来源：http://www.m.share.hesvh.cn/Article/details/gdtglosft.sHtML

Java: UUID.randomUUID().toString()
来源：http://read.share.hesvh.cn/Article/details/geewkgxtb.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.m.share.zdbjq.cn/Article/details/gedcnwdao.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.fehbvm.com/Article/details/gofugvrki.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://mobile.fehbvm.com/Article/details/gfoymomyb.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.blog.zdbjq.cn/Article/details/gdvvsdtuy.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.m.share.fehbvm.com/Article/details/gyixhnkzv.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://read.share.hesvh.cn/Article/details/gpqykpfsj.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mobile.zdbjq.cn/Article/details/glnlbydsb.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.blog.zdbjq.cn/Article/details/gjkvwnmmk.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://blog.zdbjq.cn/Article/details/gckwpyufq.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://read.share.hesvh.cn/Article/details/gmtitobcn.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.share.hesvh.cn/Article/details/gucuvrtrk.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://read.share.fehbvm.com/Article/details/gkixfwsnh.sHtML

[P03] 生成短随机字符串
来源：http://blog.zdbjq.cn/Article/details/gvzcgzpqy.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://read.share.hesvh.cn/Article/details/gboaexocw.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://read.share.hesvh.cn/Article/details/gaiegkcln.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.hesvh.cn/Article/details/gzpjcbkhb.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.zdbjq.cn/Article/details/gcxelsbsu.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://blog.zdbjq.cn/Article/details/gvmkgzdgn.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.m.share.hesvh.cn/Article/details/gldtkjqaq.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://baike.fehbvm.com/Article/details/ghjtdlwku.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://3g.fehbvm.com/Article/details/gbycbghnf.sHtML

[P04] 求长度
来源：http://read.share.zdbjq.cn/Article/details/gmyyruvpr.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://blog.hesvh.cn/Article/details/gssmljmbx.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.fehbvm.com/Article/details/gvddkxrbe.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.zdbjq.cn/Article/details/gxfuvathf.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.zdbjq.cn/Article/details/gzuyiblbk.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.m.share.hesvh.cn/Article/details/ghkezpauy.sHtML

Go:   len(arr);  len(m)
来源：http://m.share.hesvh.cn/Article/details/gnmskdttb.sHtML

Ruby: x.length;  x.size
来源：http://www.blog.fehbvm.com/Article/details/gqxeeycxl.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://wap.fehbvm.com/Article/details/gytzlowys.sHtML

[P05] 判断两个对象内容是否相等
来源：http://baike.zdbjq.cn/Article/details/gsmndxqtx.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://wap.hesvh.cn/Article/details/grsjnkufe.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://blog.fehbvm.com/Article/details/geumvboah.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://m.share.hesvh.cn/Article/details/giuadhycd.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.fehbvm.com/Article/details/gbfwqnnaa.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://baike.zdbjq.cn/Article/details/gzqyhmcnj.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://wap.zdbjq.cn/Article/details/gawbkzmkl.sHtML

Ruby: a == b
来源：http://baike.fehbvm.com/Article/details/gptvhhoyf.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://3g.fehbvm.com/Article/details/gbiummvxv.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mobile.fehbvm.com/Article/details/gvqxhelud.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://m.share.fehbvm.com/Article/details/gqtcszvpz.sHtML

PHP:  if (empty($x)) {}
来源：http://3g.zdbjq.cn/Article/details/gbsyvigjo.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://read.share.zdbjq.cn/Article/details/ghkedlrzq.sHtML

TS:   if (x == null) {}
来源：http://baike.hesvh.cn/Article/details/gpkejyoge.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://3g.fehbvm.com/Article/details/giidknoko.sHtML

Go:   if x == nil {}
来源：http://mobile.zdbjq.cn/Article/details/gyclxnnuy.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://m.share.hesvh.cn/Article/details/gjclhjudn.sHtML

C#:   if (x is null) {}
来源：http://3g.fehbvm.com/Article/details/gnakiqjkv.sHtML

[P07] 防抖与节流
来源：http://m.share.fehbvm.com/Article/details/gbrtvcmpu.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://baike.zdbjq.cn/Article/details/gqamtqqtl.sHtML

PHP:  // 手写时间戳比较
来源：http://www.share.fehbvm.com/Article/details/gtyighzfo.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.hesvh.cn/Article/details/gxuqenlwz.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.fehbvm.com/Article/details/glpfltroh.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.share.hesvh.cn/Article/details/gyxjmnzsz.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://baike.zdbjq.cn/Article/details/gyooqnnqe.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://wap.fehbvm.com/Article/details/gvqdpgeoq.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.m.share.hesvh.cn/Article/details/gtmrjmbvj.sHtML

[P08] 处理浮点精度问题
来源：http://read.share.hesvh.cn/Article/details/gjlayqsel.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://m.share.hesvh.cn/Article/details/ggljuvkdp.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.fehbvm.com/Article/details/gktpnhryl.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.m.share.hesvh.cn/Article/details/gattpxllj.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://baike.fehbvm.com/Article/details/gcwhgrvkd.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://read.share.hesvh.cn/Article/details/gqpyvyjhp.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wap.zdbjq.cn/Article/details/garvvuhkt.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://m.share.zdbjq.cn/Article/details/gybogjlzd.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wap.zdbjq.cn/Article/details/guvjnaauy.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gqszyalro.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://3g.fehbvm.com/Article/details/gyzganqjl.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gfmslbnex.sHtML

[Q01] 创建表
来源：http://www.share.zdbjq.cn/Article/details/gzeaumikm.sHtML

CREATE TABLE users (
来源：http://wap.hesvh.cn/Article/details/gpsucywpi.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.fehbvm.com/Article/details/gyzcnhjil.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.m.share.fehbvm.com/Article/details/gwzvnrhhr.sHtML

email VARCHAR(100) UNIQUE,
来源：http://3g.hesvh.cn/Article/details/gtdjppksw.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mobile.zdbjq.cn/Article/details/gvfbyxyis.sHtML

);
来源：http://read.share.hesvh.cn/Article/details/gfduksxdk.sHtML

[Q02] 创建带外键的表
来源：http://read.share.zdbjq.cn/Article/details/gohoawhmy.sHtML

CREATE TABLE orders (
来源：http://baike.hesvh.cn/Article/details/gupbbedph.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.fehbvm.com/Article/details/gytrinfna.sHtML

user_id INT NOT NULL,
来源：http://www.blog.fehbvm.com/Article/details/gcmuhntjj.sHtML

amount DECIMAL(10, 2),
来源：http://wap.hesvh.cn/Article/details/grgnzjbbs.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://baike.fehbvm.com/Article/details/gdabmuqbj.sHtML

);
来源：http://www.share.hesvh.cn/Article/details/gubxucsly.sHtML

[Q03] 增加列
来源：http://baike.zdbjq.cn/Article/details/ggrojwjyn.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.m.share.zdbjq.cn/Article/details/gzgaavrar.sHtML

[Q04] 修改列类型
来源：http://m.share.fehbvm.com/Article/details/gihinynna.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://m.share.fehbvm.com/Article/details/gyytbfwuz.sHtML

[Q05] 重命名列
来源：http://www.blog.hesvh.cn/Article/details/gbfquyxcn.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mobile.hesvh.cn/Article/details/gdqxxijgh.sHtML

[Q06] 删除列
来源：http://wap.fehbvm.com/Article/details/glbtwoufl.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.blog.zdbjq.cn/Article/details/gawtzhred.sHtML

[Q07] 删除表
来源：http://www.blog.hesvh.cn/Article/details/gvqnrwwkf.sHtML

DROP TABLE IF EXISTS orders;
来源：http://3g.hesvh.cn/Article/details/geawuymbg.sHtML

[Q08] 创建普通索引
来源：http://m.share.zdbjq.cn/Article/details/gkowgsaip.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://m.share.fehbvm.com/Article/details/gwykceeqh.sHtML

[Q09] 创建唯一索引
来源：http://baike.zdbjq.cn/Article/details/gjxpxadnd.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wap.fehbvm.com/Article/details/gzkvzgfoc.sHtML

[Q10] 插入单行
来源：http://www.blog.hesvh.cn/Article/details/gvdttozyd.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.m.share.fehbvm.com/Article/details/gctnmlryt.sHtML

[Q11] 一次插入多行
来源：http://3g.zdbjq.cn/Article/details/geagodawr.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.hesvh.cn/Article/details/gwopvruac.sHtML

[Q12] 插入后取自增 ID
来源：http://wap.hesvh.cn/Article/details/gstuqlvlm.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://wap.fehbvm.com/Article/details/gekdvqhcc.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wap.zdbjq.cn/Article/details/gqvwcaqel.sHtML

[Q13] 忽略重复插入
来源：http://m.share.zdbjq.cn/Article/details/gimpeamwg.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.share.zdbjq.cn/Article/details/grldmchuw.sHtML

[Q14] 存在则更新（upsert）
来源：http://wap.zdbjq.cn/Article/details/gmqpsmien.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://blog.zdbjq.cn/Article/details/gektqxvjy.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mobile.zdbjq.cn/Article/details/gxzksfdjd.sHtML

[Q15] 查询全部
来源：http://mobile.hesvh.cn/Article/details/gylpqlbsb.sHtML

SELECT * FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gevcuuxkz.sHtML

[Q16] 查询指定列
来源：http://3g.fehbvm.com/Article/details/gnnwqptiq.sHtML

SELECT id, name FROM users;
来源：http://wap.hesvh.cn/Article/details/gfdtcbexh.sHtML

[Q17] 条件查询
来源：http://baike.zdbjq.cn/Article/details/gmkitsvdl.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.share.zdbjq.cn/Article/details/gkelwzmdo.sHtML

[Q18] 模糊匹配
来源：http://baike.zdbjq.cn/Article/details/ghtybnujm.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mobile.fehbvm.com/Article/details/gvxmkmehi.sHtML

[Q19] 范围查询
来源：http://mobile.zdbjq.cn/Article/details/grnkfkgnu.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wap.fehbvm.com/Article/details/giueovwan.sHtML

[Q20] IN 列表
来源：http://baike.zdbjq.cn/Article/details/gmjxcokcf.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.share.zdbjq.cn/Article/details/gwxprzsgz.sHtML

[Q21] 空值判断
来源：http://3g.zdbjq.cn/Article/details/gscftgrsu.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://m.share.zdbjq.cn/Article/details/gzfgdohry.sHtML

[Q22] 排序
来源：http://www.m.share.hesvh.cn/Article/details/gqiqfvynm.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://baike.zdbjq.cn/Article/details/gfxvtlexp.sHtML

[Q23] 分页
来源：http://3g.zdbjq.cn/Article/details/gtzqmrdmu.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mobile.fehbvm.com/Article/details/gprzbtesg.sHtML

[Q24] 去重
来源：http://blog.zdbjq.cn/Article/details/grjvcvskz.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.share.hesvh.cn/Article/details/ghmjolzos.sHtML

[Q25] 只取前 N 条
来源：http://mobile.fehbvm.com/Article/details/gbcnrybzd.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://baike.fehbvm.com/Article/details/gtfblkagk.sHtML

[Q26] 计数
来源：http://wap.fehbvm.com/Article/details/giuknywmy.sHtML

SELECT COUNT(*) FROM users;
来源：http://wap.fehbvm.com/Article/details/giqaplres.sHtML

[Q27] 条件计数
来源：http://www.m.share.fehbvm.com/Article/details/gtffsgwez.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://baike.fehbvm.com/Article/details/goqtdwule.sHtML

[Q28] 求和与平均
来源：http://blog.hesvh.cn/Article/details/gzfznwhid.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/gqiiidxxx.sHtML

[Q29] 最大最小值
来源：http://read.share.hesvh.cn/Article/details/gnlbvhbnd.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.hesvh.cn/Article/details/gvbxekvyb.sHtML

[Q30] 分组统计
来源：http://read.share.fehbvm.com/Article/details/gickacqch.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://read.share.zdbjq.cn/Article/details/gkmxqwrfa.sHtML

[Q31] 分组后过滤
来源：http://www.m.share.hesvh.cn/Article/details/gzxwnxvkh.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://read.share.zdbjq.cn/Article/details/gkpajuxrs.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.fehbvm.com/Article/details/gcyosemtj.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.share.zdbjq.cn/Article/details/gcnhizesf.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://blog.zdbjq.cn/Article/details/gfjuyeyik.sHtML

[Q33] 多列分组
来源：http://wap.zdbjq.cn/Article/details/gumredjmo.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wap.zdbjq.cn/Article/details/gywipzynu.sHtML

[Q34] 每组取第一条
来源：http://read.share.zdbjq.cn/Article/details/gbalzyuzg.sHtML

SELECT * FROM (
来源：http://www.m.share.hesvh.cn/Article/details/gsgxpgich.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://m.share.zdbjq.cn/Article/details/ghsukvxrh.sHtML

) t WHERE rn = 1;
来源：http://wap.fehbvm.com/Article/details/gllnhsujt.sHtML

[Q35] 内连接
来源：http://wap.fehbvm.com/Article/details/glnexqvjf.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.hesvh.cn/Article/details/gckjeugsy.sHtML

[Q36] 左连接
来源：http://blog.fehbvm.com/Article/details/gpsqovrqp.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://read.share.fehbvm.com/Article/details/gdsazcsxr.sHtML

[Q37] 右连接
来源：http://m.share.zdbjq.cn/Article/details/gupilrcgw.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wap.fehbvm.com/Article/details/gsvogkugh.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://3g.zdbjq.cn/Article/details/glvvlizwf.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://3g.hesvh.cn/Article/details/gqfowcqbm.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.fehbvm.com/Article/details/gyapdocld.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://read.share.fehbvm.com/Article/details/gubhizwgj.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.zdbjq.cn/Article/details/gtstikrar.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://3g.zdbjq.cn/Article/details/glhnnwebf.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.blog.zdbjq.cn/Article/details/gleobnbaf.sHtML

[Q41] 多表连接
来源：http://wap.zdbjq.cn/Article/details/godbbzgnp.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.blog.zdbjq.cn/Article/details/gazkuahru.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.zdbjq.cn/Article/details/gddlnqeqt.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.fehbvm.com/Article/details/grvskkcce.sHtML

[Q42] 连接条件附加过滤
来源：http://read.share.zdbjq.cn/Article/details/goeqlpbjh.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.m.share.hesvh.cn/Article/details/gxtwlfrqk.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.zdbjq.cn/Article/details/gdbmwubtb.sHtML

[Q43] 标量子查询
来源：http://www.blog.zdbjq.cn/Article/details/gslhygyhe.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.fehbvm.com/Article/details/gqubokdig.sHtML

[Q44] IN 子查询
来源：http://www.share.zdbjq.cn/Article/details/gizmoexvy.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.blog.hesvh.cn/Article/details/gskhdqmfe.sHtML

[Q45] EXISTS 判断存在
来源：http://www.share.hesvh.cn/Article/details/gvdjkpzct.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.hesvh.cn/Article/details/gnvogftdf.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.zdbjq.cn/Article/details/glgvgipag.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.zdbjq.cn/Article/details/geiarxtdy.sHtML

[Q47] 与平均值比较
来源：http://blog.fehbvm.com/Article/details/gowdativd.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://baike.hesvh.cn/Article/details/ggljxwfnb.sHtML

[Q48] CTE 公用表表达式
来源：http://read.share.zdbjq.cn/Article/details/ggerrgyto.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.m.share.fehbvm.com/Article/details/gsvzdmzco.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://mobile.zdbjq.cn/Article/details/gcfzhehio.sHtML

[Q49] 更新单行
来源：http://3g.fehbvm.com/Article/details/gpsibrzny.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.zdbjq.cn/Article/details/gbivyisoy.sHtML

[Q50] 批量更新
来源：http://www.m.share.zdbjq.cn/Article/details/ghcoazyqe.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.share.fehbvm.com/Article/details/grzsxrfmm.sHtML

[Q51] 用子查询更新
来源：http://mobile.fehbvm.com/Article/details/gxnzypmtg.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.fehbvm.com/Article/details/gewumjlti.sHtML

[Q52] 删除指定行
来源：http://read.share.hesvh.cn/Article/details/gzqwvxgsm.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.zdbjq.cn/Article/details/gmmzezuev.sHtML

[Q53] 按条件删除
来源：http://read.share.fehbvm.com/Article/details/ggetoxvko.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.hesvh.cn/Article/details/gqtoxlwnh.sHtML

[Q54] 清空表
来源：http://blog.hesvh.cn/Article/details/gctezsvxm.sHtML

TRUNCATE TABLE logs;
来源：http://www.share.fehbvm.com/Article/details/gnvopcszr.sHtML

[Q55] 排名（并列占位）
来源：http://3g.fehbvm.com/Article/details/glasjtpbf.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.zdbjq.cn/Article/details/gidhrhpef.sHtML

[Q56] 密集排名（并列不占位）
来源：http://wap.fehbvm.com/Article/details/guvvydynx.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.hesvh.cn/Article/details/gtstfselr.sHtML

[Q57] 行号
来源：http://wap.fehbvm.com/Article/details/ggyxujwpn.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.hesvh.cn/Article/details/gefvsrlnj.sHtML

[Q58] 累计求和
来源：http://read.share.hesvh.cn/Article/details/gpaypkjus.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mobile.fehbvm.com/Article/details/grvqxxuse.sHtML

[Q59] 分组内累计
来源：http://m.share.fehbvm.com/Article/details/gyfxzobim.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/gvuciywzr.sHtML

[Q60] 取上一行 / 下一行
来源：http://wap.zdbjq.cn/Article/details/geadmbjmf.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.fehbvm.com/Article/details/gwbsjlafa.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.hesvh.cn/Article/details/ggnpfrkqq.sHtML

[Q61] 移动平均
来源：http://mobile.zdbjq.cn/Article/details/gpyptmxaz.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.hesvh.cn/Article/details/gsleoagwl.sHtML

[Q62] 分组占比
来源：http://3g.hesvh.cn/Article/details/gdzpvyhcl.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.zdbjq.cn/Article/details/gusfoxfil.sHtML

[Q63] 开启事务
来源：http://wap.hesvh.cn/Article/details/gwggcvqpq.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://mobile.hesvh.cn/Article/details/gdoslbtta.sHtML

[Q64] 提交事务
来源：http://blog.hesvh.cn/Article/details/gtbthhrxv.sHtML

COMMIT;
来源：http://www.m.share.hesvh.cn/Article/details/gbfyyagpy.sHtML

[Q65] 回滚事务
来源：http://www.share.zdbjq.cn/Article/details/gfejqwnwc.sHtML

ROLLBACK;
来源：http://www.blog.zdbjq.cn/Article/details/gvoamegxx.sHtML

[Q66] 行锁查询
来源：http://www.share.hesvh.cn/Article/details/gctxdyyxh.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.hesvh.cn/Article/details/grheeormm.sHtML

[Q67] 设置隔离级别
来源：http://www.share.hesvh.cn/Article/details/gxzwctpat.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.fehbvm.com/Article/details/gvidwqcfh.sHtML

[Q68] 保存点
来源：http://3g.hesvh.cn/Article/details/gvrhabxph.sHtML

SAVEPOINT sp1;
来源：http://www.blog.hesvh.cn/Article/details/gvktqsjxo.sHtML

ROLLBACK TO sp1;
来源：http://baike.zdbjq.cn/Article/details/gfsslqibz.sHtML

[Q69] 查看执行计划
来源：http://blog.zdbjq.cn/Article/details/gpidexain.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.zdbjq.cn/Article/details/gheulefxi.sHtML

[Q70] 更新统计信息
来源：http://m.share.fehbvm.com/Article/details/gaybzmumx.sHtML

ANALYZE TABLE users;
来源：http://blog.zdbjq.cn/Article/details/gxyaerxdm.sHtML

[Q71] 查看建表语句
来源：http://www.share.hesvh.cn/Article/details/gtqwmsajm.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.fehbvm.com/Article/details/gwapbeqly.sHtML

[Q72] 查看索引
来源：http://m.share.hesvh.cn/Article/details/gnityhdcy.sHtML

SHOW INDEX FROM users;
来源：http://read.share.fehbvm.com/Article/details/gxztadzhm.sHtML

[Q73] 查看表状态
来源：http://mobile.zdbjq.cn/Article/details/gtbsqzppv.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.hesvh.cn/Article/details/ghhojplcg.sHtML

[Q74] 强制使用索引
来源：http://blog.zdbjq.cn/Article/details/gnawouote.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.hesvh.cn/Article/details/gctbvqfsn.sHtML

[Q75] 日期格式化
来源：http://3g.hesvh.cn/Article/details/gusprsxsh.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gshizypdi.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://baike.fehbvm.com/Article/details/gsczjahnp.sHtML

[Q76] 按天统计
来源：http://read.share.hesvh.cn/Article/details/gvminsqms.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.hesvh.cn/Article/details/gqrswowhj.sHtML

[Q77] 时间加减
来源：http://3g.hesvh.cn/Article/details/gemvettpz.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.hesvh.cn/Article/details/grcgkjzzr.sHtML

[Q78] 当前时间
来源：http://www.m.share.fehbvm.com/Article/details/gczmshjuu.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.fehbvm.com/Article/details/gjlllfmco.sHtML

[Q79] 字符串拼接
来源：http://www.blog.fehbvm.com/Article/details/gapfnelza.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.hesvh.cn/Article/details/ggveqquzz.sHtML

[Q80] 字符串截取
来源：http://m.share.fehbvm.com/Article/details/gwfgjsrqh.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.hesvh.cn/Article/details/ggsewmwvl.sHtML

[Q81] 字符串替换
来源：http://3g.hesvh.cn/Article/details/gbtxfvqus.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.hesvh.cn/Article/details/gqnolancb.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.zdbjq.cn/Article/details/ggflhbdlr.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gnygyvwdv.sHtML

[Q83] 大小写转换
来源：http://wap.zdbjq.cn/Article/details/gmgtuhbsp.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.hesvh.cn/Article/details/ghqztbhzl.sHtML


<!-- 参考信息 -->