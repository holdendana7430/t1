代发 wailian999

PHP:  // 递归实现，或用 usort
来源：http://hz.hywenlv.cn/gthnihnouv.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.meibo888.top/gtonyzzixl.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.yvedp.cn/gtrxaokdzy.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.xinyue.icu/gthqicfvya.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.yvedp.cn/gtvjqhnnpn.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.zhiwuduotai.top/gtkoibzdhx.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.quarkkingdee.top/gtipetvhel.html

[N04] 斐波那契数列
来源：http://hz.hysaishi.cn/gtiecfwnvg.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.bjfxy.top/gtdrndzpkx.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.guannengcc.top/gtpffwviga.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.daria6918.cn/gtwxesiotu.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.jiagoushi.top/gtfwraryij.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.gzhubu.top/gthvcliiwb.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.chenlongwang.top/gtntqtyccf.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.ydjk.org.cn/gtbeuvuiuu.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.shangyingyoupin.top/gtgaxutaxx.html

[N05] 最大公约数
来源：http://hz.zhaomingkeji.xyz/gtsrugjrzo.html

Py:   math.gcd(a, b)
来源：http://hz.jqgufenzy.top/gtxftyygik.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.hammf.cn/gtkzcjlbfg.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.tian-w.cn/gtkfzrhryz.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.nanxuanxn.top/gtusnxcukd.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.redwolf501.top/gtyupnkkll.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.jinyuanbaomall.cn/gtszzuvofc.html

Ruby: a.gcd(b)
来源：http://hz.zhijiandao.cn/gtzyzejgiw.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.yuanzhike.top/gtvbwjcbpb.html

[N06] 判断回文字符串
来源：http://hz.sweek.top/gtmlrdyvuc.html

Py:   s == s[::-1]
来源：http://hz.nanxuanxn.top/gtgoiqlthb.html

PHP:  $s === strrev($s);
来源：http://hz.hysaishi.cn/gtranwviso.html

JS:   s === [...s].reverse().join("")
来源：http://hz.pengpengdd.cyou/gtswwgipdr.html

TS:   s === [...s].reverse().join("")
来源：http://hz.zhoulong.xyz/gttupkhpen.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.hfpthk.cn/gtsztelogr.html

Go:   // 双指针从两端比较
来源：http://hz.feifeiyinyue.top/gtvmeyotdi.html

Ruby: s == s.reverse
来源：http://hz.jqgufenzy.top/gtsissrwmg.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.yj20258888.top/gtgsklkcgy.html

[N07] 两数之和（返回下标）
来源：http://hz.zycfv.cn/gtffwuldeh.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.zhixingplan.top/gtzxnwaaeo.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.hammf.cn/gtijernoav.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.xylfe.cn/gtaiafowty.html

TS:   // 手写 Map<string, number>
来源：http://hz.yuanzhike.top/gtqydfdenh.html

Java: // 手写 HashMap
来源：http://hz.zhixingplan.top/gtnuxwylmv.html

Go:   // 手写 map[int]int
来源：http://hz.jyoumei.cn/gtrjzvcjoq.html

Ruby: // 手写 Hash
来源：http://hz.sysykeji.top/gtfadxfskv.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.sufxvd.cn/gthwyalbgf.html

[N08] 生成全排列
来源：http://hz.ywan-chungtsiang.top/gtxsgawczw.html

Py:   itertools.permutations(arr)
来源：http://hz.shzxlz.cn/gtziyysnxd.html

PHP:  // 手写递归交换
来源：http://hz.yongpay.top/gtemqudmtb.html

JS:   // 手写回溯递归
来源：http://hz.gogol.net.cn/gtlukvrsda.html

TS:   // 手写回溯递归
来源：http://hz.redwolf501.top/gtzzgjyfbe.html

Java: // 手写回溯递归
来源：http://hz.daria6918.cn/gtszhwhfsn.html

Go:   // 手写回溯递归
来源：http://hz.zhaomingkeji.xyz/gtecjzfeyl.html

Ruby: arr.permutation.to_a
来源：http://hz.zhoulong.xyz/gtviyrskdd.html

C#:   // 手写回溯递归
来源：http://hz.quarkkingdee.top/gtrwqixfuz.html

[N09] 栈与队列
来源：http://hz.ywan-chungtsiang.top/gtdzzjzpqn.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.mhx1999.top/gtzkaorvyy.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.yj202588.top/gtkicvubjg.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.birdmap.top/gtiqsbjuqp.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.yvedp.cn/gtcsemqyke.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.iojbl.cn/gtpoaldrhi.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.sysykeji.top/gtnkxmpjls.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.jinqigfzy.top/gtjdlszomd.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.sysykeji.top/gtcgwdaxyq.html

[N10] 链表节点定义
来源：http://hz.yanxiufei.cn/gtaxglkwep.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.smart0.xyz/gtwrdjrykc.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.yanxiufei.cn/gtigsksvsl.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.yanxiufei.cn/gtyeghyzwc.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.xziqi.cn/gtrtplvlfr.html

Java: class Node { int v; Node next; }
来源：http://hz.smart0.xyz/gtrzfytdxn.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.cdnleiting.top/gtheedeaii.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.jinqigufen.top/gtvxwkrgmt.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.tanke756.top/gtrupcpqsk.html

[N11] 二叉树中序遍历
来源：http://hz.zhongyouzk.top/gtcjigtxjq.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.cdnleiting.top/gtrxibyprx.html

PHP:  // 手写递归函数
来源：http://hz.gzhubu.top/gtinghxjtq.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.yuanzhike.top/gtykfjzwjq.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.daxiang520.top/gtdhulfbsx.html

Java: // 手写递归
来源：http://hz.zycfv.cn/gtnxrohswo.html

Go:   // 手写递归
来源：http://hz.xinyue.icu/gtgowpswnx.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.redwolf501.top/gtkvkxugvv.html

C#:   // 手写递归
来源：http://hz.dianchejie.cn/gtpwkvqsyz.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.yangfankeji.com/gtpdvlsftv.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.yonumen.top/gtsweeillu.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.cucudq.cn/gtkhyovyka.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.jinqigufen.top/gtzmmdgjah.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.vqdsnc.cn/gtyqanblky.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.52xcode.cn/gtycwiphpv.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.sxryk.cn/gtiqaxycql.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.ydzc1.top/gtcnqoatny.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.zhoulong.xyz/gtpizvzlyy.html

================================================================================
来源：http://hz.shzxlz.cn/gtvzxxbltf.html

O. 并发与异步
来源：http://hz.jinyuanbaomall.cn/gtiynivvmc.html

================================================================================
来源：http://hz.jqgfzy.top/gtdzjaedhg.html

[O01] 启动一个线程
来源：http://hz.jqgfzy.top/gtuobxqxdd.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.hnqzz.top/gtfrvqtzdd.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.yueranfly.top/gttmawqobv.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.hfpthk.cn/gtkikukrtb.html

TS:   // 同 JS
来源：http://hz.vqdsnc.cn/gttqvoowxv.html

Java: new Thread(() -> f()).start()
来源：http://hz.andypj.xyz/gtfexiptxp.html

Go:   go f()
来源：http://hz.jyoumei.cn/gtquujwjxt.html

Ruby: Thread.new { f }
来源：http://hz.ydzc1.top/gtpcxfxoaa.html

C#:   Task.Run(() => F());
来源：http://hz.cucudq.cn/gtcjrvmeal.html

[O02] 使用线程池
来源：http://hz.ydzc1.top/gthjwgmxxr.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.hongshengwenyu.top/gtoinnalhg.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.svipenyu.cn/gtqmshqkcg.html

JS:   // worker_threads 线程池
来源：http://hz.c1oappe.top/gtdczqkfaf.html

TS:   // worker_threads 线程池
来源：http://hz.316326.xyz/gtrmkvrahj.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.jinqigufen.top/gtigpijijs.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.daria6918.cn/gtxuehpobc.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.jinqigufen.top/gtfvcwvxqi.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.tian-w.cn/gtzhhtevcz.html

[O03] 加锁保护共享数据
来源：http://hz.yj20258.top/gtrriszdxk.html

Py:   with lock: shared += 1
来源：http://hz.vqdsnc.cn/gtpplotrpy.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.chenjidiqi.icu/gtowtpmpeo.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.cashguo.top/gtexswkzvn.html

TS:   // 同 JS
来源：http://hz.9152youxi.cn/gtnrrmyayv.html

Java: synchronized (this) { shared++; }
来源：http://hz.xuanzx.com/gtrdhzcqel.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.cqqwz.cn/gtnjteojsj.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.zhoulong.xyz/gtdvnlmuyr.html

C#:   lock (gate) { shared++; }
来源：http://hz.ydjk.org.cn/gtelhdprur.html

[O04] 定义异步函数并等待
来源：http://hz.cucudq.cn/gtqbhqxzwd.html

Py:   async def f():⏎    await g()
来源：http://hz.0kj1m.cn/gtupohmcbw.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.yvedp.cn/gtpfffyoox.html

JS:   async function f() { await g(); }
来源：http://hz.jinghuilouyu.cn/gtonrhowfb.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.52xcode.cn/gtfqchavps.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.jinqigufen.top/gtyiofapen.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.yongpay.top/gtoenxpurw.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.yj20258888.top/gtmminezca.html

C#:   async Task F() { await G(); }
来源：http://hz.aibaodan.cn/gtldbckmon.html

[O05] 并发执行并等待全部完成
来源：http://hz.yueranfly.top/gtysectehb.html

Py:   asyncio.gather(*tasks)
来源：http://hz.ydzc1.top/gtbbrwhcpu.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.jinqigufen.top/gtehvdonao.html

JS:   await Promise.all(tasks)
来源：http://hz.hnqzz.top/gthkeqtajj.html

TS:   await Promise.all(tasks)
来源：http://hz.shanyushiyangtech.top/gtuiuvawvu.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.jiagoushi.top/gtgyktamne.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.nanxinkj.top/gtkeyrfnwc.html

Ruby: threads.map(&:join)
来源：http://hz.zhaomingkeji.xyz/gtnqhjcwba.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.yueranfly.top/gtrpvtsbxp.html

[O06] 使用进程池
来源：http://hz.sxryk.cn/gtrevgynwl.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.fzhhl.top/gtujjhumsi.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.jinghuilouyu.cn/gtmedlcuuh.html

JS:   // child_process / cluster 模块
来源：http://hz.316326.xyz/gtisqyxejm.html

TS:   // child_process / cluster 模块
来源：http://hz.pycfn.com/gtwviasbvb.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.birdmap.top/gtopnvmliq.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.zhiwuduotai.top/gtlacmywuf.html

Ruby: // fork 块
来源：http://hz.sweek.top/gtmqhcftdm.html

C#:   Parallel.For
来源：http://hz.nanxuanxn.top/gttkvfctfl.html

================================================================================
来源：http://hz.zhengqikj.top/gtqizexnke.html

P. 常用工具函数
来源：http://hz.shzxlz.cn/gtiaptntzm.html

================================================================================
来源：http://hz.hywenlv.cn/gtfwrkcczi.html

[P01] 生成 UUID
来源：http://hz.cdnleiting.top/gtirebwvoi.html

Py:   str(uuid.uuid4())
来源：http://hz.zhoulong.xyz/gtyoswrefh.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.ydzc1.top/gtgcglvtrz.html

JS:   crypto.randomUUID()
来源：http://hz.52xcode.cn/gtvayjqjcn.html

TS:   crypto.randomUUID()
来源：http://hz.sweek.top/gtuzyoavwg.html

Java: UUID.randomUUID().toString()
来源：http://hz.jianghu66.top/gtwcrdvaou.html

Go:   // 用 github.com/google/uuid
来源：http://hz.zhoulong.xyz/gtipomsrdm.html

Ruby: SecureRandom.uuid
来源：http://hz.gotoacloud.top/gtgjfryexx.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.zhixingplan.top/gtnpayujul.html

[P02] MD5 / SHA256 摘要
来源：http://hz.chenjidiqi.icu/gtzqqswxev.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.sufxvd.cn/gtylmifxxs.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.zhongyouzk.top/gtspaawwro.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.yongpay.top/gtneozzadw.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.sweek.top/gtluayindq.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.ybcxt.top/gtdsnyvptb.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.jiagoushi.top/gtqmsdwmdc.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.9152youxi.cn/gtvsvbsdbe.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.jinqigfzy.top/gthfjxafma.html

[P03] 生成短随机字符串
来源：http://hz.ydzc1.top/gtgvcewtwx.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.gotoacloud.top/gttejomvri.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.pengpengdd.cyou/gtyudtlwhc.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.gotoacloud.top/gtlphdrbid.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.smart0.xyz/gtvuzxjkzm.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.dashuyun.cn/gtnvuatsbo.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.yuanzhike.top/gtlcbzrggw.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.cheryme.top/gtvgbruthw.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.fengsongda.top/gtfkclppll.html

[P04] 求长度
来源：http://hz.yj20258.top/gtbqdojapu.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.jyoumei.cn/gtxswtegtl.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.xinyue.icu/gtleahxnpr.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.dashuyun.cn/gtpmdslnsn.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.jinqigufen.top/gtorohvhdq.html

Java: list.size();  map.size();  s.length()
来源：http://hz.zhijiandao.cn/gthwtycyzm.html

Go:   len(arr);  len(m)
来源：http://hz.cucudq.cn/gtzxjegvik.html

Ruby: x.length;  x.size
来源：http://hz.yuanzhike.top/gthhuyrqka.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.ybcxt.top/gtozmrwsga.html

[P05] 判断两个对象内容是否相等
来源：http://hz.sxryk.cn/gtcoqysglk.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.iojbl.cn/gtghhsiuql.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.tianlin.xyz/gtntauunvv.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.andypj.xyz/gtqrjbyrez.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.ydzc1.top/gthpediosv.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.xingfuxueyuan.xyz/gtlywxcwdd.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.yuxming.cn/gtcqcqdliz.html

Ruby: a == b
来源：http://hz.sweek.top/gteolncdej.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.cqqwz.cn/gtijjhbvfd.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.sweek.top/gtocliywpo.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.ehwqpu.com/gtlhnvilnl.html

PHP:  if (empty($x)) {}
来源：http://hz.yongpay.top/gtxvtuumla.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.nwbrower.top/gtbjqpahft.html

TS:   if (x == null) {}
来源：http://hz.daria6918.cn/gtstmcrpcs.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.cdnleiting.top/gtdvqqeaeo.html

Go:   if x == nil {}
来源：http://hz.yj202588.top/gttjfpsiee.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.cqqwz.cn/gtqngfsdyd.html

C#:   if (x is null) {}
来源：http://hz.shuidangran.top/gtuloauaij.html

[P07] 防抖与节流
来源：http://hz.xuetiantiany.cn/gtqrfwkbjy.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.chenlongwang.top/gtrmadpsto.html

PHP:  // 手写时间戳比较
来源：http://hz.yueranfly.top/gtiyqghtlt.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.jiagoushi.top/gtnmtlrbas.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.jyoumei.cn/gtalxtqyiw.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.52xcode.cn/gtlptypusb.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.quarkkingdee.top/gtnlbktepf.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.daria6918.cn/gtzejhbswp.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.havefunace.top/gtnpngvzwr.html

[P08] 处理浮点精度问题
来源：http://hz.jqgfzy.top/gtpufwzdxo.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.bjfxy.top/gtojsohmgh.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.yj202588.top/gtbzgujvdv.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.yuxming.cn/gtpsmvpupb.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.xziqi.cn/gtgptxobhf.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.c1oappe.top/gtyvexictn.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.quarkkingdee.top/gtzhuhrtfz.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.shangyingyoupin.top/gtixfabrxj.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.jinyuanbaomall.cn/gtilcsbfog.html

================================================================================
来源：http://hz.shuidangran.top/gtcvguifwp.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.jianghu66.top/gtdczqsqpj.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtkateylml.html

[Q01] 创建表
来源：http://hz.snrcjt.cn/gthwpjufld.html

CREATE TABLE users (
来源：http://hz.c1oappe.top/gtwkktupvk.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.gzhubu.top/gtkikidmit.html

name VARCHAR(50) NOT NULL,
来源：http://hz.tanke756.top/gtugnbgibx.html

email VARCHAR(100) UNIQUE,
来源：http://hz.jlsjyb.cn/gtvshrnwlt.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.kuanghao11.cn/gtaepwimey.html

);
来源：http://hz.yanxiufei.cn/gtagtwxjym.html

[Q02] 创建带外键的表
来源：http://hz.yj20258888.top/gtzyscunow.html

CREATE TABLE orders (
来源：http://hz.yonumen.top/gtejvbiukl.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.ydzc1.top/gtogqdrlhx.html

user_id INT NOT NULL,
来源：http://hz.jlsjyb.cn/gtsnybbqjq.html

amount DECIMAL(10, 2),
来源：http://hz.xuetiantiany.cn/gtnmkyrtdh.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.ehwqpu.com/gtiexawxch.html

);
来源：http://hz.xziqi.cn/gtpjrzbgmj.html

[Q03] 增加列
来源：http://hz.hfpthk.cn/gtaxgxjfiq.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.snrcjt.cn/gtinbwvnhb.html

[Q04] 修改列类型
来源：http://hz.shanyushiyangtech.top/gtzhecjweu.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.316326.xyz/gtcrdgbrqq.html

[Q05] 重命名列
来源：http://hz.zycfv.cn/gtbxdqnekc.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.nanxuanxn.top/gtubugfoik.html

[Q06] 删除列
来源：http://hz.yangfankeji.com/gtdllajkbq.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.yuxming.cn/gtefdwzmoc.html

[Q07] 删除表
来源：http://hz.sweek.top/gtiinvzwwy.html

DROP TABLE IF EXISTS orders;
来源：http://hz.hfpthk.cn/gtpplnvjyy.html

[Q08] 创建普通索引
来源：http://hz.yuanzhike.top/gtlclgjfzx.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.jinqigufen.top/gtsimqsuuq.html

[Q09] 创建唯一索引
来源：http://hz.redwolf501.top/gtvsbatwci.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.daxiang520.top/gtlbrxmebj.html

[Q10] 插入单行
来源：http://hz.jyoumei.cn/gttenqrrcn.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.fengsongda.top/gtzwztwlkn.html

[Q11] 一次插入多行
来源：http://hz.chenzaomai.com/gtfsemuakm.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.xylfe.cn/gtlkwzried.html

[Q12] 插入后取自增 ID
来源：http://hz.xuanzx.com/gtvtiezetg.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.meibo888.top/gtnlqcosfw.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.hnqzz.top/gtrrkpyyca.html

[Q13] 忽略重复插入
来源：http://hz.pengpengdd.cyou/gtwmmjnnqj.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.bjfxy.top/gtffsvgnsz.html

[Q14] 存在则更新（upsert）
来源：http://hz.jianghu66.top/gtcnmujlvk.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.hywenlv.cn/gtmxwywgef.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.9152youxi.cn/gtslfwbkxb.html

[Q15] 查询全部
来源：http://hz.yongpay.top/gtwoywbhnh.html

SELECT * FROM users;
来源：http://hz.0kj1m.cn/gtypbsrgsh.html

[Q16] 查询指定列
来源：http://hz.yj20258.top/gtirqbndcg.html

SELECT id, name FROM users;
来源：http://hz.jinqigufen.top/gtgpruczmm.html

[Q17] 条件查询
来源：http://hz.ybcxt.top/gtuvjzopsl.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.shanyushiyangkeji.top/gttpkcfwhi.html

[Q18] 模糊匹配
来源：http://hz.zhongyouzk.top/gtdmingpxf.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.meibo888.top/gtkpphckuz.html

[Q19] 范围查询
来源：http://hz.chenlongwang.top/gtfpcjfbor.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.gzhubu.top/gttsmwipes.html

[Q20] IN 列表
来源：http://hz.xinyue.icu/gtobgfcfui.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.shzxlz.cn/gtzkgxidsx.html

[Q21] 空值判断
来源：http://hz.dashuyun.cn/gtmdafdqbh.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.jinghuilouyu.cn/gtthkcqpqf.html

[Q22] 排序
来源：http://hz.daxiang520.top/gtdfpesurf.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.zhoulong.xyz/gtasgtppnz.html

[Q23] 分页
来源：http://hz.pycfn.com/gtjteswbyh.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.smart0.xyz/gtldnpfcjg.html

[Q24] 去重
来源：http://hz.sufxvd.cn/gtputnhcpm.html

SELECT DISTINCT city FROM users;
来源：http://hz.shanyushiyangkeji.top/gtpimcikbg.html

[Q25] 只取前 N 条
来源：http://hz.zycfv.cn/gtapahuntk.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.shanyushiyangkeji.top/gtpukgibcb.html

[Q26] 计数
来源：http://hz.xziqi.cn/gtrzglaeoo.html

SELECT COUNT(*) FROM users;
来源：http://hz.gotoacloud.top/gtwcgvuhhz.html

[Q27] 条件计数
来源：http://hz.jinqigufen.top/gtiniedtej.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.sxryk.cn/gtkrqqahrw.html

[Q28] 求和与平均
来源：http://hz.yuanzhike.top/gtcrwjmcjo.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.xuanzx.com/gtedeuhwld.html

[Q29] 最大最小值
来源：http://hz.tianlin.xyz/gtwqyjqdie.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.tanke756.top/gtqqlfvlva.html

[Q30] 分组统计
来源：http://hz.sweek.top/gtfxafnglq.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.cheryme.top/gtcoinasoy.html

[Q31] 分组后过滤
来源：http://hz.guannengcc.top/gtrbyvzdja.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.jqgufenzy.top/gtwgypqwrv.html

[Q32] 分组拼接字符串
来源：http://hz.dashuyun.cn/gtzioswwpj.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.haohaochexian.top/gtbfqrhhfy.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.yvedp.cn/gtorrkwwfa.html


<!-- 参考信息 -->