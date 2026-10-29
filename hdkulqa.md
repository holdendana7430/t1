代发 wailian999

Go:   // 手写递归
来源：http://3g.hesvh.cn/Article/details/gfkmueetm.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.blog.hesvh.cn/Article/details/gveuuhjsu.sHtML

C#:   // 手写递归
来源：http://www.m.share.zdbjq.cn/Article/details/gobafuubt.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://3g.hesvh.cn/Article/details/ginctaoqi.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://baike.hesvh.cn/Article/details/gumoybwlm.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.hesvh.cn/Article/details/gobnhkwpy.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.hesvh.cn/Article/details/gmyhczdcq.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.zdbjq.cn/Article/details/glqkiwbdn.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.fehbvm.com/Article/details/gttvrcrln.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://m.share.hesvh.cn/Article/details/gbgvxqeiy.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.blog.zdbjq.cn/Article/details/gqfiekwwz.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.hesvh.cn/Article/details/gprunfxah.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gziyzrrvq.sHtML

O. 并发与异步
来源：http://m.share.zdbjq.cn/Article/details/gyakesumd.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/ghxrxwwko.sHtML

[O01] 启动一个线程
来源：http://www.blog.zdbjq.cn/Article/details/gsjqywwxb.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wap.zdbjq.cn/Article/details/gyrxsqcli.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.m.share.fehbvm.com/Article/details/gebshqorp.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://3g.hesvh.cn/Article/details/gxwdmrrjy.sHtML

TS:   // 同 JS
来源：http://www.share.hesvh.cn/Article/details/gaqxfdlyh.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.blog.zdbjq.cn/Article/details/gxrnvsanu.sHtML

Go:   go f()
来源：http://mobile.hesvh.cn/Article/details/gwlwxzcai.sHtML

Ruby: Thread.new { f }
来源：http://www.m.share.fehbvm.com/Article/details/gslodneey.sHtML

C#:   Task.Run(() => F());
来源：http://m.share.zdbjq.cn/Article/details/geerxtsge.sHtML

[O02] 使用线程池
来源：http://www.blog.zdbjq.cn/Article/details/gckuuocwl.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://read.share.hesvh.cn/Article/details/gkfuyavvk.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://baike.fehbvm.com/Article/details/gsoosibfj.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.fehbvm.com/Article/details/gdoiynqzm.sHtML

TS:   // worker_threads 线程池
来源：http://mobile.zdbjq.cn/Article/details/gbnsosfgt.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://read.share.hesvh.cn/Article/details/gegdomvzx.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://blog.hesvh.cn/Article/details/gszconxrz.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.zdbjq.cn/Article/details/gvwjbhtmf.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.share.hesvh.cn/Article/details/gzayyrhlv.sHtML

[O03] 加锁保护共享数据
来源：http://blog.zdbjq.cn/Article/details/gqcdctvqm.sHtML

Py:   with lock: shared += 1
来源：http://blog.fehbvm.com/Article/details/gufbptzie.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.m.share.fehbvm.com/Article/details/gihcdvnzr.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://read.share.zdbjq.cn/Article/details/gwjziaxns.sHtML

TS:   // 同 JS
来源：http://blog.zdbjq.cn/Article/details/gfxputkin.sHtML

Java: synchronized (this) { shared++; }
来源：http://mobile.fehbvm.com/Article/details/gqoqqweqe.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.share.zdbjq.cn/Article/details/gvmsxdoyl.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://m.share.zdbjq.cn/Article/details/glcnvgjnw.sHtML

C#:   lock (gate) { shared++; }
来源：http://mobile.zdbjq.cn/Article/details/gjvzkocqq.sHtML

[O04] 定义异步函数并等待
来源：http://mobile.hesvh.cn/Article/details/geeterudz.sHtML

Py:   async def f():⏎    await g()
来源：http://www.m.share.fehbvm.com/Article/details/gjdlpjvtx.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.fehbvm.com/Article/details/ghlitykfk.sHtML

JS:   async function f() { await g(); }
来源：http://3g.hesvh.cn/Article/details/ghsaytvdr.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.m.share.fehbvm.com/Article/details/gepbehgxy.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://baike.zdbjq.cn/Article/details/gaisukxtu.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://read.share.hesvh.cn/Article/details/grqawoqzh.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://3g.zdbjq.cn/Article/details/gkyimuysi.sHtML

C#:   async Task F() { await G(); }
来源：http://baike.zdbjq.cn/Article/details/gxzsalgnl.sHtML

[O05] 并发执行并等待全部完成
来源：http://3g.hesvh.cn/Article/details/ghguuhlug.sHtML

Py:   asyncio.gather(*tasks)
来源：http://wap.zdbjq.cn/Article/details/gopedhoaw.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://3g.fehbvm.com/Article/details/gddkvshow.sHtML

JS:   await Promise.all(tasks)
来源：http://mobile.zdbjq.cn/Article/details/gpondgbrs.sHtML

TS:   await Promise.all(tasks)
来源：http://read.share.zdbjq.cn/Article/details/gwdplfyyo.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://m.share.zdbjq.cn/Article/details/gngntauaq.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://blog.zdbjq.cn/Article/details/ghvrkbhyk.sHtML

Ruby: threads.map(&:join)
来源：http://www.share.zdbjq.cn/Article/details/gxpaiddbc.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.m.share.fehbvm.com/Article/details/gsmqretfo.sHtML

[O06] 使用进程池
来源：http://baike.hesvh.cn/Article/details/guxazgtpt.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mobile.hesvh.cn/Article/details/gynadfufn.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://wap.hesvh.cn/Article/details/gzkopmuul.sHtML

JS:   // child_process / cluster 模块
来源：http://read.share.fehbvm.com/Article/details/ggictsxao.sHtML

TS:   // child_process / cluster 模块
来源：http://baike.hesvh.cn/Article/details/gjnfwcsox.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://3g.fehbvm.com/Article/details/gvzoqfkkk.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wap.zdbjq.cn/Article/details/gfnlcpsbj.sHtML

Ruby: // fork 块
来源：http://read.share.hesvh.cn/Article/details/gshdoebir.sHtML

C#:   Parallel.For
来源：http://www.share.zdbjq.cn/Article/details/gjezkoqup.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/ggavellvq.sHtML

P. 常用工具函数
来源：http://baike.fehbvm.com/Article/details/gbvfnibal.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gnwgpyvjn.sHtML

[P01] 生成 UUID
来源：http://wap.hesvh.cn/Article/details/gkkgaxjqo.sHtML

Py:   str(uuid.uuid4())
来源：http://www.blog.zdbjq.cn/Article/details/gsajaubse.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.share.zdbjq.cn/Article/details/gjnehrklg.sHtML

JS:   crypto.randomUUID()
来源：http://www.m.share.hesvh.cn/Article/details/gvmkwltsz.sHtML

TS:   crypto.randomUUID()
来源：http://www.blog.zdbjq.cn/Article/details/gpkxjqcan.sHtML

Java: UUID.randomUUID().toString()
来源：http://mobile.fehbvm.com/Article/details/gkiucbcjd.sHtML

Go:   // 用 github.com/google/uuid
来源：http://read.share.hesvh.cn/Article/details/gelucabje.sHtML

Ruby: SecureRandom.uuid
来源：http://read.share.zdbjq.cn/Article/details/gqvehtwkj.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://mobile.zdbjq.cn/Article/details/gafowxseu.sHtML

[P02] MD5 / SHA256 摘要
来源：http://3g.hesvh.cn/Article/details/gfekmgjfh.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mobile.hesvh.cn/Article/details/gmqsgbasx.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.fehbvm.com/Article/details/gtgxoqvug.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://blog.fehbvm.com/Article/details/gmoadxniu.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.share.fehbvm.com/Article/details/gbkidpjtg.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mobile.fehbvm.com/Article/details/ghmzntvze.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://3g.hesvh.cn/Article/details/glwokhlol.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://3g.zdbjq.cn/Article/details/gyxowqfrh.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.blog.zdbjq.cn/Article/details/glcfbpmoz.sHtML

[P03] 生成短随机字符串
来源：http://www.share.zdbjq.cn/Article/details/gckhsuvqa.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://read.share.fehbvm.com/Article/details/gofmfzwuy.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://baike.hesvh.cn/Article/details/gsakfgbdw.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.fehbvm.com/Article/details/gzmvlxhmo.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.zdbjq.cn/Article/details/gdpchyfec.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wap.fehbvm.com/Article/details/gpovuhnox.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.m.share.fehbvm.com/Article/details/ggvbmobne.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.m.share.fehbvm.com/Article/details/gnrezsalw.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wap.zdbjq.cn/Article/details/gkficutrw.sHtML

[P04] 求长度
来源：http://read.share.hesvh.cn/Article/details/gwpqiheit.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wap.fehbvm.com/Article/details/gaimbvmjj.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.zdbjq.cn/Article/details/gdyhmvmgv.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.zdbjq.cn/Article/details/gjjxllwsi.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.zdbjq.cn/Article/details/gvdtxwoco.sHtML

Java: list.size();  map.size();  s.length()
来源：http://mobile.hesvh.cn/Article/details/gruhqcyqa.sHtML

Go:   len(arr);  len(m)
来源：http://read.share.fehbvm.com/Article/details/gjkawrtog.sHtML

Ruby: x.length;  x.size
来源：http://www.m.share.zdbjq.cn/Article/details/glvsdnwth.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://baike.zdbjq.cn/Article/details/gaxkpfnpg.sHtML

[P05] 判断两个对象内容是否相等
来源：http://read.share.fehbvm.com/Article/details/gmgylyegu.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://mobile.zdbjq.cn/Article/details/gdkpdrvsx.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.blog.fehbvm.com/Article/details/gnezuafav.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://3g.hesvh.cn/Article/details/gwtdnixgd.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.zdbjq.cn/Article/details/gwesmkjss.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://baike.hesvh.cn/Article/details/gnseoyfnr.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.share.zdbjq.cn/Article/details/gyomlusxr.sHtML

Ruby: a == b
来源：http://baike.hesvh.cn/Article/details/gbvmzzyjo.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://read.share.fehbvm.com/Article/details/gczncwszk.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://3g.hesvh.cn/Article/details/ggxjbenci.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mobile.fehbvm.com/Article/details/gfykumadb.sHtML

PHP:  if (empty($x)) {}
来源：http://www.share.fehbvm.com/Article/details/gvyqclarp.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://3g.fehbvm.com/Article/details/gibtpuetd.sHtML

TS:   if (x == null) {}
来源：http://wap.hesvh.cn/Article/details/gtaszaamh.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://baike.zdbjq.cn/Article/details/gmawjgkgj.sHtML

Go:   if x == nil {}
来源：http://mobile.hesvh.cn/Article/details/ghhgafwdy.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.m.share.fehbvm.com/Article/details/gkhendyug.sHtML

C#:   if (x is null) {}
来源：http://www.share.fehbvm.com/Article/details/gnxmxarcs.sHtML

[P07] 防抖与节流
来源：http://blog.zdbjq.cn/Article/details/glpyzpqdp.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://baike.fehbvm.com/Article/details/gqhlljplx.sHtML

PHP:  // 手写时间戳比较
来源：http://www.share.zdbjq.cn/Article/details/glaojytfg.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.fehbvm.com/Article/details/gilexlzgd.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.fehbvm.com/Article/details/gzsskgdrj.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://m.share.fehbvm.com/Article/details/gtsrbutzm.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.hesvh.cn/Article/details/gdjzdriqh.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://m.share.zdbjq.cn/Article/details/giyohujmc.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://baike.fehbvm.com/Article/details/gslynlcjn.sHtML

[P08] 处理浮点精度问题
来源：http://baike.hesvh.cn/Article/details/ghujumclx.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wap.hesvh.cn/Article/details/gyrxpnzhg.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://read.share.zdbjq.cn/Article/details/gqgxfsrnb.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.hesvh.cn/Article/details/gykjpapzt.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://blog.zdbjq.cn/Article/details/gfucfmuex.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wap.zdbjq.cn/Article/details/gvhwmavrj.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.share.hesvh.cn/Article/details/gjtqqjtuj.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mobile.zdbjq.cn/Article/details/ghginjgxd.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://baike.fehbvm.com/Article/details/gekdotqau.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gmcmiobkt.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://blog.zdbjq.cn/Article/details/ghmmsxbvd.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/ginviitgu.sHtML

[Q01] 创建表
来源：http://baike.hesvh.cn/Article/details/gqpbiedlu.sHtML

CREATE TABLE users (
来源：http://www.blog.hesvh.cn/Article/details/gdenmajpx.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.hesvh.cn/Article/details/ggznbtknu.sHtML

name VARCHAR(50) NOT NULL,
来源：http://mobile.fehbvm.com/Article/details/gynknxaqa.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.m.share.zdbjq.cn/Article/details/grexsjzse.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://blog.zdbjq.cn/Article/details/gdppbdkgx.sHtML

);
来源：http://www.share.fehbvm.com/Article/details/gedrckqnv.sHtML

[Q02] 创建带外键的表
来源：http://www.m.share.hesvh.cn/Article/details/gquxqrtqq.sHtML

CREATE TABLE orders (
来源：http://www.share.hesvh.cn/Article/details/gpoqcclnq.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.hesvh.cn/Article/details/gwrytdrdx.sHtML

user_id INT NOT NULL,
来源：http://www.blog.hesvh.cn/Article/details/gldxuayep.sHtML

amount DECIMAL(10, 2),
来源：http://blog.zdbjq.cn/Article/details/gcluqrjth.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wap.fehbvm.com/Article/details/glnnjkttv.sHtML

);
来源：http://3g.zdbjq.cn/Article/details/gjnxhthao.sHtML

[Q03] 增加列
来源：http://baike.zdbjq.cn/Article/details/girhzzzqv.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://3g.fehbvm.com/Article/details/gwsoenmtu.sHtML

[Q04] 修改列类型
来源：http://blog.hesvh.cn/Article/details/gjlhalavk.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mobile.zdbjq.cn/Article/details/gwvjiqtsg.sHtML

[Q05] 重命名列
来源：http://baike.zdbjq.cn/Article/details/gzdqxiqvw.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.m.share.hesvh.cn/Article/details/gpgpovdzf.sHtML

[Q06] 删除列
来源：http://3g.hesvh.cn/Article/details/gwyzjoutc.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.share.fehbvm.com/Article/details/gipdtypxi.sHtML

[Q07] 删除表
来源：http://read.share.hesvh.cn/Article/details/gftzcadrr.sHtML

DROP TABLE IF EXISTS orders;
来源：http://read.share.fehbvm.com/Article/details/gumxbnoot.sHtML

[Q08] 创建普通索引
来源：http://www.blog.hesvh.cn/Article/details/gfmgvreet.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.share.fehbvm.com/Article/details/gdxqmpcwk.sHtML

[Q09] 创建唯一索引
来源：http://www.share.hesvh.cn/Article/details/gclkcfyjk.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://read.share.fehbvm.com/Article/details/gooyafpex.sHtML

[Q10] 插入单行
来源：http://read.share.hesvh.cn/Article/details/gmsjfonhq.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.share.zdbjq.cn/Article/details/gopwyfrot.sHtML

[Q11] 一次插入多行
来源：http://mobile.zdbjq.cn/Article/details/gusixpgkz.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://blog.fehbvm.com/Article/details/gcuarqlur.sHtML

[Q12] 插入后取自增 ID
来源：http://baike.hesvh.cn/Article/details/gzrxzhwkp.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://wap.hesvh.cn/Article/details/gyvumhpmo.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.m.share.zdbjq.cn/Article/details/gvgzymgms.sHtML

[Q13] 忽略重复插入
来源：http://mobile.zdbjq.cn/Article/details/glvzsuhtv.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mobile.fehbvm.com/Article/details/gnpjgmwxm.sHtML

[Q14] 存在则更新（upsert）
来源：http://blog.fehbvm.com/Article/details/gtusihubv.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://m.share.hesvh.cn/Article/details/gwgepomvy.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.m.share.zdbjq.cn/Article/details/gwzippvae.sHtML

[Q15] 查询全部
来源：http://read.share.hesvh.cn/Article/details/goqkskfkn.sHtML

SELECT * FROM users;
来源：http://www.share.zdbjq.cn/Article/details/ghfmmwpss.sHtML

[Q16] 查询指定列
来源：http://3g.zdbjq.cn/Article/details/ghipkxrym.sHtML

SELECT id, name FROM users;
来源：http://wap.fehbvm.com/Article/details/goihmrcwe.sHtML

[Q17] 条件查询
来源：http://www.blog.fehbvm.com/Article/details/gmhrcvsrk.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.share.zdbjq.cn/Article/details/gppekiiho.sHtML

[Q18] 模糊匹配
来源：http://www.share.hesvh.cn/Article/details/gufdzoknj.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://read.share.zdbjq.cn/Article/details/gsaatvuoo.sHtML

[Q19] 范围查询
来源：http://blog.fehbvm.com/Article/details/gmciceeuf.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.share.hesvh.cn/Article/details/gjyctvngp.sHtML

[Q20] IN 列表
来源：http://read.share.hesvh.cn/Article/details/glotrrird.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.zdbjq.cn/Article/details/gfucqmbxh.sHtML

[Q21] 空值判断
来源：http://3g.fehbvm.com/Article/details/gixrnhuaj.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.blog.hesvh.cn/Article/details/grafkonbx.sHtML

[Q22] 排序
来源：http://wap.hesvh.cn/Article/details/gbgtrobwm.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.zdbjq.cn/Article/details/gixnyvped.sHtML

[Q23] 分页
来源：http://m.share.zdbjq.cn/Article/details/gknopryvm.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mobile.zdbjq.cn/Article/details/glwsudshj.sHtML

[Q24] 去重
来源：http://3g.zdbjq.cn/Article/details/gerkwulci.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gyvkmvcxm.sHtML

[Q25] 只取前 N 条
来源：http://blog.zdbjq.cn/Article/details/gfayogykf.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://m.share.hesvh.cn/Article/details/guzvjvexi.sHtML

[Q26] 计数
来源：http://wap.hesvh.cn/Article/details/gzsvjvtck.sHtML

SELECT COUNT(*) FROM users;
来源：http://wap.hesvh.cn/Article/details/gfirfrrqz.sHtML

[Q27] 条件计数
来源：http://3g.fehbvm.com/Article/details/gkmhiyuii.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://read.share.hesvh.cn/Article/details/gswhwxwrp.sHtML

[Q28] 求和与平均
来源：http://read.share.fehbvm.com/Article/details/gqgggjpjm.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wap.hesvh.cn/Article/details/gnxzepvsj.sHtML

[Q29] 最大最小值
来源：http://3g.zdbjq.cn/Article/details/gjnfvltfs.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.fehbvm.com/Article/details/gunwcejyz.sHtML

[Q30] 分组统计
来源：http://3g.hesvh.cn/Article/details/gvbyltwui.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://baike.zdbjq.cn/Article/details/gesiybcpc.sHtML

[Q31] 分组后过滤
来源：http://www.blog.zdbjq.cn/Article/details/giwsuxpyp.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.m.share.hesvh.cn/Article/details/gcgumghav.sHtML

[Q32] 分组拼接字符串
来源：http://mobile.zdbjq.cn/Article/details/gkbwwpvbg.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://read.share.fehbvm.com/Article/details/gboctnmuk.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.fehbvm.com/Article/details/gwfklfdgk.sHtML

[Q33] 多列分组
来源：http://www.blog.hesvh.cn/Article/details/ggkqvgesq.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://baike.hesvh.cn/Article/details/gkwqepnng.sHtML

[Q34] 每组取第一条
来源：http://read.share.hesvh.cn/Article/details/gwkunoeyr.sHtML

SELECT * FROM (
来源：http://blog.fehbvm.com/Article/details/glpkuanop.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.blog.hesvh.cn/Article/details/gynupjule.sHtML

) t WHERE rn = 1;
来源：http://read.share.hesvh.cn/Article/details/gaanbgkug.sHtML

[Q35] 内连接
来源：http://mobile.hesvh.cn/Article/details/gjlmxowml.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://read.share.fehbvm.com/Article/details/gpdcughvk.sHtML

[Q36] 左连接
来源：http://m.share.zdbjq.cn/Article/details/gbcbovpbp.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.zdbjq.cn/Article/details/gytjhlimf.sHtML

[Q37] 右连接
来源：http://wap.hesvh.cn/Article/details/gjkytgjzx.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.share.zdbjq.cn/Article/details/gettfebdf.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.fehbvm.com/Article/details/gileptsmp.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.blog.hesvh.cn/Article/details/ghfxsbuwu.sHtML

[Q39] 自连接（查上下级）
来源：http://read.share.fehbvm.com/Article/details/gzeldjvfb.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://read.share.hesvh.cn/Article/details/grgdousja.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.fehbvm.com/Article/details/glprfmbhv.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.m.share.zdbjq.cn/Article/details/gjdzbtxdc.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://baike.zdbjq.cn/Article/details/goeqlnhpy.sHtML

[Q41] 多表连接
来源：http://wap.hesvh.cn/Article/details/gbbbxeyke.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.fehbvm.com/Article/details/ggjseptbj.sHtML

JOIN users u ON u.id = o.user_id
来源：http://baike.fehbvm.com/Article/details/grmnaktpe.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://wap.hesvh.cn/Article/details/gmdkcvkjw.sHtML

[Q42] 连接条件附加过滤
来源：http://mobile.hesvh.cn/Article/details/genafcjjt.sHtML

SELECT u.name, o.amount FROM users u
来源：http://wap.fehbvm.com/Article/details/gsxgyxvlg.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.hesvh.cn/Article/details/ghpbnmndb.sHtML

[Q43] 标量子查询
来源：http://www.m.share.hesvh.cn/Article/details/gcodcvmvn.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.m.share.zdbjq.cn/Article/details/gbumjtrky.sHtML

[Q44] IN 子查询
来源：http://3g.zdbjq.cn/Article/details/gzdtpiqav.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.fehbvm.com/Article/details/gkcayuytd.sHtML

[Q45] EXISTS 判断存在
来源：http://mobile.fehbvm.com/Article/details/gvjlsoxvx.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.zdbjq.cn/Article/details/gndnuqnet.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.hesvh.cn/Article/details/gwbopznxk.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.fehbvm.com/Article/details/gitgevvdv.sHtML

[Q47] 与平均值比较
来源：http://3g.fehbvm.com/Article/details/gonnpubgr.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wap.fehbvm.com/Article/details/gywqqzrja.sHtML

[Q48] CTE 公用表表达式
来源：http://3g.zdbjq.cn/Article/details/ggphdhgeh.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.zdbjq.cn/Article/details/gdyxcqbkd.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.hesvh.cn/Article/details/gkokwlnhm.sHtML

[Q49] 更新单行
来源：http://mobile.fehbvm.com/Article/details/gsqeymhtd.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.fehbvm.com/Article/details/gojtuyvyc.sHtML

[Q50] 批量更新
来源：http://www.m.share.zdbjq.cn/Article/details/gwredilfb.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.share.zdbjq.cn/Article/details/gceykljlb.sHtML

[Q51] 用子查询更新
来源：http://wap.zdbjq.cn/Article/details/gesgngrxx.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.zdbjq.cn/Article/details/gdrhlacjl.sHtML

[Q52] 删除指定行
来源：http://m.share.zdbjq.cn/Article/details/gdftgecsn.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.fehbvm.com/Article/details/gkmubuiaw.sHtML

[Q53] 按条件删除
来源：http://wap.hesvh.cn/Article/details/gxgvwmkpz.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://m.share.zdbjq.cn/Article/details/gceblgxtz.sHtML

[Q54] 清空表
来源：http://read.share.fehbvm.com/Article/details/gfreiqtay.sHtML

TRUNCATE TABLE logs;
来源：http://mobile.hesvh.cn/Article/details/golnbxvut.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.fehbvm.com/Article/details/gtbfdwbri.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://blog.zdbjq.cn/Article/details/gumxqmnie.sHtML

[Q56] 密集排名（并列不占位）
来源：http://mobile.zdbjq.cn/Article/details/gffuxkelv.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.share.fehbvm.com/Article/details/gpbagnmdt.sHtML

[Q57] 行号
来源：http://read.share.hesvh.cn/Article/details/ghbbvuuey.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gwroxqkiv.sHtML

[Q58] 累计求和
来源：http://www.m.share.fehbvm.com/Article/details/gnaejcivy.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.hesvh.cn/Article/details/gwwkkvjix.sHtML

[Q59] 分组内累计
来源：http://3g.fehbvm.com/Article/details/gxmnaldso.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://3g.zdbjq.cn/Article/details/gbpwlhjem.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.zdbjq.cn/Article/details/gofopqeff.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.hesvh.cn/Article/details/gwvegkuqc.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://baike.fehbvm.com/Article/details/gpsyreyds.sHtML

[Q61] 移动平均
来源：http://blog.hesvh.cn/Article/details/gahryjfgf.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wap.fehbvm.com/Article/details/gyailvawn.sHtML

[Q62] 分组占比
来源：http://3g.zdbjq.cn/Article/details/ganomfhms.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.zdbjq.cn/Article/details/gdxerspxv.sHtML

[Q63] 开启事务
来源：http://blog.hesvh.cn/Article/details/gknvhirzy.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.hesvh.cn/Article/details/gtcxzazjo.sHtML

[Q64] 提交事务
来源：http://m.share.fehbvm.com/Article/details/gagafclgr.sHtML

COMMIT;
来源：http://blog.zdbjq.cn/Article/details/gsisfwmyb.sHtML

[Q65] 回滚事务
来源：http://read.share.fehbvm.com/Article/details/gqlzbnpwx.sHtML

ROLLBACK;
来源：http://m.share.hesvh.cn/Article/details/gdpvenxrz.sHtML

[Q66] 行锁查询
来源：http://blog.zdbjq.cn/Article/details/gyvktmepn.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.fehbvm.com/Article/details/ggkpehdgz.sHtML


<!-- 参考信息 -->