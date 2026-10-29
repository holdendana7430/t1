代发 wailian999

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://baike.zdbjq.cn/Article/details/gjrsytcwt.sHtML

TS:   // 同 JS
来源：http://read.share.fehbvm.com/Article/details/gvmxgeoip.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.share.hesvh.cn/Article/details/glxjopihw.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.share.zdbjq.cn/Article/details/glejdhqre.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://read.share.fehbvm.com/Article/details/gfavrhotf.sHtML

C#:   lock (gate) { shared++; }
来源：http://3g.fehbvm.com/Article/details/gvklhhiyb.sHtML

[O04] 定义异步函数并等待
来源：http://wap.zdbjq.cn/Article/details/gmppeljlo.sHtML

Py:   async def f():⏎    await g()
来源：http://3g.fehbvm.com/Article/details/gttqebzgm.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://3g.fehbvm.com/Article/details/gnbtpgrft.sHtML

JS:   async function f() { await g(); }
来源：http://www.share.fehbvm.com/Article/details/gbqxdiicf.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.share.hesvh.cn/Article/details/gkurrjhbq.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.fehbvm.com/Article/details/glpgzrrxd.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://blog.fehbvm.com/Article/details/gwhdsmtvm.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://3g.fehbvm.com/Article/details/givkjrhnf.sHtML

C#:   async Task F() { await G(); }
来源：http://wap.hesvh.cn/Article/details/gcnrqgelc.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.m.share.zdbjq.cn/Article/details/gbgiaoogd.sHtML

Py:   asyncio.gather(*tasks)
来源：http://3g.zdbjq.cn/Article/details/grqeujryr.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://3g.fehbvm.com/Article/details/gmvzteppn.sHtML

JS:   await Promise.all(tasks)
来源：http://baike.zdbjq.cn/Article/details/gopupwkgd.sHtML

TS:   await Promise.all(tasks)
来源：http://baike.zdbjq.cn/Article/details/ghghjbkps.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://blog.zdbjq.cn/Article/details/gghagpmyx.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wap.hesvh.cn/Article/details/gyyfiryiw.sHtML

Ruby: threads.map(&:join)
来源：http://wap.zdbjq.cn/Article/details/givunupiq.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.m.share.hesvh.cn/Article/details/giszodqnz.sHtML

[O06] 使用进程池
来源：http://www.share.hesvh.cn/Article/details/gdfxglhgl.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://blog.fehbvm.com/Article/details/gomabwewk.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://3g.zdbjq.cn/Article/details/gzjhkcpgc.sHtML

JS:   // child_process / cluster 模块
来源：http://www.share.hesvh.cn/Article/details/ggqimfgin.sHtML

TS:   // child_process / cluster 模块
来源：http://www.blog.fehbvm.com/Article/details/gefclrwyu.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://blog.zdbjq.cn/Article/details/gxkbdugyv.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mobile.zdbjq.cn/Article/details/gwsapckas.sHtML

Ruby: // fork 块
来源：http://mobile.fehbvm.com/Article/details/gjjsnexsd.sHtML

C#:   Parallel.For
来源：http://www.share.fehbvm.com/Article/details/gmlbpcyrm.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gctaxiosx.sHtML

P. 常用工具函数
来源：http://www.share.zdbjq.cn/Article/details/gqcfexwbw.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/ghkiybfkt.sHtML

[P01] 生成 UUID
来源：http://read.share.zdbjq.cn/Article/details/gzyjrptjp.sHtML

Py:   str(uuid.uuid4())
来源：http://baike.fehbvm.com/Article/details/gkyojkosg.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mobile.zdbjq.cn/Article/details/gvgmqcbgc.sHtML

JS:   crypto.randomUUID()
来源：http://www.m.share.zdbjq.cn/Article/details/gyptxkzvx.sHtML

TS:   crypto.randomUUID()
来源：http://wap.zdbjq.cn/Article/details/gzblavqdt.sHtML

Java: UUID.randomUUID().toString()
来源：http://wap.fehbvm.com/Article/details/grlvvuwpq.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.zdbjq.cn/Article/details/gjoxlanjw.sHtML

Ruby: SecureRandom.uuid
来源：http://read.share.zdbjq.cn/Article/details/gcfjdsucd.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.blog.fehbvm.com/Article/details/gnqpkqtih.sHtML

[P02] MD5 / SHA256 摘要
来源：http://read.share.hesvh.cn/Article/details/gqoffzynm.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.m.share.zdbjq.cn/Article/details/gxtuebyaa.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://baike.fehbvm.com/Article/details/ghmfemczd.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wap.hesvh.cn/Article/details/gdelxozhu.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://baike.zdbjq.cn/Article/details/geibyxmcr.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://baike.fehbvm.com/Article/details/gwpaeugod.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://3g.zdbjq.cn/Article/details/ghhwofjxn.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://3g.hesvh.cn/Article/details/gtdfbhhfi.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.m.share.fehbvm.com/Article/details/gqivlcrbz.sHtML

[P03] 生成短随机字符串
来源：http://www.blog.zdbjq.cn/Article/details/gafcknxno.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://read.share.fehbvm.com/Article/details/gwxbukjne.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://read.share.hesvh.cn/Article/details/gaatlopni.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.hesvh.cn/Article/details/gnogiphwo.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.zdbjq.cn/Article/details/gbjqybtjx.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://3g.hesvh.cn/Article/details/ghvohyypf.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.fehbvm.com/Article/details/gfesxkika.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.share.zdbjq.cn/Article/details/gukhucktr.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.share.fehbvm.com/Article/details/gllnmdsoj.sHtML

[P04] 求长度
来源：http://wap.hesvh.cn/Article/details/gwwmfwuno.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://read.share.fehbvm.com/Article/details/gcybjhxrd.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.hesvh.cn/Article/details/gunsedopo.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.fehbvm.com/Article/details/gwabknplx.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.zdbjq.cn/Article/details/gglhoksmz.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.blog.hesvh.cn/Article/details/gsdniaadx.sHtML

Go:   len(arr);  len(m)
来源：http://www.share.hesvh.cn/Article/details/gqnidwugl.sHtML

Ruby: x.length;  x.size
来源：http://mobile.hesvh.cn/Article/details/gnbmtfxnl.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.blog.fehbvm.com/Article/details/gcfhsxcxe.sHtML

[P05] 判断两个对象内容是否相等
来源：http://baike.fehbvm.com/Article/details/gjilefqns.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.blog.zdbjq.cn/Article/details/gqlmqcgep.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://m.share.fehbvm.com/Article/details/geruywdkq.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wap.zdbjq.cn/Article/details/gotuvufof.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.zdbjq.cn/Article/details/gdrzqyeff.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://blog.fehbvm.com/Article/details/gmealekak.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://mobile.fehbvm.com/Article/details/gyezupqqr.sHtML

Ruby: a == b
来源：http://baike.fehbvm.com/Article/details/gmafelzai.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wap.fehbvm.com/Article/details/geyaiouke.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.blog.zdbjq.cn/Article/details/gorevcitx.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://blog.hesvh.cn/Article/details/gzysnrchy.sHtML

PHP:  if (empty($x)) {}
来源：http://read.share.fehbvm.com/Article/details/gzdaxibtm.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://3g.fehbvm.com/Article/details/glfvbdwew.sHtML

TS:   if (x == null) {}
来源：http://www.share.zdbjq.cn/Article/details/guivwawbq.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.share.zdbjq.cn/Article/details/gsdspzqzk.sHtML

Go:   if x == nil {}
来源：http://wap.hesvh.cn/Article/details/gruwukgbo.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.share.zdbjq.cn/Article/details/geaecawrb.sHtML

C#:   if (x is null) {}
来源：http://www.m.share.zdbjq.cn/Article/details/geiwtcjia.sHtML

[P07] 防抖与节流
来源：http://baike.zdbjq.cn/Article/details/gzcgedliu.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.m.share.hesvh.cn/Article/details/gbaouwsep.sHtML

PHP:  // 手写时间戳比较
来源：http://www.blog.zdbjq.cn/Article/details/gsvftmutp.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.hesvh.cn/Article/details/gfppecmos.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.hesvh.cn/Article/details/guedgzcim.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://blog.fehbvm.com/Article/details/grhrrlfrk.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.hesvh.cn/Article/details/ggahcpeug.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://read.share.zdbjq.cn/Article/details/gbdsblhci.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.share.hesvh.cn/Article/details/gkolsswjc.sHtML

[P08] 处理浮点精度问题
来源：http://www.share.hesvh.cn/Article/details/gopbrhhhp.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.blog.fehbvm.com/Article/details/gssizfyoz.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.fehbvm.com/Article/details/ginjuukpa.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://blog.hesvh.cn/Article/details/gwdjqkutc.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://read.share.zdbjq.cn/Article/details/gqhnskabp.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.m.share.hesvh.cn/Article/details/ggkoveptk.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.blog.fehbvm.com/Article/details/gfmdxeewv.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://baike.hesvh.cn/Article/details/gyzyvuveb.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mobile.hesvh.cn/Article/details/gmjpytmob.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gxgjaoevx.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://m.share.hesvh.cn/Article/details/ghjnvljch.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gekwdqgmn.sHtML

[Q01] 创建表
来源：http://www.blog.zdbjq.cn/Article/details/gjxhajcgu.sHtML

CREATE TABLE users (
来源：http://read.share.zdbjq.cn/Article/details/gizhevjuw.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.zdbjq.cn/Article/details/gqekmyveq.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.m.share.fehbvm.com/Article/details/gadbsjpwd.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.blog.hesvh.cn/Article/details/gqknksvid.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://baike.zdbjq.cn/Article/details/ghiyhrmcv.sHtML

);
来源：http://www.m.share.zdbjq.cn/Article/details/gxyojtgml.sHtML

[Q02] 创建带外键的表
来源：http://3g.zdbjq.cn/Article/details/gcvvgeojb.sHtML

CREATE TABLE orders (
来源：http://blog.hesvh.cn/Article/details/gtegfsgiq.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.zdbjq.cn/Article/details/ggafupwdp.sHtML

user_id INT NOT NULL,
来源：http://www.blog.zdbjq.cn/Article/details/gawlanlrh.sHtML

amount DECIMAL(10, 2),
来源：http://www.share.hesvh.cn/Article/details/gdrqvioku.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.share.zdbjq.cn/Article/details/gsbfdtxbz.sHtML

);
来源：http://read.share.hesvh.cn/Article/details/gzqlehwty.sHtML

[Q03] 增加列
来源：http://3g.fehbvm.com/Article/details/gpfyesyam.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wap.hesvh.cn/Article/details/gronkizrx.sHtML

[Q04] 修改列类型
来源：http://3g.fehbvm.com/Article/details/gsdfjpzvs.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://blog.fehbvm.com/Article/details/grbwlgonb.sHtML

[Q05] 重命名列
来源：http://mobile.fehbvm.com/Article/details/ggfwgdzhd.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.share.hesvh.cn/Article/details/gginssfjl.sHtML

[Q06] 删除列
来源：http://m.share.hesvh.cn/Article/details/gxibrjuyb.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.share.hesvh.cn/Article/details/gwhufrxmj.sHtML

[Q07] 删除表
来源：http://read.share.hesvh.cn/Article/details/gtvtnipoh.sHtML

DROP TABLE IF EXISTS orders;
来源：http://3g.zdbjq.cn/Article/details/ghpbdgwec.sHtML

[Q08] 创建普通索引
来源：http://blog.hesvh.cn/Article/details/gkkanxqbz.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://3g.fehbvm.com/Article/details/gqdmebeqo.sHtML

[Q09] 创建唯一索引
来源：http://www.blog.fehbvm.com/Article/details/gpfvgyseo.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mobile.fehbvm.com/Article/details/gwkwlarwj.sHtML

[Q10] 插入单行
来源：http://www.blog.zdbjq.cn/Article/details/gjfsuyprv.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.fehbvm.com/Article/details/gedzzjnyk.sHtML

[Q11] 一次插入多行
来源：http://www.blog.fehbvm.com/Article/details/gakkknlcm.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.hesvh.cn/Article/details/gghfiyjow.sHtML

[Q12] 插入后取自增 ID
来源：http://www.share.zdbjq.cn/Article/details/giokrsscy.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://read.share.hesvh.cn/Article/details/gikjouzwn.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://read.share.zdbjq.cn/Article/details/gefgofwoj.sHtML

[Q13] 忽略重复插入
来源：http://m.share.hesvh.cn/Article/details/ghnqlfupw.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.share.hesvh.cn/Article/details/ghwkeiyfr.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.share.zdbjq.cn/Article/details/gwrbzioqg.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://m.share.fehbvm.com/Article/details/gzndgcnae.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://read.share.zdbjq.cn/Article/details/gztqgiwsm.sHtML

[Q15] 查询全部
来源：http://www.share.fehbvm.com/Article/details/gxrwienqs.sHtML

SELECT * FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/ggtwgegjt.sHtML

[Q16] 查询指定列
来源：http://blog.fehbvm.com/Article/details/gvduspnsu.sHtML

SELECT id, name FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gqfypfjfl.sHtML

[Q17] 条件查询
来源：http://m.share.fehbvm.com/Article/details/gjrytfjjq.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.share.zdbjq.cn/Article/details/gcfphzgfw.sHtML

[Q18] 模糊匹配
来源：http://blog.zdbjq.cn/Article/details/gypjjdwoz.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wap.hesvh.cn/Article/details/ggvftgaso.sHtML

[Q19] 范围查询
来源：http://m.share.hesvh.cn/Article/details/gsliruskv.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://read.share.fehbvm.com/Article/details/ghdptlgak.sHtML

[Q20] IN 列表
来源：http://m.share.fehbvm.com/Article/details/gpveapiru.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.fehbvm.com/Article/details/grglwcuuq.sHtML

[Q21] 空值判断
来源：http://read.share.zdbjq.cn/Article/details/gxcutieso.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://wap.zdbjq.cn/Article/details/gwkslpycf.sHtML

[Q22] 排序
来源：http://m.share.zdbjq.cn/Article/details/gxgxeznhp.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://read.share.fehbvm.com/Article/details/gcrxdtdbc.sHtML

[Q23] 分页
来源：http://blog.hesvh.cn/Article/details/gihsrqfsq.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://m.share.zdbjq.cn/Article/details/gqpyilsiq.sHtML

[Q24] 去重
来源：http://mobile.zdbjq.cn/Article/details/gpubsfhxk.sHtML

SELECT DISTINCT city FROM users;
来源：http://baike.fehbvm.com/Article/details/gizrjjyfd.sHtML

[Q25] 只取前 N 条
来源：http://blog.fehbvm.com/Article/details/gxlgxshyk.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://baike.hesvh.cn/Article/details/gpsrfblwq.sHtML

[Q26] 计数
来源：http://m.share.zdbjq.cn/Article/details/gnczbskth.sHtML

SELECT COUNT(*) FROM users;
来源：http://m.share.fehbvm.com/Article/details/gzyvdwcek.sHtML

[Q27] 条件计数
来源：http://baike.zdbjq.cn/Article/details/gvsovletj.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.zdbjq.cn/Article/details/gzqvookzc.sHtML

[Q28] 求和与平均
来源：http://m.share.fehbvm.com/Article/details/gcrujwrqe.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/grjtpyytg.sHtML

[Q29] 最大最小值
来源：http://www.m.share.zdbjq.cn/Article/details/grzwxvaec.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://wap.zdbjq.cn/Article/details/gqcoafbdq.sHtML

[Q30] 分组统计
来源：http://www.blog.fehbvm.com/Article/details/gyhsfvjpd.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.zdbjq.cn/Article/details/gdgnuehsp.sHtML

[Q31] 分组后过滤
来源：http://read.share.zdbjq.cn/Article/details/gugoqledf.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.blog.zdbjq.cn/Article/details/gpgduxmat.sHtML

[Q32] 分组拼接字符串
来源：http://3g.fehbvm.com/Article/details/glrqiratk.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://3g.fehbvm.com/Article/details/ghgvsxapz.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wap.zdbjq.cn/Article/details/gwmotlrsf.sHtML

[Q33] 多列分组
来源：http://www.share.zdbjq.cn/Article/details/gazmnneeg.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.share.hesvh.cn/Article/details/ghicihqil.sHtML

[Q34] 每组取第一条
来源：http://blog.zdbjq.cn/Article/details/gwwtxkkbc.sHtML

SELECT * FROM (
来源：http://read.share.hesvh.cn/Article/details/goncprfcw.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mobile.fehbvm.com/Article/details/gjovncxpe.sHtML

) t WHERE rn = 1;
来源：http://www.share.zdbjq.cn/Article/details/gisfmvxou.sHtML

[Q35] 内连接
来源：http://m.share.hesvh.cn/Article/details/gwvoifvms.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wap.zdbjq.cn/Article/details/glvuaxpwf.sHtML

[Q36] 左连接
来源：http://3g.hesvh.cn/Article/details/glfwusvwf.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://read.share.hesvh.cn/Article/details/gwmoieooa.sHtML

[Q37] 右连接
来源：http://www.blog.hesvh.cn/Article/details/gxmarxndq.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://m.share.zdbjq.cn/Article/details/gopsqtafk.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://wap.hesvh.cn/Article/details/gkqlncmdn.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://blog.zdbjq.cn/Article/details/gauiawlxk.sHtML

[Q39] 自连接（查上下级）
来源：http://blog.zdbjq.cn/Article/details/gvbklfsnh.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.m.share.fehbvm.com/Article/details/gqgesvwra.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://m.share.hesvh.cn/Article/details/gcyvktijj.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://baike.fehbvm.com/Article/details/gyfucmmuz.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mobile.zdbjq.cn/Article/details/grccgxrix.sHtML

[Q41] 多表连接
来源：http://baike.hesvh.cn/Article/details/gresitbos.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://read.share.zdbjq.cn/Article/details/gzuwbnvux.sHtML

JOIN users u ON u.id = o.user_id
来源：http://mobile.hesvh.cn/Article/details/gyvexhyom.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.fehbvm.com/Article/details/gduigjacl.sHtML

[Q42] 连接条件附加过滤
来源：http://read.share.fehbvm.com/Article/details/gvitkoqmf.sHtML

SELECT u.name, o.amount FROM users u
来源：http://m.share.zdbjq.cn/Article/details/gklkzaymb.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wap.hesvh.cn/Article/details/grtdeqbpn.sHtML

[Q43] 标量子查询
来源：http://www.blog.fehbvm.com/Article/details/gaueueddv.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.m.share.hesvh.cn/Article/details/gtzgzqbvv.sHtML

[Q44] IN 子查询
来源：http://m.share.zdbjq.cn/Article/details/gtfsflruc.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://read.share.hesvh.cn/Article/details/gtxmhqfdf.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.fehbvm.com/Article/details/glcbfdvjk.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.hesvh.cn/Article/details/grknzbamn.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://3g.fehbvm.com/Article/details/geqrzzpfc.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.hesvh.cn/Article/details/gwmdxabzr.sHtML

[Q47] 与平均值比较
来源：http://baike.hesvh.cn/Article/details/gojzcmxgn.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.fehbvm.com/Article/details/gldhidzba.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.zdbjq.cn/Article/details/gwkkzvexj.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.share.fehbvm.com/Article/details/gtzamjocb.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.fehbvm.com/Article/details/gplgzzhcs.sHtML

[Q49] 更新单行
来源：http://mobile.fehbvm.com/Article/details/gryxsmxzx.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mobile.fehbvm.com/Article/details/gmiwuknty.sHtML

[Q50] 批量更新
来源：http://www.share.hesvh.cn/Article/details/gfjcrrfgj.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://baike.fehbvm.com/Article/details/gpaqkssfd.sHtML

[Q51] 用子查询更新
来源：http://read.share.fehbvm.com/Article/details/gmvjhwjzf.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://3g.fehbvm.com/Article/details/gragwhxzi.sHtML

[Q52] 删除指定行
来源：http://wap.zdbjq.cn/Article/details/glfinngnp.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.hesvh.cn/Article/details/gxomdocpo.sHtML

[Q53] 按条件删除
来源：http://baike.hesvh.cn/Article/details/gznrqheti.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.hesvh.cn/Article/details/gdxohcsvl.sHtML

[Q54] 清空表
来源：http://wap.hesvh.cn/Article/details/gvpcdxpld.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.zdbjq.cn/Article/details/gsbmebyrw.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.fehbvm.com/Article/details/gevosykja.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://3g.zdbjq.cn/Article/details/gbllxplqc.sHtML

[Q56] 密集排名（并列不占位）
来源：http://wap.fehbvm.com/Article/details/gizmtxeuo.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.hesvh.cn/Article/details/gssuxwurk.sHtML

[Q57] 行号
来源：http://mobile.zdbjq.cn/Article/details/gyqldzjce.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.zdbjq.cn/Article/details/gnbfbrycp.sHtML

[Q58] 累计求和
来源：http://3g.fehbvm.com/Article/details/gdmhfymrm.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/grfczxtxr.sHtML

[Q59] 分组内累计
来源：http://www.share.fehbvm.com/Article/details/gdtijqcjw.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gbhwulost.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.fehbvm.com/Article/details/glwzbrspc.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.zdbjq.cn/Article/details/gjbilopci.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://baike.fehbvm.com/Article/details/gnrnksyvm.sHtML

[Q61] 移动平均
来源：http://wap.fehbvm.com/Article/details/gvjbyxola.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/glzqyhxnl.sHtML

[Q62] 分组占比
来源：http://www.m.share.fehbvm.com/Article/details/gjmefcffh.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.hesvh.cn/Article/details/guktehsfr.sHtML

[Q63] 开启事务
来源：http://mobile.zdbjq.cn/Article/details/gmgviwcje.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.zdbjq.cn/Article/details/gelylzgch.sHtML

[Q64] 提交事务
来源：http://www.blog.hesvh.cn/Article/details/gxskxmkch.sHtML

COMMIT;
来源：http://mobile.zdbjq.cn/Article/details/gwwubydpl.sHtML

[Q65] 回滚事务
来源：http://www.blog.hesvh.cn/Article/details/gdataupts.sHtML

ROLLBACK;
来源：http://mobile.hesvh.cn/Article/details/gevcwcyqt.sHtML

[Q66] 行锁查询
来源：http://www.m.share.fehbvm.com/Article/details/gkohltwgc.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mobile.hesvh.cn/Article/details/glcsoqfoi.sHtML

[Q67] 设置隔离级别
来源：http://wap.fehbvm.com/Article/details/ghegfekwf.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.m.share.fehbvm.com/Article/details/gbwiychxa.sHtML

[Q68] 保存点
来源：http://m.share.fehbvm.com/Article/details/ggdlgqwge.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.fehbvm.com/Article/details/gdndjrati.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.fehbvm.com/Article/details/gtasdfooo.sHtML

[Q69] 查看执行计划
来源：http://www.share.zdbjq.cn/Article/details/gozlfqfwh.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.hesvh.cn/Article/details/glxktngns.sHtML

[Q70] 更新统计信息
来源：http://read.share.hesvh.cn/Article/details/gygsqqemw.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.zdbjq.cn/Article/details/gxrycxlgh.sHtML

[Q71] 查看建表语句
来源：http://www.share.fehbvm.com/Article/details/glhpmrpjv.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.hesvh.cn/Article/details/gkakbngde.sHtML

[Q72] 查看索引
来源：http://baike.fehbvm.com/Article/details/gqfnidffc.sHtML

SHOW INDEX FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gvzifryve.sHtML

[Q73] 查看表状态
来源：http://www.share.hesvh.cn/Article/details/gwztndcvt.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.hesvh.cn/Article/details/gohrqerjo.sHtML

[Q74] 强制使用索引
来源：http://m.share.zdbjq.cn/Article/details/gexuziozj.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.hesvh.cn/Article/details/ghenujwxh.sHtML

[Q75] 日期格式化
来源：http://baike.fehbvm.com/Article/details/gkszmufac.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.hesvh.cn/Article/details/gxucrhofa.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.hesvh.cn/Article/details/gvczjhcta.sHtML

[Q76] 按天统计
来源：http://read.share.fehbvm.com/Article/details/gbdydmvvc.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.zdbjq.cn/Article/details/gbiqckxnj.sHtML

[Q77] 时间加减
来源：http://read.share.hesvh.cn/Article/details/gxcdgeoao.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.hesvh.cn/Article/details/gnzkmoanj.sHtML

[Q78] 当前时间
来源：http://baike.zdbjq.cn/Article/details/gxwofndwl.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.zdbjq.cn/Article/details/gzlqwljpy.sHtML

[Q79] 字符串拼接
来源：http://m.share.fehbvm.com/Article/details/gmdbkjufj.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://m.share.hesvh.cn/Article/details/gfeseuati.sHtML

[Q80] 字符串截取
来源：http://mobile.hesvh.cn/Article/details/gvpxtydxd.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/ggxbldjio.sHtML

[Q81] 字符串替换
来源：http://m.share.fehbvm.com/Article/details/gkcbnxmic.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gyoybuoza.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.hesvh.cn/Article/details/ghxmdhivn.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gbfijilgf.sHtML

[Q83] 大小写转换
来源：http://read.share.hesvh.cn/Article/details/gvjowezpk.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.hesvh.cn/Article/details/gykscibvd.sHtML


<!-- 参考信息 -->