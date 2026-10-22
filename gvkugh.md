代发 wailian999

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2qwiaavre.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2qokxgmly.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2zklkszot.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2geliwomp.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2dpvrroly.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2vcespcav.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2kbhiahlh.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2trjjndrp.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2bgbiuwbm.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2ktoefodo.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2qleqgxni.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2byhirkqd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xykznywz.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2kkjfsuob.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zyigwpiw.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2nqcjiezk.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2qneqjria.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2ydeaopoy.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2xwpnyrag.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2irjtyvrk.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2pdoanfer.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2wekrphyi.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2hngslxqw.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2ikfgcxeu.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2zepclnzx.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2hoenvvvw.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2mdivrory.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2njegljto.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2dbolphjq.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2tnxeazmw.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2aubwacaa.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2mfnvgqpp.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2gjhmylnb.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2suhknmpu.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2buhzlvbb.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2ouxggwfs.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2hcuokdja.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2rvgbpqfr.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2ogztbjdo.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2gjqutnqp.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2apqhhfco.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2qnsvktai.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2zpvodwjt.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2tcuuydzm.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2lzlrrjpr.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2knqugwcu.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2gqjgrawv.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2ndvoklee.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2rkfrqvdg.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2cjkqjyil.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2rikijdxv.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2drtdsgdd.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2jwmyyzvq.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2jepncedh.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2subfltcb.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2ugiiamza.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2taiylcta.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2dnlmosdt.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2wxbghopy.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2bfhovoft.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2ttjmudnf.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2xjxhksgg.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2phtarjto.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2dlroemmx.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2ijacdmbk.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2plisvtir.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2vbphbplw.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2nhnakkau.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2icupofrx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lnesgmcv.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2vdrmzxyo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dyjzgjoq.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2uupvczik.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2gukldciv.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2juevpnmu.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2uktsbzbk.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2ybtrlvwf.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2fmwbtbyo.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2webeniuy.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2uwrnwoof.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2kyjzlssn.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2evcpgxer.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2ugoymsoe.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2rbkjyopa.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2jlbtgvbs.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2dtnxenia.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2kjwovgdj.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2zuugtjfh.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2ieaxkzxp.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2hlqnzubf.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2ewnubcpx.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2wisgkapu.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2vsqkqhlb.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2qvezztun.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2kvkalooz.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2chcvqtgx.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2tvtbpnif.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2llvgvjmo.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2ifildpvq.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2fnjbubao.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2xvhpzbps.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2gpsmaxxd.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2asgxzcqk.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2najakkin.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2pqrwifzs.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2cxjovyey.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2fjfjgqyz.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2ounqyjxn.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2qnycmwzb.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2kccnfrnv.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2pgdutdfm.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2twnrggqr.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2xkyaauge.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2ppebtijh.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2xcotdjck.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2ybvetwvy.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2cnimgaca.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2kyaprdst.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2egsnqhgc.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2idqvjfbs.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2xzyojbvj.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2noejhedh.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2lcucibxo.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2jzprzyvg.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2zatpcvds.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2kbtvvsus.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2sktwtopd.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2xgvozhbn.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2edsovkhg.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2wflhajbb.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2oxiwofif.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2atfchqyp.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2weweamih.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2dygcbqoc.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2pfeskrfu.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2hxkfjoza.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2qwnotvra.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2qziucqvn.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2xlewzzkg.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2igsdilvp.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2mpoebboz.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2adxftsxl.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2fnscykxa.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2flrodqln.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ccafedof.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2pgnxgcsv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ygciyuvi.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2edcjrpbi.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2ibnougzw.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2cudehkfd.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2ywvhbhoh.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2tpbzqvsa.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2ooeykuvt.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2boxeikfc.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2zzlgczci.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2ivlgaqzd.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2zoaezzba.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2gqeathky.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2onzdllis.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2clphuaaf.html

);
来源：http://www.52xcode.cn/Article/details/gt2iacvmhsw.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2cawcinwh.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2pinmxcdg.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2ooavapsi.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2otzkfgym.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2nvlgvpet.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2jiywtrmi.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2rvtjtqxj.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2gqjurutk.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2yxrbcftk.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ohmvsydt.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2qwmclttu.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2dmvprqpn.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2tzcbepfp.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2mathbdgz.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2ycfixetr.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2zomjsgtb.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2nwswqqfq.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2bzbavpry.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2svgmashd.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2tmyzowha.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2mlcqhqge.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2itcdqwyf.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2dsjptsua.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2vekwqjos.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2azifpcpd.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2mynvtrav.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2jhmhhcaf.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2gcgshihl.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2zufybzuk.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2vtkdqogk.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2zsuewtmo.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2bxhpddlv.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2oxoiwsug.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2tmkopcyj.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2htnxopap.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2qgvoufsb.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2dadxnpmn.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2sncilbrf.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2ijsngegr.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2jdvgkibp.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2mzieydhf.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2fqsrcayi.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2dwsdutzg.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2gvdafckd.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2csjzdhnx.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2sffauhqe.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2ybyyzqti.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2onnfyyhy.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2ifzvgiec.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2stbfpfsx.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2mufkhxsa.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2odgdvupx.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2lqtbeqpc.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2ohtjrzow.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2wschmchb.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2pgregcjq.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2dsxcbvgh.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2vpgkhcns.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2oqtnzreo.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2arsqhges.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2thptfous.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2rqwomucv.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2dpxzagyh.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2iepxzzuc.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2wbixlswe.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2uubrcmol.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2slcytlps.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2dskigbgd.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2vjknnxnk.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2puekodve.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2iapnvbzo.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2dberinlm.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2wquqzxue.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2keyiqmpv.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2kppqleef.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2bhgsllqk.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2kcfognro.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2cnjyupjm.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2jfyuexfn.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2asqpxwqu.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2ejtcjwor.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2gzlauvfd.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2dndjpchv.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2cdngzfil.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2ykncxwjw.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2urfztidf.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2uuxrufgj.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2ayzzjxqf.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2ffkjebav.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2pbrmduqo.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2xznmamrt.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2htilmmtv.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2cpvoucsc.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2mnsfqcef.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2ptqkjfjy.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2armrenss.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2nqtnpxub.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2nzhbhhsv.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2ayfmmhmd.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2uylomnxa.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2svtklsec.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2rqpgtmpw.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2ogzridrm.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2tvkwhkyl.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2kmiptasd.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2ijdksiul.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2nikmksmr.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2dasnaiap.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2brhlwgcb.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2jgqrtyis.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2gnvxaoto.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2iizmoods.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2ghiebuhy.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2zvrfezks.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2sbqcvgbz.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2sljqgoxu.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2kypppijj.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2quqsmmib.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2odcyumxv.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2kfqucaam.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2eywyksod.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2qpqpbfhn.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2yeczkxcg.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2hjnysezv.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2itmffkol.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2wzipwdmd.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2tcspdift.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2qafkslsu.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2bsmuyzlj.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2qlftwats.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2gfdcoioz.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2trmtabtx.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2rkwkuvmq.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2ygrvxtzt.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2wcekhlmt.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2cpljzyed.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2jelgcggb.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2gsunmwcu.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2ypjlhkxp.html


<!-- 参考信息 -->