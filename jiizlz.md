代发 wailian999

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3vylfodyg.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3fodmnmqc.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3mbsbgzdd.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3qbfbyrgp.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3owzumqrm.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3phknkxlc.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3hyrqftvx.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3zfsifqbh.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3jrucqtsu.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3qctxqmrc.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3rkjfwwxn.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3saybjzbc.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3xkkleowr.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3skwxheew.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3rfddjhvz.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3hynozibl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zchnzout.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3ylmimthk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yjefbtpp.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3zhibojta.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3muamxtdg.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3lzkuwxom.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3iitkrffx.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3jbvuahih.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3hpxnhfwn.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3seludmhd.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3awsueprg.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3egnrggxr.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3rffafbrf.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3jzvuyrpt.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3sxvkzwxt.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3krzgxuiz.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3bxrnmuoe.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3dpayrtig.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3nolhlson.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3qdlosvii.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3ezbdgcsy.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3dptoazxp.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3rpbscjhr.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3gdczwual.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3yleybybb.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3trxvpyog.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3eiymfvjl.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3jbfvmtxg.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3nkaydyea.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3pjnhqsxh.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3mrmliibt.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3bihrfhgq.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3xtcigshb.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3dxhsebkk.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3oshmbztm.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3dpqklthe.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3afyzfeeh.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3toostogk.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3sfbbdafb.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3ajviifcm.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3qoxbzfre.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3lwxsfogb.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3fpchjasg.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3soaxwhzg.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3sqbeeftn.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3aoewkohc.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3znjbwpye.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3urvohecf.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3hydneoqf.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3vipdbnyq.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3hjdzucro.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3teghpdtt.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3glcszbsa.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3zuqrwata.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3tikvsjbw.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3xjaelnzh.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3fyolmfjc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3eeieyudy.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3ewuwuues.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3olqvczsz.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3qiaydfts.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3opwxuapd.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3obnidnxl.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3muqagone.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3orvtyzpj.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3qpjectqc.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3hdjaklot.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3ytfgwdph.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3dktkewvl.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3ukivhcnb.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3dgqfwlnu.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3isyopvfm.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3xdyivlkp.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3mdyzzkuj.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3ymnpwmgg.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3fxjoimyz.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3skbtqwna.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3uiphjefw.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3jrgiawgq.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3fduawaie.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3teddwfga.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3lqdforot.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3zifzwmhc.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3ajrttpqe.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3aoxtespu.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3qrexiiyd.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3mgahypiq.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3dgdvqzqj.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3qddxxqir.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3wzgdhlqo.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3emhibcbs.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3lnxgqabl.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3ruwouimo.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3gositnpv.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3cumacqnx.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3qzhrekwd.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3izrhwudc.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3xkguxpvt.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3odhywshg.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3xiieoqic.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3oeqsjcke.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3ctxhocua.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3rezeuvpx.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3ntwavkjw.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3exekvkwl.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3pqbqjgnh.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3boqxemzm.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3zrorgsnx.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3pibcubui.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3sqnkcvaw.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ovhfyozq.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3yryzjlqb.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3azatecxq.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3wznalucu.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3pnazblfv.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3dpowikzk.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3avwiuynm.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3rvtsqxsn.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3vuflhfns.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3rxgpgxjy.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3rfoutrbu.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3acukriml.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3zotfffid.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3ghamwuoe.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3raxxvnuy.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3cfcgenel.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3izadaifm.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3peaoznne.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3pedhwdjr.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3jmjaseth.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3rolxjnbh.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3uayewlxj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kfmuxyzf.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3thtqdvlu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qoldjiae.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3wydjqenr.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3rhwvqqgq.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3ddcpdaty.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3gheupoef.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3qacfjehk.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3mnkuyhhe.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3zxyjozln.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3pcdtbhlo.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3lhwgrrdb.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3wmsicwzz.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3jtisfkzz.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3cnojyzxc.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3sygtxtzp.html

);
来源：http://www.52xcode.cn/Article/details/gt3gggvigxr.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3uanzdsgr.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3mrlrfniu.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3omchyqhg.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3zpugyfsm.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3aretdiyn.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3spptjgyn.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3dcjokcul.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3mriuulme.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3gchfarms.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3rlzjlzit.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3huqfqjqr.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3nsfbyhwk.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3ppgbygqg.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3ctvrzlfn.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3qaskxicv.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3fxomwplf.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3hgzvkpht.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3yxzximer.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3vzhcwxth.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3hxtkjmwf.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3yhlmozjz.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3ybyvnawf.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3bszavvlh.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3luxuzrnz.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3ernmzsps.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3nlmnkqiw.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3dyfdsszb.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3auuxvrsi.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3qtvkzqzf.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3bjvcefnx.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3wvyjlpbi.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3kzkfykin.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3untkrdtv.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3pbvdmftq.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3uahvcejd.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3uqbehalj.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3nqqeolqt.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3woxoftst.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3dafflene.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3xywdgkot.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3ryqjmmwe.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3wvuldodf.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3vsrwxaxk.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3hvsjgrty.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3vrlauotp.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3cjdxzlyi.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3ydhczgft.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3cdbfoaef.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3akywvyte.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ufccxznv.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3ignbtnvf.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3rxjgvwjd.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3sxkjjbzh.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3qohqgtxq.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3gwzlebjm.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3mdxdupdi.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3hkdhieas.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3niijwnab.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3ghxmlxaz.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3tkwtscne.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3gelzqewr.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3hbezrdpi.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3ksgyqaya.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3uohqxekg.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3islybiim.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3bliealli.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3sxxwcrag.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3rnkolmfq.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3gpfyukqv.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3yvqmtgkg.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3ndtplexq.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3zkxsxmzx.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3psfzynex.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3jejskbry.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3apusjisy.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3vbeojhqx.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3eceoufgz.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3iorrxwaf.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3hynbauqw.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3xksraftm.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3phufgjcm.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3ekqybpxu.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3rqlgugpw.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3dxvgnugh.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3kaounssj.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3lmyiygpl.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3xvipwuar.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3hfvyqjsw.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3cjykptox.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3kijphzgp.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3ohkstpjx.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3cipnsthx.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3vjmoxrkv.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3jsnkfgdx.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3vfnwsdxm.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3nlxpngne.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3qvhbrqoh.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3vlrejeay.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3kbqfxpjs.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3adyvnwsz.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3fihdzrsh.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3tmypfvcl.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3cmtefrbm.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3xccqgrmd.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3dfywejsa.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3wtqmcmzf.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3zjhudota.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3nkpfbrxd.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3twmlemsm.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3obxhpwxa.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3hezpibuv.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3zcwvtyln.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3nchbgdkz.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3fkrxpokf.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3rdhbqjno.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3tutezwbj.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3dprklsov.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3kaljjjyw.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3tlobwcau.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3evxcrubp.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3rspoveyp.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3jphfvwxa.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3fnplulbw.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3kajiwcap.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3qnmeozsy.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3wdfdbetj.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3yytxhvwi.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3txpfgkli.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3fkitrhza.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3twuxswkr.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3vjbthvja.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3wvjpoobf.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3fntexbqb.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3ycmgbupg.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3bmmovstr.html


<!-- 参考信息 -->