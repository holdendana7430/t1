代发 wailian999

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2qvyxqqol.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2jmqujyhd.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2bvyvimha.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2uckxshjq.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2zkwkbeoe.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2vzjzslxn.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2mxveaaai.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2cgbkdcse.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2zsouqvla.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2mbqdyker.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2zmsraohe.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2ycolhqfc.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2opvnjztn.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2denkcwin.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2qdwwwcfa.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2jaqeshbs.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2vgslpqzo.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2cumftqys.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2zhfmtyek.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2ywsrbdha.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2goqwccfo.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2rkiiwkik.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2ikvolvao.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2piktuvlo.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2gypcedtv.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2lbfetwqp.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2gcdpaqth.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2vmhvzyno.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2bfqrmjsz.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2ipijpzkb.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2ocddbxra.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2cmyhktrf.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2msirxnfm.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2hhiumbwh.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2hajdrnfl.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2ymjamnwj.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2fpzjqadu.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2ecdtnfsk.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2poyiquce.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2zvbgfppb.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2vnjxzlcj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jswqbmza.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2jixfssvy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mrnmfwqn.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2frgkgznw.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2kdmtintu.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2jjsyllvl.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2soigdohw.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2auxsmwxz.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2aqfikcqp.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2eqvhdyhv.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2ztlwdmwq.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2yknuunfp.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2bsbydfdh.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2yyvfspii.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2hjdxloto.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2ctzrwsoi.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2kxhdofgn.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2umktyahs.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2tzkouzny.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2lwhagmxe.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2vklyqupx.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2tmzjathm.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2icrsxstp.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2skzhwzrk.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2zcfthfwf.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2fsbhjtki.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2cxhfjyvi.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2oaybcxsc.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2pzghdjtl.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2tmlyqlvc.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2tpzihjkt.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2erpezdov.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2ifhscyze.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2uxfuqpmh.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2hkltzest.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2ossnpkjp.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2qdaupked.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2mxdnzgpx.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2mtdtxotn.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2xfhzmomi.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2atwoguiu.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2uhjrwxkg.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2cqdhpzvo.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2btoyztdk.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2qxlhtdnv.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2tudgwcdb.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2ipmapzjw.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2xbbijnea.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2fkovhgwc.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2rnhsyasg.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2wuaireee.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2oxtqbles.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2mfspskva.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2kxcloect.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2pldluqmt.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2vngcotjt.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2eecclaeu.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2zbltgpvx.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2domxphix.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2erezuvbg.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2exspqwfz.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2wrmirwlx.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2prraydkd.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2jqmgjqxh.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2wmemfrzl.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2vitdhfjz.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2icgmcsnr.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2rlurdtny.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2vcmzagin.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2xsnduldm.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2fphbqojf.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2xielicfn.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2wwldedxb.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2mwgpgutm.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2ihksnmnk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hnmesfnj.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2gjoeznez.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lfnnotgj.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2cixxhyzy.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2agkoztjj.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2xzgnpsdl.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2pynoxuwb.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2qtnflcbg.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2rrdjbhbj.html

);
来源：http://www.52xcode.cn/Article/details/gt2mpphjrac.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2ywkcekfm.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2vdffqneu.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2hzatlccg.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2iketwppn.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2zstdjnvs.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2dxkokevb.html

);
来源：http://www.52xcode.cn/Article/details/gt2ndyehjcm.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2zseqdetl.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2wwqdsmww.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2jtxzqmxe.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2zhjfqrpy.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2eceyavxj.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2ptgszjyd.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2kwfhgffc.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2aaztwzkl.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2zotmrzay.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2yrdbpevi.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2pcqkdgzi.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2zcfilakw.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2ahwovjga.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2eyvdihov.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2igewduhc.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2knhskhgh.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2blkrwkca.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2jvodhqdx.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2fwvvexpf.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2kzuyslsu.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2glqmziru.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2raeervij.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2guedmafi.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2vxbuztmx.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2uelcsaap.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2jyowxlyx.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2hinxnnlw.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2uuzqlckc.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2zaevprei.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2tpwdotwd.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2gzafcxdz.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2pvfbgyik.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2akxynjpr.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2enyndalv.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2irtcjsmv.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2laslogxr.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2trkopike.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2pjknjrge.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2frmymkst.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2bzcvbuws.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2aywxbiih.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2ezfsitky.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2vopkqloo.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2gkpndtfr.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2jlgovcft.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2kegoxpmx.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2urwtcpcf.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2nzzwnvni.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2cxqzrgig.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2wdgcdyvw.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2qlnlitnr.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2iglysziz.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2qozxkvkp.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2poqnflvg.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2yepuyngl.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2edeicoko.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2vubbsssv.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2cqexbpnr.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2zzyrktkd.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2vqagootp.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2wipxabmd.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2djblslcn.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2dvxwvcna.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2nrmdnxpd.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2rtfmtobx.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2gnpzpvsd.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2wjdsluvg.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2uubvpecd.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2tzovihvw.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2gdouplgn.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2dkrbfeuc.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2kaqlenpn.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2gbkxgpak.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2rnkjpuyi.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2snsuxznq.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2wjjeziur.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2egzcydjy.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2fcalgpaw.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2vdxflkfq.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2spzlxkmm.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2eksjrpeg.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2tnpnqqfl.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2bqhtyvgl.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2yxmtommg.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2opiuejpx.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2ltizqskr.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2zaupzkbh.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2uprbgrkp.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2ftuydgnr.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2zualmtmf.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2haswpvcd.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2tfnrecjj.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2rqpwfmug.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2nmxwnknl.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2eqtaeryd.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2gllgioor.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2pxxjrnfg.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2ztqxezrm.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2crfkxlsa.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2qlqsciqu.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2lpnknlib.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2myzvlcfo.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2rimrnphv.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2nimkuytj.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2alepjyde.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2mqfypyip.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2grcakogt.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2bbztunnv.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2jbfaepfi.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2pgpccmfo.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2rzbktueg.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2xgoqwphp.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2uiwyapym.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2prezxkre.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2vysftlll.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2stpscbjy.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2sycbsfhw.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2isbpvhlw.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2qadxbmpv.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2liutnrhb.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2hhilsrah.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2fwrsbkgh.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2cyuzzhbg.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2huewpzbd.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2nubhrblc.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2egfubmmc.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2hfbomazn.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2nilicmll.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2hsfdkvbv.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2fdzhcint.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2odvgagcs.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2xbqwtxys.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2rcwdwkay.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2ezckanhc.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2lwwufrda.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2qbwuqwee.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2vshfzmec.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2kymblpjo.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2szujwbcx.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2hysydllx.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2xyjvfnig.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2tahjsmju.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2njinvkhn.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2thjtemov.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2aivcphes.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2bohbaksl.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2talloqxg.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2shbhjbeh.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2pnvezkwg.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2grcjtikj.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2bcsuftpj.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2nfeyqtgk.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2glauxapc.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2ciwbeljs.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2xmulanyn.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2jlpiwkao.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2whrbdzfn.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2opxutdlr.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2pqhwkrty.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2zfxkgwkg.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2tovrzjps.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2hypizdui.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2slcpynei.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2mgjayage.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2odgttyjt.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2jvxobeuh.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2upcxwtfx.html


<!-- 参考信息 -->