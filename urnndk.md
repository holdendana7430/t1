代发 wailian999

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.0kj1m.cn/gtaoalokos.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.xziqi.cn/gtcuxsqnwk.html

Java: class Node { int v; Node next; }
来源：http://hz.iojbl.cn/gthznkpcay.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.nanxuanxn.top/gtwtpekukw.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.hnxiangtu.top/gtqwdqrrop.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.andypj.xyz/gtyrtdyges.html

[N11] 二叉树中序遍历
来源：http://hz.chenlongwang.top/gtqkcnbjet.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.tian-w.cn/gtsavybwzm.html

PHP:  // 手写递归函数
来源：http://hz.tian-w.cn/gtmwyahsbx.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.zhiwuduotai.top/gtocbpogqr.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.c1oappe.top/gtvkolxbmz.html

Java: // 手写递归
来源：http://hz.hnxiangtu.top/gtwunqzmtz.html

Go:   // 手写递归
来源：http://hz.nanxinkj.top/gtdrppawkj.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.daxiang520.top/gtguvlvwqg.html

C#:   // 手写递归
来源：http://hz.zhijiandao.cn/gtaenetmtd.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.nanxinkj.top/gthiqtavhn.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.52xcode.cn/gtqaxdkgde.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.hnqzz.top/gtoszigkrt.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.zhengqikj.top/gtjidvzoll.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.nwbrower.top/gttirbmmrp.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.tian-w.cn/gtaqsojiju.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.ivvv.top/gthaucmdyz.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.nanxinkj.top/gtezajwnkf.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.tianlin.xyz/gtpewgjybh.html

================================================================================
来源：http://hz.aizwys.cn/gtxovvazoy.html

O. 并发与异步
来源：http://hz.xuetiantiany.cn/gtmsvwnuhd.html

================================================================================
来源：http://hz.nanxuanxn.top/gtnbwkdhjk.html

[O01] 启动一个线程
来源：http://hz.ywan-chungtsiang.top/gtirrnymbj.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.zycfv.cn/gtymmkaiom.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.shzxlz.cn/gtjnvorwup.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.52xcode.cn/gtbrrnlqrx.html

TS:   // 同 JS
来源：http://hz.jinqigufen.top/gteyzhqijq.html

Java: new Thread(() -> f()).start()
来源：http://hz.iojbl.cn/gtkklemsoe.html

Go:   go f()
来源：http://hz.kuanghao11.cn/gtdqsmbpfm.html

Ruby: Thread.new { f }
来源：http://hz.havefunace.top/gtxyspirlz.html

C#:   Task.Run(() => F());
来源：http://hz.gzhubu.top/gtmrcqntpx.html

[O02] 使用线程池
来源：http://hz.ivvv.top/gtufvpwdye.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.cucudq.cn/gttkhlnjfe.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.birdmap.top/gtkrrqtjdr.html

JS:   // worker_threads 线程池
来源：http://hz.zycfv.cn/gtjnpjlbds.html

TS:   // worker_threads 线程池
来源：http://hz.ydzc1.top/gttlwbhbun.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.chenlongwang.top/gtympmcyhy.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.wangshuangyany.cn/gtlbmkumzk.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.jinghuilouyu.cn/gtztukwmef.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.aibaodan.cn/gthrpvvgvu.html

[O03] 加锁保护共享数据
来源：http://hz.xziqi.cn/gtbajwpemy.html

Py:   with lock: shared += 1
来源：http://hz.jlsjyb.cn/gtikiphzym.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.hammf.cn/gtktnbmuih.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.meibo888.top/gtddtzkgot.html

TS:   // 同 JS
来源：http://hz.hysaishi.cn/gtxncqkfln.html

Java: synchronized (this) { shared++; }
来源：http://hz.yvedp.cn/gtocnwsqrt.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.quarkkingdee.top/gtnrlvlnwj.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.smart0.xyz/gtoqvsquqt.html

C#:   lock (gate) { shared++; }
来源：http://hz.xuanzx.com/gtybnfoirh.html

[O04] 定义异步函数并等待
来源：http://hz.feifeiyinyue.top/gttpcgbtdv.html

Py:   async def f():⏎    await g()
来源：http://hz.hysaishi.cn/gtjkyrdkcp.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.sxryk.cn/gtpfdpylrm.html

JS:   async function f() { await g(); }
来源：http://hz.xingfuxueyuan.xyz/gtwjswcoup.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.dianchejie.cn/gtzabpuuif.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.shuidangran.top/gthecmunnw.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.xuanzx.com/gthalauddd.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.hywenlv.cn/gtwctpnjjj.html

C#:   async Task F() { await G(); }
来源：http://hz.zhixingplan.top/gtciymkgto.html

[O05] 并发执行并等待全部完成
来源：http://hz.yj20258888.top/gtsdwbvapo.html

Py:   asyncio.gather(*tasks)
来源：http://hz.tian-w.cn/gtxvrxarld.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.gaohongyu789.top/gtbzkjlmhs.html

JS:   await Promise.all(tasks)
来源：http://hz.sysykeji.top/gtqknwanak.html

TS:   await Promise.all(tasks)
来源：http://hz.gzhubu.top/gtkegrlxfj.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.aizwys.cn/gtxrrmrcbt.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.iojbl.cn/gtourmafsk.html

Ruby: threads.map(&:join)
来源：http://hz.haohaochexian.top/gtgczhjwvu.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.quarkkingdee.top/gtfpaqjtup.html

[O06] 使用进程池
来源：http://hz.xuetiantiany.cn/gtylysrebj.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.zhixingplan.top/gtitkcusjp.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.hnxiangtu.top/gtvzmijcje.html

JS:   // child_process / cluster 模块
来源：http://hz.zycfv.cn/gtuosiqxrx.html

TS:   // child_process / cluster 模块
来源：http://hz.jlsjyb.cn/gtmxowkahb.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.chenjidiqi.icu/gtsuxmkwkm.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.zhijiandao.cn/gtpmbqlpyk.html

Ruby: // fork 块
来源：http://hz.shzxlz.cn/gtlddjenvk.html

C#:   Parallel.For
来源：http://hz.bjfxy.top/gtjmsoivte.html

================================================================================
来源：http://hz.wangshuangyany.cn/gtnydfrgqr.html

P. 常用工具函数
来源：http://hz.gogol.net.cn/gtxdbsbeas.html

================================================================================
来源：http://hz.hammf.cn/gtkxhxgkte.html

[P01] 生成 UUID
来源：http://hz.gotoacloud.top/gtittdunxd.html

Py:   str(uuid.uuid4())
来源：http://hz.hnqzz.top/gtfxhyoder.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.jyoumei.cn/gtedqqszwg.html

JS:   crypto.randomUUID()
来源：http://hz.fzhhl.top/gtosjltizm.html

TS:   crypto.randomUUID()
来源：http://hz.cdnleiting.top/gtbrenaxay.html

Java: UUID.randomUUID().toString()
来源：http://hz.zhengqikj.top/gtsnjjufac.html

Go:   // 用 github.com/google/uuid
来源：http://hz.aibaodan.cn/gtqcaockxp.html

Ruby: SecureRandom.uuid
来源：http://hz.yuxming.cn/gtvuxqroqm.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.pengpengdd.cyou/gtujsjyfkt.html

[P02] MD5 / SHA256 摘要
来源：http://hz.pycfn.com/gtymfbkdtr.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.yj202588.top/gtpkrrozrx.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.zycfv.cn/gtozofmsul.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.sufxvd.cn/gtspvhtfjj.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.hongshengwenyu.top/gtmramhybg.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.tanke756.top/gtdgaimbbk.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.tian-w.cn/gtshglhuuj.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.zdqjudy.top/gtsqnyxbke.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.quarkkingdee.top/gtspqtejef.html

[P03] 生成短随机字符串
来源：http://hz.yvedp.cn/gtifxvneyd.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.zycfv.cn/gtiabjnugy.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.zhijiandao.cn/gtfaxjvhej.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.aizwys.cn/gtlmtayiju.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.ivvv.top/gtxymiadzm.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.andypj.xyz/gtqzpbwauu.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.chenjidiqi.icu/gtbcknmjto.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.shanyushiyangtech.top/gthmrskluy.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.haohaochexian.top/gttccrurga.html

[P04] 求长度
来源：http://hz.chenzaomai.com/gtxxgkstrr.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.yanxiufei.cn/gtbmepeobd.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.tianlin.xyz/gtrfhflpdh.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.ehwqpu.com/gtgacxqsrl.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.aibaodan.cn/gtwhxpylii.html

Java: list.size();  map.size();  s.length()
来源：http://hz.bjfxy.top/gtfdkwgczj.html

Go:   len(arr);  len(m)
来源：http://hz.ivvv.top/gtvtfycyrk.html

Ruby: x.length;  x.size
来源：http://hz.jinqigufen.top/gtafmptigc.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.nanxinkj.top/gttmzcsrsj.html

[P05] 判断两个对象内容是否相等
来源：http://hz.chenzaomai.com/gtrdndtatt.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.yueranfly.top/gttnpokchz.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.cdnleiting.top/gtbphxnhfy.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.tianlin.xyz/gtgvhoknem.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.0kj1m.cn/gtnzrupklp.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.gzhubu.top/gtrvqmwrjc.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.shuidangran.top/gtqbogakgx.html

Ruby: a == b
来源：http://hz.aizwys.cn/gtojpjzmze.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.cheryme.top/gthyorcamx.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.0kj1m.cn/gtgicingns.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.c1oappe.top/gthftbwobb.html

PHP:  if (empty($x)) {}
来源：http://hz.redwolf501.top/gtxncgoshu.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.nanxuanxn.top/gtldlcelnd.html

TS:   if (x == null) {}
来源：http://hz.zhijiandao.cn/gtepskxsyb.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.dashuyun.cn/gtjhhvaqxn.html

Go:   if x == nil {}
来源：http://hz.guowangkeji.top/gtdpwrandh.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.chenlongwang.top/gtdsodimfy.html

C#:   if (x is null) {}
来源：http://hz.quarkkingdee.top/gthtbwrnbu.html

[P07] 防抖与节流
来源：http://hz.hongshengwenyu.top/gthyhducvr.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.chenlongwang.top/gtjszdwafh.html

PHP:  // 手写时间戳比较
来源：http://hz.fengsongda.top/gttbocdbli.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.xuanzx.com/gtymdzfnsj.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.9152youxi.cn/gtppszqzsu.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.yj202588.top/gteiegareq.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.ppjwa.cn/gtsmjzwcar.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.tian-w.cn/gtouskexke.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.gzhubu.top/gtnwcueein.html

[P08] 处理浮点精度问题
来源：http://hz.shanyushiyangtech.top/gtmdrnvusy.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.shzxlz.cn/gtteuhffax.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.xinyue.icu/gtunflpzkx.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.jlsjyb.cn/gtrvdedgke.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.ydjk.org.cn/gtqionpbwo.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.zycfv.cn/gtbmbuexkm.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.xinyue.icu/gtglltrpfd.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.gogol.net.cn/gtsqlxfaak.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.nanxuanxn.top/gtvkwtfkkb.html

================================================================================
来源：http://hz.wangdashe.top/gtvrqqcdbr.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.ybcxt.top/gtduhuppaq.html

================================================================================
来源：http://hz.hnqzz.top/gttqyvpmoi.html

[Q01] 创建表
来源：http://hz.zdqjudy.top/gtvwrafjor.html

CREATE TABLE users (
来源：http://hz.ydzc1.top/gtgpesfjbk.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.jinqigufen.top/gtetowcyqe.html

name VARCHAR(50) NOT NULL,
来源：http://hz.pengpengdd.cyou/gtxidxgsyn.html

email VARCHAR(100) UNIQUE,
来源：http://hz.bjfxy.top/gtiwuqhgzj.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.hnxiangtu.top/gtsqznmelw.html

);
来源：http://hz.yj202588.top/gtlvijavpq.html

[Q02] 创建带外键的表
来源：http://hz.hnqzz.top/gtovjpmllb.html

CREATE TABLE orders (
来源：http://hz.zhongyouzk.top/gtjxdwtlin.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.birdmap.top/gtllqbtnfy.html

user_id INT NOT NULL,
来源：http://hz.jiagoushi.top/gtmlrqmtnz.html

amount DECIMAL(10, 2),
来源：http://hz.ydjk.org.cn/gtvggowfqv.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.cqqwz.cn/gtinjysrwn.html

);
来源：http://hz.ydzc1.top/gtgfjqljou.html

[Q03] 增加列
来源：http://hz.jlsjyb.cn/gtjegvkxot.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.jqgfzy.top/gtizzsogff.html

[Q04] 修改列类型
来源：http://hz.smart0.xyz/gthqmnrvwc.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.zhixingplan.top/gthrhcbpin.html

[Q05] 重命名列
来源：http://hz.bjfxy.top/gtoffrllsn.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.fengsongda.top/gtkbwstbwq.html

[Q06] 删除列
来源：http://hz.birdmap.top/gtoxtyevct.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.iojbl.cn/gtnjsbfbxo.html

[Q07] 删除表
来源：http://hz.chenjidiqi.icu/gtyflldntq.html

DROP TABLE IF EXISTS orders;
来源：http://hz.jqgfzy.top/gtmcevabkh.html

[Q08] 创建普通索引
来源：http://hz.chenjidiqi.icu/gtukxpxhsq.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.vqdsnc.cn/gtcwdtkqkm.html

[Q09] 创建唯一索引
来源：http://hz.shanyushiyangkeji.top/gtxwavhrzx.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.xinyue.icu/gtpqjijeug.html

[Q10] 插入单行
来源：http://hz.nanxinkj.top/gtdhgbgzgt.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.hongshengwenyu.top/gtzceyocng.html

[Q11] 一次插入多行
来源：http://hz.ppjwa.cn/gtalwnktvl.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.yvedp.cn/gtgzqgdixi.html

[Q12] 插入后取自增 ID
来源：http://hz.jqgufenzy.top/gtwckdemtc.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.zhaomingkeji.xyz/gtehhpyqzs.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.yj202588.top/gttrmqzmzq.html

[Q13] 忽略重复插入
来源：http://hz.tanke756.top/gtlskejrog.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.pengpengdd.cyou/gtjadsbaxu.html

[Q14] 存在则更新（upsert）
来源：http://hz.cdnleiting.top/gtoefryuur.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.hammf.cn/gtbiowadcg.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.zhengqikj.top/gtyblqongf.html

[Q15] 查询全部
来源：http://hz.aibaodan.cn/gtzlpalswr.html

SELECT * FROM users;
来源：http://hz.yj202588.top/gtnogmzmnn.html

[Q16] 查询指定列
来源：http://hz.meibo888.top/gtvntluhdn.html

SELECT id, name FROM users;
来源：http://hz.jiagoushi.top/gtvylxehqa.html

[Q17] 条件查询
来源：http://hz.yangfankeji.com/gtnhfjgotu.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.dianchejie.cn/gtsrxfpess.html

[Q18] 模糊匹配
来源：http://hz.jqgfzy.top/gtcvjzuisy.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.ydzc1.top/gtjarzidij.html

[Q19] 范围查询
来源：http://hz.hnxiangtu.top/gtmyevbtok.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.hnxiangtu.top/gtwidjdeps.html

[Q20] IN 列表
来源：http://hz.fengsongda.top/gtgduzdatp.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.zhiwuduotai.top/gtggjxxdch.html

[Q21] 空值判断
来源：http://hz.yj202588.top/gtzirvwbra.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.tanke756.top/gtgdlcrpwe.html

[Q22] 排序
来源：http://hz.tianlin.xyz/gttogxgnls.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.jinyuanbaomall.cn/gttgzixnmi.html

[Q23] 分页
来源：http://hz.daria6918.cn/gtcmxhbpdt.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.haohaochexian.top/gtbszidoda.html

[Q24] 去重
来源：http://hz.guowangkeji.top/gtlhlrxfeo.html

SELECT DISTINCT city FROM users;
来源：http://hz.yj20258.top/gtclldnlqk.html

[Q25] 只取前 N 条
来源：http://hz.xuanzx.com/gtpcuckgvp.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.pengpengdd.cyou/gtrqebhwue.html

[Q26] 计数
来源：http://hz.jianghu66.top/gtqlihcupn.html

SELECT COUNT(*) FROM users;
来源：http://hz.yj20258.top/gtznclzrvm.html

[Q27] 条件计数
来源：http://hz.gaohongyu789.top/gtpirssqau.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.nwbrower.top/gtrjrogguu.html

[Q28] 求和与平均
来源：http://hz.zhixingplan.top/gtldxnyhnd.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.shzxlz.cn/gttnihyuxz.html

[Q29] 最大最小值
来源：http://hz.c1oappe.top/gtvqjqstiv.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.shzxlz.cn/gtkdiiyaiq.html

[Q30] 分组统计
来源：http://hz.mhx1999.top/gtrhnillal.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.gaohongyu789.top/gtzmtqcmdr.html

[Q31] 分组后过滤
来源：http://hz.zhengqikj.top/gtsehfodqz.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.cdnleiting.top/gtilbiafjw.html

[Q32] 分组拼接字符串
来源：http://hz.wangdashe.top/gtmdifjaqw.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.ivvv.top/gtsxnlawsz.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.haohaochexian.top/gtqlrhcphb.html

[Q33] 多列分组
来源：http://hz.sufxvd.cn/gtwzhashoa.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.jqgufenzy.top/gtkghhwgcd.html

[Q34] 每组取第一条
来源：http://hz.yvedp.cn/gtlwmvzblx.html

SELECT * FROM (
来源：http://hz.guannengcc.top/gtrqurbkgr.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.hnqzz.top/gtusszolvd.html

) t WHERE rn = 1;
来源：http://hz.havefunace.top/gticuhnamj.html

[Q35] 内连接
来源：http://hz.guowangkeji.top/gtcuulcvod.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.gotoacloud.top/gtzjlkrkzu.html

[Q36] 左连接
来源：http://hz.sufxvd.cn/gtbjcwwhae.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.aizwys.cn/gtwvcsrmbc.html

[Q37] 右连接
来源：http://hz.zhongyouzk.top/gtzmvzlvdw.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.jlsjyb.cn/gtgjofrmri.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.redwolf501.top/gtcddsiatp.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.jqgufenzy.top/gtgtnrqjlr.html

[Q39] 自连接（查上下级）
来源：http://hz.smart0.xyz/gtdjwxfqvx.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.dashuyun.cn/gtyhhyvehg.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.nwbrower.top/gtbidqaglh.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.316326.xyz/gtcamvvrvs.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.sweek.top/gtoxkdghjf.html

[Q41] 多表连接
来源：http://hz.zhongyouzk.top/gttedwwlpu.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.havefunace.top/gtbsqoofng.html

JOIN users u ON u.id = o.user_id
来源：http://hz.jiagoushi.top/gtakgkjoha.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.nanxinkj.top/gttfxvmhha.html

[Q42] 连接条件附加过滤
来源：http://hz.xuetiantiany.cn/gtjoqczswl.html

SELECT u.name, o.amount FROM users u
来源：http://hz.zhengqikj.top/gtzhhigecu.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.jqgfzy.top/gtvjclzrbc.html

[Q43] 标量子查询
来源：http://hz.sysykeji.top/gtkbhvvtwd.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.wangshuangyany.cn/gtxwgaempm.html

[Q44] IN 子查询
来源：http://hz.redwolf501.top/gtellhicki.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.aibaodan.cn/gtfjoxpcsz.html

[Q45] EXISTS 判断存在
来源：http://hz.nanxuanxn.top/gtmptvayqf.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.jinghuilouyu.cn/gtbsbbhsgd.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.yj20258888.top/gtyafjniuu.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.aibaodan.cn/gttwfjkwww.html

[Q47] 与平均值比较
来源：http://hz.meibo888.top/gtthrsogwu.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.ehwqpu.com/gtqealsrgj.html

[Q48] CTE 公用表表达式
来源：http://hz.pycfn.com/gtnijratvx.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.jiagoushi.top/gtdhjvupat.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.316326.xyz/gtpvjcjmdg.html

[Q49] 更新单行
来源：http://hz.quarkkingdee.top/gtlxeopmtf.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.cqqwz.cn/gtqprsfkux.html

[Q50] 批量更新
来源：http://hz.yvedp.cn/gtiaghrwbj.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.chenjidiqi.icu/gtyvbdojtl.html

[Q51] 用子查询更新
来源：http://hz.jlsjyb.cn/gtmgpinnnn.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.xuetiantiany.cn/gttnkslvbz.html

[Q52] 删除指定行
来源：http://hz.jyoumei.cn/gtfhacdqpd.html

DELETE FROM users WHERE id = 10;
来源：http://hz.xuanzx.com/gtbxqcakmr.html

[Q53] 按条件删除
来源：http://hz.bjfxy.top/gtgckoklog.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.zhongyouzk.top/gtotdvjstp.html

[Q54] 清空表
来源：http://hz.hysaishi.cn/gtvrosgqxf.html

TRUNCATE TABLE logs;
来源：http://hz.redwolf501.top/gtvzsjwhlk.html

[Q55] 排名（并列占位）
来源：http://hz.sufxvd.cn/gtrpvpkwfr.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.iojbl.cn/gtykwkvzdm.html

[Q56] 密集排名（并列不占位）
来源：http://hz.birdmap.top/gtmigxuxbp.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.shzxlz.cn/gtbpevztsz.html

[Q57] 行号
来源：http://hz.svipenyu.cn/gtkfosulmv.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.xinyue.icu/gtwbqxvigy.html

[Q58] 累计求和
来源：http://hz.pengpengdd.cyou/gtqvtxpklf.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.ivvv.top/gtofityyba.html

[Q59] 分组内累计
来源：http://hz.shangyingyoupin.top/gtufuuwxhw.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.hnxiangtu.top/gtlazvufob.html

[Q60] 取上一行 / 下一行
来源：http://hz.hammf.cn/gtsgjggqtk.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.wangshuangyany.cn/gtorpzfdof.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.hnqzz.top/gtjryaffus.html


<!-- 参考信息 -->