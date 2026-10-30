代发 wailian999

Ruby: Node = Struct.new(:v, :next)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gihaxuopy.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.fanxiaobao.xyz/Article/details/glhjtcotq.sHtML

[N11] 二叉树中序遍历
来源：http://blog.fanxiaobao.xyz/Article/details/gpfxjoaaf.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://read.share.fanxiaobao.xyz/Article/details/gjmgaciut.sHtML

PHP:  // 手写递归函数
来源：http://read.share.fanxiaobao.xyz/Article/details/ghjgmcinm.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.fanxiaobao.xyz/Article/details/gpnzlmtfb.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.fanxiaobao.xyz/Article/details/gorpjqxmn.sHtML

Java: // 手写递归
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzywcbpmm.sHtML

Go:   // 手写递归
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcphoxfkc.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://3g.fanxiaobao.xyz/Article/details/gijqoukcj.sHtML

C#:   // 手写递归
来源：http://www.share.fanxiaobao.xyz/Article/details/gkiwdbgnt.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://baike.fanxiaobao.xyz/Article/details/gbdskhibk.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://read.share.fanxiaobao.xyz/Article/details/ghlmeunow.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wap.fanxiaobao.xyz/Article/details/gailowyri.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfnumcxrh.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.fanxiaobao.xyz/Article/details/gjnrzzkzk.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.fanxiaobao.xyz/Article/details/gsdysfvsl.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.fanxiaobao.xyz/Article/details/gtihfuoln.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.share.fanxiaobao.xyz/Article/details/gabmgtrda.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.fanxiaobao.xyz/Article/details/gswxpfgqd.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gfgdklneb.sHtML

O. 并发与异步
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpzzzmnrv.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gkmwgqsey.sHtML

[O01] 启动一个线程
来源：http://3g.fanxiaobao.xyz/Article/details/gaekldlxy.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://m.share.fanxiaobao.xyz/Article/details/gldylttcf.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wap.fanxiaobao.xyz/Article/details/gqgnpcqdv.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mobile.fanxiaobao.xyz/Article/details/gmjntrwqu.sHtML

TS:   // 同 JS
来源：http://mobile.fanxiaobao.xyz/Article/details/gwvvwckpf.sHtML

Java: new Thread(() -> f()).start()
来源：http://baike.fanxiaobao.xyz/Article/details/ganxhfzhy.sHtML

Go:   go f()
来源：http://read.share.fanxiaobao.xyz/Article/details/gamdpsudq.sHtML

Ruby: Thread.new { f }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gryyvrwpi.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.fanxiaobao.xyz/Article/details/gicjfjlgg.sHtML

[O02] 使用线程池
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghryoveit.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.fanxiaobao.xyz/Article/details/guubbftmx.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blog.fanxiaobao.xyz/Article/details/genxobkmw.sHtML

JS:   // worker_threads 线程池
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpmsmhxib.sHtML

TS:   // worker_threads 线程池
来源：http://read.share.fanxiaobao.xyz/Article/details/gnliqwuou.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://m.share.fanxiaobao.xyz/Article/details/gylioauae.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://blog.fanxiaobao.xyz/Article/details/glbgciztn.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://3g.fanxiaobao.xyz/Article/details/gjenizxhy.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://3g.fanxiaobao.xyz/Article/details/glczndhlb.sHtML

[O03] 加锁保护共享数据
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvdscansq.sHtML

Py:   with lock: shared += 1
来源：http://mobile.fanxiaobao.xyz/Article/details/gcanohrtp.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://3g.fanxiaobao.xyz/Article/details/grzekbjro.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://read.share.fanxiaobao.xyz/Article/details/gpujiqojx.sHtML

TS:   // 同 JS
来源：http://www.share.fanxiaobao.xyz/Article/details/gdaecbtoh.sHtML

Java: synchronized (this) { shared++; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gransozph.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.share.fanxiaobao.xyz/Article/details/gaekkrooc.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.fanxiaobao.xyz/Article/details/gydcuwevv.sHtML

C#:   lock (gate) { shared++; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gihjmnrfs.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfabjpauy.sHtML

Py:   async def f():⏎    await g()
来源：http://read.share.fanxiaobao.xyz/Article/details/gxyprihjh.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mobile.fanxiaobao.xyz/Article/details/guokwtenv.sHtML

JS:   async function f() { await g(); }
来源：http://blog.fanxiaobao.xyz/Article/details/gofxgdcnm.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gnbvdcpgl.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mobile.fanxiaobao.xyz/Article/details/gpjfxpnai.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://3g.fanxiaobao.xyz/Article/details/ggmouuxxm.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaepghquy.sHtML

C#:   async Task F() { await G(); }
来源：http://3g.fanxiaobao.xyz/Article/details/gjjbkiqzl.sHtML

[O05] 并发执行并等待全部完成
来源：http://blog.fanxiaobao.xyz/Article/details/gwedooaat.sHtML

Py:   asyncio.gather(*tasks)
来源：http://wap.fanxiaobao.xyz/Article/details/geoklhlaq.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcrwhhnin.sHtML

JS:   await Promise.all(tasks)
来源：http://mobile.fanxiaobao.xyz/Article/details/gggnwpbrk.sHtML

TS:   await Promise.all(tasks)
来源：http://mobile.fanxiaobao.xyz/Article/details/ghinagwrh.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://m.share.fanxiaobao.xyz/Article/details/gvyfnorlc.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mobile.fanxiaobao.xyz/Article/details/gkkyrfevr.sHtML

Ruby: threads.map(&:join)
来源：http://baike.fanxiaobao.xyz/Article/details/gaypuuevw.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://blog.fanxiaobao.xyz/Article/details/ghmxcnium.sHtML

[O06] 使用进程池
来源：http://www.share.fanxiaobao.xyz/Article/details/gjboonasm.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://baike.fanxiaobao.xyz/Article/details/gyamlbabc.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://wap.fanxiaobao.xyz/Article/details/gsgbqpgpy.sHtML

JS:   // child_process / cluster 模块
来源：http://3g.fanxiaobao.xyz/Article/details/grkkofzdo.sHtML

TS:   // child_process / cluster 模块
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glyiozsyy.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://read.share.fanxiaobao.xyz/Article/details/gkoptapan.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://baike.fanxiaobao.xyz/Article/details/grhtuisdp.sHtML

Ruby: // fork 块
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsowdswjd.sHtML

C#:   Parallel.For
来源：http://3g.fanxiaobao.xyz/Article/details/gkvzhdvmr.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxerymhim.sHtML

P. 常用工具函数
来源：http://blog.fanxiaobao.xyz/Article/details/gphvdliab.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gmbwczzjr.sHtML

[P01] 生成 UUID
来源：http://read.share.fanxiaobao.xyz/Article/details/glmepxkos.sHtML

Py:   str(uuid.uuid4())
来源：http://m.share.fanxiaobao.xyz/Article/details/gzlyposjp.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://read.share.fanxiaobao.xyz/Article/details/gxnhsoyie.sHtML

JS:   crypto.randomUUID()
来源：http://wap.fanxiaobao.xyz/Article/details/ggcuzveme.sHtML

TS:   crypto.randomUUID()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcexpjkls.sHtML

Java: UUID.randomUUID().toString()
来源：http://m.share.fanxiaobao.xyz/Article/details/gbbncnrvn.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.blog.fanxiaobao.xyz/Article/details/gugabccrb.sHtML

Ruby: SecureRandom.uuid
来源：http://wap.fanxiaobao.xyz/Article/details/gwpaostan.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtqzwzwaf.sHtML

[P02] MD5 / SHA256 摘要
来源：http://blog.fanxiaobao.xyz/Article/details/gvogjnlvi.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://read.share.fanxiaobao.xyz/Article/details/gpoioziha.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://mobile.fanxiaobao.xyz/Article/details/gbyfliopn.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://baike.fanxiaobao.xyz/Article/details/gvxclrabk.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.fanxiaobao.xyz/Article/details/ginxnhfbg.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://blog.fanxiaobao.xyz/Article/details/gthigdqej.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaxhqsilx.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://baike.fanxiaobao.xyz/Article/details/gvwxmftxu.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://blog.fanxiaobao.xyz/Article/details/gyqhukscc.sHtML

[P03] 生成短随机字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/gnreppamg.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://blog.fanxiaobao.xyz/Article/details/gswgfdwve.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://read.share.fanxiaobao.xyz/Article/details/gtivxxbrw.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.fanxiaobao.xyz/Article/details/gprpofiht.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.fanxiaobao.xyz/Article/details/gjshhylza.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wap.fanxiaobao.xyz/Article/details/gwmomfhnh.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://baike.fanxiaobao.xyz/Article/details/gzetzajgq.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://baike.fanxiaobao.xyz/Article/details/gtpsljbnv.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wap.fanxiaobao.xyz/Article/details/gcwprowaj.sHtML

[P04] 求长度
来源：http://blog.fanxiaobao.xyz/Article/details/gbmfyatzi.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://3g.fanxiaobao.xyz/Article/details/gacxsxbjh.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.fanxiaobao.xyz/Article/details/gyurvhdej.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.fanxiaobao.xyz/Article/details/gljmudgsz.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnewktcvy.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gseriqpne.sHtML

Go:   len(arr);  len(m)
来源：http://blog.fanxiaobao.xyz/Article/details/gnujvdckf.sHtML

Ruby: x.length;  x.size
来源：http://baike.fanxiaobao.xyz/Article/details/gzwyibdiq.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdkzkikme.sHtML

[P05] 判断两个对象内容是否相等
来源：http://read.share.fanxiaobao.xyz/Article/details/gfbipwdsf.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.share.fanxiaobao.xyz/Article/details/gkmhmkfsw.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.share.fanxiaobao.xyz/Article/details/gqonawzuo.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mobile.fanxiaobao.xyz/Article/details/glwcsyrsm.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxgxjdcji.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://read.share.fanxiaobao.xyz/Article/details/gtxbgkwmk.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.share.fanxiaobao.xyz/Article/details/glrhejcwq.sHtML

Ruby: a == b
来源：http://read.share.fanxiaobao.xyz/Article/details/gyetaqnay.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://blog.fanxiaobao.xyz/Article/details/gyapgdyid.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://m.share.fanxiaobao.xyz/Article/details/gqbwthkvb.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvlaroiby.sHtML

PHP:  if (empty($x)) {}
来源：http://3g.fanxiaobao.xyz/Article/details/gkscspnue.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://baike.fanxiaobao.xyz/Article/details/gaukpakyi.sHtML

TS:   if (x == null) {}
来源：http://wap.fanxiaobao.xyz/Article/details/gfwxkmkno.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://wap.fanxiaobao.xyz/Article/details/ghckvvpol.sHtML

Go:   if x == nil {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gewikfpxs.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.fanxiaobao.xyz/Article/details/gmhgwjgqu.sHtML

C#:   if (x is null) {}
来源：http://3g.fanxiaobao.xyz/Article/details/gzzxyqzqp.sHtML

[P07] 防抖与节流
来源：http://baike.fanxiaobao.xyz/Article/details/gqpkndlex.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.blog.fanxiaobao.xyz/Article/details/glxeozhtx.sHtML

PHP:  // 手写时间戳比较
来源：http://wap.fanxiaobao.xyz/Article/details/glessiojb.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqdjsnirm.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.fanxiaobao.xyz/Article/details/gthhpurct.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gjqjnocsa.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://m.share.fanxiaobao.xyz/Article/details/gzasexdzm.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvhlspdcj.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glsuddbiu.sHtML

[P08] 处理浮点精度问题
来源：http://www.share.fanxiaobao.xyz/Article/details/golgxbfgg.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://baike.fanxiaobao.xyz/Article/details/gpgqclmhz.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://m.share.fanxiaobao.xyz/Article/details/gpcrilbez.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://3g.fanxiaobao.xyz/Article/details/gddiuflxr.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://blog.fanxiaobao.xyz/Article/details/ggbvlfkdu.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://m.share.fanxiaobao.xyz/Article/details/gwkuqplis.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://3g.fanxiaobao.xyz/Article/details/gtsjosxbm.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://baike.fanxiaobao.xyz/Article/details/gqjhwcgkc.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://3g.fanxiaobao.xyz/Article/details/gdygpdndi.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gykdygehu.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://baike.fanxiaobao.xyz/Article/details/gjnuyzgkp.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcsikdpts.sHtML

[Q01] 创建表
来源：http://3g.fanxiaobao.xyz/Article/details/gwfiaufmd.sHtML

CREATE TABLE users (
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwdfjtfmn.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.fanxiaobao.xyz/Article/details/gepilrvzk.sHtML

name VARCHAR(50) NOT NULL,
来源：http://3g.fanxiaobao.xyz/Article/details/gkplzdqrs.sHtML

email VARCHAR(100) UNIQUE,
来源：http://wap.fanxiaobao.xyz/Article/details/gesofhfux.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://3g.fanxiaobao.xyz/Article/details/golgxkgac.sHtML

);
来源：http://m.share.fanxiaobao.xyz/Article/details/gvzpdsmoi.sHtML

[Q02] 创建带外键的表
来源：http://m.share.fanxiaobao.xyz/Article/details/guudfkzdy.sHtML

CREATE TABLE orders (
来源：http://mobile.fanxiaobao.xyz/Article/details/gwbbdvumm.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.fanxiaobao.xyz/Article/details/gywgqdrqh.sHtML

user_id INT NOT NULL,
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdwphqkiu.sHtML

amount DECIMAL(10, 2),
来源：http://m.share.fanxiaobao.xyz/Article/details/gkvivwexk.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.blog.fanxiaobao.xyz/Article/details/golvxpyeg.sHtML

);
来源：http://3g.fanxiaobao.xyz/Article/details/gtghwwqlg.sHtML

[Q03] 增加列
来源：http://m.share.fanxiaobao.xyz/Article/details/ghwneyufr.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mobile.fanxiaobao.xyz/Article/details/giqsoeord.sHtML

[Q04] 修改列类型
来源：http://m.share.fanxiaobao.xyz/Article/details/gwrsxkoml.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://blog.fanxiaobao.xyz/Article/details/ghfdnzifc.sHtML

[Q05] 重命名列
来源：http://mobile.fanxiaobao.xyz/Article/details/gwjqqeehw.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wap.fanxiaobao.xyz/Article/details/gaakkwkvb.sHtML

[Q06] 删除列
来源：http://mobile.fanxiaobao.xyz/Article/details/ggwnvemul.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.blog.fanxiaobao.xyz/Article/details/giumcqsia.sHtML

[Q07] 删除表
来源：http://www.blog.fanxiaobao.xyz/Article/details/grgrsxsoc.sHtML

DROP TABLE IF EXISTS orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/grsudbxzv.sHtML

[Q08] 创建普通索引
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwmypozhg.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://blog.fanxiaobao.xyz/Article/details/ghdypyive.sHtML

[Q09] 创建唯一索引
来源：http://www.share.fanxiaobao.xyz/Article/details/gqnafnitq.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://baike.fanxiaobao.xyz/Article/details/gdwdvajmv.sHtML

[Q10] 插入单行
来源：http://www.share.fanxiaobao.xyz/Article/details/gopgxxghp.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://blog.fanxiaobao.xyz/Article/details/gqacunmtb.sHtML

[Q11] 一次插入多行
来源：http://mobile.fanxiaobao.xyz/Article/details/gdcrgswxf.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.share.fanxiaobao.xyz/Article/details/gsrtzryio.sHtML

[Q12] 插入后取自增 ID
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqpbqzpnj.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://blog.fanxiaobao.xyz/Article/details/ggkdhbsdi.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wap.fanxiaobao.xyz/Article/details/gupiudaqd.sHtML

[Q13] 忽略重复插入
来源：http://m.share.fanxiaobao.xyz/Article/details/glvciglbt.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfcnhxygj.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkcuqkpae.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gojtzedns.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mobile.fanxiaobao.xyz/Article/details/geqqalftf.sHtML

[Q15] 查询全部
来源：http://3g.fanxiaobao.xyz/Article/details/ggwvezheq.sHtML

SELECT * FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gywbllssp.sHtML

[Q16] 查询指定列
来源：http://wap.fanxiaobao.xyz/Article/details/gpkaqeost.sHtML

SELECT id, name FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gzamzwtwp.sHtML

[Q17] 条件查询
来源：http://read.share.fanxiaobao.xyz/Article/details/gbirbfdwc.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/grqlfaxui.sHtML

[Q18] 模糊匹配
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmygrynqf.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mobile.fanxiaobao.xyz/Article/details/gbqeewzvn.sHtML

[Q19] 范围查询
来源：http://baike.fanxiaobao.xyz/Article/details/gxczlguts.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://read.share.fanxiaobao.xyz/Article/details/gfyboouwb.sHtML

[Q20] IN 列表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfiqmzpdv.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxlpbxgpq.sHtML

[Q21] 空值判断
来源：http://baike.fanxiaobao.xyz/Article/details/gonyqbocx.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://3g.fanxiaobao.xyz/Article/details/gnrihlupt.sHtML

[Q22] 排序
来源：http://m.share.fanxiaobao.xyz/Article/details/gqpmhvech.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://read.share.fanxiaobao.xyz/Article/details/gshxirpov.sHtML

[Q23] 分页
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpubmcteg.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggeuihrow.sHtML

[Q24] 去重
来源：http://blog.fanxiaobao.xyz/Article/details/gmqrxioey.sHtML

SELECT DISTINCT city FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gjfcxwjas.sHtML

[Q25] 只取前 N 条
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gusdyshob.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://m.share.fanxiaobao.xyz/Article/details/gwyoqyhbj.sHtML

[Q26] 计数
来源：http://baike.fanxiaobao.xyz/Article/details/gefkttnrh.sHtML

SELECT COUNT(*) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gerbhlbsw.sHtML

[Q27] 条件计数
来源：http://www.share.fanxiaobao.xyz/Article/details/gpdtosbqv.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/glxmkgvei.sHtML

[Q28] 求和与平均
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqbemsbjm.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjvdpntxr.sHtML

[Q29] 最大最小值
来源：http://3g.fanxiaobao.xyz/Article/details/ghcevhfzk.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gtyxmvtrl.sHtML

[Q30] 分组统计
来源：http://read.share.fanxiaobao.xyz/Article/details/grkwdzwjy.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.fanxiaobao.xyz/Article/details/gkqyphfpn.sHtML

[Q31] 分组后过滤
来源：http://mobile.fanxiaobao.xyz/Article/details/gdbgmbzyd.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wap.fanxiaobao.xyz/Article/details/ggsqbjmkm.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtrroldmb.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://m.share.fanxiaobao.xyz/Article/details/gqnketqfn.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://blog.fanxiaobao.xyz/Article/details/gfynhvxnl.sHtML

[Q33] 多列分组
来源：http://m.share.fanxiaobao.xyz/Article/details/gwokltmaj.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://baike.fanxiaobao.xyz/Article/details/glskcrhaf.sHtML

[Q34] 每组取第一条
来源：http://3g.fanxiaobao.xyz/Article/details/gdgsontlc.sHtML

SELECT * FROM (
来源：http://baike.fanxiaobao.xyz/Article/details/guqfnbmpf.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://m.share.fanxiaobao.xyz/Article/details/gxeieqyjc.sHtML

) t WHERE rn = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gazeoknod.sHtML

[Q35] 内连接
来源：http://www.share.fanxiaobao.xyz/Article/details/goykmjsej.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvpbmojib.sHtML

[Q36] 左连接
来源：http://read.share.fanxiaobao.xyz/Article/details/gyeadayxi.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.fanxiaobao.xyz/Article/details/gspiskybz.sHtML

[Q37] 右连接
来源：http://3g.fanxiaobao.xyz/Article/details/gzmxhpewf.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://baike.fanxiaobao.xyz/Article/details/gyyodlruj.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnpzziysx.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://blog.fanxiaobao.xyz/Article/details/grjmxgvtp.sHtML

[Q39] 自连接（查上下级）
来源：http://mobile.fanxiaobao.xyz/Article/details/gebaskdzo.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.blog.fanxiaobao.xyz/Article/details/gysnsqnvw.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://blog.fanxiaobao.xyz/Article/details/gdebxnnsf.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://m.share.fanxiaobao.xyz/Article/details/gdytzglsr.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://baike.fanxiaobao.xyz/Article/details/gxwttyzlo.sHtML

[Q41] 多表连接
来源：http://www.share.fanxiaobao.xyz/Article/details/gpmrrhcqn.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.fanxiaobao.xyz/Article/details/gljblkwgl.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.share.fanxiaobao.xyz/Article/details/gswdkeaug.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.blog.fanxiaobao.xyz/Article/details/glwjsnodo.sHtML

[Q42] 连接条件附加过滤
来源：http://wap.fanxiaobao.xyz/Article/details/gzvqitdkv.sHtML

SELECT u.name, o.amount FROM users u
来源：http://wap.fanxiaobao.xyz/Article/details/gmhsvpsxq.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://read.share.fanxiaobao.xyz/Article/details/gnplmefvd.sHtML

[Q43] 标量子查询
来源：http://www.share.fanxiaobao.xyz/Article/details/gaprfjfuz.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wap.fanxiaobao.xyz/Article/details/gyhrbwjzp.sHtML

[Q44] IN 子查询
来源：http://m.share.fanxiaobao.xyz/Article/details/gjenncxeg.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://m.share.fanxiaobao.xyz/Article/details/gqewvbqpn.sHtML

[Q45] EXISTS 判断存在
来源：http://blog.fanxiaobao.xyz/Article/details/gywtnnptk.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.fanxiaobao.xyz/Article/details/gglwkdueo.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.fanxiaobao.xyz/Article/details/glwxpkbpp.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.fanxiaobao.xyz/Article/details/gxzevjzox.sHtML

[Q47] 与平均值比较
来源：http://read.share.fanxiaobao.xyz/Article/details/gxregmaln.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.share.fanxiaobao.xyz/Article/details/gekmiiomr.sHtML

[Q48] CTE 公用表表达式
来源：http://m.share.fanxiaobao.xyz/Article/details/gkvgvgbdr.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.fanxiaobao.xyz/Article/details/gplycvwvl.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwkvukczm.sHtML

[Q49] 更新单行
来源：http://mobile.fanxiaobao.xyz/Article/details/gcysobuvg.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.fanxiaobao.xyz/Article/details/gaxerdbyp.sHtML

[Q50] 批量更新
来源：http://blog.fanxiaobao.xyz/Article/details/gfzwmpdeo.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.share.fanxiaobao.xyz/Article/details/gdifvwdan.sHtML

[Q51] 用子查询更新
来源：http://baike.fanxiaobao.xyz/Article/details/geuudyifo.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gzgpshcpt.sHtML

[Q52] 删除指定行
来源：http://wap.fanxiaobao.xyz/Article/details/ggqwoylic.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.fanxiaobao.xyz/Article/details/getdyjzqi.sHtML

[Q53] 按条件删除
来源：http://www.share.fanxiaobao.xyz/Article/details/gmnwyxeol.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://3g.fanxiaobao.xyz/Article/details/gdkjneddd.sHtML

[Q54] 清空表
来源：http://3g.fanxiaobao.xyz/Article/details/gvjicdioi.sHtML

TRUNCATE TABLE logs;
来源：http://www.blog.fanxiaobao.xyz/Article/details/glerzhdtu.sHtML

[Q55] 排名（并列占位）
来源：http://wap.fanxiaobao.xyz/Article/details/glrfownsz.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.fanxiaobao.xyz/Article/details/galwsplyz.sHtML

[Q56] 密集排名（并列不占位）
来源：http://mobile.fanxiaobao.xyz/Article/details/gfwynugmj.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://baike.fanxiaobao.xyz/Article/details/gtbzkfiun.sHtML

[Q57] 行号
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbnjlslas.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gpcnjqxok.sHtML

[Q58] 累计求和
来源：http://m.share.fanxiaobao.xyz/Article/details/gopfnwgfj.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkoflrmjf.sHtML

[Q59] 分组内累计
来源：http://read.share.fanxiaobao.xyz/Article/details/gnsokkwnk.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/gvztiltjv.sHtML

[Q60] 取上一行 / 下一行
来源：http://blog.fanxiaobao.xyz/Article/details/ghckzmpjw.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.fanxiaobao.xyz/Article/details/gcxloljrm.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/gphfoythb.sHtML

[Q61] 移动平均
来源：http://blog.fanxiaobao.xyz/Article/details/gvktwvcoy.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.fanxiaobao.xyz/Article/details/gilfacrjy.sHtML

[Q62] 分组占比
来源：http://read.share.fanxiaobao.xyz/Article/details/gyvkbrzhm.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://baike.fanxiaobao.xyz/Article/details/gzephptqf.sHtML


<!-- 参考信息 -->