代发 wailian999

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2mlobdube.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2qfdsgiaz.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2muozocax.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2zdvawjgq.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2xqtlwmkj.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2nbytqvqa.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2ktvqzjcp.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2jbwemmqx.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2ajsmaifu.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2trnhjegh.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2ollydlxt.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2sblutlbj.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2abbdcsic.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2ucqvehrl.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2ahcubyvq.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2kaeakauc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qzgghyjd.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2gcxglcoq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hpakzawz.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2pareqowl.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2whmoqmcs.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2vemqmofm.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2xgmrvuox.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2rcgcsojo.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2emarfofd.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2hjpwqdbe.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2gkbxuhbs.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2nsnoekyu.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2btctzzkw.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2jywolvvy.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2vurwykkt.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2hefrichs.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2djnjlrca.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2dnnwutbj.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2iaydnqaz.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2famycury.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2miiralrc.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2qdcvvvpj.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2ecpwwwcj.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2tsdshetu.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2uomdqriy.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2vpxljnck.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2zpfypodz.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2iwttenyb.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2lgqpzrlr.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2nywbllsj.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2gfrjeeub.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2mddtdjyg.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2mgfsdxna.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2udiootmz.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2wuvouapn.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2sonlvtwq.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2fottunca.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2nltvwdow.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2hdvdydyg.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2ygoishej.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2lckndpap.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2vbrquwtg.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2hkthoyvv.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2wekeoxks.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2atbaraft.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2xybmcgib.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2ikzzhvjn.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2hvabkmqg.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2hnjypnwn.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2czatlxuq.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2ztixcqin.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2tkgnucld.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2ooamtiae.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2mxuczopn.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2wklfwlgs.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2vgacqlyt.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2erpbevkm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fveyxcag.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2klgnourj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ceirtqme.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2cbefvdxf.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2ywkrgehn.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2ryfmxmnb.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2ovgbzaet.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2gingnimh.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2nqeglkfq.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2eckbeteb.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2jvgsrgec.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2mdxlmfmg.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2obmcdygy.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2jsrlwfgq.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2hnjpymfv.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2tljkrzqg.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2ummzgulm.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2hldnqyyu.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2pnrugyme.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2xxmsdjvo.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2uvxtkfxx.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ctfusscd.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2lonzrpbz.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2ulimikfv.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2lzwmusnn.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2yfvwsspm.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2ejaerscj.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2uzujoepa.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2qwbifqgl.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2zaacnjtr.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2fkhhfxbo.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2etlhwmmv.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2hmcyizfc.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2cqwhqwcu.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2kgsshvmb.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2cwmweadu.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2gkhuazha.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2kcgsmezp.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2mnvsncua.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2srhlhbfp.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2xncwhcgm.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2ykkkpzkv.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2evrjgylv.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2bubqpitn.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2ecndhsjp.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2cjgjxrur.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2tflowuoa.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2itrfvaph.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2havatyzw.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2sngckavi.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nvfxpwvt.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2lijxhqfe.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2urtosdub.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2oqnssmhs.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2unfxnzwd.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2oiglljdw.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2idmtewxq.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2ukjociwd.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2oczglwxj.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2jwxnitfw.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2ugjjvoaw.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2glbochfk.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2jplxsjcv.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2cqnckpgo.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2zzcxihan.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2ptdlvkuk.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2ojlwjsyx.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2inopykgc.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2fryksznx.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2axsawklx.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2pjtljjmd.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2zuhwkpgw.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2mjtnsfir.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2vohqdfbs.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2tsqdtihu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mrecuquy.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2fnmpqkvu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dqbguoqp.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2oukhclww.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2luguilfn.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2wvyukhlt.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2ezibatpj.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2gxmqmxkt.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2niwlpktw.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2wumbnamz.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2eqajmrmr.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2poivncht.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2gaydycwy.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2gjxdqdjo.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2ktrvnpmw.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2zpxvowfr.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2dweamehm.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2khnwctru.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2ivrtjerz.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2ewmzkmyd.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2qodmjoev.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2ewuvprvb.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2gnwsoviw.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2pjjdorrm.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2seoxckei.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2kkjehbnl.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2dukndjoc.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2oadfexuv.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2rhkgnplx.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2mmqzicbj.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2uwugempo.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2ddxepfqr.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2mreanhww.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2zckwbqen.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2sxjuewvl.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2aivnjsym.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2udbquaiq.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2lqzcrjzz.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2jpjpuhod.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2itwwmdti.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2ksiawsso.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2kzdxxghv.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2rzarfpwi.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2wjqorwsv.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2bvpmoing.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2eqpurntt.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2cklddlhd.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2uxrnnunu.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2ecgvydzv.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2zsvthfcp.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2yuwncfiy.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2lvpxfsvd.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2yfefdwzz.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2smfcyrfy.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2qcfmhckl.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2bahgytus.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2ebmnnlpn.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2hmjnlnqz.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2rqwqxbzs.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2aiwqnnui.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2azihwcwl.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2rpcigdpd.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ehdbedud.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2prflfaxm.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2dzjfemlf.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2zpklhcvq.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ciqwptgz.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2usrxbmzx.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2oowihjdj.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2osugzzqn.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2wviwtimh.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2xhcypyel.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2mlkfkiod.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2rpsbmqjv.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2uoojtowr.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2xoocpnhz.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2sppfspek.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2fqmkoecz.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2evuyebsh.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2mbrqfuqf.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2uwefkjma.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2rwcbcquh.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2uqsqejhj.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2oszsprml.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2nnpqbvce.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2lkvwautf.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2nlwehemz.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2moqgxpyr.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2ksotvkqf.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2wemzqkyp.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2kekahymp.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2kitqiijq.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2ciuekapz.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2pviaeqoo.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2ewydrzmp.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2zudtkqka.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2ssevtafi.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2cnpedzcy.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2szbdobih.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2vkftutrb.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2grjzwhmn.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2litmiwrq.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2eoesezpm.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2ceygqmwn.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2yhmwcxuc.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2zipfrozw.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2ziznzheo.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2hmidbiyp.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2pbltgest.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2hosdquhd.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2jdknmkyi.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2dzkiisyh.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2nzdnjnfm.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2pupoeylt.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2wikvjczn.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2qqrckesm.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2ikmdtsjo.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2hkjkpefg.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2zzwtvjsd.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2rgmldlpa.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2ntxtfpry.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2uzhuqatm.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2ystqjyyb.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2jyjlgnes.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2qdpzmvvw.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2mfpaazpz.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2sjkyxgks.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2pfqrfevi.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2rghjkbyb.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2usmdwvzd.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2ekzpskue.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2jwkfzegx.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2ysniiyjv.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2nphavfit.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2nvuswixr.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2owrfjttf.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2nacdcgqp.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2zrospzkf.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2dipqxpza.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2animvvhr.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2fpulpwci.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2ybdotpmc.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2gnnulprd.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2orusrxxl.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2iijkywin.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2mvhxflbv.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2gqfbzwzb.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2aocjmnbc.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2kytxgmwj.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2eknqssef.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2vfceznwi.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2nlcyxnhz.html


<!-- 参考信息 -->