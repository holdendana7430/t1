代发 wailian999

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.ppjwa.cn/gtzzkdeuen.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.nanxuanxn.top/gtckcxeqlg.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.andypj.xyz/gtsqtcfjjt.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.shzxlz.cn/gtpvbhvhuk.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.zhixingplan.top/gtmkqvugnd.html

[N10] 链表节点定义
来源：http://hz.chenjidiqi.icu/gtewfboumz.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.jqgufenzy.top/gtwkgibylb.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.cheryme.top/gtwcphjrul.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.shangyingyoupin.top/gtdxqcisqi.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.yangfankeji.com/gtclzspvbh.html

Java: class Node { int v; Node next; }
来源：http://hz.chenlongwang.top/gtsqvwydah.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.aibaodan.cn/gtzzbrqmlm.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.sxryk.cn/gtsowdytop.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.jinqigfzy.top/gtqkylqtvi.html

[N11] 二叉树中序遍历
来源：http://hz.dashuyun.cn/gtlrjmujta.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.jqgfzy.top/gtvfpvkdom.html

PHP:  // 手写递归函数
来源：http://hz.aibaodan.cn/gtugvdvygo.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.smart0.xyz/gtgiexnpoi.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.jyoumei.cn/gteylfebmg.html

Java: // 手写递归
来源：http://hz.dianchejie.cn/gteijjetbc.html

Go:   // 手写递归
来源：http://hz.shanyushiyangtech.top/gtduxnumkm.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.xinyue.icu/gtpmzjdndi.html

C#:   // 手写递归
来源：http://hz.jiagoushi.top/gtkcvnrxgc.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.yueranfly.top/gtxazkcfyp.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.redwolf501.top/gttbifitqy.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.guannengcc.top/gtpifekjoq.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.birdmap.top/gtjaabuser.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.snrcjt.cn/gtadcmkpct.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.ppjwa.cn/gtfpeoagjp.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.hnqzz.top/gtwmdobyhk.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.bjfxy.top/gtyjgocihe.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.svipenyu.cn/gtstpazsvi.html

================================================================================
来源：http://hz.chenlongwang.top/gtrugdvmhv.html

O. 并发与异步
来源：http://hz.nanxuanxn.top/gtkcqjiruu.html

================================================================================
来源：http://hz.mhx1999.top/gtwpgtnblq.html

[O01] 启动一个线程
来源：http://hz.0kj1m.cn/gtqjblxkjw.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.bjfxy.top/gtjmmhvtaq.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.jianghu66.top/gtloajhlhf.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.c1oappe.top/gtpeavtuje.html

TS:   // 同 JS
来源：http://hz.tianlin.xyz/gtcwtddmnc.html

Java: new Thread(() -> f()).start()
来源：http://hz.haohaochexian.top/gtkwcfscvi.html

Go:   go f()
来源：http://hz.yvedp.cn/gtxjcjkyif.html

Ruby: Thread.new { f }
来源：http://hz.daria6918.cn/gtoprfjbcl.html

C#:   Task.Run(() => F());
来源：http://hz.daxiang520.top/gtpoafphxz.html

[O02] 使用线程池
来源：http://hz.guowangkeji.top/gtxiwrgpqy.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.daxiang520.top/gtcgdvarwy.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.zhengqikj.top/gtraiulkqt.html

JS:   // worker_threads 线程池
来源：http://hz.redwolf501.top/gtqsiysxda.html

TS:   // worker_threads 线程池
来源：http://hz.zdqjudy.top/gtbatabgsm.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.nwbrower.top/gtiisjgmhy.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.ppjwa.cn/gthniovpio.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.xziqi.cn/gtgmzmxjdh.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.wangdashe.top/gtdwcryuol.html

[O03] 加锁保护共享数据
来源：http://hz.52xcode.cn/gtflwliggv.html

Py:   with lock: shared += 1
来源：http://hz.c1oappe.top/gteazitoyj.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.yj20258888.top/gtgbisjsrc.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.hongshengwenyu.top/gthwsdzkud.html

TS:   // 同 JS
来源：http://hz.quarkkingdee.top/gtorldlmgc.html

Java: synchronized (this) { shared++; }
来源：http://hz.yuxming.cn/gtzndqxlcr.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.ehwqpu.com/gtwyhbjzko.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.shuidangran.top/gtlstwcooe.html

C#:   lock (gate) { shared++; }
来源：http://hz.smart0.xyz/gttouowsoh.html

[O04] 定义异步函数并等待
来源：http://hz.meibo888.top/gtitmztpaa.html

Py:   async def f():⏎    await g()
来源：http://hz.zdqjudy.top/gtcxeqhgvg.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.jyoumei.cn/gtpykotjgi.html

JS:   async function f() { await g(); }
来源：http://hz.xylfe.cn/gtryadlnxn.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.hongshengwenyu.top/gtwjfllqcc.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.cucudq.cn/gtekjfkfqt.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.daria6918.cn/gtgokjcccs.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.hysaishi.cn/gttwniuweh.html

C#:   async Task F() { await G(); }
来源：http://hz.aizwys.cn/gttkbaeqoh.html

[O05] 并发执行并等待全部完成
来源：http://hz.hnqzz.top/gtitsmtxqc.html

Py:   asyncio.gather(*tasks)
来源：http://hz.nanxinkj.top/gtncxcikmf.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.meibo888.top/gtqgxmknam.html

JS:   await Promise.all(tasks)
来源：http://hz.sysykeji.top/gtrhxcftms.html

TS:   await Promise.all(tasks)
来源：http://hz.meibo888.top/gthwaagggl.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.kuanghao11.cn/gtkcugqozo.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.tanke756.top/gttfydqdor.html

Ruby: threads.map(&:join)
来源：http://hz.ywan-chungtsiang.top/gtcmgelpph.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.mhx1999.top/gtysmzsgyx.html

[O06] 使用进程池
来源：http://hz.xinyue.icu/gtwembpubu.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.zhongyouzk.top/gtuskftzzd.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.pycfn.com/gtcdutsbru.html

JS:   // child_process / cluster 模块
来源：http://hz.52xcode.cn/gtejxfujwo.html

TS:   // child_process / cluster 模块
来源：http://hz.gzhubu.top/gtxodobisz.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.yuanzhike.top/gtfczbcyak.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.meibo888.top/gtqbkbpxdx.html

Ruby: // fork 块
来源：http://hz.daria6918.cn/gtwkeqcsle.html

C#:   Parallel.For
来源：http://hz.sysykeji.top/gtvgoeuacc.html

================================================================================
来源：http://hz.hfpthk.cn/gtguwehnek.html

P. 常用工具函数
来源：http://hz.hnqzz.top/gtkbvvcyim.html

================================================================================
来源：http://hz.cheryme.top/gthrgneubm.html

[P01] 生成 UUID
来源：http://hz.dashuyun.cn/gtbqdmnxnd.html

Py:   str(uuid.uuid4())
来源：http://hz.vqdsnc.cn/gtgmhnqdig.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.cashguo.top/gtltweczlc.html

JS:   crypto.randomUUID()
来源：http://hz.cheryme.top/gtlkgzhwbh.html

TS:   crypto.randomUUID()
来源：http://hz.fzhhl.top/gtvfhtecdi.html

Java: UUID.randomUUID().toString()
来源：http://hz.gogol.net.cn/gtiqjegisp.html

Go:   // 用 github.com/google/uuid
来源：http://hz.vqdsnc.cn/gtggnfsfbr.html

Ruby: SecureRandom.uuid
来源：http://hz.redwolf501.top/gtydnrhpbe.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.shanyushiyangtech.top/gtmuhlkgvh.html

[P02] MD5 / SHA256 摘要
来源：http://hz.xziqi.cn/gtbjvzpqnn.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.quarkkingdee.top/gtutoeyspa.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.ehwqpu.com/gtjlzllcno.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.yj20258888.top/gtjgnwpvss.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.cucudq.cn/gtdbarmwuw.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.yj20258.top/gtmjolxtri.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.haohaochexian.top/gtosdhrgbh.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.aibaodan.cn/gtkqwseawj.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.cqqwz.cn/gtgnbqxnbk.html

[P03] 生成短随机字符串
来源：http://hz.nwbrower.top/gtgrldimdx.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.hnqzz.top/gtyhmknzap.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.chenlongwang.top/gttzrfltww.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.svipenyu.cn/gtndjzqyfi.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.xziqi.cn/gtjtxkopcd.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.zhoulong.xyz/gtmqqyguhx.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.dashuyun.cn/gteqpeqgpq.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.ppjwa.cn/gtqblghvmh.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.yuanzhike.top/gtyzrkondl.html

[P04] 求长度
来源：http://hz.dashuyun.cn/gtccqbfplb.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.yvedp.cn/gtubtgcgbz.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.zhixingplan.top/gtfgqjwbmm.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.jlsjyb.cn/gtdpzxmkgw.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.meibo888.top/gtcjqcvkox.html

Java: list.size();  map.size();  s.length()
来源：http://hz.hnxiangtu.top/gtgkfrnpiv.html

Go:   len(arr);  len(m)
来源：http://hz.smart0.xyz/gtdnjkykkg.html

Ruby: x.length;  x.size
来源：http://hz.zhixingplan.top/gtyljlluvz.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.tianlin.xyz/gtstxooqwz.html

[P05] 判断两个对象内容是否相等
来源：http://hz.meibo888.top/gtmmucrefc.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.guowangkeji.top/gtbwyeqbvw.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.ppjwa.cn/gtrlovnjqx.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.chenlongwang.top/gthkblodvp.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.zhijiandao.cn/gtytrbknhh.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.kuanghao11.cn/gtcjbnfapz.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.xuetiantiany.cn/gtnxfzrtft.html

Ruby: a == b
来源：http://hz.wangshuangyany.cn/gtuxrdyucu.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.svipenyu.cn/gtqqgebivl.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.yanxiufei.cn/gtfgyhetgl.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.mhx1999.top/gtyzdkxnlp.html

PHP:  if (empty($x)) {}
来源：http://hz.zycfv.cn/gtfcfpbepd.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.xylfe.cn/gtfvnlgzaw.html

TS:   if (x == null) {}
来源：http://hz.cqqwz.cn/gtinifazzi.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.daria6918.cn/gtcyjbphmx.html

Go:   if x == nil {}
来源：http://hz.yuanzhike.top/gtxxgmegnf.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.bjfxy.top/gtomsjlbhi.html

C#:   if (x is null) {}
来源：http://hz.ywan-chungtsiang.top/gtmfgnyjoa.html

[P07] 防抖与节流
来源：http://hz.ydzc1.top/gtdxrolrgo.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.xuetiantiany.cn/gtfrvoprxm.html

PHP:  // 手写时间戳比较
来源：http://hz.fengsongda.top/gtzzzizhud.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.cashguo.top/gtsryxtxwf.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.quarkkingdee.top/gtzhcillds.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.jqgufenzy.top/gtlzcljims.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.havefunace.top/gtrqhkfahd.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.shuidangran.top/gtwtpwkcpd.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.xingfuxueyuan.xyz/gtcdzhaizj.html

[P08] 处理浮点精度问题
来源：http://hz.nanxuanxn.top/gtufoecvvr.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.ehwqpu.com/gtwwqzbshj.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.hnxiangtu.top/gttyasswzp.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.gogol.net.cn/gtiunutfcu.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.shanyushiyangtech.top/gtynpabthk.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.sysykeji.top/gthbfhzhym.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.ivvv.top/gtkivfftgl.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.yanxiufei.cn/gthxaiablm.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.shzxlz.cn/gtjncwlzhz.html

================================================================================
来源：http://hz.daria6918.cn/gtphcsnjhs.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.hfpthk.cn/gtkvsyudgq.html

================================================================================
来源：http://hz.jinqigfzy.top/gtempcgfvj.html

[Q01] 创建表
来源：http://hz.quarkkingdee.top/gtnqfqjwjr.html

CREATE TABLE users (
来源：http://hz.kuanghao11.cn/gtxjedgcdc.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.tianlin.xyz/gteugxvtzm.html

name VARCHAR(50) NOT NULL,
来源：http://hz.zdqjudy.top/gtxtginxob.html

email VARCHAR(100) UNIQUE,
来源：http://hz.quarkkingdee.top/gtfnwsoiju.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.feifeiyinyue.top/gtrbgiwwax.html

);
来源：http://hz.zhoulong.xyz/gtjhhprehf.html

[Q02] 创建带外键的表
来源：http://hz.aibaodan.cn/gtbyereclj.html

CREATE TABLE orders (
来源：http://hz.zycfv.cn/gtagaxphqp.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.zhixingplan.top/gtrsundsga.html

user_id INT NOT NULL,
来源：http://hz.xingfuxueyuan.xyz/gtttoduruc.html

amount DECIMAL(10, 2),
来源：http://hz.jinghuilouyu.cn/gtfhmbhuze.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.xinyue.icu/gtdkqwsxgn.html

);
来源：http://hz.svipenyu.cn/gteircqfnd.html

[Q03] 增加列
来源：http://hz.jlsjyb.cn/gtrbaobrui.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.smart0.xyz/gtcbryfmnm.html

[Q04] 修改列类型
来源：http://hz.yj20258888.top/gtihdxfdng.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.0kj1m.cn/gtdcxbauoa.html

[Q05] 重命名列
来源：http://hz.ydjk.org.cn/gtjurlewbc.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.daria6918.cn/gtucgdjzld.html

[Q06] 删除列
来源：http://hz.9152youxi.cn/gtsjyvkfpl.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.yangfankeji.com/gtfluswrvt.html

[Q07] 删除表
来源：http://hz.yongpay.top/gtfvwzvtll.html

DROP TABLE IF EXISTS orders;
来源：http://hz.sysykeji.top/gtdavzwhsm.html

[Q08] 创建普通索引
来源：http://hz.quarkkingdee.top/gtntytzqvs.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.pengpengdd.cyou/gttbrnjwmj.html

[Q09] 创建唯一索引
来源：http://hz.shuidangran.top/gtolhylkxv.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.yuxming.cn/gtefopitgj.html

[Q10] 插入单行
来源：http://hz.sxryk.cn/gtglbtgtyq.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.guowangkeji.top/gtyjbqkqrc.html

[Q11] 一次插入多行
来源：http://hz.cashguo.top/gthrvtwgcu.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.shangyingyoupin.top/gtfiyntrjj.html

[Q12] 插入后取自增 ID
来源：http://hz.cucudq.cn/gteepcaghf.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.xziqi.cn/gtnvjppbdp.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.mhx1999.top/gtrgeerrey.html

[Q13] 忽略重复插入
来源：http://hz.haohaochexian.top/gtuvhosilm.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.hnxiangtu.top/gtdvtyutcd.html

[Q14] 存在则更新（upsert）
来源：http://hz.zhijiandao.cn/gtyfrrqbvm.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.bjfxy.top/gtgudcraek.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.hfpthk.cn/gtxrrheckf.html

[Q15] 查询全部
来源：http://hz.shangyingyoupin.top/gteowyeovg.html

SELECT * FROM users;
来源：http://hz.jinghuilouyu.cn/gtjnqhhlji.html

[Q16] 查询指定列
来源：http://hz.pengpengdd.cyou/gtmsekdxhn.html

SELECT id, name FROM users;
来源：http://hz.jqgufenzy.top/gtxwoyplsk.html

[Q17] 条件查询
来源：http://hz.fengsongda.top/gtzdvxqizt.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.cqqwz.cn/gtwinqysci.html

[Q18] 模糊匹配
来源：http://hz.chenjidiqi.icu/gthuvmuwvr.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.hfpthk.cn/gtadiyshxr.html

[Q19] 范围查询
来源：http://hz.yangfankeji.com/gtyauqqkbx.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.tian-w.cn/gtqgtupkwt.html

[Q20] IN 列表
来源：http://hz.zycfv.cn/gtsrwmqrnh.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.cheryme.top/gttszxngxy.html

[Q21] 空值判断
来源：http://hz.andypj.xyz/gtogfvnqlq.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.bjfxy.top/gtymtemwad.html

[Q22] 排序
来源：http://hz.chenzaomai.com/gtvrpxmwcf.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.guowangkeji.top/gtxjgzudwc.html

[Q23] 分页
来源：http://hz.jinyuanbaomall.cn/gtulbjvfxh.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.ybcxt.top/gtppmuuogv.html

[Q24] 去重
来源：http://hz.daxiang520.top/gtykccbrvo.html

SELECT DISTINCT city FROM users;
来源：http://hz.sysykeji.top/gteqeqspds.html

[Q25] 只取前 N 条
来源：http://hz.havefunace.top/gttyinyqzn.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.mhx1999.top/gtyztbnlod.html

[Q26] 计数
来源：http://hz.birdmap.top/gtsbghjpmv.html

SELECT COUNT(*) FROM users;
来源：http://hz.xuetiantiany.cn/gtcxpvwhut.html

[Q27] 条件计数
来源：http://hz.ybcxt.top/gtohyclkxr.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.yongpay.top/gtrbsiuqfu.html

[Q28] 求和与平均
来源：http://hz.hywenlv.cn/gtspgivuqp.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.yonumen.top/gtsryxheiz.html

[Q29] 最大最小值
来源：http://hz.dianchejie.cn/gtoxyvszsa.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.snrcjt.cn/gtirmzyxyt.html

[Q30] 分组统计
来源：http://hz.chenjidiqi.icu/gtkdgajmrx.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.wangshuangyany.cn/gtlgabdpzy.html

[Q31] 分组后过滤
来源：http://hz.jinyuanbaomall.cn/gtmnqptall.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.gaohongyu789.top/gtmqnqjxey.html

[Q32] 分组拼接字符串
来源：http://hz.zhijiandao.cn/gtovhgchyv.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.cashguo.top/gtplmlbcrx.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.pengpengdd.cyou/gtwtefoxgv.html

[Q33] 多列分组
来源：http://hz.yanxiufei.cn/gtxttkrext.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.xingfuxueyuan.xyz/gtoszxlgxa.html

[Q34] 每组取第一条
来源：http://hz.jinghuilouyu.cn/gttqjuptnd.html

SELECT * FROM (
来源：http://hz.xylfe.cn/gtaqmpydgs.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.jqgufenzy.top/gtgozbgxfb.html

) t WHERE rn = 1;
来源：http://hz.jiagoushi.top/gtosbkgwce.html

[Q35] 内连接
来源：http://hz.guannengcc.top/gtcgagulbp.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.xylfe.cn/gtsgbpvclv.html

[Q36] 左连接
来源：http://hz.zhoulong.xyz/gtaklpadam.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.tianlin.xyz/gtkhypczol.html

[Q37] 右连接
来源：http://hz.pengpengdd.cyou/gttubpwmhl.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.cheryme.top/gtkwwhxcvn.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.sweek.top/gtmgmniily.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.quarkkingdee.top/gtqpwigjqg.html

[Q39] 自连接（查上下级）
来源：http://hz.zdqjudy.top/gtyjsgmacv.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.0kj1m.cn/gtgzuklpuc.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.yongpay.top/gtehevllvo.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.shangyingyoupin.top/gtzydvkcnm.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.jinyuanbaomall.cn/gtrlvxhhnw.html

[Q41] 多表连接
来源：http://hz.guannengcc.top/gtslyxohnf.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.cdnleiting.top/gtzespiihe.html

JOIN users u ON u.id = o.user_id
来源：http://hz.jlsjyb.cn/gtqesfggnj.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.svipenyu.cn/gtfadjnlsa.html

[Q42] 连接条件附加过滤
来源：http://hz.xuanzx.com/gtybvjuwbx.html

SELECT u.name, o.amount FROM users u
来源：http://hz.iojbl.cn/gtofsaoyim.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.yueranfly.top/gtvyutsyhq.html

[Q43] 标量子查询
来源：http://hz.yangfankeji.com/gtsstgpdhw.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.snrcjt.cn/gtcctwrjhp.html

[Q44] IN 子查询
来源：http://hz.wangdashe.top/gtyjiuyagx.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.snrcjt.cn/gtmkkdwtrs.html

[Q45] EXISTS 判断存在
来源：http://hz.shzxlz.cn/gtkwznrfsc.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.zhixingplan.top/gtshyikkqs.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.c1oappe.top/gtsltsnzfs.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.dianchejie.cn/gtdctpphjy.html

[Q47] 与平均值比较
来源：http://hz.sxryk.cn/gtyxmgdtmu.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.kuanghao11.cn/gthdursajj.html

[Q48] CTE 公用表表达式
来源：http://hz.sweek.top/gtohikswce.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.haohaochexian.top/gtsjnmvrsg.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.cucudq.cn/gtikrcgflr.html

[Q49] 更新单行
来源：http://hz.gaohongyu789.top/gtiqagukjv.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.aizwys.cn/gtudljprei.html

[Q50] 批量更新
来源：http://hz.ydzc1.top/gtwxkkvecy.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.sxryk.cn/gtbqxputlc.html

[Q51] 用子查询更新
来源：http://hz.xingfuxueyuan.xyz/gtvjbgwinl.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.xingfuxueyuan.xyz/gtueexandg.html

[Q52] 删除指定行
来源：http://hz.svipenyu.cn/gtbfbipbio.html

DELETE FROM users WHERE id = 10;
来源：http://hz.cheryme.top/gtchmfiyqi.html

[Q53] 按条件删除
来源：http://hz.zhengqikj.top/gtzpvojoyb.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.quarkkingdee.top/gtxegqaxfl.html

[Q54] 清空表
来源：http://hz.nanxuanxn.top/gtqyggudtl.html

TRUNCATE TABLE logs;
来源：http://hz.zhaomingkeji.xyz/gtzxlnmibm.html

[Q55] 排名（并列占位）
来源：http://hz.xinyue.icu/gtpqsbhais.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.yj20258.top/gtuswsrpsp.html

[Q56] 密集排名（并列不占位）
来源：http://hz.wangdashe.top/gthivvpoem.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.hywenlv.cn/gtfemjeyfl.html

[Q57] 行号
来源：http://hz.jinghuilouyu.cn/gtnolhjfie.html


<!-- 参考信息 -->