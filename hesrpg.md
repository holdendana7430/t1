代发 wailian999

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.sysykeji.top/gtqsagxlsv.html

[N10] 链表节点定义
来源：http://hz.yj20258.top/gtxslyiawd.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.ydzc1.top/gthwlcecvq.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.aibaodan.cn/gtpvqptkuh.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.shuidangran.top/gtbimrzwug.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.nanxuanxn.top/gtjvkhjqrs.html

Java: class Node { int v; Node next; }
来源：http://hz.fengsongda.top/gtjpeqyhrh.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.xylfe.cn/gtyqdlhlkp.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.gaohongyu789.top/gtivdaaskr.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.pycfn.com/gtyhwyiwxn.html

[N11] 二叉树中序遍历
来源：http://hz.nanxuanxn.top/gtycqhwufr.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.cucudq.cn/gtgbeyohpd.html

PHP:  // 手写递归函数
来源：http://hz.hnxiangtu.top/gtbayeqiqc.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.fengsongda.top/gtsgutelwc.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.sweek.top/gtttjsvrhh.html

Java: // 手写递归
来源：http://hz.daria6918.cn/gtthfvfqpw.html

Go:   // 手写递归
来源：http://hz.aizwys.cn/gtcdefiljj.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.andypj.xyz/gtzfxamgjc.html

C#:   // 手写递归
来源：http://hz.haohaochexian.top/gtapdxghuz.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.hnxiangtu.top/gtzajmjiyg.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.jinyuanbaomall.cn/gtffsgtrth.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.sweek.top/gtrmrndjtp.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.tianlin.xyz/gthxhexvtn.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.ehwqpu.com/gtejpiouuz.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.yongpay.top/gtbgkmswje.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.cashguo.top/gtjsglfsgv.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.tian-w.cn/gtlmxnhgbr.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.hfpthk.cn/gtckfsbtit.html

================================================================================
来源：http://hz.cucudq.cn/gtjfgvllat.html

O. 并发与异步
来源：http://hz.yueranfly.top/gtmqafdjkv.html

================================================================================
来源：http://hz.kuanghao11.cn/gtxsftyevs.html

[O01] 启动一个线程
来源：http://hz.jianghu66.top/gtvrbogaii.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.yvedp.cn/gtxqjigasb.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.52xcode.cn/gttnyopgdl.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.nwbrower.top/gtohnxhruk.html

TS:   // 同 JS
来源：http://hz.chenzaomai.com/gtzcujtawr.html

Java: new Thread(() -> f()).start()
来源：http://hz.yvedp.cn/gtsryyqfjg.html

Go:   go f()
来源：http://hz.cucudq.cn/gtrvcnlmxy.html

Ruby: Thread.new { f }
来源：http://hz.jlsjyb.cn/gttbtljtls.html

C#:   Task.Run(() => F());
来源：http://hz.jiagoushi.top/gtggyvnuya.html

[O02] 使用线程池
来源：http://hz.ydzc1.top/gtvlethgvz.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.ivvv.top/gtapgusrid.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.zhijiandao.cn/gtjrbljvqg.html

JS:   // worker_threads 线程池
来源：http://hz.zycfv.cn/gtjerajerl.html

TS:   // worker_threads 线程池
来源：http://hz.yj20258888.top/gtjuewcqxp.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.9152youxi.cn/gtwzuegubs.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.nanxuanxn.top/gtpbesorkq.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.yanxiufei.cn/gtexrstcyi.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.gotoacloud.top/gtvpfyoxxu.html

[O03] 加锁保护共享数据
来源：http://hz.wangshuangyany.cn/gtvuvhlsqo.html

Py:   with lock: shared += 1
来源：http://hz.fzhhl.top/gtosfcuyct.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.yuanzhike.top/gtuhppggjv.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.yangfankeji.com/gteaoyjkmm.html

TS:   // 同 JS
来源：http://hz.haohaochexian.top/gtyzorseox.html

Java: synchronized (this) { shared++; }
来源：http://hz.cheryme.top/gtckkjstvm.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.xingfuxueyuan.xyz/gtbncarrrw.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.gogol.net.cn/gtqjyzuqse.html

C#:   lock (gate) { shared++; }
来源：http://hz.xziqi.cn/gtrhneirjp.html

[O04] 定义异步函数并等待
来源：http://hz.guannengcc.top/gtyuaazqow.html

Py:   async def f():⏎    await g()
来源：http://hz.jqgfzy.top/gtvholpobr.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.nwbrower.top/gteykpokvw.html

JS:   async function f() { await g(); }
来源：http://hz.nanxinkj.top/gtbedhfgos.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.jinqigufen.top/gtfohpahqv.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.pengpengdd.cyou/gtgizbhepb.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.fengsongda.top/gtqohgafnh.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.hysaishi.cn/gtjtqkkble.html

C#:   async Task F() { await G(); }
来源：http://hz.chenlongwang.top/gtyptnfxih.html

[O05] 并发执行并等待全部完成
来源：http://hz.ywan-chungtsiang.top/gtioeazypf.html

Py:   asyncio.gather(*tasks)
来源：http://hz.chenlongwang.top/gtsqewimhj.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.shanyushiyangkeji.top/gtiycxogil.html

JS:   await Promise.all(tasks)
来源：http://hz.hfpthk.cn/gttgidolau.html

TS:   await Promise.all(tasks)
来源：http://hz.shzxlz.cn/gtqsruugwv.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.ivvv.top/gtuxgooyfc.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.yj202588.top/gtsxisqhfl.html

Ruby: threads.map(&:join)
来源：http://hz.meibo888.top/gtclkjarap.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.xylfe.cn/gteylejakf.html

[O06] 使用进程池
来源：http://hz.sweek.top/gtfaiplery.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.nanxinkj.top/gtroxvnxsj.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.nanxinkj.top/gtebwqjfge.html

JS:   // child_process / cluster 模块
来源：http://hz.aizwys.cn/gtynukalrv.html

TS:   // child_process / cluster 模块
来源：http://hz.xinyue.icu/gtxuwlnfuk.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.jqgfzy.top/gtuqtckmzd.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.xylfe.cn/gtvdmnowwv.html

Ruby: // fork 块
来源：http://hz.feifeiyinyue.top/gttirarjix.html

C#:   Parallel.For
来源：http://hz.ppjwa.cn/gtxfkjsdsn.html

================================================================================
来源：http://hz.zhixingplan.top/gtxlipydtb.html

P. 常用工具函数
来源：http://hz.cucudq.cn/gtnqkcgqbf.html

================================================================================
来源：http://hz.hammf.cn/gtvdswiecv.html

[P01] 生成 UUID
来源：http://hz.zhiwuduotai.top/gtlbvkdler.html

Py:   str(uuid.uuid4())
来源：http://hz.snrcjt.cn/gtynzcoxbs.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.shzxlz.cn/gtjyfrkytl.html

JS:   crypto.randomUUID()
来源：http://hz.xylfe.cn/gtovjieole.html

TS:   crypto.randomUUID()
来源：http://hz.dashuyun.cn/gtlvxcpqhk.html

Java: UUID.randomUUID().toString()
来源：http://hz.c1oappe.top/gtgqrriqyd.html

Go:   // 用 github.com/google/uuid
来源：http://hz.pengpengdd.cyou/gtgkqjljfg.html

Ruby: SecureRandom.uuid
来源：http://hz.quarkkingdee.top/gthdmdlbvh.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.jinqigfzy.top/gtonxlmxmj.html

[P02] MD5 / SHA256 摘要
来源：http://hz.xziqi.cn/gtmfpqeodz.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.xylfe.cn/gtipaqbzoz.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.pengpengdd.cyou/gtsjvwitga.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.yvedp.cn/gtpfxuvhkc.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.ivvv.top/gtohlyyoqq.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.ywan-chungtsiang.top/gtqkyqfhon.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.jinqigufen.top/gtqiaolxlz.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.yj202588.top/gtxpjtirbi.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.xuetiantiany.cn/gtydhkotmn.html

[P03] 生成短随机字符串
来源：http://hz.redwolf501.top/gtumifgaty.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.zhaomingkeji.xyz/gtareqfubg.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.ydzc1.top/gtrsjmkdaa.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.yuanzhike.top/gtgofjhjcl.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.jinqigfzy.top/gtjmaeqrda.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.yj20258.top/gtykslxwsh.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.jianghu66.top/gtosjxsmoo.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.zhaomingkeji.xyz/gtqxyfxxaw.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.tian-w.cn/gtykavhbmg.html

[P04] 求长度
来源：http://hz.hnqzz.top/gtpueojmds.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.pengpengdd.cyou/gtfdktqufz.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.wangshuangyany.cn/gtrmnrucgm.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.zhengqikj.top/gtzethaoyc.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.yongpay.top/gtlroxbaqj.html

Java: list.size();  map.size();  s.length()
来源：http://hz.yvedp.cn/gtbwrtkkho.html

Go:   len(arr);  len(m)
来源：http://hz.shangyingyoupin.top/gtutakbkoy.html

Ruby: x.length;  x.size
来源：http://hz.hnqzz.top/gtxxbclxou.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.smart0.xyz/gtxmgaakkg.html

[P05] 判断两个对象内容是否相等
来源：http://hz.birdmap.top/gtutdtdkge.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.haohaochexian.top/gtqvmkxgii.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.yj20258888.top/gtpxaayezl.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.zhaomingkeji.xyz/gtrxitrega.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.yongpay.top/gtypkaqtjs.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.xinyue.icu/gtwyodpdkj.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.iojbl.cn/gtlbjgtpnq.html

Ruby: a == b
来源：http://hz.yongpay.top/gtedaidltq.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.hnqzz.top/gtuywbjjbt.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.daxiang520.top/gtppqssrvk.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.gotoacloud.top/gtoqlubxia.html

PHP:  if (empty($x)) {}
来源：http://hz.chenjidiqi.icu/gtwhdgvlxp.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.zhixingplan.top/gtarulsdnb.html

TS:   if (x == null) {}
来源：http://hz.vqdsnc.cn/gtpevspwfp.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.ehwqpu.com/gtxzlerwjg.html

Go:   if x == nil {}
来源：http://hz.nwbrower.top/gtjzhkzanx.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.yuxming.cn/gtasvyvzfq.html

C#:   if (x is null) {}
来源：http://hz.jlsjyb.cn/gthbgviuab.html

[P07] 防抖与节流
来源：http://hz.hfpthk.cn/gttgwjbcil.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.havefunace.top/gtpnfalknm.html

PHP:  // 手写时间戳比较
来源：http://hz.jinghuilouyu.cn/gtmrvwhxph.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.jinqigufen.top/gtuesicqgl.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.shuidangran.top/gtilttydys.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.pengpengdd.cyou/gtgxeproin.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.guowangkeji.top/gthlwykmjo.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.zhaomingkeji.xyz/gtkqbxysda.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.jqgfzy.top/gtgizoxaok.html

[P08] 处理浮点精度问题
来源：http://hz.gotoacloud.top/gtefbxushg.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.ydzc1.top/gtcsskevwx.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.iojbl.cn/gtgvyqafdg.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.mhx1999.top/gtaobqeimw.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.yuxming.cn/gtjfonitoq.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.zhijiandao.cn/gtvosnyhva.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.gogol.net.cn/gtaapdxhqr.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.yongpay.top/gtvcwcphdp.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.yj20258888.top/gtztqcaucd.html

================================================================================
来源：http://hz.bjfxy.top/gtinapuure.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.jlsjyb.cn/gtgbesulgy.html

================================================================================
来源：http://hz.jinqigufen.top/gtioitmcte.html

[Q01] 创建表
来源：http://hz.shanyushiyangkeji.top/gtivqeodfx.html

CREATE TABLE users (
来源：http://hz.xuetiantiany.cn/gtkurwpwub.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.xuanzx.com/gtbpzohzfn.html

name VARCHAR(50) NOT NULL,
来源：http://hz.guowangkeji.top/gtajgfneop.html

email VARCHAR(100) UNIQUE,
来源：http://hz.zhaomingkeji.xyz/gtcatpgafl.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.tanke756.top/gtgfqpbjmm.html

);
来源：http://hz.cqqwz.cn/gtoxmvtzux.html

[Q02] 创建带外键的表
来源：http://hz.dianchejie.cn/gttukufikk.html

CREATE TABLE orders (
来源：http://hz.nanxuanxn.top/gtvnxsosrp.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.sxryk.cn/gtmlmurqso.html

user_id INT NOT NULL,
来源：http://hz.ehwqpu.com/gtsdpwgyvs.html

amount DECIMAL(10, 2),
来源：http://hz.yj20258.top/gtgtfbofbb.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.yuanzhike.top/gtattjatgi.html

);
来源：http://hz.nwbrower.top/gtnonugbgv.html

[Q03] 增加列
来源：http://hz.ivvv.top/gtppifuwqn.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.9152youxi.cn/gtrxxnmwuj.html

[Q04] 修改列类型
来源：http://hz.c1oappe.top/gtylfxzirm.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.yuanzhike.top/gtcyfpgzyi.html

[Q05] 重命名列
来源：http://hz.kuanghao11.cn/gtdvfdgmds.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.cdnleiting.top/gtgfqhvkqb.html

[Q06] 删除列
来源：http://hz.fengsongda.top/gtkayahmoe.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.dashuyun.cn/gtalrutnqx.html

[Q07] 删除表
来源：http://hz.yj20258.top/gtidgusygp.html

DROP TABLE IF EXISTS orders;
来源：http://hz.9152youxi.cn/gtlcwbihav.html

[Q08] 创建普通索引
来源：http://hz.yonumen.top/gtugamiwzl.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.shzxlz.cn/gtikkngomt.html

[Q09] 创建唯一索引
来源：http://hz.cdnleiting.top/gtzzbxfcno.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.jinyuanbaomall.cn/gtsrptxrmi.html

[Q10] 插入单行
来源：http://hz.jinghuilouyu.cn/gthkxjwrrt.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.tian-w.cn/gtnihwuqnq.html

[Q11] 一次插入多行
来源：http://hz.zhijiandao.cn/gtkzuggzvs.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.yuxming.cn/gtrgidpefh.html

[Q12] 插入后取自增 ID
来源：http://hz.feifeiyinyue.top/gtjidsjcog.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.cqqwz.cn/gtfkiacbtv.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.zhiwuduotai.top/gtstpifcoj.html

[Q13] 忽略重复插入
来源：http://hz.jinqigufen.top/gtzretguvx.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.guannengcc.top/gtamewsciw.html

[Q14] 存在则更新（upsert）
来源：http://hz.ehwqpu.com/gtendzwjzk.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.shzxlz.cn/gtrpzuzguc.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.zhongyouzk.top/gtgglqxwcf.html

[Q15] 查询全部
来源：http://hz.ivvv.top/gteyatkqwc.html

SELECT * FROM users;
来源：http://hz.nanxinkj.top/gtafgfegky.html

[Q16] 查询指定列
来源：http://hz.52xcode.cn/gtuunbufnt.html

SELECT id, name FROM users;
来源：http://hz.shanyushiyangtech.top/gtgqmvdmec.html

[Q17] 条件查询
来源：http://hz.jiagoushi.top/gtbapjnhtx.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.daxiang520.top/gtppokvoml.html

[Q18] 模糊匹配
来源：http://hz.jqgufenzy.top/gtdbpfxvoy.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.yuanzhike.top/gtiyhaszhi.html

[Q19] 范围查询
来源：http://hz.cucudq.cn/gteyuxrzwg.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.hnxiangtu.top/gtoogzswvw.html

[Q20] IN 列表
来源：http://hz.wangdashe.top/gtiumqogmm.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.feifeiyinyue.top/gtceimktko.html

[Q21] 空值判断
来源：http://hz.hysaishi.cn/gtjjrkgzdt.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.cheryme.top/gtlafpubyd.html

[Q22] 排序
来源：http://hz.fzhhl.top/gthybqwxkb.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.xuanzx.com/gtrtpofcfd.html

[Q23] 分页
来源：http://hz.shanyushiyangtech.top/gtdmtqpmog.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.feifeiyinyue.top/gtvwtcpxfl.html

[Q24] 去重
来源：http://hz.hongshengwenyu.top/gthuqgxruv.html

SELECT DISTINCT city FROM users;
来源：http://hz.aibaodan.cn/gtvjirajwn.html

[Q25] 只取前 N 条
来源：http://hz.shanyushiyangkeji.top/gtneosokyb.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.cdnleiting.top/gtafnsnxro.html

[Q26] 计数
来源：http://hz.guannengcc.top/gttrkokpqn.html

SELECT COUNT(*) FROM users;
来源：http://hz.mhx1999.top/gtowatrxwb.html

[Q27] 条件计数
来源：http://hz.yanxiufei.cn/gtnaeibmbc.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.zdqjudy.top/gtzgnwslbi.html

[Q28] 求和与平均
来源：http://hz.jiagoushi.top/gtirwhouvm.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.xinyue.icu/gtmqkpmgbr.html

[Q29] 最大最小值
来源：http://hz.yj20258.top/gttxfokcop.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.ppjwa.cn/gtbkjqvgdj.html

[Q30] 分组统计
来源：http://hz.fzhhl.top/gtuktilmgs.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.yongpay.top/gtvnpenkim.html

[Q31] 分组后过滤
来源：http://hz.shangyingyoupin.top/gtzifzojsi.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.yanxiufei.cn/gtqyfdvscp.html

[Q32] 分组拼接字符串
来源：http://hz.daria6918.cn/gtgsqenfit.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.zhixingplan.top/gttbbaazib.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.hywenlv.cn/gtkqhrmwuc.html

[Q33] 多列分组
来源：http://hz.hywenlv.cn/gtgxstafij.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.hnqzz.top/gtyzzjeqrw.html

[Q34] 每组取第一条
来源：http://hz.zdqjudy.top/gtqkadklmn.html

SELECT * FROM (
来源：http://hz.yuanzhike.top/gtfkdgrdjs.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.ppjwa.cn/gtcongwwbz.html

) t WHERE rn = 1;
来源：http://hz.birdmap.top/gtdcthledt.html

[Q35] 内连接
来源：http://hz.ehwqpu.com/gtflitircj.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.shuidangran.top/gtyoanmpdo.html

[Q36] 左连接
来源：http://hz.zhijiandao.cn/gtqpmqqoew.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.guannengcc.top/gttfuphesl.html

[Q37] 右连接
来源：http://hz.ppjwa.cn/gtvlocdbhu.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.ppjwa.cn/gtmnpooyyw.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.yj20258888.top/gtpkryfotk.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.shzxlz.cn/gtmvwacaue.html

[Q39] 自连接（查上下级）
来源：http://hz.yongpay.top/gtmqctygsv.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.yuxming.cn/gtwjgmttpr.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.feifeiyinyue.top/gtehicguba.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.hongshengwenyu.top/gtasduodgj.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.guannengcc.top/gtsinmfofm.html

[Q41] 多表连接
来源：http://hz.jqgufenzy.top/gtxaiuzvul.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.shzxlz.cn/gtayomywtb.html

JOIN users u ON u.id = o.user_id
来源：http://hz.yanxiufei.cn/gtgcxoaacs.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.aizwys.cn/gtzgmvadgf.html

[Q42] 连接条件附加过滤
来源：http://hz.pycfn.com/gtnzzpjffb.html

SELECT u.name, o.amount FROM users u
来源：http://hz.cashguo.top/gtxbduwzxr.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.yj20258888.top/gtlnnstmxw.html

[Q43] 标量子查询
来源：http://hz.xziqi.cn/gtrxjrmflb.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.yuxming.cn/gtwfjwrhks.html

[Q44] IN 子查询
来源：http://hz.zhoulong.xyz/gtrrainiiy.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.xinyue.icu/gtgowrzcuv.html

[Q45] EXISTS 判断存在
来源：http://hz.ppjwa.cn/gtghkabemz.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.meibo888.top/gtabpcrgij.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.xuanzx.com/gtcqqtkytg.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.xziqi.cn/gtnhpvcuze.html

[Q47] 与平均值比较
来源：http://hz.ywan-chungtsiang.top/gtnopxqngv.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.mhx1999.top/gtlhkkazok.html

[Q48] CTE 公用表表达式
来源：http://hz.gzhubu.top/gtuwrqkhfx.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.yj202588.top/gtynazfxiv.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.xingfuxueyuan.xyz/gtnndglmiu.html

[Q49] 更新单行
来源：http://hz.kuanghao11.cn/gtalodyxjh.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.gzhubu.top/gtwjdfaydc.html

[Q50] 批量更新
来源：http://hz.xingfuxueyuan.xyz/gtlsiodxyc.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.sysykeji.top/gtsbtvqaoo.html

[Q51] 用子查询更新
来源：http://hz.nanxuanxn.top/gtxxmjqnsd.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.jqgufenzy.top/gttccfpvck.html

[Q52] 删除指定行
来源：http://hz.nanxuanxn.top/gtkkukzzad.html

DELETE FROM users WHERE id = 10;
来源：http://hz.guannengcc.top/gtnhoqndyn.html

[Q53] 按条件删除
来源：http://hz.jqgufenzy.top/gtxtgydwpp.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.ydjk.org.cn/gtoyucbsyj.html

[Q54] 清空表
来源：http://hz.mhx1999.top/gtzwggrqmm.html

TRUNCATE TABLE logs;
来源：http://hz.guannengcc.top/gtpkpydpqj.html

[Q55] 排名（并列占位）
来源：http://hz.zycfv.cn/gtecjclpxh.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.hammf.cn/gtwyynwvym.html

[Q56] 密集排名（并列不占位）
来源：http://hz.fengsongda.top/gtojsinuie.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.birdmap.top/gteglmvook.html

[Q57] 行号
来源：http://hz.meibo888.top/gtbavfxzhf.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.pycfn.com/gtaraxwiis.html

[Q58] 累计求和
来源：http://hz.c1oappe.top/gtwlozldtv.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.cqqwz.cn/gthrlfxfhb.html

[Q59] 分组内累计
来源：http://hz.gotoacloud.top/gtqocclwkk.html


<!-- 参考信息 -->