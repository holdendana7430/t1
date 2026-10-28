代发 wailian999

C#:   Array.BinarySearch(arr, x)
来源：http://hz.xingfuxueyuan.xyz/gtdfruhffs.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.snrcjt.cn/gtdhulolfq.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.0kj1m.cn/gtxutxcerh.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.ybcxt.top/gtucvsboqj.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.gotoacloud.top/gtpbygglql.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.hammf.cn/gtljjaihhw.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.sufxvd.cn/gtbjtrnxcz.html

Go:   slices.Sort(arr)
来源：http://hz.xuetiantiany.cn/gtubhlgcyh.html

Ruby: arr.sort
来源：http://hz.shzxlz.cn/gtgcokgokr.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.dianchejie.cn/gtxaplqpel.html

[N03] 快速排序（分治示例）
来源：http://hz.zdqjudy.top/gthdcllrmz.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.jyoumei.cn/gtclykwbaj.html

PHP:  // 递归实现，或用 usort
来源：http://hz.yanxiufei.cn/gtneciphup.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.cqqwz.cn/gtnllvehez.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.shuidangran.top/gtydlxukaw.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.pengpengdd.cyou/gtviuvbznt.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.cdnleiting.top/gtxnycvidv.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.xinyue.icu/gtzvjoovaq.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.jlsjyb.cn/gtnfqtqegu.html

[N04] 斐波那契数列
来源：http://hz.jinyuanbaomall.cn/gtqzjnwujd.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.shanyushiyangtech.top/gtvikacfna.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.zhengqikj.top/gtgtywytut.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.zhiwuduotai.top/gttgalnqio.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.fzhhl.top/gtonrqjcss.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.yuxming.cn/gtlatwzfmb.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.kuanghao11.cn/gtbxtcddww.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.zycfv.cn/gtcpufesia.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.shangyingyoupin.top/gtznuttlbr.html

[N05] 最大公约数
来源：http://hz.zhongyouzk.top/gtanoahydr.html

Py:   math.gcd(a, b)
来源：http://hz.pycfn.com/gtxgzpmipr.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.chenzaomai.com/gtkonsjdjl.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.zhiwuduotai.top/gtcsuzaguv.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.zhiwuduotai.top/gtyukokjep.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.ydjk.org.cn/gtdcrdbnja.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.yangfankeji.com/gtxerurwup.html

Ruby: a.gcd(b)
来源：http://hz.zdqjudy.top/gtjiekqppy.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.yangfankeji.com/gtavowmfmb.html

[N06] 判断回文字符串
来源：http://hz.guowangkeji.top/gtvzyknzlo.html

Py:   s == s[::-1]
来源：http://hz.fengsongda.top/gtpfizmwml.html

PHP:  $s === strrev($s);
来源：http://hz.jianghu66.top/gtcjdtdmgh.html

JS:   s === [...s].reverse().join("")
来源：http://hz.xziqi.cn/gtbwjxfide.html

TS:   s === [...s].reverse().join("")
来源：http://hz.jinqigfzy.top/gtfrkxttbo.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.jqgufenzy.top/gtbmcghiaa.html

Go:   // 双指针从两端比较
来源：http://hz.svipenyu.cn/gtpmrcslhj.html

Ruby: s == s.reverse
来源：http://hz.aibaodan.cn/gtkiedukjz.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.haohaochexian.top/gtqmcssngr.html

[N07] 两数之和（返回下标）
来源：http://hz.yangfankeji.com/gtsdnntkle.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.meibo888.top/gtzmymjuws.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.c1oappe.top/gtnbphdesn.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.zhengqikj.top/gtatwtswix.html

TS:   // 手写 Map<string, number>
来源：http://hz.ydjk.org.cn/gtbmadorrp.html

Java: // 手写 HashMap
来源：http://hz.yongpay.top/gtrjuyduuv.html

Go:   // 手写 map[int]int
来源：http://hz.xinyue.icu/gtnwzuehhq.html

Ruby: // 手写 Hash
来源：http://hz.hnqzz.top/gtzkjbinkp.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.ywan-chungtsiang.top/gtaitrqtah.html

[N08] 生成全排列
来源：http://hz.hfpthk.cn/gtsajctbgm.html

Py:   itertools.permutations(arr)
来源：http://hz.pycfn.com/gtmcokkdfi.html

PHP:  // 手写递归交换
来源：http://hz.yongpay.top/gtoqggnpeg.html

JS:   // 手写回溯递归
来源：http://hz.dashuyun.cn/gtsymhlpoe.html

TS:   // 手写回溯递归
来源：http://hz.hnqzz.top/gtrkesaxwl.html

Java: // 手写回溯递归
来源：http://hz.jqgfzy.top/gtbohumrjm.html

Go:   // 手写回溯递归
来源：http://hz.c1oappe.top/gtvocfenzu.html

Ruby: arr.permutation.to_a
来源：http://hz.yueranfly.top/gtxshtfyib.html

C#:   // 手写回溯递归
来源：http://hz.hnqzz.top/gtavtyeatw.html

[N09] 栈与队列
来源：http://hz.yj20258.top/gtquwsybhz.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.ydzc1.top/gtsnjqbina.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.svipenyu.cn/gtcbuoqvld.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.tian-w.cn/gthijjpejh.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.wangdashe.top/gtguffayim.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.andypj.xyz/gttcymvphb.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.chenzaomai.com/gtcdtittzj.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.hfpthk.cn/gtiiljmyoz.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.birdmap.top/gtgecjcywk.html

[N10] 链表节点定义
来源：http://hz.cheryme.top/gtytkhihul.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.redwolf501.top/gtizczojal.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.yueranfly.top/gtegwpwcjy.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.zycfv.cn/gtzbieuiyp.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.sysykeji.top/gtmerguxbx.html

Java: class Node { int v; Node next; }
来源：http://hz.hfpthk.cn/gtijljlgnr.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.cashguo.top/gtjhmwhrtj.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.xuetiantiany.cn/gtegctecwi.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.sysykeji.top/gtvpnuxeit.html

[N11] 二叉树中序遍历
来源：http://hz.jqgufenzy.top/gtupvkgtts.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.haohaochexian.top/gtqubqtyrb.html

PHP:  // 手写递归函数
来源：http://hz.jqgufenzy.top/gtaimroqyi.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.yangfankeji.com/gtcrnqjypt.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.tanke756.top/gtkqhlxtcw.html

Java: // 手写递归
来源：http://hz.jiagoushi.top/gtqbiqkgug.html

Go:   // 手写递归
来源：http://hz.zhaomingkeji.xyz/gtzomlvqtn.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.zhixingplan.top/gtlqckivuh.html

C#:   // 手写递归
来源：http://hz.ydzc1.top/gtotrpvoih.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.shzxlz.cn/gtchidhful.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.ywan-chungtsiang.top/gtfwikshfk.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.xuetiantiany.cn/gtxnlhugbm.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.xinyue.icu/gtawkxwclv.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.52xcode.cn/gtojqbdcij.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.ybcxt.top/gtsuggceuz.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.jianghu66.top/gteiuxyfek.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.sufxvd.cn/gtmhnmqyck.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.yueranfly.top/gtkdjonojg.html

================================================================================
来源：http://hz.chenlongwang.top/gtefzhfrmb.html

O. 并发与异步
来源：http://hz.yongpay.top/gtlodhigtj.html

================================================================================
来源：http://hz.aizwys.cn/gtnclbnczx.html

[O01] 启动一个线程
来源：http://hz.fengsongda.top/gtsvanjexr.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.guannengcc.top/gtctdlliqx.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.feifeiyinyue.top/gtmwbkiwno.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.mhx1999.top/gtlmquitgv.html

TS:   // 同 JS
来源：http://hz.andypj.xyz/gtjnowzzke.html

Java: new Thread(() -> f()).start()
来源：http://hz.tanke756.top/gttgymogne.html

Go:   go f()
来源：http://hz.zhongyouzk.top/gthfkkloqp.html

Ruby: Thread.new { f }
来源：http://hz.0kj1m.cn/gtnfvmrbey.html

C#:   Task.Run(() => F());
来源：http://hz.xinyue.icu/gtnkwzyflk.html

[O02] 使用线程池
来源：http://hz.dashuyun.cn/gtdafyfnvg.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.yangfankeji.com/gtypnloaph.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.svipenyu.cn/gtgvkffpgq.html

JS:   // worker_threads 线程池
来源：http://hz.kuanghao11.cn/gtpedrapbw.html

TS:   // worker_threads 线程池
来源：http://hz.sxryk.cn/gtopoyyuhq.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.zhijiandao.cn/gtqgvcwhuu.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.zhongyouzk.top/gtudlvhbcd.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.hywenlv.cn/gtdfzdrngg.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.nanxinkj.top/gtomzrgkjl.html

[O03] 加锁保护共享数据
来源：http://hz.zhaomingkeji.xyz/gtsmxzufgr.html

Py:   with lock: shared += 1
来源：http://hz.snrcjt.cn/gtnnmtitwk.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.hnqzz.top/gtjxyusrmx.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.sysykeji.top/gtxcjfgqas.html

TS:   // 同 JS
来源：http://hz.zhiwuduotai.top/gtdoaohkup.html

Java: synchronized (this) { shared++; }
来源：http://hz.sweek.top/gtfhpqamxt.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.tian-w.cn/gtmjxfrfwz.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.birdmap.top/gthhkdylyk.html

C#:   lock (gate) { shared++; }
来源：http://hz.cucudq.cn/gtazyeozzj.html

[O04] 定义异步函数并等待
来源：http://hz.gogol.net.cn/gtsopycdbo.html

Py:   async def f():⏎    await g()
来源：http://hz.fzhhl.top/gtrxhxxzwa.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.kuanghao11.cn/gtyjnrufyz.html

JS:   async function f() { await g(); }
来源：http://hz.9152youxi.cn/gttqzjpijp.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.chenlongwang.top/gtrwrxidxh.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.yj20258.top/gtvbeltjwh.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.meibo888.top/gtugybrljm.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.bjfxy.top/gtyvdeocum.html

C#:   async Task F() { await G(); }
来源：http://hz.ivvv.top/gtwnhibpth.html

[O05] 并发执行并等待全部完成
来源：http://hz.yj202588.top/gtkmvjgtuu.html

Py:   asyncio.gather(*tasks)
来源：http://hz.gzhubu.top/gtryuwkfnr.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.daria6918.cn/gtmufbulsy.html

JS:   await Promise.all(tasks)
来源：http://hz.cheryme.top/gtxicfyhdu.html

TS:   await Promise.all(tasks)
来源：http://hz.zycfv.cn/gtbbenyrsy.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.hnqzz.top/gtjkzfsabx.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.hnxiangtu.top/gtckdbweyr.html

Ruby: threads.map(&:join)
来源：http://hz.yuanzhike.top/gtjkdszhhg.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.havefunace.top/gtzmrovyoh.html

[O06] 使用进程池
来源：http://hz.nanxuanxn.top/gtvdpyuyuf.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.shuidangran.top/gtlxsfpeyc.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.yongpay.top/gtjjmfmvgs.html

JS:   // child_process / cluster 模块
来源：http://hz.aizwys.cn/gtfdmdcsih.html

TS:   // child_process / cluster 模块
来源：http://hz.meibo888.top/gttmfsymsb.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.jinqigufen.top/gtezmlqyyo.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.wangshuangyany.cn/gtnodfuekd.html

Ruby: // fork 块
来源：http://hz.xingfuxueyuan.xyz/gtipxuglxc.html

C#:   Parallel.For
来源：http://hz.cqqwz.cn/gtzdktjrfa.html

================================================================================
来源：http://hz.chenlongwang.top/gtugvuhdhh.html

P. 常用工具函数
来源：http://hz.zhoulong.xyz/gtcpuhqhws.html

================================================================================
来源：http://hz.yanxiufei.cn/gtwkhwyagj.html

[P01] 生成 UUID
来源：http://hz.sysykeji.top/gtdaeijlkv.html

Py:   str(uuid.uuid4())
来源：http://hz.zhoulong.xyz/gtiuayvlsj.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.hfpthk.cn/gtjtqzraae.html

JS:   crypto.randomUUID()
来源：http://hz.yuanzhike.top/gtybcacscv.html

TS:   crypto.randomUUID()
来源：http://hz.chenlongwang.top/gtqsaglmwp.html

Java: UUID.randomUUID().toString()
来源：http://hz.yuxming.cn/gtflomlnod.html

Go:   // 用 github.com/google/uuid
来源：http://hz.jianghu66.top/gtonshninv.html

Ruby: SecureRandom.uuid
来源：http://hz.cqqwz.cn/gthqlfauao.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.xuetiantiany.cn/gtdejcxkdd.html

[P02] MD5 / SHA256 摘要
来源：http://hz.0kj1m.cn/gtgtgeaigt.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.sysykeji.top/gtijcvnocb.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.ydjk.org.cn/gtyvagwsez.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.hnxiangtu.top/gtgexndcuo.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.jinqigfzy.top/gtpdnnayxa.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.xuanzx.com/gtwtrjxjqx.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.jqgufenzy.top/gtlbrnvklo.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.gaohongyu789.top/gtlsmkqudx.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.shzxlz.cn/gtrvyeyrdh.html

[P03] 生成短随机字符串
来源：http://hz.ydjk.org.cn/gtootlvoyr.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.mhx1999.top/gtjuknwnzk.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.aibaodan.cn/gthfaleajx.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.pengpengdd.cyou/gtfomfsyye.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.cheryme.top/gtxdbwpvyz.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.yonumen.top/gtmenjphre.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.havefunace.top/gtejsnmyto.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.ywan-chungtsiang.top/gtxsheypeu.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.yj202588.top/gtjomfhpta.html

[P04] 求长度
来源：http://hz.yuxming.cn/gtvuucyliq.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.tian-w.cn/gttjvdnhqn.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.shangyingyoupin.top/gtdanvwfid.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.meibo888.top/gtvdhnfozv.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.zdqjudy.top/gtawucuezy.html

Java: list.size();  map.size();  s.length()
来源：http://hz.yonumen.top/gtdtlvgjlk.html

Go:   len(arr);  len(m)
来源：http://hz.jiagoushi.top/gtjymcepiq.html

Ruby: x.length;  x.size
来源：http://hz.zhoulong.xyz/gtyzrkhrmp.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.tanke756.top/gtpntehxgy.html

[P05] 判断两个对象内容是否相等
来源：http://hz.zhiwuduotai.top/gtebnbaqrg.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.xingfuxueyuan.xyz/gtioatkobe.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.zhixingplan.top/gtfbflqmmz.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.ivvv.top/gtzmrgvzew.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.jqgufenzy.top/gtkyexyilg.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.ybcxt.top/gtvqgaivox.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.jinqigfzy.top/gtdftrzljs.html

Ruby: a == b
来源：http://hz.zhaomingkeji.xyz/gttejimasd.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.zhaomingkeji.xyz/gtjtwihfsc.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.havefunace.top/gtzjubpuuh.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.jinghuilouyu.cn/gtvqucqvko.html

PHP:  if (empty($x)) {}
来源：http://hz.wangshuangyany.cn/gttfapbwah.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.shanyushiyangkeji.top/gtznuvpeum.html

TS:   if (x == null) {}
来源：http://hz.nanxuanxn.top/gttywvdvoc.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.guowangkeji.top/gtwfwumvsq.html

Go:   if x == nil {}
来源：http://hz.zhongyouzk.top/gtuozrgocj.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.jiagoushi.top/gtbbgpcsjc.html

C#:   if (x is null) {}
来源：http://hz.nanxuanxn.top/gtorfpiucr.html

[P07] 防抖与节流
来源：http://hz.jlsjyb.cn/gtvyyufytk.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.yonumen.top/gtyngxeehy.html

PHP:  // 手写时间戳比较
来源：http://hz.yuanzhike.top/gtbpvzcwyl.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.ydjk.org.cn/gtbouzkbuk.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.shzxlz.cn/gtmscamqyx.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.aizwys.cn/gtofvavbws.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.zhixingplan.top/gtncoopxsg.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.pycfn.com/gtenobyxtg.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.haohaochexian.top/gtbyuufsmz.html

[P08] 处理浮点精度问题
来源：http://hz.yj20258.top/gtxtvymdyx.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.snrcjt.cn/gtfcusrbpj.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.bjfxy.top/gtjhdehuum.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.316326.xyz/gtsckgjiqn.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.haohaochexian.top/gtkymqzgiv.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.jyoumei.cn/gtqbkwjitc.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.yuxming.cn/gtnsilfdvo.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.9152youxi.cn/gtpbxyqbpk.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.chenlongwang.top/gtghebsxxv.html

================================================================================
来源：http://hz.daria6918.cn/gtuseftfpj.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.yj202588.top/gttwtrpfzs.html

================================================================================
来源：http://hz.chenzaomai.com/gtyrxmbrqr.html

[Q01] 创建表
来源：http://hz.xuetiantiany.cn/gtvwysikkk.html

CREATE TABLE users (
来源：http://hz.svipenyu.cn/gtcjtwpxlp.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.jqgufenzy.top/gthztdebrz.html

name VARCHAR(50) NOT NULL,
来源：http://hz.snrcjt.cn/gtzwrrjbmx.html

email VARCHAR(100) UNIQUE,
来源：http://hz.yongpay.top/gtdsrkwzhn.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.gogol.net.cn/gtuvahmxdb.html

);
来源：http://hz.redwolf501.top/gtjmyiowka.html

[Q02] 创建带外键的表
来源：http://hz.zycfv.cn/gttfpnyacf.html

CREATE TABLE orders (
来源：http://hz.sweek.top/gtpbamumah.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.tanke756.top/gtqaxjweox.html

user_id INT NOT NULL,
来源：http://hz.gzhubu.top/gtqbihyzug.html

amount DECIMAL(10, 2),
来源：http://hz.yuxming.cn/gtshmtsacl.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.chenjidiqi.icu/gteovoxrmt.html

);
来源：http://hz.nanxinkj.top/gtkxucriim.html

[Q03] 增加列
来源：http://hz.316326.xyz/gtivyndljn.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.cqqwz.cn/gtojlcfdrq.html

[Q04] 修改列类型
来源：http://hz.iojbl.cn/gtxhrdwknm.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.aibaodan.cn/gtffizgwzv.html

[Q05] 重命名列
来源：http://hz.zhiwuduotai.top/gtnxrluufa.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.xuetiantiany.cn/gtszeoykmu.html

[Q06] 删除列
来源：http://hz.yangfankeji.com/gthgwewsxx.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.guowangkeji.top/gttnbgekgd.html

[Q07] 删除表
来源：http://hz.yangfankeji.com/gtrzkgugiv.html

DROP TABLE IF EXISTS orders;
来源：http://hz.shanyushiyangkeji.top/gtowmvsjhk.html

[Q08] 创建普通索引
来源：http://hz.wangshuangyany.cn/gtjkmztvpt.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.316326.xyz/gtfrvpebcm.html

[Q09] 创建唯一索引
来源：http://hz.mhx1999.top/gtfesjndeh.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.sufxvd.cn/gtmqerwmlo.html

[Q10] 插入单行
来源：http://hz.c1oappe.top/gtuzsbcmze.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.ydzc1.top/gtrwzpmyya.html

[Q11] 一次插入多行
来源：http://hz.c1oappe.top/gtrmeuwrnf.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.nwbrower.top/gtbfgoigwl.html

[Q12] 插入后取自增 ID
来源：http://hz.ehwqpu.com/gticypdtju.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.smart0.xyz/gtbjegvxyc.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.gaohongyu789.top/gtunhmvcsz.html

[Q13] 忽略重复插入
来源：http://hz.tanke756.top/gtfkeibuvc.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.jinqigfzy.top/gtxetivwfq.html

[Q14] 存在则更新（upsert）
来源：http://hz.shanyushiyangkeji.top/gttgtdrjme.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.ivvv.top/gtsrgrwqsx.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.shanyushiyangtech.top/gtgtvquyhb.html

[Q15] 查询全部
来源：http://hz.cashguo.top/gtrzlkeeta.html

SELECT * FROM users;
来源：http://hz.kuanghao11.cn/gtfzqpween.html

[Q16] 查询指定列
来源：http://hz.svipenyu.cn/gtreicwukn.html

SELECT id, name FROM users;
来源：http://hz.hammf.cn/gtydvhjvog.html

[Q17] 条件查询
来源：http://hz.redwolf501.top/gtkmccdntf.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.pycfn.com/gtarhwxuce.html

[Q18] 模糊匹配
来源：http://hz.jqgufenzy.top/gtarlqtizy.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.kuanghao11.cn/gtchrjakpj.html

[Q19] 范围查询
来源：http://hz.zdqjudy.top/gtbopfhfvy.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.andypj.xyz/gtkrkiryvm.html

[Q20] IN 列表
来源：http://hz.yj20258888.top/gtpjoysqos.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.andypj.xyz/gtafmcszob.html

[Q21] 空值判断
来源：http://hz.tianlin.xyz/gtyqwlrawg.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.zhiwuduotai.top/gttrrosvac.html

[Q22] 排序
来源：http://hz.vqdsnc.cn/gtukbjyuzx.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.0kj1m.cn/gtyxgfmyaw.html

[Q23] 分页
来源：http://hz.pengpengdd.cyou/gtakxznkmh.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.andypj.xyz/gtjbfcvvva.html

[Q24] 去重
来源：http://hz.xylfe.cn/gtxshspawv.html

SELECT DISTINCT city FROM users;
来源：http://hz.sweek.top/gtjshinhvg.html

[Q25] 只取前 N 条
来源：http://hz.feifeiyinyue.top/gtcyocchco.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.mhx1999.top/gtoodsvdzx.html

[Q26] 计数
来源：http://hz.chenzaomai.com/gtvdwikyzc.html

SELECT COUNT(*) FROM users;
来源：http://hz.yongpay.top/gtunlxnwek.html

[Q27] 条件计数
来源：http://hz.daxiang520.top/gtnnzwfafb.html


<!-- 参考信息 -->