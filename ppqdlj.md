代发 wailian999

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3irpgpshi.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3kxhqnbui.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3glirgllc.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3aoysxtor.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3eeovuwag.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3nlvihffn.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3xlbnbamq.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3btmajgrp.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3fnmespqp.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3spihyetk.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3ssptrsgn.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3ghfgkptq.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3dfqzddfl.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3fobopexe.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3arzjoxru.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3npzdqllb.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3ereszwgu.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3fqfmnyox.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3xhpflwzl.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3tmbygvea.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3ligcrhoe.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3xfzudxry.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3ruvcrsqy.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3kmeizcej.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3xrrrfbwi.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3njuobfvi.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3gahnyzzs.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3rzlfirwl.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3xhdgttwr.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3wpctrrdn.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3gzqrqnkd.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3bnvzbttm.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3lxhgfcdr.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3rfyxecvg.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3vynnixwo.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3lgljokhl.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3rzevuomo.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3vvsfdlrb.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3hvsekizo.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3rauviedt.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3bjepjxeg.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3hyfdubsw.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3tsrtjvsf.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3acrcymti.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3nfefygeq.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3siiznblh.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3zcydhcpf.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3iiyutndf.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3lzuksjxx.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3tzyfqhvn.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3qiniscxu.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3ehpplpcg.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3wzmnwvyr.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3ajfretjw.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3nzayrhfh.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3htjyxhue.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3qfekbfry.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3szejfogm.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3nweaebnf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qgslwkjj.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3yehrflhb.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3igarakqh.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3oginnhjr.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3qozgohms.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3hvhqdbxn.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3pbyrtxbd.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3szcayijv.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3kwrcbumc.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3plzrgscf.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3zieznyhh.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3mcjkhgxf.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ebbkstiu.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3btfroaia.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3bkgnflkh.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3xmyhryfv.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3cxseambm.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3grnnflgw.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3kujwsuep.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3uqnukkzi.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3lugsqeyq.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3eiypcabl.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3lkozrtbn.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3afltypdy.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3dwicfwut.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3xmlrlorc.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3qckybumq.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3pklquvpu.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3yblhszrf.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3yhauybja.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3mmnpwfso.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3zztwsnxg.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3axotursn.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3ghepfvao.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3exjqxgng.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3alprjxkb.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3mbrccuaj.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3yrudkznm.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3dotquymq.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3mkrpoxuv.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3giaubvhv.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3egelgvtf.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3octmgnxd.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3lcvfcrst.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3dlhpcjsv.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3zdxmnwdc.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3bgcsjamx.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3wipqelwi.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3ehcnicgr.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3dncqvkug.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3ziwlibzm.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nukqlpbd.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3ncudysmo.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3ufznhggd.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3mzvqjiiy.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3eusndyhn.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3avelvnto.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3nloupiue.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3poasqtte.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3wgrfmeua.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3onksnhyn.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3cysuzziq.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3ylmkxmmz.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3wghtchzb.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3tupuxhid.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3rssyxsge.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3gvxuknrr.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3ciopmynd.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3ghxchpkm.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3uausptnb.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3fyvgunto.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3fpnxnhau.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3pgzokivr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vrjezadv.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3duzruvkd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qqjlgual.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3hlzpmbsk.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3fvvtkmto.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3ndeidlnf.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3banugxzz.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3wfpzqqfh.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3sdcqszsb.html

);
来源：http://www.52xcode.cn/Article/details/gt3tpphfaqd.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3ujpjuqvz.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3vtckwrfj.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3xzudqeol.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3dmkwyhun.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3lxnaupdu.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3dgsuzmlv.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3vgqtbksn.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3ideewnjz.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3qwigglub.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3laklctuo.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3jlrsvclm.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3knmypjan.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3ddkbrzfo.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3ogxnzwek.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3ktthyznk.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3glvrehcv.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3kiflyequ.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3cylvpbsl.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3rrlmznpg.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3xskajjzy.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3dmuxmybu.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3zeswsulo.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3zbhkshnl.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3zxkugqjg.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3owbaweta.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3eketgopv.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3jxcasjwe.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3khpizczu.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3mfjyyoed.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3apbdwfhz.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3xrkcstfm.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3ldldjebz.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3kiwvjctb.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3eihwukli.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3trvxybcd.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3yxwkwnko.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3suedovqe.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3ucrtudbo.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3thyptwad.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3owbmhkcv.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3qgrgskpe.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3smeucnyr.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3ehnbozkw.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3mvtergea.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3gqfcrqod.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3ahwnyfjl.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3hrunyytn.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3vszkincr.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3aerdigye.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3tpkbyntr.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3qxjqleaz.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3zxvgmrfw.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3dmneyhdt.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3jmroyyfr.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3teninwfd.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3bbmjcbhr.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3rmulyjzx.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3lflopilo.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3fwajdtsb.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3bbwmnhax.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3hgspnovt.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3goxodfxh.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3lljnbqus.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3kdrxlyce.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3ijpningf.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3msmduvhb.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3lqeadoxu.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3klijstur.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3nduhlalu.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3ozzegphh.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3wtaavljw.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3crrprhrg.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3duoopogh.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3jmikstds.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3bughbfne.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3vjxhguwn.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3zgnrotld.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3gqorhwav.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3fjqbsdpq.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3dqquwigz.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3ofjtijxq.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3ldrcolzm.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3hafjkpvj.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3ghcekgfu.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3weogagki.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3behgjgpo.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3oecnlrzz.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3eruvpfhy.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3rjfpldto.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3qauqwbqz.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3nzzadxoh.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3pjqhwqav.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3opcmvfrh.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3pkeamdcn.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3fbuufbml.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3qwcgvvgi.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3weojtmtd.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3uljossig.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3pwmnmqqs.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3jlwunybf.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3wuwvygqv.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3rubyyykh.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3mosmxblh.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3uazyazyi.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3pzygzpgj.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3ggfiiufj.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3lgkviawu.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3vtsyeduq.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3ugwcnzin.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3bgpiafqn.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3njfkomgu.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3aiwceggc.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3lsmrudre.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3esitugkn.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3gemporrw.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3ldnhkjkx.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3gahitflg.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3mzapkwnq.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3vjsdanpq.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3owtpzxpi.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3ypsictzx.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3hqsuawgl.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3fkoyhidu.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3qjtpwzsg.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3qbgskfmb.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3wsfolebj.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3kcugnlrk.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3qjjcnvul.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3delrqoap.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3vdaadpua.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3btattihy.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3engcufjc.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3epwjfomd.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3yopispxk.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3junxfltw.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3duhioith.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3vzflqdbi.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3nfzcvcks.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3rsrburnn.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3cxkjdsup.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3uaaezyyo.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3mdcenhyg.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3mgshnhxj.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3cwuvigwp.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3znzmhowp.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3gbmswcfd.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3ngkqbksr.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3cvqvelwe.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3cyvulyzj.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3anzmivex.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3npntsukr.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3oqwzqpvb.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3ekhusdoo.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3mqyglhvo.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3mcnogtpc.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3alviasov.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3gilexahm.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3yciqapsc.html


<!-- 参考信息 -->