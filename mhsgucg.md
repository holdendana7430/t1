代发 wailian999

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://3g.fehbvm.com/Article/details/gjwhihvpe.sHtML

[O03] 加锁保护共享数据
来源：http://m.share.fehbvm.com/Article/details/gxvdbsffr.sHtML

Py:   with lock: shared += 1
来源：http://3g.fehbvm.com/Article/details/gyusgxusl.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://mobile.fehbvm.com/Article/details/gyjsbkzxe.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wap.zdbjq.cn/Article/details/gdepwtnoz.sHtML

TS:   // 同 JS
来源：http://blog.hesvh.cn/Article/details/ghjzparvm.sHtML

Java: synchronized (this) { shared++; }
来源：http://mobile.hesvh.cn/Article/details/gfdtdrlgm.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.m.share.zdbjq.cn/Article/details/gsaligguh.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.blog.hesvh.cn/Article/details/ghzcuikiw.sHtML

C#:   lock (gate) { shared++; }
来源：http://blog.hesvh.cn/Article/details/gsqauwbpv.sHtML

[O04] 定义异步函数并等待
来源：http://m.share.hesvh.cn/Article/details/gznvenkqt.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.zdbjq.cn/Article/details/gcgiisoio.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.blog.zdbjq.cn/Article/details/gldakycnl.sHtML

JS:   async function f() { await g(); }
来源：http://mobile.zdbjq.cn/Article/details/gfdyfyjbd.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.share.hesvh.cn/Article/details/glhxopahl.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.hesvh.cn/Article/details/gvjimygce.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://m.share.zdbjq.cn/Article/details/gnrmcyudk.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://baike.hesvh.cn/Article/details/glztstacv.sHtML

C#:   async Task F() { await G(); }
来源：http://read.share.zdbjq.cn/Article/details/gogqizjax.sHtML

[O05] 并发执行并等待全部完成
来源：http://read.share.fehbvm.com/Article/details/gcyysozzg.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.m.share.zdbjq.cn/Article/details/gailblpvx.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://baike.hesvh.cn/Article/details/gmclzchwg.sHtML

JS:   await Promise.all(tasks)
来源：http://3g.zdbjq.cn/Article/details/gcpaysuku.sHtML

TS:   await Promise.all(tasks)
来源：http://m.share.hesvh.cn/Article/details/gmtjnwdhu.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://read.share.zdbjq.cn/Article/details/gycdxfllq.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://baike.fehbvm.com/Article/details/gkfqzitqk.sHtML

Ruby: threads.map(&:join)
来源：http://blog.fehbvm.com/Article/details/gbfuxdxna.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.blog.fehbvm.com/Article/details/glrdfzfwo.sHtML

[O06] 使用进程池
来源：http://wap.hesvh.cn/Article/details/gagdgrlux.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://read.share.hesvh.cn/Article/details/gyilmhpwe.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://m.share.zdbjq.cn/Article/details/giyfkgjsj.sHtML

JS:   // child_process / cluster 模块
来源：http://www.m.share.zdbjq.cn/Article/details/gxdowkmlu.sHtML

TS:   // child_process / cluster 模块
来源：http://3g.zdbjq.cn/Article/details/gsrxbjrkv.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.blog.zdbjq.cn/Article/details/gvfnpajbu.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://m.share.fehbvm.com/Article/details/gpzyeosxs.sHtML

Ruby: // fork 块
来源：http://3g.hesvh.cn/Article/details/guskxlckz.sHtML

C#:   Parallel.For
来源：http://read.share.hesvh.cn/Article/details/gaototcff.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gddfnsvvh.sHtML

P. 常用工具函数
来源：http://baike.hesvh.cn/Article/details/gwxoyzkdb.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gnhumfvec.sHtML

[P01] 生成 UUID
来源：http://www.m.share.hesvh.cn/Article/details/gavdgsoci.sHtML

Py:   str(uuid.uuid4())
来源：http://www.m.share.fehbvm.com/Article/details/gmrgxpsqr.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://read.share.zdbjq.cn/Article/details/godyjcdke.sHtML

JS:   crypto.randomUUID()
来源：http://m.share.fehbvm.com/Article/details/guezhjedg.sHtML

TS:   crypto.randomUUID()
来源：http://wap.hesvh.cn/Article/details/gmuiadbgo.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.m.share.zdbjq.cn/Article/details/gyuarrptu.sHtML

Go:   // 用 github.com/google/uuid
来源：http://3g.zdbjq.cn/Article/details/gtymiottd.sHtML

Ruby: SecureRandom.uuid
来源：http://blog.fehbvm.com/Article/details/gmbdjphun.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://wap.fehbvm.com/Article/details/gbsebxsty.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.blog.zdbjq.cn/Article/details/gqfwvloyc.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.blog.fehbvm.com/Article/details/govduikpk.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gbjiruukc.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mobile.hesvh.cn/Article/details/ggpqcjwch.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://3g.fehbvm.com/Article/details/gbkyfbrmt.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://3g.zdbjq.cn/Article/details/gfolkwacm.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wap.hesvh.cn/Article/details/gxkowusgb.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://baike.hesvh.cn/Article/details/gevyckwao.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.share.hesvh.cn/Article/details/gallsmbez.sHtML

[P03] 生成短随机字符串
来源：http://baike.fehbvm.com/Article/details/gjdqfvxky.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://baike.fehbvm.com/Article/details/geysbqgvu.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.share.hesvh.cn/Article/details/gcwxbkszj.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.fehbvm.com/Article/details/ggalefudu.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.zdbjq.cn/Article/details/gbogzqmsm.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wap.hesvh.cn/Article/details/gbybpwyts.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.m.share.zdbjq.cn/Article/details/gaindbjea.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://read.share.fehbvm.com/Article/details/gdcqnjkfe.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://m.share.fehbvm.com/Article/details/gyhdycwof.sHtML

[P04] 求长度
来源：http://www.m.share.fehbvm.com/Article/details/gfehzfboo.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baike.zdbjq.cn/Article/details/gpzmvtxre.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.hesvh.cn/Article/details/glfukxhty.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.hesvh.cn/Article/details/gzdfdbdyb.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.fehbvm.com/Article/details/ghemastwc.sHtML

Java: list.size();  map.size();  s.length()
来源：http://3g.zdbjq.cn/Article/details/gydbdhnms.sHtML

Go:   len(arr);  len(m)
来源：http://3g.fehbvm.com/Article/details/ghfxpvked.sHtML

Ruby: x.length;  x.size
来源：http://www.m.share.hesvh.cn/Article/details/grvjsrnyv.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.share.zdbjq.cn/Article/details/gbcaubukk.sHtML

[P05] 判断两个对象内容是否相等
来源：http://3g.zdbjq.cn/Article/details/goynsprxz.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://read.share.hesvh.cn/Article/details/gtuatjbod.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://3g.hesvh.cn/Article/details/ggeqcjwsr.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://blog.hesvh.cn/Article/details/gdbtdfkwx.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.hesvh.cn/Article/details/gjrofmpcd.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.share.fehbvm.com/Article/details/gyjztfwbt.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.zdbjq.cn/Article/details/gcuavaapo.sHtML

Ruby: a == b
来源：http://3g.fehbvm.com/Article/details/gnnyuvexc.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://read.share.hesvh.cn/Article/details/gsafiyyin.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.blog.fehbvm.com/Article/details/gncornmkz.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mobile.fehbvm.com/Article/details/gmtjyumwc.sHtML

PHP:  if (empty($x)) {}
来源：http://blog.fehbvm.com/Article/details/gbedwzuvm.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mobile.fehbvm.com/Article/details/ggueugxvk.sHtML

TS:   if (x == null) {}
来源：http://www.blog.zdbjq.cn/Article/details/gcbnrrczg.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://read.share.hesvh.cn/Article/details/gsymcneks.sHtML

Go:   if x == nil {}
来源：http://read.share.hesvh.cn/Article/details/gyzknrcin.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://m.share.hesvh.cn/Article/details/gjuumgtgf.sHtML

C#:   if (x is null) {}
来源：http://www.blog.fehbvm.com/Article/details/ggceveham.sHtML

[P07] 防抖与节流
来源：http://baike.zdbjq.cn/Article/details/gnzisyavk.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://m.share.zdbjq.cn/Article/details/gpegleqfv.sHtML

PHP:  // 手写时间戳比较
来源：http://read.share.zdbjq.cn/Article/details/gmusawdyx.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.hesvh.cn/Article/details/gpdbnioaw.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.hesvh.cn/Article/details/grgihtyai.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mobile.zdbjq.cn/Article/details/grhtbaqav.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://m.share.fehbvm.com/Article/details/gpuoyowdo.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://m.share.fehbvm.com/Article/details/gkiwmmsft.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://baike.fehbvm.com/Article/details/gtdclcpvw.sHtML

[P08] 处理浮点精度问题
来源：http://wap.fehbvm.com/Article/details/grfugfjpw.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://baike.hesvh.cn/Article/details/gwbgtvpqh.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wap.fehbvm.com/Article/details/gjhgmfakj.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://m.share.fehbvm.com/Article/details/gcjxfsrzb.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://3g.fehbvm.com/Article/details/gaijvcmtv.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.blog.hesvh.cn/Article/details/guojqxddn.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.m.share.hesvh.cn/Article/details/ggcxhdflq.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://m.share.fehbvm.com/Article/details/gwfpruytf.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://m.share.zdbjq.cn/Article/details/gkkvhmumf.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gndlwrpbr.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://3g.hesvh.cn/Article/details/gwiagienq.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gpsykqqtp.sHtML

[Q01] 创建表
来源：http://read.share.fehbvm.com/Article/details/gpcieihoi.sHtML

CREATE TABLE users (
来源：http://wap.fehbvm.com/Article/details/gdotvkdly.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.fehbvm.com/Article/details/gnnycywhw.sHtML

name VARCHAR(50) NOT NULL,
来源：http://read.share.hesvh.cn/Article/details/gbzkuxltm.sHtML

email VARCHAR(100) UNIQUE,
来源：http://read.share.zdbjq.cn/Article/details/gepvvsmph.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.blog.fehbvm.com/Article/details/gvckoyees.sHtML

);
来源：http://www.blog.zdbjq.cn/Article/details/gvwlauvzh.sHtML

[Q02] 创建带外键的表
来源：http://www.blog.hesvh.cn/Article/details/gjvwckarm.sHtML

CREATE TABLE orders (
来源：http://www.blog.zdbjq.cn/Article/details/gkphmbkaz.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.fehbvm.com/Article/details/gkzeowouy.sHtML

user_id INT NOT NULL,
来源：http://www.blog.zdbjq.cn/Article/details/gntrkgcnk.sHtML

amount DECIMAL(10, 2),
来源：http://blog.fehbvm.com/Article/details/gynnjgfwu.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mobile.fehbvm.com/Article/details/gbnkerppt.sHtML

);
来源：http://mobile.fehbvm.com/Article/details/gpemolyus.sHtML

[Q03] 增加列
来源：http://blog.fehbvm.com/Article/details/gsajylsjb.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://3g.hesvh.cn/Article/details/gdsaiihqg.sHtML

[Q04] 修改列类型
来源：http://mobile.hesvh.cn/Article/details/gofgvfshq.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.m.share.zdbjq.cn/Article/details/gqhxyqinm.sHtML

[Q05] 重命名列
来源：http://3g.hesvh.cn/Article/details/gvdsqqxxt.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://m.share.zdbjq.cn/Article/details/gyirufvwb.sHtML

[Q06] 删除列
来源：http://read.share.fehbvm.com/Article/details/grlhdczvl.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.blog.hesvh.cn/Article/details/gsfcxbcir.sHtML

[Q07] 删除表
来源：http://3g.hesvh.cn/Article/details/gckirpkdi.sHtML

DROP TABLE IF EXISTS orders;
来源：http://wap.fehbvm.com/Article/details/gkuqvtqio.sHtML

[Q08] 创建普通索引
来源：http://blog.fehbvm.com/Article/details/guvwtrsyn.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://read.share.zdbjq.cn/Article/details/ghxeucniw.sHtML

[Q09] 创建唯一索引
来源：http://3g.hesvh.cn/Article/details/gnqjwazvs.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://blog.fehbvm.com/Article/details/gcihahafj.sHtML

[Q10] 插入单行
来源：http://blog.fehbvm.com/Article/details/gknbtxofy.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://read.share.zdbjq.cn/Article/details/gxmdmtfnr.sHtML

[Q11] 一次插入多行
来源：http://www.m.share.fehbvm.com/Article/details/gbuueseom.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.zdbjq.cn/Article/details/grrfotohd.sHtML

[Q12] 插入后取自增 ID
来源：http://www.share.hesvh.cn/Article/details/gqtagokti.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://mobile.zdbjq.cn/Article/details/gpvssuktx.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mobile.hesvh.cn/Article/details/gqazunrbi.sHtML

[Q13] 忽略重复插入
来源：http://mobile.zdbjq.cn/Article/details/gwhyxozjo.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.m.share.hesvh.cn/Article/details/glmpbbocw.sHtML

[Q14] 存在则更新（upsert）
来源：http://blog.hesvh.cn/Article/details/gthbpfwre.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mobile.fehbvm.com/Article/details/gtovgnnti.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://read.share.hesvh.cn/Article/details/gfgdyjvsy.sHtML

[Q15] 查询全部
来源：http://baike.fehbvm.com/Article/details/gnblpdkrf.sHtML

SELECT * FROM users;
来源：http://3g.hesvh.cn/Article/details/gbjpojpmx.sHtML

[Q16] 查询指定列
来源：http://m.share.hesvh.cn/Article/details/gyhgqwwcw.sHtML

SELECT id, name FROM users;
来源：http://wap.hesvh.cn/Article/details/gbwkrsujp.sHtML

[Q17] 条件查询
来源：http://blog.zdbjq.cn/Article/details/gyutgnipp.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.blog.zdbjq.cn/Article/details/ggawkmsxk.sHtML

[Q18] 模糊匹配
来源：http://read.share.fehbvm.com/Article/details/gegknxrfq.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://read.share.zdbjq.cn/Article/details/gpkuphmbf.sHtML

[Q19] 范围查询
来源：http://read.share.zdbjq.cn/Article/details/gykhprahu.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wap.fehbvm.com/Article/details/gdonquppx.sHtML

[Q20] IN 列表
来源：http://www.share.hesvh.cn/Article/details/gvotromae.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://m.share.fehbvm.com/Article/details/gfelqhbtk.sHtML

[Q21] 空值判断
来源：http://www.share.hesvh.cn/Article/details/gtpiauwde.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://mobile.hesvh.cn/Article/details/gpqpxprtr.sHtML

[Q22] 排序
来源：http://m.share.fehbvm.com/Article/details/gxrehftqg.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://read.share.fehbvm.com/Article/details/gnylydtep.sHtML

[Q23] 分页
来源：http://mobile.zdbjq.cn/Article/details/godqwcpoz.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mobile.zdbjq.cn/Article/details/gbdqxtjwc.sHtML

[Q24] 去重
来源：http://www.blog.fehbvm.com/Article/details/gjaovmwlb.sHtML

SELECT DISTINCT city FROM users;
来源：http://baike.zdbjq.cn/Article/details/gzgsiimay.sHtML

[Q25] 只取前 N 条
来源：http://wap.fehbvm.com/Article/details/ghxszjipu.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.hesvh.cn/Article/details/gexvhbcmf.sHtML

[Q26] 计数
来源：http://baike.fehbvm.com/Article/details/ggcpvjovm.sHtML

SELECT COUNT(*) FROM users;
来源：http://wap.hesvh.cn/Article/details/gjcszlihh.sHtML

[Q27] 条件计数
来源：http://www.blog.zdbjq.cn/Article/details/gdqtzgxzh.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://baike.fehbvm.com/Article/details/gftwfzfao.sHtML

[Q28] 求和与平均
来源：http://www.share.fehbvm.com/Article/details/gtskexnep.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/ggukgofyk.sHtML

[Q29] 最大最小值
来源：http://wap.fehbvm.com/Article/details/gghozwyof.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://m.share.fehbvm.com/Article/details/ggkbzuxby.sHtML

[Q30] 分组统计
来源：http://www.blog.hesvh.cn/Article/details/gkpkgrrpn.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mobile.zdbjq.cn/Article/details/gsfbvijtp.sHtML

[Q31] 分组后过滤
来源：http://blog.hesvh.cn/Article/details/gnvomqaws.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://m.share.hesvh.cn/Article/details/gclncqazc.sHtML

[Q32] 分组拼接字符串
来源：http://blog.fehbvm.com/Article/details/goplnvzif.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wap.fehbvm.com/Article/details/gonnnjucq.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://3g.fehbvm.com/Article/details/gqnjqwygp.sHtML

[Q33] 多列分组
来源：http://www.share.fehbvm.com/Article/details/gehvckprp.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wap.zdbjq.cn/Article/details/gnmhktsae.sHtML

[Q34] 每组取第一条
来源：http://www.share.zdbjq.cn/Article/details/gwfshibrl.sHtML

SELECT * FROM (
来源：http://blog.fehbvm.com/Article/details/gylblsyxb.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.blog.hesvh.cn/Article/details/gjmdrlibh.sHtML

) t WHERE rn = 1;
来源：http://mobile.fehbvm.com/Article/details/gtzbwwrml.sHtML

[Q35] 内连接
来源：http://mobile.zdbjq.cn/Article/details/ghwzhhsou.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.fehbvm.com/Article/details/gktzpmbcr.sHtML

[Q36] 左连接
来源：http://www.blog.fehbvm.com/Article/details/gswcqonru.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mobile.fehbvm.com/Article/details/getxaaqfy.sHtML

[Q37] 右连接
来源：http://3g.hesvh.cn/Article/details/gqjqmxgob.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://m.share.hesvh.cn/Article/details/gwkcdpzzu.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.fehbvm.com/Article/details/ghdanwsfx.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.hesvh.cn/Article/details/grwvslvsd.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.zdbjq.cn/Article/details/gavddboex.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://read.share.fehbvm.com/Article/details/gumekwhlw.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://blog.hesvh.cn/Article/details/gqueipsjc.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://m.share.zdbjq.cn/Article/details/gimbqjmrn.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.hesvh.cn/Article/details/gsnukfutg.sHtML

[Q41] 多表连接
来源：http://www.m.share.hesvh.cn/Article/details/gtflatsqz.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.blog.hesvh.cn/Article/details/gsvmhadzs.sHtML

JOIN users u ON u.id = o.user_id
来源：http://wap.zdbjq.cn/Article/details/gmcghxagd.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.hesvh.cn/Article/details/glbkhsezu.sHtML

[Q42] 连接条件附加过滤
来源：http://mobile.fehbvm.com/Article/details/gkcinqzsi.sHtML

SELECT u.name, o.amount FROM users u
来源：http://3g.zdbjq.cn/Article/details/guybwbodm.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.fehbvm.com/Article/details/gymhxrqvv.sHtML

[Q43] 标量子查询
来源：http://www.m.share.fehbvm.com/Article/details/guznkrkrq.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.m.share.zdbjq.cn/Article/details/gnudqdkfk.sHtML

[Q44] IN 子查询
来源：http://mobile.zdbjq.cn/Article/details/gxelslagy.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.share.hesvh.cn/Article/details/gfoloctny.sHtML

[Q45] EXISTS 判断存在
来源：http://3g.fehbvm.com/Article/details/gqlgqodgn.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.zdbjq.cn/Article/details/gqhoefcjj.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.hesvh.cn/Article/details/gowdftczf.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.hesvh.cn/Article/details/ggdjycesi.sHtML

[Q47] 与平均值比较
来源：http://wap.fehbvm.com/Article/details/gbwxligsq.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.zdbjq.cn/Article/details/grgpvrmwa.sHtML

[Q48] CTE 公用表表达式
来源：http://3g.hesvh.cn/Article/details/gngxgpulh.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.zdbjq.cn/Article/details/gdtxidsmy.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.fehbvm.com/Article/details/goutmyrib.sHtML

[Q49] 更新单行
来源：http://wap.zdbjq.cn/Article/details/gtxlakgdl.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.blog.fehbvm.com/Article/details/gnwiibqxi.sHtML

[Q50] 批量更新
来源：http://read.share.zdbjq.cn/Article/details/gedjnsbum.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://blog.fehbvm.com/Article/details/gkqkmsdkm.sHtML

[Q51] 用子查询更新
来源：http://www.share.fehbvm.com/Article/details/gnqgzaslg.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.hesvh.cn/Article/details/gehneujos.sHtML

[Q52] 删除指定行
来源：http://www.share.zdbjq.cn/Article/details/gfenpkter.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.hesvh.cn/Article/details/gvexhikuv.sHtML

[Q53] 按条件删除
来源：http://3g.zdbjq.cn/Article/details/gqtfmkikf.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://m.share.hesvh.cn/Article/details/gchsycljf.sHtML

[Q54] 清空表
来源：http://www.m.share.fehbvm.com/Article/details/gzyoovxny.sHtML

TRUNCATE TABLE logs;
来源：http://mobile.zdbjq.cn/Article/details/gssxnztgd.sHtML

[Q55] 排名（并列占位）
来源：http://3g.hesvh.cn/Article/details/gmuqpyewn.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.share.hesvh.cn/Article/details/gxasxupty.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.zdbjq.cn/Article/details/gilffbyai.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.hesvh.cn/Article/details/gihtirpnj.sHtML

[Q57] 行号
来源：http://blog.hesvh.cn/Article/details/geqmdtrdj.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.fehbvm.com/Article/details/glorlcfkw.sHtML

[Q58] 累计求和
来源：http://baike.zdbjq.cn/Article/details/guvkniqlz.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.zdbjq.cn/Article/details/gvlabloif.sHtML

[Q59] 分组内累计
来源：http://read.share.hesvh.cn/Article/details/grsopzbra.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/gerrlwzai.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.fehbvm.com/Article/details/gqxbesaer.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.fehbvm.com/Article/details/gjdisbqab.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gcwmqcasm.sHtML

[Q61] 移动平均
来源：http://read.share.hesvh.cn/Article/details/gdjlbpito.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://3g.fehbvm.com/Article/details/gkkqcgezz.sHtML

[Q62] 分组占比
来源：http://www.share.zdbjq.cn/Article/details/goxttomkw.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.fehbvm.com/Article/details/gtkxngtne.sHtML

[Q63] 开启事务
来源：http://www.share.hesvh.cn/Article/details/gakhvxste.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://mobile.hesvh.cn/Article/details/gelgvgxus.sHtML

[Q64] 提交事务
来源：http://read.share.zdbjq.cn/Article/details/gzjfmzzrk.sHtML

COMMIT;
来源：http://wap.hesvh.cn/Article/details/gzkizqgnq.sHtML

[Q65] 回滚事务
来源：http://www.blog.hesvh.cn/Article/details/gkhhnxvlu.sHtML

ROLLBACK;
来源：http://read.share.zdbjq.cn/Article/details/gsxodwuwj.sHtML

[Q66] 行锁查询
来源：http://blog.hesvh.cn/Article/details/gttpwfpwp.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wap.fehbvm.com/Article/details/gjgiwcfia.sHtML

[Q67] 设置隔离级别
来源：http://3g.zdbjq.cn/Article/details/gqjxwvvto.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.fehbvm.com/Article/details/gzdcdzaea.sHtML

[Q68] 保存点
来源：http://3g.hesvh.cn/Article/details/gdakobous.sHtML

SAVEPOINT sp1;
来源：http://blog.fehbvm.com/Article/details/ggelnyiyv.sHtML

ROLLBACK TO sp1;
来源：http://www.share.fehbvm.com/Article/details/gyahdiyrk.sHtML

[Q69] 查看执行计划
来源：http://www.share.hesvh.cn/Article/details/gzhvginym.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://blog.fehbvm.com/Article/details/gyqupsrxh.sHtML

[Q70] 更新统计信息
来源：http://blog.hesvh.cn/Article/details/gtsnllrjz.sHtML

ANALYZE TABLE users;
来源：http://read.share.zdbjq.cn/Article/details/gyarsyusj.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.fehbvm.com/Article/details/gbuvioamf.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.zdbjq.cn/Article/details/gdjpwxaxn.sHtML

[Q72] 查看索引
来源：http://mobile.fehbvm.com/Article/details/ggdhnkwlr.sHtML

SHOW INDEX FROM users;
来源：http://blog.hesvh.cn/Article/details/ggtonnvqq.sHtML

[Q73] 查看表状态
来源：http://www.blog.hesvh.cn/Article/details/gpvsaylwv.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.hesvh.cn/Article/details/gbzpuxlmi.sHtML

[Q74] 强制使用索引
来源：http://blog.hesvh.cn/Article/details/gedpmzkhv.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.fehbvm.com/Article/details/ggfhefaox.sHtML

[Q75] 日期格式化
来源：http://www.m.share.fehbvm.com/Article/details/gcvmsuxjw.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.hesvh.cn/Article/details/geqrsawco.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.zdbjq.cn/Article/details/gxmxugmgw.sHtML

[Q76] 按天统计
来源：http://www.m.share.hesvh.cn/Article/details/gtsmgrsuy.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.zdbjq.cn/Article/details/gcadruuht.sHtML

[Q77] 时间加减
来源：http://read.share.hesvh.cn/Article/details/gkrgmpinb.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.hesvh.cn/Article/details/gplckwpnc.sHtML

[Q78] 当前时间
来源：http://www.m.share.fehbvm.com/Article/details/gtqeekxak.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.zdbjq.cn/Article/details/gwkufhjij.sHtML

[Q79] 字符串拼接
来源：http://www.share.fehbvm.com/Article/details/gvojeekhi.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.hesvh.cn/Article/details/gohxxmssa.sHtML

[Q80] 字符串截取
来源：http://baike.fehbvm.com/Article/details/gnunuclep.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.hesvh.cn/Article/details/glpxpjkrd.sHtML

[Q81] 字符串替换
来源：http://read.share.zdbjq.cn/Article/details/gmpkrjyrt.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.hesvh.cn/Article/details/gyjgciedr.sHtML


<!-- 参考信息 -->