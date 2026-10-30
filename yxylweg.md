代发 wailian999

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.fehbvm.com/Article/details/gcmsoadeo.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://baike.hesvh.cn/Article/details/gnjjvmixl.sHtML

[N11] 二叉树中序遍历
来源：http://m.share.fehbvm.com/Article/details/gwiwtutiq.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.zdbjq.cn/Article/details/gefjpdlmo.sHtML

PHP:  // 手写递归函数
来源：http://www.blog.zdbjq.cn/Article/details/gdhvmofqx.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.zdbjq.cn/Article/details/gbtsqccko.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.hesvh.cn/Article/details/gqbeplkgh.sHtML

Java: // 手写递归
来源：http://www.blog.zdbjq.cn/Article/details/gefgbnktb.sHtML

Go:   // 手写递归
来源：http://3g.fehbvm.com/Article/details/gsycktwpd.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://m.share.fehbvm.com/Article/details/gigetsfgx.sHtML

C#:   // 手写递归
来源：http://www.blog.hesvh.cn/Article/details/gvfhzzknj.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://3g.fehbvm.com/Article/details/gesocjdlk.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.m.share.fehbvm.com/Article/details/gmrrcqhbk.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.m.share.zdbjq.cn/Article/details/gzwblyyuh.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.hesvh.cn/Article/details/gsdwxgjck.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.fehbvm.com/Article/details/ggsynifpa.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.hesvh.cn/Article/details/gtcdxkexx.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.zdbjq.cn/Article/details/gvwwyjrkj.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://baike.hesvh.cn/Article/details/ghnsnqlvd.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.zdbjq.cn/Article/details/gfwevcege.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gtxamgqvm.sHtML

O. 并发与异步
来源：http://baike.fehbvm.com/Article/details/gaztfppub.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gkirsbaxy.sHtML

[O01] 启动一个线程
来源：http://www.blog.fehbvm.com/Article/details/gyogbfynq.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://m.share.fehbvm.com/Article/details/gwpvmocqe.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mobile.hesvh.cn/Article/details/gggmadkls.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mobile.fehbvm.com/Article/details/gekxvmkop.sHtML

TS:   // 同 JS
来源：http://www.share.zdbjq.cn/Article/details/gepgmlnfs.sHtML

Java: new Thread(() -> f()).start()
来源：http://m.share.zdbjq.cn/Article/details/guhxrfffj.sHtML

Go:   go f()
来源：http://mobile.zdbjq.cn/Article/details/gxuqsfqnh.sHtML

Ruby: Thread.new { f }
来源：http://www.blog.zdbjq.cn/Article/details/geljdtnbg.sHtML

C#:   Task.Run(() => F());
来源：http://wap.hesvh.cn/Article/details/gxqvuazck.sHtML

[O02] 使用线程池
来源：http://www.blog.zdbjq.cn/Article/details/gpbvajxrv.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://baike.hesvh.cn/Article/details/gmiouoqjv.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://3g.fehbvm.com/Article/details/gmuifgxlp.sHtML

JS:   // worker_threads 线程池
来源：http://3g.zdbjq.cn/Article/details/gwebvocka.sHtML

TS:   // worker_threads 线程池
来源：http://www.m.share.hesvh.cn/Article/details/gtjepekyo.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://m.share.fehbvm.com/Article/details/gclvjmvdy.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.share.fehbvm.com/Article/details/glnbjshir.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://read.share.fehbvm.com/Article/details/grzdhsywu.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://3g.zdbjq.cn/Article/details/ghycbfkzt.sHtML

[O03] 加锁保护共享数据
来源：http://read.share.fehbvm.com/Article/details/gkvhsxdtc.sHtML

Py:   with lock: shared += 1
来源：http://m.share.zdbjq.cn/Article/details/gduunvlhf.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://m.share.fehbvm.com/Article/details/gxqpjdprx.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://3g.hesvh.cn/Article/details/gxqyxfmjg.sHtML

TS:   // 同 JS
来源：http://www.share.fehbvm.com/Article/details/gubtulxfx.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.blog.zdbjq.cn/Article/details/gwqwpavgk.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://m.share.fehbvm.com/Article/details/gqkylypwf.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://m.share.zdbjq.cn/Article/details/gexnjjvsp.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.fehbvm.com/Article/details/gqoojwuyh.sHtML

[O04] 定义异步函数并等待
来源：http://mobile.zdbjq.cn/Article/details/gzrmftbxp.sHtML

Py:   async def f():⏎    await g()
来源：http://www.share.zdbjq.cn/Article/details/gvwwreeyz.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://m.share.zdbjq.cn/Article/details/gyefmlcik.sHtML

JS:   async function f() { await g(); }
来源：http://m.share.fehbvm.com/Article/details/gqchagklu.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.m.share.hesvh.cn/Article/details/gllyqlzar.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.blog.fehbvm.com/Article/details/ggqysevqb.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.share.hesvh.cn/Article/details/gjejbpymq.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://blog.zdbjq.cn/Article/details/gfzjlfmuy.sHtML

C#:   async Task F() { await G(); }
来源：http://www.m.share.fehbvm.com/Article/details/gmewttgjt.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.share.hesvh.cn/Article/details/gjewxuovc.sHtML

Py:   asyncio.gather(*tasks)
来源：http://3g.hesvh.cn/Article/details/ghmlbjrbh.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.m.share.hesvh.cn/Article/details/gpqdihosa.sHtML

JS:   await Promise.all(tasks)
来源：http://wap.hesvh.cn/Article/details/gqaheucla.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.zdbjq.cn/Article/details/gdhxzvbpb.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.share.zdbjq.cn/Article/details/gyfvcydhd.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.blog.fehbvm.com/Article/details/gqtdsfrix.sHtML

Ruby: threads.map(&:join)
来源：http://baike.hesvh.cn/Article/details/gmohwtivi.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://blog.hesvh.cn/Article/details/gtybqsslh.sHtML

[O06] 使用进程池
来源：http://www.m.share.hesvh.cn/Article/details/gzjqjswpl.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://3g.zdbjq.cn/Article/details/gnnpetcsr.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://mobile.zdbjq.cn/Article/details/gkzdblwtv.sHtML

JS:   // child_process / cluster 模块
来源：http://m.share.zdbjq.cn/Article/details/gsisoital.sHtML

TS:   // child_process / cluster 模块
来源：http://www.share.hesvh.cn/Article/details/gcwozyfdt.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://read.share.fehbvm.com/Article/details/gmivfpnig.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://baike.hesvh.cn/Article/details/gxouishnl.sHtML

Ruby: // fork 块
来源：http://blog.hesvh.cn/Article/details/gqpvgrbpk.sHtML

C#:   Parallel.For
来源：http://3g.zdbjq.cn/Article/details/gtuzvqqwt.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gdwjsavyt.sHtML

P. 常用工具函数
来源：http://wap.zdbjq.cn/Article/details/gummtymbt.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gmwotkkkh.sHtML

[P01] 生成 UUID
来源：http://m.share.fehbvm.com/Article/details/gblrwicwv.sHtML

Py:   str(uuid.uuid4())
来源：http://baike.hesvh.cn/Article/details/gwntrisgv.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.m.share.zdbjq.cn/Article/details/grnuekapa.sHtML

JS:   crypto.randomUUID()
来源：http://www.m.share.zdbjq.cn/Article/details/gnicbqeow.sHtML

TS:   crypto.randomUUID()
来源：http://www.m.share.hesvh.cn/Article/details/gqbvcbnqa.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.share.hesvh.cn/Article/details/gqisbhmsn.sHtML

Go:   // 用 github.com/google/uuid
来源：http://wap.hesvh.cn/Article/details/gidjwcuwy.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.zdbjq.cn/Article/details/guqtfogya.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.m.share.hesvh.cn/Article/details/gzxbfcihs.sHtML

[P02] MD5 / SHA256 摘要
来源：http://read.share.hesvh.cn/Article/details/gtnfpzmek.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://blog.zdbjq.cn/Article/details/gybdgffno.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://read.share.hesvh.cn/Article/details/gkprisojh.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wap.fehbvm.com/Article/details/ganqriexv.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://baike.hesvh.cn/Article/details/gbkojvbxk.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wap.zdbjq.cn/Article/details/gduplrwiz.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://blog.zdbjq.cn/Article/details/gniysapyy.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.share.zdbjq.cn/Article/details/gihdjxhmc.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wap.hesvh.cn/Article/details/gyxphjdlj.sHtML

[P03] 生成短随机字符串
来源：http://m.share.zdbjq.cn/Article/details/gbijuzpvk.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wap.fehbvm.com/Article/details/glwqyvqtr.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wap.zdbjq.cn/Article/details/gngewyyfx.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.fehbvm.com/Article/details/gqpgqsdiz.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.zdbjq.cn/Article/details/gqyevueht.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.blog.hesvh.cn/Article/details/gxiecyqka.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mobile.zdbjq.cn/Article/details/gogfnouxj.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://baike.zdbjq.cn/Article/details/gtdldveep.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mobile.zdbjq.cn/Article/details/gvmnqyurf.sHtML

[P04] 求长度
来源：http://mobile.fehbvm.com/Article/details/gepecfaip.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baike.zdbjq.cn/Article/details/glmprjgbm.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.hesvh.cn/Article/details/ghlbwakzw.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.hesvh.cn/Article/details/gvlwmzlna.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.fehbvm.com/Article/details/gsinabulz.sHtML

Java: list.size();  map.size();  s.length()
来源：http://baike.hesvh.cn/Article/details/gnsqcvgex.sHtML

Go:   len(arr);  len(m)
来源：http://www.blog.zdbjq.cn/Article/details/gykxkoocp.sHtML

Ruby: x.length;  x.size
来源：http://www.share.zdbjq.cn/Article/details/geapweils.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.m.share.zdbjq.cn/Article/details/gswmxcpfy.sHtML

[P05] 判断两个对象内容是否相等
来源：http://blog.hesvh.cn/Article/details/gmihgogbx.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://mobile.hesvh.cn/Article/details/grlaquffr.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://baike.fehbvm.com/Article/details/glagusalu.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://m.share.fehbvm.com/Article/details/gcqijqoof.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.fehbvm.com/Article/details/gyvnhwnzi.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.m.share.hesvh.cn/Article/details/gepkelkxe.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://wap.fehbvm.com/Article/details/gkzpqfjlc.sHtML

Ruby: a == b
来源：http://www.m.share.zdbjq.cn/Article/details/gggcfqpgk.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.blog.fehbvm.com/Article/details/gdeekqhbm.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://baike.hesvh.cn/Article/details/gbxcysjpq.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.hesvh.cn/Article/details/gwbbvuwsl.sHtML

PHP:  if (empty($x)) {}
来源：http://wap.zdbjq.cn/Article/details/gjhkwmfur.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mobile.fehbvm.com/Article/details/gcflxwcig.sHtML

TS:   if (x == null) {}
来源：http://3g.hesvh.cn/Article/details/gjibqghfq.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.blog.fehbvm.com/Article/details/gsemxiybb.sHtML

Go:   if x == nil {}
来源：http://wap.hesvh.cn/Article/details/ggrleakzl.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://read.share.zdbjq.cn/Article/details/gwnmtwiyr.sHtML

C#:   if (x is null) {}
来源：http://wap.zdbjq.cn/Article/details/gklidjizd.sHtML

[P07] 防抖与节流
来源：http://wap.fehbvm.com/Article/details/gwwegiifn.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://read.share.hesvh.cn/Article/details/gmoltlzlr.sHtML

PHP:  // 手写时间戳比较
来源：http://m.share.fehbvm.com/Article/details/gsxmqagys.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.hesvh.cn/Article/details/gotftllcm.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.hesvh.cn/Article/details/gubcgaasx.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.m.share.fehbvm.com/Article/details/gwfcfltrr.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.m.share.fehbvm.com/Article/details/gxiyndxmg.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.share.zdbjq.cn/Article/details/gtvowmonv.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://read.share.hesvh.cn/Article/details/gljauoyqq.sHtML

[P08] 处理浮点精度问题
来源：http://mobile.fehbvm.com/Article/details/ggfudrzus.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wap.zdbjq.cn/Article/details/gmfleqbmb.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wap.hesvh.cn/Article/details/geixpcirn.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.fehbvm.com/Article/details/gjnkvjttu.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.m.share.fehbvm.com/Article/details/gxjkmmjyf.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.blog.fehbvm.com/Article/details/grbqiqlcb.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://m.share.fehbvm.com/Article/details/gyeinpfzw.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.m.share.zdbjq.cn/Article/details/gemzqgriu.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://m.share.fehbvm.com/Article/details/gswhuyqxn.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/guctfbheb.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.blog.hesvh.cn/Article/details/gckmiquyr.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gkwdbfdqe.sHtML

[Q01] 创建表
来源：http://read.share.zdbjq.cn/Article/details/gnykfxmeh.sHtML

CREATE TABLE users (
来源：http://wap.zdbjq.cn/Article/details/gcnuasumu.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.zdbjq.cn/Article/details/ghmdsoizl.sHtML

name VARCHAR(50) NOT NULL,
来源：http://read.share.hesvh.cn/Article/details/gnsnygjkz.sHtML

email VARCHAR(100) UNIQUE,
来源：http://m.share.hesvh.cn/Article/details/gkzvvluqs.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://baike.hesvh.cn/Article/details/gyfilvttt.sHtML

);
来源：http://mobile.zdbjq.cn/Article/details/gjqbghyuy.sHtML

[Q02] 创建带外键的表
来源：http://read.share.fehbvm.com/Article/details/gwfwbfomg.sHtML

CREATE TABLE orders (
来源：http://baike.hesvh.cn/Article/details/gdnltwcjn.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.hesvh.cn/Article/details/giyvqztnf.sHtML

user_id INT NOT NULL,
来源：http://m.share.fehbvm.com/Article/details/gglnqzcef.sHtML

amount DECIMAL(10, 2),
来源：http://mobile.fehbvm.com/Article/details/glayllxef.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.share.fehbvm.com/Article/details/ghuzdqkdz.sHtML

);
来源：http://www.share.hesvh.cn/Article/details/gpyppidml.sHtML

[Q03] 增加列
来源：http://read.share.zdbjq.cn/Article/details/griiqsovc.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://baike.fehbvm.com/Article/details/ggronjyeo.sHtML

[Q04] 修改列类型
来源：http://www.share.fehbvm.com/Article/details/grskybtko.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://3g.fehbvm.com/Article/details/gjmxcfyht.sHtML

[Q05] 重命名列
来源：http://blog.hesvh.cn/Article/details/gpacjrntt.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://3g.hesvh.cn/Article/details/gkhommqvx.sHtML

[Q06] 删除列
来源：http://baike.hesvh.cn/Article/details/gncxrrbyf.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://mobile.fehbvm.com/Article/details/gjwuaiora.sHtML

[Q07] 删除表
来源：http://mobile.hesvh.cn/Article/details/gduoxggeu.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.m.share.fehbvm.com/Article/details/gzulvuuje.sHtML

[Q08] 创建普通索引
来源：http://www.share.hesvh.cn/Article/details/ggksbmqwd.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.blog.zdbjq.cn/Article/details/gmrqwwuso.sHtML

[Q09] 创建唯一索引
来源：http://www.share.zdbjq.cn/Article/details/gachvbzdx.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.m.share.hesvh.cn/Article/details/ghschmdka.sHtML

[Q10] 插入单行
来源：http://mobile.zdbjq.cn/Article/details/gzuyazcho.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.share.zdbjq.cn/Article/details/gdjftkhfs.sHtML

[Q11] 一次插入多行
来源：http://m.share.fehbvm.com/Article/details/gxyrkfvis.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.hesvh.cn/Article/details/gwqbvsngo.sHtML

[Q12] 插入后取自增 ID
来源：http://www.share.zdbjq.cn/Article/details/gwbrdqzbe.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.m.share.hesvh.cn/Article/details/gtdnalvln.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.share.hesvh.cn/Article/details/gdpdfdyep.sHtML

[Q13] 忽略重复插入
来源：http://www.share.fehbvm.com/Article/details/gtzqgkmqa.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.share.zdbjq.cn/Article/details/gklhgxmof.sHtML

[Q14] 存在则更新（upsert）
来源：http://3g.zdbjq.cn/Article/details/guxvgiold.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.share.fehbvm.com/Article/details/gumsmvvux.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://blog.fehbvm.com/Article/details/gyovwfopw.sHtML

[Q15] 查询全部
来源：http://m.share.zdbjq.cn/Article/details/gcwugbgqd.sHtML

SELECT * FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gubnsxppf.sHtML

[Q16] 查询指定列
来源：http://mobile.fehbvm.com/Article/details/gxypxqbld.sHtML

SELECT id, name FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gbxsijtra.sHtML

[Q17] 条件查询
来源：http://baike.zdbjq.cn/Article/details/gtzxawtsz.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://3g.fehbvm.com/Article/details/gfnbghmgt.sHtML

[Q18] 模糊匹配
来源：http://wap.fehbvm.com/Article/details/gwbwiqogq.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wap.hesvh.cn/Article/details/gvvlvesmi.sHtML

[Q19] 范围查询
来源：http://m.share.fehbvm.com/Article/details/gkvurqrej.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://baike.hesvh.cn/Article/details/gexodfswg.sHtML

[Q20] IN 列表
来源：http://www.m.share.fehbvm.com/Article/details/giplihtzd.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://m.share.zdbjq.cn/Article/details/glymjfztk.sHtML

[Q21] 空值判断
来源：http://baike.fehbvm.com/Article/details/gcfavxnul.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://3g.hesvh.cn/Article/details/gftjzgelv.sHtML

[Q22] 排序
来源：http://wap.fehbvm.com/Article/details/gdbvzobsv.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.blog.fehbvm.com/Article/details/giizgtrjw.sHtML

[Q23] 分页
来源：http://3g.fehbvm.com/Article/details/gscpxivfa.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://3g.fehbvm.com/Article/details/gqoiwjqyr.sHtML

[Q24] 去重
来源：http://www.blog.hesvh.cn/Article/details/ggrcifkmr.sHtML

SELECT DISTINCT city FROM users;
来源：http://m.share.hesvh.cn/Article/details/gumucigjl.sHtML

[Q25] 只取前 N 条
来源：http://www.blog.fehbvm.com/Article/details/gqnfukuea.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mobile.hesvh.cn/Article/details/gzmmhygxr.sHtML

[Q26] 计数
来源：http://baike.hesvh.cn/Article/details/gicgznpdd.sHtML

SELECT COUNT(*) FROM users;
来源：http://blog.hesvh.cn/Article/details/geqqoirzw.sHtML

[Q27] 条件计数
来源：http://baike.zdbjq.cn/Article/details/gtomuoscp.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.share.fehbvm.com/Article/details/gwforvqvj.sHtML

[Q28] 求和与平均
来源：http://www.share.fehbvm.com/Article/details/gtlhptcyp.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://baike.fehbvm.com/Article/details/grrvmagmx.sHtML

[Q29] 最大最小值
来源：http://m.share.fehbvm.com/Article/details/ggeyvveet.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gqeyufopm.sHtML

[Q30] 分组统计
来源：http://baike.fehbvm.com/Article/details/genosmiwy.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://blog.zdbjq.cn/Article/details/gxnevbkyr.sHtML

[Q31] 分组后过滤
来源：http://blog.fehbvm.com/Article/details/gewdxlmzo.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mobile.fehbvm.com/Article/details/gmkxvalap.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gdzfgavsl.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wap.hesvh.cn/Article/details/gysqonxlu.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://3g.fehbvm.com/Article/details/ggmhmvzsl.sHtML

[Q33] 多列分组
来源：http://wap.zdbjq.cn/Article/details/ghiaothol.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.blog.fehbvm.com/Article/details/gpctejmpy.sHtML

[Q34] 每组取第一条
来源：http://baike.zdbjq.cn/Article/details/ggwvfojyg.sHtML

SELECT * FROM (
来源：http://wap.hesvh.cn/Article/details/gsmiusiru.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.blog.zdbjq.cn/Article/details/gmdrezyws.sHtML

) t WHERE rn = 1;
来源：http://read.share.zdbjq.cn/Article/details/ghotyupyb.sHtML

[Q35] 内连接
来源：http://www.blog.hesvh.cn/Article/details/gzzberuae.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://3g.zdbjq.cn/Article/details/guzhendbm.sHtML

[Q36] 左连接
来源：http://wap.zdbjq.cn/Article/details/gpmohaipv.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.share.fehbvm.com/Article/details/gvwxkpqcl.sHtML

[Q37] 右连接
来源：http://3g.hesvh.cn/Article/details/gboabqymy.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.hesvh.cn/Article/details/gigaqrmhg.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://mobile.hesvh.cn/Article/details/gfojwprdu.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wap.hesvh.cn/Article/details/gfxyouvzz.sHtML

[Q39] 自连接（查上下级）
来源：http://read.share.hesvh.cn/Article/details/gyvpfbict.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.m.share.fehbvm.com/Article/details/gwgawlngs.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.hesvh.cn/Article/details/gbhisbmeq.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://3g.zdbjq.cn/Article/details/gzzroesby.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.fehbvm.com/Article/details/gdhszquty.sHtML

[Q41] 多表连接
来源：http://m.share.zdbjq.cn/Article/details/gjpfrgweg.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://m.share.fehbvm.com/Article/details/gpynquxie.sHtML

JOIN users u ON u.id = o.user_id
来源：http://read.share.zdbjq.cn/Article/details/gwznzvvzz.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://blog.hesvh.cn/Article/details/goyleshco.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.hesvh.cn/Article/details/gbbzroggj.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.hesvh.cn/Article/details/gledyzwtq.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.m.share.fehbvm.com/Article/details/gijsqujkc.sHtML

[Q43] 标量子查询
来源：http://www.blog.fehbvm.com/Article/details/gbkpgjaec.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.blog.fehbvm.com/Article/details/gjzwsacht.sHtML

[Q44] IN 子查询
来源：http://wap.fehbvm.com/Article/details/gattvqwmi.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://blog.zdbjq.cn/Article/details/glumhtunh.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.fehbvm.com/Article/details/gzfcaszhu.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.zdbjq.cn/Article/details/gtxsusomv.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.hesvh.cn/Article/details/gnposrcnq.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.hesvh.cn/Article/details/galwnrtkk.sHtML

[Q47] 与平均值比较
来源：http://www.m.share.zdbjq.cn/Article/details/gflmgiyld.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.zdbjq.cn/Article/details/gdvqixsjb.sHtML

[Q48] CTE 公用表表达式
来源：http://www.blog.zdbjq.cn/Article/details/groglrkpi.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.zdbjq.cn/Article/details/gjlocuzcg.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://wap.hesvh.cn/Article/details/gpdmybslf.sHtML

[Q49] 更新单行
来源：http://www.blog.hesvh.cn/Article/details/gggmpmvin.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.zdbjq.cn/Article/details/gfkttwiwy.sHtML

[Q50] 批量更新
来源：http://wap.hesvh.cn/Article/details/gebvuxbmm.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.hesvh.cn/Article/details/ghajmkmjm.sHtML

[Q51] 用子查询更新
来源：http://blog.zdbjq.cn/Article/details/gdegsiscx.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blog.hesvh.cn/Article/details/gibjbkuhk.sHtML

[Q52] 删除指定行
来源：http://www.blog.hesvh.cn/Article/details/gsxkaulfm.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.hesvh.cn/Article/details/gvwqzdvgz.sHtML

[Q53] 按条件删除
来源：http://www.blog.zdbjq.cn/Article/details/gowrwjmjt.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.zdbjq.cn/Article/details/gkdwpruaf.sHtML

[Q54] 清空表
来源：http://m.share.zdbjq.cn/Article/details/gyxpqvfnl.sHtML

TRUNCATE TABLE logs;
来源：http://www.blog.hesvh.cn/Article/details/gvodmtzji.sHtML

[Q55] 排名（并列占位）
来源：http://www.m.share.zdbjq.cn/Article/details/gezwlnwge.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://blog.hesvh.cn/Article/details/gzlsxajde.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.blog.fehbvm.com/Article/details/gqzwletgt.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.share.fehbvm.com/Article/details/gbklujycj.sHtML

[Q57] 行号
来源：http://mobile.hesvh.cn/Article/details/gqomzahxz.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gaminpsoj.sHtML

[Q58] 累计求和
来源：http://www.m.share.fehbvm.com/Article/details/gafqfdvsb.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gsrwofxak.sHtML

[Q59] 分组内累计
来源：http://www.blog.fehbvm.com/Article/details/ggscthacn.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/gbdjatgsj.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.zdbjq.cn/Article/details/gdzxsrrjx.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://baike.hesvh.cn/Article/details/gxakzgbzg.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.hesvh.cn/Article/details/gpkbwwusr.sHtML

[Q61] 移动平均
来源：http://www.m.share.hesvh.cn/Article/details/gpiwnooan.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://3g.zdbjq.cn/Article/details/gyqwofkgf.sHtML

[Q62] 分组占比
来源：http://www.blog.fehbvm.com/Article/details/gzakdwbsl.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.zdbjq.cn/Article/details/gtrmffvue.sHtML


<!-- 参考信息 -->