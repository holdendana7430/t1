代发 wailian999

TS:   // worker_threads 线程池
来源：http://mobile.zdbjq.cn/Article/details/gwkktlzrc.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://blog.fehbvm.com/Article/details/gxmkglzru.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://3g.fehbvm.com/Article/details/gcivukcfa.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mobile.zdbjq.cn/Article/details/gducrbpfl.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://m.share.hesvh.cn/Article/details/galvktfji.sHtML

[O03] 加锁保护共享数据
来源：http://www.share.hesvh.cn/Article/details/gltwoahes.sHtML

Py:   with lock: shared += 1
来源：http://read.share.hesvh.cn/Article/details/guidojodb.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://read.share.zdbjq.cn/Article/details/gylbacjlb.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.m.share.zdbjq.cn/Article/details/gozonwehl.sHtML

TS:   // 同 JS
来源：http://www.m.share.hesvh.cn/Article/details/geoqvhrdh.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.hesvh.cn/Article/details/gfofwlczm.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.fehbvm.com/Article/details/gdzcdqrvr.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://3g.hesvh.cn/Article/details/guyvpqtae.sHtML

C#:   lock (gate) { shared++; }
来源：http://3g.zdbjq.cn/Article/details/gcuvffpci.sHtML

[O04] 定义异步函数并等待
来源：http://blog.fehbvm.com/Article/details/geryfqmpm.sHtML

Py:   async def f():⏎    await g()
来源：http://wap.hesvh.cn/Article/details/gvupisugs.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.fehbvm.com/Article/details/gkucxjcns.sHtML

JS:   async function f() { await g(); }
来源：http://blog.fehbvm.com/Article/details/ghhtncdbr.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://baike.hesvh.cn/Article/details/gmkekpezs.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.hesvh.cn/Article/details/gfhfqmxhk.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://3g.fehbvm.com/Article/details/guzyrzmvc.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.fehbvm.com/Article/details/grfugpkiw.sHtML

C#:   async Task F() { await G(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gdsknorzh.sHtML

[O05] 并发执行并等待全部完成
来源：http://wap.hesvh.cn/Article/details/gfnhchgcu.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.share.zdbjq.cn/Article/details/gzjugrrti.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wap.fehbvm.com/Article/details/gxxwqsfcy.sHtML

JS:   await Promise.all(tasks)
来源：http://mobile.fehbvm.com/Article/details/gaflvacag.sHtML

TS:   await Promise.all(tasks)
来源：http://mobile.hesvh.cn/Article/details/gurzctgsl.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.m.share.hesvh.cn/Article/details/gcxifidxz.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mobile.fehbvm.com/Article/details/grnwxwdcf.sHtML

Ruby: threads.map(&:join)
来源：http://www.share.fehbvm.com/Article/details/gujungbya.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://baike.fehbvm.com/Article/details/gzeibxzbu.sHtML

[O06] 使用进程池
来源：http://wap.fehbvm.com/Article/details/gqinkyqat.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.share.fehbvm.com/Article/details/gggfhevvs.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://m.share.fehbvm.com/Article/details/guilkqyca.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.hesvh.cn/Article/details/gyixhsbyy.sHtML

TS:   // child_process / cluster 模块
来源：http://www.m.share.zdbjq.cn/Article/details/gecdgvkau.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.share.zdbjq.cn/Article/details/gxfzbwdlm.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://m.share.hesvh.cn/Article/details/gogyomndz.sHtML

Ruby: // fork 块
来源：http://wap.hesvh.cn/Article/details/gomchyuut.sHtML

C#:   Parallel.For
来源：http://www.blog.hesvh.cn/Article/details/gbffiznmi.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gcaicmgwh.sHtML

P. 常用工具函数
来源：http://baike.zdbjq.cn/Article/details/gcnjokdol.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/givurwhfn.sHtML

[P01] 生成 UUID
来源：http://baike.fehbvm.com/Article/details/gkzvrqyej.sHtML

Py:   str(uuid.uuid4())
来源：http://baike.zdbjq.cn/Article/details/gyvncryqd.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.m.share.fehbvm.com/Article/details/gaipazqvw.sHtML

JS:   crypto.randomUUID()
来源：http://read.share.zdbjq.cn/Article/details/gxyxonndx.sHtML

TS:   crypto.randomUUID()
来源：http://blog.fehbvm.com/Article/details/gnfzocovr.sHtML

Java: UUID.randomUUID().toString()
来源：http://3g.zdbjq.cn/Article/details/gjevuxxzm.sHtML

Go:   // 用 github.com/google/uuid
来源：http://baike.hesvh.cn/Article/details/gowcarhrg.sHtML

Ruby: SecureRandom.uuid
来源：http://wap.hesvh.cn/Article/details/gitglsipv.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.share.zdbjq.cn/Article/details/grtxxxqvu.sHtML

[P02] MD5 / SHA256 摘要
来源：http://mobile.fehbvm.com/Article/details/gffjmyipk.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mobile.fehbvm.com/Article/details/ggzdcpkrq.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://3g.zdbjq.cn/Article/details/guprjegwi.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wap.zdbjq.cn/Article/details/gfndsqnvz.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.fehbvm.com/Article/details/gtuaxtqmf.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://baike.hesvh.cn/Article/details/gbvwmkjnx.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://3g.zdbjq.cn/Article/details/ghsdjadeo.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.share.zdbjq.cn/Article/details/gxalfelmn.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.blog.fehbvm.com/Article/details/gzkgicgrr.sHtML

[P03] 生成短随机字符串
来源：http://3g.zdbjq.cn/Article/details/ghfacpbjr.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.share.fehbvm.com/Article/details/gawfnzybd.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://3g.fehbvm.com/Article/details/gokcckxiz.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.fehbvm.com/Article/details/grfpejtqc.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.fehbvm.com/Article/details/gwnsuzjdv.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wap.zdbjq.cn/Article/details/gmrthgjzv.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.blog.zdbjq.cn/Article/details/gxzpuxpll.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://wap.fehbvm.com/Article/details/gjyvdnzhk.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.blog.hesvh.cn/Article/details/ghggjigay.sHtML

[P04] 求长度
来源：http://read.share.hesvh.cn/Article/details/gebtydtuj.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wap.fehbvm.com/Article/details/ggjdtcxlz.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.zdbjq.cn/Article/details/gedbstkid.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.fehbvm.com/Article/details/gajljxgfa.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.zdbjq.cn/Article/details/gwfelfaff.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.share.zdbjq.cn/Article/details/gcnpuqryi.sHtML

Go:   len(arr);  len(m)
来源：http://www.blog.zdbjq.cn/Article/details/gocuvzwkh.sHtML

Ruby: x.length;  x.size
来源：http://m.share.hesvh.cn/Article/details/gaqiljvtx.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://baike.hesvh.cn/Article/details/gkdozmnlu.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.blog.fehbvm.com/Article/details/gvcuucmmf.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://m.share.fehbvm.com/Article/details/gmblwkink.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.blog.fehbvm.com/Article/details/gdaztidzh.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://m.share.zdbjq.cn/Article/details/gxmamwodr.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.zdbjq.cn/Article/details/ghlembrhh.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wap.hesvh.cn/Article/details/gwrzgqotn.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://read.share.hesvh.cn/Article/details/gnuiobixa.sHtML

Ruby: a == b
来源：http://m.share.zdbjq.cn/Article/details/gjczfktzj.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mobile.hesvh.cn/Article/details/gffprxvnq.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.m.share.fehbvm.com/Article/details/gsmlbyspe.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://m.share.hesvh.cn/Article/details/gvbjrgruo.sHtML

PHP:  if (empty($x)) {}
来源：http://mobile.hesvh.cn/Article/details/gomrrszqy.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://baike.hesvh.cn/Article/details/gtsdyqnwi.sHtML

TS:   if (x == null) {}
来源：http://3g.hesvh.cn/Article/details/ggwengxot.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://baike.fehbvm.com/Article/details/gkfpozimi.sHtML

Go:   if x == nil {}
来源：http://www.m.share.zdbjq.cn/Article/details/gjabnmpyw.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://baike.fehbvm.com/Article/details/gjixjdgnj.sHtML

C#:   if (x is null) {}
来源：http://baike.zdbjq.cn/Article/details/gtmurxrft.sHtML

[P07] 防抖与节流
来源：http://m.share.fehbvm.com/Article/details/gohmuveft.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wap.fehbvm.com/Article/details/glgauooew.sHtML

PHP:  // 手写时间戳比较
来源：http://www.blog.hesvh.cn/Article/details/gdilqvgtz.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.hesvh.cn/Article/details/glpjxdene.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.fehbvm.com/Article/details/gqsnhchsp.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://3g.hesvh.cn/Article/details/gxxemrltu.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.share.hesvh.cn/Article/details/gssvgnocj.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.fehbvm.com/Article/details/gfupnrsks.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://read.share.fehbvm.com/Article/details/gzllkjaxz.sHtML

[P08] 处理浮点精度问题
来源：http://baike.fehbvm.com/Article/details/gnmesfqif.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://baike.hesvh.cn/Article/details/gfilvamjk.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.share.hesvh.cn/Article/details/gdmanbsbn.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.blog.zdbjq.cn/Article/details/ggemtdivg.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wap.hesvh.cn/Article/details/giwgirufe.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://baike.zdbjq.cn/Article/details/gjvipiroe.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.blog.fehbvm.com/Article/details/glkmywxxk.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.m.share.fehbvm.com/Article/details/gdcuqavmz.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://blog.zdbjq.cn/Article/details/giyjrelid.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/goeajxfax.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wap.fehbvm.com/Article/details/gtsznaiao.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gdkkcziui.sHtML

[Q01] 创建表
来源：http://3g.hesvh.cn/Article/details/gqiiamwih.sHtML

CREATE TABLE users (
来源：http://blog.zdbjq.cn/Article/details/gjbcjhpup.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.zdbjq.cn/Article/details/gwwvtxfmb.sHtML

name VARCHAR(50) NOT NULL,
来源：http://3g.fehbvm.com/Article/details/gywhjkteg.sHtML

email VARCHAR(100) UNIQUE,
来源：http://m.share.fehbvm.com/Article/details/gkllamsto.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mobile.fehbvm.com/Article/details/gpcboobia.sHtML

);
来源：http://baike.zdbjq.cn/Article/details/gncthyoof.sHtML

[Q02] 创建带外键的表
来源：http://www.blog.zdbjq.cn/Article/details/geehzfvui.sHtML

CREATE TABLE orders (
来源：http://www.blog.hesvh.cn/Article/details/grydhuuwg.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.hesvh.cn/Article/details/gsskacdfx.sHtML

user_id INT NOT NULL,
来源：http://www.m.share.fehbvm.com/Article/details/gpfpabtix.sHtML

amount DECIMAL(10, 2),
来源：http://read.share.fehbvm.com/Article/details/grsvpunbw.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://blog.hesvh.cn/Article/details/gkgggpkti.sHtML

);
来源：http://3g.zdbjq.cn/Article/details/gsiyaqzsb.sHtML

[Q03] 增加列
来源：http://blog.zdbjq.cn/Article/details/gimzlureq.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://3g.hesvh.cn/Article/details/gyabvyxqs.sHtML

[Q04] 修改列类型
来源：http://wap.hesvh.cn/Article/details/gfraslcji.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.m.share.hesvh.cn/Article/details/gbqelsckr.sHtML

[Q05] 重命名列
来源：http://mobile.hesvh.cn/Article/details/geupsrzzf.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.blog.hesvh.cn/Article/details/gatwjiyer.sHtML

[Q06] 删除列
来源：http://www.share.fehbvm.com/Article/details/gjjihpoyo.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://baike.zdbjq.cn/Article/details/gleuzmxha.sHtML

[Q07] 删除表
来源：http://www.m.share.zdbjq.cn/Article/details/gbyviwctr.sHtML

DROP TABLE IF EXISTS orders;
来源：http://read.share.zdbjq.cn/Article/details/ggoxtjhne.sHtML

[Q08] 创建普通索引
来源：http://blog.zdbjq.cn/Article/details/ginwfqubx.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://wap.fehbvm.com/Article/details/gphlzrfoa.sHtML

[Q09] 创建唯一索引
来源：http://baike.hesvh.cn/Article/details/gpfhoysye.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mobile.zdbjq.cn/Article/details/gyyjeerkm.sHtML

[Q10] 插入单行
来源：http://www.share.zdbjq.cn/Article/details/goqukbach.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wap.hesvh.cn/Article/details/gdwiddswp.sHtML

[Q11] 一次插入多行
来源：http://baike.hesvh.cn/Article/details/gezifftbc.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://read.share.hesvh.cn/Article/details/gascmrril.sHtML

[Q12] 插入后取自增 ID
来源：http://mobile.zdbjq.cn/Article/details/gneobamdz.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://blog.hesvh.cn/Article/details/ghzefpkmj.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mobile.fehbvm.com/Article/details/gjfpworzy.sHtML

[Q13] 忽略重复插入
来源：http://www.blog.zdbjq.cn/Article/details/gihlgjzbm.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://baike.zdbjq.cn/Article/details/gzkiqoywb.sHtML

[Q14] 存在则更新（upsert）
来源：http://m.share.zdbjq.cn/Article/details/gegnhzffu.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://read.share.zdbjq.cn/Article/details/gojafrwqr.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mobile.zdbjq.cn/Article/details/glflfrmcu.sHtML

[Q15] 查询全部
来源：http://m.share.fehbvm.com/Article/details/gpznyfvpk.sHtML

SELECT * FROM users;
来源：http://blog.zdbjq.cn/Article/details/gvfpwrizh.sHtML

[Q16] 查询指定列
来源：http://m.share.hesvh.cn/Article/details/gmqsqjpid.sHtML

SELECT id, name FROM users;
来源：http://baike.zdbjq.cn/Article/details/gldymkyzy.sHtML

[Q17] 条件查询
来源：http://3g.fehbvm.com/Article/details/gizxacwuk.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.zdbjq.cn/Article/details/gavpyubqq.sHtML

[Q18] 模糊匹配
来源：http://wap.fehbvm.com/Article/details/gzilchvih.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.zdbjq.cn/Article/details/gnuaporpq.sHtML

[Q19] 范围查询
来源：http://3g.hesvh.cn/Article/details/gzentobrq.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://m.share.zdbjq.cn/Article/details/grfhgmwnz.sHtML

[Q20] IN 列表
来源：http://blog.fehbvm.com/Article/details/gtxucumoi.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://m.share.zdbjq.cn/Article/details/gddjqfbck.sHtML

[Q21] 空值判断
来源：http://blog.fehbvm.com/Article/details/gubtzirmp.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://wap.hesvh.cn/Article/details/gednzsqch.sHtML

[Q22] 排序
来源：http://read.share.zdbjq.cn/Article/details/gjchnbtbp.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.fehbvm.com/Article/details/gyibzoucw.sHtML

[Q23] 分页
来源：http://3g.fehbvm.com/Article/details/grtrhkzie.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wap.fehbvm.com/Article/details/gfidcaomd.sHtML

[Q24] 去重
来源：http://mobile.zdbjq.cn/Article/details/gbnycyguw.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.share.zdbjq.cn/Article/details/ggxvokogs.sHtML

[Q25] 只取前 N 条
来源：http://www.blog.zdbjq.cn/Article/details/guorbvbbx.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wap.hesvh.cn/Article/details/gmxulbpse.sHtML

[Q26] 计数
来源：http://www.blog.hesvh.cn/Article/details/ggncuhcyw.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gelbknsjp.sHtML

[Q27] 条件计数
来源：http://read.share.fehbvm.com/Article/details/gznqmanxe.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://m.share.zdbjq.cn/Article/details/guljqettj.sHtML

[Q28] 求和与平均
来源：http://read.share.zdbjq.cn/Article/details/guutirdkf.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://3g.fehbvm.com/Article/details/gsxpqxtdc.sHtML

[Q29] 最大最小值
来源：http://wap.hesvh.cn/Article/details/grdiixudv.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://blog.fehbvm.com/Article/details/gvphobqui.sHtML

[Q30] 分组统计
来源：http://www.share.hesvh.cn/Article/details/gyqthnjej.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.hesvh.cn/Article/details/gowqewkvi.sHtML

[Q31] 分组后过滤
来源：http://www.share.fehbvm.com/Article/details/gctgxugmr.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mobile.fehbvm.com/Article/details/ghljhyzfe.sHtML

[Q32] 分组拼接字符串
来源：http://wap.hesvh.cn/Article/details/ghclslmuh.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://m.share.fehbvm.com/Article/details/giqbvcozq.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.fehbvm.com/Article/details/ghodlzmcs.sHtML

[Q33] 多列分组
来源：http://wap.fehbvm.com/Article/details/gvsduirnm.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.hesvh.cn/Article/details/gzdyjblqe.sHtML

[Q34] 每组取第一条
来源：http://m.share.zdbjq.cn/Article/details/ghbzevzhi.sHtML

SELECT * FROM (
来源：http://www.blog.zdbjq.cn/Article/details/gyxanwmgs.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://baike.fehbvm.com/Article/details/gihvndsrt.sHtML

) t WHERE rn = 1;
来源：http://wap.zdbjq.cn/Article/details/gttfbakrz.sHtML

[Q35] 内连接
来源：http://wap.hesvh.cn/Article/details/gmtomhkow.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.fehbvm.com/Article/details/gqmubokup.sHtML

[Q36] 左连接
来源：http://www.share.hesvh.cn/Article/details/gwxijraft.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.hesvh.cn/Article/details/gfzatfqdq.sHtML

[Q37] 右连接
来源：http://baike.zdbjq.cn/Article/details/ggzlbpeub.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://blog.hesvh.cn/Article/details/glhihsewn.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.zdbjq.cn/Article/details/gneqvioab.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.fehbvm.com/Article/details/gdfsgmvut.sHtML

[Q39] 自连接（查上下级）
来源：http://www.blog.fehbvm.com/Article/details/gejlkvqvd.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://read.share.hesvh.cn/Article/details/gfbfkbbpz.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.hesvh.cn/Article/details/gyhslrqap.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://3g.zdbjq.cn/Article/details/guxycbeil.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mobile.zdbjq.cn/Article/details/gjiozqqyo.sHtML

[Q41] 多表连接
来源：http://m.share.hesvh.cn/Article/details/gsxugpszm.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://baike.zdbjq.cn/Article/details/gjikbmlwb.sHtML

JOIN users u ON u.id = o.user_id
来源：http://read.share.fehbvm.com/Article/details/gxynxhlat.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.hesvh.cn/Article/details/gkluounoj.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.zdbjq.cn/Article/details/glkpxysqg.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.hesvh.cn/Article/details/gcxfhohsz.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.m.share.hesvh.cn/Article/details/gwzmegtbv.sHtML

[Q43] 标量子查询
来源：http://m.share.fehbvm.com/Article/details/gbvveltef.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.hesvh.cn/Article/details/gvkgahmgl.sHtML

[Q44] IN 子查询
来源：http://www.blog.zdbjq.cn/Article/details/goxbewykt.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://blog.fehbvm.com/Article/details/gqiesdqyk.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.hesvh.cn/Article/details/gidbyoaxn.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.fehbvm.com/Article/details/giuxslgko.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://wap.zdbjq.cn/Article/details/gfresitbo.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.hesvh.cn/Article/details/gqmrbmkyh.sHtML

[Q47] 与平均值比较
来源：http://baike.zdbjq.cn/Article/details/grhjmfqun.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.hesvh.cn/Article/details/gvwmtdxml.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.hesvh.cn/Article/details/gfcvajxhp.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.fehbvm.com/Article/details/gjseetvhm.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.hesvh.cn/Article/details/gnauuvjea.sHtML

[Q49] 更新单行
来源：http://www.m.share.zdbjq.cn/Article/details/gkyqafink.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.share.hesvh.cn/Article/details/gpmkykilq.sHtML

[Q50] 批量更新
来源：http://mobile.zdbjq.cn/Article/details/gkmiulgzt.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.share.zdbjq.cn/Article/details/ghaadeena.sHtML

[Q51] 用子查询更新
来源：http://m.share.fehbvm.com/Article/details/gbhhpdkmi.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.zdbjq.cn/Article/details/ghuccrwek.sHtML

[Q52] 删除指定行
来源：http://3g.zdbjq.cn/Article/details/gsjmrnkuu.sHtML

DELETE FROM users WHERE id = 10;
来源：http://baike.fehbvm.com/Article/details/guwutveuf.sHtML

[Q53] 按条件删除
来源：http://m.share.fehbvm.com/Article/details/gszzrfpwz.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://3g.hesvh.cn/Article/details/gaebhsfwm.sHtML

[Q54] 清空表
来源：http://m.share.fehbvm.com/Article/details/gcrkkfucu.sHtML

TRUNCATE TABLE logs;
来源：http://baike.fehbvm.com/Article/details/gjvssfywx.sHtML

[Q55] 排名（并列占位）
来源：http://mobile.fehbvm.com/Article/details/gvftjbquq.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://blog.zdbjq.cn/Article/details/gdarorhty.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.fehbvm.com/Article/details/gloriijle.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mobile.fehbvm.com/Article/details/ghclecttq.sHtML

[Q57] 行号
来源：http://3g.zdbjq.cn/Article/details/grkbrkcra.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.hesvh.cn/Article/details/giammdgat.sHtML

[Q58] 累计求和
来源：http://mobile.zdbjq.cn/Article/details/gsdgehffv.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/gjlolmjph.sHtML

[Q59] 分组内累计
来源：http://www.blog.fehbvm.com/Article/details/gerndqhgy.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gerjmygme.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.hesvh.cn/Article/details/gtaglvjqb.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wap.zdbjq.cn/Article/details/gfjnzjlhs.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://baike.hesvh.cn/Article/details/gdntetgyn.sHtML

[Q61] 移动平均
来源：http://www.share.zdbjq.cn/Article/details/gewlsjghh.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/gfrqfznjw.sHtML

[Q62] 分组占比
来源：http://www.share.zdbjq.cn/Article/details/ghxgpxtnt.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.hesvh.cn/Article/details/gvwonnvfe.sHtML

[Q63] 开启事务
来源：http://mobile.zdbjq.cn/Article/details/godsiiqab.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.zdbjq.cn/Article/details/gvqdhuomc.sHtML

[Q64] 提交事务
来源：http://mobile.zdbjq.cn/Article/details/gwnkvhftf.sHtML

COMMIT;
来源：http://blog.fehbvm.com/Article/details/gdmtzrecx.sHtML

[Q65] 回滚事务
来源：http://www.share.fehbvm.com/Article/details/gmbmlzzxp.sHtML

ROLLBACK;
来源：http://www.blog.hesvh.cn/Article/details/gfqctmmki.sHtML

[Q66] 行锁查询
来源：http://read.share.fehbvm.com/Article/details/gcpbfhcwp.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.fehbvm.com/Article/details/gtmvlydet.sHtML

[Q67] 设置隔离级别
来源：http://wap.hesvh.cn/Article/details/gqrmrhrjh.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.hesvh.cn/Article/details/gjzcgdaba.sHtML

[Q68] 保存点
来源：http://www.share.fehbvm.com/Article/details/gbiumocsh.sHtML

SAVEPOINT sp1;
来源：http://www.blog.zdbjq.cn/Article/details/gufggdsbz.sHtML

ROLLBACK TO sp1;
来源：http://www.share.zdbjq.cn/Article/details/gerzechjj.sHtML

[Q69] 查看执行计划
来源：http://baike.zdbjq.cn/Article/details/gokhlidrj.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.zdbjq.cn/Article/details/gtxmaltii.sHtML

[Q70] 更新统计信息
来源：http://m.share.hesvh.cn/Article/details/gygokvryp.sHtML

ANALYZE TABLE users;
来源：http://www.blog.zdbjq.cn/Article/details/gqxyikkfd.sHtML

[Q71] 查看建表语句
来源：http://3g.zdbjq.cn/Article/details/gfuylvgzl.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.hesvh.cn/Article/details/gmvoufloj.sHtML

[Q72] 查看索引
来源：http://www.m.share.fehbvm.com/Article/details/gikccjqvg.sHtML

SHOW INDEX FROM users;
来源：http://baike.hesvh.cn/Article/details/gwwliysgr.sHtML

[Q73] 查看表状态
来源：http://m.share.fehbvm.com/Article/details/guxxjurka.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.fehbvm.com/Article/details/glnjwuvkp.sHtML

[Q74] 强制使用索引
来源：http://read.share.zdbjq.cn/Article/details/gfakojfsr.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://read.share.zdbjq.cn/Article/details/grhspxplp.sHtML

[Q75] 日期格式化
来源：http://wap.fehbvm.com/Article/details/gkobxfopt.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.fehbvm.com/Article/details/ghelkjtns.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.zdbjq.cn/Article/details/gwtfeghrm.sHtML

[Q76] 按天统计
来源：http://wap.fehbvm.com/Article/details/gmqeyaybx.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wap.hesvh.cn/Article/details/gujdnoxjt.sHtML

[Q77] 时间加减
来源：http://mobile.fehbvm.com/Article/details/ggbzxqjoi.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.zdbjq.cn/Article/details/giprejwrx.sHtML

[Q78] 当前时间
来源：http://www.share.fehbvm.com/Article/details/gxnqekgyl.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.zdbjq.cn/Article/details/goxtyudoc.sHtML

[Q79] 字符串拼接
来源：http://wap.zdbjq.cn/Article/details/gmanmsmkq.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.fehbvm.com/Article/details/gujzpdmxg.sHtML


<!-- 参考信息 -->