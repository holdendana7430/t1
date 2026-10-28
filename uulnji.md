代发 wailian999

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.zhongyouzk.top/gtrwaumbbz.html

[N10] 链表节点定义
来源：http://hz.tanke756.top/gtzdxjgdlm.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.cdnleiting.top/gtkcckdcej.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.nwbrower.top/gtpxqqlrnu.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.cqqwz.cn/gtcyayxefa.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.c1oappe.top/gtmyuzcvwg.html

Java: class Node { int v; Node next; }
来源：http://hz.sweek.top/gtacesfsgn.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.iojbl.cn/gtioqyrdld.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.yj202588.top/gtxoccogas.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.zycfv.cn/gtibhgnufz.html

[N11] 二叉树中序遍历
来源：http://hz.yuxming.cn/gtrsugoqbn.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.sxryk.cn/gtrnxuvhus.html

PHP:  // 手写递归函数
来源：http://hz.xingfuxueyuan.xyz/gtggspible.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.jinghuilouyu.cn/gtgucazjhz.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.shanyushiyangkeji.top/gtczambrir.html

Java: // 手写递归
来源：http://hz.jyoumei.cn/gtqnwyqjrp.html

Go:   // 手写递归
来源：http://hz.xziqi.cn/gtzblizylw.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.jqgfzy.top/gtrqlkncai.html

C#:   // 手写递归
来源：http://hz.jinyuanbaomall.cn/gtjkpqmeib.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.yanxiufei.cn/gtcfbjetil.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.andypj.xyz/gtrxlyyjob.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.pycfn.com/gtrwmoxehs.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.shzxlz.cn/gtenanvedc.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.guannengcc.top/gtptkynvue.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.jinqigufen.top/gtzxiqbnjh.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.jqgufenzy.top/gtvjorjadn.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.jinghuilouyu.cn/gtpzhacusf.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.zhengqikj.top/gthtiwkvdj.html

================================================================================
来源：http://hz.svipenyu.cn/gtlcakbtea.html

O. 并发与异步
来源：http://hz.kuanghao11.cn/gtvpnfpwaq.html

================================================================================
来源：http://hz.mhx1999.top/gtmpnoalil.html

[O01] 启动一个线程
来源：http://hz.feifeiyinyue.top/gtcygdiqmf.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.aibaodan.cn/gtobwfeowa.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.yongpay.top/gtdsnuyhtn.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.gzhubu.top/gtwudwvfdi.html

TS:   // 同 JS
来源：http://hz.shuidangran.top/gtflafnvdf.html

Java: new Thread(() -> f()).start()
来源：http://hz.xuanzx.com/gtgkornuea.html

Go:   go f()
来源：http://hz.hammf.cn/gtcldyfjds.html

Ruby: Thread.new { f }
来源：http://hz.nanxinkj.top/gthkymhsbs.html

C#:   Task.Run(() => F());
来源：http://hz.ehwqpu.com/gtlxbipwww.html

[O02] 使用线程池
来源：http://hz.zhengqikj.top/gtqdsfkloy.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.yuxming.cn/gtkwfbjlen.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.redwolf501.top/gtypfolbds.html

JS:   // worker_threads 线程池
来源：http://hz.nwbrower.top/gtwlyhyzst.html

TS:   // worker_threads 线程池
来源：http://hz.havefunace.top/gtbtpkqqdp.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.hammf.cn/gtvcfjqffv.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.shanyushiyangkeji.top/gtbjlxlpiw.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.zhoulong.xyz/gtedvfmbna.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.guannengcc.top/gtngwxsuzr.html

[O03] 加锁保护共享数据
来源：http://hz.fzhhl.top/gtuxrxukft.html

Py:   with lock: shared += 1
来源：http://hz.jyoumei.cn/gtkqmlcyog.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.shuidangran.top/gtbzibblld.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.yangfankeji.com/gtcdetwwlq.html

TS:   // 同 JS
来源：http://hz.svipenyu.cn/gtwtghsbaj.html

Java: synchronized (this) { shared++; }
来源：http://hz.guowangkeji.top/gtznopiffa.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.ppjwa.cn/gtidkuqgwl.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.jqgufenzy.top/gtxeevgxpi.html

C#:   lock (gate) { shared++; }
来源：http://hz.jinqigufen.top/gtlqlmkmvv.html

[O04] 定义异步函数并等待
来源：http://hz.shanyushiyangkeji.top/gtdepyavcz.html

Py:   async def f():⏎    await g()
来源：http://hz.feifeiyinyue.top/gtwrzqhosg.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.yueranfly.top/gtctzqbldr.html

JS:   async function f() { await g(); }
来源：http://hz.ybcxt.top/gtojmwlroz.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.jinghuilouyu.cn/gthmrbkzem.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.hammf.cn/gtdfqlgkzk.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.jianghu66.top/gtwdvppwvt.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.bjfxy.top/gtuxwxcmbk.html

C#:   async Task F() { await G(); }
来源：http://hz.jianghu66.top/gtzjruqdlu.html

[O05] 并发执行并等待全部完成
来源：http://hz.shanyushiyangkeji.top/gtsngxrokj.html

Py:   asyncio.gather(*tasks)
来源：http://hz.hnqzz.top/gtorquzwhg.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.ywan-chungtsiang.top/gtuyyjadjb.html

JS:   await Promise.all(tasks)
来源：http://hz.wangshuangyany.cn/gtzqiepdci.html

TS:   await Promise.all(tasks)
来源：http://hz.ydjk.org.cn/gtcliexuwx.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.aibaodan.cn/gtjszefrjh.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.cheryme.top/gtvwcpvrzq.html

Ruby: threads.map(&:join)
来源：http://hz.iojbl.cn/gtbckubkgt.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.shanyushiyangtech.top/gtfgsqshpd.html

[O06] 使用进程池
来源：http://hz.andypj.xyz/gttetnlqmo.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.xinyue.icu/gtlaqlvzmk.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.yongpay.top/gtdzhtgdqg.html

JS:   // child_process / cluster 模块
来源：http://hz.jyoumei.cn/gtqxtfrepu.html

TS:   // child_process / cluster 模块
来源：http://hz.ppjwa.cn/gtewuwiqsl.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.9152youxi.cn/gtoaeekcav.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.fengsongda.top/gthsljlmtq.html

Ruby: // fork 块
来源：http://hz.kuanghao11.cn/gthiuehpsz.html

C#:   Parallel.For
来源：http://hz.jinqigufen.top/gttzgyvpau.html

================================================================================
来源：http://hz.iojbl.cn/gtgrxuapdd.html

P. 常用工具函数
来源：http://hz.hysaishi.cn/gtqcacaaeu.html

================================================================================
来源：http://hz.cdnleiting.top/gtczkirguw.html

[P01] 生成 UUID
来源：http://hz.yj20258888.top/gthfttjncy.html

Py:   str(uuid.uuid4())
来源：http://hz.jinyuanbaomall.cn/gtivuewixq.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.c1oappe.top/gtlzofzsuh.html

JS:   crypto.randomUUID()
来源：http://hz.cheryme.top/gtrxealgib.html

TS:   crypto.randomUUID()
来源：http://hz.kuanghao11.cn/gtsmnhvxvi.html

Java: UUID.randomUUID().toString()
来源：http://hz.shanyushiyangtech.top/gtymkgotap.html

Go:   // 用 github.com/google/uuid
来源：http://hz.ybcxt.top/gtbofrniqa.html

Ruby: SecureRandom.uuid
来源：http://hz.fengsongda.top/gtkrebletd.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.yueranfly.top/gtzlitemmg.html

[P02] MD5 / SHA256 摘要
来源：http://hz.aibaodan.cn/gtldbokjjc.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.ppjwa.cn/gtnhlcizdc.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.ehwqpu.com/gtdtdumlkl.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.yj20258.top/gtzyonjvaq.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.tanke756.top/gtvixzfizb.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.9152youxi.cn/gtkwgxhkjo.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.sysykeji.top/gtjqfbzbnd.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.ybcxt.top/gtrytcwpdw.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.feifeiyinyue.top/gtsoyuxavx.html

[P03] 生成短随机字符串
来源：http://hz.vqdsnc.cn/gtozlaifwp.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.dashuyun.cn/gtazzvhlkv.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.316326.xyz/gtjsnqqtik.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.jinqigufen.top/gtzvwbgmhr.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.hfpthk.cn/gtmqpkhqss.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.xuetiantiany.cn/gtjpiympzx.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.aibaodan.cn/gtyfwrhmyx.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.iojbl.cn/gtdxodegpo.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.xinyue.icu/gtwmmomvzy.html

[P04] 求长度
来源：http://hz.jinqigufen.top/gtzfjwqync.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.xinyue.icu/gtgpmouzta.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.jinyuanbaomall.cn/gtnmaksfpv.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.zdqjudy.top/gtlrrgjxob.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.zhijiandao.cn/gtwqepfvkk.html

Java: list.size();  map.size();  s.length()
来源：http://hz.zhaomingkeji.xyz/gtnanyuosi.html

Go:   len(arr);  len(m)
来源：http://hz.yj202588.top/gtqlnzkidv.html

Ruby: x.length;  x.size
来源：http://hz.xinyue.icu/gtvbmbmdsn.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.jinqigfzy.top/gthxdrusps.html

[P05] 判断两个对象内容是否相等
来源：http://hz.gaohongyu789.top/gtggggvrrw.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.chenjidiqi.icu/gtjfbchnjz.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.gzhubu.top/gthoxnmaom.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.mhx1999.top/gtkaethyxy.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.jqgfzy.top/gtgiqzkgmr.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.sxryk.cn/gtjpbkwulg.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.kuanghao11.cn/gtzmmgzlhg.html

Ruby: a == b
来源：http://hz.52xcode.cn/gtfufuxpic.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.shanyushiyangkeji.top/gtvedfahac.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.svipenyu.cn/gtaatjpfmd.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.shzxlz.cn/gtdbpdixad.html

PHP:  if (empty($x)) {}
来源：http://hz.kuanghao11.cn/gthnkhofup.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.hammf.cn/gtgsbnkbsa.html

TS:   if (x == null) {}
来源：http://hz.hysaishi.cn/gtzwjvkycs.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.hnqzz.top/gtcuvpzyuf.html

Go:   if x == nil {}
来源：http://hz.chenlongwang.top/gtrmfgvten.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.jyoumei.cn/gtdlwvoovt.html

C#:   if (x is null) {}
来源：http://hz.zhiwuduotai.top/gtabrinvym.html

[P07] 防抖与节流
来源：http://hz.snrcjt.cn/gtvmxijvot.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.9152youxi.cn/gtzxxbiznv.html

PHP:  // 手写时间戳比较
来源：http://hz.chenlongwang.top/gtkgebonym.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.0kj1m.cn/gtezyjfvpk.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.ybcxt.top/gtckgkxego.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.hongshengwenyu.top/gtmcjmanmm.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.tian-w.cn/gtscdtrxxg.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.yangfankeji.com/gtwfzgychl.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.dianchejie.cn/gtqhdegfci.html

[P08] 处理浮点精度问题
来源：http://hz.iojbl.cn/gtbjiniaaa.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.9152youxi.cn/gtzqboetvq.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.yuanzhike.top/gtluumbfks.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.gzhubu.top/gtxsfeehkq.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.chenjidiqi.icu/gthkzqkmjl.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.jlsjyb.cn/gtumzylypb.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.yongpay.top/gtblxmgdtr.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.jinqigfzy.top/gtyhjyzspr.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.chenlongwang.top/gtbmhvvodk.html

================================================================================
来源：http://hz.zycfv.cn/gtqmxfikze.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.tanke756.top/gtcaubzwmh.html

================================================================================
来源：http://hz.xylfe.cn/gtlljcdiox.html

[Q01] 创建表
来源：http://hz.yongpay.top/gtvcdxxbkg.html

CREATE TABLE users (
来源：http://hz.redwolf501.top/gtldkueyjr.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.aibaodan.cn/gtnzydodvb.html

name VARCHAR(50) NOT NULL,
来源：http://hz.jyoumei.cn/gtrlkvdgky.html

email VARCHAR(100) UNIQUE,
来源：http://hz.zhongyouzk.top/gtsbxyahjo.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.yvedp.cn/gtifadmwce.html

);
来源：http://hz.0kj1m.cn/gtwrkdnoxf.html

[Q02] 创建带外键的表
来源：http://hz.xylfe.cn/gtckwjbzqz.html

CREATE TABLE orders (
来源：http://hz.52xcode.cn/gttdeweivu.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.nanxuanxn.top/gtlffhjjun.html

user_id INT NOT NULL,
来源：http://hz.yanxiufei.cn/gtgapjabxo.html

amount DECIMAL(10, 2),
来源：http://hz.jinqigfzy.top/gtbfhzsffo.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.yonumen.top/gtfyurhqew.html

);
来源：http://hz.tanke756.top/gtsstulcmz.html

[Q03] 增加列
来源：http://hz.guowangkeji.top/gtaclbqznl.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.tian-w.cn/gthgixyyrt.html

[Q04] 修改列类型
来源：http://hz.nwbrower.top/gthzexeisd.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.shuidangran.top/gtfoqefhmv.html

[Q05] 重命名列
来源：http://hz.pycfn.com/gtnrkbdsbq.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.zhiwuduotai.top/gtynolsiwi.html

[Q06] 删除列
来源：http://hz.bjfxy.top/gtclalhxlv.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.pengpengdd.cyou/gtvsewecau.html

[Q07] 删除表
来源：http://hz.iojbl.cn/gttvhvohgg.html

DROP TABLE IF EXISTS orders;
来源：http://hz.hysaishi.cn/gtqxpqekgn.html

[Q08] 创建普通索引
来源：http://hz.cheryme.top/gtmrjrxujr.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.havefunace.top/gtqimrwwtv.html

[Q09] 创建唯一索引
来源：http://hz.yj20258.top/gtlmorxfeh.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.sysykeji.top/gtdbgqumki.html

[Q10] 插入单行
来源：http://hz.yanxiufei.cn/gtfcnqxdwe.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.zhengqikj.top/gtndlrtnji.html

[Q11] 一次插入多行
来源：http://hz.tanke756.top/gthwtiblyn.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.shanyushiyangtech.top/gtbqhbqbwz.html

[Q12] 插入后取自增 ID
来源：http://hz.svipenyu.cn/gttniolpah.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.zdqjudy.top/gtlijzmkmf.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.hammf.cn/gtrsawgktb.html

[Q13] 忽略重复插入
来源：http://hz.svipenyu.cn/gtzxqtratv.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.guowangkeji.top/gtufnygxxk.html

[Q14] 存在则更新（upsert）
来源：http://hz.zhixingplan.top/gtyzcsghei.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.yanxiufei.cn/gtntfletkc.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.gaohongyu789.top/gtgjuaimpf.html

[Q15] 查询全部
来源：http://hz.feifeiyinyue.top/gtucdmjpbs.html

SELECT * FROM users;
来源：http://hz.yvedp.cn/gtwvyeqdeu.html

[Q16] 查询指定列
来源：http://hz.zhixingplan.top/gtnpxzfzlu.html

SELECT id, name FROM users;
来源：http://hz.daria6918.cn/gtauxvhrgi.html

[Q17] 条件查询
来源：http://hz.sxryk.cn/gttqqlpxob.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.yj20258888.top/gtkdbkscsd.html

[Q18] 模糊匹配
来源：http://hz.nwbrower.top/gtinkljyjl.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.sufxvd.cn/gtcxwdtumw.html

[Q19] 范围查询
来源：http://hz.fengsongda.top/gthzjsmsnn.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.jinqigfzy.top/gtwstvxfey.html

[Q20] IN 列表
来源：http://hz.sufxvd.cn/gtaoyrbiwo.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.iojbl.cn/gtlvjkijzu.html

[Q21] 空值判断
来源：http://hz.zhixingplan.top/gtdqdswadv.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.ppjwa.cn/gttulwrzpm.html

[Q22] 排序
来源：http://hz.zhiwuduotai.top/gtuhecdobj.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.52xcode.cn/gtuwglhsvl.html

[Q23] 分页
来源：http://hz.hfpthk.cn/gtmmtbifnq.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.zhoulong.xyz/gtjfjmzucd.html

[Q24] 去重
来源：http://hz.zhongyouzk.top/gtljuyjcos.html

SELECT DISTINCT city FROM users;
来源：http://hz.havefunace.top/gtsmhypjui.html

[Q25] 只取前 N 条
来源：http://hz.mhx1999.top/gtfsfcvzsz.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.jqgufenzy.top/gtqnixhfrb.html

[Q26] 计数
来源：http://hz.xuanzx.com/gtfisrstqp.html

SELECT COUNT(*) FROM users;
来源：http://hz.fengsongda.top/gthgoghbft.html

[Q27] 条件计数
来源：http://hz.yj20258888.top/gteehgpukw.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.hnqzz.top/gtfzeckzeh.html

[Q28] 求和与平均
来源：http://hz.52xcode.cn/gtjrbgedmc.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.smart0.xyz/gtyjoglvwo.html

[Q29] 最大最小值
来源：http://hz.kuanghao11.cn/gtxugudahs.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.shanyushiyangkeji.top/gthwrkiwee.html

[Q30] 分组统计
来源：http://hz.jiagoushi.top/gtvhlcswxj.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.gzhubu.top/gtqniiwejm.html

[Q31] 分组后过滤
来源：http://hz.wangshuangyany.cn/gtjjrwheij.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.ehwqpu.com/gthmybatpi.html

[Q32] 分组拼接字符串
来源：http://hz.0kj1m.cn/gtehyvizlf.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.chenlongwang.top/gtsfbdgkbs.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.fengsongda.top/gtmalhmvam.html

[Q33] 多列分组
来源：http://hz.shuidangran.top/gthcgeemrl.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.guannengcc.top/gtkdsraclk.html

[Q34] 每组取第一条
来源：http://hz.hywenlv.cn/gtstewsxqt.html

SELECT * FROM (
来源：http://hz.chenjidiqi.icu/gtearrwqxi.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.bjfxy.top/gtszcsjsts.html

) t WHERE rn = 1;
来源：http://hz.zhaomingkeji.xyz/gtnkadosrs.html

[Q35] 内连接
来源：http://hz.pengpengdd.cyou/gtfqqxypev.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.jianghu66.top/gtmhnfcqte.html

[Q36] 左连接
来源：http://hz.zhoulong.xyz/gthkklbbbr.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.sufxvd.cn/gtfncchhrd.html

[Q37] 右连接
来源：http://hz.shanyushiyangkeji.top/gtmcdzoaqh.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.cdnleiting.top/gtoaicylja.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.chenlongwang.top/gtqjlsitml.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.aizwys.cn/gtsnuillpm.html

[Q39] 自连接（查上下级）
来源：http://hz.ydjk.org.cn/gtxfkvbovc.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.daxiang520.top/gtriushnqs.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.hfpthk.cn/gtvwqlzmtz.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.guowangkeji.top/gtghrcgbmh.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.9152youxi.cn/gtpvczbrpk.html

[Q41] 多表连接
来源：http://hz.meibo888.top/gtxduyzstm.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.ydjk.org.cn/gtawkkuavh.html

JOIN users u ON u.id = o.user_id
来源：http://hz.zhiwuduotai.top/gtbzulveuf.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.andypj.xyz/gtbncmncax.html

[Q42] 连接条件附加过滤
来源：http://hz.aizwys.cn/gtgsyvzffe.html

SELECT u.name, o.amount FROM users u
来源：http://hz.zhengqikj.top/gthpkoseyx.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.svipenyu.cn/gtbkrhgevc.html

[Q43] 标量子查询
来源：http://hz.tanke756.top/gthvljycve.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.birdmap.top/gtdupedltp.html

[Q44] IN 子查询
来源：http://hz.xziqi.cn/gtoiiuhzfe.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.shanyushiyangkeji.top/gtfctnfivt.html

[Q45] EXISTS 判断存在
来源：http://hz.hnxiangtu.top/gtqkthuvbo.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.yvedp.cn/gtuonjctfk.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.kuanghao11.cn/gtskgihpsu.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.zhaomingkeji.xyz/gtgpdakcks.html

[Q47] 与平均值比较
来源：http://hz.sxryk.cn/gtfrvcevur.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.jinghuilouyu.cn/gtpugczkgy.html

[Q48] CTE 公用表表达式
来源：http://hz.zhiwuduotai.top/gtfjwljsud.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.yj202588.top/gtzwzvcudf.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.zhoulong.xyz/gtjyrpvjhi.html

[Q49] 更新单行
来源：http://hz.ivvv.top/gtmyugojrn.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.yonumen.top/gtykoeelma.html

[Q50] 批量更新
来源：http://hz.xingfuxueyuan.xyz/gtaeydyjiu.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.xuetiantiany.cn/gtlzariunc.html

[Q51] 用子查询更新
来源：http://hz.aizwys.cn/gtelrlssjs.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.redwolf501.top/gtvjxuotqf.html

[Q52] 删除指定行
来源：http://hz.aizwys.cn/gtqwearqmq.html

DELETE FROM users WHERE id = 10;
来源：http://hz.aizwys.cn/gtaiybuppf.html

[Q53] 按条件删除
来源：http://hz.nanxuanxn.top/gtndvgvmju.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.hnqzz.top/gtxghupuye.html

[Q54] 清空表
来源：http://hz.haohaochexian.top/gtccqqdprm.html

TRUNCATE TABLE logs;
来源：http://hz.jiagoushi.top/gtrgbyqmdg.html

[Q55] 排名（并列占位）
来源：http://hz.yuanzhike.top/gtpwbxrewe.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.jiagoushi.top/gttfwxazmb.html

[Q56] 密集排名（并列不占位）
来源：http://hz.xinyue.icu/gtmwmmoose.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.yj202588.top/gtmwoahxyr.html

[Q57] 行号
来源：http://hz.hnxiangtu.top/gtkrodiswg.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.zhongyouzk.top/gtxuxqnkvj.html

[Q58] 累计求和
来源：http://hz.0kj1m.cn/gtswyzrbut.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.svipenyu.cn/gtlyzsgeio.html

[Q59] 分组内累计
来源：http://hz.yangfankeji.com/gtlhidpgdl.html


<!-- 参考信息 -->