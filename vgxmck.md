代发 wailian999

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.hnqzz.top/gtuqlbdvwy.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.yueranfly.top/gtvtvhbaoz.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.wangshuangyany.cn/gtbssmzzai.html

Go:   slices.Sort(arr)
来源：http://hz.jlsjyb.cn/gtwdpbnubo.html

Ruby: arr.sort
来源：http://hz.sufxvd.cn/gtpnsontbv.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.xziqi.cn/gtiepdpvqf.html

[N03] 快速排序（分治示例）
来源：http://hz.c1oappe.top/gtpgefwitg.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.zhixingplan.top/gtyrfobtoz.html

PHP:  // 递归实现，或用 usort
来源：http://hz.dianchejie.cn/gtdtrlqjwv.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.hnxiangtu.top/gtqkbsuqml.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.ydzc1.top/gtwxwlegjh.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.jqgfzy.top/gtsdyuxqqn.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.guowangkeji.top/gtidjsnppr.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.guowangkeji.top/gtwuccovrg.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.yj202588.top/gtexhvhqgx.html

[N04] 斐波那契数列
来源：http://hz.chenlongwang.top/gtnawevreu.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.jinqigfzy.top/gtnteppoug.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.chenzaomai.com/gtmqltgxfp.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.hnxiangtu.top/gtictlssgn.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.yj20258.top/gtzljtlgwn.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.jinyuanbaomall.cn/gteaeltgwi.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.zhaomingkeji.xyz/gtrrhndlzn.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.gogol.net.cn/gtyppuyybx.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.hysaishi.cn/gtalpjmlfe.html

[N05] 最大公约数
来源：http://hz.daxiang520.top/gtgrsoumzx.html

Py:   math.gcd(a, b)
来源：http://hz.shangyingyoupin.top/gtmtyasxds.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.dianchejie.cn/gtknmzvhgx.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.yonumen.top/gthzzplyin.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.gogol.net.cn/gtmiyfljdh.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.gotoacloud.top/gtykfqzwlu.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.snrcjt.cn/gtvlkvciya.html

Ruby: a.gcd(b)
来源：http://hz.zhijiandao.cn/gtapszupat.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.pengpengdd.cyou/gtxizgfkvo.html

[N06] 判断回文字符串
来源：http://hz.svipenyu.cn/gtagvhhgan.html

Py:   s == s[::-1]
来源：http://hz.ehwqpu.com/gtimkxualm.html

PHP:  $s === strrev($s);
来源：http://hz.jianghu66.top/gtoyloqgco.html

JS:   s === [...s].reverse().join("")
来源：http://hz.shanyushiyangkeji.top/gtqobdwkzg.html

TS:   s === [...s].reverse().join("")
来源：http://hz.cucudq.cn/gtfcjgbvmq.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.sweek.top/gtxepwwnjh.html

Go:   // 双指针从两端比较
来源：http://hz.daria6918.cn/gtegvinmrt.html

Ruby: s == s.reverse
来源：http://hz.gzhubu.top/gtwjcqzumj.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.shuidangran.top/gtgbprjzlp.html

[N07] 两数之和（返回下标）
来源：http://hz.chenzaomai.com/gtsepxvsuv.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.sufxvd.cn/gtaubkexxc.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.gogol.net.cn/gtrzpddhbo.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.jqgufenzy.top/gttugmdtth.html

TS:   // 手写 Map<string, number>
来源：http://hz.meibo888.top/gtzovieumo.html

Java: // 手写 HashMap
来源：http://hz.shanyushiyangtech.top/gtpqktgdjo.html

Go:   // 手写 map[int]int
来源：http://hz.zhijiandao.cn/gtrmgctlkb.html

Ruby: // 手写 Hash
来源：http://hz.svipenyu.cn/gtficonnqm.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.yueranfly.top/gtvsotvhlk.html

[N08] 生成全排列
来源：http://hz.chenzaomai.com/gtqthmfheu.html

Py:   itertools.permutations(arr)
来源：http://hz.shanyushiyangtech.top/gtmoqxdpkz.html

PHP:  // 手写递归交换
来源：http://hz.c1oappe.top/gtutjzpfku.html

JS:   // 手写回溯递归
来源：http://hz.zhixingplan.top/gtjsyvyiwj.html

TS:   // 手写回溯递归
来源：http://hz.dashuyun.cn/gtpfptyzvd.html

Java: // 手写回溯递归
来源：http://hz.yangfankeji.com/gtpvjoyvaq.html

Go:   // 手写回溯递归
来源：http://hz.jyoumei.cn/gtigeiozut.html

Ruby: arr.permutation.to_a
来源：http://hz.wangshuangyany.cn/gtwtxhawfh.html

C#:   // 手写回溯递归
来源：http://hz.aibaodan.cn/gthvdtrvjo.html

[N09] 栈与队列
来源：http://hz.ydzc1.top/gtaggwtnxi.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.shzxlz.cn/gtyrbftxya.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.shzxlz.cn/gtangzjhyi.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.shanyushiyangtech.top/gteqsvquon.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.chenjidiqi.icu/gtzwelbiyl.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.ivvv.top/gtevdonavh.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.iojbl.cn/gtcngnfgby.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.jianghu66.top/gtlkznukwo.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.gaohongyu789.top/gtvqvcbvdh.html

[N10] 链表节点定义
来源：http://hz.zhijiandao.cn/gtjsinjpuw.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.mhx1999.top/gtossepghv.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.haohaochexian.top/gtofyfomhq.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.pengpengdd.cyou/gtgggzdjvf.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.shanyushiyangkeji.top/gtcaaywcib.html

Java: class Node { int v; Node next; }
来源：http://hz.wangdashe.top/gtragtklqf.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.wangshuangyany.cn/gtaiuxgymt.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.gzhubu.top/gtdwquimwn.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.jlsjyb.cn/gtbkbdhkfe.html

[N11] 二叉树中序遍历
来源：http://hz.fzhhl.top/gtjfxowbrg.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.kuanghao11.cn/gtmgxsywvm.html

PHP:  // 手写递归函数
来源：http://hz.jinyuanbaomall.cn/gtwsklgtzv.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.jinghuilouyu.cn/gtdowjevhs.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.andypj.xyz/gtlmqsbacs.html

Java: // 手写递归
来源：http://hz.chenzaomai.com/gtuzfxvcsx.html

Go:   // 手写递归
来源：http://hz.hammf.cn/gtrmasxyih.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.guowangkeji.top/gtaflhujug.html

C#:   // 手写递归
来源：http://hz.kuanghao11.cn/gttxiysqis.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.hnqzz.top/gtajkfdvif.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.zdqjudy.top/gtxdnxjkjo.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.sufxvd.cn/gtsqrmofvq.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.aibaodan.cn/gtliylyajk.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.gaohongyu789.top/gtlqommpzn.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.snrcjt.cn/gtahmbgwpu.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.dianchejie.cn/gtrzuzysbv.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.tanke756.top/gtmuqigcpa.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.ivvv.top/gtdpauadsr.html

================================================================================
来源：http://hz.jinqigufen.top/gtijoszzod.html

O. 并发与异步
来源：http://hz.bjfxy.top/gtpmijechu.html

================================================================================
来源：http://hz.jinqigfzy.top/gttbrpytdo.html

[O01] 启动一个线程
来源：http://hz.mhx1999.top/gtjtgipxpq.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.zhiwuduotai.top/gtfueafrwb.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.xylfe.cn/gtttbnphqf.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.sweek.top/gtjiksqaas.html

TS:   // 同 JS
来源：http://hz.dashuyun.cn/gtqfbalumb.html

Java: new Thread(() -> f()).start()
来源：http://hz.zhoulong.xyz/gtibfbkfla.html

Go:   go f()
来源：http://hz.wangdashe.top/gtqgrsnmfi.html

Ruby: Thread.new { f }
来源：http://hz.316326.xyz/gtcfwiovii.html

C#:   Task.Run(() => F());
来源：http://hz.zhengqikj.top/gtxlmmhfgl.html

[O02] 使用线程池
来源：http://hz.yj20258.top/gtmnsiarqj.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.xylfe.cn/gtvixmsxia.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.wangdashe.top/gtjgolhwvx.html

JS:   // worker_threads 线程池
来源：http://hz.yvedp.cn/gtwrpwtxxo.html

TS:   // worker_threads 线程池
来源：http://hz.sysykeji.top/gtecspgcqd.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.cheryme.top/gtwwsglcpu.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.yonumen.top/gtwmxsqrkb.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.redwolf501.top/gtalqhdncv.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.zhengqikj.top/gtetoxjmds.html

[O03] 加锁保护共享数据
来源：http://hz.tanke756.top/gtvseurojo.html

Py:   with lock: shared += 1
来源：http://hz.iojbl.cn/gtshkhcwsp.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.0kj1m.cn/gtoigyqaux.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.zhaomingkeji.xyz/gthspyxdvv.html

TS:   // 同 JS
来源：http://hz.pengpengdd.cyou/gtkkeoebdy.html

Java: synchronized (this) { shared++; }
来源：http://hz.shangyingyoupin.top/gtefdgdfom.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.jqgufenzy.top/gtwaxpdgou.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.hysaishi.cn/gtxpfswfzr.html

C#:   lock (gate) { shared++; }
来源：http://hz.shzxlz.cn/gtocujfarm.html

[O04] 定义异步函数并等待
来源：http://hz.haohaochexian.top/gtcklkxuha.html

Py:   async def f():⏎    await g()
来源：http://hz.jinqigfzy.top/gtbwkbsnoy.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.zhiwuduotai.top/gtwrnnfdim.html

JS:   async function f() { await g(); }
来源：http://hz.cqqwz.cn/gtfedkmwxd.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.yueranfly.top/gtnklztkmm.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.tianlin.xyz/gtqhfacbdp.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.redwolf501.top/gttlzmjubm.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.daria6918.cn/gteyxnkkqe.html

C#:   async Task F() { await G(); }
来源：http://hz.bjfxy.top/gttwugsjyv.html

[O05] 并发执行并等待全部完成
来源：http://hz.jqgfzy.top/gtqkuiduse.html

Py:   asyncio.gather(*tasks)
来源：http://hz.chenjidiqi.icu/gterqkpwgt.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.ppjwa.cn/gtgqfvdyxz.html

JS:   await Promise.all(tasks)
来源：http://hz.birdmap.top/gtzzdhglcm.html

TS:   await Promise.all(tasks)
来源：http://hz.zdqjudy.top/gtghgjhfnt.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.snrcjt.cn/gtbsuzwmwi.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.ehwqpu.com/gtojqeifgv.html

Ruby: threads.map(&:join)
来源：http://hz.jinghuilouyu.cn/gtltbowsri.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.andypj.xyz/gthfbdcfts.html

[O06] 使用进程池
来源：http://hz.shanyushiyangtech.top/gtfnfzjsli.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.svipenyu.cn/gtztaqwgtz.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.tanke756.top/gtgsmiveja.html

JS:   // child_process / cluster 模块
来源：http://hz.sweek.top/gtuxmpfurl.html

TS:   // child_process / cluster 模块
来源：http://hz.ivvv.top/gtclygxrul.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.wangshuangyany.cn/gtbodgssor.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.tianlin.xyz/gtyrhjshxb.html

Ruby: // fork 块
来源：http://hz.ivvv.top/gtavafzsfq.html

C#:   Parallel.For
来源：http://hz.snrcjt.cn/gtmczjepru.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtyzkoosqv.html

P. 常用工具函数
来源：http://hz.tanke756.top/gtjetkjwjm.html

================================================================================
来源：http://hz.yj20258.top/gttmuumeot.html

[P01] 生成 UUID
来源：http://hz.yuanzhike.top/gtvecbexvx.html

Py:   str(uuid.uuid4())
来源：http://hz.xuanzx.com/gthfhcelvm.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.sysykeji.top/gtzzedmzpl.html

JS:   crypto.randomUUID()
来源：http://hz.ydzc1.top/gteputydbj.html

TS:   crypto.randomUUID()
来源：http://hz.hysaishi.cn/gtsxuvadhx.html

Java: UUID.randomUUID().toString()
来源：http://hz.zhiwuduotai.top/gtxmlxwyuk.html

Go:   // 用 github.com/google/uuid
来源：http://hz.birdmap.top/gtnfbqboio.html

Ruby: SecureRandom.uuid
来源：http://hz.bjfxy.top/gttbersont.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.kuanghao11.cn/gtmyfrujqr.html

[P02] MD5 / SHA256 摘要
来源：http://hz.snrcjt.cn/gtlnvuifup.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.sweek.top/gtlmcahfye.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.daxiang520.top/gtedyqbcmu.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.pengpengdd.cyou/gtsbahwcui.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.bjfxy.top/gtrdgyrhbl.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.ehwqpu.com/gtmznpgkin.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.chenlongwang.top/gtdckrpaij.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.sysykeji.top/gtjwgjeevd.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.hammf.cn/gtlrcopuad.html

[P03] 生成短随机字符串
来源：http://hz.hongshengwenyu.top/gtilprzssy.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.zhijiandao.cn/gtafwrxwpw.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.chenjidiqi.icu/gtsmouqpuc.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.daria6918.cn/gtkeicnkfe.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.jlsjyb.cn/gtizbhyijk.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.nanxuanxn.top/gtpqpjgcez.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.gogol.net.cn/gttltnoqvk.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.iojbl.cn/gtqadocxed.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.jqgufenzy.top/gtlxqcmbme.html

[P04] 求长度
来源：http://hz.gaohongyu789.top/gtlqsrrgmy.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.jinghuilouyu.cn/gtcnvjelkg.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.yueranfly.top/gtcjdeixbj.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.fzhhl.top/gtfpbvhrcz.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.0kj1m.cn/gtgykfcyku.html

Java: list.size();  map.size();  s.length()
来源：http://hz.bjfxy.top/gtscefbeem.html

Go:   len(arr);  len(m)
来源：http://hz.yangfankeji.com/gtfytqxktg.html

Ruby: x.length;  x.size
来源：http://hz.zhengqikj.top/gtcxrbryab.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.yj20258.top/gtknsavnkd.html

[P05] 判断两个对象内容是否相等
来源：http://hz.ywan-chungtsiang.top/gtnpamckpb.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.cheryme.top/gtmllrunmw.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.sufxvd.cn/gtotfshwtx.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.fengsongda.top/gtmynedrzz.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.jinghuilouyu.cn/gtwdplibsc.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.xinyue.icu/gtrjzoqpgl.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.chenlongwang.top/gtizzzleus.html

Ruby: a == b
来源：http://hz.feifeiyinyue.top/gthuklsrao.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.fzhhl.top/gtxxbudgql.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.cashguo.top/gthbangmui.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.zhiwuduotai.top/gtekqbjqjt.html

PHP:  if (empty($x)) {}
来源：http://hz.ydjk.org.cn/gtqfjphxea.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.hysaishi.cn/gtihlkyyrz.html

TS:   if (x == null) {}
来源：http://hz.c1oappe.top/gtumyjzwvo.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.xingfuxueyuan.xyz/gttlyysvxg.html

Go:   if x == nil {}
来源：http://hz.yonumen.top/gtebirobyz.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.yangfankeji.com/gtyjdxtgdd.html

C#:   if (x is null) {}
来源：http://hz.dianchejie.cn/gtactpjvio.html

[P07] 防抖与节流
来源：http://hz.svipenyu.cn/gtgafwoegq.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.jianghu66.top/gtpqrysrot.html

PHP:  // 手写时间戳比较
来源：http://hz.hywenlv.cn/gticfeydcv.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.daxiang520.top/gtmvzbbujw.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.ivvv.top/gtbslewrvp.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.aibaodan.cn/gtafbudmez.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.sweek.top/gtenutgitw.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.gotoacloud.top/gtkolinaac.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.yangfankeji.com/gtfwbicddi.html

[P08] 处理浮点精度问题
来源：http://hz.shanyushiyangkeji.top/gtxdpnglnb.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.ehwqpu.com/gthgyhwwsk.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.wangshuangyany.cn/gteubertiq.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.nanxuanxn.top/gtoignrnku.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.xziqi.cn/gthfpfveyt.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.xziqi.cn/gtmelgocvk.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.fzhhl.top/gtmbirboph.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.xuanzx.com/gtquwfazzw.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.haohaochexian.top/gtiyoulfoh.html

================================================================================
来源：http://hz.yuanzhike.top/gtwtavpczs.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.ydzc1.top/gthntskojn.html

================================================================================
来源：http://hz.jlsjyb.cn/gtvqwggoyy.html

[Q01] 创建表
来源：http://hz.chenzaomai.com/gtggqdsmip.html

CREATE TABLE users (
来源：http://hz.jinyuanbaomall.cn/gtwdzmfiuc.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.hnxiangtu.top/gtzxyvmtgn.html

name VARCHAR(50) NOT NULL,
来源：http://hz.zdqjudy.top/gtuwgsqdtx.html

email VARCHAR(100) UNIQUE,
来源：http://hz.gotoacloud.top/gttmwpgqgq.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.chenzaomai.com/gtnjpwnpko.html

);
来源：http://hz.tian-w.cn/gtlwhfjmgk.html

[Q02] 创建带外键的表
来源：http://hz.daxiang520.top/gtutkpuqab.html

CREATE TABLE orders (
来源：http://hz.nanxinkj.top/gtdcwegreo.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.gotoacloud.top/gthggtrqwe.html

user_id INT NOT NULL,
来源：http://hz.nanxinkj.top/gtdzkjocwj.html

amount DECIMAL(10, 2),
来源：http://hz.tanke756.top/gtpinebtop.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.yongpay.top/gtjgzzkzko.html

);
来源：http://hz.ydzc1.top/gtyzgwfnzb.html

[Q03] 增加列
来源：http://hz.vqdsnc.cn/gtqisggrtf.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.fzhhl.top/gtclogfpjr.html

[Q04] 修改列类型
来源：http://hz.gzhubu.top/gtszeqjlvi.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.birdmap.top/gtdxbumjsj.html

[Q05] 重命名列
来源：http://hz.9152youxi.cn/gtnfybkfru.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.jlsjyb.cn/gtmyxqpsjg.html

[Q06] 删除列
来源：http://hz.guowangkeji.top/gtortsdeis.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.jinqigufen.top/gtmssxifku.html

[Q07] 删除表
来源：http://hz.gogol.net.cn/gtatdlxpkk.html

DROP TABLE IF EXISTS orders;
来源：http://hz.pycfn.com/gtzyxvovup.html

[Q08] 创建普通索引
来源：http://hz.smart0.xyz/gtoncqjnmc.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.fengsongda.top/gtzgxmhyvq.html

[Q09] 创建唯一索引
来源：http://hz.guowangkeji.top/gteprzgfjl.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.dianchejie.cn/gtqzyilkgn.html

[Q10] 插入单行
来源：http://hz.gaohongyu789.top/gtqvlctlhv.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.daria6918.cn/gtqaqclxct.html

[Q11] 一次插入多行
来源：http://hz.zhixingplan.top/gthasbqvll.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.jlsjyb.cn/gtnbfgywss.html

[Q12] 插入后取自增 ID
来源：http://hz.yangfankeji.com/gtegpnrgvl.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.ybcxt.top/gtwvzrnwhw.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.hnxiangtu.top/gtybyaqohg.html

[Q13] 忽略重复插入
来源：http://hz.meibo888.top/gtjjxrpasl.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.cqqwz.cn/gtdcuclekq.html

[Q14] 存在则更新（upsert）
来源：http://hz.yonumen.top/gttlvkwfhy.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.yuxming.cn/gtjlyhqnva.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.sweek.top/gtmuftcwoy.html

[Q15] 查询全部
来源：http://hz.vqdsnc.cn/gtmlqdyriq.html

SELECT * FROM users;
来源：http://hz.yuanzhike.top/gtwuajhqdu.html

[Q16] 查询指定列
来源：http://hz.aizwys.cn/gtaxixpxbq.html

SELECT id, name FROM users;
来源：http://hz.cucudq.cn/gtvwxrlxmq.html

[Q17] 条件查询
来源：http://hz.jinqigfzy.top/gthorgpqto.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.316326.xyz/gtihzhmash.html

[Q18] 模糊匹配
来源：http://hz.52xcode.cn/gtlfrkljdm.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.zdqjudy.top/gtaejalsiw.html

[Q19] 范围查询
来源：http://hz.ydjk.org.cn/gtetrwtbqo.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.aibaodan.cn/gtpwjlnage.html

[Q20] IN 列表
来源：http://hz.redwolf501.top/gtpumdzjrv.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.tianlin.xyz/gtnrwlkvpl.html

[Q21] 空值判断
来源：http://hz.jianghu66.top/gthnhqdfgy.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.xuanzx.com/gtuoukzyjh.html

[Q22] 排序
来源：http://hz.xuetiantiany.cn/gtcoifccci.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.pycfn.com/gtuhqltmba.html

[Q23] 分页
来源：http://hz.bjfxy.top/gtbqkygmqe.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.zdqjudy.top/gtlwcwrzvm.html

[Q24] 去重
来源：http://hz.quarkkingdee.top/gtpsfbbhzl.html

SELECT DISTINCT city FROM users;
来源：http://hz.ivvv.top/gtqyzhsaly.html

[Q25] 只取前 N 条
来源：http://hz.meibo888.top/gtiapniipr.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.gzhubu.top/gtjmyekive.html

[Q26] 计数
来源：http://hz.hongshengwenyu.top/gtnvtqkrif.html

SELECT COUNT(*) FROM users;
来源：http://hz.redwolf501.top/gtdhmvbuuq.html

[Q27] 条件计数
来源：http://hz.chenzaomai.com/gtycctccle.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.xuetiantiany.cn/gtskndjscx.html

[Q28] 求和与平均
来源：http://hz.svipenyu.cn/gtooafipzr.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.gaohongyu789.top/gtunilihil.html

[Q29] 最大最小值
来源：http://hz.kuanghao11.cn/gttsekmvzy.html


<!-- 参考信息 -->