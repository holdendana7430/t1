代发 wailian999

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.iojbl.cn/gtbnattydh.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.yj202588.top/gtzxbitmtu.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.dashuyun.cn/gtjagwygis.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.yj20258888.top/gtedaglifs.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.xinyue.icu/gtgajgvrfa.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.shanyushiyangkeji.top/gtelwgplsx.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.nanxuanxn.top/gtyregdlrp.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.ydzc1.top/gtmneavnvu.html

[N05] 最大公约数
来源：http://hz.shanyushiyangtech.top/gtvhknzbwe.html

Py:   math.gcd(a, b)
来源：http://hz.hongshengwenyu.top/gtcozffabd.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.feifeiyinyue.top/gtbmnwfvlj.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.shzxlz.cn/gtatcynayp.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.jinqigfzy.top/gtxmkubkbt.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.ydzc1.top/gtzirvadbo.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.havefunace.top/gtaaluyupr.html

Ruby: a.gcd(b)
来源：http://hz.jlsjyb.cn/gtdygoognf.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.xingfuxueyuan.xyz/gtbcawucts.html

[N06] 判断回文字符串
来源：http://hz.yj20258888.top/gtikodvzrl.html

Py:   s == s[::-1]
来源：http://hz.gogol.net.cn/gtmgoytilg.html

PHP:  $s === strrev($s);
来源：http://hz.guowangkeji.top/gtjeujpjii.html

JS:   s === [...s].reverse().join("")
来源：http://hz.hysaishi.cn/gtnmjiczlu.html

TS:   s === [...s].reverse().join("")
来源：http://hz.wangdashe.top/gtcmnamxjs.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.xuetiantiany.cn/gtrkfbbyyj.html

Go:   // 双指针从两端比较
来源：http://hz.yvedp.cn/gtnagixdqa.html

Ruby: s == s.reverse
来源：http://hz.9152youxi.cn/gturvhwisk.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.ywan-chungtsiang.top/gtagkzezve.html

[N07] 两数之和（返回下标）
来源：http://hz.tianlin.xyz/gtsbskitur.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.iojbl.cn/gtduijjotk.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.jinqigfzy.top/gtvmztxzwi.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.gzhubu.top/gtvibclwoj.html

TS:   // 手写 Map<string, number>
来源：http://hz.316326.xyz/gtbfrenoql.html

Java: // 手写 HashMap
来源：http://hz.tian-w.cn/gtysknnzsr.html

Go:   // 手写 map[int]int
来源：http://hz.jinyuanbaomall.cn/gtfheiqthi.html

Ruby: // 手写 Hash
来源：http://hz.redwolf501.top/gttflvhavg.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.shanyushiyangkeji.top/gtehtfrjch.html

[N08] 生成全排列
来源：http://hz.xziqi.cn/gtunzbtrjc.html

Py:   itertools.permutations(arr)
来源：http://hz.nwbrower.top/gtzehkrakf.html

PHP:  // 手写递归交换
来源：http://hz.yueranfly.top/gttqneehnd.html

JS:   // 手写回溯递归
来源：http://hz.chenzaomai.com/gtajqmudao.html

TS:   // 手写回溯递归
来源：http://hz.0kj1m.cn/gtyfuhqxsz.html

Java: // 手写回溯递归
来源：http://hz.kuanghao11.cn/gthfhyjxza.html

Go:   // 手写回溯递归
来源：http://hz.yangfankeji.com/gtgvocoevb.html

Ruby: arr.permutation.to_a
来源：http://hz.yueranfly.top/gthelldaoj.html

C#:   // 手写回溯递归
来源：http://hz.zhixingplan.top/gtboimacyy.html

[N09] 栈与队列
来源：http://hz.meibo888.top/gtulsfkmsr.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.ywan-chungtsiang.top/gtdvjeizhl.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.9152youxi.cn/gtooekpvtc.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.aibaodan.cn/gtazwvrkkw.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.zhengqikj.top/gtkkqhcabv.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.zhixingplan.top/gtradooxba.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.yonumen.top/gtorzmhfvf.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.sxryk.cn/gtnnvklmks.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.gogol.net.cn/gtewwxbvoz.html

[N10] 链表节点定义
来源：http://hz.tian-w.cn/gtnvnnngzd.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.daria6918.cn/gtqacooets.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.kuanghao11.cn/gtcqtgvqbb.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.jinyuanbaomall.cn/gtofzvwjqj.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.mhx1999.top/gthgtseqef.html

Java: class Node { int v; Node next; }
来源：http://hz.xuetiantiany.cn/gteuypgobd.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.ehwqpu.com/gttfmsomvl.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.jinghuilouyu.cn/gtugmjpoxy.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.chenzaomai.com/gtkuvzvjiv.html

[N11] 二叉树中序遍历
来源：http://hz.zhaomingkeji.xyz/gthwbtambk.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.shanyushiyangtech.top/gtmjvbpecr.html

PHP:  // 手写递归函数
来源：http://hz.xingfuxueyuan.xyz/gtdsjnovnz.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.vqdsnc.cn/gtagvdkyte.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.cashguo.top/gtpmlgarcd.html

Java: // 手写递归
来源：http://hz.redwolf501.top/gtuzowgkfm.html

Go:   // 手写递归
来源：http://hz.birdmap.top/gtnvltnwbo.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.iojbl.cn/gtklqlhyud.html

C#:   // 手写递归
来源：http://hz.hnxiangtu.top/gtnwbdwcts.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.jqgfzy.top/gtgkuiqkpu.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.jiagoushi.top/gtzjbobxio.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.hywenlv.cn/gtncjjdajs.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.svipenyu.cn/gtnzrpelby.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.snrcjt.cn/gtejgguvhy.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.shanyushiyangkeji.top/gtpkvhrznz.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.xuanzx.com/gtkqpufkvq.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.pycfn.com/gthrbocimg.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.andypj.xyz/gtkiojtveb.html

================================================================================
来源：http://hz.mhx1999.top/gtebhvjvgl.html

O. 并发与异步
来源：http://hz.shuidangran.top/gttylkpltj.html

================================================================================
来源：http://hz.hysaishi.cn/gtxblwxnhu.html

[O01] 启动一个线程
来源：http://hz.dashuyun.cn/gtjdbgmkft.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.sysykeji.top/gttblclani.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.tanke756.top/gtmqkbdfqb.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.dashuyun.cn/gtofummsjh.html

TS:   // 同 JS
来源：http://hz.zhongyouzk.top/gtpzzpdxvb.html

Java: new Thread(() -> f()).start()
来源：http://hz.nanxinkj.top/gtvgqnbxsb.html

Go:   go f()
来源：http://hz.smart0.xyz/gtmshxxnvf.html

Ruby: Thread.new { f }
来源：http://hz.havefunace.top/gtroarkxre.html

C#:   Task.Run(() => F());
来源：http://hz.quarkkingdee.top/gtumufbvhy.html

[O02] 使用线程池
来源：http://hz.ehwqpu.com/gtclgkkvfv.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.pycfn.com/gtoyabteny.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.quarkkingdee.top/gtjfdpkrzg.html

JS:   // worker_threads 线程池
来源：http://hz.yueranfly.top/gtxzgcrahz.html

TS:   // worker_threads 线程池
来源：http://hz.yuxming.cn/gtyznzuanb.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.316326.xyz/gtplcibxkz.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.nanxinkj.top/gtnbqitmld.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.guannengcc.top/gtqtwgnxmm.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.havefunace.top/gtfltkrhic.html

[O03] 加锁保护共享数据
来源：http://hz.fengsongda.top/gtcpaglohl.html

Py:   with lock: shared += 1
来源：http://hz.cdnleiting.top/gtahunmqiq.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.aizwys.cn/gtitbxqlmh.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.fzhhl.top/gtqemctsde.html

TS:   // 同 JS
来源：http://hz.guowangkeji.top/gtnkpnnnwk.html

Java: synchronized (this) { shared++; }
来源：http://hz.jlsjyb.cn/gtssgiytgp.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.dashuyun.cn/gtpiwwvonb.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.yanxiufei.cn/gtwzjzaxbn.html

C#:   lock (gate) { shared++; }
来源：http://hz.ehwqpu.com/gtfdcrjkvd.html

[O04] 定义异步函数并等待
来源：http://hz.hysaishi.cn/gtjwmtizgp.html

Py:   async def f():⏎    await g()
来源：http://hz.feifeiyinyue.top/gtyqdtmjrv.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.feifeiyinyue.top/gtwjtifmvt.html

JS:   async function f() { await g(); }
来源：http://hz.zhiwuduotai.top/gthzblpcta.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.jinyuanbaomall.cn/gtojhzpcru.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.snrcjt.cn/gtdxyazljq.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.wangdashe.top/gtalffefgn.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.yongpay.top/gtnapmnklo.html

C#:   async Task F() { await G(); }
来源：http://hz.hnqzz.top/gtncsmrajt.html

[O05] 并发执行并等待全部完成
来源：http://hz.hywenlv.cn/gtvgszpzcw.html

Py:   asyncio.gather(*tasks)
来源：http://hz.ivvv.top/gtwtlcvatm.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.yj20258.top/gtueoytuwr.html

JS:   await Promise.all(tasks)
来源：http://hz.zhaomingkeji.xyz/gtfubncebi.html

TS:   await Promise.all(tasks)
来源：http://hz.svipenyu.cn/gtsuxfmkvo.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.feifeiyinyue.top/gtrgsrtlsh.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.cashguo.top/gtpecixxrj.html

Ruby: threads.map(&:join)
来源：http://hz.zhaomingkeji.xyz/gtmldtzeql.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.jinqigufen.top/gtgsqobjvc.html

[O06] 使用进程池
来源：http://hz.havefunace.top/gtcmbzjgai.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.zycfv.cn/gtzoaejmfc.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.feifeiyinyue.top/gtdvsnplke.html

JS:   // child_process / cluster 模块
来源：http://hz.guannengcc.top/gthhqogvtu.html

TS:   // child_process / cluster 模块
来源：http://hz.gaohongyu789.top/gtcmvqwgev.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.zhijiandao.cn/gtykqftjix.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.sweek.top/gthszgvmsl.html

Ruby: // fork 块
来源：http://hz.gzhubu.top/gthwepgejx.html

C#:   Parallel.For
来源：http://hz.guowangkeji.top/gtvqxlbobx.html

================================================================================
来源：http://hz.yj202588.top/gtqarybghw.html

P. 常用工具函数
来源：http://hz.fengsongda.top/gtoccijuke.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtmrvykhkb.html

[P01] 生成 UUID
来源：http://hz.xziqi.cn/gtxtmwvkwr.html

Py:   str(uuid.uuid4())
来源：http://hz.yj20258.top/gtjdphdhnq.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.zhongyouzk.top/gthhiepmyz.html

JS:   crypto.randomUUID()
来源：http://hz.jlsjyb.cn/gtntnfqghf.html

TS:   crypto.randomUUID()
来源：http://hz.tian-w.cn/gtquhwlhby.html

Java: UUID.randomUUID().toString()
来源：http://hz.snrcjt.cn/gtxejiubfs.html

Go:   // 用 github.com/google/uuid
来源：http://hz.chenlongwang.top/gtufaxhyyc.html

Ruby: SecureRandom.uuid
来源：http://hz.zhaomingkeji.xyz/gtjpgkebqh.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.sxryk.cn/gtgpmezlho.html

[P02] MD5 / SHA256 摘要
来源：http://hz.sweek.top/gtnosehral.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.hammf.cn/gtvjswelii.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.yongpay.top/gtthfbfhed.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.meibo888.top/gtfwogcfwp.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.havefunace.top/gtypfoliqw.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.yuanzhike.top/gtqhsvtxfk.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.cheryme.top/gtwneodgsi.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.zhiwuduotai.top/gtgskloqud.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.316326.xyz/gtlbxtdyun.html

[P03] 生成短随机字符串
来源：http://hz.0kj1m.cn/gtzdzjaduq.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.hongshengwenyu.top/gtxiacsgir.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.iojbl.cn/gtcyrgcupl.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.ivvv.top/gtmsrvvtru.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.tianlin.xyz/gtlqcedcsa.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.jinyuanbaomall.cn/gtdrhrgtsn.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.hongshengwenyu.top/gtjxrlpalf.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.jqgfzy.top/gtwhxfbeex.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.hnqzz.top/gtvwtvksko.html

[P04] 求长度
来源：http://hz.zdqjudy.top/gtblzcxfhs.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.gzhubu.top/gtxnarpeoy.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.bjfxy.top/gticgrviqt.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.yongpay.top/gtzacyvkvk.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.ydzc1.top/gtgigxnozh.html

Java: list.size();  map.size();  s.length()
来源：http://hz.kuanghao11.cn/gthetctnir.html

Go:   len(arr);  len(m)
来源：http://hz.mhx1999.top/gtoispnfog.html

Ruby: x.length;  x.size
来源：http://hz.zhongyouzk.top/gtxviipkpv.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.redwolf501.top/gtqjadgapq.html

[P05] 判断两个对象内容是否相等
来源：http://hz.smart0.xyz/gtbbdrxjjj.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.jqgufenzy.top/gtgrvobcyy.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.yuxming.cn/gtdgaicayx.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.yueranfly.top/gtgduzovfj.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.smart0.xyz/gtfptvhcia.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.andypj.xyz/gtnzzaqyyc.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.cucudq.cn/gtjrcssuzx.html

Ruby: a == b
来源：http://hz.nwbrower.top/gtcvyiukwu.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.hywenlv.cn/gtjlnjxdca.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.zdqjudy.top/gtdhttkjvo.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.ybcxt.top/gtsttgolzz.html

PHP:  if (empty($x)) {}
来源：http://hz.nwbrower.top/gtbroxvxmi.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.gotoacloud.top/gthahgdcnz.html

TS:   if (x == null) {}
来源：http://hz.kuanghao11.cn/gtvycrinmi.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.yj202588.top/gtgfkxihqg.html

Go:   if x == nil {}
来源：http://hz.hammf.cn/gtrbaxvwpj.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.yj20258888.top/gtbapoucsp.html

C#:   if (x is null) {}
来源：http://hz.hfpthk.cn/gtduezdnsw.html

[P07] 防抖与节流
来源：http://hz.quarkkingdee.top/gtbrhgizhx.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.cucudq.cn/gtkflhsdyp.html

PHP:  // 手写时间戳比较
来源：http://hz.zhengqikj.top/gtyfkurpsm.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.hywenlv.cn/gtjlzskfkx.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.iojbl.cn/gtjsmgdfak.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.pengpengdd.cyou/gtspykbmmi.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.zhengqikj.top/gtofpuknnj.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.tian-w.cn/gtssztvykm.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.svipenyu.cn/gtnljvdxzv.html

[P08] 处理浮点精度问题
来源：http://hz.sysykeji.top/gtcbdieqxa.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.quarkkingdee.top/gtdkqqdtzh.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.chenzaomai.com/gtlpfoxafz.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.yj20258888.top/gtuvjrghsq.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.yonumen.top/gtllneksqy.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.shuidangran.top/gtquulvcnv.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.daxiang520.top/gtcftgustv.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.aibaodan.cn/gtjzytbyex.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.jlsjyb.cn/gtcosrhqmc.html

================================================================================
来源：http://hz.zdqjudy.top/gtujuiwany.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.shanyushiyangtech.top/gtfzogoeie.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtxbviameb.html

[Q01] 创建表
来源：http://hz.fzhhl.top/gtkaequzla.html

CREATE TABLE users (
来源：http://hz.gaohongyu789.top/gtrfseatao.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.jlsjyb.cn/gteqlyetih.html

name VARCHAR(50) NOT NULL,
来源：http://hz.hammf.cn/gtbueqqtoq.html

email VARCHAR(100) UNIQUE,
来源：http://hz.jinghuilouyu.cn/gtyvnqyrvu.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.yvedp.cn/gtajxuimbm.html

);
来源：http://hz.sufxvd.cn/gtfqlnmzft.html

[Q02] 创建带外键的表
来源：http://hz.shanyushiyangkeji.top/gtebacmvhf.html

CREATE TABLE orders (
来源：http://hz.xziqi.cn/gtejzyeqoy.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.tianlin.xyz/gtgoxhkmtm.html

user_id INT NOT NULL,
来源：http://hz.shangyingyoupin.top/gtafnhjvur.html

amount DECIMAL(10, 2),
来源：http://hz.nanxinkj.top/gtzihirwym.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.ywan-chungtsiang.top/gtoezffwvj.html

);
来源：http://hz.xuanzx.com/gtvjsaijfr.html

[Q03] 增加列
来源：http://hz.shanyushiyangtech.top/gtldekkibh.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.jlsjyb.cn/gtlguauada.html

[Q04] 修改列类型
来源：http://hz.guowangkeji.top/gtzbkkibku.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.cashguo.top/gtckgnnynk.html

[Q05] 重命名列
来源：http://hz.c1oappe.top/gthonaagzx.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.snrcjt.cn/gttusohdor.html

[Q06] 删除列
来源：http://hz.ppjwa.cn/gtfgzhmwbt.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.pycfn.com/gtbuttfshi.html

[Q07] 删除表
来源：http://hz.nwbrower.top/gtpypxhrbo.html

DROP TABLE IF EXISTS orders;
来源：http://hz.xinyue.icu/gtjcovjnkd.html

[Q08] 创建普通索引
来源：http://hz.yj20258888.top/gtqdnhjcvf.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.quarkkingdee.top/gtqomqsslw.html

[Q09] 创建唯一索引
来源：http://hz.smart0.xyz/gtsyfkyvhm.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.havefunace.top/gtlhqpjwkx.html

[Q10] 插入单行
来源：http://hz.zhixingplan.top/gtdjxgmpie.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.jinyuanbaomall.cn/gtncwystft.html

[Q11] 一次插入多行
来源：http://hz.316326.xyz/gtuhebklwo.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.yj20258888.top/gttaqmafvi.html

[Q12] 插入后取自增 ID
来源：http://hz.sysykeji.top/gtmrrwkcpx.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.52xcode.cn/gtvdnvvynm.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.yueranfly.top/gtdqnqedfe.html

[Q13] 忽略重复插入
来源：http://hz.xylfe.cn/gtooethzdn.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.fengsongda.top/gtemejetam.html

[Q14] 存在则更新（upsert）
来源：http://hz.xziqi.cn/gtcicvbzdf.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.sweek.top/gtwtivmxsz.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.fzhhl.top/gtmpnxsiap.html

[Q15] 查询全部
来源：http://hz.guowangkeji.top/gtaeaxwesw.html

SELECT * FROM users;
来源：http://hz.pengpengdd.cyou/gtdlfjetzd.html

[Q16] 查询指定列
来源：http://hz.yanxiufei.cn/gtiistbbze.html

SELECT id, name FROM users;
来源：http://hz.316326.xyz/gtreaxmmhd.html

[Q17] 条件查询
来源：http://hz.gzhubu.top/gttqsbwekh.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.aizwys.cn/gtyylbfako.html

[Q18] 模糊匹配
来源：http://hz.yuanzhike.top/gtoxjhrven.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.jyoumei.cn/gthbjrktfz.html

[Q19] 范围查询
来源：http://hz.nanxinkj.top/gtjgxlllnv.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.aizwys.cn/gtonpnnhff.html

[Q20] IN 列表
来源：http://hz.aizwys.cn/gtepfcgjuh.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.vqdsnc.cn/gtrzjxismw.html

[Q21] 空值判断
来源：http://hz.chenlongwang.top/gtjijrjhsc.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.hfpthk.cn/gtmvixfkvg.html

[Q22] 排序
来源：http://hz.fzhhl.top/gthuabkded.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.cdnleiting.top/gtjqtbfvew.html

[Q23] 分页
来源：http://hz.shuidangran.top/gtzjflkacz.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.zhoulong.xyz/gtrjyngluv.html

[Q24] 去重
来源：http://hz.yvedp.cn/gtrnceaesd.html

SELECT DISTINCT city FROM users;
来源：http://hz.gogol.net.cn/gtgxibdwbt.html

[Q25] 只取前 N 条
来源：http://hz.cucudq.cn/gtunfvhvww.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.haohaochexian.top/gtwpmfcooi.html

[Q26] 计数
来源：http://hz.c1oappe.top/gtwwosemiu.html

SELECT COUNT(*) FROM users;
来源：http://hz.yvedp.cn/gtfuozkgqa.html

[Q27] 条件计数
来源：http://hz.gzhubu.top/gtyukfzczg.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.hywenlv.cn/gtnbjuhtnw.html

[Q28] 求和与平均
来源：http://hz.ppjwa.cn/gtczduboyz.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.nwbrower.top/gtwznztgjw.html

[Q29] 最大最小值
来源：http://hz.nanxuanxn.top/gtmhvocrfz.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.chenzaomai.com/gtllqgffty.html

[Q30] 分组统计
来源：http://hz.gzhubu.top/gtravxwxtq.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.yueranfly.top/gtkdoqozwb.html

[Q31] 分组后过滤
来源：http://hz.zhaomingkeji.xyz/gteqtbwtev.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.cheryme.top/gtotqfefzn.html

[Q32] 分组拼接字符串
来源：http://hz.chenjidiqi.icu/gtbhsxuhel.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.wangdashe.top/gtmdzrlqdm.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.xuanzx.com/gtcxnyhfdy.html

[Q33] 多列分组
来源：http://hz.sxryk.cn/gtjetfcbql.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.pengpengdd.cyou/gtouekomvz.html

[Q34] 每组取第一条
来源：http://hz.mhx1999.top/gtptehbsly.html

SELECT * FROM (
来源：http://hz.yj20258888.top/gtjgdyaukc.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.wangdashe.top/gtichwavoi.html

) t WHERE rn = 1;
来源：http://hz.yj20258888.top/gtoqetzejv.html

[Q35] 内连接
来源：http://hz.hammf.cn/gtqirdximz.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.gaohongyu789.top/gtbntpahph.html


<!-- 参考信息 -->