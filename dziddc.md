代发 wailian999

C#:   Array.BinarySearch(arr, x)
来源：http://hz.jiagoushi.top/gtbwnypdfg.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.jinyuanbaomall.cn/gtqyvodhwi.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.dashuyun.cn/gtinaqaugv.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.quarkkingdee.top/gtkdrtawcc.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.cdnleiting.top/gtznmxkmgf.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.yanxiufei.cn/gttxybnzok.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.316326.xyz/gtztzmykpx.html

Go:   slices.Sort(arr)
来源：http://hz.nwbrower.top/gtytwdqagf.html

Ruby: arr.sort
来源：http://hz.shuidangran.top/gtemggicgm.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.ivvv.top/gtmkblsidq.html

[N03] 快速排序（分治示例）
来源：http://hz.jianghu66.top/gtlesyrpzv.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.ydzc1.top/gtjuipkwep.html

PHP:  // 递归实现，或用 usort
来源：http://hz.cucudq.cn/gtijchtnid.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.ydzc1.top/gtmvikqxdu.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.yj20258.top/gtzcazcwtv.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.jinqigufen.top/gtsarkenee.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.jianghu66.top/gtvhwbtpje.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.yj20258.top/gtnvgqkjnk.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.sysykeji.top/gtfgrmbfob.html

[N04] 斐波那契数列
来源：http://hz.shanyushiyangkeji.top/gtjhaikkgp.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.hnqzz.top/gtejitpbgt.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.haohaochexian.top/gtbnlmcsdj.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.zdqjudy.top/gtrhbiekww.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.zhijiandao.cn/gtdnczuwbr.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.cashguo.top/gtpesbcccp.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.hywenlv.cn/gtnglrmknd.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.zhaomingkeji.xyz/gtktevqdjs.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.yanxiufei.cn/gtyuqfyiuc.html

[N05] 最大公约数
来源：http://hz.havefunace.top/gtlsryoyva.html

Py:   math.gcd(a, b)
来源：http://hz.zhaomingkeji.xyz/gtswxxnwkx.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.andypj.xyz/gtyohduoma.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.316326.xyz/gtnbbsovyr.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.0kj1m.cn/gtxdbsqptc.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.guowangkeji.top/gtgkjavsnp.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.xylfe.cn/gtdjaawsce.html

Ruby: a.gcd(b)
来源：http://hz.yj202588.top/gtjhihhdld.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.zdqjudy.top/gtnutetkip.html

[N06] 判断回文字符串
来源：http://hz.cdnleiting.top/gtndpwtotw.html

Py:   s == s[::-1]
来源：http://hz.ivvv.top/gtgyrykref.html

PHP:  $s === strrev($s);
来源：http://hz.fzhhl.top/gtdlqdtolo.html

JS:   s === [...s].reverse().join("")
来源：http://hz.zhongyouzk.top/gtitqyfkww.html

TS:   s === [...s].reverse().join("")
来源：http://hz.fzhhl.top/gtjejizcrz.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.jinqigfzy.top/gtwimnmyxf.html

Go:   // 双指针从两端比较
来源：http://hz.sweek.top/gtawneurxe.html

Ruby: s == s.reverse
来源：http://hz.guowangkeji.top/gtblxzhuvf.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.hnqzz.top/gtdrnrmdru.html

[N07] 两数之和（返回下标）
来源：http://hz.cqqwz.cn/gtcoosntfc.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.nanxinkj.top/gtfgehmfej.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.smart0.xyz/gtzyvcnxny.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.daria6918.cn/gthodjrozn.html

TS:   // 手写 Map<string, number>
来源：http://hz.guannengcc.top/gtobxbeyfj.html

Java: // 手写 HashMap
来源：http://hz.sysykeji.top/gtpamxfzmz.html

Go:   // 手写 map[int]int
来源：http://hz.jiagoushi.top/gterhwoalk.html

Ruby: // 手写 Hash
来源：http://hz.jinqigfzy.top/gtshqxuofe.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.hammf.cn/gtgakbtagc.html

[N08] 生成全排列
来源：http://hz.daria6918.cn/gtffajlasq.html

Py:   itertools.permutations(arr)
来源：http://hz.jlsjyb.cn/gtyplmpswa.html

PHP:  // 手写递归交换
来源：http://hz.jinqigufen.top/gtjywxvrlj.html

JS:   // 手写回溯递归
来源：http://hz.shuidangran.top/gtnbzpzlqu.html

TS:   // 手写回溯递归
来源：http://hz.jinqigufen.top/gtcxrvasid.html

Java: // 手写回溯递归
来源：http://hz.yangfankeji.com/gtnvhwpqdy.html

Go:   // 手写回溯递归
来源：http://hz.meibo888.top/gtvlqbmbkv.html

Ruby: arr.permutation.to_a
来源：http://hz.jinqigufen.top/gtvnplguuw.html

C#:   // 手写回溯递归
来源：http://hz.chenzaomai.com/gtpqatdphd.html

[N09] 栈与队列
来源：http://hz.0kj1m.cn/gtsougkzom.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.meibo888.top/gtonqtgade.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.ywan-chungtsiang.top/gtdjczfkne.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.ydzc1.top/gtfkdcwgot.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.jinyuanbaomall.cn/gtmuvrzytv.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.zhixingplan.top/gtaqkmyxhw.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.gogol.net.cn/gtgdfglxjm.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.yangfankeji.com/gtijqlvvcr.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.ydjk.org.cn/gtaaucnybi.html

[N10] 链表节点定义
来源：http://hz.hnxiangtu.top/gtoxbnxhka.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.hywenlv.cn/gtwlqlvuuz.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.cashguo.top/gtziafsqxu.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.shzxlz.cn/gtiactcntw.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.mhx1999.top/gtlmhwaiqx.html

Java: class Node { int v; Node next; }
来源：http://hz.jlsjyb.cn/gtgqhwuojt.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.316326.xyz/gtbskardlv.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.cdnleiting.top/gtouwzouvg.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.xinyue.icu/gttwfaqymw.html

[N11] 二叉树中序遍历
来源：http://hz.tanke756.top/gtaglwusqn.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.hywenlv.cn/gtkewqtadn.html

PHP:  // 手写递归函数
来源：http://hz.xylfe.cn/gtetogyoec.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.316326.xyz/gtirxaonzw.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.pycfn.com/gthjwftxwy.html

Java: // 手写递归
来源：http://hz.sufxvd.cn/gtdsqatted.html

Go:   // 手写递归
来源：http://hz.hfpthk.cn/gteztljdel.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.vqdsnc.cn/gtcbxraqmn.html

C#:   // 手写递归
来源：http://hz.jqgfzy.top/gtreljdznc.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.zhongyouzk.top/gteytepnfh.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.shanyushiyangtech.top/gtwcwqmhjm.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.vqdsnc.cn/gtkltuvvxd.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.ydjk.org.cn/gtpxkuatxd.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.jinghuilouyu.cn/gtrwcpqncy.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.gzhubu.top/gthilykugm.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.jyoumei.cn/gtucbjbmed.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.cqqwz.cn/gtfwpfirgq.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.chenlongwang.top/gtimntiozd.html

================================================================================
来源：http://hz.cucudq.cn/gtvcrtzmwi.html

O. 并发与异步
来源：http://hz.xuanzx.com/gtssatmlxi.html

================================================================================
来源：http://hz.ydjk.org.cn/gtxkogfxyi.html

[O01] 启动一个线程
来源：http://hz.fengsongda.top/gtbxdreksq.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.aibaodan.cn/gttcofsfmd.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.quarkkingdee.top/gthfkureyb.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.redwolf501.top/gtpfcopvhl.html

TS:   // 同 JS
来源：http://hz.jinyuanbaomall.cn/gtduxqhulo.html

Java: new Thread(() -> f()).start()
来源：http://hz.fzhhl.top/gtrzmrvstr.html

Go:   go f()
来源：http://hz.snrcjt.cn/gtepfabqkv.html

Ruby: Thread.new { f }
来源：http://hz.gogol.net.cn/gtbzxlsmnj.html

C#:   Task.Run(() => F());
来源：http://hz.hfpthk.cn/gtbkqylrsh.html

[O02] 使用线程池
来源：http://hz.316326.xyz/gtzwiqshws.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.yuxming.cn/gtwvgmxxig.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.sysykeji.top/gtqnuhsfvq.html

JS:   // worker_threads 线程池
来源：http://hz.daxiang520.top/gtxgbjsize.html

TS:   // worker_threads 线程池
来源：http://hz.zdqjudy.top/gtsuqjrfqk.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.pengpengdd.cyou/gtkhjcakcc.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.zhoulong.xyz/gtlcqfnmzr.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.yonumen.top/gtxyoulwaw.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.daria6918.cn/gtuqfqrutz.html

[O03] 加锁保护共享数据
来源：http://hz.aibaodan.cn/gtojfpehcb.html

Py:   with lock: shared += 1
来源：http://hz.yueranfly.top/gtlukdujrz.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.9152youxi.cn/gtildifnyk.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.jianghu66.top/gtdqyhdyda.html

TS:   // 同 JS
来源：http://hz.andypj.xyz/gtwtjwnxoe.html

Java: synchronized (this) { shared++; }
来源：http://hz.wangdashe.top/gteuinmlhu.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.sufxvd.cn/gtdjsiovhk.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.cdnleiting.top/gtiptscwne.html

C#:   lock (gate) { shared++; }
来源：http://hz.ivvv.top/gtqkwfpczw.html

[O04] 定义异步函数并等待
来源：http://hz.kuanghao11.cn/gtptqxnqsw.html

Py:   async def f():⏎    await g()
来源：http://hz.hywenlv.cn/gtuxqjqmci.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.yj202588.top/gtgwpgpfeu.html

JS:   async function f() { await g(); }
来源：http://hz.zhengqikj.top/gthvnckncp.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.guowangkeji.top/gteamhnhap.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.cucudq.cn/gtgeaqqmkq.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.xingfuxueyuan.xyz/gtllhmdulb.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.nanxuanxn.top/gtqehetofv.html

C#:   async Task F() { await G(); }
来源：http://hz.mhx1999.top/gtunooeuek.html

[O05] 并发执行并等待全部完成
来源：http://hz.cdnleiting.top/gtxkfikrkz.html

Py:   asyncio.gather(*tasks)
来源：http://hz.daxiang520.top/gtwdaqqkpj.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.yuxming.cn/gtwmlncetx.html

JS:   await Promise.all(tasks)
来源：http://hz.havefunace.top/gtuypdwnxm.html

TS:   await Promise.all(tasks)
来源：http://hz.dashuyun.cn/gtnhzsxjyf.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.jinqigufen.top/gtrybinuyd.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.dashuyun.cn/gtcrwtypfn.html

Ruby: threads.map(&:join)
来源：http://hz.yuxming.cn/gtgsguflhk.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.birdmap.top/gtpopjibhg.html

[O06] 使用进程池
来源：http://hz.redwolf501.top/gtuififedb.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.gzhubu.top/gtkmhuqvlc.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.nanxuanxn.top/gtkfmpetrw.html

JS:   // child_process / cluster 模块
来源：http://hz.chenjidiqi.icu/gtskxsvrrq.html

TS:   // child_process / cluster 模块
来源：http://hz.0kj1m.cn/gtbfjfmmca.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.redwolf501.top/gtypgefonq.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.yangfankeji.com/gtuyfmamot.html

Ruby: // fork 块
来源：http://hz.jianghu66.top/gtvgzxhiep.html

C#:   Parallel.For
来源：http://hz.gogol.net.cn/gtsrcckmbg.html

================================================================================
来源：http://hz.hysaishi.cn/gtasgfwruz.html

P. 常用工具函数
来源：http://hz.fengsongda.top/gtiqmbapur.html

================================================================================
来源：http://hz.daxiang520.top/gtfapuzyqb.html

[P01] 生成 UUID
来源：http://hz.tianlin.xyz/gtkrfplyks.html

Py:   str(uuid.uuid4())
来源：http://hz.chenzaomai.com/gtjttxjdjj.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.316326.xyz/gtqtjwxfwy.html

JS:   crypto.randomUUID()
来源：http://hz.gaohongyu789.top/gtneouwple.html

TS:   crypto.randomUUID()
来源：http://hz.chenzaomai.com/gtbvodadrg.html

Java: UUID.randomUUID().toString()
来源：http://hz.zhixingplan.top/gtldtqoyhf.html

Go:   // 用 github.com/google/uuid
来源：http://hz.hammf.cn/gtibhaziig.html

Ruby: SecureRandom.uuid
来源：http://hz.cucudq.cn/gthxzenhds.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.quarkkingdee.top/gtnsbicqgz.html

[P02] MD5 / SHA256 摘要
来源：http://hz.tianlin.xyz/gtytxvrayl.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.gaohongyu789.top/gtqdpmkqls.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.cdnleiting.top/gtbhbvcpum.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.daxiang520.top/gtsonszrks.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.nanxinkj.top/gtggcxzlrt.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.havefunace.top/gtjebwomcg.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.jlsjyb.cn/gtembenppz.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.hnxiangtu.top/gtesszsqfz.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.cashguo.top/gtibftgcds.html

[P03] 生成短随机字符串
来源：http://hz.sweek.top/gtoemzfgdj.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.c1oappe.top/gtdptqhque.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.meibo888.top/gtalenjkdu.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.meibo888.top/gtkyiyuhzu.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.dianchejie.cn/gtyiejzcgo.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.nanxinkj.top/gtwfexurnf.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.fzhhl.top/gtyhjnxces.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.sufxvd.cn/gtutmtktye.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.pycfn.com/gtpshsqigr.html

[P04] 求长度
来源：http://hz.ydzc1.top/gtfhzjfped.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.yongpay.top/gtqnmlumld.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.aizwys.cn/gtuafurczz.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.zycfv.cn/gtztajqsbj.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.meibo888.top/gtexbdggfb.html

Java: list.size();  map.size();  s.length()
来源：http://hz.jlsjyb.cn/gtfeooaldd.html

Go:   len(arr);  len(m)
来源：http://hz.yuanzhike.top/gtacuhxgcj.html

Ruby: x.length;  x.size
来源：http://hz.fzhhl.top/gthebfqple.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.ivvv.top/gtgoatycdz.html

[P05] 判断两个对象内容是否相等
来源：http://hz.316326.xyz/gthfayfypg.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.shzxlz.cn/gtoyaqepux.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.ivvv.top/gtujmkjhwv.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.dianchejie.cn/gtlygzrnkb.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.cucudq.cn/gtydsuxkim.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.gaohongyu789.top/gtaitqhkev.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.aizwys.cn/gtgnvislxg.html

Ruby: a == b
来源：http://hz.tanke756.top/gtxfrulfkx.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.daria6918.cn/gtdgkuexfz.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.jinyuanbaomall.cn/gtntakftgo.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.hammf.cn/gtpvezqvyi.html

PHP:  if (empty($x)) {}
来源：http://hz.jinqigufen.top/gtwrxddnom.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.shangyingyoupin.top/gtvrpczwjy.html

TS:   if (x == null) {}
来源：http://hz.52xcode.cn/gtypvxryzs.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.wangdashe.top/gtuzhnmhrj.html

Go:   if x == nil {}
来源：http://hz.gogol.net.cn/gtaxcgdybi.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.jqgufenzy.top/gtbwsbnzvg.html

C#:   if (x is null) {}
来源：http://hz.chenlongwang.top/gtbydggmsp.html

[P07] 防抖与节流
来源：http://hz.fzhhl.top/gtssokhrxl.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.cheryme.top/gtiuksjjmk.html

PHP:  // 手写时间戳比较
来源：http://hz.zhengqikj.top/gtqycayqrc.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.bjfxy.top/gtnntufzwl.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.sufxvd.cn/gtauqnahfl.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.hongshengwenyu.top/gtdgjtkgde.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.aizwys.cn/gthhifhful.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.xingfuxueyuan.xyz/gtpexbdotg.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.ppjwa.cn/gtlnvabxey.html

[P08] 处理浮点精度问题
来源：http://hz.chenzaomai.com/gtynlukfwz.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.cdnleiting.top/gtbdjxoact.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.pycfn.com/gtpgozyqrm.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.kuanghao11.cn/gtlncybuns.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.xziqi.cn/gtjnarqcfy.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.meibo888.top/gtqdzbghcw.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.9152youxi.cn/gtpoypnyqq.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.xingfuxueyuan.xyz/gtdvpjcmdc.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.hongshengwenyu.top/gtgezpvmrp.html

================================================================================
来源：http://hz.9152youxi.cn/gtwdkttwld.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.jinqigufen.top/gtprwgtctv.html

================================================================================
来源：http://hz.9152youxi.cn/gtoiyurwvz.html

[Q01] 创建表
来源：http://hz.andypj.xyz/gtonwpnadg.html

CREATE TABLE users (
来源：http://hz.jinqigfzy.top/gtydtqocfu.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.xuetiantiany.cn/gtrkqsnfsd.html

name VARCHAR(50) NOT NULL,
来源：http://hz.vqdsnc.cn/gtaiyumgpu.html

email VARCHAR(100) UNIQUE,
来源：http://hz.gogol.net.cn/gtcujpgmpk.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.hywenlv.cn/gtzomqsghx.html

);
来源：http://hz.0kj1m.cn/gtydfaiuah.html

[Q02] 创建带外键的表
来源：http://hz.jinqigfzy.top/gtbhfuphej.html

CREATE TABLE orders (
来源：http://hz.hammf.cn/gtocnqwojy.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.ydzc1.top/gtngyqetmx.html

user_id INT NOT NULL,
来源：http://hz.shangyingyoupin.top/gtxxfywypp.html

amount DECIMAL(10, 2),
来源：http://hz.shuidangran.top/gtlendgjhk.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.jinqigufen.top/gttfzdsnbq.html

);
来源：http://hz.yj20258.top/gtimujdpmk.html

[Q03] 增加列
来源：http://hz.dashuyun.cn/gtoeotxsxw.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.tanke756.top/gtkknqaoxr.html

[Q04] 修改列类型
来源：http://hz.fengsongda.top/gtvygkmpks.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.yuxming.cn/gtorfcrott.html

[Q05] 重命名列
来源：http://hz.ybcxt.top/gtrunrtrhp.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.ppjwa.cn/gtlxxfdqpf.html

[Q06] 删除列
来源：http://hz.jinqigufen.top/gtrjteuoed.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.kuanghao11.cn/gtemglltes.html

[Q07] 删除表
来源：http://hz.xuetiantiany.cn/gtdukyussz.html

DROP TABLE IF EXISTS orders;
来源：http://hz.cqqwz.cn/gtkeerieur.html

[Q08] 创建普通索引
来源：http://hz.jianghu66.top/gtqyrvekjj.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.jinyuanbaomall.cn/gtnbdtqtgb.html

[Q09] 创建唯一索引
来源：http://hz.chenzaomai.com/gtvbpywetc.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.nanxuanxn.top/gtfkzupaci.html

[Q10] 插入单行
来源：http://hz.zhaomingkeji.xyz/gtazlzdaxj.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.yuxming.cn/gtmehphkzm.html

[Q11] 一次插入多行
来源：http://hz.haohaochexian.top/gtlxkzddzo.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.xylfe.cn/gtbfsuihsj.html

[Q12] 插入后取自增 ID
来源：http://hz.nanxuanxn.top/gtqsmmszio.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.havefunace.top/gtvungpsmq.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.zdqjudy.top/gtsitsoety.html

[Q13] 忽略重复插入
来源：http://hz.haohaochexian.top/gtvvbkopaw.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.mhx1999.top/gtyyaofyys.html

[Q14] 存在则更新（upsert）
来源：http://hz.nwbrower.top/gtcnyoywfz.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.quarkkingdee.top/gtvhlnvdcn.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.zhijiandao.cn/gtnzrtasnk.html

[Q15] 查询全部
来源：http://hz.sufxvd.cn/gtrntmmxfz.html

SELECT * FROM users;
来源：http://hz.hfpthk.cn/gtevvnrbgf.html

[Q16] 查询指定列
来源：http://hz.ppjwa.cn/gtxetvbqat.html

SELECT id, name FROM users;
来源：http://hz.sxryk.cn/gtudrxrwgm.html

[Q17] 条件查询
来源：http://hz.hnxiangtu.top/gtxovtijdi.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.hnqzz.top/gtkcpimlcl.html

[Q18] 模糊匹配
来源：http://hz.jinqigufen.top/gtpmtwjizt.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.ybcxt.top/gtcfaynnrs.html

[Q19] 范围查询
来源：http://hz.zhiwuduotai.top/gtjdikhbki.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.feifeiyinyue.top/gtxwklocqb.html

[Q20] IN 列表
来源：http://hz.zhiwuduotai.top/gtrynbfizz.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.ywan-chungtsiang.top/gtepbhiemb.html

[Q21] 空值判断
来源：http://hz.sufxvd.cn/gtamrhkizy.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.jlsjyb.cn/gtjiothboi.html

[Q22] 排序
来源：http://hz.xuanzx.com/gtedksfxfb.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.316326.xyz/gtwfbwyizn.html

[Q23] 分页
来源：http://hz.316326.xyz/gtcaedghda.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.mhx1999.top/gtdiwclmri.html

[Q24] 去重
来源：http://hz.zhoulong.xyz/gtvphvtxiu.html

SELECT DISTINCT city FROM users;
来源：http://hz.ywan-chungtsiang.top/gtwaapydca.html

[Q25] 只取前 N 条
来源：http://hz.tian-w.cn/gtcnaekvht.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.yonumen.top/gtgmnrclqu.html

[Q26] 计数
来源：http://hz.zdqjudy.top/gtfvexekjz.html

SELECT COUNT(*) FROM users;
来源：http://hz.yueranfly.top/gtdrvzbele.html

[Q27] 条件计数
来源：http://hz.yangfankeji.com/gttshublmc.html


<!-- 参考信息 -->