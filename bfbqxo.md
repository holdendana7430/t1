代发 wailian999

[N05] 最大公约数
来源：http://hz.jqgufenzy.top/gtgrirdvpb.html

Py:   math.gcd(a, b)
来源：http://hz.jinqigfzy.top/gtuvnplqmd.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.xuetiantiany.cn/gtgqsdwtzq.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.xuanzx.com/gtpwuvoqdd.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.andypj.xyz/gtquwbbrff.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.hnqzz.top/gtmiuebwpg.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.meibo888.top/gtkzujiazx.html

Ruby: a.gcd(b)
来源：http://hz.ywan-chungtsiang.top/gtognmeozx.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.ydzc1.top/gtpwzrdhei.html

[N06] 判断回文字符串
来源：http://hz.sxryk.cn/gtwggmtwxw.html

Py:   s == s[::-1]
来源：http://hz.chenjidiqi.icu/gtjgdvlfoj.html

PHP:  $s === strrev($s);
来源：http://hz.chenzaomai.com/gtymmtutxs.html

JS:   s === [...s].reverse().join("")
来源：http://hz.aizwys.cn/gtxgkhhuri.html

TS:   s === [...s].reverse().join("")
来源：http://hz.yj20258.top/gtcemaplxf.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.dashuyun.cn/gtarblutan.html

Go:   // 双指针从两端比较
来源：http://hz.mhx1999.top/gtjxiptydu.html

Ruby: s == s.reverse
来源：http://hz.aizwys.cn/gtekyoyvvw.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.ehwqpu.com/gtzueqfmxi.html

[N07] 两数之和（返回下标）
来源：http://hz.ybcxt.top/gtrofxtzfu.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.nanxuanxn.top/gtwjypmuqz.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.guowangkeji.top/gtlrywnutg.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.vqdsnc.cn/gttoffpdvl.html

TS:   // 手写 Map<string, number>
来源：http://hz.snrcjt.cn/gtbdpphrkj.html

Java: // 手写 HashMap
来源：http://hz.fzhhl.top/gtxzdxzthx.html

Go:   // 手写 map[int]int
来源：http://hz.sweek.top/gtnpvlebtq.html

Ruby: // 手写 Hash
来源：http://hz.gogol.net.cn/gtssobdrtt.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.shzxlz.cn/gtdfnilfzz.html

[N08] 生成全排列
来源：http://hz.yonumen.top/gtqgnyyulu.html

Py:   itertools.permutations(arr)
来源：http://hz.hnxiangtu.top/gtpivuuvyg.html

PHP:  // 手写递归交换
来源：http://hz.dashuyun.cn/gtpvbtpzeh.html

JS:   // 手写回溯递归
来源：http://hz.aizwys.cn/gtquonnyjz.html

TS:   // 手写回溯递归
来源：http://hz.ehwqpu.com/gtlzrvqqad.html

Java: // 手写回溯递归
来源：http://hz.smart0.xyz/gtygrmapff.html

Go:   // 手写回溯递归
来源：http://hz.zdqjudy.top/gtnehxyfvy.html

Ruby: arr.permutation.to_a
来源：http://hz.xingfuxueyuan.xyz/gtpmnwhkgn.html

C#:   // 手写回溯递归
来源：http://hz.dashuyun.cn/gtawktadfg.html

[N09] 栈与队列
来源：http://hz.yj20258888.top/gtnhfczgin.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.gaohongyu789.top/gtskrfvcwv.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.andypj.xyz/gtcovqipri.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.cdnleiting.top/gticanbxzl.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.ehwqpu.com/gtksrpuamy.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.aizwys.cn/gtkfsxufyi.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.xuetiantiany.cn/gtagffsznq.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.mhx1999.top/gtvxlyymzz.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.jinghuilouyu.cn/gtyzhskgvy.html

[N10] 链表节点定义
来源：http://hz.svipenyu.cn/gtcjdzsmqs.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.gotoacloud.top/gtfficaqbv.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.hnqzz.top/gtngouncfx.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.yj20258.top/gtbnjtpwpm.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.birdmap.top/gtyppegjrj.html

Java: class Node { int v; Node next; }
来源：http://hz.sufxvd.cn/gtyprlbjmu.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.xingfuxueyuan.xyz/gtosldekbb.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.ivvv.top/gtdachgwsu.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.zhaomingkeji.xyz/gtjiyxrkng.html

[N11] 二叉树中序遍历
来源：http://hz.shangyingyoupin.top/gtjeesrxbw.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.cqqwz.cn/gtgvbrtavg.html

PHP:  // 手写递归函数
来源：http://hz.gogol.net.cn/gtnrmfudrt.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.tanke756.top/gtxahrginr.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.c1oappe.top/gtpigtquxt.html

Java: // 手写递归
来源：http://hz.aibaodan.cn/gtlbnzyrkr.html

Go:   // 手写递归
来源：http://hz.sysykeji.top/gtpemmncmj.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.birdmap.top/gtckceujlv.html

C#:   // 手写递归
来源：http://hz.haohaochexian.top/gtatnvxezx.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.316326.xyz/gtjmwhdztq.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.fzhhl.top/gthilfukyy.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.pengpengdd.cyou/gteyqsdcfp.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.quarkkingdee.top/gtsztuigkf.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.pengpengdd.cyou/gtfnrrscdd.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.zhiwuduotai.top/gtwhtkjfmw.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.tianlin.xyz/gtsrqbkntf.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.fengsongda.top/gtcszflgnt.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.yj20258.top/gteefmjxgu.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtotwaosuq.html

O. 并发与异步
来源：http://hz.yj20258888.top/gtyoznnoko.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtuxwklbuw.html

[O01] 启动一个线程
来源：http://hz.sysykeji.top/gtohutzouq.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.ehwqpu.com/gtdlvmcgxw.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.nanxinkj.top/gtnxopykvc.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.c1oappe.top/gtpghabshq.html

TS:   // 同 JS
来源：http://hz.tanke756.top/gtvicabzuh.html

Java: new Thread(() -> f()).start()
来源：http://hz.cheryme.top/gtndiaiypi.html

Go:   go f()
来源：http://hz.xuetiantiany.cn/gtyemefmlu.html

Ruby: Thread.new { f }
来源：http://hz.yuanzhike.top/gtpdkwzedg.html

C#:   Task.Run(() => F());
来源：http://hz.fzhhl.top/gttargyukx.html

[O02] 使用线程池
来源：http://hz.meibo888.top/gthzhlqjng.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.chenlongwang.top/gtfoyitqxx.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.vqdsnc.cn/gtpmowlfem.html

JS:   // worker_threads 线程池
来源：http://hz.havefunace.top/gtwtwtsoxw.html

TS:   // worker_threads 线程池
来源：http://hz.jinyuanbaomall.cn/gtzwhimqws.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.shuidangran.top/gtgeekwlir.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.birdmap.top/gthukneqbc.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.zhaomingkeji.xyz/gtcjyvlzbl.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.kuanghao11.cn/gtnmwuvfeb.html

[O03] 加锁保护共享数据
来源：http://hz.zhijiandao.cn/gtocmknvou.html

Py:   with lock: shared += 1
来源：http://hz.c1oappe.top/gtxqigniuf.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.cucudq.cn/gtzojfmnfb.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.mhx1999.top/gtxhxwuecp.html

TS:   // 同 JS
来源：http://hz.quarkkingdee.top/gtmnwpfodz.html

Java: synchronized (this) { shared++; }
来源：http://hz.svipenyu.cn/gtplxbbijt.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.daxiang520.top/gtftzcimji.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.zhaomingkeji.xyz/gtkwexfznc.html

C#:   lock (gate) { shared++; }
来源：http://hz.haohaochexian.top/gtvbwikmki.html

[O04] 定义异步函数并等待
来源：http://hz.guowangkeji.top/gtbmdfyutq.html

Py:   async def f():⏎    await g()
来源：http://hz.guannengcc.top/gtjsrufnoc.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.ydzc1.top/gtvwsiqitp.html

JS:   async function f() { await g(); }
来源：http://hz.chenzaomai.com/gtdpwrbiuw.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.zhoulong.xyz/gtnvimuoxe.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.nwbrower.top/gtmhapzvti.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.meibo888.top/gtdzyerlga.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.yongpay.top/gtemtqkjkz.html

C#:   async Task F() { await G(); }
来源：http://hz.yueranfly.top/gtteqwxfch.html

[O05] 并发执行并等待全部完成
来源：http://hz.iojbl.cn/gtuvpifzkv.html

Py:   asyncio.gather(*tasks)
来源：http://hz.chenjidiqi.icu/gtksilyvtx.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.haohaochexian.top/gtjgtzstau.html

JS:   await Promise.all(tasks)
来源：http://hz.zhoulong.xyz/gtmzddzied.html

TS:   await Promise.all(tasks)
来源：http://hz.meibo888.top/gtyecpytgb.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.jiagoushi.top/gtapbcykhj.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.yueranfly.top/gtdcutilqs.html

Ruby: threads.map(&:join)
来源：http://hz.ehwqpu.com/gthbvnbnhg.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.shzxlz.cn/gtfxfmfagm.html

[O06] 使用进程池
来源：http://hz.gaohongyu789.top/gtegklwrgu.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.zhiwuduotai.top/gtwjwrsolq.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.cqqwz.cn/gtolqdqafa.html

JS:   // child_process / cluster 模块
来源：http://hz.hnxiangtu.top/gtrdbjjbky.html

TS:   // child_process / cluster 模块
来源：http://hz.yonumen.top/gttbmieuhc.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.andypj.xyz/gtaaaeddyl.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.vqdsnc.cn/gtwalzycyh.html

Ruby: // fork 块
来源：http://hz.shzxlz.cn/gtunticnmd.html

C#:   Parallel.For
来源：http://hz.yuanzhike.top/gtxoulnocu.html

================================================================================
来源：http://hz.yanxiufei.cn/gttepzzbmj.html

P. 常用工具函数
来源：http://hz.meibo888.top/gtequmdgjb.html

================================================================================
来源：http://hz.hnxiangtu.top/gtdkljilpi.html

[P01] 生成 UUID
来源：http://hz.xuetiantiany.cn/gthjihffgs.html

Py:   str(uuid.uuid4())
来源：http://hz.ywan-chungtsiang.top/gthtaqfbkr.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.shuidangran.top/gtadthempm.html

JS:   crypto.randomUUID()
来源：http://hz.pycfn.com/gttrigaaxh.html

TS:   crypto.randomUUID()
来源：http://hz.pycfn.com/gtlrjheqry.html

Java: UUID.randomUUID().toString()
来源：http://hz.yonumen.top/gtaeptfvsu.html

Go:   // 用 github.com/google/uuid
来源：http://hz.cashguo.top/gtuysjkcmd.html

Ruby: SecureRandom.uuid
来源：http://hz.shzxlz.cn/gthxwqtbgm.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.daria6918.cn/gtbiqlvgwa.html

[P02] MD5 / SHA256 摘要
来源：http://hz.daxiang520.top/gtxvpgfuwz.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.nanxuanxn.top/gtrdoiobzo.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.jianghu66.top/gtsdeyjqja.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.snrcjt.cn/gtiurussqw.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.xuanzx.com/gtvyfhxbpu.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.smart0.xyz/gtxmfrxrgb.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.jinqigufen.top/gtsaibmmco.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.svipenyu.cn/gtkydkxcpp.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.zhixingplan.top/gtxsylnjik.html

[P03] 生成短随机字符串
来源：http://hz.smart0.xyz/gtbynrybio.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.redwolf501.top/gtdohxepfl.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.shanyushiyangkeji.top/gtrgbpbpar.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.zhaomingkeji.xyz/gtdnjgbxci.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.daria6918.cn/gttlvfjbtf.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.yj202588.top/gtvgpxaxkh.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.zycfv.cn/gtyeduirjc.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.feifeiyinyue.top/gtocohcltk.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.guowangkeji.top/gtyyclatkg.html

[P04] 求长度
来源：http://hz.9152youxi.cn/gtgrbboafr.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.yvedp.cn/gtcpxfpfaz.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.hysaishi.cn/gtiossyamu.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.ivvv.top/gttnceqdnd.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.hfpthk.cn/gtreskvrig.html

Java: list.size();  map.size();  s.length()
来源：http://hz.dianchejie.cn/gthpczonzj.html

Go:   len(arr);  len(m)
来源：http://hz.zycfv.cn/gtysrrzbns.html

Ruby: x.length;  x.size
来源：http://hz.nanxinkj.top/gtojlckdze.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.dianchejie.cn/gttwcnmvmc.html

[P05] 判断两个对象内容是否相等
来源：http://hz.snrcjt.cn/gtskkyscgw.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.nanxuanxn.top/gttjrchfuf.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.pycfn.com/gtdrthizlu.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.shanyushiyangkeji.top/gtzuvxvnvr.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.jinyuanbaomall.cn/gtcmcjcazv.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.pengpengdd.cyou/gtykvijkxv.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.dianchejie.cn/gttlkarzno.html

Ruby: a == b
来源：http://hz.jqgufenzy.top/gtrcmgfsmk.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.xingfuxueyuan.xyz/gtovlyilca.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.aibaodan.cn/gtxckznpqz.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.shuidangran.top/gtgvhiaqds.html

PHP:  if (empty($x)) {}
来源：http://hz.9152youxi.cn/gtmxfvpljd.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.xingfuxueyuan.xyz/gtyzjqjwzo.html

TS:   if (x == null) {}
来源：http://hz.bjfxy.top/gtzyksvvqk.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.chenzaomai.com/gtxtoqiptn.html

Go:   if x == nil {}
来源：http://hz.shangyingyoupin.top/gtnxrjceln.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.shanyushiyangtech.top/gtpgbdyegz.html

C#:   if (x is null) {}
来源：http://hz.cheryme.top/gtxrqwrmhq.html

[P07] 防抖与节流
来源：http://hz.tanke756.top/gtcqewvcnn.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.vqdsnc.cn/gtccomhazm.html

PHP:  // 手写时间戳比较
来源：http://hz.jinqigfzy.top/gtpepyifma.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.jqgufenzy.top/gttvmuasdx.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.shuidangran.top/gtgvmibfem.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.tian-w.cn/gtxhalaxen.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.316326.xyz/gtfrlwbbip.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.cashguo.top/gtdotbspau.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.sxryk.cn/gtewxnpqsn.html

[P08] 处理浮点精度问题
来源：http://hz.jyoumei.cn/gtcrcuzylf.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.chenlongwang.top/gtziipvfta.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.jianghu66.top/gtiknhfclp.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.sysykeji.top/gtulgvowiu.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.daria6918.cn/gtekchqnul.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.52xcode.cn/gttsmlrkov.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.fengsongda.top/gtdgddihxw.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.c1oappe.top/gtujmiitki.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.jinqigufen.top/gtxvjmaopv.html

================================================================================
来源：http://hz.cqqwz.cn/gtdjtlfjaj.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.yvedp.cn/gtozezehsw.html

================================================================================
来源：http://hz.gaohongyu789.top/gtaokekref.html

[Q01] 创建表
来源：http://hz.0kj1m.cn/gtapurbzxb.html

CREATE TABLE users (
来源：http://hz.jinqigfzy.top/gtpcucpscp.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.hnxiangtu.top/gtvjyxyozp.html

name VARCHAR(50) NOT NULL,
来源：http://hz.yuxming.cn/gtjbgszkri.html

email VARCHAR(100) UNIQUE,
来源：http://hz.wangdashe.top/gtumfpevvs.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.ybcxt.top/gtlnlooakx.html

);
来源：http://hz.sxryk.cn/gttfzysnsi.html

[Q02] 创建带外键的表
来源：http://hz.yongpay.top/gtyhohjoza.html

CREATE TABLE orders (
来源：http://hz.vqdsnc.cn/gtohxifudq.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.yangfankeji.com/gtmwejzxqf.html

user_id INT NOT NULL,
来源：http://hz.fengsongda.top/gtzlcanapi.html

amount DECIMAL(10, 2),
来源：http://hz.dashuyun.cn/gtdpbosxek.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.jyoumei.cn/gtrsgydixn.html

);
来源：http://hz.pycfn.com/gtdqmvcxhi.html

[Q03] 增加列
来源：http://hz.sufxvd.cn/gtcbszhwyt.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.meibo888.top/gtkgfmbxif.html

[Q04] 修改列类型
来源：http://hz.guowangkeji.top/gtrurdfkfz.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.316326.xyz/gtbwitdfly.html

[Q05] 重命名列
来源：http://hz.wangdashe.top/gtruokvaxh.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.xuetiantiany.cn/gtyfspdneu.html

[Q06] 删除列
来源：http://hz.xinyue.icu/gtmtzshwrj.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.hammf.cn/gtuhruhzas.html

[Q07] 删除表
来源：http://hz.havefunace.top/gthpugicrw.html

DROP TABLE IF EXISTS orders;
来源：http://hz.aibaodan.cn/gtpoujhicg.html

[Q08] 创建普通索引
来源：http://hz.nwbrower.top/gtjkzcrviz.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.haohaochexian.top/gtxfpdajac.html

[Q09] 创建唯一索引
来源：http://hz.zdqjudy.top/gtpltykgtl.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.hammf.cn/gtqmnodurk.html

[Q10] 插入单行
来源：http://hz.zycfv.cn/gtgznyihvp.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.pycfn.com/gtxornwrqz.html

[Q11] 一次插入多行
来源：http://hz.yuxming.cn/gtyfqprwav.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.0kj1m.cn/gtjjojpheb.html

[Q12] 插入后取自增 ID
来源：http://hz.chenjidiqi.icu/gtheybaipo.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.jinqigfzy.top/gtdijtdgqg.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.jqgufenzy.top/gtqbcsqcbt.html

[Q13] 忽略重复插入
来源：http://hz.pengpengdd.cyou/gtlifuvufm.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.yueranfly.top/gtxcrlmirl.html

[Q14] 存在则更新（upsert）
来源：http://hz.nanxuanxn.top/gtonwprjeb.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.snrcjt.cn/gtpkmxfwsl.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.cqqwz.cn/gtfzlwfinz.html

[Q15] 查询全部
来源：http://hz.feifeiyinyue.top/gtctnmgaqs.html

SELECT * FROM users;
来源：http://hz.snrcjt.cn/gtybuvgquh.html

[Q16] 查询指定列
来源：http://hz.ehwqpu.com/gtrcftohob.html

SELECT id, name FROM users;
来源：http://hz.jianghu66.top/gtgnaftfwt.html

[Q17] 条件查询
来源：http://hz.jinghuilouyu.cn/gtwlbaoezs.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.cashguo.top/gtetrfzfqn.html

[Q18] 模糊匹配
来源：http://hz.quarkkingdee.top/gtnxfchcjp.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.shangyingyoupin.top/gtadecnjit.html

[Q19] 范围查询
来源：http://hz.fengsongda.top/gtwhjwgytl.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.gzhubu.top/gtigjoodzg.html

[Q20] IN 列表
来源：http://hz.ydzc1.top/gtblmpwxzn.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.yuanzhike.top/gtcpukmhbr.html

[Q21] 空值判断
来源：http://hz.sufxvd.cn/gtoxebeljt.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.zhoulong.xyz/gtofpewgcc.html

[Q22] 排序
来源：http://hz.yuanzhike.top/gtffdxdqrn.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.zhiwuduotai.top/gtfmugrsin.html

[Q23] 分页
来源：http://hz.jqgfzy.top/gtrounqloj.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.chenjidiqi.icu/gtoskvjtxr.html

[Q24] 去重
来源：http://hz.pengpengdd.cyou/gtphyilqpw.html

SELECT DISTINCT city FROM users;
来源：http://hz.mhx1999.top/gtvldnoqce.html

[Q25] 只取前 N 条
来源：http://hz.chenjidiqi.icu/gtgmpqpvvu.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.birdmap.top/gtmezhamds.html

[Q26] 计数
来源：http://hz.guowangkeji.top/gtoaxqjnhk.html

SELECT COUNT(*) FROM users;
来源：http://hz.zhaomingkeji.xyz/gtncwsiixt.html

[Q27] 条件计数
来源：http://hz.haohaochexian.top/gtwdxsgoac.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.redwolf501.top/gtqxdwcicz.html

[Q28] 求和与平均
来源：http://hz.nanxuanxn.top/gtdhulirvu.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.guannengcc.top/gtqsqbczpz.html

[Q29] 最大最小值
来源：http://hz.hnxiangtu.top/gtgmnhebcj.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.zhaomingkeji.xyz/gtqrywvtzt.html

[Q30] 分组统计
来源：http://hz.vqdsnc.cn/gtgpzunmxh.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.ywan-chungtsiang.top/gttfwapkqm.html

[Q31] 分组后过滤
来源：http://hz.hammf.cn/gtksbyrxqr.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.zhixingplan.top/gtufeyocef.html

[Q32] 分组拼接字符串
来源：http://hz.yj202588.top/gtovjpfpfc.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.hnxiangtu.top/gtcoroneei.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.cashguo.top/gtjnycttsj.html

[Q33] 多列分组
来源：http://hz.xinyue.icu/gtcknmleke.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.gogol.net.cn/gtbrvoafbm.html

[Q34] 每组取第一条
来源：http://hz.zhiwuduotai.top/gtlbvwayhx.html

SELECT * FROM (
来源：http://hz.jqgfzy.top/gtwxjtlqqi.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.wangdashe.top/gtduvocywq.html

) t WHERE rn = 1;
来源：http://hz.jqgfzy.top/gtfjsbnnyu.html

[Q35] 内连接
来源：http://hz.iojbl.cn/gtoxjhrpth.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.jqgufenzy.top/gtowuspccq.html

[Q36] 左连接
来源：http://hz.cdnleiting.top/gtpienrqsv.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.feifeiyinyue.top/gtgwhezfpc.html

[Q37] 右连接
来源：http://hz.vqdsnc.cn/gtwhrvlarj.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.feifeiyinyue.top/gtiyxkulvx.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.zhixingplan.top/gtzpywubfq.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.zhixingplan.top/gttlduydlx.html

[Q39] 自连接（查上下级）
来源：http://hz.9152youxi.cn/gtwpgmvrko.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.jinqigufen.top/gtfwgcnltl.html


<!-- 参考信息 -->