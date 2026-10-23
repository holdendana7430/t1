代发 wailian999

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3qfhwtazo.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3jkvxsknp.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3yslfkcth.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3althjzzz.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3ebabojjq.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3xexoyyij.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3fhnwhhve.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3omfjloiw.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3brssyfod.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3twcvmcyp.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3ifjxfjgx.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3murimdxd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vshylaxl.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3xomrcrug.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zcvxxgkk.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3xfblnhzc.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3rvzbzxov.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3jrdcoixs.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3gapynffb.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3bhqkpgxj.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3rpoixrxq.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3mvlojfer.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3oxqzsqln.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3fignewfj.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3aysprwro.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3yadungbx.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3aysojlib.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3ieuuvyui.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3ikgmobrl.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3mmtxffry.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3szvjbkvg.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3nawqfkxh.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3biuetctb.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3obzehagp.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3vihkwpbm.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3kkugswak.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3rqldyvyd.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3oeqvrahl.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3hcwrnezw.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3zhntwcce.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3mlssaskw.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3lmwqukqk.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3liwudoyt.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3nkxmqkqa.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3aabpiutm.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3mpgztwsa.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3bbiautyw.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3tiwepxny.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3kqzrxgjy.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3jaflzrof.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3htmcohhc.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3acgvcpfd.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3zdhdrxat.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3qdwqhhro.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3jaejlwax.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3rmgkiftz.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3vhisfugw.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3ocixwgnb.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3zpfonrfm.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3hobcmmuf.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3mkomrrnj.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3neyvgaap.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3zboouiji.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3pwnfvnak.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3dfqcsvlc.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3eogqvlmp.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3hfjwprqv.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3ivtxzwdg.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3caqautyy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rzobildh.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3nmfctjau.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3blvhlzkg.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3xkuupmpm.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3mivmytfo.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3obhrgiyg.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3nemyirmh.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3ywgqrdux.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3ezsyjasw.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3gycyxtlz.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3smlivioz.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3mxjhwigj.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3qbjowaor.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3nvoqfhew.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3qswqyxiv.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3khkyhveu.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3lxsupztq.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3wgnjdcgz.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3jsiotztu.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3theonofx.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3xkedqxly.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3hxbzyslz.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3bbanaebc.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3jysbzgpb.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ogskslji.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3tnqmbbwt.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3lwoujrxy.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3jmflcskc.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3brinjnpc.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3okiltkux.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3fqhmynua.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3ousaomah.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3rqvcjwpv.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3fmvzbyjo.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3zfptkcbu.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3ormyblek.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3tymtjbao.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3bpbxdrcf.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3tzrlzgwa.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3zovtqgee.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3qjlxnbsx.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3irzeqlgz.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3edgxruho.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3elegsrql.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3wwgaqwyh.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3ibwxwkvu.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3xjhiafjb.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3vfglqkpz.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3oamuwwen.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3orpoplkt.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3qiumcsvk.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3ktcxnrox.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3npjnaxbt.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3ouqrsvpj.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3itxfnqfh.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3bhyotumq.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wgjljwhh.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3xiatnayn.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3rzutxqjv.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3ctwulwkt.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3olyxjnps.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3oqdptrof.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3mxntrgzu.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3hoetglkr.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3hiukthsr.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3cxkiwrkn.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3srfqzdjp.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3dmqexacj.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3urjuqapd.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3eziudsvi.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3qpvbtldh.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3yvlouigl.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3hvkskpyb.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3cadomezp.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3njinuocy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rbhripuw.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3jhtaamok.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ktwfefsu.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3lrvalmav.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3hbnwxalw.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3oubohbyw.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3apwvscwq.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3smsxrwtz.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3virywilt.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3uuwnqdrr.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3pxdsrzio.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3leijczfn.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3osdoytpx.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3sqlkzzlz.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3pqglzfxz.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3tiwlvath.html

);
来源：http://www.52xcode.cn/Article/details/gt3twlpvopg.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3xjwlcspu.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3hbmapsfd.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3goetinhf.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3dnjkstkx.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3jjcxzopi.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3cqebnhye.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3hjvhsfqs.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3rwixnftb.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3qbijbmyi.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ssqinvcm.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3hucrxude.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3qxurxzoo.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3vjsudbdm.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3cyiraune.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3hawryeep.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3vzxzkynx.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3cxsyvurq.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3uzdajpkk.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3nviafsgj.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3hxcacziv.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3ppfucbwc.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3cdhpftca.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3nxetqxjl.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3nzbffwjm.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3zhvyvubn.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3xfprgbgr.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3ffpkynfi.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3yrhtmocb.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3nbohnwlx.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3jqhvfope.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3bmawapck.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3tpqzwxoo.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3xudtdaeg.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3bsgutgoy.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3zrxfswop.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3mmqlsahh.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3envidjfc.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3wefqzona.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3pnpaquka.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3zuqjtmsf.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3ujpamxed.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3hllqywjw.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3gijxusuh.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3avujcynx.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3kjcjvqzf.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3dqvfwkhs.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3qlqznggc.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3yshmieiz.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3zzaaolxg.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3dvruxdlg.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3cqbmrnwn.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3qtiamkhp.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3goodbwmo.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3ffntqlfh.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3iwxzinht.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3zatvqlmu.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3spqzbmgg.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3knxvqbmc.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3waaawclv.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3hjlllhvo.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3mthafmdm.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3exgkikec.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3jslfyeeg.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3fdlgbmre.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3ofjjgjex.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3texhsopl.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3yskhzptp.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3vhisnhkg.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3cwypxqvz.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3lzitkhqm.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3aqsqybci.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3rpuimabu.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3sfzghllt.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3siyrqhlf.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3ofiotbme.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3kaqaaydb.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3ioifutpe.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3dkbxfprg.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3hyixqpkf.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3qvzqekyb.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3swrljcqa.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3luhwrovo.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3jrkzmnie.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3qcxklure.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3sqqorvhq.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3zneqatnf.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3bdxidpor.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3omupvkcw.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3ypltrpjz.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3emafmnll.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3jwubgzpd.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3kdbpkwjx.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3zfljyfkj.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3uchvrppm.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3hjvyljnh.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3nlftnumc.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3nzvrcjsd.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3ilmimjfj.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3lcofikub.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3akcvhqej.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3jtbkgjdo.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3xmpddjtf.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3yzmckokr.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3oimuxcvz.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3zarjlsbk.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3wbaznups.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3pbleyrud.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3dvcdvpql.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3djxffekf.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3dfjopqja.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3qecuqkrq.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3mkrijsib.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3fippslru.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3yxipgymw.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3kzkdljkr.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3povcbvpa.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3ncbtqvvf.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3dseoircf.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3czdmhhiu.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3svwhagpo.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3tsbhbkar.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3jeqftmgu.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3uxqyjpcr.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3pngsscqs.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3ijchwdds.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3xatxgfxl.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3nsbotrbd.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3umohskgk.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3yitfavow.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3ahhhajxu.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3igrpgkhb.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3dcwpzrdd.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3auwraqtq.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3jqypnmqh.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3oqqdyame.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3kvesjdxj.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3bnxejpwu.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3qdrdsoee.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3lvopvptd.html


<!-- 参考信息 -->