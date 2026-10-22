代发 wailian999

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2vgoayssn.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2kfiejzuf.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2xkfykffy.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2poktqhbg.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2pawzdvyv.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2ghzejgoc.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2khqlqlbl.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2ysehzdyr.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2ebkbirrl.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2hlxkvbvu.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2mcwxsrre.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2buczzque.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2ejfmfwuh.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2lcflkbxz.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2xzgveznp.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2mnlqsltf.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2fvgyzetx.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2zonzmhsx.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2sxqdyhfy.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2gywrgqkr.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2ikkubojr.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2sxxculpn.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2fayhxmzt.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2xtxuhtei.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2pxemvlpp.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2knmkrmgx.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2yrvztryy.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2uoemetkr.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2twybqdjc.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2shjbehxc.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2qwjxaxbh.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2uyxfgbti.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2oprnxkiy.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2gtwxdzfm.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2mhtafjlq.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2yhpqzlkr.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2ktmzyuac.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2wghziowy.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2bvohepec.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2krdohdhe.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2rkuoqvgv.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2snhlpwfm.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2xxtjyhcv.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2nagapjxe.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2cgpowzer.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yivirxzo.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2dmzdhncq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gdbzgzgs.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2gxmhnytd.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2azusnoti.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2iecxkepa.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2jhmfakwm.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2fqkqlzgu.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2nkyuwfce.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2qwmuhvtu.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2usnmbcit.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2laenpshs.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2kfbaiysy.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2tqpmknfb.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2qqbhdiec.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2dgrfbdus.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2pbqancey.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2pejizksw.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2hntikbuw.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2yewndkwg.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2woqacebr.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2zvoxxghb.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2myvxxddr.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2mohwrjjr.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2zvsfywhb.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ptjlapgg.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2dvcogruz.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2todcyuhs.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2nqtsdanv.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2ffwdbdjj.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2soabnyzb.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2ffyelmgk.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2glgaggvg.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2pxnygccj.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2ijdxlkoy.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2mnxqphjy.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2eqfkrogd.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2qefegcke.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2bnrqgmsi.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2rqegtaur.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2gqfiyhlr.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2lgxsalpi.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2tyhojruw.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2olpesnmk.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2smdkduiu.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2aaaxovuz.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2hefnytwu.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2bvpkgznk.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2llxngauo.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2ohdmsjld.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kipvnydc.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2ugpvkmgh.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vqgojuwd.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2piaqpksb.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2ernsnwpp.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2ffumqcrz.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jngkdnbp.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2prpbyuos.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2yyfvfquk.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2qtrwxexd.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2dffueomc.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2xaexigse.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ukiupqms.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2izheyrdi.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2jkprvxqm.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2bevdgkde.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2drhbajie.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2zwlbcjwm.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2zzysyhju.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2hsnluiwn.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2tobwuhza.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2jmdnpsup.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2kivjfxrv.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2xcybeyfw.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2pnuthmkv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xdnjyisx.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2dbanpytz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2auullijl.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2gtnptfwc.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2gkltaiqi.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2wlltldkj.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2wsakgbex.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2fhejkwrd.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2pmwcubie.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2cqjdxhhn.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2lgjshfvd.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2dodtemdc.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2gnbaxdoc.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2lqbeozyi.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2ustnooqd.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2aqmxyhdr.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2zqicdvky.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2fcfccefp.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2wiuecqyw.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2iitkbtuf.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2depbgrng.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2inftmwhc.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2mcnczfqk.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2hgrmonvf.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2sqdcohym.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2dvyqptsa.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2sjuqdkxv.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2bhgvmeom.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2fikllifc.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2laafyokd.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2efmtqzpd.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2qkbzaolc.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2hdrjxquv.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2tjhexwxd.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2kkaanoyo.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2apnzfxsi.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2fiitoymi.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2phvykhym.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2nnsxhmcs.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2frujrvzg.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2boappesv.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2ulsqyfdy.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2blumzngm.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2fhrebdmh.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2tebfilyn.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2ipneziye.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2nvhrcjkk.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2uuvdrmlt.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2zsshqfhp.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2gaifuifv.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2hatozgxh.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2nmlqcgkh.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2oetobqjg.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2fpdfvgyc.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ywfvuqpk.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2celgicjc.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2dwrieohq.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2mddyaaik.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2epvtcooc.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2sqnnuorl.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2aiiprirj.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2frfnuhqa.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2kqltyugq.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2vaavfdky.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2dxyffjhh.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2rsvxnpbe.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2waeobcxz.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2xlyzuhui.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2snzktxyl.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2tsgrjunm.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2zeaimkhe.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2tpsssgrl.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2nglywpat.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2vsvohytr.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2kfnxkkug.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2gtyrmhmw.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2lfgmawuo.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2dxbmtkwu.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2bmbenmln.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2vgyywdiy.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2fnpvlcpr.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2qpzmqagm.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2vckhflmp.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2wmgosdia.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2aijqvfsq.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2jjwqgfmf.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2ugovcdlr.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2gefvpxei.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2eekozozv.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2xiwcyqxb.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2xlevesni.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2meotoefe.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2psjobgzg.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2gvsffoxt.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2httiiogc.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2sqvytqae.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2ophgijkt.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2riqeceid.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2tlrsbrnu.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2ymjqybzl.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2mguoxsdn.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2ixbgzpzs.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2jindexsc.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2nntlttos.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2avqaxnhh.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2bctnerzd.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2vgtpxnzy.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2gcwntycw.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2irsduksh.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2ilqitljg.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2hypkxbiw.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2ixwanjrf.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2dmeedzsp.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2yhkcexjf.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2muaynscm.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2qmasytxd.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2fcaeppqn.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2mwbucvhy.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2jjwxdkxu.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2bkmygpyf.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2zxvhmngc.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2hqddwfey.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2iimdmsep.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2pyusgtuw.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2bwegwsrr.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2wublxcnr.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2uxyzgmpo.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2zkwenkqb.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2joimrvfq.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2rfliblse.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2lufhiekm.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2hxdquylh.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2aayzkyjx.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2hzdvszxx.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2rpjrybwf.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2ywsfexen.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2tcctqbcm.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2odxbvdem.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2zrmeprul.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2xksmwkag.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2fupspdkc.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2wfkpwwwh.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2wzkziomn.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2yzkchine.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2oxfxqgbe.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2oxtvhgtk.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2gsuahyef.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2ydvfdhix.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2rbnggvzk.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2gmkowyto.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2jfmqrasn.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2ztwldolj.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2bywmtopm.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2qqaagoyk.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2sonklyzg.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2hcwfkouo.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2fzesdqqu.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2flgzjyfi.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2hdhmstwv.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2jquwsimu.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2hqpxpykp.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2indasalg.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2wqmqsffy.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2oimwgowc.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2badbjhgz.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2gfnbxala.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2gqrtkfxl.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2fzvszgfl.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2tnhbfffw.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2isegmkoc.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2ykvynoob.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2ghvvvktb.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2mdvizhyz.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2fushogyy.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2ybxmycml.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2myoqizhb.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2meavkpso.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2evqktyyi.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2qjztvvqr.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2qjshlmwo.html


<!-- 参考信息 -->