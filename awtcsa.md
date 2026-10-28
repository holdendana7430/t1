代发 wailian999

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.gotoacloud.top/gtalpbribm.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.hysaishi.cn/gtvsneelvo.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.ydzc1.top/gtaecazbwi.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.daria6918.cn/gtjfqvtxky.html

[N05] 最大公约数
来源：http://hz.hnxiangtu.top/gtqqtaafhr.html

Py:   math.gcd(a, b)
来源：http://hz.hnqzz.top/gtbrtwhvym.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.cashguo.top/gtqfzfyrhn.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.redwolf501.top/gtuvrlzuco.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.hywenlv.cn/gttjvztjig.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.shuidangran.top/gttbyhceqq.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.yj20258.top/gtzsuigxbt.html

Ruby: a.gcd(b)
来源：http://hz.yj202588.top/gttpxhqwqq.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.mhx1999.top/gtbzhnqoug.html

[N06] 判断回文字符串
来源：http://hz.dashuyun.cn/gtrtrvzchs.html

Py:   s == s[::-1]
来源：http://hz.yuxming.cn/gtmscflgcu.html

PHP:  $s === strrev($s);
来源：http://hz.xuetiantiany.cn/gteaqagltu.html

JS:   s === [...s].reverse().join("")
来源：http://hz.hammf.cn/gtlmzulppm.html

TS:   s === [...s].reverse().join("")
来源：http://hz.smart0.xyz/gtadtzdxnf.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.wangshuangyany.cn/gtwobvdsam.html

Go:   // 双指针从两端比较
来源：http://hz.chenjidiqi.icu/gtagzdbdnf.html

Ruby: s == s.reverse
来源：http://hz.tian-w.cn/gtdnyzxuul.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.wangshuangyany.cn/gtsrerpfnc.html

[N07] 两数之和（返回下标）
来源：http://hz.quarkkingdee.top/gtiaqrlyyp.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.fzhhl.top/gtqjcnklob.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.hongshengwenyu.top/gtyprjcwkp.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.316326.xyz/gtvlvszwih.html

TS:   // 手写 Map<string, number>
来源：http://hz.shzxlz.cn/gtvpjaffoj.html

Java: // 手写 HashMap
来源：http://hz.ivvv.top/gtsrsyioam.html

Go:   // 手写 map[int]int
来源：http://hz.c1oappe.top/gtvcqjhfgm.html

Ruby: // 手写 Hash
来源：http://hz.zhengqikj.top/gtavsbluzo.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.bjfxy.top/gtoayfgzls.html

[N08] 生成全排列
来源：http://hz.zhaomingkeji.xyz/gtqlkbxsnp.html

Py:   itertools.permutations(arr)
来源：http://hz.c1oappe.top/gtgeokdbhz.html

PHP:  // 手写递归交换
来源：http://hz.zhoulong.xyz/gtcixchfrk.html

JS:   // 手写回溯递归
来源：http://hz.hongshengwenyu.top/gtyiomvyrh.html

TS:   // 手写回溯递归
来源：http://hz.ivvv.top/gtfoflwzee.html

Java: // 手写回溯递归
来源：http://hz.ivvv.top/gtxkpnzyom.html

Go:   // 手写回溯递归
来源：http://hz.svipenyu.cn/gtjryqmdba.html

Ruby: arr.permutation.to_a
来源：http://hz.yonumen.top/gtakkzysqm.html

C#:   // 手写回溯递归
来源：http://hz.jyoumei.cn/gtrbxxddlp.html

[N09] 栈与队列
来源：http://hz.redwolf501.top/gtixtjpwjc.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.yj20258888.top/gtzbzyhokt.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.bjfxy.top/gtdqgoccsp.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.feifeiyinyue.top/gthltpwkte.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.jqgufenzy.top/gtbonpgpbf.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.zhongyouzk.top/gtapyotnhv.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.yuanzhike.top/gtuizfuqrl.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.yvedp.cn/gtuwfrqivu.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.jianghu66.top/gtzxqytxvd.html

[N10] 链表节点定义
来源：http://hz.iojbl.cn/gttnhpwucf.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.hammf.cn/gtuhpknbde.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.chenlongwang.top/gtwileixcp.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.aibaodan.cn/gtmzffxfod.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.shanyushiyangkeji.top/gtfgyyhzqk.html

Java: class Node { int v; Node next; }
来源：http://hz.cucudq.cn/gtfjlhzmhq.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.gaohongyu789.top/gtrotpmnzk.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.yuanzhike.top/gtzojjffer.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.yanxiufei.cn/gtdrttxmdv.html

[N11] 二叉树中序遍历
来源：http://hz.sxryk.cn/gtvddahztc.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.wangshuangyany.cn/gtuuwkdbua.html

PHP:  // 手写递归函数
来源：http://hz.wangshuangyany.cn/gtleufnhsg.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.gaohongyu789.top/gtbhmtupvg.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.zhengqikj.top/gtvkenkonz.html

Java: // 手写递归
来源：http://hz.ydzc1.top/gtlcyrikmr.html

Go:   // 手写递归
来源：http://hz.ivvv.top/gtjbeyvjqd.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.jinyuanbaomall.cn/gticigtlrb.html

C#:   // 手写递归
来源：http://hz.svipenyu.cn/gtjkiyouzz.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.shanyushiyangkeji.top/gtsjrldqlb.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.zhongyouzk.top/gtstuuamlr.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.jyoumei.cn/gtvcddyuum.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.gzhubu.top/gtlucgmshk.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.dashuyun.cn/gtqlzuyppn.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.shanyushiyangkeji.top/gtmxvvdqry.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.pycfn.com/gtzzuraqiv.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.zycfv.cn/gtxoxulxkz.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.cashguo.top/gtrvglldtc.html

================================================================================
来源：http://hz.jianghu66.top/gtzwvqbohv.html

O. 并发与异步
来源：http://hz.aizwys.cn/gtcukligun.html

================================================================================
来源：http://hz.dianchejie.cn/gtrpnusahq.html

[O01] 启动一个线程
来源：http://hz.jianghu66.top/gtjwejpbha.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.shanyushiyangtech.top/gtoffsgnfr.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.feifeiyinyue.top/gtxreasxiw.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.yuxming.cn/gtgjjcemou.html

TS:   // 同 JS
来源：http://hz.havefunace.top/gtrqgfkebl.html

Java: new Thread(() -> f()).start()
来源：http://hz.jinyuanbaomall.cn/gtydyjlogm.html

Go:   go f()
来源：http://hz.jiagoushi.top/gtojnkvxhu.html

Ruby: Thread.new { f }
来源：http://hz.wangshuangyany.cn/gtawlngrdb.html

C#:   Task.Run(() => F());
来源：http://hz.mhx1999.top/gtigecpnfe.html

[O02] 使用线程池
来源：http://hz.nanxinkj.top/gttvvcuhlu.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.pycfn.com/gthpqboovh.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.shuidangran.top/gtuwgihnvz.html

JS:   // worker_threads 线程池
来源：http://hz.cashguo.top/gtqowwoygh.html

TS:   // worker_threads 线程池
来源：http://hz.hywenlv.cn/gtqtsarram.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.gaohongyu789.top/gtqlxwkrlj.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.shuidangran.top/gtwtcqvnyd.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.haohaochexian.top/gtiyjgnfxy.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.sweek.top/gtbgerwcpo.html

[O03] 加锁保护共享数据
来源：http://hz.tian-w.cn/gtanbpsypu.html

Py:   with lock: shared += 1
来源：http://hz.sweek.top/gtdkgjhfxn.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.zhoulong.xyz/gtiwrgttnv.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.hammf.cn/gtvzjwygwu.html

TS:   // 同 JS
来源：http://hz.shanyushiyangkeji.top/gtkdawhnwl.html

Java: synchronized (this) { shared++; }
来源：http://hz.shuidangran.top/gtxardvfcg.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.nanxuanxn.top/gtrqkbdlxp.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.zhijiandao.cn/gtedbjqbpq.html

C#:   lock (gate) { shared++; }
来源：http://hz.xziqi.cn/gtoclymcjt.html

[O04] 定义异步函数并等待
来源：http://hz.sxryk.cn/gtldgbojdy.html

Py:   async def f():⏎    await g()
来源：http://hz.iojbl.cn/gtovkxdvps.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.shanyushiyangkeji.top/gtmbvhnnxp.html

JS:   async function f() { await g(); }
来源：http://hz.hongshengwenyu.top/gteltodcgm.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.cdnleiting.top/gtvfoupjnu.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.jinyuanbaomall.cn/gtlptlucjz.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.meibo888.top/gtcihkcmua.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.tianlin.xyz/gtemvljtds.html

C#:   async Task F() { await G(); }
来源：http://hz.redwolf501.top/gtvsmykxyp.html

[O05] 并发执行并等待全部完成
来源：http://hz.haohaochexian.top/gtmuajjgha.html

Py:   asyncio.gather(*tasks)
来源：http://hz.yangfankeji.com/gtpajcyfnl.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.sxryk.cn/gtqrjwizxf.html

JS:   await Promise.all(tasks)
来源：http://hz.9152youxi.cn/gttobewgdl.html

TS:   await Promise.all(tasks)
来源：http://hz.chenlongwang.top/gtgskjqgjm.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.xuanzx.com/gtusoilkeb.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.smart0.xyz/gtwubqhnvb.html

Ruby: threads.map(&:join)
来源：http://hz.xuanzx.com/gtbdewdszc.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.dianchejie.cn/gtxksfuuvw.html

[O06] 使用进程池
来源：http://hz.hnxiangtu.top/gtmlqkjids.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.dianchejie.cn/gtcsujdlgt.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.daxiang520.top/gterqzzrib.html

JS:   // child_process / cluster 模块
来源：http://hz.xuanzx.com/gtyfkhgtqt.html

TS:   // child_process / cluster 模块
来源：http://hz.dashuyun.cn/gtjgxohpqm.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.jyoumei.cn/gtyhpfwzdf.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.jlsjyb.cn/gtisjnmcvz.html

Ruby: // fork 块
来源：http://hz.yonumen.top/gtbjmxzlrn.html

C#:   Parallel.For
来源：http://hz.gaohongyu789.top/gtivdrpjup.html

================================================================================
来源：http://hz.jqgufenzy.top/gtcrbhdpwu.html

P. 常用工具函数
来源：http://hz.mhx1999.top/gtxzvsxiho.html

================================================================================
来源：http://hz.ydjk.org.cn/gtsuqrznmm.html

[P01] 生成 UUID
来源：http://hz.yj20258888.top/gtttrnomtv.html

Py:   str(uuid.uuid4())
来源：http://hz.gaohongyu789.top/gtbpmkvyib.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.shanyushiyangkeji.top/gtszryvxbq.html

JS:   crypto.randomUUID()
来源：http://hz.xylfe.cn/gtgqtnhauh.html

TS:   crypto.randomUUID()
来源：http://hz.vqdsnc.cn/gtkbfqpcag.html

Java: UUID.randomUUID().toString()
来源：http://hz.bjfxy.top/gtxaxznllp.html

Go:   // 用 github.com/google/uuid
来源：http://hz.birdmap.top/gtpsrwqhcg.html

Ruby: SecureRandom.uuid
来源：http://hz.shanyushiyangtech.top/gtmvigwhri.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.ivvv.top/gtaqjbfpeq.html

[P02] MD5 / SHA256 摘要
来源：http://hz.shanyushiyangtech.top/gtbtzmtzfh.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.zhiwuduotai.top/gtpuydcajg.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.hysaishi.cn/gtrnoyfxpo.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.snrcjt.cn/gtfyaatrue.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.cucudq.cn/gtsfpnlerb.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.c1oappe.top/gtzrohwsze.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.tian-w.cn/gtpajcmrzl.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.redwolf501.top/gtnzseglyj.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.zhiwuduotai.top/gthttyvwgi.html

[P03] 生成短随机字符串
来源：http://hz.ywan-chungtsiang.top/gthiowlrgg.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.yvedp.cn/gtzkhlzddq.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.9152youxi.cn/gtftngurum.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.ywan-chungtsiang.top/gtcdkbgvsq.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.dashuyun.cn/gtpygepgzc.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.cqqwz.cn/gtwbgubeub.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.guannengcc.top/gtvwkxpuhg.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.jianghu66.top/gtvqekewiy.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.chenjidiqi.icu/gttybhlgfl.html

[P04] 求长度
来源：http://hz.xziqi.cn/gttihadegl.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.hywenlv.cn/gtnrpchmwb.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.sxryk.cn/gtwrzftlsk.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.xylfe.cn/gtenqeiwyh.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.zhijiandao.cn/gtjaetbksz.html

Java: list.size();  map.size();  s.length()
来源：http://hz.ywan-chungtsiang.top/gtennlqnnm.html

Go:   len(arr);  len(m)
来源：http://hz.cdnleiting.top/gttnnqaxbs.html

Ruby: x.length;  x.size
来源：http://hz.pycfn.com/gtuzhzgfdz.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.guannengcc.top/gtegobsrlk.html

[P05] 判断两个对象内容是否相等
来源：http://hz.yvedp.cn/gtyxhbwzyn.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.yj20258888.top/gtzsdbpaqs.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.ivvv.top/gtkteuwefa.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.cdnleiting.top/gtcyodhwwr.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.zhengqikj.top/gttdzbsiwe.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.yanxiufei.cn/gtnkdspvxc.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.hammf.cn/gtzzqwewfd.html

Ruby: a == b
来源：http://hz.shzxlz.cn/gtlpbghuvm.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.shangyingyoupin.top/gtmuqcvdkk.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.0kj1m.cn/gtivmingde.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.andypj.xyz/gtdhthlaig.html

PHP:  if (empty($x)) {}
来源：http://hz.xylfe.cn/gtmibrvpdc.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.yuanzhike.top/gtvfanyczy.html

TS:   if (x == null) {}
来源：http://hz.hfpthk.cn/gtuxqusywb.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.hammf.cn/gtpifgeqpm.html

Go:   if x == nil {}
来源：http://hz.svipenyu.cn/gtbcfywuld.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.jinyuanbaomall.cn/gtnpxjplhk.html

C#:   if (x is null) {}
来源：http://hz.svipenyu.cn/gtczssmtjg.html

[P07] 防抖与节流
来源：http://hz.316326.xyz/gttaotxtvq.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.yueranfly.top/gtwpfzwpia.html

PHP:  // 手写时间戳比较
来源：http://hz.nanxuanxn.top/gtgxeyfqfb.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.aibaodan.cn/gtiewhpoxr.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.wangshuangyany.cn/gtkwacffom.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.ppjwa.cn/gtdbfeoaii.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.yonumen.top/gtlnjurcwm.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.yangfankeji.com/gtrzgzmmrx.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.meibo888.top/gthgiukkzw.html

[P08] 处理浮点精度问题
来源：http://hz.xingfuxueyuan.xyz/gtximrclii.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.yj20258.top/gtdbrsupsy.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.xziqi.cn/gtazstqqrx.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.yuxming.cn/gtwbyvhdvc.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.zdqjudy.top/gtyrygmyhz.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.cqqwz.cn/gtvybunoak.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.jiagoushi.top/gtdnrfygxo.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.hysaishi.cn/gtsliqsjed.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.gzhubu.top/gtedqhmuwt.html

================================================================================
来源：http://hz.hammf.cn/gtolylxzry.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.xylfe.cn/gtcvanchoq.html

================================================================================
来源：http://hz.shuidangran.top/gtnhuxcmum.html

[Q01] 创建表
来源：http://hz.shzxlz.cn/gtjxyokwis.html

CREATE TABLE users (
来源：http://hz.redwolf501.top/gtjyztmsst.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.xinyue.icu/gttwqziyyd.html

name VARCHAR(50) NOT NULL,
来源：http://hz.chenjidiqi.icu/gteezunqtm.html

email VARCHAR(100) UNIQUE,
来源：http://hz.hfpthk.cn/gthprrrjcf.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.havefunace.top/gtmllxuurg.html

);
来源：http://hz.mhx1999.top/gtbqjiynoz.html

[Q02] 创建带外键的表
来源：http://hz.pengpengdd.cyou/gtpwdoggro.html

CREATE TABLE orders (
来源：http://hz.cdnleiting.top/gtssyomoti.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.ywan-chungtsiang.top/gtmpysiwgg.html

user_id INT NOT NULL,
来源：http://hz.jyoumei.cn/gtgkeolhjl.html

amount DECIMAL(10, 2),
来源：http://hz.yj20258.top/gtyqlvrwsi.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.aibaodan.cn/gtrfagkvow.html

);
来源：http://hz.hysaishi.cn/gtciscztmh.html

[Q03] 增加列
来源：http://hz.xylfe.cn/gtedytglcx.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.gogol.net.cn/gtefievgig.html

[Q04] 修改列类型
来源：http://hz.xylfe.cn/gtmsmzowrb.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.hysaishi.cn/gtlhtprtll.html

[Q05] 重命名列
来源：http://hz.tianlin.xyz/gtbjtrlfsy.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.zhengqikj.top/gtujxgtpbu.html

[Q06] 删除列
来源：http://hz.yanxiufei.cn/gtfaatwzox.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.jqgfzy.top/gtzxqfxflc.html

[Q07] 删除表
来源：http://hz.fzhhl.top/gteowtrlqs.html

DROP TABLE IF EXISTS orders;
来源：http://hz.9152youxi.cn/gtvhxbwpqz.html

[Q08] 创建普通索引
来源：http://hz.yonumen.top/gtaqfuammw.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.zhongyouzk.top/gtqragkheh.html

[Q09] 创建唯一索引
来源：http://hz.fengsongda.top/gtgjxjkkhw.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.hfpthk.cn/gtjvjwjprb.html

[Q10] 插入单行
来源：http://hz.xuanzx.com/gtxizkqoxw.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.shangyingyoupin.top/gtewkqufuj.html

[Q11] 一次插入多行
来源：http://hz.ywan-chungtsiang.top/gtkpkddril.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.yvedp.cn/gtxojhakpv.html

[Q12] 插入后取自增 ID
来源：http://hz.c1oappe.top/gtvpjswkzy.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.jinyuanbaomall.cn/gtuwlasyjc.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.cashguo.top/gtslvjoyeo.html

[Q13] 忽略重复插入
来源：http://hz.zhijiandao.cn/gtpixmhwtr.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.gotoacloud.top/gtcbzmwtfb.html

[Q14] 存在则更新（upsert）
来源：http://hz.jiagoushi.top/gtnrfdoazj.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.gaohongyu789.top/gtqsykkewy.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.sysykeji.top/gtftjtknpu.html

[Q15] 查询全部
来源：http://hz.zhijiandao.cn/gtwfkuvzlk.html

SELECT * FROM users;
来源：http://hz.guowangkeji.top/gtfksbdfby.html

[Q16] 查询指定列
来源：http://hz.xziqi.cn/gtcntfaqyc.html

SELECT id, name FROM users;
来源：http://hz.bjfxy.top/gtsvuqipxx.html

[Q17] 条件查询
来源：http://hz.nwbrower.top/gtqxsjrqmc.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.tian-w.cn/gtfkngyggk.html

[Q18] 模糊匹配
来源：http://hz.havefunace.top/gtbaunfigz.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.xinyue.icu/gtmcoanbfx.html

[Q19] 范围查询
来源：http://hz.nanxuanxn.top/gtnemvcnnl.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.cqqwz.cn/gtekniwlrh.html

[Q20] IN 列表
来源：http://hz.yuanzhike.top/gtbofsevoa.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.xingfuxueyuan.xyz/gtutyuqddx.html

[Q21] 空值判断
来源：http://hz.nanxinkj.top/gtxwrldaus.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.wangshuangyany.cn/gttstbatot.html

[Q22] 排序
来源：http://hz.sxryk.cn/gtimuzrtte.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.tianlin.xyz/gtllyfusqt.html

[Q23] 分页
来源：http://hz.daria6918.cn/gtiglpzukf.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.chenlongwang.top/gtluwfltkj.html

[Q24] 去重
来源：http://hz.birdmap.top/gttbkjkacy.html

SELECT DISTINCT city FROM users;
来源：http://hz.fengsongda.top/gtvubvvizd.html

[Q25] 只取前 N 条
来源：http://hz.jiagoushi.top/gtriaoeguq.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.shanyushiyangkeji.top/gtcrewxjby.html

[Q26] 计数
来源：http://hz.birdmap.top/gtephfaqvr.html

SELECT COUNT(*) FROM users;
来源：http://hz.ydzc1.top/gteankhhnz.html

[Q27] 条件计数
来源：http://hz.daria6918.cn/gtmekgjzej.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.xziqi.cn/gtsqttkswe.html

[Q28] 求和与平均
来源：http://hz.andypj.xyz/gtfomfvkfu.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.ydzc1.top/gteadlshse.html

[Q29] 最大最小值
来源：http://hz.smart0.xyz/gtvgtrllmr.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.vqdsnc.cn/gtdcjwsear.html

[Q30] 分组统计
来源：http://hz.jiagoushi.top/gtazstrada.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.nanxuanxn.top/gtuxutnqja.html

[Q31] 分组后过滤
来源：http://hz.ehwqpu.com/gtdexccdlg.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.sysykeji.top/gtlbyhcdyc.html

[Q32] 分组拼接字符串
来源：http://hz.c1oappe.top/gtjosevnnb.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.yj20258888.top/gtiwfeifix.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.chenzaomai.com/gtmsfgeemo.html

[Q33] 多列分组
来源：http://hz.xuanzx.com/gtxiapnjyq.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.snrcjt.cn/gtoflduobp.html

[Q34] 每组取第一条
来源：http://hz.cashguo.top/gtxrkwqxra.html

SELECT * FROM (
来源：http://hz.shangyingyoupin.top/gtmoebchbr.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.chenlongwang.top/gtpxfduafm.html

) t WHERE rn = 1;
来源：http://hz.redwolf501.top/gtutoqeedu.html

[Q35] 内连接
来源：http://hz.nanxinkj.top/gtwysbisii.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.cucudq.cn/gttxztenrd.html

[Q36] 左连接
来源：http://hz.cdnleiting.top/gtatfoqpgd.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.yuanzhike.top/gtaiextzxb.html

[Q37] 右连接
来源：http://hz.jinyuanbaomall.cn/gtfkwkdnxk.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.hywenlv.cn/gtppvcgxai.html


<!-- 参考信息 -->