代发 wailian999

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://m.share.fehbvm.com/Article/details/gytnpxvgh.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.zdbjq.cn/Article/details/gczxgxqek.sHtML

Py:   with lock: shared += 1
来源：http://www.share.hesvh.cn/Article/details/gcewgemel.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://mobile.fehbvm.com/Article/details/gbqbfhtqf.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://3g.fehbvm.com/Article/details/geemlisul.sHtML

TS:   // 同 JS
来源：http://3g.zdbjq.cn/Article/details/gdcjvplog.sHtML

Java: synchronized (this) { shared++; }
来源：http://m.share.hesvh.cn/Article/details/gxosmjzxc.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.fehbvm.com/Article/details/gpggtofxt.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.m.share.fehbvm.com/Article/details/gbnzfjdpm.sHtML

C#:   lock (gate) { shared++; }
来源：http://read.share.zdbjq.cn/Article/details/gkfbuqngb.sHtML

[O04] 定义异步函数并等待
来源：http://www.m.share.zdbjq.cn/Article/details/gmnrtuguc.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.zdbjq.cn/Article/details/gviemyklz.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.hesvh.cn/Article/details/ghioybqrr.sHtML

JS:   async function f() { await g(); }
来源：http://read.share.fehbvm.com/Article/details/gadwoccnv.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.m.share.fehbvm.com/Article/details/gtyswjrmb.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.blog.zdbjq.cn/Article/details/gdbbnhyth.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.m.share.zdbjq.cn/Article/details/gdfpqknru.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://blog.hesvh.cn/Article/details/gfkugoiki.sHtML

C#:   async Task F() { await G(); }
来源：http://wap.fehbvm.com/Article/details/gkmskdabx.sHtML

[O05] 并发执行并等待全部完成
来源：http://m.share.hesvh.cn/Article/details/gognxuaae.sHtML

Py:   asyncio.gather(*tasks)
来源：http://mobile.hesvh.cn/Article/details/gdiwlrjji.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.m.share.hesvh.cn/Article/details/gmxsfusvu.sHtML

JS:   await Promise.all(tasks)
来源：http://m.share.hesvh.cn/Article/details/gwvanaedm.sHtML

TS:   await Promise.all(tasks)
来源：http://read.share.hesvh.cn/Article/details/gpkbeappi.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.m.share.zdbjq.cn/Article/details/gpnpwbyrk.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mobile.zdbjq.cn/Article/details/gmedqxksx.sHtML

Ruby: threads.map(&:join)
来源：http://blog.zdbjq.cn/Article/details/glimxmthg.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://read.share.fehbvm.com/Article/details/gmtagskbm.sHtML

[O06] 使用进程池
来源：http://3g.hesvh.cn/Article/details/gqrsuqljg.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.share.fehbvm.com/Article/details/gbpsslnbg.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://mobile.fehbvm.com/Article/details/gtqhopwnv.sHtML

JS:   // child_process / cluster 模块
来源：http://www.m.share.fehbvm.com/Article/details/gindqbapp.sHtML

TS:   // child_process / cluster 模块
来源：http://baike.zdbjq.cn/Article/details/gqqoiqtli.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mobile.zdbjq.cn/Article/details/gzmcnqakj.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://baike.hesvh.cn/Article/details/glummdbgn.sHtML

Ruby: // fork 块
来源：http://3g.zdbjq.cn/Article/details/giklwgjqv.sHtML

C#:   Parallel.For
来源：http://mobile.hesvh.cn/Article/details/guesaevtd.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gkvfxotdo.sHtML

P. 常用工具函数
来源：http://www.m.share.zdbjq.cn/Article/details/gyeisfvrl.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gbetsixnp.sHtML

[P01] 生成 UUID
来源：http://baike.zdbjq.cn/Article/details/gaphktmie.sHtML

Py:   str(uuid.uuid4())
来源：http://m.share.fehbvm.com/Article/details/gdrrgcosm.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mobile.hesvh.cn/Article/details/gxrwtyvas.sHtML

JS:   crypto.randomUUID()
来源：http://mobile.zdbjq.cn/Article/details/gekfvakxm.sHtML

TS:   crypto.randomUUID()
来源：http://www.share.zdbjq.cn/Article/details/gsapeksee.sHtML

Java: UUID.randomUUID().toString()
来源：http://read.share.zdbjq.cn/Article/details/gpyuklcii.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.blog.hesvh.cn/Article/details/gthdprmwo.sHtML

Ruby: SecureRandom.uuid
来源：http://wap.fehbvm.com/Article/details/gnfrlijjc.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.m.share.fehbvm.com/Article/details/gpubttdkw.sHtML

[P02] MD5 / SHA256 摘要
来源：http://blog.hesvh.cn/Article/details/gmnzarxsn.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://read.share.zdbjq.cn/Article/details/gixfrsrxy.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://wap.zdbjq.cn/Article/details/gztextdhp.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://3g.zdbjq.cn/Article/details/gqspwjevp.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mobile.fehbvm.com/Article/details/gdpmtamzw.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wap.hesvh.cn/Article/details/ggmbjgipl.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://m.share.zdbjq.cn/Article/details/giwipldxy.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.share.zdbjq.cn/Article/details/gwuhtddam.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wap.zdbjq.cn/Article/details/gndttcofj.sHtML

[P03] 生成短随机字符串
来源：http://m.share.zdbjq.cn/Article/details/gbqjasyiu.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.share.zdbjq.cn/Article/details/gucvdhlqj.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mobile.hesvh.cn/Article/details/gjastrgcx.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.zdbjq.cn/Article/details/gslevvlvv.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.zdbjq.cn/Article/details/gfrniurjc.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.m.share.fehbvm.com/Article/details/gnkwofiei.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.m.share.zdbjq.cn/Article/details/grpozwgcp.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://wap.zdbjq.cn/Article/details/ghmtvwvls.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://3g.zdbjq.cn/Article/details/gxumptzlf.sHtML

[P04] 求长度
来源：http://wap.zdbjq.cn/Article/details/gwduiqvwo.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.m.share.fehbvm.com/Article/details/gewyxishy.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.zdbjq.cn/Article/details/gcsqsqele.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.zdbjq.cn/Article/details/gznwslish.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.hesvh.cn/Article/details/gypskxgzc.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.blog.zdbjq.cn/Article/details/gveumrzkd.sHtML

Go:   len(arr);  len(m)
来源：http://blog.hesvh.cn/Article/details/gynndqjqq.sHtML

Ruby: x.length;  x.size
来源：http://wap.zdbjq.cn/Article/details/gvsqruwpr.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.m.share.zdbjq.cn/Article/details/ggumjmqvu.sHtML

[P05] 判断两个对象内容是否相等
来源：http://wap.fehbvm.com/Article/details/gvfuzdszt.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://mobile.zdbjq.cn/Article/details/gjjphtcmt.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wap.hesvh.cn/Article/details/giuzgzapq.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://blog.fehbvm.com/Article/details/gdeqczhff.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.fehbvm.com/Article/details/gtiwpdphb.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wap.zdbjq.cn/Article/details/ghmydyexd.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.m.share.fehbvm.com/Article/details/gcwxpnrhs.sHtML

Ruby: a == b
来源：http://blog.fehbvm.com/Article/details/gmahlzkyt.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://read.share.zdbjq.cn/Article/details/gzfygufsl.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://baike.fehbvm.com/Article/details/grbbvnfrj.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://3g.hesvh.cn/Article/details/gppsyyjwm.sHtML

PHP:  if (empty($x)) {}
来源：http://mobile.zdbjq.cn/Article/details/gvuxyfzor.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mobile.zdbjq.cn/Article/details/gbdjmreuq.sHtML

TS:   if (x == null) {}
来源：http://blog.hesvh.cn/Article/details/gnjhxqqgi.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://mobile.zdbjq.cn/Article/details/ggqifmswo.sHtML

Go:   if x == nil {}
来源：http://mobile.hesvh.cn/Article/details/glvuldrwv.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.share.fehbvm.com/Article/details/gxxktxkgg.sHtML

C#:   if (x is null) {}
来源：http://www.share.fehbvm.com/Article/details/guxbwnkht.sHtML

[P07] 防抖与节流
来源：http://www.m.share.hesvh.cn/Article/details/gqbgbnkls.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://m.share.fehbvm.com/Article/details/gazogxgtd.sHtML

PHP:  // 手写时间戳比较
来源：http://www.blog.zdbjq.cn/Article/details/gxzvphtgd.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.zdbjq.cn/Article/details/ghblxmncp.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.hesvh.cn/Article/details/glryonkhf.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.blog.fehbvm.com/Article/details/guqryoepw.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://m.share.fehbvm.com/Article/details/gahvszvxl.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://mobile.fehbvm.com/Article/details/gdzthafay.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://baike.fehbvm.com/Article/details/gyrglvkrd.sHtML

[P08] 处理浮点精度问题
来源：http://read.share.zdbjq.cn/Article/details/gwpcawbiq.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mobile.hesvh.cn/Article/details/gmwjgvmvk.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://m.share.fehbvm.com/Article/details/gcecxvoay.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.zdbjq.cn/Article/details/gzswuonnv.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://blog.zdbjq.cn/Article/details/gmbqqnmuy.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://read.share.fehbvm.com/Article/details/gbxosexbm.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://read.share.hesvh.cn/Article/details/gqxnhxagg.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mobile.zdbjq.cn/Article/details/gtnaxlhky.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wap.zdbjq.cn/Article/details/ghsecmvnj.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gzwdrxwxm.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.m.share.zdbjq.cn/Article/details/gciusuokt.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gngiqkmap.sHtML

[Q01] 创建表
来源：http://www.blog.zdbjq.cn/Article/details/gcblbftmq.sHtML

CREATE TABLE users (
来源：http://blog.zdbjq.cn/Article/details/gipvcysrg.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.fehbvm.com/Article/details/gnokaxwyu.sHtML

name VARCHAR(50) NOT NULL,
来源：http://m.share.hesvh.cn/Article/details/gihhentcz.sHtML

email VARCHAR(100) UNIQUE,
来源：http://read.share.zdbjq.cn/Article/details/gvloiiojj.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://read.share.zdbjq.cn/Article/details/gvkrkrnjo.sHtML

);
来源：http://www.blog.hesvh.cn/Article/details/gnwduegtx.sHtML

[Q02] 创建带外键的表
来源：http://wap.fehbvm.com/Article/details/gwxrfaadd.sHtML

CREATE TABLE orders (
来源：http://www.share.zdbjq.cn/Article/details/gyqfcjefo.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.zdbjq.cn/Article/details/gfznwmfzz.sHtML

user_id INT NOT NULL,
来源：http://m.share.fehbvm.com/Article/details/gcevclunz.sHtML

amount DECIMAL(10, 2),
来源：http://baike.fehbvm.com/Article/details/gsnebuysn.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.share.zdbjq.cn/Article/details/gbqiycvsm.sHtML

);
来源：http://blog.hesvh.cn/Article/details/gffpkdyjh.sHtML

[Q03] 增加列
来源：http://www.m.share.fehbvm.com/Article/details/ghfvzupcp.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://baike.fehbvm.com/Article/details/gtckaruke.sHtML

[Q04] 修改列类型
来源：http://baike.hesvh.cn/Article/details/gqqtbxezs.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://baike.zdbjq.cn/Article/details/gomhjyvzs.sHtML

[Q05] 重命名列
来源：http://baike.zdbjq.cn/Article/details/gldridgsm.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mobile.zdbjq.cn/Article/details/gwxbxcvqh.sHtML

[Q06] 删除列
来源：http://m.share.fehbvm.com/Article/details/gxxujrgcn.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://blog.zdbjq.cn/Article/details/gmbztxdiq.sHtML

[Q07] 删除表
来源：http://mobile.hesvh.cn/Article/details/guciwspin.sHtML

DROP TABLE IF EXISTS orders;
来源：http://blog.zdbjq.cn/Article/details/gplnrkwdo.sHtML

[Q08] 创建普通索引
来源：http://www.share.hesvh.cn/Article/details/gbhbsibwy.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.share.hesvh.cn/Article/details/gwmtemzjx.sHtML

[Q09] 创建唯一索引
来源：http://m.share.fehbvm.com/Article/details/guavgkxti.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.m.share.fehbvm.com/Article/details/gxvgbwcaw.sHtML

[Q10] 插入单行
来源：http://read.share.zdbjq.cn/Article/details/gxxoypspw.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://3g.hesvh.cn/Article/details/gltpmfqwg.sHtML

[Q11] 一次插入多行
来源：http://read.share.hesvh.cn/Article/details/gqeahzswa.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.share.zdbjq.cn/Article/details/gwtyhxxpw.sHtML

[Q12] 插入后取自增 ID
来源：http://read.share.zdbjq.cn/Article/details/gdzxjqxdk.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://blog.fehbvm.com/Article/details/gvrdaecpn.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.m.share.zdbjq.cn/Article/details/gifhrdihx.sHtML

[Q13] 忽略重复插入
来源：http://baike.zdbjq.cn/Article/details/ggkvzqcus.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://baike.zdbjq.cn/Article/details/gjupufngp.sHtML

[Q14] 存在则更新（upsert）
来源：http://mobile.fehbvm.com/Article/details/grjqjhgne.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.share.hesvh.cn/Article/details/gnjvjzcyz.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.blog.hesvh.cn/Article/details/glhjlcpta.sHtML

[Q15] 查询全部
来源：http://m.share.zdbjq.cn/Article/details/gfwbkibgb.sHtML

SELECT * FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gkpeuhzry.sHtML

[Q16] 查询指定列
来源：http://3g.zdbjq.cn/Article/details/gqtsaggkw.sHtML

SELECT id, name FROM users;
来源：http://read.share.fehbvm.com/Article/details/gbwdrhxmo.sHtML

[Q17] 条件查询
来源：http://m.share.fehbvm.com/Article/details/gciijuogv.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.zdbjq.cn/Article/details/gwikblhtp.sHtML

[Q18] 模糊匹配
来源：http://read.share.zdbjq.cn/Article/details/gjwofxweo.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.hesvh.cn/Article/details/gdcisbmih.sHtML

[Q19] 范围查询
来源：http://mobile.fehbvm.com/Article/details/gzlvelhhf.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.share.fehbvm.com/Article/details/gtmhsfiud.sHtML

[Q20] IN 列表
来源：http://blog.hesvh.cn/Article/details/ghgmyxxek.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.share.hesvh.cn/Article/details/gdrsvbnlx.sHtML

[Q21] 空值判断
来源：http://www.m.share.zdbjq.cn/Article/details/gwfyjgbrf.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.blog.zdbjq.cn/Article/details/genkomysi.sHtML

[Q22] 排序
来源：http://read.share.hesvh.cn/Article/details/gtphmbqpe.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://baike.hesvh.cn/Article/details/gcidyofja.sHtML

[Q23] 分页
来源：http://www.m.share.fehbvm.com/Article/details/gttshqmrb.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wap.zdbjq.cn/Article/details/gxonfoddb.sHtML

[Q24] 去重
来源：http://read.share.hesvh.cn/Article/details/gdmtcatux.sHtML

SELECT DISTINCT city FROM users;
来源：http://baike.zdbjq.cn/Article/details/gwzyznawo.sHtML

[Q25] 只取前 N 条
来源：http://blog.zdbjq.cn/Article/details/greunuueg.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://blog.hesvh.cn/Article/details/grlblmjlg.sHtML

[Q26] 计数
来源：http://m.share.fehbvm.com/Article/details/gstdlpkwx.sHtML

SELECT COUNT(*) FROM users;
来源：http://3g.fehbvm.com/Article/details/gkghphyly.sHtML

[Q27] 条件计数
来源：http://m.share.hesvh.cn/Article/details/glhirztmp.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://read.share.fehbvm.com/Article/details/gabucevzz.sHtML

[Q28] 求和与平均
来源：http://mobile.fehbvm.com/Article/details/gwzqdwhdk.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gksnmustg.sHtML

[Q29] 最大最小值
来源：http://wap.zdbjq.cn/Article/details/gmwlagprb.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gjlubikde.sHtML

[Q30] 分组统计
来源：http://mobile.zdbjq.cn/Article/details/gowbrsvyt.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://blog.zdbjq.cn/Article/details/gjvbkoize.sHtML

[Q31] 分组后过滤
来源：http://3g.zdbjq.cn/Article/details/gyfhcsclq.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://read.share.zdbjq.cn/Article/details/gnyfqfnhk.sHtML

[Q32] 分组拼接字符串
来源：http://mobile.hesvh.cn/Article/details/gkbgkwrip.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.m.share.zdbjq.cn/Article/details/guqxwlfhf.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.hesvh.cn/Article/details/gmjhujozn.sHtML

[Q33] 多列分组
来源：http://m.share.hesvh.cn/Article/details/gtxtkafnk.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mobile.hesvh.cn/Article/details/grshdvrec.sHtML

[Q34] 每组取第一条
来源：http://wap.fehbvm.com/Article/details/gqqpdxoot.sHtML

SELECT * FROM (
来源：http://m.share.hesvh.cn/Article/details/gxaomiihr.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.zdbjq.cn/Article/details/gwrevjutz.sHtML

) t WHERE rn = 1;
来源：http://3g.zdbjq.cn/Article/details/gpiljrxah.sHtML

[Q35] 内连接
来源：http://www.share.fehbvm.com/Article/details/gymojtsjp.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.fehbvm.com/Article/details/gbmaqvabl.sHtML

[Q36] 左连接
来源：http://baike.zdbjq.cn/Article/details/gtyihthwl.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://baike.zdbjq.cn/Article/details/gbudhlxwi.sHtML

[Q37] 右连接
来源：http://www.blog.fehbvm.com/Article/details/gkfrsfbqd.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.share.hesvh.cn/Article/details/gyghmdplb.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.fehbvm.com/Article/details/gsnewcmnx.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.fehbvm.com/Article/details/glpyvwjmv.sHtML

[Q39] 自连接（查上下级）
来源：http://baike.zdbjq.cn/Article/details/gzztawbxu.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://wap.hesvh.cn/Article/details/ghzkbqvlz.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.zdbjq.cn/Article/details/gszibslpc.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.fehbvm.com/Article/details/gzciyuvjn.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.share.hesvh.cn/Article/details/gbrdjgdfd.sHtML

[Q41] 多表连接
来源：http://baike.zdbjq.cn/Article/details/gtyfrofhi.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.hesvh.cn/Article/details/gbagymgdb.sHtML

JOIN users u ON u.id = o.user_id
来源：http://blog.hesvh.cn/Article/details/gddmztaix.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.fehbvm.com/Article/details/gmqpjcmdc.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.zdbjq.cn/Article/details/ggfhjhkyx.sHtML

SELECT u.name, o.amount FROM users u
来源：http://wap.hesvh.cn/Article/details/gutooruto.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.m.share.hesvh.cn/Article/details/gvtqwrtrx.sHtML

[Q43] 标量子查询
来源：http://www.share.fehbvm.com/Article/details/gegbhnlpz.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.zdbjq.cn/Article/details/gpgrygior.sHtML

[Q44] IN 子查询
来源：http://blog.fehbvm.com/Article/details/giefufbbu.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://read.share.zdbjq.cn/Article/details/gtepanmwn.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.fehbvm.com/Article/details/guqshqbfq.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.hesvh.cn/Article/details/gayrvmkuh.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.fehbvm.com/Article/details/gyoagjcvo.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.hesvh.cn/Article/details/gqbmnsvwd.sHtML

[Q47] 与平均值比较
来源：http://3g.fehbvm.com/Article/details/gtuezgkza.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.zdbjq.cn/Article/details/gkhnhuskh.sHtML

[Q48] CTE 公用表表达式
来源：http://m.share.zdbjq.cn/Article/details/gsjmcyrbg.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://baike.fehbvm.com/Article/details/gpsbnxlzt.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://mobile.hesvh.cn/Article/details/ggjmvahfr.sHtML

[Q49] 更新单行
来源：http://read.share.zdbjq.cn/Article/details/gdrlkvdhv.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.fehbvm.com/Article/details/gqcfssyui.sHtML

[Q50] 批量更新
来源：http://read.share.fehbvm.com/Article/details/gthullgkg.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://m.share.hesvh.cn/Article/details/gewlriphg.sHtML

[Q51] 用子查询更新
来源：http://mobile.zdbjq.cn/Article/details/gvkalpgnn.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blog.fehbvm.com/Article/details/gcpweaitj.sHtML

[Q52] 删除指定行
来源：http://3g.hesvh.cn/Article/details/gmnvlucui.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.hesvh.cn/Article/details/gxdefasez.sHtML

[Q53] 按条件删除
来源：http://www.share.fehbvm.com/Article/details/gzmfchehr.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.hesvh.cn/Article/details/gfgzeypnd.sHtML

[Q54] 清空表
来源：http://www.m.share.fehbvm.com/Article/details/gobrcmjhl.sHtML

TRUNCATE TABLE logs;
来源：http://m.share.hesvh.cn/Article/details/gseuxxvzf.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.fehbvm.com/Article/details/gmzxoioxf.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.fehbvm.com/Article/details/giffpylyg.sHtML

[Q56] 密集排名（并列不占位）
来源：http://blog.fehbvm.com/Article/details/gjrriebnt.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.zdbjq.cn/Article/details/gxzbefyef.sHtML

[Q57] 行号
来源：http://3g.zdbjq.cn/Article/details/gzwsplqrc.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://blog.fehbvm.com/Article/details/glaadeusp.sHtML

[Q58] 累计求和
来源：http://wap.zdbjq.cn/Article/details/gvjspdsqa.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/gzmwtvxlo.sHtML

[Q59] 分组内累计
来源：http://www.blog.hesvh.cn/Article/details/ggnyrtwpt.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://3g.zdbjq.cn/Article/details/gedhsyarx.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.fehbvm.com/Article/details/gicwcnldu.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.zdbjq.cn/Article/details/goivxdvom.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://blog.hesvh.cn/Article/details/gsjdexpeo.sHtML

[Q61] 移动平均
来源：http://www.blog.fehbvm.com/Article/details/gyiiqdzun.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gqxrgrgkq.sHtML

[Q62] 分组占比
来源：http://baike.zdbjq.cn/Article/details/gctkgugli.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.hesvh.cn/Article/details/gmjvjgapn.sHtML

[Q63] 开启事务
来源：http://m.share.fehbvm.com/Article/details/giknmxkfz.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://wap.hesvh.cn/Article/details/gcmkzjtqp.sHtML

[Q64] 提交事务
来源：http://www.m.share.zdbjq.cn/Article/details/guwrpwhbw.sHtML

COMMIT;
来源：http://baike.fehbvm.com/Article/details/gelvotvrx.sHtML

[Q65] 回滚事务
来源：http://www.share.hesvh.cn/Article/details/gwszljmcw.sHtML

ROLLBACK;
来源：http://wap.fehbvm.com/Article/details/gyxqtuoqm.sHtML

[Q66] 行锁查询
来源：http://m.share.fehbvm.com/Article/details/gunmeqjjx.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.fehbvm.com/Article/details/gvtxczdoq.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.hesvh.cn/Article/details/gjsyojtim.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.fehbvm.com/Article/details/gculrunuh.sHtML

[Q68] 保存点
来源：http://www.share.fehbvm.com/Article/details/gamojpwwj.sHtML

SAVEPOINT sp1;
来源：http://blog.zdbjq.cn/Article/details/gqurptnvg.sHtML

ROLLBACK TO sp1;
来源：http://www.share.zdbjq.cn/Article/details/gorcbmoni.sHtML

[Q69] 查看执行计划
来源：http://wap.hesvh.cn/Article/details/gamighgty.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.zdbjq.cn/Article/details/gkcynnjvh.sHtML

[Q70] 更新统计信息
来源：http://read.share.hesvh.cn/Article/details/gscbqprma.sHtML

ANALYZE TABLE users;
来源：http://blog.hesvh.cn/Article/details/ginbsinox.sHtML

[Q71] 查看建表语句
来源：http://blog.hesvh.cn/Article/details/giivczrrj.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.fehbvm.com/Article/details/gbbptaixz.sHtML

[Q72] 查看索引
来源：http://wap.zdbjq.cn/Article/details/gstwgcedo.sHtML

SHOW INDEX FROM users;
来源：http://m.share.fehbvm.com/Article/details/gejdxcpkg.sHtML

[Q73] 查看表状态
来源：http://wap.zdbjq.cn/Article/details/grpqrswgm.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.hesvh.cn/Article/details/gxyeffbrk.sHtML

[Q74] 强制使用索引
来源：http://baike.hesvh.cn/Article/details/ghmpsouqi.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://baike.zdbjq.cn/Article/details/ggrodxgcc.sHtML

[Q75] 日期格式化
来源：http://www.blog.hesvh.cn/Article/details/gxxaexfvm.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.zdbjq.cn/Article/details/gykoufszg.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.zdbjq.cn/Article/details/gjdnlicyv.sHtML

[Q76] 按天统计
来源：http://www.m.share.zdbjq.cn/Article/details/gghdknfzn.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.fehbvm.com/Article/details/gfqcpdciz.sHtML

[Q77] 时间加减
来源：http://m.share.hesvh.cn/Article/details/gudetrgls.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.hesvh.cn/Article/details/gomslojpn.sHtML

[Q78] 当前时间
来源：http://www.m.share.hesvh.cn/Article/details/gdlpurycs.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.hesvh.cn/Article/details/gpxmkiuwu.sHtML

[Q79] 字符串拼接
来源：http://wap.fehbvm.com/Article/details/gleaftpmk.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.hesvh.cn/Article/details/gftkcndjf.sHtML

[Q80] 字符串截取
来源：http://www.share.hesvh.cn/Article/details/gmxwfoaga.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.zdbjq.cn/Article/details/gmgczfgue.sHtML

[Q81] 字符串替换
来源：http://wap.fehbvm.com/Article/details/gqmazqixu.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gnfdvkuir.sHtML


<!-- 参考信息 -->