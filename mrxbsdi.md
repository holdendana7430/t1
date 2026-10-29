代发 wailian999

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.m.share.fehbvm.com/Article/details/gxrjchzsn.sHtML

[O03] 加锁保护共享数据
来源：http://baike.hesvh.cn/Article/details/ghlicsjmd.sHtML

Py:   with lock: shared += 1
来源：http://wap.hesvh.cn/Article/details/gmmvwchhv.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://wap.zdbjq.cn/Article/details/gzkhwxqgx.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.m.share.hesvh.cn/Article/details/gfzdnblvi.sHtML

TS:   // 同 JS
来源：http://blog.hesvh.cn/Article/details/gykwvomzl.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.fehbvm.com/Article/details/glwoymxvj.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.hesvh.cn/Article/details/ggidupgou.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.blog.hesvh.cn/Article/details/glweynetz.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.fehbvm.com/Article/details/gdqeyldst.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.hesvh.cn/Article/details/gmniqwdxf.sHtML

Py:   async def f():⏎    await g()
来源：http://www.m.share.zdbjq.cn/Article/details/gnqppyhot.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://blog.hesvh.cn/Article/details/guhswdybd.sHtML

JS:   async function f() { await g(); }
来源：http://mobile.zdbjq.cn/Article/details/gheplpqdp.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.share.fehbvm.com/Article/details/glastnurd.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mobile.zdbjq.cn/Article/details/ghwsbrwoc.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://m.share.fehbvm.com/Article/details/gukrpytux.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://wap.fehbvm.com/Article/details/gmiwrcmxn.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.fehbvm.com/Article/details/gpbeqitkr.sHtML

[O05] 并发执行并等待全部完成
来源：http://mobile.zdbjq.cn/Article/details/gvsxykrit.sHtML

Py:   asyncio.gather(*tasks)
来源：http://read.share.fehbvm.com/Article/details/gzhrqwbpn.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://3g.hesvh.cn/Article/details/grtdfnral.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.zdbjq.cn/Article/details/gxedihbzy.sHtML

TS:   await Promise.all(tasks)
来源：http://mobile.hesvh.cn/Article/details/gjncngvat.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wap.fehbvm.com/Article/details/gsvjtflro.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://blog.hesvh.cn/Article/details/ggsqqdeyw.sHtML

Ruby: threads.map(&:join)
来源：http://read.share.hesvh.cn/Article/details/gornvzikn.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://3g.hesvh.cn/Article/details/gjukkcfrl.sHtML

[O06] 使用进程池
来源：http://www.m.share.zdbjq.cn/Article/details/gnvllzpun.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.share.hesvh.cn/Article/details/gvdjmsrtv.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.blog.zdbjq.cn/Article/details/gyvanxufz.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.hesvh.cn/Article/details/gwftfikxa.sHtML

TS:   // child_process / cluster 模块
来源：http://www.blog.zdbjq.cn/Article/details/gjvjolkbl.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://read.share.zdbjq.cn/Article/details/gawbqoacr.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mobile.zdbjq.cn/Article/details/gcfajmode.sHtML

Ruby: // fork 块
来源：http://baike.hesvh.cn/Article/details/gkzdxynbw.sHtML

C#:   Parallel.For
来源：http://baike.hesvh.cn/Article/details/glzdhcfdn.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/glezhsmgr.sHtML

P. 常用工具函数
来源：http://mobile.zdbjq.cn/Article/details/gjfaacblu.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gudclnnsy.sHtML

[P01] 生成 UUID
来源：http://read.share.fehbvm.com/Article/details/gxdajrtnu.sHtML

Py:   str(uuid.uuid4())
来源：http://3g.fehbvm.com/Article/details/gpyqpgfvr.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.m.share.fehbvm.com/Article/details/gprkgptiz.sHtML

JS:   crypto.randomUUID()
来源：http://blog.fehbvm.com/Article/details/gsanlqrma.sHtML

TS:   crypto.randomUUID()
来源：http://www.blog.zdbjq.cn/Article/details/glygirvpx.sHtML

Java: UUID.randomUUID().toString()
来源：http://wap.fehbvm.com/Article/details/ggozouhst.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.m.share.hesvh.cn/Article/details/gxbmscvrs.sHtML

Ruby: SecureRandom.uuid
来源：http://3g.fehbvm.com/Article/details/gzykodgid.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://read.share.zdbjq.cn/Article/details/gohbheyrw.sHtML

[P02] MD5 / SHA256 摘要
来源：http://mobile.fehbvm.com/Article/details/gbkjcpnqn.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://3g.hesvh.cn/Article/details/gomwhmnqm.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gcrcneuwf.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://blog.hesvh.cn/Article/details/gzfbbryby.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mobile.zdbjq.cn/Article/details/gjmfjkigo.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.m.share.zdbjq.cn/Article/details/ghlbytunc.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://read.share.fehbvm.com/Article/details/gampgyhjk.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://baike.zdbjq.cn/Article/details/gjjovnisz.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.share.zdbjq.cn/Article/details/gdyfhipzm.sHtML

[P03] 生成短随机字符串
来源：http://read.share.fehbvm.com/Article/details/gvnjejwur.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mobile.hesvh.cn/Article/details/gurulxsep.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://read.share.zdbjq.cn/Article/details/gxsmfaamp.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.hesvh.cn/Article/details/ghadhgdyn.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.zdbjq.cn/Article/details/godsgcrvi.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.zdbjq.cn/Article/details/ggegwfpug.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://3g.hesvh.cn/Article/details/gswfycvpm.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://m.share.zdbjq.cn/Article/details/gunchzlen.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://read.share.hesvh.cn/Article/details/gamoymiiu.sHtML

[P04] 求长度
来源：http://mobile.hesvh.cn/Article/details/gfjwqtisp.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.blog.fehbvm.com/Article/details/gmkafwzlm.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.zdbjq.cn/Article/details/giescpmmi.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.hesvh.cn/Article/details/gmuojspiy.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.zdbjq.cn/Article/details/gmmzbeoyt.sHtML

Java: list.size();  map.size();  s.length()
来源：http://read.share.zdbjq.cn/Article/details/gldktotrl.sHtML

Go:   len(arr);  len(m)
来源：http://baike.zdbjq.cn/Article/details/gnbwwbgrj.sHtML

Ruby: x.length;  x.size
来源：http://wap.fehbvm.com/Article/details/gvaevwsgm.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://baike.fehbvm.com/Article/details/gelvxmqac.sHtML

[P05] 判断两个对象内容是否相等
来源：http://3g.zdbjq.cn/Article/details/gevfrnfem.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://wap.fehbvm.com/Article/details/ghmxtrhgb.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://baike.zdbjq.cn/Article/details/giffonftc.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.share.hesvh.cn/Article/details/gpsvaonbj.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.zdbjq.cn/Article/details/gbgfkmuxq.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://read.share.zdbjq.cn/Article/details/gnexrcfzv.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://3g.zdbjq.cn/Article/details/giydtqecq.sHtML

Ruby: a == b
来源：http://m.share.hesvh.cn/Article/details/gzgozzkls.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.m.share.fehbvm.com/Article/details/glwtjqfsb.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://baike.fehbvm.com/Article/details/ghzbibeog.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.hesvh.cn/Article/details/gpduhvsqd.sHtML

PHP:  if (empty($x)) {}
来源：http://mobile.zdbjq.cn/Article/details/gahfsoanx.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://blog.hesvh.cn/Article/details/ggqwjlokn.sHtML

TS:   if (x == null) {}
来源：http://wap.zdbjq.cn/Article/details/gxphedrpb.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://read.share.fehbvm.com/Article/details/grasbbipo.sHtML

Go:   if x == nil {}
来源：http://www.blog.zdbjq.cn/Article/details/gujpvotlz.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.share.zdbjq.cn/Article/details/gqyzrmumr.sHtML

C#:   if (x is null) {}
来源：http://www.share.fehbvm.com/Article/details/gsiwxvnyk.sHtML

[P07] 防抖与节流
来源：http://www.m.share.fehbvm.com/Article/details/gtvlpplbe.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://read.share.fehbvm.com/Article/details/gpsdywldi.sHtML

PHP:  // 手写时间戳比较
来源：http://blog.fehbvm.com/Article/details/gqsxueamv.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.hesvh.cn/Article/details/grkcbvtaf.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.hesvh.cn/Article/details/glqyokmeh.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.blog.hesvh.cn/Article/details/gawfczihd.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://m.share.hesvh.cn/Article/details/gifsgntga.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://baike.fehbvm.com/Article/details/gbfnbjdgx.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.blog.zdbjq.cn/Article/details/genjabemt.sHtML

[P08] 处理浮点精度问题
来源：http://3g.hesvh.cn/Article/details/gikolhvuw.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.share.zdbjq.cn/Article/details/gifeyryjq.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mobile.hesvh.cn/Article/details/gvvrwnycb.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.share.zdbjq.cn/Article/details/gzufefzcr.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://baike.hesvh.cn/Article/details/gtknjqyhd.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.share.hesvh.cn/Article/details/gxkpwwdgg.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://3g.fehbvm.com/Article/details/gnhqvdjwv.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mobile.fehbvm.com/Article/details/goyhktvvx.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mobile.hesvh.cn/Article/details/ggecklnll.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/guitefxic.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://3g.hesvh.cn/Article/details/gvoyacojm.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gghsrabic.sHtML

[Q01] 创建表
来源：http://wap.zdbjq.cn/Article/details/gplmdoovg.sHtML

CREATE TABLE users (
来源：http://www.blog.zdbjq.cn/Article/details/gszdszsvu.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.zdbjq.cn/Article/details/grpfjfqov.sHtML

name VARCHAR(50) NOT NULL,
来源：http://wap.fehbvm.com/Article/details/gchfulwln.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.blog.zdbjq.cn/Article/details/gyfglmhen.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.share.zdbjq.cn/Article/details/gwqbpkyxw.sHtML

);
来源：http://3g.fehbvm.com/Article/details/gyjhicuan.sHtML

[Q02] 创建带外键的表
来源：http://www.m.share.zdbjq.cn/Article/details/grphssunv.sHtML

CREATE TABLE orders (
来源：http://read.share.hesvh.cn/Article/details/goqfjtzrd.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.zdbjq.cn/Article/details/gkxnakcga.sHtML

user_id INT NOT NULL,
来源：http://wap.hesvh.cn/Article/details/gtnftvolu.sHtML

amount DECIMAL(10, 2),
来源：http://blog.hesvh.cn/Article/details/gghyrgaaj.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://m.share.zdbjq.cn/Article/details/gzmfdwjwh.sHtML

);
来源：http://baike.hesvh.cn/Article/details/gdokepsjv.sHtML

[Q03] 增加列
来源：http://wap.fehbvm.com/Article/details/gjhawrkuy.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.blog.hesvh.cn/Article/details/gkmkjvfus.sHtML

[Q04] 修改列类型
来源：http://wap.hesvh.cn/Article/details/gfilsxoqg.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.m.share.fehbvm.com/Article/details/gsddmrscn.sHtML

[Q05] 重命名列
来源：http://wap.zdbjq.cn/Article/details/gfdfyxyke.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wap.zdbjq.cn/Article/details/gxckamhxh.sHtML

[Q06] 删除列
来源：http://read.share.zdbjq.cn/Article/details/gdsgpbfox.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://blog.zdbjq.cn/Article/details/gnonmavsk.sHtML

[Q07] 删除表
来源：http://wap.hesvh.cn/Article/details/gpplgtcnd.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.share.fehbvm.com/Article/details/gpixmlukq.sHtML

[Q08] 创建普通索引
来源：http://baike.zdbjq.cn/Article/details/gfbdbttvf.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://blog.fehbvm.com/Article/details/gujdhnaml.sHtML

[Q09] 创建唯一索引
来源：http://baike.zdbjq.cn/Article/details/grptevxpe.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.share.zdbjq.cn/Article/details/giknviriv.sHtML

[Q10] 插入单行
来源：http://3g.hesvh.cn/Article/details/glourukrs.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wap.fehbvm.com/Article/details/gpcdlgtod.sHtML

[Q11] 一次插入多行
来源：http://read.share.fehbvm.com/Article/details/gvowxglcp.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.share.fehbvm.com/Article/details/gvatqetrq.sHtML

[Q12] 插入后取自增 ID
来源：http://wap.hesvh.cn/Article/details/glavzahbc.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://mobile.zdbjq.cn/Article/details/gzprlitar.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.m.share.zdbjq.cn/Article/details/gavdayned.sHtML

[Q13] 忽略重复插入
来源：http://m.share.hesvh.cn/Article/details/gaazdeznt.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://m.share.fehbvm.com/Article/details/gupagbhqr.sHtML

[Q14] 存在则更新（upsert）
来源：http://3g.hesvh.cn/Article/details/gkstfmcdr.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.share.zdbjq.cn/Article/details/gelgajmsp.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.m.share.zdbjq.cn/Article/details/gxinpuxjz.sHtML

[Q15] 查询全部
来源：http://wap.zdbjq.cn/Article/details/gmuwfbzxf.sHtML

SELECT * FROM users;
来源：http://blog.hesvh.cn/Article/details/gifdtvzzx.sHtML

[Q16] 查询指定列
来源：http://wap.zdbjq.cn/Article/details/gzlrompzc.sHtML

SELECT id, name FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/ghiqjhmcj.sHtML

[Q17] 条件查询
来源：http://baike.fehbvm.com/Article/details/gbzstwbtk.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gkxjorzmy.sHtML

[Q18] 模糊匹配
来源：http://www.m.share.zdbjq.cn/Article/details/gtsqfkwgy.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://3g.zdbjq.cn/Article/details/gxmxrkirt.sHtML

[Q19] 范围查询
来源：http://www.share.fehbvm.com/Article/details/gmugjqose.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://m.share.hesvh.cn/Article/details/ghiwkvhxv.sHtML

[Q20] IN 列表
来源：http://www.m.share.fehbvm.com/Article/details/gkfgzymky.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://m.share.hesvh.cn/Article/details/gllpichaq.sHtML

[Q21] 空值判断
来源：http://www.share.zdbjq.cn/Article/details/gwlgjbkvg.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://baike.fehbvm.com/Article/details/ggyapkspx.sHtML

[Q22] 排序
来源：http://wap.fehbvm.com/Article/details/gvxkuvein.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://3g.fehbvm.com/Article/details/giaptwmdh.sHtML

[Q23] 分页
来源：http://blog.zdbjq.cn/Article/details/gtqugsfeq.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wap.fehbvm.com/Article/details/gjyvinjvi.sHtML

[Q24] 去重
来源：http://www.share.fehbvm.com/Article/details/godspycow.sHtML

SELECT DISTINCT city FROM users;
来源：http://wap.fehbvm.com/Article/details/gwhwlivck.sHtML

[Q25] 只取前 N 条
来源：http://www.blog.fehbvm.com/Article/details/gehiwynhy.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://m.share.fehbvm.com/Article/details/gtyovudrz.sHtML

[Q26] 计数
来源：http://mobile.hesvh.cn/Article/details/gqzdygumg.sHtML

SELECT COUNT(*) FROM users;
来源：http://mobile.hesvh.cn/Article/details/gzutwgqcv.sHtML

[Q27] 条件计数
来源：http://www.blog.hesvh.cn/Article/details/gdiumynim.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gmnpnfuez.sHtML

[Q28] 求和与平均
来源：http://m.share.hesvh.cn/Article/details/gqwbbaxzu.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wap.hesvh.cn/Article/details/gvodlxcxo.sHtML

[Q29] 最大最小值
来源：http://baike.hesvh.cn/Article/details/gohgjsfbp.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://wap.hesvh.cn/Article/details/grqlclvbg.sHtML

[Q30] 分组统计
来源：http://mobile.hesvh.cn/Article/details/genczkqza.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://baike.zdbjq.cn/Article/details/gzyxeysfd.sHtML

[Q31] 分组后过滤
来源：http://baike.hesvh.cn/Article/details/gbgxykgjp.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.zdbjq.cn/Article/details/gwcchqkqg.sHtML

[Q32] 分组拼接字符串
来源：http://mobile.fehbvm.com/Article/details/gmdkarwef.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://baike.hesvh.cn/Article/details/gptydcewg.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wap.hesvh.cn/Article/details/gjizqsopr.sHtML

[Q33] 多列分组
来源：http://baike.zdbjq.cn/Article/details/gudxqgirx.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.blog.zdbjq.cn/Article/details/gxikbqapm.sHtML

[Q34] 每组取第一条
来源：http://www.blog.fehbvm.com/Article/details/gmjrohdfh.sHtML

SELECT * FROM (
来源：http://3g.hesvh.cn/Article/details/gcvmgadrt.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.m.share.hesvh.cn/Article/details/gsajgybty.sHtML

) t WHERE rn = 1;
来源：http://3g.zdbjq.cn/Article/details/glnybnfud.sHtML

[Q35] 内连接
来源：http://mobile.hesvh.cn/Article/details/gpcyhmwxb.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://blog.zdbjq.cn/Article/details/gdnynfhcu.sHtML

[Q36] 左连接
来源：http://www.share.fehbvm.com/Article/details/gekchzcmy.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.fehbvm.com/Article/details/grfezskcj.sHtML

[Q37] 右连接
来源：http://m.share.fehbvm.com/Article/details/gdenzpkwq.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.hesvh.cn/Article/details/gyxlcmmfs.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://blog.fehbvm.com/Article/details/giehgnqny.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.zdbjq.cn/Article/details/gnptmkudz.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.zdbjq.cn/Article/details/gszzybhre.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.hesvh.cn/Article/details/gqtbshgim.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.fehbvm.com/Article/details/gvbqeyhas.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.fehbvm.com/Article/details/grsvnmblk.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.fehbvm.com/Article/details/gtujvdbvi.sHtML

[Q41] 多表连接
来源：http://www.blog.hesvh.cn/Article/details/grcgpibnb.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://m.share.hesvh.cn/Article/details/gkgmuwjhv.sHtML

JOIN users u ON u.id = o.user_id
来源：http://baike.fehbvm.com/Article/details/gwkqzkxyz.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://blog.zdbjq.cn/Article/details/gkbnynvai.sHtML

[Q42] 连接条件附加过滤
来源：http://wap.fehbvm.com/Article/details/gsqulqddf.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.zdbjq.cn/Article/details/gyzgdksby.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://read.share.hesvh.cn/Article/details/gphsudhhz.sHtML

[Q43] 标量子查询
来源：http://m.share.hesvh.cn/Article/details/gfbclllwr.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://read.share.fehbvm.com/Article/details/gcgnocsey.sHtML

[Q44] IN 子查询
来源：http://www.share.hesvh.cn/Article/details/gbntvkczm.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.hesvh.cn/Article/details/gokmweplj.sHtML

[Q45] EXISTS 判断存在
来源：http://read.share.hesvh.cn/Article/details/gxrojuxtt.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.hesvh.cn/Article/details/gxwmpuqbt.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://wap.zdbjq.cn/Article/details/gcldvjbzp.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.fehbvm.com/Article/details/ghyorwamh.sHtML

[Q47] 与平均值比较
来源：http://m.share.zdbjq.cn/Article/details/gauyeedgi.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mobile.fehbvm.com/Article/details/gdsfierch.sHtML

[Q48] CTE 公用表表达式
来源：http://3g.hesvh.cn/Article/details/gmovbhlhv.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://m.share.zdbjq.cn/Article/details/gjpmteveo.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.fehbvm.com/Article/details/gwvyfldah.sHtML

[Q49] 更新单行
来源：http://blog.hesvh.cn/Article/details/gzaweoeaf.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.fehbvm.com/Article/details/giphzrkgn.sHtML

[Q50] 批量更新
来源：http://read.share.zdbjq.cn/Article/details/ghzxloyvt.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.share.hesvh.cn/Article/details/gledgigat.sHtML

[Q51] 用子查询更新
来源：http://www.m.share.fehbvm.com/Article/details/gddverkjm.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gmeiygtsc.sHtML

[Q52] 删除指定行
来源：http://mobile.fehbvm.com/Article/details/gvkbsheqs.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.blog.hesvh.cn/Article/details/ghapgwoyl.sHtML

[Q53] 按条件删除
来源：http://mobile.zdbjq.cn/Article/details/gmyuaqqbq.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.share.zdbjq.cn/Article/details/ggnunciwa.sHtML

[Q54] 清空表
来源：http://www.share.hesvh.cn/Article/details/gzcomvkei.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.zdbjq.cn/Article/details/ggtniisae.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.zdbjq.cn/Article/details/glbwgzyqv.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.fehbvm.com/Article/details/gfxgbuewq.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.blog.zdbjq.cn/Article/details/gyyxuvkei.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.hesvh.cn/Article/details/gcoifkova.sHtML

[Q57] 行号
来源：http://read.share.hesvh.cn/Article/details/gpiradhws.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.hesvh.cn/Article/details/geeortjur.sHtML

[Q58] 累计求和
来源：http://read.share.fehbvm.com/Article/details/geksiwclm.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.hesvh.cn/Article/details/gfaxrsxti.sHtML

[Q59] 分组内累计
来源：http://m.share.fehbvm.com/Article/details/gjpyjjzuz.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://read.share.fehbvm.com/Article/details/gwjuucqjd.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.zdbjq.cn/Article/details/gytyluidv.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.hesvh.cn/Article/details/gdfswxfql.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.zdbjq.cn/Article/details/ghycplzsi.sHtML

[Q61] 移动平均
来源：http://mobile.hesvh.cn/Article/details/gqyxnbibt.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/gkydxugio.sHtML

[Q62] 分组占比
来源：http://baike.hesvh.cn/Article/details/gmwhpqksx.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.hesvh.cn/Article/details/gzyzbuifr.sHtML

[Q63] 开启事务
来源：http://read.share.fehbvm.com/Article/details/geatpdbus.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.hesvh.cn/Article/details/gocradmiy.sHtML

[Q64] 提交事务
来源：http://www.blog.hesvh.cn/Article/details/gbwaxcmia.sHtML

COMMIT;
来源：http://read.share.zdbjq.cn/Article/details/guommyvci.sHtML

[Q65] 回滚事务
来源：http://www.share.hesvh.cn/Article/details/giljemsyr.sHtML

ROLLBACK;
来源：http://blog.fehbvm.com/Article/details/gfttwotec.sHtML

[Q66] 行锁查询
来源：http://www.m.share.fehbvm.com/Article/details/gggknxmjs.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.zdbjq.cn/Article/details/giihkeeal.sHtML

[Q67] 设置隔离级别
来源：http://www.share.fehbvm.com/Article/details/gpgnnipiz.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.fehbvm.com/Article/details/gcfqqbvzn.sHtML

[Q68] 保存点
来源：http://www.share.zdbjq.cn/Article/details/gcjcapftb.sHtML

SAVEPOINT sp1;
来源：http://mobile.fehbvm.com/Article/details/gpodlmsvr.sHtML

ROLLBACK TO sp1;
来源：http://baike.fehbvm.com/Article/details/ghanjcqad.sHtML

[Q69] 查看执行计划
来源：http://www.share.hesvh.cn/Article/details/gpqrvheeb.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.fehbvm.com/Article/details/gbhtklhhv.sHtML

[Q70] 更新统计信息
来源：http://www.blog.zdbjq.cn/Article/details/ghzdkybbe.sHtML

ANALYZE TABLE users;
来源：http://baike.zdbjq.cn/Article/details/gjcwrehws.sHtML

[Q71] 查看建表语句
来源：http://wap.hesvh.cn/Article/details/gbcjewgpp.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.zdbjq.cn/Article/details/glgmwqmat.sHtML

[Q72] 查看索引
来源：http://www.blog.zdbjq.cn/Article/details/geliftpfs.sHtML

SHOW INDEX FROM users;
来源：http://baike.zdbjq.cn/Article/details/gvwdyupts.sHtML

[Q73] 查看表状态
来源：http://www.share.zdbjq.cn/Article/details/gwjlssnyb.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.hesvh.cn/Article/details/gnzraxmgl.sHtML

[Q74] 强制使用索引
来源：http://blog.hesvh.cn/Article/details/gfvqjqmln.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.zdbjq.cn/Article/details/gkiwmndrz.sHtML

[Q75] 日期格式化
来源：http://read.share.fehbvm.com/Article/details/gwqyzqnpr.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.zdbjq.cn/Article/details/ggdrblywk.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.fehbvm.com/Article/details/gicnjiasl.sHtML

[Q76] 按天统计
来源：http://baike.hesvh.cn/Article/details/giayjzxsy.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.zdbjq.cn/Article/details/ggpdtgzhx.sHtML

[Q77] 时间加减
来源：http://3g.hesvh.cn/Article/details/gimxcvmoz.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.fehbvm.com/Article/details/gqzrvwfkm.sHtML

[Q78] 当前时间
来源：http://blog.zdbjq.cn/Article/details/gasucbkhg.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.fehbvm.com/Article/details/gmsiwqrbr.sHtML

[Q79] 字符串拼接
来源：http://mobile.hesvh.cn/Article/details/gjpvxttgv.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.hesvh.cn/Article/details/gkjmppwls.sHtML

[Q80] 字符串截取
来源：http://wap.fehbvm.com/Article/details/gzohkexzy.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.hesvh.cn/Article/details/gbfafufcc.sHtML

[Q81] 字符串替换
来源：http://read.share.hesvh.cn/Article/details/gwrnwcvcb.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gdibtioir.sHtML


<!-- 参考信息 -->