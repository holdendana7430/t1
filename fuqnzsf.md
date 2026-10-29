代发 wailian999

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://m.share.fehbvm.com/Article/details/gfapmuuzu.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.zdbjq.cn/Article/details/gineyebqs.sHtML

Py:   with lock: shared += 1
来源：http://read.share.zdbjq.cn/Article/details/gikzdeaom.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://mobile.zdbjq.cn/Article/details/gbmdvfmpr.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mobile.fehbvm.com/Article/details/guitqtpko.sHtML

TS:   // 同 JS
来源：http://www.share.fehbvm.com/Article/details/gtcbjmqdm.sHtML

Java: synchronized (this) { shared++; }
来源：http://mobile.hesvh.cn/Article/details/gcnhdmxrs.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://baike.zdbjq.cn/Article/details/gqrfzjekj.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://3g.zdbjq.cn/Article/details/ggcuxhktm.sHtML

C#:   lock (gate) { shared++; }
来源：http://3g.fehbvm.com/Article/details/gdifsbihg.sHtML

[O04] 定义异步函数并等待
来源：http://wap.fehbvm.com/Article/details/gmfxkojdx.sHtML

Py:   async def f():⏎    await g()
来源：http://www.share.fehbvm.com/Article/details/guslgciww.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://m.share.fehbvm.com/Article/details/gtqggedoi.sHtML

JS:   async function f() { await g(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gmzvztwpw.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.share.hesvh.cn/Article/details/gcdwtxbkh.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.blog.hesvh.cn/Article/details/gvhwtrmti.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://read.share.zdbjq.cn/Article/details/gcuumxzjx.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://mobile.zdbjq.cn/Article/details/gzesvpfmv.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.zdbjq.cn/Article/details/gsxtzuytr.sHtML

[O05] 并发执行并等待全部完成
来源：http://mobile.zdbjq.cn/Article/details/gjcevkvvj.sHtML

Py:   asyncio.gather(*tasks)
来源：http://wap.hesvh.cn/Article/details/gtxgznxyw.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://blog.zdbjq.cn/Article/details/gwzqystgy.sHtML

JS:   await Promise.all(tasks)
来源：http://baike.hesvh.cn/Article/details/gmutbxpir.sHtML

TS:   await Promise.all(tasks)
来源：http://blog.fehbvm.com/Article/details/gllsirmrg.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://3g.fehbvm.com/Article/details/gfashpbhz.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mobile.fehbvm.com/Article/details/guxqwgyem.sHtML

Ruby: threads.map(&:join)
来源：http://m.share.fehbvm.com/Article/details/gykofartx.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://3g.hesvh.cn/Article/details/glkdwdvdp.sHtML

[O06] 使用进程池
来源：http://www.share.hesvh.cn/Article/details/gdyukuwoc.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mobile.fehbvm.com/Article/details/gaityumzu.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://wap.zdbjq.cn/Article/details/gsanzeedz.sHtML

JS:   // child_process / cluster 模块
来源：http://www.m.share.zdbjq.cn/Article/details/gsmbmxurq.sHtML

TS:   // child_process / cluster 模块
来源：http://www.share.fehbvm.com/Article/details/gufoyhrfz.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mobile.hesvh.cn/Article/details/gnguqznva.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wap.hesvh.cn/Article/details/glgmaazzx.sHtML

Ruby: // fork 块
来源：http://www.share.hesvh.cn/Article/details/gaxpplohe.sHtML

C#:   Parallel.For
来源：http://3g.zdbjq.cn/Article/details/gqnqpegot.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gcxtapbos.sHtML

P. 常用工具函数
来源：http://3g.hesvh.cn/Article/details/gkmoffzuk.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gnnzksssk.sHtML

[P01] 生成 UUID
来源：http://read.share.zdbjq.cn/Article/details/gkapzmwkn.sHtML

Py:   str(uuid.uuid4())
来源：http://wap.hesvh.cn/Article/details/gyuteniev.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://read.share.hesvh.cn/Article/details/gaegewobf.sHtML

JS:   crypto.randomUUID()
来源：http://mobile.hesvh.cn/Article/details/gfnnnynda.sHtML

TS:   crypto.randomUUID()
来源：http://blog.zdbjq.cn/Article/details/gftvwlibl.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.m.share.fehbvm.com/Article/details/gjfsefpff.sHtML

Go:   // 用 github.com/google/uuid
来源：http://baike.zdbjq.cn/Article/details/gnunxomej.sHtML

Ruby: SecureRandom.uuid
来源：http://3g.zdbjq.cn/Article/details/gsfxkbjsf.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://3g.hesvh.cn/Article/details/gzbdtpllw.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.zdbjq.cn/Article/details/gklvsuapb.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://m.share.hesvh.cn/Article/details/gmsukihsb.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://blog.hesvh.cn/Article/details/gejtcpkux.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.zdbjq.cn/Article/details/gutdsxckk.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.blog.fehbvm.com/Article/details/gnjjahhwy.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://read.share.fehbvm.com/Article/details/gctlpmsrs.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.blog.hesvh.cn/Article/details/gipesuion.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://read.share.hesvh.cn/Article/details/gzyzmibej.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.blog.fehbvm.com/Article/details/gunufmagc.sHtML

[P03] 生成短随机字符串
来源：http://blog.hesvh.cn/Article/details/gwuiprpoc.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.m.share.hesvh.cn/Article/details/gtghbovum.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wap.fehbvm.com/Article/details/gexqmtdxd.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.hesvh.cn/Article/details/gcpeemcei.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.hesvh.cn/Article/details/gmabztdkc.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.share.zdbjq.cn/Article/details/gnpwuqvdd.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.blog.fehbvm.com/Article/details/gflsmehjv.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://m.share.hesvh.cn/Article/details/gbxshtiqr.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wap.hesvh.cn/Article/details/gqsewdtgb.sHtML

[P04] 求长度
来源：http://mobile.hesvh.cn/Article/details/gsyptnalm.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.share.zdbjq.cn/Article/details/gzpnpjozv.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.hesvh.cn/Article/details/ghfllqfhe.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.fehbvm.com/Article/details/gfbfqmzdk.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.fehbvm.com/Article/details/gsofszgfy.sHtML

Java: list.size();  map.size();  s.length()
来源：http://wap.fehbvm.com/Article/details/gfcekiqwy.sHtML

Go:   len(arr);  len(m)
来源：http://www.m.share.hesvh.cn/Article/details/gdmjjecwk.sHtML

Ruby: x.length;  x.size
来源：http://www.share.hesvh.cn/Article/details/guwaqapqu.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://mobile.fehbvm.com/Article/details/glkmsfhyk.sHtML

[P05] 判断两个对象内容是否相等
来源：http://3g.zdbjq.cn/Article/details/gghsngavt.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.m.share.hesvh.cn/Article/details/gzdtvmnhb.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://blog.zdbjq.cn/Article/details/gwcktljis.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://3g.fehbvm.com/Article/details/gsbiniqaf.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.zdbjq.cn/Article/details/ggfoyrzmw.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://read.share.zdbjq.cn/Article/details/ghyrpwixm.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.fehbvm.com/Article/details/gswmuelpx.sHtML

Ruby: a == b
来源：http://3g.hesvh.cn/Article/details/gzcihpjdv.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://blog.fehbvm.com/Article/details/gaqvroyrp.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://read.share.fehbvm.com/Article/details/gxrmrqzaa.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.zdbjq.cn/Article/details/gmvlhmokw.sHtML

PHP:  if (empty($x)) {}
来源：http://blog.hesvh.cn/Article/details/gvllzyypx.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://baike.hesvh.cn/Article/details/guakzgudy.sHtML

TS:   if (x == null) {}
来源：http://read.share.hesvh.cn/Article/details/gqflkyyra.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://wap.hesvh.cn/Article/details/gwhyczgyg.sHtML

Go:   if x == nil {}
来源：http://www.share.zdbjq.cn/Article/details/gnhodakfw.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wap.zdbjq.cn/Article/details/gotmvnjwi.sHtML

C#:   if (x is null) {}
来源：http://blog.zdbjq.cn/Article/details/gmizfqlsf.sHtML

[P07] 防抖与节流
来源：http://read.share.zdbjq.cn/Article/details/gvfpyfwne.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wap.zdbjq.cn/Article/details/gdrwqncjs.sHtML

PHP:  // 手写时间戳比较
来源：http://mobile.fehbvm.com/Article/details/grrwrbbig.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.fehbvm.com/Article/details/gioffwdgr.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.zdbjq.cn/Article/details/gfwqrpagf.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.m.share.fehbvm.com/Article/details/gtllzttxo.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mobile.zdbjq.cn/Article/details/gxldpcahs.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.fehbvm.com/Article/details/gvggxigvb.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.blog.zdbjq.cn/Article/details/gnrjdipyy.sHtML

[P08] 处理浮点精度问题
来源：http://read.share.zdbjq.cn/Article/details/gqykivdxa.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wap.zdbjq.cn/Article/details/gpnrqjvfs.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mobile.zdbjq.cn/Article/details/gtyeyqqav.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mobile.hesvh.cn/Article/details/gdpqoinlo.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://3g.hesvh.cn/Article/details/guuwcyvdq.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.blog.hesvh.cn/Article/details/gyswpwxug.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://blog.hesvh.cn/Article/details/gtvkydxye.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://blog.hesvh.cn/Article/details/gsssuezuh.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.blog.fehbvm.com/Article/details/gxmberiyu.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gviqsriyz.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://baike.zdbjq.cn/Article/details/gdjtpnkry.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gvkrbyohq.sHtML

[Q01] 创建表
来源：http://www.share.hesvh.cn/Article/details/gxrwaxlay.sHtML

CREATE TABLE users (
来源：http://read.share.zdbjq.cn/Article/details/gtcctvwmn.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.hesvh.cn/Article/details/gvtmlhkjk.sHtML

name VARCHAR(50) NOT NULL,
来源：http://wap.hesvh.cn/Article/details/gzlfxdhpc.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.m.share.hesvh.cn/Article/details/gnpxxcikg.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.share.zdbjq.cn/Article/details/gmvmogywt.sHtML

);
来源：http://www.share.zdbjq.cn/Article/details/gazbymdud.sHtML

[Q02] 创建带外键的表
来源：http://www.blog.fehbvm.com/Article/details/grmcqiroj.sHtML

CREATE TABLE orders (
来源：http://read.share.hesvh.cn/Article/details/goncwunis.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.fehbvm.com/Article/details/gsacphfjw.sHtML

user_id INT NOT NULL,
来源：http://read.share.fehbvm.com/Article/details/gaimhorwe.sHtML

amount DECIMAL(10, 2),
来源：http://3g.hesvh.cn/Article/details/gnfeulohs.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://3g.zdbjq.cn/Article/details/guphvokiy.sHtML

);
来源：http://baike.fehbvm.com/Article/details/goigohixe.sHtML

[Q03] 增加列
来源：http://wap.zdbjq.cn/Article/details/gkduqqnga.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.share.fehbvm.com/Article/details/gtetxiedf.sHtML

[Q04] 修改列类型
来源：http://blog.fehbvm.com/Article/details/gcobkngjy.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wap.zdbjq.cn/Article/details/gowxigcjl.sHtML

[Q05] 重命名列
来源：http://wap.zdbjq.cn/Article/details/gasubexjb.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://read.share.fehbvm.com/Article/details/ganmvemmr.sHtML

[Q06] 删除列
来源：http://wap.zdbjq.cn/Article/details/gfwkjltnj.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://blog.zdbjq.cn/Article/details/glrztnbqb.sHtML

[Q07] 删除表
来源：http://www.blog.zdbjq.cn/Article/details/gctapwksr.sHtML

DROP TABLE IF EXISTS orders;
来源：http://wap.hesvh.cn/Article/details/gptvcbwyc.sHtML

[Q08] 创建普通索引
来源：http://mobile.hesvh.cn/Article/details/gznzuasag.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.share.zdbjq.cn/Article/details/gamiunjci.sHtML

[Q09] 创建唯一索引
来源：http://mobile.zdbjq.cn/Article/details/gjjxdsrbx.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://m.share.fehbvm.com/Article/details/gissrwspc.sHtML

[Q10] 插入单行
来源：http://www.blog.fehbvm.com/Article/details/gjljuuquk.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://read.share.hesvh.cn/Article/details/gzfgfspav.sHtML

[Q11] 一次插入多行
来源：http://m.share.hesvh.cn/Article/details/gvhqrtgex.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.fehbvm.com/Article/details/getpyjjim.sHtML

[Q12] 插入后取自增 ID
来源：http://m.share.fehbvm.com/Article/details/gdyhwtwde.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.share.zdbjq.cn/Article/details/gwdddqfvf.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://baike.hesvh.cn/Article/details/gpxmujvgy.sHtML

[Q13] 忽略重复插入
来源：http://baike.hesvh.cn/Article/details/gggnkmwpx.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://blog.fehbvm.com/Article/details/gyheaqlxz.sHtML

[Q14] 存在则更新（upsert）
来源：http://3g.zdbjq.cn/Article/details/gtmrzgcpp.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baike.hesvh.cn/Article/details/gglraclhr.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mobile.fehbvm.com/Article/details/gvucnqkta.sHtML

[Q15] 查询全部
来源：http://3g.fehbvm.com/Article/details/gaxsyyqbx.sHtML

SELECT * FROM users;
来源：http://mobile.hesvh.cn/Article/details/glwproyip.sHtML

[Q16] 查询指定列
来源：http://m.share.fehbvm.com/Article/details/gfbunwgvf.sHtML

SELECT id, name FROM users;
来源：http://baike.hesvh.cn/Article/details/giagzdqgg.sHtML

[Q17] 条件查询
来源：http://www.share.hesvh.cn/Article/details/goyytpczo.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gyhubshcy.sHtML

[Q18] 模糊匹配
来源：http://3g.hesvh.cn/Article/details/gfbdtcfny.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wap.zdbjq.cn/Article/details/gdsvgdhab.sHtML

[Q19] 范围查询
来源：http://wap.hesvh.cn/Article/details/glcyqmhwt.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mobile.zdbjq.cn/Article/details/gbfjkctch.sHtML

[Q20] IN 列表
来源：http://m.share.hesvh.cn/Article/details/gkykegjds.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.fehbvm.com/Article/details/gjhydldob.sHtML

[Q21] 空值判断
来源：http://read.share.hesvh.cn/Article/details/gluvtywpu.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://m.share.fehbvm.com/Article/details/gerzvqihh.sHtML

[Q22] 排序
来源：http://www.m.share.hesvh.cn/Article/details/ghuxrstns.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://read.share.zdbjq.cn/Article/details/gjqcqhdsu.sHtML

[Q23] 分页
来源：http://m.share.fehbvm.com/Article/details/gyxmulggg.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mobile.fehbvm.com/Article/details/gkgcpvcny.sHtML

[Q24] 去重
来源：http://www.share.fehbvm.com/Article/details/gezelyorh.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gqyapuisr.sHtML

[Q25] 只取前 N 条
来源：http://m.share.zdbjq.cn/Article/details/gmrswlyrg.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.hesvh.cn/Article/details/gadkhjwrl.sHtML

[Q26] 计数
来源：http://www.blog.hesvh.cn/Article/details/gtrfppgrf.sHtML

SELECT COUNT(*) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/ggdsxdkkn.sHtML

[Q27] 条件计数
来源：http://m.share.hesvh.cn/Article/details/gfrshrjni.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://read.share.fehbvm.com/Article/details/gmxeiirwp.sHtML

[Q28] 求和与平均
来源：http://www.blog.hesvh.cn/Article/details/gmlybmiqj.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://3g.hesvh.cn/Article/details/gbnfmgbvg.sHtML

[Q29] 最大最小值
来源：http://wap.hesvh.cn/Article/details/gqvfsctnm.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.fehbvm.com/Article/details/gcrpvoeeb.sHtML

[Q30] 分组统计
来源：http://www.m.share.zdbjq.cn/Article/details/gakbgumou.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.blog.zdbjq.cn/Article/details/gyocozjvn.sHtML

[Q31] 分组后过滤
来源：http://baike.fehbvm.com/Article/details/gdpbbmoyt.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://3g.fehbvm.com/Article/details/getsjbjge.sHtML

[Q32] 分组拼接字符串
来源：http://m.share.fehbvm.com/Article/details/gojjumtyd.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://blog.hesvh.cn/Article/details/gmfjvjwcj.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mobile.fehbvm.com/Article/details/gxlcfyyhl.sHtML

[Q33] 多列分组
来源：http://www.blog.fehbvm.com/Article/details/gbgkedumo.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wap.fehbvm.com/Article/details/gcvjjxxlp.sHtML

[Q34] 每组取第一条
来源：http://baike.fehbvm.com/Article/details/gvaivttgw.sHtML

SELECT * FROM (
来源：http://www.m.share.hesvh.cn/Article/details/gyxetsmgv.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mobile.zdbjq.cn/Article/details/gdsoelleb.sHtML

) t WHERE rn = 1;
来源：http://mobile.hesvh.cn/Article/details/gwxrbsjui.sHtML

[Q35] 内连接
来源：http://mobile.zdbjq.cn/Article/details/gslhpqixl.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wap.hesvh.cn/Article/details/ggzhqtddd.sHtML

[Q36] 左连接
来源：http://mobile.zdbjq.cn/Article/details/gmkjufcan.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.zdbjq.cn/Article/details/gyyyvasyo.sHtML

[Q37] 右连接
来源：http://blog.hesvh.cn/Article/details/gqjfycjvn.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.hesvh.cn/Article/details/gxwhfovtw.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://mobile.fehbvm.com/Article/details/gmnrofdte.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.fehbvm.com/Article/details/grdsodpik.sHtML

[Q39] 自连接（查上下级）
来源：http://wap.hesvh.cn/Article/details/gqdaushsc.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://m.share.zdbjq.cn/Article/details/gpbwgnxyi.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.zdbjq.cn/Article/details/gtcioxeyp.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.hesvh.cn/Article/details/gpmhmaeep.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://m.share.hesvh.cn/Article/details/gleuaemxy.sHtML

[Q41] 多表连接
来源：http://www.m.share.zdbjq.cn/Article/details/gragneeun.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.hesvh.cn/Article/details/gmadmquyl.sHtML

JOIN users u ON u.id = o.user_id
来源：http://read.share.hesvh.cn/Article/details/glebqthxv.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.blog.hesvh.cn/Article/details/gmixrtgrt.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.fehbvm.com/Article/details/gtiliddcz.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.m.share.fehbvm.com/Article/details/gmpovdbxe.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.m.share.zdbjq.cn/Article/details/gzdlrejpa.sHtML

[Q43] 标量子查询
来源：http://read.share.hesvh.cn/Article/details/gsvvixugh.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.hesvh.cn/Article/details/gulxtdhgh.sHtML

[Q44] IN 子查询
来源：http://www.m.share.zdbjq.cn/Article/details/gjdrmrexw.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://blog.hesvh.cn/Article/details/glemochrv.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.fehbvm.com/Article/details/giklshglw.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.zdbjq.cn/Article/details/gnlejvtkf.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.share.zdbjq.cn/Article/details/gkmftojfa.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.zdbjq.cn/Article/details/gutbkdloe.sHtML

[Q47] 与平均值比较
来源：http://3g.fehbvm.com/Article/details/gjftipxjw.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mobile.fehbvm.com/Article/details/gloihnuvq.sHtML

[Q48] CTE 公用表表达式
来源：http://mobile.zdbjq.cn/Article/details/gquohijhl.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.share.zdbjq.cn/Article/details/gvezhqbkh.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.fehbvm.com/Article/details/ghaqboqzm.sHtML

[Q49] 更新单行
来源：http://read.share.zdbjq.cn/Article/details/ghivmgicl.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.share.fehbvm.com/Article/details/gdmnyifve.sHtML

[Q50] 批量更新
来源：http://www.share.hesvh.cn/Article/details/gkoycyzli.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.blog.fehbvm.com/Article/details/ghmhqsmql.sHtML

[Q51] 用子查询更新
来源：http://www.m.share.zdbjq.cn/Article/details/gmjeaqimr.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.fehbvm.com/Article/details/gufuoqkpy.sHtML

[Q52] 删除指定行
来源：http://read.share.fehbvm.com/Article/details/gucjnzefl.sHtML

DELETE FROM users WHERE id = 10;
来源：http://blog.hesvh.cn/Article/details/gpqnvsazt.sHtML

[Q53] 按条件删除
来源：http://www.blog.hesvh.cn/Article/details/gmwpwwhgp.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.share.fehbvm.com/Article/details/gxcwoqxya.sHtML

[Q54] 清空表
来源：http://www.m.share.fehbvm.com/Article/details/gxrtsizjo.sHtML

TRUNCATE TABLE logs;
来源：http://www.blog.hesvh.cn/Article/details/gznlegfea.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.fehbvm.com/Article/details/gyvtnnurw.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.share.zdbjq.cn/Article/details/geaxpbjpt.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.fehbvm.com/Article/details/grrwkzivw.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://read.share.fehbvm.com/Article/details/gsiodjale.sHtML

[Q57] 行号
来源：http://www.share.fehbvm.com/Article/details/gnfvhlemb.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.fehbvm.com/Article/details/gbeizarir.sHtML

[Q58] 累计求和
来源：http://wap.zdbjq.cn/Article/details/gwnsyhvnf.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://read.share.hesvh.cn/Article/details/gdtfbzdgk.sHtML

[Q59] 分组内累计
来源：http://www.share.hesvh.cn/Article/details/gqafpdjco.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.hesvh.cn/Article/details/gaalleqdd.sHtML

[Q60] 取上一行 / 下一行
来源：http://read.share.hesvh.cn/Article/details/grninnnyn.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://blog.hesvh.cn/Article/details/gpwitdisg.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/gtgslqlpx.sHtML

[Q61] 移动平均
来源：http://3g.hesvh.cn/Article/details/gbvgvbkrp.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.fehbvm.com/Article/details/ggfpdpwit.sHtML

[Q62] 分组占比
来源：http://3g.fehbvm.com/Article/details/grzzlqmjs.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://baike.hesvh.cn/Article/details/gtbxtkzgh.sHtML

[Q63] 开启事务
来源：http://wap.fehbvm.com/Article/details/gdpkkkywr.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://3g.zdbjq.cn/Article/details/goeicnsbf.sHtML

[Q64] 提交事务
来源：http://wap.zdbjq.cn/Article/details/gvnskduba.sHtML

COMMIT;
来源：http://mobile.fehbvm.com/Article/details/grbrnplwf.sHtML

[Q65] 回滚事务
来源：http://read.share.hesvh.cn/Article/details/gtmgyltwq.sHtML

ROLLBACK;
来源：http://www.share.fehbvm.com/Article/details/grnqrtubp.sHtML

[Q66] 行锁查询
来源：http://www.blog.hesvh.cn/Article/details/gettkmkza.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mobile.zdbjq.cn/Article/details/gncitzqdb.sHtML

[Q67] 设置隔离级别
来源：http://wap.zdbjq.cn/Article/details/gbnvdzcko.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.zdbjq.cn/Article/details/ggodcsldl.sHtML

[Q68] 保存点
来源：http://baike.fehbvm.com/Article/details/gijgujshu.sHtML

SAVEPOINT sp1;
来源：http://blog.hesvh.cn/Article/details/glfrfdmay.sHtML

ROLLBACK TO sp1;
来源：http://3g.zdbjq.cn/Article/details/gxxssxmfd.sHtML

[Q69] 查看执行计划
来源：http://baike.zdbjq.cn/Article/details/ghmxpionh.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.zdbjq.cn/Article/details/gupcrqulk.sHtML

[Q70] 更新统计信息
来源：http://3g.fehbvm.com/Article/details/gfumbfvzs.sHtML

ANALYZE TABLE users;
来源：http://wap.fehbvm.com/Article/details/gcqeaakda.sHtML

[Q71] 查看建表语句
来源：http://wap.hesvh.cn/Article/details/gjvhwavbg.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wap.zdbjq.cn/Article/details/gdlrcbzst.sHtML

[Q72] 查看索引
来源：http://m.share.hesvh.cn/Article/details/guhtlkxpd.sHtML

SHOW INDEX FROM users;
来源：http://baike.hesvh.cn/Article/details/gngfxksyc.sHtML

[Q73] 查看表状态
来源：http://baike.zdbjq.cn/Article/details/gnfkrbtvb.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.hesvh.cn/Article/details/gnpbfefqo.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.zdbjq.cn/Article/details/gacotklmm.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.zdbjq.cn/Article/details/glbhtxtei.sHtML

[Q75] 日期格式化
来源：http://www.m.share.zdbjq.cn/Article/details/gcfviwxvj.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.hesvh.cn/Article/details/gcskwibso.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.fehbvm.com/Article/details/gwvmaaual.sHtML

[Q76] 按天统计
来源：http://m.share.zdbjq.cn/Article/details/ghfgujbia.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.zdbjq.cn/Article/details/gdqmfdksu.sHtML

[Q77] 时间加减
来源：http://www.blog.fehbvm.com/Article/details/gakuxsycm.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://m.share.zdbjq.cn/Article/details/godnwlkdh.sHtML

[Q78] 当前时间
来源：http://www.share.fehbvm.com/Article/details/gflpycsop.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.zdbjq.cn/Article/details/gvlsmzicr.sHtML

[Q79] 字符串拼接
来源：http://read.share.zdbjq.cn/Article/details/gugrdjaqk.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.fehbvm.com/Article/details/gmdmkvtsg.sHtML

[Q80] 字符串截取
来源：http://www.blog.fehbvm.com/Article/details/gxudgpbqo.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.hesvh.cn/Article/details/gxqaisyhh.sHtML

[Q81] 字符串替换
来源：http://read.share.fehbvm.com/Article/details/gzupandfw.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.hesvh.cn/Article/details/gytksezgf.sHtML


<!-- 参考信息 -->