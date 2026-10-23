代发 wailian999

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3hqtylujv.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3wmyaeztd.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3awlynizb.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3zfztlain.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3jqgfxxef.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3jaaedohx.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3pwpifzjj.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3rwakthhu.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3rjanghso.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3hjqwjtxz.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3xhasiuhz.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3ekvmrjlq.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3zvtaneyt.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3ihuriaji.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3udnsggof.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3bqfgcrvi.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3oaizqofn.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3vxzkxpkl.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3wdczjcbd.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3upanzqrr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3olgypomo.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3boxyoxyw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wppackov.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3mcijooqj.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3vorshuam.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3wiyszbfl.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3hmpwjeos.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3gffjwonm.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3feymtdcc.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3dwxscjlp.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3jmdonpua.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3xauphpvp.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3hfovojkt.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3vpsajibb.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3kujsotmj.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3muldamef.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3bmampplf.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3puyjtcyo.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3vnfryiuq.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3hgpefzim.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3igiemvnx.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3xnoszhwu.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3flasixvd.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3wknkqcpd.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3myvnvkmp.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3btmmyuvt.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3ljtqnucz.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3tkblwxzr.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3nwutjqoh.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3fjevebxs.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3rzhncpvp.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3bwpybsis.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3krcammos.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3susnthfg.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3gavylqct.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3lbcfhwci.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3rpdpbdjh.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3ifjdvuim.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3lpazgwbv.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3lqnepnms.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3arfzfpbt.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3gbaswokt.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3xlywntnq.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3zuqbmlog.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3aiyhzxsv.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3zgniqsla.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3smydkhva.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3rmcltoil.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3nbnkptll.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3wuzzqkwm.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3ghxcqlfq.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3sheclwfr.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3evajxfje.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3cudtppab.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3qqdjdjus.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3lixnhkdi.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3oidmkwxa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rcbestgv.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3snjztmwg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vywwluoj.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3bcfuevtl.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3rkzhaxxw.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3jdctlhbh.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3bwpicgbd.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3irpawrvo.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3pmlvqwdm.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3nqhebkrg.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3ljppklvu.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3logcmxxz.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3zlbwytnp.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3yxrhaeff.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3znbnpdfl.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3inampgur.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3oduafski.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3cfhqgbpi.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3adkxdylq.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ehasujfh.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3axbhwjvr.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3zfoxzcki.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3obcmumft.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3gxlnavlu.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3heysutfd.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3rekiiggj.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3vpuwicqf.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3eqxuxhnq.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3rxwzysyp.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3mwkmjjbw.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3hwrosgvw.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3uwftxaav.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3xdcljxmn.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3oytlpvhi.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3iunupjxj.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3vseafoda.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3ekpyebzm.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3kzcvzxwj.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3yrlzlzjn.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3cajkkxle.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3gbksxxyc.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3xiqrdptl.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3tayoalvj.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3ojwxzhry.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3vuobuuxx.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3nlkteyfi.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3fnmnbdsk.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3zcruanmy.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3aurnwbze.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3fikyemqc.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3dwxxrduy.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3llokzndc.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3zwbhmvdw.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vdlbtdnd.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3fmdnujwf.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3dmwvlpzl.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qudveqxc.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3jecutwju.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3kdabyiio.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3qwrahfcb.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3ixvsucsh.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3vnugipkc.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3nvljuqxt.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3dscvyeta.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3kkojcvbr.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3vqswbgus.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3zfnqjaei.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3izkknput.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3eupdfxgg.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3gbbfiict.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3jbfedtia.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3zbgujzvb.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3urryhigc.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3locwsurl.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3murrmoec.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jvnldpjz.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3tuowhznx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xhgrfzip.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3jpxnutcu.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3cldtqvky.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3svogmyjm.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3biacubek.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3pakeqolp.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3fjtxcvta.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3cunsepvo.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3wmempmfu.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3iomogxjy.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3wlgvcoat.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3gxmigqhc.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3pnajzasr.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3xypiiegc.html

);
来源：http://www.52xcode.cn/Article/details/gt3xirdzuyt.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3vafvbwia.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3sdcxwfxq.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3qfumtnmw.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3xmivttoz.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3jezbwhpb.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3kmyaetwd.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3hflcvsay.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3btsxhoeq.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3rfklpdwo.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3oofmmujo.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3bibgxxbc.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3rmyndjho.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3frxifryy.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3mlmwnejn.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3gkjmjbql.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3veccnyef.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3sxyyvoyb.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3nwfumnyd.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3glqgytfr.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3iawazdbc.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3zozvobld.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3lqydrkjo.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3eyovdpni.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3cxzbtjjc.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3zktfehlf.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3cvknnqof.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3bzwsktlm.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3nsunhulj.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3bhkvoigz.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3woemucfm.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3tqhxdhkp.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ychzsaub.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3lwavmgit.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3scxelqep.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3jhnklxkh.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3czigkfco.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3oohnihxj.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3cejkebia.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3aotyelge.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3riugipfy.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3fshwhmtr.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3skomxxlg.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3yfrqgxnx.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3mhjubscl.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3vpmfppag.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3umbuovjz.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3yqnwfywl.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3hesjopbs.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3dtkfzyrf.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3jevetnrb.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3xmovscjn.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3moutzvee.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3dnrxvegb.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3fuwsafzs.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3wwygwtgp.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3peayvzah.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3pfeltdjl.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3bgsitkqq.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3ogpwlihi.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3omcyvhlp.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3nbhexdtl.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3ejnififv.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3gboswrjh.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3wwjtqfce.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3melflyfn.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3pebzdgmj.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3yrixfzun.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3eiurckmp.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3hrbpibop.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3nurfefyh.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3zifzzguc.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3ighhxboa.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3sofkyhvu.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3lbvgqffz.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3zxzixzif.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3iefqwffv.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3rxizwsln.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3wrzqjluv.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3lkdfzvev.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3snbffuct.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3evhpmdfv.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3ltdjuyfy.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3lbzkzalm.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3usrbdmyk.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3yolfopqv.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3duxvcond.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3ppiqlfza.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3ocfvnszz.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3cbrnzjyl.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3jjchtvvb.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3tardlpil.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3kqvqumpz.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3cfevdtpm.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3smpcnqmb.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3gimqmqun.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3vexckqcl.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3znflkkpd.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3lkesqivm.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3hcrmnsqz.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3dwwraadi.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3ebkbyhro.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3wewvasjp.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3vdayfhjw.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3wwkycdar.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3rytugxlm.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3awosktty.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3pnelpfqk.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3kmqkxgtr.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3xjydwwez.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3ahrvugoo.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3wqkmlosi.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3lervogmk.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3hirnodku.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3xjeeaknq.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3lguygvzr.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3akstmven.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3zchnnrlc.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3gngshmcm.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3urirwvvo.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3xpgtqefv.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3jjdrktmh.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3lgpbbvec.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3yfkaazxq.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3riwexbwx.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3eblmdkih.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3lpwemsie.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3xolivubu.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3vcxatjnj.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ogyrvepr.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3hzoksmhp.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3rrhscxiv.html


<!-- 参考信息 -->