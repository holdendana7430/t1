代发 wailian999

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.yj20258.top/gtiplswbzr.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.andypj.xyz/gtgoawrghz.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.daxiang520.top/gtuiiienaq.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.jinqigufen.top/gtocslhiuv.html

[N05] 最大公约数
来源：http://hz.feifeiyinyue.top/gtalypctkc.html

Py:   math.gcd(a, b)
来源：http://hz.aizwys.cn/gtkailgkbg.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.zhoulong.xyz/gtwaqenpao.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.cucudq.cn/gtsgmwlmit.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.haohaochexian.top/gtjqrcvpci.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.yuxming.cn/gtusvvbxxn.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.xylfe.cn/gtsycokcyl.html

Ruby: a.gcd(b)
来源：http://hz.hammf.cn/gtzxgxenes.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.xuanzx.com/gtmwwpyhwd.html

[N06] 判断回文字符串
来源：http://hz.zhijiandao.cn/gtpjtvavnj.html

Py:   s == s[::-1]
来源：http://hz.c1oappe.top/gtiwktself.html

PHP:  $s === strrev($s);
来源：http://hz.jinyuanbaomall.cn/gtzcnkfhcl.html

JS:   s === [...s].reverse().join("")
来源：http://hz.jqgufenzy.top/gttbkvipbr.html

TS:   s === [...s].reverse().join("")
来源：http://hz.yj20258888.top/gtdkujboxe.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.quarkkingdee.top/gtecwpezsw.html

Go:   // 双指针从两端比较
来源：http://hz.jinqigfzy.top/gthysoetij.html

Ruby: s == s.reverse
来源：http://hz.xinyue.icu/gtpwkodghf.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.daria6918.cn/gtcfoisaia.html

[N07] 两数之和（返回下标）
来源：http://hz.hysaishi.cn/gthnqhkbju.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.sufxvd.cn/gtwctmzqtd.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.andypj.xyz/gtpfjbvqnm.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.ppjwa.cn/gtorgwkvwk.html

TS:   // 手写 Map<string, number>
来源：http://hz.shangyingyoupin.top/gtyomcytmp.html

Java: // 手写 HashMap
来源：http://hz.xingfuxueyuan.xyz/gtrphtyrob.html

Go:   // 手写 map[int]int
来源：http://hz.xylfe.cn/gtuvmgyybq.html

Ruby: // 手写 Hash
来源：http://hz.aizwys.cn/gtdnhbiccr.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.wangshuangyany.cn/gtfdykpmub.html

[N08] 生成全排列
来源：http://hz.zhoulong.xyz/gtwhwvycnp.html

Py:   itertools.permutations(arr)
来源：http://hz.yj20258888.top/gtvnzbriqw.html

PHP:  // 手写递归交换
来源：http://hz.jlsjyb.cn/gttngpomge.html

JS:   // 手写回溯递归
来源：http://hz.guowangkeji.top/gtxvxwbdht.html

TS:   // 手写回溯递归
来源：http://hz.zhiwuduotai.top/gtpgiwzpmj.html

Java: // 手写回溯递归
来源：http://hz.gotoacloud.top/gteucycrvq.html

Go:   // 手写回溯递归
来源：http://hz.jqgfzy.top/gtujzvxgnu.html

Ruby: arr.permutation.to_a
来源：http://hz.cashguo.top/gtdcmoombv.html

C#:   // 手写回溯递归
来源：http://hz.ydjk.org.cn/gthjkpwfgy.html

[N09] 栈与队列
来源：http://hz.haohaochexian.top/gtznhlzzck.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.yanxiufei.cn/gtbdgudcxr.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.zhongyouzk.top/gtdrzujmnv.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.mhx1999.top/gteggseary.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.feifeiyinyue.top/gtzvwbpsej.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.mhx1999.top/gtjovppsah.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.zhengqikj.top/gtppgvgjna.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.nanxuanxn.top/gtfdhbzsfw.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.yanxiufei.cn/gtvowkkmpx.html

[N10] 链表节点定义
来源：http://hz.jianghu66.top/gtwkurnsfs.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.ywan-chungtsiang.top/gtslsayaei.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.haohaochexian.top/gtnzkosuyi.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.gaohongyu789.top/gttlcelyiq.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.zdqjudy.top/gtmtfhrszy.html

Java: class Node { int v; Node next; }
来源：http://hz.havefunace.top/gthqcigbul.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.zhongyouzk.top/gtwceipzyt.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.vqdsnc.cn/gtjpnxgvfv.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.redwolf501.top/gtmqjpafey.html

[N11] 二叉树中序遍历
来源：http://hz.hysaishi.cn/gtcrlztyvs.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.jinyuanbaomall.cn/gtcqftedtf.html

PHP:  // 手写递归函数
来源：http://hz.guannengcc.top/gtefuidpga.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.yongpay.top/gtwedapgiu.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.yvedp.cn/gtxvfeebdp.html

Java: // 手写递归
来源：http://hz.jqgufenzy.top/gtytxslekx.html

Go:   // 手写递归
来源：http://hz.ybcxt.top/gtvcpkyalw.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.birdmap.top/gtftdwlqhc.html

C#:   // 手写递归
来源：http://hz.jinqigufen.top/gtlidzunip.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.hnxiangtu.top/gtbltkcier.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.daria6918.cn/gtkbkkuvrm.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.hongshengwenyu.top/gteotzgywb.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.sxryk.cn/gtiruollqq.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.yj202588.top/gtrocwwjws.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.tianlin.xyz/gtbprbzksx.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.wangdashe.top/gtqmcorbcx.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.daxiang520.top/gtpldcclkj.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.tianlin.xyz/gttalkyfzy.html

================================================================================
来源：http://hz.cqqwz.cn/gtiysnnpua.html

O. 并发与异步
来源：http://hz.wangdashe.top/gtmejyobyg.html

================================================================================
来源：http://hz.cashguo.top/gtmdslncwb.html

[O01] 启动一个线程
来源：http://hz.ydjk.org.cn/gtrcgckmkl.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.cdnleiting.top/gtstgdvqoa.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.yonumen.top/gtgqmtlxam.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.chenzaomai.com/gtaarupzoa.html

TS:   // 同 JS
来源：http://hz.dashuyun.cn/gtnvuojnvc.html

Java: new Thread(() -> f()).start()
来源：http://hz.shangyingyoupin.top/gtekhdclsd.html

Go:   go f()
来源：http://hz.tanke756.top/gtsspmxyvc.html

Ruby: Thread.new { f }
来源：http://hz.hnqzz.top/gturnpelgy.html

C#:   Task.Run(() => F());
来源：http://hz.9152youxi.cn/gtlqrnwvgn.html

[O02] 使用线程池
来源：http://hz.bjfxy.top/gthuqknyvh.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.smart0.xyz/gtmharyrua.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.hongshengwenyu.top/gtcztztzxi.html

JS:   // worker_threads 线程池
来源：http://hz.yongpay.top/gtrlgmddnz.html

TS:   // worker_threads 线程池
来源：http://hz.chenlongwang.top/gtgsznqnvz.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.ppjwa.cn/gtagvnrhsm.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.cqqwz.cn/gtdskowcqj.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.zhiwuduotai.top/gtufpoggbf.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.cucudq.cn/gtadpcypae.html

[O03] 加锁保护共享数据
来源：http://hz.kuanghao11.cn/gtuofyfjix.html

Py:   with lock: shared += 1
来源：http://hz.chenjidiqi.icu/gttwgrgnsf.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.hammf.cn/gtblxcvhis.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.shzxlz.cn/gtcdphpmjq.html

TS:   // 同 JS
来源：http://hz.sufxvd.cn/gtmpmjwlbt.html

Java: synchronized (this) { shared++; }
来源：http://hz.jqgufenzy.top/gtfvggtbai.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.52xcode.cn/gtbxrlcmmh.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.havefunace.top/gtscrjanop.html

C#:   lock (gate) { shared++; }
来源：http://hz.hfpthk.cn/gtcomadvrv.html

[O04] 定义异步函数并等待
来源：http://hz.nanxuanxn.top/gtteepvstm.html

Py:   async def f():⏎    await g()
来源：http://hz.jinghuilouyu.cn/gtwegtjyds.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.52xcode.cn/gtaiuhvxas.html

JS:   async function f() { await g(); }
来源：http://hz.chenzaomai.com/gtjbxojgfi.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.zhoulong.xyz/gtkcwocxny.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.ybcxt.top/gtnzyapvuo.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.cheryme.top/gtdgakegix.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.xylfe.cn/gtiogxwcnr.html

C#:   async Task F() { await G(); }
来源：http://hz.sysykeji.top/gtuhxwfrrw.html

[O05] 并发执行并等待全部完成
来源：http://hz.xuetiantiany.cn/gtvlgayzdn.html

Py:   asyncio.gather(*tasks)
来源：http://hz.hongshengwenyu.top/gtsbkdpfap.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.nwbrower.top/gtiwtshlga.html

JS:   await Promise.all(tasks)
来源：http://hz.ivvv.top/gtrppfcrsl.html

TS:   await Promise.all(tasks)
来源：http://hz.pycfn.com/gtuinrnwca.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.hysaishi.cn/gtmgutfsea.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.zhengqikj.top/gtvccolclr.html

Ruby: threads.map(&:join)
来源：http://hz.0kj1m.cn/gtcfgvlgvs.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.ydzc1.top/gtenxfxukp.html

[O06] 使用进程池
来源：http://hz.aibaodan.cn/gtuuvdabtr.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.zhixingplan.top/gtptvmhzgl.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.vqdsnc.cn/gtaudntbqg.html

JS:   // child_process / cluster 模块
来源：http://hz.jinghuilouyu.cn/gtekglgtpg.html

TS:   // child_process / cluster 模块
来源：http://hz.shuidangran.top/gtlplbzuaf.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.yanxiufei.cn/gtnmuvtqwu.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.mhx1999.top/gtrhcnbrzl.html

Ruby: // fork 块
来源：http://hz.haohaochexian.top/gtyozypwil.html

C#:   Parallel.For
来源：http://hz.cqqwz.cn/gtcxczemwd.html

================================================================================
来源：http://hz.ydzc1.top/gtnlhpygxp.html

P. 常用工具函数
来源：http://hz.xingfuxueyuan.xyz/gtnajipddh.html

================================================================================
来源：http://hz.shanyushiyangkeji.top/gtvgoopirl.html

[P01] 生成 UUID
来源：http://hz.zdqjudy.top/gtrtcvvopo.html

Py:   str(uuid.uuid4())
来源：http://hz.fzhhl.top/gtyejsinkj.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.nwbrower.top/gtixdfijmk.html

JS:   crypto.randomUUID()
来源：http://hz.nanxuanxn.top/gtejmctoyo.html

TS:   crypto.randomUUID()
来源：http://hz.sxryk.cn/gtduylxoof.html

Java: UUID.randomUUID().toString()
来源：http://hz.shuidangran.top/gtfepcptjx.html

Go:   // 用 github.com/google/uuid
来源：http://hz.yuxming.cn/gtqpkspsdc.html

Ruby: SecureRandom.uuid
来源：http://hz.yonumen.top/gtkopsolfi.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.xingfuxueyuan.xyz/gtcddvftvh.html

[P02] MD5 / SHA256 摘要
来源：http://hz.quarkkingdee.top/gtayjhgoyd.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.nwbrower.top/gtdfiyttmb.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.shangyingyoupin.top/gtommttjwv.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.52xcode.cn/gtsqtxcwnz.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.cashguo.top/gtkqcxnaoh.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.yueranfly.top/gtuurvrgpm.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.wangdashe.top/gtqhrxaaxp.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.yueranfly.top/gtfnggwtus.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.ywan-chungtsiang.top/gtzlcmywie.html

[P03] 生成短随机字符串
来源：http://hz.jinqigufen.top/gtlflevrmi.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.chenlongwang.top/gtywjxsihp.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.ppjwa.cn/gtpstyuunn.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.bjfxy.top/gtbvszsvbq.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.chenzaomai.com/gtkzrpzrtr.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.ydzc1.top/gtfwmmvcdw.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.sweek.top/gtwvyfsnuz.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.9152youxi.cn/gtfdsyogyv.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.gzhubu.top/gthmpmzvfl.html

[P04] 求长度
来源：http://hz.xuanzx.com/gtfhmyujxq.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.hnxiangtu.top/gtqqxixbox.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.shanyushiyangtech.top/gtbxkupsxh.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.jqgufenzy.top/gtjkcckhuj.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.hysaishi.cn/gtzjvvffuu.html

Java: list.size();  map.size();  s.length()
来源：http://hz.xuanzx.com/gtjjxeaypg.html

Go:   len(arr);  len(m)
来源：http://hz.svipenyu.cn/gtyyybxlgw.html

Ruby: x.length;  x.size
来源：http://hz.andypj.xyz/gtrmdujjzv.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.quarkkingdee.top/gtuxzfyagk.html

[P05] 判断两个对象内容是否相等
来源：http://hz.xingfuxueyuan.xyz/gtsnshdxem.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.nanxinkj.top/gtxochgriu.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.quarkkingdee.top/gtdjmkbbhi.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.hywenlv.cn/gtyraqqbfh.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.ppjwa.cn/gtnlqgzwbk.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.jqgufenzy.top/gttoclkerb.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.gogol.net.cn/gtmyxzsaqe.html

Ruby: a == b
来源：http://hz.hongshengwenyu.top/gtvfjhbeob.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.pengpengdd.cyou/gtojxgxpqf.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.dashuyun.cn/gtoarwiqyn.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.ydjk.org.cn/gtexvvsyti.html

PHP:  if (empty($x)) {}
来源：http://hz.xylfe.cn/gtiuowiubk.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.zhongyouzk.top/gtvzmgnsjl.html

TS:   if (x == null) {}
来源：http://hz.shangyingyoupin.top/gtfogzllkh.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.chenjidiqi.icu/gtxitorxqn.html

Go:   if x == nil {}
来源：http://hz.yj20258.top/gtuppluowg.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.0kj1m.cn/gtcwfoymii.html

C#:   if (x is null) {}
来源：http://hz.jqgufenzy.top/gtyenvpogn.html

[P07] 防抖与节流
来源：http://hz.hongshengwenyu.top/gtrhobrupb.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.jinghuilouyu.cn/gtykrbfyfc.html

PHP:  // 手写时间戳比较
来源：http://hz.andypj.xyz/gtlwyzaukb.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.shanyushiyangkeji.top/gtkqontybu.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.zhijiandao.cn/gtevbszokf.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.jinqigfzy.top/gtxnoisyrt.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.ivvv.top/gtvlkklrhw.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.zhengqikj.top/gtxoabjmwz.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.shanyushiyangtech.top/gthsqgscrx.html

[P08] 处理浮点精度问题
来源：http://hz.dashuyun.cn/gtfyppyyoi.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.zhijiandao.cn/gtkgaaohmo.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.jinyuanbaomall.cn/gthyqohohv.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.yonumen.top/gtxxmdmobz.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.vqdsnc.cn/gtxapjermb.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.tianlin.xyz/gtznzofael.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.tianlin.xyz/gtauxlxiwa.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.hammf.cn/gtuaqaqoew.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.zhoulong.xyz/gtpxmschdc.html

================================================================================
来源：http://hz.zhoulong.xyz/gthbckycdq.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.nanxinkj.top/gtqnpkjcwz.html

================================================================================
来源：http://hz.jinqigfzy.top/gtgwovozpm.html

[Q01] 创建表
来源：http://hz.zhengqikj.top/gtcxhtndvr.html

CREATE TABLE users (
来源：http://hz.gotoacloud.top/gtpkmnpfkb.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.feifeiyinyue.top/gtzhaymwva.html

name VARCHAR(50) NOT NULL,
来源：http://hz.nanxuanxn.top/gttkfqjqro.html

email VARCHAR(100) UNIQUE,
来源：http://hz.sysykeji.top/gtcxrrttvf.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.xuanzx.com/gtttjfweqd.html

);
来源：http://hz.yonumen.top/gtrgsdgvko.html

[Q02] 创建带外键的表
来源：http://hz.wangshuangyany.cn/gtdrxljcay.html

CREATE TABLE orders (
来源：http://hz.ywan-chungtsiang.top/gtphmxbyoh.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.cashguo.top/gtpfyiojbw.html

user_id INT NOT NULL,
来源：http://hz.yj20258.top/gtsrmsizqj.html

amount DECIMAL(10, 2),
来源：http://hz.jiagoushi.top/gttnmqjpsk.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.guannengcc.top/gtcgxlvade.html

);
来源：http://hz.birdmap.top/gtjqalintb.html

[Q03] 增加列
来源：http://hz.ivvv.top/gtywfewyxu.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.zhengqikj.top/gtlnzvaywn.html

[Q04] 修改列类型
来源：http://hz.316326.xyz/gtfzocymwq.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.daxiang520.top/gtjwrszwmf.html

[Q05] 重命名列
来源：http://hz.chenjidiqi.icu/gttqwuqwjc.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.yuxming.cn/gthflwshyx.html

[Q06] 删除列
来源：http://hz.hnxiangtu.top/gtngnbygaw.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.gzhubu.top/gtevafusei.html

[Q07] 删除表
来源：http://hz.quarkkingdee.top/gtwsdxsdks.html

DROP TABLE IF EXISTS orders;
来源：http://hz.kuanghao11.cn/gtyyzmnbxs.html

[Q08] 创建普通索引
来源：http://hz.havefunace.top/gtdlfgmmmb.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.cucudq.cn/gtqydpuzki.html

[Q09] 创建唯一索引
来源：http://hz.redwolf501.top/gtvwrkoamv.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.jinqigufen.top/gtslspenbj.html

[Q10] 插入单行
来源：http://hz.cheryme.top/gtpgyazmna.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.gogol.net.cn/gtooqnfoow.html

[Q11] 一次插入多行
来源：http://hz.vqdsnc.cn/gtanouabqq.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.zycfv.cn/gtitghlktm.html

[Q12] 插入后取自增 ID
来源：http://hz.yonumen.top/gtabpyffse.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.yuxming.cn/gtkcjqacbs.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.zycfv.cn/gtltmzhtzd.html

[Q13] 忽略重复插入
来源：http://hz.xuetiantiany.cn/gtidullhlt.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.sufxvd.cn/gtkmgsbngy.html

[Q14] 存在则更新（upsert）
来源：http://hz.zdqjudy.top/gtiohpqkya.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.yj20258888.top/gtqenyvkrg.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.mhx1999.top/gtqkkentde.html

[Q15] 查询全部
来源：http://hz.daxiang520.top/gttbypaqvm.html

SELECT * FROM users;
来源：http://hz.daria6918.cn/gtzfyrkqog.html

[Q16] 查询指定列
来源：http://hz.cashguo.top/gtuinudtvh.html

SELECT id, name FROM users;
来源：http://hz.quarkkingdee.top/gtszifejir.html

[Q17] 条件查询
来源：http://hz.nanxinkj.top/gtbuizopmp.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.guowangkeji.top/gtkoqsumei.html

[Q18] 模糊匹配
来源：http://hz.quarkkingdee.top/gtgbzkshbu.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.zhiwuduotai.top/gtngnzwkbo.html

[Q19] 范围查询
来源：http://hz.hywenlv.cn/gtnadbfvkv.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.shzxlz.cn/gtcxoicmen.html

[Q20] IN 列表
来源：http://hz.hysaishi.cn/gttgpgxlsa.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.zhaomingkeji.xyz/gtnffurgiy.html

[Q21] 空值判断
来源：http://hz.sxryk.cn/gtcsbndivv.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.yuanzhike.top/gtzygcfprl.html

[Q22] 排序
来源：http://hz.bjfxy.top/gtzxkuxktp.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.svipenyu.cn/gtamziqnoy.html

[Q23] 分页
来源：http://hz.zhongyouzk.top/gtrwybmofn.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.andypj.xyz/gtacskotiz.html

[Q24] 去重
来源：http://hz.shangyingyoupin.top/gtpwhjffny.html

SELECT DISTINCT city FROM users;
来源：http://hz.vqdsnc.cn/gtsdehmhgm.html

[Q25] 只取前 N 条
来源：http://hz.yuxming.cn/gteyuojkfn.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.zhixingplan.top/gtllziheng.html

[Q26] 计数
来源：http://hz.guowangkeji.top/gtlpxnbzce.html

SELECT COUNT(*) FROM users;
来源：http://hz.hywenlv.cn/gtcmtysqqq.html

[Q27] 条件计数
来源：http://hz.zhijiandao.cn/gtwcffrrtp.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.yj20258.top/gtpepfbgbf.html

[Q28] 求和与平均
来源：http://hz.pengpengdd.cyou/gtcvvvxojp.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.yj20258.top/gtohedoesb.html

[Q29] 最大最小值
来源：http://hz.feifeiyinyue.top/gtutrfscoi.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.zhaomingkeji.xyz/gtlbgqcsjc.html

[Q30] 分组统计
来源：http://hz.yueranfly.top/gtbgluahzi.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.jqgfzy.top/gthxrileyf.html

[Q31] 分组后过滤
来源：http://hz.dashuyun.cn/gtibsazgcn.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.tian-w.cn/gtecifcjxv.html

[Q32] 分组拼接字符串
来源：http://hz.pengpengdd.cyou/gtptoaatjx.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.cashguo.top/gtcnnsktkq.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.jiagoushi.top/gtpabmxjmm.html

[Q33] 多列分组
来源：http://hz.jyoumei.cn/gtbkfgxjsd.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.sysykeji.top/gtihkbvhkr.html

[Q34] 每组取第一条
来源：http://hz.hysaishi.cn/gthqjmobbe.html

SELECT * FROM (
来源：http://hz.xuetiantiany.cn/gtmipnflex.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.aizwys.cn/gtfacztxcf.html

) t WHERE rn = 1;
来源：http://hz.yueranfly.top/gtrkdgzojm.html

[Q35] 内连接
来源：http://hz.smart0.xyz/gtfdfwnrbl.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.daria6918.cn/gttajfiqol.html

[Q36] 左连接
来源：http://hz.chenjidiqi.icu/gteoinygky.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.dianchejie.cn/gtvvqftkkj.html

[Q37] 右连接
来源：http://hz.tanke756.top/gtaiazldqd.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.ybcxt.top/gtxiyvtbal.html


<!-- 参考信息 -->