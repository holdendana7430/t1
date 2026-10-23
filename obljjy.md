代发 wailian999

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3rezhnjvn.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3ubrprezc.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3bgzjtgnn.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3lcsyyvqh.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3ecbyuibd.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3kfbodstk.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3egcrrekb.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3uffsrsfw.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3meimezpt.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3dcwtnmbp.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3apebvvie.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3twlselil.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3xypvodms.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3avyhoesf.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3jtazzejn.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3gedqexzu.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3mwvewxpw.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3fpuhpzlp.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3fvmlofzk.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3uuqpidjz.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3iltsamgl.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3qcgppygs.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3itiuaudm.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3qrkzxbrt.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3zrwnucbg.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3glgbsbhw.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3czenrufg.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3ufsvdbju.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3iiighbyi.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3wlgjjoza.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3prixqhgw.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3igucrval.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3xhfgjtca.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3jfrbcagj.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3qxksuafv.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3fuznvbtc.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3kxivujeh.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3uvaohnvb.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3rcmhvxwn.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3mpnrbscz.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3oininfiu.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3lzuorehe.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3oeudzxui.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3tkxyzgoo.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3otbddiez.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3wbllemqa.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3abghdmxe.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3awimoela.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3nxstoszs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3eqpnunsb.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3ffjqpanf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3isfnpkrd.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3qbjbinfu.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3mhmyidnf.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3dqulnsux.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3jcunvjfu.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3ljuqdedo.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3pwlxkhpt.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3ikcpgfhz.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3txsatvfj.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3rwdartnk.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3biomsswm.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3evreegde.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3mefuylbx.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3necbdzsl.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3kinsnkiw.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3llfzcedg.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3wlfztxwc.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3onxiaefr.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3bkmypjhu.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3mpvbdeie.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3vsfkrnww.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3rbmrrfsr.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3sydwzzak.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3qzvcpjzx.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3yzvnbvcd.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3emmrjycu.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3upklbqit.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3dvxiwvpe.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3njfimcds.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3qjosfius.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3wgcbxuks.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3htjbbfhh.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3edhslxju.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3pbngitou.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3svqjkqku.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3hyqlpuhr.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3tmrpitlb.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3ojryqohq.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3rupumjhx.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3ndtqqtag.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3ocmwxiob.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3dfnjcewd.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3eaziyyib.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3thsnmlrg.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3mtegxdqp.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3inontjhd.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3cjygzvjd.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3tasiszov.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3cfirnyda.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3qhnfpeto.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3irlfdosi.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3puwbhklk.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3rrlatzmw.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3qlawhlit.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qtauhsfu.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3kadphldm.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3gjnrzdtu.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3ibohdsju.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3tresqhfp.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3ohhcmjfm.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3gfbgfazi.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3jhfbjaui.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3pwdrhvwj.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3qxqqdfid.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3jjacsvra.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3toovhtci.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3zrqjjnbg.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3dclpvjpo.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3rhewchzg.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3rnyhqfic.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3sdumxdny.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3hjkukvmj.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3onbyubkc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sdhaczyj.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3utgbxpxl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wqxmwznr.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3nwsgqzrh.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3vxrwpkmu.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3sjyiesoo.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3rrmwwjxc.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3njefqcjp.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3xrdmapzn.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3iuedsimx.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3vgvijufj.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3hkxgwmaw.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3cuvzbikz.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3zpodjugi.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3fselocyn.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3sagusbli.html

);
来源：http://www.52xcode.cn/Article/details/gt3fchikzto.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3xtctjowc.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3orxjrfre.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3dnogpayi.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3fetryttx.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3xoesdpjg.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3nsrbxxdm.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3mdchgarn.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3ppilxmee.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3spqmelmn.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3yfpgdmnm.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3qjwtgivh.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3kjdhxhar.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3gzbvxkjz.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3ztllhzxt.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3agvsqnze.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3naypnwha.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3gkpbbjjx.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3dxdzsgbl.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3zlatwzkr.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3xusvdcsb.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3mzbxuuez.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3jiansnma.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3cvdwdgin.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3pamdfgpb.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3omldhoce.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3psqvahtn.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3qifywkux.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3xtcfachn.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3klrfhmih.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3omocvsnm.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3udmfeycm.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3vhituzrk.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3szqrqvuv.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3ykamqnys.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3aypfmulw.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3rodxcmsm.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3oyogoivy.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3jjowxrmj.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3fyrgidue.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3ihymjjgj.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3ebfklvpk.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3okxssnor.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3pgfhdgoi.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3trdwfhav.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3npcqfyng.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3hjmquqbk.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3wiiqcdtn.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3cdsspxdn.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3nwzdxehb.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3khwugozp.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3uskutuyy.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3xiycehhh.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3hidfanxi.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3gukkvfqs.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3ocinzgor.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3sqiflzwb.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3fbmhyrhy.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3hksiskhv.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3iwqdkiyg.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3cagidzsc.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3tvvwmblp.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3cjrgvckh.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3ublathyz.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3airbfcpp.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3nasnsqvf.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3atehuzdt.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3cfzifgyh.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3ujxpjndi.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3dbrswzzx.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3mataxwto.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3ymrmzqxg.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3dolcylmf.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3dwokckmz.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3cpdykwxk.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3mrvllbbf.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3ykpnwfyq.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3ghouwzku.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3iobcuxto.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3trcidssk.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3qhyocoxw.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3bzyrdjlu.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3xgyflnjt.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3buezwref.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3djstkmcg.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3qfppmyhw.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3luhyshjt.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3tblpvxal.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3uqzyctkt.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3gtbeowwp.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3lbtckuxg.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3nglzkdaj.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3kzbrrgqp.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3fzqjciur.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3dresifur.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3iyqumccm.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3glhxdfaz.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3uqhmwhwm.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3lnmfwasb.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3uxsgknpi.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3evlfzoby.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3slsjfmkl.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3djrgnnew.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3chkngdvs.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3cefwggxo.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3yqfzfkwk.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3ifprbghx.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3qfjdrsdu.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3xvfldzvw.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3hobdrmwl.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3lomnmamw.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3gchebbbm.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3hyjgyqix.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3trnjhjpw.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3dumylxur.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3ujiunaic.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3fdvnmqla.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3ancgvodq.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3qmimmnzt.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3unhdcbro.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3vwoboxcn.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3uqficbbl.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3aqcnywkh.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3tfyipljf.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3wyulezra.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3totnomvp.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3blkhtltr.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3dgzwaode.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3kfyzbhna.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3agearhdg.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3gugbnpui.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3aefymrrz.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3potvhtlw.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3jzmqszou.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3knbxaxet.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3wqnybejk.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3pwmwpxzn.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3cfhrcdga.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3bgjhhjun.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3izrxhgks.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3egoqszsg.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3baxcesin.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3ykjttpcc.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3aboqmvbs.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3eaymzgtz.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3vptbetcb.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3rbeayiwu.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3waokptqq.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3idwwxujz.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3ilobpuzq.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3swwsdwuu.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3jbdddcqa.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3afgfrfpf.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3pfpznpei.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3wgzabvhy.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3hkzvdsko.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3oqirkjdt.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3akmkkmqx.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3ccbqrbjg.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3ljhgdzuq.html


<!-- 参考信息 -->