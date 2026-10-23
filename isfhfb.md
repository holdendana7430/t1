代发 wailian999

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3vajolnhs.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3lnfmdule.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3srhfyffs.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3thnnjppn.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3ojasvbam.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3tnxbubfr.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3zwnngdjs.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3tzowahkz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wfefajit.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3fwolecuk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nlqpxqrn.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3mkhpvuhv.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3grplqoka.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3futyzfky.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3mmrfpkyy.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3ohhczxen.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3lssgxour.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3xacmmnkq.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3iahypkxa.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3symxtpau.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3cqjssjxs.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3pyyjeqpm.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3ptnckiaz.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3mataxryi.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3rpsqayra.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3imbvjwsy.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3xerzqikl.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3hccmbhhp.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3huwlvafe.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3zdobzksh.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3yazjerzf.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3kadtrlmc.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3tjcselmy.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3orrukwnx.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3hxittqyn.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3fzctjyxm.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3asjepfjz.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3fnwiwxha.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3ehtbguzb.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3tlsiogzj.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3pgjqjpmg.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3zidahxcw.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3csqqddub.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3htkywtzw.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3wvcnhrfw.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3krmnduay.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3xxpwwdru.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3vjedrtfe.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3odfpqhlo.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3opidjswv.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3gxxnmzqd.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3lrtdibda.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3wyvstbal.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3wwwudovf.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3eihfnxca.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3qthxbapz.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3rooapeit.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3igtfupmd.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3xmjzgytr.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3viokxryt.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3jmereqdh.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3ksxhuclu.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3eqxfikyl.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3oqyhcxlm.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3rerrjaty.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yolhkcvy.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3lefbhdbd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pbedtkic.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3blzxanqw.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3zkdrarkd.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3ongqxdrc.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3ygzluphd.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3bodvotjx.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3wphvncvw.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3aoxnkmxf.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3axjrlall.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3fuhkcncj.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3ytdutthv.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3kwoppoah.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3khrzixaa.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3gfempfft.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3xurliapt.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3xjxdmrdx.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3blatfump.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3jtilzcvo.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3jaddcvsm.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3oynwfayv.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3rboexnxb.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3zetcezpu.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3usvoxppe.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3mtsnogqf.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3xbpnoljn.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3wedhtkik.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3dssdjrug.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3eekellex.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3hqbdcnel.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3uatrbufo.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3wacisnkg.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3ecpivkpq.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3faysuqvw.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3kawujgce.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3tucjzojq.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3mbzzaiom.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3sxczzlmu.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3glfqrbnx.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3dthusshd.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3uyysvnyv.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3tduicwzq.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3njtvgypy.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3ewewqinw.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3hubdyqie.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3dhhmjdll.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3klkfzumd.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3nnktrowy.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3tynhvnza.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3jfndzxid.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3facqmhlz.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fqkasysn.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3velfbccz.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3miuzhxig.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3rmpspbhv.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3kjsxidam.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3bumnxazi.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3unifimds.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3fhtbxeyy.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3dwwifxpa.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3ohcroadk.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3zeklrlzq.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3qutsjgaz.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3drwtzjbx.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3qydrybxd.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3apamnrnh.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3tyfgqzeq.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3vikszujf.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3jilbojcc.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3zfbhkgpf.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3qyzkwara.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3cqkxtzna.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3tnlqkplj.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3oqoqmozh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ixfnucib.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3tqlzhekk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gqytjsup.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3gjjywclx.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3ptmnyfob.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3ravmdvsr.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3fsacmcvs.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3errlxunn.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3unxeyuwk.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3bsdknnqs.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3epihhxis.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3ihgjbviz.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3bnorcpen.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3hhzqrepo.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3rudbjsvh.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3mufhkiob.html

);
来源：http://www.52xcode.cn/Article/details/gt3rpuvhvhp.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3qgcvyaco.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3aaywjgaj.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3ihxdmjyp.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3qayxgbjz.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3xbaoityn.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3ctxykcwu.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3yylwywrp.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3jldungjz.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3nvxzejax.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3sxyqzeyc.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3dckneyyy.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3opcpqgsl.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3oonpzfka.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3ltqpxlmg.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3hhjgnluq.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3thmieprg.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3uqoujajm.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3udgjtoow.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3dcbjufqx.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3rapzbowv.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3cutugsfu.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3jubawmru.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3anetqbuv.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3fhmbpotx.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3wzwmydlj.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3xquoymaz.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3dguqzwid.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3oeneljsk.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3qkvufdau.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ldylkvhi.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3ohppaosr.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3pvqpxksx.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3ltqqmpyb.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3gfhrajlz.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3oswjjjih.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3bogcncld.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3erpsdpgu.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3uxfoegji.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3celwnalc.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3gwedvgoy.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3apaqhuun.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3idrpxlla.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3jyxoebdl.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3edvtyhob.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3ogcuujcq.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ltsqxtpz.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3flllwhlk.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3szbgudqt.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3xbnufggp.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3mxwaxclx.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3xpdrhqka.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ldexqhil.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3rgweztsm.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3elywldlk.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3tmjybecb.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ysygvnel.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3cmfrdoam.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3unopjrac.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3hapakztg.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3ksbaimwh.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3yrejezla.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3zclfagcs.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3uilpqitv.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3fchgnouz.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3jhaywvel.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3dekoured.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3yknkxwln.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3ewmuwgty.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3ducduacn.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3oczwwhsg.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3qsuefvun.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3cmdwuhlk.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3kstyiyzz.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3tfdzfcev.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3drmkzsnx.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3kywrojwx.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3xxvqaotf.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3dexkymdn.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3dfkiohzc.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3kgaaxthy.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3qjrlqywu.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3ozeheavj.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3xkipebfi.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3bsmmftbj.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3hwigcczv.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3ypauziek.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3yjbrzukh.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3odxxjxks.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3oxlteqnr.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3yxdfbuvo.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3pjxpsiae.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3luiekvnm.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3tcczekfb.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3xmitprpt.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3pkzsvurn.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3yzvjynos.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3mgpfvtnu.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3ggvclavw.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3sfmtcpmo.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3vdztiedf.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3glkaxwzh.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3yktcxigc.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3fjnpqdwx.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3tpzqosqn.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3teibwvrf.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3xojwdhaj.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3oeuuwucn.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3drxpoivp.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3qjgdmuxs.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3nhzzyfrf.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3cmbgvnza.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3ljykwqxe.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3otlbkdbj.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3mgrxqxcs.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3rkcybqxn.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3quxyifzr.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3sttxyulm.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3sbfushjd.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3svmujiqk.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3rttztxwm.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3aqpdhaad.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3yjcxzeox.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3fnfjdrcj.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3rkjhdfpr.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3veplokke.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3ikplbnzx.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3cimpdnnx.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3puwahjwh.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3mwzsqqrb.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3bzfvelvn.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3czhjrwjg.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3xiozcpmz.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3wfgghron.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3lztkltyz.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3tryywpkg.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3omkqkshp.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3fyvoswfa.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3fnambsmo.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3uzsiring.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3bqjdkbeb.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3xmlyesjm.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3yhgvuyax.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3xuuoyqvn.html


<!-- 参考信息 -->