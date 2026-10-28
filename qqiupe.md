代发 wailian999

Py:   itertools.permutations(arr)
来源：http://hz.cqqwz.cn/gtauyivlry.html

PHP:  // 手写递归交换
来源：http://hz.xylfe.cn/gteswbggzs.html

JS:   // 手写回溯递归
来源：http://hz.zhaomingkeji.xyz/gtgfweevzu.html

TS:   // 手写回溯递归
来源：http://hz.jyoumei.cn/gtazdilcff.html

Java: // 手写回溯递归
来源：http://hz.tianlin.xyz/gtjjembmac.html

Go:   // 手写回溯递归
来源：http://hz.quarkkingdee.top/gtgoprznay.html

Ruby: arr.permutation.to_a
来源：http://hz.shanyushiyangtech.top/gthrstmilw.html

C#:   // 手写回溯递归
来源：http://hz.hnxiangtu.top/gttgypyvkm.html

[N09] 栈与队列
来源：http://hz.sxryk.cn/gthaofwwgb.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.haohaochexian.top/gtexrvkffz.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.cdnleiting.top/gtnlsgfoyf.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.sweek.top/gtfibnlein.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.c1oappe.top/gtfgahzreg.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.gotoacloud.top/gttbxeifbk.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.meibo888.top/gtrknpvuom.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.jinqigufen.top/gtlbkgagey.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.birdmap.top/gtjfqvozfq.html

[N10] 链表节点定义
来源：http://hz.dashuyun.cn/gthjsrcudv.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.yongpay.top/gtcbkapipa.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.316326.xyz/gtfnqkadul.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.meibo888.top/gtpredkbdu.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.zdqjudy.top/gtqonauxlt.html

Java: class Node { int v; Node next; }
来源：http://hz.hongshengwenyu.top/gtcrpgqwva.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.hnqzz.top/gtyabliwvq.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.0kj1m.cn/gtxyxzttjd.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.chenjidiqi.icu/gtehxzozla.html

[N11] 二叉树中序遍历
来源：http://hz.jyoumei.cn/gtdnzonqlx.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.haohaochexian.top/gtjfeiuuxf.html

PHP:  // 手写递归函数
来源：http://hz.9152youxi.cn/gtsttxfhqa.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.nanxuanxn.top/gtodribkii.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.gzhubu.top/gtpcuptkww.html

Java: // 手写递归
来源：http://hz.yvedp.cn/gtcngbhfkx.html

Go:   // 手写递归
来源：http://hz.gzhubu.top/gtapbjncfo.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.kuanghao11.cn/gtmhwovdas.html

C#:   // 手写递归
来源：http://hz.jianghu66.top/gttpgvjwxr.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.zdqjudy.top/gtgproaque.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.0kj1m.cn/gtkhfuzrya.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.jinqigfzy.top/gtcojtyuad.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.shzxlz.cn/gtcragvthl.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.yangfankeji.com/gthdslpauk.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.tian-w.cn/gtlxfbzlvz.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.ybcxt.top/gtpkkauren.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.yvedp.cn/gtwrzhaphm.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.fengsongda.top/gtcyewtmhp.html

================================================================================
来源：http://hz.yj202588.top/gtldakjtfs.html

O. 并发与异步
来源：http://hz.hongshengwenyu.top/gtsemagfhi.html

================================================================================
来源：http://hz.daxiang520.top/gtaoucolqa.html

[O01] 启动一个线程
来源：http://hz.xingfuxueyuan.xyz/gtnleddyga.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.hysaishi.cn/gtkdujalbc.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.wangshuangyany.cn/gthnmjrwft.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.shangyingyoupin.top/gtnkhsrkjp.html

TS:   // 同 JS
来源：http://hz.yj20258888.top/gtcechiwpl.html

Java: new Thread(() -> f()).start()
来源：http://hz.zhaomingkeji.xyz/gtoreqnzql.html

Go:   go f()
来源：http://hz.sxryk.cn/gtrcagdbpi.html

Ruby: Thread.new { f }
来源：http://hz.ehwqpu.com/gtrtfxklpa.html

C#:   Task.Run(() => F());
来源：http://hz.xylfe.cn/gtgractmku.html

[O02] 使用线程池
来源：http://hz.ybcxt.top/gtvxlueabl.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.jinqigufen.top/gtqflwlhiy.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.dashuyun.cn/gtmehrmkny.html

JS:   // worker_threads 线程池
来源：http://hz.yongpay.top/gtllgriean.html

TS:   // worker_threads 线程池
来源：http://hz.jinghuilouyu.cn/gtsvgnmque.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.ydjk.org.cn/gteqmrmcwz.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.redwolf501.top/gtcdursjbu.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.ppjwa.cn/gtsnluiilw.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.yj20258.top/gtqnfwjinf.html

[O03] 加锁保护共享数据
来源：http://hz.316326.xyz/gtqjbanzmi.html

Py:   with lock: shared += 1
来源：http://hz.chenlongwang.top/gtmpbcppwu.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.cucudq.cn/gtslhgvqml.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.fengsongda.top/gtxuanfoko.html

TS:   // 同 JS
来源：http://hz.tian-w.cn/gtuwauyifz.html

Java: synchronized (this) { shared++; }
来源：http://hz.pengpengdd.cyou/gtifsekhps.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.cheryme.top/gtlzjsgozd.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.nanxinkj.top/gtlcbcisls.html

C#:   lock (gate) { shared++; }
来源：http://hz.shanyushiyangkeji.top/gtzxcuoqwf.html

[O04] 定义异步函数并等待
来源：http://hz.zycfv.cn/gtbpejfgym.html

Py:   async def f():⏎    await g()
来源：http://hz.jinqigufen.top/gthqupjscd.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.smart0.xyz/gteixxbqla.html

JS:   async function f() { await g(); }
来源：http://hz.jinghuilouyu.cn/gtgmcuqwky.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.fengsongda.top/gthuoxsprl.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.ydjk.org.cn/gtepgsssic.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.havefunace.top/gtpfwrydrm.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.yuxming.cn/gtusumxnif.html

C#:   async Task F() { await G(); }
来源：http://hz.yueranfly.top/gtcchaxzwr.html

[O05] 并发执行并等待全部完成
来源：http://hz.daria6918.cn/gtbxueoujh.html

Py:   asyncio.gather(*tasks)
来源：http://hz.hfpthk.cn/gtflfctzbc.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.tanke756.top/gtvrnnfukg.html

JS:   await Promise.all(tasks)
来源：http://hz.dashuyun.cn/gtymkpzlmz.html

TS:   await Promise.all(tasks)
来源：http://hz.hysaishi.cn/gtfaoxgxkd.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.yuanzhike.top/gttxqcfdum.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.jinqigfzy.top/gtclkegbrm.html

Ruby: threads.map(&:join)
来源：http://hz.52xcode.cn/gtsmhxxjkq.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.yj20258888.top/gtfqvonsqa.html

[O06] 使用进程池
来源：http://hz.fzhhl.top/gtxgfzstdc.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.c1oappe.top/gtsfaoldpu.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.xziqi.cn/gtewvvxjon.html

JS:   // child_process / cluster 模块
来源：http://hz.daxiang520.top/gtybemcfkd.html

TS:   // child_process / cluster 模块
来源：http://hz.52xcode.cn/gtwcxzsbmi.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.yonumen.top/gtxyfylkth.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.hysaishi.cn/gtfrsooltu.html

Ruby: // fork 块
来源：http://hz.havefunace.top/gtnfjidjyx.html

C#:   Parallel.For
来源：http://hz.yongpay.top/gtmlxiqnxm.html

================================================================================
来源：http://hz.ehwqpu.com/gtsdryyppr.html

P. 常用工具函数
来源：http://hz.ybcxt.top/gtixvapilf.html

================================================================================
来源：http://hz.gzhubu.top/gtirogcahn.html

[P01] 生成 UUID
来源：http://hz.andypj.xyz/gtmdozmkft.html

Py:   str(uuid.uuid4())
来源：http://hz.zhaomingkeji.xyz/gtrnyfpwwi.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.sweek.top/gtrrknppdq.html

JS:   crypto.randomUUID()
来源：http://hz.svipenyu.cn/gtfhwtlqrv.html

TS:   crypto.randomUUID()
来源：http://hz.shuidangran.top/gtumbbjfgg.html

Java: UUID.randomUUID().toString()
来源：http://hz.birdmap.top/gtyfegyyjg.html

Go:   // 用 github.com/google/uuid
来源：http://hz.fengsongda.top/gtmatzjupg.html

Ruby: SecureRandom.uuid
来源：http://hz.dianchejie.cn/gtwvfeasad.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.cqqwz.cn/gtigyqnaet.html

[P02] MD5 / SHA256 摘要
来源：http://hz.gzhubu.top/gtfhhkwacp.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.52xcode.cn/gtivqhinqr.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.zhaomingkeji.xyz/gtpiowmstu.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.daria6918.cn/gtrzrlfrhi.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.guowangkeji.top/gtjbsfekxf.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.cheryme.top/gtlnbwmnle.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.ivvv.top/gtjxuwjrnt.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.hnqzz.top/gteapcpnmy.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.hnqzz.top/gtwzasjayz.html

[P03] 生成短随机字符串
来源：http://hz.bjfxy.top/gtxebmgfou.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.pycfn.com/gttfnegvvz.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.ydzc1.top/gtewlqlkho.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.sysykeji.top/gtwngyrzmv.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.yj20258.top/gtmmvxsmmr.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.guannengcc.top/gtlsvvcifn.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.kuanghao11.cn/gtsvqiexuh.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.haohaochexian.top/gtvgnlrezt.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.nwbrower.top/gtmhqwkulm.html

[P04] 求长度
来源：http://hz.jinghuilouyu.cn/gtxcicefbk.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.zhiwuduotai.top/gtbivcmhzn.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.yongpay.top/gtblbtdcmd.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.c1oappe.top/gtjsawsrfr.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.jyoumei.cn/gtrktkwhww.html

Java: list.size();  map.size();  s.length()
来源：http://hz.quarkkingdee.top/gtvdlboddw.html

Go:   len(arr);  len(m)
来源：http://hz.yongpay.top/gtrkilggpg.html

Ruby: x.length;  x.size
来源：http://hz.mhx1999.top/gtqfarwjgl.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.hfpthk.cn/gtpmzfnzxp.html

[P05] 判断两个对象内容是否相等
来源：http://hz.svipenyu.cn/gttagqtnfp.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.52xcode.cn/gtdnpynqfq.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.yangfankeji.com/gtfvoxhyhz.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.ywan-chungtsiang.top/gtosvuhvtq.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.snrcjt.cn/gtvwhhkxrb.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.ywan-chungtsiang.top/gtvcupximw.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.smart0.xyz/gtlkdalabl.html

Ruby: a == b
来源：http://hz.ivvv.top/gtlbinddob.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.sweek.top/gtswpgwwct.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.gogol.net.cn/gthfihghjq.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.xingfuxueyuan.xyz/gtgbzxyzpj.html

PHP:  if (empty($x)) {}
来源：http://hz.jinqigufen.top/gtsttbmhjn.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.zhoulong.xyz/gtsfbitapt.html

TS:   if (x == null) {}
来源：http://hz.aizwys.cn/gtwaarfvgg.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.dashuyun.cn/gtveexsbsv.html

Go:   if x == nil {}
来源：http://hz.ybcxt.top/gtmoaohqce.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.sysykeji.top/gtdjdykoxo.html

C#:   if (x is null) {}
来源：http://hz.9152youxi.cn/gtmiudfxpr.html

[P07] 防抖与节流
来源：http://hz.smart0.xyz/gtlcouovdw.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.cashguo.top/gtouonsbwp.html

PHP:  // 手写时间戳比较
来源：http://hz.xinyue.icu/gtksskjzkk.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.nwbrower.top/gtuuouxvzs.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.zhengqikj.top/gtetvmhouc.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.redwolf501.top/gtjsmmafjo.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.xylfe.cn/gtsvxvlknb.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.cucudq.cn/gttjstzlxc.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.shzxlz.cn/gtehhpavdb.html

[P08] 处理浮点精度问题
来源：http://hz.redwolf501.top/gtdwocnwri.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.gotoacloud.top/gttlvkachr.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.tanke756.top/gtckszozfu.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.daxiang520.top/gtoueffpqu.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.daxiang520.top/gtraqzvipc.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.meibo888.top/gtcuhlpmei.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.zhixingplan.top/gtrknwpyxf.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.haohaochexian.top/gtlpunqlri.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.sufxvd.cn/gtcgnjllcj.html

================================================================================
来源：http://hz.ybcxt.top/gtdaxgudam.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.feifeiyinyue.top/gtpwyqulmf.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gtgziwyips.html

[Q01] 创建表
来源：http://hz.hnqzz.top/gtohbjhwnz.html

CREATE TABLE users (
来源：http://hz.haohaochexian.top/gtivqzprvb.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.guannengcc.top/gtvbjoxaln.html

name VARCHAR(50) NOT NULL,
来源：http://hz.nwbrower.top/gtjrokqjnv.html

email VARCHAR(100) UNIQUE,
来源：http://hz.jianghu66.top/gtdjsupjjy.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.sweek.top/gtklxzgxuj.html

);
来源：http://hz.wangdashe.top/gtjgywvdnv.html

[Q02] 创建带外键的表
来源：http://hz.yangfankeji.com/gtdlvhaomk.html

CREATE TABLE orders (
来源：http://hz.wangdashe.top/gtxxmfhqaz.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.gzhubu.top/gtrubyobeh.html

user_id INT NOT NULL,
来源：http://hz.zhixingplan.top/gtdlbjqucp.html

amount DECIMAL(10, 2),
来源：http://hz.tian-w.cn/gtyqyzziif.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.dashuyun.cn/gtpftclvta.html

);
来源：http://hz.cashguo.top/gtlhuiepnu.html

[Q03] 增加列
来源：http://hz.0kj1m.cn/gtfmdsscdg.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.yueranfly.top/gtwsrwuowh.html

[Q04] 修改列类型
来源：http://hz.ppjwa.cn/gttaffxatu.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.gogol.net.cn/gtbdhclptb.html

[Q05] 重命名列
来源：http://hz.jinqigfzy.top/gtshehvowe.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.c1oappe.top/gtqytrlgrf.html

[Q06] 删除列
来源：http://hz.shanyushiyangtech.top/gtoppwqqld.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.gotoacloud.top/gtvknhmkmr.html

[Q07] 删除表
来源：http://hz.daxiang520.top/gtyvckwiva.html

DROP TABLE IF EXISTS orders;
来源：http://hz.svipenyu.cn/gtygfzjmez.html

[Q08] 创建普通索引
来源：http://hz.cqqwz.cn/gtizuftozo.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.shanyushiyangtech.top/gtpjbbinqa.html

[Q09] 创建唯一索引
来源：http://hz.dashuyun.cn/gthgwdlhbr.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.meibo888.top/gtlvrbjxlu.html

[Q10] 插入单行
来源：http://hz.yangfankeji.com/gtuniurvjm.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.ehwqpu.com/gtztalggkd.html

[Q11] 一次插入多行
来源：http://hz.shangyingyoupin.top/gtmcfjlcfy.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.hongshengwenyu.top/gtormuxlbn.html

[Q12] 插入后取自增 ID
来源：http://hz.0kj1m.cn/gtitflxzaw.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.yuxming.cn/gtlnpvsyhq.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.yongpay.top/gtuoeizoms.html

[Q13] 忽略重复插入
来源：http://hz.hfpthk.cn/gtlzzsexns.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.zdqjudy.top/gthxcrufjx.html

[Q14] 存在则更新（upsert）
来源：http://hz.tianlin.xyz/gtevyocban.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.jqgufenzy.top/gtyrjknjpw.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.shanyushiyangtech.top/gtzdcgosvx.html

[Q15] 查询全部
来源：http://hz.aibaodan.cn/gtyaimtxoh.html

SELECT * FROM users;
来源：http://hz.zdqjudy.top/gtkzgpkrcc.html

[Q16] 查询指定列
来源：http://hz.iojbl.cn/gtxspffibm.html

SELECT id, name FROM users;
来源：http://hz.wangshuangyany.cn/gtghxqzkfp.html

[Q17] 条件查询
来源：http://hz.c1oappe.top/gthapbabqr.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.gotoacloud.top/gtuewrpprc.html

[Q18] 模糊匹配
来源：http://hz.c1oappe.top/gtngmfqvxi.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.aizwys.cn/gtchteyhbd.html

[Q19] 范围查询
来源：http://hz.yuxming.cn/gtbapmopqq.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.guannengcc.top/gtpouofryk.html

[Q20] IN 列表
来源：http://hz.havefunace.top/gtjhqyfqaa.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.hfpthk.cn/gttelvjlmp.html

[Q21] 空值判断
来源：http://hz.c1oappe.top/gtuhxmqnce.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.iojbl.cn/gtxxrhujkf.html

[Q22] 排序
来源：http://hz.jinqigfzy.top/gttqznmvxc.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.daria6918.cn/gtityggyes.html

[Q23] 分页
来源：http://hz.redwolf501.top/gtkgwwdkwl.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.316326.xyz/gttztuujme.html

[Q24] 去重
来源：http://hz.shuidangran.top/gtlakzsfcn.html

SELECT DISTINCT city FROM users;
来源：http://hz.ivvv.top/gttgsoafoe.html

[Q25] 只取前 N 条
来源：http://hz.yanxiufei.cn/gtzhurhijm.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.gzhubu.top/gtcufycpih.html

[Q26] 计数
来源：http://hz.52xcode.cn/gtcaeelfjn.html

SELECT COUNT(*) FROM users;
来源：http://hz.zhiwuduotai.top/gtbwwchjwb.html

[Q27] 条件计数
来源：http://hz.jqgufenzy.top/gtjmgyilcu.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.dianchejie.cn/gtwbltzdzi.html

[Q28] 求和与平均
来源：http://hz.0kj1m.cn/gtwbixslvg.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.shangyingyoupin.top/gtzbqpzcxl.html

[Q29] 最大最小值
来源：http://hz.shangyingyoupin.top/gtxiqefcus.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.dianchejie.cn/gtluvqxpjz.html

[Q30] 分组统计
来源：http://hz.hammf.cn/gtyoqnrdcb.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.jinqigufen.top/gttonqrlfh.html

[Q31] 分组后过滤
来源：http://hz.yonumen.top/gthjcvkrnx.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.aizwys.cn/gtiktxavbb.html

[Q32] 分组拼接字符串
来源：http://hz.dashuyun.cn/gtpfvjdjdb.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.cdnleiting.top/gtpwoinqdh.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.cqqwz.cn/gtxklnapuh.html

[Q33] 多列分组
来源：http://hz.ybcxt.top/gtijeabfjt.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.yonumen.top/gtidedvnft.html

[Q34] 每组取第一条
来源：http://hz.andypj.xyz/gtjbnfovuf.html

SELECT * FROM (
来源：http://hz.yvedp.cn/gtgywwegyc.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.chenjidiqi.icu/gtrshwpcuq.html

) t WHERE rn = 1;
来源：http://hz.sweek.top/gtbisgbhnl.html

[Q35] 内连接
来源：http://hz.hywenlv.cn/gtfaxxstli.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.snrcjt.cn/gtrawnavdt.html

[Q36] 左连接
来源：http://hz.sufxvd.cn/gtknrrfren.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.zhengqikj.top/gtlqwvnsas.html

[Q37] 右连接
来源：http://hz.ppjwa.cn/gtzkqklrvn.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.xziqi.cn/gtgurnnxmj.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.yj20258888.top/gtykqtveuy.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.andypj.xyz/gtjlrvfobz.html

[Q39] 自连接（查上下级）
来源：http://hz.gotoacloud.top/gthideungb.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.bjfxy.top/gtonrvkiwx.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.redwolf501.top/gtdqwemett.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.haohaochexian.top/gtfgfhcmvg.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.hysaishi.cn/gtbjsjjchg.html

[Q41] 多表连接
来源：http://hz.tanke756.top/gtbgqifles.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.yongpay.top/gtldwkeijo.html

JOIN users u ON u.id = o.user_id
来源：http://hz.cheryme.top/gtpxrbbznl.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.hfpthk.cn/gtfqzhhote.html

[Q42] 连接条件附加过滤
来源：http://hz.meibo888.top/gtzfdnebkx.html

SELECT u.name, o.amount FROM users u
来源：http://hz.zhaomingkeji.xyz/gtvfjeqdhe.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.wangshuangyany.cn/gtfqlropzi.html

[Q43] 标量子查询
来源：http://hz.jlsjyb.cn/gtetsjpgru.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.yongpay.top/gtfgtdyqtf.html

[Q44] IN 子查询
来源：http://hz.yangfankeji.com/gtyedfiyqv.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.ivvv.top/gtjeqjtona.html

[Q45] EXISTS 判断存在
来源：http://hz.ppjwa.cn/gtjwgupdxk.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.zhiwuduotai.top/gtpjlmuxmj.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.guannengcc.top/gtzfystvrs.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.gotoacloud.top/gtubivxwot.html

[Q47] 与平均值比较
来源：http://hz.dianchejie.cn/gtaospcnjh.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.tian-w.cn/gtjtkthnqh.html

[Q48] CTE 公用表表达式
来源：http://hz.xylfe.cn/gtqmehbshg.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.yuanzhike.top/gtnkhlfwug.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.jinqigfzy.top/gtbrpfyekz.html

[Q49] 更新单行
来源：http://hz.aibaodan.cn/gtldjhptfh.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.hfpthk.cn/gttrecrmbd.html

[Q50] 批量更新
来源：http://hz.chenlongwang.top/gtdgrdurff.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.hywenlv.cn/gtvagmaxgi.html

[Q51] 用子查询更新
来源：http://hz.pengpengdd.cyou/gtmhjbnjps.html


<!-- 参考信息 -->