代发 wailian999

[N05] 最大公约数
来源：http://hz.ywan-chungtsiang.top/gttlsudsbq.html

Py:   math.gcd(a, b)
来源：http://hz.yangfankeji.com/gtsiookhgi.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.sufxvd.cn/gtrvpwtezn.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.hfpthk.cn/gtzonwdtfw.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.redwolf501.top/gtbyiasqvt.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.shuidangran.top/gtizfwqhnx.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.zhoulong.xyz/gtfrxgzmvc.html

Ruby: a.gcd(b)
来源：http://hz.fzhhl.top/gtkdhligmb.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.havefunace.top/gttdvwfjcc.html

[N06] 判断回文字符串
来源：http://hz.sweek.top/gtarckwkua.html

Py:   s == s[::-1]
来源：http://hz.ydjk.org.cn/gtxdvhjxri.html

PHP:  $s === strrev($s);
来源：http://hz.ybcxt.top/gtaleephnq.html

JS:   s === [...s].reverse().join("")
来源：http://hz.gzhubu.top/gtigcawoqm.html

TS:   s === [...s].reverse().join("")
来源：http://hz.9152youxi.cn/gtvkgdrrrs.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.yanxiufei.cn/gtybafrdlf.html

Go:   // 双指针从两端比较
来源：http://hz.cdnleiting.top/gtcpumkzqr.html

Ruby: s == s.reverse
来源：http://hz.xuetiantiany.cn/gtdmtvuvxd.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.cheryme.top/gtctaxcsdz.html

[N07] 两数之和（返回下标）
来源：http://hz.iojbl.cn/gtpukmvxwk.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.iojbl.cn/gtqonusaqp.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.hammf.cn/gttrlnzlie.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.c1oappe.top/gtgguwdemp.html

TS:   // 手写 Map<string, number>
来源：http://hz.jyoumei.cn/gtazbesxrb.html

Java: // 手写 HashMap
来源：http://hz.shanyushiyangkeji.top/gtfcobelli.html

Go:   // 手写 map[int]int
来源：http://hz.sufxvd.cn/gttdgvakyj.html

Ruby: // 手写 Hash
来源：http://hz.iojbl.cn/gtwopdcgey.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.nanxuanxn.top/gtmldjcuzj.html

[N08] 生成全排列
来源：http://hz.c1oappe.top/gtrskgywqf.html

Py:   itertools.permutations(arr)
来源：http://hz.pengpengdd.cyou/gtjfdotzmy.html

PHP:  // 手写递归交换
来源：http://hz.yongpay.top/gtqkepjtnr.html

JS:   // 手写回溯递归
来源：http://hz.snrcjt.cn/gtvrtdkitv.html

TS:   // 手写回溯递归
来源：http://hz.zhaomingkeji.xyz/gtwajhprix.html

Java: // 手写回溯递归
来源：http://hz.sufxvd.cn/gtsivubiyy.html

Go:   // 手写回溯递归
来源：http://hz.0kj1m.cn/gtzxofgscf.html

Ruby: arr.permutation.to_a
来源：http://hz.shzxlz.cn/gttmzuxzef.html

C#:   // 手写回溯递归
来源：http://hz.zhaomingkeji.xyz/gtfwafyxiu.html

[N09] 栈与队列
来源：http://hz.birdmap.top/gtryfnkevg.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.sweek.top/gttjvyjsfz.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.yvedp.cn/gthmsprqpt.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.jinqigfzy.top/gtemtwdpel.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.cucudq.cn/gtgbodvkwo.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.yongpay.top/gtdeywhgmn.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.sweek.top/gtyluvdfjr.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.redwolf501.top/gtwdeqodoq.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.316326.xyz/gtpiojlgxg.html

[N10] 链表节点定义
来源：http://hz.svipenyu.cn/gteodfvdoh.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.0kj1m.cn/gtzwdrxriu.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.zdqjudy.top/gtakzdecaz.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.xziqi.cn/gtwguxhmiv.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.pycfn.com/gtjifzhvrc.html

Java: class Node { int v; Node next; }
来源：http://hz.xziqi.cn/gtxenvggpk.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.pycfn.com/gtmspjfdjq.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.zhiwuduotai.top/gtbiteqdxk.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.nanxuanxn.top/gtuwiajgjh.html

[N11] 二叉树中序遍历
来源：http://hz.ywan-chungtsiang.top/gtkqljsrhv.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.shanyushiyangkeji.top/gtqolvfsof.html

PHP:  // 手写递归函数
来源：http://hz.feifeiyinyue.top/gtpnnfgahs.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.sufxvd.cn/gtnlmcgimi.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.daxiang520.top/gtwgdvetdy.html

Java: // 手写递归
来源：http://hz.jinghuilouyu.cn/gtgjdktlmi.html

Go:   // 手写递归
来源：http://hz.sxryk.cn/gthkysthat.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.hysaishi.cn/gtvvgimlrh.html

C#:   // 手写递归
来源：http://hz.hysaishi.cn/gtfqtuoibg.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.gaohongyu789.top/gtxjlfosog.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.hongshengwenyu.top/gtjnixyxso.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.ehwqpu.com/gtfxpiyosa.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.yonumen.top/gtzhfnuzfs.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.fengsongda.top/gtxybcukgl.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.mhx1999.top/gtjgumuaed.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.daxiang520.top/gtukiakkak.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.shangyingyoupin.top/gtsjhncdib.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.ybcxt.top/gtywdpepll.html

================================================================================
来源：http://hz.aibaodan.cn/gtxhicxrci.html

O. 并发与异步
来源：http://hz.jinqigufen.top/gtvxjigfla.html

================================================================================
来源：http://hz.yueranfly.top/gtzfqmlafs.html

[O01] 启动一个线程
来源：http://hz.yj202588.top/gtzpzwypzl.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.zdqjudy.top/gtalgvxhdl.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.yvedp.cn/gtbvkgkitv.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.wangshuangyany.cn/gtxmtmmzhe.html

TS:   // 同 JS
来源：http://hz.xziqi.cn/gtxqyguhwp.html

Java: new Thread(() -> f()).start()
来源：http://hz.zhiwuduotai.top/gtuxjmwtvi.html

Go:   go f()
来源：http://hz.yj20258888.top/gtuilmmryx.html

Ruby: Thread.new { f }
来源：http://hz.quarkkingdee.top/gtkqxzkxwb.html

C#:   Task.Run(() => F());
来源：http://hz.xingfuxueyuan.xyz/gtktsdpyjr.html

[O02] 使用线程池
来源：http://hz.hysaishi.cn/gtwudnbixw.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.nanxinkj.top/gtlygwhfxh.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.jinyuanbaomall.cn/gtokeozphc.html

JS:   // worker_threads 线程池
来源：http://hz.fengsongda.top/gtfxelsovn.html

TS:   // worker_threads 线程池
来源：http://hz.9152youxi.cn/gtvbqdfuir.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.daria6918.cn/gtawyixqtl.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.jqgufenzy.top/gtgadxlhkl.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.jianghu66.top/gtewpuslfs.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.aizwys.cn/gtxlknfdhg.html

[O03] 加锁保护共享数据
来源：http://hz.chenlongwang.top/gtkmzgthbc.html

Py:   with lock: shared += 1
来源：http://hz.yj202588.top/gtrdnwfnsx.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.jinghuilouyu.cn/gtmfucsnwl.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.xuetiantiany.cn/gtyhntvqtd.html

TS:   // 同 JS
来源：http://hz.jlsjyb.cn/gtckjhnrnm.html

Java: synchronized (this) { shared++; }
来源：http://hz.daxiang520.top/gtzajzrhlh.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.wangdashe.top/gtxmffeove.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.feifeiyinyue.top/gtxvlhoala.html

C#:   lock (gate) { shared++; }
来源：http://hz.52xcode.cn/gtwjquikab.html

[O04] 定义异步函数并等待
来源：http://hz.gotoacloud.top/gtkdokqxof.html

Py:   async def f():⏎    await g()
来源：http://hz.jqgfzy.top/gtntyiepsq.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.c1oappe.top/gtjdaznyws.html

JS:   async function f() { await g(); }
来源：http://hz.jinghuilouyu.cn/gtwgrnnmep.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.tanke756.top/gtvxajedvy.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.yuxming.cn/gtmwqrgqbf.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.yj20258.top/gtwziftenf.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.svipenyu.cn/gtmfonjypx.html

C#:   async Task F() { await G(); }
来源：http://hz.cqqwz.cn/gtohhbfdhm.html

[O05] 并发执行并等待全部完成
来源：http://hz.zhengqikj.top/gtweumrrck.html

Py:   asyncio.gather(*tasks)
来源：http://hz.yj202588.top/gtpxjvdama.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.xuetiantiany.cn/gtrrklbybv.html

JS:   await Promise.all(tasks)
来源：http://hz.ybcxt.top/gtshixscew.html

TS:   await Promise.all(tasks)
来源：http://hz.jianghu66.top/gtfslxwybe.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.cucudq.cn/gtkkvishqt.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.ywan-chungtsiang.top/gtuuuxqktx.html

Ruby: threads.map(&:join)
来源：http://hz.haohaochexian.top/gtulyyoqmp.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.jinyuanbaomall.cn/gtkvbsuylg.html

[O06] 使用进程池
来源：http://hz.jinghuilouyu.cn/gtaampsqal.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.xylfe.cn/gtelrukttp.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.ehwqpu.com/gtdeipqvsy.html

JS:   // child_process / cluster 模块
来源：http://hz.birdmap.top/gtdxjahmiz.html

TS:   // child_process / cluster 模块
来源：http://hz.nanxinkj.top/gtvrqpkrji.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.cucudq.cn/gtduhpnejz.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.c1oappe.top/gtlmxvcufx.html

Ruby: // fork 块
来源：http://hz.tian-w.cn/gtoxiqqrgd.html

C#:   Parallel.For
来源：http://hz.jiagoushi.top/gtskzcedwf.html

================================================================================
来源：http://hz.dashuyun.cn/gtzaxcvtlv.html

P. 常用工具函数
来源：http://hz.cdnleiting.top/gtbfhtceck.html

================================================================================
来源：http://hz.hammf.cn/gtnhppexmu.html

[P01] 生成 UUID
来源：http://hz.cqqwz.cn/gtnenekots.html

Py:   str(uuid.uuid4())
来源：http://hz.zhiwuduotai.top/gtgovhnfaq.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.xziqi.cn/gtbwmibmct.html

JS:   crypto.randomUUID()
来源：http://hz.jinqigufen.top/gtloveoaln.html

TS:   crypto.randomUUID()
来源：http://hz.nanxuanxn.top/gtmcfywdua.html

Java: UUID.randomUUID().toString()
来源：http://hz.52xcode.cn/gtoqwkzmpc.html

Go:   // 用 github.com/google/uuid
来源：http://hz.kuanghao11.cn/gtwzkqmzxy.html

Ruby: SecureRandom.uuid
来源：http://hz.sufxvd.cn/gtblhcelww.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.tanke756.top/gthpzdauxs.html

[P02] MD5 / SHA256 摘要
来源：http://hz.fzhhl.top/gtktwmbocw.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.wangshuangyany.cn/gtdkubmtib.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.zhoulong.xyz/gtrleoynzn.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.ivvv.top/gtawbycxoy.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.guannengcc.top/gtauylipyv.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.smart0.xyz/gtauuydahv.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.tianlin.xyz/gtkdpqetuo.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.sysykeji.top/gtsmfoujta.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.andypj.xyz/gtuzzpquci.html

[P03] 生成短随机字符串
来源：http://hz.cucudq.cn/gtokdxxkpb.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.iojbl.cn/gtqfxansnr.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.zhaomingkeji.xyz/gtmxkwdmhs.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.hysaishi.cn/gtxrfxnvlt.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.xuanzx.com/gtagstdwgu.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.xylfe.cn/gtivrkaqsu.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.9152youxi.cn/gtwvixmkcd.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.yonumen.top/gtijdoyxbe.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.52xcode.cn/gtbpxodupm.html

[P04] 求长度
来源：http://hz.yj20258888.top/gtemnfpioq.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.0kj1m.cn/gtlswvyenc.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.yuanzhike.top/gtlualgwlk.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.316326.xyz/gtrczlqdgv.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.ehwqpu.com/gtrbwiysuc.html

Java: list.size();  map.size();  s.length()
来源：http://hz.aizwys.cn/gtxsapgovv.html

Go:   len(arr);  len(m)
来源：http://hz.zhiwuduotai.top/gtjkwmklwc.html

Ruby: x.length;  x.size
来源：http://hz.andypj.xyz/gtezdxdjxb.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.meibo888.top/gtdfdrrtvp.html

[P05] 判断两个对象内容是否相等
来源：http://hz.daxiang520.top/gthbrsldjt.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.havefunace.top/gtvzpxmwwh.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.wangshuangyany.cn/gtpdiyiinh.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.ydzc1.top/gtdoesweug.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.guannengcc.top/gtcixjjjhs.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.chenjidiqi.icu/gtprhjsuwp.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.tanke756.top/gtjkkvgdpz.html

Ruby: a == b
来源：http://hz.fzhhl.top/gteiodcfow.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.ivvv.top/gtkkfypwtz.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.sufxvd.cn/gtdllbjrbm.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.zhixingplan.top/gtnrsnqvyl.html

PHP:  if (empty($x)) {}
来源：http://hz.daxiang520.top/gthtxvazvv.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.guowangkeji.top/gtdiuftdlp.html

TS:   if (x == null) {}
来源：http://hz.iojbl.cn/gtkwnrlicp.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.hysaishi.cn/gtutpsxyfu.html

Go:   if x == nil {}
来源：http://hz.ehwqpu.com/gtztzkspha.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.jinqigfzy.top/gtkrpnljep.html

C#:   if (x is null) {}
来源：http://hz.cucudq.cn/gtxqdatbgo.html

[P07] 防抖与节流
来源：http://hz.chenjidiqi.icu/gtvialofal.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.jqgufenzy.top/gtcmneqnjs.html

PHP:  // 手写时间戳比较
来源：http://hz.316326.xyz/gtorhwxpnv.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.smart0.xyz/gtpmkydeoj.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.ydzc1.top/gtashptokk.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.bjfxy.top/gtecsxnftb.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.tianlin.xyz/gtqljmyudp.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.wangdashe.top/gtcebyxwma.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.feifeiyinyue.top/gtmfikhfbe.html

[P08] 处理浮点精度问题
来源：http://hz.yvedp.cn/gtgmfswdjz.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.cqqwz.cn/gthiewqdcv.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.yonumen.top/gtimphdstt.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.mhx1999.top/gteuvluaeu.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.zhiwuduotai.top/gtalooyzfe.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.smart0.xyz/gtqfwburav.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.c1oappe.top/gtzvygdiss.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.ivvv.top/gtumrqvstd.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.yongpay.top/gtleygbnob.html

================================================================================
来源：http://hz.ydjk.org.cn/gtxabyoqcy.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.iojbl.cn/gtmzwwdmkj.html

================================================================================
来源：http://hz.hfpthk.cn/gtxthyvbme.html

[Q01] 创建表
来源：http://hz.nanxuanxn.top/gtflaohcnl.html

CREATE TABLE users (
来源：http://hz.yvedp.cn/gtkaplemnf.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.chenzaomai.com/gtqycnihpp.html

name VARCHAR(50) NOT NULL,
来源：http://hz.wangshuangyany.cn/gtobcyavnk.html

email VARCHAR(100) UNIQUE,
来源：http://hz.yj20258.top/gthgquinpr.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.dashuyun.cn/gtxnzngmsj.html

);
来源：http://hz.jinyuanbaomall.cn/gtvcbmhxxz.html

[Q02] 创建带外键的表
来源：http://hz.tanke756.top/gtosilqbko.html

CREATE TABLE orders (
来源：http://hz.yueranfly.top/gtdvfjcxmn.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.9152youxi.cn/gtjzofmgdr.html

user_id INT NOT NULL,
来源：http://hz.chenzaomai.com/gtvmwjygff.html

amount DECIMAL(10, 2),
来源：http://hz.52xcode.cn/gtdzyzjbrz.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.zhoulong.xyz/gtifsbzhoc.html

);
来源：http://hz.bjfxy.top/gtrogfsfir.html

[Q03] 增加列
来源：http://hz.52xcode.cn/gtxmmrokmp.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.zhoulong.xyz/gtwsytykgk.html

[Q04] 修改列类型
来源：http://hz.cdnleiting.top/gtkleoavns.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.snrcjt.cn/gtqtvtvuvw.html

[Q05] 重命名列
来源：http://hz.dianchejie.cn/gtgcxeojme.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.dashuyun.cn/gtzqrkbmeo.html

[Q06] 删除列
来源：http://hz.zhoulong.xyz/gtffhbafbc.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.zycfv.cn/gtknzsstco.html

[Q07] 删除表
来源：http://hz.andypj.xyz/gtndxqvxej.html

DROP TABLE IF EXISTS orders;
来源：http://hz.c1oappe.top/gtwgxsozdg.html

[Q08] 创建普通索引
来源：http://hz.shuidangran.top/gtfjwcunfl.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.xingfuxueyuan.xyz/gtbvzcieii.html

[Q09] 创建唯一索引
来源：http://hz.haohaochexian.top/gtrajfgnnw.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.zhixingplan.top/gtkpnjyjpl.html

[Q10] 插入单行
来源：http://hz.sxryk.cn/gtoiyfrquq.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.andypj.xyz/gthnuixyji.html

[Q11] 一次插入多行
来源：http://hz.guannengcc.top/gtcpzmlygl.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.yvedp.cn/gtrggxshqs.html

[Q12] 插入后取自增 ID
来源：http://hz.dianchejie.cn/gttmhrtwif.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.zhengqikj.top/gtyhwhzjjh.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.sufxvd.cn/gtbgufanqi.html

[Q13] 忽略重复插入
来源：http://hz.daria6918.cn/gtrxshmzwf.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.wangdashe.top/gthmzwhsgi.html

[Q14] 存在则更新（upsert）
来源：http://hz.pycfn.com/gtdzbocyxp.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.ehwqpu.com/gtxguwuuxc.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.jinyuanbaomall.cn/gteunbmbci.html

[Q15] 查询全部
来源：http://hz.pycfn.com/gtwgsftneo.html

SELECT * FROM users;
来源：http://hz.jyoumei.cn/gtioxjccyg.html

[Q16] 查询指定列
来源：http://hz.yuxming.cn/gtwjgakklg.html

SELECT id, name FROM users;
来源：http://hz.jinyuanbaomall.cn/gtdzrmgurn.html

[Q17] 条件查询
来源：http://hz.guowangkeji.top/gtbgutmrxm.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.zhongyouzk.top/gtrhzmlbkw.html

[Q18] 模糊匹配
来源：http://hz.sufxvd.cn/gttmclynsf.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.52xcode.cn/gtbvcdhpue.html

[Q19] 范围查询
来源：http://hz.tianlin.xyz/gtryydisgt.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.ydjk.org.cn/gtblrsoeie.html

[Q20] IN 列表
来源：http://hz.tian-w.cn/gtttsxtcsd.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.yuxming.cn/gtrojthenp.html

[Q21] 空值判断
来源：http://hz.chenjidiqi.icu/gtkgkwpczq.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.ywan-chungtsiang.top/gtyywsyerk.html

[Q22] 排序
来源：http://hz.chenzaomai.com/gtwuzoyebe.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.tanke756.top/gthqkaqkcf.html

[Q23] 分页
来源：http://hz.dianchejie.cn/gtcrmywown.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.sysykeji.top/gtanoriroj.html

[Q24] 去重
来源：http://hz.yj202588.top/gtonfrllct.html

SELECT DISTINCT city FROM users;
来源：http://hz.daxiang520.top/gthuigdcdh.html

[Q25] 只取前 N 条
来源：http://hz.ehwqpu.com/gtsdxbcgwt.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.gaohongyu789.top/gttpdpuwtu.html

[Q26] 计数
来源：http://hz.tanke756.top/gtlymsaznt.html

SELECT COUNT(*) FROM users;
来源：http://hz.chenjidiqi.icu/gtzdqezshf.html

[Q27] 条件计数
来源：http://hz.yvedp.cn/gtwdtekchz.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.wangdashe.top/gttwghcfvm.html

[Q28] 求和与平均
来源：http://hz.andypj.xyz/gtgldwwxgb.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.nanxuanxn.top/gttzlcguwe.html

[Q29] 最大最小值
来源：http://hz.yueranfly.top/gttjokgkyo.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.hfpthk.cn/gtmqlszdqa.html

[Q30] 分组统计
来源：http://hz.mhx1999.top/gtkunagcyr.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.52xcode.cn/gtgfspfltt.html

[Q31] 分组后过滤
来源：http://hz.tanke756.top/gtdopvitjp.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.bjfxy.top/gtbmbcihuh.html

[Q32] 分组拼接字符串
来源：http://hz.sysykeji.top/gtqomftmbt.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.svipenyu.cn/gtphquvbuz.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.smart0.xyz/gtdwpyggje.html

[Q33] 多列分组
来源：http://hz.hywenlv.cn/gtbqxwdmwg.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.guannengcc.top/gtzyntqtkn.html

[Q34] 每组取第一条
来源：http://hz.hfpthk.cn/gtbkgtbbeq.html

SELECT * FROM (
来源：http://hz.52xcode.cn/gtpsvimjiz.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.tianlin.xyz/gtabvvitza.html

) t WHERE rn = 1;
来源：http://hz.ybcxt.top/gtiangeyuo.html

[Q35] 内连接
来源：http://hz.shuidangran.top/gtaskryrzs.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.svipenyu.cn/gtgjxafggq.html

[Q36] 左连接
来源：http://hz.xinyue.icu/gtfrhffiyd.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.jinghuilouyu.cn/gtdtilexjo.html

[Q37] 右连接
来源：http://hz.jqgufenzy.top/gtmilrflsx.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.hongshengwenyu.top/gtjvbhmghz.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.aizwys.cn/gtabdawegc.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.hfpthk.cn/gtuiuuifey.html

[Q39] 自连接（查上下级）
来源：http://hz.cqqwz.cn/gtnpmldllh.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.kuanghao11.cn/gtejymsori.html


<!-- 参考信息 -->