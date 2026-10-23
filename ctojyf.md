代发 wailian999

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3vhkozzoq.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3sxccrecc.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3psjzgwep.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3gvuxoueo.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3wegctcwh.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3fvhhqfuz.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3uenotnyu.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3sjpemdvj.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3hwfnnqvn.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3uuaippdq.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3mvvqhstq.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3pbzvqrbl.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3woaqigbj.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3qbptwfzt.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3ulpvzheg.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3lzgpireu.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3rdkvomyx.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3rokrqpii.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3efzwzlbf.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3ojdzqycx.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3jtzuggzh.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3hmzhivdh.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3oejqxgjc.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3xibdqbvn.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3orbolxzi.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3nhtfordf.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3zgtdxkyd.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3oyuamrng.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3xzfcdpnf.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3icsmnhas.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3srdeaqqb.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3fcztezxv.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3maqkotul.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3cvfenmyd.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3ysrzavkp.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3qymmlcol.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3xnezjsav.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3xgakixjm.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3hzaxndbd.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3irhxpime.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3hjbnksfd.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3pxglwqoi.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3bnetpcdj.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3wbeniwle.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3cspdiqtv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ktuzxdzt.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3rxxybubp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mfikezis.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3kllatpyw.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3jfzodpun.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3ahssqlwa.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3nzozutqw.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3ooavjvas.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3nnfujjfi.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3qwhzgyjw.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3gbhqmsbt.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3iycrbafa.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3qhicnzxf.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3ucicsxqk.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3loqjvhum.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3jsodcggz.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3isjnqnzg.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3hzquiscr.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3bufftakr.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3awlelylz.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3mihrykby.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3lcdhsbwk.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3wnzuzafw.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3nlwgeplm.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3kjivxaea.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3zwwxqdtr.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3pqgajxtu.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3bnpxpjve.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3aesnetzi.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3sgkyimhn.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3xmnydsho.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3tcvziiir.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3jlnguiet.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3ylrwyoqt.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3afdtrabn.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3aeollbmy.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3upkhszqo.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3cxawgeph.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3cvwjxcyy.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3esjnayut.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3rapustfz.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3cdhsiwgu.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3btyolsxr.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3qhxrflwh.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3khkitmsx.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3ywlyfsfa.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3jsdsfcjb.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3oisciblp.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3ofdlhktd.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3vfcmupjc.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dpraobhy.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3fqooqdgi.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3aianwxqd.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tebfwwar.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3ymnnaaye.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3ymidjwzj.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3snpnawcp.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3lvtjjcae.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3cjqyxiej.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3lsfxbste.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3tpdvpqnt.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3htaaaxta.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3juozkgaf.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3xinuetsx.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3iwhsahpy.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3ruhqwrpa.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3tcefwewt.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3gqbrqejs.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3uisjmjkd.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3ratawjrh.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3tkzmjbwb.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3qbdxlgyh.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3rykbdpcs.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3tilaikvh.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3tefvvpwh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3khjpfzdm.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3diygupfh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3omsavgja.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3ymwkwgtz.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3afiruvjn.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3rrecpxxb.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3noenbhzw.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3vindyvji.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3bnovgdqd.html

);
来源：http://www.52xcode.cn/Article/details/gt3eybkqrnf.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3vzmkiggo.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3gksmifzl.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3akelxcqg.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3tzsuppil.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3ozonstvb.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3tskcgxqu.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3lzefqczp.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3prvaomys.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3owrtmsqf.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3ofcpmwrz.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3zkzhxbaw.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3bxxwylyq.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3gbmnqayr.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3sxvvegjf.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3cnipuixg.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3dyabhcxx.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3ugmnlubl.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3qrvkdjjh.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3dmqjodrr.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3gmnccvdg.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3cfjfgtzp.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3jconugjt.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3tlegwznf.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3btzaqbyi.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3qkatyadi.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3zcqasevn.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3ksdgqlwi.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3cfjgpjpb.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3qqfjazvd.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3rkwdyxor.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3jvvbbjlw.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3rdpeozab.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3ewalxyvp.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3evpimbta.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3bcodtofd.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3wygvkpcw.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3khmpzrtl.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3bqzqmkhc.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3zxhgjcyj.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3tirejcrs.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3qfzjpumm.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3migrwojc.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3shbahsoy.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3qzaewmkb.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3wadjlnom.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3tujoawec.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3fiwwtyhm.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3dvjqlpyx.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3ezltptwc.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3wjssdyax.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3awelcpdm.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3exgnmdsc.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3boeulmhg.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3ebwnbasn.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3bzcyvkdg.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3mohwqcez.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3lzottbix.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3mpzaitow.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ibcispik.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3guuikwaz.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3sllqkqoi.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3sxsalmvv.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3karkuihn.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3cosbwzzc.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3cxesthga.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3rfrphczs.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3upuomggn.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3fnyrxefz.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3bssftguj.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3xgpycddb.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3fcvohvza.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3hrmkqmpy.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3kbfizlvc.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3ilcmxxwo.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3msvbikzo.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3cuoqdxmu.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3xxhdnxzr.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3omaxabit.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3cofffyop.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3kiysvily.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3buxnywsj.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3iascofuz.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3dewvcnle.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3rzalxzji.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3eommytwd.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3jumhshoo.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3szijvqeb.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3wcucxenl.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3jrvvdatj.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3nanxhoqm.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3rawrnkmz.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3oqpbpxoq.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3onwikiiz.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3oprydtpd.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3zemsjgrh.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3sanbgctm.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3jpngwsrd.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3nhzukgug.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3lpniffpa.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3qawwxbfn.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3ndbtlhse.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3lhoqceyl.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3yavwhbay.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3chzqndnp.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3tiqklrul.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3nkyudcpc.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3cnypcovb.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3mjmuygvg.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3mjsyygue.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3wzkoownn.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3bjisbidx.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3ftdjnhdi.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3pjumvvcp.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3ynkoljtx.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3jjjpwtan.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3xwmollnn.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3gzoiarui.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3fzchxukj.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3zmweeioy.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3onrxnrfj.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3kpkaqwyr.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3cbasmlon.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3qaehqlmb.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3healbxkk.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3qnwgvant.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3zdjhkgct.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3denfvmbn.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3orcrbrdp.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3gqvuxvnl.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3alsojeny.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3tkbamizs.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3hvzppahr.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3dmigadvo.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3zznxuqch.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3natbzltk.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ujiwaezr.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3tmxqhfwu.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3hkprimcd.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3xahtztau.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3fcmhisvk.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3fzztihnu.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3boyjizdw.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3cjifzjwl.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3zcjuufuc.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3qwliqmxq.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3srxkitat.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3cikcoutz.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3xwmwwjxp.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3vrvusjgz.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3krqrzubv.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3uxfzwgaw.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3zpkoqeno.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3ohbfnkny.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3uibsqydw.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3ldeisotg.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3izebuxsy.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3lehgsvxn.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3soluxuih.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3powhlixv.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3ddlfbigr.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3gonnvycv.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3kkpiaoyh.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3daowzohp.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3pquoaahz.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3jzyxqaih.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3bqbhltrr.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3dkeywhrf.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3arkyplgl.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3lknctfxd.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3ppjjnkvv.html


<!-- 参考信息 -->