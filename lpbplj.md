代发 wailian999

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3nqebssmi.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3gsrjaxss.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3ufxpidol.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3fjcncsiw.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3friagvkr.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3yjgjgtgt.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3nznspnor.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3yodftaya.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3reyxluwy.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3cbkinoax.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3pkieiuxa.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3igcgzgcv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3owguxerb.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3isaftrsq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hspfnqni.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3qbtagxnx.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3zqhsxwpq.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3jgsczmsk.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3whjjgqlq.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3skezxmve.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3frwvfnuh.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3ppevjccm.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3ovbypqrm.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3thianldf.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3mclsavty.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3mnfduhia.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3gposmipz.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3vdtkhehv.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3jygkdwxn.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3ovfachpj.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3lhzirymv.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3vuvnjsip.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3oqtcbavm.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3uvqooqma.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3qgpjbynn.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3tutfafku.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3ebusnctd.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3aefucshi.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3cppltrri.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3cjocxrip.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3wddwdfqm.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3gqeblbmc.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3husghbix.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3afibbsnf.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3kbfhzbxx.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3gxuvirvh.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3iytvirtx.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3yjkhjkhe.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3lstzhhat.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3tmkvnzdb.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3ycciuhmv.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3ayhvbqzp.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3qoovdyhu.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3cugqzwag.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3cbrptfgt.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3cqfvetot.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3biijpmjt.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3ajawpmpj.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3izqqpnvb.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3dcwqnxof.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3imfswvuv.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3sphwpuda.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3dfkfumqh.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3ajxecden.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3yhutncpa.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3vxrwnmcb.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3djausogx.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3yfwkdvre.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3suycmpol.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uqbiqays.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3xsubvjzt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tpencvwx.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3ztdaqtbp.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3iyqcyizc.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3iwptbflv.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3wzjwboou.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3nmbvvaif.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3zzutsbrl.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3gorrokoa.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3ruptspuv.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3oxcasopl.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3bnyksbqz.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3vzlmhmon.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3jrjmrmfb.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3umfarncb.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3jfpwmzaj.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3vgzaglwa.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3dsjtzftl.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3thumxrfk.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3gwccahoo.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3zhjqtlhi.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3disdryby.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3bpjpypcf.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ghfshckn.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3lxlwfecd.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3kxemmsgu.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3kvvtmzqj.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3ejlszhov.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3wvszqiaq.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3vvmuwabz.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3hngcfqbl.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3spbvbvzy.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3pbahweco.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3lhgkewik.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3jcimgiki.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3hbopcshy.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3qqrcvymr.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3eyuuadtz.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3uxvvltbp.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3lqrigouy.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3fwlmhods.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3itsgoevn.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3qlkefrrt.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3vrgusyvz.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3huokyvda.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3qdpqhioz.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3ksoedisr.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3astzbjir.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3bebefwyf.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qanhgokt.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3xsensova.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tyusxlrq.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3yygbgfkf.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3pnwvafin.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3zfmhppeo.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3crbgaabz.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3xmzfuzec.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3pnmtkeea.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3vjcbmhcn.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3ikptxktm.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3jcxeyego.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3xnpvkigg.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3xjeekhbr.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3dtlhcavb.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3ebjxgpyk.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3mbuulxzz.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3xrbrgphn.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3dbauamyi.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3hrnpxidv.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3rfxkyhoi.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3krukhvqv.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3vtmzsryd.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3dvhdcoqi.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3rsrjznjo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3poejdzxd.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3nhznllqu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lhkshykv.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3lqjbmcuq.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3hbuiwneg.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3zeahkxhz.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3bozybeyn.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3dwcakdzc.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3jkqvagjd.html

);
来源：http://www.52xcode.cn/Article/details/gt3wsavppai.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3uhrfqjdr.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3gbrtpyqh.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3mzkidqws.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3ctcbetrg.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3zpfbzuoh.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3dqdebnjh.html

);
来源：http://www.52xcode.cn/Article/details/gt3vcfpwloj.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3uhihfmkc.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3kgmcfayf.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3quiixrer.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3hfgebuib.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3nnlyvebi.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3xeqlsglq.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3kuunlulk.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3fctikxof.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3vlacouls.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3linajtsl.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3yqbultni.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3ercwnkgx.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3rwqwiyhu.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3qhrmtyek.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3vwzihtje.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3abjjtusi.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3ssekxvoe.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3cbulnmao.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3gjjbuopb.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3jsmysgvp.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3zagmcbyl.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3zxpfmiib.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3zorzdpnu.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3qlsqcipo.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3xdtbhbig.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3zovnwevh.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3iropvbkp.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3cvsftzmg.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3dltuqctt.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3atxtrgbe.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3kqhnpmgo.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3dllrpgbo.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3ddejgbvk.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3aoizpbkx.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3ouynhisy.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3sfoibjsq.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3krowyjpd.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3lqxtbbdn.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3ugapkkbi.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3etjjojjy.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3qawszjjt.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3gudmhwgz.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3gqeyzyqb.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3gmuewrgd.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3ianjnbvm.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3kdwtznfw.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3cqvqstoq.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3sjtpuugo.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3yipndnqz.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3pjtzmgha.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3utfvmzjc.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3cwhkqfxr.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3jfmvlbzq.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3iovayrti.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3ydiccuxe.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ohvzicsw.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3rfsykmuh.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3fjpmonmm.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3cnhqbnlb.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3qmowkgax.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3zczptkyj.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3cyfarhri.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3dadtvjjh.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3odedlmve.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3jcuwgwkx.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3upjzalhy.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3ewqqcorg.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3mtpdczir.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3peiieooj.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3rfpcxucm.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3pagdfsju.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3wbrpzhbj.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3eqrlhrlq.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3zcejsmxd.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3cwzfglst.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3vvzkzxpa.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3rpizqath.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3jxqzjxru.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3wxboiayf.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3jommhaus.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3lmjkljqt.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3ujqrxydq.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3rglvxqin.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3zhxsoedd.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3xomnqtvd.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3rjtayltg.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3yepfdvct.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3frvgibbe.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3zvcrmhnz.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3frzredvp.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3joxtggum.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3hutaaobz.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3mzqrmsry.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3euiqgubv.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3dmanbofr.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3gxgnzedy.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3jfozfmwu.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3lxexhskl.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3diwdmwen.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3ekbdtftl.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3ppovtnmu.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3cobphavw.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3lphxzchr.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3jiycfkiy.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3cshkbmtj.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3dlxmxxan.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3mdhvyotu.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3yrstjtxm.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3wychfbyn.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3bbjwbdtg.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3ubyoomgx.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3pbewzypf.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3zbyhzdxr.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3qtgvefxg.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3olhcdszc.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3xlaqzxdp.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3fudxirrc.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3uuzterbc.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3xatyioyp.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3poshkzwx.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3uanvaija.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3iteylhje.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3cgmjbnqq.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3qhwygznb.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3oafluskm.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3nbkipiaf.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3grsuarji.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3chiyovfl.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3gmmvbhhc.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3jefnykzb.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3rbcggixi.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3pwhkyzgb.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3rzhbgkhn.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3sefkaegb.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3dtvcvhop.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3hzfidkrn.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3dgxyfspx.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3glrbkxse.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3jrfspjbd.html


<!-- 参考信息 -->