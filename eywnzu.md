代发 wailian999

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3eurgeqcb.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3ytmtiwcz.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3jmjeppvl.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3bsfjxshn.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3fklvndao.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3plulkowm.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3rhbdaxzo.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3zjhnxdva.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3uitqqfsh.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3uxseyiio.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3wgzobwkh.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3aoqtajff.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3cfravmjy.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3oacduiis.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3uquzspfu.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3svubwewl.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3zejmlras.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3eddapoww.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3ripfdeoi.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3qhsyxcpi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yjdolfzv.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3vltxomgj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yxoxmfwo.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3vgfhcpho.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3rrlmzfiq.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3djksedyv.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3zpvhjpnx.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3lqmfhgjm.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3verljclk.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3qoovcthu.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3gfrwcorm.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3nuhgfebi.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3jrkaaakd.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3bmtkkpui.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3dmrtnhkr.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3ccabpkfq.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3uowfsxmv.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3behsqohv.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3tackculc.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3cpvbnack.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3cmibecrq.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3kqgwdrwk.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3zuynummu.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3qtslijia.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3cutzydiq.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3rdhfmvua.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3sqmwgxgf.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3bfghguky.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3wvzrgsjx.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3wepqzocm.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3hhuporho.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3nbwzauva.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3xzhezxbm.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3hniajbdp.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3vmpqbyww.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3vqynbdos.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3hkugnall.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3qehdhobq.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3xnjorkng.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3umexgasg.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3svxwouvj.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3xclpggqw.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3ahkfffrq.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3rcvwvjqg.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3kdtkhoxe.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3blevpkqh.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3jzwvuqto.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3aapqxkqq.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3qmzuonjx.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3bjuhzkrc.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3dqszkfyd.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3vzrnwjso.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3mjupddev.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3winpxgsg.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3ckmsrplv.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3ecbmmzox.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3csqdlzth.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pmmikwum.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3couxpdmq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uabqdnwa.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3anjkrdit.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3ryhehpvd.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3jbumoczl.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3vxjpbjak.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3bilgwcia.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3siwhuxzc.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3rbvujrzc.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3qnwpwxhc.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3qhlfgslc.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3xvdpjfeg.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3pxodawyo.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3jnljuqit.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3uhjqaqbm.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3bgeabdiw.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3ogybigue.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3qjubrmac.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3nwgzeamt.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3uxvsmvfw.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3jwvbrrxj.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3vvmqhzyn.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3sdqacgsw.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3curxioua.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3aprsoelk.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3yagibpux.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3qwtplwvz.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3rszqwwyr.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3kufqozgu.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3jjbosidu.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3fqeojduo.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3xssuqupw.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3actvited.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3gsvulbvs.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3hbezclyh.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3hdriaksk.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3gvfirdbx.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3dptntawg.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3xrbakxvw.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3rfgfkpic.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3jzelxvqj.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3hrcbdsgn.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3ukqrpdwd.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3mfhiblzz.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3cnpaauqh.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3jlfbqazf.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3lbcxckof.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3issjlzyb.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3payegktn.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fbtxyzuw.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3vprywjdt.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3sonmzbve.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3btlhamyp.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3pcaqmrat.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3tscymtjk.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3jepdisij.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3eymlqbse.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3dmcoupmp.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3uoaoopda.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3cmedgtvb.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3lqkenpya.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3qlrjxhfl.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3rrukmoqp.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3ffedhqaf.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3ntlxcvsg.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3wiuaoxlr.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3tlbgbqyg.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3hvybqyih.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3qevxxlhp.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3wxbndvws.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3rfbpnsjd.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3ekodsbml.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3bbempjuo.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3kjjnpods.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uaomomjr.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3xqsrixfw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vzcsrhod.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3zebotjio.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3rutusjfn.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3zffmyqki.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3wtefiavd.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3npbxfcob.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3kusejmfo.html

);
来源：http://www.52xcode.cn/Article/details/gt3sjvufwvu.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3hydlxctp.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3tmtqnnua.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3kuqzoowh.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3uyjmymsi.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3qhbyvzik.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3ckvdwthg.html

);
来源：http://www.52xcode.cn/Article/details/gt3fjymjkck.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3zaklldod.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3ckhrokst.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3oamxpemx.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3zictwsjz.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3gwuxeghd.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3bwghrpxc.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3pfcnwusu.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3eifasvqn.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3flhnqmsr.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3zxzcrrzu.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3pkuqrkbc.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3osugfgwl.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3jbjoipxp.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3jeufqebn.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3jwwsxlan.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3skixxvqe.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3efnuxmex.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3xsweevnb.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3qwpvafyd.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3mfxnuent.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3fgbhlavc.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3exkbfpvh.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3hogsfumw.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3mhrkobtt.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3bnsbfiwb.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3vctumyna.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3kzinqmux.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3wmlnjhwv.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3hdeqnrol.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3jmqgqlod.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3vjicskyd.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3fggqplgd.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3ttjewktu.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3vqsdhyux.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3idoofaym.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3gblvnoka.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3onbxuqnz.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ajitwyhf.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3bmdjaisw.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3jmrwkilx.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3qrjrsrzc.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3arxyeceb.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3hmladdfa.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3jitccgnn.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3awnvsooo.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3cwwnkwlk.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3wnafwjyq.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3lygswjyk.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3erlywhvx.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3wovmvkaw.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3kefhybjv.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3srnjgoel.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3zbvlrqbc.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3mdphbaut.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3iuayebcx.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ydnehzov.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3yuyrwjff.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3rbygzxxc.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3pdofqfso.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3hhfpyuzg.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3drqkdyjn.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3dulmzzsc.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3koioncua.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3peqgaqfb.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3czsdhoez.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3ewawntaf.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3vfwhvzaw.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3aqtjrzub.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3kbsarrmk.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3kstqgvei.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3rlijywyn.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3qwtohtgl.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3vmsvkcyk.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3wetavabc.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3nxjptbno.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3syjasbnp.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3jbpnngoy.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3qugeiwyg.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3uxaotvkn.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3dtzsavcz.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3mefshzov.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3qipqoyok.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3rdiosrbl.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3ztbjqhrt.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3xurzbmdb.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3dxyaneaj.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3vrvwsanz.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3byyetbqh.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3kgsdijyx.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3ctxlitfg.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3fdqnoloa.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3aoazwkaz.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3arpbxfsp.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3mzjkftch.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3intqrtzf.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3qjwzodob.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3ravyexnr.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3mpqoyykr.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3pjaiyqlu.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3ynxlvvel.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3edugxdyz.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3bikpeolt.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3mncwkijp.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3mlndoxql.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3pkiqokcu.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3vmqlixao.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3mfojmhsn.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3nwvcekiq.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3vzgsyhmg.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3hpshkuew.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3wbiqxlhv.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3ogqwxhjh.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3qvaxulcw.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3djfceood.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3rqhckhnz.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3deuduioi.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3cemuontl.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3oirocmnn.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3acfutmsx.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ngidzkoc.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3rhtmlsuu.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3zcuvowmc.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3ykmbmfpa.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3wtwmgwbi.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3emnhbnkf.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3uddgkmrz.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3iwyiioli.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3lqiibgzo.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3bsgmgmwg.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3xszitmym.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3qucqgath.html


<!-- 参考信息 -->