代发 wailian999

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2dwjnfgcj.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2qwrcdnkd.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2etvybsev.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2beoksknr.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2gayellqb.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2ivqywvnb.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2xnmbxzrr.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2gmrrlamj.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2vnqmjgnf.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2peeesrjz.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2irnngxgc.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2emxscjcf.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2jvqneqjd.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2ozyqufwa.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2dfqlkxct.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2jwbxrual.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hwjsraag.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2buabyzwk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jzzdqfmu.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2dnbbubhv.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2zrihemal.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2pmlccznr.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2ikrunmhp.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2qsjsmuhr.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2esgbmyjy.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2pxzgkizz.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2cmfvjvnj.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2tijmfoil.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2njutxipe.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2jtwhphpj.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2ceuknlqk.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2qjgiodme.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2boziarax.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2sscdtykx.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2guvkffhi.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2rewgmjnd.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2qtwlftvh.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2vgmsohzh.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2kaddhucw.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2jusfsfro.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2twblvodw.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2dnyyxhon.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2kgnxpdbp.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2omqfggtk.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2tvsdfeiu.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2pzftcfcp.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2ixlgpzii.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2hiatzrqf.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2qfemlmqt.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2nbzqvubh.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2vrpqvruj.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2vrktegxl.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2ezmotbgi.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2vqvckkvd.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2phqspiwt.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2gbotidwk.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2empgemmy.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2czzfegcz.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2wwajsuws.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2ecfblgrc.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2joadolev.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2uitcrdxu.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2uxkrokun.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2ueknaqdm.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2tnsnijcb.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2vsslaewt.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2lragnuqx.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2wqzhfkvb.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2vhytpqtq.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2uyktmluf.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2lvstoser.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2atiyyqlu.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2fzzfotkz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ndlctzaj.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2ozbfljbp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tsjbsvca.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2dbdbynjx.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2jkkbytta.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2lveiqibb.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2qoxghyqv.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2miplxamp.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2kqhhmdtk.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2fcqpxswl.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2anqwdkuk.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2jmdvtmbf.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2futmojmc.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2nerzqcfu.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2nwfurpnz.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2lhjsoqqj.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2zmwkvkvj.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2pxoqjoek.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2lhckclya.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2gmmnbfto.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2vkggvtqu.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2crzhodzg.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2fleqltem.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2ypruejbk.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2pelqxqnz.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2ldppqfyi.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2nitiscdw.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2wksiiwzo.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2fbwkzjka.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2ealclykb.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2lukmebsc.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2ozucachb.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2tqaubaij.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2qhzccjaj.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2zdugujsb.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2wmuekbdp.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2hqwcsfmj.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2hsccgvml.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2lbatxuxz.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2oglgscxj.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2rfbikcht.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2kntgtgto.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2ajjvhumu.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2euexhwka.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2qdkzgnhq.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2euljyaiu.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2hutjfbba.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2dchsdtff.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2fehfbflg.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2ogtvepux.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2cncpldaz.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2tnchllgn.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2nwljblht.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2cdmcvpop.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2xonrncwl.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2lxwheflq.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mlxmatfw.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2shyylduh.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2cvgsdxmp.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2nrqjmvol.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2tcilhhuw.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2ueuibpjr.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2erjvzppo.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2emepgnqg.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2ivxruqie.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2fqcslklm.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2gmbkdadj.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2hakplwxz.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2hfczsgxe.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2rqjuvggz.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2nayvsrmn.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2udxgdpvh.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2qgimykyd.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2kmwxqurp.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2vzejxych.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2atuzhyip.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2djcmhefu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lnzrunez.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2rkxiqosv.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2zxzwzsyx.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2ojypzevh.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2vrqxnlyw.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2gclozsau.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2qdfvhgdx.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2jxxszosb.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2llpeadqk.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2tmlblbkx.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2nojvvoro.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2pvfofcuv.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2ygyegzrd.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2lzgbfskj.html

);
来源：http://www.52xcode.cn/Article/details/gt2smtrwxao.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2ffeukauq.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2gabjsvpm.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2nluybgvv.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2vhobbuad.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2vbieornh.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2lxintepx.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2ozvbrhns.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2lzmogkdd.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2fhcxwrff.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2yzcurjtx.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2yfnhboju.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2akczuwng.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2lrdpiyri.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2iejwktkn.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2iktchwgu.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2oxzabhhe.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2ejdqlsnh.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2kqnnyqbd.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2ujsdpbbr.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2uddkfbei.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2jxndvzxx.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2cvjykbrc.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2irrxpmij.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2ipmllajs.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2gvhhhwbp.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2tfzrfada.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2lhipddib.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2talmxklw.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2gezxtuqo.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2rlamtkvd.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2uejvijwk.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2zolaqeor.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2nyoboija.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2cnqarwli.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2nhwvcjdw.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2whcgmcrz.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2mgjsylnd.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2whpezkvo.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2llosdlvl.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2hjrvklyp.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2tqzynugy.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2hjbkyudz.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2pvwxtysw.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2dusdiftz.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2dliynneu.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2avdcbotb.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2zjvvlyet.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2szgxetsf.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2pysfnltz.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2lhdpkjyk.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2fhcyqfhn.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2zmceuhat.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2fwasvdpm.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2htoojrws.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2wnwnxbjg.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2lwzamlde.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2satgizck.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2rbtqngus.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2zzzxkdmu.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2zhvnjvtx.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2gqyyxasw.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2xfumbkdm.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2bcaebqpe.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2kwnugfrq.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2rntjusft.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2paymynhu.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2tkfgbmya.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2iebopmla.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2tmgsrndh.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2nhuatnus.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2rqfgkylt.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2koimhuhw.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2ihdnlwxc.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2nvxfbypk.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2barfhsoa.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2ajgtkzld.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2giiuyjkj.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2kvbozyym.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2yqmrjhrm.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2yldvdmjm.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2rwwtzowu.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2ysfzwdnb.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2zjvvitrq.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2pmqvmzsf.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2mqofapny.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2dbaqjtyi.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2mmovzqmv.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2acbcrbba.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2keheffcx.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2qolfxxaw.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2yckjbqmf.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2kchuodks.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2pldgdnvp.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2uzhhidim.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2tjvosimu.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2fatrwblk.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2prgywvod.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2undyalpf.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2cbnjhegb.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2dioqkqzn.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2maafnisq.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2pwxomqbu.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2woztient.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2zimcwdni.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2eocedrpz.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2ddsqjrak.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2qscviaed.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2wvokfayj.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2iewuyqww.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2yzmsqvfe.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2pbolpryq.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2iznjiaoy.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2mtmchlwr.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2mjdmrbww.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2jxcbmgqg.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2jyxgcspg.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2qvlpzmwt.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2cjinxyxd.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2dffeptpg.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2qjdvhmog.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2qtygqzaw.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2weufiost.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2dlwdtkhf.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2xbdkeijt.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2zqpxoamx.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2pwjllyyf.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2zgvhvggo.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2xhaerfmf.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2yhswdebe.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2ubvsewti.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2aolqpins.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2xqfblacm.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2dzdwmnnm.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2uafntlkm.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2apgepbmb.html


<!-- 参考信息 -->