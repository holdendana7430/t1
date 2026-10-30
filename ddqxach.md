代发 wailian999

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gztlgweqc.sHtML

[O03] 加锁保护共享数据
来源：http://3g.fanxiaobao.xyz/Article/details/gxtsijdtm.sHtML

Py:   with lock: shared += 1
来源：http://wap.fanxiaobao.xyz/Article/details/gpziofbcl.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.fanxiaobao.xyz/Article/details/gpvgqgiqo.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://read.share.fanxiaobao.xyz/Article/details/gfvzokxcj.sHtML

TS:   // 同 JS
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcrarsqun.sHtML

Java: synchronized (this) { shared++; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gurodjyez.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://baike.fanxiaobao.xyz/Article/details/grubofxpy.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://wap.fanxiaobao.xyz/Article/details/gczustqqh.sHtML

C#:   lock (gate) { shared++; }
来源：http://blog.fanxiaobao.xyz/Article/details/gtsetdgwo.sHtML

[O04] 定义异步函数并等待
来源：http://blog.fanxiaobao.xyz/Article/details/gnwufjfsh.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.fanxiaobao.xyz/Article/details/ghdmmenjx.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdswdigjr.sHtML

JS:   async function f() { await g(); }
来源：http://baike.fanxiaobao.xyz/Article/details/gdgglofcb.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gaagurhrz.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqehnrcqm.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqldadwan.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://read.share.fanxiaobao.xyz/Article/details/gfxvyxjiz.sHtML

C#:   async Task F() { await G(); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gzzmliwqp.sHtML

[O05] 并发执行并等待全部完成
来源：http://mobile.fanxiaobao.xyz/Article/details/glamcjihu.sHtML

Py:   asyncio.gather(*tasks)
来源：http://mobile.fanxiaobao.xyz/Article/details/goicjsuyi.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://3g.fanxiaobao.xyz/Article/details/gibxrwcdo.sHtML

JS:   await Promise.all(tasks)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghydthdyt.sHtML

TS:   await Promise.all(tasks)
来源：http://wap.fanxiaobao.xyz/Article/details/gglfdbknv.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gofpdttnk.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wap.fanxiaobao.xyz/Article/details/gaotkermg.sHtML

Ruby: threads.map(&:join)
来源：http://wap.fanxiaobao.xyz/Article/details/ghaueglkp.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gbqnkkscj.sHtML

[O06] 使用进程池
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbodmviip.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://m.share.fanxiaobao.xyz/Article/details/gaafbcotz.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://3g.fanxiaobao.xyz/Article/details/goduvrocz.sHtML

JS:   // child_process / cluster 模块
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbjzubtcs.sHtML

TS:   // child_process / cluster 模块
来源：http://wap.fanxiaobao.xyz/Article/details/gmaamqoct.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvcrngzmf.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://read.share.fanxiaobao.xyz/Article/details/gawmokobq.sHtML

Ruby: // fork 块
来源：http://m.share.fanxiaobao.xyz/Article/details/gmbtpdesu.sHtML

C#:   Parallel.For
来源：http://baike.fanxiaobao.xyz/Article/details/gavzikxql.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gnbnemrdu.sHtML

P. 常用工具函数
来源：http://read.share.fanxiaobao.xyz/Article/details/godoiyjar.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmqlzfetz.sHtML

[P01] 生成 UUID
来源：http://3g.fanxiaobao.xyz/Article/details/gsbbmvrsm.sHtML

Py:   str(uuid.uuid4())
来源：http://baike.fanxiaobao.xyz/Article/details/ghdssqyuj.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyrptangw.sHtML

JS:   crypto.randomUUID()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmwatvbyq.sHtML

TS:   crypto.randomUUID()
来源：http://wap.fanxiaobao.xyz/Article/details/gczzkeboa.sHtML

Java: UUID.randomUUID().toString()
来源：http://read.share.fanxiaobao.xyz/Article/details/glveafwod.sHtML

Go:   // 用 github.com/google/uuid
来源：http://3g.fanxiaobao.xyz/Article/details/ghqihkrey.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.fanxiaobao.xyz/Article/details/gvelkqcay.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://3g.fanxiaobao.xyz/Article/details/gtididdyn.sHtML

[P02] MD5 / SHA256 摘要
来源：http://blog.fanxiaobao.xyz/Article/details/gckmtjkja.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://m.share.fanxiaobao.xyz/Article/details/ghgpzjovh.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://read.share.fanxiaobao.xyz/Article/details/gdmghdskn.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://blog.fanxiaobao.xyz/Article/details/gubfywsjy.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.fanxiaobao.xyz/Article/details/gjygewhvf.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://m.share.fanxiaobao.xyz/Article/details/glkuqtsmn.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://blog.fanxiaobao.xyz/Article/details/gymudxuod.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://blog.fanxiaobao.xyz/Article/details/gybtqmjyz.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://blog.fanxiaobao.xyz/Article/details/gdbnbmchc.sHtML

[P03] 生成短随机字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/gypzqpqpm.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://m.share.fanxiaobao.xyz/Article/details/gletbpfpc.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guvzppepv.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.fanxiaobao.xyz/Article/details/glhutmhzf.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.fanxiaobao.xyz/Article/details/gociwprms.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.fanxiaobao.xyz/Article/details/gtkgvmgpp.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wap.fanxiaobao.xyz/Article/details/gaphosuri.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://read.share.fanxiaobao.xyz/Article/details/gropknqzj.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guijhmodl.sHtML

[P04] 求长度
来源：http://mobile.fanxiaobao.xyz/Article/details/gnlnqfaga.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gloqdklxe.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.fanxiaobao.xyz/Article/details/gfamhlnqv.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpixamufs.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.fanxiaobao.xyz/Article/details/gyrcuriot.sHtML

Java: list.size();  map.size();  s.length()
来源：http://read.share.fanxiaobao.xyz/Article/details/gohhrwyul.sHtML

Go:   len(arr);  len(m)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjzzhhphi.sHtML

Ruby: x.length;  x.size
来源：http://www.share.fanxiaobao.xyz/Article/details/gwduzusbz.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwrxdyufj.sHtML

[P05] 判断两个对象内容是否相等
来源：http://baike.fanxiaobao.xyz/Article/details/guiryhwyz.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://baike.fanxiaobao.xyz/Article/details/gsrsbkwxh.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://read.share.fanxiaobao.xyz/Article/details/gwjvabpbc.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://blog.fanxiaobao.xyz/Article/details/gpawlyqrd.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.fanxiaobao.xyz/Article/details/gmogaejtd.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfsipbmbe.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://baike.fanxiaobao.xyz/Article/details/gbubwzjja.sHtML

Ruby: a == b
来源：http://wap.fanxiaobao.xyz/Article/details/gwnquwfql.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.share.fanxiaobao.xyz/Article/details/gidzrzlxj.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wap.fanxiaobao.xyz/Article/details/gxilwbmfg.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqckcqhir.sHtML

PHP:  if (empty($x)) {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfaczrpms.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.share.fanxiaobao.xyz/Article/details/grccznvhk.sHtML

TS:   if (x == null) {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggqxzoyjc.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gafqqtfvp.sHtML

Go:   if x == nil {}
来源：http://www.share.fanxiaobao.xyz/Article/details/ghlszhpvi.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggqubhxuk.sHtML

C#:   if (x is null) {}
来源：http://m.share.fanxiaobao.xyz/Article/details/geglkfmss.sHtML

[P07] 防抖与节流
来源：http://blog.fanxiaobao.xyz/Article/details/gdtozayrz.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mobile.fanxiaobao.xyz/Article/details/glfkbydzq.sHtML

PHP:  // 手写时间戳比较
来源：http://3g.fanxiaobao.xyz/Article/details/gdsxsqebk.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.fanxiaobao.xyz/Article/details/gzksrilpo.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.fanxiaobao.xyz/Article/details/gjsvjhqhr.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gobcotvmd.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://3g.fanxiaobao.xyz/Article/details/gjdwatvue.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.fanxiaobao.xyz/Article/details/gzxygtysh.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://m.share.fanxiaobao.xyz/Article/details/gnextnypa.sHtML

[P08] 处理浮点精度问题
来源：http://wap.fanxiaobao.xyz/Article/details/gstedefpk.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wap.fanxiaobao.xyz/Article/details/ghwwkjcrk.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxbtcayqb.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://3g.fanxiaobao.xyz/Article/details/gddgzlcua.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://baike.fanxiaobao.xyz/Article/details/gsrjbxdle.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnbpmsuit.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wap.fanxiaobao.xyz/Article/details/gqreedvom.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcyhrbxei.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.share.fanxiaobao.xyz/Article/details/gajqutxot.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbaksgiep.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gclhftopx.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/goxvlbggy.sHtML

[Q01] 创建表
来源：http://blog.fanxiaobao.xyz/Article/details/gelhbhgjd.sHtML

CREATE TABLE users (
来源：http://blog.fanxiaobao.xyz/Article/details/geymvrnja.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.fanxiaobao.xyz/Article/details/gtnpeysgx.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsiaudyyl.sHtML

email VARCHAR(100) UNIQUE,
来源：http://blog.fanxiaobao.xyz/Article/details/gmbwxvtug.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxtfmghbc.sHtML

);
来源：http://blog.fanxiaobao.xyz/Article/details/grfdwvscp.sHtML

[Q02] 创建带外键的表
来源：http://read.share.fanxiaobao.xyz/Article/details/grvtqemfx.sHtML

CREATE TABLE orders (
来源：http://wap.fanxiaobao.xyz/Article/details/gqvrrbvpt.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.fanxiaobao.xyz/Article/details/gkmiamalr.sHtML

user_id INT NOT NULL,
来源：http://3g.fanxiaobao.xyz/Article/details/gppldympm.sHtML

amount DECIMAL(10, 2),
来源：http://baike.fanxiaobao.xyz/Article/details/ghjjpnfda.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://m.share.fanxiaobao.xyz/Article/details/gbyclqjeo.sHtML

);
来源：http://read.share.fanxiaobao.xyz/Article/details/gmjkebfxa.sHtML

[Q03] 增加列
来源：http://3g.fanxiaobao.xyz/Article/details/ggtxvapcy.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gugpywues.sHtML

[Q04] 修改列类型
来源：http://read.share.fanxiaobao.xyz/Article/details/glzmexbdm.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvgwfusmm.sHtML

[Q05] 重命名列
来源：http://blog.fanxiaobao.xyz/Article/details/gybfqvtiu.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://baike.fanxiaobao.xyz/Article/details/gpugcvcvj.sHtML

[Q06] 删除列
来源：http://mobile.fanxiaobao.xyz/Article/details/glzcqafkn.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.share.fanxiaobao.xyz/Article/details/gwfrocwti.sHtML

[Q07] 删除表
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjsjqakpn.sHtML

DROP TABLE IF EXISTS orders;
来源：http://3g.fanxiaobao.xyz/Article/details/gmhlmwkck.sHtML

[Q08] 创建普通索引
来源：http://blog.fanxiaobao.xyz/Article/details/gqgiknfci.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://mobile.fanxiaobao.xyz/Article/details/gpwbbfrwp.sHtML

[Q09] 创建唯一索引
来源：http://www.share.fanxiaobao.xyz/Article/details/gzroinvsk.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gefeyjauv.sHtML

[Q10] 插入单行
来源：http://blog.fanxiaobao.xyz/Article/details/gtonpyglj.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://read.share.fanxiaobao.xyz/Article/details/gpkhyakxs.sHtML

[Q11] 一次插入多行
来源：http://baike.fanxiaobao.xyz/Article/details/gkoiltzhi.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://m.share.fanxiaobao.xyz/Article/details/gvfchnggm.sHtML

[Q12] 插入后取自增 ID
来源：http://baike.fanxiaobao.xyz/Article/details/gxlesdcea.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://baike.fanxiaobao.xyz/Article/details/gcnugtxnw.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://baike.fanxiaobao.xyz/Article/details/gxdfdwfxk.sHtML

[Q13] 忽略重复插入
来源：http://read.share.fanxiaobao.xyz/Article/details/gdqmvsgsk.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mobile.fanxiaobao.xyz/Article/details/gtrsjhxbq.sHtML

[Q14] 存在则更新（upsert）
来源：http://blog.fanxiaobao.xyz/Article/details/gtsjjgaji.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://m.share.fanxiaobao.xyz/Article/details/gnznilnwv.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://m.share.fanxiaobao.xyz/Article/details/gurejsnjw.sHtML

[Q15] 查询全部
来源：http://mobile.fanxiaobao.xyz/Article/details/gxxzwqied.sHtML

SELECT * FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/guuahulwo.sHtML

[Q16] 查询指定列
来源：http://m.share.fanxiaobao.xyz/Article/details/gorcniytm.sHtML

SELECT id, name FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gctwjfrah.sHtML

[Q17] 条件查询
来源：http://wap.fanxiaobao.xyz/Article/details/gyskqcuhm.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/gqfiaoojk.sHtML

[Q18] 模糊匹配
来源：http://wap.fanxiaobao.xyz/Article/details/gwvabzcyj.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://m.share.fanxiaobao.xyz/Article/details/gdipcgknb.sHtML

[Q19] 范围查询
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwqlnbyif.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://m.share.fanxiaobao.xyz/Article/details/gmjdluikd.sHtML

[Q20] IN 列表
来源：http://blog.fanxiaobao.xyz/Article/details/gvfqfzaer.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wap.fanxiaobao.xyz/Article/details/gxctxttgx.sHtML

[Q21] 空值判断
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwcldtuhe.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://mobile.fanxiaobao.xyz/Article/details/gbapdoctl.sHtML

[Q22] 排序
来源：http://www.share.fanxiaobao.xyz/Article/details/gpacfwnoa.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://3g.fanxiaobao.xyz/Article/details/gkiqtxprc.sHtML

[Q23] 分页
来源：http://wap.fanxiaobao.xyz/Article/details/gsfrjorzh.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mobile.fanxiaobao.xyz/Article/details/gyntwvnce.sHtML

[Q24] 去重
来源：http://www.share.fanxiaobao.xyz/Article/details/getlvnyuo.sHtML

SELECT DISTINCT city FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gctkseqfk.sHtML

[Q25] 只取前 N 条
来源：http://wap.fanxiaobao.xyz/Article/details/grmlgjhpv.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.share.fanxiaobao.xyz/Article/details/gcbokijqb.sHtML

[Q26] 计数
来源：http://wap.fanxiaobao.xyz/Article/details/gqrsdvbyc.sHtML

SELECT COUNT(*) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gaossimga.sHtML

[Q27] 条件计数
来源：http://read.share.fanxiaobao.xyz/Article/details/gdnpbcsyf.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwdvmusiq.sHtML

[Q28] 求和与平均
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbwmzeuvi.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggzgdyjjj.sHtML

[Q29] 最大最小值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsvowlluk.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gugwqmocz.sHtML

[Q30] 分组统计
来源：http://3g.fanxiaobao.xyz/Article/details/ggpzaxzvv.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzjbktefe.sHtML

[Q31] 分组后过滤
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsormrxbs.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wap.fanxiaobao.xyz/Article/details/gcsmlruhx.sHtML

[Q32] 分组拼接字符串
来源：http://wap.fanxiaobao.xyz/Article/details/gyzufygbg.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gczawgyth.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mobile.fanxiaobao.xyz/Article/details/gfgxjpsib.sHtML

[Q33] 多列分组
来源：http://3g.fanxiaobao.xyz/Article/details/gfttfulqz.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.share.fanxiaobao.xyz/Article/details/gvhyagszi.sHtML

[Q34] 每组取第一条
来源：http://3g.fanxiaobao.xyz/Article/details/gwgqyehop.sHtML

SELECT * FROM (
来源：http://m.share.fanxiaobao.xyz/Article/details/gwdpbfebv.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mobile.fanxiaobao.xyz/Article/details/gyeyobgwk.sHtML

) t WHERE rn = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/glrpqexho.sHtML

[Q35] 内连接
来源：http://m.share.fanxiaobao.xyz/Article/details/gofjuwqij.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://blog.fanxiaobao.xyz/Article/details/gwvrcisnp.sHtML

[Q36] 左连接
来源：http://m.share.fanxiaobao.xyz/Article/details/gisndzkcw.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvawghwpc.sHtML

[Q37] 右连接
来源：http://www.blog.fanxiaobao.xyz/Article/details/gawphyixx.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.fanxiaobao.xyz/Article/details/gebpfxzax.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnzqtkmll.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://3g.fanxiaobao.xyz/Article/details/gmfsvqyyb.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.fanxiaobao.xyz/Article/details/gubjdurcy.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.fanxiaobao.xyz/Article/details/gvppajcxv.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mobile.fanxiaobao.xyz/Article/details/gyjttxjjo.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://m.share.fanxiaobao.xyz/Article/details/gzjwilria.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mobile.fanxiaobao.xyz/Article/details/gyhjdamxr.sHtML

[Q41] 多表连接
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqgnrepee.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://3g.fanxiaobao.xyz/Article/details/gpiwaecpf.sHtML

JOIN users u ON u.id = o.user_id
来源：http://3g.fanxiaobao.xyz/Article/details/gaahmrpit.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://3g.fanxiaobao.xyz/Article/details/gxptfwgtf.sHtML

[Q42] 连接条件附加过滤
来源：http://mobile.fanxiaobao.xyz/Article/details/gfwdtoakb.sHtML

SELECT u.name, o.amount FROM users u
来源：http://baike.fanxiaobao.xyz/Article/details/gtwyoliry.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.fanxiaobao.xyz/Article/details/gqfbenpji.sHtML

[Q43] 标量子查询
来源：http://baike.fanxiaobao.xyz/Article/details/gjtcguray.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wap.fanxiaobao.xyz/Article/details/gmolqknkf.sHtML

[Q44] IN 子查询
来源：http://3g.fanxiaobao.xyz/Article/details/gleszdfon.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbreugdyy.sHtML

[Q45] EXISTS 判断存在
来源：http://mobile.fanxiaobao.xyz/Article/details/grscwkzij.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwadqqrzh.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://blog.fanxiaobao.xyz/Article/details/ghormcxtw.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.fanxiaobao.xyz/Article/details/ghlmcoshw.sHtML

[Q47] 与平均值比较
来源：http://mobile.fanxiaobao.xyz/Article/details/gigykrjdg.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mobile.fanxiaobao.xyz/Article/details/gtctsqldu.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.fanxiaobao.xyz/Article/details/gpntosxmu.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.fanxiaobao.xyz/Article/details/gyyydqize.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.fanxiaobao.xyz/Article/details/gmeecbbah.sHtML

[Q49] 更新单行
来源：http://blog.fanxiaobao.xyz/Article/details/gjsvdhhnw.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/googlqacq.sHtML

[Q50] 批量更新
来源：http://www.blog.fanxiaobao.xyz/Article/details/gayluuabn.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqlpoyuzb.sHtML

[Q51] 用子查询更新
来源：http://blog.fanxiaobao.xyz/Article/details/giavobwdf.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbflkpktw.sHtML

[Q52] 删除指定行
来源：http://wap.fanxiaobao.xyz/Article/details/gbkktqznw.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.fanxiaobao.xyz/Article/details/gjlixkyxq.sHtML

[Q53] 按条件删除
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdxarnsnk.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://3g.fanxiaobao.xyz/Article/details/gfppqdmnn.sHtML

[Q54] 清空表
来源：http://mobile.fanxiaobao.xyz/Article/details/ghplgvrmp.sHtML

TRUNCATE TABLE logs;
来源：http://blog.fanxiaobao.xyz/Article/details/gqibaxlki.sHtML

[Q55] 排名（并列占位）
来源：http://m.share.fanxiaobao.xyz/Article/details/gypltsaic.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://blog.fanxiaobao.xyz/Article/details/ghkjqxtua.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyyxtkwdc.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.share.fanxiaobao.xyz/Article/details/gwkfcawqk.sHtML

[Q57] 行号
来源：http://read.share.fanxiaobao.xyz/Article/details/gnlklsugi.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gpdmgfhdq.sHtML

[Q58] 累计求和
来源：http://mobile.fanxiaobao.xyz/Article/details/gvdapieym.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.fanxiaobao.xyz/Article/details/gwfhcjdui.sHtML

[Q59] 分组内累计
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyfsmfqcw.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.fanxiaobao.xyz/Article/details/gajsfyfyu.sHtML

[Q60] 取上一行 / 下一行
来源：http://read.share.fanxiaobao.xyz/Article/details/gwfprwsfg.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://baike.fanxiaobao.xyz/Article/details/gcknbohlh.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.fanxiaobao.xyz/Article/details/gkglpzbyq.sHtML

[Q61] 移动平均
来源：http://baike.fanxiaobao.xyz/Article/details/grvzwfrsx.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geyivjwxe.sHtML

[Q62] 分组占比
来源：http://www.share.fanxiaobao.xyz/Article/details/gdyvmblst.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcnpungdd.sHtML

[Q63] 开启事务
来源：http://baike.fanxiaobao.xyz/Article/details/grfrbkllp.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.fanxiaobao.xyz/Article/details/grcduqqqt.sHtML

[Q64] 提交事务
来源：http://blog.fanxiaobao.xyz/Article/details/gjnkhwxjc.sHtML

COMMIT;
来源：http://wap.fanxiaobao.xyz/Article/details/ghvylgfyr.sHtML

[Q65] 回滚事务
来源：http://m.share.fanxiaobao.xyz/Article/details/gqlqcfugp.sHtML

ROLLBACK;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghhmxkooy.sHtML

[Q66] 行锁查询
来源：http://mobile.fanxiaobao.xyz/Article/details/gehwcekug.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wap.fanxiaobao.xyz/Article/details/gmyvrvzra.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggzyxdtrr.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.fanxiaobao.xyz/Article/details/gqvvfjwpl.sHtML

[Q68] 保存点
来源：http://m.share.fanxiaobao.xyz/Article/details/ghynfpiwf.sHtML

SAVEPOINT sp1;
来源：http://www.share.fanxiaobao.xyz/Article/details/grwvnifpu.sHtML

ROLLBACK TO sp1;
来源：http://baike.fanxiaobao.xyz/Article/details/goynlafvf.sHtML

[Q69] 查看执行计划
来源：http://read.share.fanxiaobao.xyz/Article/details/gfsphilpy.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.fanxiaobao.xyz/Article/details/gopbnczio.sHtML

[Q70] 更新统计信息
来源：http://wap.fanxiaobao.xyz/Article/details/gcifsddpf.sHtML

ANALYZE TABLE users;
来源：http://wap.fanxiaobao.xyz/Article/details/gkhdbfkas.sHtML

[Q71] 查看建表语句
来源：http://mobile.fanxiaobao.xyz/Article/details/gqnwzrlyo.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.fanxiaobao.xyz/Article/details/gvmzpfkml.sHtML

[Q72] 查看索引
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvpwvygdh.sHtML

SHOW INDEX FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gtgwamlzs.sHtML

[Q73] 查看表状态
来源：http://mobile.fanxiaobao.xyz/Article/details/gvajnfyif.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.fanxiaobao.xyz/Article/details/gqwpvjiel.sHtML

[Q74] 强制使用索引
来源：http://mobile.fanxiaobao.xyz/Article/details/gekqsajum.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.fanxiaobao.xyz/Article/details/gufzccfxy.sHtML

[Q75] 日期格式化
来源：http://m.share.fanxiaobao.xyz/Article/details/gstzcpzya.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glpkzfsnx.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.fanxiaobao.xyz/Article/details/gcsrqjqzc.sHtML

[Q76] 按天统计
来源：http://baike.fanxiaobao.xyz/Article/details/gcqidbeuu.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.fanxiaobao.xyz/Article/details/gtebwazmg.sHtML

[Q77] 时间加减
来源：http://baike.fanxiaobao.xyz/Article/details/gexrxfvbo.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.fanxiaobao.xyz/Article/details/gpvujybtl.sHtML

[Q78] 当前时间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcpgmudgk.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.fanxiaobao.xyz/Article/details/gwosgsszk.sHtML

[Q79] 字符串拼接
来源：http://baike.fanxiaobao.xyz/Article/details/gaxvjqkua.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.fanxiaobao.xyz/Article/details/gnitdphcg.sHtML

[Q80] 字符串截取
来源：http://read.share.fanxiaobao.xyz/Article/details/gfdsarvlp.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gulruuqhi.sHtML

[Q81] 字符串替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gczmfiabl.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/giafghdli.sHtML


<!-- 参考信息 -->