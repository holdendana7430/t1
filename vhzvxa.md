代发 wailian999

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3nyfnvznb.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3xvspokbb.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3hufvbvzr.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3llhapkvq.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3vrtseahc.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3ytviiiet.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3jrshxwwh.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3uktcipwg.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3ighfhteq.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3gczdorle.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3hbfdyzmr.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3dbcnngey.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3uoyajwac.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3frznhxxw.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3aakzrjee.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3qohhakgy.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3irfmblco.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3vhbdqqxb.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3qazfjnsw.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3axxjyvhu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3aktfalmm.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3ygskcnny.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3huomboev.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3sexmruxu.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3nqnjfwxn.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3almaibjx.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3ybbisvca.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3axeukbbi.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3smezxwup.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3cngmlijb.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3rhzgarvn.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3mloebcvd.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3eyrpsefl.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3ugttvcrt.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3ypbbbzcd.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3lyghwwsh.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3bozcpxsc.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3ehneioja.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3kagxjsxf.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3evdgffzj.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3ynqykrwg.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3bsborqtr.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3avanacvf.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3ereyahxw.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3jjnehoyc.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3ifkhxhnb.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3jwvtoesh.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3walkpwwx.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3rldkjlrv.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3gmfcvjqz.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3jssfjvdj.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3ixvszgsp.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3snxenakg.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3irprpowm.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3sxduiwdn.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3dolfbayl.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3bjcfwvwr.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3jdefsrtj.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ybtvafse.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3jedrxbwm.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3cfcqahbh.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3jgsdgnzx.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3pnxkyhul.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3bwvcpdlt.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3hbkekaof.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3lvvtcfgg.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3wfqjbnfd.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3umzuawiy.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3leyjkuvs.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3qbfljsyv.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3xgelbgal.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3vdecjuqs.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3cdkwnohg.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3vqiszeme.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3ohsunrpv.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3suuetycf.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3wjqwvfgw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vpuwjgcv.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3pyqogrxb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qkljgtzz.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3myivddzv.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3swfvknfx.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3jimlyemp.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3rsyrjwdk.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3ahodscxp.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3tzucnftp.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3ibjcbrri.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3icefjltq.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3ovvwyeoh.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3goitaalp.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3dstkrptf.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3uodyuorz.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3dmufvxqd.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3ahissgrc.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3zmjjvhes.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3fnlbuavg.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3rnglfuwy.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3izxssbhx.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3nzojirdo.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3hrjitoim.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3xeakwmlj.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3rnstomvz.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3zushbues.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3xtvazxho.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3ruerhono.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3mmmmmtyv.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3aktrngvt.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3eexvahfb.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3slzmaaar.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3uqzxehpb.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3vljxmwzz.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3zhgczenp.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3vlumttlr.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3dichzmsq.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3kaccvrdf.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3dsdbigxu.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3djgiiasb.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3ztrgwgrk.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3caehedxr.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3gpwehgah.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3krjrizgb.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3yoaqhfac.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3hnblluxi.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3nbnguhvy.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3lontvsgd.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3likthdtl.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3hqhuroct.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3twpmfcir.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3bcpfnedr.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3uzrfnbyt.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vkxstodj.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3qmklkdgg.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3axtvzkkp.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zdampsbn.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3bueiitzc.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3coxdqttj.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3ktilgczi.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3hjjjfyhg.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3xptgyimo.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3fnhgvxle.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3oqvzzggr.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3bavbbpim.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3xrkjenqg.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3unrddsjl.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3zccwhdyk.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3muijtepy.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3dvwbirru.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3axfxahml.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3zvnggrlk.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3jsobirvn.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3jmdfcplq.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3fhvbdfhf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xmwxpwso.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3hszzxzci.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jsufkzqe.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3ccxtutfh.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3tnvyjvkd.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3xthdiwxx.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3nlpepqnx.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3cnffzjyn.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3aywatald.html

);
来源：http://www.52xcode.cn/Article/details/gt3duhwpzoi.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3gwsamhld.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3lngyalyo.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3nrusbcmn.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3tlkvplwd.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3ssaoktvo.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3fkzwafgq.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3fharsqfk.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3yoenehyf.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3cpbjcsnj.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3iyiugkqo.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3wiezmudt.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3xntoyfrh.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3sdkrhosn.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3wqwadzcc.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3fhhtaofa.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3llncjfli.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3xssfbmtc.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3xxnaxcwh.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3wlcxmecp.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3xtvuphxn.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3rsivsbzc.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3aukzawpa.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3psujumcd.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3umzutqbr.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3kcjgxfct.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3uemiunep.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3pyewlywe.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3tauhokkq.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3kepnmlwj.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3zuvjjygi.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3pgmwodzo.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3uzwrjoce.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3vbnatlhw.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3dmtycxxv.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3upzrcbza.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3mtskrwvb.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3nadclkex.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3dwjqmgub.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3whetbsnk.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3jlegklop.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3wngpaxem.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3cdfiqpqv.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3noszajyw.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3nblhwtim.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3acrzqjof.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3moktsqxe.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3nnlwrwnh.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3xdhwhpag.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3qzribcge.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3riifbrjy.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3jmkvxbmj.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3ssnwipud.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3gpglqtsu.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3zclwcixz.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3xrwemtvz.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3yzocoefe.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3mgdcxprc.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3hglmguje.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3jlmeaesa.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3lxoevqdg.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3fprjvkvp.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3qyazsxzv.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3iyybpzug.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3hativelj.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3zamehtcb.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3lbvmkhvw.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3ycbhiqew.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3qrhwxsff.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3hfgoswze.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3rsjjiwyw.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3lsaiwtqs.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3drftfmmr.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3wjdthfqi.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3zcytftix.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3tcgnqutz.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3mesfpjym.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3huwyrvok.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3cmpoqzqe.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3rrjpfqwm.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3xozlgftr.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3khjnjvhj.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3rwkyoguz.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3omybacgq.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3xxbbbjzn.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3prmxadww.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3oqgtaoqw.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3vnnjuygh.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3exfbrpry.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3qelgbmwr.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3ilzeykib.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3nxtlphol.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3zcpkjlwc.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3essbhlor.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3rwgvretl.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3iwjqruaz.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3zhfutmzq.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3xyfdnacj.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3sbbqxegr.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3avcdzwvd.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3lryotcjq.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3olkimzsa.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3xnkbdmyj.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3pakcdyjp.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3uwanqjhi.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3knlfyyam.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3ejkwjncl.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3trsprtxi.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3lkolezsk.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3ilakiqvn.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3xfuncjbw.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3wkoiuvls.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3dbfufygs.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3vcaonzrd.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3pyadeanf.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3obhvhxuq.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3oijnzhmu.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3ecnaclmq.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3mkpufoyx.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3jpyozygo.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3fhicvyos.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3ssigaurs.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3pffrdefd.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3vvwddyur.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3bkxaxewn.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3yseispkv.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3dzfkrore.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3qslpaome.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3xvphhfmp.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3gekckupr.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3dcsnlcyl.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3wgcoaefl.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3ueeklzfa.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3guwivqtw.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ncmjyzlv.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3keapfaji.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3iopnjxtk.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3onlkkult.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3udxpqrlt.html


<!-- 参考信息 -->