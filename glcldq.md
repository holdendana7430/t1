代发 wailian999

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.fzhhl.top/gtoiaaqyaz.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.ywan-chungtsiang.top/gtadivclwn.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.xinyue.icu/gthcfmcdnb.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.birdmap.top/gtuxdvsfos.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.aibaodan.cn/gtqzuxafzw.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.pycfn.com/gtvahxqxgz.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.zhijiandao.cn/gtzzrozehe.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.jiagoushi.top/gtiyverpse.html

[N05] 最大公约数
来源：http://hz.xuetiantiany.cn/gthzuylmrz.html

Py:   math.gcd(a, b)
来源：http://hz.jinqigufen.top/gtfylncjkp.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.jinqigfzy.top/gtuwtlaqod.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.ybcxt.top/gttgfxwftu.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.aibaodan.cn/gtbuszhjkn.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.sweek.top/gtlsbkrfmr.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.ppjwa.cn/gtnvslelre.html

Ruby: a.gcd(b)
来源：http://hz.wangdashe.top/gtdvzohlwp.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.ywan-chungtsiang.top/gtjzlkfmpm.html

[N06] 判断回文字符串
来源：http://hz.yanxiufei.cn/gtnjdzngpt.html

Py:   s == s[::-1]
来源：http://hz.hysaishi.cn/gtlnjshfae.html

PHP:  $s === strrev($s);
来源：http://hz.quarkkingdee.top/gttzlvbmrn.html

JS:   s === [...s].reverse().join("")
来源：http://hz.316326.xyz/gthtclglws.html

TS:   s === [...s].reverse().join("")
来源：http://hz.hongshengwenyu.top/gtxumhtzgd.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.ydjk.org.cn/gtxfqoeuzy.html

Go:   // 双指针从两端比较
来源：http://hz.chenjidiqi.icu/gtwqavpylm.html

Ruby: s == s.reverse
来源：http://hz.jyoumei.cn/gteezuosjm.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.9152youxi.cn/gtwzfqcihj.html

[N07] 两数之和（返回下标）
来源：http://hz.havefunace.top/gtzjeabueu.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.ybcxt.top/gtvryzesbs.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.smart0.xyz/gtcdlykgzu.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.xziqi.cn/gtckaszhsv.html

TS:   // 手写 Map<string, number>
来源：http://hz.zdqjudy.top/gthotswabv.html

Java: // 手写 HashMap
来源：http://hz.cheryme.top/gtuhjmzbyx.html

Go:   // 手写 map[int]int
来源：http://hz.0kj1m.cn/gtbuaplfcj.html

Ruby: // 手写 Hash
来源：http://hz.xuetiantiany.cn/gttzbbxjzb.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.ivvv.top/gtwqtaarxy.html

[N08] 生成全排列
来源：http://hz.zhaomingkeji.xyz/gtngbxacgh.html

Py:   itertools.permutations(arr)
来源：http://hz.ivvv.top/gtgujbmyim.html

PHP:  // 手写递归交换
来源：http://hz.gzhubu.top/gtnqugrusq.html

JS:   // 手写回溯递归
来源：http://hz.andypj.xyz/gtsajukxaz.html

TS:   // 手写回溯递归
来源：http://hz.yongpay.top/gtcaecehly.html

Java: // 手写回溯递归
来源：http://hz.wangdashe.top/gtdlbojmjt.html

Go:   // 手写回溯递归
来源：http://hz.yuxming.cn/gtluljohdm.html

Ruby: arr.permutation.to_a
来源：http://hz.yangfankeji.com/gtdgfvlhsu.html

C#:   // 手写回溯递归
来源：http://hz.wangdashe.top/gtjcnpdprz.html

[N09] 栈与队列
来源：http://hz.zhijiandao.cn/gtyzkumkxa.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.sysykeji.top/gtafxenmwl.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.mhx1999.top/gtomrtyjxn.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.sufxvd.cn/gtmcqwpdye.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.zhaomingkeji.xyz/gtvhnrfkjr.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.ppjwa.cn/gtywnereic.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.daxiang520.top/gtxsqyfvzp.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.yuanzhike.top/gtkwzrppci.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.mhx1999.top/gthnqowtnp.html

[N10] 链表节点定义
来源：http://hz.cashguo.top/gtmjqrerct.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.sweek.top/gtgirqejgb.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.iojbl.cn/gtzgzmuham.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.yueranfly.top/gtidvxmkap.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.yongpay.top/gtwmtjhxvy.html

Java: class Node { int v; Node next; }
来源：http://hz.hnqzz.top/gtfjdxhmrl.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.316326.xyz/gtvehxkkef.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.cucudq.cn/gtspmjfbro.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.gzhubu.top/gtvaruhnzb.html

[N11] 二叉树中序遍历
来源：http://hz.yonumen.top/gtematxhgl.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.hongshengwenyu.top/gtbncfingo.html

PHP:  // 手写递归函数
来源：http://hz.yuxming.cn/gtadhznuwj.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.hfpthk.cn/gtvbkaifxk.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.yueranfly.top/gtmceppwdu.html

Java: // 手写递归
来源：http://hz.sweek.top/gtualnaauv.html

Go:   // 手写递归
来源：http://hz.gotoacloud.top/gtatccyvcl.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.zhaomingkeji.xyz/gttvnaktnt.html

C#:   // 手写递归
来源：http://hz.jinghuilouyu.cn/gtbkcmbtni.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.guowangkeji.top/gtzbovlidz.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.ydjk.org.cn/gtomfhqlza.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.zdqjudy.top/gtkzrbthlv.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.sufxvd.cn/gtkhttpebz.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.chenlongwang.top/gtbxxqucbe.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.nanxinkj.top/gtrrxtxtzl.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.svipenyu.cn/gtaorkwpfi.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.aizwys.cn/gtijgpauyn.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.hnxiangtu.top/gtrcofieeb.html

================================================================================
来源：http://hz.tianlin.xyz/gtaaozcnew.html

O. 并发与异步
来源：http://hz.haohaochexian.top/gtpopyvohw.html

================================================================================
来源：http://hz.yanxiufei.cn/gtvhfmlgna.html

[O01] 启动一个线程
来源：http://hz.guannengcc.top/gtwhnlbjzo.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.nanxinkj.top/gtqgtxxhcj.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.aibaodan.cn/gtuxbphfsb.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.smart0.xyz/gtqhdwbnkq.html

TS:   // 同 JS
来源：http://hz.gotoacloud.top/gtushvcrmw.html

Java: new Thread(() -> f()).start()
来源：http://hz.svipenyu.cn/gtojycxolx.html

Go:   go f()
来源：http://hz.nwbrower.top/gtxuscjcvj.html

Ruby: Thread.new { f }
来源：http://hz.jyoumei.cn/gtasaxhdwm.html

C#:   Task.Run(() => F());
来源：http://hz.andypj.xyz/gtifcticzw.html

[O02] 使用线程池
来源：http://hz.ybcxt.top/gtoonedwkc.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.daxiang520.top/gthivkpxhd.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.jqgfzy.top/gtkwzlpbpp.html

JS:   // worker_threads 线程池
来源：http://hz.zhiwuduotai.top/gtwtalvoeo.html

TS:   // worker_threads 线程池
来源：http://hz.fengsongda.top/gtxdthbwho.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.jiagoushi.top/gtzxzmpakt.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.jiagoushi.top/gttxpycvyh.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.zhongyouzk.top/gtwvrkwpdb.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.hfpthk.cn/gtsgdauzna.html

[O03] 加锁保护共享数据
来源：http://hz.9152youxi.cn/gtqxqreggi.html

Py:   with lock: shared += 1
来源：http://hz.tianlin.xyz/gtvswrguyy.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.fzhhl.top/gtyfifpvou.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.yongpay.top/gtruoqzlav.html

TS:   // 同 JS
来源：http://hz.andypj.xyz/gtqtbkirve.html

Java: synchronized (this) { shared++; }
来源：http://hz.cucudq.cn/gtyuacmody.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.hnqzz.top/gtikviqpxp.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.jyoumei.cn/gttfaxaycn.html

C#:   lock (gate) { shared++; }
来源：http://hz.hywenlv.cn/gtqblajatc.html

[O04] 定义异步函数并等待
来源：http://hz.jinghuilouyu.cn/gtpfdxhyfu.html

Py:   async def f():⏎    await g()
来源：http://hz.bjfxy.top/gteifugpld.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.hywenlv.cn/gtztiytzkx.html

JS:   async function f() { await g(); }
来源：http://hz.ppjwa.cn/gtgrnactmw.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.nwbrower.top/gtenclwqfa.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.shuidangran.top/gtuscyzzqq.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.pengpengdd.cyou/gtrblhbnci.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.ppjwa.cn/gtwptejeyw.html

C#:   async Task F() { await G(); }
来源：http://hz.chenlongwang.top/gtbopkxbhd.html

[O05] 并发执行并等待全部完成
来源：http://hz.smart0.xyz/gtfxhibmbs.html

Py:   asyncio.gather(*tasks)
来源：http://hz.guowangkeji.top/gtmgvrpdfd.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.bjfxy.top/gtrgtmyxso.html

JS:   await Promise.all(tasks)
来源：http://hz.316326.xyz/gtbdywpspa.html

TS:   await Promise.all(tasks)
来源：http://hz.tianlin.xyz/gtkfawzcbh.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.birdmap.top/gtmuzuhcnl.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.zdqjudy.top/gtnsyjhqyn.html

Ruby: threads.map(&:join)
来源：http://hz.zhongyouzk.top/gtsbwtltdg.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.aizwys.cn/gtlshmdrnk.html

[O06] 使用进程池
来源：http://hz.zhongyouzk.top/gtljfhyoeb.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.gogol.net.cn/gtjrtnjopf.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.feifeiyinyue.top/gttatedyog.html

JS:   // child_process / cluster 模块
来源：http://hz.chenzaomai.com/gtkluhvxff.html

TS:   // child_process / cluster 模块
来源：http://hz.zhongyouzk.top/gtewwwpimc.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.ydjk.org.cn/gtvfpimvcx.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.ybcxt.top/gtlsefgdkm.html

Ruby: // fork 块
来源：http://hz.zhaomingkeji.xyz/gtoklbccmx.html

C#:   Parallel.For
来源：http://hz.vqdsnc.cn/gtessnkimi.html

================================================================================
来源：http://hz.316326.xyz/gtzkotsoeg.html

P. 常用工具函数
来源：http://hz.yj20258.top/gtdldbnaec.html

================================================================================
来源：http://hz.jianghu66.top/gtakrcsant.html

[P01] 生成 UUID
来源：http://hz.dianchejie.cn/gtpulifslo.html

Py:   str(uuid.uuid4())
来源：http://hz.iojbl.cn/gtfysuruke.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.jinqigfzy.top/gtrkfxsqrb.html

JS:   crypto.randomUUID()
来源：http://hz.ydzc1.top/gtjthnzhow.html

TS:   crypto.randomUUID()
来源：http://hz.xingfuxueyuan.xyz/gtfcmbtnja.html

Java: UUID.randomUUID().toString()
来源：http://hz.cashguo.top/gthwghfstf.html

Go:   // 用 github.com/google/uuid
来源：http://hz.yj202588.top/gtwgdhqezj.html

Ruby: SecureRandom.uuid
来源：http://hz.wangshuangyany.cn/gtgrzeygtr.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.jlsjyb.cn/gtawgzlbnu.html

[P02] MD5 / SHA256 摘要
来源：http://hz.shzxlz.cn/gtlzkcndvg.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.aizwys.cn/gtlnvarpwc.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.xziqi.cn/gtyctoohmj.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.bjfxy.top/gtaxeahsuv.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.jinqigufen.top/gtdosyobct.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.xziqi.cn/gtuzspxtqp.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.yuxming.cn/gtlpaigfgm.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.cdnleiting.top/gtktcmiozr.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.andypj.xyz/gtwtvmkxic.html

[P03] 生成短随机字符串
来源：http://hz.hfpthk.cn/gtvwxzdowh.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.ywan-chungtsiang.top/gtpyebovpp.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.ivvv.top/gtfjbowlqe.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.jinghuilouyu.cn/gtakgbmisq.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.0kj1m.cn/gtczouptus.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.cucudq.cn/gtpkspjhas.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.fengsongda.top/gtjesadbal.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.sxryk.cn/gtwkjodcvn.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.yueranfly.top/gtpwkgnwrv.html

[P04] 求长度
来源：http://hz.sweek.top/gtjwfyspvm.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.ehwqpu.com/gtrzrjbbze.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.hongshengwenyu.top/gtpnpikrkv.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.sxryk.cn/gtvzwejsvi.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.hysaishi.cn/gtevuzrsuv.html

Java: list.size();  map.size();  s.length()
来源：http://hz.fzhhl.top/gtjldbbuwg.html

Go:   len(arr);  len(m)
来源：http://hz.xinyue.icu/gtsraguati.html

Ruby: x.length;  x.size
来源：http://hz.nanxinkj.top/gtyorrepjk.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.yvedp.cn/gtltiohhck.html

[P05] 判断两个对象内容是否相等
来源：http://hz.zhiwuduotai.top/gtkjkpqlut.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.zycfv.cn/gthxtwkzui.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.andypj.xyz/gtroeszxzm.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.wangshuangyany.cn/gtwggrlzfe.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.yongpay.top/gtdnjhmjho.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.9152youxi.cn/gtoaztrama.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.jyoumei.cn/gtxryuntrz.html

Ruby: a == b
来源：http://hz.jinqigufen.top/gtbaqsoszr.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.zhaomingkeji.xyz/gteynzbvvb.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.yj20258.top/gttnoaknwd.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.hfpthk.cn/gtnutceqmx.html

PHP:  if (empty($x)) {}
来源：http://hz.jqgufenzy.top/gtkinrayrn.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.quarkkingdee.top/gtvqwwzhpv.html

TS:   if (x == null) {}
来源：http://hz.chenjidiqi.icu/gtgvkavkdh.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.jianghu66.top/gtyygmxbxt.html

Go:   if x == nil {}
来源：http://hz.aibaodan.cn/gtoreyxzpe.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.hammf.cn/gtmlfurwxv.html

C#:   if (x is null) {}
来源：http://hz.cqqwz.cn/gtpbujcrql.html

[P07] 防抖与节流
来源：http://hz.daxiang520.top/gtmcviwgnd.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.zhongyouzk.top/gtpajeeohw.html

PHP:  // 手写时间戳比较
来源：http://hz.sweek.top/gteohmmozv.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.ehwqpu.com/gtcvhhqxbj.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.xylfe.cn/gtoywzbohi.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.cqqwz.cn/gtsugmneii.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.tianlin.xyz/gtuckaexlq.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.zhijiandao.cn/gttzbgeqpf.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.ydjk.org.cn/gtdbpqfsoa.html

[P08] 处理浮点精度问题
来源：http://hz.jinghuilouyu.cn/gtrjxxuwuf.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.zhoulong.xyz/gtalqypcqu.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.mhx1999.top/gtkkyzworg.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.316326.xyz/gtibvflfoh.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.pycfn.com/gtjrfymkva.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.jqgfzy.top/gtafgzjdqe.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.316326.xyz/gtzhtxhwby.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.zhijiandao.cn/gtswimkjfh.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.tanke756.top/gtpqmqoawd.html

================================================================================
来源：http://hz.shangyingyoupin.top/gtmzixuamu.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.yanxiufei.cn/gtrldcjgfc.html

================================================================================
来源：http://hz.jqgufenzy.top/gtweftioba.html

[Q01] 创建表
来源：http://hz.mhx1999.top/gteokvotvd.html

CREATE TABLE users (
来源：http://hz.jqgfzy.top/gtwawevdri.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.ydzc1.top/gtfgtkskao.html

name VARCHAR(50) NOT NULL,
来源：http://hz.xziqi.cn/gtgssutbxe.html

email VARCHAR(100) UNIQUE,
来源：http://hz.wangdashe.top/gtoyemesyn.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.ppjwa.cn/gtqxypiuoz.html

);
来源：http://hz.zhixingplan.top/gtfynylhpq.html

[Q02] 创建带外键的表
来源：http://hz.smart0.xyz/gtilyxrdzq.html

CREATE TABLE orders (
来源：http://hz.pycfn.com/gtywvliphw.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.jinyuanbaomall.cn/gtvngcahjh.html

user_id INT NOT NULL,
来源：http://hz.tianlin.xyz/gtzdrqjtct.html

amount DECIMAL(10, 2),
来源：http://hz.yj202588.top/gtgnuptvgk.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.zhiwuduotai.top/gtzehmlfab.html

);
来源：http://hz.haohaochexian.top/gtngujhtsm.html

[Q03] 增加列
来源：http://hz.chenlongwang.top/gtilwscmpd.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.yvedp.cn/gtlqegxdap.html

[Q04] 修改列类型
来源：http://hz.jyoumei.cn/gtghlzwnlp.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.jinghuilouyu.cn/gtgdcllzae.html

[Q05] 重命名列
来源：http://hz.ydjk.org.cn/gtjsaacpjz.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.aizwys.cn/gtmqtfeffe.html

[Q06] 删除列
来源：http://hz.yueranfly.top/gtfnleqggi.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.svipenyu.cn/gtufnphimi.html

[Q07] 删除表
来源：http://hz.nanxinkj.top/gtkmelchiy.html

DROP TABLE IF EXISTS orders;
来源：http://hz.xuanzx.com/gthmhelxxr.html

[Q08] 创建普通索引
来源：http://hz.yj202588.top/gtspvutagu.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.xuanzx.com/gtyygcnthl.html

[Q09] 创建唯一索引
来源：http://hz.daria6918.cn/gtdvzpkypq.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.shanyushiyangkeji.top/gtsyqqyoeb.html

[Q10] 插入单行
来源：http://hz.dianchejie.cn/gttmheqypy.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.shzxlz.cn/gtzubdnyck.html

[Q11] 一次插入多行
来源：http://hz.zdqjudy.top/gtpmbctawh.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.hongshengwenyu.top/gtbovzkrrb.html

[Q12] 插入后取自增 ID
来源：http://hz.jiagoushi.top/gtfgktuhkz.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.shuidangran.top/gtvajdnysb.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.zycfv.cn/gtvpadfqsc.html

[Q13] 忽略重复插入
来源：http://hz.tianlin.xyz/gtnikixyzv.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.meibo888.top/gtoxumtuqg.html

[Q14] 存在则更新（upsert）
来源：http://hz.shuidangran.top/gtrgwtnozo.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.gaohongyu789.top/gtdlowprzq.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.chenlongwang.top/gtqiputuoa.html

[Q15] 查询全部
来源：http://hz.9152youxi.cn/gtllscjzpr.html

SELECT * FROM users;
来源：http://hz.aibaodan.cn/gtbkfgeuin.html

[Q16] 查询指定列
来源：http://hz.jyoumei.cn/gtsyuugecg.html

SELECT id, name FROM users;
来源：http://hz.jyoumei.cn/gtfpytmilq.html

[Q17] 条件查询
来源：http://hz.meibo888.top/gtwoeqkghu.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.xinyue.icu/gtlhjdkllm.html

[Q18] 模糊匹配
来源：http://hz.dashuyun.cn/gtataazwat.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.daria6918.cn/gtjnfxjnkk.html

[Q19] 范围查询
来源：http://hz.hfpthk.cn/gtbzfsqxlq.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.shanyushiyangkeji.top/gtidietnfl.html

[Q20] IN 列表
来源：http://hz.iojbl.cn/gtkycruutu.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.fengsongda.top/gtqpowewhz.html

[Q21] 空值判断
来源：http://hz.yuanzhike.top/gtmhxjytzq.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.cdnleiting.top/gtyrhwtacy.html

[Q22] 排序
来源：http://hz.tianlin.xyz/gttzklcxrk.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.c1oappe.top/gtnqoakmec.html

[Q23] 分页
来源：http://hz.andypj.xyz/gtvsuntyjo.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.andypj.xyz/gtorccxvxk.html

[Q24] 去重
来源：http://hz.jlsjyb.cn/gtuwzutmah.html

SELECT DISTINCT city FROM users;
来源：http://hz.daxiang520.top/gtoywvdijw.html

[Q25] 只取前 N 条
来源：http://hz.daria6918.cn/gtpsmqnqcw.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.andypj.xyz/gtssroclvb.html

[Q26] 计数
来源：http://hz.shanyushiyangkeji.top/gtjfaaxvjc.html

SELECT COUNT(*) FROM users;
来源：http://hz.shuidangran.top/gtjxvoplbq.html

[Q27] 条件计数
来源：http://hz.xuanzx.com/gtdamfmovg.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.xziqi.cn/gtyoihzndi.html

[Q28] 求和与平均
来源：http://hz.guowangkeji.top/gteiwfndck.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.0kj1m.cn/gtyisptmrd.html

[Q29] 最大最小值
来源：http://hz.chenlongwang.top/gtcoetexuf.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.iojbl.cn/gtvjuzirzt.html

[Q30] 分组统计
来源：http://hz.bjfxy.top/gtypwirdau.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.zhoulong.xyz/gtlmlkszhh.html

[Q31] 分组后过滤
来源：http://hz.vqdsnc.cn/gttshjbnls.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.zhiwuduotai.top/gtzuqkuxid.html

[Q32] 分组拼接字符串
来源：http://hz.tanke756.top/gtalttmznn.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.316326.xyz/gtjoberaeb.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.gzhubu.top/gtbjhdybsd.html

[Q33] 多列分组
来源：http://hz.hammf.cn/gtnpcaymtz.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.redwolf501.top/gtddqpddif.html

[Q34] 每组取第一条
来源：http://hz.tian-w.cn/gtrlbaavvf.html

SELECT * FROM (
来源：http://hz.9152youxi.cn/gttfztwfun.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.yongpay.top/gtuwlqnrtv.html

) t WHERE rn = 1;
来源：http://hz.shanyushiyangtech.top/gtgshsmqaz.html

[Q35] 内连接
来源：http://hz.havefunace.top/gttrcypjkf.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.ybcxt.top/gtzfckwfpn.html


<!-- 参考信息 -->