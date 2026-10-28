代发 wailian999

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.ydzc1.top/gtchzepydy.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.cheryme.top/gtcrvsmekj.html

Java: class Node { int v; Node next; }
来源：http://hz.jyoumei.cn/gtjmgapuza.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.pycfn.com/gtyawlvntt.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.52xcode.cn/gttsfbqjll.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.shuidangran.top/gtgqjhhcaa.html

[N11] 二叉树中序遍历
来源：http://hz.0kj1m.cn/gtjzsaohud.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.yonumen.top/gtypspsxht.html

PHP:  // 手写递归函数
来源：http://hz.ehwqpu.com/gtigfqfmwo.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.mhx1999.top/gtxsezzxvi.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.tian-w.cn/gtumwsvzrx.html

Java: // 手写递归
来源：http://hz.yuanzhike.top/gtnosqyxrr.html

Go:   // 手写递归
来源：http://hz.gotoacloud.top/gtljeanfut.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.zhaomingkeji.xyz/gtowojmonq.html

C#:   // 手写递归
来源：http://hz.feifeiyinyue.top/gtfptgviis.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.hongshengwenyu.top/gtdahgbthn.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.cdnleiting.top/gtxjrsqzzw.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.dashuyun.cn/gtrtgpttfb.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.jqgfzy.top/gtiqnnzipb.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.zhaomingkeji.xyz/gtzpbrxcba.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.zhaomingkeji.xyz/gtbnglcsgl.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.yonumen.top/gtvgdsiotm.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.sweek.top/gtcfbetcft.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.sysykeji.top/gtfeioxrtv.html

================================================================================
来源：http://hz.316326.xyz/gtfethnvaj.html

O. 并发与异步
来源：http://hz.vqdsnc.cn/gtkhrfsnii.html

================================================================================
来源：http://hz.jqgufenzy.top/gtbxwgadwc.html

[O01] 启动一个线程
来源：http://hz.xinyue.icu/gtakzelndt.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.cucudq.cn/gtwiznawff.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.svipenyu.cn/gtlbwelytn.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.jinqigufen.top/gtmwqgjwug.html

TS:   // 同 JS
来源：http://hz.svipenyu.cn/gtyqivutzu.html

Java: new Thread(() -> f()).start()
来源：http://hz.hysaishi.cn/gtuwbcaggy.html

Go:   go f()
来源：http://hz.jianghu66.top/gtkhxaqmlz.html

Ruby: Thread.new { f }
来源：http://hz.ywan-chungtsiang.top/gtqwudfdnl.html

C#:   Task.Run(() => F());
来源：http://hz.nwbrower.top/gtisjpzwbs.html

[O02] 使用线程池
来源：http://hz.cheryme.top/gtlypljtet.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.sweek.top/gtpgpghksw.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.chenjidiqi.icu/gtlpohltvd.html

JS:   // worker_threads 线程池
来源：http://hz.cqqwz.cn/gtpvglbmgx.html

TS:   // worker_threads 线程池
来源：http://hz.jinqigufen.top/gtgijmaeot.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.yongpay.top/gtmuavrffv.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.jinghuilouyu.cn/gtdnmgglia.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.tanke756.top/gtjcakjpuw.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.meibo888.top/gtrgefldah.html

[O03] 加锁保护共享数据
来源：http://hz.chenzaomai.com/gtxceonpuq.html

Py:   with lock: shared += 1
来源：http://hz.hywenlv.cn/gtnnyxmthp.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.zycfv.cn/gtjuriyvqb.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.pengpengdd.cyou/gtisdnizju.html

TS:   // 同 JS
来源：http://hz.cdnleiting.top/gtqlydpofo.html

Java: synchronized (this) { shared++; }
来源：http://hz.dianchejie.cn/gtwarsasgx.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.ehwqpu.com/gtfhhxpsik.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.fzhhl.top/gtzqfurtxs.html

C#:   lock (gate) { shared++; }
来源：http://hz.ywan-chungtsiang.top/gtyfxxtwqw.html

[O04] 定义异步函数并等待
来源：http://hz.yonumen.top/gtccistcsw.html

Py:   async def f():⏎    await g()
来源：http://hz.zhiwuduotai.top/gttrmdgiaj.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.quarkkingdee.top/gtprxjeong.html

JS:   async function f() { await g(); }
来源：http://hz.xylfe.cn/gtmlrihhif.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.chenjidiqi.icu/gtfvhqnreh.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.cashguo.top/gtkzkpfnfu.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.shanyushiyangkeji.top/gtibeszgzx.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.xingfuxueyuan.xyz/gtdlwqvdbt.html

C#:   async Task F() { await G(); }
来源：http://hz.jinghuilouyu.cn/gtzmwkqoeh.html

[O05] 并发执行并等待全部完成
来源：http://hz.smart0.xyz/gtcvtsqklq.html

Py:   asyncio.gather(*tasks)
来源：http://hz.hysaishi.cn/gtidfjtoqo.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.yanxiufei.cn/gtbseochgi.html

JS:   await Promise.all(tasks)
来源：http://hz.9152youxi.cn/gtdzcmtbtu.html

TS:   await Promise.all(tasks)
来源：http://hz.dashuyun.cn/gturfqnadl.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.guannengcc.top/gtrimguqor.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.redwolf501.top/gtwwfpqdrb.html

Ruby: threads.map(&:join)
来源：http://hz.yanxiufei.cn/gtcftmfukq.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.jyoumei.cn/gtygeyssme.html

[O06] 使用进程池
来源：http://hz.nanxinkj.top/gtrelbyutn.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.cqqwz.cn/gtzlnwogah.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.9152youxi.cn/gtxqqlqhir.html

JS:   // child_process / cluster 模块
来源：http://hz.zhixingplan.top/gtuuzrvgzp.html

TS:   // child_process / cluster 模块
来源：http://hz.xuetiantiany.cn/gttnavyuun.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.jiagoushi.top/gtnmmhyvwb.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.chenlongwang.top/gtwugbnksj.html

Ruby: // fork 块
来源：http://hz.quarkkingdee.top/gtmiygandc.html

C#:   Parallel.For
来源：http://hz.jqgufenzy.top/gtotimdnwk.html

================================================================================
来源：http://hz.cucudq.cn/gtcdwuhtmw.html

P. 常用工具函数
来源：http://hz.iojbl.cn/gtsxuvldqn.html

================================================================================
来源：http://hz.tian-w.cn/gtmzgqaypr.html

[P01] 生成 UUID
来源：http://hz.nanxinkj.top/gtzaiszovy.html

Py:   str(uuid.uuid4())
来源：http://hz.andypj.xyz/gtmpvjhglb.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.nanxuanxn.top/gtglbduepx.html

JS:   crypto.randomUUID()
来源：http://hz.zhengqikj.top/gtygxgmgme.html

TS:   crypto.randomUUID()
来源：http://hz.cucudq.cn/gtobjxdcpz.html

Java: UUID.randomUUID().toString()
来源：http://hz.yvedp.cn/gtugexghzi.html

Go:   // 用 github.com/google/uuid
来源：http://hz.hnxiangtu.top/gtzqynvvox.html

Ruby: SecureRandom.uuid
来源：http://hz.jqgfzy.top/gtubvxnawu.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.zhiwuduotai.top/gthjxnwscf.html

[P02] MD5 / SHA256 摘要
来源：http://hz.zhoulong.xyz/gtwkchlbps.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.xuetiantiany.cn/gtpyndapqr.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.zhongyouzk.top/gtjdnyhddk.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.daxiang520.top/gtnfmmbzif.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.ydzc1.top/gtrfkehpaq.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.gzhubu.top/gtfomjoarn.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.xylfe.cn/gthkgrvdhm.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.ppjwa.cn/gtrmrogqhi.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.hongshengwenyu.top/gtpukvkrgp.html

[P03] 生成短随机字符串
来源：http://hz.tanke756.top/gtktizobga.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.ywan-chungtsiang.top/gtofvidjcg.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.wangshuangyany.cn/gtnokhowhq.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.zhijiandao.cn/gtkvfprlaf.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.shanyushiyangkeji.top/gtajimhnld.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.hnxiangtu.top/gtqbdaqwrg.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.hammf.cn/gtwmcspqkc.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.kuanghao11.cn/gtefrntudn.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.yangfankeji.com/gtwpksimfg.html

[P04] 求长度
来源：http://hz.yj20258.top/gtktfzxtlj.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.jqgfzy.top/gtetfbswtg.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.vqdsnc.cn/gtarrodgcs.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.ydzc1.top/gtonbnulyn.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.chenlongwang.top/gtnoyvnkoa.html

Java: list.size();  map.size();  s.length()
来源：http://hz.gogol.net.cn/gtmtgejbci.html

Go:   len(arr);  len(m)
来源：http://hz.0kj1m.cn/gtumoxwdhp.html

Ruby: x.length;  x.size
来源：http://hz.hywenlv.cn/gtziekhijk.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.yanxiufei.cn/gtcafqnnco.html

[P05] 判断两个对象内容是否相等
来源：http://hz.xuetiantiany.cn/gtvpsaowin.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.tanke756.top/gtszlwrrvz.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.gotoacloud.top/gtyodrwura.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.redwolf501.top/gttnuxkvyb.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.hnxiangtu.top/gticageiuw.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.jianghu66.top/gtljgbgcmw.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.chenzaomai.com/gtcutwpoej.html

Ruby: a == b
来源：http://hz.jinqigufen.top/gtsfmnabae.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.svipenyu.cn/gtosayfoeq.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.shangyingyoupin.top/gtzyjpercj.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.aizwys.cn/gtykpjmcqf.html

PHP:  if (empty($x)) {}
来源：http://hz.hongshengwenyu.top/gthuiovgzn.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.quarkkingdee.top/gtsshcqlrk.html

TS:   if (x == null) {}
来源：http://hz.aizwys.cn/gtavmgbaiq.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.hnqzz.top/gtjpwzjjbe.html

Go:   if x == nil {}
来源：http://hz.ywan-chungtsiang.top/gtyagdubhf.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.svipenyu.cn/gtqpiygkef.html

C#:   if (x is null) {}
来源：http://hz.yonumen.top/gtxaiebrns.html

[P07] 防抖与节流
来源：http://hz.yj20258.top/gtoidtdxns.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.yonumen.top/gtncopqdjp.html

PHP:  // 手写时间戳比较
来源：http://hz.zhixingplan.top/gtoekdpybz.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.xuetiantiany.cn/gthcndiqye.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.quarkkingdee.top/gtrosbhpse.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.hywenlv.cn/gtknvvptpp.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.c1oappe.top/gtcnutsoyf.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.iojbl.cn/gtzsunnhui.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.sufxvd.cn/gtbrwobyqo.html

[P08] 处理浮点精度问题
来源：http://hz.9152youxi.cn/gtwqdkqhzo.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.cdnleiting.top/gtonamaivd.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.gotoacloud.top/gtibiredap.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.yj20258.top/gtwvotgxcd.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.havefunace.top/gtlkfcgwvu.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.yuxming.cn/gtxyknfeqm.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.bjfxy.top/gtsykyxpbu.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.chenzaomai.com/gtidsbvfsm.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.yongpay.top/gtqyvxndkz.html

================================================================================
来源：http://hz.ydjk.org.cn/gtlqcewgkl.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.wangshuangyany.cn/gtxpoxcygy.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gtfmabpisu.html

[Q01] 创建表
来源：http://hz.ydjk.org.cn/gtdkbhewej.html

CREATE TABLE users (
来源：http://hz.daxiang520.top/gtoehxogzg.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.ppjwa.cn/gtwxtjuzww.html

name VARCHAR(50) NOT NULL,
来源：http://hz.zdqjudy.top/gtdztxqqof.html

email VARCHAR(100) UNIQUE,
来源：http://hz.xziqi.cn/gtzckhqocf.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.zhiwuduotai.top/gtfhnfblww.html

);
来源：http://hz.shuidangran.top/gtswsepzwf.html

[Q02] 创建带外键的表
来源：http://hz.hfpthk.cn/gtsppbomwq.html

CREATE TABLE orders (
来源：http://hz.cashguo.top/gtlasnhuxq.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.cashguo.top/gtkgqvmvqm.html

user_id INT NOT NULL,
来源：http://hz.xuetiantiany.cn/gtgshtphtz.html

amount DECIMAL(10, 2),
来源：http://hz.ivvv.top/gtkfwzxwwo.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.yj202588.top/gteszimepq.html

);
来源：http://hz.aizwys.cn/gtlggjmiwt.html

[Q03] 增加列
来源：http://hz.shanyushiyangtech.top/gtaduzdukz.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.jiagoushi.top/gtsxavyaqy.html

[Q04] 修改列类型
来源：http://hz.cucudq.cn/gtwfhtaoch.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.jiagoushi.top/gtldzlgswm.html

[Q05] 重命名列
来源：http://hz.xylfe.cn/gthysofijo.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.yanxiufei.cn/gtpoodguaw.html

[Q06] 删除列
来源：http://hz.ehwqpu.com/gtgagnfvjp.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.ehwqpu.com/gthicpzibr.html

[Q07] 删除表
来源：http://hz.gogol.net.cn/gtykbuvedo.html

DROP TABLE IF EXISTS orders;
来源：http://hz.birdmap.top/gtzsijnsrl.html

[Q08] 创建普通索引
来源：http://hz.dashuyun.cn/gtdrosrjth.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.52xcode.cn/gtezbghzpu.html

[Q09] 创建唯一索引
来源：http://hz.yanxiufei.cn/gtdlkahbkq.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.yangfankeji.com/gtfmmvuteh.html

[Q10] 插入单行
来源：http://hz.vqdsnc.cn/gticphzwrq.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.jqgufenzy.top/gthtrutiki.html

[Q11] 一次插入多行
来源：http://hz.yonumen.top/gthucxnyuj.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.zycfv.cn/gtgqbwuvmo.html

[Q12] 插入后取自增 ID
来源：http://hz.daria6918.cn/gtubytheil.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.hywenlv.cn/gtntwdjptp.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.andypj.xyz/gtmgyfttjb.html

[Q13] 忽略重复插入
来源：http://hz.shuidangran.top/gttkcfvobo.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.jinyuanbaomall.cn/gtoluexvyu.html

[Q14] 存在则更新（upsert）
来源：http://hz.svipenyu.cn/gtgjvndflt.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.feifeiyinyue.top/gtbpieuufy.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.cqqwz.cn/gtkdamdiop.html

[Q15] 查询全部
来源：http://hz.yueranfly.top/gtjzxlyxli.html

SELECT * FROM users;
来源：http://hz.xziqi.cn/gtmedzokqm.html

[Q16] 查询指定列
来源：http://hz.aibaodan.cn/gtfxykejku.html

SELECT id, name FROM users;
来源：http://hz.wangdashe.top/gtakibkjri.html

[Q17] 条件查询
来源：http://hz.ywan-chungtsiang.top/gtktyziycy.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.wangdashe.top/gtforlzlek.html

[Q18] 模糊匹配
来源：http://hz.316326.xyz/gthtlaiuch.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.yj20258.top/gtfwmwkqqo.html

[Q19] 范围查询
来源：http://hz.jqgufenzy.top/gtilqljptb.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.sweek.top/gtorzphbro.html

[Q20] IN 列表
来源：http://hz.cucudq.cn/gtzpmpqvpl.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.jianghu66.top/gtllqwshgs.html

[Q21] 空值判断
来源：http://hz.meibo888.top/gtaeapyacd.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.aizwys.cn/gtcavmvcrx.html

[Q22] 排序
来源：http://hz.andypj.xyz/gttwywhcdv.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.cheryme.top/gtsvvogawc.html

[Q23] 分页
来源：http://hz.zhiwuduotai.top/gtgkbugwqu.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.tian-w.cn/gtainjrfbx.html

[Q24] 去重
来源：http://hz.gotoacloud.top/gtzxgzhntf.html

SELECT DISTINCT city FROM users;
来源：http://hz.sysykeji.top/gtwpimxmom.html

[Q25] 只取前 N 条
来源：http://hz.snrcjt.cn/gtfxqpovks.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.guannengcc.top/gtbfvnnkti.html

[Q26] 计数
来源：http://hz.nanxuanxn.top/gtnmpqjddo.html

SELECT COUNT(*) FROM users;
来源：http://hz.vqdsnc.cn/gtyhwxpqii.html

[Q27] 条件计数
来源：http://hz.yj20258.top/gtulpfpxpq.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.sufxvd.cn/gtblvwjfzj.html

[Q28] 求和与平均
来源：http://hz.nwbrower.top/gtcxvsclqh.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.jqgufenzy.top/gtlidszkpf.html

[Q29] 最大最小值
来源：http://hz.jqgufenzy.top/gtaumnqiew.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.gzhubu.top/gtxhfyrtmm.html

[Q30] 分组统计
来源：http://hz.cdnleiting.top/gtolieqlyh.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.meibo888.top/gtkmsrllmp.html

[Q31] 分组后过滤
来源：http://hz.hfpthk.cn/gtddxgmvaz.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.yongpay.top/gtqxstrnho.html

[Q32] 分组拼接字符串
来源：http://hz.daria6918.cn/gtaicrotqa.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.gogol.net.cn/gtbuuthjqp.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.havefunace.top/gtjuncpypf.html

[Q33] 多列分组
来源：http://hz.cqqwz.cn/gtuyojxrfu.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.svipenyu.cn/gtcykridqt.html

[Q34] 每组取第一条
来源：http://hz.jinqigfzy.top/gtkihkuyla.html

SELECT * FROM (
来源：http://hz.ydzc1.top/gtsnczevug.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.yj202588.top/gtntwistek.html

) t WHERE rn = 1;
来源：http://hz.zhiwuduotai.top/gtqnpdevvf.html

[Q35] 内连接
来源：http://hz.zhengqikj.top/gtyiuqhvxp.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.nanxuanxn.top/gtgjgiumod.html

[Q36] 左连接
来源：http://hz.cashguo.top/gtclkbvzmb.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.shzxlz.cn/gtgxltvgnl.html

[Q37] 右连接
来源：http://hz.0kj1m.cn/gthtvosuqt.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.zdqjudy.top/gtzukcdtwh.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.feifeiyinyue.top/gtxgjfjgkp.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.meibo888.top/gtxxhvaoje.html

[Q39] 自连接（查上下级）
来源：http://hz.ydjk.org.cn/gtvoesizae.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.nanxuanxn.top/gtrhdottzj.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.shanyushiyangkeji.top/gtpvbelfmw.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.zhengqikj.top/gtnlnhzwsi.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.fengsongda.top/gtogyuqftg.html

[Q41] 多表连接
来源：http://hz.zhaomingkeji.xyz/gtgsefdxkb.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.haohaochexian.top/gtxbsrzstf.html

JOIN users u ON u.id = o.user_id
来源：http://hz.hywenlv.cn/gtxpysxbts.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.bjfxy.top/gtwvvmricx.html

[Q42] 连接条件附加过滤
来源：http://hz.hnqzz.top/gttwwlokfs.html

SELECT u.name, o.amount FROM users u
来源：http://hz.sxryk.cn/gtdbbrxriv.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.jqgufenzy.top/gtlrxowtfc.html

[Q43] 标量子查询
来源：http://hz.ivvv.top/gtxtypnhgz.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.gzhubu.top/gtqoznjpau.html

[Q44] IN 子查询
来源：http://hz.zycfv.cn/gttbfupkiq.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.jqgfzy.top/gtunxoverl.html

[Q45] EXISTS 判断存在
来源：http://hz.yanxiufei.cn/gtzhyawmbp.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.guannengcc.top/gtasivirav.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.daxiang520.top/gtpmwlzxpj.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.redwolf501.top/gtbnxumnuv.html

[Q47] 与平均值比较
来源：http://hz.sxryk.cn/gtgienxcaa.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.shanyushiyangkeji.top/gtdfdsfkhv.html

[Q48] CTE 公用表表达式
来源：http://hz.yuxming.cn/gthducuxez.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.quarkkingdee.top/gtedaiqamu.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.ivvv.top/gtiscnuwad.html

[Q49] 更新单行
来源：http://hz.quarkkingdee.top/gthseiwnog.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.jyoumei.cn/gtuisiwdhe.html

[Q50] 批量更新
来源：http://hz.zhengqikj.top/gtafzikwqs.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.jqgfzy.top/gtgpkfnzif.html

[Q51] 用子查询更新
来源：http://hz.yuanzhike.top/gtkgiwxqmk.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.yueranfly.top/gtlbuogaph.html

[Q52] 删除指定行
来源：http://hz.yj20258888.top/gtpbvuindb.html

DELETE FROM users WHERE id = 10;
来源：http://hz.jinqigufen.top/gtvdjbcfaw.html

[Q53] 按条件删除
来源：http://hz.zhixingplan.top/gtnnljqkvm.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.zhiwuduotai.top/gtjhsrgmpw.html

[Q54] 清空表
来源：http://hz.316326.xyz/gtcjoacapt.html

TRUNCATE TABLE logs;
来源：http://hz.tanke756.top/gtdbfapenq.html

[Q55] 排名（并列占位）
来源：http://hz.hnxiangtu.top/gtzggeyuap.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.daxiang520.top/gtxeniwfrc.html

[Q56] 密集排名（并列不占位）
来源：http://hz.yuanzhike.top/gtrmudfmoo.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.yanxiufei.cn/gtloxhcema.html

[Q57] 行号
来源：http://hz.fzhhl.top/gtnhatcohf.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.birdmap.top/gtwzatovdr.html

[Q58] 累计求和
来源：http://hz.redwolf501.top/gtxhpnxrsr.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.yueranfly.top/gtaomopske.html

[Q59] 分组内累计
来源：http://hz.aibaodan.cn/gtzgqunkie.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.sufxvd.cn/gtdalmbxju.html

[Q60] 取上一行 / 下一行
来源：http://hz.jqgufenzy.top/gtzfjnypbu.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.cucudq.cn/gtjeprlovr.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.daxiang520.top/gtakpuxnaw.html


<!-- 参考信息 -->