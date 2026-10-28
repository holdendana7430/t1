代发 wailian999

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.gogol.net.cn/gtdfgsityf.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.cdnleiting.top/gttygrfzos.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.kuanghao11.cn/gtdyddlnue.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.ybcxt.top/gtaqufrpek.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.cqqwz.cn/gtszihsbbd.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.birdmap.top/gtladvyszh.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.sufxvd.cn/gtvrobtkht.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.chenzaomai.com/gttpwdqybg.html

[N05] 最大公约数
来源：http://hz.hammf.cn/gtmsvereal.html

Py:   math.gcd(a, b)
来源：http://hz.redwolf501.top/gtsabujsej.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.shzxlz.cn/gtqhmnlcyh.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.jinghuilouyu.cn/gttpayfprb.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.cashguo.top/gtyqgjjgzs.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.daxiang520.top/gthzgigenf.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.dianchejie.cn/gtupbqsuvs.html

Ruby: a.gcd(b)
来源：http://hz.quarkkingdee.top/gtdvpvgjqn.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.yvedp.cn/gtrgdgpqnk.html

[N06] 判断回文字符串
来源：http://hz.shzxlz.cn/gtzsdpptqe.html

Py:   s == s[::-1]
来源：http://hz.zhongyouzk.top/gtltwzwysk.html

PHP:  $s === strrev($s);
来源：http://hz.quarkkingdee.top/gtzixkwdlx.html

JS:   s === [...s].reverse().join("")
来源：http://hz.ydzc1.top/gtgcxtoxmr.html

TS:   s === [...s].reverse().join("")
来源：http://hz.chenzaomai.com/gtnvqriccz.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.feifeiyinyue.top/gtuznnhtql.html

Go:   // 双指针从两端比较
来源：http://hz.jyoumei.cn/gtgzjtghfp.html

Ruby: s == s.reverse
来源：http://hz.cdnleiting.top/gtkhbhwpmj.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.pengpengdd.cyou/gthwdhvppt.html

[N07] 两数之和（返回下标）
来源：http://hz.xinyue.icu/gtbicmxlrw.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.nanxinkj.top/gthtbpyirz.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.haohaochexian.top/gtmtijwwrx.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.kuanghao11.cn/gtbcrixzlo.html

TS:   // 手写 Map<string, number>
来源：http://hz.jinghuilouyu.cn/gtkhywuqwy.html

Java: // 手写 HashMap
来源：http://hz.chenlongwang.top/gtuduxnhzs.html

Go:   // 手写 map[int]int
来源：http://hz.9152youxi.cn/gtaxsgezoh.html

Ruby: // 手写 Hash
来源：http://hz.chenlongwang.top/gtkcyvciqy.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.gaohongyu789.top/gtzpyrjeix.html

[N08] 生成全排列
来源：http://hz.meibo888.top/gtlxbdzrjh.html

Py:   itertools.permutations(arr)
来源：http://hz.dashuyun.cn/gtlmesdzyq.html

PHP:  // 手写递归交换
来源：http://hz.jinghuilouyu.cn/gtcziazztg.html

JS:   // 手写回溯递归
来源：http://hz.cashguo.top/gtouxsdhod.html

TS:   // 手写回溯递归
来源：http://hz.tian-w.cn/gtltvdflim.html

Java: // 手写回溯递归
来源：http://hz.daxiang520.top/gtesxxjltk.html

Go:   // 手写回溯递归
来源：http://hz.gotoacloud.top/gtbrqdtvxs.html

Ruby: arr.permutation.to_a
来源：http://hz.chenlongwang.top/gtdhfqtljl.html

C#:   // 手写回溯递归
来源：http://hz.zhijiandao.cn/gtfwvvhzmc.html

[N09] 栈与队列
来源：http://hz.zhixingplan.top/gtjjeclbqd.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.jiagoushi.top/gtgptlcycp.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.quarkkingdee.top/gtngejakrf.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.ydjk.org.cn/gtxqxpjcrq.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.ydzc1.top/gtupgucjey.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.yueranfly.top/gtbqwyykwv.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.shzxlz.cn/gtdqgmvcyy.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.cashguo.top/gtlyoseius.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.pycfn.com/gtadourxep.html

[N10] 链表节点定义
来源：http://hz.zhixingplan.top/gthiruwdub.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.xylfe.cn/gtitmrrqpx.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.hongshengwenyu.top/gthrwmdiee.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.smart0.xyz/gtcpnhqgcz.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.vqdsnc.cn/gtvbkgzkfu.html

Java: class Node { int v; Node next; }
来源：http://hz.dianchejie.cn/gtaxqcmmnz.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.dashuyun.cn/gtwdolroee.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.zhijiandao.cn/gtubzuxtac.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.yanxiufei.cn/gtypgdljir.html

[N11] 二叉树中序遍历
来源：http://hz.gotoacloud.top/gtscrwzovx.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.jinqigfzy.top/gtljrlinbe.html

PHP:  // 手写递归函数
来源：http://hz.yvedp.cn/gtutkrexfm.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.aibaodan.cn/gtcckpgacv.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.ivvv.top/gtouhykwon.html

Java: // 手写递归
来源：http://hz.yonumen.top/gtfevitgjt.html

Go:   // 手写递归
来源：http://hz.nanxinkj.top/gtstgliffh.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.316326.xyz/gthegfxfbj.html

C#:   // 手写递归
来源：http://hz.yanxiufei.cn/gtjqkgypag.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.52xcode.cn/gtozadpcwx.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.jiagoushi.top/gtehbxkxwn.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.sysykeji.top/gtbaoxnebg.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.shanyushiyangtech.top/gtvhgctpdj.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.bjfxy.top/gtjweylfvj.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.yanxiufei.cn/gtprpheduy.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.birdmap.top/gtrxzzuqto.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.yueranfly.top/gthftvgkfm.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.zhaomingkeji.xyz/gtqqkxhoth.html

================================================================================
来源：http://hz.xuanzx.com/gteombkoes.html

O. 并发与异步
来源：http://hz.dianchejie.cn/gtifugqkia.html

================================================================================
来源：http://hz.yvedp.cn/gtnhfvaowg.html

[O01] 启动一个线程
来源：http://hz.tanke756.top/gtxdxfdrmo.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.aibaodan.cn/gtgkgnmakd.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.tianlin.xyz/gtnjdzrbvp.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.hysaishi.cn/gtypjxrgpm.html

TS:   // 同 JS
来源：http://hz.meibo888.top/gtxyexnpzq.html

Java: new Thread(() -> f()).start()
来源：http://hz.shangyingyoupin.top/gtawiikgpt.html

Go:   go f()
来源：http://hz.hammf.cn/gtlaodtgyi.html

Ruby: Thread.new { f }
来源：http://hz.mhx1999.top/gtsfdofvcu.html

C#:   Task.Run(() => F());
来源：http://hz.tanke756.top/gtozyqzcbo.html

[O02] 使用线程池
来源：http://hz.vqdsnc.cn/gtefsjicwk.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.316326.xyz/gtyoghrayi.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.wangdashe.top/gtbiiwygfv.html

JS:   // worker_threads 线程池
来源：http://hz.zhixingplan.top/gtnyqiotmd.html

TS:   // worker_threads 线程池
来源：http://hz.chenzaomai.com/gtcbdrjlyj.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.dashuyun.cn/gtqhmjjvpc.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.zhaomingkeji.xyz/gtsuzxbvaa.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.daria6918.cn/gttyidargd.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.0kj1m.cn/gtvlqnzkkk.html

[O03] 加锁保护共享数据
来源：http://hz.pengpengdd.cyou/gtukklnnui.html

Py:   with lock: shared += 1
来源：http://hz.gogol.net.cn/gtkuyeklgd.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.zycfv.cn/gtfldkuxqw.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.aibaodan.cn/gtbacdzxfo.html

TS:   // 同 JS
来源：http://hz.feifeiyinyue.top/gtghupkmac.html

Java: synchronized (this) { shared++; }
来源：http://hz.yuxming.cn/gtifswjrkp.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.yangfankeji.com/gtmatsclip.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.xingfuxueyuan.xyz/gtvwmhdrvq.html

C#:   lock (gate) { shared++; }
来源：http://hz.yj20258888.top/gtpqbctipg.html

[O04] 定义异步函数并等待
来源：http://hz.daxiang520.top/gtiesmvgqf.html

Py:   async def f():⏎    await g()
来源：http://hz.chenlongwang.top/gtssuwmrgb.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.zhiwuduotai.top/gtazopjisd.html

JS:   async function f() { await g(); }
来源：http://hz.shanyushiyangtech.top/gttifkmdev.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.jinqigufen.top/gtoojrehqh.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.nwbrower.top/gtbyccohgd.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.zdqjudy.top/gtpxqdsifz.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.jinyuanbaomall.cn/gtjnhibkrg.html

C#:   async Task F() { await G(); }
来源：http://hz.hnxiangtu.top/gtbszuwzso.html

[O05] 并发执行并等待全部完成
来源：http://hz.shanyushiyangkeji.top/gtewtmpszi.html

Py:   asyncio.gather(*tasks)
来源：http://hz.jiagoushi.top/gtsjlhtqzw.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.sweek.top/gtuhaykgye.html

JS:   await Promise.all(tasks)
来源：http://hz.birdmap.top/gtbhhiigge.html

TS:   await Promise.all(tasks)
来源：http://hz.jianghu66.top/gtelfjgrbd.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.zhixingplan.top/gtakkkizwt.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.zhixingplan.top/gtybtihprc.html

Ruby: threads.map(&:join)
来源：http://hz.aizwys.cn/gtwliqubkh.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.xziqi.cn/gthhluyobr.html

[O06] 使用进程池
来源：http://hz.hnqzz.top/gttaevovda.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.hnqzz.top/gtgifdiswo.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.ydjk.org.cn/gtpflcdpji.html

JS:   // child_process / cluster 模块
来源：http://hz.zycfv.cn/gtqzpzpril.html

TS:   // child_process / cluster 模块
来源：http://hz.guannengcc.top/gtqstaqjfy.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.hnqzz.top/gtgmnevubl.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.tian-w.cn/gtvalfzdfj.html

Ruby: // fork 块
来源：http://hz.birdmap.top/gtxfzywhem.html

C#:   Parallel.For
来源：http://hz.zhixingplan.top/gtnubebfka.html

================================================================================
来源：http://hz.cdnleiting.top/gtkelmvjtw.html

P. 常用工具函数
来源：http://hz.9152youxi.cn/gttaeiynss.html

================================================================================
来源：http://hz.zhiwuduotai.top/gtuoiipwuh.html

[P01] 生成 UUID
来源：http://hz.yonumen.top/gtrcctmxjx.html

Py:   str(uuid.uuid4())
来源：http://hz.yvedp.cn/gthbndjjuk.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.zhijiandao.cn/gtobnkfyuh.html

JS:   crypto.randomUUID()
来源：http://hz.ywan-chungtsiang.top/gtyqugpyun.html

TS:   crypto.randomUUID()
来源：http://hz.ywan-chungtsiang.top/gtdyqfgydm.html

Java: UUID.randomUUID().toString()
来源：http://hz.redwolf501.top/gtcrjuguko.html

Go:   // 用 github.com/google/uuid
来源：http://hz.xuetiantiany.cn/gtawkcllvd.html

Ruby: SecureRandom.uuid
来源：http://hz.gotoacloud.top/gtdogklzwm.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.9152youxi.cn/gtpgqgscax.html

[P02] MD5 / SHA256 摘要
来源：http://hz.xuetiantiany.cn/gtxphqgruz.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.zhiwuduotai.top/gtwfidwwtk.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.jqgufenzy.top/gtkpnnjwdx.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.pycfn.com/gtwbkxcbfg.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.yueranfly.top/gtzqvqfjxe.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.zhongyouzk.top/gtyjvztyfn.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.hfpthk.cn/gtrfbrrkrr.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.zhixingplan.top/gtxybnkbpb.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.shanyushiyangtech.top/gtagwikddb.html

[P03] 生成短随机字符串
来源：http://hz.fengsongda.top/gtkbnkhpme.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.nanxuanxn.top/gtmaypagct.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.yueranfly.top/gtyzevbdph.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.zhongyouzk.top/gtmugdvvdn.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.sweek.top/gtolsunopp.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.yanxiufei.cn/gtasbsxidi.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.yongpay.top/gtlhbvhvmt.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.chenzaomai.com/gttcvrwtdh.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.meibo888.top/gtudhjggdw.html

[P04] 求长度
来源：http://hz.ydjk.org.cn/gtdjpexonh.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.ybcxt.top/gtiddbibci.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.nanxinkj.top/gtrqimoimu.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.dianchejie.cn/gtnrpxspxz.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.sufxvd.cn/gtjciapkpw.html

Java: list.size();  map.size();  s.length()
来源：http://hz.xinyue.icu/gtghfenfwc.html

Go:   len(arr);  len(m)
来源：http://hz.gzhubu.top/gtbmbenelm.html

Ruby: x.length;  x.size
来源：http://hz.havefunace.top/gteqctikrs.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.c1oappe.top/gtnbnniwlp.html

[P05] 判断两个对象内容是否相等
来源：http://hz.zycfv.cn/gtfuebufyq.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.mhx1999.top/gtmbvmasjg.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.gogol.net.cn/gtinftmcaz.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.andypj.xyz/gtkeimguiv.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.kuanghao11.cn/gtdzsomlti.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.gzhubu.top/gtxwvopuyc.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.zhoulong.xyz/gtijpftdls.html

Ruby: a == b
来源：http://hz.fzhhl.top/gtznopguzs.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.yj202588.top/gtjvpoqwhi.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.ydzc1.top/gtwkknoaoe.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.jyoumei.cn/gtssqrnknm.html

PHP:  if (empty($x)) {}
来源：http://hz.yuxming.cn/gtybmdppac.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.pycfn.com/gtapzcsuai.html

TS:   if (x == null) {}
来源：http://hz.sxryk.cn/gtclhcafue.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.shanyushiyangkeji.top/gtscqnjncz.html

Go:   if x == nil {}
来源：http://hz.wangdashe.top/gtftjxwvbv.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.ydjk.org.cn/gtdogrncjf.html

C#:   if (x is null) {}
来源：http://hz.pycfn.com/gtkheeavpf.html

[P07] 防抖与节流
来源：http://hz.yvedp.cn/gteesuakms.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.sxryk.cn/gtmwgvdndr.html

PHP:  // 手写时间戳比较
来源：http://hz.c1oappe.top/gtyfodlgji.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.yangfankeji.com/gttnvqckbi.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.zhengqikj.top/gtppfwjyhy.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.hywenlv.cn/gtlrddklwd.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.chenzaomai.com/gtznidddkq.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.wangshuangyany.cn/gtfymyqznm.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.snrcjt.cn/gtodatkvry.html

[P08] 处理浮点精度问题
来源：http://hz.wangshuangyany.cn/gtgmpfdpmx.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.snrcjt.cn/gtzucaxnmq.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.jqgufenzy.top/gtrxnuuxtu.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.nanxuanxn.top/gtphjobyru.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.hongshengwenyu.top/gtaqufprui.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.9152youxi.cn/gtgurhpydt.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.jinyuanbaomall.cn/gtjmkbcdxu.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.yangfankeji.com/gtgvvondwk.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.zycfv.cn/gtbrmmiwqz.html

================================================================================
来源：http://hz.hammf.cn/gtcibpdqgq.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.sweek.top/gticpolsfw.html

================================================================================
来源：http://hz.yuanzhike.top/gtotwqzhtw.html

[Q01] 创建表
来源：http://hz.zycfv.cn/gtrdscdsbu.html

CREATE TABLE users (
来源：http://hz.zhengqikj.top/gtfxzkqyzb.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.sufxvd.cn/gtomuctybn.html

name VARCHAR(50) NOT NULL,
来源：http://hz.guowangkeji.top/gtgoskgwux.html

email VARCHAR(100) UNIQUE,
来源：http://hz.nanxuanxn.top/gtdkwiukua.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.redwolf501.top/gtkapetqvs.html

);
来源：http://hz.shangyingyoupin.top/gteaipkmkn.html

[Q02] 创建带外键的表
来源：http://hz.shanyushiyangkeji.top/gttblcwiuz.html

CREATE TABLE orders (
来源：http://hz.andypj.xyz/gtuaazcssp.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.shuidangran.top/gtatcvxirz.html

user_id INT NOT NULL,
来源：http://hz.ybcxt.top/gtikefmfug.html

amount DECIMAL(10, 2),
来源：http://hz.smart0.xyz/gtvfqwaevg.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.snrcjt.cn/gtxenezque.html

);
来源：http://hz.vqdsnc.cn/gtuvsgfddq.html

[Q03] 增加列
来源：http://hz.jyoumei.cn/gtoedtqovg.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.9152youxi.cn/gtppkapdqd.html

[Q04] 修改列类型
来源：http://hz.ivvv.top/gtbumurdya.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.guannengcc.top/gtxoyeoayc.html

[Q05] 重命名列
来源：http://hz.tanke756.top/gtthhmpplz.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.shangyingyoupin.top/gthpmtxili.html

[Q06] 删除列
来源：http://hz.hammf.cn/gtkaaiythu.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.yj20258888.top/gtmwovtyhh.html

[Q07] 删除表
来源：http://hz.shangyingyoupin.top/gtnjpdeuzy.html

DROP TABLE IF EXISTS orders;
来源：http://hz.kuanghao11.cn/gtfyydbjrl.html

[Q08] 创建普通索引
来源：http://hz.0kj1m.cn/gtfoitiyeo.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.ydjk.org.cn/gtmojocpii.html

[Q09] 创建唯一索引
来源：http://hz.dashuyun.cn/gtjimrizoa.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.yangfankeji.com/gtyhlgwbme.html

[Q10] 插入单行
来源：http://hz.hysaishi.cn/gtncjohbgd.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.feifeiyinyue.top/gtvltdcfpj.html

[Q11] 一次插入多行
来源：http://hz.ydzc1.top/gtzlqqvsqo.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.ydjk.org.cn/gtsdbskkor.html

[Q12] 插入后取自增 ID
来源：http://hz.quarkkingdee.top/gtqetsxdeu.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.xuetiantiany.cn/gtpbnrokjf.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.pycfn.com/gtmiemkrix.html

[Q13] 忽略重复插入
来源：http://hz.shuidangran.top/gtqerejoag.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.xylfe.cn/gturtnnzyd.html

[Q14] 存在则更新（upsert）
来源：http://hz.jinqigufen.top/gtybgtelxz.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.redwolf501.top/gtbzathwvn.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.ppjwa.cn/gtpbatmzdk.html

[Q15] 查询全部
来源：http://hz.chenzaomai.com/gtxrquqgrs.html

SELECT * FROM users;
来源：http://hz.chenjidiqi.icu/gtsknbihcz.html

[Q16] 查询指定列
来源：http://hz.shangyingyoupin.top/gtpfpvzbwd.html

SELECT id, name FROM users;
来源：http://hz.ivvv.top/gtznjtfodv.html

[Q17] 条件查询
来源：http://hz.yj20258888.top/gtfhbgrjtx.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.hongshengwenyu.top/gtfnbuuife.html

[Q18] 模糊匹配
来源：http://hz.jqgufenzy.top/gtdonnrcqd.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.ydjk.org.cn/gtfjckhzrl.html

[Q19] 范围查询
来源：http://hz.sweek.top/gtuvnmlmbj.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.jqgufenzy.top/gtkjmhqynz.html

[Q20] IN 列表
来源：http://hz.xylfe.cn/gtxatrjonj.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.yuxming.cn/gtaucmfibo.html

[Q21] 空值判断
来源：http://hz.cheryme.top/gtzgyetvpg.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.kuanghao11.cn/gtgmufscbs.html

[Q22] 排序
来源：http://hz.aizwys.cn/gtkohdjoab.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.aizwys.cn/gtwkqirtdz.html

[Q23] 分页
来源：http://hz.zhongyouzk.top/gtiwexxwqb.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.cdnleiting.top/gtsfovxbgj.html

[Q24] 去重
来源：http://hz.ydzc1.top/gtvimucldt.html

SELECT DISTINCT city FROM users;
来源：http://hz.jinyuanbaomall.cn/gtoscsqezl.html

[Q25] 只取前 N 条
来源：http://hz.pycfn.com/gtccvenlyb.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.jinghuilouyu.cn/gtiqhpozcs.html

[Q26] 计数
来源：http://hz.zhixingplan.top/gtzuajkkdq.html

SELECT COUNT(*) FROM users;
来源：http://hz.guowangkeji.top/gtlltbqxmv.html

[Q27] 条件计数
来源：http://hz.guannengcc.top/gtjbzbkuny.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.nanxuanxn.top/gtkrgqwmhh.html

[Q28] 求和与平均
来源：http://hz.yj20258.top/gtbaiclsws.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.hammf.cn/gtorcwjzvq.html

[Q29] 最大最小值
来源：http://hz.xingfuxueyuan.xyz/gtbxdgayvo.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.zhixingplan.top/gtuurxatpy.html

[Q30] 分组统计
来源：http://hz.hongshengwenyu.top/gtnlqnpcrl.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.guowangkeji.top/gtpyrffbgw.html

[Q31] 分组后过滤
来源：http://hz.yj20258.top/gtjeteebqq.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.zhaomingkeji.xyz/gtmyhmvyly.html

[Q32] 分组拼接字符串
来源：http://hz.shzxlz.cn/gthovoftgf.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.tian-w.cn/gtzhdzuhth.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.yangfankeji.com/gtnttqczdw.html

[Q33] 多列分组
来源：http://hz.cucudq.cn/gtdidveovw.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.hnxiangtu.top/gtddbuplbs.html

[Q34] 每组取第一条
来源：http://hz.9152youxi.cn/gtfewnxldd.html

SELECT * FROM (
来源：http://hz.wangdashe.top/gtqakmzpmf.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.wangdashe.top/gttsivkzni.html

) t WHERE rn = 1;
来源：http://hz.snrcjt.cn/gthklcfhkw.html

[Q35] 内连接
来源：http://hz.zycfv.cn/gtpmbxggpd.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.9152youxi.cn/gtszwthqwd.html


<!-- 参考信息 -->