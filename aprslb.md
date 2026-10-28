代发 wailian999

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.xuetiantiany.cn/gtpmlqndfw.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.mhx1999.top/gtevkwuzfp.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.wangdashe.top/gtgttvlern.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.yuxming.cn/gtzyvbihjx.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.xuetiantiany.cn/gtnpwagumu.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.bjfxy.top/gtluyykgxc.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.zhixingplan.top/gtidrmamxh.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.hfpthk.cn/gtoxpamcnc.html

[N05] 最大公约数
来源：http://hz.quarkkingdee.top/gtkdqlqxwf.html

Py:   math.gcd(a, b)
来源：http://hz.jlsjyb.cn/gtnsrriddj.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.jinghuilouyu.cn/gtkwnbfhcg.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.andypj.xyz/gtguyfjhrz.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.zhoulong.xyz/gtbveukqdw.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.gogol.net.cn/gtuzkuvgiq.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.nanxinkj.top/gtvozzspts.html

Ruby: a.gcd(b)
来源：http://hz.yongpay.top/gtkmlbbxge.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.zhaomingkeji.xyz/gttzxrbwne.html

[N06] 判断回文字符串
来源：http://hz.shzxlz.cn/gtmhtkbrit.html

Py:   s == s[::-1]
来源：http://hz.mhx1999.top/gtxhobuquy.html

PHP:  $s === strrev($s);
来源：http://hz.nanxuanxn.top/gtnxzubkxz.html

JS:   s === [...s].reverse().join("")
来源：http://hz.vqdsnc.cn/gtkynhotub.html

TS:   s === [...s].reverse().join("")
来源：http://hz.haohaochexian.top/gtqnzcdgsw.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.zhaomingkeji.xyz/gtuxgwsklr.html

Go:   // 双指针从两端比较
来源：http://hz.jiagoushi.top/gtshyutpvy.html

Ruby: s == s.reverse
来源：http://hz.zhaomingkeji.xyz/gtkcodtwdt.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.nanxinkj.top/gtfsbxgknd.html

[N07] 两数之和（返回下标）
来源：http://hz.hammf.cn/gtzjpkpxyj.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.zhengqikj.top/gtyzecqrrt.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.shangyingyoupin.top/gtdiylvyxj.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.nanxinkj.top/gtojblkzdr.html

TS:   // 手写 Map<string, number>
来源：http://hz.c1oappe.top/gtvtxwfoei.html

Java: // 手写 HashMap
来源：http://hz.fzhhl.top/gtnjqwocdk.html

Go:   // 手写 map[int]int
来源：http://hz.yj20258888.top/gtxopxnhgf.html

Ruby: // 手写 Hash
来源：http://hz.tanke756.top/gttxyuknga.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.ywan-chungtsiang.top/gtffduauui.html

[N08] 生成全排列
来源：http://hz.ydzc1.top/gtdgrlbqxt.html

Py:   itertools.permutations(arr)
来源：http://hz.yueranfly.top/gtxgmuhmtk.html

PHP:  // 手写递归交换
来源：http://hz.shangyingyoupin.top/gtrrrdlahk.html

JS:   // 手写回溯递归
来源：http://hz.c1oappe.top/gtmpjxegdp.html

TS:   // 手写回溯递归
来源：http://hz.nanxinkj.top/gttzrwxndm.html

Java: // 手写回溯递归
来源：http://hz.iojbl.cn/gtpwadvgon.html

Go:   // 手写回溯递归
来源：http://hz.aibaodan.cn/gtyheykntp.html

Ruby: arr.permutation.to_a
来源：http://hz.tianlin.xyz/gtfcpxkgot.html

C#:   // 手写回溯递归
来源：http://hz.guowangkeji.top/gtyyybndbe.html

[N09] 栈与队列
来源：http://hz.gzhubu.top/gtubiwzwie.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.zhaomingkeji.xyz/gtsolylbbc.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.nanxinkj.top/gtoaujycdb.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.cheryme.top/gtsnhbueed.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.daxiang520.top/gtsdfypqor.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.chenzaomai.com/gtpvcvxqlm.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.zhixingplan.top/gtjhraoeqn.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.9152youxi.cn/gtbdioshnz.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.zhiwuduotai.top/gtfobykxwa.html

[N10] 链表节点定义
来源：http://hz.meibo888.top/gtsoumstig.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.gzhubu.top/gtywzbihhv.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.shuidangran.top/gtvsbjqook.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.hysaishi.cn/gtsznoyoae.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.xziqi.cn/gtvazbdsin.html

Java: class Node { int v; Node next; }
来源：http://hz.feifeiyinyue.top/gtaydhtfol.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.cqqwz.cn/gtxyoayrry.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.jlsjyb.cn/gtxzmvtobe.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.yueranfly.top/gterugvhpa.html

[N11] 二叉树中序遍历
来源：http://hz.yangfankeji.com/gtaooyunsn.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.andypj.xyz/gtkzugwqkx.html

PHP:  // 手写递归函数
来源：http://hz.hnqzz.top/gtwcsocgum.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.sufxvd.cn/gtlcznwusu.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.meibo888.top/gtzkybbxev.html

Java: // 手写递归
来源：http://hz.gogol.net.cn/gtihzozkil.html

Go:   // 手写递归
来源：http://hz.tian-w.cn/gtlbtwvtkb.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.shzxlz.cn/gthxtelwej.html

C#:   // 手写递归
来源：http://hz.ywan-chungtsiang.top/gtjjprmikp.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.hnqzz.top/gtxqdbnbwt.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.cdnleiting.top/gtlcyeefdt.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.ywan-chungtsiang.top/gtqztxivrp.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.feifeiyinyue.top/gtzrdfgapd.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.zhoulong.xyz/gthnhrjelv.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.cheryme.top/gttxxpykxf.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.nwbrower.top/gtlitnscfl.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.redwolf501.top/gtkmrchcrj.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.bjfxy.top/gttquvruul.html

================================================================================
来源：http://hz.guowangkeji.top/gtfmoslksi.html

O. 并发与异步
来源：http://hz.9152youxi.cn/gtedhjwfkb.html

================================================================================
来源：http://hz.jlsjyb.cn/gtszncaqil.html

[O01] 启动一个线程
来源：http://hz.gzhubu.top/gtekyiabvh.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.hysaishi.cn/gtmgerhyoo.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.jinyuanbaomall.cn/gtcpazxzrz.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.snrcjt.cn/gtrvcsmoiv.html

TS:   // 同 JS
来源：http://hz.zhengqikj.top/gteawhksft.html

Java: new Thread(() -> f()).start()
来源：http://hz.hysaishi.cn/gtccrwqbbj.html

Go:   go f()
来源：http://hz.9152youxi.cn/gttngdeviw.html

Ruby: Thread.new { f }
来源：http://hz.yj20258.top/gtyasmpnsn.html

C#:   Task.Run(() => F());
来源：http://hz.chenzaomai.com/gtpmfeipla.html

[O02] 使用线程池
来源：http://hz.yonumen.top/gtfroatbwv.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.shanyushiyangtech.top/gtirvmmfam.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.xingfuxueyuan.xyz/gtauheflsc.html

JS:   // worker_threads 线程池
来源：http://hz.jqgufenzy.top/gtuwfrkhce.html

TS:   // worker_threads 线程池
来源：http://hz.yongpay.top/gtbkulgjwl.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.chenjidiqi.icu/gtpelbisic.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.birdmap.top/gtmtpvpyrr.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.jinqigufen.top/gtjuejhuwl.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.52xcode.cn/gtufsrhvps.html

[O03] 加锁保护共享数据
来源：http://hz.meibo888.top/gtguiuvmpi.html

Py:   with lock: shared += 1
来源：http://hz.snrcjt.cn/gtzkihagab.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.haohaochexian.top/gtmkhdnkud.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.yvedp.cn/gtpgijjtja.html

TS:   // 同 JS
来源：http://hz.xinyue.icu/gtgfgdhatq.html

Java: synchronized (this) { shared++; }
来源：http://hz.cucudq.cn/gtmmhseruj.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.c1oappe.top/gthvxjrtrc.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.guannengcc.top/gtnngdmenh.html

C#:   lock (gate) { shared++; }
来源：http://hz.yongpay.top/gtdnmieegf.html

[O04] 定义异步函数并等待
来源：http://hz.ivvv.top/gtdsfwtbvm.html

Py:   async def f():⏎    await g()
来源：http://hz.vqdsnc.cn/gtegvjthdg.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.guannengcc.top/gtpeiqkwzj.html

JS:   async function f() { await g(); }
来源：http://hz.0kj1m.cn/gtyseahbsn.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.yvedp.cn/gtoddvssyr.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.zhixingplan.top/gtldrifxfw.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.xziqi.cn/gtanruidbf.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.yonumen.top/gtdsxizmii.html

C#:   async Task F() { await G(); }
来源：http://hz.ydjk.org.cn/gtoljzcdbo.html

[O05] 并发执行并等待全部完成
来源：http://hz.shuidangran.top/gtkftygklk.html

Py:   asyncio.gather(*tasks)
来源：http://hz.hammf.cn/gtnaaimnbp.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.shangyingyoupin.top/gtulydnaog.html

JS:   await Promise.all(tasks)
来源：http://hz.hongshengwenyu.top/gtidojoffm.html

TS:   await Promise.all(tasks)
来源：http://hz.yj20258888.top/gtykbsjalu.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.hfpthk.cn/gtygbplaog.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.dianchejie.cn/gtxxfgzaoq.html

Ruby: threads.map(&:join)
来源：http://hz.mhx1999.top/gtapaufhmb.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.wangdashe.top/gtnzmuyyfl.html

[O06] 使用进程池
来源：http://hz.daxiang520.top/gtmqnunqvl.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.jqgufenzy.top/gtvhvpxbsl.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.cqqwz.cn/gtryruuyrj.html

JS:   // child_process / cluster 模块
来源：http://hz.yangfankeji.com/gtexbwwmru.html

TS:   // child_process / cluster 模块
来源：http://hz.sysykeji.top/gtawmhnavm.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.hywenlv.cn/gtcpddfjzv.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.haohaochexian.top/gtwwmcdtzg.html

Ruby: // fork 块
来源：http://hz.aibaodan.cn/gtxuqwcafs.html

C#:   Parallel.For
来源：http://hz.chenlongwang.top/gtcwyflifr.html

================================================================================
来源：http://hz.yuxming.cn/gttnbinpbb.html

P. 常用工具函数
来源：http://hz.zdqjudy.top/gtbxrzyoyb.html

================================================================================
来源：http://hz.daria6918.cn/gtrnhqfizt.html

[P01] 生成 UUID
来源：http://hz.jinqigufen.top/gtaddbezdm.html

Py:   str(uuid.uuid4())
来源：http://hz.redwolf501.top/gtovmngxrt.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.cheryme.top/gtdqufhtbn.html

JS:   crypto.randomUUID()
来源：http://hz.sufxvd.cn/gtmezvojsz.html

TS:   crypto.randomUUID()
来源：http://hz.jqgfzy.top/gtxyjsjgbc.html

Java: UUID.randomUUID().toString()
来源：http://hz.yanxiufei.cn/gtnqkdribq.html

Go:   // 用 github.com/google/uuid
来源：http://hz.redwolf501.top/gtvfetsrut.html

Ruby: SecureRandom.uuid
来源：http://hz.nwbrower.top/gtbxcuruep.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.shuidangran.top/gtcpkcdoeq.html

[P02] MD5 / SHA256 摘要
来源：http://hz.zhiwuduotai.top/gtncrzegwp.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.ywan-chungtsiang.top/gttofsnisz.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.sufxvd.cn/gthkntlyzl.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.hongshengwenyu.top/gtncaaifwj.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.0kj1m.cn/gtfvczxywt.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.yonumen.top/gtpmjodjhb.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.jinyuanbaomall.cn/gtoxtwshwk.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.yonumen.top/gtxnvonlfp.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.zhijiandao.cn/gtyzwmeexy.html

[P03] 生成短随机字符串
来源：http://hz.xuanzx.com/gtviumwzar.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.cashguo.top/gtanwjklln.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.jqgfzy.top/gthprjorla.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.mhx1999.top/gtkaovgvgr.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.feifeiyinyue.top/gtczxvyajp.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.hongshengwenyu.top/gthzymwkpq.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.c1oappe.top/gtzctduafe.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.xinyue.icu/gtbyolwkdb.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.vqdsnc.cn/gtjfecyimw.html

[P04] 求长度
来源：http://hz.zdqjudy.top/gtbhbpnecm.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.shangyingyoupin.top/gtwfibdyxj.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.svipenyu.cn/gtvydhrulp.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.ywan-chungtsiang.top/gtzvbujtiw.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.hnxiangtu.top/gtuttsbcfx.html

Java: list.size();  map.size();  s.length()
来源：http://hz.gotoacloud.top/gthaisbrps.html

Go:   len(arr);  len(m)
来源：http://hz.vqdsnc.cn/gtgbjagkaf.html

Ruby: x.length;  x.size
来源：http://hz.c1oappe.top/gtsetrznvs.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.sufxvd.cn/gtrbbfqdca.html

[P05] 判断两个对象内容是否相等
来源：http://hz.dianchejie.cn/gtvvkqvxol.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.sweek.top/gtoimxbzlk.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.sweek.top/gtneoirggx.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.meibo888.top/gtjyvaopbt.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.dashuyun.cn/gtvtifeane.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.pengpengdd.cyou/gtzfblfvxj.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.shzxlz.cn/gtgaouygna.html

Ruby: a == b
来源：http://hz.tianlin.xyz/gtbcuyuvju.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.jqgufenzy.top/gtvaojtzid.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.daxiang520.top/gtoznvvxmf.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.9152youxi.cn/gtpzsribod.html

PHP:  if (empty($x)) {}
来源：http://hz.shanyushiyangtech.top/gthsxcjhue.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.sxryk.cn/gtxrkooafx.html

TS:   if (x == null) {}
来源：http://hz.meibo888.top/gtyqttqcok.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.zhiwuduotai.top/gtcznsmraq.html

Go:   if x == nil {}
来源：http://hz.yvedp.cn/gtombrcbyv.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.yangfankeji.com/gtzbyopsoo.html

C#:   if (x is null) {}
来源：http://hz.vqdsnc.cn/gtdyrcurhe.html

[P07] 防抖与节流
来源：http://hz.dashuyun.cn/gtqtthbecb.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.redwolf501.top/gthfjnvbvn.html

PHP:  // 手写时间戳比较
来源：http://hz.zdqjudy.top/gtptyvdqyx.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.aizwys.cn/gtksxmtudq.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.jinqigfzy.top/gtwialhdgu.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.316326.xyz/gtegvyupse.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.jinghuilouyu.cn/gtfcxzsths.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.hysaishi.cn/gtgtfjfncb.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.tanke756.top/gthmojoqhk.html

[P08] 处理浮点精度问题
来源：http://hz.zhongyouzk.top/gtfczzwjvb.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.52xcode.cn/gtuzfmrbio.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.cheryme.top/gtfvhxzdek.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.gaohongyu789.top/gtwarvghjb.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.sxryk.cn/gteygzwbra.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.jinqigufen.top/gtlhqbptms.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.quarkkingdee.top/gtywwlrcsr.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.yj20258.top/gtixzfntat.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.wangshuangyany.cn/gtcpezgudt.html

================================================================================
来源：http://hz.tian-w.cn/gtijxjswnr.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.chenjidiqi.icu/gtbakzdjoo.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gtgdwfccyp.html

[Q01] 创建表
来源：http://hz.jinyuanbaomall.cn/gtxiwifzsl.html

CREATE TABLE users (
来源：http://hz.316326.xyz/gtlawzglhq.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.smart0.xyz/gtuqjqvjhd.html

name VARCHAR(50) NOT NULL,
来源：http://hz.zhoulong.xyz/gtfyudgepc.html

email VARCHAR(100) UNIQUE,
来源：http://hz.sufxvd.cn/gtmbqwpepu.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.pengpengdd.cyou/gtifuwekcl.html

);
来源：http://hz.ydzc1.top/gtgfsdlckl.html

[Q02] 创建带外键的表
来源：http://hz.havefunace.top/gtiqactnjk.html

CREATE TABLE orders (
来源：http://hz.jqgufenzy.top/gtutajgemh.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.feifeiyinyue.top/gtjaxzvosd.html

user_id INT NOT NULL,
来源：http://hz.ywan-chungtsiang.top/gtqesblaux.html

amount DECIMAL(10, 2),
来源：http://hz.jinqigufen.top/gtpcqbyyvf.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.zhiwuduotai.top/gtnwzqqfar.html

);
来源：http://hz.xingfuxueyuan.xyz/gtasmlwnnp.html

[Q03] 增加列
来源：http://hz.xuetiantiany.cn/gtfdajgqtk.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.shanyushiyangkeji.top/gtbuodjodl.html

[Q04] 修改列类型
来源：http://hz.cdnleiting.top/gtbtcyjkuz.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.guannengcc.top/gthvquvqzt.html

[Q05] 重命名列
来源：http://hz.guannengcc.top/gtaxjdmemv.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.yongpay.top/gtcfoyxcnw.html

[Q06] 删除列
来源：http://hz.hywenlv.cn/gtbnbfjgth.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.meibo888.top/gtcyztegsj.html

[Q07] 删除表
来源：http://hz.mhx1999.top/gtpkfpwcaa.html

DROP TABLE IF EXISTS orders;
来源：http://hz.hammf.cn/gtgqwdtorj.html

[Q08] 创建普通索引
来源：http://hz.daxiang520.top/gtbrfxqqdk.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.9152youxi.cn/gtsrszvcxr.html

[Q09] 创建唯一索引
来源：http://hz.ydjk.org.cn/gtgqrrkyyw.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.ydzc1.top/gtleupqubo.html

[Q10] 插入单行
来源：http://hz.c1oappe.top/gtpfoyisfb.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.gzhubu.top/gtwuqdvbgo.html

[Q11] 一次插入多行
来源：http://hz.ivvv.top/gtivaivwap.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.xingfuxueyuan.xyz/gtmhpkyycn.html

[Q12] 插入后取自增 ID
来源：http://hz.guowangkeji.top/gtleevibrh.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.sufxvd.cn/gtueuboktr.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.feifeiyinyue.top/gtdesweahf.html

[Q13] 忽略重复插入
来源：http://hz.9152youxi.cn/gtcshhwnfw.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.chenjidiqi.icu/gtzvsstwgz.html

[Q14] 存在则更新（upsert）
来源：http://hz.kuanghao11.cn/gtzyhufmhc.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.wangshuangyany.cn/gtqxagquap.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.pengpengdd.cyou/gttsqmuzxe.html

[Q15] 查询全部
来源：http://hz.cheryme.top/gttzjgselh.html

SELECT * FROM users;
来源：http://hz.jianghu66.top/gtgyqnvwiy.html

[Q16] 查询指定列
来源：http://hz.tanke756.top/gtpildnaue.html

SELECT id, name FROM users;
来源：http://hz.xuanzx.com/gtqljzflau.html

[Q17] 条件查询
来源：http://hz.jiagoushi.top/gtpcechwkd.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.cdnleiting.top/gtylsbjsgd.html

[Q18] 模糊匹配
来源：http://hz.mhx1999.top/gtsysnhekq.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.hnqzz.top/gtgxubfdim.html

[Q19] 范围查询
来源：http://hz.fengsongda.top/gtypmcsegb.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.ydzc1.top/gtxxrasmho.html

[Q20] IN 列表
来源：http://hz.yonumen.top/gtgketvsgz.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.shangyingyoupin.top/gtilooqrgi.html

[Q21] 空值判断
来源：http://hz.shangyingyoupin.top/gtackqkgii.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.cqqwz.cn/gtwiwkjubw.html

[Q22] 排序
来源：http://hz.xziqi.cn/gtnwzsbmjr.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.nanxuanxn.top/gtslubcsce.html

[Q23] 分页
来源：http://hz.zycfv.cn/gtnhmwqbso.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.quarkkingdee.top/gtzmvtockw.html

[Q24] 去重
来源：http://hz.52xcode.cn/gtgyuprfme.html

SELECT DISTINCT city FROM users;
来源：http://hz.jiagoushi.top/gtjjnuyhek.html

[Q25] 只取前 N 条
来源：http://hz.ydjk.org.cn/gthkmkyfcr.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.xziqi.cn/gtanxkacrc.html

[Q26] 计数
来源：http://hz.guannengcc.top/gtytocxrku.html

SELECT COUNT(*) FROM users;
来源：http://hz.xziqi.cn/gtmwgsekbs.html

[Q27] 条件计数
来源：http://hz.jinghuilouyu.cn/gtafvmmkfk.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.chenjidiqi.icu/gtzidstfes.html

[Q28] 求和与平均
来源：http://hz.smart0.xyz/gtqugmagar.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.shanyushiyangtech.top/gttrbaurts.html

[Q29] 最大最小值
来源：http://hz.yongpay.top/gtojlhoapx.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.redwolf501.top/gtfzeeuhpp.html

[Q30] 分组统计
来源：http://hz.nanxinkj.top/gtdmjzgiox.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.yj202588.top/gttviadjrd.html

[Q31] 分组后过滤
来源：http://hz.feifeiyinyue.top/gtuzhximmd.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.daxiang520.top/gteduigwze.html

[Q32] 分组拼接字符串
来源：http://hz.hnqzz.top/gtglsalfcs.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.gotoacloud.top/gtygbzsijy.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.havefunace.top/gttojagkwl.html

[Q33] 多列分组
来源：http://hz.gogol.net.cn/gtwulkuqoc.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.sweek.top/gtsnijonxi.html

[Q34] 每组取第一条
来源：http://hz.xuetiantiany.cn/gtjldmdxve.html

SELECT * FROM (
来源：http://hz.zycfv.cn/gtpnbcnirf.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.daria6918.cn/gtukczrdck.html

) t WHERE rn = 1;
来源：http://hz.sysykeji.top/gtotiqgjog.html

[Q35] 内连接
来源：http://hz.sxryk.cn/gtporbdiyd.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.zhengqikj.top/gtdsielzjy.html


<!-- 参考信息 -->