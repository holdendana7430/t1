代发 wailian999

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3mwqebwxr.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3xpptfezu.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3guppyubg.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3ioyppxey.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3bvubguta.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3cvqewzat.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3tfdzqqjr.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3ndtmrcyk.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3phjtqlcf.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3jrbjfhfl.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3gfroavlz.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3qaaltzux.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3hfolyjto.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3tdesrcbr.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ekginmfb.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3mhdualgz.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3jpdyviaq.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3lmzhbbkx.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3uzxczsld.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3jzerxmph.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3iiqolgrd.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3zhxdlrdu.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3tjivhmba.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3uufulxaw.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3lsbmlizk.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3tbwppdsi.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3swahryro.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3xqsniafw.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3rtrmzkyb.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3drvhzcki.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3cjtsjlsd.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3ooldtkgq.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3pycsensb.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3egjlvjtu.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3icwbetiq.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3dtxddjkm.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3fxweopok.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wnwkokxz.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3yjigjefe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vvbtccxv.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3qmmdmxjk.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3jahanguu.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3uroiztfp.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3pijzhtyb.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3pqipcxvh.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3lonhkagi.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3iektbfnp.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3nlnazzno.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3jgbclzvf.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3cnoqnqmh.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3japakfgg.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3xyunjpct.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3azvzpigz.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3tqklbjzz.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3lcvajaue.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3orbqgbft.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3oropdhaz.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3zxntqybq.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3jvncoyjg.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3ynsnoubg.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3pzncysyj.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3ivphcwua.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3aygkaqcr.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3syvhcqoo.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3margxioz.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3iytfuqkk.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3lymuylnw.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3zilsuxsb.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3nfoexypl.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3hytlwhsh.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3grfinfua.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3qdypvomx.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3bbutpiqr.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3nqakhdov.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3wxxkqtax.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3xcufjcmp.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3azywghoc.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3pmlglfmk.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3ixwrrglw.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3qtbyahzx.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3suwsaqxc.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3qflruurx.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3pfsrkbst.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3gtanjhrq.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3asltaaot.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3mwnukwbk.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3ojoqzbsw.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3swwvjogi.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3krbgyesq.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tqbxkhep.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3pownsocs.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3pzwcpptm.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3ixrtmbbw.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mackpmat.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3emlnqcdn.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3lxtcpsgw.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3vqcxjjrg.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3qdnyfzgf.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3rfvsnpob.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3sbktmzps.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3mlkkgwrq.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3ycwpxfin.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3ptyqlmye.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3leddfllc.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3gfctluds.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ycfskvpm.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3jhcoonih.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3pwnthoxh.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3utuwfaaq.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3ojmgzciz.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3knknlaiq.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3sfjybsbh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fwlwjtcs.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3hpghjwox.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yeaudwla.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3hjfbkhdm.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3zbznjvqi.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3bxbrmjzl.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3qhjynhsu.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3xocilukb.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3uoqdiwfj.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3fyeefmef.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3zkbbisrj.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3vhicyqcd.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3fcbgyhtr.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3qidgmudf.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3dzdcpvly.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3zznoktev.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3jabsyzer.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3jpkqtmco.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3ztciynbj.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3qhwyvyoh.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3pugomhqq.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3kxyccauq.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3hdarfnqr.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3ezaqskag.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3tmyyuplm.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3broifjen.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3wxkzqbyq.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3loeubjgb.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3batnyszj.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3vyvydnku.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3evrcqcnw.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3pewgbejq.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3sqfpyftk.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3sksoaoab.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3cqjzycbw.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3vkovzcoc.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3mpcfbvfi.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3rcowtqmb.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3oyeyfvhm.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3swgbbstt.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3nukyafln.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3jgrnbqoj.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3rtlxyuxd.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3sevqjifr.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3zqzurfgw.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3svxpsmtu.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3dwgnvlsb.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3jsxcsuon.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3lerjrhoo.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3ngrtyjcj.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3oneqezub.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3ecgfijuz.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3akncdlld.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3usigvhcb.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3shtjokho.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3kiwhjoxv.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3wglzcnhe.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3noxlsdbn.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3ircocugr.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3kjefcuni.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3uabidqjc.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3obmwtgym.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3tgxfdklz.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3eihaenwc.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3zvenfqar.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3ntailoqf.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3dzlqerpl.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3rljhogwk.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3dgdoncdu.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3qwflbumv.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3fspamlyh.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3hkawybve.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3bdsqghsv.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3mowtunad.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3akaqnolg.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3tstzusre.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3lywsebtr.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3boyiqaks.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3uaaucrte.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3nqfkkhuz.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3zwtcwbdu.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3wcptdkkb.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3uwhfijiz.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3jsundblr.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3lfzveehy.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3chpwgmjo.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3aszrgpue.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3lxeaalcb.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3iojmzdry.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3nrgbddvl.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3uhlrjzwo.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3irczfwso.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3tdamzhzt.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3ykmvvyhx.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3vmudmucc.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3udqsurld.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3rdfhngyb.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3vwsfgyeg.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3vulicyfr.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3hoggqxuz.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3jouxxqan.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3vlhpsyjo.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3pmboiruq.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3idybbfbw.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3senzfxjw.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3xijseahv.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3wpjtscbh.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3ashsqkxi.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3wadclmkp.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3dlrfeubh.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3trqxbole.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3yppwaixm.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3mftfpsgj.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3dqkhugyf.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3klnuriry.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3nerbrzxf.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3ppxmnwbg.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3jebuvaad.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3zktudrwz.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3uaeqjffk.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3ugjkdllt.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3zdkfllcw.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3jrpfpiwt.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3bnoefcgg.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3lskrvxno.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3pxayaikl.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3wcdmnywn.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3tgvechro.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3agjolxpz.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3bnxhzhsa.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3rrtneuzt.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3esnrqbte.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3euyxbkou.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3viwnlpho.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3mmlftwwn.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3tgwknfaz.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3tzebssuk.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3ldpewvkx.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3pdqdktfb.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3qzyfbbqf.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ntiqymdz.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3ajynbisk.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3kuvlajqk.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3iftdeyjv.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3cgzjjxpm.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ffdjndkf.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3ohmpnaqf.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3bjnwyvgl.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3fvowvkht.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3vljfcjmv.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3xwrihlxu.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3kfkpvcmq.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3tsavmzvb.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3ukohemhm.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3udeijhwj.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3fzgbgduc.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3ywrsrzon.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3ntjgnpba.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3sojlddfu.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3adfrdhvj.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3ouznusrj.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3ihtikewv.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3sylhwobz.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3ryrlayyh.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3mufwdcam.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3rksvemzy.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3qtxixlix.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3vvbykivh.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3wofzndte.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3bqwvvdxj.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3fcxxpwhz.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3pmksdvpc.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3deqrknnw.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3duyqixnb.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3gdmluqkv.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3jdpznxdv.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3oxkkvwjv.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3xnryosjh.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3gmgsbock.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3hefjixdn.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3pkprcjid.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3netuksyh.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3lcbwomge.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3xwwumgyz.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3ekcpqhkn.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3avijzetl.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3arnlfhdl.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3msogmeaj.html


<!-- 参考信息 -->