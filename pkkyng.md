代发 wailian999

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3vvxhlvav.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3mmzbmitw.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3yukjnsrv.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3tuukjhwu.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3yfqtbudr.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3pphvvrwi.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3mahcolow.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3yucatgsb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3aueurcva.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3zcukxbhv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wnbfvfal.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3quzbgdwn.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3knlmvofr.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3jztcxeyf.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3jrntkzmb.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3jjvpfxlk.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3iixuqxqp.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3lormudqg.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3flslgiaq.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3ojqkjffk.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3pwrymugs.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3nptnqjeg.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3icytvsaz.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3natviudc.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3ylbqitmt.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3xuofkfjd.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3zcxvgout.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3txymbjri.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3jizkehaf.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3rihnwthh.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3nypzvgpm.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3ixrzgfpk.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3qdqjvfdz.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3pwnnqijl.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ffrjuhtb.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3oyyoozcy.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3mvxysiiv.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3jrpyapvv.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3mrxduios.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3liddzdhs.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3utienrqh.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3kadlkaye.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3cbgzmarc.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3pxyasbwj.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3xaumiozj.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3pasjpaeq.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3wcyzijck.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3oafktooh.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3qxbjkxvv.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3trsnzmjm.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3nvayuhys.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3lfgqqxwr.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3edcveygq.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3ihtbkkge.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3rmbsexph.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3sqdmifoe.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3sofheseq.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3cdhnfbcc.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3jbhzhmjg.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3qmcstjwl.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3ihivmqcu.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3fohqaiqg.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3agvmnjaw.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3sujvtiut.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3eiyydrrw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ifdkzkpz.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3qutcubzl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gebqqlik.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3dllbhfxx.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3zlvnmzuf.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3vndaychz.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3xqnmxgod.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3oerzlnqe.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3ukuhligk.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3qkobrkug.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3vggumilx.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3ylgpskbm.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3dcztzsgv.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3kogrgrwa.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3hkzwxpib.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3lwunctij.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3nackqvjp.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3yyfmzkke.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3ebddbtio.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3yxadneqw.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3quvjnwzh.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3jbssvmau.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3lszrwowx.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3sepvvqjo.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3axkepzty.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3jtzmxfcy.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3wehmntst.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3xhfvedst.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3cygasedr.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3nernxjgs.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3yemgpmhg.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3dtznytmo.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3lasjvmqq.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3tjkrfxfs.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3yhxtftby.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3wrersalo.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3whbdqvfu.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3pwrhpenf.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3jhbdvlpc.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3osmounfw.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3iioumsuv.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3rjmavhhi.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3brappdpj.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3zeaamiuq.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3mlpulhxl.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3dnbxjyge.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3yhdkgoch.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3bhtnvivz.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3cknrwdld.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3lamwesyk.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3umuwpgrq.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3bfpradxf.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3rnvcvggm.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3gygsekgr.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3jnqurfsa.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3lzloxabu.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3zutdqhsa.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3apqcbxog.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3lkkgjvyi.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3ftpvcjji.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3zjnnijzp.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3mbaztnho.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ogvhodos.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3weobdasl.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3iyaubqxs.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3gsyeowck.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3mgjwpwec.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3mdzxjyds.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3otmjdetg.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3dkioqkrp.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3opmvepng.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3ewrwfmnv.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3bdjgaptm.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3rmpvfyiv.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3ungvhdfb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bmpiybcw.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3pseylmng.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ubhvuedh.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3kjfjzket.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3vvgmvufy.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3weoyebzv.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3maraxjyd.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3fmhyjfxa.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3kbmjdedw.html

);
来源：http://www.52xcode.cn/Article/details/gt3gvwkktng.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3jsnhxjjz.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3zhkwctqx.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3wohlukpj.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3zszxpvzo.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3dvxfxwko.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3diiwxxjo.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3zozfahnr.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3kfedmcac.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3zzczcwbu.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3gorbcfin.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3weinxufc.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3ogfraawe.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3rgqzfjcw.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3ulaaynny.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3dyqyanyl.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3rwrnyngk.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ijdnzsdj.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3jemnguhy.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3ttwwcnyo.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3lekoebff.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3zpydcuql.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3jmifdfco.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3tyjmixoc.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3aofuabxu.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3tixquoyt.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3snrmzrkc.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3wifablhk.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3udywkcmx.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3ycrndvfm.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3xgtrqync.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3uywioypn.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3czmhnjdw.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3cohgesji.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3ivpcbpum.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3cogclmon.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3mxfluurp.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3vehhljuc.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3npynzcna.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3mjxyqmjk.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3jyzbbfct.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3diatmddk.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3lbunncan.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3jtbvgynw.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3gucplrua.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3pnnatzss.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3zkbxmyfw.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3wrqassgb.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3mhqkixdr.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3ctvdilbx.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3tsvbywrn.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3fbopeksc.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3fcuqkmye.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3qudrqsss.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3norwemhu.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3wttjhqyt.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3atmndvki.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ygquheyt.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3kmunnkcp.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3gicnxdei.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3xifawhgn.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3mzvuanad.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3jfrhmnjl.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3jibyyauj.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3udcxvqfd.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3lubbiino.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3oxgpoibx.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3clrkezig.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3jfglkcoy.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3yfhbjozb.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3ugprvwir.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3qpmznkzr.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3kffzrnhd.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3vtstvfzl.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3soztzjyg.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3qmkxpjgg.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3lcxcexwf.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3dpynxyob.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3iaqpqcwl.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3cumtynfo.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3adbcuhru.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3frfwdbcn.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3fnupiwvd.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3kgnxdvhc.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3biupclrg.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3kcpimysc.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3grqhgemf.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3mxrdrxdu.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3gqldwsbl.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3otxzqgis.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3qwieuquh.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3iwvmuzww.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3lukwiksr.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3vbpaouni.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3ghznkejf.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3qzoljusp.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3utudedzs.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3vwtkyyrk.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3zonnjghy.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3ueafnifl.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3qbrsyadg.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3teebzpie.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3bdgsyqgv.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3axopbqiv.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3fjlrpwug.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3rscsfinn.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3ysbxpzcm.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3zvlxbwno.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3cesxcita.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3vezwxpci.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3jvuvqusc.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3vcsslceq.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3qnveppun.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3assseyff.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3nmdpvypg.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3jgzjqaes.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3zbxvstdj.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3bksekttd.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3orxhcttj.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3dvmffhin.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3wjkhxnaw.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3uzvkvzsx.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3rpibqvxs.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3xqxyioni.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3dcloxuvq.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3giagabze.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3uzaajlsh.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3aqhhwjeu.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3jnfipilw.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3hvuwtizh.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3luuqvwye.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3gdwwjxvj.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3itgoxwoa.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3ewqkijsb.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3qpzlcsqm.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3kmuhovrp.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ffglkean.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3lyabgxtf.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3ehifxkio.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3tnviwirh.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3lmavitdn.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3ebrwzzuv.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3zrmdzvcg.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3pnqyruhp.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3irvdavuj.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3tpgxtsep.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3cqkvtxfb.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3mevyvwgf.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3qqsndiny.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3mjdyrzrz.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3vhugkwds.html


<!-- 参考信息 -->