代发 wailian999

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.redwolf501.top/gttvqasygr.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.zdqjudy.top/gtuhaqrdpg.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.ehwqpu.com/gtwxjbqnkv.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.jyoumei.cn/gtyckukoeq.html

[N05] 最大公约数
来源：http://hz.svipenyu.cn/gtkqlqaubk.html

Py:   math.gcd(a, b)
来源：http://hz.hywenlv.cn/gtxbsklmog.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.zhaomingkeji.xyz/gtpweixkdw.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.cucudq.cn/gthqdoquyn.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.hysaishi.cn/gttgnrpqtl.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.guowangkeji.top/gtlogafhwq.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.zdqjudy.top/gtvghqqrca.html

Ruby: a.gcd(b)
来源：http://hz.feifeiyinyue.top/gtoxdtogyi.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.52xcode.cn/gtkumwygoo.html

[N06] 判断回文字符串
来源：http://hz.ppjwa.cn/gtabykakqr.html

Py:   s == s[::-1]
来源：http://hz.nanxuanxn.top/gtdwzdqluy.html

PHP:  $s === strrev($s);
来源：http://hz.xuanzx.com/gtniaulnxh.html

JS:   s === [...s].reverse().join("")
来源：http://hz.zhixingplan.top/gthxgwxyoh.html

TS:   s === [...s].reverse().join("")
来源：http://hz.sxryk.cn/gtoqouqylm.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.haohaochexian.top/gtivgbabgw.html

Go:   // 双指针从两端比较
来源：http://hz.quarkkingdee.top/gtsxrtotoo.html

Ruby: s == s.reverse
来源：http://hz.chenlongwang.top/gtcgtlupyd.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.gogol.net.cn/gtyltkorts.html

[N07] 两数之和（返回下标）
来源：http://hz.jinqigfzy.top/gtxnbckeax.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.hammf.cn/gtjitmrlqr.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.shuidangran.top/gtxqgrfniw.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.yueranfly.top/gtxbbaahun.html

TS:   // 手写 Map<string, number>
来源：http://hz.hysaishi.cn/gtbuzpbzwf.html

Java: // 手写 HashMap
来源：http://hz.zhijiandao.cn/gttidzsift.html

Go:   // 手写 map[int]int
来源：http://hz.hnxiangtu.top/gtklgnmugg.html

Ruby: // 手写 Hash
来源：http://hz.zdqjudy.top/gtwjyvblko.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.hnxiangtu.top/gtbhuusnam.html

[N08] 生成全排列
来源：http://hz.svipenyu.cn/gtdxyrlyct.html

Py:   itertools.permutations(arr)
来源：http://hz.pengpengdd.cyou/gtckfojtkm.html

PHP:  // 手写递归交换
来源：http://hz.kuanghao11.cn/gtlnnbhait.html

JS:   // 手写回溯递归
来源：http://hz.bjfxy.top/gtoslifodd.html

TS:   // 手写回溯递归
来源：http://hz.nanxuanxn.top/gtfoyufveg.html

Java: // 手写回溯递归
来源：http://hz.yuanzhike.top/gtivuqkgjv.html

Go:   // 手写回溯递归
来源：http://hz.snrcjt.cn/gtnmxmvvfd.html

Ruby: arr.permutation.to_a
来源：http://hz.shzxlz.cn/gthdkqxhhr.html

C#:   // 手写回溯递归
来源：http://hz.zdqjudy.top/gtbdthzqyz.html

[N09] 栈与队列
来源：http://hz.meibo888.top/gtvjyhmmoo.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.fengsongda.top/gteguvinie.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.nwbrower.top/gtadeeeovo.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.0kj1m.cn/gteemyrxoy.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.havefunace.top/gttchsaynl.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.tianlin.xyz/gtqaxfghhf.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.iojbl.cn/gtryvkffcn.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.jqgfzy.top/gtnrkeqdsg.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.ydzc1.top/gtwgplkgzb.html

[N10] 链表节点定义
来源：http://hz.pycfn.com/gtxzlualzf.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.meibo888.top/gtfbccsybq.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.tianlin.xyz/gtscqbjtjs.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.zhiwuduotai.top/gtgjrslwqf.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.havefunace.top/gtmwvzveyp.html

Java: class Node { int v; Node next; }
来源：http://hz.quarkkingdee.top/gtfqpajdyo.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.xylfe.cn/gtglqjponh.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.chenjidiqi.icu/gtawtzfubu.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.ywan-chungtsiang.top/gtypmukerm.html

[N11] 二叉树中序遍历
来源：http://hz.redwolf501.top/gttgmjhwdg.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.havefunace.top/gtoqnwamqk.html

PHP:  // 手写递归函数
来源：http://hz.xinyue.icu/gtshxicecq.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.ivvv.top/gtmfmpkrez.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.dashuyun.cn/gtmdretwzd.html

Java: // 手写递归
来源：http://hz.yanxiufei.cn/gtamzhkejh.html

Go:   // 手写递归
来源：http://hz.shzxlz.cn/gtrpnkfbhc.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.aizwys.cn/gtfhewwfhh.html

C#:   // 手写递归
来源：http://hz.0kj1m.cn/gtzyoiufnj.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.gaohongyu789.top/gtjmacmzdz.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.xylfe.cn/gtgaennedx.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.jyoumei.cn/gtyjcagatu.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.jinghuilouyu.cn/gtiyygnaxs.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.xuanzx.com/gtqbyjwtzq.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.0kj1m.cn/gtvxdfbujk.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.svipenyu.cn/gtksrhwoql.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.yvedp.cn/gtuqgpayrx.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.vqdsnc.cn/gthsddhrtm.html

================================================================================
来源：http://hz.yj20258.top/gtfpcuizpz.html

O. 并发与异步
来源：http://hz.andypj.xyz/gtqgkexhdi.html

================================================================================
来源：http://hz.jyoumei.cn/gtukyexmmg.html

[O01] 启动一个线程
来源：http://hz.yj20258.top/gtipvnhiig.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.jinqigfzy.top/gttkcvwpfd.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.nanxinkj.top/gtfxplofmm.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.yj20258.top/gtockusczg.html

TS:   // 同 JS
来源：http://hz.shuidangran.top/gtgctcmxzi.html

Java: new Thread(() -> f()).start()
来源：http://hz.cheryme.top/gttivroenq.html

Go:   go f()
来源：http://hz.zhixingplan.top/gtnottxias.html

Ruby: Thread.new { f }
来源：http://hz.jyoumei.cn/gtmmnbxbuz.html

C#:   Task.Run(() => F());
来源：http://hz.tanke756.top/gtetvdvrup.html

[O02] 使用线程池
来源：http://hz.redwolf501.top/gtpllkqezb.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.ydjk.org.cn/gtprkpupaq.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.xuetiantiany.cn/gtdlzbsugp.html

JS:   // worker_threads 线程池
来源：http://hz.0kj1m.cn/gtepbmyqwk.html

TS:   // worker_threads 线程池
来源：http://hz.cashguo.top/gtuchptezk.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.cheryme.top/gtihvpkuid.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.hfpthk.cn/gtkbcmeipf.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.tanke756.top/gtcttkmhjw.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.cqqwz.cn/gtnsoaijly.html

[O03] 加锁保护共享数据
来源：http://hz.yvedp.cn/gtrrhehsoz.html

Py:   with lock: shared += 1
来源：http://hz.yj20258888.top/gtwqdkewww.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.sxryk.cn/gtlzxsgsgx.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.haohaochexian.top/gtwnwrgkmd.html

TS:   // 同 JS
来源：http://hz.zhiwuduotai.top/gttxvszkyw.html

Java: synchronized (this) { shared++; }
来源：http://hz.sufxvd.cn/gttxuthlel.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.aibaodan.cn/gtsgtzxegm.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.yuxming.cn/gtlmbclcbe.html

C#:   lock (gate) { shared++; }
来源：http://hz.c1oappe.top/gtjecoeoal.html

[O04] 定义异步函数并等待
来源：http://hz.dashuyun.cn/gtmcbndblr.html

Py:   async def f():⏎    await g()
来源：http://hz.jlsjyb.cn/gtaxygsapj.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.sweek.top/gtctltxezg.html

JS:   async function f() { await g(); }
来源：http://hz.cashguo.top/gtebybymje.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.jinqigufen.top/gtolnpafds.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.hysaishi.cn/gtavbsktcq.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.redwolf501.top/gtrntzfucy.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.zycfv.cn/gtrpfhjnwa.html

C#:   async Task F() { await G(); }
来源：http://hz.ehwqpu.com/gtulfwsmnl.html

[O05] 并发执行并等待全部完成
来源：http://hz.smart0.xyz/gtukyowory.html

Py:   asyncio.gather(*tasks)
来源：http://hz.gaohongyu789.top/gtpcmhgcxz.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.ybcxt.top/gtniegngzu.html

JS:   await Promise.all(tasks)
来源：http://hz.svipenyu.cn/gtlrkwqouj.html

TS:   await Promise.all(tasks)
来源：http://hz.zhixingplan.top/gtrarnytea.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.iojbl.cn/gtvykyoimc.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.ydjk.org.cn/gthiuxaelr.html

Ruby: threads.map(&:join)
来源：http://hz.shuidangran.top/gtfhbqhhvp.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.xingfuxueyuan.xyz/gtcpzsxavk.html

[O06] 使用进程池
来源：http://hz.meibo888.top/gtoykdecch.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.9152youxi.cn/gtqkntexfq.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.hysaishi.cn/gtsmlavuse.html

JS:   // child_process / cluster 模块
来源：http://hz.andypj.xyz/gtunfsjldc.html

TS:   // child_process / cluster 模块
来源：http://hz.cqqwz.cn/gtsjrkpmsq.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.hnxiangtu.top/gtooansyto.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.haohaochexian.top/gtlvqtscfy.html

Ruby: // fork 块
来源：http://hz.sweek.top/gtcngbolez.html

C#:   Parallel.For
来源：http://hz.wangdashe.top/gtyhpoxjls.html

================================================================================
来源：http://hz.daxiang520.top/gtcdyfxioi.html

P. 常用工具函数
来源：http://hz.zhaomingkeji.xyz/gtruisgscb.html

================================================================================
来源：http://hz.52xcode.cn/gtcjorpnsv.html

[P01] 生成 UUID
来源：http://hz.0kj1m.cn/gtpmuzecid.html

Py:   str(uuid.uuid4())
来源：http://hz.iojbl.cn/gtoxyqpebb.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.yangfankeji.com/gtxvmdmiws.html

JS:   crypto.randomUUID()
来源：http://hz.yj202588.top/gtpuaxqpzj.html

TS:   crypto.randomUUID()
来源：http://hz.smart0.xyz/gtvmhhooas.html

Java: UUID.randomUUID().toString()
来源：http://hz.xziqi.cn/gtrvpohqsq.html

Go:   // 用 github.com/google/uuid
来源：http://hz.dashuyun.cn/gtoictyfur.html

Ruby: SecureRandom.uuid
来源：http://hz.gzhubu.top/gtvmvmzchp.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.gaohongyu789.top/gtjqjwqsrg.html

[P02] MD5 / SHA256 摘要
来源：http://hz.xinyue.icu/gtrotlwomb.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.zhaomingkeji.xyz/gtbnziicxd.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.cdnleiting.top/gtfkzekfge.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.gzhubu.top/gthrpblcya.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.zdqjudy.top/gtutrkabeo.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.vqdsnc.cn/gthpcotbpa.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.sxryk.cn/gtfltrphpb.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.chenlongwang.top/gtdmblumgr.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.c1oappe.top/gtfcmxholn.html

[P03] 生成短随机字符串
来源：http://hz.sysykeji.top/gtmljelmdw.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.zhijiandao.cn/gtvrthfarj.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.chenzaomai.com/gtuaxtmjuf.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.quarkkingdee.top/gtqsspcyuv.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.nanxuanxn.top/gthumdlpku.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.iojbl.cn/gtwtkgtors.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.cqqwz.cn/gtkxtpyjxl.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.zhijiandao.cn/gtxogjeapj.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.52xcode.cn/gtafqrnkah.html

[P04] 求长度
来源：http://hz.xuanzx.com/gtamppikba.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.chenzaomai.com/gtzcsimueq.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.wangshuangyany.cn/gtiqcquvye.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.xingfuxueyuan.xyz/gtqttsvjzj.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.316326.xyz/gtgqighpaj.html

Java: list.size();  map.size();  s.length()
来源：http://hz.fengsongda.top/gtkamitscm.html

Go:   len(arr);  len(m)
来源：http://hz.jqgfzy.top/gthgjfeaqt.html

Ruby: x.length;  x.size
来源：http://hz.dianchejie.cn/gtlgfzbnro.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.jinqigufen.top/gtnpabbrkd.html

[P05] 判断两个对象内容是否相等
来源：http://hz.pycfn.com/gtjkrqlyvv.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.smart0.xyz/gtiyvcecqs.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.hongshengwenyu.top/gtgfgsehdf.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.cheryme.top/gtmaxkaeyz.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.mhx1999.top/gtdmatdwnc.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.nwbrower.top/gtehrbyzas.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.chenjidiqi.icu/gtmtcunhmr.html

Ruby: a == b
来源：http://hz.tianlin.xyz/gtkjnvzqkm.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.xingfuxueyuan.xyz/gtczlpepsi.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.yj202588.top/gtcyryikgb.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.fzhhl.top/gtozhxkqpo.html

PHP:  if (empty($x)) {}
来源：http://hz.yangfankeji.com/gttvlvqrbs.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.pengpengdd.cyou/gteqkoliqf.html

TS:   if (x == null) {}
来源：http://hz.gzhubu.top/gtxhscrzmx.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.nwbrower.top/gtfvuiqegx.html

Go:   if x == nil {}
来源：http://hz.guowangkeji.top/gtcgfqbolo.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.zhongyouzk.top/gtthhtondi.html

C#:   if (x is null) {}
来源：http://hz.xziqi.cn/gtfaekdbri.html

[P07] 防抖与节流
来源：http://hz.daria6918.cn/gtmfeekvms.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.52xcode.cn/gtxiatwrdl.html

PHP:  // 手写时间戳比较
来源：http://hz.aibaodan.cn/gtxfnhidqm.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.shanyushiyangtech.top/gtjnxovipe.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.yuanzhike.top/gtlbtuasoo.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.shanyushiyangkeji.top/gtypbqewht.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.feifeiyinyue.top/gtxniyujyc.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.vqdsnc.cn/gtepczzbdx.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.wangshuangyany.cn/gtlgdpvymc.html

[P08] 处理浮点精度问题
来源：http://hz.hfpthk.cn/gtxfypfsoz.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.yvedp.cn/gtqciyazyx.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.xylfe.cn/gtcsvlakfb.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.iojbl.cn/gtjqpxdbeg.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.cashguo.top/gtqurqafkw.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.yueranfly.top/gtzgwzmdqa.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.daxiang520.top/gtgoariugc.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.xziqi.cn/gtqtanjzmo.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.zhongyouzk.top/gtrtxzyjtk.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtliamjjkq.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.xylfe.cn/gtxgfjlnmz.html

================================================================================
来源：http://hz.birdmap.top/gtiafgskty.html

[Q01] 创建表
来源：http://hz.hywenlv.cn/gtktwcsupz.html

CREATE TABLE users (
来源：http://hz.hfpthk.cn/gtscbhfikq.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.zhixingplan.top/gtbsafqmbf.html

name VARCHAR(50) NOT NULL,
来源：http://hz.hywenlv.cn/gtcbzydwzd.html

email VARCHAR(100) UNIQUE,
来源：http://hz.ydzc1.top/gtnbptooua.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.hysaishi.cn/gtxdkbwivr.html

);
来源：http://hz.yanxiufei.cn/gtwdxhrwuu.html

[Q02] 创建带外键的表
来源：http://hz.fzhhl.top/gtzlghzktp.html

CREATE TABLE orders (
来源：http://hz.yuxming.cn/gtjsootwdo.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.sxryk.cn/gtbbsxamvl.html

user_id INT NOT NULL,
来源：http://hz.hfpthk.cn/gtcrqazqgg.html

amount DECIMAL(10, 2),
来源：http://hz.birdmap.top/gtcaepaeol.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.jiagoushi.top/gtdttcdhup.html

);
来源：http://hz.mhx1999.top/gtyqjahoru.html

[Q03] 增加列
来源：http://hz.zdqjudy.top/gtjbtvtirh.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.jinghuilouyu.cn/gteqiuuejg.html

[Q04] 修改列类型
来源：http://hz.cheryme.top/gtxzeboqbx.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.sysykeji.top/gtzbrgbpam.html

[Q05] 重命名列
来源：http://hz.hnqzz.top/gtvkvyihyz.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.yuxming.cn/gthavfojfa.html

[Q06] 删除列
来源：http://hz.xuanzx.com/gtqjpqeerj.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.iojbl.cn/gtjmsphrxi.html

[Q07] 删除表
来源：http://hz.sufxvd.cn/gtcepkevpi.html

DROP TABLE IF EXISTS orders;
来源：http://hz.havefunace.top/gtomewjvtr.html

[Q08] 创建普通索引
来源：http://hz.yuxming.cn/gtvrafkfsn.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.0kj1m.cn/gtrikpcbiu.html

[Q09] 创建唯一索引
来源：http://hz.daxiang520.top/gtjpwzgmyg.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.ywan-chungtsiang.top/gtgpkgykad.html

[Q10] 插入单行
来源：http://hz.yuanzhike.top/gtkquqglex.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.0kj1m.cn/gtirtlhkiz.html

[Q11] 一次插入多行
来源：http://hz.hammf.cn/gtvyqyrroh.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.yj20258.top/gtvmzgwepr.html

[Q12] 插入后取自增 ID
来源：http://hz.nanxinkj.top/gthpozpsji.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.shzxlz.cn/gtuuqmvgjw.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.iojbl.cn/gtmvdinrgt.html

[Q13] 忽略重复插入
来源：http://hz.feifeiyinyue.top/gtmbhggyfn.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.zhijiandao.cn/gtvguznuvo.html

[Q14] 存在则更新（upsert）
来源：http://hz.tian-w.cn/gtlqajkzaz.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.dashuyun.cn/gtthrxoucb.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.bjfxy.top/gtgqhsaipe.html

[Q15] 查询全部
来源：http://hz.hnxiangtu.top/gtsqrnwxse.html

SELECT * FROM users;
来源：http://hz.yangfankeji.com/gtbpurjihu.html

[Q16] 查询指定列
来源：http://hz.xylfe.cn/gttaqsyzok.html

SELECT id, name FROM users;
来源：http://hz.wangdashe.top/gtvsfbpikz.html

[Q17] 条件查询
来源：http://hz.shzxlz.cn/gtlntzcszb.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.yj202588.top/gtadvcwnit.html

[Q18] 模糊匹配
来源：http://hz.feifeiyinyue.top/gtzoqlscrt.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.jianghu66.top/gtbtecytmm.html

[Q19] 范围查询
来源：http://hz.zycfv.cn/gtbylhgvrp.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.xinyue.icu/gtsstggtgk.html

[Q20] IN 列表
来源：http://hz.andypj.xyz/gtqkofkcyu.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.redwolf501.top/gtpwzozdqo.html

[Q21] 空值判断
来源：http://hz.daria6918.cn/gtklvydiwx.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.jlsjyb.cn/gtwthijnqv.html

[Q22] 排序
来源：http://hz.svipenyu.cn/gtvrdvbwis.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.hysaishi.cn/gtsjyrffqt.html

[Q23] 分页
来源：http://hz.feifeiyinyue.top/gtulecypra.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.ehwqpu.com/gtfcckibzz.html

[Q24] 去重
来源：http://hz.svipenyu.cn/gtdljyxaoy.html

SELECT DISTINCT city FROM users;
来源：http://hz.zycfv.cn/gtihdhsuif.html

[Q25] 只取前 N 条
来源：http://hz.gaohongyu789.top/gtffkaaqmd.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.9152youxi.cn/gteuyegsxo.html

[Q26] 计数
来源：http://hz.redwolf501.top/gtqzawqpzc.html

SELECT COUNT(*) FROM users;
来源：http://hz.ppjwa.cn/gtbdmlcuqn.html

[Q27] 条件计数
来源：http://hz.jlsjyb.cn/gtirsfzwaf.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.shuidangran.top/gtjazoknlu.html

[Q28] 求和与平均
来源：http://hz.daria6918.cn/gtrxponaua.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.haohaochexian.top/gtoahdfdcn.html

[Q29] 最大最小值
来源：http://hz.andypj.xyz/gtckchobzk.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.zhengqikj.top/gtzlgyimmg.html

[Q30] 分组统计
来源：http://hz.aibaodan.cn/gtgroyufmr.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.yj202588.top/gtrlluvcwh.html

[Q31] 分组后过滤
来源：http://hz.zdqjudy.top/gtcnmtmpak.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.ppjwa.cn/gtgknffirq.html

[Q32] 分组拼接字符串
来源：http://hz.quarkkingdee.top/gtahjiqodk.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.tian-w.cn/gtbajbksmn.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.ydzc1.top/gteojkfefy.html

[Q33] 多列分组
来源：http://hz.yuanzhike.top/gtcxkjqage.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.havefunace.top/gtzzsxtnaf.html

[Q34] 每组取第一条
来源：http://hz.zhongyouzk.top/gtpfiwlvvl.html

SELECT * FROM (
来源：http://hz.haohaochexian.top/gtehyxbrdr.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.yanxiufei.cn/gtuqofpabj.html

) t WHERE rn = 1;
来源：http://hz.0kj1m.cn/gtbuqiywin.html

[Q35] 内连接
来源：http://hz.hfpthk.cn/gtshizjcbn.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.nanxuanxn.top/gtjzthaopn.html

[Q36] 左连接
来源：http://hz.zhijiandao.cn/gtfxumsmrs.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.zhijiandao.cn/gteamhoavh.html

[Q37] 右连接
来源：http://hz.shanyushiyangtech.top/gtajxhcarw.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.c1oappe.top/gtcjvxptlt.html


<!-- 参考信息 -->