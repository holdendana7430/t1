代发 wailian999

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3esukqvjt.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3ajctuwml.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3zstrxulr.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3zcrvceaf.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3xbqxexlj.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3eiyalwch.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3vwygktnb.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3kqpohguu.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3ntnptcnt.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3acnxngec.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3yqqyztyk.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3bkozfamr.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3pepzbeyo.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3enqdmxgm.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3kjjgpmvb.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3fykmmapy.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3tzhcchfb.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3goprdsqe.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3lfdmamev.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3oegwsbwj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nibrfhlp.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3qzprhwba.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fityyfnu.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3rjyogoyh.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3ljyknywe.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3vkfjxwxt.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3gugavjkh.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3ctealqam.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3jqgqnopr.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3terdpuxt.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3wwhlsyiy.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3xupmzunq.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3mmdlkbkm.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3xmvzwsvx.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3sfvcjpdg.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3fvfajwpd.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3swrvbyef.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3wxmiwcmt.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3eimytpza.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3gbnfmlho.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3uydjtxuo.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3zbightja.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3ejldqccx.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3bxnkdsut.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3larzchtq.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3gndbvqda.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3cdywgwms.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3dvqwgxoo.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3alsnwudd.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3pqizxrto.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3qaktremu.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3xczfbmir.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3yyrzchtb.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3frbibart.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3gejyvgmn.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3ambpyfco.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3qcsmtnou.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3jhijfmxe.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3fmngruoj.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3bepeprck.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3istacpro.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3slyfppai.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3mnavigun.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3nfwsoxhy.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3ezxruwun.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3ihtqptwr.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3jygqdrdj.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3vqreqnfw.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3pqucmwip.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3cvctiwvo.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3mnlxicue.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3leknsktc.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3mlomouqk.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3tqkjosds.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3nygrtjvp.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3gyuufjbt.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3atqvbtwn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rghltska.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3peejhgcd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ckgukhwq.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3coeixdqt.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3fniaamoo.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3uxszkccj.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3qdtfnarc.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3mhjoxxyo.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3ekzdwacz.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3igupxejd.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3tvsrmobe.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3oyxudefd.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3tqdgpgfv.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3ccmkejxf.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3vshmfepy.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3tymyztwk.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3yahqxbks.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3dhnohlwy.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3zcrwzzbr.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3ozjbabot.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3qkozhric.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ncddkgie.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3dlzhagau.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3svhpaywt.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3vsfxtszm.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3gohkqbnt.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3ytagheuy.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3fsmlyvrv.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3dmomkvfh.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3xinhysvv.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3jwsqqvew.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3nxwpsxtv.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3lxlpuqud.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3bnhzhtxa.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3eoelyzlw.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3bxlvffwa.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3hdyaexgm.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3ghhpbbml.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3mleowpqc.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3apinnymi.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3yycktdmi.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3ndyctejd.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3mgiyrfrk.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3bfgfljde.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3ukslubno.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3brpdrvde.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3sjvhygvo.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3mhqzjzrg.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3gogwsgqo.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3gjqagcxv.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3oxhojwlg.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3pittuhol.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3kmjkzpbo.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3bldttchm.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3yijkiuto.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3ubdkdphs.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3dzuudiaa.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3zvvivybc.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3ragysxbl.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3kqhbclbo.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3ecrbbheh.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3nkbzyzep.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3jbrmncsz.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3jaqefvlv.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3sohyzheo.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3ksqjiqab.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3uvbnroxo.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3tswakhfo.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3xclfocpd.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3nbgctesy.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3hrirxmor.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3sduldnmu.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3zfyocoin.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3ljrzeggo.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3plgiumbp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3oxtyjxow.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3hboxxwrz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gvlqtlyc.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3igguxmuw.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3qsfozpjf.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3umpssvor.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3pbovndgn.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3khrqosaq.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3gvlaioiz.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3konymlcu.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3bwldownc.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3kundjlho.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3aucisjch.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3cxuwlhrr.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3syxwvzda.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3dmbclvtj.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3zcuyxakf.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3jcpeuaer.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3ttwdnubw.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3nkiblaqm.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3qfftuxvo.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3osvhcrhj.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3zkhifwmk.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3mstoiwxh.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3nadropvm.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3dyereixw.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3xylwvqsp.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3pshutedu.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3utnmocgg.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3dvbuluxc.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3repzgrgy.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3yjjjgsit.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3wrrqkhbp.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3yhmovbbt.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3wehdhile.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3qmkicbje.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3vmidubfa.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3ffusgpls.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3uprutdkq.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3qlsfhsao.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3xeycjhks.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3csriqtyq.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3uydtimkk.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3djttdfxr.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3yvprhojl.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3kbbmksnc.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3gpahknar.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3quaasdfl.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3xvolosod.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3zezephem.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3fqkiycgo.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3jvaiaafc.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3xabcddtj.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3gkylrjle.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3qlahqecn.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3rmgmvuji.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3nmahgsyn.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3fhtbyxjj.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3ytsmgkoy.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3vbrnemdx.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3saxmfvfx.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3excixmoq.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3bzkbrfku.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3nzzybqgz.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3pstrtngx.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3aidkpdkm.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3sisobjjy.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3blxarnvs.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3isfskysb.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3dnvcirgo.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3xdugviis.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3hsfrqrkd.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ugbuvztv.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3dsqhfape.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3rwgptglj.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3pfvgight.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3fodncibd.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3lhipwoxu.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3bdgvkfrj.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3rcqaqibc.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3twmqxysv.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3wdijggws.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3ysotnrju.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3mtkubxzo.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3txqhksol.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3iiuiwavq.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3bmvzpzph.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3qnhdxlcx.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3uzaurirx.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3oqqyvlyk.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3vnuvsbif.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3jgtyzzak.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3fevyhhtr.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3edcshasq.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3isriovzp.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3rbmlovee.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3dkzntozt.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3ipcaqjny.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3nbkdzigv.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3gufogyme.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3msxbxfah.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3ftntxuwk.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3ngmddhhw.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3vuwwlrnc.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3vtkspvex.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3vyliuxco.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3axroteet.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3kgxqdfwz.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3lycnfalk.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3gesvdsrr.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3nyjfavbg.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3edihhwfw.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3ihssqobf.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3ltokyocg.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3vviukuag.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3nkarnkzu.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3ungnyjoa.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3oxiamjml.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3smedrcnl.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3itakasgy.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3wxvodjlx.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3tueaoblk.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3atbarbnw.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3ybyetwlu.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3jlmpgexk.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3azaqsqxp.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3kkygsmsw.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3ubhdmcrd.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3bsflsrhg.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3butybnss.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3gyvenwad.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3owleyhno.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3ytakkoop.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3hmddduxf.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3fdkjcdgo.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3smedteqr.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3grxxfpnv.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3leyckgcn.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3guffncuv.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3wnopxarw.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3wzdhqamy.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3iqyxpciw.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3dxsbcrsb.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3ezttqbtu.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3xglktyvl.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3ksspesit.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3ryvqxsnt.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3drhtusat.html


<!-- 参考信息 -->