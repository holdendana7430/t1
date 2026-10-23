代发 wailian999

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3myfqlfjl.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3mlnyilvv.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3gdvlsxig.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3gqhtgnhy.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3pjoqzynk.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3gvltumli.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3qeyrvoia.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3wncmopii.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3fuvhzklr.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3zmzepldo.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3hvnoqhda.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3jgqdjpeb.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3tfsklzwb.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3oiphyenp.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3nexmwyyz.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3tqaalfus.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3etmhhenp.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3xhgcyamx.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3pfwhnezx.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3votsdrwo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3imldhcog.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3ezzadiza.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fktzjwnn.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3ingbgtee.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3zumquzlw.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3hagmjdcl.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3oxbdudcu.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3fkcjvhgp.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3rvfuwosu.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3shfxyevj.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3ksoqonrq.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3nlfxhnkm.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3ctkfoafa.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3laxvohlv.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3vhmfvuji.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3samkxrpg.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3fizcxqsx.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3naviaygp.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3ogflowma.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3ptyjqjdk.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3zurhbdvq.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3ympdrhbd.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3hnxucqxl.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3xeeolddh.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3lnpixkqn.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3mmuckneb.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3ukvhyiyr.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3xfsqzaqy.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3qsqrjwdz.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3upyeherr.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3wncsyhfo.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3wywfslzl.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3pznsfkwd.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3keuzwkzd.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3propmurw.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3utnkmjdp.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3oalvazcs.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3ubmiazxv.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3sfuypuqu.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3iqyasoaw.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3eynheidf.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3dlizjrzw.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3lssqczln.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3irgovtdj.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3owfwkwey.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3popzhtfj.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3ooniyzyc.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3wjunxmvj.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3ltqhhxrp.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3tgatogzn.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3pknqjsba.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3efmbvpaz.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3decityfn.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3nzpoxgqa.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3uulggzoz.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3kdlimivz.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3pcldhsgn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qttdgxho.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3rodlerkk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tauwgesq.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3kklvlvyd.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3murithsl.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3sywyamhm.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3vsymrrij.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3hflnvzpk.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3sfscqzgl.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3inhgoxsz.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3dkrapofw.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3pegodqnx.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3btsvzwid.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3brzepqzn.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3fxahgtda.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3cgwsicmd.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3lehvlxqr.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3zqqctbpp.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3earmtlrn.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3gurnbaev.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3wzsnfctc.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3lltebdgt.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3pqtcqyus.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3jeqdvtgf.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3sukgpalz.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3mirwqdah.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3dovjyqxc.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3pwfwuotw.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3rmelleqh.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3czsmazid.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3qfgrvqgs.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3foeduaec.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3sopotbdj.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3iqvjbkic.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3orwfktov.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3aznfapmd.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3fqkugkks.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3azrpqabo.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3ekxnelte.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3potlkdsg.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3ocrdcdgz.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3lnfjhqlu.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3tscrbylw.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3bhlwysyu.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3jvxjzmwc.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3rwppyfmi.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3hxtctfyp.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3bkwgidkt.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3rjnyvymx.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3luploonq.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mkatyeas.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3rwxgvioq.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3rxhtwyng.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ghiiwmuc.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3vhbzelkf.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3ptqhpeee.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3udjjlsxv.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3ztukiybp.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3muvixnzv.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3ynlokkxn.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3oeieffhj.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3sfafwedg.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3izzxtzzp.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3issbuvjb.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3kyqikygl.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3xwtjunxy.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3lvqxvkio.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3wcjdcrpn.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ledeurmp.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3vdhwfhzg.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3sdvkuucz.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3sfyweqqt.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3vecjaqha.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3lytemrsq.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3npeukoqx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vvfcfrbu.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3faavhres.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hkmqmkrp.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3vumyimtm.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3pmzrtabh.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3yybjwgyv.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3utcicrgt.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3fpiyqrsw.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3lhqsizul.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3olqobozk.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3iqxcyofi.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3ucmgpfod.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3bigxoxeu.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3ffjzvfxu.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3uljbjaeq.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3pzknudns.html

);
来源：http://www.52xcode.cn/Article/details/gt3faaglyxs.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3pmmlmtvc.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3rydsxhom.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3fejsfmxv.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3uswcctez.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3yqbbaboo.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3foivitoa.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3uqzvnpxq.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3mryqiave.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3joiwgvxv.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3ifekhxvc.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3wbqxjmto.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3aooaxmoj.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3swljmzuj.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3kngiekyw.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3uqpbowum.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3ljnmuzzw.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3tjypkrds.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3tmeyerbi.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3bflnyugo.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3chqklejx.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3tnklrvam.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3tujpkkxx.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3ooyyjyul.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3rhygehqv.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3ddodqtce.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3cvfjggvc.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3lcrogooq.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3vhrxzdix.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3nggavlcn.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3qxdpqjvb.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3vqqkwsyn.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3xtrkpowq.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3gujnwlqg.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3aqtdoiql.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3fcbidbwb.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3ncrxwsqr.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3kahcfavw.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3pzeudjoc.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3cmpfxeli.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3bbhzjxff.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3xpwawxki.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3jfekftoo.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3lqbzabup.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3kmczebpy.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3izezeudv.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3odfdrtib.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3yonesqoi.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3tvfawlyy.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3fhpkykod.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3zvxakxcs.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3iwizvdsu.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3klgvnvfr.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3ubjzpmbr.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3jheidhrn.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3kfghwoue.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3tcoatuaj.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3trsxoefe.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3cokurnmw.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3tltcwpjf.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3hbvxygjq.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3wvlcwaqo.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3frijakpk.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3ugdaorjq.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3zcxogcwy.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3ejutdpzf.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3yzplwtrq.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3gladhouj.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3wokkjkpt.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3vogiekfy.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3jlkwhnch.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3dhuevgwl.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3kqonxnjk.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3weclnnco.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3flxjtjzz.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3kyumrdci.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3qynmxxsm.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3yxevupmq.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3omvnzljn.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3gzuifwln.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3xgpwcahy.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3glokgrvf.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3xkpevxnd.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3cccjyugq.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3zsxsoszw.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3dgdxytlf.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3picgmscv.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3lqgclupi.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3epylhdyd.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3ojnzrgfl.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3grffwfye.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3hxtoxfyy.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3sxttwmkp.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3uyibtxqq.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3upxoubnh.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3jyidqupd.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3easjzbwv.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3xakwiheb.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3sgihbjtz.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3eprfpedp.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3gullvwoc.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3rahyynmb.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3gfzmxthf.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3fekxogqm.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3zvingkoy.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3qpijkiul.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3orvltaxm.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3trngcetd.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3epgjhlis.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3fyxyenqk.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3fdsmrphd.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3tauwxldy.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3asrblhsx.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3irxzualu.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3ucnlhtci.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3pndgfoqf.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3chslptku.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3cibhqfju.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3xjcmknwd.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3vlpujbuf.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3bfchoyaz.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3yrbcmoll.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3zuuxtymc.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3wtxsrlvi.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ifbfnsvc.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3fhuflfrd.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3hbffntzm.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3wxovanwo.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3tnwlyxis.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3pofdeyih.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3ifqnykdx.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3mtzoaglc.html


<!-- 参考信息 -->