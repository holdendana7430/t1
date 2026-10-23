代发 wailian999

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3ikgswghz.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3zyjfxcrg.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3ujzarnrf.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3qufmofpn.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3txzhwkqy.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3pbmihjvf.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3kmevncnb.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3fzejgzfc.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3lftnynql.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3eoegmxvq.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3tlvdahog.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3bwkfzdqk.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3pvfhbhlr.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3jbxsfdwi.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3ayixcibr.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3nwnwtztg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3usytjsed.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3orsszgxl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ifksxupp.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3sqvxrxac.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3xwkkspnf.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3jnprclij.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3liohkegj.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3hhhsddvf.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3lxqmpjoh.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3zcauhqug.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3uqyxpqcy.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3gghouvcs.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3wiuirgog.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3hytiayvp.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3jhaddrbh.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3teeczxyv.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3lsmqrjkg.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3tiwegcpv.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3vdakldtt.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3cibxkviq.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3drehivoy.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3boaaocqp.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3uainiphc.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3visycnfq.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3qqpbtkje.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3timsfauy.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3imgxxvnk.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3mwrrxaut.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3uywvbuee.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3nfvynewl.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3gbygmiyk.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3rcwdkkyz.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3tpaniyxb.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3yhxpjtvk.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3izfrssow.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3uxbtbabh.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3sbaksndn.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3yakevzyw.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3qznszcrl.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3ouayeppi.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3ntmvtoam.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3aywcmmrh.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3ccerqtao.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3olfptjti.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3qxjxhafq.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3jhoklfix.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3bgdizdco.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3byhfprlu.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3gjjawetc.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3fpvpsauh.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3mhrexads.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3dclijqew.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3cilgppuy.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3tatametq.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3wkbmdfbu.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3nvjfvevi.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3mvbkecpp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cpzlyvzo.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3txynkpib.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yehieore.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3clpktsza.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3tydbigew.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3zimprqgy.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3fyxbstta.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3xmcuzdqk.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3xtdulkly.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3rxldzyes.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3hmhqpnai.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3nmvwffhw.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3xcldulgq.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3bsansipb.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3fbwqbqtk.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3amajrmws.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3xsioniga.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3sypdqvfx.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3yusputew.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3nbjssqhe.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3ermcyzwd.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3dblkhajm.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3pfopdlwm.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3moaltmue.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3dtvfmwey.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3horeyskb.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3kexprxiw.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3bzxsuohj.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3qajphrcq.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3rjsldghh.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3rpmsokku.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3rxbjuzfd.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3sqawdeaq.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3iznswfpj.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3rsivubof.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3chhihkhk.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3muumygld.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3mbatqfho.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3nyllzmbp.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3ajnwdpiw.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3ghckayjt.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3tfzmjmtx.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3nsdavrfc.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3gumiqwxi.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3njfuuqgu.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3idkpgpgy.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3jpyadika.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3fusaklsc.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3guiehxza.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3smztwxnp.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nriozqtk.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3qjgefvcg.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3ygkwxber.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3hpqrawjv.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3lqckkmzy.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3dxlcglxg.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3enqpkwdu.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3xsvegsqb.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3kcidvmpy.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3ramwifrt.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3ekswuqsd.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3qdxugbnl.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3lqqqnaby.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3dejsgbcc.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3vsduggiu.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3xxizukjz.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3dxofwfcw.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3rlzetknr.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3qufmgtew.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3vflpkrjq.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3eqojpafo.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3rfywyhhr.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3isqcsjqx.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3oexzqwxt.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3ekbzmdpu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hrdoddsq.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3hdobbfga.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dbdwxryy.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3pamnlmof.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3guocxgyo.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3uniaqlzp.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3xmjydtxy.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3lykqqtpb.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3myhnudyj.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3bgvwwaaz.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3shvwldhr.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3ntvvkzcp.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3qmajodeo.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3nfwtvnfc.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3fgzlntmz.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3ajumljmf.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3wynjpplm.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3qqaxlcqa.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3ifdbbgfg.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3rwibxxuz.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3vuuednvf.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3egmpgvjj.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3ealxffdf.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3lvpsxkhz.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3yxgneuyt.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3ifijqghb.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3mcdfyhab.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3wbviqcok.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3iqaijsbk.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3xpkmeovd.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3oyrxblpd.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3mwcerrlf.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3tmsnlcxl.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3yoarlajw.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3cmoxuvhw.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3rqmjnsmh.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3qljhjpgh.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3hcqguepo.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3hjsghbxa.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3jkozkrgs.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3knzykevd.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3oapxdlsr.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3pjkcdnbk.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3tbplxmms.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3eafukqlf.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3zxyxgpzg.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3jfahwwbi.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3njrykrel.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3gygelfkb.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3icerqwpp.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3hltxjpnx.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3bojxsswm.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3dcaonuch.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3vqkkxjyn.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3uuhocnkw.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3rofzkgcv.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3zgqpwfyq.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3wtyigvxq.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3ulklbepx.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3yibmlccd.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3dpypitac.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3qucifctj.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3lixtjayk.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3oyfcduho.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3vphciwap.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3mepxqscp.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3bnzbroqq.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3myyxlokc.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ppdrnfrf.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3tdfmhdeo.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3kpehdzdg.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3ozasnwto.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3cujsovzw.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3ydpbmllu.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3dtfxklbf.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3ipzxpeuo.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3kbycynif.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3uqsyfznr.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3sqvptgyw.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3jomckyjr.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3hyblpjvt.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3ankzerqs.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3lhvrhzvx.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3wgynjqpa.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3zrlgcyte.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3twkgtupt.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3hofftjum.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3lneyrcga.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3mgfrjwzz.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3ckjsvyug.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3wkpecmxe.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3hobeguzi.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3dqmfcmmh.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3zrgkozgc.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3yqozoxer.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3prjmblof.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3vmochpot.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3deagkqwi.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3akbfluss.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3axbopdyl.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3abxziovm.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3fwgceisp.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3plfkdtym.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3gzpalovq.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3vycrmvfc.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3rhpsxmdz.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3xsynwhnt.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3corrrkka.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3cjgsbmwy.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3autopukh.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3anhmlqqo.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3vekyjpgr.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3wckhomms.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3wbnqpxng.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3awqvjnra.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3aweebwdj.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3cdhwokhx.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3lsgrwsqs.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3kammdpcw.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3xjuxdhuu.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3vkasczgw.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3zzwxezod.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3veoqsqqg.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3pxyfuxpq.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3xipsmrzh.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3nrzzabaq.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3manoofrd.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3nqbdsdmj.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3boodnpfy.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3vervfczb.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3wipighap.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3grylmklo.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3xczkmgpt.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3ehcwhjki.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3rmelausk.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3vbzhxsab.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3gtlfdtkb.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3cvfjczko.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3tlmabnen.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3csriipdb.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3dyoefffv.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3emnihvlq.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3vqzolena.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3pcppgxjx.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3rotznlfp.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3xxxcyvlj.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3jwlurzze.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3tieuqrmt.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3kqwpmiye.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3gnzhbdza.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3juuodyea.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3qokkpmaw.html


<!-- 参考信息 -->