代发 wailian999

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.aizwys.cn/gtlvzcsfwt.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.jqgufenzy.top/gtmfamrnyw.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.jinyuanbaomall.cn/gtybolwfut.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.gaohongyu789.top/gtplpcgbfn.html

[N05] 最大公约数
来源：http://hz.hywenlv.cn/gtavkzhmzw.html

Py:   math.gcd(a, b)
来源：http://hz.xingfuxueyuan.xyz/gtkrutptxf.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.snrcjt.cn/gttzfavoiu.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.zhijiandao.cn/gtkaezkirl.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.dashuyun.cn/gttixshjcu.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.tianlin.xyz/gtjkqbdbek.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.jiagoushi.top/gthpjufqda.html

Ruby: a.gcd(b)
来源：http://hz.xziqi.cn/gtnqnmdnyl.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.316326.xyz/gtkqbmauup.html

[N06] 判断回文字符串
来源：http://hz.yj20258888.top/gtfifqzfkd.html

Py:   s == s[::-1]
来源：http://hz.sxryk.cn/gtbbwvquvs.html

PHP:  $s === strrev($s);
来源：http://hz.ydjk.org.cn/gtprhmchkl.html

JS:   s === [...s].reverse().join("")
来源：http://hz.ehwqpu.com/gtdnkyyzro.html

TS:   s === [...s].reverse().join("")
来源：http://hz.tianlin.xyz/gtfkvrawne.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.cashguo.top/gtpowijpnx.html

Go:   // 双指针从两端比较
来源：http://hz.jyoumei.cn/gtxtufjgau.html

Ruby: s == s.reverse
来源：http://hz.yj20258888.top/gtbzfsfwxx.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.yuanzhike.top/gtalkleqst.html

[N07] 两数之和（返回下标）
来源：http://hz.fzhhl.top/gtkhouojwr.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.jlsjyb.cn/gtrqqwxuoh.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.hammf.cn/gtkymkbyyc.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.sufxvd.cn/gtuajngsnl.html

TS:   // 手写 Map<string, number>
来源：http://hz.yj20258888.top/gtfyjpypiw.html

Java: // 手写 HashMap
来源：http://hz.c1oappe.top/gtbistknmw.html

Go:   // 手写 map[int]int
来源：http://hz.svipenyu.cn/gtngkniwhk.html

Ruby: // 手写 Hash
来源：http://hz.chenjidiqi.icu/gtvxmcdwre.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.xylfe.cn/gtqxqzzgun.html

[N08] 生成全排列
来源：http://hz.meibo888.top/gtcbpagzlj.html

Py:   itertools.permutations(arr)
来源：http://hz.redwolf501.top/gttbjvbiey.html

PHP:  // 手写递归交换
来源：http://hz.ydjk.org.cn/gtcrwldgci.html

JS:   // 手写回溯递归
来源：http://hz.zhiwuduotai.top/gtclrvdhtg.html

TS:   // 手写回溯递归
来源：http://hz.xuanzx.com/gtfurgibti.html

Java: // 手写回溯递归
来源：http://hz.chenzaomai.com/gtijlaqrrh.html

Go:   // 手写回溯递归
来源：http://hz.cheryme.top/gtsmuxefpg.html

Ruby: arr.permutation.to_a
来源：http://hz.hysaishi.cn/gttszzgovj.html

C#:   // 手写回溯递归
来源：http://hz.hfpthk.cn/gtafjaugkp.html

[N09] 栈与队列
来源：http://hz.yanxiufei.cn/gtbftleezk.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.nwbrower.top/gtpfvspklv.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.xuanzx.com/gtwzsaagtk.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.sweek.top/gtiandqrxr.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.yj20258888.top/gtgokcxwnz.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.sufxvd.cn/gtbtuyoxlo.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.sweek.top/gtkgkfjzbb.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.cdnleiting.top/gtmehnrmpo.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.zhengqikj.top/gtyswwclos.html

[N10] 链表节点定义
来源：http://hz.zhongyouzk.top/gtnkgrqoam.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.chenjidiqi.icu/gtxwcbzybd.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.hnqzz.top/gtmccncjpa.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.yanxiufei.cn/gtokilkxho.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.sufxvd.cn/gtkyrnquvy.html

Java: class Node { int v; Node next; }
来源：http://hz.sweek.top/gtukmpdewq.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.dianchejie.cn/gtfpqlklro.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.tanke756.top/gtpavpjrmu.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.fengsongda.top/gtnudxowna.html

[N11] 二叉树中序遍历
来源：http://hz.yj20258888.top/gtgmizfwth.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.pengpengdd.cyou/gtxlymodil.html

PHP:  // 手写递归函数
来源：http://hz.guowangkeji.top/gtflwqufrx.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.yanxiufei.cn/gtosouqtws.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.zycfv.cn/gttovfjqax.html

Java: // 手写递归
来源：http://hz.dianchejie.cn/gtmkablxju.html

Go:   // 手写递归
来源：http://hz.ehwqpu.com/gtvqzwpmuj.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.zhaomingkeji.xyz/gtbhtsxdgv.html

C#:   // 手写递归
来源：http://hz.cheryme.top/gtoosmacey.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.dashuyun.cn/gtipviajvp.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.yonumen.top/gtrfxmnthu.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.xuanzx.com/gtjkkmfcwv.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.wangdashe.top/gtkaygfxzb.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.cashguo.top/gtrgecvcqs.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.cashguo.top/gtfbrwqhsl.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.guannengcc.top/gtedjftttz.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.aibaodan.cn/gtfpjlhxak.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.yuxming.cn/gtgbzczpvy.html

================================================================================
来源：http://hz.hnqzz.top/gtualkqdfs.html

O. 并发与异步
来源：http://hz.yj202588.top/gtehapmrgp.html

================================================================================
来源：http://hz.zycfv.cn/gtlutpnqxv.html

[O01] 启动一个线程
来源：http://hz.shangyingyoupin.top/gtpnfwsukz.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.9152youxi.cn/gtmllhqzxm.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.smart0.xyz/gtexwfnsjq.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.cheryme.top/gtpfwpuybf.html

TS:   // 同 JS
来源：http://hz.bjfxy.top/gtnvoaakgb.html

Java: new Thread(() -> f()).start()
来源：http://hz.yj20258888.top/gtljwrrvff.html

Go:   go f()
来源：http://hz.hfpthk.cn/gtpwhgyirq.html

Ruby: Thread.new { f }
来源：http://hz.yuxming.cn/gtoksxagrd.html

C#:   Task.Run(() => F());
来源：http://hz.xuetiantiany.cn/gtjdbbmket.html

[O02] 使用线程池
来源：http://hz.hnxiangtu.top/gthyjimosq.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.9152youxi.cn/gtewujhesd.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.birdmap.top/gtkwgbtpeb.html

JS:   // worker_threads 线程池
来源：http://hz.cqqwz.cn/gtutknrdjc.html

TS:   // worker_threads 线程池
来源：http://hz.kuanghao11.cn/gtmqvucjlt.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.zdqjudy.top/gtlhospztk.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.yvedp.cn/gtsqzvgqnr.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.sysykeji.top/gtckzjwgbs.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.andypj.xyz/gtsokkqycc.html

[O03] 加锁保护共享数据
来源：http://hz.yangfankeji.com/gthbywrlwd.html

Py:   with lock: shared += 1
来源：http://hz.xingfuxueyuan.xyz/gtrkoultgi.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.zhijiandao.cn/gtlaynofur.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.jianghu66.top/gtskzpqucl.html

TS:   // 同 JS
来源：http://hz.hfpthk.cn/gtqaqzqadl.html

Java: synchronized (this) { shared++; }
来源：http://hz.xinyue.icu/gthtgvshfs.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.havefunace.top/gtchuqnevg.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.snrcjt.cn/gtoqyrmgng.html

C#:   lock (gate) { shared++; }
来源：http://hz.jianghu66.top/gtanwwpkgf.html

[O04] 定义异步函数并等待
来源：http://hz.jiagoushi.top/gtvukinwsu.html

Py:   async def f():⏎    await g()
来源：http://hz.hongshengwenyu.top/gtxcohndok.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.zhaomingkeji.xyz/gtwochthtt.html

JS:   async function f() { await g(); }
来源：http://hz.shanyushiyangtech.top/gtzchucttw.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.pycfn.com/gtskmylpfh.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.jinqigufen.top/gtkecoixzf.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.aizwys.cn/gtzmyvkoof.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.jinghuilouyu.cn/gtrfontqqk.html

C#:   async Task F() { await G(); }
来源：http://hz.cucudq.cn/gtapesgjhq.html

[O05] 并发执行并等待全部完成
来源：http://hz.zhaomingkeji.xyz/gtrsxchwtv.html

Py:   asyncio.gather(*tasks)
来源：http://hz.bjfxy.top/gttmcdctbe.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.gaohongyu789.top/gtwklihuzi.html

JS:   await Promise.all(tasks)
来源：http://hz.dianchejie.cn/gtbvrlykgw.html

TS:   await Promise.all(tasks)
来源：http://hz.xinyue.icu/gtzfprptcb.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.tian-w.cn/gtldmtiarg.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.quarkkingdee.top/gtiqyctzlo.html

Ruby: threads.map(&:join)
来源：http://hz.ybcxt.top/gtugskzhgu.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.jyoumei.cn/gtcsnfpojz.html

[O06] 使用进程池
来源：http://hz.jinyuanbaomall.cn/gtseuoqepu.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.ppjwa.cn/gtfqpnunmv.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.hnqzz.top/gtvubgngxd.html

JS:   // child_process / cluster 模块
来源：http://hz.smart0.xyz/gtiliankzh.html

TS:   // child_process / cluster 模块
来源：http://hz.xuetiantiany.cn/gtuurfodra.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.zhixingplan.top/gtxmzkpqmo.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.hysaishi.cn/gtkonyktss.html

Ruby: // fork 块
来源：http://hz.jianghu66.top/gtxiettuaa.html

C#:   Parallel.For
来源：http://hz.yj202588.top/gtenhnccpj.html

================================================================================
来源：http://hz.zhongyouzk.top/gtbhdhljcs.html

P. 常用工具函数
来源：http://hz.daxiang520.top/gtxhvdsigv.html

================================================================================
来源：http://hz.jyoumei.cn/gtgaatdbtg.html

[P01] 生成 UUID
来源：http://hz.gogol.net.cn/gtvxewgpyc.html

Py:   str(uuid.uuid4())
来源：http://hz.yonumen.top/gtekigkceu.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.jinqigufen.top/gtgjknaohl.html

JS:   crypto.randomUUID()
来源：http://hz.guannengcc.top/gtwvzxxpht.html

TS:   crypto.randomUUID()
来源：http://hz.shanyushiyangkeji.top/gtbvqbgjfs.html

Java: UUID.randomUUID().toString()
来源：http://hz.snrcjt.cn/gtoqiuotny.html

Go:   // 用 github.com/google/uuid
来源：http://hz.kuanghao11.cn/gtsdgvqoll.html

Ruby: SecureRandom.uuid
来源：http://hz.shangyingyoupin.top/gtmjnlhvkr.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.52xcode.cn/gtsijurhmh.html

[P02] MD5 / SHA256 摘要
来源：http://hz.yvedp.cn/gtcdiqdudw.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.nanxuanxn.top/gtwzooidyi.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.zhongyouzk.top/gtuqtkkthv.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.bjfxy.top/gtfzkdqjgx.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.fzhhl.top/gtwfxlztyj.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.xuanzx.com/gtxmdohcwp.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.ehwqpu.com/gtqnpyfrwm.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.yj202588.top/gttirudqmw.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.cqqwz.cn/gtrdavbrln.html

[P03] 生成短随机字符串
来源：http://hz.fzhhl.top/gtgubudfdz.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.smart0.xyz/gtmzmpsgjq.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.9152youxi.cn/gtqecimqse.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.hammf.cn/gtipjcgzak.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.bjfxy.top/gtbumplrdw.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.yuxming.cn/gtsltuulqz.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.shanyushiyangtech.top/gtpchhlslk.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.sweek.top/gtdcdwdyrg.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.nwbrower.top/gtlupykbmt.html

[P04] 求长度
来源：http://hz.fzhhl.top/gtdjxolbjb.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.jianghu66.top/gtsepiruze.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.guowangkeji.top/gtzyumwshg.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.tanke756.top/gtsuevnlcv.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.cucudq.cn/gthxoygpkt.html

Java: list.size();  map.size();  s.length()
来源：http://hz.svipenyu.cn/gtyajirwsd.html

Go:   len(arr);  len(m)
来源：http://hz.svipenyu.cn/gteygmedau.html

Ruby: x.length;  x.size
来源：http://hz.zhiwuduotai.top/gtbwjbmdbs.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.hfpthk.cn/gtzagfxotx.html

[P05] 判断两个对象内容是否相等
来源：http://hz.yonumen.top/gtjddybxxm.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.dianchejie.cn/gtgnbthjhh.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.nwbrower.top/gtszvcghxh.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.zdqjudy.top/gtpujdcrxi.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.daxiang520.top/gtseyxrwlu.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.xinyue.icu/gtxcnbafjz.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.cheryme.top/gtlyynxowy.html

Ruby: a == b
来源：http://hz.yj20258.top/gttpddnhuv.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.jinyuanbaomall.cn/gtwxbbszng.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.ivvv.top/gtoyfjcgim.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.shangyingyoupin.top/gtofhpbbna.html

PHP:  if (empty($x)) {}
来源：http://hz.hammf.cn/gtefhptbuo.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.sweek.top/gtfbcsoyyo.html

TS:   if (x == null) {}
来源：http://hz.sysykeji.top/gtjczngyhp.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.tian-w.cn/gtakjxgiyl.html

Go:   if x == nil {}
来源：http://hz.cqqwz.cn/gtnjerprss.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.jyoumei.cn/gttaocumww.html

C#:   if (x is null) {}
来源：http://hz.guowangkeji.top/gtpfzxpjpx.html

[P07] 防抖与节流
来源：http://hz.yj202588.top/gtelbbniio.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.jinyuanbaomall.cn/gthyepfcts.html

PHP:  // 手写时间戳比较
来源：http://hz.hywenlv.cn/gtgauisrxa.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.jinghuilouyu.cn/gttmsdxpnh.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.zhaomingkeji.xyz/gtlzxjeqzn.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.zhoulong.xyz/gtbnfdxqhf.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.zhiwuduotai.top/gtfprgfdlt.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.ydjk.org.cn/gtcdbjyfgd.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.chenlongwang.top/gtmidkrlfw.html

[P08] 处理浮点精度问题
来源：http://hz.yuanzhike.top/gtdeqahape.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.yj20258888.top/gtnkfnwneh.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.nanxuanxn.top/gtbfpsyewj.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.cqqwz.cn/gtaozzevzf.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.chenlongwang.top/gtwbvdocly.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.wangshuangyany.cn/gtezrcakbq.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.cqqwz.cn/gtrtkcrqhu.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.hongshengwenyu.top/gtjybofald.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.xuanzx.com/gtkgfabdby.html

================================================================================
来源：http://hz.yj202588.top/gtghelfqkx.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.zhixingplan.top/gtxitdoxpf.html

================================================================================
来源：http://hz.zhiwuduotai.top/gtbsdcgovr.html

[Q01] 创建表
来源：http://hz.shzxlz.cn/gtgzyzidxm.html

CREATE TABLE users (
来源：http://hz.ybcxt.top/gtgvlcbdsb.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.daria6918.cn/gtjnssvfqk.html

name VARCHAR(50) NOT NULL,
来源：http://hz.jyoumei.cn/gtzvjdpfma.html

email VARCHAR(100) UNIQUE,
来源：http://hz.52xcode.cn/gtitvoatkc.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.shanyushiyangtech.top/gtsyceuvos.html

);
来源：http://hz.iojbl.cn/gtavavmuof.html

[Q02] 创建带外键的表
来源：http://hz.yanxiufei.cn/gtylirjyqr.html

CREATE TABLE orders (
来源：http://hz.gotoacloud.top/gtohsdvppq.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.birdmap.top/gtegqmybub.html

user_id INT NOT NULL,
来源：http://hz.cheryme.top/gtopnlnwle.html

amount DECIMAL(10, 2),
来源：http://hz.nanxinkj.top/gtmbljhhvc.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.xziqi.cn/gtxdidhmvn.html

);
来源：http://hz.cheryme.top/gtxlvdllyv.html

[Q03] 增加列
来源：http://hz.nwbrower.top/gthwgmzljx.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.zhoulong.xyz/gtibwetusq.html

[Q04] 修改列类型
来源：http://hz.yj20258.top/gttvjrjdrm.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.daxiang520.top/gtgbjbuxnq.html

[Q05] 重命名列
来源：http://hz.dianchejie.cn/gtlammnjtv.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.ehwqpu.com/gtqnkdebio.html

[Q06] 删除列
来源：http://hz.jinghuilouyu.cn/gthditfquj.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.tianlin.xyz/gtegubkevp.html

[Q07] 删除表
来源：http://hz.jinghuilouyu.cn/gtrxklsior.html

DROP TABLE IF EXISTS orders;
来源：http://hz.ivvv.top/gtzfvuheyf.html

[Q08] 创建普通索引
来源：http://hz.nwbrower.top/gtcytluksl.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.zdqjudy.top/gtiuorywzl.html

[Q09] 创建唯一索引
来源：http://hz.jlsjyb.cn/gtzrasvbti.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.chenjidiqi.icu/gtlppskgvp.html

[Q10] 插入单行
来源：http://hz.jianghu66.top/gtdlzzjuzb.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.zhoulong.xyz/gtyvufnlcw.html

[Q11] 一次插入多行
来源：http://hz.yueranfly.top/gtacvezbfa.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.iojbl.cn/gteicnzlyh.html

[Q12] 插入后取自增 ID
来源：http://hz.redwolf501.top/gtgbaqyrqn.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.shanyushiyangkeji.top/gtskqrciiy.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.hongshengwenyu.top/gtxxajcgkj.html

[Q13] 忽略重复插入
来源：http://hz.gaohongyu789.top/gttpjocbho.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.c1oappe.top/gtjzjmethg.html

[Q14] 存在则更新（upsert）
来源：http://hz.cheryme.top/gtxvinjvbs.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.316326.xyz/gteoyvuttm.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.nanxuanxn.top/gtuqpibmok.html

[Q15] 查询全部
来源：http://hz.cdnleiting.top/gtpkwsqmxa.html

SELECT * FROM users;
来源：http://hz.yonumen.top/gtkbmvxpbv.html

[Q16] 查询指定列
来源：http://hz.jiagoushi.top/gtlmanenzw.html

SELECT id, name FROM users;
来源：http://hz.jqgufenzy.top/gtayhfbjwp.html

[Q17] 条件查询
来源：http://hz.pengpengdd.cyou/gtpurgjzsa.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.hysaishi.cn/gtokcmphki.html

[Q18] 模糊匹配
来源：http://hz.yangfankeji.com/gtfilxkncx.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.dianchejie.cn/gtqlibersk.html

[Q19] 范围查询
来源：http://hz.daxiang520.top/gtfiiertae.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.ydjk.org.cn/gthdimjovx.html

[Q20] IN 列表
来源：http://hz.pengpengdd.cyou/gtxetyfwlz.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.redwolf501.top/gtmrpurbrv.html

[Q21] 空值判断
来源：http://hz.yangfankeji.com/gthzzxycza.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.cucudq.cn/gtsclrokpt.html

[Q22] 排序
来源：http://hz.jyoumei.cn/gthnhnjjjn.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.shuidangran.top/gtgcnhggir.html

[Q23] 分页
来源：http://hz.fzhhl.top/gtuhvafrki.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.0kj1m.cn/gtxzguulpi.html

[Q24] 去重
来源：http://hz.snrcjt.cn/gtvsdryars.html

SELECT DISTINCT city FROM users;
来源：http://hz.nwbrower.top/gtqscvzzjz.html

[Q25] 只取前 N 条
来源：http://hz.fzhhl.top/gtmkhhcpkj.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.nanxuanxn.top/gtuvlqbqek.html

[Q26] 计数
来源：http://hz.jinqigufen.top/gthkgzuggw.html

SELECT COUNT(*) FROM users;
来源：http://hz.nanxuanxn.top/gtaprgmaix.html

[Q27] 条件计数
来源：http://hz.zhengqikj.top/gtbslwehwe.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.shuidangran.top/gtqqxpksmr.html

[Q28] 求和与平均
来源：http://hz.nanxuanxn.top/gtpmqgymwm.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.bjfxy.top/gtsfgzzegu.html

[Q29] 最大最小值
来源：http://hz.cucudq.cn/gtqqcoehic.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.nanxinkj.top/gtsziodmtk.html

[Q30] 分组统计
来源：http://hz.jqgfzy.top/gtoxhpmprn.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.tanke756.top/gthlzauxqz.html

[Q31] 分组后过滤
来源：http://hz.smart0.xyz/gtpedgwpgn.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.chenjidiqi.icu/gtptmkiwaa.html

[Q32] 分组拼接字符串
来源：http://hz.hammf.cn/gtuekflyya.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.aibaodan.cn/gtxtkknkat.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.yuxming.cn/gtkcdeertv.html

[Q33] 多列分组
来源：http://hz.redwolf501.top/gtzmuxpwrv.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.snrcjt.cn/gtyzglvfsv.html

[Q34] 每组取第一条
来源：http://hz.xingfuxueyuan.xyz/gtaodxzkxe.html

SELECT * FROM (
来源：http://hz.smart0.xyz/gtxkpmbnqw.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.yonumen.top/gtnvvodwdb.html

) t WHERE rn = 1;
来源：http://hz.dashuyun.cn/gtyfxcukuy.html

[Q35] 内连接
来源：http://hz.chenjidiqi.icu/gtkmiwwtgh.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.zhaomingkeji.xyz/gtuiawkxvk.html

[Q36] 左连接
来源：http://hz.hnxiangtu.top/gtkkpinqft.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.xinyue.icu/gtwsncpkrv.html

[Q37] 右连接
来源：http://hz.gaohongyu789.top/gtefrfruix.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.ppjwa.cn/gtzosluwoj.html


<!-- 参考信息 -->