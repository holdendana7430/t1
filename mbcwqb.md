代发 wailian999

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3xfxteueu.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3qymwzfjw.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3axbbaftm.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3utygsidd.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3xmawvyeb.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3ertdwadu.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3xurxtnuz.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3ikemvsyq.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3inwojmfg.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3ozadwlzl.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3rlqvwslp.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3lvgyseix.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3xbapnvhu.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3jtewuntq.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3xnvkncqs.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3lpskdymr.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3brgvrsgb.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3nrrrtuyx.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3pqapaonq.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3nxjfihyp.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3idotdpfv.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3bsumfnoi.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3vfdaatha.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3satcjkgf.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3fvyckbun.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3zdsyidec.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3khklluif.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3ehwpztwp.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3szksksse.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3quafvujm.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ssuyrhlb.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3quvwqzac.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3mctjvnms.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3dzdwztrp.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3xgkfreuw.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3nuitqblh.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3kqdyovbg.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3lrvipbob.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3hwjvbgip.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3seeceyjm.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3dwjatmvz.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3ljxhbrqm.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3aqtymcir.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3gcszmzcx.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3lqnckspi.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3oapzcasw.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3dldjieyz.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3tiwlrluq.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3rbgzymhx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sjjeapvm.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3nleccreq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dgcmgboc.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3ftgyyree.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3orbmhpkz.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3ppfgrmte.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3fjixoawm.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3qyaosjzo.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3nlajpkln.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3jxugenyt.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3lwumohwk.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3blkagzuj.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3munyzdnp.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3agsqijjx.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3skyjmizf.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3uxnvajnz.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3bbiltevc.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3pfeuhfqa.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3qienbyxp.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3fvlxqdpv.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3dtkqcvky.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3rcigcmrn.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3shseoedf.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3fwjdrlho.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3ypolgqxm.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3rieexpjc.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3xvnlaqmh.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3ppvclkjb.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3vpfmwsik.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3jbnxdzwv.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3nvryisvd.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3nwxrvtei.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3olftgcur.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3fydkbeky.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3wpmrdbuk.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3pzyohhqs.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3jjftgudh.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3fiwupzgc.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3yryupshx.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3jkvbnyfc.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3pkgfrlva.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3lneruhiz.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3gbdydnpo.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3hhvutsxp.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3vkgwhbyd.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3cuqoolif.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3axzssgkr.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3jbbwolip.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3aclbcrbs.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3oyjfyift.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qtzzsrkl.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3otgrbzjd.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rwcpxxcj.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bzmwzkzv.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3lumgmpds.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3yrhcoedk.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fkogsywn.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3ifhuehav.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3guovaizr.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3hdjnfttn.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3ryzutvet.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3xpxmsiwn.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3wmcqndsu.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3mstimnvw.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3lplndgvp.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3margcczx.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3vqyckcrs.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3geanncda.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3fbvbfvtq.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3vvekemwv.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3gcrumhnc.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3yzpggnts.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3chumumyi.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3jbxjnewg.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3ptfhxsdl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3twnveylf.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3izzeadgk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mwkvpghw.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3avwdmpxc.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3gzjngutt.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3kcyrdrnk.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3fiamaryr.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3lpehnjsk.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3pwjibkxx.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3inbfeoam.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3bftxsbox.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3cwqgvpwv.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3wxiawoms.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3mkcvgwoz.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3usrkprnu.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3qukvekyi.html

);
来源：http://www.52xcode.cn/Article/details/gt3tclatzus.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3izayimuc.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3rrdwfvyr.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3mealmkcd.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3oorcohhv.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3wwgiicat.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3isjwmisg.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3auzfimws.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3zrpzhssk.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3zyghuhca.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3kmqugypy.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3pyzavzxv.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3llvbyekr.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3raqlkcwv.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3ywxxsayf.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3ydtadzxn.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3mtldircg.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3rvhbesed.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3tdfnnocf.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3vnhrtgws.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3atomyjgl.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3orwgvltd.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3eyesafoz.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3cchdylms.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3fkkqvsds.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3tdssqnio.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3ajacnjbc.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3oblhvwdo.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3fgwiuvlq.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3psqvfyab.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3udijaxcy.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3dqsxuyen.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3ftxznpzj.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3fwkprizh.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3cbqngjjt.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3tkabjywt.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3kkwwamht.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3fasadjfg.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3uiqttndk.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3inkbzdyj.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3kexrszdd.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3lcggqfix.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3fqjujney.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3xgfxehey.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3tuzrothm.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3rlbvpcae.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3itpcsoxr.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3xpdshpxj.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3hsvzatvt.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3ipoalfzc.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3aniuhpzk.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3zsjqgokz.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ubonjqjr.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3sncqrccj.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3seeqstgk.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3rogammls.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3yeperqwo.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3vvobrhwa.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3qsjavvzp.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3tyfqrjkf.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3zvvybxcf.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3lmiieujv.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3ipghdqie.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3iefqvpbz.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3rdhajjuj.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3qudisnvb.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3sxlmxejp.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3nmbwerrp.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3gjeptgva.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3zhmfyahz.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3oldnbmun.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3ytelxobx.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3kmrzpikl.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3oheaabfx.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3ocdzjkck.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3gjlndwvj.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3pfbhrxxk.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3onokgjup.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3yrbatxcm.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3ewyclwwt.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3ipuqsmva.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3pwutmveq.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3rytwqgkq.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3awsvperq.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3lkvrjqgl.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3ymbkrqez.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3nxdtgtma.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3bocjivyr.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3aeyvtpxa.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3gnmwsjym.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3xorefijf.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3auouserg.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3senncifv.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3ypzreglh.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3ayjrgtzj.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3naxzvmsp.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3azazxpvx.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3bevvbtjp.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3bgficvuv.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3zazbeyvy.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3yagbvbzc.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3nlxmlgqj.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3igeexymy.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3cjhjmdyk.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3yaitviry.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3fhssylrt.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3nvobsvvi.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3hxnylcel.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3ulvxqhzr.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3uqequzje.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3nykauypp.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3deihdczb.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3vcwrujno.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3etpzttkm.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3eimgctho.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3dvxlzxrq.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3pzjduacx.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3hvveojay.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3zgbdiexp.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3kldbjbsn.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3bgttiopn.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3tckiensw.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3yujshemn.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3tdfxsupp.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3wqqoadnz.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3stqmqkbg.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3unrhcdrf.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3jhbkxjup.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3oclhxoeb.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ncazqmoh.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3vmuugpoz.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3oytgxmim.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3cqhtflvk.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3eblkbbgo.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3hoqrehye.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3gkbzglmn.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3ryyqzcsx.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3cxvsjeqg.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3pnaxsbfl.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3stqfvgxu.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3stnaojzk.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3eltiodvw.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3ldevivqa.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3gizpdktg.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3amsdyxur.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3bjthknfg.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3kcetoxig.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3vmwlupfk.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3bszicglh.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3kdunqabd.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3hhslmuqj.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3bvnvygcp.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3wvlaxodl.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3avavvyrr.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3qrvddswz.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3djjjshld.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3lgtgeqmn.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3sbtcxcil.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3cyudyffs.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3jrepnhhi.html


<!-- 参考信息 -->