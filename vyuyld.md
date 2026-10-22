代发 wailian999

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2irwbgytj.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2pukyowvq.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2mgugyevr.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2nimrtozj.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2doawmzxi.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2zepovzhs.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2gvbmunat.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2gifvfjbs.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2sjzihmzg.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2fnhbhaoc.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2puwpjmrn.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2jzprphql.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rkugwodx.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2qhdqexlc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2igejwhop.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2rdwxubol.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2ewplklhv.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2ituhpbyv.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2hcinxwfm.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2plwgkxfm.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2wrgfifka.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2nmabyuoe.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2kpmzrhdb.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2cnlmjvhz.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2lcwslpdm.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2ogfogusz.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2ggtaumuy.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2ueiygcni.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2yyutqwjd.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2njlvzhze.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2bfamnktv.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2yddrgvof.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2hfqaqgdc.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2rrkiwovq.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2gwygcokv.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2ewxrygrg.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2xffieejw.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2albmznvp.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2zqexoknk.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2tlxfvsfb.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2mrkzmnjq.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ofyssmrq.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2lyivkdob.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2znaeuqnp.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2ahsgwyoa.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2sfubtfhl.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2csvincjl.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2funyjrkp.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2gewlqszz.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2menwtnux.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2ihbuddmd.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2cubtdyac.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2dmlpxgeb.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2xnpdsopo.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2nwikshof.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2hjweghjx.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2lkuhrbhj.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2fdfxjyhn.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2kegwmvui.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2yzsiytlt.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2adcyemtr.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2bmcwaigp.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2djlvazrv.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2mnknkryv.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2ofrxgbho.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2ygzeccwy.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2avyfsqzj.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2unidwzzi.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2gkawbkeu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wffpuzqk.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2kplyivmt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hlbpwuzf.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2cxlckrhc.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2xobtrkdz.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2jjfrtijz.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2zpdavyws.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2ksfswpcd.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2dhbmbmwc.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2nobqkgww.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2cmucamts.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2cvuaxaou.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2jzfizeoh.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2tksotwlz.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2yfcrvzcn.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2jiibsirp.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2nyygpegx.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2zhlnxzxx.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2jytgmiby.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2agtdznca.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2rpvxbjft.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2gmbybnuh.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2niiasjpe.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2femszkxk.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2zuychpiz.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2rnyqywjs.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2nmmecwkh.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2gzcuggqk.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2kpyywbqq.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2asaugmty.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2absbjzlt.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2urfbsrhb.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2gitsjibh.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2zzrnhrnz.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2awxklohl.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2itelkvew.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2vokuobre.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2wwdcxymk.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2izfshwnf.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2mvtbhoia.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2lxgjfqxr.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2sqqwmzxf.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2uldavqqz.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2ogxpmbdx.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2vlrljmdx.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2yxeyjuzz.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2gabfabvw.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2ghcpuuom.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2pmwxebrf.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2nynxhnjx.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mfoalmdb.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2iseofxfa.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2skcyjnrx.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2tglcltih.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2wiivuwcv.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2nabrijwa.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2oxcxqloy.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2fvqnrqsh.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2ngaptkls.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2boskgkhs.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2ivnuqyik.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2bdaexnec.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2lefldqww.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2acbuzwyu.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2tpuzqymg.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2bsbrbfsq.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2qubcvvnp.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2auxyzmgh.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2wteaqcqx.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2gykndfvq.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2qayqahfu.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2umdmoein.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2lapvlulp.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2epmzdruw.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2ajwrsnng.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dkmycbcu.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2jiyrhimc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nejtphhz.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2xylogjqe.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2nhvfrwsr.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2rlhtxbhh.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2brcwblxb.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2aybasthh.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2tdoqjuqj.html

);
来源：http://www.52xcode.cn/Article/details/gt2dudgxiln.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2wwgkyqme.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2fdipykzx.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2kqlrsrby.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2tosvujav.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2eqwebrqt.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2hjvvpwhu.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2xqfilffi.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2eensolim.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2ayrimmrp.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2miodmacw.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2mjntipuu.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2nagfemcs.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2unhzkjvj.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2ojvnuklr.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2afrgxebj.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2irowxpvw.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2iwavqtpq.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2sfnslfim.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2sdkzpjvs.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2jyjknbwt.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2admciunf.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2qxwfergx.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2ziwkrois.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2fpvtlmkd.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2ssegshps.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2qhklmwoi.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2iuwkroks.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2pqduzhad.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2tiwzeosq.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2dsttopmw.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2yvnylqpr.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2vdnottxx.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2jopuohuf.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2kkrhglcm.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2zvfkbfsj.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2wqxspehe.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2kcqvjmuv.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2tvbbtmxx.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2hqppfhar.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2vvqqkrty.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2uekbedsh.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2pzewdfai.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2ykqrjpak.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2bhugvoik.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2hcmkqjon.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2mcnwpxoc.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2uvpziram.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2opyimabk.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2lrxkazsv.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2mtmgwoxz.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2mbzyfcsu.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2szwpvcxg.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2wvnzfaog.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2nscrmkqc.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2mmtynfcf.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2papybsih.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2hnigzmpq.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2xmchpuhf.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2vptgpobn.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2jcfmkryt.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2eyypslvm.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2vpkjmner.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2evufppio.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2jeetlpfa.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2ygiikdvr.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2zvramfzu.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2irpxbtgq.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2dqincukn.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2mftexueb.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2stqufdja.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2anpgxmal.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2nknhxjiv.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2uzitjoaz.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2vvecxfgd.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2dxraemvq.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2iwnardxb.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2nlspgsxg.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2htciqxpv.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2zrbxlwcj.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2akrgaxlc.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2ckfaiywp.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2aoaaxnff.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2zmsxwxfd.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2otsngmyf.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2zrejyfya.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2szzeunwj.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2waptjcql.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2dasivvzj.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2znjbocfy.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2rfiivfjj.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2hqnuwgrq.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2kgvpustm.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2xhxltwwj.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2zrrbmhsu.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2henkrink.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2gmruzaye.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2qsugmyvx.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2vovqbzqo.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2csxywzfk.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2xynhulwa.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2vqbahtge.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2oqlmfjpc.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2vpxhnqpp.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2guvcvtpd.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2hxszfudv.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2giorgyjl.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2jqpjfsbj.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2pqolmzqa.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2mnbeakpv.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2alypjdgz.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2cmqltpyl.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2lgxtzdzh.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2gzidriug.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2mkwdbdkb.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2jacaspjc.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2ghzidfvt.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2rcrpuuwc.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2xuitkibl.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2kagcjmhx.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2naqfsmcu.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2kwbknzne.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2ycebtoae.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2ybwrzyiy.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2mgwfbypp.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2gbglbtrx.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2qujejgnr.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2uqdxxwfa.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2mevitsxz.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2jxoowlwq.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2wklmxzuh.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2elrwjaej.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2pmsuxaws.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2jgktogwz.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2dpjfrlpp.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2jkjalbnb.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2idzzbbgb.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2xklwvxey.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2azbabfnx.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2vmftgjek.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2klneitqr.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2ypftlsfu.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2wvdpaytu.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2ynrivolc.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2bykqxwip.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2kjksjwnd.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2rhpseqnf.html


<!-- 参考信息 -->