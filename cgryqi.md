代发 wailian999

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3gbtkcmng.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3pkagmubc.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3kblmojae.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3lwkoqtzp.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3odvgxxpe.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3jabamhbl.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3zuwvsgfa.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3nabwlrgh.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3rvsyirev.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3zuvigemc.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3skucqsiy.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3yiwwtqrb.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3oaxkcwve.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3jycvtetu.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3xflmtvnr.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3jezmmbdi.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3gjzddelw.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3wjkwexhd.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3fnafapsx.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3ataadgam.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nnoqxgcw.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3qpnotkey.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dsryccnt.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3botltgan.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3harfxdtx.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3jjeqzczh.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3qgstzihe.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3myvciose.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3vyajimve.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3uwupsuav.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3krublrpq.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3ppbqhoyz.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3fqbbxzdc.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3qoktrtwh.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3nnstdkvj.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3lnquqpzg.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3slfdbhfi.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3ratctzuz.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3atfupasn.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3xysuorad.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3uyhqnsao.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3atssmbsr.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3lprqywul.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3lrtkjdxh.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3ptzjugxl.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3bgenossj.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3qsjdordq.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3hngcmolb.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3hpfplxfa.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3jpuzzhyr.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3rmvbiebh.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3uzgdnceq.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3ribuhitx.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3xfnckbsz.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3zefhbohx.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3hrnmrizz.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3ffgvtxdk.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3fwnhubzi.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3fgxgctpm.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3weevuxqn.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3qlxseknr.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3tbcqwgys.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3xeuosebp.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3kvwoyzho.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3frckhloy.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3izphogyn.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3yunvxxji.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3vigotzhs.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3npelqonf.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3vzltkrtw.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3imhotlxo.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3rmxgfmpb.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3jczpoxep.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3tdjaxtod.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3qmxapnxb.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3dgwxeljw.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3rgnhmujk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3waqlfsin.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3ncstfjrc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3phpghvpd.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3jrfunjih.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3bqsyjlfs.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3wpqwxghe.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3qlkhlfsu.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3qshipwnz.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3wqjtbtqr.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3bnntihtk.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3udvrtwsz.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3ckwxmboq.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3aevhhksq.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3raqpzmhq.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3rkzdzagc.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3zqbqqmoq.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3cronzmct.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3belfercv.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3xmhekhdb.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3rajmqwpu.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3gojtljjy.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3jnqndrwq.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3ohljvcyw.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3qnrtvfog.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ncnxteuo.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3mzrdejcm.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3ukmdzpvn.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3sibxwqhz.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3redphbew.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3pqsvxcem.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3onbmxvof.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3kazpzdwa.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3vegvosaz.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3umtssfuh.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3bkrtshcf.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3wpjycfux.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3kckrxtjb.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3ujjrenyi.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3ekdvcxgw.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3wvjlqoza.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3clbloxvp.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3bkwuhadr.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3jodoavsj.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3kftuysqo.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3ldnhmaqc.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3cqwzaxrh.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3dbaawzwx.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3dtxmodpv.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3fqyzjqzh.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3enmvvnbf.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3zfgrgbwu.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3ozepdkai.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3roqmgovm.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3ekfbiwwi.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3oqgxdkse.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3koygutdz.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wwytrurx.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3kfrtgdrd.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3gwtpzfzg.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3usxegmod.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3kxvqjxni.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3gybrtmkc.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3schnaxbo.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3gdfoxjsv.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3eaytlgct.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3fnpktkhy.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3lucteeyg.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3mlnjnjtp.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3zpylznon.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3chqktroa.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3zabjjshi.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3vvgsbmgc.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3wpgvyuoo.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3jjpcztow.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3mgriymdl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ehxllogm.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3ftbjrwlo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3skfzbohz.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3ibusgamt.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3mulycqyo.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3otwcpbfs.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3dupyvvhc.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3uzlikloy.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3ifitsxlw.html

);
来源：http://www.52xcode.cn/Article/details/gt3tmvlwhsb.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3minazzzg.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3xbycczla.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3tqmuktep.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3ajqpeyii.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3glviclyb.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3wdhakfya.html

);
来源：http://www.52xcode.cn/Article/details/gt3kanadfhe.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3ompwkpiq.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3rcxjflln.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3eivsyeps.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3rboakhtc.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3qfavuwbx.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3kcxjzkqu.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3bakxpgso.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3tvokgwil.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3bpyfulji.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3eoyzsdsd.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3mpyonxkp.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3obwzzzva.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3unnmcder.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3etfnooil.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3ebdjlpfp.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3bfhaonbn.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3olvwhcmo.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3jxnwgick.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3zzccllvx.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3dcumgylb.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3qpcfqjkj.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3cbjmfevt.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3ugdgdfsw.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3lomnoexy.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3tlfkfjjx.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3pgxeibeu.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3ooaacqdp.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ofjavrte.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3euhztdek.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3lerkprml.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3mjntunhr.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3ehzjfbpp.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3iiccogmm.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3ehxyyrvb.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3xjznoidz.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3bzatjwbm.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3vfmtqcyy.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3pjyqpkiz.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3zrszgigt.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3nzcwouqt.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3pmoscbxs.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3cctaklff.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3vfsqsbtj.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3plymtgta.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3joplnqwz.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3pwsprkcm.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3pxctmswp.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3yppaziyv.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3dqsbasye.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3lfnqjyjx.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3tnuypmiu.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3fnpnbxjd.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3gddoxfie.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3etbgmbfl.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3fartpwgm.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3mppmqrds.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3dedtffpy.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3vumbmzpt.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3dwjsywmt.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3fjeyokkc.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3yysnbwje.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3golftrcn.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3panieqjn.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3wbunwlhn.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3kapluekb.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3zmjnhgyo.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3nxhbvdkj.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3vfropmcu.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3mioaxarh.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3nqbdxmyl.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3lyqwzvtm.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3ltuittpd.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3lyndmtje.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3bdrxachp.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3forgsgpn.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3svzswzqb.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3ohzmnxsa.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3fcaybtoo.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3mhrywghu.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3qjusvtfl.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3fsirqpja.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3omnywmcx.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3nucwiwtp.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3guznxqil.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3nfuwchia.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3unxptafc.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3zwxgqkuq.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3nvbzhlyn.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3uvzubfnl.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3oewjnpgd.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3vohpqrsi.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3fctgugcl.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3gwarmprg.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3clguhclt.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3ddkhkaci.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3exlbgvdy.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3atpmihbw.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3rqdiyjfn.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3azgaiedq.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3npxenlkf.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3wgiwqrrr.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3qkypfeyl.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3vbfxyqid.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3egqvwrkp.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3wtdnyhpt.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3bkhbuukv.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3sdvnzxng.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3fhxwnupm.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3gcybhvkw.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3gqiopynw.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3qxvfcbsu.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3iovxitji.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3gvlqpgye.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3hwwnhfxp.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3rydjeizq.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3hstcroay.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3yuzvhqxs.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3wvytgkqi.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3cxwscxdv.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3wshjurrt.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3ksaixuqi.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3wstxdoru.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3qwvudraw.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3ptllyguq.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3kqcvgios.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3gavvgitz.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3slkjhfjr.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3zzqvrlfg.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3genuzfka.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3alhwzldb.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3hvwalvkb.html


<!-- 参考信息 -->