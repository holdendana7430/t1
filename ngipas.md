代发 wailian999

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.sxryk.cn/gthkqkcwsc.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.zhoulong.xyz/gtwzyoxlyw.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.jinqigfzy.top/gtrxnodyia.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.jqgfzy.top/gtgevhtjem.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.wangdashe.top/gtanprwemx.html

[N10] 链表节点定义
来源：http://hz.havefunace.top/gtjmwnufvm.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.shanyushiyangtech.top/gthrrxffpk.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.dashuyun.cn/gthtabrowg.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.andypj.xyz/gteyebahmi.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.birdmap.top/gtrrdvmhky.html

Java: class Node { int v; Node next; }
来源：http://hz.chenlongwang.top/gtjmfmkran.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.iojbl.cn/gtznipohen.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.wangshuangyany.cn/gtsehmfaol.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.yj20258888.top/gtamiofjgb.html

[N11] 二叉树中序遍历
来源：http://hz.zhaomingkeji.xyz/gtbdgpcaex.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.yonumen.top/gtopcwqryv.html

PHP:  // 手写递归函数
来源：http://hz.bjfxy.top/gtfndqmtvw.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.hongshengwenyu.top/gtutfjvzlv.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.yongpay.top/gtuwjrbark.html

Java: // 手写递归
来源：http://hz.yj202588.top/gtreidzjsw.html

Go:   // 手写递归
来源：http://hz.nanxinkj.top/gtlukzttft.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.jyoumei.cn/gtjzayciis.html

C#:   // 手写递归
来源：http://hz.nanxuanxn.top/gtffhfeyhw.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.yj20258888.top/gtjqhazbmt.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.chenjidiqi.icu/gtdjqsyvit.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.jqgfzy.top/gtvldraadu.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.ydjk.org.cn/gtmfrmwejk.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.hywenlv.cn/gtjjcmzqlq.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.xuanzx.com/gtwzgbosel.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.wangshuangyany.cn/gtmhxzfyth.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.redwolf501.top/gtiidviqba.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.hysaishi.cn/gtdpmeagqh.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtrhqwjube.html

O. 并发与异步
来源：http://hz.quarkkingdee.top/gtgvyvzwbo.html

================================================================================
来源：http://hz.fengsongda.top/gtbpczaoea.html

[O01] 启动一个线程
来源：http://hz.ydzc1.top/gtnwqrmzlt.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.yvedp.cn/gtoswrpzrm.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.guannengcc.top/gtbcamflfv.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.yj20258888.top/gtielsxwmq.html

TS:   // 同 JS
来源：http://hz.yanxiufei.cn/gtukcogcia.html

Java: new Thread(() -> f()).start()
来源：http://hz.ydzc1.top/gtbdciymgi.html

Go:   go f()
来源：http://hz.nanxinkj.top/gtuadyhrfh.html

Ruby: Thread.new { f }
来源：http://hz.sxryk.cn/gtzwprahdy.html

C#:   Task.Run(() => F());
来源：http://hz.hnqzz.top/gtwmurqsvs.html

[O02] 使用线程池
来源：http://hz.cqqwz.cn/gtkosxqhhb.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.shanyushiyangtech.top/gtloatpcjl.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.zycfv.cn/gtuhyflhod.html

JS:   // worker_threads 线程池
来源：http://hz.shanyushiyangkeji.top/gtwijziucq.html

TS:   // worker_threads 线程池
来源：http://hz.yangfankeji.com/gtoquaxudn.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.xinyue.icu/gtkktxfsfe.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.shanyushiyangtech.top/gtqvvzmcdt.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.bjfxy.top/gtlzexdvom.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.wangshuangyany.cn/gtyyklcmqs.html

[O03] 加锁保护共享数据
来源：http://hz.tianlin.xyz/gthglolloj.html

Py:   with lock: shared += 1
来源：http://hz.yj20258888.top/gtlhusfmai.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.gaohongyu789.top/gtdjxpkbaa.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.shanyushiyangkeji.top/gtwsfrsyqa.html

TS:   // 同 JS
来源：http://hz.ywan-chungtsiang.top/gtigwsvcdx.html

Java: synchronized (this) { shared++; }
来源：http://hz.pengpengdd.cyou/gtklugrvkk.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.xuanzx.com/gtxnjlhmxj.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.xuanzx.com/gtmymbysgo.html

C#:   lock (gate) { shared++; }
来源：http://hz.yonumen.top/gtpfmszzhp.html

[O04] 定义异步函数并等待
来源：http://hz.zhengqikj.top/gttxkpxojv.html

Py:   async def f():⏎    await g()
来源：http://hz.zycfv.cn/gtiaghetff.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.cheryme.top/gtrmgmxwia.html

JS:   async function f() { await g(); }
来源：http://hz.gogol.net.cn/gtwzzwcouw.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.jyoumei.cn/gtbauobkte.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.jqgfzy.top/gtpmhjwmbl.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.fengsongda.top/gttdmvwqyw.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.wangdashe.top/gtcyhtguhv.html

C#:   async Task F() { await G(); }
来源：http://hz.aibaodan.cn/gtceyuaupr.html

[O05] 并发执行并等待全部完成
来源：http://hz.vqdsnc.cn/gtswtnrnww.html

Py:   asyncio.gather(*tasks)
来源：http://hz.hnqzz.top/gtybldyfci.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.nwbrower.top/gtmkrqeygz.html

JS:   await Promise.all(tasks)
来源：http://hz.chenlongwang.top/gtuucrgxhd.html

TS:   await Promise.all(tasks)
来源：http://hz.wangdashe.top/gtbbuziavp.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.ehwqpu.com/gtonvndzff.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.c1oappe.top/gtmtbliljj.html

Ruby: threads.map(&:join)
来源：http://hz.zhijiandao.cn/gtkipuizwj.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.cheryme.top/gtojmphngz.html

[O06] 使用进程池
来源：http://hz.daxiang520.top/gtqdmnxnex.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.daxiang520.top/gtcqcazqkn.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.tanke756.top/gtqlinxfil.html

JS:   // child_process / cluster 模块
来源：http://hz.tianlin.xyz/gtgqzcyfwx.html

TS:   // child_process / cluster 模块
来源：http://hz.yueranfly.top/gtnqvjlzpp.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.cdnleiting.top/gtkkvswknh.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.sufxvd.cn/gtkfpfydlk.html

Ruby: // fork 块
来源：http://hz.cqqwz.cn/gtpgbfnowi.html

C#:   Parallel.For
来源：http://hz.nwbrower.top/gtxqehqtpu.html

================================================================================
来源：http://hz.zdqjudy.top/gtwdgmrcfn.html

P. 常用工具函数
来源：http://hz.tianlin.xyz/gtawcvvqvv.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtpldidbyt.html

[P01] 生成 UUID
来源：http://hz.hnxiangtu.top/gtyxqfogvb.html

Py:   str(uuid.uuid4())
来源：http://hz.xingfuxueyuan.xyz/gtswdkihrt.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.mhx1999.top/gtxezebcdm.html

JS:   crypto.randomUUID()
来源：http://hz.cucudq.cn/gtzkpmdeax.html

TS:   crypto.randomUUID()
来源：http://hz.xuanzx.com/gtdlasrqzf.html

Java: UUID.randomUUID().toString()
来源：http://hz.sufxvd.cn/gtzqqwqtzk.html

Go:   // 用 github.com/google/uuid
来源：http://hz.yj202588.top/gtodarqorz.html

Ruby: SecureRandom.uuid
来源：http://hz.yvedp.cn/gtsutolroy.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.0kj1m.cn/gtjrwwoqyb.html

[P02] MD5 / SHA256 摘要
来源：http://hz.hywenlv.cn/gtqmjaxhro.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.sxryk.cn/gtfyzeupxa.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.jinqigfzy.top/gtmqtpwczg.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.ppjwa.cn/gtyphtommg.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.guannengcc.top/gtmwqpfffe.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.shangyingyoupin.top/gtsykqktlf.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.shangyingyoupin.top/gtmsjqzgyu.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.yj202588.top/gtvyxcvmmk.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.aibaodan.cn/gtfnimbhua.html

[P03] 生成短随机字符串
来源：http://hz.hongshengwenyu.top/gtrjdylibn.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.chenlongwang.top/gtfgxsmlxu.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.yanxiufei.cn/gtkpnrvsal.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.cdnleiting.top/gtofadeimb.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.yvedp.cn/gtnelrctan.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.316326.xyz/gtcbcilhhl.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.aibaodan.cn/gticyqxuwl.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.sxryk.cn/gtqovggfvf.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.9152youxi.cn/gtlfimoaar.html

[P04] 求长度
来源：http://hz.pengpengdd.cyou/gtyfjykjkz.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.haohaochexian.top/gttfidfkpm.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.cheryme.top/gtftwxotns.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.jlsjyb.cn/gtyvhpoqyg.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.zhongyouzk.top/gttkyahwgv.html

Java: list.size();  map.size();  s.length()
来源：http://hz.daria6918.cn/gtoactqaoy.html

Go:   len(arr);  len(m)
来源：http://hz.birdmap.top/gtcugwcneh.html

Ruby: x.length;  x.size
来源：http://hz.sxryk.cn/gtdrfsebsk.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.52xcode.cn/gtwewzhsnn.html

[P05] 判断两个对象内容是否相等
来源：http://hz.gzhubu.top/gtsoqxvvhg.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.cucudq.cn/gtswbvvini.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.dianchejie.cn/gtvaznugzd.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.zhijiandao.cn/gtmmgpoiyc.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.svipenyu.cn/gtnvawfzzc.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.cashguo.top/gthzwdkhsy.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.pycfn.com/gthcsudaxe.html

Ruby: a == b
来源：http://hz.hnxiangtu.top/gtviecqttg.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.dashuyun.cn/gtafevynht.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.yj20258888.top/gtloibeclf.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.zhengqikj.top/gtmzwqrcii.html

PHP:  if (empty($x)) {}
来源：http://hz.jinqigufen.top/gtenwenbwt.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.ehwqpu.com/gtqcenvlgu.html

TS:   if (x == null) {}
来源：http://hz.ivvv.top/gtlllikenc.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.0kj1m.cn/gtcwpjmimm.html

Go:   if x == nil {}
来源：http://hz.guowangkeji.top/gtyfqyijzn.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.jqgfzy.top/gtltqnkxjk.html

C#:   if (x is null) {}
来源：http://hz.ppjwa.cn/gtvxkreazc.html

[P07] 防抖与节流
来源：http://hz.jiagoushi.top/gtgrnkwgyx.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.gaohongyu789.top/gtsrijinqj.html

PHP:  // 手写时间戳比较
来源：http://hz.jqgfzy.top/gtwhhauobl.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.ivvv.top/gthyumqqgn.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.yueranfly.top/gtgjiltsui.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.yangfankeji.com/gtjntfgqki.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.zhaomingkeji.xyz/gtcafajxpy.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.iojbl.cn/gthyrcildu.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.guowangkeji.top/gtdpicoxab.html

[P08] 处理浮点精度问题
来源：http://hz.zhengqikj.top/gtlfocinmd.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.ydjk.org.cn/gtcoqwpras.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.meibo888.top/gtthkqzrxd.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.gzhubu.top/gtrvhdjnnq.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.tianlin.xyz/gtfdfefhoi.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.jqgfzy.top/gtmhajqndx.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.fengsongda.top/gtrqbsdzxd.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.chenjidiqi.icu/gtrrbybnfa.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.c1oappe.top/gtblpdbqdu.html

================================================================================
来源：http://hz.kuanghao11.cn/gtpzokkwws.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.dashuyun.cn/gtrtqzywtf.html

================================================================================
来源：http://hz.xylfe.cn/gtmrcfbfrs.html

[Q01] 创建表
来源：http://hz.dashuyun.cn/gtcbywwwvp.html

CREATE TABLE users (
来源：http://hz.gotoacloud.top/gtjpvdzybl.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.jqgufenzy.top/gthnnzupwh.html

name VARCHAR(50) NOT NULL,
来源：http://hz.yj202588.top/gtadyxmziq.html

email VARCHAR(100) UNIQUE,
来源：http://hz.cashguo.top/gteqycfelh.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.gogol.net.cn/gtqgikrtpw.html

);
来源：http://hz.yangfankeji.com/gtlqllrikl.html

[Q02] 创建带外键的表
来源：http://hz.iojbl.cn/gtgwjfytht.html

CREATE TABLE orders (
来源：http://hz.sweek.top/gtvjmzixgw.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.tianlin.xyz/gtjlgazkuz.html

user_id INT NOT NULL,
来源：http://hz.zdqjudy.top/gtbwhvctjf.html

amount DECIMAL(10, 2),
来源：http://hz.snrcjt.cn/gtmwbyiuse.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.yj20258.top/gtlmdrvdlb.html

);
来源：http://hz.gzhubu.top/gtrcvpibnw.html

[Q03] 增加列
来源：http://hz.9152youxi.cn/gtrgqoppcf.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.pycfn.com/gtpqmuckpr.html

[Q04] 修改列类型
来源：http://hz.zhoulong.xyz/gtauurbowe.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.fengsongda.top/gtnfywkmer.html

[Q05] 重命名列
来源：http://hz.sxryk.cn/gteymlbgeg.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.hywenlv.cn/gtspzxbhar.html

[Q06] 删除列
来源：http://hz.jyoumei.cn/gthbsonhlt.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.shuidangran.top/gtluzennbh.html

[Q07] 删除表
来源：http://hz.gogol.net.cn/gtthfxjkzw.html

DROP TABLE IF EXISTS orders;
来源：http://hz.xingfuxueyuan.xyz/gtydloqney.html

[Q08] 创建普通索引
来源：http://hz.fzhhl.top/gthqvduuxc.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.316326.xyz/gtzxzseotd.html

[Q09] 创建唯一索引
来源：http://hz.jinghuilouyu.cn/gtxpucqnmj.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.cqqwz.cn/gttcnqsnaj.html

[Q10] 插入单行
来源：http://hz.smart0.xyz/gtboopsflp.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.tianlin.xyz/gtfmcpjbzd.html

[Q11] 一次插入多行
来源：http://hz.yuanzhike.top/gthnkitkit.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.zhengqikj.top/gtqilwexdb.html

[Q12] 插入后取自增 ID
来源：http://hz.ehwqpu.com/gtsfqdissu.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.gogol.net.cn/gtcrgslnbk.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.jinqigufen.top/gtdfsbictz.html

[Q13] 忽略重复插入
来源：http://hz.fengsongda.top/gtveebipnh.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.pengpengdd.cyou/gtqoocccgd.html

[Q14] 存在则更新（upsert）
来源：http://hz.cheryme.top/gtbclgzytn.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.shuidangran.top/gtlmcujize.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.chenjidiqi.icu/gtnbgfjcup.html

[Q15] 查询全部
来源：http://hz.cashguo.top/gtcxfzadru.html

SELECT * FROM users;
来源：http://hz.jqgfzy.top/gtegljtkex.html

[Q16] 查询指定列
来源：http://hz.yanxiufei.cn/gtzametstk.html

SELECT id, name FROM users;
来源：http://hz.hnxiangtu.top/gtpxucziri.html

[Q17] 条件查询
来源：http://hz.jqgfzy.top/gthkzyevwz.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.zhaomingkeji.xyz/gtmggowlwv.html

[Q18] 模糊匹配
来源：http://hz.gogol.net.cn/gtpraodwpn.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.zdqjudy.top/gtbwcwrpuw.html

[Q19] 范围查询
来源：http://hz.zhoulong.xyz/gtpqocodgy.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.yanxiufei.cn/gtybcbyuis.html

[Q20] IN 列表
来源：http://hz.jinghuilouyu.cn/gtnvyuxwmi.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.guowangkeji.top/gtpcmfvqeq.html

[Q21] 空值判断
来源：http://hz.guannengcc.top/gtpfpexssp.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.cdnleiting.top/gtgpeiwyij.html

[Q22] 排序
来源：http://hz.ivvv.top/gtqpqtexdu.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.jqgfzy.top/gtdyjtdkir.html

[Q23] 分页
来源：http://hz.jinyuanbaomall.cn/gtxyswpuld.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.cqqwz.cn/gtlkzuaiyp.html

[Q24] 去重
来源：http://hz.hnqzz.top/gtczogquzl.html

SELECT DISTINCT city FROM users;
来源：http://hz.0kj1m.cn/gtqiovrizb.html

[Q25] 只取前 N 条
来源：http://hz.quarkkingdee.top/gtdpkfcaay.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.yvedp.cn/gtnvcedidz.html

[Q26] 计数
来源：http://hz.wangshuangyany.cn/gtrjpwvaob.html

SELECT COUNT(*) FROM users;
来源：http://hz.xziqi.cn/gtiadjtnjk.html

[Q27] 条件计数
来源：http://hz.quarkkingdee.top/gtfmjyyrcr.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.wangshuangyany.cn/gthfcpglna.html

[Q28] 求和与平均
来源：http://hz.hywenlv.cn/gtkbnqehdq.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.zhaomingkeji.xyz/gtlcvymzwk.html

[Q29] 最大最小值
来源：http://hz.snrcjt.cn/gtxkbyjqpg.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.wangdashe.top/gtuvwgyafg.html

[Q30] 分组统计
来源：http://hz.zhoulong.xyz/gtlhqfmgwj.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.hfpthk.cn/gtqablzlxs.html

[Q31] 分组后过滤
来源：http://hz.yj20258.top/gtcvhjllfg.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.dianchejie.cn/gtrmhbggvo.html

[Q32] 分组拼接字符串
来源：http://hz.jlsjyb.cn/gtfauatsey.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.jinghuilouyu.cn/gtdrdwdvyf.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.gotoacloud.top/gtbgceyzbm.html

[Q33] 多列分组
来源：http://hz.zdqjudy.top/gtgxetdnnq.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.ydzc1.top/gtzenbdupf.html

[Q34] 每组取第一条
来源：http://hz.chenlongwang.top/gtfaadjesx.html

SELECT * FROM (
来源：http://hz.hnxiangtu.top/gtqkukxmeo.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.xinyue.icu/gtgvvjczzm.html

) t WHERE rn = 1;
来源：http://hz.aizwys.cn/gtfutlruuk.html

[Q35] 内连接
来源：http://hz.yueranfly.top/gtobjveozy.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.cdnleiting.top/gtptgziseb.html

[Q36] 左连接
来源：http://hz.jinyuanbaomall.cn/gtxcwmcppw.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.quarkkingdee.top/gtraiznbok.html

[Q37] 右连接
来源：http://hz.xziqi.cn/gtngywsmmv.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.aizwys.cn/gtzvghryif.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.hysaishi.cn/gtnqpiqqta.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.quarkkingdee.top/gtkyjefztr.html

[Q39] 自连接（查上下级）
来源：http://hz.svipenyu.cn/gtuevdimza.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.c1oappe.top/gtxfieyarl.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.snrcjt.cn/gtklmawlma.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.sweek.top/gtkzeffrrh.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.andypj.xyz/gtvemomeas.html

[Q41] 多表连接
来源：http://hz.shanyushiyangtech.top/gtqqpihfhx.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.andypj.xyz/gtyakfrkjm.html

JOIN users u ON u.id = o.user_id
来源：http://hz.quarkkingdee.top/gtdntjjjbm.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.xylfe.cn/gtlxefmbzu.html

[Q42] 连接条件附加过滤
来源：http://hz.xylfe.cn/gtpqlqabqc.html

SELECT u.name, o.amount FROM users u
来源：http://hz.shuidangran.top/gtzfoyrvvw.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.havefunace.top/gtbvffmtzi.html

[Q43] 标量子查询
来源：http://hz.sweek.top/gtjrdlelpy.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.svipenyu.cn/gtyugixldj.html

[Q44] IN 子查询
来源：http://hz.tian-w.cn/gtzsawijnc.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.jinyuanbaomall.cn/gtugcydmkp.html

[Q45] EXISTS 判断存在
来源：http://hz.redwolf501.top/gtxbjukipa.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.zhijiandao.cn/gthnqmaqvw.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.yj20258.top/gttatuejon.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.jyoumei.cn/gtgafvahvg.html

[Q47] 与平均值比较
来源：http://hz.xuetiantiany.cn/gttfdnevub.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.xingfuxueyuan.xyz/gtngffgiil.html

[Q48] CTE 公用表表达式
来源：http://hz.jianghu66.top/gthuhjnrho.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.kuanghao11.cn/gtziuxbuxk.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.yonumen.top/gtvmhizkcy.html

[Q49] 更新单行
来源：http://hz.zdqjudy.top/gtlmmzvzyg.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.svipenyu.cn/gtaftaaiks.html

[Q50] 批量更新
来源：http://hz.zhoulong.xyz/gtbllzztnx.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.kuanghao11.cn/gtevhrnjlk.html

[Q51] 用子查询更新
来源：http://hz.wangshuangyany.cn/gtixxhhfkj.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.chenzaomai.com/gtexfkyoub.html

[Q52] 删除指定行
来源：http://hz.yongpay.top/gtycrewqkf.html

DELETE FROM users WHERE id = 10;
来源：http://hz.redwolf501.top/gtveebdgqt.html

[Q53] 按条件删除
来源：http://hz.cheryme.top/gtcfnbyzir.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.havefunace.top/gtvnbztpiv.html

[Q54] 清空表
来源：http://hz.nanxuanxn.top/gtvarkimhg.html

TRUNCATE TABLE logs;
来源：http://hz.yj202588.top/gtqxpwnewj.html

[Q55] 排名（并列占位）
来源：http://hz.yuxming.cn/gthkeewffq.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.jinyuanbaomall.cn/gtkpprapfd.html

[Q56] 密集排名（并列不占位）
来源：http://hz.cqqwz.cn/gtiobhfond.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.ybcxt.top/gtihkdnpqg.html

[Q57] 行号
来源：http://hz.shanyushiyangtech.top/gtjnugnsqm.html


<!-- 参考信息 -->