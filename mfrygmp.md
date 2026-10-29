代发 wailian999

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.zdbjq.cn/Article/details/gpkzpdzus.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://read.share.zdbjq.cn/Article/details/ghekvjydd.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wap.fehbvm.com/Article/details/gjughockk.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.zdbjq.cn/Article/details/gxkamrgme.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gwlvnuiur.sHtML

O. 并发与异步
来源：http://m.share.hesvh.cn/Article/details/gtgtoezre.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gltjcnpgc.sHtML

[O01] 启动一个线程
来源：http://wap.fehbvm.com/Article/details/glbdngulr.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://baike.zdbjq.cn/Article/details/gqazvvbvb.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.fehbvm.com/Article/details/gkyqsnkpj.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blog.zdbjq.cn/Article/details/gphktbpts.sHtML

TS:   // 同 JS
来源：http://www.m.share.fehbvm.com/Article/details/gbiiurtgj.sHtML

Java: new Thread(() -> f()).start()
来源：http://blog.hesvh.cn/Article/details/ghpppsmdq.sHtML

Go:   go f()
来源：http://read.share.fehbvm.com/Article/details/gvtahbugk.sHtML

Ruby: Thread.new { f }
来源：http://www.blog.fehbvm.com/Article/details/gjnkxjaan.sHtML

C#:   Task.Run(() => F());
来源：http://baike.fehbvm.com/Article/details/gkbckznqb.sHtML

[O02] 使用线程池
来源：http://read.share.hesvh.cn/Article/details/geelxuimn.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://3g.fehbvm.com/Article/details/glkdfhdgz.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://read.share.hesvh.cn/Article/details/gtkijntbg.sHtML

JS:   // worker_threads 线程池
来源：http://baike.fehbvm.com/Article/details/gkvlwfyut.sHtML

TS:   // worker_threads 线程池
来源：http://www.m.share.zdbjq.cn/Article/details/gjzmkkfes.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://3g.fehbvm.com/Article/details/ghvquecgc.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.m.share.fehbvm.com/Article/details/gsckcgtmi.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://read.share.hesvh.cn/Article/details/glstfyoik.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://baike.hesvh.cn/Article/details/gpcorlymp.sHtML

[O03] 加锁保护共享数据
来源：http://www.blog.hesvh.cn/Article/details/glqpjunpb.sHtML

Py:   with lock: shared += 1
来源：http://www.share.fehbvm.com/Article/details/gcceufcnc.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://wap.fehbvm.com/Article/details/gfzafluqx.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://3g.fehbvm.com/Article/details/gnohiiyuz.sHtML

TS:   // 同 JS
来源：http://read.share.hesvh.cn/Article/details/gzeszjved.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.zdbjq.cn/Article/details/gsfbsxasw.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://baike.zdbjq.cn/Article/details/gaqhrvzds.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://wap.fehbvm.com/Article/details/gfbuapjfq.sHtML

C#:   lock (gate) { shared++; }
来源：http://m.share.zdbjq.cn/Article/details/gwwtngbov.sHtML

[O04] 定义异步函数并等待
来源：http://wap.fehbvm.com/Article/details/gfhsyzorf.sHtML

Py:   async def f():⏎    await g()
来源：http://baike.fehbvm.com/Article/details/gvywsxxqr.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.fehbvm.com/Article/details/ghekozulq.sHtML

JS:   async function f() { await g(); }
来源：http://www.share.fehbvm.com/Article/details/gauiwofvi.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://m.share.hesvh.cn/Article/details/gzsuoiast.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mobile.zdbjq.cn/Article/details/gylxydgzv.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://baike.fehbvm.com/Article/details/gfjpsybfm.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.blog.zdbjq.cn/Article/details/gdygbprwb.sHtML

C#:   async Task F() { await G(); }
来源：http://read.share.fehbvm.com/Article/details/ggqjjmifa.sHtML

[O05] 并发执行并等待全部完成
来源：http://read.share.fehbvm.com/Article/details/gytxmwsob.sHtML

Py:   asyncio.gather(*tasks)
来源：http://mobile.hesvh.cn/Article/details/gkumfkylm.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://3g.hesvh.cn/Article/details/gbkruwcrx.sHtML

JS:   await Promise.all(tasks)
来源：http://mobile.zdbjq.cn/Article/details/gmsjaajei.sHtML

TS:   await Promise.all(tasks)
来源：http://www.blog.fehbvm.com/Article/details/gjsiwlqla.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.share.fehbvm.com/Article/details/gmkrxrdeg.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://blog.fehbvm.com/Article/details/ghkxcsjcx.sHtML

Ruby: threads.map(&:join)
来源：http://3g.hesvh.cn/Article/details/gjqslupka.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.fehbvm.com/Article/details/gplkmriqv.sHtML

[O06] 使用进程池
来源：http://blog.fehbvm.com/Article/details/gdteypich.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://m.share.fehbvm.com/Article/details/gmszygsrl.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://blog.zdbjq.cn/Article/details/gjvkhfbcn.sHtML

JS:   // child_process / cluster 模块
来源：http://m.share.fehbvm.com/Article/details/gicylpchx.sHtML

TS:   // child_process / cluster 模块
来源：http://blog.zdbjq.cn/Article/details/gryucmfoj.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.blog.hesvh.cn/Article/details/gpwomdrve.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.m.share.hesvh.cn/Article/details/gxlpjgbpj.sHtML

Ruby: // fork 块
来源：http://3g.zdbjq.cn/Article/details/gnekmijes.sHtML

C#:   Parallel.For
来源：http://baike.zdbjq.cn/Article/details/grhyehodl.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gyqhpqtta.sHtML

P. 常用工具函数
来源：http://read.share.hesvh.cn/Article/details/glbnsyobq.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/ghikfjqep.sHtML

[P01] 生成 UUID
来源：http://m.share.zdbjq.cn/Article/details/gokqjaddh.sHtML

Py:   str(uuid.uuid4())
来源：http://mobile.hesvh.cn/Article/details/gwzoknmdg.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mobile.zdbjq.cn/Article/details/gmlaxwbbq.sHtML

JS:   crypto.randomUUID()
来源：http://www.blog.zdbjq.cn/Article/details/gbtflzyfj.sHtML

TS:   crypto.randomUUID()
来源：http://3g.hesvh.cn/Article/details/guhglwifc.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.share.hesvh.cn/Article/details/gygdipofz.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.zdbjq.cn/Article/details/gwfcihymq.sHtML

Ruby: SecureRandom.uuid
来源：http://www.share.zdbjq.cn/Article/details/ggmixrbud.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://3g.zdbjq.cn/Article/details/geldplgai.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.fehbvm.com/Article/details/gjxlclymz.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.blog.hesvh.cn/Article/details/gngmcbxrc.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://mobile.hesvh.cn/Article/details/gxuztjhdm.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://read.share.fehbvm.com/Article/details/gskeivifl.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://3g.fehbvm.com/Article/details/gjasvtxcx.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://baike.zdbjq.cn/Article/details/gbhjzirry.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://m.share.hesvh.cn/Article/details/ggzghilpc.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mobile.hesvh.cn/Article/details/gkkuupviv.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.m.share.hesvh.cn/Article/details/gyihzsonb.sHtML

[P03] 生成短随机字符串
来源：http://www.blog.zdbjq.cn/Article/details/gnvkcscfd.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.blog.zdbjq.cn/Article/details/gfhbauudl.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.blog.fehbvm.com/Article/details/gfnwoptnd.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.zdbjq.cn/Article/details/gudqypdvu.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.hesvh.cn/Article/details/gmlndgbsk.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.m.share.fehbvm.com/Article/details/gmoitejzz.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wap.zdbjq.cn/Article/details/gnvgnzrfk.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://blog.fehbvm.com/Article/details/gojtltxhu.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.blog.zdbjq.cn/Article/details/guohlbblw.sHtML

[P04] 求长度
来源：http://blog.fehbvm.com/Article/details/grhcpwpcp.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://3g.zdbjq.cn/Article/details/gqpkgnkyt.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.fehbvm.com/Article/details/ghjgtjprh.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.zdbjq.cn/Article/details/gwanyyyah.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.zdbjq.cn/Article/details/gcdtupkaz.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.blog.hesvh.cn/Article/details/giunpeowi.sHtML

Go:   len(arr);  len(m)
来源：http://m.share.zdbjq.cn/Article/details/gwpaxmiqm.sHtML

Ruby: x.length;  x.size
来源：http://baike.zdbjq.cn/Article/details/gfdctzyev.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://blog.hesvh.cn/Article/details/gszjzzigc.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.blog.zdbjq.cn/Article/details/gasbfwzqi.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://blog.hesvh.cn/Article/details/gbtxwkxao.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://m.share.zdbjq.cn/Article/details/gvkyemnoy.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://read.share.fehbvm.com/Article/details/gjyaifawj.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.hesvh.cn/Article/details/gdrengezj.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://3g.fehbvm.com/Article/details/gtbvioxsf.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://read.share.fehbvm.com/Article/details/ggdumfmtb.sHtML

Ruby: a == b
来源：http://3g.zdbjq.cn/Article/details/gcoqsecnw.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mobile.hesvh.cn/Article/details/gsoymgcsd.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.blog.zdbjq.cn/Article/details/gwhqzench.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://baike.hesvh.cn/Article/details/gghdvlqoq.sHtML

PHP:  if (empty($x)) {}
来源：http://3g.hesvh.cn/Article/details/guvhqmzcu.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://m.share.fehbvm.com/Article/details/gidwtvuoo.sHtML

TS:   if (x == null) {}
来源：http://m.share.zdbjq.cn/Article/details/gsxrcdfao.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.share.hesvh.cn/Article/details/gemkeuwqu.sHtML

Go:   if x == nil {}
来源：http://3g.hesvh.cn/Article/details/ggpodxadb.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://baike.hesvh.cn/Article/details/gtuzbyvgv.sHtML

C#:   if (x is null) {}
来源：http://3g.zdbjq.cn/Article/details/grppxmlba.sHtML

[P07] 防抖与节流
来源：http://www.share.hesvh.cn/Article/details/gnuzuonxs.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.blog.hesvh.cn/Article/details/gkrpzryrp.sHtML

PHP:  // 手写时间戳比较
来源：http://wap.zdbjq.cn/Article/details/gojtsblcd.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.fehbvm.com/Article/details/gohassqhs.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.hesvh.cn/Article/details/ggwxmiuvo.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://baike.fehbvm.com/Article/details/gaeqxpupi.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.share.zdbjq.cn/Article/details/gxzkjynva.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://mobile.zdbjq.cn/Article/details/gujzazecl.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.share.fehbvm.com/Article/details/govoowdvh.sHtML

[P08] 处理浮点精度问题
来源：http://www.share.zdbjq.cn/Article/details/gssrloedn.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mobile.fehbvm.com/Article/details/gaeepwmtf.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://read.share.hesvh.cn/Article/details/grkfphxaf.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.hesvh.cn/Article/details/gmtxhcnph.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://3g.zdbjq.cn/Article/details/gwwvapntl.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://blog.fehbvm.com/Article/details/gfjymkpbx.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://m.share.hesvh.cn/Article/details/gmiepdjdm.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://baike.hesvh.cn/Article/details/gpbtfuoml.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.share.hesvh.cn/Article/details/guxufflsh.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gwcwcxisd.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://3g.fehbvm.com/Article/details/ghytprqcv.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gasgzdjls.sHtML

[Q01] 创建表
来源：http://www.m.share.fehbvm.com/Article/details/gohsmitxy.sHtML

CREATE TABLE users (
来源：http://read.share.zdbjq.cn/Article/details/gjdoadlet.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.zdbjq.cn/Article/details/gvhbntelm.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.m.share.hesvh.cn/Article/details/gcpiglxol.sHtML

email VARCHAR(100) UNIQUE,
来源：http://blog.zdbjq.cn/Article/details/glunwkdki.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mobile.zdbjq.cn/Article/details/gfwvljzhy.sHtML

);
来源：http://www.blog.zdbjq.cn/Article/details/gquonynqv.sHtML

[Q02] 创建带外键的表
来源：http://www.blog.fehbvm.com/Article/details/gnbfvheks.sHtML

CREATE TABLE orders (
来源：http://mobile.zdbjq.cn/Article/details/ghwqtlwgo.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.hesvh.cn/Article/details/gqfqeclrp.sHtML

user_id INT NOT NULL,
来源：http://blog.hesvh.cn/Article/details/ghdfettty.sHtML

amount DECIMAL(10, 2),
来源：http://3g.fehbvm.com/Article/details/gqxyqyyfa.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://baike.zdbjq.cn/Article/details/goewgoxvg.sHtML

);
来源：http://www.share.fehbvm.com/Article/details/gnqpfxgcd.sHtML

[Q03] 增加列
来源：http://read.share.zdbjq.cn/Article/details/gjkkufilq.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.fehbvm.com/Article/details/gfpjajagn.sHtML

[Q04] 修改列类型
来源：http://blog.fehbvm.com/Article/details/gfkdjzyil.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wap.zdbjq.cn/Article/details/gimiwjntj.sHtML

[Q05] 重命名列
来源：http://wap.zdbjq.cn/Article/details/gufumutfg.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.share.zdbjq.cn/Article/details/gqfexmltb.sHtML

[Q06] 删除列
来源：http://www.blog.hesvh.cn/Article/details/gvurptwzw.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.blog.hesvh.cn/Article/details/godcmzbgf.sHtML

[Q07] 删除表
来源：http://wap.fehbvm.com/Article/details/gutyrcajs.sHtML

DROP TABLE IF EXISTS orders;
来源：http://baike.zdbjq.cn/Article/details/gkbzxkubg.sHtML

[Q08] 创建普通索引
来源：http://www.blog.zdbjq.cn/Article/details/gzwkcezyi.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://wap.hesvh.cn/Article/details/grmhgmthk.sHtML

[Q09] 创建唯一索引
来源：http://m.share.zdbjq.cn/Article/details/gqocxwkio.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.share.fehbvm.com/Article/details/gsrdgfpyb.sHtML

[Q10] 插入单行
来源：http://www.share.fehbvm.com/Article/details/gkijstmdh.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mobile.zdbjq.cn/Article/details/gucinhcob.sHtML

[Q11] 一次插入多行
来源：http://blog.fehbvm.com/Article/details/gygkkdomc.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://read.share.fehbvm.com/Article/details/gxbkvhbhd.sHtML

[Q12] 插入后取自增 ID
来源：http://www.m.share.hesvh.cn/Article/details/gysiffspq.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://read.share.fehbvm.com/Article/details/gndejlhdd.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mobile.zdbjq.cn/Article/details/gdyjuakbn.sHtML

[Q13] 忽略重复插入
来源：http://read.share.hesvh.cn/Article/details/gdfwyxsqt.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://m.share.fehbvm.com/Article/details/guvtcpcjm.sHtML

[Q14] 存在则更新（upsert）
来源：http://baike.zdbjq.cn/Article/details/gpinrhrod.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baike.fehbvm.com/Article/details/gmzsgxcgd.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://m.share.zdbjq.cn/Article/details/gmptyvjgh.sHtML

[Q15] 查询全部
来源：http://m.share.fehbvm.com/Article/details/ghaqxrlro.sHtML

SELECT * FROM users;
来源：http://mobile.fehbvm.com/Article/details/gendzrbmt.sHtML

[Q16] 查询指定列
来源：http://baike.hesvh.cn/Article/details/gcqurjhlo.sHtML

SELECT id, name FROM users;
来源：http://mobile.hesvh.cn/Article/details/gzjvcgtkv.sHtML

[Q17] 条件查询
来源：http://www.m.share.fehbvm.com/Article/details/gscwyxuvd.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.fehbvm.com/Article/details/gqhgtyfns.sHtML

[Q18] 模糊匹配
来源：http://3g.hesvh.cn/Article/details/gqdkzpebx.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://read.share.fehbvm.com/Article/details/gsywqsbrj.sHtML

[Q19] 范围查询
来源：http://mobile.fehbvm.com/Article/details/gmxtsygqc.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://m.share.fehbvm.com/Article/details/gslffuuwf.sHtML

[Q20] IN 列表
来源：http://www.blog.hesvh.cn/Article/details/gczxvaxno.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.share.fehbvm.com/Article/details/gtlgmlfhm.sHtML

[Q21] 空值判断
来源：http://www.blog.zdbjq.cn/Article/details/gevlxauag.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.blog.fehbvm.com/Article/details/gnuutqinv.sHtML

[Q22] 排序
来源：http://www.m.share.zdbjq.cn/Article/details/guxnzwpxb.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.hesvh.cn/Article/details/gcpodpdoc.sHtML

[Q23] 分页
来源：http://www.blog.zdbjq.cn/Article/details/graauyjxt.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://3g.fehbvm.com/Article/details/gxifzbmkw.sHtML

[Q24] 去重
来源：http://read.share.zdbjq.cn/Article/details/gskjdqioy.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/glbsgvwpj.sHtML

[Q25] 只取前 N 条
来源：http://mobile.hesvh.cn/Article/details/gkondkpoy.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://3g.hesvh.cn/Article/details/gqznexvfi.sHtML

[Q26] 计数
来源：http://read.share.fehbvm.com/Article/details/grcuudeem.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.share.hesvh.cn/Article/details/gvhtkhlih.sHtML

[Q27] 条件计数
来源：http://blog.zdbjq.cn/Article/details/gzxulxyow.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mobile.hesvh.cn/Article/details/ghojjilkb.sHtML

[Q28] 求和与平均
来源：http://wap.zdbjq.cn/Article/details/gmwvcvsaq.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/gdylblaiw.sHtML

[Q29] 最大最小值
来源：http://www.share.zdbjq.cn/Article/details/gtrluwfmq.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gaqhpdaxd.sHtML

[Q30] 分组统计
来源：http://baike.fehbvm.com/Article/details/gncobclze.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.hesvh.cn/Article/details/grvcuwnno.sHtML

[Q31] 分组后过滤
来源：http://wap.hesvh.cn/Article/details/gidnuvxhl.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.hesvh.cn/Article/details/gptfvhqho.sHtML

[Q32] 分组拼接字符串
来源：http://mobile.zdbjq.cn/Article/details/gowerfuyr.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.share.fehbvm.com/Article/details/gtgaobhlf.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wap.hesvh.cn/Article/details/gznnegjgu.sHtML

[Q33] 多列分组
来源：http://wap.fehbvm.com/Article/details/giotcawgz.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wap.zdbjq.cn/Article/details/gjmapsrhr.sHtML

[Q34] 每组取第一条
来源：http://www.share.hesvh.cn/Article/details/gzqkenwoi.sHtML

SELECT * FROM (
来源：http://www.m.share.hesvh.cn/Article/details/gjlgkvrtx.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://3g.fehbvm.com/Article/details/gqvvjlbkn.sHtML

) t WHERE rn = 1;
来源：http://www.blog.zdbjq.cn/Article/details/ghzgwjqsl.sHtML

[Q35] 内连接
来源：http://3g.hesvh.cn/Article/details/gbdynirot.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.zdbjq.cn/Article/details/gxvwroipw.sHtML

[Q36] 左连接
来源：http://www.blog.hesvh.cn/Article/details/gkzlxdooj.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.fehbvm.com/Article/details/gficatmes.sHtML

[Q37] 右连接
来源：http://blog.fehbvm.com/Article/details/gzwmqvvpt.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://baike.hesvh.cn/Article/details/gulfhdvhj.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://blog.fehbvm.com/Article/details/gxmsffsfl.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.zdbjq.cn/Article/details/gcptjiwdx.sHtML

[Q39] 自连接（查上下级）
来源：http://baike.fehbvm.com/Article/details/gvfifdigy.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://baike.fehbvm.com/Article/details/ggfnthbbd.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mobile.hesvh.cn/Article/details/gddlsdvnt.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.hesvh.cn/Article/details/gbjfsiyyj.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://blog.hesvh.cn/Article/details/ggwsaqwwx.sHtML

[Q41] 多表连接
来源：http://www.m.share.hesvh.cn/Article/details/gpwplwqmk.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.share.zdbjq.cn/Article/details/gkulauyur.sHtML

JOIN users u ON u.id = o.user_id
来源：http://read.share.fehbvm.com/Article/details/gcedsnzxo.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.fehbvm.com/Article/details/gijatudij.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.zdbjq.cn/Article/details/gbpxbtxsg.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.share.hesvh.cn/Article/details/gqiyluzmu.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.fehbvm.com/Article/details/gbikdkexl.sHtML

[Q43] 标量子查询
来源：http://blog.fehbvm.com/Article/details/gmeaalzll.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://blog.zdbjq.cn/Article/details/glbjubyzv.sHtML

[Q44] IN 子查询
来源：http://www.m.share.fehbvm.com/Article/details/gawjhyolm.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.hesvh.cn/Article/details/gjbgvnesz.sHtML

[Q45] EXISTS 判断存在
来源：http://wap.zdbjq.cn/Article/details/gzsdauwbx.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.fehbvm.com/Article/details/gqtrienhx.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://m.share.zdbjq.cn/Article/details/gxyijtdqb.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.fehbvm.com/Article/details/geldzuodd.sHtML

[Q47] 与平均值比较
来源：http://www.m.share.fehbvm.com/Article/details/gfdudocbe.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.fehbvm.com/Article/details/gfzjqwbrf.sHtML

[Q48] CTE 公用表表达式
来源：http://3g.fehbvm.com/Article/details/gfgblekls.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.blog.zdbjq.cn/Article/details/gcqznzicy.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://wap.zdbjq.cn/Article/details/gyhowdxff.sHtML

[Q49] 更新单行
来源：http://wap.fehbvm.com/Article/details/gsctjsutt.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.share.zdbjq.cn/Article/details/gqujgwbpv.sHtML

[Q50] 批量更新
来源：http://wap.zdbjq.cn/Article/details/gmmvlvijy.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.m.share.hesvh.cn/Article/details/gdcufhlnz.sHtML

[Q51] 用子查询更新
来源：http://blog.fehbvm.com/Article/details/gabiorzbf.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wap.hesvh.cn/Article/details/gnqdyrsci.sHtML

[Q52] 删除指定行
来源：http://www.share.fehbvm.com/Article/details/gdycvkiko.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.m.share.hesvh.cn/Article/details/gcgudbsze.sHtML

[Q53] 按条件删除
来源：http://www.share.hesvh.cn/Article/details/guzzzcpkv.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.hesvh.cn/Article/details/gjklzxcro.sHtML

[Q54] 清空表
来源：http://www.share.zdbjq.cn/Article/details/gelbwkjkp.sHtML

TRUNCATE TABLE logs;
来源：http://blog.hesvh.cn/Article/details/gafzousru.sHtML

[Q55] 排名（并列占位）
来源：http://m.share.fehbvm.com/Article/details/guphocbrv.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.blog.hesvh.cn/Article/details/guxeddvqd.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.m.share.zdbjq.cn/Article/details/gzrgzousd.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mobile.zdbjq.cn/Article/details/gjrijkiyc.sHtML

[Q57] 行号
来源：http://mobile.hesvh.cn/Article/details/glzlbpfkg.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gxdrjqzax.sHtML

[Q58] 累计求和
来源：http://blog.zdbjq.cn/Article/details/gioyilvxh.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gxnsyrbdw.sHtML

[Q59] 分组内累计
来源：http://read.share.hesvh.cn/Article/details/gdfdirekq.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.zdbjq.cn/Article/details/gvspsffdd.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.zdbjq.cn/Article/details/gjcsgkxuj.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.m.share.hesvh.cn/Article/details/gzkpwktse.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.fehbvm.com/Article/details/gmysyxplp.sHtML

[Q61] 移动平均
来源：http://www.share.fehbvm.com/Article/details/goielydfz.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.fehbvm.com/Article/details/giljzathb.sHtML

[Q62] 分组占比
来源：http://3g.fehbvm.com/Article/details/gdnqawluf.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://baike.zdbjq.cn/Article/details/ggsudjbhf.sHtML

[Q63] 开启事务
来源：http://www.share.zdbjq.cn/Article/details/grmgfbqsw.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.zdbjq.cn/Article/details/gdjtumlzj.sHtML

[Q64] 提交事务
来源：http://www.m.share.fehbvm.com/Article/details/gkkggebjd.sHtML

COMMIT;
来源：http://www.share.hesvh.cn/Article/details/grhmytxcu.sHtML

[Q65] 回滚事务
来源：http://www.blog.hesvh.cn/Article/details/ghojxvnbv.sHtML

ROLLBACK;
来源：http://read.share.fehbvm.com/Article/details/gehfjyvmm.sHtML

[Q66] 行锁查询
来源：http://read.share.hesvh.cn/Article/details/gqqetconr.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.blog.fehbvm.com/Article/details/gmwzxnrni.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.hesvh.cn/Article/details/gbratrpxn.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.fehbvm.com/Article/details/gwjncbvbk.sHtML

[Q68] 保存点
来源：http://read.share.hesvh.cn/Article/details/gxxmjwmvv.sHtML

SAVEPOINT sp1;
来源：http://blog.zdbjq.cn/Article/details/gfrobeavf.sHtML

ROLLBACK TO sp1;
来源：http://blog.fehbvm.com/Article/details/gffqtifui.sHtML

[Q69] 查看执行计划
来源：http://3g.zdbjq.cn/Article/details/gdytohgto.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://blog.hesvh.cn/Article/details/gelyvgjzp.sHtML

[Q70] 更新统计信息
来源：http://wap.hesvh.cn/Article/details/gasjfhlgw.sHtML


<!-- 参考信息 -->