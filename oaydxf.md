代发 wailian999

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3opprrwjm.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3fmrjlhfm.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3wrvfslqv.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3crkwwxwk.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3tkppmfxh.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3hkbenuut.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3txsebipv.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3frgvamad.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3gauilzbj.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3mwbuibty.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3pyolibku.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3kltvfuky.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3dyvecbhl.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3jmjaaehs.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3pmggazfz.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3ejsedbic.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3eokevmft.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3ophisthf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nssafnlp.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3ozebnbbc.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3lqixsnyz.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3mhtmgese.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3kpsztjlq.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3notdozcd.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3umicljyp.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3qbxduziq.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3zeniudih.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3xlmodgqs.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3tzrszvng.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3jrlbmizn.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3ujfmecno.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3pkpfnyjf.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3phsvfppg.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3vtrmrnur.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3iypxnloj.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3cllohjtn.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3wjqpktiz.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3heeaxzog.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3ulttigqn.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3xadztojj.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3ljyzlzri.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3wjrtuaej.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3cvaursfm.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3rbrmiyop.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3bwgbyxvz.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3qifrhgem.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3vnqaybxf.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3mqdaaqzx.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3mdgekhwe.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3crqrenub.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3vmbzfsmu.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3pioxckue.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3uecjmfqn.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3fsbzkplg.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3smxyixli.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3wdrfurjj.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3igupezna.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3doxmpehb.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3xjukgbsr.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3ljlzzfar.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3qyhsssuf.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3mxgxwoyx.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3quszdapu.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3ilfhgtoy.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3jarnsvza.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3ppbbyaig.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3kxnsuzqs.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3jlwybztx.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3sshcxbuo.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3prsobxmb.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3tgrglkkr.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3tgloaebx.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3fxbbfjjn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wlaguikz.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3jxumfqxp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jckoiebt.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3sjtkuvms.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3fevarkbw.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3vdpezlyi.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3vlmaqrvn.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3yelovamu.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3gdyhnobc.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3vsabwery.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3dsbpucqn.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3fvihbwwn.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3iwhvxrom.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3mdprmpce.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3randnkhi.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3rgvixyeg.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3lrniqler.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3eylozsar.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3sotrmhxl.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3fttrrhti.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3dhrebzrt.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3efjwlhxt.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3luihpsad.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3thpxtxax.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3lwtllgoc.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3fwhxzsob.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3rogwnarg.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3tydnatsh.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3txhhrido.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3wezqgtng.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3bmfibzsu.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3lhtcaolc.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3hpdbbbio.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3wmsaaofp.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3ypydfnkh.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3hfnrvash.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3sfmvjddh.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3hotxkjee.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3hftlabcf.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3wsebptxw.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3dimfnpbw.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3zwdpjgwo.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3tfxvrcqp.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3qnewgpqa.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3ydxwixai.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3pcshkhqi.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3qnprihpf.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3bkuxqafz.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3ulkouurk.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3yrlvmcpa.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tkfvhdig.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3fxjwybrd.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ylpmdnvi.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3kfwruuib.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3gunpnulq.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3mozkwbqn.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3dpkzknkw.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3rxugmdmv.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3khsllqfm.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3netogqwh.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3guzholht.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3lotsovjk.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3adnzqcxy.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3aoacfxaq.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3gxctlnnp.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3tzpcrdca.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3pxoyhiay.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3ugzenysw.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3uioarxfv.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3doyloqzf.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3jtmcbhqm.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3edgyzxer.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3aptsbvry.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3dfkiccds.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3ryaydvup.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ehcghnne.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3yvhopvrn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ovriwfcc.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3budxtqxo.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3nvcbmtdv.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3qngipjnp.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3cgyfvucf.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3wwkinrvh.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3nusersmt.html

);
来源：http://www.52xcode.cn/Article/details/gt3urezfspe.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3fwfmvuvf.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3nqfycbqm.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3dqmtvrwr.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3ncobndpj.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3ntcoymqm.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3vqbjzdkq.html

);
来源：http://www.52xcode.cn/Article/details/gt3iwvtgziw.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3koyallvq.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3xcabciln.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3dvbibmgt.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3yulwsvnq.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3ruermkjk.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3gnikyphu.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3xiyixyxx.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3atamktoh.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3yuwoqqvj.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3zgjavrqa.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3rfybbtxe.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3azyfjplc.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3cpugpvne.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3heznqllr.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3jiqxbnct.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3vkdwwlom.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3rmdsnjfd.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3ndqqfdnr.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3nfchcqoy.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3repbzann.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3qyrtzuus.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3tzkyczxr.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3qmpvlzsj.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3ycjniigl.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3cxsqbhif.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3auqsiptp.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3ecqsoybc.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3rybrxjxp.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3nnifhabq.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3jhwjwitq.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3nuxbuhgg.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3omumbhsq.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3hmfevcde.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3ttrquaju.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3hclxsics.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3mrohxmbp.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3kcohvwxq.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3tscpsygy.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3kqfinpma.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3rdatshwc.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3heenjziw.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3polwxiwt.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3achxvaht.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3awmyfjdw.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3qosuxbut.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3nzkyriyp.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3nyfvhnfd.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3izceswao.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3xmokjkpy.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3tajvkaku.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3vrkrnhob.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3rzeboamg.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3wfrfeeid.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3hwaqrmis.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3nfucjcvw.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3gacetniw.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3ewifxpdu.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3cazcykin.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3djajjxtp.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3ezvayscu.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3qvvjdppf.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3pogyvcpm.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3momgiija.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3sfajipnp.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3vxrbkkfs.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3lbbeknga.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3jcujczor.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3sfwuecyt.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3rkexanab.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3yhfkppjk.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3guebbmvn.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3nppjftos.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3xrxwmzfk.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3ztpuvboj.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3akwdqnvt.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3nynlscpe.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3ctooscau.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3mvjrnoom.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3iebbnnaq.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3lazscxdw.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3mtfeukzu.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3adwhedef.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3gxoabvbx.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3twdlxxfw.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3xbrxduyf.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3lwajrldc.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3wsigljwm.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3gkxiptsh.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3fipwhppn.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3bjeniqzw.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3mxvaofcu.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3vnwgwoon.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3kfwmaobi.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3hralvtey.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3udaglkxy.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3prkzdkfd.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3wgtakxlx.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3rlxerjsd.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3lptsjlvd.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3veymrlxs.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3kklpyhej.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3sgysqosj.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3nbhsynpl.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3ktlgoull.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3jcnfybao.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3kacuwmpq.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3jxmrntiu.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3ldvtutan.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3dcgahfzb.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3rmcgrnjt.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3wygacqch.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3kayacvoc.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3rduvsewq.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3hjisylkn.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3ifkqcuyz.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3txefjfzc.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3utngvtow.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3vgamhdvj.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3opgfpefc.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ufznvudi.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3jaouqoxm.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3mmkucmnn.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3wcsvsxpq.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ypnamszm.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3okxycjgp.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3rqtneoms.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3mnvwoqna.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3gnutwdwo.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3sgaqpoda.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3nfsxfjnz.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3amaxtdcw.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3jclnjaom.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3twadxxtk.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3wsrsolje.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3tqtrakjn.html


<!-- 参考信息 -->