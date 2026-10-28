代发 wailian999

Java: // 手写回溯递归
来源：http://hz.hywenlv.cn/gttzvhtxxj.html

Go:   // 手写回溯递归
来源：http://hz.jyoumei.cn/gtlsguhbdm.html

Ruby: arr.permutation.to_a
来源：http://hz.shuidangran.top/gtcuzgflyx.html

C#:   // 手写回溯递归
来源：http://hz.shzxlz.cn/gtbybeoikk.html

[N09] 栈与队列
来源：http://hz.jianghu66.top/gtmpkefnit.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.aibaodan.cn/gtpsfrhtdz.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.jiagoushi.top/gthzhhsxuu.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.chenzaomai.com/gttsefqzfd.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.cqqwz.cn/gtpknxeiwh.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.yuxming.cn/gtljpscqqb.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.jqgfzy.top/gtvlfzqfqp.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.fengsongda.top/gtijftjuqo.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.birdmap.top/gtrwlsoxmp.html

[N10] 链表节点定义
来源：http://hz.yueranfly.top/gtcbpvctrw.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.feifeiyinyue.top/gtcrzbtxcs.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.havefunace.top/gtkiqiuadk.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.smart0.xyz/gtrutmoudn.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.xuetiantiany.cn/gtcfevluws.html

Java: class Node { int v; Node next; }
来源：http://hz.zdqjudy.top/gtbjawcxyb.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.yj20258.top/gtqjcbtwij.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.shzxlz.cn/gtqiiapvoi.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.nwbrower.top/gtnzrnyrkv.html

[N11] 二叉树中序遍历
来源：http://hz.zhongyouzk.top/gtkaenqerc.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.jiagoushi.top/gtzsqylyyn.html

PHP:  // 手写递归函数
来源：http://hz.pengpengdd.cyou/gtxdnyemgq.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.chenzaomai.com/gtswkthwkl.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.zhongyouzk.top/gtjuppbqsm.html

Java: // 手写递归
来源：http://hz.zhaomingkeji.xyz/gtmuxoyfos.html

Go:   // 手写递归
来源：http://hz.gzhubu.top/gtfbcshnvq.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.xuanzx.com/gtkpjrokuo.html

C#:   // 手写递归
来源：http://hz.hfpthk.cn/gtrslwtaqg.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.yongpay.top/gtzgmszbdb.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.snrcjt.cn/gtitcgnaty.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.nwbrower.top/gtxgyuolxd.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.xuetiantiany.cn/gttjwivvfw.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.shanyushiyangkeji.top/gtugpgmdcv.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.iojbl.cn/gtlljjgoak.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.hywenlv.cn/gtawmrilyr.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.hnxiangtu.top/gtugraudbs.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.andypj.xyz/gttewaqsej.html

================================================================================
来源：http://hz.yanxiufei.cn/gtopwcdtgp.html

O. 并发与异步
来源：http://hz.shanyushiyangtech.top/gtfetdflel.html

================================================================================
来源：http://hz.yuanzhike.top/gtewokzfht.html

[O01] 启动一个线程
来源：http://hz.c1oappe.top/gtlzbpnegr.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.bjfxy.top/gtxkdbvnno.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.0kj1m.cn/gtvfaowbvr.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.jianghu66.top/gtjywiggzh.html

TS:   // 同 JS
来源：http://hz.tian-w.cn/gtdsjhozci.html

Java: new Thread(() -> f()).start()
来源：http://hz.shanyushiyangkeji.top/gtqurqcrfd.html

Go:   go f()
来源：http://hz.shuidangran.top/gtpzcprzjv.html

Ruby: Thread.new { f }
来源：http://hz.cqqwz.cn/gtbivaqwpw.html

C#:   Task.Run(() => F());
来源：http://hz.nwbrower.top/gtzzpmdbye.html

[O02] 使用线程池
来源：http://hz.xuanzx.com/gtcgtyxmbc.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.iojbl.cn/gtkhnexjrf.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.shangyingyoupin.top/gtypyqgnns.html

JS:   // worker_threads 线程池
来源：http://hz.jlsjyb.cn/gtjfgbbjzm.html

TS:   // worker_threads 线程池
来源：http://hz.shanyushiyangkeji.top/gtyxrqvuwe.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.chenjidiqi.icu/gtusosaufd.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.hysaishi.cn/gtpzkulqaz.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.jinqigfzy.top/gtythttdzo.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.fengsongda.top/gtrceojhwz.html

[O03] 加锁保护共享数据
来源：http://hz.ybcxt.top/gtswmsvtpm.html

Py:   with lock: shared += 1
来源：http://hz.shuidangran.top/gtcotizbco.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.snrcjt.cn/gtlpmdjher.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.zhaomingkeji.xyz/gtwguqvaym.html

TS:   // 同 JS
来源：http://hz.svipenyu.cn/gtyuchvqdo.html

Java: synchronized (this) { shared++; }
来源：http://hz.ydjk.org.cn/gtrwlnwsem.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.fzhhl.top/gtnoajmlxk.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.aizwys.cn/gtxbdfmqth.html

C#:   lock (gate) { shared++; }
来源：http://hz.dianchejie.cn/gtxjtiryhu.html

[O04] 定义异步函数并等待
来源：http://hz.yj20258.top/gttvseniaz.html

Py:   async def f():⏎    await g()
来源：http://hz.jlsjyb.cn/gtkygxibbc.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.jinghuilouyu.cn/gtbfjfiojl.html

JS:   async function f() { await g(); }
来源：http://hz.zycfv.cn/gtrewllfac.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.zhiwuduotai.top/gtbzuyuxeh.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.zdqjudy.top/gtssobpxzl.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.xuetiantiany.cn/gtysbejggw.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.316326.xyz/gtsgxfwtzy.html

C#:   async Task F() { await G(); }
来源：http://hz.guannengcc.top/gtjugxesmh.html

[O05] 并发执行并等待全部完成
来源：http://hz.316326.xyz/gtmghnrobd.html

Py:   asyncio.gather(*tasks)
来源：http://hz.tianlin.xyz/gtftpcieja.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.yangfankeji.com/gtxbmwhbgv.html

JS:   await Promise.all(tasks)
来源：http://hz.yanxiufei.cn/gtkycqfqbq.html

TS:   await Promise.all(tasks)
来源：http://hz.jyoumei.cn/gtmttimufu.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.zycfv.cn/gtchlwyqiz.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.quarkkingdee.top/gtifnursqt.html

Ruby: threads.map(&:join)
来源：http://hz.xinyue.icu/gtpnkruojb.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.aibaodan.cn/gtdckbvvta.html

[O06] 使用进程池
来源：http://hz.cdnleiting.top/gtirxbjugy.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.cdnleiting.top/gtdkkklfoj.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.cqqwz.cn/gtrwkixjqu.html

JS:   // child_process / cluster 模块
来源：http://hz.bjfxy.top/gtclpjsdpj.html

TS:   // child_process / cluster 模块
来源：http://hz.gaohongyu789.top/gtacllibgq.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.c1oappe.top/gtyqgbtbha.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.hongshengwenyu.top/gtibiemnwj.html

Ruby: // fork 块
来源：http://hz.jqgufenzy.top/gtyoxxjidi.html

C#:   Parallel.For
来源：http://hz.zhiwuduotai.top/gtpjceylnt.html

================================================================================
来源：http://hz.jqgfzy.top/gtdrpoykaj.html

P. 常用工具函数
来源：http://hz.ywan-chungtsiang.top/gtmfanobwk.html

================================================================================
来源：http://hz.dashuyun.cn/gtufwwpcla.html

[P01] 生成 UUID
来源：http://hz.zdqjudy.top/gtygavjzke.html

Py:   str(uuid.uuid4())
来源：http://hz.yangfankeji.com/gtqlsqvcei.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.xylfe.cn/gtbctfzprb.html

JS:   crypto.randomUUID()
来源：http://hz.xuetiantiany.cn/gtkgugfiab.html

TS:   crypto.randomUUID()
来源：http://hz.gzhubu.top/gtexaxcmns.html

Java: UUID.randomUUID().toString()
来源：http://hz.ppjwa.cn/gtocbfyyqq.html

Go:   // 用 github.com/google/uuid
来源：http://hz.havefunace.top/gtcipzpatk.html

Ruby: SecureRandom.uuid
来源：http://hz.aizwys.cn/gtmcpmijtg.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.zhiwuduotai.top/gtzvogeqek.html

[P02] MD5 / SHA256 摘要
来源：http://hz.jlsjyb.cn/gtstpzsogf.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.jyoumei.cn/gtshfnqslc.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.wangshuangyany.cn/gtmvbdtlxc.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.sxryk.cn/gtmkcehtrp.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.bjfxy.top/gtpjemxloc.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.wangshuangyany.cn/gtchieaoyd.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.ybcxt.top/gtwqtbudgi.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.iojbl.cn/gtrvcwobqa.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.haohaochexian.top/gtaoyhicmd.html

[P03] 生成短随机字符串
来源：http://hz.jinyuanbaomall.cn/gtgrsdxooj.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.chenjidiqi.icu/gtvhthniaw.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.yuanzhike.top/gteukybiwj.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.jinghuilouyu.cn/gtrjslcirf.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.dashuyun.cn/gtpwrcmpno.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.havefunace.top/gttagwuuqt.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.ppjwa.cn/gtazsvwfvb.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.guannengcc.top/gtpuzzivcu.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.jinghuilouyu.cn/gtuenpalel.html

[P04] 求长度
来源：http://hz.smart0.xyz/gtcvmvmnoj.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.fengsongda.top/gttexjyega.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.feifeiyinyue.top/gtdnisagxy.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.ydjk.org.cn/gtbrftonfq.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.meibo888.top/gttmxamhul.html

Java: list.size();  map.size();  s.length()
来源：http://hz.daxiang520.top/gtaepqmvoz.html

Go:   len(arr);  len(m)
来源：http://hz.zhixingplan.top/gtqnqmwcnu.html

Ruby: x.length;  x.size
来源：http://hz.0kj1m.cn/gtvblnxjnw.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.hongshengwenyu.top/gtpopnwcxb.html

[P05] 判断两个对象内容是否相等
来源：http://hz.guowangkeji.top/gtufcyaaxe.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.redwolf501.top/gtcalbjhci.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.mhx1999.top/gtygexrcnk.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.gaohongyu789.top/gtayjowuwp.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.pycfn.com/gtprjywukn.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.ywan-chungtsiang.top/gtgpgmupda.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.hywenlv.cn/gtqinfwcwe.html

Ruby: a == b
来源：http://hz.haohaochexian.top/gtnhwdtpee.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.yongpay.top/gtokpbsuzg.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.guannengcc.top/gtgupugawp.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.tianlin.xyz/gtekruickz.html

PHP:  if (empty($x)) {}
来源：http://hz.316326.xyz/gteienuxns.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.52xcode.cn/gtdsqjfboo.html

TS:   if (x == null) {}
来源：http://hz.bjfxy.top/gtmowouwtz.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.9152youxi.cn/gtowtkcduq.html

Go:   if x == nil {}
来源：http://hz.guowangkeji.top/gtpunktrsm.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.zhixingplan.top/gtrovskpii.html

C#:   if (x is null) {}
来源：http://hz.chenzaomai.com/gtckubzjsv.html

[P07] 防抖与节流
来源：http://hz.ppjwa.cn/gtcwigpizp.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.ybcxt.top/gtnuxtktoi.html

PHP:  // 手写时间戳比较
来源：http://hz.hongshengwenyu.top/gtsuouqfds.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.hnqzz.top/gtfhxvgblx.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.jyoumei.cn/gtwxswliko.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.chenlongwang.top/gtwoayabvq.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.svipenyu.cn/gtgfntrhbe.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.yj20258.top/gtzrxoeazg.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.52xcode.cn/gtgwyzgcmm.html

[P08] 处理浮点精度问题
来源：http://hz.yuxming.cn/gtyrmgxyrn.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.0kj1m.cn/gtkkgjyzqb.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.guowangkeji.top/gtscbenxvy.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.zhixingplan.top/gtuqusdrfb.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.yj20258888.top/gtjquwvzhn.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.jinghuilouyu.cn/gttrajntua.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.yvedp.cn/gtojpepauf.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.dashuyun.cn/gtptdjklfm.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.ywan-chungtsiang.top/gtofwrwmkg.html

================================================================================
来源：http://hz.xziqi.cn/gtwwyqdewo.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.zhoulong.xyz/gtsskcwxzt.html

================================================================================
来源：http://hz.ydzc1.top/gtwvctnrpk.html

[Q01] 创建表
来源：http://hz.meibo888.top/gtqqexpxjq.html

CREATE TABLE users (
来源：http://hz.chenjidiqi.icu/gtexlckcog.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.smart0.xyz/gtlfdxnfpe.html

name VARCHAR(50) NOT NULL,
来源：http://hz.svipenyu.cn/gtjdqawken.html

email VARCHAR(100) UNIQUE,
来源：http://hz.fzhhl.top/gtnrahpxnf.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.yj202588.top/gtwryvnugj.html

);
来源：http://hz.yonumen.top/gtnglqiart.html

[Q02] 创建带外键的表
来源：http://hz.dianchejie.cn/gtbxelevfn.html

CREATE TABLE orders (
来源：http://hz.havefunace.top/gttrqkrejq.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.jinqigfzy.top/gtztitgwka.html

user_id INT NOT NULL,
来源：http://hz.jinqigfzy.top/gtgqjkdhlt.html

amount DECIMAL(10, 2),
来源：http://hz.guowangkeji.top/gteiusojeu.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.yj202588.top/gtgueyadnn.html

);
来源：http://hz.tianlin.xyz/gtooenkntj.html

[Q03] 增加列
来源：http://hz.feifeiyinyue.top/gtkdtgqhke.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.nwbrower.top/gtluclxwaj.html

[Q04] 修改列类型
来源：http://hz.ywan-chungtsiang.top/gtewaxjsyf.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.guowangkeji.top/gtlldwkxkw.html

[Q05] 重命名列
来源：http://hz.316326.xyz/gtubsbrocd.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.yj20258888.top/gtvhtqiprw.html

[Q06] 删除列
来源：http://hz.jinqigufen.top/gtkwlaseoj.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.shangyingyoupin.top/gtnawhbtow.html

[Q07] 删除表
来源：http://hz.kuanghao11.cn/gttfwitkgu.html

DROP TABLE IF EXISTS orders;
来源：http://hz.fengsongda.top/gthngqskgx.html

[Q08] 创建普通索引
来源：http://hz.yj202588.top/gtdhvlntib.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.redwolf501.top/gtnninzcqv.html

[Q09] 创建唯一索引
来源：http://hz.aibaodan.cn/gtqekgiwkv.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.yangfankeji.com/gtcbgavael.html

[Q10] 插入单行
来源：http://hz.gaohongyu789.top/gtazjgkyvv.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.sxryk.cn/gtuhqxnfww.html

[Q11] 一次插入多行
来源：http://hz.jinqigfzy.top/gtvxnldnxp.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.feifeiyinyue.top/gtcioendxr.html

[Q12] 插入后取自增 ID
来源：http://hz.zhongyouzk.top/gttxnlhqmu.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.ywan-chungtsiang.top/gtslssqvnt.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.hywenlv.cn/gtamurygfd.html

[Q13] 忽略重复插入
来源：http://hz.sxryk.cn/gtgygvoprg.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.meibo888.top/gtuxmgdrie.html

[Q14] 存在则更新（upsert）
来源：http://hz.gzhubu.top/gtdawnxakz.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.zhiwuduotai.top/gtlbwaduqf.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.zhaomingkeji.xyz/gtreulwmfq.html

[Q15] 查询全部
来源：http://hz.hongshengwenyu.top/gtnihtwdsg.html

SELECT * FROM users;
来源：http://hz.0kj1m.cn/gtihfeiicf.html

[Q16] 查询指定列
来源：http://hz.dashuyun.cn/gtpuobqgjl.html

SELECT id, name FROM users;
来源：http://hz.kuanghao11.cn/gtcxroeqtt.html

[Q17] 条件查询
来源：http://hz.316326.xyz/gtoumgldva.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.sxryk.cn/gtzducsuhi.html

[Q18] 模糊匹配
来源：http://hz.jinghuilouyu.cn/gtzlnlvsrj.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.52xcode.cn/gtaaukjekp.html

[Q19] 范围查询
来源：http://hz.fengsongda.top/gtghpyjtho.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.daria6918.cn/gtvopnpqfa.html

[Q20] IN 列表
来源：http://hz.gotoacloud.top/gtfbfmrckb.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.ydjk.org.cn/gticcrmdaj.html

[Q21] 空值判断
来源：http://hz.hywenlv.cn/gtbkuvpkif.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.xuetiantiany.cn/gtvwbznawi.html

[Q22] 排序
来源：http://hz.jyoumei.cn/gtasjjcmul.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.zhoulong.xyz/gtswiunwom.html

[Q23] 分页
来源：http://hz.c1oappe.top/gtzzvokikb.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.c1oappe.top/gtshljshxd.html

[Q24] 去重
来源：http://hz.yj20258888.top/gtwzgrurwe.html

SELECT DISTINCT city FROM users;
来源：http://hz.xinyue.icu/gtodxqicez.html

[Q25] 只取前 N 条
来源：http://hz.daria6918.cn/gthnnzufal.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.hysaishi.cn/gtowdjzbxr.html

[Q26] 计数
来源：http://hz.tianlin.xyz/gtuwowqazu.html

SELECT COUNT(*) FROM users;
来源：http://hz.gaohongyu789.top/gtydamnqtw.html

[Q27] 条件计数
来源：http://hz.yangfankeji.com/gtovmrpnnm.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.gzhubu.top/gtbovdrwsr.html

[Q28] 求和与平均
来源：http://hz.shuidangran.top/gthzmqxdol.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.jlsjyb.cn/gtqtamnvfl.html

[Q29] 最大最小值
来源：http://hz.snrcjt.cn/gtwctankpz.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.yongpay.top/gtaqtrcsrj.html

[Q30] 分组统计
来源：http://hz.daxiang520.top/gtncmnwevi.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.zhiwuduotai.top/gtxemjrhyr.html

[Q31] 分组后过滤
来源：http://hz.svipenyu.cn/gtkcbynfjw.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.cqqwz.cn/gtamxgegzd.html

[Q32] 分组拼接字符串
来源：http://hz.52xcode.cn/gtdwlfspqx.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.jinyuanbaomall.cn/gtcwdydzxc.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.zycfv.cn/gttrvexvik.html

[Q33] 多列分组
来源：http://hz.nwbrower.top/gttrlojuxb.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.gotoacloud.top/gtbffcqozz.html

[Q34] 每组取第一条
来源：http://hz.fengsongda.top/gtgiskmxdr.html

SELECT * FROM (
来源：http://hz.meibo888.top/gtmrwkpgsk.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.mhx1999.top/gtdavnbgjb.html

) t WHERE rn = 1;
来源：http://hz.redwolf501.top/gtdmuumskj.html

[Q35] 内连接
来源：http://hz.aizwys.cn/gtjlnxxysh.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.chenzaomai.com/gtkensttiv.html

[Q36] 左连接
来源：http://hz.bjfxy.top/gtmfseqopi.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.gzhubu.top/gtxmxtdsox.html

[Q37] 右连接
来源：http://hz.jinghuilouyu.cn/gtqnwsppif.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.hywenlv.cn/gtlhrutctu.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.jinyuanbaomall.cn/gtdypwakrd.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.pengpengdd.cyou/gthqifqgyx.html

[Q39] 自连接（查上下级）
来源：http://hz.jlsjyb.cn/gtptsivjnl.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.yueranfly.top/gtzwbykmmw.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.xuanzx.com/gtbexzdsug.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.tian-w.cn/gtyjikirgt.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.jyoumei.cn/gtefnkqlul.html

[Q41] 多表连接
来源：http://hz.pengpengdd.cyou/gtrvlzxale.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.ywan-chungtsiang.top/gtgalnvsog.html

JOIN users u ON u.id = o.user_id
来源：http://hz.xziqi.cn/gtqdfgponp.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.birdmap.top/gtiitsxchd.html

[Q42] 连接条件附加过滤
来源：http://hz.daxiang520.top/gtgtccvmxj.html

SELECT u.name, o.amount FROM users u
来源：http://hz.zhiwuduotai.top/gticqqizvk.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.cheryme.top/gtjnncnnjc.html

[Q43] 标量子查询
来源：http://hz.daria6918.cn/gtnycqhvdf.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.dianchejie.cn/gtgttdeidi.html

[Q44] IN 子查询
来源：http://hz.9152youxi.cn/gtcgxdzqlq.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.xylfe.cn/gtvwqgbqvz.html

[Q45] EXISTS 判断存在
来源：http://hz.yuxming.cn/gtbblkspqe.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.birdmap.top/gtrhxiinxq.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.yanxiufei.cn/gtvbrbetxf.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.jyoumei.cn/gtkesarehc.html

[Q47] 与平均值比较
来源：http://hz.xuanzx.com/gtckggktcf.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.zhongyouzk.top/gtyccwqnqc.html

[Q48] CTE 公用表表达式
来源：http://hz.sufxvd.cn/gtocvvmvqw.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.yonumen.top/gtrbwfheow.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.chenjidiqi.icu/gtvkfbyauy.html

[Q49] 更新单行
来源：http://hz.jqgufenzy.top/gtpzzadthp.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.zhoulong.xyz/gttwfkrdac.html

[Q50] 批量更新
来源：http://hz.tanke756.top/gtmxklacma.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.chenjidiqi.icu/gtiqiphoom.html

[Q51] 用子查询更新
来源：http://hz.yvedp.cn/gtoucbdqoc.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.yuanzhike.top/gtbogeiodx.html

[Q52] 删除指定行
来源：http://hz.sweek.top/gtbwrnuhgq.html

DELETE FROM users WHERE id = 10;
来源：http://hz.sxryk.cn/gtaghkhcnp.html

[Q53] 按条件删除
来源：http://hz.ppjwa.cn/gtdpcactzd.html


<!-- 参考信息 -->