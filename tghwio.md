代发 wailian999

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.zhengqikj.top/gtlyqtxmgw.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.xinyue.icu/gtvxxplrrz.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.yuxming.cn/gtafqbsrgm.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.zhijiandao.cn/gtlqefcisd.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.yj20258.top/gtksvpkrfs.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.zhongyouzk.top/gtpmkiqxkf.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.birdmap.top/gtuxwhbzkk.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.dashuyun.cn/gttfqsghto.html

[N05] 最大公约数
来源：http://hz.hnxiangtu.top/gttaogyndc.html

Py:   math.gcd(a, b)
来源：http://hz.aizwys.cn/gtlxsuqlbw.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.hfpthk.cn/gtgdxgrnmi.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.fengsongda.top/gtilmmdaxo.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.jqgfzy.top/gttvcdcjja.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.ydjk.org.cn/gtlhpzrxsb.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.xinyue.icu/gtvpnkenmq.html

Ruby: a.gcd(b)
来源：http://hz.316326.xyz/gtolfiegdl.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.guowangkeji.top/gtayyfbfue.html

[N06] 判断回文字符串
来源：http://hz.zhengqikj.top/gtsshxzldq.html

Py:   s == s[::-1]
来源：http://hz.sysykeji.top/gttlhqpbig.html

PHP:  $s === strrev($s);
来源：http://hz.jianghu66.top/gtidtcqtaj.html

JS:   s === [...s].reverse().join("")
来源：http://hz.yuanzhike.top/gtnijuhyvh.html

TS:   s === [...s].reverse().join("")
来源：http://hz.xuanzx.com/gtokxiysjw.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.andypj.xyz/gtygctleay.html

Go:   // 双指针从两端比较
来源：http://hz.mhx1999.top/gtyiayunwi.html

Ruby: s == s.reverse
来源：http://hz.shanyushiyangtech.top/gtnlfpxgid.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.fzhhl.top/gttmqhdbgb.html

[N07] 两数之和（返回下标）
来源：http://hz.yj20258.top/gttqgylnpq.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.hysaishi.cn/gtwojryjwz.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.aibaodan.cn/gtpfepibzu.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.zhengqikj.top/gthdffkutr.html

TS:   // 手写 Map<string, number>
来源：http://hz.dashuyun.cn/gtykjmczxa.html

Java: // 手写 HashMap
来源：http://hz.yj20258.top/gtyvkxmviy.html

Go:   // 手写 map[int]int
来源：http://hz.jiagoushi.top/gtqnxxukrt.html

Ruby: // 手写 Hash
来源：http://hz.jiagoushi.top/gttwbenrta.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.zycfv.cn/gtsnnqirvv.html

[N08] 生成全排列
来源：http://hz.jianghu66.top/gtexeoqwlz.html

Py:   itertools.permutations(arr)
来源：http://hz.sxryk.cn/gtiezvvxzl.html

PHP:  // 手写递归交换
来源：http://hz.meibo888.top/gtpejajbvd.html

JS:   // 手写回溯递归
来源：http://hz.aizwys.cn/gtaaqoxoow.html

TS:   // 手写回溯递归
来源：http://hz.jianghu66.top/gtpgcsioxy.html

Java: // 手写回溯递归
来源：http://hz.gaohongyu789.top/gtqstxzdec.html

Go:   // 手写回溯递归
来源：http://hz.cdnleiting.top/gthyxtjvxd.html

Ruby: arr.permutation.to_a
来源：http://hz.zhoulong.xyz/gtaputkzdn.html

C#:   // 手写回溯递归
来源：http://hz.yueranfly.top/gtgvarehld.html

[N09] 栈与队列
来源：http://hz.zhijiandao.cn/gtmigplekw.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.hnqzz.top/gteputyffv.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.cucudq.cn/gtnnnxitff.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.cdnleiting.top/gtayvhrnor.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.quarkkingdee.top/gtuqwjmhuy.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.svipenyu.cn/gtqlmfyouu.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.gotoacloud.top/gtmapvdxxc.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.zhengqikj.top/gtbnwuwxfh.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.0kj1m.cn/gttcxnsecj.html

[N10] 链表节点定义
来源：http://hz.bjfxy.top/gtlrdivrsh.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.jinqigufen.top/gtzuvkrwva.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.fzhhl.top/gtibafhmrs.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.yvedp.cn/gttgsmjukz.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.dashuyun.cn/gtarlgvcxi.html

Java: class Node { int v; Node next; }
来源：http://hz.shanyushiyangtech.top/gtwohuslvt.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.jqgfzy.top/gthujpfdew.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.fzhhl.top/gtzigkcmxm.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.jinqigfzy.top/gtbslawcwc.html

[N11] 二叉树中序遍历
来源：http://hz.zhengqikj.top/gtafkgrdrs.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.bjfxy.top/gtazzygkcr.html

PHP:  // 手写递归函数
来源：http://hz.fzhhl.top/gtzdfhnwai.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.fzhhl.top/gtklruqwsx.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.shangyingyoupin.top/gtmcmnyphg.html

Java: // 手写递归
来源：http://hz.zhengqikj.top/gttbncmiqb.html

Go:   // 手写递归
来源：http://hz.zhixingplan.top/gtdufyocbu.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.zhengqikj.top/gtgpltkijb.html

C#:   // 手写递归
来源：http://hz.yonumen.top/gtyabaohyt.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.0kj1m.cn/gtrveqbkxw.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.havefunace.top/gticxndxii.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.ywan-chungtsiang.top/gtavygpxsa.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.jyoumei.cn/gtygtijcog.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.yj20258.top/gtfwaicapa.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.zhoulong.xyz/gtiymbvgyk.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.shanyushiyangkeji.top/gtcozwnqeb.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.xuetiantiany.cn/gtfirtuhpa.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.snrcjt.cn/gtwniaglcv.html

================================================================================
来源：http://hz.xylfe.cn/gtsrrghhji.html

O. 并发与异步
来源：http://hz.cucudq.cn/gtqxbzausp.html

================================================================================
来源：http://hz.jqgfzy.top/gtdczwxgho.html

[O01] 启动一个线程
来源：http://hz.iojbl.cn/gtfhobztby.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.zhixingplan.top/gtscuweady.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.jqgfzy.top/gtoxdnghra.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.dianchejie.cn/gtcccchhoo.html

TS:   // 同 JS
来源：http://hz.haohaochexian.top/gtatzjmvtz.html

Java: new Thread(() -> f()).start()
来源：http://hz.haohaochexian.top/gtpgiphyxr.html

Go:   go f()
来源：http://hz.zhijiandao.cn/gtreleoglo.html

Ruby: Thread.new { f }
来源：http://hz.gogol.net.cn/gtibjcpgez.html

C#:   Task.Run(() => F());
来源：http://hz.c1oappe.top/gtjvjpbljg.html

[O02] 使用线程池
来源：http://hz.xingfuxueyuan.xyz/gtbhpijrib.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.hongshengwenyu.top/gtddqbzttc.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.wangdashe.top/gtmbqgnsom.html

JS:   // worker_threads 线程池
来源：http://hz.jinqigufen.top/gtebuqdedd.html

TS:   // worker_threads 线程池
来源：http://hz.ydjk.org.cn/gtrgrykpin.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.sysykeji.top/gtrjrmehdp.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.chenzaomai.com/gtsantclpp.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.nwbrower.top/gtkrudfspb.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.chenlongwang.top/gtyyuserpg.html

[O03] 加锁保护共享数据
来源：http://hz.yonumen.top/gtejoaqgah.html

Py:   with lock: shared += 1
来源：http://hz.vqdsnc.cn/gtcydzdivj.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.yj20258888.top/gtzgksynjv.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.ybcxt.top/gtiqqulgaz.html

TS:   // 同 JS
来源：http://hz.9152youxi.cn/gthgtdzbtr.html

Java: synchronized (this) { shared++; }
来源：http://hz.chenlongwang.top/gtqazjckrb.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.chenzaomai.com/gtpjdkdzfu.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.xuanzx.com/gtrnufblnk.html

C#:   lock (gate) { shared++; }
来源：http://hz.cashguo.top/gtqrjxobli.html

[O04] 定义异步函数并等待
来源：http://hz.hfpthk.cn/gtlsmekggx.html

Py:   async def f():⏎    await g()
来源：http://hz.xinyue.icu/gtubxgllvm.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.yanxiufei.cn/gtkbhmbhos.html

JS:   async function f() { await g(); }
来源：http://hz.xziqi.cn/gtkgtbegvk.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.zhengqikj.top/gthksbyuhm.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.c1oappe.top/gtoezibjfp.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.yj20258888.top/gtlwdosboa.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.sysykeji.top/gtcqmzdjqx.html

C#:   async Task F() { await G(); }
来源：http://hz.ybcxt.top/gtmcnuezow.html

[O05] 并发执行并等待全部完成
来源：http://hz.cheryme.top/gtnwlpqusx.html

Py:   asyncio.gather(*tasks)
来源：http://hz.birdmap.top/gtgzczssff.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.316326.xyz/gtwsrtemnh.html

JS:   await Promise.all(tasks)
来源：http://hz.zhiwuduotai.top/gtnieyehse.html

TS:   await Promise.all(tasks)
来源：http://hz.cashguo.top/gtuzlqiarx.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.vqdsnc.cn/gtoygvqrhm.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.nanxuanxn.top/gtbcocciyz.html

Ruby: threads.map(&:join)
来源：http://hz.dianchejie.cn/gtaytmbfse.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.ppjwa.cn/gtdymggmpn.html

[O06] 使用进程池
来源：http://hz.fzhhl.top/gtqhdmetqb.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.xingfuxueyuan.xyz/gttzbgvhab.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.zycfv.cn/gtlnmhjfdd.html

JS:   // child_process / cluster 模块
来源：http://hz.snrcjt.cn/gtcffomzqf.html

TS:   // child_process / cluster 模块
来源：http://hz.redwolf501.top/gtqdrczkei.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.jiagoushi.top/gtuhyumuot.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.ppjwa.cn/gtrjdbagbm.html

Ruby: // fork 块
来源：http://hz.tian-w.cn/gtbzaomlfs.html

C#:   Parallel.For
来源：http://hz.xingfuxueyuan.xyz/gtngvdkcow.html

================================================================================
来源：http://hz.jqgfzy.top/gtcrhmyxen.html

P. 常用工具函数
来源：http://hz.quarkkingdee.top/gttmkeqjst.html

================================================================================
来源：http://hz.yvedp.cn/gtbpzveais.html

[P01] 生成 UUID
来源：http://hz.9152youxi.cn/gtejzzvcgu.html

Py:   str(uuid.uuid4())
来源：http://hz.meibo888.top/gtqdftdzpe.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.haohaochexian.top/gtkwvbyscs.html

JS:   crypto.randomUUID()
来源：http://hz.jyoumei.cn/gtzmltergp.html

TS:   crypto.randomUUID()
来源：http://hz.jqgfzy.top/gtkufwmdxa.html

Java: UUID.randomUUID().toString()
来源：http://hz.yuxming.cn/gtytemufie.html

Go:   // 用 github.com/google/uuid
来源：http://hz.52xcode.cn/gtfpwztffa.html

Ruby: SecureRandom.uuid
来源：http://hz.chenjidiqi.icu/gtiqwvatpa.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.havefunace.top/gtrerislme.html

[P02] MD5 / SHA256 摘要
来源：http://hz.jlsjyb.cn/gtwirgfpmf.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.pengpengdd.cyou/gtbskppllw.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.xingfuxueyuan.xyz/gtahzophhk.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.jianghu66.top/gthfnnpgnn.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.ybcxt.top/gtgsrdxezy.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.xylfe.cn/gtavqlpqvc.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.sufxvd.cn/gtgsxepbfv.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.zycfv.cn/gtdsjnlnqk.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.chenlongwang.top/gthqlobxgo.html

[P03] 生成短随机字符串
来源：http://hz.birdmap.top/gtfjmdshii.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.jinqigufen.top/gtynqbbgyl.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.hysaishi.cn/gtswqagsmc.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.zycfv.cn/gtovdcyeto.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.xziqi.cn/gtomqudskj.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.ydzc1.top/gtneqfpwiz.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.snrcjt.cn/gtnhmspmnd.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.chenzaomai.com/gtngakfsft.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.dianchejie.cn/gtqlsoilpp.html

[P04] 求长度
来源：http://hz.zhijiandao.cn/gtnxgllstw.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.aizwys.cn/gtbohyrxfm.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.yangfankeji.com/gtjzaabfpp.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.hongshengwenyu.top/gtfodcsvyl.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.pycfn.com/gtsbclfmrv.html

Java: list.size();  map.size();  s.length()
来源：http://hz.andypj.xyz/gtdwlkygjt.html

Go:   len(arr);  len(m)
来源：http://hz.shangyingyoupin.top/gtxhlxgfnh.html

Ruby: x.length;  x.size
来源：http://hz.ydzc1.top/gtwbbmbqmu.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.gzhubu.top/gtnjqbvgjd.html

[P05] 判断两个对象内容是否相等
来源：http://hz.redwolf501.top/gtbnfvicqi.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.gaohongyu789.top/gtbpxyamyz.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.chenzaomai.com/gtvirlcoyv.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.xuetiantiany.cn/gtmoosmhey.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.ivvv.top/gtdwstmatm.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.sxryk.cn/gtigfwvhmq.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.yuxming.cn/gttttddkax.html

Ruby: a == b
来源：http://hz.daria6918.cn/gtzfixzhqk.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.jqgufenzy.top/gtyhmtgghh.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.hongshengwenyu.top/gtbmbqkimh.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.yonumen.top/gtqmqkjrxx.html

PHP:  if (empty($x)) {}
来源：http://hz.cucudq.cn/gtroedneyi.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.yj202588.top/gtiykvhcjg.html

TS:   if (x == null) {}
来源：http://hz.jlsjyb.cn/gtvahkehom.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.snrcjt.cn/gtesujskqz.html

Go:   if x == nil {}
来源：http://hz.pycfn.com/gtybdvfqmr.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.nwbrower.top/gtvvitthci.html

C#:   if (x is null) {}
来源：http://hz.yueranfly.top/gtgmbxptkc.html

[P07] 防抖与节流
来源：http://hz.52xcode.cn/gtmcjqbjku.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.yj202588.top/gtliejnygv.html

PHP:  // 手写时间戳比较
来源：http://hz.zhixingplan.top/gtpcbvkmyb.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.andypj.xyz/gtnujppfeb.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.pycfn.com/gtchzuknvf.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.ppjwa.cn/gtecvpucvg.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.ppjwa.cn/gtkfqjkikd.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.hammf.cn/gtwsagpwqs.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.cheryme.top/gtmewmcbqz.html

[P08] 处理浮点精度问题
来源：http://hz.pengpengdd.cyou/gtgfcougjt.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.nwbrower.top/gthnnmuutt.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.jqgfzy.top/gtzkrcmdft.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.tianlin.xyz/gtbmgtgfty.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.xylfe.cn/gtozmiygvy.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.xuetiantiany.cn/gtnyblmvrh.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.nanxinkj.top/gtctbtedfi.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.birdmap.top/gtaxucfrbt.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.zhongyouzk.top/gtthtiupol.html

================================================================================
来源：http://hz.bjfxy.top/gtwckscobw.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.cheryme.top/gtbjzgyfbo.html

================================================================================
来源：http://hz.c1oappe.top/gtwoiqkwop.html

[Q01] 创建表
来源：http://hz.ydzc1.top/gtzksvtoae.html

CREATE TABLE users (
来源：http://hz.jinyuanbaomall.cn/gtlvhahlhn.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.hywenlv.cn/gtreaolcrj.html

name VARCHAR(50) NOT NULL,
来源：http://hz.haohaochexian.top/gtgingcpfe.html

email VARCHAR(100) UNIQUE,
来源：http://hz.hfpthk.cn/gtpkrdiyhe.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.zhaomingkeji.xyz/gtccldssoi.html

);
来源：http://hz.jqgfzy.top/gtuawxknxh.html

[Q02] 创建带外键的表
来源：http://hz.ydzc1.top/gtuwibwfam.html

CREATE TABLE orders (
来源：http://hz.xuetiantiany.cn/gtsecpirlg.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.jinyuanbaomall.cn/gtlsrmtule.html

user_id INT NOT NULL,
来源：http://hz.sufxvd.cn/gtkfspzisy.html

amount DECIMAL(10, 2),
来源：http://hz.xingfuxueyuan.xyz/gtyuvbqcxj.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.redwolf501.top/gtanaiogdn.html

);
来源：http://hz.havefunace.top/gtvstkpmhw.html

[Q03] 增加列
来源：http://hz.hywenlv.cn/gtellyruel.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.yvedp.cn/gtivovofbo.html

[Q04] 修改列类型
来源：http://hz.quarkkingdee.top/gtkilodymo.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.meibo888.top/gtbhpeyrie.html

[Q05] 重命名列
来源：http://hz.shangyingyoupin.top/gtkxqngxcv.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.guannengcc.top/gtzlnmncvc.html

[Q06] 删除列
来源：http://hz.ybcxt.top/gtumzsmysy.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.yuxming.cn/gtqffzmqyk.html

[Q07] 删除表
来源：http://hz.zycfv.cn/gtsxiukbzm.html

DROP TABLE IF EXISTS orders;
来源：http://hz.sufxvd.cn/gtbfpthmep.html

[Q08] 创建普通索引
来源：http://hz.svipenyu.cn/gttdyxchob.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.smart0.xyz/gtgixfhgyd.html

[Q09] 创建唯一索引
来源：http://hz.hysaishi.cn/gtdpzvgndq.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.zdqjudy.top/gtncxntqwi.html

[Q10] 插入单行
来源：http://hz.shangyingyoupin.top/gtdcousexo.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.shzxlz.cn/gtyamvwcyq.html

[Q11] 一次插入多行
来源：http://hz.shuidangran.top/gtztheattv.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.yuanzhike.top/gtlnhmqqmp.html

[Q12] 插入后取自增 ID
来源：http://hz.wangshuangyany.cn/gtvfxylsqp.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.cashguo.top/gterjwtijn.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.ydjk.org.cn/gtyvoxcbfh.html

[Q13] 忽略重复插入
来源：http://hz.ywan-chungtsiang.top/gtixicqstf.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.dashuyun.cn/gtfhadddbk.html

[Q14] 存在则更新（upsert）
来源：http://hz.yueranfly.top/gttzpnlkez.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.yanxiufei.cn/gtrwqyuqex.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.dianchejie.cn/gtuugnwoqy.html

[Q15] 查询全部
来源：http://hz.52xcode.cn/gtlruzasfv.html

SELECT * FROM users;
来源：http://hz.pycfn.com/gtxhdxzylw.html

[Q16] 查询指定列
来源：http://hz.yj202588.top/gthlbhkxmo.html

SELECT id, name FROM users;
来源：http://hz.yueranfly.top/gtlrysyzvh.html

[Q17] 条件查询
来源：http://hz.hysaishi.cn/gtvjehkqlg.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.snrcjt.cn/gtgxdwnjze.html

[Q18] 模糊匹配
来源：http://hz.xylfe.cn/gtayxfzbeu.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.wangdashe.top/gtyubgsogg.html

[Q19] 范围查询
来源：http://hz.nanxuanxn.top/gtxwrlpfaj.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.ydzc1.top/gtdrmqfabt.html

[Q20] IN 列表
来源：http://hz.zhoulong.xyz/gtkkhirvvh.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.shangyingyoupin.top/gtcrxasrqx.html

[Q21] 空值判断
来源：http://hz.ywan-chungtsiang.top/gtckzkobid.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.ybcxt.top/gtuwoygagu.html

[Q22] 排序
来源：http://hz.nanxinkj.top/gtzbrzijzt.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.xylfe.cn/gtoibwjbka.html

[Q23] 分页
来源：http://hz.jinqigfzy.top/gtkqebkcka.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.yueranfly.top/gtlefxotlw.html

[Q24] 去重
来源：http://hz.tian-w.cn/gtgfshkyqx.html

SELECT DISTINCT city FROM users;
来源：http://hz.zdqjudy.top/gtewlkogrg.html

[Q25] 只取前 N 条
来源：http://hz.birdmap.top/gtlughcgvp.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.chenjidiqi.icu/gtgcfwbkjo.html

[Q26] 计数
来源：http://hz.wangdashe.top/gtivngftmv.html

SELECT COUNT(*) FROM users;
来源：http://hz.jqgfzy.top/gtrsnwxhaq.html

[Q27] 条件计数
来源：http://hz.andypj.xyz/gttpvwopwi.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.fengsongda.top/gtobhdwqsl.html

[Q28] 求和与平均
来源：http://hz.chenjidiqi.icu/gtsdeqqoad.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.hysaishi.cn/gtwzalhtru.html

[Q29] 最大最小值
来源：http://hz.yj20258888.top/gtiwpscecy.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.52xcode.cn/gtryuyirld.html

[Q30] 分组统计
来源：http://hz.smart0.xyz/gtqxtqxlzn.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.cdnleiting.top/gtfdfjgmxf.html

[Q31] 分组后过滤
来源：http://hz.ehwqpu.com/gtamcedxdo.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.feifeiyinyue.top/gtmzavkoiz.html

[Q32] 分组拼接字符串
来源：http://hz.hnxiangtu.top/gtatktblka.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.gaohongyu789.top/gtmjgrwmfw.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.yj20258888.top/gtbxwuaglj.html

[Q33] 多列分组
来源：http://hz.xziqi.cn/gtxtxksznn.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.nanxuanxn.top/gtfonvywyp.html

[Q34] 每组取第一条
来源：http://hz.hnxiangtu.top/gtqoqxhwsv.html

SELECT * FROM (
来源：http://hz.haohaochexian.top/gtbaxcjrkk.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.kuanghao11.cn/gtnrxjsnyl.html

) t WHERE rn = 1;
来源：http://hz.cheryme.top/gtcxkttmiv.html

[Q35] 内连接
来源：http://hz.jinqigufen.top/gtbfwbnaxi.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.dianchejie.cn/gthgrodnmu.html


<!-- 参考信息 -->