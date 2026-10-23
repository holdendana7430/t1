代发 wailian999

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3rpkpvxwo.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3qzivyrjh.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3jlaufjnz.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3eqkvrwdz.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3xtgxvhgf.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3yhabhbvb.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ywuyucqd.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3tkplfsqh.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3lwyqawmb.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3zlfbzkyq.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3ajdkeqmw.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3ufmetxlo.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3lthtssbt.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3dtsmzwpe.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ryofscrm.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3ztzuxlax.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3uoqevorq.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3qdgkqbzr.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3pzfsgsld.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3hljpvaxs.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3oaakjdjy.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3uzhdqjzn.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3kehseatd.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3weugsoom.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3seivsrya.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3kstuhazz.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3ffhhjoaq.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3uhqxogxe.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3lwyrfubj.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3hhujvoqq.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3ihjlzduy.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3ksebelnz.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3gojtbofx.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3cxcmsbde.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3pzhgmzhj.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3onjrwpfs.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3qouyiyst.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ticlzllo.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3ktylnzdq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wywjbfiw.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3rqmpgywp.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3bpjkouwc.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3fejguyos.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3vpwjhles.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3porswvwk.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3kxcnrxon.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3qmyhmklr.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3nmkvsnsl.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3xsnzpiuu.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3sxacmkat.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3lboawuzs.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3gyezagdr.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3yhzpkehm.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3ihcqdidp.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3ceapsgco.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3icqaylrw.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3hsctseto.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3igfnebyc.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3lunggmks.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3opnmyhbt.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3otdfsjhg.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3wpvdffes.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3kthvuvzv.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3qogsfnuw.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3jrbaqrke.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3gkeywhff.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3jlimjwav.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3ctxnvvac.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3chpfesar.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3jpwgfyft.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3znzaogfi.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3wjfpkirl.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3sgxacgsa.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3zyxcxava.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3gguwjxxa.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3zonwmqqp.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3xcjfqski.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3dimjtmic.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3dsgbqhtz.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3zsgplqwe.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3ojugwjpm.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3xajaxevi.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3owpkddnk.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3xsinvjsm.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3hpnkxhuz.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3oneugrxk.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3yzglmsds.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3mbypbjjs.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3dbctdmbb.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3jsmaqjyj.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fsdxbabq.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3riyyvdic.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3bizhovls.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3ttknwnsg.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3mcugkxlg.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3rrfhdagw.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3glmfybwg.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3abuipqje.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3ysiaxpor.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3flfivxsn.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3fsvpesje.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3gwmskvea.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3fpjuadyx.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3jxdgxrpi.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3nhreehqj.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3amepdgcl.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3yabcaoxb.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3eesftegs.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3ctbrbskx.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3ckfsmegc.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3mofnsltw.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3pxvsrmix.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3otylmqis.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3gjhpvubk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uympvkcf.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3otapaaqz.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3vonjmyyd.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3wvnxkzua.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3jwkamfek.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3lptiwees.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3mdrbyvtz.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3huewwcjg.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3jfflitco.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3auccxnwy.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3oyrpbpju.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3icfkefdz.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3ufhspczb.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3sgnrrenj.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3yjjgccsk.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3yilvwtix.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3biyaskyf.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3fmmfvsmc.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3klciwnnb.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3ovbwhakl.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3dmfuubws.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3fkhszafx.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3kfaghoby.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3tsnnmvop.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3meciizep.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3yxxxazug.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3ppnrosru.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3neklailw.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3umajztra.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3zvznniyk.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3yvajmkqt.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3aknzajnp.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3njielknt.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3cccrstid.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3jbjsitgy.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3ibfpgphr.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3xoynkuji.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3daqfqquj.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3cowaoewq.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3hqccxbrq.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3zrpkboij.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3xmvlyztl.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ghzhkerz.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3yfxsiggx.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3czwzsvbd.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3xsjyhfsd.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3hjmxnrda.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3thsqeikc.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3mahciibq.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3cyflpgla.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3iindrclk.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3lhxdgisw.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3kypgctmg.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3cinvnbqz.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3bdsirhbm.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3uwvcibwl.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3fhuflofa.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3mhyihuwz.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3nwhgujlt.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3evibzwde.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3chgvqpha.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3yvjctjnv.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3vwzffmhi.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3zzvqolru.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3zjofjyfh.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3tjfxowss.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3kpdqdtvs.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3aquikrpx.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3mqcnggqo.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3ylnaqhvd.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3byrhfhey.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3edlgubzn.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3njopjywz.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3ydtawted.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3iwsvlwey.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3ijciqjaw.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3nsnjvzkd.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3zvldwzew.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3uuozltlh.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3ohwdhusi.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3pcuiyfik.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3cbfjejhz.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3sqeqioho.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3myhleeog.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3hwfzcdxi.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3swdljxyb.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3xzsdntbx.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3wyetlzdc.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3cstrafrr.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3afxaswag.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3ruajjgul.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3gctddqbh.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3yagoyiwg.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3vafaldlt.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3xajfrcbi.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3xuioorcy.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3yiqynsyh.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3gblxhfsu.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3frxchlga.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3gmaseeqo.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3gqrvaxhy.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3yqdrokhg.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3bvkqxpqy.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3meulwojb.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3oktzutim.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3hcdxqytt.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3tquepxme.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3ttyefklq.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3iiuracpm.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3ytwsnzvs.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3sckezecl.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3fjefpxno.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3skocfhvn.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3whvibray.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3siwobivo.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3lzsoogab.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3gfgrzmhm.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3ubdwxwxp.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3tsdzcyyj.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3usoidhln.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3xrbekvkk.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3phklonrz.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3ukmweyah.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3ztzuhefw.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3ctqxukol.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3ughsbfuf.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3noloxgkv.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3nybostpc.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3cmyxriaw.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3irdzmebe.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3gbvkgmca.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3rpjwqfbx.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3gtmryplq.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3zmsgebrt.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3tmsgvcds.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3hyxbxfqn.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3enlzqhch.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3iatafygx.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3uorvrzeu.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3kdovfhhy.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3aifnpjoi.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3rmpnshli.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3bxtiilsk.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3dfkgtdlh.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3caqjwgur.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3htsifrvp.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3yseijvyw.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3wxnixqxi.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3vdwzfzgs.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3dnuwpuur.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3biaeewup.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3qwkxjgcs.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3xcqyjijt.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3rjaemzah.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3jxtlxrtt.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3ouoruwdn.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3dljgaciv.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3bkhhtthy.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3ohzqpktn.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3iubvogsj.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3ljpnhxmt.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3pbwwgtzm.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3bdmabhhd.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3laeotyju.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3kyuajtqg.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3wlvhrjbl.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3flojyqqf.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3uiywsijp.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3ioitrvkn.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3ggggzvyo.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3zpisfccl.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3rjtjvnxi.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3mhltxwik.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3qfumgyoy.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3xelqpgkr.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3vgovdzsc.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3rbfzqgye.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3remnjllj.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3mqyisysc.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3xvwyppfc.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3dyrulhzg.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3pwpbvlbt.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3ngbqikqt.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3pevoissz.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3xvqfcalv.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3pcqxllht.html


<!-- 参考信息 -->