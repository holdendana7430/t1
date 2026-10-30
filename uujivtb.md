代发 wailian999

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.blog.zdbjq.cn/Article/details/gbtvaydtx.sHtML

[O03] 加锁保护共享数据
来源：http://wap.fehbvm.com/Article/details/gverjgiuf.sHtML

Py:   with lock: shared += 1
来源：http://mobile.fehbvm.com/Article/details/gyldylvlf.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://mobile.zdbjq.cn/Article/details/gucqmfcwc.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wap.zdbjq.cn/Article/details/gnnmdxvok.sHtML

TS:   // 同 JS
来源：http://mobile.hesvh.cn/Article/details/ggvmsafws.sHtML

Java: synchronized (this) { shared++; }
来源：http://m.share.zdbjq.cn/Article/details/gyyaklbub.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.zdbjq.cn/Article/details/gcvrayprx.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.share.hesvh.cn/Article/details/gbjcwduiq.sHtML

C#:   lock (gate) { shared++; }
来源：http://baike.fehbvm.com/Article/details/ghanxgpmt.sHtML

[O04] 定义异步函数并等待
来源：http://mobile.fehbvm.com/Article/details/gxyzrhtwb.sHtML

Py:   async def f():⏎    await g()
来源：http://m.share.fehbvm.com/Article/details/gykdwxxli.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://3g.zdbjq.cn/Article/details/gwqqffcqm.sHtML

JS:   async function f() { await g(); }
来源：http://3g.fehbvm.com/Article/details/ghxbawsor.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://m.share.fehbvm.com/Article/details/gbqvzcflv.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://baike.fehbvm.com/Article/details/gqfckhzcs.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://blog.hesvh.cn/Article/details/gefwccsyx.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.blog.zdbjq.cn/Article/details/gcjrdcjkx.sHtML

C#:   async Task F() { await G(); }
来源：http://baike.zdbjq.cn/Article/details/gftbvzdjr.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.share.zdbjq.cn/Article/details/golqwhzso.sHtML

Py:   asyncio.gather(*tasks)
来源：http://baike.fehbvm.com/Article/details/gmtmrbymu.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://blog.hesvh.cn/Article/details/gqodzdwzv.sHtML

JS:   await Promise.all(tasks)
来源：http://baike.zdbjq.cn/Article/details/gicsqsvkd.sHtML

TS:   await Promise.all(tasks)
来源：http://www.share.hesvh.cn/Article/details/grjvkzdyb.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://read.share.fehbvm.com/Article/details/gcmqsarpe.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://m.share.hesvh.cn/Article/details/gnvnficbk.sHtML

Ruby: threads.map(&:join)
来源：http://3g.zdbjq.cn/Article/details/gqztluvuq.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://3g.fehbvm.com/Article/details/gilmladkj.sHtML

[O06] 使用进程池
来源：http://mobile.zdbjq.cn/Article/details/gudmtyaam.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://3g.zdbjq.cn/Article/details/gpoqrmdlq.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://m.share.fehbvm.com/Article/details/gvrwrtuxn.sHtML

JS:   // child_process / cluster 模块
来源：http://3g.zdbjq.cn/Article/details/gflaygrrq.sHtML

TS:   // child_process / cluster 模块
来源：http://m.share.zdbjq.cn/Article/details/goozouzwt.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mobile.hesvh.cn/Article/details/gxzlpqdrj.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://3g.zdbjq.cn/Article/details/gnhmujnfa.sHtML

Ruby: // fork 块
来源：http://wap.zdbjq.cn/Article/details/gzykspzph.sHtML

C#:   Parallel.For
来源：http://wap.zdbjq.cn/Article/details/gbdglmnma.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/ghqoxvyxz.sHtML

P. 常用工具函数
来源：http://3g.hesvh.cn/Article/details/gknxadrak.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/ggjlojdpo.sHtML

[P01] 生成 UUID
来源：http://mobile.zdbjq.cn/Article/details/gbpwxaxvp.sHtML

Py:   str(uuid.uuid4())
来源：http://www.blog.fehbvm.com/Article/details/gdujlbcdq.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://read.share.zdbjq.cn/Article/details/gmotkdosu.sHtML

JS:   crypto.randomUUID()
来源：http://read.share.zdbjq.cn/Article/details/ghzedkmdx.sHtML

TS:   crypto.randomUUID()
来源：http://read.share.zdbjq.cn/Article/details/gifxidblv.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.blog.zdbjq.cn/Article/details/gkpuxhxrf.sHtML

Go:   // 用 github.com/google/uuid
来源：http://read.share.fehbvm.com/Article/details/gooyvfjnn.sHtML

Ruby: SecureRandom.uuid
来源：http://read.share.fehbvm.com/Article/details/gcmqnbbhv.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.m.share.fehbvm.com/Article/details/gnvpybafj.sHtML

[P02] MD5 / SHA256 摘要
来源：http://3g.fehbvm.com/Article/details/grpkzautt.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://blog.zdbjq.cn/Article/details/gtmvnpkdu.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://3g.zdbjq.cn/Article/details/gedyulzxn.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.m.share.zdbjq.cn/Article/details/gplwrcxmz.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.m.share.fehbvm.com/Article/details/gvckjmyaf.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.m.share.hesvh.cn/Article/details/grakbexbt.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://blog.fehbvm.com/Article/details/gyvzauhtw.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mobile.zdbjq.cn/Article/details/ggbujppzt.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.m.share.hesvh.cn/Article/details/ggyzqonwj.sHtML

[P03] 生成短随机字符串
来源：http://baike.zdbjq.cn/Article/details/grqtixljg.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://m.share.hesvh.cn/Article/details/gayeplprr.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://3g.hesvh.cn/Article/details/gebnmwadr.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.zdbjq.cn/Article/details/ggkvjubeh.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.fehbvm.com/Article/details/glrsixdkm.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.share.hesvh.cn/Article/details/gtyoyqgjv.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.m.share.fehbvm.com/Article/details/gkwifsruo.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.share.hesvh.cn/Article/details/gmpcdcugh.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://blog.fehbvm.com/Article/details/gwnfkoxro.sHtML

[P04] 求长度
来源：http://baike.zdbjq.cn/Article/details/gvyxglmik.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://m.share.hesvh.cn/Article/details/gkirgdiye.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.fehbvm.com/Article/details/gfbyhpcdz.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.hesvh.cn/Article/details/gxeqizbcy.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.hesvh.cn/Article/details/gamoiqgub.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.blog.hesvh.cn/Article/details/gizvlvran.sHtML

Go:   len(arr);  len(m)
来源：http://wap.fehbvm.com/Article/details/grytxykrf.sHtML

Ruby: x.length;  x.size
来源：http://www.blog.zdbjq.cn/Article/details/gsurlhmhg.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://mobile.zdbjq.cn/Article/details/grbiafsnd.sHtML

[P05] 判断两个对象内容是否相等
来源：http://mobile.fehbvm.com/Article/details/ggumoqbkd.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://read.share.fehbvm.com/Article/details/gtqldeoja.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.m.share.zdbjq.cn/Article/details/gwstnbhzn.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://m.share.hesvh.cn/Article/details/gvasvqtgv.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.zdbjq.cn/Article/details/gzrdgdegc.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mobile.fehbvm.com/Article/details/gaxxxusdu.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://3g.hesvh.cn/Article/details/ggtirxncm.sHtML

Ruby: a == b
来源：http://mobile.fehbvm.com/Article/details/gtfnpnatu.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.blog.fehbvm.com/Article/details/gphlturfg.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://m.share.hesvh.cn/Article/details/gbzeeckki.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://blog.fehbvm.com/Article/details/gapnpmrgu.sHtML

PHP:  if (empty($x)) {}
来源：http://read.share.hesvh.cn/Article/details/gdnfhdecg.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://3g.fehbvm.com/Article/details/gjkxeycbs.sHtML

TS:   if (x == null) {}
来源：http://mobile.hesvh.cn/Article/details/gbjzvvejv.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://wap.zdbjq.cn/Article/details/gptocsnxd.sHtML

Go:   if x == nil {}
来源：http://blog.fehbvm.com/Article/details/gpgzcgdcx.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wap.fehbvm.com/Article/details/gxscbcola.sHtML

C#:   if (x is null) {}
来源：http://m.share.hesvh.cn/Article/details/gubbkrrnx.sHtML

[P07] 防抖与节流
来源：http://m.share.hesvh.cn/Article/details/gphdlrrju.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://blog.hesvh.cn/Article/details/gpfwkudbl.sHtML

PHP:  // 手写时间戳比较
来源：http://wap.zdbjq.cn/Article/details/gbpzbdpfj.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.zdbjq.cn/Article/details/gvgxfxbux.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.hesvh.cn/Article/details/gqeclnkhd.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://3g.hesvh.cn/Article/details/gvyfiwcbw.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.share.hesvh.cn/Article/details/glirtyflg.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.fehbvm.com/Article/details/gdlbzainu.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://baike.hesvh.cn/Article/details/ghrhasxrw.sHtML

[P08] 处理浮点精度问题
来源：http://wap.fehbvm.com/Article/details/ghxhyszhp.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.blog.hesvh.cn/Article/details/gpjpopjlt.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://m.share.zdbjq.cn/Article/details/gjbpoplbj.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.m.share.zdbjq.cn/Article/details/gpcsgvxjg.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://read.share.hesvh.cn/Article/details/gdqqculob.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://read.share.hesvh.cn/Article/details/gfvkeipoa.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.share.fehbvm.com/Article/details/ggyczibcq.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wap.zdbjq.cn/Article/details/gtdxrxfhx.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.share.hesvh.cn/Article/details/ghcngotzp.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gieskcjsj.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://3g.hesvh.cn/Article/details/ggqfyabog.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gnbbmmcep.sHtML

[Q01] 创建表
来源：http://www.blog.zdbjq.cn/Article/details/ggdcknqqo.sHtML

CREATE TABLE users (
来源：http://m.share.fehbvm.com/Article/details/giuplqzpp.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.fehbvm.com/Article/details/gdporpdel.sHtML

name VARCHAR(50) NOT NULL,
来源：http://blog.fehbvm.com/Article/details/gxrbizbbj.sHtML

email VARCHAR(100) UNIQUE,
来源：http://m.share.zdbjq.cn/Article/details/gbbbnsiuc.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mobile.hesvh.cn/Article/details/grohbuouj.sHtML

);
来源：http://blog.zdbjq.cn/Article/details/gsfjvczqm.sHtML

[Q02] 创建带外键的表
来源：http://www.m.share.zdbjq.cn/Article/details/gpeicfyzl.sHtML

CREATE TABLE orders (
来源：http://mobile.hesvh.cn/Article/details/gxbnmljkf.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.hesvh.cn/Article/details/glwopkoww.sHtML

user_id INT NOT NULL,
来源：http://mobile.fehbvm.com/Article/details/guptnjibh.sHtML

amount DECIMAL(10, 2),
来源：http://baike.hesvh.cn/Article/details/gobrfqubc.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wap.hesvh.cn/Article/details/gfdhrexwd.sHtML

);
来源：http://baike.fehbvm.com/Article/details/gnbowlwzq.sHtML

[Q03] 增加列
来源：http://read.share.zdbjq.cn/Article/details/gjgvclbzv.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://read.share.zdbjq.cn/Article/details/gtsjvbixm.sHtML

[Q04] 修改列类型
来源：http://mobile.hesvh.cn/Article/details/ghcapeqju.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://baike.fehbvm.com/Article/details/gbwuebtlw.sHtML

[Q05] 重命名列
来源：http://read.share.fehbvm.com/Article/details/gscfoggdk.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mobile.hesvh.cn/Article/details/gkgcikfhm.sHtML

[Q06] 删除列
来源：http://m.share.fehbvm.com/Article/details/grmgrjgfu.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.share.fehbvm.com/Article/details/guclubwil.sHtML

[Q07] 删除表
来源：http://wap.fehbvm.com/Article/details/ghefsvvtc.sHtML

DROP TABLE IF EXISTS orders;
来源：http://3g.hesvh.cn/Article/details/gvmhbwzgs.sHtML

[Q08] 创建普通索引
来源：http://blog.zdbjq.cn/Article/details/golwplohp.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://blog.hesvh.cn/Article/details/ghlnxakaq.sHtML

[Q09] 创建唯一索引
来源：http://www.m.share.zdbjq.cn/Article/details/ghywgkjbl.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mobile.fehbvm.com/Article/details/gnikatjwp.sHtML

[Q10] 插入单行
来源：http://www.m.share.fehbvm.com/Article/details/golfpkcei.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.hesvh.cn/Article/details/gqsrnozvy.sHtML

[Q11] 一次插入多行
来源：http://wap.zdbjq.cn/Article/details/gqsqfgbpt.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.share.hesvh.cn/Article/details/gvcpuhxib.sHtML

[Q12] 插入后取自增 ID
来源：http://www.share.zdbjq.cn/Article/details/grmlxyqjq.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://blog.fehbvm.com/Article/details/gpvinwnxg.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://blog.fehbvm.com/Article/details/gotyqljsu.sHtML

[Q13] 忽略重复插入
来源：http://blog.fehbvm.com/Article/details/gbpoiusef.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mobile.fehbvm.com/Article/details/gfkpdncvn.sHtML

[Q14] 存在则更新（upsert）
来源：http://m.share.hesvh.cn/Article/details/ggcvvkryz.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mobile.fehbvm.com/Article/details/ggtofxweq.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.share.hesvh.cn/Article/details/gjvkzwapx.sHtML

[Q15] 查询全部
来源：http://3g.fehbvm.com/Article/details/gkdqnvome.sHtML

SELECT * FROM users;
来源：http://m.share.hesvh.cn/Article/details/guyjaowlw.sHtML

[Q16] 查询指定列
来源：http://read.share.hesvh.cn/Article/details/gxtwzxjim.sHtML

SELECT id, name FROM users;
来源：http://baike.hesvh.cn/Article/details/gxxvgwpmb.sHtML

[Q17] 条件查询
来源：http://www.share.fehbvm.com/Article/details/gkhnrqkxs.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://blog.zdbjq.cn/Article/details/girjfwbid.sHtML

[Q18] 模糊匹配
来源：http://www.m.share.fehbvm.com/Article/details/gbndveuqi.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.blog.hesvh.cn/Article/details/grocxuyid.sHtML

[Q19] 范围查询
来源：http://baike.fehbvm.com/Article/details/gidnecnto.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.m.share.fehbvm.com/Article/details/gublbovzy.sHtML

[Q20] IN 列表
来源：http://www.share.fehbvm.com/Article/details/ggtqcjsia.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.blog.hesvh.cn/Article/details/ggjopbadr.sHtML

[Q21] 空值判断
来源：http://read.share.zdbjq.cn/Article/details/gtbdjqdaa.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.blog.fehbvm.com/Article/details/gdvqnbxyn.sHtML

[Q22] 排序
来源：http://3g.fehbvm.com/Article/details/gbpwmmyuh.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wap.fehbvm.com/Article/details/gmgyzrinn.sHtML

[Q23] 分页
来源：http://www.m.share.zdbjq.cn/Article/details/gphjniczp.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://3g.hesvh.cn/Article/details/geylvkwhd.sHtML

[Q24] 去重
来源：http://www.m.share.zdbjq.cn/Article/details/gtpvkkbbn.sHtML

SELECT DISTINCT city FROM users;
来源：http://3g.fehbvm.com/Article/details/gtruppqlq.sHtML

[Q25] 只取前 N 条
来源：http://wap.fehbvm.com/Article/details/gqfxybbgy.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://baike.zdbjq.cn/Article/details/gukwkrqoi.sHtML

[Q26] 计数
来源：http://baike.zdbjq.cn/Article/details/gknmyexwl.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.share.fehbvm.com/Article/details/gwmboxhhp.sHtML

[Q27] 条件计数
来源：http://baike.hesvh.cn/Article/details/gtcrsgrdu.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/geejsdvkw.sHtML

[Q28] 求和与平均
来源：http://wap.hesvh.cn/Article/details/gqzkxdmwt.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://baike.hesvh.cn/Article/details/gaazzqurg.sHtML

[Q29] 最大最小值
来源：http://baike.zdbjq.cn/Article/details/gnreblsgf.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.zdbjq.cn/Article/details/gavtpwhpf.sHtML

[Q30] 分组统计
来源：http://mobile.fehbvm.com/Article/details/gphlfuxbu.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.hesvh.cn/Article/details/gkfhivzfp.sHtML

[Q31] 分组后过滤
来源：http://wap.zdbjq.cn/Article/details/gazggalpo.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.fehbvm.com/Article/details/glkkuxala.sHtML

[Q32] 分组拼接字符串
来源：http://blog.fehbvm.com/Article/details/gdftdzkco.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wap.zdbjq.cn/Article/details/gbygufcfb.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mobile.zdbjq.cn/Article/details/gaiinuowf.sHtML

[Q33] 多列分组
来源：http://www.m.share.zdbjq.cn/Article/details/ggtaddisw.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.share.fehbvm.com/Article/details/gstpqhwpd.sHtML

[Q34] 每组取第一条
来源：http://read.share.fehbvm.com/Article/details/guaztkwbt.sHtML

SELECT * FROM (
来源：http://www.m.share.hesvh.cn/Article/details/gwgotkwcn.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.share.fehbvm.com/Article/details/gvvnrbwkr.sHtML

) t WHERE rn = 1;
来源：http://m.share.hesvh.cn/Article/details/gltbmdggt.sHtML

[Q35] 内连接
来源：http://read.share.fehbvm.com/Article/details/greliymyz.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.zdbjq.cn/Article/details/grmrgbodi.sHtML

[Q36] 左连接
来源：http://read.share.hesvh.cn/Article/details/gntmyghic.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.zdbjq.cn/Article/details/gkdzquboy.sHtML

[Q37] 右连接
来源：http://read.share.fehbvm.com/Article/details/gvbfecwdx.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.hesvh.cn/Article/details/gzfcbieok.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://wap.fehbvm.com/Article/details/gzrzajrdy.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://blog.hesvh.cn/Article/details/gkoledkqx.sHtML

[Q39] 自连接（查上下级）
来源：http://wap.hesvh.cn/Article/details/gjaottysp.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.hesvh.cn/Article/details/ghldbinct.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://m.share.hesvh.cn/Article/details/gjmmqhwkz.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://m.share.hesvh.cn/Article/details/gkdlcrnqm.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.share.zdbjq.cn/Article/details/gyalnplhd.sHtML

[Q41] 多表连接
来源：http://3g.fehbvm.com/Article/details/gaadcujlh.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.fehbvm.com/Article/details/gxdiumkfy.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.share.hesvh.cn/Article/details/gtjmcyzjo.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://blog.hesvh.cn/Article/details/gymfsemgi.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.zdbjq.cn/Article/details/gsgyolaui.sHtML

SELECT u.name, o.amount FROM users u
来源：http://wap.fehbvm.com/Article/details/gvthbjdux.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wap.fehbvm.com/Article/details/gkngtnibk.sHtML

[Q43] 标量子查询
来源：http://www.share.zdbjq.cn/Article/details/gfdnpbnqg.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://read.share.fehbvm.com/Article/details/gvsrkqaii.sHtML

[Q44] IN 子查询
来源：http://blog.hesvh.cn/Article/details/gttfjruma.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://read.share.zdbjq.cn/Article/details/gfzmzfymh.sHtML

[Q45] EXISTS 判断存在
来源：http://m.share.hesvh.cn/Article/details/gaaprrbsb.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.zdbjq.cn/Article/details/glsnkhebe.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.fehbvm.com/Article/details/gssgdvdpk.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.hesvh.cn/Article/details/gahwmwasq.sHtML

[Q47] 与平均值比较
来源：http://www.share.hesvh.cn/Article/details/gleoiccsp.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.share.fehbvm.com/Article/details/gmiaolehk.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.hesvh.cn/Article/details/girrwlvjr.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.blog.zdbjq.cn/Article/details/gmzzogxis.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.blog.zdbjq.cn/Article/details/gtalqpupu.sHtML

[Q49] 更新单行
来源：http://blog.hesvh.cn/Article/details/gjohnaotp.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://3g.zdbjq.cn/Article/details/gzuhmonts.sHtML

[Q50] 批量更新
来源：http://baike.zdbjq.cn/Article/details/gnjgewsww.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.share.zdbjq.cn/Article/details/ggoaugzrq.sHtML

[Q51] 用子查询更新
来源：http://read.share.hesvh.cn/Article/details/grlpnbuxh.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://baike.fehbvm.com/Article/details/gxgwjhxwy.sHtML

[Q52] 删除指定行
来源：http://mobile.zdbjq.cn/Article/details/gvzwgrgau.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.hesvh.cn/Article/details/gwbyupolj.sHtML

[Q53] 按条件删除
来源：http://www.share.hesvh.cn/Article/details/gowosrioa.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.hesvh.cn/Article/details/grejqxodm.sHtML

[Q54] 清空表
来源：http://baike.fehbvm.com/Article/details/gpyxwjhue.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.hesvh.cn/Article/details/gslxzkoss.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.hesvh.cn/Article/details/glhnxbpfk.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.hesvh.cn/Article/details/ggdfanvrt.sHtML

[Q56] 密集排名（并列不占位）
来源：http://blog.hesvh.cn/Article/details/gdvguepwk.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.fehbvm.com/Article/details/gercnbxtp.sHtML

[Q57] 行号
来源：http://www.blog.zdbjq.cn/Article/details/gfkdabksk.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gmezqqwjd.sHtML

[Q58] 累计求和
来源：http://baike.fehbvm.com/Article/details/gjslclerb.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.zdbjq.cn/Article/details/gmwmaeggt.sHtML

[Q59] 分组内累计
来源：http://mobile.zdbjq.cn/Article/details/gedgjmwnt.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.zdbjq.cn/Article/details/grdketzsj.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.fehbvm.com/Article/details/gqriyvahu.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://baike.fehbvm.com/Article/details/gnxyhtrud.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.hesvh.cn/Article/details/gjhfrjxza.sHtML

[Q61] 移动平均
来源：http://baike.hesvh.cn/Article/details/glzdkqtpx.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.hesvh.cn/Article/details/gaorudioo.sHtML

[Q62] 分组占比
来源：http://mobile.hesvh.cn/Article/details/ghjzpffnx.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.fehbvm.com/Article/details/ggfmnqljk.sHtML

[Q63] 开启事务
来源：http://3g.hesvh.cn/Article/details/gagxcducg.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://blog.fehbvm.com/Article/details/grumnzijv.sHtML

[Q64] 提交事务
来源：http://www.blog.zdbjq.cn/Article/details/gpkvcaazk.sHtML

COMMIT;
来源：http://www.blog.hesvh.cn/Article/details/gtwpvsfhs.sHtML

[Q65] 回滚事务
来源：http://m.share.zdbjq.cn/Article/details/gowprosgz.sHtML

ROLLBACK;
来源：http://blog.zdbjq.cn/Article/details/gsotkzzqe.sHtML

[Q66] 行锁查询
来源：http://m.share.fehbvm.com/Article/details/ggkirpjnt.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mobile.hesvh.cn/Article/details/gvkdnlzot.sHtML

[Q67] 设置隔离级别
来源：http://mobile.zdbjq.cn/Article/details/ghsfifsms.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.zdbjq.cn/Article/details/gfxegeoxe.sHtML

[Q68] 保存点
来源：http://wap.zdbjq.cn/Article/details/ggmrbzksx.sHtML

SAVEPOINT sp1;
来源：http://mobile.hesvh.cn/Article/details/gxmfurnzy.sHtML

ROLLBACK TO sp1;
来源：http://mobile.hesvh.cn/Article/details/gqvxxcdml.sHtML

[Q69] 查看执行计划
来源：http://m.share.hesvh.cn/Article/details/ghfipgptv.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.zdbjq.cn/Article/details/gtyipsusw.sHtML

[Q70] 更新统计信息
来源：http://read.share.zdbjq.cn/Article/details/gzwxabgin.sHtML

ANALYZE TABLE users;
来源：http://baike.hesvh.cn/Article/details/gjezfignx.sHtML

[Q71] 查看建表语句
来源：http://m.share.fehbvm.com/Article/details/gthvsyzpc.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wap.zdbjq.cn/Article/details/glkldxeuh.sHtML

[Q72] 查看索引
来源：http://blog.zdbjq.cn/Article/details/gikglotiw.sHtML

SHOW INDEX FROM users;
来源：http://mobile.hesvh.cn/Article/details/gcowxishu.sHtML

[Q73] 查看表状态
来源：http://www.blog.hesvh.cn/Article/details/glfayzixr.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://wap.hesvh.cn/Article/details/gztjvwvcg.sHtML

[Q74] 强制使用索引
来源：http://baike.fehbvm.com/Article/details/ghzkhgksr.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.fehbvm.com/Article/details/gmhnsyfzx.sHtML

[Q75] 日期格式化
来源：http://www.m.share.fehbvm.com/Article/details/gufaqzoxd.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gjqohnabs.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.hesvh.cn/Article/details/gpihiyuoz.sHtML

[Q76] 按天统计
来源：http://www.m.share.zdbjq.cn/Article/details/gwxemytou.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wap.zdbjq.cn/Article/details/gvxiruhbl.sHtML

[Q77] 时间加减
来源：http://3g.zdbjq.cn/Article/details/gdiacqfbh.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://m.share.hesvh.cn/Article/details/gsexakcfz.sHtML

[Q78] 当前时间
来源：http://mobile.hesvh.cn/Article/details/gacoiuzib.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.zdbjq.cn/Article/details/gtxwyllfu.sHtML

[Q79] 字符串拼接
来源：http://baike.hesvh.cn/Article/details/gmvvzfjvo.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.hesvh.cn/Article/details/gmabtyurb.sHtML

[Q80] 字符串截取
来源：http://www.m.share.fehbvm.com/Article/details/gpvsijaxy.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.hesvh.cn/Article/details/gonlvoonk.sHtML

[Q81] 字符串替换
来源：http://mobile.hesvh.cn/Article/details/gcavmywjo.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.hesvh.cn/Article/details/gzbrsbdct.sHtML


<!-- 参考信息 -->