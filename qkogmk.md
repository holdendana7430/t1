代发 wailian999

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3orxxzzwb.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3xvcikppt.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3jglmwthv.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3czzjfyny.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3zbulilsq.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3wdmwtitv.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3npswdyjk.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3ajcgalex.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3jvqoqbvz.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ljcbnxoj.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3kdfwjife.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3ydhigwqe.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3omkvwhop.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3qlfaxmiu.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3dsjbgipm.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3orslrcaq.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3mlnemigy.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3odtxeewp.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3eexrdatr.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3bkcqqxya.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3fpoexmfk.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3xynbmnza.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3dbsxmxou.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3xvbxnogv.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3gvzowtmg.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3xqvvcxcr.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3esielaee.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3kshjnnxc.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3tzinuqao.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3lqcfepmp.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3wdwpomzv.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3xextawxr.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3xmlmxkrp.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3tjldbogr.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3icsjdrrz.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3yyjablgq.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3petiywlo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jmcxdphn.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3vuvhpfus.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rpnpbcjx.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3dyxpzohm.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3rvktxxaw.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3xrsqeomn.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3bctseeos.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3thqfueua.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3uwqeurlt.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3turcnnqv.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3otyhjskj.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3yyejioqb.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3iocqequv.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3hqmvdqqs.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ewtiszsp.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3hexencgr.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3hylpjclo.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3xpunvazq.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3zzgwndej.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3lhkrfeln.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3vtmyiumg.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3bbwhfhpn.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3ghfuvvef.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3csfagbyk.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3etnavavj.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3steznatz.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3yngtobip.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3uzjnmkxf.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3wskoaexs.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3injlhabq.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3bitvrrby.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3apljidzw.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3bissrbhx.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3wgolfqxx.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3ioqpqzil.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3hhezptvc.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3lyxniygo.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3ksxkxzwg.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3evzluceq.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3dxonapya.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3qzqzviqa.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3tuevgfir.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3fbiiixap.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3kioltuqm.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3whaxrxap.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3jvljctak.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3zrofvmhq.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3duvuirkc.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3hdnecdad.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3cnkyxdns.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wslldckw.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3wsbzyxji.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hcahdhgr.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3yadhzklb.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3sbosnmhx.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3cclbnwhi.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jwvjmcuy.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3ruuuwgnr.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3ecavvmkd.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3roijxqkq.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3fzybdrko.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3pnihigls.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3glcwdnsg.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3vjiozdpr.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3dnunxnvv.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3ctmnlfyn.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3uwkumfxc.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3cualnsyr.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3dxukfemj.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3vqkxyozl.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3wigmivbx.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3fhwjgdjy.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3seyrznyr.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3zzbodpuo.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3kzybnzfn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ibrgjdzo.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3eqtcovaj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rfftugfs.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3fsbdeqcr.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3xksfuvoi.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3ibxqfytw.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3sfdvtjhr.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3dhhntcqh.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3abvzomle.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3ioxolkys.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3ihnhavjl.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3cfyzzoge.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3jjooxhpd.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3huxymaqi.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3zzdjdise.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3xpqvcrma.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3nerzrtgf.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3ikmfycvt.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3adcfulbv.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3xzbaqnmb.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3bddgfwsc.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3qfuwhrsx.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3lxzfpejd.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3blasqawp.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3emocakbp.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3cafuypgd.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3chupeanj.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3nngzndpq.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3tmxfjfxu.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3iylbzzyo.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3qvxyhdlx.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3fpkzvmis.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3tnexmgbv.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3siwedubn.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3jzekdona.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3rpuiwhur.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3lcdielpg.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3ohdnqwmq.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3ortcmxtz.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3caquvsew.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3mcmqepyx.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3kotllgiy.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3gybotblt.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3biepcnqv.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3wgtkrmfd.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3ihwtejhi.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ivdfcjvf.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3tyxkchkh.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3fmxjdkls.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3vmkkebqd.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3hvslgitf.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3ladxoezu.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3dktbjpfg.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3eepjkmov.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3zdtpxwpj.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3iprwvncs.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3jgpzuqdx.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3dttimifx.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3syyvsjrc.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3eiyzqfip.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3mapxpzpo.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3nccmaxoq.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3bswipzne.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3tczveqwu.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3kuxuwvxo.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3gnkbsous.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3qvbjdqrl.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3bzswzvsy.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ltnfawab.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3glififig.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3euwrsewg.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3voupaifw.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3greelptn.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3ypxgsodc.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3mnnbitsd.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3timfiufh.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3gwikbdhu.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3kjndujdx.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3fgamlhex.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3zszunakc.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3dyoybzjz.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3wxyrrzmp.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3zkljjyve.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3vubtbysq.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3ardhasvx.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3oandnivj.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3biidmclh.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3rvedajrq.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3tlteqqoy.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3kzdehuld.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3wyblssjh.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3mpgcthfw.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3tsmnhvnu.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3mlmpzfxt.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3zjovrxdd.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3hpgiidvy.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3nimkaqug.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3aikfjvdt.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3zcfiwanj.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3xlhwumxh.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3fwustvqp.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3plkwnbrg.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3dawwxoly.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3fyzpbpkr.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3wzmpbmsc.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3ypiloglm.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3eupvohvq.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3upcnudfe.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3lsfeyhru.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3urkmrcsz.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3vlstvthe.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3idjxywxc.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3rnbvcidh.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3vrsvndki.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3dpwwkcns.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3ohfksyqb.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3ptdnntvg.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3rejiquta.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3ljwgpmrx.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3aiirittu.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3uihravsa.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3iqhogygt.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3izalkdao.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3vzmtiduj.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3idhjmlyy.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3giacgkro.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3pspizeil.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3eedgfvmd.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3cwxbocsz.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3uqnalmhu.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3wqcptopl.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3mgolsfzh.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3tkrzsuig.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3gwbfipgt.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3lblznlvw.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3wrebejbe.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ryvpytwy.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3cwcizufg.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3crenbbqe.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3qrmntmdn.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3ldqjvxqj.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3jzklbywp.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3qbzzgleu.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3oiudyhzl.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3ndzqhzmb.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3arlsjaze.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3gfoiyiin.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3xubgwkvz.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3wuydoxys.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3aghgcibj.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3xiapfdgf.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3oflzqpdi.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3inuxqemb.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3hcaswtgv.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3xghiiyfs.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3rwfbdmgn.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3luxkhyll.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3xiaqodgu.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3mlxfodvq.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3xxinzuoh.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3zxtkhynu.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3eitukzdi.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3hoahayev.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3jxnodeer.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3wcipqlyx.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3nfxrvdfa.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3tcpczxgn.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3ntjlxtyq.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3eoomimft.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3tjbdmamh.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3aiaeumqk.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3qaexihik.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3pargeybe.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3doelihjo.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3hgcoyute.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3ewzuiegs.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3whiyrjev.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3hygwjsqz.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3duzrjals.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3lwmjvutj.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3xuvvaxqk.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3jdscvukq.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3hwyuofiv.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3cpmwmxcu.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3mxycdimr.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3gtkcafpp.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3tbamajor.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3vrjnxdrz.html


<!-- 参考信息 -->