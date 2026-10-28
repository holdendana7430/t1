代发 wailian999

PHP:  // 递归实现，或用 usort
来源：http://hz.cheryme.top/gtxxfgdmrz.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.yj20258888.top/gtbbjennqk.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.jinghuilouyu.cn/gtzsbidtbo.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.ybcxt.top/gtyxojlcgg.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.zhijiandao.cn/gtsfufxyvr.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.fengsongda.top/gtmtsjkeum.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.fzhhl.top/gtfrikjrpy.html

[N04] 斐波那契数列
来源：http://hz.daxiang520.top/gtxzylefji.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.wangdashe.top/gtsrvkmjed.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.nanxuanxn.top/gtqphgzmhb.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.guannengcc.top/gtzmlaxhqs.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.shuidangran.top/gtsepzfjby.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.sxryk.cn/gttwjrqahy.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.xziqi.cn/gtvkmupyfm.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.hammf.cn/gttiphvcea.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.cdnleiting.top/gtikyiiqly.html

[N05] 最大公约数
来源：http://hz.cheryme.top/gtuybsbehv.html

Py:   math.gcd(a, b)
来源：http://hz.nanxuanxn.top/gtrfiaokyg.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.yangfankeji.com/gtinspcfzh.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.ydzc1.top/gtlvhqdbtw.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.zhixingplan.top/gtodluiaqd.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.mhx1999.top/gtmhiikqrb.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.xinyue.icu/gtsodbcqrl.html

Ruby: a.gcd(b)
来源：http://hz.xingfuxueyuan.xyz/gtjsdloapf.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.yj202588.top/gtcyyyhwar.html

[N06] 判断回文字符串
来源：http://hz.pengpengdd.cyou/gtbncdtpxl.html

Py:   s == s[::-1]
来源：http://hz.iojbl.cn/gtdyshykop.html

PHP:  $s === strrev($s);
来源：http://hz.hywenlv.cn/gtztcwiehy.html

JS:   s === [...s].reverse().join("")
来源：http://hz.gogol.net.cn/gtjthejuko.html

TS:   s === [...s].reverse().join("")
来源：http://hz.ehwqpu.com/gtdzlwscgb.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.cqqwz.cn/gtehwdmadh.html

Go:   // 双指针从两端比较
来源：http://hz.vqdsnc.cn/gtsousxeab.html

Ruby: s == s.reverse
来源：http://hz.zhixingplan.top/gtgmaugmdu.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.ehwqpu.com/gtwhkdaeco.html

[N07] 两数之和（返回下标）
来源：http://hz.hnxiangtu.top/gthedujmor.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.zhiwuduotai.top/gtkinbmgau.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.havefunace.top/gtygareijt.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.yj20258.top/gtylevgevq.html

TS:   // 手写 Map<string, number>
来源：http://hz.yuxming.cn/gtjhmpyqih.html

Java: // 手写 HashMap
来源：http://hz.shzxlz.cn/gtdrrpfvxn.html

Go:   // 手写 map[int]int
来源：http://hz.gogol.net.cn/gtpampwjfq.html

Ruby: // 手写 Hash
来源：http://hz.hongshengwenyu.top/gtnesedweu.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.pengpengdd.cyou/gthaorsxej.html

[N08] 生成全排列
来源：http://hz.yongpay.top/gtlrlnqmxj.html

Py:   itertools.permutations(arr)
来源：http://hz.fengsongda.top/gtqsnrsiks.html

PHP:  // 手写递归交换
来源：http://hz.iojbl.cn/gtbdzufinp.html

JS:   // 手写回溯递归
来源：http://hz.yanxiufei.cn/gtmydxvdhg.html

TS:   // 手写回溯递归
来源：http://hz.gotoacloud.top/gtuodzzzut.html

Java: // 手写回溯递归
来源：http://hz.aizwys.cn/gteuujyzbu.html

Go:   // 手写回溯递归
来源：http://hz.smart0.xyz/gtsurubcza.html

Ruby: arr.permutation.to_a
来源：http://hz.52xcode.cn/gtlgtafruy.html

C#:   // 手写回溯递归
来源：http://hz.ppjwa.cn/gtzjdqmcap.html

[N09] 栈与队列
来源：http://hz.chenzaomai.com/gtvljoibup.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.kuanghao11.cn/gtjvdigptg.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.xziqi.cn/gtpldwrbls.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.ivvv.top/gtnwbvcnnn.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.ybcxt.top/gtnbfhzoaz.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.andypj.xyz/gthwmikotd.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.jiagoushi.top/gtygmxymob.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.tianlin.xyz/gtdrovvlgf.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.jiagoushi.top/gtfauzoube.html

[N10] 链表节点定义
来源：http://hz.shangyingyoupin.top/gtjxwikuhi.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.zhongyouzk.top/gtoqfwxnlx.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.iojbl.cn/gtdvkefflq.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.jinyuanbaomall.cn/gtvdivjlbr.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.pengpengdd.cyou/gtcbmyvohp.html

Java: class Node { int v; Node next; }
来源：http://hz.xuetiantiany.cn/gtkxwqudth.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.zhixingplan.top/gtyoursbcx.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.c1oappe.top/gtvwvoivfq.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.gzhubu.top/gtfvyyvufg.html

[N11] 二叉树中序遍历
来源：http://hz.pengpengdd.cyou/gtapbcaaod.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.yanxiufei.cn/gtkgtbvswj.html

PHP:  // 手写递归函数
来源：http://hz.havefunace.top/gtkfdeqfao.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.jinqigufen.top/gtwtlvgbxh.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.mhx1999.top/gtzdxbofer.html

Java: // 手写递归
来源：http://hz.guannengcc.top/gtybjiesik.html

Go:   // 手写递归
来源：http://hz.sweek.top/gtsogjnwlw.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.jinqigufen.top/gtqywnrctu.html

C#:   // 手写递归
来源：http://hz.ydzc1.top/gtxomgrjuj.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.nanxinkj.top/gtcqsurgvb.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.iojbl.cn/gtqqdmgekm.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.yanxiufei.cn/gtmjutjbrl.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.nanxuanxn.top/gtphglbyak.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.ppjwa.cn/gtfnyhozay.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.andypj.xyz/gtxtmwnltv.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.hnqzz.top/gtsqzttbuv.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.dianchejie.cn/gtsidkiuoz.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.cucudq.cn/gthdjymqjn.html

================================================================================
来源：http://hz.sufxvd.cn/gtfvyljnhm.html

O. 并发与异步
来源：http://hz.gaohongyu789.top/gttowpideu.html

================================================================================
来源：http://hz.xuetiantiany.cn/gttrctptum.html

[O01] 启动一个线程
来源：http://hz.c1oappe.top/gttcpclwxw.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.smart0.xyz/gtmuktqfrc.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.zhoulong.xyz/gtvegohtyu.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.xinyue.icu/gtzgdukffn.html

TS:   // 同 JS
来源：http://hz.xylfe.cn/gtebfslrdy.html

Java: new Thread(() -> f()).start()
来源：http://hz.yvedp.cn/gtbovhykai.html

Go:   go f()
来源：http://hz.quarkkingdee.top/gtwzwibhpx.html

Ruby: Thread.new { f }
来源：http://hz.jinqigufen.top/gtlatniacv.html

C#:   Task.Run(() => F());
来源：http://hz.iojbl.cn/gtgjjcabpd.html

[O02] 使用线程池
来源：http://hz.zhongyouzk.top/gtvwvbywrj.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.xuetiantiany.cn/gtezxejwxi.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.vqdsnc.cn/gtikbzwntn.html

JS:   // worker_threads 线程池
来源：http://hz.cqqwz.cn/gtaorgdisy.html

TS:   // worker_threads 线程池
来源：http://hz.yuxming.cn/gtaycarfvt.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.shanyushiyangkeji.top/gtmomlkzoc.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.gotoacloud.top/gtczafeaqs.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.xziqi.cn/gtssoualka.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.shanyushiyangkeji.top/gtvzpmckin.html

[O03] 加锁保护共享数据
来源：http://hz.c1oappe.top/gteyntnhdd.html

Py:   with lock: shared += 1
来源：http://hz.cucudq.cn/gtrihbnhoq.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.ydjk.org.cn/gtkmkibbpk.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.gzhubu.top/gtgngowfut.html

TS:   // 同 JS
来源：http://hz.sufxvd.cn/gtzwnfmzkq.html

Java: synchronized (this) { shared++; }
来源：http://hz.jqgufenzy.top/gtrgiummof.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.9152youxi.cn/gtkybdozlg.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.jiagoushi.top/gtqqknichq.html

C#:   lock (gate) { shared++; }
来源：http://hz.shzxlz.cn/gtvkkbnvoe.html

[O04] 定义异步函数并等待
来源：http://hz.haohaochexian.top/gtazqzxvvz.html

Py:   async def f():⏎    await g()
来源：http://hz.zhongyouzk.top/gtxfhzxldr.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.quarkkingdee.top/gtmawhjlbu.html

JS:   async function f() { await g(); }
来源：http://hz.9152youxi.cn/gtwbcqzqqh.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.0kj1m.cn/gtvcsukuus.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.chenjidiqi.icu/gtriwbbmbj.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.jinghuilouyu.cn/gtvmrzhpua.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.nanxuanxn.top/gtyfnfvygt.html

C#:   async Task F() { await G(); }
来源：http://hz.svipenyu.cn/gtpklhambe.html

[O05] 并发执行并等待全部完成
来源：http://hz.aibaodan.cn/gtwvtobsbr.html

Py:   asyncio.gather(*tasks)
来源：http://hz.aibaodan.cn/gtcrnpdxjm.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.guowangkeji.top/gtvbrxlgzj.html

JS:   await Promise.all(tasks)
来源：http://hz.ybcxt.top/gtjzcxasty.html

TS:   await Promise.all(tasks)
来源：http://hz.chenjidiqi.icu/gtxtkwoewt.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.tian-w.cn/gttnnpoatn.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.ydjk.org.cn/gtqstifnbw.html

Ruby: threads.map(&:join)
来源：http://hz.xylfe.cn/gtcxxnlcgv.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.jinghuilouyu.cn/gtoitizkzo.html

[O06] 使用进程池
来源：http://hz.zhijiandao.cn/gtecdkupfi.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.jiagoushi.top/gtpueysige.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.quarkkingdee.top/gtlyqbcyrc.html

JS:   // child_process / cluster 模块
来源：http://hz.jianghu66.top/gtwfblixxx.html

TS:   // child_process / cluster 模块
来源：http://hz.sxryk.cn/gtglagenlg.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.ydzc1.top/gtijqpixzf.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.yonumen.top/gtjddazdlw.html

Ruby: // fork 块
来源：http://hz.jyoumei.cn/gtjbrwgiyc.html

C#:   Parallel.For
来源：http://hz.shanyushiyangkeji.top/gtqmdsycfq.html

================================================================================
来源：http://hz.guannengcc.top/gtfarrweha.html

P. 常用工具函数
来源：http://hz.wangdashe.top/gtwxbumnpp.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gtsdedybip.html

[P01] 生成 UUID
来源：http://hz.andypj.xyz/gtssrxbwvz.html

Py:   str(uuid.uuid4())
来源：http://hz.zycfv.cn/gtooijyotl.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.daria6918.cn/gtthgafuks.html

JS:   crypto.randomUUID()
来源：http://hz.vqdsnc.cn/gtncesafoa.html

TS:   crypto.randomUUID()
来源：http://hz.zhoulong.xyz/gtimlbulrl.html

Java: UUID.randomUUID().toString()
来源：http://hz.xinyue.icu/gtphzrafzc.html

Go:   // 用 github.com/google/uuid
来源：http://hz.chenlongwang.top/gtuexirmcl.html

Ruby: SecureRandom.uuid
来源：http://hz.meibo888.top/gtogzebtxf.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.yongpay.top/gtoqhcfwch.html

[P02] MD5 / SHA256 摘要
来源：http://hz.yonumen.top/gtekhnrjsg.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.sweek.top/gtddemphyu.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.wangshuangyany.cn/gtvwfcdqdb.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.snrcjt.cn/gtaouqbrqv.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.zhengqikj.top/gtfyodihkl.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.havefunace.top/gtakiquxrz.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.gogol.net.cn/gtkmvzkmwa.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.hnxiangtu.top/gthdjaljqt.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.hnxiangtu.top/gtfxrhnvjc.html

[P03] 生成短随机字符串
来源：http://hz.pycfn.com/gtivgmqwyz.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.sweek.top/gtmeaijqrp.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.ywan-chungtsiang.top/gtyaicoips.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.guannengcc.top/gtqotxoccv.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.chenlongwang.top/gtfftqgson.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.havefunace.top/gtwunxvakv.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.ivvv.top/gttkmszusd.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.cheryme.top/gtpklliiej.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.bjfxy.top/gtbmguauzo.html

[P04] 求长度
来源：http://hz.kuanghao11.cn/gtllomehgr.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.tanke756.top/gtembdeoue.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.xuetiantiany.cn/gtdsmwhcem.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.yanxiufei.cn/gtccgrrgql.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.yangfankeji.com/gtzwbqfdxe.html

Java: list.size();  map.size();  s.length()
来源：http://hz.vqdsnc.cn/gtjbwahgvl.html

Go:   len(arr);  len(m)
来源：http://hz.wangdashe.top/gtiqthozew.html

Ruby: x.length;  x.size
来源：http://hz.hammf.cn/gtyczpcqtn.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.ppjwa.cn/gtfhlfjzbj.html

[P05] 判断两个对象内容是否相等
来源：http://hz.zhixingplan.top/gtzincdbme.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.jianghu66.top/gtfkkvwxyw.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.vqdsnc.cn/gtcjrhsxwj.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.chenzaomai.com/gtnkhipgtk.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.xuetiantiany.cn/gtzjfxxnmk.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.jinyuanbaomall.cn/gtrggctmgd.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.kuanghao11.cn/gtnylqfgjc.html

Ruby: a == b
来源：http://hz.hnqzz.top/gtrshwtuoj.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.yj20258888.top/gtgksdsncm.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.smart0.xyz/gttirljaov.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.ydzc1.top/gtvlpzfhbl.html

PHP:  if (empty($x)) {}
来源：http://hz.yuxming.cn/gtreosasrl.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.zhiwuduotai.top/gtuylrupbj.html

TS:   if (x == null) {}
来源：http://hz.cucudq.cn/gtzgdniika.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.birdmap.top/gtuvbfcmpu.html

Go:   if x == nil {}
来源：http://hz.pengpengdd.cyou/gtmjsbukpo.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.svipenyu.cn/gtnzlvupji.html

C#:   if (x is null) {}
来源：http://hz.jlsjyb.cn/gtqjrvrcgv.html

[P07] 防抖与节流
来源：http://hz.xingfuxueyuan.xyz/gtddmjfkqm.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.c1oappe.top/gtcxfzrmlj.html

PHP:  // 手写时间戳比较
来源：http://hz.kuanghao11.cn/gtcxdvyfhw.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.hongshengwenyu.top/gtapxmzeao.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.sweek.top/gtarvowrpu.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.yj202588.top/gtyycgxvyl.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.zdqjudy.top/gtlkzcoula.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.hnxiangtu.top/gtloxugcss.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.jqgfzy.top/gtjagfvwiw.html

[P08] 处理浮点精度问题
来源：http://hz.jiagoushi.top/gtyltfnwoq.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.xuanzx.com/gtvawguhnv.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.zhengqikj.top/gtfengqthr.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.daxiang520.top/gtsxwrnsnt.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.pycfn.com/gtgvjfibva.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.xziqi.cn/gtkxptmrze.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.gogol.net.cn/gtdsgwllht.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.cucudq.cn/gtuxonfdle.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.hnxiangtu.top/gtihjugupe.html

================================================================================
来源：http://hz.0kj1m.cn/gtjcojvhiv.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.9152youxi.cn/gtajbfjprp.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtxsvdopsm.html

[Q01] 创建表
来源：http://hz.svipenyu.cn/gtsgglywwn.html

CREATE TABLE users (
来源：http://hz.316326.xyz/gtzgfphsix.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.nwbrower.top/gtisibtuuz.html

name VARCHAR(50) NOT NULL,
来源：http://hz.yangfankeji.com/gtwcwwpjuy.html

email VARCHAR(100) UNIQUE,
来源：http://hz.jiagoushi.top/gttlxxjfmx.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.ywan-chungtsiang.top/gtrqawdadb.html

);
来源：http://hz.bjfxy.top/gtbogtslpd.html

[Q02] 创建带外键的表
来源：http://hz.shangyingyoupin.top/gtxnftdchj.html

CREATE TABLE orders (
来源：http://hz.zhongyouzk.top/gtkdaxkjrl.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.ivvv.top/gthemysagl.html

user_id INT NOT NULL,
来源：http://hz.tian-w.cn/gtkcbvmsid.html

amount DECIMAL(10, 2),
来源：http://hz.ybcxt.top/gtjpvhuygd.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.chenzaomai.com/gtcplxavlb.html

);
来源：http://hz.pengpengdd.cyou/gtjomragew.html

[Q03] 增加列
来源：http://hz.c1oappe.top/gtuwjgsbas.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.ybcxt.top/gtqsdpujbo.html

[Q04] 修改列类型
来源：http://hz.zhiwuduotai.top/gtmkdirpwv.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.hysaishi.cn/gtqzkpszpp.html

[Q05] 重命名列
来源：http://hz.hnxiangtu.top/gtjmvsjuai.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.sweek.top/gtkddaehqw.html

[Q06] 删除列
来源：http://hz.andypj.xyz/gtcmrtfqct.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.birdmap.top/gtwfyxbwri.html

[Q07] 删除表
来源：http://hz.shuidangran.top/gtkfgksxrx.html

DROP TABLE IF EXISTS orders;
来源：http://hz.c1oappe.top/gtyrpjvmps.html

[Q08] 创建普通索引
来源：http://hz.gaohongyu789.top/gtjihdfkwj.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.jyoumei.cn/gtiogkpdxj.html

[Q09] 创建唯一索引
来源：http://hz.bjfxy.top/gtakfwqpon.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.sufxvd.cn/gtavxkezcn.html

[Q10] 插入单行
来源：http://hz.zdqjudy.top/gtumveqyqz.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.ivvv.top/gtrcxkvxlq.html

[Q11] 一次插入多行
来源：http://hz.zhengqikj.top/gtezpikidx.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.sxryk.cn/gttbywubhl.html

[Q12] 插入后取自增 ID
来源：http://hz.yueranfly.top/gtxzsrriju.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.redwolf501.top/gtbrrlsdzq.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.ehwqpu.com/gthxivmovi.html

[Q13] 忽略重复插入
来源：http://hz.guowangkeji.top/gtkbysrkrb.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.zhaomingkeji.xyz/gtjhcjjvkr.html

[Q14] 存在则更新（upsert）
来源：http://hz.zdqjudy.top/gtftjxxnug.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.iojbl.cn/gtsdaxfbfh.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.chenjidiqi.icu/gtcqlbgcbk.html

[Q15] 查询全部
来源：http://hz.kuanghao11.cn/gtghmduvku.html

SELECT * FROM users;
来源：http://hz.birdmap.top/gtdxgqlobs.html

[Q16] 查询指定列
来源：http://hz.hammf.cn/gthpckkrir.html

SELECT id, name FROM users;
来源：http://hz.sufxvd.cn/gteqvrkwux.html

[Q17] 条件查询
来源：http://hz.smart0.xyz/gtugnapeak.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.smart0.xyz/gtjzrfpzfv.html

[Q18] 模糊匹配
来源：http://hz.sufxvd.cn/gtiotvijle.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.xziqi.cn/gteqpwkcef.html

[Q19] 范围查询
来源：http://hz.snrcjt.cn/gtigjjffph.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.zhoulong.xyz/gtvgyqvwrb.html

[Q20] IN 列表
来源：http://hz.chenlongwang.top/gteyqxqzzv.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.ehwqpu.com/gthtywyjvl.html

[Q21] 空值判断
来源：http://hz.jinqigfzy.top/gtahhhxswl.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.svipenyu.cn/gtirurvncy.html

[Q22] 排序
来源：http://hz.jiagoushi.top/gtjzmsunuv.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.zhengqikj.top/gtkzvmtzno.html

[Q23] 分页
来源：http://hz.wangdashe.top/gtyvcrijdb.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.yj202588.top/gtdmoobtdb.html

[Q24] 去重
来源：http://hz.vqdsnc.cn/gtopdzxyhd.html

SELECT DISTINCT city FROM users;
来源：http://hz.fzhhl.top/gtdmygznjg.html

[Q25] 只取前 N 条
来源：http://hz.jqgfzy.top/gtjqraxbsp.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.smart0.xyz/gtdndjbkoa.html

[Q26] 计数
来源：http://hz.hammf.cn/gtetuhllve.html

SELECT COUNT(*) FROM users;
来源：http://hz.cdnleiting.top/gtdefrzhfq.html

[Q27] 条件计数
来源：http://hz.ybcxt.top/gtvlzyaufh.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.ywan-chungtsiang.top/gttzpifovp.html

[Q28] 求和与平均
来源：http://hz.pycfn.com/gtjwlgkpwa.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.shanyushiyangkeji.top/gthpfontmc.html

[Q29] 最大最小值
来源：http://hz.andypj.xyz/gtkvwjkibt.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.zhijiandao.cn/gttxqjueqj.html

[Q30] 分组统计
来源：http://hz.jinqigfzy.top/gtuclapfep.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.chenzaomai.com/gtbsgblrsa.html

[Q31] 分组后过滤
来源：http://hz.mhx1999.top/gtnmtdkryl.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.hywenlv.cn/gtqtesbmmp.html

[Q32] 分组拼接字符串
来源：http://hz.meibo888.top/gtcqurmvzt.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.yj20258888.top/gtqewqbpnq.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.gogol.net.cn/gtvbhwrbpp.html


<!-- 参考信息 -->