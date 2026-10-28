代发 wailian999

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.zhaomingkeji.xyz/gtukhbuxhk.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.dianchejie.cn/gtvlqvmqkn.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.aizwys.cn/gttyshxbnj.html

[N04] 斐波那契数列
来源：http://hz.0kj1m.cn/gtcbxkxncp.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.xinyue.icu/gtxauxoabv.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.hnxiangtu.top/gtmedcgnlo.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.guannengcc.top/gtjqkpkijt.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.redwolf501.top/gtkjogyhmh.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.c1oappe.top/gtrcqedfmi.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.tian-w.cn/gtvxtzdcbl.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.feifeiyinyue.top/gtixuyhiwz.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.birdmap.top/gtpeuftuwf.html

[N05] 最大公约数
来源：http://hz.chenjidiqi.icu/gtvvowgnhp.html

Py:   math.gcd(a, b)
来源：http://hz.yuxming.cn/gtayishmig.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.gzhubu.top/gtuyxkxbyx.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.gogol.net.cn/gtvtsqbjpp.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.snrcjt.cn/gtpberfrgv.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.zhongyouzk.top/gtchseyrde.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.jqgfzy.top/gtoygloacn.html

Ruby: a.gcd(b)
来源：http://hz.jiagoushi.top/gtbvjgwass.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.0kj1m.cn/gtpfjysolh.html

[N06] 判断回文字符串
来源：http://hz.jqgfzy.top/gtlzikpfar.html

Py:   s == s[::-1]
来源：http://hz.haohaochexian.top/gtdgbamfwo.html

PHP:  $s === strrev($s);
来源：http://hz.bjfxy.top/gtknmripiu.html

JS:   s === [...s].reverse().join("")
来源：http://hz.9152youxi.cn/gtgxsbhpkl.html

TS:   s === [...s].reverse().join("")
来源：http://hz.dashuyun.cn/gtqehzuauo.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.jlsjyb.cn/gtnxktisum.html

Go:   // 双指针从两端比较
来源：http://hz.jinqigfzy.top/gthokrifgz.html

Ruby: s == s.reverse
来源：http://hz.meibo888.top/gtxeffovoj.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.vqdsnc.cn/gtfnvwpqeu.html

[N07] 两数之和（返回下标）
来源：http://hz.gaohongyu789.top/gttejwvznf.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.gzhubu.top/gtvzhtcuqv.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.jiagoushi.top/gteopcrczi.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.yanxiufei.cn/gtsuxdozgf.html

TS:   // 手写 Map<string, number>
来源：http://hz.tanke756.top/gtkyvmmukq.html

Java: // 手写 HashMap
来源：http://hz.chenzaomai.com/gtgoqavljx.html

Go:   // 手写 map[int]int
来源：http://hz.guowangkeji.top/gttuqovsrq.html

Ruby: // 手写 Hash
来源：http://hz.tanke756.top/gtgmyqkyus.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.cqqwz.cn/gtrpqubpwg.html

[N08] 生成全排列
来源：http://hz.jlsjyb.cn/gtyjgdrunm.html

Py:   itertools.permutations(arr)
来源：http://hz.ivvv.top/gtuotviqpw.html

PHP:  // 手写递归交换
来源：http://hz.hywenlv.cn/gtdsgjzghq.html

JS:   // 手写回溯递归
来源：http://hz.ywan-chungtsiang.top/gtkewhgbgw.html

TS:   // 手写回溯递归
来源：http://hz.fzhhl.top/gtwufjqzza.html

Java: // 手写回溯递归
来源：http://hz.wangdashe.top/gthjthhfqm.html

Go:   // 手写回溯递归
来源：http://hz.yueranfly.top/gteusqdsad.html

Ruby: arr.permutation.to_a
来源：http://hz.zhijiandao.cn/gtmunwsscb.html

C#:   // 手写回溯递归
来源：http://hz.xingfuxueyuan.xyz/gtuovhjvwy.html

[N09] 栈与队列
来源：http://hz.snrcjt.cn/gtujubuquu.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.jinqigfzy.top/gtkiknefci.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.ybcxt.top/gtxdenbvbs.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.sufxvd.cn/gtncdxrxdr.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.havefunace.top/gtpbuqprea.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.nwbrower.top/gtgtuezgav.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.zhijiandao.cn/gtlonvkeyy.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.snrcjt.cn/gtsmvyehob.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.smart0.xyz/gtvgsikvyg.html

[N10] 链表节点定义
来源：http://hz.ywan-chungtsiang.top/gtpbfqiojf.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.yuanzhike.top/gtqmolgcfd.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.hywenlv.cn/gtytwnpoqz.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.yongpay.top/gthfkmmjve.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.cheryme.top/gtxsooalsf.html

Java: class Node { int v; Node next; }
来源：http://hz.cheryme.top/gtvpfbtcnr.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.yongpay.top/gtyqbzivzq.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.dashuyun.cn/gtnvwsmcys.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.daxiang520.top/gtjkxafjiy.html

[N11] 二叉树中序遍历
来源：http://hz.jyoumei.cn/gtvwqcvwec.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.smart0.xyz/gtftpvvcpc.html

PHP:  // 手写递归函数
来源：http://hz.daria6918.cn/gtyjjifcul.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.gogol.net.cn/gtjcdmqnjc.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.guowangkeji.top/gtkvnsrqcr.html

Java: // 手写递归
来源：http://hz.jinqigfzy.top/gtocdnkniy.html

Go:   // 手写递归
来源：http://hz.gotoacloud.top/gtikuepqjt.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.tanke756.top/gtujtflmpv.html

C#:   // 手写递归
来源：http://hz.hnxiangtu.top/gtjzoiznnv.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.hysaishi.cn/gtkbghjwlg.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.snrcjt.cn/gtxjyqjkhs.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.tian-w.cn/gttgfxylub.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.daxiang520.top/gtdteegizx.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.zhaomingkeji.xyz/gttccljvyh.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.daxiang520.top/gtuocplrzj.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.jiagoushi.top/gtbjkjxret.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.kuanghao11.cn/gtwwikqwat.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.cheryme.top/gthoyjdujp.html

================================================================================
来源：http://hz.tanke756.top/gtouffdbfb.html

O. 并发与异步
来源：http://hz.aibaodan.cn/gtexvqwlnm.html

================================================================================
来源：http://hz.mhx1999.top/gtccraobfg.html

[O01] 启动一个线程
来源：http://hz.pengpengdd.cyou/gturkcgdjc.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.jlsjyb.cn/gtnmdzednx.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.shanyushiyangtech.top/gthmyfjtju.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.daria6918.cn/gticwqlanc.html

TS:   // 同 JS
来源：http://hz.shangyingyoupin.top/gthykpmhaa.html

Java: new Thread(() -> f()).start()
来源：http://hz.sweek.top/gtezxpyyro.html

Go:   go f()
来源：http://hz.quarkkingdee.top/gtyjlwishg.html

Ruby: Thread.new { f }
来源：http://hz.jinqigfzy.top/gtbppjrlvq.html

C#:   Task.Run(() => F());
来源：http://hz.zhongyouzk.top/gtzyvnvart.html

[O02] 使用线程池
来源：http://hz.hnqzz.top/gttzbgcgnz.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.cashguo.top/gtycxuwtfu.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.kuanghao11.cn/gtbrrfjkej.html

JS:   // worker_threads 线程池
来源：http://hz.gaohongyu789.top/gtngzekmjv.html

TS:   // worker_threads 线程池
来源：http://hz.zhoulong.xyz/gtvaznpsbi.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.vqdsnc.cn/gtuulhqinl.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.svipenyu.cn/gttzvvbkpe.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.gzhubu.top/gtfefqkxao.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.jinqigfzy.top/gtxtdvvbjp.html

[O03] 加锁保护共享数据
来源：http://hz.ywan-chungtsiang.top/gthjwawsye.html

Py:   with lock: shared += 1
来源：http://hz.nwbrower.top/gtyynamzil.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.chenjidiqi.icu/gtmqttkocl.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.sysykeji.top/gtfbetyljo.html

TS:   // 同 JS
来源：http://hz.redwolf501.top/gtsfztzjzc.html

Java: synchronized (this) { shared++; }
来源：http://hz.hnxiangtu.top/gtcbdtsrhs.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.hnxiangtu.top/gtzetvtrts.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.c1oappe.top/gtbwsmahhg.html

C#:   lock (gate) { shared++; }
来源：http://hz.wangshuangyany.cn/gtughjjmyy.html

[O04] 定义异步函数并等待
来源：http://hz.jinyuanbaomall.cn/gthiydycxz.html

Py:   async def f():⏎    await g()
来源：http://hz.xingfuxueyuan.xyz/gtuxcvtiip.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.shanyushiyangkeji.top/gttdtrhmqw.html

JS:   async function f() { await g(); }
来源：http://hz.9152youxi.cn/gtipawjnsu.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.birdmap.top/gtzpzzdxks.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.tian-w.cn/gtiaspikcg.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.zhengqikj.top/gtiewwmvoe.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.zhixingplan.top/gtjkcxvcgx.html

C#:   async Task F() { await G(); }
来源：http://hz.jinyuanbaomall.cn/gtucjhfhsm.html

[O05] 并发执行并等待全部完成
来源：http://hz.jinqigufen.top/gttvvfzauy.html

Py:   asyncio.gather(*tasks)
来源：http://hz.aizwys.cn/gtgdyzrczb.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.gogol.net.cn/gtjkfkwvyv.html

JS:   await Promise.all(tasks)
来源：http://hz.shzxlz.cn/gtkskctbmk.html

TS:   await Promise.all(tasks)
来源：http://hz.smart0.xyz/gtqsfpuiqp.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.xuanzx.com/gtpaakboun.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.iojbl.cn/gtximfsqsm.html

Ruby: threads.map(&:join)
来源：http://hz.ybcxt.top/gtcynokhsv.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.52xcode.cn/gtbzihexqf.html

[O06] 使用进程池
来源：http://hz.hysaishi.cn/gtupzkbygs.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.guannengcc.top/gtkhivpsfx.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.zhixingplan.top/gtqkvzvbus.html

JS:   // child_process / cluster 模块
来源：http://hz.xylfe.cn/gtkmiodbry.html

TS:   // child_process / cluster 模块
来源：http://hz.vqdsnc.cn/gtbqigcjor.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.meibo888.top/gtbxkupfgb.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.ivvv.top/gtsndtwpgk.html

Ruby: // fork 块
来源：http://hz.hfpthk.cn/gtjojuwfbv.html

C#:   Parallel.For
来源：http://hz.sysykeji.top/gtijrvsfct.html

================================================================================
来源：http://hz.hywenlv.cn/gtjoosrgev.html

P. 常用工具函数
来源：http://hz.cheryme.top/gtoksibhkj.html

================================================================================
来源：http://hz.xuanzx.com/gtdkpdzejf.html

[P01] 生成 UUID
来源：http://hz.svipenyu.cn/gtjpovokxo.html

Py:   str(uuid.uuid4())
来源：http://hz.ybcxt.top/gtrvpxkxad.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.redwolf501.top/gtxyzqzwfi.html

JS:   crypto.randomUUID()
来源：http://hz.jqgufenzy.top/gtsmqqiuxo.html

TS:   crypto.randomUUID()
来源：http://hz.hfpthk.cn/gtuztliymi.html

Java: UUID.randomUUID().toString()
来源：http://hz.ydjk.org.cn/gtvrplynvw.html

Go:   // 用 github.com/google/uuid
来源：http://hz.316326.xyz/gtcxjiwjwv.html

Ruby: SecureRandom.uuid
来源：http://hz.fengsongda.top/gtctxtmhmd.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.zhiwuduotai.top/gtlcdftrxn.html

[P02] MD5 / SHA256 摘要
来源：http://hz.andypj.xyz/gtroxiimbh.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.guannengcc.top/gtmukceqsl.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.316326.xyz/gtesmypysj.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.shanyushiyangkeji.top/gtqxrpduyu.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.quarkkingdee.top/gtkippugcn.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.hysaishi.cn/gtkdykxnyk.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.c1oappe.top/gtnyjjmsjs.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.chenzaomai.com/gtjfymiiad.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.jlsjyb.cn/gtkktvikmf.html

[P03] 生成短随机字符串
来源：http://hz.havefunace.top/gtvjfwszdm.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.ydjk.org.cn/gtajzmpfxk.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.xziqi.cn/gtnrtarcgz.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.nanxuanxn.top/gtuhlnsefd.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.wangdashe.top/gtdtbmccbo.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.dianchejie.cn/gthjuagtrn.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.dashuyun.cn/gtubshspdw.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.tanke756.top/gtfaulpwvr.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.aibaodan.cn/gtaojxfnuo.html

[P04] 求长度
来源：http://hz.yj202588.top/gtkbrmthzx.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.quarkkingdee.top/gttqfccqnp.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.52xcode.cn/gtryfeoifm.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.shzxlz.cn/gtlludqpqq.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.zhixingplan.top/gtpbcigsgt.html

Java: list.size();  map.size();  s.length()
来源：http://hz.aibaodan.cn/gtxcelmctk.html

Go:   len(arr);  len(m)
来源：http://hz.havefunace.top/gtjbchvsdw.html

Ruby: x.length;  x.size
来源：http://hz.mhx1999.top/gtakbuombe.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.zhengqikj.top/gtvglxojit.html

[P05] 判断两个对象内容是否相等
来源：http://hz.xylfe.cn/gtrexdzwpp.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.xylfe.cn/gtoxhjmntz.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.svipenyu.cn/gtsflzgbdy.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.ybcxt.top/gtfsiwblca.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.yj20258.top/gtzcrkucur.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.gogol.net.cn/gtgvjqzjze.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.cheryme.top/gtoacjohyi.html

Ruby: a == b
来源：http://hz.mhx1999.top/gtxcwrcoog.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.feifeiyinyue.top/gtblsedfpr.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.zycfv.cn/gtclcodueb.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.hywenlv.cn/gtizahtcff.html

PHP:  if (empty($x)) {}
来源：http://hz.andypj.xyz/gtfpfwwqwe.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.kuanghao11.cn/gtdzolicgw.html

TS:   if (x == null) {}
来源：http://hz.ivvv.top/gtrxwodern.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.hammf.cn/gtuuyrhdrt.html

Go:   if x == nil {}
来源：http://hz.havefunace.top/gtlpsgtlft.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.aizwys.cn/gtisrwzrvp.html

C#:   if (x is null) {}
来源：http://hz.sweek.top/gtknjgcben.html

[P07] 防抖与节流
来源：http://hz.dianchejie.cn/gtcfntgnby.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.gaohongyu789.top/gtwijbkfiw.html

PHP:  // 手写时间戳比较
来源：http://hz.redwolf501.top/gtxshkofrd.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.jianghu66.top/gtnzlwwiug.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.hnxiangtu.top/gtkrrocqwk.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.yonumen.top/gthetqvxdo.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.hysaishi.cn/gtrkmxjstj.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.hysaishi.cn/gtengrpclo.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.jqgfzy.top/gtqrulgepx.html

[P08] 处理浮点精度问题
来源：http://hz.yongpay.top/gtcyhgwgrq.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.316326.xyz/gthabjmvfl.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.jinqigfzy.top/gtdhlorsbb.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.dashuyun.cn/gtepwxcgdk.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.hywenlv.cn/gtfxldrjvo.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.jqgufenzy.top/gtyrgxktpv.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.gotoacloud.top/gtoclrnjxb.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.wangdashe.top/gtohflrrsf.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.gotoacloud.top/gtpjcspjlw.html

================================================================================
来源：http://hz.tanke756.top/gttvgelkos.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.nanxuanxn.top/gtujcrbuqb.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtrpuuhvoo.html

[Q01] 创建表
来源：http://hz.zhongyouzk.top/gtkjzykaql.html

CREATE TABLE users (
来源：http://hz.haohaochexian.top/gteqmfiecv.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.9152youxi.cn/gtybannldx.html

name VARCHAR(50) NOT NULL,
来源：http://hz.cashguo.top/gtidewklfe.html

email VARCHAR(100) UNIQUE,
来源：http://hz.snrcjt.cn/gtawdmvvgf.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.guannengcc.top/gttocqvpfp.html

);
来源：http://hz.zhengqikj.top/gtudmwvpvw.html

[Q02] 创建带外键的表
来源：http://hz.sweek.top/gtkbwzhopu.html

CREATE TABLE orders (
来源：http://hz.tian-w.cn/gttasqneyw.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.yj20258.top/gtlemplgxo.html

user_id INT NOT NULL,
来源：http://hz.cucudq.cn/gtfbxidiit.html

amount DECIMAL(10, 2),
来源：http://hz.feifeiyinyue.top/gtbxomuzki.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.ehwqpu.com/gtzfabphkr.html

);
来源：http://hz.zdqjudy.top/gtbajwzlmn.html

[Q03] 增加列
来源：http://hz.chenzaomai.com/gtmocmgeop.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.bjfxy.top/gttjbcacqr.html

[Q04] 修改列类型
来源：http://hz.tian-w.cn/gtbsrtmkmx.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.andypj.xyz/gtxrenkwqq.html

[Q05] 重命名列
来源：http://hz.c1oappe.top/gtanpukkaf.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.haohaochexian.top/gtlgufsyuy.html

[Q06] 删除列
来源：http://hz.zycfv.cn/gtganvvbex.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.hysaishi.cn/gtfdwumvkf.html

[Q07] 删除表
来源：http://hz.316326.xyz/gtpjbwburs.html

DROP TABLE IF EXISTS orders;
来源：http://hz.dianchejie.cn/gtvojizozf.html

[Q08] 创建普通索引
来源：http://hz.nwbrower.top/gthufvajnz.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.yongpay.top/gtdjormmvv.html

[Q09] 创建唯一索引
来源：http://hz.jqgfzy.top/gtsuhpxwkn.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.tanke756.top/gtufjhxllt.html

[Q10] 插入单行
来源：http://hz.havefunace.top/gtbusjgtgw.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.gzhubu.top/gtngrmskcf.html

[Q11] 一次插入多行
来源：http://hz.jinqigfzy.top/gtseatkixn.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.yj20258.top/gtbwkjdaur.html

[Q12] 插入后取自增 ID
来源：http://hz.zhongyouzk.top/gtnmdaadav.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.shanyushiyangtech.top/gtqsslonxe.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.guannengcc.top/gtlptnbjlt.html

[Q13] 忽略重复插入
来源：http://hz.jinqigfzy.top/gtlvshanlv.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.hammf.cn/gtypzxyejk.html

[Q14] 存在则更新（upsert）
来源：http://hz.ydjk.org.cn/gtvfnranyw.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.zhoulong.xyz/gthnlzuggz.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.bjfxy.top/gtsqvyzgsr.html

[Q15] 查询全部
来源：http://hz.yanxiufei.cn/gtdgoyfcgw.html

SELECT * FROM users;
来源：http://hz.sufxvd.cn/gtjrefdceg.html

[Q16] 查询指定列
来源：http://hz.zdqjudy.top/gtriyynkdo.html

SELECT id, name FROM users;
来源：http://hz.quarkkingdee.top/gtsejxawmg.html

[Q17] 条件查询
来源：http://hz.svipenyu.cn/gtwsrpnuxu.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.xuetiantiany.cn/gtdkhqgvfa.html

[Q18] 模糊匹配
来源：http://hz.jyoumei.cn/gtrxhuwxjt.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.316326.xyz/gtcwfyvdwy.html

[Q19] 范围查询
来源：http://hz.hnxiangtu.top/gtyvwppvjr.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.cucudq.cn/gtsaytmmqa.html

[Q20] IN 列表
来源：http://hz.yj20258.top/gtzmduegjz.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.cashguo.top/gtdhfpcdaf.html

[Q21] 空值判断
来源：http://hz.zhijiandao.cn/gtonrwebyr.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.snrcjt.cn/gtqulsvoba.html

[Q22] 排序
来源：http://hz.gzhubu.top/gtwwnazrls.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.yuxming.cn/gthcmtpksj.html

[Q23] 分页
来源：http://hz.cdnleiting.top/gtgaskxwir.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.hfpthk.cn/gtnviqeyob.html

[Q24] 去重
来源：http://hz.redwolf501.top/gtlahnaojg.html

SELECT DISTINCT city FROM users;
来源：http://hz.jqgfzy.top/gtysqhogtl.html

[Q25] 只取前 N 条
来源：http://hz.yj202588.top/gtszanzqaf.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.zhijiandao.cn/gtuhyxzyif.html

[Q26] 计数
来源：http://hz.zhixingplan.top/gtyreszrgl.html

SELECT COUNT(*) FROM users;
来源：http://hz.jqgufenzy.top/gtwdttnukz.html

[Q27] 条件计数
来源：http://hz.jlsjyb.cn/gtvzxurgkg.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.yongpay.top/gtdhwiwnmt.html

[Q28] 求和与平均
来源：http://hz.jyoumei.cn/gthtbgcbes.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.zhijiandao.cn/gtfbmsyurg.html

[Q29] 最大最小值
来源：http://hz.shzxlz.cn/gtdqoxabue.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.zhongyouzk.top/gtcpwfoikv.html

[Q30] 分组统计
来源：http://hz.pycfn.com/gtnpvqfymk.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.nanxuanxn.top/gtbnmnejeg.html

[Q31] 分组后过滤
来源：http://hz.shanyushiyangkeji.top/gtjaqwjgvc.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.jinghuilouyu.cn/gthxfsfkln.html

[Q32] 分组拼接字符串
来源：http://hz.gotoacloud.top/gtkzguenms.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.sweek.top/gtwxjasvfs.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.chenzaomai.com/gtwapsjade.html

[Q33] 多列分组
来源：http://hz.jinqigfzy.top/gtoqkmpbco.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.yj202588.top/gthrbacvqc.html

[Q34] 每组取第一条
来源：http://hz.jlsjyb.cn/gtwgxopkcv.html

SELECT * FROM (
来源：http://hz.yj202588.top/gtqhfyliap.html


<!-- 参考信息 -->