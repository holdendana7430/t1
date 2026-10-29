代发 wailian999

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://blog.zdbjq.cn/Article/details/guznvugcz.sHtML

[O03] 加锁保护共享数据
来源：http://mobile.zdbjq.cn/Article/details/grmvuqpfb.sHtML

Py:   with lock: shared += 1
来源：http://mobile.zdbjq.cn/Article/details/gzpyqfdzc.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.share.zdbjq.cn/Article/details/ghkxeanoz.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.m.share.hesvh.cn/Article/details/gygcsjlhn.sHtML

TS:   // 同 JS
来源：http://blog.fehbvm.com/Article/details/gnbopcjpc.sHtML

Java: synchronized (this) { shared++; }
来源：http://read.share.hesvh.cn/Article/details/gluurykqd.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.share.zdbjq.cn/Article/details/gtgukqnge.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://blog.fehbvm.com/Article/details/gvdzxxzbw.sHtML

C#:   lock (gate) { shared++; }
来源：http://3g.hesvh.cn/Article/details/gwfbccssx.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.zdbjq.cn/Article/details/gervhqqyo.sHtML

Py:   async def f():⏎    await g()
来源：http://www.share.hesvh.cn/Article/details/gsalhkfnx.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://blog.hesvh.cn/Article/details/goiubpvxu.sHtML

JS:   async function f() { await g(); }
来源：http://www.share.zdbjq.cn/Article/details/gfasyjsdo.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://3g.fehbvm.com/Article/details/gccvicisb.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.share.fehbvm.com/Article/details/gslxhkvyi.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://3g.fehbvm.com/Article/details/grhvkqjpf.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://read.share.fehbvm.com/Article/details/gibgaamtp.sHtML

C#:   async Task F() { await G(); }
来源：http://read.share.zdbjq.cn/Article/details/gkaackdsy.sHtML

[O05] 并发执行并等待全部完成
来源：http://baike.hesvh.cn/Article/details/gavqaujmk.sHtML

Py:   asyncio.gather(*tasks)
来源：http://read.share.zdbjq.cn/Article/details/glnplgftj.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wap.hesvh.cn/Article/details/gumguotao.sHtML

JS:   await Promise.all(tasks)
来源：http://wap.zdbjq.cn/Article/details/giqveowff.sHtML

TS:   await Promise.all(tasks)
来源：http://baike.zdbjq.cn/Article/details/goymyrfzh.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mobile.zdbjq.cn/Article/details/gzhceeren.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wap.hesvh.cn/Article/details/gguoukqvq.sHtML

Ruby: threads.map(&:join)
来源：http://www.m.share.hesvh.cn/Article/details/gpitdvmpt.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://m.share.hesvh.cn/Article/details/gpooltomq.sHtML

[O06] 使用进程池
来源：http://www.m.share.hesvh.cn/Article/details/gzecnuyts.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://m.share.fehbvm.com/Article/details/gxzlyktmw.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://read.share.zdbjq.cn/Article/details/glcxsuvcj.sHtML

JS:   // child_process / cluster 模块
来源：http://3g.fehbvm.com/Article/details/gbvcchsvy.sHtML

TS:   // child_process / cluster 模块
来源：http://www.m.share.fehbvm.com/Article/details/glcpbwqnq.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.zdbjq.cn/Article/details/gvzcjainn.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.share.zdbjq.cn/Article/details/gvrjjoxjo.sHtML

Ruby: // fork 块
来源：http://blog.fehbvm.com/Article/details/gvqargsfr.sHtML

C#:   Parallel.For
来源：http://3g.fehbvm.com/Article/details/ggaxyvxdl.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gxrywyqfs.sHtML

P. 常用工具函数
来源：http://m.share.hesvh.cn/Article/details/grhrihhyq.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gyxgmtivz.sHtML

[P01] 生成 UUID
来源：http://m.share.fehbvm.com/Article/details/gpetfdyjg.sHtML

Py:   str(uuid.uuid4())
来源：http://read.share.zdbjq.cn/Article/details/giiyhsfiu.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://baike.fehbvm.com/Article/details/gkprslwxs.sHtML

JS:   crypto.randomUUID()
来源：http://www.blog.hesvh.cn/Article/details/graezrgtt.sHtML

TS:   crypto.randomUUID()
来源：http://wap.fehbvm.com/Article/details/gsdwqwrqm.sHtML

Java: UUID.randomUUID().toString()
来源：http://3g.hesvh.cn/Article/details/gbemyzpci.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.hesvh.cn/Article/details/gfuyuxppa.sHtML

Ruby: SecureRandom.uuid
来源：http://mobile.hesvh.cn/Article/details/gfvnukcuu.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.blog.zdbjq.cn/Article/details/gweyvdvqc.sHtML

[P02] MD5 / SHA256 摘要
来源：http://wap.fehbvm.com/Article/details/gpceqlltg.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.blog.hesvh.cn/Article/details/gkfgrckhn.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.share.zdbjq.cn/Article/details/gnfwpjwjx.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://read.share.fehbvm.com/Article/details/godiwqpyi.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.fehbvm.com/Article/details/giofggyxk.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://3g.zdbjq.cn/Article/details/gpprfckcs.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.share.hesvh.cn/Article/details/gjeuljyze.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://3g.zdbjq.cn/Article/details/gyasnespy.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.share.fehbvm.com/Article/details/gfkncfwgt.sHtML

[P03] 生成短随机字符串
来源：http://www.m.share.zdbjq.cn/Article/details/golekeisk.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://m.share.zdbjq.cn/Article/details/gyhaetnkf.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.blog.zdbjq.cn/Article/details/gzmuryqoz.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.fehbvm.com/Article/details/guzxxytbf.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.fehbvm.com/Article/details/giwfokkuu.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://blog.zdbjq.cn/Article/details/gnikiullp.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mobile.hesvh.cn/Article/details/gvqvllzpe.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://blog.fehbvm.com/Article/details/gphzllqvb.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://m.share.fehbvm.com/Article/details/gtybnddnd.sHtML

[P04] 求长度
来源：http://3g.fehbvm.com/Article/details/gbzpxwjdz.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.m.share.zdbjq.cn/Article/details/guhmcahcv.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.hesvh.cn/Article/details/goiakojut.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.zdbjq.cn/Article/details/gzgevackj.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.zdbjq.cn/Article/details/gtvcxlbta.sHtML

Java: list.size();  map.size();  s.length()
来源：http://baike.zdbjq.cn/Article/details/glkvuhnhp.sHtML

Go:   len(arr);  len(m)
来源：http://baike.hesvh.cn/Article/details/gjzkujnyi.sHtML

Ruby: x.length;  x.size
来源：http://www.m.share.zdbjq.cn/Article/details/gtbbxkffb.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://read.share.hesvh.cn/Article/details/gwoflzxtr.sHtML

[P05] 判断两个对象内容是否相等
来源：http://mobile.fehbvm.com/Article/details/gayhggwgj.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://blog.hesvh.cn/Article/details/gchwflccn.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wap.hesvh.cn/Article/details/gspjzidqo.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.share.hesvh.cn/Article/details/gjnrfkmdx.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.fehbvm.com/Article/details/gzwimyohy.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://3g.zdbjq.cn/Article/details/gaupugtof.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.m.share.hesvh.cn/Article/details/gboruwuim.sHtML

Ruby: a == b
来源：http://wap.hesvh.cn/Article/details/gvqsefktb.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://baike.fehbvm.com/Article/details/gtahtikmb.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://read.share.hesvh.cn/Article/details/gntdgwuva.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://baike.hesvh.cn/Article/details/gcdvgvtqw.sHtML

PHP:  if (empty($x)) {}
来源：http://baike.fehbvm.com/Article/details/gbhkmzswy.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mobile.hesvh.cn/Article/details/ghlrifhvm.sHtML

TS:   if (x == null) {}
来源：http://m.share.fehbvm.com/Article/details/ghzkiaivw.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.share.fehbvm.com/Article/details/gitaqsart.sHtML

Go:   if x == nil {}
来源：http://read.share.fehbvm.com/Article/details/gldixcnbf.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.share.zdbjq.cn/Article/details/gbvddolvl.sHtML

C#:   if (x is null) {}
来源：http://m.share.fehbvm.com/Article/details/gizgxwbpu.sHtML

[P07] 防抖与节流
来源：http://m.share.zdbjq.cn/Article/details/gllemxxad.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.share.zdbjq.cn/Article/details/gbsmbrzpy.sHtML

PHP:  // 手写时间戳比较
来源：http://wap.fehbvm.com/Article/details/glqegmjlz.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.fehbvm.com/Article/details/gddinenfp.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.hesvh.cn/Article/details/geodsxkcq.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wap.zdbjq.cn/Article/details/gdfmecxmh.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.share.zdbjq.cn/Article/details/gcsccuzzb.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.share.fehbvm.com/Article/details/gcxvzmyko.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.m.share.fehbvm.com/Article/details/geshckmhp.sHtML

[P08] 处理浮点精度问题
来源：http://mobile.zdbjq.cn/Article/details/gmgleahmj.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://3g.hesvh.cn/Article/details/gpxbaqrub.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mobile.fehbvm.com/Article/details/ghyatmnnz.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.fehbvm.com/Article/details/gerlocods.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://blog.hesvh.cn/Article/details/gfakariwa.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wap.fehbvm.com/Article/details/gzuiruhuc.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://m.share.hesvh.cn/Article/details/goschrlzc.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mobile.zdbjq.cn/Article/details/gkzobmhst.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://blog.fehbvm.com/Article/details/gulwrvfgr.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gilpobjxn.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://blog.zdbjq.cn/Article/details/ggseuzwkf.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gkpxvtmuz.sHtML

[Q01] 创建表
来源：http://read.share.fehbvm.com/Article/details/gtytbsuwx.sHtML

CREATE TABLE users (
来源：http://baike.hesvh.cn/Article/details/gstfoznfd.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.hesvh.cn/Article/details/gzbkhmhoa.sHtML

name VARCHAR(50) NOT NULL,
来源：http://read.share.fehbvm.com/Article/details/glinmntpx.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.m.share.fehbvm.com/Article/details/gykscbvxr.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.share.hesvh.cn/Article/details/grvsiozjp.sHtML

);
来源：http://wap.fehbvm.com/Article/details/gwztnpekd.sHtML

[Q02] 创建带外键的表
来源：http://baike.zdbjq.cn/Article/details/gaefprgnh.sHtML

CREATE TABLE orders (
来源：http://mobile.fehbvm.com/Article/details/gkmaeentd.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.zdbjq.cn/Article/details/gzjcmnbee.sHtML

user_id INT NOT NULL,
来源：http://3g.fehbvm.com/Article/details/glukkgyem.sHtML

amount DECIMAL(10, 2),
来源：http://m.share.zdbjq.cn/Article/details/gtnajbetl.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.blog.fehbvm.com/Article/details/guglbgpre.sHtML

);
来源：http://www.blog.zdbjq.cn/Article/details/gjcinocrr.sHtML

[Q03] 增加列
来源：http://m.share.zdbjq.cn/Article/details/gbxjrmhdp.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.blog.zdbjq.cn/Article/details/grjpreaxy.sHtML

[Q04] 修改列类型
来源：http://mobile.zdbjq.cn/Article/details/gjgvxlftv.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://blog.fehbvm.com/Article/details/gclqtenqa.sHtML

[Q05] 重命名列
来源：http://wap.hesvh.cn/Article/details/gwtzebprq.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://3g.fehbvm.com/Article/details/goniwxyry.sHtML

[Q06] 删除列
来源：http://read.share.fehbvm.com/Article/details/gpegewjao.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://baike.zdbjq.cn/Article/details/gsodywdab.sHtML

[Q07] 删除表
来源：http://3g.zdbjq.cn/Article/details/gonvvzwbm.sHtML

DROP TABLE IF EXISTS orders;
来源：http://m.share.fehbvm.com/Article/details/gwmmcujnd.sHtML

[Q08] 创建普通索引
来源：http://www.blog.zdbjq.cn/Article/details/gqqyexmvf.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.share.hesvh.cn/Article/details/glfptwibd.sHtML

[Q09] 创建唯一索引
来源：http://www.m.share.hesvh.cn/Article/details/gjbnrldea.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://read.share.fehbvm.com/Article/details/gpirsfyba.sHtML

[Q10] 插入单行
来源：http://mobile.zdbjq.cn/Article/details/gugtadlut.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.share.zdbjq.cn/Article/details/gpkpoynme.sHtML

[Q11] 一次插入多行
来源：http://wap.fehbvm.com/Article/details/ghisztsuv.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://m.share.hesvh.cn/Article/details/gpnqfqwnk.sHtML

[Q12] 插入后取自增 ID
来源：http://www.share.hesvh.cn/Article/details/gmbdclupx.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://3g.zdbjq.cn/Article/details/gsxptogil.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://m.share.fehbvm.com/Article/details/gheshmhgo.sHtML

[Q13] 忽略重复插入
来源：http://m.share.zdbjq.cn/Article/details/gzdojlwht.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://m.share.hesvh.cn/Article/details/gajtrsfgl.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.share.hesvh.cn/Article/details/ggkgjsayh.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mobile.zdbjq.cn/Article/details/guntqrqme.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://3g.zdbjq.cn/Article/details/grnasyrtb.sHtML

[Q15] 查询全部
来源：http://www.m.share.hesvh.cn/Article/details/gpzsgsccx.sHtML

SELECT * FROM users;
来源：http://wap.fehbvm.com/Article/details/gtwdcbkff.sHtML

[Q16] 查询指定列
来源：http://read.share.fehbvm.com/Article/details/gpjwyccoc.sHtML

SELECT id, name FROM users;
来源：http://baike.hesvh.cn/Article/details/gxgalmcam.sHtML

[Q17] 条件查询
来源：http://blog.fehbvm.com/Article/details/gbhdutdql.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.blog.fehbvm.com/Article/details/gcvfbddab.sHtML

[Q18] 模糊匹配
来源：http://baike.fehbvm.com/Article/details/gfbazpqmc.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://m.share.zdbjq.cn/Article/details/gjrpuvzdy.sHtML

[Q19] 范围查询
来源：http://m.share.hesvh.cn/Article/details/gwvqaakse.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://m.share.zdbjq.cn/Article/details/gcekbblbb.sHtML

[Q20] IN 列表
来源：http://mobile.zdbjq.cn/Article/details/gxlfokizl.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wap.hesvh.cn/Article/details/ggpxhwaye.sHtML

[Q21] 空值判断
来源：http://read.share.zdbjq.cn/Article/details/gltpyozzn.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://read.share.hesvh.cn/Article/details/gszymqrav.sHtML

[Q22] 排序
来源：http://wap.fehbvm.com/Article/details/gdtixlvte.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.zdbjq.cn/Article/details/geooqbzdr.sHtML

[Q23] 分页
来源：http://blog.zdbjq.cn/Article/details/gedyrdrjk.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.blog.hesvh.cn/Article/details/gvhldvgyd.sHtML

[Q24] 去重
来源：http://www.share.hesvh.cn/Article/details/grmgnlydl.sHtML

SELECT DISTINCT city FROM users;
来源：http://blog.hesvh.cn/Article/details/gggdwqccc.sHtML

[Q25] 只取前 N 条
来源：http://www.m.share.hesvh.cn/Article/details/ghrdvvxvu.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://baike.hesvh.cn/Article/details/gpzpvfzkh.sHtML

[Q26] 计数
来源：http://baike.zdbjq.cn/Article/details/gwkzxmxbm.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gajdlbtqw.sHtML

[Q27] 条件计数
来源：http://mobile.fehbvm.com/Article/details/glfzuqggu.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://baike.hesvh.cn/Article/details/ggpeldtbr.sHtML

[Q28] 求和与平均
来源：http://read.share.fehbvm.com/Article/details/ggqskcrix.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://blog.fehbvm.com/Article/details/gksmdjdgj.sHtML

[Q29] 最大最小值
来源：http://www.blog.zdbjq.cn/Article/details/goctxavol.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gnvyiifsv.sHtML

[Q30] 分组统计
来源：http://blog.fehbvm.com/Article/details/geyguphbp.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.hesvh.cn/Article/details/gkumozgbv.sHtML

[Q31] 分组后过滤
来源：http://read.share.hesvh.cn/Article/details/gzhlausdu.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://read.share.fehbvm.com/Article/details/gpbfhkraj.sHtML

[Q32] 分组拼接字符串
来源：http://wap.zdbjq.cn/Article/details/ggrbeevju.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://baike.hesvh.cn/Article/details/gubeidoxq.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://blog.zdbjq.cn/Article/details/gqcpbytxi.sHtML

[Q33] 多列分组
来源：http://3g.zdbjq.cn/Article/details/gsuweyrtv.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.share.zdbjq.cn/Article/details/gxubmjlck.sHtML

[Q34] 每组取第一条
来源：http://read.share.zdbjq.cn/Article/details/ggtjtvrsq.sHtML

SELECT * FROM (
来源：http://read.share.zdbjq.cn/Article/details/gwdozdulj.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.zdbjq.cn/Article/details/gfdogcwbq.sHtML

) t WHERE rn = 1;
来源：http://mobile.hesvh.cn/Article/details/gvxlyoiwn.sHtML

[Q35] 内连接
来源：http://www.blog.zdbjq.cn/Article/details/gbvybuwea.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://m.share.hesvh.cn/Article/details/gmlajkvla.sHtML

[Q36] 左连接
来源：http://blog.hesvh.cn/Article/details/guegsenmg.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.zdbjq.cn/Article/details/gagoltckl.sHtML

[Q37] 右连接
来源：http://mobile.zdbjq.cn/Article/details/gceyjnkyk.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.share.fehbvm.com/Article/details/grjsaqoxk.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.fehbvm.com/Article/details/gmeqxnxxl.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://baike.hesvh.cn/Article/details/gayonnrml.sHtML

[Q39] 自连接（查上下级）
来源：http://mobile.zdbjq.cn/Article/details/grgeurhzd.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://read.share.hesvh.cn/Article/details/grdjysdvx.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.blog.hesvh.cn/Article/details/getkayuzw.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.hesvh.cn/Article/details/gpbzfkqfu.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.hesvh.cn/Article/details/gnebvdzhf.sHtML

[Q41] 多表连接
来源：http://3g.fehbvm.com/Article/details/ghtngbpkr.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.fehbvm.com/Article/details/gxnyrfsin.sHtML

JOIN users u ON u.id = o.user_id
来源：http://read.share.fehbvm.com/Article/details/gspltvxwu.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://wap.hesvh.cn/Article/details/gtbhuxhbk.sHtML

[Q42] 连接条件附加过滤
来源：http://baike.hesvh.cn/Article/details/gauutzqdv.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.blog.fehbvm.com/Article/details/gmwgwbxwb.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://m.share.zdbjq.cn/Article/details/gcqlboruw.sHtML

[Q43] 标量子查询
来源：http://blog.fehbvm.com/Article/details/gqegccdww.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.fehbvm.com/Article/details/gvzyopzyz.sHtML

[Q44] IN 子查询
来源：http://read.share.hesvh.cn/Article/details/glfexoqtv.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mobile.hesvh.cn/Article/details/gvfchojjr.sHtML

[Q45] EXISTS 判断存在
来源：http://www.blog.fehbvm.com/Article/details/goofiioos.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.zdbjq.cn/Article/details/gkfszlopi.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://wap.hesvh.cn/Article/details/gqiivaphx.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.zdbjq.cn/Article/details/gwwuloasz.sHtML

[Q47] 与平均值比较
来源：http://read.share.fehbvm.com/Article/details/ghfrhpfsf.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.zdbjq.cn/Article/details/gbfridzgq.sHtML

[Q48] CTE 公用表表达式
来源：http://mobile.zdbjq.cn/Article/details/genothijd.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://m.share.fehbvm.com/Article/details/gqqpkckmc.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://mobile.zdbjq.cn/Article/details/gwqhlqwhg.sHtML

[Q49] 更新单行
来源：http://www.m.share.fehbvm.com/Article/details/gfzjofqpq.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.fehbvm.com/Article/details/gjqvvknlr.sHtML

[Q50] 批量更新
来源：http://wap.hesvh.cn/Article/details/glmfsmski.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://baike.fehbvm.com/Article/details/gximgppgm.sHtML

[Q51] 用子查询更新
来源：http://wap.zdbjq.cn/Article/details/gugvjgzxf.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.fehbvm.com/Article/details/gksvmmgld.sHtML

[Q52] 删除指定行
来源：http://mobile.hesvh.cn/Article/details/gxirsilky.sHtML

DELETE FROM users WHERE id = 10;
来源：http://blog.hesvh.cn/Article/details/gfqhpsugl.sHtML

[Q53] 按条件删除
来源：http://read.share.zdbjq.cn/Article/details/ghrjppmnh.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.fehbvm.com/Article/details/grrrtmhia.sHtML

[Q54] 清空表
来源：http://blog.fehbvm.com/Article/details/gdqofmtjo.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.fehbvm.com/Article/details/gaoqfcigq.sHtML

[Q55] 排名（并列占位）
来源：http://mobile.zdbjq.cn/Article/details/gapmcgclg.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.zdbjq.cn/Article/details/gvcwiabbn.sHtML

[Q56] 密集排名（并列不占位）
来源：http://blog.fehbvm.com/Article/details/ggctrrrfb.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://read.share.zdbjq.cn/Article/details/gioigogno.sHtML

[Q57] 行号
来源：http://blog.fehbvm.com/Article/details/gjbmqcish.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://3g.fehbvm.com/Article/details/gxwehlncd.sHtML

[Q58] 累计求和
来源：http://mobile.hesvh.cn/Article/details/gzcjpioye.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.hesvh.cn/Article/details/gzutzcjjq.sHtML

[Q59] 分组内累计
来源：http://blog.hesvh.cn/Article/details/gyjfmzrsj.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.hesvh.cn/Article/details/gfkupleaf.sHtML

[Q60] 取上一行 / 下一行
来源：http://blog.zdbjq.cn/Article/details/gbruesqqj.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wap.zdbjq.cn/Article/details/gwogsqmuu.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.fehbvm.com/Article/details/gkyqkxzqw.sHtML

[Q61] 移动平均
来源：http://www.m.share.zdbjq.cn/Article/details/gbxvnqyko.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.zdbjq.cn/Article/details/glwmaeizp.sHtML

[Q62] 分组占比
来源：http://mobile.fehbvm.com/Article/details/gbsqmsocd.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.hesvh.cn/Article/details/glvyuhbns.sHtML

[Q63] 开启事务
来源：http://www.blog.zdbjq.cn/Article/details/gponosdec.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.fehbvm.com/Article/details/gfnzpwakn.sHtML

[Q64] 提交事务
来源：http://read.share.zdbjq.cn/Article/details/gkqwwbszd.sHtML

COMMIT;
来源：http://3g.fehbvm.com/Article/details/gtmbjglwi.sHtML

[Q65] 回滚事务
来源：http://m.share.fehbvm.com/Article/details/gtmcteohd.sHtML

ROLLBACK;
来源：http://read.share.zdbjq.cn/Article/details/gydgfkijx.sHtML

[Q66] 行锁查询
来源：http://wap.zdbjq.cn/Article/details/gyhsazxfa.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.hesvh.cn/Article/details/gdsillqrf.sHtML

[Q67] 设置隔离级别
来源：http://m.share.hesvh.cn/Article/details/gicdnvoao.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.hesvh.cn/Article/details/gxtoijqch.sHtML

[Q68] 保存点
来源：http://www.share.zdbjq.cn/Article/details/gmkjlmeas.sHtML

SAVEPOINT sp1;
来源：http://blog.hesvh.cn/Article/details/gyvbhqomw.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.hesvh.cn/Article/details/gztxsnlrn.sHtML

[Q69] 查看执行计划
来源：http://www.blog.zdbjq.cn/Article/details/gzewqbnow.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.fehbvm.com/Article/details/gqdguqcpf.sHtML

[Q70] 更新统计信息
来源：http://3g.hesvh.cn/Article/details/gngtnbmxa.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.fehbvm.com/Article/details/gzvqdkhmr.sHtML

[Q71] 查看建表语句
来源：http://m.share.zdbjq.cn/Article/details/gojyobpqv.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.zdbjq.cn/Article/details/gtgwrxkku.sHtML

[Q72] 查看索引
来源：http://www.m.share.zdbjq.cn/Article/details/ggzbxjeta.sHtML

SHOW INDEX FROM users;
来源：http://m.share.fehbvm.com/Article/details/ghmfdqrps.sHtML

[Q73] 查看表状态
来源：http://3g.hesvh.cn/Article/details/gunpacejs.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.hesvh.cn/Article/details/gpjllkbww.sHtML

[Q74] 强制使用索引
来源：http://wap.hesvh.cn/Article/details/gviietrew.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.hesvh.cn/Article/details/glekzkptd.sHtML

[Q75] 日期格式化
来源：http://www.blog.hesvh.cn/Article/details/gjmspcofl.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.hesvh.cn/Article/details/ggomznjry.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.zdbjq.cn/Article/details/gcjtsmfzx.sHtML

[Q76] 按天统计
来源：http://m.share.fehbvm.com/Article/details/gceqqykxh.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.fehbvm.com/Article/details/gboipdhfn.sHtML

[Q77] 时间加减
来源：http://baike.hesvh.cn/Article/details/gzdxpgfit.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.zdbjq.cn/Article/details/gpjukeyyg.sHtML

[Q78] 当前时间
来源：http://blog.fehbvm.com/Article/details/gavlkzzto.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.zdbjq.cn/Article/details/ggsxpzewm.sHtML

[Q79] 字符串拼接
来源：http://wap.fehbvm.com/Article/details/gdgfidutg.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.zdbjq.cn/Article/details/ghslemjej.sHtML

[Q80] 字符串截取
来源：http://m.share.zdbjq.cn/Article/details/gevdvgxkn.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.fehbvm.com/Article/details/glntkereu.sHtML

[Q81] 字符串替换
来源：http://www.m.share.hesvh.cn/Article/details/grfhqqcer.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gxdopalfg.sHtML


<!-- 参考信息 -->