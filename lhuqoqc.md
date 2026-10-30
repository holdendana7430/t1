代发 wailian999

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mobile.hesvh.cn/Article/details/gtxdcdtde.sHtML

TS:   // 同 JS
来源：http://read.share.fehbvm.com/Article/details/gbgroxncr.sHtML

Java: synchronized (this) { shared++; }
来源：http://3g.fehbvm.com/Article/details/grinvscni.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.m.share.fehbvm.com/Article/details/ggmwcbuzm.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.blog.hesvh.cn/Article/details/gsifzirkv.sHtML

C#:   lock (gate) { shared++; }
来源：http://m.share.fehbvm.com/Article/details/gzscmjtph.sHtML

[O04] 定义异步函数并等待
来源：http://m.share.zdbjq.cn/Article/details/gmwcnhyqx.sHtML

Py:   async def f():⏎    await g()
来源：http://wap.hesvh.cn/Article/details/gigvqrncl.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://baike.fehbvm.com/Article/details/gwltpfcus.sHtML

JS:   async function f() { await g(); }
来源：http://wap.fehbvm.com/Article/details/gbfufmgte.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://baike.hesvh.cn/Article/details/gfgpihynv.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mobile.fehbvm.com/Article/details/gwofxexwp.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://read.share.hesvh.cn/Article/details/gmnyqludu.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.m.share.zdbjq.cn/Article/details/gwmrvziyu.sHtML

C#:   async Task F() { await G(); }
来源：http://3g.hesvh.cn/Article/details/gfmxuxtff.sHtML

[O05] 并发执行并等待全部完成
来源：http://baike.fehbvm.com/Article/details/gmhhpmfkp.sHtML

Py:   asyncio.gather(*tasks)
来源：http://blog.zdbjq.cn/Article/details/gijezjfly.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wap.zdbjq.cn/Article/details/gfidyamux.sHtML

JS:   await Promise.all(tasks)
来源：http://m.share.zdbjq.cn/Article/details/gemltpssf.sHtML

TS:   await Promise.all(tasks)
来源：http://wap.hesvh.cn/Article/details/gyknuqrbk.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.blog.zdbjq.cn/Article/details/gvzhmsyke.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.m.share.zdbjq.cn/Article/details/gapxkbpgh.sHtML

Ruby: threads.map(&:join)
来源：http://3g.zdbjq.cn/Article/details/gsolnjjjr.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.blog.hesvh.cn/Article/details/gpkqxnjbd.sHtML

[O06] 使用进程池
来源：http://wap.hesvh.cn/Article/details/giwufjypt.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://read.share.zdbjq.cn/Article/details/gefhdnpst.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://blog.fehbvm.com/Article/details/gbgvszmqq.sHtML

JS:   // child_process / cluster 模块
来源：http://baike.hesvh.cn/Article/details/glgcujrdy.sHtML

TS:   // child_process / cluster 模块
来源：http://www.share.fehbvm.com/Article/details/gtudkyxjs.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mobile.fehbvm.com/Article/details/gfjsmtyho.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mobile.zdbjq.cn/Article/details/gqhldktif.sHtML

Ruby: // fork 块
来源：http://m.share.hesvh.cn/Article/details/gcdwabnxx.sHtML

C#:   Parallel.For
来源：http://www.m.share.hesvh.cn/Article/details/gcauwywqi.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gyydnxtgr.sHtML

P. 常用工具函数
来源：http://m.share.hesvh.cn/Article/details/gdnocodfe.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/geooetcnl.sHtML

[P01] 生成 UUID
来源：http://m.share.hesvh.cn/Article/details/gpdgonzdj.sHtML

Py:   str(uuid.uuid4())
来源：http://baike.hesvh.cn/Article/details/gagbnlifp.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.blog.hesvh.cn/Article/details/gawylhint.sHtML

JS:   crypto.randomUUID()
来源：http://blog.zdbjq.cn/Article/details/gfnfsdnin.sHtML

TS:   crypto.randomUUID()
来源：http://m.share.hesvh.cn/Article/details/gwpybdfkd.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.blog.hesvh.cn/Article/details/gmntyarga.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.share.zdbjq.cn/Article/details/gzqxxcdce.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.hesvh.cn/Article/details/gleamidyx.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://baike.hesvh.cn/Article/details/gmxmhvewg.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.blog.fehbvm.com/Article/details/gascfjmsm.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://baike.hesvh.cn/Article/details/gmvugddzc.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://blog.hesvh.cn/Article/details/gtgdgefxz.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.m.share.zdbjq.cn/Article/details/gvxyxjzsh.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mobile.fehbvm.com/Article/details/gfesqrrak.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://3g.hesvh.cn/Article/details/gmfrgggip.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://blog.fehbvm.com/Article/details/gurmfdvqc.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.blog.hesvh.cn/Article/details/gopdojhhh.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mobile.zdbjq.cn/Article/details/grzkbjpgv.sHtML

[P03] 生成短随机字符串
来源：http://www.blog.hesvh.cn/Article/details/gyjrllrdn.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.blog.zdbjq.cn/Article/details/gzjvfolkv.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://blog.zdbjq.cn/Article/details/gyupmxmhj.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.hesvh.cn/Article/details/gdackchfw.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.zdbjq.cn/Article/details/gxezdxtuy.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.m.share.hesvh.cn/Article/details/gfdakievg.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mobile.hesvh.cn/Article/details/gnornzodx.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://blog.zdbjq.cn/Article/details/gxiinkrpg.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://read.share.zdbjq.cn/Article/details/gmdqdnqde.sHtML

[P04] 求长度
来源：http://www.share.hesvh.cn/Article/details/gqqqbyhyr.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://3g.fehbvm.com/Article/details/geyzsezfi.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.hesvh.cn/Article/details/ggivqltlz.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.hesvh.cn/Article/details/gjduejmme.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.hesvh.cn/Article/details/gamgubszf.sHtML

Java: list.size();  map.size();  s.length()
来源：http://m.share.hesvh.cn/Article/details/gippeurlr.sHtML

Go:   len(arr);  len(m)
来源：http://baike.zdbjq.cn/Article/details/gqkjzaoxy.sHtML

Ruby: x.length;  x.size
来源：http://wap.zdbjq.cn/Article/details/glaknmsdz.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://blog.zdbjq.cn/Article/details/gosmkpfzm.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.share.hesvh.cn/Article/details/ghnjuplzp.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://read.share.fehbvm.com/Article/details/gsjhdcura.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://read.share.zdbjq.cn/Article/details/gwyjbctvi.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://m.share.fehbvm.com/Article/details/guxvhchmq.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.fehbvm.com/Article/details/gqoviappr.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://read.share.hesvh.cn/Article/details/gbpksummn.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://read.share.hesvh.cn/Article/details/gpdvdsvzx.sHtML

Ruby: a == b
来源：http://m.share.fehbvm.com/Article/details/gywgwulpn.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.m.share.hesvh.cn/Article/details/gstqeypqn.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://m.share.hesvh.cn/Article/details/gxkqilnfr.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://blog.zdbjq.cn/Article/details/grokrrnbk.sHtML

PHP:  if (empty($x)) {}
来源：http://www.m.share.fehbvm.com/Article/details/gcsjtdyvp.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://read.share.hesvh.cn/Article/details/gawlwujgb.sHtML

TS:   if (x == null) {}
来源：http://www.blog.zdbjq.cn/Article/details/gaicljuxe.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://wap.zdbjq.cn/Article/details/gamcpfvwo.sHtML

Go:   if x == nil {}
来源：http://m.share.hesvh.cn/Article/details/gjbrywpau.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wap.zdbjq.cn/Article/details/gswcduaef.sHtML

C#:   if (x is null) {}
来源：http://wap.fehbvm.com/Article/details/gumlpgoxn.sHtML

[P07] 防抖与节流
来源：http://mobile.zdbjq.cn/Article/details/gqolpehhb.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.blog.fehbvm.com/Article/details/gdshguqlf.sHtML

PHP:  // 手写时间戳比较
来源：http://www.share.zdbjq.cn/Article/details/ghqonkjeo.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.hesvh.cn/Article/details/gnxxfemmw.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.zdbjq.cn/Article/details/gloftacmu.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://blog.fehbvm.com/Article/details/gvtfjlmxb.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.share.fehbvm.com/Article/details/ggyalnesa.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.blog.fehbvm.com/Article/details/gwgfbuwro.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mobile.fehbvm.com/Article/details/gsdovqmzz.sHtML

[P08] 处理浮点精度问题
来源：http://blog.fehbvm.com/Article/details/ghymgbmec.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wap.fehbvm.com/Article/details/gmcadaebx.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://baike.fehbvm.com/Article/details/giavdnugc.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.blog.fehbvm.com/Article/details/gpjfqpnff.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mobile.fehbvm.com/Article/details/gfyhhgbog.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://read.share.hesvh.cn/Article/details/grvvxnuij.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.blog.zdbjq.cn/Article/details/grkfzofai.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mobile.zdbjq.cn/Article/details/gideithuz.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.m.share.fehbvm.com/Article/details/gqfaaoyfe.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gsccoeibs.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://read.share.fehbvm.com/Article/details/gsuwanvos.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gzgjuomuu.sHtML

[Q01] 创建表
来源：http://www.blog.fehbvm.com/Article/details/gsvskzfac.sHtML

CREATE TABLE users (
来源：http://read.share.hesvh.cn/Article/details/geoybbpok.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.hesvh.cn/Article/details/gouitxprm.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.share.hesvh.cn/Article/details/gxmpkccxd.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.share.hesvh.cn/Article/details/gdydqydck.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://blog.hesvh.cn/Article/details/gojxffxlh.sHtML

);
来源：http://m.share.hesvh.cn/Article/details/gkkjrgsxy.sHtML

[Q02] 创建带外键的表
来源：http://baike.zdbjq.cn/Article/details/ghvifzyus.sHtML

CREATE TABLE orders (
来源：http://mobile.zdbjq.cn/Article/details/gfeqlbpuk.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.fehbvm.com/Article/details/gaoieotkz.sHtML

user_id INT NOT NULL,
来源：http://www.m.share.hesvh.cn/Article/details/gvdsbzmzf.sHtML

amount DECIMAL(10, 2),
来源：http://3g.hesvh.cn/Article/details/gukboqmyr.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://baike.fehbvm.com/Article/details/gknuffubm.sHtML

);
来源：http://blog.hesvh.cn/Article/details/grcwgxycp.sHtML

[Q03] 增加列
来源：http://wap.hesvh.cn/Article/details/gdgjosskl.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.m.share.fehbvm.com/Article/details/gogspzpdt.sHtML

[Q04] 修改列类型
来源：http://blog.hesvh.cn/Article/details/gtsyevijy.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mobile.zdbjq.cn/Article/details/gncpqfprh.sHtML

[Q05] 重命名列
来源：http://wap.fehbvm.com/Article/details/gdkeyujmv.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.blog.hesvh.cn/Article/details/gwwqrbusd.sHtML

[Q06] 删除列
来源：http://read.share.hesvh.cn/Article/details/ggtjepogm.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://read.share.fehbvm.com/Article/details/glrbwkbpn.sHtML

[Q07] 删除表
来源：http://wap.zdbjq.cn/Article/details/gtplzziqs.sHtML

DROP TABLE IF EXISTS orders;
来源：http://3g.hesvh.cn/Article/details/gicmevyqi.sHtML

[Q08] 创建普通索引
来源：http://www.blog.hesvh.cn/Article/details/ggvhmkcbz.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://blog.zdbjq.cn/Article/details/gjapzvysp.sHtML

[Q09] 创建唯一索引
来源：http://m.share.hesvh.cn/Article/details/gdzhbqpip.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wap.fehbvm.com/Article/details/gsxrfyqok.sHtML

[Q10] 插入单行
来源：http://m.share.hesvh.cn/Article/details/gzlyocalw.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://blog.zdbjq.cn/Article/details/gjpdbufpe.sHtML

[Q11] 一次插入多行
来源：http://blog.hesvh.cn/Article/details/gvukkqbkv.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.share.hesvh.cn/Article/details/gihcmspuk.sHtML

[Q12] 插入后取自增 ID
来源：http://www.share.zdbjq.cn/Article/details/gxkqopqvi.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://3g.fehbvm.com/Article/details/gnwexfxrz.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wap.zdbjq.cn/Article/details/gmxikexle.sHtML

[Q13] 忽略重复插入
来源：http://blog.hesvh.cn/Article/details/glbahqtzx.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.m.share.hesvh.cn/Article/details/ghfxlmuvv.sHtML

[Q14] 存在则更新（upsert）
来源：http://baike.fehbvm.com/Article/details/ggtsdrqdf.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baike.zdbjq.cn/Article/details/gxntuieri.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://baike.hesvh.cn/Article/details/gowprvwua.sHtML

[Q15] 查询全部
来源：http://m.share.zdbjq.cn/Article/details/ggulnugvz.sHtML

SELECT * FROM users;
来源：http://www.share.zdbjq.cn/Article/details/grzafpdwj.sHtML

[Q16] 查询指定列
来源：http://wap.fehbvm.com/Article/details/griwiclpw.sHtML

SELECT id, name FROM users;
来源：http://blog.hesvh.cn/Article/details/gfefwuamz.sHtML

[Q17] 条件查询
来源：http://3g.fehbvm.com/Article/details/gvwldlvnj.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.zdbjq.cn/Article/details/gtsspxbeg.sHtML

[Q18] 模糊匹配
来源：http://www.m.share.zdbjq.cn/Article/details/gjxegsckp.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://3g.hesvh.cn/Article/details/grsueduvd.sHtML

[Q19] 范围查询
来源：http://3g.fehbvm.com/Article/details/gzwrjhhxo.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://3g.zdbjq.cn/Article/details/ghgwdmxew.sHtML

[Q20] IN 列表
来源：http://blog.zdbjq.cn/Article/details/gmjxqqlwl.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://blog.hesvh.cn/Article/details/gvitnlsba.sHtML

[Q21] 空值判断
来源：http://3g.fehbvm.com/Article/details/gejgoipdn.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.m.share.zdbjq.cn/Article/details/gppscigem.sHtML

[Q22] 排序
来源：http://read.share.zdbjq.cn/Article/details/gswbzimpf.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://blog.zdbjq.cn/Article/details/gbtejgkyu.sHtML

[Q23] 分页
来源：http://3g.hesvh.cn/Article/details/gixkjneaj.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.blog.hesvh.cn/Article/details/ghdmpdecr.sHtML

[Q24] 去重
来源：http://www.m.share.hesvh.cn/Article/details/genfmkwqv.sHtML

SELECT DISTINCT city FROM users;
来源：http://blog.zdbjq.cn/Article/details/gsraaxcte.sHtML

[Q25] 只取前 N 条
来源：http://3g.fehbvm.com/Article/details/gfcvsbzvx.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://3g.fehbvm.com/Article/details/gmlqtvvsz.sHtML

[Q26] 计数
来源：http://3g.fehbvm.com/Article/details/gygegsfwb.sHtML

SELECT COUNT(*) FROM users;
来源：http://3g.hesvh.cn/Article/details/gfvckssab.sHtML

[Q27] 条件计数
来源：http://3g.zdbjq.cn/Article/details/gllqtnncz.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gszubjggh.sHtML

[Q28] 求和与平均
来源：http://www.share.zdbjq.cn/Article/details/gvocoyyup.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/gypfgwftu.sHtML

[Q29] 最大最小值
来源：http://www.share.zdbjq.cn/Article/details/gbcmvzvls.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://blog.hesvh.cn/Article/details/gmqtmckxt.sHtML

[Q30] 分组统计
来源：http://read.share.fehbvm.com/Article/details/givockyxu.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.zdbjq.cn/Article/details/gnicpuzqx.sHtML

[Q31] 分组后过滤
来源：http://www.m.share.hesvh.cn/Article/details/gidyyvesi.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.blog.fehbvm.com/Article/details/gyucbqgvd.sHtML

[Q32] 分组拼接字符串
来源：http://blog.hesvh.cn/Article/details/ghzgzkahy.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.m.share.fehbvm.com/Article/details/gnfkfjige.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mobile.zdbjq.cn/Article/details/gwqdmnzue.sHtML

[Q33] 多列分组
来源：http://www.blog.hesvh.cn/Article/details/gyeghqdxq.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.m.share.hesvh.cn/Article/details/ghbyltuan.sHtML

[Q34] 每组取第一条
来源：http://www.m.share.fehbvm.com/Article/details/ghjmecklj.sHtML

SELECT * FROM (
来源：http://read.share.hesvh.cn/Article/details/gvvhbtsmt.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.fehbvm.com/Article/details/gwabnaqml.sHtML

) t WHERE rn = 1;
来源：http://3g.hesvh.cn/Article/details/gnizvrilm.sHtML

[Q35] 内连接
来源：http://3g.zdbjq.cn/Article/details/gjtqzpakh.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://read.share.hesvh.cn/Article/details/gguyyzqiy.sHtML

[Q36] 左连接
来源：http://read.share.fehbvm.com/Article/details/gexytnjae.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.hesvh.cn/Article/details/gvdbshpur.sHtML

[Q37] 右连接
来源：http://wap.zdbjq.cn/Article/details/gabkumqvb.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.share.zdbjq.cn/Article/details/gkblpewtc.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://3g.zdbjq.cn/Article/details/gpunluwox.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://baike.zdbjq.cn/Article/details/gexfikghm.sHtML

[Q39] 自连接（查上下级）
来源：http://baike.hesvh.cn/Article/details/gibcgduvl.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.m.share.fehbvm.com/Article/details/gbbklxhax.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.hesvh.cn/Article/details/glvbvunzl.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://m.share.zdbjq.cn/Article/details/gxiwzella.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.fehbvm.com/Article/details/gmuqhbjoj.sHtML

[Q41] 多表连接
来源：http://read.share.fehbvm.com/Article/details/ghwkjlvjh.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.blog.hesvh.cn/Article/details/gcuvgcexa.sHtML

JOIN users u ON u.id = o.user_id
来源：http://baike.fehbvm.com/Article/details/gmhsrpzwr.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.hesvh.cn/Article/details/gpgxljqzv.sHtML

[Q42] 连接条件附加过滤
来源：http://baike.fehbvm.com/Article/details/gooxhcerz.sHtML

SELECT u.name, o.amount FROM users u
来源：http://baike.fehbvm.com/Article/details/gwyexgxnt.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.fehbvm.com/Article/details/gqomucdlu.sHtML

[Q43] 标量子查询
来源：http://www.blog.fehbvm.com/Article/details/gfrysjwlb.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://blog.zdbjq.cn/Article/details/gwzkjajgb.sHtML

[Q44] IN 子查询
来源：http://wap.zdbjq.cn/Article/details/gphpssfoa.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.hesvh.cn/Article/details/giddjqyth.sHtML

[Q45] EXISTS 判断存在
来源：http://read.share.hesvh.cn/Article/details/gnpjyyjmr.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.hesvh.cn/Article/details/gmgrexxyi.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.share.zdbjq.cn/Article/details/ggxrvkpuq.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.fehbvm.com/Article/details/ghtumamyx.sHtML

[Q47] 与平均值比较
来源：http://baike.zdbjq.cn/Article/details/gveqbigjc.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.zdbjq.cn/Article/details/grnwyewol.sHtML

[Q48] CTE 公用表表达式
来源：http://mobile.zdbjq.cn/Article/details/ghqakzzsi.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://read.share.fehbvm.com/Article/details/glyeseuyd.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.fehbvm.com/Article/details/gdedzfony.sHtML

[Q49] 更新单行
来源：http://read.share.fehbvm.com/Article/details/gieheghdy.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://3g.hesvh.cn/Article/details/gvhsunkor.sHtML

[Q50] 批量更新
来源：http://www.share.fehbvm.com/Article/details/gyulqdnjm.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.hesvh.cn/Article/details/ghdonwnue.sHtML

[Q51] 用子查询更新
来源：http://m.share.hesvh.cn/Article/details/gwwuvapvr.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.share.hesvh.cn/Article/details/gcnaerfbp.sHtML

[Q52] 删除指定行
来源：http://www.share.hesvh.cn/Article/details/gfozvcfin.sHtML

DELETE FROM users WHERE id = 10;
来源：http://blog.hesvh.cn/Article/details/gyqfhukas.sHtML

[Q53] 按条件删除
来源：http://www.blog.fehbvm.com/Article/details/grodctohz.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.hesvh.cn/Article/details/gpmjdbblg.sHtML

[Q54] 清空表
来源：http://wap.hesvh.cn/Article/details/gzsghswbf.sHtML

TRUNCATE TABLE logs;
来源：http://m.share.fehbvm.com/Article/details/gevenaebu.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.zdbjq.cn/Article/details/gjvfyojyn.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.hesvh.cn/Article/details/gwofupaul.sHtML

[Q56] 密集排名（并列不占位）
来源：http://3g.zdbjq.cn/Article/details/gcrsindso.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.share.zdbjq.cn/Article/details/gqyedwztg.sHtML

[Q57] 行号
来源：http://read.share.fehbvm.com/Article/details/gsjzgmcwd.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.zdbjq.cn/Article/details/ghimvbfon.sHtML

[Q58] 累计求和
来源：http://www.share.hesvh.cn/Article/details/gehslfgvc.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.hesvh.cn/Article/details/gwcuhyeuu.sHtML

[Q59] 分组内累计
来源：http://mobile.zdbjq.cn/Article/details/gqdpsvkqw.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.hesvh.cn/Article/details/gpkrkecuc.sHtML

[Q60] 取上一行 / 下一行
来源：http://blog.hesvh.cn/Article/details/gngghdghr.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.zdbjq.cn/Article/details/gipvbemws.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.fehbvm.com/Article/details/gfgchlgep.sHtML

[Q61] 移动平均
来源：http://baike.zdbjq.cn/Article/details/glieutvdh.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.share.hesvh.cn/Article/details/gnjprorlk.sHtML

[Q62] 分组占比
来源：http://3g.zdbjq.cn/Article/details/griepjfji.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.fehbvm.com/Article/details/gvxumdtxv.sHtML

[Q63] 开启事务
来源：http://3g.zdbjq.cn/Article/details/gpxxnpfnq.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://3g.zdbjq.cn/Article/details/grqyhvoxm.sHtML

[Q64] 提交事务
来源：http://read.share.hesvh.cn/Article/details/gcukibevm.sHtML

COMMIT;
来源：http://wap.hesvh.cn/Article/details/gqqyetbac.sHtML

[Q65] 回滚事务
来源：http://wap.fehbvm.com/Article/details/gelqzeqvu.sHtML

ROLLBACK;
来源：http://www.m.share.hesvh.cn/Article/details/gbrwiraew.sHtML

[Q66] 行锁查询
来源：http://wap.hesvh.cn/Article/details/glzpkhita.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.zdbjq.cn/Article/details/gwumtyyac.sHtML

[Q67] 设置隔离级别
来源：http://3g.hesvh.cn/Article/details/gdozaggwb.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.fehbvm.com/Article/details/gnvnbfnhq.sHtML

[Q68] 保存点
来源：http://baike.fehbvm.com/Article/details/gepnsairf.sHtML

SAVEPOINT sp1;
来源：http://3g.zdbjq.cn/Article/details/gkwxqjdbw.sHtML

ROLLBACK TO sp1;
来源：http://wap.hesvh.cn/Article/details/gmggsbjhy.sHtML

[Q69] 查看执行计划
来源：http://mobile.zdbjq.cn/Article/details/gtmqseuwv.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.hesvh.cn/Article/details/gfsbpfcln.sHtML

[Q70] 更新统计信息
来源：http://www.share.fehbvm.com/Article/details/gkmpzwbcl.sHtML

ANALYZE TABLE users;
来源：http://read.share.fehbvm.com/Article/details/gqerqkdlw.sHtML

[Q71] 查看建表语句
来源：http://3g.hesvh.cn/Article/details/gsujzfwxk.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.zdbjq.cn/Article/details/ggaxebhsh.sHtML

[Q72] 查看索引
来源：http://blog.hesvh.cn/Article/details/gemwwdvjv.sHtML

SHOW INDEX FROM users;
来源：http://blog.fehbvm.com/Article/details/glzkiafiw.sHtML

[Q73] 查看表状态
来源：http://www.blog.zdbjq.cn/Article/details/giujjyiml.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.zdbjq.cn/Article/details/geiijivic.sHtML

[Q74] 强制使用索引
来源：http://m.share.fehbvm.com/Article/details/gcjaizfgu.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://baike.hesvh.cn/Article/details/gdkzwtqbi.sHtML

[Q75] 日期格式化
来源：http://m.share.fehbvm.com/Article/details/ghveeohvd.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.zdbjq.cn/Article/details/gkwhnwxaj.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.hesvh.cn/Article/details/gcakgaojf.sHtML

[Q76] 按天统计
来源：http://3g.zdbjq.cn/Article/details/gelqilprq.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.fehbvm.com/Article/details/gpbpkwcbo.sHtML

[Q77] 时间加减
来源：http://mobile.fehbvm.com/Article/details/gkuolwcup.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.zdbjq.cn/Article/details/glvftgroa.sHtML

[Q78] 当前时间
来源：http://m.share.fehbvm.com/Article/details/ggtvqipgj.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.zdbjq.cn/Article/details/ggnvmqcph.sHtML

[Q79] 字符串拼接
来源：http://www.share.zdbjq.cn/Article/details/gzyeoijyg.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.zdbjq.cn/Article/details/gvqendomh.sHtML

[Q80] 字符串截取
来源：http://mobile.zdbjq.cn/Article/details/giukydwyd.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.hesvh.cn/Article/details/ggunbqmjg.sHtML

[Q81] 字符串替换
来源：http://baike.zdbjq.cn/Article/details/ghnsaqbiu.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gowfwivjl.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.hesvh.cn/Article/details/gklbmjcsa.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.fehbvm.com/Article/details/gqrmnnwab.sHtML

[Q83] 大小写转换
来源：http://mobile.hesvh.cn/Article/details/gqcrlwqov.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.fehbvm.com/Article/details/gzqkaacym.sHtML


<!-- 参考信息 -->