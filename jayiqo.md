代发 wailian999

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.pycfn.com/gtrbbmbrri.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.ppjwa.cn/gtwzvvigdb.html

TS:   // 手写 Map<string, number>
来源：http://hz.c1oappe.top/gtigkzcgwz.html

Java: // 手写 HashMap
来源：http://hz.jqgfzy.top/gtkcogvfha.html

Go:   // 手写 map[int]int
来源：http://hz.chenzaomai.com/gtdwofhsid.html

Ruby: // 手写 Hash
来源：http://hz.hnqzz.top/gtrcqsizlj.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.cdnleiting.top/gtobcaakhf.html

[N08] 生成全排列
来源：http://hz.yanxiufei.cn/gttvipwkwd.html

Py:   itertools.permutations(arr)
来源：http://hz.shzxlz.cn/gtmodigdyj.html

PHP:  // 手写递归交换
来源：http://hz.guannengcc.top/gtpwwmwpnu.html

JS:   // 手写回溯递归
来源：http://hz.shanyushiyangkeji.top/gtzjivmiop.html

TS:   // 手写回溯递归
来源：http://hz.c1oappe.top/gtdffuusiv.html

Java: // 手写回溯递归
来源：http://hz.aizwys.cn/gtdefvzpmn.html

Go:   // 手写回溯递归
来源：http://hz.dashuyun.cn/gtrjedoglp.html

Ruby: arr.permutation.to_a
来源：http://hz.snrcjt.cn/gttdnljiwd.html

C#:   // 手写回溯递归
来源：http://hz.316326.xyz/gtuyxxielc.html

[N09] 栈与队列
来源：http://hz.52xcode.cn/gtjooduchu.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.xziqi.cn/gtrgkcdqec.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.gaohongyu789.top/gtnskohpne.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.zhiwuduotai.top/gthswaizdl.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.yj20258888.top/gtsjhdvtaf.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.xuetiantiany.cn/gthybzintx.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.guowangkeji.top/gtwyexotgq.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.aibaodan.cn/gtmdexbetd.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.jinghuilouyu.cn/gtgylauqzc.html

[N10] 链表节点定义
来源：http://hz.sysykeji.top/gtbwgsgcow.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.sufxvd.cn/gtzvsxzujh.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.yuxming.cn/gttuemiizs.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.redwolf501.top/gtibgcnzhg.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.yuanzhike.top/gtwtdluqht.html

Java: class Node { int v; Node next; }
来源：http://hz.yuanzhike.top/gtlqgmttqd.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.cucudq.cn/gtfkeverqp.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.yanxiufei.cn/gtemuhjsor.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.sufxvd.cn/gtappyemgi.html

[N11] 二叉树中序遍历
来源：http://hz.jianghu66.top/gtwgxrglpm.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.jinghuilouyu.cn/gtzoheuedr.html

PHP:  // 手写递归函数
来源：http://hz.shuidangran.top/gtriatmubj.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.jyoumei.cn/gtbetngigy.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.nanxinkj.top/gtuhpghbue.html

Java: // 手写递归
来源：http://hz.zhijiandao.cn/gtooohvqih.html

Go:   // 手写递归
来源：http://hz.chenlongwang.top/gtlvvqgjzw.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.xziqi.cn/gtmwbtxhrj.html

C#:   // 手写递归
来源：http://hz.zhaomingkeji.xyz/gtstdlrnrc.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.havefunace.top/gtstujhstp.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.yueranfly.top/gtfliorqat.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.yj20258.top/gtzsapspmn.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.zhixingplan.top/gttherrzjw.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.iojbl.cn/gtiaxbctvy.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.yvedp.cn/gtaadtlqta.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.yongpay.top/gtfapdljxp.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.zhijiandao.cn/gtaxfdbdmp.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.snrcjt.cn/gtgzvinwvs.html

================================================================================
来源：http://hz.fengsongda.top/gtsxzisyed.html

O. 并发与异步
来源：http://hz.yueranfly.top/gtbfowcyif.html

================================================================================
来源：http://hz.52xcode.cn/gtdqmdzwcp.html

[O01] 启动一个线程
来源：http://hz.ydzc1.top/gtdpdbqbmg.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.quarkkingdee.top/gtarkohuru.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.cheryme.top/gtjfuiucsp.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.52xcode.cn/gthzubxaks.html

TS:   // 同 JS
来源：http://hz.xingfuxueyuan.xyz/gtergowvff.html

Java: new Thread(() -> f()).start()
来源：http://hz.cheryme.top/gtreqduzcf.html

Go:   go f()
来源：http://hz.fengsongda.top/gtcmokzlkd.html

Ruby: Thread.new { f }
来源：http://hz.sxryk.cn/gtdahtivbb.html

C#:   Task.Run(() => F());
来源：http://hz.gzhubu.top/gtjqcvmsqm.html

[O02] 使用线程池
来源：http://hz.pengpengdd.cyou/gtmowjprrg.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.snrcjt.cn/gtwxrpzozd.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.316326.xyz/gtpbbvakvp.html

JS:   // worker_threads 线程池
来源：http://hz.chenlongwang.top/gtwenuauof.html

TS:   // worker_threads 线程池
来源：http://hz.jqgfzy.top/gtexkgbpjo.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.52xcode.cn/gthniklxtk.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.pengpengdd.cyou/gtwjdsmpib.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.ydzc1.top/gtcllewwql.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.tanke756.top/gtouupsoyk.html

[O03] 加锁保护共享数据
来源：http://hz.hnqzz.top/gtfpryktui.html

Py:   with lock: shared += 1
来源：http://hz.dianchejie.cn/gtbilrfpdk.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.yonumen.top/gtuqgdjxyq.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.zhiwuduotai.top/gtvohveakc.html

TS:   // 同 JS
来源：http://hz.gzhubu.top/gtdxzisxhx.html

Java: synchronized (this) { shared++; }
来源：http://hz.gzhubu.top/gtnnlnmhtf.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.kuanghao11.cn/gtvojcsgdl.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.chenlongwang.top/gtspwpojnj.html

C#:   lock (gate) { shared++; }
来源：http://hz.cqqwz.cn/gtwezzecjs.html

[O04] 定义异步函数并等待
来源：http://hz.yongpay.top/gtwvkegdxo.html

Py:   async def f():⏎    await g()
来源：http://hz.gzhubu.top/gtwsvhqsxi.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.c1oappe.top/gtykibwpkz.html

JS:   async function f() { await g(); }
来源：http://hz.yangfankeji.com/gtwdorvqak.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.yj20258.top/gtedgleuqs.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.jianghu66.top/gtqlnuigkq.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.guannengcc.top/gttujjltgk.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.ppjwa.cn/gthnuzyjqd.html

C#:   async Task F() { await G(); }
来源：http://hz.dianchejie.cn/gtpvmuclsi.html

[O05] 并发执行并等待全部完成
来源：http://hz.jinqigfzy.top/gtcwiiayxw.html

Py:   asyncio.gather(*tasks)
来源：http://hz.shuidangran.top/gtjyrsjmup.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.hfpthk.cn/gtlcojszho.html

JS:   await Promise.all(tasks)
来源：http://hz.guowangkeji.top/gtbgntwdqk.html

TS:   await Promise.all(tasks)
来源：http://hz.tian-w.cn/gthcqdjstm.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.jlsjyb.cn/gtvtrbeqca.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.jinqigfzy.top/gtauimqhmf.html

Ruby: threads.map(&:join)
来源：http://hz.chenlongwang.top/gtezwqrlfi.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.yj20258888.top/gtzeqmamzf.html

[O06] 使用进程池
来源：http://hz.guowangkeji.top/gtxjipgwvk.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.yj202588.top/gtrbqmwskq.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.fengsongda.top/gthibiwjqg.html

JS:   // child_process / cluster 模块
来源：http://hz.shangyingyoupin.top/gtdiwvcfxz.html

TS:   // child_process / cluster 模块
来源：http://hz.tian-w.cn/gtjwqwzedz.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.zdqjudy.top/gtxlzkmyjr.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.guannengcc.top/gtmtymslwm.html

Ruby: // fork 块
来源：http://hz.hongshengwenyu.top/gtooldqdek.html

C#:   Parallel.For
来源：http://hz.gotoacloud.top/gtvphkcbkv.html

================================================================================
来源：http://hz.tanke756.top/gtlagihrxk.html

P. 常用工具函数
来源：http://hz.daria6918.cn/gtccotepbp.html

================================================================================
来源：http://hz.fengsongda.top/gtawlpldkh.html

[P01] 生成 UUID
来源：http://hz.yj20258888.top/gtxmkkgmje.html

Py:   str(uuid.uuid4())
来源：http://hz.yuxming.cn/gtgizlrwvy.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.9152youxi.cn/gtjvpzwzjk.html

JS:   crypto.randomUUID()
来源：http://hz.yanxiufei.cn/gttyyyqent.html

TS:   crypto.randomUUID()
来源：http://hz.nanxinkj.top/gtxidalfhk.html

Java: UUID.randomUUID().toString()
来源：http://hz.yuxming.cn/gtkldqeggy.html

Go:   // 用 github.com/google/uuid
来源：http://hz.guowangkeji.top/gthjfacgwa.html

Ruby: SecureRandom.uuid
来源：http://hz.tanke756.top/gtczdhtfeg.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.yongpay.top/gtwwaebofw.html

[P02] MD5 / SHA256 摘要
来源：http://hz.gogol.net.cn/gtnryrfdwx.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.fzhhl.top/gthvomxzve.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.fengsongda.top/gtumokgqis.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.xuanzx.com/gtnwxxbdbi.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.jianghu66.top/gthbekccui.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.hysaishi.cn/gtgdmxcplt.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.yueranfly.top/gtdtxpaafl.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.wangshuangyany.cn/gtlpzesfnp.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.hnqzz.top/gtwusycuhi.html

[P03] 生成短随机字符串
来源：http://hz.fengsongda.top/gtyrwkpryx.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.shzxlz.cn/gtuntbfiou.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.fzhhl.top/gtvzhcmgkx.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.nanxuanxn.top/gttceuesms.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.zhiwuduotai.top/gtcmrzjind.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.ywan-chungtsiang.top/gtanakybqz.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.nwbrower.top/gtghtecwnj.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.yj20258.top/gtvetpueni.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.cqqwz.cn/gtqboyawhe.html

[P04] 求长度
来源：http://hz.hnqzz.top/gtirovshqh.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.tanke756.top/gtcotynwae.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.fzhhl.top/gtkcuizfyq.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.jinghuilouyu.cn/gtzgyuoocp.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.zhaomingkeji.xyz/gtztkxkqch.html

Java: list.size();  map.size();  s.length()
来源：http://hz.tanke756.top/gtbkjfkhgu.html

Go:   len(arr);  len(m)
来源：http://hz.yvedp.cn/gtvrrldmjx.html

Ruby: x.length;  x.size
来源：http://hz.xinyue.icu/gtxmeeqjzh.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.birdmap.top/gtniazgdby.html

[P05] 判断两个对象内容是否相等
来源：http://hz.jiagoushi.top/gtgaicbpet.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.birdmap.top/gtinylbdqp.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.xuanzx.com/gtgrdhkjyd.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.ydzc1.top/gtavjsnkcj.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.shzxlz.cn/gttmygyien.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.wangdashe.top/gtgureaplj.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.zhoulong.xyz/gtebjvotvd.html

Ruby: a == b
来源：http://hz.zhijiandao.cn/gtsusxjqfi.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.zhengqikj.top/gtfikxgbxj.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.sxryk.cn/gtpzlzmrjz.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.quarkkingdee.top/gtwmvltvej.html

PHP:  if (empty($x)) {}
来源：http://hz.xuetiantiany.cn/gtbnsnklbx.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.xuanzx.com/gtjcqwrmxj.html

TS:   if (x == null) {}
来源：http://hz.yj20258888.top/gtbfdstzbk.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.cheryme.top/gtbzzgpgtd.html

Go:   if x == nil {}
来源：http://hz.chenlongwang.top/gtddmupylm.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.jinghuilouyu.cn/gtippjnqvn.html

C#:   if (x is null) {}
来源：http://hz.sxryk.cn/gtrzbysjne.html

[P07] 防抖与节流
来源：http://hz.zycfv.cn/gtvnnmlmup.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.svipenyu.cn/gtefhtulrs.html

PHP:  // 手写时间戳比较
来源：http://hz.wangshuangyany.cn/gtwehiupbj.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.gzhubu.top/gthbdwowmb.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.gaohongyu789.top/gtlzcivesk.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.yueranfly.top/gtenwxuszx.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.dashuyun.cn/gtciyqnxil.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.jqgufenzy.top/gttyqaoemm.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.jinyuanbaomall.cn/gtdmybkvht.html

[P08] 处理浮点精度问题
来源：http://hz.chenzaomai.com/gttxqhxadm.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.0kj1m.cn/gtubkkxuqo.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.shzxlz.cn/gtrdghrlzb.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.redwolf501.top/gtffqpeqsi.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.zhaomingkeji.xyz/gtjiskgipp.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.havefunace.top/gtaqwbcpdx.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.9152youxi.cn/gtfasbofya.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.zhixingplan.top/gtppbexhqf.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.jinghuilouyu.cn/gtgkqdejli.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtgksdvlaz.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.shanyushiyangtech.top/gteiqjsbod.html

================================================================================
来源：http://hz.yj20258888.top/gtkedkiaqs.html

[Q01] 创建表
来源：http://hz.nanxinkj.top/gttajlsbrq.html

CREATE TABLE users (
来源：http://hz.0kj1m.cn/gtxqlmxxmu.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.havefunace.top/gtrbbufnot.html

name VARCHAR(50) NOT NULL,
来源：http://hz.daxiang520.top/gtjbqxdwvo.html

email VARCHAR(100) UNIQUE,
来源：http://hz.zhijiandao.cn/gtmhvoengm.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.ehwqpu.com/gthlupimfg.html

);
来源：http://hz.316326.xyz/gtgnxpnplb.html

[Q02] 创建带外键的表
来源：http://hz.vqdsnc.cn/gtststnhjq.html

CREATE TABLE orders (
来源：http://hz.yj20258.top/gtykjfzxmz.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.meibo888.top/gtohdzbgvs.html

user_id INT NOT NULL,
来源：http://hz.9152youxi.cn/gtfbilndcd.html

amount DECIMAL(10, 2),
来源：http://hz.aibaodan.cn/gtrhfukbbk.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.dianchejie.cn/gtxfmzcfdc.html

);
来源：http://hz.jqgufenzy.top/gtcgocnofm.html

[Q03] 增加列
来源：http://hz.xinyue.icu/gtwprcgaxn.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.jyoumei.cn/gthnftghkn.html

[Q04] 修改列类型
来源：http://hz.zhijiandao.cn/gtpsboldpd.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.cashguo.top/gtxzzaccvt.html

[Q05] 重命名列
来源：http://hz.yuanzhike.top/gtpfdqmnek.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.sxryk.cn/gtiwbtggcc.html

[Q06] 删除列
来源：http://hz.dashuyun.cn/gtlzoaxfus.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.iojbl.cn/gtzymizwsu.html

[Q07] 删除表
来源：http://hz.cheryme.top/gtxmnclrmk.html

DROP TABLE IF EXISTS orders;
来源：http://hz.jqgufenzy.top/gtkutlgkzx.html

[Q08] 创建普通索引
来源：http://hz.jinyuanbaomall.cn/gtxbjbetxe.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.yueranfly.top/gtwujbgpsc.html

[Q09] 创建唯一索引
来源：http://hz.zycfv.cn/gtnfmbzpvi.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.jqgufenzy.top/gtlgvscbzp.html

[Q10] 插入单行
来源：http://hz.ydjk.org.cn/gtetqqcvwm.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.jianghu66.top/gtcrxyioam.html

[Q11] 一次插入多行
来源：http://hz.svipenyu.cn/gtfqufdrng.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.fzhhl.top/gtpuzjdstb.html

[Q12] 插入后取自增 ID
来源：http://hz.chenlongwang.top/gtpukjuzbs.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.zhaomingkeji.xyz/gtlniqloav.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.c1oappe.top/gtqdeaeagb.html

[Q13] 忽略重复插入
来源：http://hz.0kj1m.cn/gtqdpvedkw.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.svipenyu.cn/gtpqabglrs.html

[Q14] 存在则更新（upsert）
来源：http://hz.yj20258888.top/gtcuezzkhi.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.chenzaomai.com/gtridymnwu.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.ppjwa.cn/gtmbanclgn.html

[Q15] 查询全部
来源：http://hz.hongshengwenyu.top/gthiatfovp.html

SELECT * FROM users;
来源：http://hz.yanxiufei.cn/gtxcwpvrex.html

[Q16] 查询指定列
来源：http://hz.tian-w.cn/gttgchlfsh.html

SELECT id, name FROM users;
来源：http://hz.svipenyu.cn/gtqkldrnxn.html

[Q17] 条件查询
来源：http://hz.gogol.net.cn/gtlvbbwnyk.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.bjfxy.top/gtuvfmkwbp.html

[Q18] 模糊匹配
来源：http://hz.shzxlz.cn/gtsdpglvmx.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.hnxiangtu.top/gtjusydekk.html

[Q19] 范围查询
来源：http://hz.tianlin.xyz/gtmsrpupsz.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.ywan-chungtsiang.top/gtkehjwmbe.html

[Q20] IN 列表
来源：http://hz.chenzaomai.com/gtazqaezcn.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.havefunace.top/gtihlswwbc.html

[Q21] 空值判断
来源：http://hz.yonumen.top/gtviddktei.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.sweek.top/gtsrtueczk.html

[Q22] 排序
来源：http://hz.guowangkeji.top/gtkdjxhiat.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.cucudq.cn/gtixdjpdhx.html

[Q23] 分页
来源：http://hz.chenzaomai.com/gtyfvturnw.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.kuanghao11.cn/gtjtgjwvqe.html

[Q24] 去重
来源：http://hz.316326.xyz/gtxetigbls.html

SELECT DISTINCT city FROM users;
来源：http://hz.fzhhl.top/gthozlbfku.html

[Q25] 只取前 N 条
来源：http://hz.pycfn.com/gtaaqubryq.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.ivvv.top/gtqybqfjnn.html

[Q26] 计数
来源：http://hz.zdqjudy.top/gthemhourn.html

SELECT COUNT(*) FROM users;
来源：http://hz.cucudq.cn/gtkafizvos.html

[Q27] 条件计数
来源：http://hz.hnxiangtu.top/gtidsrgrqj.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.zhengqikj.top/gtbuimsxfi.html

[Q28] 求和与平均
来源：http://hz.sysykeji.top/gtdpmvpsrb.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.yj20258888.top/gtwbsmyuch.html

[Q29] 最大最小值
来源：http://hz.zhengqikj.top/gtixykfjuv.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.0kj1m.cn/gtkkfnyozn.html

[Q30] 分组统计
来源：http://hz.shanyushiyangtech.top/gtydbncbwj.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.zhaomingkeji.xyz/gthoiyxydq.html

[Q31] 分组后过滤
来源：http://hz.yanxiufei.cn/gtzsqahaoy.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.jiagoushi.top/gthqinjhrg.html

[Q32] 分组拼接字符串
来源：http://hz.cucudq.cn/gtstoyqfbl.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.xuetiantiany.cn/gtkoksbmly.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.hywenlv.cn/gtppduvvco.html

[Q33] 多列分组
来源：http://hz.zhixingplan.top/gtkknjbrje.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.sufxvd.cn/gtgqcvdurj.html

[Q34] 每组取第一条
来源：http://hz.shzxlz.cn/gtciujfbox.html

SELECT * FROM (
来源：http://hz.fengsongda.top/gtigxoxpvp.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.pycfn.com/gtirjxrfxw.html

) t WHERE rn = 1;
来源：http://hz.cheryme.top/gtqrxqvyyo.html

[Q35] 内连接
来源：http://hz.jyoumei.cn/gtbvdhuyhj.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.cucudq.cn/gtfvxzqvjn.html

[Q36] 左连接
来源：http://hz.svipenyu.cn/gtuygluxip.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.sweek.top/gtyuvnjjzy.html

[Q37] 右连接
来源：http://hz.yj202588.top/gtczigynqq.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.hongshengwenyu.top/gtrvgjekom.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.smart0.xyz/gtvaugwvkq.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.jlsjyb.cn/gtugxlmkpm.html

[Q39] 自连接（查上下级）
来源：http://hz.hnxiangtu.top/gtmthdcxck.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.zhaomingkeji.xyz/gtbotrxpgs.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.shangyingyoupin.top/gtplydaxzs.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.yuxming.cn/gtngulpddp.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.tian-w.cn/gtsjvkzrpb.html

[Q41] 多表连接
来源：http://hz.yonumen.top/gtmxztxyhi.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.guowangkeji.top/gtehvpbffe.html

JOIN users u ON u.id = o.user_id
来源：http://hz.jlsjyb.cn/gtkrircekf.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.chenjidiqi.icu/gtgpkfcpvh.html

[Q42] 连接条件附加过滤
来源：http://hz.ivvv.top/gthxycmckx.html

SELECT u.name, o.amount FROM users u
来源：http://hz.zhijiandao.cn/gtifqvbbfe.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.hysaishi.cn/gthwgwrzrb.html

[Q43] 标量子查询
来源：http://hz.zdqjudy.top/gtvcsukfnr.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.sxryk.cn/gtnbipzdja.html

[Q44] IN 子查询
来源：http://hz.zhaomingkeji.xyz/gtbapqlwby.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.feifeiyinyue.top/gtnddqvldn.html

[Q45] EXISTS 判断存在
来源：http://hz.xuanzx.com/gttnxlxbfl.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.shanyushiyangtech.top/gtrdhgsveo.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.gzhubu.top/gtzyrvuqme.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.cheryme.top/gtborthyit.html

[Q47] 与平均值比较
来源：http://hz.zhaomingkeji.xyz/gtegoedjzb.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.aizwys.cn/gttozgpqzw.html


<!-- 参考信息 -->