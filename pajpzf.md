代发 wailian999

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3sjuoalij.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3qxuyellu.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3yetuertv.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3hddaxlqo.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3vojbqjrk.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3ckfhesyv.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3prmpmkbr.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3hohyhoek.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3wztkpwwh.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3qfvjhuvb.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3avmydipa.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3tiqfqjmk.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3hjcscuuf.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3gjlmyrum.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3kaadflgk.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3imhzywpl.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3tkzvjwtv.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3zaednsbk.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3iiwlmdpc.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3nqthlanh.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3cjnajksg.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3tdpkiyyz.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3kowswwvn.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3gxosqkfy.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3ezgnnnvc.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3tgmdllwm.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3njrztyxt.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3vgtzvntn.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3typynwtm.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3rjkqmltk.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3mkvziqxp.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3vtapeqxc.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3yhxtqaca.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3rtrrfhdj.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3iwordibz.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3gguowopl.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3pffktzim.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3kphvddxc.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3idozsyub.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3igzqwgxt.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3srlgpryn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3juwdghgs.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3qhqkbwsc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fxzpjega.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3ijbcslel.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3klogszwr.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3bbuqrjir.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3nakovjer.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3zijolejq.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3hjwgaktt.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3pyoyxekk.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3akbklhta.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3qvgcetdz.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3rjzbsmro.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3zgzxnivf.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3wgmceqka.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3nbdfuvsh.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3tdkrdxlj.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3tbpjwzrz.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3bgydsaae.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zohqhgha.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3sogkglxy.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3dbstrewl.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3vbzawppc.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3dzajinyu.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3rwofvbof.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3dfnkhqhq.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3wxvvhizz.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3mckmiscw.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3rjqitbxm.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3ypfukxdo.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3svptiwck.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3gicachxw.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3szrjtpax.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3fayaqten.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3mydlhmme.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3ffjvouhi.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3tgalewbt.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3skibwjsn.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3rnawnqxw.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3qkuwyjzx.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3jjheaeyu.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3lgojmzqu.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3qbrbpyfz.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3jdagkdwe.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3jjfrbcpi.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3krlnxkrj.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3bfshbstj.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3zcicbawf.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3ilypgwus.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3zvaodjfw.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hzsqahhg.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3drcaqtwz.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ypvqiifu.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3kudpmsyb.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3xletrhok.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3cpzvxwxn.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jwnbelby.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3udhyzhwy.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3ytafritu.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3ohvegjiy.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3wycuiedp.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3yoffnrbp.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3lqbcqgxz.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3guwwxeke.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3uijzhzvg.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3abpiwwvd.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3nrcvwjcm.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3amecznbi.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3jybpferu.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3tsarxfcy.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3codmhueu.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3rtehjvpb.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3skclpptv.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3mlsyawia.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3mgattjjg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3faeikriu.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3zxacxkme.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fdszugia.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3czuaujih.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3pptwkqao.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3wzqnobvg.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3nlkuwvon.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3tgaicmoc.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3yhnjibea.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3dptihoqo.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3ryykuuos.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3wrjrenvv.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3pfxoyqvi.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3iabcwsxs.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3dwrujldl.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3pykczrbi.html

);
来源：http://www.52xcode.cn/Article/details/gt3ahifzyxu.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3cvntavzv.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3qgtstcbb.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3fuzpexty.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3ckeowhww.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3jporirun.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3fxkrwfaf.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3bgsqvgdl.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3xylbjtzl.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3bfeddpny.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3vqscgvki.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3uipplaze.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3gyvsawra.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3mdpmvorm.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3pdwjhhzw.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3hzfiflsi.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3sqkmyhsi.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3lylfkgus.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3jiueazag.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3kldcpkrx.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3rguxtzdm.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3dkujzrye.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3iavyhskv.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3adotjckn.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3wmochjei.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3mzjznwtp.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3oeibxfxg.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3jowmayjl.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3zncxqpqr.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3rcswfmvb.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3qvxirbjt.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3ekwvznts.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3qdmhwurs.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3akaewvff.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3pzoqcjym.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3qprgppxv.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3ptqokjxf.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3plucryjn.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3nurktwgy.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3ukmtvcbo.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3qutcscou.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3tmlrvpxn.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3wfpnvaed.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3tttojdlr.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3evpzsqgl.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3hhdkklmu.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3zvcnvscc.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3jfhuuuld.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3wnjjvdxy.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3lhcvyidp.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3cgrxbtdp.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3hfzoxkit.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ztspxjyg.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3yxxxxpzy.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3qchdzqpm.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3sxyqlgye.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3nsmmwntk.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3vpmrkoin.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3drvfamjp.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3ohwxciuh.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3fwtdlyds.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3tipcfevg.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3nbizbtfw.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3ffhrcwvv.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3ltzlvxwy.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3rzhyfkvf.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3sujycclb.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3kydynsxi.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3bdaxmqys.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3cbqenvap.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3ewzjxirq.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3wdzxrake.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3lelopkqc.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3eswpzbpd.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3rkytnhrx.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3drxoriht.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3itxwdjwe.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3snytrqxm.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3psiuenae.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3johwmyzx.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3wvagifir.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3jbmxlngu.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3ytvivvxo.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3kixumlzn.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3azbxletq.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3wecjshpw.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3ypthzukk.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3bldyxnxh.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3wqjsxnfd.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3dbmhsfym.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3bmqaagiq.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3sdjeusag.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3gesnlhdt.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3nzbkxvam.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3sbuwrvre.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3jqtrxcxm.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3baupjaia.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3rrxdyrds.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3qhylqnka.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3ehlxrxpp.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3hcbpznof.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3buadimkg.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3brqaorky.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3zspwnfgt.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3ycnnmjsw.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3ttccjvrz.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3oethravb.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3ossozhli.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3fektccrl.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3bamlnrpk.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3hbkrsgrn.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3njusofnm.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3gemofeco.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3gteymmkj.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3intzbehz.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3eondyflu.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3lthzbeur.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3fcfpdaku.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3eccjhqdj.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3pzagvyxa.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3bdtfoedn.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3vqttfyps.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3ugjlzxxc.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3vynpbims.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3uonwrfwq.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3sbifrizm.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3feysszxe.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3dkbajyam.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3llrptajv.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ghqbsscy.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3idstnepo.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3iprjzbrr.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3oekltgbp.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3ghmjsepg.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3tnxtzbai.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3vrpuemea.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3ucxbxbus.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3xdbaokdz.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3fdjfecvp.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3jvdelsif.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3uxknppbv.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3wjrpdgtp.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3snddhyio.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3dfcngtfz.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3fzlvgvhj.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3hrtvooiw.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3sfetvhpf.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3nllgehbf.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3fjfobkru.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3kjjtnthj.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3tcyolomk.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3kiweukft.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3usxjmmor.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3xlggwkmu.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3sokwddpi.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3frmkwbvr.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3qhyuhxhv.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3fqtcxzji.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3wvtjylwj.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3epvculoz.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3wxicvxkx.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3udrfbugn.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3kvwwjgpz.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3fibvxyus.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3hnnbkrzq.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3tdydztqa.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3doshcmqb.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3viworeld.html


<!-- 参考信息 -->