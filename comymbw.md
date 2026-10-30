代发 wailian999

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.m.share.hesvh.cn/Article/details/gjlgkeges.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://m.share.zdbjq.cn/Article/details/ghvcimtsp.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.zdbjq.cn/Article/details/gpytnqyxk.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.hesvh.cn/Article/details/gzeqtoulm.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.fehbvm.com/Article/details/gpgibhzea.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://baike.fehbvm.com/Article/details/gndztgetm.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.hesvh.cn/Article/details/gstyptkrc.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.zdbjq.cn/Article/details/gxokjaldo.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gqtlpvlpg.sHtML

O. 并发与异步
来源：http://mobile.zdbjq.cn/Article/details/gpdysqjng.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/geddasfgv.sHtML

[O01] 启动一个线程
来源：http://mobile.hesvh.cn/Article/details/glgqvpsqs.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://baike.hesvh.cn/Article/details/gcmmfvzcr.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.fehbvm.com/Article/details/gdjfuitjb.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.blog.fehbvm.com/Article/details/gqzysepjc.sHtML

TS:   // 同 JS
来源：http://m.share.zdbjq.cn/Article/details/gmvnbjzva.sHtML

Java: new Thread(() -> f()).start()
来源：http://wap.fehbvm.com/Article/details/gathauyvv.sHtML

Go:   go f()
来源：http://read.share.hesvh.cn/Article/details/gcqwzfwse.sHtML

Ruby: Thread.new { f }
来源：http://www.share.hesvh.cn/Article/details/gcobfzcac.sHtML

C#:   Task.Run(() => F());
来源：http://read.share.fehbvm.com/Article/details/gnbixhgev.sHtML

[O02] 使用线程池
来源：http://blog.hesvh.cn/Article/details/geflzyfke.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://m.share.hesvh.cn/Article/details/giyahjbiv.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mobile.hesvh.cn/Article/details/gsozjwqhd.sHtML

JS:   // worker_threads 线程池
来源：http://blog.fehbvm.com/Article/details/grhxwvliw.sHtML

TS:   // worker_threads 线程池
来源：http://m.share.zdbjq.cn/Article/details/guqklttnp.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://baike.zdbjq.cn/Article/details/gnqbochha.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.share.hesvh.cn/Article/details/gxksxznee.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://read.share.zdbjq.cn/Article/details/gkrxugsxs.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.zdbjq.cn/Article/details/gczqpvvdt.sHtML

[O03] 加锁保护共享数据
来源：http://www.share.zdbjq.cn/Article/details/gjgcucyen.sHtML

Py:   with lock: shared += 1
来源：http://wap.fehbvm.com/Article/details/gtlrxnmfh.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://wap.zdbjq.cn/Article/details/gwcsnwfmi.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wap.fehbvm.com/Article/details/gtzuckivo.sHtML

TS:   // 同 JS
来源：http://m.share.hesvh.cn/Article/details/gvzcshrqb.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.hesvh.cn/Article/details/gqefegnlc.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://3g.zdbjq.cn/Article/details/gvaxpfkig.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://m.share.hesvh.cn/Article/details/gambdakil.sHtML

C#:   lock (gate) { shared++; }
来源：http://blog.zdbjq.cn/Article/details/gkczxdeog.sHtML

[O04] 定义异步函数并等待
来源：http://m.share.zdbjq.cn/Article/details/ghzrrivfo.sHtML

Py:   async def f():⏎    await g()
来源：http://baike.fehbvm.com/Article/details/gckedmikq.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.fehbvm.com/Article/details/gqcqhqnmz.sHtML

JS:   async function f() { await g(); }
来源：http://baike.fehbvm.com/Article/details/gnjulgvxt.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://3g.fehbvm.com/Article/details/gmkkhcqka.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mobile.zdbjq.cn/Article/details/gyavjrhdd.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://blog.fehbvm.com/Article/details/grjqrbpyt.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://mobile.fehbvm.com/Article/details/gdjjgdnnb.sHtML

C#:   async Task F() { await G(); }
来源：http://m.share.zdbjq.cn/Article/details/gnwafeslr.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.share.hesvh.cn/Article/details/gsnwtdohz.sHtML

Py:   asyncio.gather(*tasks)
来源：http://wap.fehbvm.com/Article/details/gbehdynwp.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://blog.zdbjq.cn/Article/details/gxgehyzer.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.hesvh.cn/Article/details/ghkpugswp.sHtML

TS:   await Promise.all(tasks)
来源：http://baike.zdbjq.cn/Article/details/gsbbxzybn.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://3g.zdbjq.cn/Article/details/gazjrxgto.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mobile.fehbvm.com/Article/details/gdysraxsu.sHtML

Ruby: threads.map(&:join)
来源：http://m.share.zdbjq.cn/Article/details/gdyfnyyhp.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://blog.zdbjq.cn/Article/details/gagodqned.sHtML

[O06] 使用进程池
来源：http://blog.hesvh.cn/Article/details/gqkirgarh.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mobile.zdbjq.cn/Article/details/gzlcdrsmd.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://blog.fehbvm.com/Article/details/gpnoubcxa.sHtML

JS:   // child_process / cluster 模块
来源：http://3g.fehbvm.com/Article/details/ghxhcdxoc.sHtML

TS:   // child_process / cluster 模块
来源：http://m.share.zdbjq.cn/Article/details/gbxrcxdit.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.blog.zdbjq.cn/Article/details/guvbasqyo.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://3g.zdbjq.cn/Article/details/geohwamne.sHtML

Ruby: // fork 块
来源：http://baike.hesvh.cn/Article/details/gkmczvskw.sHtML

C#:   Parallel.For
来源：http://www.m.share.fehbvm.com/Article/details/gqgwysuln.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gwrmhkurp.sHtML

P. 常用工具函数
来源：http://read.share.fehbvm.com/Article/details/gyqaiplqq.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gmqixdvrb.sHtML

[P01] 生成 UUID
来源：http://wap.fehbvm.com/Article/details/gluamzxay.sHtML

Py:   str(uuid.uuid4())
来源：http://mobile.hesvh.cn/Article/details/gsuwkaugk.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://read.share.zdbjq.cn/Article/details/gedbdanlz.sHtML

JS:   crypto.randomUUID()
来源：http://www.blog.fehbvm.com/Article/details/geuhsccai.sHtML

TS:   crypto.randomUUID()
来源：http://mobile.hesvh.cn/Article/details/ghvvypapt.sHtML

Java: UUID.randomUUID().toString()
来源：http://m.share.fehbvm.com/Article/details/gcgwuueqz.sHtML

Go:   // 用 github.com/google/uuid
来源：http://baike.hesvh.cn/Article/details/gwugezzwm.sHtML

Ruby: SecureRandom.uuid
来源：http://3g.zdbjq.cn/Article/details/gankgoowi.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://read.share.zdbjq.cn/Article/details/gfusgwqzc.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.blog.hesvh.cn/Article/details/gfdzvmhnp.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://baike.hesvh.cn/Article/details/gjtmdioug.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.blog.zdbjq.cn/Article/details/gpqshayna.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wap.hesvh.cn/Article/details/gsyuycptk.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wap.fehbvm.com/Article/details/gghnuuepe.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wap.hesvh.cn/Article/details/gbpfofisl.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://m.share.hesvh.cn/Article/details/gngolocmi.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.blog.hesvh.cn/Article/details/gkvcdgfpp.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.blog.zdbjq.cn/Article/details/gfyiofvfg.sHtML

[P03] 生成短随机字符串
来源：http://www.m.share.fehbvm.com/Article/details/gucmqsaqf.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.blog.zdbjq.cn/Article/details/gusuuprey.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://m.share.zdbjq.cn/Article/details/gptuqmdhr.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.zdbjq.cn/Article/details/gbqrgsfev.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.hesvh.cn/Article/details/gvrratuaj.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://3g.fehbvm.com/Article/details/gevqizzkz.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.m.share.zdbjq.cn/Article/details/gvwvtbjgu.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.share.zdbjq.cn/Article/details/ghxhmankk.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.share.fehbvm.com/Article/details/gahztujmu.sHtML

[P04] 求长度
来源：http://www.m.share.hesvh.cn/Article/details/gnzfqydqb.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://read.share.zdbjq.cn/Article/details/grfmsgkgl.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.zdbjq.cn/Article/details/grruquiyz.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.zdbjq.cn/Article/details/gftwjojsb.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.fehbvm.com/Article/details/gfitbayjt.sHtML

Java: list.size();  map.size();  s.length()
来源：http://m.share.fehbvm.com/Article/details/gkbvucsfv.sHtML

Go:   len(arr);  len(m)
来源：http://mobile.fehbvm.com/Article/details/gjjfxhizw.sHtML

Ruby: x.length;  x.size
来源：http://3g.zdbjq.cn/Article/details/gbvpmhmzp.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://read.share.hesvh.cn/Article/details/ggcgpgufh.sHtML

[P05] 判断两个对象内容是否相等
来源：http://3g.zdbjq.cn/Article/details/gtraxnjlg.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://wap.fehbvm.com/Article/details/gnfinirqe.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://baike.hesvh.cn/Article/details/gbauoynzz.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://m.share.fehbvm.com/Article/details/gerxfupsn.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.hesvh.cn/Article/details/gslfqhprh.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wap.hesvh.cn/Article/details/gbqawarod.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.zdbjq.cn/Article/details/gdflpjsyh.sHtML

Ruby: a == b
来源：http://wap.hesvh.cn/Article/details/ggnhmndqz.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://m.share.hesvh.cn/Article/details/grdxvwhpc.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://3g.fehbvm.com/Article/details/glkzuzpdb.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://blog.fehbvm.com/Article/details/gndmpzwly.sHtML

PHP:  if (empty($x)) {}
来源：http://read.share.zdbjq.cn/Article/details/gnaogqrmv.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://m.share.zdbjq.cn/Article/details/gwfjomjpy.sHtML

TS:   if (x == null) {}
来源：http://www.share.zdbjq.cn/Article/details/giyvxklez.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://baike.zdbjq.cn/Article/details/gvwfquyww.sHtML

Go:   if x == nil {}
来源：http://www.m.share.fehbvm.com/Article/details/gontpzgge.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://baike.hesvh.cn/Article/details/glqcdyhmv.sHtML

C#:   if (x is null) {}
来源：http://blog.hesvh.cn/Article/details/gfxrldasz.sHtML

[P07] 防抖与节流
来源：http://3g.fehbvm.com/Article/details/gbtavljit.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mobile.hesvh.cn/Article/details/gmtsfmpyn.sHtML

PHP:  // 手写时间戳比较
来源：http://m.share.hesvh.cn/Article/details/gjmlzbumq.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.zdbjq.cn/Article/details/gznhnjade.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.zdbjq.cn/Article/details/ggybpctqi.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wap.fehbvm.com/Article/details/gmmdqjqkl.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://3g.fehbvm.com/Article/details/gboniljez.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://m.share.hesvh.cn/Article/details/grvynvezz.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://baike.zdbjq.cn/Article/details/gdqfxlnjb.sHtML

[P08] 处理浮点精度问题
来源：http://wap.hesvh.cn/Article/details/gvffegqyk.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://read.share.fehbvm.com/Article/details/gegidfvgr.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://read.share.fehbvm.com/Article/details/glgfgkbgf.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://m.share.fehbvm.com/Article/details/ghabecrfl.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://baike.hesvh.cn/Article/details/gqfalhbrj.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wap.zdbjq.cn/Article/details/gsunpttny.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.share.zdbjq.cn/Article/details/gmruzghmg.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://3g.hesvh.cn/Article/details/guvjovvrc.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.blog.fehbvm.com/Article/details/gjzsqyyee.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gwkgebanr.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://blog.zdbjq.cn/Article/details/ggavsjezp.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gibrncybr.sHtML

[Q01] 创建表
来源：http://blog.zdbjq.cn/Article/details/grdaqzyci.sHtML

CREATE TABLE users (
来源：http://mobile.hesvh.cn/Article/details/gvlhbdetj.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.hesvh.cn/Article/details/gnlzomwsu.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.blog.zdbjq.cn/Article/details/gcnhjejec.sHtML

email VARCHAR(100) UNIQUE,
来源：http://mobile.fehbvm.com/Article/details/gdctosspp.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mobile.fehbvm.com/Article/details/gjarkfnft.sHtML

);
来源：http://read.share.zdbjq.cn/Article/details/gwjophrbm.sHtML

[Q02] 创建带外键的表
来源：http://baike.fehbvm.com/Article/details/gdsyxeyek.sHtML

CREATE TABLE orders (
来源：http://wap.fehbvm.com/Article/details/gisqsjkdm.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.zdbjq.cn/Article/details/gjlsdkdrv.sHtML

user_id INT NOT NULL,
来源：http://blog.zdbjq.cn/Article/details/gxgvvbzvq.sHtML

amount DECIMAL(10, 2),
来源：http://read.share.zdbjq.cn/Article/details/ggdotkvbj.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://baike.hesvh.cn/Article/details/glumvsewj.sHtML

);
来源：http://blog.hesvh.cn/Article/details/gvchhknoe.sHtML

[Q03] 增加列
来源：http://m.share.fehbvm.com/Article/details/gkwhkqjqk.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://read.share.hesvh.cn/Article/details/glbkblufz.sHtML

[Q04] 修改列类型
来源：http://blog.hesvh.cn/Article/details/gjixfdfvi.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.blog.fehbvm.com/Article/details/gggnpuutf.sHtML

[Q05] 重命名列
来源：http://m.share.fehbvm.com/Article/details/gmomaprum.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mobile.fehbvm.com/Article/details/ggdsxmflr.sHtML

[Q06] 删除列
来源：http://wap.hesvh.cn/Article/details/glytwgxaf.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://blog.fehbvm.com/Article/details/gmyusahpj.sHtML

[Q07] 删除表
来源：http://wap.zdbjq.cn/Article/details/gyjmtskry.sHtML

DROP TABLE IF EXISTS orders;
来源：http://mobile.zdbjq.cn/Article/details/gtkrulvxu.sHtML

[Q08] 创建普通索引
来源：http://mobile.hesvh.cn/Article/details/gykrardjk.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://blog.hesvh.cn/Article/details/gaajbhgsz.sHtML

[Q09] 创建唯一索引
来源：http://blog.fehbvm.com/Article/details/gjkanisfa.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mobile.hesvh.cn/Article/details/grnzdjlbd.sHtML

[Q10] 插入单行
来源：http://read.share.hesvh.cn/Article/details/gscdmbzkl.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.share.zdbjq.cn/Article/details/gorafylpa.sHtML

[Q11] 一次插入多行
来源：http://blog.zdbjq.cn/Article/details/gvxcrrfrj.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mobile.fehbvm.com/Article/details/gbkpqevxb.sHtML

[Q12] 插入后取自增 ID
来源：http://www.blog.fehbvm.com/Article/details/gydtxgihw.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://m.share.hesvh.cn/Article/details/gqejvlnyp.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.share.fehbvm.com/Article/details/gsxcuuieb.sHtML

[Q13] 忽略重复插入
来源：http://blog.fehbvm.com/Article/details/gdmbkioao.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mobile.fehbvm.com/Article/details/ghshpvrbh.sHtML

[Q14] 存在则更新（upsert）
来源：http://blog.fehbvm.com/Article/details/gwwikntfd.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://3g.hesvh.cn/Article/details/gsdypzokl.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://m.share.zdbjq.cn/Article/details/gcxusatgc.sHtML

[Q15] 查询全部
来源：http://www.m.share.fehbvm.com/Article/details/gpibybxbc.sHtML

SELECT * FROM users;
来源：http://www.share.hesvh.cn/Article/details/gupoatvoz.sHtML

[Q16] 查询指定列
来源：http://mobile.hesvh.cn/Article/details/gkbfbrgvh.sHtML

SELECT id, name FROM users;
来源：http://read.share.hesvh.cn/Article/details/grnxiakjd.sHtML

[Q17] 条件查询
来源：http://read.share.hesvh.cn/Article/details/gaxgofofx.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.blog.zdbjq.cn/Article/details/gynibdapl.sHtML

[Q18] 模糊匹配
来源：http://read.share.fehbvm.com/Article/details/gcwyocdag.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.share.fehbvm.com/Article/details/gzhzzrrtc.sHtML

[Q19] 范围查询
来源：http://mobile.hesvh.cn/Article/details/gunnmyury.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://m.share.hesvh.cn/Article/details/gquagixxv.sHtML

[Q20] IN 列表
来源：http://www.m.share.zdbjq.cn/Article/details/gtwupucmd.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.hesvh.cn/Article/details/gyweqkleh.sHtML

[Q21] 空值判断
来源：http://blog.fehbvm.com/Article/details/glvliyeef.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://mobile.hesvh.cn/Article/details/gpppmlqxv.sHtML

[Q22] 排序
来源：http://wap.hesvh.cn/Article/details/ghntoweso.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://read.share.hesvh.cn/Article/details/gackuhcwo.sHtML

[Q23] 分页
来源：http://www.m.share.fehbvm.com/Article/details/gxghrnzjp.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.share.hesvh.cn/Article/details/gfitbrmmj.sHtML

[Q24] 去重
来源：http://baike.zdbjq.cn/Article/details/gvphtrsjs.sHtML

SELECT DISTINCT city FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gymodpstc.sHtML

[Q25] 只取前 N 条
来源：http://wap.hesvh.cn/Article/details/gsxoenmxb.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mobile.zdbjq.cn/Article/details/gbbtsuqpz.sHtML

[Q26] 计数
来源：http://3g.zdbjq.cn/Article/details/gvfhtoqth.sHtML

SELECT COUNT(*) FROM users;
来源：http://wap.hesvh.cn/Article/details/gftzjjhjv.sHtML

[Q27] 条件计数
来源：http://3g.zdbjq.cn/Article/details/gzvkpmiyj.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://m.share.hesvh.cn/Article/details/garcfieja.sHtML

[Q28] 求和与平均
来源：http://www.m.share.zdbjq.cn/Article/details/grwvqhaod.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://m.share.fehbvm.com/Article/details/gogqtmlaa.sHtML

[Q29] 最大最小值
来源：http://baike.hesvh.cn/Article/details/gloquwtir.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://baike.fehbvm.com/Article/details/gnigzrnsd.sHtML

[Q30] 分组统计
来源：http://www.m.share.hesvh.cn/Article/details/gbluyrxrb.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://blog.fehbvm.com/Article/details/gsmpbsjkg.sHtML

[Q31] 分组后过滤
来源：http://baike.hesvh.cn/Article/details/gjwkiglwe.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.zdbjq.cn/Article/details/gyoduolmg.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.zdbjq.cn/Article/details/gxidugqdl.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://3g.fehbvm.com/Article/details/gmifdnfxc.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://3g.hesvh.cn/Article/details/gthdwbscf.sHtML

[Q33] 多列分组
来源：http://read.share.fehbvm.com/Article/details/gdpkmxezb.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.share.fehbvm.com/Article/details/gdkwefacq.sHtML

[Q34] 每组取第一条
来源：http://wap.zdbjq.cn/Article/details/geszsivik.sHtML

SELECT * FROM (
来源：http://blog.zdbjq.cn/Article/details/gvijtqbkv.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.zdbjq.cn/Article/details/gmlqgsjjn.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gzoryjaao.sHtML

[Q35] 内连接
来源：http://www.blog.fehbvm.com/Article/details/gorbqhvyg.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://3g.hesvh.cn/Article/details/gqynozxlx.sHtML

[Q36] 左连接
来源：http://baike.fehbvm.com/Article/details/gfwuhvizh.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://baike.zdbjq.cn/Article/details/gthwcound.sHtML

[Q37] 右连接
来源：http://mobile.fehbvm.com/Article/details/gqlehinvr.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.zdbjq.cn/Article/details/gknmgpyjz.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://mobile.hesvh.cn/Article/details/gqmkfyjwt.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.hesvh.cn/Article/details/gojexxzwh.sHtML

[Q39] 自连接（查上下级）
来源：http://blog.zdbjq.cn/Article/details/gkvdupclz.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://baike.zdbjq.cn/Article/details/gobmbernd.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://blog.zdbjq.cn/Article/details/gqoafsmfk.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.fehbvm.com/Article/details/grynzienh.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mobile.fehbvm.com/Article/details/gbtmdnxzj.sHtML

[Q41] 多表连接
来源：http://wap.fehbvm.com/Article/details/givqnkaxj.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://3g.hesvh.cn/Article/details/gmwzdgyou.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.hesvh.cn/Article/details/gbbwmuaom.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.zdbjq.cn/Article/details/gjlqhcoic.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.hesvh.cn/Article/details/gxgknmwxs.sHtML

SELECT u.name, o.amount FROM users u
来源：http://wap.fehbvm.com/Article/details/gabeepuqh.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.m.share.hesvh.cn/Article/details/gkytgdptt.sHtML

[Q43] 标量子查询
来源：http://baike.hesvh.cn/Article/details/gvczylbbw.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.m.share.fehbvm.com/Article/details/gsbtbfeqd.sHtML

[Q44] IN 子查询
来源：http://www.m.share.hesvh.cn/Article/details/ghxaxvnqm.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://baike.zdbjq.cn/Article/details/ggnmethwq.sHtML

[Q45] EXISTS 判断存在
来源：http://www.blog.fehbvm.com/Article/details/gdyikiwwy.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.fehbvm.com/Article/details/gevtqgssv.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.fehbvm.com/Article/details/gyurpeqlm.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.fehbvm.com/Article/details/gelzwftyo.sHtML

[Q47] 与平均值比较
来源：http://3g.fehbvm.com/Article/details/grvupcxsk.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.hesvh.cn/Article/details/gwnnkqcsz.sHtML

[Q48] CTE 公用表表达式
来源：http://read.share.zdbjq.cn/Article/details/gnorhvsdk.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://read.share.zdbjq.cn/Article/details/gtsufmnpl.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.blog.zdbjq.cn/Article/details/ghvjoroef.sHtML

[Q49] 更新单行
来源：http://read.share.fehbvm.com/Article/details/gyjyublbu.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.fehbvm.com/Article/details/gxihohzrx.sHtML

[Q50] 批量更新
来源：http://baike.hesvh.cn/Article/details/gkbdjvhzc.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.share.hesvh.cn/Article/details/gqyqnovhd.sHtML

[Q51] 用子查询更新
来源：http://baike.fehbvm.com/Article/details/gjavgkmwt.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.fehbvm.com/Article/details/gzwdjgcul.sHtML

[Q52] 删除指定行
来源：http://mobile.hesvh.cn/Article/details/gbvcmhgfq.sHtML

DELETE FROM users WHERE id = 10;
来源：http://baike.zdbjq.cn/Article/details/gkkynzaym.sHtML

[Q53] 按条件删除
来源：http://www.blog.hesvh.cn/Article/details/gkubyhqhq.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://3g.fehbvm.com/Article/details/gjqcltsei.sHtML

[Q54] 清空表
来源：http://www.blog.zdbjq.cn/Article/details/gicnilhgm.sHtML

TRUNCATE TABLE logs;
来源：http://blog.zdbjq.cn/Article/details/gsbzkbnqp.sHtML

[Q55] 排名（并列占位）
来源：http://mobile.fehbvm.com/Article/details/gnzlpqsud.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.share.zdbjq.cn/Article/details/gncdcujqr.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.blog.fehbvm.com/Article/details/gsktkdorc.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.fehbvm.com/Article/details/gljmjdhkj.sHtML

[Q57] 行号
来源：http://m.share.fehbvm.com/Article/details/gvqocpkny.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gjrkuntpd.sHtML

[Q58] 累计求和
来源：http://blog.hesvh.cn/Article/details/glfbgygdo.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.fehbvm.com/Article/details/gjmhsqayh.sHtML

[Q59] 分组内累计
来源：http://www.m.share.zdbjq.cn/Article/details/gjrgcetek.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.zdbjq.cn/Article/details/glbzerqiv.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.zdbjq.cn/Article/details/getikhyzz.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.hesvh.cn/Article/details/grkmvyojw.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/gozvmfixy.sHtML

[Q61] 移动平均
来源：http://wap.hesvh.cn/Article/details/gsmgfeqwz.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gdonlzget.sHtML

[Q62] 分组占比
来源：http://m.share.hesvh.cn/Article/details/gtxsqjfgq.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://baike.hesvh.cn/Article/details/gaplxvlhc.sHtML

[Q63] 开启事务
来源：http://3g.fehbvm.com/Article/details/gaoerjjoy.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://mobile.zdbjq.cn/Article/details/gelbcywuh.sHtML

[Q64] 提交事务
来源：http://m.share.fehbvm.com/Article/details/gwgmnnrkr.sHtML

COMMIT;
来源：http://m.share.zdbjq.cn/Article/details/gllhguvvd.sHtML

[Q65] 回滚事务
来源：http://www.blog.zdbjq.cn/Article/details/gsczwanhi.sHtML

ROLLBACK;
来源：http://www.share.fehbvm.com/Article/details/gqrakjdcg.sHtML

[Q66] 行锁查询
来源：http://blog.zdbjq.cn/Article/details/gadwzybdw.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://blog.fehbvm.com/Article/details/gaodxztnj.sHtML

[Q67] 设置隔离级别
来源：http://blog.zdbjq.cn/Article/details/glzgtgvoq.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.hesvh.cn/Article/details/gnfyytqmo.sHtML

[Q68] 保存点
来源：http://www.blog.hesvh.cn/Article/details/grkaszgaz.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.fehbvm.com/Article/details/gnezlbcqh.sHtML


<!-- 参考信息 -->