代发 wailian999

C#:   Array.BinarySearch(arr, x)
来源：http://hz.meibo888.top/gtuqniisdl.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.zhongyouzk.top/gtpmkreuzy.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.nanxinkj.top/gtmnpguwnn.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.yuxming.cn/gtcaxzndsy.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.dianchejie.cn/gtdaukmjqm.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.ybcxt.top/gtkpfjvbmk.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.yangfankeji.com/gttqeeqbwx.html

Go:   slices.Sort(arr)
来源：http://hz.hywenlv.cn/gtfegzhgzb.html

Ruby: arr.sort
来源：http://hz.yj202588.top/gtawlqaaeg.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.andypj.xyz/gtdmeiglan.html

[N03] 快速排序（分治示例）
来源：http://hz.shuidangran.top/gtjrcxxnhk.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.guowangkeji.top/gtxffpoamd.html

PHP:  // 递归实现，或用 usort
来源：http://hz.hnxiangtu.top/gtesloeqht.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.meibo888.top/gtmrngnirz.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.pengpengdd.cyou/gtvmgmhciz.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.hnqzz.top/gtoltatohg.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.jinyuanbaomall.cn/gtqmkbfrim.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.hongshengwenyu.top/gtkpfjnuwu.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.sxryk.cn/gtjobljuhz.html

[N04] 斐波那契数列
来源：http://hz.xuetiantiany.cn/gtxierrzdl.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.jinyuanbaomall.cn/gtwrbqzdue.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.pengpengdd.cyou/gteavqlcpj.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.chenlongwang.top/gtwnixvxix.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.zhiwuduotai.top/gtddlofhxf.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.sysykeji.top/gtfdeqyzgh.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.ppjwa.cn/gtzpuzawqr.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.tianlin.xyz/gtrqefxyze.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.guowangkeji.top/gtfyigaloe.html

[N05] 最大公约数
来源：http://hz.daria6918.cn/gttlneokrx.html

Py:   math.gcd(a, b)
来源：http://hz.andypj.xyz/gtjuzclcgp.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.hfpthk.cn/gtqyilnrvo.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.guowangkeji.top/gtwuoptova.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.daxiang520.top/gtkppyhcmm.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.hongshengwenyu.top/gtvseouxad.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.daria6918.cn/gtluttlbut.html

Ruby: a.gcd(b)
来源：http://hz.yueranfly.top/gtuogqrlob.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.gotoacloud.top/gtwojakgax.html

[N06] 判断回文字符串
来源：http://hz.birdmap.top/gtgonrmexy.html

Py:   s == s[::-1]
来源：http://hz.cheryme.top/gtgauwltjd.html

PHP:  $s === strrev($s);
来源：http://hz.0kj1m.cn/gtbqrojqbo.html

JS:   s === [...s].reverse().join("")
来源：http://hz.c1oappe.top/gtwcbnwxaq.html

TS:   s === [...s].reverse().join("")
来源：http://hz.hnxiangtu.top/gteguupouk.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.zhijiandao.cn/gtwimhghok.html

Go:   // 双指针从两端比较
来源：http://hz.meibo888.top/gtslunkubo.html

Ruby: s == s.reverse
来源：http://hz.fengsongda.top/gtaxzgnfld.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.hammf.cn/gtbxaukrdz.html

[N07] 两数之和（返回下标）
来源：http://hz.hnqzz.top/gtqqynoask.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.kuanghao11.cn/gtjpovnyng.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.chenlongwang.top/gtyujubuua.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.xylfe.cn/gtrolgoihx.html

TS:   // 手写 Map<string, number>
来源：http://hz.hongshengwenyu.top/gtpzcepehb.html

Java: // 手写 HashMap
来源：http://hz.zhiwuduotai.top/gthfbhamkx.html

Go:   // 手写 map[int]int
来源：http://hz.xziqi.cn/gtzlpubhxn.html

Ruby: // 手写 Hash
来源：http://hz.iojbl.cn/gtxghzpqme.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.jiagoushi.top/gtdvcurxga.html

[N08] 生成全排列
来源：http://hz.xuetiantiany.cn/gtyzxgpehw.html

Py:   itertools.permutations(arr)
来源：http://hz.bjfxy.top/gtiemluvsq.html

PHP:  // 手写递归交换
来源：http://hz.yj20258.top/gtwxjsjnvp.html

JS:   // 手写回溯递归
来源：http://hz.ehwqpu.com/gtaqmouslz.html

TS:   // 手写回溯递归
来源：http://hz.xinyue.icu/gtwqxzfwrt.html

Java: // 手写回溯递归
来源：http://hz.yanxiufei.cn/gtcobhagjv.html

Go:   // 手写回溯递归
来源：http://hz.jlsjyb.cn/gtpkmyfxoq.html

Ruby: arr.permutation.to_a
来源：http://hz.9152youxi.cn/gtzblxszgq.html

C#:   // 手写回溯递归
来源：http://hz.shanyushiyangkeji.top/gtbcltvnrb.html

[N09] 栈与队列
来源：http://hz.vqdsnc.cn/gtubtdybrr.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.birdmap.top/gtvrtglasr.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.xuetiantiany.cn/gtmvasguxb.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.zhoulong.xyz/gtkvdkbjqu.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.9152youxi.cn/gtxqdqtarx.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.daria6918.cn/gthnzrkzmf.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.pycfn.com/gtfxqzpsuf.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.jianghu66.top/gtauktefbh.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.zhijiandao.cn/gtuzplhhmg.html

[N10] 链表节点定义
来源：http://hz.hfpthk.cn/gtqqukhelj.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.dashuyun.cn/gtbijgdbkl.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.yongpay.top/gtybheeurh.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.zhaomingkeji.xyz/gtrfslmcqp.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.hongshengwenyu.top/gtocvxdbwv.html

Java: class Node { int v; Node next; }
来源：http://hz.vqdsnc.cn/gtyquowcda.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.haohaochexian.top/gtpeqlyygj.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.zhongyouzk.top/gtdhojgwfv.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.ybcxt.top/gttkfcqihq.html

[N11] 二叉树中序遍历
来源：http://hz.cashguo.top/gtqrctodnw.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.52xcode.cn/gtmhkpysku.html

PHP:  // 手写递归函数
来源：http://hz.havefunace.top/gtzcdqijmw.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.pengpengdd.cyou/gtyrikucnj.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.iojbl.cn/gtwectoinh.html

Java: // 手写递归
来源：http://hz.jlsjyb.cn/gtivemlqkl.html

Go:   // 手写递归
来源：http://hz.xuetiantiany.cn/gtyiqjtbik.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.jiagoushi.top/gtsghzihji.html

C#:   // 手写递归
来源：http://hz.zhongyouzk.top/gtgasvlico.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.xuetiantiany.cn/gtfkyullqh.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.xziqi.cn/gtdyaapjmp.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.gotoacloud.top/gtwqaedewd.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.xziqi.cn/gtucvnsvpt.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.tian-w.cn/gtguzqibpf.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.sufxvd.cn/gtngkkrjql.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.hywenlv.cn/gtqniofzue.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.zdqjudy.top/gtrsluquvg.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.shuidangran.top/gtjivprssa.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtszrwvlpz.html

O. 并发与异步
来源：http://hz.pengpengdd.cyou/gtopczqzke.html

================================================================================
来源：http://hz.chenzaomai.com/gtpyhghydh.html

[O01] 启动一个线程
来源：http://hz.mhx1999.top/gtfaugrrpn.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.aibaodan.cn/gtguumkwnt.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.hongshengwenyu.top/gtyqjwcsie.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.hysaishi.cn/gtflwnyapk.html

TS:   // 同 JS
来源：http://hz.zycfv.cn/gtwgrahdar.html

Java: new Thread(() -> f()).start()
来源：http://hz.chenlongwang.top/gtvcyeuyuv.html

Go:   go f()
来源：http://hz.cdnleiting.top/gtwmacwaan.html

Ruby: Thread.new { f }
来源：http://hz.zhoulong.xyz/gtjxerfxgt.html

C#:   Task.Run(() => F());
来源：http://hz.ybcxt.top/gtaimnicee.html

[O02] 使用线程池
来源：http://hz.zhongyouzk.top/gtelahxhnr.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.zhijiandao.cn/gtqpegllla.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.cqqwz.cn/gtvrcgisdk.html

JS:   // worker_threads 线程池
来源：http://hz.yonumen.top/gtqgysjsjc.html

TS:   // worker_threads 线程池
来源：http://hz.hnqzz.top/gtnyojflgr.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.havefunace.top/gtjqhmyhgf.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.gaohongyu789.top/gtdudjnxvr.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.hywenlv.cn/gtoqbgguux.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.hfpthk.cn/gttiragpfn.html

[O03] 加锁保护共享数据
来源：http://hz.wangshuangyany.cn/gtgnemuhgl.html

Py:   with lock: shared += 1
来源：http://hz.chenzaomai.com/gtgqmrtylw.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.xuetiantiany.cn/gtoeanzkde.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.nanxinkj.top/gtdimbvlxo.html

TS:   // 同 JS
来源：http://hz.nanxuanxn.top/gtnouwkwaa.html

Java: synchronized (this) { shared++; }
来源：http://hz.chenjidiqi.icu/gtkxfzlgwh.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.9152youxi.cn/gtdjnizeaj.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.hnxiangtu.top/gtpwxkbpaf.html

C#:   lock (gate) { shared++; }
来源：http://hz.gotoacloud.top/gtorjctpwb.html

[O04] 定义异步函数并等待
来源：http://hz.dianchejie.cn/gtugybpnqz.html

Py:   async def f():⏎    await g()
来源：http://hz.tianlin.xyz/gtxwtyttno.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.yangfankeji.com/gtubqrsnko.html

JS:   async function f() { await g(); }
来源：http://hz.0kj1m.cn/gtaxrddynw.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.ydjk.org.cn/gtnkmfmfcy.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.cqqwz.cn/gtagasagbx.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.jqgufenzy.top/gtnxhslohq.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.hammf.cn/gtvvdkcyna.html

C#:   async Task F() { await G(); }
来源：http://hz.nanxuanxn.top/gtxdpsrhsw.html

[O05] 并发执行并等待全部完成
来源：http://hz.ydzc1.top/gtoxwaposz.html

Py:   asyncio.gather(*tasks)
来源：http://hz.tian-w.cn/gtjtsgpdxi.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.zhaomingkeji.xyz/gtiiondzve.html

JS:   await Promise.all(tasks)
来源：http://hz.wangdashe.top/gthbpyzssl.html

TS:   await Promise.all(tasks)
来源：http://hz.havefunace.top/gtcvepixln.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.fengsongda.top/gtayfacryx.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.yangfankeji.com/gtmiwimmza.html

Ruby: threads.map(&:join)
来源：http://hz.shuidangran.top/gtthxnxzyw.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.hfpthk.cn/gtnyysftck.html

[O06] 使用进程池
来源：http://hz.gaohongyu789.top/gtbndkcllo.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.kuanghao11.cn/gtffwpmjla.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.xuetiantiany.cn/gtliumfphy.html

JS:   // child_process / cluster 模块
来源：http://hz.sysykeji.top/gtgramkckl.html

TS:   // child_process / cluster 模块
来源：http://hz.ehwqpu.com/gtqzqcpeay.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.zhongyouzk.top/gtarooxdci.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.andypj.xyz/gtryudpzkt.html

Ruby: // fork 块
来源：http://hz.hnqzz.top/gtorpppaxz.html

C#:   Parallel.For
来源：http://hz.yj20258.top/gtbvchssid.html

================================================================================
来源：http://hz.jqgufenzy.top/gtcknxlcyp.html

P. 常用工具函数
来源：http://hz.shanyushiyangtech.top/gteoftpvqs.html

================================================================================
来源：http://hz.zhengqikj.top/gtadzdcfhh.html

[P01] 生成 UUID
来源：http://hz.daria6918.cn/gtcvvbnvjx.html

Py:   str(uuid.uuid4())
来源：http://hz.jqgufenzy.top/gtskohzjii.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.haohaochexian.top/gtznovryoi.html

JS:   crypto.randomUUID()
来源：http://hz.yueranfly.top/gtaedsabwf.html

TS:   crypto.randomUUID()
来源：http://hz.cucudq.cn/gtbikufqhk.html

Java: UUID.randomUUID().toString()
来源：http://hz.ppjwa.cn/gttlwknffe.html

Go:   // 用 github.com/google/uuid
来源：http://hz.nanxuanxn.top/gtiqknmoik.html

Ruby: SecureRandom.uuid
来源：http://hz.snrcjt.cn/gtugzuuosp.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.zhiwuduotai.top/gtqugmzzcq.html

[P02] MD5 / SHA256 摘要
来源：http://hz.ydjk.org.cn/gthihnuvvb.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.ppjwa.cn/gtrwhwibjd.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.chenlongwang.top/gtpmdonulp.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.andypj.xyz/gtshrbtltw.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.ybcxt.top/gtioqbyqdl.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.redwolf501.top/gtbhxnydet.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.feifeiyinyue.top/gtufjddmva.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.cdnleiting.top/gthginxaqm.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.svipenyu.cn/gteugvmpxm.html

[P03] 生成短随机字符串
来源：http://hz.feifeiyinyue.top/gtihfhhuoy.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.ybcxt.top/gtwnrwdyhm.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.sxryk.cn/gteafvtmgc.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.cqqwz.cn/gtnrpfdqbq.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.jinghuilouyu.cn/gtffyscnjs.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.yuanzhike.top/gtzzyvencr.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.cucudq.cn/gtkghxzaty.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.cdnleiting.top/gtvomrejwp.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.dianchejie.cn/gtwnvhoudj.html

[P04] 求长度
来源：http://hz.tian-w.cn/gtujbypxaz.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.zhengqikj.top/gtaeehnqau.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.chenzaomai.com/gteggxmege.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.zycfv.cn/gtphxupazj.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.feifeiyinyue.top/gtrelohljp.html

Java: list.size();  map.size();  s.length()
来源：http://hz.zhaomingkeji.xyz/gtjfdmpqwv.html

Go:   len(arr);  len(m)
来源：http://hz.guowangkeji.top/gtoswyrihp.html

Ruby: x.length;  x.size
来源：http://hz.jinyuanbaomall.cn/gtlwkclema.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.zhongyouzk.top/gtlrqjtygx.html

[P05] 判断两个对象内容是否相等
来源：http://hz.wangdashe.top/gtahsjjmbo.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.haohaochexian.top/gtjuqfzrwn.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.jyoumei.cn/gtiqzpracn.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.wangdashe.top/gtzfxswwzj.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.ybcxt.top/gtrqivyptu.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.daria6918.cn/gtqmhyzxre.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.0kj1m.cn/gtgqkiwvqz.html

Ruby: a == b
来源：http://hz.jinghuilouyu.cn/gtkfggoerr.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.birdmap.top/gttzqgswyf.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.sweek.top/gtbmxepaco.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.cashguo.top/gtjsbtjroa.html

PHP:  if (empty($x)) {}
来源：http://hz.vqdsnc.cn/gthgxlnusc.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.haohaochexian.top/gtqozbzhoi.html

TS:   if (x == null) {}
来源：http://hz.fzhhl.top/gtzsqbctps.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.vqdsnc.cn/gtwjvguvpe.html

Go:   if x == nil {}
来源：http://hz.hammf.cn/gtiugjskcy.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.sysykeji.top/gtzfizvpds.html

C#:   if (x is null) {}
来源：http://hz.jiagoushi.top/gtthplfkur.html

[P07] 防抖与节流
来源：http://hz.yj202588.top/gtnuosobfy.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.ehwqpu.com/gtclatjsaj.html

PHP:  // 手写时间戳比较
来源：http://hz.pengpengdd.cyou/gtqujwmweq.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.cashguo.top/gtamnaaxom.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.redwolf501.top/gtoqeytmva.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.c1oappe.top/gtcejqovfa.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.sysykeji.top/gtquouyfet.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.jinghuilouyu.cn/gtueoyiohr.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.gzhubu.top/gtkpibphuj.html

[P08] 处理浮点精度问题
来源：http://hz.dashuyun.cn/gtibhodawt.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.nanxinkj.top/gtezyyugka.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.zycfv.cn/gtbnciugdc.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.zycfv.cn/gtnhfreesy.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.jqgufenzy.top/gtnturcval.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.fengsongda.top/gtfifvrljc.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.yj20258.top/gtgdzhhdbx.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.cheryme.top/gtahxbtpcr.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.zycfv.cn/gtucwrxdcl.html

================================================================================
来源：http://hz.redwolf501.top/gtlxqmbujn.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.hysaishi.cn/gtkvxyaerf.html

================================================================================
来源：http://hz.ppjwa.cn/gtmgjfieti.html

[Q01] 创建表
来源：http://hz.shanyushiyangkeji.top/gteybkayov.html

CREATE TABLE users (
来源：http://hz.yangfankeji.com/gtyomiifgq.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.shanyushiyangtech.top/gtwzlmyoec.html

name VARCHAR(50) NOT NULL,
来源：http://hz.zhixingplan.top/gtgtzwyghk.html

email VARCHAR(100) UNIQUE,
来源：http://hz.hammf.cn/gtlaeyftrp.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.hnxiangtu.top/gtwgozxvap.html

);
来源：http://hz.jqgufenzy.top/gtgdcaebpr.html

[Q02] 创建带外键的表
来源：http://hz.jinghuilouyu.cn/gtloikhzpx.html

CREATE TABLE orders (
来源：http://hz.tianlin.xyz/gtzfdbckae.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.shzxlz.cn/gtndkffndr.html

user_id INT NOT NULL,
来源：http://hz.cdnleiting.top/gtydpgkytf.html

amount DECIMAL(10, 2),
来源：http://hz.xylfe.cn/gtzznysxpl.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.meibo888.top/gtyfygcgyj.html

);
来源：http://hz.shzxlz.cn/gtmjqxqaeu.html

[Q03] 增加列
来源：http://hz.yangfankeji.com/gtlgrjsvbr.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.sufxvd.cn/gtqcneyahx.html

[Q04] 修改列类型
来源：http://hz.fengsongda.top/gtbcqweevv.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.gotoacloud.top/gtpsixhrct.html

[Q05] 重命名列
来源：http://hz.nanxinkj.top/gtdbparykv.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.ppjwa.cn/gtuvqceudd.html

[Q06] 删除列
来源：http://hz.shanyushiyangkeji.top/gtlqvttajg.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.jinyuanbaomall.cn/gtchngcgbb.html

[Q07] 删除表
来源：http://hz.gzhubu.top/gtheqvlrhd.html

DROP TABLE IF EXISTS orders;
来源：http://hz.hnqzz.top/gtbmzczcui.html

[Q08] 创建普通索引
来源：http://hz.birdmap.top/gtqitdyblr.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.fzhhl.top/gttbjcrxml.html

[Q09] 创建唯一索引
来源：http://hz.chenjidiqi.icu/gtkaxcfzxb.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.wangdashe.top/gtfylcckrg.html

[Q10] 插入单行
来源：http://hz.jqgufenzy.top/gtmorqugme.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.tian-w.cn/gtsnjszgxd.html

[Q11] 一次插入多行
来源：http://hz.jinqigfzy.top/gtotjambuy.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.quarkkingdee.top/gtfdxceqvf.html

[Q12] 插入后取自增 ID
来源：http://hz.dashuyun.cn/gtrbyzvgen.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.yj202588.top/gtxmhulezw.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.jianghu66.top/gtwmiqnztd.html

[Q13] 忽略重复插入
来源：http://hz.hysaishi.cn/gtoojhgylg.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.guowangkeji.top/gtgdyxhjdo.html

[Q14] 存在则更新（upsert）
来源：http://hz.feifeiyinyue.top/gtilaojtbk.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.hnqzz.top/gtyrarguqj.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.tanke756.top/gtbdusxfqn.html

[Q15] 查询全部
来源：http://hz.pycfn.com/gtmzqrynrh.html

SELECT * FROM users;
来源：http://hz.ywan-chungtsiang.top/gtmzlsjvop.html

[Q16] 查询指定列
来源：http://hz.316326.xyz/gtseqrzvrc.html

SELECT id, name FROM users;
来源：http://hz.vqdsnc.cn/gtubbdqzsg.html

[Q17] 条件查询
来源：http://hz.hnxiangtu.top/gtfxdvgyjz.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.mhx1999.top/gtsezycyuc.html

[Q18] 模糊匹配
来源：http://hz.chenlongwang.top/gtvalcccoy.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.fzhhl.top/gteotmzrqq.html

[Q19] 范围查询
来源：http://hz.xuanzx.com/gttrnicbvj.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.0kj1m.cn/gtggjbidpb.html

[Q20] IN 列表
来源：http://hz.yonumen.top/gtzzjlvfqn.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.hysaishi.cn/gtlquutbku.html

[Q21] 空值判断
来源：http://hz.ywan-chungtsiang.top/gtzoqzpwgl.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.iojbl.cn/gtzzsiqazq.html

[Q22] 排序
来源：http://hz.sweek.top/gtdqeyemdx.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.shzxlz.cn/gtsxeoverv.html

[Q23] 分页
来源：http://hz.daria6918.cn/gtytzllsho.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.sweek.top/gtvnrbagsw.html

[Q24] 去重
来源：http://hz.kuanghao11.cn/gtjqlrmoje.html

SELECT DISTINCT city FROM users;
来源：http://hz.jinyuanbaomall.cn/gtxckojpxe.html

[Q25] 只取前 N 条
来源：http://hz.dashuyun.cn/gtrutubqwk.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.chenjidiqi.icu/gtydxajjql.html

[Q26] 计数
来源：http://hz.shuidangran.top/gtleyozbep.html

SELECT COUNT(*) FROM users;
来源：http://hz.yvedp.cn/gtdewomkyc.html

[Q27] 条件计数
来源：http://hz.9152youxi.cn/gtakjnmesb.html


<!-- 参考信息 -->