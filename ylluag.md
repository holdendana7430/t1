代发 wailian999

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.0kj1m.cn/gtcbirgzvt.html

[N10] 链表节点定义
来源：http://hz.0kj1m.cn/gtrniqokct.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.ppjwa.cn/gthlnhgyvi.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.jinqigufen.top/gtwkdpqfrt.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.jinqigfzy.top/gtvqlpanry.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.meibo888.top/gtkcxumtmk.html

Java: class Node { int v; Node next; }
来源：http://hz.yonumen.top/gtfpicrcee.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.hywenlv.cn/gtilbacdys.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.shangyingyoupin.top/gtbkuwdbjm.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.316326.xyz/gtelkjxvwj.html

[N11] 二叉树中序遍历
来源：http://hz.wangshuangyany.cn/gtsasnenlw.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.c1oappe.top/gtvkwrpyyb.html

PHP:  // 手写递归函数
来源：http://hz.hywenlv.cn/gtqctordcv.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.yueranfly.top/gtozwqwgoe.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.fzhhl.top/gtgaayerqz.html

Java: // 手写递归
来源：http://hz.nanxinkj.top/gtyfpljbek.html

Go:   // 手写递归
来源：http://hz.c1oappe.top/gtnzgvqvln.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.pycfn.com/gtbixovvfs.html

C#:   // 手写递归
来源：http://hz.hfpthk.cn/gtqxklmiah.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.jinyuanbaomall.cn/gtiviflwtx.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.shuidangran.top/gtikzpkklj.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.wangshuangyany.cn/gtnueurmvy.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.shangyingyoupin.top/gthxzhlyaj.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.cashguo.top/gtelkutfjg.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.yj20258888.top/gtszytkumu.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.svipenyu.cn/gtaonnnlkh.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.hongshengwenyu.top/gtzfybrfwn.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.xuanzx.com/gtgrybvfnp.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtgxewjsdi.html

O. 并发与异步
来源：http://hz.0kj1m.cn/gtbdoqdrvj.html

================================================================================
来源：http://hz.jinqigufen.top/gtbgvfjpnk.html

[O01] 启动一个线程
来源：http://hz.ywan-chungtsiang.top/gtlxtzwvkd.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.yuanzhike.top/gtfeconwmk.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.c1oappe.top/gtnkqxkflk.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.jinqigufen.top/gtxclocztz.html

TS:   // 同 JS
来源：http://hz.ydzc1.top/gttrmoziob.html

Java: new Thread(() -> f()).start()
来源：http://hz.xinyue.icu/gtnxnwumql.html

Go:   go f()
来源：http://hz.hfpthk.cn/gtavyznnjx.html

Ruby: Thread.new { f }
来源：http://hz.jinghuilouyu.cn/gtgnfjpmdz.html

C#:   Task.Run(() => F());
来源：http://hz.shuidangran.top/gtklmynwyu.html

[O02] 使用线程池
来源：http://hz.jinyuanbaomall.cn/gtgdodzeco.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.52xcode.cn/gteixgcscz.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.ivvv.top/gtcxypfmky.html

JS:   // worker_threads 线程池
来源：http://hz.ybcxt.top/gtpqkdlage.html

TS:   // worker_threads 线程池
来源：http://hz.nwbrower.top/gtufvanioh.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.zhijiandao.cn/gtzrznifad.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.andypj.xyz/gtspikysef.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.jinyuanbaomall.cn/gtmcfyaudw.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.birdmap.top/gtxqdgozvc.html

[O03] 加锁保护共享数据
来源：http://hz.gaohongyu789.top/gtkjawspzb.html

Py:   with lock: shared += 1
来源：http://hz.fzhhl.top/gtspfngnuh.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.cheryme.top/gtnvflgfwi.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.aibaodan.cn/gthzvwrlfo.html

TS:   // 同 JS
来源：http://hz.zycfv.cn/gtvuqddadu.html

Java: synchronized (this) { shared++; }
来源：http://hz.vqdsnc.cn/gtekfdghdb.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.hysaishi.cn/gtrngevyqh.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.smart0.xyz/gtkgutqlbk.html

C#:   lock (gate) { shared++; }
来源：http://hz.yj20258888.top/gtbzfrvevx.html

[O04] 定义异步函数并等待
来源：http://hz.zycfv.cn/gtvvtaxazk.html

Py:   async def f():⏎    await g()
来源：http://hz.316326.xyz/gtfyxtzafc.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.ywan-chungtsiang.top/gtbejljmrf.html

JS:   async function f() { await g(); }
来源：http://hz.feifeiyinyue.top/gtzwzytxov.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.xylfe.cn/gttjcljkno.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.ppjwa.cn/gtoahrlaqd.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.feifeiyinyue.top/gtfzzdmuxe.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.aizwys.cn/gtgasgpihk.html

C#:   async Task F() { await G(); }
来源：http://hz.fengsongda.top/gtytaqgcyx.html

[O05] 并发执行并等待全部完成
来源：http://hz.jinyuanbaomall.cn/gtilmzjasi.html

Py:   asyncio.gather(*tasks)
来源：http://hz.daria6918.cn/gthdevxcor.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.daxiang520.top/gtxxgefgyd.html

JS:   await Promise.all(tasks)
来源：http://hz.sufxvd.cn/gtplaniwok.html

TS:   await Promise.all(tasks)
来源：http://hz.yj20258888.top/gtuhsxorup.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.fengsongda.top/gtqoadwbtx.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.shanyushiyangkeji.top/gtfmimihyl.html

Ruby: threads.map(&:join)
来源：http://hz.tianlin.xyz/gtscrtovgx.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.xziqi.cn/gtvjlkskue.html

[O06] 使用进程池
来源：http://hz.cucudq.cn/gtbuccdeyj.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.fengsongda.top/gtijezuqrk.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.xuanzx.com/gtbqibzzzu.html

JS:   // child_process / cluster 模块
来源：http://hz.daria6918.cn/gtqyiaeaum.html

TS:   // child_process / cluster 模块
来源：http://hz.hongshengwenyu.top/gtevyjfmyi.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.hysaishi.cn/gtnbztwdgt.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.nwbrower.top/gtwgszirre.html

Ruby: // fork 块
来源：http://hz.52xcode.cn/gtqcdbbjce.html

C#:   Parallel.For
来源：http://hz.sufxvd.cn/gtinwblnya.html

================================================================================
来源：http://hz.pycfn.com/gtxtjphmsk.html

P. 常用工具函数
来源：http://hz.feifeiyinyue.top/gtfyikzjyl.html

================================================================================
来源：http://hz.shuidangran.top/gtdgegzftc.html

[P01] 生成 UUID
来源：http://hz.jqgufenzy.top/gthfdzonvm.html

Py:   str(uuid.uuid4())
来源：http://hz.jyoumei.cn/gtaxgceawz.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.hnxiangtu.top/gtphryupud.html

JS:   crypto.randomUUID()
来源：http://hz.daxiang520.top/gtlkjrqkhi.html

TS:   crypto.randomUUID()
来源：http://hz.tian-w.cn/gtzpmgxtrj.html

Java: UUID.randomUUID().toString()
来源：http://hz.0kj1m.cn/gtirgmvujp.html

Go:   // 用 github.com/google/uuid
来源：http://hz.meibo888.top/gtxijopeks.html

Ruby: SecureRandom.uuid
来源：http://hz.wangdashe.top/gttqvlgkgc.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.bjfxy.top/gtkuvpnzzb.html

[P02] MD5 / SHA256 摘要
来源：http://hz.sysykeji.top/gtjodnxwph.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.zhoulong.xyz/gtshbbudwr.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.daria6918.cn/gtmqdkybri.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.shangyingyoupin.top/gtzrjdcwso.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.52xcode.cn/gtjlsdwxkg.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.cashguo.top/gtkkcenngh.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.yj20258.top/gtuqdggkoc.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.sufxvd.cn/gtjzrquckw.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.wangshuangyany.cn/gtqaamkvtq.html

[P03] 生成短随机字符串
来源：http://hz.daria6918.cn/gthiqoomaa.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.tanke756.top/gtdahzizhx.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.shanyushiyangtech.top/gttsaiwjis.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.shanyushiyangtech.top/gtiwcrxiom.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.ppjwa.cn/gtufhqruir.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.yanxiufei.cn/gtpdfobono.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.ywan-chungtsiang.top/gtdcvmyvhk.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.nanxinkj.top/gtczmronrk.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.316326.xyz/gthxatobrl.html

[P04] 求长度
来源：http://hz.9152youxi.cn/gtskrmbdlw.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.jlsjyb.cn/gtzvbeyncd.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.zhoulong.xyz/gtfobbbgic.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.shanyushiyangkeji.top/gtwvhmtlgu.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.smart0.xyz/gtlnkrtxuw.html

Java: list.size();  map.size();  s.length()
来源：http://hz.jinghuilouyu.cn/gtgpmjgrpn.html

Go:   len(arr);  len(m)
来源：http://hz.zhoulong.xyz/gtyjovkifg.html

Ruby: x.length;  x.size
来源：http://hz.yj20258888.top/gtdtqavjgb.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.shangyingyoupin.top/gtcvuxmpro.html

[P05] 判断两个对象内容是否相等
来源：http://hz.gotoacloud.top/gtffkoueik.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.cheryme.top/gtzuexxugh.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.bjfxy.top/gtablizvcu.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.yonumen.top/gtnatlsvfg.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.jlsjyb.cn/gtxeyzaeue.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.sufxvd.cn/gtnvwxzdhp.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.sufxvd.cn/gtartmsfyn.html

Ruby: a == b
来源：http://hz.havefunace.top/gteliziiyg.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.nwbrower.top/gturwvxnza.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.dashuyun.cn/gtbdwvysni.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.ehwqpu.com/gtwcdnbsia.html

PHP:  if (empty($x)) {}
来源：http://hz.ybcxt.top/gtpjlmzrqj.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.hfpthk.cn/gtosqmecdf.html

TS:   if (x == null) {}
来源：http://hz.yj202588.top/gtterglltw.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.gzhubu.top/gtccdzpenr.html

Go:   if x == nil {}
来源：http://hz.chenjidiqi.icu/gtxfifrvzt.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.feifeiyinyue.top/gtstwchyjc.html

C#:   if (x is null) {}
来源：http://hz.andypj.xyz/gtzzxeilrq.html

[P07] 防抖与节流
来源：http://hz.zdqjudy.top/gtsqjtcfch.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.yueranfly.top/gtxddhzojs.html

PHP:  // 手写时间戳比较
来源：http://hz.jqgufenzy.top/gtkkhurnnj.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.zhongyouzk.top/gtqjxwadcr.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.jqgfzy.top/gtichxvdzk.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.sysykeji.top/gtgvfsshcp.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.xinyue.icu/gtdmgxmsbf.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.chenzaomai.com/gtdwwlunas.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.mhx1999.top/gtmxhvvjwd.html

[P08] 处理浮点精度问题
来源：http://hz.fzhhl.top/gtaxsfxwsl.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.gzhubu.top/gtvdxdejlp.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.chenlongwang.top/gtqryfuisc.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.hywenlv.cn/gtvwyqsvvw.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.yj20258888.top/gtrxrooazx.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.hammf.cn/gtyzuqlazc.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.daxiang520.top/gtdfqcugck.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.shanyushiyangtech.top/gtqoostfbq.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.jinghuilouyu.cn/gtnipbqryb.html

================================================================================
来源：http://hz.shzxlz.cn/gtfodnlhmy.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.0kj1m.cn/gtepmetkip.html

================================================================================
来源：http://hz.yongpay.top/gtyczepycd.html

[Q01] 创建表
来源：http://hz.zdqjudy.top/gtmqgeubkc.html

CREATE TABLE users (
来源：http://hz.feifeiyinyue.top/gtussoobjs.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.haohaochexian.top/gtnqpdbpxh.html

name VARCHAR(50) NOT NULL,
来源：http://hz.wangdashe.top/gtqcsqyyeo.html

email VARCHAR(100) UNIQUE,
来源：http://hz.svipenyu.cn/gtzwwqeojm.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.vqdsnc.cn/gttjtxtmsh.html

);
来源：http://hz.yj20258888.top/gteujiwlce.html

[Q02] 创建带外键的表
来源：http://hz.chenlongwang.top/gtvuhlojeo.html

CREATE TABLE orders (
来源：http://hz.jqgfzy.top/gtjmkieqqd.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.gaohongyu789.top/gtwtucxkyh.html

user_id INT NOT NULL,
来源：http://hz.jiagoushi.top/gtuqwdqdjd.html

amount DECIMAL(10, 2),
来源：http://hz.ppjwa.cn/gtmiaxffbf.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.0kj1m.cn/gtjizrirrm.html

);
来源：http://hz.tanke756.top/gttszluwwy.html

[Q03] 增加列
来源：http://hz.sufxvd.cn/gtnsjmfoed.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.iojbl.cn/gthmvyfjhz.html

[Q04] 修改列类型
来源：http://hz.chenzaomai.com/gtzadahmbw.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.cheryme.top/gtafhkovej.html

[Q05] 重命名列
来源：http://hz.zycfv.cn/gtuvvwoxon.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.tian-w.cn/gtjicflzkg.html

[Q06] 删除列
来源：http://hz.guannengcc.top/gtmjarfgog.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.chenzaomai.com/gtvysygmhm.html

[Q07] 删除表
来源：http://hz.jinqigfzy.top/gtkjyvpkzi.html

DROP TABLE IF EXISTS orders;
来源：http://hz.hammf.cn/gttrlbygmx.html

[Q08] 创建普通索引
来源：http://hz.yangfankeji.com/gtmdhzdcut.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.yuxming.cn/gtjawtbmpq.html

[Q09] 创建唯一索引
来源：http://hz.daxiang520.top/gtjojcfjcg.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.smart0.xyz/gtcukvvqio.html

[Q10] 插入单行
来源：http://hz.gotoacloud.top/gthqmpjwdw.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.haohaochexian.top/gtszcpqyjk.html

[Q11] 一次插入多行
来源：http://hz.zhiwuduotai.top/gtytmdpfmq.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.zhijiandao.cn/gthznibrkc.html

[Q12] 插入后取自增 ID
来源：http://hz.shuidangran.top/gtukimgrfr.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.zhijiandao.cn/gtrwmfkobe.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.gotoacloud.top/gttrzbuyva.html

[Q13] 忽略重复插入
来源：http://hz.dianchejie.cn/gtkiojdvow.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.mhx1999.top/gtdysvolmg.html

[Q14] 存在则更新（upsert）
来源：http://hz.havefunace.top/gtrcttyvzj.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.cheryme.top/gtkwktdail.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.yongpay.top/gtxrtzzcxf.html

[Q15] 查询全部
来源：http://hz.yueranfly.top/gtsybbjpna.html

SELECT * FROM users;
来源：http://hz.guannengcc.top/gtqvmwkpys.html

[Q16] 查询指定列
来源：http://hz.kuanghao11.cn/gtaffkilej.html

SELECT id, name FROM users;
来源：http://hz.xinyue.icu/gtfvtcpvkd.html

[Q17] 条件查询
来源：http://hz.sysykeji.top/gtmzzpprql.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.316326.xyz/gtlmtkczyq.html

[Q18] 模糊匹配
来源：http://hz.yonumen.top/gtcnwdwvtx.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.snrcjt.cn/gtmckysnaq.html

[Q19] 范围查询
来源：http://hz.chenlongwang.top/gtsmiraqub.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.xuetiantiany.cn/gtxwyvicyi.html

[Q20] IN 列表
来源：http://hz.xuanzx.com/gtpqlzoxbu.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.sufxvd.cn/gtslgqewxx.html

[Q21] 空值判断
来源：http://hz.cqqwz.cn/gtvofevnfv.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.hnxiangtu.top/gtkfdiwtfn.html

[Q22] 排序
来源：http://hz.shanyushiyangkeji.top/gtlxzqfkij.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.shuidangran.top/gtxvpcmbgm.html

[Q23] 分页
来源：http://hz.xuetiantiany.cn/gtqxnuldoz.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.andypj.xyz/gtabrbibfk.html

[Q24] 去重
来源：http://hz.aibaodan.cn/gtbkyxyhnn.html

SELECT DISTINCT city FROM users;
来源：http://hz.yanxiufei.cn/gthwifsnty.html

[Q25] 只取前 N 条
来源：http://hz.zhixingplan.top/gteoendtrz.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.xinyue.icu/gtfgemnphq.html

[Q26] 计数
来源：http://hz.zhengqikj.top/gtawtmzqhu.html

SELECT COUNT(*) FROM users;
来源：http://hz.pycfn.com/gtmdljvtgk.html

[Q27] 条件计数
来源：http://hz.zhijiandao.cn/gtskzzlfjp.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.aizwys.cn/gtgkmlyhni.html

[Q28] 求和与平均
来源：http://hz.shangyingyoupin.top/gtqxaikiap.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.zhoulong.xyz/gtejncgvci.html

[Q29] 最大最小值
来源：http://hz.jinqigufen.top/gtajckvgcr.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.yongpay.top/gtdamicixy.html

[Q30] 分组统计
来源：http://hz.guannengcc.top/gtlepqrlkq.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.hywenlv.cn/gtvldgwblw.html

[Q31] 分组后过滤
来源：http://hz.yj20258888.top/gtwmueshbg.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.ppjwa.cn/gtwtyjvzuq.html

[Q32] 分组拼接字符串
来源：http://hz.jianghu66.top/gtcrldatzv.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.pycfn.com/gtmykrryki.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.sysykeji.top/gtkbhwqxmb.html

[Q33] 多列分组
来源：http://hz.chenjidiqi.icu/gtnoqhffaa.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.daxiang520.top/gtdqhcmkjh.html

[Q34] 每组取第一条
来源：http://hz.pycfn.com/gtqklghmsu.html

SELECT * FROM (
来源：http://hz.0kj1m.cn/gtmbgxyxxd.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.gzhubu.top/gtoyhqxyhx.html

) t WHERE rn = 1;
来源：http://hz.jiagoushi.top/gtnpxdnlqs.html

[Q35] 内连接
来源：http://hz.wangshuangyany.cn/gtxghvqlbg.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.yj20258888.top/gtfayxwmwz.html

[Q36] 左连接
来源：http://hz.jinyuanbaomall.cn/gtyphpjgwf.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.chenlongwang.top/gtreiamaqz.html

[Q37] 右连接
来源：http://hz.nanxinkj.top/gtyivaywlb.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.nanxuanxn.top/gttwegfnuv.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.pengpengdd.cyou/gtbcyipzti.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.vqdsnc.cn/gthjirfldg.html

[Q39] 自连接（查上下级）
来源：http://hz.zycfv.cn/gtuqqcpodc.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.iojbl.cn/gtfdlbmzzv.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.gotoacloud.top/gtaqdufjii.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.nanxuanxn.top/gtfkzipjiw.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.9152youxi.cn/gtahjfblmi.html

[Q41] 多表连接
来源：http://hz.tian-w.cn/gttopgxtcw.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.ydzc1.top/gttqigypgd.html

JOIN users u ON u.id = o.user_id
来源：http://hz.shangyingyoupin.top/gtsrsmwhvy.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.quarkkingdee.top/gthiuzptqb.html

[Q42] 连接条件附加过滤
来源：http://hz.sysykeji.top/gtpfzyvrso.html

SELECT u.name, o.amount FROM users u
来源：http://hz.gaohongyu789.top/gtqjapdoet.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.tianlin.xyz/gtgxqtylgl.html

[Q43] 标量子查询
来源：http://hz.zhiwuduotai.top/gtqxvvxrza.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.sxryk.cn/gtsdeyrnby.html

[Q44] IN 子查询
来源：http://hz.316326.xyz/gtzjzgawaw.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.yongpay.top/gtutrhbigt.html

[Q45] EXISTS 判断存在
来源：http://hz.tanke756.top/gtyogaswtu.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.shzxlz.cn/gtnmqzuolt.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.yuanzhike.top/gtvpggbvfa.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.xuanzx.com/gtxcvflyfo.html

[Q47] 与平均值比较
来源：http://hz.xuanzx.com/gthszigyfx.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.kuanghao11.cn/gtajdrnbsc.html

[Q48] CTE 公用表表达式
来源：http://hz.ivvv.top/gtcqtgspyp.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.yj20258.top/gtlzlvzhsa.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.ehwqpu.com/gtrgqeuter.html

[Q49] 更新单行
来源：http://hz.iojbl.cn/gtafpopuet.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.quarkkingdee.top/gtcovacvcu.html

[Q50] 批量更新
来源：http://hz.redwolf501.top/gtcmjiuxur.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.jinqigfzy.top/gtysozzqlw.html

[Q51] 用子查询更新
来源：http://hz.hnqzz.top/gtbjuzdevk.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.jinghuilouyu.cn/gtbgfwamzg.html

[Q52] 删除指定行
来源：http://hz.jianghu66.top/gtpslsvode.html

DELETE FROM users WHERE id = 10;
来源：http://hz.pengpengdd.cyou/gtngxmlohk.html

[Q53] 按条件删除
来源：http://hz.chenzaomai.com/gtwlmhuahh.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.zhijiandao.cn/gtzbjxjxkj.html

[Q54] 清空表
来源：http://hz.sysykeji.top/gtjiwnywmn.html

TRUNCATE TABLE logs;
来源：http://hz.xuetiantiany.cn/gtjyarwlex.html

[Q55] 排名（并列占位）
来源：http://hz.zhongyouzk.top/gtwbbykjox.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.zhengqikj.top/gtwtcfiohu.html

[Q56] 密集排名（并列不占位）
来源：http://hz.jinyuanbaomall.cn/gtatpqmsyd.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.zhengqikj.top/gtigrmwcpg.html

[Q57] 行号
来源：http://hz.ywan-chungtsiang.top/gtyisofpnh.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.chenjidiqi.icu/gtmmqefvqt.html

[Q58] 累计求和
来源：http://hz.andypj.xyz/gtuzwlkzau.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.redwolf501.top/gtjutjllid.html

[Q59] 分组内累计
来源：http://hz.bjfxy.top/gtwkuhswht.html


<!-- 参考信息 -->