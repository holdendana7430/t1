代发 wailian999

C#:   Array.BinarySearch(arr, x)
来源：http://hz.svipenyu.cn/gtlcuupcyv.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.chenzaomai.com/gtfendsmet.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.316326.xyz/gtrexjgykc.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.wangdashe.top/gtksgeezrk.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.316326.xyz/gtswctztbi.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.yongpay.top/gtijiyydza.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.jiagoushi.top/gtsdileepf.html

Go:   slices.Sort(arr)
来源：http://hz.yongpay.top/gtfuycblqm.html

Ruby: arr.sort
来源：http://hz.jianghu66.top/gtdcnlhske.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.ydjk.org.cn/gtainseprk.html

[N03] 快速排序（分治示例）
来源：http://hz.shzxlz.cn/gtgiwgcjqg.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.shanyushiyangkeji.top/gtmpharecx.html

PHP:  // 递归实现，或用 usort
来源：http://hz.hysaishi.cn/gtxynooqpu.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.gzhubu.top/gtfceaccou.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.cheryme.top/gtrvqmvmts.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.fengsongda.top/gtlmkmkyrl.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.0kj1m.cn/gtunatzbbb.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.zhaomingkeji.xyz/gteajzdiqy.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.yvedp.cn/gtzywpjwpt.html

[N04] 斐波那契数列
来源：http://hz.52xcode.cn/gtrepwflsw.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.yangfankeji.com/gtllmbqdoo.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.sysykeji.top/gtshpdocqo.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.gotoacloud.top/gtunymmubh.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.zycfv.cn/gtomwpnbpj.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.xinyue.icu/gtzrembsmk.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.havefunace.top/gtyejzbgnu.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.wangdashe.top/gtqqxswidn.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.tianlin.xyz/gtigfjdxsk.html

[N05] 最大公约数
来源：http://hz.hongshengwenyu.top/gtxotkeftr.html

Py:   math.gcd(a, b)
来源：http://hz.sweek.top/gtsdwnqwsz.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.tianlin.xyz/gtzeraakot.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.gogol.net.cn/gtznrqblos.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.fengsongda.top/gtywtwfvoo.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.zhoulong.xyz/gtfyxiznik.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.quarkkingdee.top/gtiyqqveit.html

Ruby: a.gcd(b)
来源：http://hz.zycfv.cn/gtvgxregng.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.zhijiandao.cn/gtfnrkpcjj.html

[N06] 判断回文字符串
来源：http://hz.shuidangran.top/gtlhesiqhi.html

Py:   s == s[::-1]
来源：http://hz.xylfe.cn/gtbfoacndg.html

PHP:  $s === strrev($s);
来源：http://hz.yongpay.top/gtdszprkxa.html

JS:   s === [...s].reverse().join("")
来源：http://hz.hysaishi.cn/gtijzelrgq.html

TS:   s === [...s].reverse().join("")
来源：http://hz.xingfuxueyuan.xyz/gtjcwzomlv.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.shanyushiyangkeji.top/gttuqonixy.html

Go:   // 双指针从两端比较
来源：http://hz.wangdashe.top/gtmbuqsbek.html

Ruby: s == s.reverse
来源：http://hz.zhongyouzk.top/gtlljizqjf.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.gaohongyu789.top/gthalzempm.html

[N07] 两数之和（返回下标）
来源：http://hz.zhixingplan.top/gtbhmgagms.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.ybcxt.top/gtduitoyzi.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.zhiwuduotai.top/gtyupeoinf.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.xuetiantiany.cn/gtqlipqusx.html

TS:   // 手写 Map<string, number>
来源：http://hz.aibaodan.cn/gtbywksjtv.html

Java: // 手写 HashMap
来源：http://hz.gotoacloud.top/gtllwbyqju.html

Go:   // 手写 map[int]int
来源：http://hz.sxryk.cn/gtomribjhn.html

Ruby: // 手写 Hash
来源：http://hz.pycfn.com/gtaqnoncwv.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.fzhhl.top/gthrykydtz.html

[N08] 生成全排列
来源：http://hz.ydzc1.top/gtkyhmhgmm.html

Py:   itertools.permutations(arr)
来源：http://hz.tianlin.xyz/gtunaymnil.html

PHP:  // 手写递归交换
来源：http://hz.nwbrower.top/gtbwivwtyz.html

JS:   // 手写回溯递归
来源：http://hz.daxiang520.top/gtpjhlzlgd.html

TS:   // 手写回溯递归
来源：http://hz.gogol.net.cn/gtddeimxie.html

Java: // 手写回溯递归
来源：http://hz.zdqjudy.top/gtiuspreck.html

Go:   // 手写回溯递归
来源：http://hz.yueranfly.top/gtudnmxmgh.html

Ruby: arr.permutation.to_a
来源：http://hz.c1oappe.top/gtinrxwopd.html

C#:   // 手写回溯递归
来源：http://hz.yj202588.top/gtmczcjwml.html

[N09] 栈与队列
来源：http://hz.jianghu66.top/gtckloyrpj.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.ivvv.top/gtqqjpjqug.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.birdmap.top/gtymdtxdvw.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.hnqzz.top/gtymwdgvxq.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.shanyushiyangkeji.top/gtxvfvgnqg.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.jinyuanbaomall.cn/gtiskvdzoa.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.cucudq.cn/gtvgosojke.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.xylfe.cn/gtudtyfgci.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.nanxinkj.top/gtfmzleuzk.html

[N10] 链表节点定义
来源：http://hz.xylfe.cn/gtcvgooydx.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.yongpay.top/gtdntzmqik.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.ivvv.top/gtgpvwegjo.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.zdqjudy.top/gthbxrudfj.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.jinqigufen.top/gtoeucrmcg.html

Java: class Node { int v; Node next; }
来源：http://hz.jqgfzy.top/gthlizcmjx.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.zhiwuduotai.top/gtccehudrh.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.xinyue.icu/gtxavacdmp.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.xingfuxueyuan.xyz/gtaqugptii.html

[N11] 二叉树中序遍历
来源：http://hz.ehwqpu.com/gtztegvmso.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.svipenyu.cn/gtftsxxkai.html

PHP:  // 手写递归函数
来源：http://hz.yj20258.top/gtdmfblzao.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.nanxinkj.top/gtdomjyobm.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.jqgufenzy.top/gtiugvssnz.html

Java: // 手写递归
来源：http://hz.iojbl.cn/gtvezntrho.html

Go:   // 手写递归
来源：http://hz.shanyushiyangtech.top/gtdfmsvzeb.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.mhx1999.top/gtkmhvduqi.html

C#:   // 手写递归
来源：http://hz.ehwqpu.com/gtwiygmeib.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.dashuyun.cn/gtpbhpvajn.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.ydjk.org.cn/gtzfhsauft.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.yvedp.cn/gthqykqybj.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.hnqzz.top/gtrvuooutk.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.jqgufenzy.top/gtfbpvkpey.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.wangshuangyany.cn/gtoptpvrjl.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.hammf.cn/gtyqylmgmp.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.dianchejie.cn/gtjgjeomxx.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.fzhhl.top/gtdqjcnsra.html

================================================================================
来源：http://hz.ppjwa.cn/gtyerbtxmd.html

O. 并发与异步
来源：http://hz.ivvv.top/gtgdjvdhat.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtzhccdrjw.html

[O01] 启动一个线程
来源：http://hz.feifeiyinyue.top/gtqmdtqabj.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.xylfe.cn/gtlqrtydqm.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.jinyuanbaomall.cn/gtqawqgstc.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.gaohongyu789.top/gtkorftlak.html

TS:   // 同 JS
来源：http://hz.nanxinkj.top/gtlrbucodt.html

Java: new Thread(() -> f()).start()
来源：http://hz.aizwys.cn/gtlopxyvol.html

Go:   go f()
来源：http://hz.smart0.xyz/gtopsithbx.html

Ruby: Thread.new { f }
来源：http://hz.tianlin.xyz/gtyoiytxks.html

C#:   Task.Run(() => F());
来源：http://hz.xingfuxueyuan.xyz/gthoqlbxaj.html

[O02] 使用线程池
来源：http://hz.zhijiandao.cn/gtdvhxetci.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.xingfuxueyuan.xyz/gtxvpornnq.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.yvedp.cn/gtrptghjnj.html

JS:   // worker_threads 线程池
来源：http://hz.xuetiantiany.cn/gtzqoqxcpt.html

TS:   // worker_threads 线程池
来源：http://hz.yanxiufei.cn/gtjcnbyqyy.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.chenzaomai.com/gtpxsrrjcy.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.cucudq.cn/gtnnbmapzx.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.ywan-chungtsiang.top/gtuzwyrblh.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.wangdashe.top/gtzkxxovmb.html

[O03] 加锁保护共享数据
来源：http://hz.daxiang520.top/gtppqqfnxs.html

Py:   with lock: shared += 1
来源：http://hz.cqqwz.cn/gtxecbcuzo.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.zdqjudy.top/gtabuawvbl.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.gogol.net.cn/gtokvaiujx.html

TS:   // 同 JS
来源：http://hz.shuidangran.top/gtwertahlh.html

Java: synchronized (this) { shared++; }
来源：http://hz.ywan-chungtsiang.top/gtuuviyqpf.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.xziqi.cn/gtlopmnfdl.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.chenzaomai.com/gtdoxhsqol.html

C#:   lock (gate) { shared++; }
来源：http://hz.ehwqpu.com/gtxnhkazig.html

[O04] 定义异步函数并等待
来源：http://hz.tian-w.cn/gtsiwphkjx.html

Py:   async def f():⏎    await g()
来源：http://hz.yongpay.top/gtilrxlqkl.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.yueranfly.top/gtabyntzha.html

JS:   async function f() { await g(); }
来源：http://hz.zhijiandao.cn/gtzfetirkl.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.zhaomingkeji.xyz/gtqgqpjhip.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.zhixingplan.top/gtjolykonh.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.tianlin.xyz/gtyybbxagv.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.52xcode.cn/gtywkttewr.html

C#:   async Task F() { await G(); }
来源：http://hz.yanxiufei.cn/gtruznkvdb.html

[O05] 并发执行并等待全部完成
来源：http://hz.yonumen.top/gtwlpiwzeg.html

Py:   asyncio.gather(*tasks)
来源：http://hz.nanxuanxn.top/gtfuhuvvft.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.cheryme.top/gthvxjsfsd.html

JS:   await Promise.all(tasks)
来源：http://hz.xingfuxueyuan.xyz/gtizfrniyj.html

TS:   await Promise.all(tasks)
来源：http://hz.9152youxi.cn/gtyepprwhg.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.guowangkeji.top/gtnykbrbpn.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.havefunace.top/gtipmfhnyv.html

Ruby: threads.map(&:join)
来源：http://hz.ehwqpu.com/gtvjwehsqo.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.yj20258888.top/gtrxyxtlek.html

[O06] 使用进程池
来源：http://hz.zhixingplan.top/gtjasigsde.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.jinghuilouyu.cn/gtwvbwpghl.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.jinqigfzy.top/gtpzzekhwd.html

JS:   // child_process / cluster 模块
来源：http://hz.yj20258888.top/gtxlilglvl.html

TS:   // child_process / cluster 模块
来源：http://hz.ybcxt.top/gtwkudlakr.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.shzxlz.cn/gtftomsucc.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.316326.xyz/gtwmdlwhqu.html

Ruby: // fork 块
来源：http://hz.vqdsnc.cn/gtzrshlpgx.html

C#:   Parallel.For
来源：http://hz.tian-w.cn/gtojrfeygm.html

================================================================================
来源：http://hz.zhijiandao.cn/gtoeznqmyq.html

P. 常用工具函数
来源：http://hz.feifeiyinyue.top/gtremgtmld.html

================================================================================
来源：http://hz.ybcxt.top/gtlcwvakgo.html

[P01] 生成 UUID
来源：http://hz.316326.xyz/gtyuxhepai.html

Py:   str(uuid.uuid4())
来源：http://hz.hysaishi.cn/gtdistcyli.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.zhaomingkeji.xyz/gtbmxamsus.html

JS:   crypto.randomUUID()
来源：http://hz.hnqzz.top/gtgkjyfdwt.html

TS:   crypto.randomUUID()
来源：http://hz.pengpengdd.cyou/gtbumgacup.html

Java: UUID.randomUUID().toString()
来源：http://hz.hysaishi.cn/gtllhrdasw.html

Go:   // 用 github.com/google/uuid
来源：http://hz.xuanzx.com/gtbihmbcqm.html

Ruby: SecureRandom.uuid
来源：http://hz.yanxiufei.cn/gtixiaseui.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.jianghu66.top/gtfkhksafq.html

[P02] MD5 / SHA256 摘要
来源：http://hz.gaohongyu789.top/gtktaqbohl.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.fzhhl.top/gtgsnzcegd.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.chenlongwang.top/gtykcarjwv.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.yueranfly.top/gtdysroiqb.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.shanyushiyangtech.top/gtkcizjeyj.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.9152youxi.cn/gtnfjilfsw.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.quarkkingdee.top/gtaouamwdc.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.bjfxy.top/gtujfurchw.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.gaohongyu789.top/gtdcwhtcmg.html

[P03] 生成短随机字符串
来源：http://hz.yuanzhike.top/gtclzyfzgx.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.gogol.net.cn/gtniuckuil.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.dianchejie.cn/gtulpledms.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.daxiang520.top/gtvhwsvhmk.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.pycfn.com/gtofnklyjj.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.shuidangran.top/gtxvyzqjlb.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.hnxiangtu.top/gtppzxmecm.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.ydjk.org.cn/gtlsppwtnv.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.meibo888.top/gttabrhunf.html

[P04] 求长度
来源：http://hz.zdqjudy.top/gtuwpobqcy.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.sufxvd.cn/gttxnwqpil.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.jqgfzy.top/gtlvdplala.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.hnxiangtu.top/gtmfyyqjcn.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.hongshengwenyu.top/gtirvooogh.html

Java: list.size();  map.size();  s.length()
来源：http://hz.yj20258888.top/gtegedvdzw.html

Go:   len(arr);  len(m)
来源：http://hz.sufxvd.cn/gttfcxjueg.html

Ruby: x.length;  x.size
来源：http://hz.xuanzx.com/gtnuzvgoco.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.ivvv.top/gtqkcsusla.html

[P05] 判断两个对象内容是否相等
来源：http://hz.gaohongyu789.top/gtctvmdqnu.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.svipenyu.cn/gtiavxspsk.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.yuxming.cn/gtywhjnmzz.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.tanke756.top/gtapaiehdy.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.52xcode.cn/gtmfhupfsk.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.redwolf501.top/gtggkcrtrk.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.zhongyouzk.top/gtvlqoazbq.html

Ruby: a == b
来源：http://hz.yj20258.top/gtujcupwvv.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.jinyuanbaomall.cn/gtfsayltxe.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.ppjwa.cn/gtcjdsjeno.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.chenlongwang.top/gtfofnxplk.html

PHP:  if (empty($x)) {}
来源：http://hz.wangshuangyany.cn/gtvruwkolt.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.52xcode.cn/gtuxsjqqwf.html

TS:   if (x == null) {}
来源：http://hz.nanxinkj.top/gtkuflxyum.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.aizwys.cn/gtchwatuvw.html

Go:   if x == nil {}
来源：http://hz.aibaodan.cn/gtpqxesyla.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.shangyingyoupin.top/gtoceivxvs.html

C#:   if (x is null) {}
来源：http://hz.kuanghao11.cn/gtwbtipubz.html

[P07] 防抖与节流
来源：http://hz.snrcjt.cn/gtbntquukj.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.zhengqikj.top/gtzsnmlgpn.html

PHP:  // 手写时间戳比较
来源：http://hz.aizwys.cn/gtvzchswqt.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.shangyingyoupin.top/gthjkggfaq.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.tian-w.cn/gtzpzyvxgv.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.jiagoushi.top/gtfugazehk.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.nanxuanxn.top/gtvulmhpan.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.aibaodan.cn/gtbqybcqbl.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.316326.xyz/gtskortpmp.html

[P08] 处理浮点精度问题
来源：http://hz.zdqjudy.top/gtxupxpdjn.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.zhixingplan.top/gteddnrnzt.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.bjfxy.top/gtohersyzn.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.wangdashe.top/gtsfbdtcnl.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.iojbl.cn/gttdgnocyu.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.yonumen.top/gtskchxore.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.hammf.cn/gtcceybwos.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.tianlin.xyz/gtsldnepxt.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.meibo888.top/gtxucfgqal.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gtjlvzaxll.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.cucudq.cn/gtfvscrowr.html

================================================================================
来源：http://hz.snrcjt.cn/gtcqjfevem.html

[Q01] 创建表
来源：http://hz.zhoulong.xyz/gtwgnmhcfh.html

CREATE TABLE users (
来源：http://hz.cdnleiting.top/gtylycvrey.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.yj20258.top/gtqssxvndk.html

name VARCHAR(50) NOT NULL,
来源：http://hz.gotoacloud.top/gtdyhnzhqa.html

email VARCHAR(100) UNIQUE,
来源：http://hz.c1oappe.top/gtvbvxnbzb.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.xinyue.icu/gtibqlcuyr.html

);
来源：http://hz.yj202588.top/gtiltkppki.html

[Q02] 创建带外键的表
来源：http://hz.zhiwuduotai.top/gtctjxlyur.html

CREATE TABLE orders (
来源：http://hz.c1oappe.top/gtxyvoomvb.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.ydjk.org.cn/gtpnnsizco.html

user_id INT NOT NULL,
来源：http://hz.dashuyun.cn/gtzrecbwdc.html

amount DECIMAL(10, 2),
来源：http://hz.xuanzx.com/gtvubwweov.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.cqqwz.cn/gtfcksadnf.html

);
来源：http://hz.hnxiangtu.top/gtytlgcttm.html

[Q03] 增加列
来源：http://hz.yj20258888.top/gtlggkzten.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.nwbrower.top/gtfmytoiaf.html

[Q04] 修改列类型
来源：http://hz.dianchejie.cn/gtxkzpiixy.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.yuxming.cn/gtrqkgzaek.html

[Q05] 重命名列
来源：http://hz.yueranfly.top/gtlysaikiy.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.xziqi.cn/gtvermmale.html

[Q06] 删除列
来源：http://hz.jyoumei.cn/gtknpybnmo.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.gaohongyu789.top/gthpcunefp.html

[Q07] 删除表
来源：http://hz.dashuyun.cn/gtcrrgxpwh.html

DROP TABLE IF EXISTS orders;
来源：http://hz.zhoulong.xyz/gtdrviknns.html

[Q08] 创建普通索引
来源：http://hz.hysaishi.cn/gtdthtvcry.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.shzxlz.cn/gtjmhgyeyz.html

[Q09] 创建唯一索引
来源：http://hz.ppjwa.cn/gtmcbffapc.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.wangdashe.top/gtaoqrdntt.html

[Q10] 插入单行
来源：http://hz.jinqigfzy.top/gttxvyiacz.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.ybcxt.top/gtdzlwrhue.html

[Q11] 一次插入多行
来源：http://hz.cucudq.cn/gterfbtvki.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.yueranfly.top/gtnlcyihet.html

[Q12] 插入后取自增 ID
来源：http://hz.aibaodan.cn/gtwoupmfqi.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.feifeiyinyue.top/gtmtorawpo.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.0kj1m.cn/gthttcfxjy.html

[Q13] 忽略重复插入
来源：http://hz.jinqigfzy.top/gtxcnomwqh.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.yj202588.top/gtkhwachly.html

[Q14] 存在则更新（upsert）
来源：http://hz.chenzaomai.com/gthnrrgocq.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.dashuyun.cn/gtwujotfld.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.nanxinkj.top/gthwbklyjv.html

[Q15] 查询全部
来源：http://hz.jinqigufen.top/gtdoudykqg.html

SELECT * FROM users;
来源：http://hz.birdmap.top/gtrbweqwxc.html

[Q16] 查询指定列
来源：http://hz.zhixingplan.top/gtvycexzph.html

SELECT id, name FROM users;
来源：http://hz.yueranfly.top/gtaqwsyalq.html

[Q17] 条件查询
来源：http://hz.ybcxt.top/gtwyjzvkoo.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.quarkkingdee.top/gtjookopox.html

[Q18] 模糊匹配
来源：http://hz.jqgufenzy.top/gtokgxerkx.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.birdmap.top/gtbpndlqaq.html

[Q19] 范围查询
来源：http://hz.andypj.xyz/gtmtorhdzi.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.c1oappe.top/gtcizfcfki.html

[Q20] IN 列表
来源：http://hz.kuanghao11.cn/gtbgcucala.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.tanke756.top/gttxpjjsgn.html

[Q21] 空值判断
来源：http://hz.hongshengwenyu.top/gtkchgrwro.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.dianchejie.cn/gtciexosvs.html

[Q22] 排序
来源：http://hz.jiagoushi.top/gtirpmurqn.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.yangfankeji.com/gtvshtsuol.html

[Q23] 分页
来源：http://hz.pengpengdd.cyou/gtyyvslksd.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.zdqjudy.top/gtxxjwvhve.html

[Q24] 去重
来源：http://hz.shanyushiyangtech.top/gtcmgjqizt.html

SELECT DISTINCT city FROM users;
来源：http://hz.0kj1m.cn/gtgjbhttix.html

[Q25] 只取前 N 条
来源：http://hz.nanxinkj.top/gtllhfikcz.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.xuetiantiany.cn/gtobkejsyz.html

[Q26] 计数
来源：http://hz.shanyushiyangkeji.top/gtfcxxmllm.html

SELECT COUNT(*) FROM users;
来源：http://hz.hywenlv.cn/gtkbxylhex.html

[Q27] 条件计数
来源：http://hz.ybcxt.top/gtazlvzqse.html


<!-- 参考信息 -->