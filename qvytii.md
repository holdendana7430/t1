代发 wailian999

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2mzpvrwcv.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2okpbwdra.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2vvppftru.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2dwsxfbyy.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2biwxraso.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2bdyyomgt.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2ydmhszkl.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2zrujsnzt.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2pyksatbc.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2qagvguic.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2qdikfsgy.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2qyzymfek.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2zcziocbi.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2bcbjflvp.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2arwxkitg.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2goovhqpx.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2qchbfnub.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2rxzhrfmx.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2wytspclu.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2agrydcrt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xeixniws.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2tryeidow.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hmjcofyp.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2hktoxrbm.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2srdytnlk.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2qhfmzwxh.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2ohlnisbd.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2hqwxnbzb.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2uzamndpf.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2errhmsjk.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2jtdjdzaw.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2plmowtkd.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2juhvzytl.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2dylggohr.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2okitkemf.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2lhyclesb.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2kexrpmyt.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2xtagbaag.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2jhfmgxnm.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2ymbwayii.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2ubuvxcdf.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2btvosirz.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2zxlyigzc.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2pmnppbno.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2jbjiwinp.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2uilydtak.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2gqproukh.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2ohgevnvn.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2ubdgxtlt.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2xkizpxon.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2dwrgascf.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2lroueehr.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2ztagccer.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2wiprtjxy.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2yqlxkrss.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2cklnhoge.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2circemmf.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2szpsdfpl.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2ieovbimb.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2skejrsba.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2sslimxmz.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2osxcvwzf.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2iywowomp.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2zeefjwnp.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2dadptxqq.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2cbxredgw.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2vrjkwkzp.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2tmltemsa.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2gzapjltj.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2uqjckqoz.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2jhtemjtg.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2jsfqruma.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2aqgjilnm.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2udnaoiom.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2mvnugmkr.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2duahbmud.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2ossnfkma.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2azzqnmak.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2wkhakoiv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2afkkvmfk.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2vsqtvarb.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2bghnpubk.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2ztbixvjd.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2bbprtwlt.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2hkjgkqqi.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2hbuwxfkj.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2kdukwkzc.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2mwkrailc.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2iizoaftk.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2ipppnizz.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2mkgfzcel.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2rsqednsr.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2lqpwpznb.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2poaxutpz.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2zljvkzjh.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2rhngddvt.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ztlmtjcj.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2btpgxyri.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2gddrexiq.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2bvdwhgqo.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2vgjycmtc.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ctxokpwd.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2axbdwwek.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2hgdcbstr.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2pnacfzsq.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2axzezyvi.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2dovxmrok.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2nlvszzqn.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2jnqrldlc.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2rhvyqxoy.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2zsjgomtl.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2rvqwerry.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2nvrqdjeq.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2sjtzhmct.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2ohkxlfhf.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2gzhcvtfo.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2jcqxhrir.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2zgltolmu.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2lhuixjbq.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2cpdmqlik.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2wnjbelzf.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2edmxisvt.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2gfxjkdyq.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2uixlmfep.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2rrbfkjzs.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2deydbsix.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2envzldax.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dxkhxpuw.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2faqubufi.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mcdimtsd.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ysjortux.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2glvmwody.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2kauxbxnq.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2upvgcxsi.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2gxgjptuz.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2xwerrpkk.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2bqjgymjy.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2hxeheird.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2fjihcljj.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2yxgjgjtm.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2mwbgqrsf.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2ifeeaqiw.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2jngdppac.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2zdsymjmt.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2dkroynhu.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2fslgohhy.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2qcdrvfux.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2cvdrozxa.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2ovmprmui.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2yrmpdnbe.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2ebiaxvex.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2sfehlneh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tmnwhoco.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2ixbetsou.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2umehluig.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2whowletf.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2cvewtowf.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2tdcaswvf.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2mrcomicm.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2gvggbjtk.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2ksfenhgr.html

);
来源：http://www.52xcode.cn/Article/details/gt2dbtjdatj.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2medarion.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2uhlexehf.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2aqaislwc.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2mrebsvzi.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2ltjhvxjm.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2hugswtjz.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2lgdigbky.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2yvlswecd.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2kllwtmlo.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2urendpuq.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2stftddxn.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2hxipltua.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2fvhiucbd.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2mywgzqjr.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2exnyujxf.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2nfodbetc.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2axuctdrd.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2lwvzbxsh.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2mxxdflbe.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2ptgiengc.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2woyvoxxx.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2iciisqoo.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2vhpnclnv.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2vejdpzoh.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2vsewvnnb.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2licstclx.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2jndlivfo.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2nupjyxmz.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2lszjjftw.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2zpwgdlcz.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2xpaucuuh.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2empsaxvs.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2vhazwlmd.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2vlzmiljg.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2mhenjwrg.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2tzyykecl.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ihtojbzs.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2uasyyznc.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2hffxdxkr.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2ggaxuiei.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2pvdpefxh.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2kiiedoxs.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2ufhyaxds.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2yckjofxv.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2uuzmvmde.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2tixasmrw.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2uxkdnipq.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2uolqwcmy.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2tniveikp.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2vywtuwjc.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2odyobpiv.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2efzmcyrz.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2okvzesta.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2dgkqfbmf.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2btvtjohj.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2fndngoki.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2diwufvej.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2pukbavzp.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2zdvqkhbn.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2sxewvgxf.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2noizjzmw.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2txzcmdfj.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2peealgwd.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2wgmygdbc.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2cfcehqnc.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2wcfkeqki.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2qriginzj.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2tytauevd.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2mpchnlhd.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2wjjdgkak.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2prrpckyd.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2pzowbfcp.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2kjljxrvf.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2vmhxzjnt.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2kmuzdriu.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2mifjmdkz.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2tvfivejh.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2vuzftakg.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2dwrcvtjv.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2teuzwlsh.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2tbzbvouf.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2uaieureb.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2dvvqxfyl.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2fagpnwqp.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2zeewqwda.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2xdwovwxq.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2llkvitwy.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2zvshthkt.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2cwcekmvd.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2kqbbkmsb.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2jslftttx.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2fzoskwcb.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2pkbigfol.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2acmsapmu.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2hlfxnfyw.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2cpsqnbwz.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2pwvciinn.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2ztsfpluf.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2vzbnushp.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2rtldejeg.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2fcfezley.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2plzalhhu.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2narhwbxz.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2cabtztdr.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2nncfimvy.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2ubbeyzfr.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2qlfexipf.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2okmzgywc.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2nprzyucf.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2nepouwge.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2qbckhqqs.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2zwcjgspl.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2viaztbmk.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2wkxhtibm.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2kglmaxlz.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2pddsrkgn.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2qqfadnaq.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2eyyfiwlg.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2ltzgpdir.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2nykgunme.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2nsvsfeel.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2hvlwbqtu.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2idnebgzv.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2jskwrtng.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2oiiidjzz.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2ewcejcvs.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2xayedgri.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2xjmpille.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2xzgzdkrm.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2lkvktypo.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2hbbzqklf.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2dixcgugw.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2tzvdovmu.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ymdiaaju.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2jmyyfpwu.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ogcjwcfn.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2holpmywr.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2jazkaicr.html


<!-- 参考信息 -->