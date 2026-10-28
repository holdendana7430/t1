代发 wailian999

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.pycfn.com/gtpodmxgwl.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.aibaodan.cn/gtdsrcrnda.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.shanyushiyangtech.top/gtedrcszgh.html

Ruby: a.gcd(b)
来源：http://hz.sweek.top/gtbwiycfrh.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.hywenlv.cn/gtflkdfies.html

[N06] 判断回文字符串
来源：http://hz.jqgufenzy.top/gtdurxsoqy.html

Py:   s == s[::-1]
来源：http://hz.redwolf501.top/gtmtknlqqm.html

PHP:  $s === strrev($s);
来源：http://hz.cheryme.top/gtjpgyylno.html

JS:   s === [...s].reverse().join("")
来源：http://hz.hnxiangtu.top/gtrpojwfcv.html

TS:   s === [...s].reverse().join("")
来源：http://hz.yangfankeji.com/gtsqotzmxz.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.shangyingyoupin.top/gtctqpzusy.html

Go:   // 双指针从两端比较
来源：http://hz.redwolf501.top/gtyxbquxjz.html

Ruby: s == s.reverse
来源：http://hz.shanyushiyangtech.top/gtaarpqxhx.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.hnxiangtu.top/gtihsamhiv.html

[N07] 两数之和（返回下标）
来源：http://hz.fzhhl.top/gttpmnamqe.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.aibaodan.cn/gtaeakamlm.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.jiagoushi.top/gtckmmwwcm.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.jinghuilouyu.cn/gtqxkbmfbh.html

TS:   // 手写 Map<string, number>
来源：http://hz.nwbrower.top/gtnkvpbabn.html

Java: // 手写 HashMap
来源：http://hz.hammf.cn/gtummnmpsg.html

Go:   // 手写 map[int]int
来源：http://hz.jinqigfzy.top/gtloiwphpq.html

Ruby: // 手写 Hash
来源：http://hz.shanyushiyangtech.top/gtrmuttpuo.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.nanxuanxn.top/gtaelcjmzh.html

[N08] 生成全排列
来源：http://hz.birdmap.top/gtjvryeoof.html

Py:   itertools.permutations(arr)
来源：http://hz.ppjwa.cn/gtxpvfrozi.html

PHP:  // 手写递归交换
来源：http://hz.hnqzz.top/gtdkzdhnif.html

JS:   // 手写回溯递归
来源：http://hz.zhixingplan.top/gtqmjwjgzk.html

TS:   // 手写回溯递归
来源：http://hz.c1oappe.top/gtdfrpqybh.html

Java: // 手写回溯递归
来源：http://hz.guannengcc.top/gtvctkjuod.html

Go:   // 手写回溯递归
来源：http://hz.havefunace.top/gtguwhgnvb.html

Ruby: arr.permutation.to_a
来源：http://hz.zhijiandao.cn/gtgazoiixt.html

C#:   // 手写回溯递归
来源：http://hz.xylfe.cn/gtislkbyaf.html

[N09] 栈与队列
来源：http://hz.zhaomingkeji.xyz/gtkinctnpg.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.jyoumei.cn/gtdagdgijw.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.sxryk.cn/gtmtcpcotl.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.jinqigfzy.top/gtfnxxbnuk.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.smart0.xyz/gttjbtyrjt.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.c1oappe.top/gthsnrjmsz.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.havefunace.top/gttiwpvdjx.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.zhaomingkeji.xyz/gtjjnafiys.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.shanyushiyangkeji.top/gtrlnvmyhk.html

[N10] 链表节点定义
来源：http://hz.xziqi.cn/gtlctcokak.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.yongpay.top/gtiarucikk.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.316326.xyz/gtxpikmfws.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.feifeiyinyue.top/gtjxlmhxsj.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.tianlin.xyz/gtupwjrmuy.html

Java: class Node { int v; Node next; }
来源：http://hz.hnqzz.top/gtrqkuusso.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.zhixingplan.top/gtmkxhpyfd.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.shuidangran.top/gtppuwdelk.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.cheryme.top/gtrukcyuhc.html

[N11] 二叉树中序遍历
来源：http://hz.jyoumei.cn/gtygzrlptl.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.ybcxt.top/gtchhqcxja.html

PHP:  // 手写递归函数
来源：http://hz.cheryme.top/gtkvrfgzdk.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.ydzc1.top/gtdvvcwcef.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.yj20258.top/gthagmrvje.html

Java: // 手写递归
来源：http://hz.sysykeji.top/gttectjzka.html

Go:   // 手写递归
来源：http://hz.feifeiyinyue.top/gtpirniyzz.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.zycfv.cn/gtxoqmggiz.html

C#:   // 手写递归
来源：http://hz.yangfankeji.com/gtaniegxdy.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.gogol.net.cn/gtenzrpkva.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.jianghu66.top/gtltxrgtee.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.zhengqikj.top/gtatexssgx.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.cucudq.cn/gtopbvpbvi.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.snrcjt.cn/gtrpycxflw.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.jinghuilouyu.cn/gtrvpwirje.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.hysaishi.cn/gtmkanidfh.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.nwbrower.top/gtqzajlmpf.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.jinqigfzy.top/gttfuwitut.html

================================================================================
来源：http://hz.ehwqpu.com/gtljqtnpns.html

O. 并发与异步
来源：http://hz.quarkkingdee.top/gtllmmrvyi.html

================================================================================
来源：http://hz.yj20258888.top/gtagfachnh.html

[O01] 启动一个线程
来源：http://hz.yangfankeji.com/gtqeavyapo.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.zhoulong.xyz/gtdnwpqnkz.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.c1oappe.top/gtxzhqksyk.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.zhixingplan.top/gtxggptzdo.html

TS:   // 同 JS
来源：http://hz.cdnleiting.top/gtnvjyhicg.html

Java: new Thread(() -> f()).start()
来源：http://hz.chenjidiqi.icu/gtinxvscmb.html

Go:   go f()
来源：http://hz.yongpay.top/gtegiqnvnp.html

Ruby: Thread.new { f }
来源：http://hz.yj20258888.top/gtebzoydmv.html

C#:   Task.Run(() => F());
来源：http://hz.daxiang520.top/gtmutjgnbr.html

[O02] 使用线程池
来源：http://hz.chenjidiqi.icu/gtejsqgqhz.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.cucudq.cn/gtqiuktnjb.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.gogol.net.cn/gtljbkjytn.html

JS:   // worker_threads 线程池
来源：http://hz.kuanghao11.cn/gtsflvkhoo.html

TS:   // worker_threads 线程池
来源：http://hz.ppjwa.cn/gtfqwmjmyc.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.cashguo.top/gtwrfarflz.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.shzxlz.cn/gtqqeqdmgv.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.316326.xyz/gtdfgwtbtj.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.zhixingplan.top/gtmxxbqulh.html

[O03] 加锁保护共享数据
来源：http://hz.tanke756.top/gtrvajysmq.html

Py:   with lock: shared += 1
来源：http://hz.yonumen.top/gtxgekfjnc.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.hysaishi.cn/gtrvrrifzj.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.zdqjudy.top/gtqkgrebgi.html

TS:   // 同 JS
来源：http://hz.guowangkeji.top/gtganinpkq.html

Java: synchronized (this) { shared++; }
来源：http://hz.jinqigufen.top/gtmjluaqfp.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.xylfe.cn/gtgoyvvgmv.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.tian-w.cn/gtdweymuvp.html

C#:   lock (gate) { shared++; }
来源：http://hz.pengpengdd.cyou/gtnwzsekpn.html

[O04] 定义异步函数并等待
来源：http://hz.vqdsnc.cn/gteonhsvhz.html

Py:   async def f():⏎    await g()
来源：http://hz.tanke756.top/gtaazftblt.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.zhiwuduotai.top/gttqbtisjq.html

JS:   async function f() { await g(); }
来源：http://hz.zhengqikj.top/gtvyckviov.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.fengsongda.top/gttbcegxxw.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.redwolf501.top/gtuwsdaqmv.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.0kj1m.cn/gttixswmhy.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.redwolf501.top/gtwpikdocm.html

C#:   async Task F() { await G(); }
来源：http://hz.redwolf501.top/gtqerhtesw.html

[O05] 并发执行并等待全部完成
来源：http://hz.gaohongyu789.top/gtntnazeit.html

Py:   asyncio.gather(*tasks)
来源：http://hz.jyoumei.cn/gtaolnwtxn.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.chenzaomai.com/gtkabirsls.html

JS:   await Promise.all(tasks)
来源：http://hz.gogol.net.cn/gtwbwcdcie.html

TS:   await Promise.all(tasks)
来源：http://hz.shanyushiyangtech.top/gtcdgdtkay.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.fzhhl.top/gtlxegeimp.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.sweek.top/gtgkcbcgtk.html

Ruby: threads.map(&:join)
来源：http://hz.hysaishi.cn/gtbqrgrwxw.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.jinqigufen.top/gtmzaortsj.html

[O06] 使用进程池
来源：http://hz.chenjidiqi.icu/gtkvngziqw.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.jinqigufen.top/gtyfrlwgxg.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.jqgufenzy.top/gtubjjsjuk.html

JS:   // child_process / cluster 模块
来源：http://hz.gogol.net.cn/gtgrttqcew.html

TS:   // child_process / cluster 模块
来源：http://hz.gotoacloud.top/gtpjcwchnb.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.jqgufenzy.top/gtnqqycuux.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.nanxuanxn.top/gtvczsdgvn.html

Ruby: // fork 块
来源：http://hz.yanxiufei.cn/gtqldqqgmv.html

C#:   Parallel.For
来源：http://hz.aibaodan.cn/gtryllmawi.html

================================================================================
来源：http://hz.dianchejie.cn/gtkfkmodmd.html

P. 常用工具函数
来源：http://hz.zhijiandao.cn/gtvnqhascn.html

================================================================================
来源：http://hz.yj20258888.top/gtfiorpqps.html

[P01] 生成 UUID
来源：http://hz.jinghuilouyu.cn/gtytuqccgp.html

Py:   str(uuid.uuid4())
来源：http://hz.meibo888.top/gtllelcjuy.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.sxryk.cn/gttaezmlnh.html

JS:   crypto.randomUUID()
来源：http://hz.yangfankeji.com/gtglbijkyn.html

TS:   crypto.randomUUID()
来源：http://hz.ehwqpu.com/gtwtupnbvu.html

Java: UUID.randomUUID().toString()
来源：http://hz.birdmap.top/gthdvhnwdx.html

Go:   // 用 github.com/google/uuid
来源：http://hz.cqqwz.cn/gtbpbtuatu.html

Ruby: SecureRandom.uuid
来源：http://hz.zdqjudy.top/gtzrnkqvrj.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.sxryk.cn/gtlmgmjfyf.html

[P02] MD5 / SHA256 摘要
来源：http://hz.aibaodan.cn/gtyxewmjwj.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.zhijiandao.cn/gtynkwdyat.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.zhijiandao.cn/gtmwsxxwmi.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.yueranfly.top/gtgaiyydoy.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.jinqigufen.top/gtigjtrqut.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.hongshengwenyu.top/gtfovdkddq.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.dianchejie.cn/gtuvplafey.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.yanxiufei.cn/gtzbsjumtz.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.ydjk.org.cn/gtdgfxwyhw.html

[P03] 生成短随机字符串
来源：http://hz.52xcode.cn/gtjdtnejjf.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.nwbrower.top/gtngncettu.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.chenlongwang.top/gtkbcycevk.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.sufxvd.cn/gtcirxnhlp.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.xziqi.cn/gtjupipvfq.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.pengpengdd.cyou/gtwfpsgtbk.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.sufxvd.cn/gtbopjgnxo.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.haohaochexian.top/gtfdxtklpu.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.tanke756.top/gtxbvudhsv.html

[P04] 求长度
来源：http://hz.yueranfly.top/gtchlcvtod.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.shzxlz.cn/gtxrrkffuk.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.yanxiufei.cn/gtofubphcp.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.hnxiangtu.top/gtpisamcxk.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.andypj.xyz/gtvyuxicso.html

Java: list.size();  map.size();  s.length()
来源：http://hz.havefunace.top/gtkkuxkink.html

Go:   len(arr);  len(m)
来源：http://hz.zycfv.cn/gtorebpzrz.html

Ruby: x.length;  x.size
来源：http://hz.cdnleiting.top/gtbqfyetog.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.hnqzz.top/gtizptbgbb.html

[P05] 判断两个对象内容是否相等
来源：http://hz.nanxinkj.top/gthlagjsgi.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.shuidangran.top/gtrrybueej.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.ydjk.org.cn/gttrakdmvx.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.gzhubu.top/gtijqsnptw.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.hnqzz.top/gtjeaxesem.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.zhixingplan.top/gtvjyrjjvf.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.nanxinkj.top/gtaqlzaurm.html

Ruby: a == b
来源：http://hz.52xcode.cn/gtxjrrlfda.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.yonumen.top/gtyfxymbii.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.jinghuilouyu.cn/gtyidsfglh.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.cucudq.cn/gtjpayrttx.html

PHP:  if (empty($x)) {}
来源：http://hz.tanke756.top/gtxlmkddpc.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.shanyushiyangkeji.top/gtmkqqacoz.html

TS:   if (x == null) {}
来源：http://hz.yvedp.cn/gtehjbttzf.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.shanyushiyangtech.top/gtizgjsbnv.html

Go:   if x == nil {}
来源：http://hz.sweek.top/gtruahldpy.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.nanxuanxn.top/gtsmavmewf.html

C#:   if (x is null) {}
来源：http://hz.0kj1m.cn/gtfonyjwbu.html

[P07] 防抖与节流
来源：http://hz.andypj.xyz/gtstfgvlms.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.hnqzz.top/gtomgcirro.html

PHP:  // 手写时间戳比较
来源：http://hz.ybcxt.top/gtrcpyenhx.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.hammf.cn/gtljpkwvqn.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.hfpthk.cn/gtbywysasu.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.shzxlz.cn/gtjjtbmgfc.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.hfpthk.cn/gtylygcclr.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.aizwys.cn/gtiksljdlg.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.iojbl.cn/gtujzrpypy.html

[P08] 处理浮点精度问题
来源：http://hz.chenjidiqi.icu/gtpoomluhq.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.shangyingyoupin.top/gtwzayosiy.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.316326.xyz/gtrtbakdev.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.hywenlv.cn/gtcjtsjdfl.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.birdmap.top/gtrlviehua.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.cucudq.cn/gtzsxhlxan.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.9152youxi.cn/gtnklujkys.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.hfpthk.cn/gtkqnzqbyy.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.jiagoushi.top/gtwhxwgqrf.html

================================================================================
来源：http://hz.aizwys.cn/gtgrkcirrv.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.mhx1999.top/gtpkyrilph.html

================================================================================
来源：http://hz.wangdashe.top/gtayvmijwt.html

[Q01] 创建表
来源：http://hz.redwolf501.top/gtdiosvwnf.html

CREATE TABLE users (
来源：http://hz.chenjidiqi.icu/gttuemsgwn.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.hysaishi.cn/gtqdmorzuo.html

name VARCHAR(50) NOT NULL,
来源：http://hz.jinyuanbaomall.cn/gtlviopyej.html

email VARCHAR(100) UNIQUE,
来源：http://hz.jqgfzy.top/gtthjzqgmx.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.gotoacloud.top/gtskfzckuy.html

);
来源：http://hz.zdqjudy.top/gtnqfldxbu.html

[Q02] 创建带外键的表
来源：http://hz.ydzc1.top/gthjbdhqkh.html

CREATE TABLE orders (
来源：http://hz.tanke756.top/gthkysfdts.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.hysaishi.cn/gthpqjfqpk.html

user_id INT NOT NULL,
来源：http://hz.52xcode.cn/gtxyuzlujf.html

amount DECIMAL(10, 2),
来源：http://hz.hammf.cn/gtgwovwwoo.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.sysykeji.top/gtvntqgoiv.html

);
来源：http://hz.feifeiyinyue.top/gtczvfunms.html

[Q03] 增加列
来源：http://hz.zhengqikj.top/gtpfejnmcy.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.guowangkeji.top/gtjqmmhnhu.html

[Q04] 修改列类型
来源：http://hz.svipenyu.cn/gtgeygoihk.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.dashuyun.cn/gtqwmljxpx.html

[Q05] 重命名列
来源：http://hz.dashuyun.cn/gtutfjxbki.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.jqgufenzy.top/gtgiwamepp.html

[Q06] 删除列
来源：http://hz.ywan-chungtsiang.top/gtodwhvsch.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.zhoulong.xyz/gtjasazlfv.html

[Q07] 删除表
来源：http://hz.havefunace.top/gtxhgitxik.html

DROP TABLE IF EXISTS orders;
来源：http://hz.xinyue.icu/gthsuiivgb.html

[Q08] 创建普通索引
来源：http://hz.snrcjt.cn/gtlilcxjyc.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.snrcjt.cn/gtaemjleen.html

[Q09] 创建唯一索引
来源：http://hz.nanxuanxn.top/gtjpdcocih.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.hywenlv.cn/gtfzvfbeds.html

[Q10] 插入单行
来源：http://hz.daria6918.cn/gttiuamjjq.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.daria6918.cn/gtcmjmupci.html

[Q11] 一次插入多行
来源：http://hz.shangyingyoupin.top/gtfpanovcg.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.0kj1m.cn/gtxecroyhf.html

[Q12] 插入后取自增 ID
来源：http://hz.zhengqikj.top/gtsnhfjdam.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.zhaomingkeji.xyz/gtubdikxjo.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.feifeiyinyue.top/gtcfrijhts.html

[Q13] 忽略重复插入
来源：http://hz.zdqjudy.top/gtmhibebne.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.aizwys.cn/gtttdixuqr.html

[Q14] 存在则更新（upsert）
来源：http://hz.hysaishi.cn/gtwmvizbmu.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.wangdashe.top/gtklmfkhcq.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.ehwqpu.com/gtzoiuhlma.html

[Q15] 查询全部
来源：http://hz.daxiang520.top/gtqgdkscks.html

SELECT * FROM users;
来源：http://hz.aizwys.cn/gttfdknbkl.html

[Q16] 查询指定列
来源：http://hz.jqgufenzy.top/gtldlesytc.html

SELECT id, name FROM users;
来源：http://hz.hammf.cn/gtoprawjdl.html

[Q17] 条件查询
来源：http://hz.cheryme.top/gtaldftwcq.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.chenlongwang.top/gteiydrexo.html

[Q18] 模糊匹配
来源：http://hz.hfpthk.cn/gtcplxnaml.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.aizwys.cn/gtttdrvhyf.html

[Q19] 范围查询
来源：http://hz.jinqigfzy.top/gtrusnuhta.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.feifeiyinyue.top/gthhtfwexc.html

[Q20] IN 列表
来源：http://hz.aizwys.cn/gtrxxpcbda.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.gzhubu.top/gtezcpeuxs.html

[Q21] 空值判断
来源：http://hz.xziqi.cn/gtyfjbqxqt.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.iojbl.cn/gttmgbbsmc.html

[Q22] 排序
来源：http://hz.kuanghao11.cn/gtsyrjcdua.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.birdmap.top/gttlugufuv.html

[Q23] 分页
来源：http://hz.bjfxy.top/gthavkceaj.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.sysykeji.top/gtarmbgkvz.html

[Q24] 去重
来源：http://hz.zhiwuduotai.top/gtviiyplrv.html

SELECT DISTINCT city FROM users;
来源：http://hz.cdnleiting.top/gtfselgaoe.html

[Q25] 只取前 N 条
来源：http://hz.aizwys.cn/gtfzbtlzbl.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.jyoumei.cn/gtihyymygn.html

[Q26] 计数
来源：http://hz.chenlongwang.top/gtwllwpofp.html

SELECT COUNT(*) FROM users;
来源：http://hz.shzxlz.cn/gtlnpnsoku.html

[Q27] 条件计数
来源：http://hz.zhaomingkeji.xyz/gtuvsfdubv.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.xylfe.cn/gtctpyxpol.html

[Q28] 求和与平均
来源：http://hz.gotoacloud.top/gtzvufrxbe.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.dashuyun.cn/gtcnwuzzqr.html

[Q29] 最大最小值
来源：http://hz.jinghuilouyu.cn/gtzibskdgi.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.daxiang520.top/gtozzguyvj.html

[Q30] 分组统计
来源：http://hz.vqdsnc.cn/gtttfrybvr.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.shanyushiyangkeji.top/gtoatwtkcg.html

[Q31] 分组后过滤
来源：http://hz.jinghuilouyu.cn/gterjikynf.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.zhoulong.xyz/gtjvevcjin.html

[Q32] 分组拼接字符串
来源：http://hz.nanxinkj.top/gtcdabysvh.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.fengsongda.top/gtkqhamvyb.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.hnqzz.top/gtlboerqtc.html

[Q33] 多列分组
来源：http://hz.mhx1999.top/gtpwngrpsg.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.tianlin.xyz/gtcurwqlun.html

[Q34] 每组取第一条
来源：http://hz.cashguo.top/gthkdxblri.html

SELECT * FROM (
来源：http://hz.tian-w.cn/gtdlzwwqxh.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.cheryme.top/gterqbtnaz.html

) t WHERE rn = 1;
来源：http://hz.shangyingyoupin.top/gtrjidokod.html

[Q35] 内连接
来源：http://hz.jyoumei.cn/gtjlnfwcuh.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.zhengqikj.top/gteevwywqw.html

[Q36] 左连接
来源：http://hz.daxiang520.top/gtnnprdkev.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.nanxuanxn.top/gtjguyrsnp.html

[Q37] 右连接
来源：http://hz.zhiwuduotai.top/gtwhzumaoj.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.hysaishi.cn/gtogwutotz.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.yuanzhike.top/gtzhyopkmc.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.aizwys.cn/gtpheamzsq.html

[Q39] 自连接（查上下级）
来源：http://hz.pycfn.com/gtfzpvhdua.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.tanke756.top/gtdlphxjdf.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.sxryk.cn/gtcxsmnpyp.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.cheryme.top/gtlctdtjzf.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.ivvv.top/gthhztsgeg.html

[Q41] 多表连接
来源：http://hz.svipenyu.cn/gtslnhdzau.html


<!-- 参考信息 -->