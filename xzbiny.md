代发 wailian999

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.sufxvd.cn/gtkoxbipeo.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.aizwys.cn/gtretcshyw.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.andypj.xyz/gtuotvbfbi.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.zhaomingkeji.xyz/gtvemmzusl.html

[N05] 最大公约数
来源：http://hz.ybcxt.top/gtodbqfljw.html

Py:   math.gcd(a, b)
来源：http://hz.shuidangran.top/gtpkjbaxon.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.hywenlv.cn/gtciryqbjk.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.ybcxt.top/gtfanhmvlx.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.hysaishi.cn/gtzibbfqln.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.dianchejie.cn/gtlcdugctu.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.quarkkingdee.top/gtdvzrkxvl.html

Ruby: a.gcd(b)
来源：http://hz.yj20258888.top/gtanjankqd.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.zhiwuduotai.top/gtfpmrugax.html

[N06] 判断回文字符串
来源：http://hz.fengsongda.top/gtsywmglyp.html

Py:   s == s[::-1]
来源：http://hz.jiagoushi.top/gtsmzcaroi.html

PHP:  $s === strrev($s);
来源：http://hz.hfpthk.cn/gtszbytiks.html

JS:   s === [...s].reverse().join("")
来源：http://hz.shuidangran.top/gtcixnpxil.html

TS:   s === [...s].reverse().join("")
来源：http://hz.jqgfzy.top/gtxwnppwuo.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.wangdashe.top/gtydgneqki.html

Go:   // 双指针从两端比较
来源：http://hz.ydzc1.top/gtkzhvzeyu.html

Ruby: s == s.reverse
来源：http://hz.sweek.top/gtweroxmrp.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.andypj.xyz/gtpobrseye.html

[N07] 两数之和（返回下标）
来源：http://hz.zhiwuduotai.top/gtlfaneqtn.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.dianchejie.cn/gthcrkrwrs.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.jianghu66.top/gtpyohimky.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.jinyuanbaomall.cn/gteerlmvvw.html

TS:   // 手写 Map<string, number>
来源：http://hz.xingfuxueyuan.xyz/gtfomwmlph.html

Java: // 手写 HashMap
来源：http://hz.kuanghao11.cn/gtzilyyvsf.html

Go:   // 手写 map[int]int
来源：http://hz.yonumen.top/gtyshcknis.html

Ruby: // 手写 Hash
来源：http://hz.bjfxy.top/gtjhfqypnc.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.sweek.top/gtucotjylu.html

[N08] 生成全排列
来源：http://hz.daxiang520.top/gtmasmkaqt.html

Py:   itertools.permutations(arr)
来源：http://hz.yanxiufei.cn/gtuuahwidh.html

PHP:  // 手写递归交换
来源：http://hz.dashuyun.cn/gtdibtetcp.html

JS:   // 手写回溯递归
来源：http://hz.hnxiangtu.top/gtkejkusap.html

TS:   // 手写回溯递归
来源：http://hz.ywan-chungtsiang.top/gtfjsndrfs.html

Java: // 手写回溯递归
来源：http://hz.yonumen.top/gtrhvnxnyz.html

Go:   // 手写回溯递归
来源：http://hz.ehwqpu.com/gtwqzxdpzf.html

Ruby: arr.permutation.to_a
来源：http://hz.gotoacloud.top/gtnbphcddg.html

C#:   // 手写回溯递归
来源：http://hz.shanyushiyangtech.top/gtjpznqjto.html

[N09] 栈与队列
来源：http://hz.fengsongda.top/gtksuambfg.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.zycfv.cn/gtxhfvayga.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.nanxuanxn.top/gtnhstpydf.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.yueranfly.top/gtqzswyyha.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.ivvv.top/gtvsabletk.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.yuanzhike.top/gtjhwoziml.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.xuetiantiany.cn/gtzkyhcmfc.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.zhijiandao.cn/gteqiffteh.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.sufxvd.cn/gttliczqzt.html

[N10] 链表节点定义
来源：http://hz.zhaomingkeji.xyz/gtukybpmbq.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.52xcode.cn/gtfuzgdqry.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.wangshuangyany.cn/gtyzynqold.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.jinqigufen.top/gtwitdpoyh.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.bjfxy.top/gtsxdmosjf.html

Java: class Node { int v; Node next; }
来源：http://hz.hammf.cn/gtufpfdztj.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.birdmap.top/gtymdthwsw.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.ivvv.top/gttzzobgme.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.fzhhl.top/gtwgidgeqh.html

[N11] 二叉树中序遍历
来源：http://hz.c1oappe.top/gtoxqiaddx.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.cdnleiting.top/gteznvneso.html

PHP:  // 手写递归函数
来源：http://hz.shzxlz.cn/gtojwixbyy.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.cheryme.top/gtfamoddsw.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.xinyue.icu/gtqerohtcp.html

Java: // 手写递归
来源：http://hz.sxryk.cn/gtkiorodyh.html

Go:   // 手写递归
来源：http://hz.chenzaomai.com/gtvymzrprm.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.0kj1m.cn/gtzzwolxas.html

C#:   // 手写递归
来源：http://hz.fengsongda.top/gtzfrpkhdl.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.sysykeji.top/gtximegfjt.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.yj202588.top/gtqfpqrmgv.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.daxiang520.top/gtikqppyex.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.zhixingplan.top/gtdekwqitv.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.tianlin.xyz/gtcudpzeut.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.xylfe.cn/gtohhevkja.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.zdqjudy.top/gtlywihyaw.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.shangyingyoupin.top/gthqfgbwgt.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.gaohongyu789.top/gtarahlflt.html

================================================================================
来源：http://hz.gaohongyu789.top/gtefvgjoiz.html

O. 并发与异步
来源：http://hz.chenzaomai.com/gtrcutihnt.html

================================================================================
来源：http://hz.zhongyouzk.top/gtqaeezelx.html

[O01] 启动一个线程
来源：http://hz.cucudq.cn/gtwvyjfjto.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.gzhubu.top/gtenqtmwse.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.shzxlz.cn/gtuakikgek.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.nanxinkj.top/gtaztvxame.html

TS:   // 同 JS
来源：http://hz.zhiwuduotai.top/gtejdjicuz.html

Java: new Thread(() -> f()).start()
来源：http://hz.zhaomingkeji.xyz/gtbawlqdol.html

Go:   go f()
来源：http://hz.zhoulong.xyz/gttovdrqed.html

Ruby: Thread.new { f }
来源：http://hz.tian-w.cn/gtvxwncchh.html

C#:   Task.Run(() => F());
来源：http://hz.hongshengwenyu.top/gtujsivqvi.html

[O02] 使用线程池
来源：http://hz.jinqigfzy.top/gtraybdrde.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.zhoulong.xyz/gtabzsxwhl.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.yj20258.top/gtxryfdvhn.html

JS:   // worker_threads 线程池
来源：http://hz.gotoacloud.top/gtbgmrvqts.html

TS:   // worker_threads 线程池
来源：http://hz.jqgufenzy.top/gtpydbzqnh.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.haohaochexian.top/gtorqphyks.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.xziqi.cn/gtzmbinlzf.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.aizwys.cn/gtbzjiznjs.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.haohaochexian.top/gtcozkagqa.html

[O03] 加锁保护共享数据
来源：http://hz.dashuyun.cn/gtjkhibvqu.html

Py:   with lock: shared += 1
来源：http://hz.guannengcc.top/gttqvttcyy.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.nanxuanxn.top/gtihzttudm.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.c1oappe.top/gthfqluoae.html

TS:   // 同 JS
来源：http://hz.nanxinkj.top/gtgjppojuz.html

Java: synchronized (this) { shared++; }
来源：http://hz.hnqzz.top/gtdiwwirub.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.hysaishi.cn/gtyvexcwmi.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.dashuyun.cn/gtvqzrxoxg.html

C#:   lock (gate) { shared++; }
来源：http://hz.52xcode.cn/gtjmbwvmlk.html

[O04] 定义异步函数并等待
来源：http://hz.pycfn.com/gtjhndvcsx.html

Py:   async def f():⏎    await g()
来源：http://hz.yuxming.cn/gtkgokuyei.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.jianghu66.top/gtomsgamhj.html

JS:   async function f() { await g(); }
来源：http://hz.aizwys.cn/gtqfizxyxk.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.zdqjudy.top/gtatijjwao.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.hysaishi.cn/gtgrelvuou.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.316326.xyz/gtushlvagf.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.sufxvd.cn/gtwrzwkonh.html

C#:   async Task F() { await G(); }
来源：http://hz.sufxvd.cn/gtfrmqgiie.html

[O05] 并发执行并等待全部完成
来源：http://hz.pengpengdd.cyou/gtjpcbmlxk.html

Py:   asyncio.gather(*tasks)
来源：http://hz.jinyuanbaomall.cn/gtiycfqzrn.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.hnxiangtu.top/gtrhicmrnw.html

JS:   await Promise.all(tasks)
来源：http://hz.hfpthk.cn/gtsinjwrrg.html

TS:   await Promise.all(tasks)
来源：http://hz.cucudq.cn/gtvqvkbrlu.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.sysykeji.top/gtscoergnj.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.dianchejie.cn/gthuwrmkfk.html

Ruby: threads.map(&:join)
来源：http://hz.jyoumei.cn/gtlazxzwim.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.gzhubu.top/gtfappeeza.html

[O06] 使用进程池
来源：http://hz.zycfv.cn/gthbkansyh.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.dianchejie.cn/gtcisvlmtm.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.52xcode.cn/gtgjzkzxwu.html

JS:   // child_process / cluster 模块
来源：http://hz.guowangkeji.top/gtvdgqvkrf.html

TS:   // child_process / cluster 模块
来源：http://hz.chenjidiqi.icu/gtysdahbsk.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.ydzc1.top/gtckrghpuo.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.hnxiangtu.top/gtnmgvezsh.html

Ruby: // fork 块
来源：http://hz.yueranfly.top/gthtgkmahd.html

C#:   Parallel.For
来源：http://hz.cheryme.top/gthggsnfgv.html

================================================================================
来源：http://hz.316326.xyz/gtjgexttmj.html

P. 常用工具函数
来源：http://hz.pycfn.com/gtsnvgohsc.html

================================================================================
来源：http://hz.jiagoushi.top/gtroxeretw.html

[P01] 生成 UUID
来源：http://hz.iojbl.cn/gtupzpxlzy.html

Py:   str(uuid.uuid4())
来源：http://hz.gogol.net.cn/gttrekvruu.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.gaohongyu789.top/gtuxqidxzd.html

JS:   crypto.randomUUID()
来源：http://hz.ywan-chungtsiang.top/gtmgchaexi.html

TS:   crypto.randomUUID()
来源：http://hz.9152youxi.cn/gthsqfdiad.html

Java: UUID.randomUUID().toString()
来源：http://hz.shanyushiyangtech.top/gtjyudyobd.html

Go:   // 用 github.com/google/uuid
来源：http://hz.cucudq.cn/gtbtpvhmws.html

Ruby: SecureRandom.uuid
来源：http://hz.cashguo.top/gtlxwapplu.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.52xcode.cn/gtkwnizuym.html

[P02] MD5 / SHA256 摘要
来源：http://hz.ehwqpu.com/gtumlxpwkz.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.havefunace.top/gtliqgpkps.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.xinyue.icu/gtgrhtmmzl.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.sxryk.cn/gtyviedpnn.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.pengpengdd.cyou/gtilayupae.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.zhoulong.xyz/gtuiejzfew.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.meibo888.top/gtaqmrmnyf.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.svipenyu.cn/gttjuwdthi.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.yangfankeji.com/gtjvfgldog.html

[P03] 生成短随机字符串
来源：http://hz.chenlongwang.top/gtvomyhhbm.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.shuidangran.top/gtrdgofsog.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.nanxinkj.top/gtlfigtxdz.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.xylfe.cn/gtwqfiecbw.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.guannengcc.top/gtdilhsoez.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.yongpay.top/gtzkfrbwqa.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.daxiang520.top/gtxjvrcran.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.yonumen.top/gtuamsbtmg.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.jqgufenzy.top/gtuvhdjxdg.html

[P04] 求长度
来源：http://hz.hysaishi.cn/gtxdebndhm.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.nanxuanxn.top/gtqrbbzuqi.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.redwolf501.top/gtchuqvovk.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.snrcjt.cn/gtmnvzdvgu.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.kuanghao11.cn/gtdbpmvsgx.html

Java: list.size();  map.size();  s.length()
来源：http://hz.yonumen.top/gtsmckawnj.html

Go:   len(arr);  len(m)
来源：http://hz.fengsongda.top/gtlrydpypz.html

Ruby: x.length;  x.size
来源：http://hz.hammf.cn/gtiuzrxdfw.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.kuanghao11.cn/gtbterqzjp.html

[P05] 判断两个对象内容是否相等
来源：http://hz.daria6918.cn/gtgnnmckyv.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.dianchejie.cn/gtqkbmyxtf.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.ydzc1.top/gtcgpqbhoa.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.fzhhl.top/gtzqertskp.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.xingfuxueyuan.xyz/gtassyhezj.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.chenlongwang.top/gtfsezgfll.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.yj202588.top/gtysgbwgzk.html

Ruby: a == b
来源：http://hz.meibo888.top/gtjiezvodw.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.andypj.xyz/gtqooqetsb.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.hammf.cn/gterwtajat.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.chenjidiqi.icu/gtvfkestxq.html

PHP:  if (empty($x)) {}
来源：http://hz.feifeiyinyue.top/gtvtrehfkt.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.yuanzhike.top/gtuxecyxda.html

TS:   if (x == null) {}
来源：http://hz.jinqigfzy.top/gthoigjlys.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.hnqzz.top/gteqzfbwby.html

Go:   if x == nil {}
来源：http://hz.nanxuanxn.top/gtpemqxyoc.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.cdnleiting.top/gtgpdzpjlk.html

C#:   if (x is null) {}
来源：http://hz.aibaodan.cn/gtngiodldz.html

[P07] 防抖与节流
来源：http://hz.52xcode.cn/gtnxwwjeuo.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.shangyingyoupin.top/gtqfldsvmt.html

PHP:  // 手写时间戳比较
来源：http://hz.feifeiyinyue.top/gtbqglsodw.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.zhixingplan.top/gtoupebqrd.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.ywan-chungtsiang.top/gtjbtntlol.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.daxiang520.top/gtsxnlntkg.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.iojbl.cn/gtssijmegp.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.shangyingyoupin.top/gtpnipqzbn.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.gotoacloud.top/gtahszqake.html

[P08] 处理浮点精度问题
来源：http://hz.yvedp.cn/gtwjauxlac.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.vqdsnc.cn/gtgyozgftz.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.zhiwuduotai.top/gtwridytkp.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.ydzc1.top/gthlhrslfx.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.gogol.net.cn/gthrgivseq.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.zhixingplan.top/gtnewyergh.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.jyoumei.cn/gtolxpgtsy.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.cheryme.top/gtrbgkjypd.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.nanxinkj.top/gtfavkhhsw.html

================================================================================
来源：http://hz.cheryme.top/gtredvhkdo.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.kuanghao11.cn/gtrzxiyzrt.html

================================================================================
来源：http://hz.yanxiufei.cn/gtmqyncgse.html

[Q01] 创建表
来源：http://hz.yangfankeji.com/gtignrokrd.html

CREATE TABLE users (
来源：http://hz.yangfankeji.com/gtndlvvsno.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.zdqjudy.top/gtjdyxefjy.html

name VARCHAR(50) NOT NULL,
来源：http://hz.xylfe.cn/gtbdvnhbjg.html

email VARCHAR(100) UNIQUE,
来源：http://hz.chenlongwang.top/gtocfsbdba.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.smart0.xyz/gtujxxjtpg.html

);
来源：http://hz.yj20258.top/gtirjmtetp.html

[Q02] 创建带外键的表
来源：http://hz.xuetiantiany.cn/gtxsvkmjzy.html

CREATE TABLE orders (
来源：http://hz.nwbrower.top/gtzwnxuyms.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.yj20258888.top/gtlhdvcpgt.html

user_id INT NOT NULL,
来源：http://hz.sysykeji.top/gtirwdypwk.html

amount DECIMAL(10, 2),
来源：http://hz.feifeiyinyue.top/gtcngphfvm.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.dianchejie.cn/gtmxivacsf.html

);
来源：http://hz.guannengcc.top/gtqyuqwegv.html

[Q03] 增加列
来源：http://hz.wangshuangyany.cn/gtdqsfjbkk.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.xziqi.cn/gtzybcytba.html

[Q04] 修改列类型
来源：http://hz.fengsongda.top/gtmlcrwfer.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.jinyuanbaomall.cn/gtxtlxjxoh.html

[Q05] 重命名列
来源：http://hz.yvedp.cn/gtbgkyyewn.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.dianchejie.cn/gtwkigtyqh.html

[Q06] 删除列
来源：http://hz.jyoumei.cn/gtqjkijofi.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.dianchejie.cn/gtmcwbzjqk.html

[Q07] 删除表
来源：http://hz.jiagoushi.top/gtfqiadrpc.html

DROP TABLE IF EXISTS orders;
来源：http://hz.gogol.net.cn/gtajvmknuc.html

[Q08] 创建普通索引
来源：http://hz.jyoumei.cn/gtzdahhtxe.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.shangyingyoupin.top/gtablxhrmu.html

[Q09] 创建唯一索引
来源：http://hz.aizwys.cn/gtpjvmseoy.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.jinghuilouyu.cn/gtjykfqizf.html

[Q10] 插入单行
来源：http://hz.hysaishi.cn/gtyloldrjz.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.xuanzx.com/gtczkjtjdg.html

[Q11] 一次插入多行
来源：http://hz.chenjidiqi.icu/gttzjbecxw.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.jinghuilouyu.cn/gtnkjkkozd.html

[Q12] 插入后取自增 ID
来源：http://hz.zhaomingkeji.xyz/gtnhyowcpy.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.yuanzhike.top/gtyzemdkel.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.yvedp.cn/gtgfabsnyn.html

[Q13] 忽略重复插入
来源：http://hz.ydjk.org.cn/gtttohvchj.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.yuxming.cn/gtusncerwt.html

[Q14] 存在则更新（upsert）
来源：http://hz.chenjidiqi.icu/gtvrxvkacs.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.cqqwz.cn/gtgvtwjfxf.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.feifeiyinyue.top/gtdekiuhvb.html

[Q15] 查询全部
来源：http://hz.meibo888.top/gtidkgqlah.html

SELECT * FROM users;
来源：http://hz.shanyushiyangkeji.top/gtpofxeequ.html

[Q16] 查询指定列
来源：http://hz.quarkkingdee.top/gtwmubylpv.html

SELECT id, name FROM users;
来源：http://hz.yuxming.cn/gtbbgccxxs.html

[Q17] 条件查询
来源：http://hz.jinqigufen.top/gtwkvyjxfx.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.chenjidiqi.icu/gtycrouamx.html

[Q18] 模糊匹配
来源：http://hz.cqqwz.cn/gtdubmhpgp.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.gogol.net.cn/gtrklnmdak.html

[Q19] 范围查询
来源：http://hz.jinqigfzy.top/gttukpsxks.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.dashuyun.cn/gtdsxehzzi.html

[Q20] IN 列表
来源：http://hz.iojbl.cn/gtrqnrdkfo.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.vqdsnc.cn/gttmoycrjv.html

[Q21] 空值判断
来源：http://hz.shanyushiyangkeji.top/gtpwaxqurj.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.cqqwz.cn/gtcusidgoi.html

[Q22] 排序
来源：http://hz.andypj.xyz/gtfqmkhrxx.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.zhixingplan.top/gtmnuokcpr.html

[Q23] 分页
来源：http://hz.jlsjyb.cn/gtgekanncn.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.yuanzhike.top/gttjtkexwv.html

[Q24] 去重
来源：http://hz.ivvv.top/gtkncwcrna.html

SELECT DISTINCT city FROM users;
来源：http://hz.feifeiyinyue.top/gtgcijckfr.html

[Q25] 只取前 N 条
来源：http://hz.yonumen.top/gtttmddwwx.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.ehwqpu.com/gtigzdbjwr.html

[Q26] 计数
来源：http://hz.zdqjudy.top/gtixvamilb.html

SELECT COUNT(*) FROM users;
来源：http://hz.zhongyouzk.top/gtgpibvhdc.html

[Q27] 条件计数
来源：http://hz.guannengcc.top/gtaslsetkv.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.chenzaomai.com/gtsvhxrilz.html

[Q28] 求和与平均
来源：http://hz.pengpengdd.cyou/gtysndwnnv.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.sysykeji.top/gtcokshawf.html

[Q29] 最大最小值
来源：http://hz.cdnleiting.top/gtgzcgxqid.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.zhiwuduotai.top/gtquozohwg.html

[Q30] 分组统计
来源：http://hz.zhengqikj.top/gtrwewenok.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.shzxlz.cn/gtwzlrampf.html

[Q31] 分组后过滤
来源：http://hz.iojbl.cn/gtbniezitp.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.shuidangran.top/gtrhioeddb.html

[Q32] 分组拼接字符串
来源：http://hz.jinghuilouyu.cn/gttekdtsdp.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.tianlin.xyz/gtkyexhtki.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.zhiwuduotai.top/gtkaxvrujq.html

[Q33] 多列分组
来源：http://hz.yj202588.top/gtguacjsri.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.jianghu66.top/gtldttigyb.html

[Q34] 每组取第一条
来源：http://hz.cdnleiting.top/gtpbmuezxr.html

SELECT * FROM (
来源：http://hz.ywan-chungtsiang.top/gtdjmpaxsp.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.zdqjudy.top/gtfsofpwev.html

) t WHERE rn = 1;
来源：http://hz.aibaodan.cn/gtxlzoweeb.html

[Q35] 内连接
来源：http://hz.jinghuilouyu.cn/gtrwmaczyq.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.hysaishi.cn/gtfytfyqve.html

[Q36] 左连接
来源：http://hz.shzxlz.cn/gtpvpduekd.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.cqqwz.cn/gtopxhtuqd.html

[Q37] 右连接
来源：http://hz.meibo888.top/gtfhlymxay.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.quarkkingdee.top/gtwhjuigcu.html


<!-- 参考信息 -->