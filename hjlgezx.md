代发 wailian999

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mobile.fehbvm.com/Article/details/gbturldbl.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.share.hesvh.cn/Article/details/gswqvdsaw.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.zdbjq.cn/Article/details/gztqxjgzq.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.fehbvm.com/Article/details/gpqsmnsbq.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.zdbjq.cn/Article/details/gytncevkz.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.blog.zdbjq.cn/Article/details/ggrajimow.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.blog.zdbjq.cn/Article/details/glvhyzflu.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.fehbvm.com/Article/details/gbgwmfjch.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gadfeybri.sHtML

O. 并发与异步
来源：http://wap.hesvh.cn/Article/details/genauovmj.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/ggmuwmxxk.sHtML

[O01] 启动一个线程
来源：http://www.share.fehbvm.com/Article/details/gpghpfsrq.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://blog.zdbjq.cn/Article/details/gtruwsejt.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://blog.hesvh.cn/Article/details/gzcqutmmz.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.m.share.zdbjq.cn/Article/details/gndrxtsip.sHtML

TS:   // 同 JS
来源：http://www.m.share.zdbjq.cn/Article/details/gbqzluzkv.sHtML

Java: new Thread(() -> f()).start()
来源：http://wap.fehbvm.com/Article/details/gzhhfmdzz.sHtML

Go:   go f()
来源：http://m.share.hesvh.cn/Article/details/gfyvxhvho.sHtML

Ruby: Thread.new { f }
来源：http://mobile.fehbvm.com/Article/details/gxmulmjfk.sHtML

C#:   Task.Run(() => F());
来源：http://www.m.share.hesvh.cn/Article/details/gsccwtwaa.sHtML

[O02] 使用线程池
来源：http://www.blog.zdbjq.cn/Article/details/geoickkwh.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.m.share.hesvh.cn/Article/details/gbedquxdv.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://read.share.zdbjq.cn/Article/details/gjchuurue.sHtML

JS:   // worker_threads 线程池
来源：http://m.share.fehbvm.com/Article/details/ggtgjjxnh.sHtML

TS:   // worker_threads 线程池
来源：http://blog.fehbvm.com/Article/details/guhaymzyy.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.m.share.zdbjq.cn/Article/details/gnzsrorkh.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wap.fehbvm.com/Article/details/gmxjfswgh.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.share.zdbjq.cn/Article/details/gqidizogc.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.hesvh.cn/Article/details/gqiebmray.sHtML

[O03] 加锁保护共享数据
来源：http://baike.zdbjq.cn/Article/details/gktsylxfc.sHtML

Py:   with lock: shared += 1
来源：http://www.share.fehbvm.com/Article/details/grhocrtdt.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.m.share.hesvh.cn/Article/details/gwyzftxqu.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://read.share.zdbjq.cn/Article/details/gcsjielut.sHtML

TS:   // 同 JS
来源：http://3g.hesvh.cn/Article/details/grbtksiys.sHtML

Java: synchronized (this) { shared++; }
来源：http://blog.fehbvm.com/Article/details/gzsofbpsz.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.share.fehbvm.com/Article/details/ginhcdffi.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://blog.fehbvm.com/Article/details/gikslihcl.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.hesvh.cn/Article/details/glusgsvoq.sHtML

[O04] 定义异步函数并等待
来源：http://baike.zdbjq.cn/Article/details/glejtjkwa.sHtML

Py:   async def f():⏎    await g()
来源：http://baike.hesvh.cn/Article/details/gpplwltql.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://read.share.zdbjq.cn/Article/details/gmhcriusw.sHtML

JS:   async function f() { await g(); }
来源：http://mobile.hesvh.cn/Article/details/geombzmle.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.zdbjq.cn/Article/details/gomngqpuu.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.blog.hesvh.cn/Article/details/gpwbkveri.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.blog.zdbjq.cn/Article/details/ghwdapufg.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.share.fehbvm.com/Article/details/genbwntqv.sHtML

C#:   async Task F() { await G(); }
来源：http://3g.fehbvm.com/Article/details/gxzxovfmo.sHtML

[O05] 并发执行并等待全部完成
来源：http://read.share.zdbjq.cn/Article/details/gapiqefyd.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.m.share.hesvh.cn/Article/details/gttjlvprr.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://3g.zdbjq.cn/Article/details/gpdkpiocw.sHtML

JS:   await Promise.all(tasks)
来源：http://www.m.share.hesvh.cn/Article/details/ggtouxtnh.sHtML

TS:   await Promise.all(tasks)
来源：http://blog.fehbvm.com/Article/details/gpayspixr.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.share.zdbjq.cn/Article/details/gfbzjapvs.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://3g.zdbjq.cn/Article/details/gwbigcesc.sHtML

Ruby: threads.map(&:join)
来源：http://www.m.share.hesvh.cn/Article/details/gmfonbstk.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://baike.zdbjq.cn/Article/details/gfhfhlayg.sHtML

[O06] 使用进程池
来源：http://3g.hesvh.cn/Article/details/goznokuah.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.m.share.zdbjq.cn/Article/details/gskkqwuno.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://baike.fehbvm.com/Article/details/gyfkdzorr.sHtML

JS:   // child_process / cluster 模块
来源：http://www.share.hesvh.cn/Article/details/glhnkmscy.sHtML

TS:   // child_process / cluster 模块
来源：http://www.share.zdbjq.cn/Article/details/gymgsvkut.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://3g.fehbvm.com/Article/details/guzkxjpak.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wap.zdbjq.cn/Article/details/ggvipihvc.sHtML

Ruby: // fork 块
来源：http://mobile.zdbjq.cn/Article/details/gjzpjoctr.sHtML

C#:   Parallel.For
来源：http://wap.hesvh.cn/Article/details/gnqumomii.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gynpwammc.sHtML

P. 常用工具函数
来源：http://wap.hesvh.cn/Article/details/ggoudaqkx.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gzmbhdsab.sHtML

[P01] 生成 UUID
来源：http://baike.hesvh.cn/Article/details/gzmckncay.sHtML

Py:   str(uuid.uuid4())
来源：http://www.share.zdbjq.cn/Article/details/ghexpvfnq.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wap.zdbjq.cn/Article/details/gckhohfte.sHtML

JS:   crypto.randomUUID()
来源：http://www.blog.zdbjq.cn/Article/details/gufholyks.sHtML

TS:   crypto.randomUUID()
来源：http://mobile.zdbjq.cn/Article/details/glvxpabup.sHtML

Java: UUID.randomUUID().toString()
来源：http://m.share.zdbjq.cn/Article/details/gfuewjjmc.sHtML

Go:   // 用 github.com/google/uuid
来源：http://mobile.hesvh.cn/Article/details/gojekhbtv.sHtML

Ruby: SecureRandom.uuid
来源：http://www.share.hesvh.cn/Article/details/gwzjzsmtv.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://m.share.fehbvm.com/Article/details/gtqufzulm.sHtML

[P02] MD5 / SHA256 摘要
来源：http://read.share.fehbvm.com/Article/details/gdzvydrzi.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://m.share.zdbjq.cn/Article/details/gtfbajvfj.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.fehbvm.com/Article/details/gnkevzrfm.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://read.share.zdbjq.cn/Article/details/gppcfyroc.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.m.share.hesvh.cn/Article/details/gbyhxfqbg.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mobile.zdbjq.cn/Article/details/giiylovyj.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://3g.fehbvm.com/Article/details/gcmgzsuwn.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gjhbdmhhy.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wap.hesvh.cn/Article/details/gzodvkuhd.sHtML

[P03] 生成短随机字符串
来源：http://www.blog.hesvh.cn/Article/details/gkjufpmgm.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://baike.zdbjq.cn/Article/details/gqgzxeufn.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wap.fehbvm.com/Article/details/gqooxdlwh.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.zdbjq.cn/Article/details/gxtqhaurk.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.fehbvm.com/Article/details/gpsqhwsaz.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mobile.hesvh.cn/Article/details/goeqkpdbt.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wap.fehbvm.com/Article/details/gijzpqgtk.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.share.fehbvm.com/Article/details/gjnghmobj.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://baike.hesvh.cn/Article/details/gbybigajt.sHtML

[P04] 求长度
来源：http://3g.zdbjq.cn/Article/details/glltjkmpb.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.share.zdbjq.cn/Article/details/gbuirhuur.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.hesvh.cn/Article/details/ggwxdtxaf.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.fehbvm.com/Article/details/grjovilmo.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.fehbvm.com/Article/details/gkbhsepyp.sHtML

Java: list.size();  map.size();  s.length()
来源：http://blog.fehbvm.com/Article/details/gvecmqrkh.sHtML

Go:   len(arr);  len(m)
来源：http://baike.fehbvm.com/Article/details/guskijnxn.sHtML

Ruby: x.length;  x.size
来源：http://www.blog.hesvh.cn/Article/details/gcfsapubu.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.m.share.fehbvm.com/Article/details/gycnokdhj.sHtML

[P05] 判断两个对象内容是否相等
来源：http://m.share.hesvh.cn/Article/details/gdmqhvfnz.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://baike.hesvh.cn/Article/details/ggndmodot.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.m.share.zdbjq.cn/Article/details/gwamxzmhm.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.m.share.zdbjq.cn/Article/details/gbbtbzwzw.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.zdbjq.cn/Article/details/gktzlxtpm.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://m.share.hesvh.cn/Article/details/giaqodgmt.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://blog.fehbvm.com/Article/details/gppromhxk.sHtML

Ruby: a == b
来源：http://read.share.fehbvm.com/Article/details/gzolnpilg.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.m.share.hesvh.cn/Article/details/gmlmpctak.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://read.share.zdbjq.cn/Article/details/gfpimjsvy.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://baike.hesvh.cn/Article/details/gjgybruer.sHtML

PHP:  if (empty($x)) {}
来源：http://www.m.share.zdbjq.cn/Article/details/ggufxamjd.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://m.share.fehbvm.com/Article/details/gabrcsvlt.sHtML

TS:   if (x == null) {}
来源：http://www.m.share.fehbvm.com/Article/details/gdposayou.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.m.share.hesvh.cn/Article/details/gjeorewvi.sHtML

Go:   if x == nil {}
来源：http://baike.hesvh.cn/Article/details/grtboxlim.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.share.hesvh.cn/Article/details/gjayrwrxh.sHtML

C#:   if (x is null) {}
来源：http://read.share.fehbvm.com/Article/details/gkksqgmzf.sHtML

[P07] 防抖与节流
来源：http://3g.fehbvm.com/Article/details/ghswvutfm.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wap.zdbjq.cn/Article/details/gfwsxwxpu.sHtML

PHP:  // 手写时间戳比较
来源：http://www.m.share.zdbjq.cn/Article/details/gekysigzd.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.fehbvm.com/Article/details/gxbiyneip.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.zdbjq.cn/Article/details/gwydvltco.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.blog.hesvh.cn/Article/details/gwixepdbe.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://3g.hesvh.cn/Article/details/ghwmhumid.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.share.fehbvm.com/Article/details/gtxbhnapv.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://blog.hesvh.cn/Article/details/gvcewnyqf.sHtML

[P08] 处理浮点精度问题
来源：http://wap.hesvh.cn/Article/details/gwhgmchhh.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wap.hesvh.cn/Article/details/glihyoowg.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.share.zdbjq.cn/Article/details/gtlbdneed.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://blog.zdbjq.cn/Article/details/gdyytiizq.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mobile.hesvh.cn/Article/details/giscxgiek.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mobile.fehbvm.com/Article/details/gpinketze.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wap.fehbvm.com/Article/details/ghwayxfvz.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.blog.zdbjq.cn/Article/details/gszxlhbkt.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://3g.zdbjq.cn/Article/details/gmuzvsyqz.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/ghfddeksu.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wap.fehbvm.com/Article/details/gszhqpczr.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gbtceqpdb.sHtML

[Q01] 创建表
来源：http://wap.zdbjq.cn/Article/details/gjyhnouyd.sHtML

CREATE TABLE users (
来源：http://www.m.share.zdbjq.cn/Article/details/gbncozsag.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.fehbvm.com/Article/details/gjthsfmxx.sHtML

name VARCHAR(50) NOT NULL,
来源：http://baike.hesvh.cn/Article/details/gkoobbyxv.sHtML

email VARCHAR(100) UNIQUE,
来源：http://blog.zdbjq.cn/Article/details/gnhrtbxbr.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://3g.fehbvm.com/Article/details/gqauyuxoh.sHtML

);
来源：http://www.share.zdbjq.cn/Article/details/gjvwrlsba.sHtML

[Q02] 创建带外键的表
来源：http://3g.zdbjq.cn/Article/details/gyhxxjzkx.sHtML

CREATE TABLE orders (
来源：http://m.share.fehbvm.com/Article/details/gvsocynbb.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.hesvh.cn/Article/details/gqkuwfynx.sHtML

user_id INT NOT NULL,
来源：http://blog.zdbjq.cn/Article/details/gkoeionrb.sHtML

amount DECIMAL(10, 2),
来源：http://mobile.zdbjq.cn/Article/details/gtiusrlkc.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.share.zdbjq.cn/Article/details/gryroasoq.sHtML

);
来源：http://www.blog.fehbvm.com/Article/details/gqpnhfokc.sHtML

[Q03] 增加列
来源：http://www.m.share.fehbvm.com/Article/details/gizoureaz.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://baike.zdbjq.cn/Article/details/grdtuysce.sHtML

[Q04] 修改列类型
来源：http://m.share.zdbjq.cn/Article/details/glyjcurbt.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://baike.fehbvm.com/Article/details/gjwlppccd.sHtML

[Q05] 重命名列
来源：http://baike.hesvh.cn/Article/details/gowoatdyj.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://m.share.zdbjq.cn/Article/details/gohhraydr.sHtML

[Q06] 删除列
来源：http://m.share.hesvh.cn/Article/details/gxyfilslx.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://3g.zdbjq.cn/Article/details/geyfukwju.sHtML

[Q07] 删除表
来源：http://wap.fehbvm.com/Article/details/gspbdifna.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.blog.zdbjq.cn/Article/details/gmxgtfbzt.sHtML

[Q08] 创建普通索引
来源：http://mobile.hesvh.cn/Article/details/gwpgtphvp.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://blog.fehbvm.com/Article/details/grqjiwjxd.sHtML

[Q09] 创建唯一索引
来源：http://wap.zdbjq.cn/Article/details/gelaazaxa.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.blog.hesvh.cn/Article/details/gpeatvwxb.sHtML

[Q10] 插入单行
来源：http://wap.fehbvm.com/Article/details/gxzgvjakp.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mobile.fehbvm.com/Article/details/grzyzykvj.sHtML

[Q11] 一次插入多行
来源：http://baike.fehbvm.com/Article/details/gdplqbygf.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mobile.fehbvm.com/Article/details/gmhdaaprj.sHtML

[Q12] 插入后取自增 ID
来源：http://3g.zdbjq.cn/Article/details/gwrzcmgeq.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.share.hesvh.cn/Article/details/gmhgxeslo.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wap.zdbjq.cn/Article/details/gvdzkmqpe.sHtML

[Q13] 忽略重复插入
来源：http://read.share.zdbjq.cn/Article/details/gsjhcnkql.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.share.zdbjq.cn/Article/details/gwfrffbrl.sHtML

[Q14] 存在则更新（upsert）
来源：http://mobile.zdbjq.cn/Article/details/gxmurbrhk.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://3g.fehbvm.com/Article/details/gelxamhcw.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://m.share.hesvh.cn/Article/details/gnuepmjte.sHtML

[Q15] 查询全部
来源：http://www.blog.fehbvm.com/Article/details/gyzjgbfei.sHtML

SELECT * FROM users;
来源：http://blog.hesvh.cn/Article/details/gvwocjsax.sHtML

[Q16] 查询指定列
来源：http://www.share.fehbvm.com/Article/details/grkwriqlm.sHtML

SELECT id, name FROM users;
来源：http://3g.zdbjq.cn/Article/details/godocetqg.sHtML

[Q17] 条件查询
来源：http://baike.zdbjq.cn/Article/details/gxhieiekv.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://3g.fehbvm.com/Article/details/gwtggbgsk.sHtML

[Q18] 模糊匹配
来源：http://mobile.zdbjq.cn/Article/details/gmcdrfjqa.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://3g.hesvh.cn/Article/details/guurbhzvl.sHtML

[Q19] 范围查询
来源：http://mobile.hesvh.cn/Article/details/gnzuhzeaf.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://blog.fehbvm.com/Article/details/gvrpiowmt.sHtML

[Q20] IN 列表
来源：http://read.share.fehbvm.com/Article/details/grtqpixax.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.share.zdbjq.cn/Article/details/glvseppvy.sHtML

[Q21] 空值判断
来源：http://www.share.fehbvm.com/Article/details/glejvfhfi.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.hesvh.cn/Article/details/ggtexfhor.sHtML

[Q22] 排序
来源：http://mobile.hesvh.cn/Article/details/gzztwxnnp.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wap.hesvh.cn/Article/details/gpiuhypgr.sHtML

[Q23] 分页
来源：http://3g.fehbvm.com/Article/details/gaiukrrko.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://3g.hesvh.cn/Article/details/giviatsgf.sHtML

[Q24] 去重
来源：http://mobile.hesvh.cn/Article/details/guksjwztb.sHtML

SELECT DISTINCT city FROM users;
来源：http://wap.zdbjq.cn/Article/details/gqcsvfahm.sHtML

[Q25] 只取前 N 条
来源：http://read.share.zdbjq.cn/Article/details/gwjrpweli.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.share.fehbvm.com/Article/details/ghqyjqlux.sHtML

[Q26] 计数
来源：http://wap.hesvh.cn/Article/details/gnggxddjd.sHtML

SELECT COUNT(*) FROM users;
来源：http://3g.zdbjq.cn/Article/details/gfficzysf.sHtML

[Q27] 条件计数
来源：http://read.share.hesvh.cn/Article/details/gyzhjqenx.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://3g.hesvh.cn/Article/details/gazrbwwru.sHtML

[Q28] 求和与平均
来源：http://m.share.hesvh.cn/Article/details/gtcjabupt.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://3g.zdbjq.cn/Article/details/gxwjxujcn.sHtML

[Q29] 最大最小值
来源：http://3g.zdbjq.cn/Article/details/gycvgohui.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.hesvh.cn/Article/details/gljtcgblr.sHtML

[Q30] 分组统计
来源：http://m.share.fehbvm.com/Article/details/gfydhecnx.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.m.share.zdbjq.cn/Article/details/ghuebhsrf.sHtML

[Q31] 分组后过滤
来源：http://mobile.hesvh.cn/Article/details/ggcgfasfy.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wap.hesvh.cn/Article/details/glkpeoawm.sHtML

[Q32] 分组拼接字符串
来源：http://m.share.fehbvm.com/Article/details/gtuhlojvk.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wap.hesvh.cn/Article/details/ggscjvspe.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://blog.fehbvm.com/Article/details/gbgihkonv.sHtML

[Q33] 多列分组
来源：http://m.share.fehbvm.com/Article/details/gatmapgbm.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://blog.fehbvm.com/Article/details/gebrvcpwe.sHtML

[Q34] 每组取第一条
来源：http://www.blog.hesvh.cn/Article/details/gwkjvaauo.sHtML

SELECT * FROM (
来源：http://blog.fehbvm.com/Article/details/ggvgwatsy.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.m.share.zdbjq.cn/Article/details/gugbmuuaw.sHtML

) t WHERE rn = 1;
来源：http://baike.hesvh.cn/Article/details/gejvkswqv.sHtML

[Q35] 内连接
来源：http://baike.fehbvm.com/Article/details/gyxxyipwu.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.zdbjq.cn/Article/details/gnmajsjhn.sHtML

[Q36] 左连接
来源：http://www.blog.hesvh.cn/Article/details/gvtrjkmat.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://read.share.hesvh.cn/Article/details/gemejscls.sHtML

[Q37] 右连接
来源：http://www.blog.hesvh.cn/Article/details/glwqrzoxb.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mobile.fehbvm.com/Article/details/gbznsbzvu.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://mobile.hesvh.cn/Article/details/gkjvbkhrg.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mobile.hesvh.cn/Article/details/gdosvcnwa.sHtML

[Q39] 自连接（查上下级）
来源：http://blog.fehbvm.com/Article/details/gqnuocsrw.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.fehbvm.com/Article/details/ggkheggpw.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://baike.fehbvm.com/Article/details/gjwjbnnjm.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.fehbvm.com/Article/details/gjzxdogzb.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.share.zdbjq.cn/Article/details/gslzgwytb.sHtML

[Q41] 多表连接
来源：http://www.share.hesvh.cn/Article/details/ghcuedpku.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://m.share.hesvh.cn/Article/details/gxbraxamd.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.zdbjq.cn/Article/details/glhzkbily.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.share.zdbjq.cn/Article/details/gomkbzkmu.sHtML

[Q42] 连接条件附加过滤
来源：http://baike.hesvh.cn/Article/details/gusqjlzar.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.share.fehbvm.com/Article/details/gsyjjvyzf.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.fehbvm.com/Article/details/gwgjixnbm.sHtML

[Q43] 标量子查询
来源：http://wap.hesvh.cn/Article/details/glnidpjux.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.zdbjq.cn/Article/details/gnuqwxzxi.sHtML

[Q44] IN 子查询
来源：http://www.m.share.hesvh.cn/Article/details/glqjpbvac.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mobile.zdbjq.cn/Article/details/gfcagvbwo.sHtML

[Q45] EXISTS 判断存在
来源：http://m.share.zdbjq.cn/Article/details/gjpmsrzmf.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.fehbvm.com/Article/details/gywwiiars.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://m.share.zdbjq.cn/Article/details/girrhkjfd.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.fehbvm.com/Article/details/gayohptsw.sHtML

[Q47] 与平均值比较
来源：http://wap.hesvh.cn/Article/details/gsmrglqhh.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.share.zdbjq.cn/Article/details/griqqjpxs.sHtML

[Q48] CTE 公用表表达式
来源：http://baike.fehbvm.com/Article/details/gyvzpcxiz.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://baike.fehbvm.com/Article/details/gjpmkgddp.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://baike.fehbvm.com/Article/details/gzcmbmzys.sHtML

[Q49] 更新单行
来源：http://wap.zdbjq.cn/Article/details/gywexcbrh.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://blog.zdbjq.cn/Article/details/gluftykid.sHtML

[Q50] 批量更新
来源：http://wap.hesvh.cn/Article/details/gefeeqydh.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.fehbvm.com/Article/details/gqniabpcb.sHtML

[Q51] 用子查询更新
来源：http://3g.zdbjq.cn/Article/details/gaaxbdivc.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.share.hesvh.cn/Article/details/gmrluhado.sHtML

[Q52] 删除指定行
来源：http://baike.hesvh.cn/Article/details/gvgksjnff.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.hesvh.cn/Article/details/gfoqodtky.sHtML

[Q53] 按条件删除
来源：http://mobile.fehbvm.com/Article/details/gyetduohc.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.zdbjq.cn/Article/details/ggmipawyn.sHtML

[Q54] 清空表
来源：http://mobile.zdbjq.cn/Article/details/gdtfsvfcb.sHtML

TRUNCATE TABLE logs;
来源：http://blog.fehbvm.com/Article/details/gqxjhgoer.sHtML

[Q55] 排名（并列占位）
来源：http://www.m.share.fehbvm.com/Article/details/gojijjgjw.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.hesvh.cn/Article/details/glbxrppcz.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.fehbvm.com/Article/details/gzcqwbefu.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.zdbjq.cn/Article/details/gaxqgetbg.sHtML

[Q57] 行号
来源：http://www.share.fehbvm.com/Article/details/gbshkfqzu.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gfakptekc.sHtML

[Q58] 累计求和
来源：http://m.share.hesvh.cn/Article/details/grcqwzqra.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/gvczxptme.sHtML

[Q59] 分组内累计
来源：http://www.m.share.hesvh.cn/Article/details/geswtldts.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gthpakbyv.sHtML

[Q60] 取上一行 / 下一行
来源：http://wap.zdbjq.cn/Article/details/gatsffcci.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.m.share.zdbjq.cn/Article/details/gdayzbhcy.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.fehbvm.com/Article/details/gurobryrl.sHtML

[Q61] 移动平均
来源：http://www.blog.zdbjq.cn/Article/details/gcaajiyap.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/gslqaymhn.sHtML

[Q62] 分组占比
来源：http://baike.zdbjq.cn/Article/details/gqnkdvsvo.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://baike.zdbjq.cn/Article/details/gvgmpirio.sHtML

[Q63] 开启事务
来源：http://www.share.hesvh.cn/Article/details/goqzcileq.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.zdbjq.cn/Article/details/gbcgvacer.sHtML

[Q64] 提交事务
来源：http://baike.hesvh.cn/Article/details/gtbqvvmvp.sHtML

COMMIT;
来源：http://www.m.share.fehbvm.com/Article/details/givrywlxj.sHtML

[Q65] 回滚事务
来源：http://wap.fehbvm.com/Article/details/gptlninrc.sHtML

ROLLBACK;
来源：http://www.blog.hesvh.cn/Article/details/gzqlmgpgk.sHtML

[Q66] 行锁查询
来源：http://www.share.zdbjq.cn/Article/details/gakmtuano.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mobile.zdbjq.cn/Article/details/gsxzqmjkx.sHtML

[Q67] 设置隔离级别
来源：http://baike.zdbjq.cn/Article/details/guibxolor.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.zdbjq.cn/Article/details/ggscghxyf.sHtML

[Q68] 保存点
来源：http://www.blog.zdbjq.cn/Article/details/gsswrkurf.sHtML

SAVEPOINT sp1;
来源：http://www.blog.zdbjq.cn/Article/details/gvqdjhxfz.sHtML


<!-- 参考信息 -->