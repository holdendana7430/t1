代发 wailian999

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.cdnleiting.top/gtawmtlucx.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.bjfxy.top/gtppctdxwr.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.jyoumei.cn/gtkmdqyjqn.html

[N04] 斐波那契数列
来源：http://hz.sxryk.cn/gtkqjuqgdl.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.52xcode.cn/gtyquowsng.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.andypj.xyz/gttxejqtze.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.xingfuxueyuan.xyz/gtzmkxzrgb.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.ehwqpu.com/gtcdstcthf.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.gaohongyu789.top/gtkwkevwsi.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.xinyue.icu/gtzyqnaavn.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.sysykeji.top/gtitiqxzcs.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.jyoumei.cn/gtsdjgyfiv.html

[N05] 最大公约数
来源：http://hz.c1oappe.top/gtrnacpuqa.html

Py:   math.gcd(a, b)
来源：http://hz.zycfv.cn/gtpidtidri.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.havefunace.top/gtohdnyrvf.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.0kj1m.cn/gtsavhrhyq.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.jyoumei.cn/gttyauwspa.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.cheryme.top/gthbwuewrp.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.vqdsnc.cn/gtbryxrlas.html

Ruby: a.gcd(b)
来源：http://hz.xziqi.cn/gthcndxgfp.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.ppjwa.cn/gtlyorjzji.html

[N06] 判断回文字符串
来源：http://hz.jinyuanbaomall.cn/gtazvvuzja.html

Py:   s == s[::-1]
来源：http://hz.chenjidiqi.icu/gtkqdwrqkl.html

PHP:  $s === strrev($s);
来源：http://hz.sysykeji.top/gtogslobjl.html

JS:   s === [...s].reverse().join("")
来源：http://hz.mhx1999.top/gtgpsazvjw.html

TS:   s === [...s].reverse().join("")
来源：http://hz.ydjk.org.cn/gtgzlzxpak.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.zhixingplan.top/gtawddxlhz.html

Go:   // 双指针从两端比较
来源：http://hz.gzhubu.top/gtztfqnnik.html

Ruby: s == s.reverse
来源：http://hz.redwolf501.top/gthboeykkt.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.xylfe.cn/gtbzjiwpre.html

[N07] 两数之和（返回下标）
来源：http://hz.yonumen.top/gtiryrnlgm.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.daria6918.cn/gtfpnijhku.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.shanyushiyangkeji.top/gtreknfemc.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.shuidangran.top/gtkosqwqww.html

TS:   // 手写 Map<string, number>
来源：http://hz.haohaochexian.top/gtqaglweyq.html

Java: // 手写 HashMap
来源：http://hz.tanke756.top/gtosumqwbm.html

Go:   // 手写 map[int]int
来源：http://hz.hammf.cn/gtqcciqusn.html

Ruby: // 手写 Hash
来源：http://hz.shuidangran.top/gtclchzpxw.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.tian-w.cn/gtdgghmovt.html

[N08] 生成全排列
来源：http://hz.hfpthk.cn/gtjpcbeusc.html

Py:   itertools.permutations(arr)
来源：http://hz.shuidangran.top/gtrdpruseq.html

PHP:  // 手写递归交换
来源：http://hz.yongpay.top/gtywfjjrrz.html

JS:   // 手写回溯递归
来源：http://hz.hammf.cn/gtunhltlrm.html

TS:   // 手写回溯递归
来源：http://hz.yanxiufei.cn/gtyouthbpx.html

Java: // 手写回溯递归
来源：http://hz.yongpay.top/gtpbbdldfk.html

Go:   // 手写回溯递归
来源：http://hz.jianghu66.top/gtenqyljal.html

Ruby: arr.permutation.to_a
来源：http://hz.xziqi.cn/gtkanxfodr.html

C#:   // 手写回溯递归
来源：http://hz.yueranfly.top/gtpmmypggf.html

[N09] 栈与队列
来源：http://hz.gaohongyu789.top/gtfsbismpf.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.birdmap.top/gtfsjnrxoc.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.jqgfzy.top/gttyvychuc.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.c1oappe.top/gtmnxhyntn.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.feifeiyinyue.top/gtnkojddio.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.bjfxy.top/gtuszxzfde.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.meibo888.top/gtvchhkgdf.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.dianchejie.cn/gtwgjwqyet.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.52xcode.cn/gtxcxnytiy.html

[N10] 链表节点定义
来源：http://hz.jinghuilouyu.cn/gtbfjnqbtz.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.zhiwuduotai.top/gtdvqtqkpf.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.ydjk.org.cn/gtpghxtdby.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.sxryk.cn/gtxsymaqht.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.redwolf501.top/gtejonxjkm.html

Java: class Node { int v; Node next; }
来源：http://hz.xingfuxueyuan.xyz/gtixjcoalf.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.xingfuxueyuan.xyz/gtshhkubqu.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.gaohongyu789.top/gtizgruind.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.52xcode.cn/gtdkvwwxdt.html

[N11] 二叉树中序遍历
来源：http://hz.xinyue.icu/gtyfpfyqbe.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.daria6918.cn/gtmacspaeo.html

PHP:  // 手写递归函数
来源：http://hz.shzxlz.cn/gtrpcgjfvi.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.hongshengwenyu.top/gtomrgtugv.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.hnqzz.top/gtslcrdprg.html

Java: // 手写递归
来源：http://hz.xingfuxueyuan.xyz/gthaqayqnm.html

Go:   // 手写递归
来源：http://hz.zhongyouzk.top/gtvnvivmdd.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.yangfankeji.com/gtimalivub.html

C#:   // 手写递归
来源：http://hz.chenzaomai.com/gtwjupzmiy.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.ppjwa.cn/gthikryliv.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.fengsongda.top/gtywfuysiz.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.xuetiantiany.cn/gtpzlbuozf.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.jinqigfzy.top/gtpzwrlkpe.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.aibaodan.cn/gtfbpncfyk.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.fengsongda.top/gtqiazsjsr.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.hnqzz.top/gtzlizxzkc.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.chenjidiqi.icu/gtaxggenjf.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.hongshengwenyu.top/gtroqsoyei.html

================================================================================
来源：http://hz.ppjwa.cn/gtzoglndog.html

O. 并发与异步
来源：http://hz.tanke756.top/gtmxedagan.html

================================================================================
来源：http://hz.52xcode.cn/gtcysumirx.html

[O01] 启动一个线程
来源：http://hz.yangfankeji.com/gtmyxvromt.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.gogol.net.cn/gtqpynlnzp.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.jinghuilouyu.cn/gtgeqvrevi.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.shzxlz.cn/gtqgocgmik.html

TS:   // 同 JS
来源：http://hz.birdmap.top/gtywuojouq.html

Java: new Thread(() -> f()).start()
来源：http://hz.svipenyu.cn/gtlhrhdufm.html

Go:   go f()
来源：http://hz.cucudq.cn/gtrpzuxqig.html

Ruby: Thread.new { f }
来源：http://hz.zhiwuduotai.top/gtsjszegxu.html

C#:   Task.Run(() => F());
来源：http://hz.dashuyun.cn/gtoideblra.html

[O02] 使用线程池
来源：http://hz.hnxiangtu.top/gtnyuyygts.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.hysaishi.cn/gttlgpsndm.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.daria6918.cn/gtjsiuvkqa.html

JS:   // worker_threads 线程池
来源：http://hz.shangyingyoupin.top/gttrdrptvl.html

TS:   // worker_threads 线程池
来源：http://hz.ehwqpu.com/gtssesraik.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.chenzaomai.com/gtqfzijrol.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.tianlin.xyz/gtrgrycjjt.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.hongshengwenyu.top/gtdawbpbqx.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.zhengqikj.top/gtceftzedr.html

[O03] 加锁保护共享数据
来源：http://hz.dianchejie.cn/gtntftrokg.html

Py:   with lock: shared += 1
来源：http://hz.ybcxt.top/gtdedokscu.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.tian-w.cn/gtubcpmlmy.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.zhoulong.xyz/gtvgywxbmz.html

TS:   // 同 JS
来源：http://hz.jqgufenzy.top/gtmwcmlepg.html

Java: synchronized (this) { shared++; }
来源：http://hz.dianchejie.cn/gtbqgsdhzw.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.yuanzhike.top/gtqriwkdeq.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.jinqigfzy.top/gteqgtrmxr.html

C#:   lock (gate) { shared++; }
来源：http://hz.zhongyouzk.top/gtimllmkvn.html

[O04] 定义异步函数并等待
来源：http://hz.yj20258.top/gtzrpmbftr.html

Py:   async def f():⏎    await g()
来源：http://hz.yuxming.cn/gtveirygsh.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.52xcode.cn/gtzhegvzwi.html

JS:   async function f() { await g(); }
来源：http://hz.wangdashe.top/gtygucxall.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.yueranfly.top/gtoktokjdp.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.vqdsnc.cn/gtcahcqpjl.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.ybcxt.top/gtprqcdepz.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.yvedp.cn/gtnyodfeos.html

C#:   async Task F() { await G(); }
来源：http://hz.cucudq.cn/gtixnukcng.html

[O05] 并发执行并等待全部完成
来源：http://hz.cqqwz.cn/gtggojmiha.html

Py:   asyncio.gather(*tasks)
来源：http://hz.pengpengdd.cyou/gtgzrnfcpg.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.tianlin.xyz/gtbekkhopn.html

JS:   await Promise.all(tasks)
来源：http://hz.pycfn.com/gturuernus.html

TS:   await Promise.all(tasks)
来源：http://hz.yangfankeji.com/gtksavmukh.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.zhengqikj.top/gtiznzxbjm.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.yuanzhike.top/gtakwwslxg.html

Ruby: threads.map(&:join)
来源：http://hz.gotoacloud.top/gtlyudwrwg.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.zdqjudy.top/gtfyxnhzfu.html

[O06] 使用进程池
来源：http://hz.ydjk.org.cn/gttfacqaxf.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.havefunace.top/gtgodyquky.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.dashuyun.cn/gteitcmxyx.html

JS:   // child_process / cluster 模块
来源：http://hz.ivvv.top/gtrnjyutkl.html

TS:   // child_process / cluster 模块
来源：http://hz.c1oappe.top/gttzenfpzs.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.sysykeji.top/gtkpalptgp.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.hfpthk.cn/gtjezzofjb.html

Ruby: // fork 块
来源：http://hz.fengsongda.top/gtkckfnxqc.html

C#:   Parallel.For
来源：http://hz.yongpay.top/gtwpqqnlcq.html

================================================================================
来源：http://hz.jinqigufen.top/gtcrvmqelp.html

P. 常用工具函数
来源：http://hz.jyoumei.cn/gtxsorqdjz.html

================================================================================
来源：http://hz.hnxiangtu.top/gtpgcewppb.html

[P01] 生成 UUID
来源：http://hz.dashuyun.cn/gtdijbllso.html

Py:   str(uuid.uuid4())
来源：http://hz.nanxuanxn.top/gttqitwvwn.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.daria6918.cn/gtfjjtqdng.html

JS:   crypto.randomUUID()
来源：http://hz.yangfankeji.com/gtykjxajug.html

TS:   crypto.randomUUID()
来源：http://hz.zhengqikj.top/gtlcdojcxa.html

Java: UUID.randomUUID().toString()
来源：http://hz.aizwys.cn/gtxksrlkiy.html

Go:   // 用 github.com/google/uuid
来源：http://hz.jqgfzy.top/gtpwbfqbqd.html

Ruby: SecureRandom.uuid
来源：http://hz.xuetiantiany.cn/gtueeqybjb.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.hongshengwenyu.top/gtemhzlgur.html

[P02] MD5 / SHA256 摘要
来源：http://hz.svipenyu.cn/gthgkhhlfc.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.yj20258.top/gtczwgwfzn.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.yj202588.top/gtqnlvtyon.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.sxryk.cn/gtzfudaino.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.chenzaomai.com/gtpospbeht.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.sufxvd.cn/gtyvoxqxkx.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.shangyingyoupin.top/gtgvnhzibh.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.cdnleiting.top/gteuykpsxu.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.andypj.xyz/gtndfvuuej.html

[P03] 生成短随机字符串
来源：http://hz.svipenyu.cn/gtarsxrgwk.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.xylfe.cn/gtcgabkjla.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.wangshuangyany.cn/gtwyzlutwu.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.meibo888.top/gtlaybfvbh.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.yuxming.cn/gtancrclat.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.yj202588.top/gtobggcehp.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.zhengqikj.top/gtkyxuatyy.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.gogol.net.cn/gtcrjgcvqb.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.havefunace.top/gtmsafsljy.html

[P04] 求长度
来源：http://hz.ivvv.top/gtmbkntauw.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.jqgfzy.top/gtjbazjlxx.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.tian-w.cn/gtniexzxwb.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.hywenlv.cn/gtswcdsedx.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.gotoacloud.top/gtfjgrqmes.html

Java: list.size();  map.size();  s.length()
来源：http://hz.xylfe.cn/gtsgrntkaa.html

Go:   len(arr);  len(m)
来源：http://hz.zycfv.cn/gtmqtdarar.html

Ruby: x.length;  x.size
来源：http://hz.kuanghao11.cn/gtvfvhgxaw.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.zhijiandao.cn/gtxpbhouey.html

[P05] 判断两个对象内容是否相等
来源：http://hz.shanyushiyangtech.top/gtllpgparx.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.tian-w.cn/gtnbsoknrw.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.jinqigfzy.top/gtqvbpwozf.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.yj20258.top/gtjbnlsnmq.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.shanyushiyangkeji.top/gtdlctnavy.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.0kj1m.cn/gtugqzgbqm.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.daria6918.cn/gtrahwxbun.html

Ruby: a == b
来源：http://hz.jiagoushi.top/gtcbppnlbd.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.gotoacloud.top/gtygnuvwgn.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.gogol.net.cn/gtevbmgkhn.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.daxiang520.top/gtvrokhxrz.html

PHP:  if (empty($x)) {}
来源：http://hz.jinqigufen.top/gthjgrebav.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.zhaomingkeji.xyz/gtnyuusdlk.html

TS:   if (x == null) {}
来源：http://hz.andypj.xyz/gtutnkjcua.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.ivvv.top/gtlpjdyhnf.html

Go:   if x == nil {}
来源：http://hz.iojbl.cn/gtgotjpzan.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.gaohongyu789.top/gtmzsirrao.html

C#:   if (x is null) {}
来源：http://hz.guannengcc.top/gtxkfzarmy.html

[P07] 防抖与节流
来源：http://hz.zhaomingkeji.xyz/gtcdvffmgl.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.haohaochexian.top/gtroatmoqk.html

PHP:  // 手写时间戳比较
来源：http://hz.vqdsnc.cn/gtrvluwihh.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.aizwys.cn/gtfunyhuzo.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.cdnleiting.top/gtkgmegtbq.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.nwbrower.top/gtpfanlimy.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.smart0.xyz/gtinfapque.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.gzhubu.top/gtuldtqyox.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.xinyue.icu/gtfnzliwsa.html

[P08] 处理浮点精度问题
来源：http://hz.yj20258.top/gtqsroxvtp.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.yj20258.top/gtihixmaes.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.tanke756.top/gtmgjzvsui.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.xingfuxueyuan.xyz/gtbnmlhqlt.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.xingfuxueyuan.xyz/gtqhlyhppf.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.nanxinkj.top/gtgwsjabtb.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.shanyushiyangkeji.top/gtvbuyilrt.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.zdqjudy.top/gtagkonliu.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.aizwys.cn/gtqfknspsj.html

================================================================================
来源：http://hz.smart0.xyz/gtehdlgorq.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.xziqi.cn/gtjspqyenz.html

================================================================================
来源：http://hz.gogol.net.cn/gtyonznbhs.html

[Q01] 创建表
来源：http://hz.zhijiandao.cn/gtbihqrflg.html

CREATE TABLE users (
来源：http://hz.smart0.xyz/gtshunevsn.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.redwolf501.top/gthercdjri.html

name VARCHAR(50) NOT NULL,
来源：http://hz.zhoulong.xyz/gtyqtyizub.html

email VARCHAR(100) UNIQUE,
来源：http://hz.52xcode.cn/gtldihbhdo.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.zhaomingkeji.xyz/gtodhtvzdt.html

);
来源：http://hz.9152youxi.cn/gtmsboktcr.html

[Q02] 创建带外键的表
来源：http://hz.dashuyun.cn/gtgrghuvta.html

CREATE TABLE orders (
来源：http://hz.sysykeji.top/gttnlgqrzk.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.jinghuilouyu.cn/gtjphurywx.html

user_id INT NOT NULL,
来源：http://hz.quarkkingdee.top/gtwpktewex.html

amount DECIMAL(10, 2),
来源：http://hz.shanyushiyangkeji.top/gtfkrikojs.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.xuetiantiany.cn/gtwdbxzkye.html

);
来源：http://hz.gotoacloud.top/gtfbdqqcok.html

[Q03] 增加列
来源：http://hz.svipenyu.cn/gtakpnrqmd.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.yvedp.cn/gtavawxqzm.html

[Q04] 修改列类型
来源：http://hz.yj20258.top/gtlyupomql.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.316326.xyz/gtnaoyexlh.html

[Q05] 重命名列
来源：http://hz.jinghuilouyu.cn/gtsccoebdh.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.yvedp.cn/gtgaoqpemi.html

[Q06] 删除列
来源：http://hz.jianghu66.top/gtzigjdyuh.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.havefunace.top/gtbbjtmdbi.html

[Q07] 删除表
来源：http://hz.316326.xyz/gtwjckgxpb.html

DROP TABLE IF EXISTS orders;
来源：http://hz.9152youxi.cn/gtjgocwzrl.html

[Q08] 创建普通索引
来源：http://hz.snrcjt.cn/gtzibvlkff.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.zhengqikj.top/gtocythwgg.html

[Q09] 创建唯一索引
来源：http://hz.hywenlv.cn/gtgdawzkby.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.zhaomingkeji.xyz/gtjtjfwxji.html

[Q10] 插入单行
来源：http://hz.jinqigufen.top/gtalbvwfpo.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.hongshengwenyu.top/gtosqwynyb.html

[Q11] 一次插入多行
来源：http://hz.9152youxi.cn/gtixknjizf.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.9152youxi.cn/gtpanrpipn.html

[Q12] 插入后取自增 ID
来源：http://hz.ppjwa.cn/gtswsjlbxp.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.fengsongda.top/gtdeftvgmc.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.cqqwz.cn/gtmbwduxjk.html

[Q13] 忽略重复插入
来源：http://hz.nanxuanxn.top/gtaxjuoxbl.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.cheryme.top/gtexfsdsjw.html

[Q14] 存在则更新（upsert）
来源：http://hz.nanxuanxn.top/gtjfhhmuzw.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.ybcxt.top/gthvtwxwmj.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.zhengqikj.top/gtwvqsbkau.html

[Q15] 查询全部
来源：http://hz.jinyuanbaomall.cn/gtrbxhdhgj.html

SELECT * FROM users;
来源：http://hz.zhixingplan.top/gthqxdzvlx.html

[Q16] 查询指定列
来源：http://hz.birdmap.top/gtuzcnkszz.html

SELECT id, name FROM users;
来源：http://hz.yuanzhike.top/gtquhldnlv.html

[Q17] 条件查询
来源：http://hz.kuanghao11.cn/gtbjfuvfae.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.ydjk.org.cn/gtqvlkjmei.html

[Q18] 模糊匹配
来源：http://hz.sysykeji.top/gthfwkeupg.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.jinyuanbaomall.cn/gtbtysbxxj.html

[Q19] 范围查询
来源：http://hz.ppjwa.cn/gtjqjnhewg.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.jinghuilouyu.cn/gtfdolzitb.html

[Q20] IN 列表
来源：http://hz.jinqigfzy.top/gtdvlfydsj.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.fengsongda.top/gtifssnlnc.html

[Q21] 空值判断
来源：http://hz.yuxming.cn/gtpqnghdmr.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.yj20258888.top/gtsjzxooet.html

[Q22] 排序
来源：http://hz.hnxiangtu.top/gtpzgwrvsb.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.zhijiandao.cn/gtiltqjgnt.html

[Q23] 分页
来源：http://hz.jiagoushi.top/gtmqokfbfk.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.zhengqikj.top/gtnldpyadl.html

[Q24] 去重
来源：http://hz.jyoumei.cn/gtyfrkatnw.html

SELECT DISTINCT city FROM users;
来源：http://hz.jinqigufen.top/gtnmztkvuz.html

[Q25] 只取前 N 条
来源：http://hz.snrcjt.cn/gthecgjcfi.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.shanyushiyangtech.top/gtsafwetcm.html

[Q26] 计数
来源：http://hz.c1oappe.top/gtkdpftapt.html

SELECT COUNT(*) FROM users;
来源：http://hz.mhx1999.top/gtmonozusb.html

[Q27] 条件计数
来源：http://hz.zhijiandao.cn/gtavrayxax.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.zycfv.cn/gtrewmeyie.html

[Q28] 求和与平均
来源：http://hz.kuanghao11.cn/gtgqdamhlw.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.svipenyu.cn/gtxtirqbmu.html

[Q29] 最大最小值
来源：http://hz.daria6918.cn/gtddkevxlc.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.xingfuxueyuan.xyz/gtbgxyvsst.html

[Q30] 分组统计
来源：http://hz.52xcode.cn/gtyfqxorcd.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.zhongyouzk.top/gtddvlagnt.html

[Q31] 分组后过滤
来源：http://hz.jqgufenzy.top/gtmiqubdnl.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.zhengqikj.top/gttwwoqpky.html

[Q32] 分组拼接字符串
来源：http://hz.ehwqpu.com/gtyyqlwtce.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.gzhubu.top/gtkjpehawf.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.nanxinkj.top/gtkhaujily.html

[Q33] 多列分组
来源：http://hz.cashguo.top/gtunpcliap.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.tian-w.cn/gtzzwhsuvp.html

[Q34] 每组取第一条
来源：http://hz.snrcjt.cn/gtrhljkxoj.html

SELECT * FROM (
来源：http://hz.shuidangran.top/gtxnmxdpcv.html


<!-- 参考信息 -->