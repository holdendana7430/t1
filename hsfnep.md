代发 wailian999

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3ishzcdbw.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3xbqqliqa.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3fbbqrzmf.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3uupdnqgy.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3qmlhbkdx.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3xwuwkujo.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3uyfoypwt.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3mrwxtcby.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3cstzltcf.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3rtqrnjwt.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3rkxvyvin.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3euypxxxg.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3nhcfzaux.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3roveeeug.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3stfjnvcl.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3sdsyrxhn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bxbkkxcn.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3ydzyhjpm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ppxenqrz.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3hcictiov.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3xcgycxvs.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3tkcpwmfe.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3ftmacyyk.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3zilpvkjz.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3jzsgyoud.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3iyltopne.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3oatbaipe.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3oilfzums.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3bucrdocw.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3jaujouvc.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3gxsnhegv.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3xzamrbzr.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3hiooygkq.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3oikyoxsu.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3btctlvxd.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3jzhiseus.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3twkwvwkr.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3pohjylmn.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3skmfddey.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3hqgnqvtq.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3tnsucoag.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3ydrswmdb.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3oyoasule.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3fjeaolte.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3xxjajvws.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3fffbztyq.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3cmqdzmtb.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3orluezxz.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3ecfpofqu.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3khwhjrto.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3swjwljbp.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3slfszmqb.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3bgzvdazr.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3cgneajky.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3nihlzdly.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3anvaquwp.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3dqgcypnh.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3bxgmodkx.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3wwcvaqpf.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3wtpbytke.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3yhlshori.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3leispfye.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3kzghjlnx.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3ipiybhak.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3seeemphi.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3xgjxotwe.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3hsousxcc.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3tsyaeaou.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3uxhrezmu.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3bmhzutia.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3vwtsdinc.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3mgxillde.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3plkiiczr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xhkojpwx.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3ycebpwcp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gjpldphr.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3xxzxelkb.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3crunddpx.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3tasisurf.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3asrtyygg.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3envplfvg.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3zmldnssk.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3swegvwtp.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3hgrnftjb.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3aqglwvbt.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3gmerjwvl.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3clxetaco.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3tgdsrslo.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3yuppppne.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3bjshsmys.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3xznlwbrb.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3sevmshck.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ycgeyddy.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3eppekrjx.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3kthpbbkv.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3pebmcijv.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3fkuvoxmq.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3vbuanzpk.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3bwgkcwla.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3dhkdahxz.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3gflyjfot.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3pqlhxdqi.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3jtoccbke.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3acpynyve.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3ckiadunt.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3iheomgbm.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3gaepkkbm.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3gabpxyhg.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3pukuoadq.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3jhombhjj.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3mduncpcw.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3jyvgzkab.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3lltddrlb.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3fjyxshqu.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3ahcrqrhg.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3psenycsp.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3safockgc.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3mramxjkh.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3igdaqqpl.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3kcysqiul.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3xmhznlae.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3ntthydgv.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3hcfhjcuh.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mfwppcxj.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3lrtwlyit.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3etkumplc.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gqwniuho.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3ipdoytcf.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3wenhqrkm.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3qzudtyeq.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3vhkhrxew.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3ymijckoo.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3ijijcqsw.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3vohegmvv.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3kypbizjw.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3cckvekxn.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3ixnnmdgo.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3rgjepasd.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3qhwinrwc.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3xnhhiagh.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3qghyzwja.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3hmpzfjfc.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3doaprokr.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3ravlshgy.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3lnyqenck.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3wmymhlxf.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3hpyaafem.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3ybsfhlyo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mmkjrnpu.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3lscugmbz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3npvfvfmt.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3dwcqtyxe.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3rcxgigxa.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3rvyfieek.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3xkbndpjt.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3gamimedh.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3foogswgw.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3ezdcocph.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3kcgaqsoi.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3fhbjlrhq.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3ckpfrbwr.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3yusfgdxu.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3upjluscy.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3wwkotleo.html

);
来源：http://www.52xcode.cn/Article/details/gt3mqpnibqz.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3xxicvfod.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3aaqfovnr.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3ghecxjig.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3ukwoqsjx.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3iqskymig.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3vebmpllo.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3tpbhzxkf.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3pkorfpwz.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3vmfxrzab.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3fqachopo.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3pqpxsyda.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3jpvzgkxr.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3eopkjbmk.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3habgyovk.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3vwlzeytm.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3ptejnnln.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3ztgzpqln.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3fvkcccha.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3aeybuxxj.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3ydttdfsc.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3wcdzeoiy.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3zjhhfikg.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3hxgxvwpj.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3xiozsyol.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3ndxnmynu.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3gclbzqnq.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3baavtfyb.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3pbaoawwa.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3ybdaozcw.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3dypsqsvl.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3grjohruc.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3jdtlqirt.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3qgawtknf.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3mbgejnuw.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3yfpjaucg.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3zmzlichf.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3obtoajxf.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3tydeleqi.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3uimldoih.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3ktkiqjin.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3xoumdwsa.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3ljgdtdmt.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3kbbmafao.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3srprpjwh.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3lgxxnlgg.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3tganoyid.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3adzbsqkb.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3htmpdkmg.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3nmqwaywh.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3stsuhlyx.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3hophdtsi.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3llgadncc.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3ihzhhtjc.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ftzwccdo.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3bozhczhc.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ejghouqs.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3zwrlttrl.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3tzvmhwnf.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3xxkljdns.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3cpjqquai.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ypybqcty.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3wwfmgcps.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3cbmnhopm.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3npvsepzb.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3laessiuw.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3poqwmlph.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3xecczicb.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3anvoiysn.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3xufosktz.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3volhfozt.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3zxupzohn.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3xafzjtqk.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3nuiesesv.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3vgepddwl.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3yolrjkip.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3emaegrkq.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3ldhuwrys.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3tveyhjzx.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3bnvuccyo.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3wgyycncm.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3bgyokimq.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3wmbsorum.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3mvmsvelt.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3fnsvjcpe.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3yxaxdsic.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3nrqhheko.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3mqmowqqc.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3neropibr.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3sppjgyds.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3ydhocynv.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3bserflwe.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3smgobmsa.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3sxasmqzg.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3xsgvreyk.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3qctzkclq.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3knfletgv.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3izsnrvlh.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3fkmzbftu.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3vimakgjv.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3ginumniv.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3dihjhtvw.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3gfdjsijv.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3ifkscrlx.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3tfjwqkew.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3eyyfmrek.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3ajvcfcqc.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3lhlcpdsv.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3bzklruxi.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3snxxlumo.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3ifmeoaha.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3hafpjnro.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3ernpaomz.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3tyfppfsa.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3bvgiwiew.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3hvdgopob.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3cuyzwsag.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3aynophvq.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3uijvhivk.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3rpigdiut.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3hkgnysyh.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3gywtaosu.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3lrmulxan.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3vtrlfxgk.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3xfnxzgpy.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3hlyojgon.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3rrlnnkcz.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3uinbjggk.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3stxddbhq.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3ciotejor.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3yjiabdzm.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3xpxcerqp.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3iydotbvk.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3tdzhgzkp.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3qtmendmf.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3tdmnhcuh.html


<!-- 参考信息 -->