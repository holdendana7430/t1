代发 wailian999

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.daria6918.cn/gtgheiqxiu.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.yonumen.top/gtxypchmzv.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.jinyuanbaomall.cn/gtcpkdeoya.html

Go:   slices.Sort(arr)
来源：http://hz.hnxiangtu.top/gtbfmkdkua.html

Ruby: arr.sort
来源：http://hz.jinyuanbaomall.cn/gtjpemyxqw.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.yanxiufei.cn/gtztsqcmol.html

[N03] 快速排序（分治示例）
来源：http://hz.gaohongyu789.top/gtyqdfkztm.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.nanxinkj.top/gtntptsnex.html

PHP:  // 递归实现，或用 usort
来源：http://hz.jyoumei.cn/gtlmfyxlvh.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.wangdashe.top/gthgdfhtri.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.shzxlz.cn/gthuhpsuwl.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.shangyingyoupin.top/gtbrxisbmn.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.xuetiantiany.cn/gtwdjkudju.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.yvedp.cn/gtqduuzrfs.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.ehwqpu.com/gtfjargosa.html

[N04] 斐波那契数列
来源：http://hz.hfpthk.cn/gtumohzdzk.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.cashguo.top/gtroqzxhnt.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.bjfxy.top/gtqllevplp.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.gotoacloud.top/gtqmedirrt.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.yvedp.cn/gtepamnuwr.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.cdnleiting.top/gtkvvzasnh.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.bjfxy.top/gtxlhqyqua.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.ybcxt.top/gtomtamciu.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.c1oappe.top/gtduympkhu.html

[N05] 最大公约数
来源：http://hz.xylfe.cn/gtjjrqajen.html

Py:   math.gcd(a, b)
来源：http://hz.jqgfzy.top/gtviyahlzi.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.tian-w.cn/gtjcicoubw.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.jinghuilouyu.cn/gtypwoenbg.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.jiagoushi.top/gtiutiducs.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.ivvv.top/gtpxzfyuea.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.jqgufenzy.top/gtkxrvknik.html

Ruby: a.gcd(b)
来源：http://hz.yj20258.top/gtqzceorgv.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.zdqjudy.top/gtqyeuwlho.html

[N06] 判断回文字符串
来源：http://hz.ivvv.top/gtxusovkhq.html

Py:   s == s[::-1]
来源：http://hz.hammf.cn/gtrzkadgdx.html

PHP:  $s === strrev($s);
来源：http://hz.ivvv.top/gtikfseabw.html

JS:   s === [...s].reverse().join("")
来源：http://hz.gotoacloud.top/gtfgwuncbe.html

TS:   s === [...s].reverse().join("")
来源：http://hz.yanxiufei.cn/gtdjzwmzti.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.svipenyu.cn/gtjsvwzlmj.html

Go:   // 双指针从两端比较
来源：http://hz.hysaishi.cn/gtnyyviuxe.html

Ruby: s == s.reverse
来源：http://hz.52xcode.cn/gtbfupqabv.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.quarkkingdee.top/gtrxvxmrau.html

[N07] 两数之和（返回下标）
来源：http://hz.gogol.net.cn/gtihfqcyyh.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.yj20258888.top/gtdidvrjrm.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.ppjwa.cn/gtjxhdvasr.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.shanyushiyangkeji.top/gtlrdlqegl.html

TS:   // 手写 Map<string, number>
来源：http://hz.hfpthk.cn/gtjthoqiid.html

Java: // 手写 HashMap
来源：http://hz.guannengcc.top/gtasuprsgd.html

Go:   // 手写 map[int]int
来源：http://hz.sweek.top/gtmzbaluch.html

Ruby: // 手写 Hash
来源：http://hz.kuanghao11.cn/gtngpprwcl.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.ybcxt.top/gtwnakkroa.html

[N08] 生成全排列
来源：http://hz.havefunace.top/gtlogzdebf.html

Py:   itertools.permutations(arr)
来源：http://hz.cucudq.cn/gtpinfpoza.html

PHP:  // 手写递归交换
来源：http://hz.chenjidiqi.icu/gtrcqijnir.html

JS:   // 手写回溯递归
来源：http://hz.tian-w.cn/gtdkjzleab.html

TS:   // 手写回溯递归
来源：http://hz.52xcode.cn/gtgmtxiyzh.html

Java: // 手写回溯递归
来源：http://hz.zycfv.cn/gtrufdwrwe.html

Go:   // 手写回溯递归
来源：http://hz.yvedp.cn/gtfdwllmzr.html

Ruby: arr.permutation.to_a
来源：http://hz.9152youxi.cn/gtuellacve.html

C#:   // 手写回溯递归
来源：http://hz.jiagoushi.top/gthhsrpfuv.html

[N09] 栈与队列
来源：http://hz.hfpthk.cn/gtaurgjujp.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.ivvv.top/gtjbnfajqb.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.yuxming.cn/gtqpldtpau.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.havefunace.top/gtppiosrht.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.mhx1999.top/gtlekwtkxr.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.guowangkeji.top/gtexjebfbe.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.ybcxt.top/gtdvxxsnby.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.nanxuanxn.top/gtgizezzwt.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.nanxuanxn.top/gtqyklomep.html

[N10] 链表节点定义
来源：http://hz.chenlongwang.top/gttbcgmort.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.sufxvd.cn/gtrlkuvmna.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.ywan-chungtsiang.top/gteccdrpup.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.haohaochexian.top/gtbwoxksqm.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.hysaishi.cn/gtgaerdpfe.html

Java: class Node { int v; Node next; }
来源：http://hz.yuanzhike.top/gtulmsefjo.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.52xcode.cn/gtsmkucbhd.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.jqgufenzy.top/gtyudvxcys.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.ywan-chungtsiang.top/gtmhqpyvvr.html

[N11] 二叉树中序遍历
来源：http://hz.shuidangran.top/gtnqfaexkx.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.hfpthk.cn/gtgdjfhlpy.html

PHP:  // 手写递归函数
来源：http://hz.snrcjt.cn/gtyhwtaqrj.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.xinyue.icu/gtvygizzqi.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.haohaochexian.top/gtssctuahx.html

Java: // 手写递归
来源：http://hz.iojbl.cn/gtgxjtpaxz.html

Go:   // 手写递归
来源：http://hz.xziqi.cn/gtsoywwsun.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.gotoacloud.top/gtqcnvehav.html

C#:   // 手写递归
来源：http://hz.jinqigufen.top/gtqpkamcxy.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.shzxlz.cn/gtfalszges.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.guannengcc.top/gtinhjsaeu.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.jianghu66.top/gtgrfasopc.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.c1oappe.top/gtywpffqgf.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.gzhubu.top/gtyxwbyojp.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.hfpthk.cn/gtddhpaycs.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.shanyushiyangtech.top/gtrhmjgxzs.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.zhaomingkeji.xyz/gtjzqkpqsp.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.zhengqikj.top/gtxdqpdzwm.html

================================================================================
来源：http://hz.zhixingplan.top/gtvhxsiuuz.html

O. 并发与异步
来源：http://hz.hywenlv.cn/gtuluwmpjo.html

================================================================================
来源：http://hz.jinqigfzy.top/gtgxmehavn.html

[O01] 启动一个线程
来源：http://hz.sysykeji.top/gtethfoajp.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.fzhhl.top/gtrfjavhrt.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.daxiang520.top/gtrfnfxqyq.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.yj202588.top/gtjrwpluno.html

TS:   // 同 JS
来源：http://hz.hnxiangtu.top/gtjaomwugc.html

Java: new Thread(() -> f()).start()
来源：http://hz.redwolf501.top/gtlgjppbuz.html

Go:   go f()
来源：http://hz.daria6918.cn/gtwoqfbixc.html

Ruby: Thread.new { f }
来源：http://hz.sysykeji.top/gtiuhtxksl.html

C#:   Task.Run(() => F());
来源：http://hz.vqdsnc.cn/gtezufwebn.html

[O02] 使用线程池
来源：http://hz.yangfankeji.com/gtkqqvcpaq.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.yangfankeji.com/gtiogcdivf.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.daxiang520.top/gtamcnseax.html

JS:   // worker_threads 线程池
来源：http://hz.nanxuanxn.top/gtrjuvlhob.html

TS:   // worker_threads 线程池
来源：http://hz.hammf.cn/gtrthvsanw.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.zhixingplan.top/gtalvhxblx.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.jyoumei.cn/gtjlzglcai.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.shangyingyoupin.top/gtbpqaybkk.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.xinyue.icu/gtqzwthtwz.html

[O03] 加锁保护共享数据
来源：http://hz.yangfankeji.com/gthzmlivhv.html

Py:   with lock: shared += 1
来源：http://hz.xingfuxueyuan.xyz/gtdoxwocpc.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.jianghu66.top/gtfjnqohys.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.zycfv.cn/gteyrlhlao.html

TS:   // 同 JS
来源：http://hz.wangshuangyany.cn/gtipbyxcso.html

Java: synchronized (this) { shared++; }
来源：http://hz.sysykeji.top/gtmtmfugev.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.hywenlv.cn/gtfeovahlv.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.xingfuxueyuan.xyz/gtjoukbpcb.html

C#:   lock (gate) { shared++; }
来源：http://hz.cqqwz.cn/gtjujhkidf.html

[O04] 定义异步函数并等待
来源：http://hz.svipenyu.cn/gtrtxikuda.html

Py:   async def f():⏎    await g()
来源：http://hz.snrcjt.cn/gtyrxtkbrq.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.aibaodan.cn/gtbbcvulhk.html

JS:   async function f() { await g(); }
来源：http://hz.hysaishi.cn/gtqamamneu.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.yj20258.top/gtjqrzcjme.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.redwolf501.top/gtrvkphkjv.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.guowangkeji.top/gtphivewaz.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.quarkkingdee.top/gtjzaqplhh.html

C#:   async Task F() { await G(); }
来源：http://hz.jinqigufen.top/gtuykrqswk.html

[O05] 并发执行并等待全部完成
来源：http://hz.jinqigufen.top/gtohpofrql.html

Py:   asyncio.gather(*tasks)
来源：http://hz.zhoulong.xyz/gtlsfvvyfw.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.cqqwz.cn/gtkjeuasoe.html

JS:   await Promise.all(tasks)
来源：http://hz.birdmap.top/gthcjwxfcg.html

TS:   await Promise.all(tasks)
来源：http://hz.fengsongda.top/gtulwbmsnz.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.birdmap.top/gtcagjgwjh.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.meibo888.top/gtnefggjmz.html

Ruby: threads.map(&:join)
来源：http://hz.jinqigfzy.top/gtkqajfjtz.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.hywenlv.cn/gteqgbmxze.html

[O06] 使用进程池
来源：http://hz.haohaochexian.top/gtygkxhamw.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.redwolf501.top/gtfhmdrtnc.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.chenlongwang.top/gtmzgxthal.html

JS:   // child_process / cluster 模块
来源：http://hz.hongshengwenyu.top/gtsppyxzmk.html

TS:   // child_process / cluster 模块
来源：http://hz.daxiang520.top/gtmxjumfbl.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.ydzc1.top/gtfwxvumxl.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.wangdashe.top/gtafbsxmyl.html

Ruby: // fork 块
来源：http://hz.shanyushiyangkeji.top/gtxulqhccw.html

C#:   Parallel.For
来源：http://hz.chenlongwang.top/gtfuyuyonn.html

================================================================================
来源：http://hz.ydzc1.top/gtksjgaclm.html

P. 常用工具函数
来源：http://hz.fengsongda.top/gthigxllzk.html

================================================================================
来源：http://hz.nanxuanxn.top/gthrnbncfx.html

[P01] 生成 UUID
来源：http://hz.gaohongyu789.top/gtfgzoaugc.html

Py:   str(uuid.uuid4())
来源：http://hz.aizwys.cn/gtnebsqpmh.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.chenlongwang.top/gtpqdcrtqo.html

JS:   crypto.randomUUID()
来源：http://hz.havefunace.top/gtoobwsbkb.html

TS:   crypto.randomUUID()
来源：http://hz.xuanzx.com/gttusjpimv.html

Java: UUID.randomUUID().toString()
来源：http://hz.shanyushiyangtech.top/gttzcmqnnb.html

Go:   // 用 github.com/google/uuid
来源：http://hz.gogol.net.cn/gtgahgmuow.html

Ruby: SecureRandom.uuid
来源：http://hz.bjfxy.top/gtyzbdrwat.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.ppjwa.cn/gtssnewlpg.html

[P02] MD5 / SHA256 摘要
来源：http://hz.nanxinkj.top/gtiltishyg.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.316326.xyz/gtulxcexfn.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.zhaomingkeji.xyz/gthqmlppss.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.kuanghao11.cn/gtfskrswne.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.zhaomingkeji.xyz/gtptttqqvj.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.yanxiufei.cn/gtrsrofppb.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.cheryme.top/gtmbaxfauu.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.shanyushiyangkeji.top/gtbmrjltih.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.c1oappe.top/gtygbredyi.html

[P03] 生成短随机字符串
来源：http://hz.yuanzhike.top/gtoxqkyjab.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.c1oappe.top/gtcwzdedzs.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.yj20258888.top/gtkqqxxqhd.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.jqgufenzy.top/gtsttuvwbt.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.gaohongyu789.top/gtjgqhhcru.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.zdqjudy.top/gtclyekztx.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.ehwqpu.com/gtvqruldag.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.meibo888.top/gtzwfaxkbo.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.zhongyouzk.top/gtyeojmpfe.html

[P04] 求长度
来源：http://hz.guannengcc.top/gtrfqfqtoj.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.jinyuanbaomall.cn/gtmcwzzgun.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.andypj.xyz/gtoovgjzqu.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.pengpengdd.cyou/gtvljbawyo.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.pycfn.com/gtzllnfhem.html

Java: list.size();  map.size();  s.length()
来源：http://hz.jinqigufen.top/gtgedibodq.html

Go:   len(arr);  len(m)
来源：http://hz.cucudq.cn/gtpigqvybs.html

Ruby: x.length;  x.size
来源：http://hz.hnxiangtu.top/gthoxroijv.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.cucudq.cn/gthxurwyge.html

[P05] 判断两个对象内容是否相等
来源：http://hz.sweek.top/gtojenrwua.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.sysykeji.top/gtkgoqlhqr.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.zhixingplan.top/gtivdhktxi.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.xziqi.cn/gttbzbfyui.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.hammf.cn/gtcclohkey.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.sysykeji.top/gtxbqmpgbu.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.xziqi.cn/gtinpeteya.html

Ruby: a == b
来源：http://hz.fengsongda.top/gtzocywrkj.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.wangshuangyany.cn/gtfsnsuete.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.aibaodan.cn/gtqyydmbep.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.ppjwa.cn/gtegqdxatd.html

PHP:  if (empty($x)) {}
来源：http://hz.yangfankeji.com/gtdqkvrmhh.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.dianchejie.cn/gtaghcvxec.html

TS:   if (x == null) {}
来源：http://hz.smart0.xyz/gtppislvmz.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.tian-w.cn/gthswglyra.html

Go:   if x == nil {}
来源：http://hz.xuanzx.com/gtoejlxnrr.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.jianghu66.top/gtcdpdzikd.html

C#:   if (x is null) {}
来源：http://hz.haohaochexian.top/gtsyikvnwi.html

[P07] 防抖与节流
来源：http://hz.zycfv.cn/gtvhfbddut.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.jqgfzy.top/gtxkmtofmt.html

PHP:  // 手写时间戳比较
来源：http://hz.jyoumei.cn/gtbndopvws.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.dianchejie.cn/gttwdfaimg.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.yj202588.top/gteqgjebar.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.nanxinkj.top/gtfrfyfxyp.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.wangdashe.top/gtufvkpfaz.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.havefunace.top/gtwdfntoiy.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.zhoulong.xyz/gtzuanobnr.html

[P08] 处理浮点精度问题
来源：http://hz.zdqjudy.top/gtljaosqjp.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.zhengqikj.top/gtvzsqmbtf.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.jinghuilouyu.cn/gtzekcbmds.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.zhaomingkeji.xyz/gtreqbwvds.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.chenlongwang.top/gtwkwvntti.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.tian-w.cn/gtmlpehnlo.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.gzhubu.top/gtrfqnsioi.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.dashuyun.cn/gtwdwrxgfi.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.gzhubu.top/gtbxnvyouz.html

================================================================================
来源：http://hz.yanxiufei.cn/gthwfizqgn.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.yj20258.top/gtttmhadpr.html

================================================================================
来源：http://hz.jqgfzy.top/gtlwjjyvig.html

[Q01] 创建表
来源：http://hz.dashuyun.cn/gtvbomidmu.html

CREATE TABLE users (
来源：http://hz.yongpay.top/gtimwhvnnc.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.gzhubu.top/gtkolbegbq.html

name VARCHAR(50) NOT NULL,
来源：http://hz.daxiang520.top/gtcozsnqos.html

email VARCHAR(100) UNIQUE,
来源：http://hz.cucudq.cn/gtglnewvhl.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.nanxinkj.top/gtjmztkywv.html

);
来源：http://hz.sxryk.cn/gtwgjhkhbu.html

[Q02] 创建带外键的表
来源：http://hz.andypj.xyz/gtjujbmfxv.html

CREATE TABLE orders (
来源：http://hz.nanxinkj.top/gtvbzmuave.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.haohaochexian.top/gtumsssrwx.html

user_id INT NOT NULL,
来源：http://hz.yj20258888.top/gtfawicjdv.html

amount DECIMAL(10, 2),
来源：http://hz.gzhubu.top/gtordrrnwr.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.guowangkeji.top/gtbktvedfi.html

);
来源：http://hz.tian-w.cn/gthqfnnwig.html

[Q03] 增加列
来源：http://hz.jinqigfzy.top/gthnlewbob.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.haohaochexian.top/gthvbquwys.html

[Q04] 修改列类型
来源：http://hz.andypj.xyz/gtsvixaund.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.cdnleiting.top/gttyeixqeh.html

[Q05] 重命名列
来源：http://hz.hammf.cn/gtyjaoceut.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.yj202588.top/gtpvjfhdkr.html

[Q06] 删除列
来源：http://hz.yj202588.top/gtehysafwu.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.jlsjyb.cn/gtfwftjjty.html

[Q07] 删除表
来源：http://hz.hnxiangtu.top/gtsyijelsh.html

DROP TABLE IF EXISTS orders;
来源：http://hz.feifeiyinyue.top/gtzeihamgw.html

[Q08] 创建普通索引
来源：http://hz.gaohongyu789.top/gtqqdeniip.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.ydjk.org.cn/gttttnclsx.html

[Q09] 创建唯一索引
来源：http://hz.zhoulong.xyz/gtdiefrows.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.yvedp.cn/gtmalzxynd.html

[Q10] 插入单行
来源：http://hz.ppjwa.cn/gtoxdbatij.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.guannengcc.top/gtxnfsjqzr.html

[Q11] 一次插入多行
来源：http://hz.zdqjudy.top/gtzbqblbor.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.svipenyu.cn/gtcfpqpfng.html

[Q12] 插入后取自增 ID
来源：http://hz.iojbl.cn/gtutlvkrbv.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.316326.xyz/gtipxssppq.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.kuanghao11.cn/gtlnzohdqk.html

[Q13] 忽略重复插入
来源：http://hz.zhixingplan.top/gtgovzbhou.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.zhixingplan.top/gtkliemfhh.html

[Q14] 存在则更新（upsert）
来源：http://hz.chenzaomai.com/gtjwbqkver.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.hnxiangtu.top/gtwuzwjufu.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.yonumen.top/gtaaxytgey.html

[Q15] 查询全部
来源：http://hz.jianghu66.top/gthxktwyrq.html

SELECT * FROM users;
来源：http://hz.hnqzz.top/gtzmzdzjte.html

[Q16] 查询指定列
来源：http://hz.tian-w.cn/gtjczemliq.html

SELECT id, name FROM users;
来源：http://hz.bjfxy.top/gtfsyiqari.html

[Q17] 条件查询
来源：http://hz.kuanghao11.cn/gtcjdfwdvx.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.gogol.net.cn/gtmhyjtrtx.html

[Q18] 模糊匹配
来源：http://hz.c1oappe.top/gtdyatdxuk.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.zdqjudy.top/gtngjxkbwr.html

[Q19] 范围查询
来源：http://hz.yuanzhike.top/gtbppvoggb.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.mhx1999.top/gttwotqmgd.html

[Q20] IN 列表
来源：http://hz.iojbl.cn/gtbrmyiaof.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.nwbrower.top/gtqpbccjxc.html

[Q21] 空值判断
来源：http://hz.yongpay.top/gtliwkvnkn.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.shanyushiyangkeji.top/gtrntylwrl.html

[Q22] 排序
来源：http://hz.andypj.xyz/gtuytuosvv.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.xuetiantiany.cn/gtvgaflqcr.html

[Q23] 分页
来源：http://hz.zhengqikj.top/gtzbuyaiwe.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.0kj1m.cn/gttmhqqkkz.html

[Q24] 去重
来源：http://hz.smart0.xyz/gthqlhrnfn.html

SELECT DISTINCT city FROM users;
来源：http://hz.gogol.net.cn/gttjtnavru.html

[Q25] 只取前 N 条
来源：http://hz.sweek.top/gtrepkjula.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.yueranfly.top/gtxodyioxw.html

[Q26] 计数
来源：http://hz.hnqzz.top/gtdvtgjpgh.html

SELECT COUNT(*) FROM users;
来源：http://hz.9152youxi.cn/gtjvctkqtv.html

[Q27] 条件计数
来源：http://hz.birdmap.top/gtwlitpegw.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.ydjk.org.cn/gtpkcngciu.html

[Q28] 求和与平均
来源：http://hz.zhiwuduotai.top/gtjaqmhhcc.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.ehwqpu.com/gtpjswzhpr.html

[Q29] 最大最小值
来源：http://hz.tian-w.cn/gtblixaujx.html


<!-- 参考信息 -->