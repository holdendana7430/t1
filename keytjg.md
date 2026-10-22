代发 wailian999

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2adnoczff.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2gswxodqg.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2sodbawku.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2hnbrpoov.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2pyswruax.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2bcwqoqfk.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2knwzoowt.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2xgmovjky.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2dxbvlydr.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2iymzfedc.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2mmmcaiom.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2ffguhebb.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2dvlpxrjp.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2bqlgdicx.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2yykhzcyu.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2vpfospsn.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2vxoqvztz.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2qzxakxnj.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2jbgdhbjg.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2vdlqcwip.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tjvvxduu.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2orfdoywc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mrcsrqrz.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2xlxodqnq.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2resjjyus.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2ynbtclad.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2otszwvsk.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2vfxtdumv.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2qvlfehxf.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2andllocx.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2wvngxdnj.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2wrkufxas.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2mbniunfy.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2ewqjyttm.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2goadpcle.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2cwfkdtxz.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2clutosvs.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2jkyvoccp.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2gmeaohuv.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2ofubeigy.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2bfftixhd.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2nncqabzb.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2tjpcoddf.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2wwkaamhb.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2cmskrfxk.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2uvdfchtq.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2anwinogp.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2fofoojhc.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2timyxqdl.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2upvrbskd.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2bplgdkvz.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2vvywgjlc.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2osxhognf.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2eiffpads.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2byupnvzr.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2upyaakwk.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2fnripbee.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2zoioxsyi.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2uxphfxgr.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2qdocpsrb.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2fvojmhfh.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2hmwsbqtw.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2hhtmuekz.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2qbtqvxvp.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2uuycctqo.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2zqkfzqmo.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2shuzagkv.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2jarvcjjr.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2sklkosgi.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2zcwxqfqi.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2pnknbiaz.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2vbnuquoy.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2iqjcwogg.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2byfdzxkh.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2tqhxdykg.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2vnizcdxi.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2xabtcknz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ubeetrxf.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2bnctxain.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2shlpvxjk.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2ehtueyos.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2puignmlw.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2dtroltye.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2eozlaihe.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2juwrsgyf.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2oyeqmefq.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2xqfjkocp.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2wbflnzwl.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2gzuucjsz.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2casikyin.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2yjrwuuzo.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2yywfbtmk.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2xasseypw.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2amcoqxwo.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2xucvzjfo.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2pjgcsbbs.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2nrqzxkit.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2ntogfgrt.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2tecpynci.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2wwsyblxm.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2cpqmgyrs.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2ydktdxyb.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2qpglpwug.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2nkowvtni.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2zgaprmjl.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2rwkngunu.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2owwgfrbs.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2xvvpxiez.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2fjvofcvv.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2ezmsnpbv.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2hedkxozc.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2abretcwr.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2rpbhbxiw.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2pyaipcgm.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2optlpxng.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2erthfupz.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2zinanayx.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2cgdqohrn.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2ledocziu.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2fvlpmrzj.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2xwtssjny.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2ycxqfhrx.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2ghzivdqg.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2qyvhjiow.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2fvygluuc.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2timvddlf.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2wiwqquyi.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2thknwilv.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2fuitkvwt.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2itemgsgc.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2feyowvzb.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2lvgbunhq.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2ookufexj.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2acpjgycw.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2kwbddpyu.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2qnzsvhoz.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2noouvmli.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2cinfifel.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2btibkfgf.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2yjhyhigm.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2vdhaxbxh.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2hgmbgjqz.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2obywlnix.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2isidanve.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2nmjpgvtg.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2yyoneigh.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2qqvviitt.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2wkupixcs.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2awqkqauh.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2uoujuyoe.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2ohljjqnv.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2cwbrxakm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uiufbyth.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2ugshaija.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lftigbse.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2ynfvcasi.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2ejybwpbt.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2rckfgxoo.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2uvgqikoe.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2aopuyoyi.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2knlmnegv.html

);
来源：http://www.52xcode.cn/Article/details/gt2vfwhlrmf.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2bhjeviqp.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2ogzoohce.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2ufibxubu.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2vgbaatoc.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2kstnzrnp.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2rfgnvsop.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2vlkuwkuf.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2yazgguku.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2vcrinwng.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2wcgwuptp.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2vdnndaxy.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2dmbjvgfd.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2rwhbngpr.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2wfkybnps.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2cbidqzyd.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2jcjkrugt.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2sgxjbguh.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2jdjmdfvk.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2qdzwoutz.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2xdvpvood.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2cvsyusmn.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2zfikfbun.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2brxoskkg.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2wdfnkjyu.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2fwbwbupx.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2eqwncdqz.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2urjhfrzw.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2dgrjtmfs.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2eexjwfbk.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2xyvalzhp.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2ncfuazof.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2mxhypmkz.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2rlyeifcg.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2dqiluypo.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2wuolvidy.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2etnhnyez.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2mrtbdxci.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2glgfyibf.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2eoivixts.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2xzpxfdvk.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2fovoddmz.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2aabjduzx.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2kqgoctkb.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2tlmduubu.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2uuypmmaq.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2xnffkwnz.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2qhiqswqd.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2pmklesvy.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2lgrxwldw.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2xmeknyah.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2bznznrws.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2ttgaoknb.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2bwxfsxqw.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2ajcfgwig.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2ksouqilr.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2iqmtcccp.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2skolhjvk.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2qzhucbkc.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2wmaknpuz.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2pavsaemm.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2cmsmxucg.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2uatsdmbp.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2lcbpxyzc.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2bxnkufll.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2xeyraspg.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2sqgpmcyg.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2doybpmrx.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2ulmgsfxw.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2uodkidlu.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2ycgtqvkh.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2zovgdmbc.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2mssamyap.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2eyngzwle.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2ahgiinqx.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2jeodjhxt.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2zzqcmacf.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2aopmhdbd.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2jhxmanwe.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2pyrqaeak.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2ykkazhrx.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2uymiejfs.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2srmvekwh.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2fqawlubd.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2nfyqbgvb.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2daerxrph.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2eaplwdae.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2sqlxrfbu.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2xwrjjfad.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2xxkgbtlc.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2vdfgaguh.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2vofnpqno.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2rpvyeceg.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2dfooquse.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2czybcsgw.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2ulsjvqis.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2yqrccctm.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2mcrwtubm.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2gdyedojf.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2tdsawobb.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2hwzwtony.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2pqyhifmf.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2tatrrsmw.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2sgjnmgkj.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2ewyyzwxz.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2sfaerweu.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2zmsckwfo.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2nezhrmdz.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2jixeojfu.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2yveqqoqr.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2ckdewfco.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2hkvrfdzr.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2pyuobqde.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2fdjoclca.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2sfbirsiz.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2iokntfhg.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2gswvqgsd.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2vjindxfk.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2yixoloue.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2bmnbhihx.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2akwaomll.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2dbuvexlx.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2nfscodqr.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2yijbqddt.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2ixhfjcrx.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2hhemkcgj.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2dridjwzr.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2gmqdqtag.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2lgemixie.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2cxnppvpn.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2wxpncthn.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2awyapipc.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2uodybcym.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2skxgexvc.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2bwkhkrqe.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2ktjhgfmr.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2avcbonfw.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2qyfbxlcs.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2iokbekdc.html


<!-- 参考信息 -->