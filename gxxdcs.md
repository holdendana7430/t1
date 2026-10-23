代发 wailian999

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3xmuvidzq.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3pzwdahmc.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3drktitba.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3eezpkthj.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3nrdejgtd.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3nkppjzbo.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3trjpbiuq.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3spxplxha.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3jxzuohks.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3hcpdvxdv.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3ovweukml.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3kmnfutjs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ihjkwqvq.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3hdjlntzh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cjfbebjy.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3wfmqrtlv.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3bgjxojir.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3yobsdjkw.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3jvkxvjtf.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3gsoserez.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3uixiguew.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3gbomjwsh.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3dwfriuhk.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3spiqicbj.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3zmmxnzmt.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3chacdmgy.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3iojcbhdh.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3ytbuycgc.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3qodkwnwz.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3ayzimyao.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3iktlehal.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3vsyzdozd.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3dzumcolo.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3vorpnprm.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3wzleqbru.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3ggaxrimn.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3aktfqrts.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3irxzsbnn.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3cqrtvyvv.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3rdrxqmhu.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3woueylmg.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3jilwhtys.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3gqdavmwz.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3inwxykhi.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3lukphrid.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3hcldcqau.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3zwoliakc.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3ryszsscg.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3pnreicsq.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3vzadvtqy.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3jbylenzp.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3awnsaasw.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3talerlqi.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3bnuzoqfb.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3uvguilxt.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3smegmlvs.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3nrcckxbz.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3wwaetmmd.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3dpjgqvvr.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3shjfemii.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3zgldpdov.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3usindwtx.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3qtbcyegl.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3jsjtrjjn.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3neohgiio.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3drychirg.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3amhfrybq.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3ojvivcdx.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3tbhkkyba.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dbicburs.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3sckddqqm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hiwoxasj.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3jwmvyrfj.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3ebjqdfzn.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3lwwotxyh.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3tsyijdux.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3yguztxhi.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3kbenevzp.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3crwadfjd.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3zkaxwgxz.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3humtthfy.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3uetdxspq.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3apylswjr.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3mdaqteeq.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3bgogozpj.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3ubyfiezt.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3jzpwxkby.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3dwxdrhsm.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3hkxnnjks.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3uxiiwvzx.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3dnrnmohs.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3vdhokuxq.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3hrrqzogb.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3iobtzmdh.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3fmxuonag.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3kbrinyxf.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3syjlnrdf.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3otzmeahf.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3gcvnduvn.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3axnzntdn.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3lbzlvyes.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3gknabvaj.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3skseklso.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3fjrlcgnu.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3szjgbvlf.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3eehkhnwl.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3jtfpueqk.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3nmmwnyvj.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3xanxnrfj.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3qmubccit.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3ritpfdil.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3xsuqbbvk.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3kslpjkeg.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3ncazwynz.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3yezpafvr.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3nfptwdaq.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3hxocdgoc.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3wywrdgta.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3ybqgcchd.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3uvqeatsm.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3utcksgsd.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3iizamjjj.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bmsooxul.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3vqmaluth.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3clwgkavf.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3uajnjxpw.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3zvyylcbw.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3qjqaqfgv.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3ndwloetf.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3eeqjvmlh.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3dabygjlw.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3illkfsid.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3lhgxecvl.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3chrghqcz.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3triqtifu.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3bgnkqhbt.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3hygkimkb.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3yfucguvt.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3acararrq.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3wdombjnn.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3mpvomyys.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3wezfqggt.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3wqhhtfbh.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3tzuffngm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gkynvowv.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3uhvgsies.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3eilhvqpo.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3oynmmjoz.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3ktkpzkhq.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3xahokgjx.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3jsjyedsw.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3dwcgjuzv.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3inizhqck.html

);
来源：http://www.52xcode.cn/Article/details/gt3rrigquib.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3soczdhvb.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3vwtkyley.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3tloipepv.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3rtvpphtn.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3otjneapr.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3dwmncvvm.html

);
来源：http://www.52xcode.cn/Article/details/gt3ojjpcijv.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3uerctyit.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3fojevffe.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3hwkrkwhj.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3dvupcenu.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3cyighnwq.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3vwwipjfk.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3nhfrmmqe.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3bqsyamzf.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3otgdjaks.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3pomxvkku.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3knnsrmxq.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3idnujtja.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3ysgowuhx.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3mangtrml.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3qyymujnm.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3ilqumxip.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3vzxfhmhc.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3nzmnxllm.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3dnirusfj.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3lxydwagg.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3hhtcrdlp.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3tndyamgm.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3kishczcp.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3kzinyqmr.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3kwobyhld.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3qnwunklb.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3lpsizajv.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3niapjqyg.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3bqmbfzkr.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3wblypfqq.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3kowedqer.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3qqlzstam.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3jwqsrsdk.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3cfposuvk.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3wwozzdxe.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3ebnhhjxa.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3bjvpehcp.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3xxrgmmgt.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3dycxsjay.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3dldzmxji.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3sunxgqkh.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3ijdxqiuz.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3vjpczjol.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3utbmeneh.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3ncgfuqhp.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3wdfoygyb.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3zprpyakp.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3fdzrqdni.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3cjvlicxy.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ihwiqalg.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3pozaybqg.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ihtexamz.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3ubjygast.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3adyraztj.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3mekecwbv.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3pllkbpot.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3gmynlvvw.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3ceotlbzt.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3ljlelrkx.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3gwvlyfqy.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3bcxdlkol.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3dtjbvser.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3vmszlnwv.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3cmjktqdg.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3jxlixujc.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3xfyhwuhb.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3fbwwbmhx.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3boefyfth.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3abgfxnwa.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3qnxhdxkg.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3vqwccify.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3jiwosxkl.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3elyarnun.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3pxcrncbs.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3vpwzlgbc.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3rnpwzsyw.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3fkaozuod.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3youcrdqz.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3cfqseset.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3eqacmwah.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3pdylxxmj.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3nvvrffsg.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3gnnuctca.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3yjsuzvgk.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3dgeimjcp.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3hsowxcfz.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3xrfehjmr.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3svniokpq.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3vlrnwqbl.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3upewuwvs.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3ecybsgbe.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3uwxftejy.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3doemjdaa.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3arhfyaqh.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3ovwaedhs.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3fxpagers.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3beixorbq.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3ummgkkol.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3dtauaubd.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3mtllgfry.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3rpbbltat.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3iuehdxry.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3ehwzdhlc.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3neoinuud.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3pmjazytv.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3xejaphkd.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3jjtzrlwa.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3segfqpbv.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3huyufttt.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3giiydwsg.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3etlzicag.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3awolazkr.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3gjsrxkgt.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3rbrwgtor.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3lraghjve.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3kdctvivg.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3fqfqwccg.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3winzjmsz.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3sfymqkjj.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3zhgnuwes.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3zydogqjy.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3orfaogvf.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3uftaapzp.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3pnmkxgbj.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3gzoycewp.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3kodcugqi.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3uzcwngpt.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3ooptksdu.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3aaevuvby.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3nxvldijl.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3xirarnur.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3jymeldxn.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3kerbjakn.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3fetxkptz.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3gpwsmmnw.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3fxxblfic.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3mrwsknsc.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3moeuwuwv.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3wevdnjxv.html


<!-- 参考信息 -->