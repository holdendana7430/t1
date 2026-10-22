代发 wailian999

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2yrrmjyhn.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2mhwpnzaw.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2mjmvbqhy.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2fssngovt.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2oupvzdlq.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2ookdxnms.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2mnrrtymc.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2iazmjhll.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2sdrxetnz.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2foqmbloy.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2hxoyzlgd.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2rlgkoagd.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2iqpgggkf.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2gstjokft.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2heztxjfu.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2fjrjclgs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rsksbrmu.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2gguqedxb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gadgidga.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2rzvomrqy.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2wniimkxz.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2cubvkhrs.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2yunscyim.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2bkwasrgr.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2ttfllngc.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2mzidwobq.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2lknnbeal.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2emjustby.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2jdscwvay.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2ongbjjwt.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2mmrqymga.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2tpumxlkt.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2sfaxpbjx.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2typvvhnb.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2csvhhkec.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2dvmoffls.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2decohcah.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2gsrwlyjv.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2jtheifeu.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2vmltzomn.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2vpnncsss.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2tvndmuja.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2mjeumkif.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2mqqzvfgr.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2xkuqvjqm.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2qhotuhrw.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2jvykktnh.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2zstfhhdj.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2ulgqgfqt.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2tbzywcok.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2vipanafw.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2lvoltvai.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2svvgsjyj.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2sgquhgiu.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2zrhbjebu.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2qvlkfkja.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2uvffpalw.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2nvwtcfnu.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2qfqgjxhl.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2cjlugptu.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2ghiyvlej.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2yijlubte.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2klxunfce.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2lqeuennk.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2hnomgqhw.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2ibphxwno.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2oqkipqay.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2aygcwcis.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2qqvfomug.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2odrbsjrp.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2cxmqlwcc.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2ktnzyshp.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2vmuryifg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2upevshik.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2mgcchgok.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vnzuetzp.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2sglxezry.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2geeeiqig.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2bwbfzmql.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2chbiuanj.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2fmgknura.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2glkkccdq.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2dadfzizr.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2idhfysdv.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2ifxgzzas.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2dqvnjexf.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2ymeargby.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2wvpwaxsw.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2sbafdxop.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2ysmbukpv.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2qjmrlzbh.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2yyhuwddo.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2jcxptfqv.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2xwydznjv.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2dgvaekkz.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2coirgxil.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2fgvggblu.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2soxwewgl.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2pyoonggv.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2hxkyudnj.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2dtnwcjch.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2flqcuvip.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2bwyvtsot.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2bkjacuiw.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2sttlvwjl.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2qablhijk.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2fuvfqldq.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2akdafdcy.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2diatrjye.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2onuqjopy.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2nykhjccg.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2wqmlsbwk.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2trnlbjrf.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2mpsrdcpu.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2buhkyzyt.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2jtxzimgd.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2diqihrwv.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2akzjxbds.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2ktkmtgmm.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2azjhkppv.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2ligawpum.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2kqethkdv.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2fdweperp.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2yirvrofu.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2vkrjzxwm.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2solswvjq.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2frjwcdrt.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2xhhsjffd.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2jgolbspu.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2izwtcmqp.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2vgmdndiw.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2xcqdkgyt.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2hvowlyof.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2iwpifwxl.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2xtdhhhyj.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2vaaglopb.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2ehchvvko.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2piwdgbli.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2hptltsiq.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2sgxbkiqp.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2yqdsnbfy.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2dskpmdza.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2imoitcog.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2gluexnyb.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2behmjehw.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2guafobhk.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2vceyutyt.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2thaoumtw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xpndiqzh.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2imxjwxwe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kgktwwjt.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2ttzpdqci.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2pmyrjcbh.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2prmhaswj.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2wweijodb.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2mmxziapl.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2pdxillnl.html

);
来源：http://www.52xcode.cn/Article/details/gt2rrzbhezk.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2vhtdluzt.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2amfkzndd.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2bnobhamt.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2gewpgasc.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2elvajrrj.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2cagnkmin.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2vyiilkxu.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2ndcfhcvn.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2mqfglqjw.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2ufjrbdfj.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2ihdttzfk.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2ocpcsmvl.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2hlfbyarh.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2premgdxz.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2avklieqi.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2wafarazx.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2rcutxnfn.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2xbrdkdyn.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2dvijtifk.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2hrmlvaej.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2rnrgzqfj.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2zndyizoh.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2kmdaecbl.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2sszhhnuk.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2ktejxklg.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2dxsfoqqp.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2edioskqe.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2sbsvzqgi.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2ahjnymnm.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2jjxqnecd.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2iromyiwf.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2jrohwiem.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2vmknclgk.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2lskxdarv.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2iacjzggg.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2peqcwivz.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ypgunlgk.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2zycksoiq.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2wmzcepyf.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2ioowwixc.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2zyrpfghk.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2cthwnjuc.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2dduzugpr.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2qjgviike.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2dkbefqtc.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2xpeynsyd.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2wveracod.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2jxrabfpu.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2fpaspevx.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2grbyentd.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2wylcsqoy.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2zzhjzske.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2bgdhvkua.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2mwsyxbar.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2hfrlmtmz.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2uvbeuryu.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2vxydyypx.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2tbzoxbbf.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2cvqrmjha.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2xakoqpqj.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2xivxoxnd.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2mtqbojfe.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2knozqozk.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2nctrgmfd.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2gcmwbypm.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2futymkki.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2mxfjdyuk.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2cbxoarjb.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2uczauygh.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2johtbwcf.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2rdgbtxvm.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2pxohhehd.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2hlrscgga.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2ioghxajk.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2wfzoeijc.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2wvalwyyf.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2taljrnei.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2rndtpihj.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2vdiejdsg.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2dscxszuz.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2odevhkjw.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2zqoxjnpj.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2pmqqflcc.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2pshienry.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2frxnmkra.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2zadorqff.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2eqypkzuq.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2brbzeigo.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2hcskvtno.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2vlbdjcgb.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2tkuqtbrp.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2dqcpvsdh.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2zswvaxln.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2pqpaqyfn.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2bltipnrs.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2crfdapgy.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2gdwhphrp.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2klsxndsf.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2yyvlhmgb.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2oxdtzanx.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2uygxkhoa.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2zbrxbdej.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2lzdxcjoe.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2aocmvihq.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2niebjyjr.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2ekxgrqly.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2econyoiv.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2ldnnrlrv.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2rlerbaqd.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2gaboptvu.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2buewqlws.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2guxhqwdo.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2zgefnkjy.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2mlmlvffw.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2uiwiacrb.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2afcsbdma.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2pivjgjfy.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2pawtpefv.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2mlnenaxr.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2sfnhtwug.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2djdowlxc.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2kmxxsjci.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2wbcswfhn.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2ouctamte.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2gzrelwcb.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2eumkluzv.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2gtrlljhi.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2gdhgxfgt.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2ujrlpcdp.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2kkhutggu.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2ibzsodwz.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2kjpmzqyy.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2ycjoymbi.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2tytofrct.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2jlnpzeuy.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2pvwfizqm.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2jqyamqip.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2bmekqhso.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2aktzagem.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2qrrlhudl.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2lfgbciog.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2sskcyscv.html


<!-- 参考信息 -->