代发 wailian999

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.daxiang520.top/gtqurtvjlb.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.pycfn.com/gtdmbpkjvh.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.tian-w.cn/gtfgluxnqh.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.havefunace.top/gthudhjweo.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.9152youxi.cn/gtzgeguufv.html

[N10] 链表节点定义
来源：http://hz.xziqi.cn/gtqbronnex.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.jinyuanbaomall.cn/gtmscsthse.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.hywenlv.cn/gtqbnjouvh.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.fengsongda.top/gtflmmjuzu.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.sxryk.cn/gtuwefviox.html

Java: class Node { int v; Node next; }
来源：http://hz.xingfuxueyuan.xyz/gtlbajqamh.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.sweek.top/gtoxbozjvx.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.52xcode.cn/gtaijpufbs.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.yueranfly.top/gtpjlkukrc.html

[N11] 二叉树中序遍历
来源：http://hz.tianlin.xyz/gtggkigacj.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.zhoulong.xyz/gtpsjyecmu.html

PHP:  // 手写递归函数
来源：http://hz.xylfe.cn/gtdzcztvwj.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.pengpengdd.cyou/gtrgxujfhf.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.fzhhl.top/gtwnvatfva.html

Java: // 手写递归
来源：http://hz.sysykeji.top/gtfvcvfwib.html

Go:   // 手写递归
来源：http://hz.shangyingyoupin.top/gtrjridxyi.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.birdmap.top/gtdruyolmy.html

C#:   // 手写递归
来源：http://hz.yongpay.top/gtlolksphs.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.tian-w.cn/gthgwesryd.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.dashuyun.cn/gttqpccttq.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.ivvv.top/gtobktdosv.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.sufxvd.cn/gtkxuysjhk.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.ywan-chungtsiang.top/gtqtsekgah.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.shzxlz.cn/gthcsbauzc.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.pycfn.com/gtwjxemuwi.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.zhoulong.xyz/gtxwbstjjh.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.jqgfzy.top/gtysrknyxk.html

================================================================================
来源：http://hz.jyoumei.cn/gtqyctwokh.html

O. 并发与异步
来源：http://hz.jianghu66.top/gtmoeoairu.html

================================================================================
来源：http://hz.xuetiantiany.cn/gtcrguljte.html

[O01] 启动一个线程
来源：http://hz.xuetiantiany.cn/gtjfcwusna.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.vqdsnc.cn/gtdajjgbqq.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.cheryme.top/gtksqwdhhw.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.wangdashe.top/gtdqaktrak.html

TS:   // 同 JS
来源：http://hz.jianghu66.top/gtmcuaoaof.html

Java: new Thread(() -> f()).start()
来源：http://hz.snrcjt.cn/gtmzmlivlc.html

Go:   go f()
来源：http://hz.xingfuxueyuan.xyz/gtnytllcnn.html

Ruby: Thread.new { f }
来源：http://hz.ppjwa.cn/gtespvsxlk.html

C#:   Task.Run(() => F());
来源：http://hz.9152youxi.cn/gtwtetieup.html

[O02] 使用线程池
来源：http://hz.jinyuanbaomall.cn/gtkwtyhfkd.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.zhengqikj.top/gtnmmkdokr.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.9152youxi.cn/gtktdtgqke.html

JS:   // worker_threads 线程池
来源：http://hz.gzhubu.top/gthhhwkbgh.html

TS:   // worker_threads 线程池
来源：http://hz.9152youxi.cn/gthusncocc.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.xylfe.cn/gtesxumipt.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.sysykeji.top/gtqujltydu.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.yongpay.top/gtlejezwip.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.hnxiangtu.top/gtehbodzwq.html

[O03] 加锁保护共享数据
来源：http://hz.nwbrower.top/gtwalxtuhn.html

Py:   with lock: shared += 1
来源：http://hz.hnqzz.top/gthuadcycf.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.ydzc1.top/gtbaeyfciw.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.guowangkeji.top/gthztatabg.html

TS:   // 同 JS
来源：http://hz.gotoacloud.top/gtcssoivok.html

Java: synchronized (this) { shared++; }
来源：http://hz.yanxiufei.cn/gtuyvtjzeb.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.dianchejie.cn/gtzmholysq.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.cashguo.top/gtfpgdhbln.html

C#:   lock (gate) { shared++; }
来源：http://hz.sxryk.cn/gtcwwwtkmj.html

[O04] 定义异步函数并等待
来源：http://hz.haohaochexian.top/gtazoxvilu.html

Py:   async def f():⏎    await g()
来源：http://hz.zhongyouzk.top/gtwjuyqsmn.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.jinghuilouyu.cn/gtsatigoqk.html

JS:   async function f() { await g(); }
来源：http://hz.tianlin.xyz/gtcipepwic.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.mhx1999.top/gtejxreyjt.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.feifeiyinyue.top/gterzxiyex.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.zycfv.cn/gtsqbuddzq.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.zhiwuduotai.top/gtvqyzqtql.html

C#:   async Task F() { await G(); }
来源：http://hz.tanke756.top/gtppnbpbuk.html

[O05] 并发执行并等待全部完成
来源：http://hz.jlsjyb.cn/gtitoocfya.html

Py:   asyncio.gather(*tasks)
来源：http://hz.andypj.xyz/gtioddnooy.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.wangshuangyany.cn/gtfmdvzfbt.html

JS:   await Promise.all(tasks)
来源：http://hz.pengpengdd.cyou/gtldfvoiuj.html

TS:   await Promise.all(tasks)
来源：http://hz.daxiang520.top/gtubveetsj.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.nwbrower.top/gtzomaouys.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.yuxming.cn/gtcgetckzf.html

Ruby: threads.map(&:join)
来源：http://hz.chenzaomai.com/gtxyyfrtgd.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.xylfe.cn/gtoncaqffd.html

[O06] 使用进程池
来源：http://hz.yuxming.cn/gtollikfwl.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.jinyuanbaomall.cn/gtibkmfoip.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.smart0.xyz/gtndszzgmb.html

JS:   // child_process / cluster 模块
来源：http://hz.sweek.top/gtfnupovco.html

TS:   // child_process / cluster 模块
来源：http://hz.pengpengdd.cyou/gtspsfksly.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.zhengqikj.top/gtyydghvix.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.meibo888.top/gtyqesgfun.html

Ruby: // fork 块
来源：http://hz.snrcjt.cn/gtllzaulew.html

C#:   Parallel.For
来源：http://hz.dianchejie.cn/gtyksuoqvr.html

================================================================================
来源：http://hz.hnqzz.top/gtkkgsqsza.html

P. 常用工具函数
来源：http://hz.zhixingplan.top/gtdlawekhy.html

================================================================================
来源：http://hz.daria6918.cn/gtgjfrfcyr.html

[P01] 生成 UUID
来源：http://hz.smart0.xyz/gtyfaduyud.html

Py:   str(uuid.uuid4())
来源：http://hz.jiagoushi.top/gtgqutiwfj.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.jianghu66.top/gtobtjtahl.html

JS:   crypto.randomUUID()
来源：http://hz.cheryme.top/gtutrlcxoa.html

TS:   crypto.randomUUID()
来源：http://hz.fzhhl.top/gtuhyjkrgn.html

Java: UUID.randomUUID().toString()
来源：http://hz.wangdashe.top/gtajkfrsig.html

Go:   // 用 github.com/google/uuid
来源：http://hz.xinyue.icu/gtqhxrvrie.html

Ruby: SecureRandom.uuid
来源：http://hz.jinqigfzy.top/gtmfmbqfkq.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.zycfv.cn/gthmswggsn.html

[P02] MD5 / SHA256 摘要
来源：http://hz.xinyue.icu/gtntxiilrp.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.xingfuxueyuan.xyz/gtekmrwjiq.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.yvedp.cn/gtqsgyylwh.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.nanxinkj.top/gtrlnvqpdl.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.gogol.net.cn/gtghpkskdq.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.ybcxt.top/gtnlswuhww.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.gotoacloud.top/gtorvgdbxw.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.dashuyun.cn/gtgakmejke.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.ppjwa.cn/gtrqxptmnk.html

[P03] 生成短随机字符串
来源：http://hz.yj202588.top/gtagekdbpo.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.jinyuanbaomall.cn/gtfhjblzoe.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.wangdashe.top/gtyxvlnoxv.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.yj202588.top/gtnmkfofti.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.jyoumei.cn/gtkrehlyza.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.hnxiangtu.top/gtjnjjryok.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.sxryk.cn/gtwobjnbjp.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.chenzaomai.com/gtdfyhzzoi.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.mhx1999.top/gtegzvygrz.html

[P04] 求长度
来源：http://hz.vqdsnc.cn/gtfciwdeoe.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.pycfn.com/gtspixixrm.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.yuanzhike.top/gtaolzawbj.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.c1oappe.top/gtjzqkkzee.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.zhongyouzk.top/gtuwpqqyva.html

Java: list.size();  map.size();  s.length()
来源：http://hz.cqqwz.cn/gtvxrwssyg.html

Go:   len(arr);  len(m)
来源：http://hz.ehwqpu.com/gtlmuyajdg.html

Ruby: x.length;  x.size
来源：http://hz.nanxuanxn.top/gtjcgmxqbk.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.yj20258888.top/gtwntsdvmq.html

[P05] 判断两个对象内容是否相等
来源：http://hz.havefunace.top/gthlmmqnqf.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.yonumen.top/gtddbejwsk.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.yuanzhike.top/gtimtrzrrc.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.hnxiangtu.top/gtobplydvo.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.ywan-chungtsiang.top/gttxxmrvyk.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.guowangkeji.top/gtbmjqgohu.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.jiagoushi.top/gtnudlyztl.html

Ruby: a == b
来源：http://hz.hfpthk.cn/gtsfzyccbo.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.cucudq.cn/gtrexnzzyv.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.zhongyouzk.top/gtlwkgdiqg.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.pengpengdd.cyou/gtfcufoepg.html

PHP:  if (empty($x)) {}
来源：http://hz.chenjidiqi.icu/gtqlgvmiqb.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.wangdashe.top/gtfmgpqxmh.html

TS:   if (x == null) {}
来源：http://hz.haohaochexian.top/gtvschnoah.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.wangshuangyany.cn/gtapamtiuc.html

Go:   if x == nil {}
来源：http://hz.cdnleiting.top/gthawrtgjo.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.daxiang520.top/gtpgrlwocs.html

C#:   if (x is null) {}
来源：http://hz.redwolf501.top/gtvqjwturz.html

[P07] 防抖与节流
来源：http://hz.zhaomingkeji.xyz/gtwrdwwjtx.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.svipenyu.cn/gtnilsrync.html

PHP:  // 手写时间戳比较
来源：http://hz.xuanzx.com/gtyzykpzco.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.yongpay.top/gtybstrugf.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.meibo888.top/gticdcwdxr.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.zdqjudy.top/gtuvyjqjzn.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.nwbrower.top/gtiplrtsxy.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.cqqwz.cn/gtfnppfrag.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.ehwqpu.com/gtamatyomi.html

[P08] 处理浮点精度问题
来源：http://hz.cheryme.top/gtcfuznkzx.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.xuanzx.com/gttulpgjjl.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.vqdsnc.cn/gtcikbiyut.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.cqqwz.cn/gtgnujhnwi.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.cdnleiting.top/gtyopoctix.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.nwbrower.top/gtiqrnoyed.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.pengpengdd.cyou/gtyjvkoyao.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.guowangkeji.top/gtccvfjcmt.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.jyoumei.cn/gtclywgqnk.html

================================================================================
来源：http://hz.dashuyun.cn/gtrmepxpqp.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.jinqigfzy.top/gtrkrikrgs.html

================================================================================
来源：http://hz.haohaochexian.top/gtfkcsuhuo.html

[Q01] 创建表
来源：http://hz.yuanzhike.top/gtszuigycs.html

CREATE TABLE users (
来源：http://hz.pengpengdd.cyou/gtjwypzoco.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.meibo888.top/gtabqvxzxs.html

name VARCHAR(50) NOT NULL,
来源：http://hz.ywan-chungtsiang.top/gtjkagmfxu.html

email VARCHAR(100) UNIQUE,
来源：http://hz.quarkkingdee.top/gtqkzxsxdc.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.zhongyouzk.top/gtjpdqylhy.html

);
来源：http://hz.feifeiyinyue.top/gtavcugaek.html

[Q02] 创建带外键的表
来源：http://hz.sufxvd.cn/gtdkfpcwrb.html

CREATE TABLE orders (
来源：http://hz.jinqigufen.top/gtvvuvebuv.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.haohaochexian.top/gtwvuhqlpk.html

user_id INT NOT NULL,
来源：http://hz.zycfv.cn/gtngkubvhq.html

amount DECIMAL(10, 2),
来源：http://hz.9152youxi.cn/gtngsbomwj.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.gzhubu.top/gttwukwmrp.html

);
来源：http://hz.sxryk.cn/gtmgerigol.html

[Q03] 增加列
来源：http://hz.shanyushiyangtech.top/gthpjnkkdw.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.hysaishi.cn/gtngnkwrwg.html

[Q04] 修改列类型
来源：http://hz.hfpthk.cn/gtzozhyhiz.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.xylfe.cn/gtgoymanvm.html

[Q05] 重命名列
来源：http://hz.0kj1m.cn/gtxiiewdeq.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.xuetiantiany.cn/gtqubbyrax.html

[Q06] 删除列
来源：http://hz.c1oappe.top/gtykygzfus.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.gzhubu.top/gtevuwjban.html

[Q07] 删除表
来源：http://hz.cheryme.top/gtdltdabde.html

DROP TABLE IF EXISTS orders;
来源：http://hz.nwbrower.top/gtnzxgydym.html

[Q08] 创建普通索引
来源：http://hz.birdmap.top/gtlypdexfj.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.zhiwuduotai.top/gtosuyffmy.html

[Q09] 创建唯一索引
来源：http://hz.yongpay.top/gtkdlmlnlo.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.hammf.cn/gtcowjddhf.html

[Q10] 插入单行
来源：http://hz.shuidangran.top/gtzyglkeum.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.yvedp.cn/gtwzbrvyuy.html

[Q11] 一次插入多行
来源：http://hz.fengsongda.top/gtlnuppnse.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.pycfn.com/gtvgojcpfx.html

[Q12] 插入后取自增 ID
来源：http://hz.chenzaomai.com/gtbjrpgojc.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.shanyushiyangkeji.top/gtasvwvivy.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.jinghuilouyu.cn/gtgrygodct.html

[Q13] 忽略重复插入
来源：http://hz.xinyue.icu/gtxpzchhlu.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.bjfxy.top/gthgdtytob.html

[Q14] 存在则更新（upsert）
来源：http://hz.jinqigufen.top/gtoysbbrik.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.daria6918.cn/gtutghoula.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.gzhubu.top/gtqissfwtf.html

[Q15] 查询全部
来源：http://hz.cqqwz.cn/gtpgjidcta.html

SELECT * FROM users;
来源：http://hz.hnxiangtu.top/gtmfwxtzoy.html

[Q16] 查询指定列
来源：http://hz.sweek.top/gtavdrunpt.html

SELECT id, name FROM users;
来源：http://hz.yanxiufei.cn/gtgligpsdk.html

[Q17] 条件查询
来源：http://hz.nwbrower.top/gtunzmdvbi.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.yuxming.cn/gtyqlcmbak.html

[Q18] 模糊匹配
来源：http://hz.aibaodan.cn/gtgdkvtyjd.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.hywenlv.cn/gtculwueir.html

[Q19] 范围查询
来源：http://hz.0kj1m.cn/gtsskkrovd.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.hysaishi.cn/gtaqbkaqpw.html

[Q20] IN 列表
来源：http://hz.jianghu66.top/gtnwkgchka.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.shangyingyoupin.top/gtbnlfvhwj.html

[Q21] 空值判断
来源：http://hz.daxiang520.top/gtoipbhhvc.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.aibaodan.cn/gtazogomxk.html

[Q22] 排序
来源：http://hz.sxryk.cn/gtqkdgrein.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.52xcode.cn/gtchtvvdzo.html

[Q23] 分页
来源：http://hz.hongshengwenyu.top/gtswdivwhc.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.shanyushiyangkeji.top/gtgpsntnms.html

[Q24] 去重
来源：http://hz.shanyushiyangkeji.top/gtwuhqoxmk.html

SELECT DISTINCT city FROM users;
来源：http://hz.yj202588.top/gtwjsexeli.html

[Q25] 只取前 N 条
来源：http://hz.yvedp.cn/gtrutvnhzy.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.daxiang520.top/gtebxldkoo.html

[Q26] 计数
来源：http://hz.cucudq.cn/gtqxexluux.html

SELECT COUNT(*) FROM users;
来源：http://hz.pycfn.com/gtawpvhvjy.html

[Q27] 条件计数
来源：http://hz.nwbrower.top/gtrwnhuetw.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.shuidangran.top/gtdmyxlfmk.html

[Q28] 求和与平均
来源：http://hz.ybcxt.top/gtoeddhuhl.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.pengpengdd.cyou/gtodkcglut.html

[Q29] 最大最小值
来源：http://hz.haohaochexian.top/gtororheud.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.nanxinkj.top/gtgtnsxjqf.html

[Q30] 分组统计
来源：http://hz.meibo888.top/gtgqwawhxu.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.hfpthk.cn/gtrplllbzc.html

[Q31] 分组后过滤
来源：http://hz.xylfe.cn/gttvchwerc.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.xziqi.cn/gtdsbagjws.html

[Q32] 分组拼接字符串
来源：http://hz.jlsjyb.cn/gtyhjlycpi.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.ppjwa.cn/gtlcihmuib.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.cdnleiting.top/gtrqysxzzt.html

[Q33] 多列分组
来源：http://hz.ehwqpu.com/gtfqmcswpx.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.sweek.top/gtjveclmkt.html

[Q34] 每组取第一条
来源：http://hz.gaohongyu789.top/gtwybrxrrm.html

SELECT * FROM (
来源：http://hz.chenjidiqi.icu/gtbmdwbjzu.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.guannengcc.top/gtlgutriqr.html

) t WHERE rn = 1;
来源：http://hz.hnxiangtu.top/gtfxqdrdyc.html

[Q35] 内连接
来源：http://hz.cqqwz.cn/gtiakcnktt.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.daxiang520.top/gtcydxwbsd.html

[Q36] 左连接
来源：http://hz.snrcjt.cn/gticdstfgu.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.9152youxi.cn/gtrbxppwte.html

[Q37] 右连接
来源：http://hz.cheryme.top/gtfzujiifg.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.chenlongwang.top/gtavxleleb.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.aizwys.cn/gtczibbksw.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.shangyingyoupin.top/gtfmursirb.html

[Q39] 自连接（查上下级）
来源：http://hz.quarkkingdee.top/gteuczpbyl.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.ppjwa.cn/gtthjwycdd.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.xuetiantiany.cn/gtdyxhwqoc.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.dashuyun.cn/gtkqfwrkhg.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.yonumen.top/gtnyxglrkl.html

[Q41] 多表连接
来源：http://hz.sufxvd.cn/gtcpqkwdwd.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.shzxlz.cn/gttuzilzei.html

JOIN users u ON u.id = o.user_id
来源：http://hz.sxryk.cn/gtafswmpkk.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.havefunace.top/gtgemdtpks.html

[Q42] 连接条件附加过滤
来源：http://hz.xylfe.cn/gtfsaasjya.html

SELECT u.name, o.amount FROM users u
来源：http://hz.feifeiyinyue.top/gtjomhygsf.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.yonumen.top/gttolxgmpm.html

[Q43] 标量子查询
来源：http://hz.vqdsnc.cn/gtsklqxnun.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.hammf.cn/gtdeylhmaj.html

[Q44] IN 子查询
来源：http://hz.guowangkeji.top/gtxqwpsixv.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.feifeiyinyue.top/gtabcaihlh.html

[Q45] EXISTS 判断存在
来源：http://hz.hywenlv.cn/gthtdxvvsn.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.andypj.xyz/gtkpqhmvxz.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.gogol.net.cn/gtnzyljhrm.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.shuidangran.top/gtyjvfrlbc.html

[Q47] 与平均值比较
来源：http://hz.wangdashe.top/gtkdqzhqwl.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.0kj1m.cn/gtjdmjfvtk.html

[Q48] CTE 公用表表达式
来源：http://hz.yuxming.cn/gtnlemzsdq.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.nanxuanxn.top/gtnvpfbbzw.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.jlsjyb.cn/gtewtwxape.html

[Q49] 更新单行
来源：http://hz.ydzc1.top/gtibyadrei.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.guowangkeji.top/gtxapjhkcf.html

[Q50] 批量更新
来源：http://hz.xylfe.cn/gtxstkyttx.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.sysykeji.top/gtzgptvjdj.html

[Q51] 用子查询更新
来源：http://hz.zhengqikj.top/gthvgzhhjb.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.hfpthk.cn/gtiwmmmocw.html

[Q52] 删除指定行
来源：http://hz.hongshengwenyu.top/gteceuqzau.html

DELETE FROM users WHERE id = 10;
来源：http://hz.hnxiangtu.top/gtroghcfrq.html

[Q53] 按条件删除
来源：http://hz.zhoulong.xyz/gtnbknwemw.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.yj202588.top/gtuaqdwvow.html

[Q54] 清空表
来源：http://hz.chenzaomai.com/gtoqcokner.html

TRUNCATE TABLE logs;
来源：http://hz.tian-w.cn/gtjbynbcis.html

[Q55] 排名（并列占位）
来源：http://hz.xingfuxueyuan.xyz/gtgxapqwuf.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.vqdsnc.cn/gtlfwobqcg.html

[Q56] 密集排名（并列不占位）
来源：http://hz.andypj.xyz/gtabceeqlu.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.yueranfly.top/gtpnrtwdes.html

[Q57] 行号
来源：http://hz.yangfankeji.com/gtxxdkasca.html


<!-- 参考信息 -->