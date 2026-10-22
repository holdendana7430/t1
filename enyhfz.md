代发 wailian999

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2qwfpfxgf.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2qapfelvg.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2nesdjvfs.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2nesycbfy.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2vgtdiagu.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2jirkynkk.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2mipandkn.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2ycrwdvgv.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2ebxuoffb.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2ukjxfzbq.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2vnymwvfe.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2gahdxmjp.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2gqodidhz.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2uhtnhfnq.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2svxyjaoh.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2zizmubgp.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2cywlwrlf.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2szatrosd.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2vhzhdzky.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2gzankgmw.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2dujhpjmm.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2tlafluzv.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2hrcudvsc.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2hbcnhppv.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2gedhrxcj.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2qzjrzyza.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2dzemyfss.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2lrnpyngw.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2ckmchtkn.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2vwdxnhbi.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2gbunhqzx.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2oqkvdset.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2qaakmafg.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2ixzhzmec.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2vzgtrfnl.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2cccxbtgg.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2sqbxludt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zpaapjok.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2dslpephi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pfgpfdsg.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2lpxnthsd.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2chqcihqv.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2hnnqlypf.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2vxweyaik.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2ayikrywp.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2hmowjilq.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2idbzklso.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2bnguxpnk.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2dgihygfh.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2tycrholo.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2dleufzbc.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2ghstfjlz.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2gfrjoxex.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2txfyoqxy.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2pvbviqnd.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2bptoesoj.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2yrknbjxs.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2owpcuulu.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2jrcfdgvb.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2pblqrcve.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2wytzjyme.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2vtfcjbwc.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2kztervte.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2kxtljtsb.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2iaddvszw.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2qqqugtqd.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2piyigaqk.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2hlbdmekl.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2ugltoriq.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2kaglaeuw.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2mrylimti.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2lhdhvlhe.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2lorsgtxl.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2lvinunil.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2ywtgvroe.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2hmtqejzd.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2otrgfawe.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2xkqnhxjk.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2nmmqvnal.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2eorgyeke.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2rkxthaes.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2dnstpazb.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2eyliloul.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2efrhesib.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2svbpukpb.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2vaqtvkax.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2saltfgio.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2lizozcqo.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2hypizmxs.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2lmtqzksn.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2qywcvdxr.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2rdxqhyop.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2bdvpigus.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2udiadimr.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2kwcmlmtd.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2xtjubwuu.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2ujxxdqya.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2mgpntmrx.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2lhxyybwp.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2ndbgjoip.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2negmxwtw.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2hnoyqsxk.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2sglkhita.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2gpoafvxs.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2ilhumbjl.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2rlsnwuot.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2ihvztxek.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2qliajwfd.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2aftflwtw.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2ryzmyers.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2lcfmfgul.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2mjnmgkdl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lazvpisu.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2oaxrqknj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qnewqgaz.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2rwrvinte.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2dndpveek.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2bhtkcnuy.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2znoohyxm.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2jdmfkngz.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2gjbcctuo.html

);
来源：http://www.52xcode.cn/Article/details/gt2nydywkrb.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2zwghjjkl.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2gfgddbko.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2wsntrvve.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2fqffrswl.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2rxnaseco.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2bsmcptij.html

);
来源：http://www.52xcode.cn/Article/details/gt2ahiihkel.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2krggawlq.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2voacrosa.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2sdloirll.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2hkkiqsfn.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2esoevwyl.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2ncynpjzu.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2uorshjwp.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2vevxevtg.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2vogjnmrr.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2asudxaug.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2fbwybiox.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2nnqbpank.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2abltgnqy.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2urpuzrvu.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2radinujq.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2mdueigho.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2isrfrufm.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2nblohhyy.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2toufphuy.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2offkskzo.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2dqbzjuao.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2gmfvqtud.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2sktuwmrg.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2zbbyydos.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2ozeoovxb.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2xiigaedo.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2sorgtdtj.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2khrukgoy.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2uyojopxr.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2jkrssngr.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2whwtmlsh.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2wjpmuidg.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2kpntatzw.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2nqcvnnba.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2dzwdwxln.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2scidmlfo.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2athhbqez.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2lboasahv.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2izgmylpa.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2fxbzapml.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2xlmewnht.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2ajreovpn.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2qfznyrjv.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2jryfpxzt.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2gaeqtgjf.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2nyayoolh.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2pcwzgwij.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2azuupgfh.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2cfqhmgjv.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2oeiaqlgi.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2lpaajaez.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2oanvahbo.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2embepbfd.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2joypzczd.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2bgtqqexc.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2tpjmlwgk.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2oqdgpxjt.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2tttymomd.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2uxtjjkcf.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2spnbfmjt.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2xpjvcdkv.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2ktrosdxr.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2ttxetzyd.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2rtcbkdle.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2xwwfradq.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2czppeozv.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2fmkgdayr.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2tfmfkccr.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2dppphyie.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2sojhiuvq.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2ionnafoy.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2mmmfplom.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2chzfpmif.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2cmupnrxp.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2xvwpvxdl.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2kivjnhuq.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2nsnagthv.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2seyfrtio.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2qfqqysap.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2ifamhrei.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2jnpjwahv.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2mbppatuw.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2kcvnucrc.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2znvqrloy.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2agucbvwb.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2imlwvjkl.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2lxgvldkr.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2nlduqiss.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2eglurrnx.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2xrcboopu.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2dybbtdah.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2iebqrvds.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2dsbggblj.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2mersypmk.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2wvfgfznu.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2vdrgwljy.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2nstyeibt.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2tkvhkaps.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2xermzqpw.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2qcdjawts.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2uqgjgzdt.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2fdqanrlt.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2gbwmjrkm.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2ikryoehr.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2haplrqgl.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2dhdsfdxe.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2dxryfddz.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2wygphqbx.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2aiwdmovp.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2skpxqdby.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2etjyztzj.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2azwngcbj.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2eyvjalkk.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2hkuhcuzp.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2izyqltdi.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2qbjktbwk.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2nduzopeb.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2szapqjcb.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2nphkfcfe.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2blajanpj.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2adugyfjp.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2sqejecoj.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2camhuleh.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2ialbijlj.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2imoaqgxs.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2eipueiqt.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2uskpkdba.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2gvcbwvwf.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2nglszspg.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2ksiqovhb.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2intjzhar.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2dhuybmhk.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2mxjpeviw.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2zkqwgzln.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2hqbgtahl.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2zepuycqy.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2tmjcwrxp.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2rhgkmewo.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2wwhvkurc.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2zvvzyrxb.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2igrwmvta.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2afsamvzr.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2citppmdy.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2gikujaqg.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2kipvunxe.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2owpyoepq.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2jkqsnfpx.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2ixdcleus.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2okktxcdr.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2mwwunmly.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2afbbelzr.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ncljxehq.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2tvryllza.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2spsjpwbg.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2dzrllcbs.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2tsxfoxkx.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2iiwceysg.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2mrkpniel.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2ybkyowgc.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2mrnrrwbv.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2sdqnmuxy.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2wmzjijdz.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2nfjquqca.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2tydiyylp.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2yqpqjrxr.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2ipxunyhi.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2qzogvofv.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2wghyrimr.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2pknuyrxl.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2bbxyyzdp.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ynswmcnz.html


<!-- 参考信息 -->