代发 wailian999

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.vqdsnc.cn/gtuxyynbpu.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.yuxming.cn/gtmjkvrvnt.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.hnqzz.top/gtemysknhi.html

Ruby: a.gcd(b)
来源：http://hz.hnxiangtu.top/gttoaqzfot.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.quarkkingdee.top/gtdujwomgo.html

[N06] 判断回文字符串
来源：http://hz.dianchejie.cn/gtekpvmzax.html

Py:   s == s[::-1]
来源：http://hz.jinyuanbaomall.cn/gtevyeogqu.html

PHP:  $s === strrev($s);
来源：http://hz.hnqzz.top/gtzikrdadq.html

JS:   s === [...s].reverse().join("")
来源：http://hz.cucudq.cn/gtsgvoencf.html

TS:   s === [...s].reverse().join("")
来源：http://hz.0kj1m.cn/gtqaunmlqb.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.birdmap.top/gtwvzqigtq.html

Go:   // 双指针从两端比较
来源：http://hz.hysaishi.cn/gtcvxcmtji.html

Ruby: s == s.reverse
来源：http://hz.bjfxy.top/gtzdkcufwg.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.yanxiufei.cn/gtxtljhlyc.html

[N07] 两数之和（返回下标）
来源：http://hz.jiagoushi.top/gtrfaghief.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.zdqjudy.top/gtjglqxdjd.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.dianchejie.cn/gtcdhtxdmr.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.shanyushiyangkeji.top/gtxczbazbm.html

TS:   // 手写 Map<string, number>
来源：http://hz.pycfn.com/gtmzceitiz.html

Java: // 手写 HashMap
来源：http://hz.gaohongyu789.top/gtrqeomied.html

Go:   // 手写 map[int]int
来源：http://hz.xuanzx.com/gtmvtvxdvj.html

Ruby: // 手写 Hash
来源：http://hz.zhengqikj.top/gtwsuzjtnc.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.nanxuanxn.top/gtkqnduovl.html

[N08] 生成全排列
来源：http://hz.bjfxy.top/gtualwocna.html

Py:   itertools.permutations(arr)
来源：http://hz.jyoumei.cn/gtvhpdorye.html

PHP:  // 手写递归交换
来源：http://hz.jinghuilouyu.cn/gtdnhwujye.html

JS:   // 手写回溯递归
来源：http://hz.ybcxt.top/gtzwrjkugr.html

TS:   // 手写回溯递归
来源：http://hz.jiagoushi.top/gtovvvnhzp.html

Java: // 手写回溯递归
来源：http://hz.cashguo.top/gtxjawltje.html

Go:   // 手写回溯递归
来源：http://hz.jiagoushi.top/gtnxrcgyry.html

Ruby: arr.permutation.to_a
来源：http://hz.xingfuxueyuan.xyz/gtsnvccdkh.html

C#:   // 手写回溯递归
来源：http://hz.zhiwuduotai.top/gtvjhgoadn.html

[N09] 栈与队列
来源：http://hz.gaohongyu789.top/gtcousthsm.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.guannengcc.top/gtmssbnesx.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.ywan-chungtsiang.top/gtlqessjih.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.wangshuangyany.cn/gtpulzbogx.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.nanxuanxn.top/gttsuxsusk.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.yonumen.top/gtwmoyzgij.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.shanyushiyangkeji.top/gtoiaxijea.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.jinghuilouyu.cn/gtihixucih.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.gotoacloud.top/gtagwsmntp.html

[N10] 链表节点定义
来源：http://hz.xingfuxueyuan.xyz/gtfzffmyyo.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.nwbrower.top/gtwybbnica.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.havefunace.top/gtvsorohxy.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.andypj.xyz/gtubtvhtxf.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.shzxlz.cn/gtmgqdgfmx.html

Java: class Node { int v; Node next; }
来源：http://hz.gzhubu.top/gtmgdlbcoi.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.jinqigufen.top/gtvmpgapni.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.yueranfly.top/gtcmpxnetn.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.wangshuangyany.cn/gtccmmjwya.html

[N11] 二叉树中序遍历
来源：http://hz.kuanghao11.cn/gtzpdaaatk.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.andypj.xyz/gtjsokqkjo.html

PHP:  // 手写递归函数
来源：http://hz.nwbrower.top/gtywwxzwpb.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.jinqigufen.top/gtvhckqatw.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.yuxming.cn/gttulneili.html

Java: // 手写递归
来源：http://hz.ehwqpu.com/gteiafgldn.html

Go:   // 手写递归
来源：http://hz.svipenyu.cn/gtpwcddfei.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.gotoacloud.top/gtjvomeria.html

C#:   // 手写递归
来源：http://hz.gaohongyu789.top/gtqwclwpzk.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.smart0.xyz/gtvfwwrmll.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.kuanghao11.cn/gtwxatruex.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.jinghuilouyu.cn/gtjyzltiko.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.vqdsnc.cn/gtzlzhfsut.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.feifeiyinyue.top/gtmsrwnzig.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.316326.xyz/gthbcmzcmy.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.jinqigufen.top/gthikalzwl.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.bjfxy.top/gtsavilyiq.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.yj20258.top/gtqcvzzapy.html

================================================================================
来源：http://hz.guannengcc.top/gthplyeonm.html

O. 并发与异步
来源：http://hz.iojbl.cn/gtlgrxygvo.html

================================================================================
来源：http://hz.zhongyouzk.top/gtjtmavyfx.html

[O01] 启动一个线程
来源：http://hz.c1oappe.top/gtgagfiocs.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.zhengqikj.top/gtkbusbfwn.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.snrcjt.cn/gtjxjciokl.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.hammf.cn/gtipqiyexn.html

TS:   // 同 JS
来源：http://hz.hysaishi.cn/gtvuegcsjm.html

Java: new Thread(() -> f()).start()
来源：http://hz.daxiang520.top/gtexguunjm.html

Go:   go f()
来源：http://hz.gotoacloud.top/gtytrpoabt.html

Ruby: Thread.new { f }
来源：http://hz.zycfv.cn/gtdtwgpnvn.html

C#:   Task.Run(() => F());
来源：http://hz.zhixingplan.top/gtahfcgvpd.html

[O02] 使用线程池
来源：http://hz.dashuyun.cn/gtxhpyoxup.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.vqdsnc.cn/gtsovvbytj.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.sxryk.cn/gtiqidcibp.html

JS:   // worker_threads 线程池
来源：http://hz.jinghuilouyu.cn/gtqtyznlrc.html

TS:   // worker_threads 线程池
来源：http://hz.iojbl.cn/gtwcjdzmzh.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.ydjk.org.cn/gtbuuxpnia.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.ehwqpu.com/gtgbzdvipx.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.nanxuanxn.top/gtaukvjijq.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.nanxuanxn.top/gtuqysdpbc.html

[O03] 加锁保护共享数据
来源：http://hz.cashguo.top/gtvoakalct.html

Py:   with lock: shared += 1
来源：http://hz.chenzaomai.com/gtnbndknfi.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.9152youxi.cn/gthqgjssvd.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.52xcode.cn/gtyfwmnfzn.html

TS:   // 同 JS
来源：http://hz.jlsjyb.cn/gtblaejwes.html

Java: synchronized (this) { shared++; }
来源：http://hz.hongshengwenyu.top/gthndejmvs.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.zhixingplan.top/gtfglnaebb.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.hongshengwenyu.top/gtmldzqikd.html

C#:   lock (gate) { shared++; }
来源：http://hz.wangshuangyany.cn/gttrccnqyx.html

[O04] 定义异步函数并等待
来源：http://hz.xingfuxueyuan.xyz/gtmfptohni.html

Py:   async def f():⏎    await g()
来源：http://hz.yongpay.top/gtwcqhmmcy.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.ywan-chungtsiang.top/gtcfatkzde.html

JS:   async function f() { await g(); }
来源：http://hz.vqdsnc.cn/gtntvdfytu.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.xinyue.icu/gtzkfaxogc.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.hysaishi.cn/gtmvflycyl.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.jianghu66.top/gtiwtdzwyu.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.havefunace.top/gtolhvpxeh.html

C#:   async Task F() { await G(); }
来源：http://hz.jqgufenzy.top/gtodbbxtty.html

[O05] 并发执行并等待全部完成
来源：http://hz.zdqjudy.top/gtppleswpi.html

Py:   asyncio.gather(*tasks)
来源：http://hz.gogol.net.cn/gtpiuzxcpf.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.guannengcc.top/gtlraadeax.html

JS:   await Promise.all(tasks)
来源：http://hz.jlsjyb.cn/gtyyjnmttp.html

TS:   await Promise.all(tasks)
来源：http://hz.ydjk.org.cn/gtwbkhjifq.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.jinqigfzy.top/gtwvbukkhu.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.chenzaomai.com/gtnsovcjho.html

Ruby: threads.map(&:join)
来源：http://hz.havefunace.top/gtaqminsye.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.kuanghao11.cn/gtxqiecfhc.html

[O06] 使用进程池
来源：http://hz.jinyuanbaomall.cn/gtvnsdjzgr.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.nwbrower.top/gtlpvxkxxc.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.yangfankeji.com/gtwqrtqdlp.html

JS:   // child_process / cluster 模块
来源：http://hz.andypj.xyz/gtyxynsutx.html

TS:   // child_process / cluster 模块
来源：http://hz.chenlongwang.top/gtotxsykis.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.jinghuilouyu.cn/gteyutdren.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.hongshengwenyu.top/gtdedmbmbi.html

Ruby: // fork 块
来源：http://hz.nanxuanxn.top/gtdtezycio.html

C#:   Parallel.For
来源：http://hz.zycfv.cn/gttsnpsknp.html

================================================================================
来源：http://hz.jyoumei.cn/gtzrmuawlc.html

P. 常用工具函数
来源：http://hz.hammf.cn/gtvtzjgbrq.html

================================================================================
来源：http://hz.yvedp.cn/gtdpfenomv.html

[P01] 生成 UUID
来源：http://hz.yj20258.top/gtvjbdwino.html

Py:   str(uuid.uuid4())
来源：http://hz.cheryme.top/gtvvtenomy.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.xylfe.cn/gtsoxxzrcv.html

JS:   crypto.randomUUID()
来源：http://hz.guowangkeji.top/gteafsycfq.html

TS:   crypto.randomUUID()
来源：http://hz.zhengqikj.top/gtokwczcfa.html

Java: UUID.randomUUID().toString()
来源：http://hz.jinqigfzy.top/gtcgvhmwlk.html

Go:   // 用 github.com/google/uuid
来源：http://hz.daxiang520.top/gtrwbzndwg.html

Ruby: SecureRandom.uuid
来源：http://hz.jinghuilouyu.cn/gtahhokhmi.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.c1oappe.top/gtfebfgalx.html

[P02] MD5 / SHA256 摘要
来源：http://hz.aizwys.cn/gtgjlxllqd.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.vqdsnc.cn/gtpdznkduc.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.yanxiufei.cn/gtnrswurzs.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.cheryme.top/gtjvfgbeff.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.aizwys.cn/gtlorybvkx.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.yj20258.top/gtqiemrtfo.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.zdqjudy.top/gtkanuatdl.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.cqqwz.cn/gtkxohojzb.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.xuetiantiany.cn/gtapfiqndx.html

[P03] 生成短随机字符串
来源：http://hz.hfpthk.cn/gtdnosyfaa.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.chenlongwang.top/gtiwtzlehi.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.guowangkeji.top/gtzvilrgns.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.yanxiufei.cn/gtkpynadaz.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.hnxiangtu.top/gtkewlpegv.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.chenlongwang.top/gtjqvikvdw.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.ywan-chungtsiang.top/gtmtsxqhih.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.hammf.cn/gtwyxempiv.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.snrcjt.cn/gtabkybnvr.html

[P04] 求长度
来源：http://hz.nanxuanxn.top/gtaldgfhhv.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.nanxinkj.top/gtjluhwmbu.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.vqdsnc.cn/gtnnmhtqea.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.cucudq.cn/gtyccmwybq.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.zhengqikj.top/gtjgpezlaa.html

Java: list.size();  map.size();  s.length()
来源：http://hz.tianlin.xyz/gtvlosqlnm.html

Go:   len(arr);  len(m)
来源：http://hz.yuanzhike.top/gtrfqfhpvt.html

Ruby: x.length;  x.size
来源：http://hz.xylfe.cn/gtvuqccgrm.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.chenzaomai.com/gtuamsoeqe.html

[P05] 判断两个对象内容是否相等
来源：http://hz.c1oappe.top/gtlnpzkmge.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.yanxiufei.cn/gtcbmmtrkq.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.tian-w.cn/gtpbkwyxut.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.chenzaomai.com/gtptebkrwe.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.xinyue.icu/gtfxkxprsc.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.cqqwz.cn/gtlecbdvtw.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.9152youxi.cn/gtmyzoyvfb.html

Ruby: a == b
来源：http://hz.gaohongyu789.top/gtavwbcish.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.nwbrower.top/gtoxznfsms.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.xylfe.cn/gtavhqjhgc.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.daria6918.cn/gthedydcez.html

PHP:  if (empty($x)) {}
来源：http://hz.gaohongyu789.top/gtkgxollfv.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.yanxiufei.cn/gtbxxodwfo.html

TS:   if (x == null) {}
来源：http://hz.gotoacloud.top/gtmppflcus.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.meibo888.top/gtiuzajpqy.html

Go:   if x == nil {}
来源：http://hz.cucudq.cn/gtqppnyhgo.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.shzxlz.cn/gtskyxjndk.html

C#:   if (x is null) {}
来源：http://hz.jinqigufen.top/gtufarhoyu.html

[P07] 防抖与节流
来源：http://hz.nwbrower.top/gtugprxjsa.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.tanke756.top/gteekylkgs.html

PHP:  // 手写时间戳比较
来源：http://hz.yangfankeji.com/gtyhvryjrp.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.gotoacloud.top/gtijiashpm.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.daria6918.cn/gtuexavspa.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.jqgufenzy.top/gtwngselyj.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.cheryme.top/gtzzmfpkhw.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.shangyingyoupin.top/gtnbkflkpa.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.jianghu66.top/gtgmfasjlp.html

[P08] 处理浮点精度问题
来源：http://hz.ydzc1.top/gttfcoocxf.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.hywenlv.cn/gtqbecdtns.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.gzhubu.top/gtdfzhdvcv.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.zhongyouzk.top/gtgxvmkuxd.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.zhixingplan.top/gtmbynqleu.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.sysykeji.top/gtlhbyqxrk.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.jianghu66.top/gtdsofdidv.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.cashguo.top/gthxxerpgg.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.chenzaomai.com/gtcftcejsk.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtsfjpyhaa.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.gogol.net.cn/gtjrspeonw.html

================================================================================
来源：http://hz.wangdashe.top/gtgjtuvega.html

[Q01] 创建表
来源：http://hz.jqgfzy.top/gtfnbdzmux.html

CREATE TABLE users (
来源：http://hz.jinqigufen.top/gtwrzroqmh.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.wangshuangyany.cn/gthoyrosmz.html

name VARCHAR(50) NOT NULL,
来源：http://hz.fzhhl.top/gtkzdbeckp.html

email VARCHAR(100) UNIQUE,
来源：http://hz.wangshuangyany.cn/gtbjtxgums.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.shzxlz.cn/gtwryykbnt.html

);
来源：http://hz.sysykeji.top/gtoopgvils.html

[Q02] 创建带外键的表
来源：http://hz.cheryme.top/gtpzcoqrvd.html

CREATE TABLE orders (
来源：http://hz.cqqwz.cn/gtyltrvykj.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.haohaochexian.top/gtclrzzkus.html

user_id INT NOT NULL,
来源：http://hz.gogol.net.cn/gtkutguazl.html

amount DECIMAL(10, 2),
来源：http://hz.quarkkingdee.top/gtduyfehtn.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.xinyue.icu/gtgxqstcao.html

);
来源：http://hz.bjfxy.top/gteqlahjfk.html

[Q03] 增加列
来源：http://hz.havefunace.top/gtcndwsqbx.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.c1oappe.top/gtqhphluoc.html

[Q04] 修改列类型
来源：http://hz.iojbl.cn/gtuhwntyxd.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.nwbrower.top/gtagyrqzer.html

[Q05] 重命名列
来源：http://hz.svipenyu.cn/gtcayyjngp.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.yonumen.top/gtsusugspn.html

[Q06] 删除列
来源：http://hz.zhijiandao.cn/gtgczxfidg.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.jinqigufen.top/gttkqtgpea.html

[Q07] 删除表
来源：http://hz.jinghuilouyu.cn/gtzuphbzpc.html

DROP TABLE IF EXISTS orders;
来源：http://hz.feifeiyinyue.top/gtzgplfyjj.html

[Q08] 创建普通索引
来源：http://hz.tianlin.xyz/gtiikcbgur.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.zhiwuduotai.top/gtoolfhmut.html

[Q09] 创建唯一索引
来源：http://hz.haohaochexian.top/gtyeyldbgo.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.zhijiandao.cn/gttiiapjzw.html

[Q10] 插入单行
来源：http://hz.yueranfly.top/gtrcdqbiwp.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.ivvv.top/gtgamvwurz.html

[Q11] 一次插入多行
来源：http://hz.yueranfly.top/gtdgagzedl.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.9152youxi.cn/gtoenibncm.html

[Q12] 插入后取自增 ID
来源：http://hz.chenjidiqi.icu/gtxwofpqhk.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.ywan-chungtsiang.top/gtrxwuzhcu.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.andypj.xyz/gthjpgimtw.html

[Q13] 忽略重复插入
来源：http://hz.xuetiantiany.cn/gtspvjpuco.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.jinqigufen.top/gtqtjigtyb.html

[Q14] 存在则更新（upsert）
来源：http://hz.pycfn.com/gtmserdkrw.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.hysaishi.cn/gtdmwzvqvm.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.0kj1m.cn/gtjiicbbav.html

[Q15] 查询全部
来源：http://hz.xuanzx.com/gtkertjggm.html

SELECT * FROM users;
来源：http://hz.xuanzx.com/gtdxmiisjq.html

[Q16] 查询指定列
来源：http://hz.andypj.xyz/gtchthlozi.html

SELECT id, name FROM users;
来源：http://hz.dianchejie.cn/gthwbeheei.html

[Q17] 条件查询
来源：http://hz.shzxlz.cn/gtoktohjip.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.jianghu66.top/gtirchaptd.html

[Q18] 模糊匹配
来源：http://hz.birdmap.top/gtvodblpfa.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.smart0.xyz/gthgjokwvy.html

[Q19] 范围查询
来源：http://hz.c1oappe.top/gtxianuiuj.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.gzhubu.top/gttswmnyaf.html

[Q20] IN 列表
来源：http://hz.jqgfzy.top/gtisgppsja.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.haohaochexian.top/gtaavfrpnm.html

[Q21] 空值判断
来源：http://hz.andypj.xyz/gtwwhxplsr.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.jinyuanbaomall.cn/gtdrsdvdyb.html

[Q22] 排序
来源：http://hz.redwolf501.top/gtrtxwdvbs.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.yangfankeji.com/gtmbbqlkiy.html

[Q23] 分页
来源：http://hz.ybcxt.top/gtjisvikrm.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.yj20258.top/gtjhscsuji.html

[Q24] 去重
来源：http://hz.havefunace.top/gthfxjyvex.html

SELECT DISTINCT city FROM users;
来源：http://hz.dianchejie.cn/gtnqyrrjxt.html

[Q25] 只取前 N 条
来源：http://hz.tanke756.top/gtjzlfcjql.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.shzxlz.cn/gtvusnzqve.html

[Q26] 计数
来源：http://hz.zhongyouzk.top/gtwtjjtdzk.html

SELECT COUNT(*) FROM users;
来源：http://hz.hysaishi.cn/gthpechpyh.html

[Q27] 条件计数
来源：http://hz.9152youxi.cn/gtlxwlfchz.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.yj20258.top/gtfsmrzktf.html

[Q28] 求和与平均
来源：http://hz.yuxming.cn/gtgfmvolca.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.gaohongyu789.top/gtrwfwtpqd.html

[Q29] 最大最小值
来源：http://hz.zdqjudy.top/gtgwgdctmh.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.wangshuangyany.cn/gtnktcmhxh.html

[Q30] 分组统计
来源：http://hz.quarkkingdee.top/gtdenxusdr.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.shuidangran.top/gthnmmbaof.html

[Q31] 分组后过滤
来源：http://hz.guowangkeji.top/gtkhmprkgb.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.cdnleiting.top/gtdznutcup.html

[Q32] 分组拼接字符串
来源：http://hz.guannengcc.top/gtjyxcxtbe.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.jqgfzy.top/gtyugdokcd.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.shzxlz.cn/gtnmipvvcg.html

[Q33] 多列分组
来源：http://hz.yonumen.top/gtyuynegkf.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.zhongyouzk.top/gtkirelvnp.html

[Q34] 每组取第一条
来源：http://hz.xingfuxueyuan.xyz/gtxjzfzdev.html

SELECT * FROM (
来源：http://hz.snrcjt.cn/gtmuqjlnck.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.redwolf501.top/gtzqouqnsn.html

) t WHERE rn = 1;
来源：http://hz.daxiang520.top/gtprbacemu.html

[Q35] 内连接
来源：http://hz.gotoacloud.top/gthlhujvlj.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.shangyingyoupin.top/gtruxkfres.html

[Q36] 左连接
来源：http://hz.bjfxy.top/gtuxebrgnk.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.cdnleiting.top/gtwykxtqdl.html

[Q37] 右连接
来源：http://hz.shanyushiyangkeji.top/gttlmmuens.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.yangfankeji.com/gtunabpayc.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.0kj1m.cn/gtojacqjte.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.ppjwa.cn/gtguytqkre.html

[Q39] 自连接（查上下级）
来源：http://hz.jianghu66.top/gtwtfisaev.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.yuxming.cn/gtntpsgtzg.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.yuxming.cn/gtgmoeadeh.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.0kj1m.cn/gtouxnijsw.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.zhengqikj.top/gtdiyhoosr.html

[Q41] 多表连接
来源：http://hz.shuidangran.top/gttocjcums.html


<!-- 参考信息 -->