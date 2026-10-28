代发 wailian999

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.daria6918.cn/gtthmcklze.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.svipenyu.cn/gttaalxuvi.html

Java: class Node { int v; Node next; }
来源：http://hz.fzhhl.top/gtsngqbhkt.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.dianchejie.cn/gtzymnqjfc.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.shanyushiyangtech.top/gttefdxjcf.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.ydjk.org.cn/gtfdzduwdz.html

[N11] 二叉树中序遍历
来源：http://hz.shanyushiyangtech.top/gtmujuivuv.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.shangyingyoupin.top/gtkmlamzvb.html

PHP:  // 手写递归函数
来源：http://hz.smart0.xyz/gtulyhyaxb.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.snrcjt.cn/gtcdojhtck.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.hywenlv.cn/gtnzpopqri.html

Java: // 手写递归
来源：http://hz.sxryk.cn/gtmdritthb.html

Go:   // 手写递归
来源：http://hz.xylfe.cn/gtobdttptp.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.nanxuanxn.top/gtqionptoq.html

C#:   // 手写递归
来源：http://hz.aizwys.cn/gtegcmpvjm.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.birdmap.top/gtdwknxgrb.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.shuidangran.top/gtauwgcebj.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.sysykeji.top/gtycjbafoz.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.xingfuxueyuan.xyz/gtfdhnrxxx.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.zhongyouzk.top/gtgmmpvfad.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.cheryme.top/gtoaeavgso.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.chenzaomai.com/gtwrjlfhjd.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.andypj.xyz/gtpzpdwskb.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.cqqwz.cn/gtxlklqigt.html

================================================================================
来源：http://hz.zycfv.cn/gtzkvdxvks.html

O. 并发与异步
来源：http://hz.zhengqikj.top/gtfuxxrnjj.html

================================================================================
来源：http://hz.guannengcc.top/gtwnkvfylg.html

[O01] 启动一个线程
来源：http://hz.yueranfly.top/gtrhcozwlr.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.nanxuanxn.top/gthhsxeepq.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.havefunace.top/gtfzuykbda.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.bjfxy.top/gtuyokeuyl.html

TS:   // 同 JS
来源：http://hz.redwolf501.top/gtujlovqno.html

Java: new Thread(() -> f()).start()
来源：http://hz.tanke756.top/gtzbeepjft.html

Go:   go f()
来源：http://hz.haohaochexian.top/gtetfovchd.html

Ruby: Thread.new { f }
来源：http://hz.snrcjt.cn/gtpozlimyb.html

C#:   Task.Run(() => F());
来源：http://hz.zhongyouzk.top/gtwtdessyb.html

[O02] 使用线程池
来源：http://hz.zhaomingkeji.xyz/gtwolmfdxo.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.c1oappe.top/gtvqinuwqc.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.0kj1m.cn/gtybrcirgm.html

JS:   // worker_threads 线程池
来源：http://hz.chenlongwang.top/gtcnyxgmqu.html

TS:   // worker_threads 线程池
来源：http://hz.zycfv.cn/gtgbqwqcrv.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.andypj.xyz/gtgguvptyp.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.smart0.xyz/gtydredruc.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.gaohongyu789.top/gtsdozjcje.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.ybcxt.top/gtnvvcpdii.html

[O03] 加锁保护共享数据
来源：http://hz.wangshuangyany.cn/gtrndjhdbb.html

Py:   with lock: shared += 1
来源：http://hz.svipenyu.cn/gtasuagatb.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.jinghuilouyu.cn/gtpoiprjnz.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.yuxming.cn/gtazbtzyhq.html

TS:   // 同 JS
来源：http://hz.shanyushiyangtech.top/gtcmmmejpj.html

Java: synchronized (this) { shared++; }
来源：http://hz.svipenyu.cn/gtfxcfegrw.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.zhengqikj.top/gtsndtvtsx.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.ppjwa.cn/gtrlahpiha.html

C#:   lock (gate) { shared++; }
来源：http://hz.jinqigufen.top/gtazeoselu.html

[O04] 定义异步函数并等待
来源：http://hz.birdmap.top/gtbwthkggk.html

Py:   async def f():⏎    await g()
来源：http://hz.hysaishi.cn/gtdjbbwcxl.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.ivvv.top/gtobfgsmjp.html

JS:   async function f() { await g(); }
来源：http://hz.yj202588.top/gtswgxocgr.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.smart0.xyz/gtciiyycpd.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.sufxvd.cn/gtvzsxyzwe.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.52xcode.cn/gtzkoraeuj.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.52xcode.cn/gtipeuvxll.html

C#:   async Task F() { await G(); }
来源：http://hz.daria6918.cn/gtyinwuybt.html

[O05] 并发执行并等待全部完成
来源：http://hz.0kj1m.cn/gtrisrmqoh.html

Py:   asyncio.gather(*tasks)
来源：http://hz.gzhubu.top/gtjsqscgfk.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.chenjidiqi.icu/gtlorfdfmo.html

JS:   await Promise.all(tasks)
来源：http://hz.nwbrower.top/gtglunrzsa.html

TS:   await Promise.all(tasks)
来源：http://hz.fengsongda.top/gtowwvtdkp.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.ppjwa.cn/gtxxrsnjsn.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.xuetiantiany.cn/gtubgxxyqy.html

Ruby: threads.map(&:join)
来源：http://hz.jianghu66.top/gtxcjrpdhp.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.chenjidiqi.icu/gtifpghnyn.html

[O06] 使用进程池
来源：http://hz.gogol.net.cn/gtyiijcruo.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.yj20258.top/gtadqeqmmn.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.yuxming.cn/gtxelatwkt.html

JS:   // child_process / cluster 模块
来源：http://hz.birdmap.top/gttotmtydl.html

TS:   // child_process / cluster 模块
来源：http://hz.xuetiantiany.cn/gtzpzxaebe.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.ydjk.org.cn/gtjouygogs.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.jinqigfzy.top/gtusdyobvi.html

Ruby: // fork 块
来源：http://hz.ivvv.top/gtgnljwbzt.html

C#:   Parallel.For
来源：http://hz.wangdashe.top/gtnvydiqfy.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtojsewmqm.html

P. 常用工具函数
来源：http://hz.xuanzx.com/gtcacxpwgv.html

================================================================================
来源：http://hz.gogol.net.cn/gtwtavfzuu.html

[P01] 生成 UUID
来源：http://hz.zhixingplan.top/gtqxfcklkm.html

Py:   str(uuid.uuid4())
来源：http://hz.fengsongda.top/gtacaegoeg.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.chenjidiqi.icu/gtkatsuhoo.html

JS:   crypto.randomUUID()
来源：http://hz.jiagoushi.top/gtzydeojre.html

TS:   crypto.randomUUID()
来源：http://hz.yj202588.top/gtewdtelns.html

Java: UUID.randomUUID().toString()
来源：http://hz.zhixingplan.top/gtnntziwlv.html

Go:   // 用 github.com/google/uuid
来源：http://hz.cashguo.top/gtqcplhubw.html

Ruby: SecureRandom.uuid
来源：http://hz.jyoumei.cn/gttptvstvx.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.nanxuanxn.top/gteanifrzi.html

[P02] MD5 / SHA256 摘要
来源：http://hz.jqgfzy.top/gtfptlhvzc.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.hammf.cn/gtptdscxwn.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.xinyue.icu/gtxooapbdj.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.quarkkingdee.top/gtelqmvpub.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.hnxiangtu.top/gtxxiaglfn.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.ydzc1.top/gtsoowbarf.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.iojbl.cn/gtednvhglu.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.zycfv.cn/gtucyjqssf.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.feifeiyinyue.top/gtbpcqvakl.html

[P03] 生成短随机字符串
来源：http://hz.xylfe.cn/gthpzjkufp.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.redwolf501.top/gtvgujafcm.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.jianghu66.top/gtbnvvdeyc.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.chenjidiqi.icu/gtzivizbnv.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.fzhhl.top/gtrsxqhekz.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.meibo888.top/gtkfobdndl.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.yongpay.top/gtfgaadjid.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.guowangkeji.top/gtqcfyyegh.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.52xcode.cn/gtiaaokrrt.html

[P04] 求长度
来源：http://hz.yangfankeji.com/gtsjgrflab.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.gogol.net.cn/gtutsrfanl.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.nanxinkj.top/gtuiyrzhxj.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.yj20258.top/gtgjhjgdsu.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.chenjidiqi.icu/gtgrrvydci.html

Java: list.size();  map.size();  s.length()
来源：http://hz.pengpengdd.cyou/gtgppkwuqa.html

Go:   len(arr);  len(m)
来源：http://hz.gaohongyu789.top/gtjzfrnver.html

Ruby: x.length;  x.size
来源：http://hz.sweek.top/gtosrulexy.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.ybcxt.top/gtacqnjyiq.html

[P05] 判断两个对象内容是否相等
来源：http://hz.xinyue.icu/gtqsllboga.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.jqgufenzy.top/gtxmbutfaq.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.jianghu66.top/gtcixhidfb.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.zhijiandao.cn/gthdayyxob.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.shuidangran.top/gtmwuoczky.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.hongshengwenyu.top/gtenlaeazc.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.quarkkingdee.top/gtsrhiilmr.html

Ruby: a == b
来源：http://hz.kuanghao11.cn/gtuxbmbtdk.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.52xcode.cn/gtxemgzhkg.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.snrcjt.cn/gtsjproqsu.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.gaohongyu789.top/gtbqavbnwx.html

PHP:  if (empty($x)) {}
来源：http://hz.vqdsnc.cn/gtspzibzae.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.yj202588.top/gtzetnzgwx.html

TS:   if (x == null) {}
来源：http://hz.jyoumei.cn/gthoprpqjo.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.guowangkeji.top/gtvnskshnu.html

Go:   if x == nil {}
来源：http://hz.smart0.xyz/gtonwjdcyg.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.hnxiangtu.top/gtrpehjziu.html

C#:   if (x is null) {}
来源：http://hz.tian-w.cn/gtmthydaip.html

[P07] 防抖与节流
来源：http://hz.jiagoushi.top/gtsbpczudg.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.haohaochexian.top/gtkrezthzr.html

PHP:  // 手写时间戳比较
来源：http://hz.zycfv.cn/gtwztyetjj.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.ybcxt.top/gtsbpcghxs.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.jinghuilouyu.cn/gtvjprnzvp.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.dashuyun.cn/gtqvounvza.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.jinghuilouyu.cn/gtshsexbdv.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.jinyuanbaomall.cn/gtalaizsom.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.jqgfzy.top/gtiuizfkzi.html

[P08] 处理浮点精度问题
来源：http://hz.zdqjudy.top/gtpwetlavn.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.cdnleiting.top/gtmbxleuft.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.0kj1m.cn/gttzvhdlrv.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.ehwqpu.com/gtxabxiqln.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.zhijiandao.cn/gtaicjbwyy.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.guowangkeji.top/gtuszdqmsd.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.hysaishi.cn/gtucpqurrr.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.pycfn.com/gtdfaiisct.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.ybcxt.top/gtcugfyqvz.html

================================================================================
来源：http://hz.xinyue.icu/gttjvgutcx.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.yj202588.top/gtzrknuluc.html

================================================================================
来源：http://hz.xziqi.cn/gtkvubbaqm.html

[Q01] 创建表
来源：http://hz.jlsjyb.cn/gtbubpfemt.html

CREATE TABLE users (
来源：http://hz.yueranfly.top/gtitdjakjt.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.gaohongyu789.top/gtcrasiokd.html

name VARCHAR(50) NOT NULL,
来源：http://hz.vqdsnc.cn/gtdntajxel.html

email VARCHAR(100) UNIQUE,
来源：http://hz.chenzaomai.com/gtrfkywxqm.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.yj20258.top/gtgelikrly.html

);
来源：http://hz.tanke756.top/gtdwxellrr.html

[Q02] 创建带外键的表
来源：http://hz.hammf.cn/gtndvmfjxk.html

CREATE TABLE orders (
来源：http://hz.daria6918.cn/gtfhcdzvzf.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.yj20258888.top/gtkbtddqxr.html

user_id INT NOT NULL,
来源：http://hz.havefunace.top/gttinohqzl.html

amount DECIMAL(10, 2),
来源：http://hz.daxiang520.top/gtgdbxnxxb.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.yangfankeji.com/gtcjavvhgf.html

);
来源：http://hz.pycfn.com/gtujdqbnlc.html

[Q03] 增加列
来源：http://hz.jianghu66.top/gtbmehizfi.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.daria6918.cn/gtxapbmyqh.html

[Q04] 修改列类型
来源：http://hz.shangyingyoupin.top/gtkeopbjzp.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.yonumen.top/gtnjkbcdaq.html

[Q05] 重命名列
来源：http://hz.tian-w.cn/gtirfmmobh.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.cqqwz.cn/gtutednktu.html

[Q06] 删除列
来源：http://hz.316326.xyz/gtgrirlyzm.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.pengpengdd.cyou/gtqznlnemc.html

[Q07] 删除表
来源：http://hz.zhixingplan.top/gtmsfgcqzx.html

DROP TABLE IF EXISTS orders;
来源：http://hz.gaohongyu789.top/gthzzuezmk.html

[Q08] 创建普通索引
来源：http://hz.xziqi.cn/gtmwvajpqn.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.quarkkingdee.top/gtsqvhkklq.html

[Q09] 创建唯一索引
来源：http://hz.dianchejie.cn/gtaqpjhfek.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.hnxiangtu.top/gtrtediobk.html

[Q10] 插入单行
来源：http://hz.sxryk.cn/gtdrrgteyo.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.redwolf501.top/gtjmjkdnox.html

[Q11] 一次插入多行
来源：http://hz.jqgufenzy.top/gtsxavkzji.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.yuxming.cn/gtenfueplo.html

[Q12] 插入后取自增 ID
来源：http://hz.zhijiandao.cn/gtekddnymp.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.xylfe.cn/gtflkjokhh.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.yj20258888.top/gtduxsknwb.html

[Q13] 忽略重复插入
来源：http://hz.ybcxt.top/gtbvtscnpo.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.yj20258888.top/gtysctozxr.html

[Q14] 存在则更新（upsert）
来源：http://hz.jinqigufen.top/gtuodulhws.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.sweek.top/gtsthexnal.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.c1oappe.top/gtmiwsmfjn.html

[Q15] 查询全部
来源：http://hz.jqgfzy.top/gtexpwuuop.html

SELECT * FROM users;
来源：http://hz.yonumen.top/gtmpnwvhyl.html

[Q16] 查询指定列
来源：http://hz.yangfankeji.com/gtvxerhzzy.html

SELECT id, name FROM users;
来源：http://hz.fengsongda.top/gthkuvbxdj.html

[Q17] 条件查询
来源：http://hz.hnxiangtu.top/gtlxazyamz.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.nanxuanxn.top/gtvpwiqqae.html

[Q18] 模糊匹配
来源：http://hz.ydjk.org.cn/gtlxlwphyi.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.havefunace.top/gtmdohbpom.html

[Q19] 范围查询
来源：http://hz.shanyushiyangkeji.top/gtyxizikhq.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.aibaodan.cn/gtgmybjogb.html

[Q20] IN 列表
来源：http://hz.aibaodan.cn/gtcrdcszyf.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.gotoacloud.top/gtudlseitr.html

[Q21] 空值判断
来源：http://hz.hywenlv.cn/gtyndaknmd.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.zycfv.cn/gtvuxebljm.html

[Q22] 排序
来源：http://hz.hnqzz.top/gthijqtkby.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.fzhhl.top/gttuzxpbck.html

[Q23] 分页
来源：http://hz.sysykeji.top/gtjcaeegwm.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.wangdashe.top/gtbuqditvu.html

[Q24] 去重
来源：http://hz.yuxming.cn/gtqoehthps.html

SELECT DISTINCT city FROM users;
来源：http://hz.cucudq.cn/gtttusbxfx.html

[Q25] 只取前 N 条
来源：http://hz.jyoumei.cn/gtbpqcdchu.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.bjfxy.top/gtihdmkgjt.html

[Q26] 计数
来源：http://hz.snrcjt.cn/gtdsuzoazv.html

SELECT COUNT(*) FROM users;
来源：http://hz.shanyushiyangkeji.top/gtfceqhoof.html

[Q27] 条件计数
来源：http://hz.tianlin.xyz/gtnmotkbja.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.chenlongwang.top/gthkaqytst.html

[Q28] 求和与平均
来源：http://hz.jqgfzy.top/gtnmqlqvdo.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.yongpay.top/gtkijqaair.html

[Q29] 最大最小值
来源：http://hz.wangshuangyany.cn/gtkltuxxwf.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.ppjwa.cn/gtvyistfpi.html

[Q30] 分组统计
来源：http://hz.daxiang520.top/gthpodcwmo.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.yanxiufei.cn/gtycpokqzw.html

[Q31] 分组后过滤
来源：http://hz.nanxinkj.top/gtwwpguosc.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.chenzaomai.com/gtgbwiodjm.html

[Q32] 分组拼接字符串
来源：http://hz.tianlin.xyz/gtliyuzjlj.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.kuanghao11.cn/gtpjjuawdb.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.redwolf501.top/gtwwxoaage.html

[Q33] 多列分组
来源：http://hz.meibo888.top/gtvszryvog.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.jyoumei.cn/gtjlhexdys.html

[Q34] 每组取第一条
来源：http://hz.sysykeji.top/gtforfeehk.html

SELECT * FROM (
来源：http://hz.pengpengdd.cyou/gtwhszgpus.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.zhiwuduotai.top/gthjbthjxg.html

) t WHERE rn = 1;
来源：http://hz.shanyushiyangkeji.top/gtxzdfsupt.html

[Q35] 内连接
来源：http://hz.redwolf501.top/gtwkyzjwlr.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.shangyingyoupin.top/gtathsrmit.html

[Q36] 左连接
来源：http://hz.sufxvd.cn/gtgwnucdvg.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.pycfn.com/gtnxjowbdn.html

[Q37] 右连接
来源：http://hz.tanke756.top/gtqrzadldv.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.shuidangran.top/gtamhvyiew.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.fengsongda.top/gtisfxwcyp.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.feifeiyinyue.top/gtwibpieue.html

[Q39] 自连接（查上下级）
来源：http://hz.nanxuanxn.top/gtwlimvxns.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.svipenyu.cn/gtijbqlfxi.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.shuidangran.top/gtqorqwnew.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.xylfe.cn/gtriklzxox.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.hnqzz.top/gtanmierhk.html

[Q41] 多表连接
来源：http://hz.jlsjyb.cn/gtsxqsaqoe.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.wangdashe.top/gtytupgavg.html

JOIN users u ON u.id = o.user_id
来源：http://hz.ywan-chungtsiang.top/gtltresxex.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.meibo888.top/gtvonjhfar.html

[Q42] 连接条件附加过滤
来源：http://hz.shangyingyoupin.top/gtwdsdhquy.html

SELECT u.name, o.amount FROM users u
来源：http://hz.jinqigufen.top/gtkuezrvrd.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.316326.xyz/gtcassrwdz.html

[Q43] 标量子查询
来源：http://hz.gotoacloud.top/gtjjlinqhe.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.ppjwa.cn/gtlmfovtjw.html

[Q44] IN 子查询
来源：http://hz.yvedp.cn/gthxehpezx.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.chenlongwang.top/gtoifrihsq.html

[Q45] EXISTS 判断存在
来源：http://hz.jyoumei.cn/gtolapiawb.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.316326.xyz/gtgekecpnv.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.sufxvd.cn/gtftxeqfvp.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.c1oappe.top/gtouaidmuv.html

[Q47] 与平均值比较
来源：http://hz.wangdashe.top/gtohsgjaxq.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.zhijiandao.cn/gtcguvfjqs.html

[Q48] CTE 公用表表达式
来源：http://hz.gogol.net.cn/gtdikoypku.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.ydjk.org.cn/gtmzhagpkw.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.bjfxy.top/gtpttshqxv.html

[Q49] 更新单行
来源：http://hz.andypj.xyz/gtwahyzfoz.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.yanxiufei.cn/gtoizyeeoz.html

[Q50] 批量更新
来源：http://hz.ywan-chungtsiang.top/gtcmncezbs.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.zhiwuduotai.top/gtvnvncogi.html

[Q51] 用子查询更新
来源：http://hz.daxiang520.top/gtktfnlhgv.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.cqqwz.cn/gtooifgkqw.html

[Q52] 删除指定行
来源：http://hz.andypj.xyz/gtsgzwrmlg.html

DELETE FROM users WHERE id = 10;
来源：http://hz.zhaomingkeji.xyz/gthirmebsa.html

[Q53] 按条件删除
来源：http://hz.gzhubu.top/gtgceexyrk.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.smart0.xyz/gtcnkcgjkj.html

[Q54] 清空表
来源：http://hz.aizwys.cn/gtjjsyznlg.html

TRUNCATE TABLE logs;
来源：http://hz.yj202588.top/gtzcgzzowh.html

[Q55] 排名（并列占位）
来源：http://hz.sweek.top/gtehekoorx.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.kuanghao11.cn/gtqgiplqvq.html

[Q56] 密集排名（并列不占位）
来源：http://hz.jianghu66.top/gtdzoktukj.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.cucudq.cn/gtebphwpec.html

[Q57] 行号
来源：http://hz.zdqjudy.top/gtbzcwwzjt.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.52xcode.cn/gtacqusdkl.html

[Q58] 累计求和
来源：http://hz.guannengcc.top/gtjdtucrrx.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.birdmap.top/gtwxvhyrnm.html

[Q59] 分组内累计
来源：http://hz.zhongyouzk.top/gtkhzhevmp.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.cheryme.top/gtlsqhensh.html

[Q60] 取上一行 / 下一行
来源：http://hz.hysaishi.cn/gtlcmbguct.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.snrcjt.cn/gtudpaepvo.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.hammf.cn/gtqxtxwrpg.html


<!-- 参考信息 -->