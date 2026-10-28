代发 wailian999

[N05] 最大公约数
来源：http://hz.guannengcc.top/gtmbopjszv.html

Py:   math.gcd(a, b)
来源：http://hz.shangyingyoupin.top/gtdsvsshkv.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.svipenyu.cn/gtvkgjpozt.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.fengsongda.top/gtgkzgisem.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.jinqigfzy.top/gtddrwnksp.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.tanke756.top/gtkfnfmfqg.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.zhiwuduotai.top/gtffzethgl.html

Ruby: a.gcd(b)
来源：http://hz.aizwys.cn/gtrwnjqokp.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.hnqzz.top/gthwkrjkmm.html

[N06] 判断回文字符串
来源：http://hz.tanke756.top/gtskxpzbta.html

Py:   s == s[::-1]
来源：http://hz.shuidangran.top/gtylixbdqb.html

PHP:  $s === strrev($s);
来源：http://hz.c1oappe.top/gtwyqsshpv.html

JS:   s === [...s].reverse().join("")
来源：http://hz.jinqigufen.top/gtwxpgiffp.html

TS:   s === [...s].reverse().join("")
来源：http://hz.xziqi.cn/gtzvwsxaty.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.daria6918.cn/gtfwrtlpyg.html

Go:   // 双指针从两端比较
来源：http://hz.jlsjyb.cn/gtwpgkrgmc.html

Ruby: s == s.reverse
来源：http://hz.xziqi.cn/gtzrlkyrnv.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.hongshengwenyu.top/gtooysnypa.html

[N07] 两数之和（返回下标）
来源：http://hz.zhixingplan.top/gtytzbnkxz.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.jinqigufen.top/gtheusxmke.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.0kj1m.cn/gthwlnmkxk.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.wangdashe.top/gtnawsvxen.html

TS:   // 手写 Map<string, number>
来源：http://hz.wangshuangyany.cn/gtuwxfkxby.html

Java: // 手写 HashMap
来源：http://hz.snrcjt.cn/gtuvmpxrry.html

Go:   // 手写 map[int]int
来源：http://hz.hnqzz.top/gtgyuyimkc.html

Ruby: // 手写 Hash
来源：http://hz.sysykeji.top/gtezarnjvg.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.zhiwuduotai.top/gtzsiemafe.html

[N08] 生成全排列
来源：http://hz.hnxiangtu.top/gtkqmffhbz.html

Py:   itertools.permutations(arr)
来源：http://hz.yj20258888.top/gtoyfccxsa.html

PHP:  // 手写递归交换
来源：http://hz.sxryk.cn/gthglshgsa.html

JS:   // 手写回溯递归
来源：http://hz.cucudq.cn/gtjtfofccm.html

TS:   // 手写回溯递归
来源：http://hz.hfpthk.cn/gtacdevyff.html

Java: // 手写回溯递归
来源：http://hz.cheryme.top/gtwsdfylzl.html

Go:   // 手写回溯递归
来源：http://hz.yonumen.top/gtqphaudxl.html

Ruby: arr.permutation.to_a
来源：http://hz.jyoumei.cn/gtvskymqiv.html

C#:   // 手写回溯递归
来源：http://hz.c1oappe.top/gtehblcbyd.html

[N09] 栈与队列
来源：http://hz.c1oappe.top/gtvjzdnogd.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.daria6918.cn/gtcnaqakeo.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.daria6918.cn/gtplvydecp.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.yangfankeji.com/gtofebdlxz.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.dashuyun.cn/gtpegzelcc.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.hongshengwenyu.top/gtiircozxr.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.gaohongyu789.top/gtehnoppbs.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.sufxvd.cn/gtyrcnrrro.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.tian-w.cn/gtbmegtyut.html

[N10] 链表节点定义
来源：http://hz.jianghu66.top/gtcfytkyeh.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.haohaochexian.top/gtzjofhhbf.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.yj20258888.top/gteiwyaxtk.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.fzhhl.top/gtvokryauf.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.dashuyun.cn/gtfzypuqax.html

Java: class Node { int v; Node next; }
来源：http://hz.tianlin.xyz/gtqqzgiqhc.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.redwolf501.top/gthhxeivoa.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.xziqi.cn/gtpavufajj.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.jinyuanbaomall.cn/gtpfteiitj.html

[N11] 二叉树中序遍历
来源：http://hz.aibaodan.cn/gtirqhxzse.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.wangshuangyany.cn/gtaoiornyi.html

PHP:  // 手写递归函数
来源：http://hz.nanxinkj.top/gtkrcdcseu.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.nanxuanxn.top/gtcicimyqm.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.hywenlv.cn/gtsofrnxlh.html

Java: // 手写递归
来源：http://hz.cdnleiting.top/gtnqlchaes.html

Go:   // 手写递归
来源：http://hz.yuxming.cn/gtxkmjjbml.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.gaohongyu789.top/gtkleywsif.html

C#:   // 手写递归
来源：http://hz.c1oappe.top/gtnjafddba.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.snrcjt.cn/gtymivmelv.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.jqgfzy.top/gtzkvfelio.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.9152youxi.cn/gtemzsghxu.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.meibo888.top/gtxzzieebr.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.nwbrower.top/gtxcsoijjh.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.ehwqpu.com/gtecmmaiuu.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.zhongyouzk.top/gtfiohthoh.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.guannengcc.top/gtsinyhzrq.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.xingfuxueyuan.xyz/gtxuazwthf.html

================================================================================
来源：http://hz.hfpthk.cn/gtqehymraj.html

O. 并发与异步
来源：http://hz.hnxiangtu.top/gtzoowricd.html

================================================================================
来源：http://hz.bjfxy.top/gtivrywcba.html

[O01] 启动一个线程
来源：http://hz.havefunace.top/gtftvmoqyf.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.zhoulong.xyz/gtvzfxltsb.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.nanxinkj.top/gtllnlfceg.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.52xcode.cn/gtloinpnss.html

TS:   // 同 JS
来源：http://hz.havefunace.top/gtxviinpbs.html

Java: new Thread(() -> f()).start()
来源：http://hz.cdnleiting.top/gtaaqpglzc.html

Go:   go f()
来源：http://hz.9152youxi.cn/gtpoqgyzba.html

Ruby: Thread.new { f }
来源：http://hz.xinyue.icu/gtpvtxlaej.html

C#:   Task.Run(() => F());
来源：http://hz.mhx1999.top/gttehzfrxf.html

[O02] 使用线程池
来源：http://hz.zhijiandao.cn/gtvumgiwzd.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.gotoacloud.top/gtnmxjsxsq.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.quarkkingdee.top/gtuzpijdig.html

JS:   // worker_threads 线程池
来源：http://hz.yuanzhike.top/gtqsqqweud.html

TS:   // worker_threads 线程池
来源：http://hz.zhiwuduotai.top/gtkhdekptc.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.haohaochexian.top/gtxtgyrqpz.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.nanxinkj.top/gtemhaxxgs.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.pengpengdd.cyou/gtgynghavw.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.jqgufenzy.top/gtthwrhamw.html

[O03] 加锁保护共享数据
来源：http://hz.cqqwz.cn/gttwkfpoqz.html

Py:   with lock: shared += 1
来源：http://hz.pengpengdd.cyou/gtwoepkurx.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.shanyushiyangtech.top/gtyluhoyym.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.xingfuxueyuan.xyz/gtahzuikkj.html

TS:   // 同 JS
来源：http://hz.daria6918.cn/gtoqrrhutv.html

Java: synchronized (this) { shared++; }
来源：http://hz.feifeiyinyue.top/gtjphiufsd.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.vqdsnc.cn/gtlncpdxcc.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.dianchejie.cn/gtapwwzfta.html

C#:   lock (gate) { shared++; }
来源：http://hz.gogol.net.cn/gtlnlsiefw.html

[O04] 定义异步函数并等待
来源：http://hz.gzhubu.top/gtlfsrifzm.html

Py:   async def f():⏎    await g()
来源：http://hz.xuanzx.com/gtxjeboqti.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.fengsongda.top/gttgpmrxft.html

JS:   async function f() { await g(); }
来源：http://hz.sxryk.cn/gtzrpxjwma.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.xingfuxueyuan.xyz/gturpxvcgk.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.c1oappe.top/gtoxgfxrjg.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.mhx1999.top/gtlympsqkn.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.yj202588.top/gtyzektspt.html

C#:   async Task F() { await G(); }
来源：http://hz.xuanzx.com/gtunadmtkv.html

[O05] 并发执行并等待全部完成
来源：http://hz.cucudq.cn/gthsutkwfl.html

Py:   asyncio.gather(*tasks)
来源：http://hz.chenjidiqi.icu/gtbcxamder.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.shangyingyoupin.top/gteuyzpwmf.html

JS:   await Promise.all(tasks)
来源：http://hz.jqgfzy.top/gthmftyfdu.html

TS:   await Promise.all(tasks)
来源：http://hz.jianghu66.top/gtslzsalbb.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.shuidangran.top/gtzqwlijgf.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.yonumen.top/gtsaokldkt.html

Ruby: threads.map(&:join)
来源：http://hz.feifeiyinyue.top/gtstmryxyr.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.nanxinkj.top/gtrquuihdy.html

[O06] 使用进程池
来源：http://hz.pengpengdd.cyou/gtzfpthjjr.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.xziqi.cn/gtioyfxltu.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.zhengqikj.top/gtjklzpwtm.html

JS:   // child_process / cluster 模块
来源：http://hz.shzxlz.cn/gtkqohgvgn.html

TS:   // child_process / cluster 模块
来源：http://hz.tian-w.cn/gtkrwwifrf.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.chenzaomai.com/gtndnhygde.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.hnqzz.top/gtdymrbrql.html

Ruby: // fork 块
来源：http://hz.zycfv.cn/gtatozctvg.html

C#:   Parallel.For
来源：http://hz.gzhubu.top/gtvkukvgup.html

================================================================================
来源：http://hz.snrcjt.cn/gtucetowbt.html

P. 常用工具函数
来源：http://hz.sxryk.cn/gtnydrajor.html

================================================================================
来源：http://hz.jinqigufen.top/gtdntajonu.html

[P01] 生成 UUID
来源：http://hz.svipenyu.cn/gtostrpotj.html

Py:   str(uuid.uuid4())
来源：http://hz.yj20258888.top/gtkkcrzvub.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.redwolf501.top/gtxegxkcnw.html

JS:   crypto.randomUUID()
来源：http://hz.guowangkeji.top/gtexjtrcui.html

TS:   crypto.randomUUID()
来源：http://hz.vqdsnc.cn/gtpomoeuuz.html

Java: UUID.randomUUID().toString()
来源：http://hz.ybcxt.top/gtnwpfqhfl.html

Go:   // 用 github.com/google/uuid
来源：http://hz.chenjidiqi.icu/gtykbishoz.html

Ruby: SecureRandom.uuid
来源：http://hz.zhengqikj.top/gtceqeigjf.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.ivvv.top/gtzqpmjule.html

[P02] MD5 / SHA256 摘要
来源：http://hz.yongpay.top/gtnvlqfvgw.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.pycfn.com/gtbgapgpye.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.hnqzz.top/gtdrriwwho.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.yongpay.top/gtckybwsjx.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.hysaishi.cn/gtkvothclz.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.gogol.net.cn/gttyybuwxz.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.dianchejie.cn/gtkzofvubr.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.zycfv.cn/gtukjgsvyu.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.chenlongwang.top/gtytdjsqdk.html

[P03] 生成短随机字符串
来源：http://hz.jinghuilouyu.cn/gtjxcrrnbv.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.ydjk.org.cn/gtwfrgvbwd.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.cqqwz.cn/gtcmxagflj.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.hywenlv.cn/gtfhqxlama.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.jianghu66.top/gtbiampkze.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.hongshengwenyu.top/gtiymtolml.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.zhaomingkeji.xyz/gtnzxlkfrc.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.jlsjyb.cn/gtjzucgxub.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.feifeiyinyue.top/gtldushfvl.html

[P04] 求长度
来源：http://hz.yuxming.cn/gtuqqsbkqg.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.316326.xyz/gtonsvmbtw.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.chenlongwang.top/gtjsflnnhu.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.yj20258888.top/gtnmzqwwas.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.jyoumei.cn/gtiruqnszf.html

Java: list.size();  map.size();  s.length()
来源：http://hz.ybcxt.top/gtafujiavp.html

Go:   len(arr);  len(m)
来源：http://hz.fzhhl.top/gtalghhfmx.html

Ruby: x.length;  x.size
来源：http://hz.cashguo.top/gtnpytanah.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.gaohongyu789.top/gtwchjtfok.html

[P05] 判断两个对象内容是否相等
来源：http://hz.cdnleiting.top/gtewpfwqmv.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.dianchejie.cn/gtannpmzyd.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.chenzaomai.com/gtswvtkzpw.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.shanyushiyangkeji.top/gtsendrtil.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.nanxuanxn.top/gtrzcwwind.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.xylfe.cn/gtltjjslfz.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.pengpengdd.cyou/gtqtgfocvb.html

Ruby: a == b
来源：http://hz.cucudq.cn/gtktpdefyd.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.tian-w.cn/gtinmyafjj.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.gzhubu.top/gtphwlscwz.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.wangshuangyany.cn/gtsnejaoii.html

PHP:  if (empty($x)) {}
来源：http://hz.tian-w.cn/gteybcefhs.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.zycfv.cn/gtawvlqxzc.html

TS:   if (x == null) {}
来源：http://hz.yongpay.top/gtaumfvmhb.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.tanke756.top/gtcesmspyd.html

Go:   if x == nil {}
来源：http://hz.snrcjt.cn/gtcbzdtjgv.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.hongshengwenyu.top/gtzqnpiiod.html

C#:   if (x is null) {}
来源：http://hz.jlsjyb.cn/gtmgavkfol.html

[P07] 防抖与节流
来源：http://hz.daxiang520.top/gtqbzxuafj.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.mhx1999.top/gtzguskuia.html

PHP:  // 手写时间戳比较
来源：http://hz.ydjk.org.cn/gtrnerzfee.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.ydzc1.top/gteikeqoxf.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.zdqjudy.top/gtquoonrlr.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.jqgufenzy.top/gtyyacuyuz.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.yanxiufei.cn/gtoxgddftu.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.jinqigfzy.top/gtshriwstg.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.daria6918.cn/gttnhcdsct.html

[P08] 处理浮点精度问题
来源：http://hz.fengsongda.top/gtkzwimotg.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.nanxuanxn.top/gtauuercsm.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.yongpay.top/gtncaaylgc.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.zhongyouzk.top/gtizmqybdf.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.vqdsnc.cn/gteoeforyw.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.52xcode.cn/gtnjzwidfn.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.gotoacloud.top/gtdaovpkea.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.guannengcc.top/gteyhtvoxm.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.9152youxi.cn/gtdwqkrkwe.html

================================================================================
来源：http://hz.gotoacloud.top/gtnfqavnvk.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.shzxlz.cn/gtocwvrkvq.html

================================================================================
来源：http://hz.shuidangran.top/gtfmvayngi.html

[Q01] 创建表
来源：http://hz.gotoacloud.top/gtpwoxuwct.html

CREATE TABLE users (
来源：http://hz.birdmap.top/gtnwznkvvk.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.snrcjt.cn/gtywvvbiaf.html

name VARCHAR(50) NOT NULL,
来源：http://hz.shzxlz.cn/gtiubymxpo.html

email VARCHAR(100) UNIQUE,
来源：http://hz.0kj1m.cn/gtluwzxzkc.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.cdnleiting.top/gtwsmmizgw.html

);
来源：http://hz.xinyue.icu/gtakytkpjx.html

[Q02] 创建带外键的表
来源：http://hz.jlsjyb.cn/gtkykbwiom.html

CREATE TABLE orders (
来源：http://hz.yuxming.cn/gtxfajtzds.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.havefunace.top/gttxhymvnz.html

user_id INT NOT NULL,
来源：http://hz.jqgfzy.top/gtgfdbwhze.html

amount DECIMAL(10, 2),
来源：http://hz.jlsjyb.cn/gtbympkpxg.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.jinghuilouyu.cn/gtezzcpemq.html

);
来源：http://hz.daria6918.cn/gtebxlggtm.html

[Q03] 增加列
来源：http://hz.zhijiandao.cn/gtcqizbwgn.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.fengsongda.top/gtcwdnasou.html

[Q04] 修改列类型
来源：http://hz.yj20258.top/gtvrnwxbxj.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.hongshengwenyu.top/gtuuirhlxs.html

[Q05] 重命名列
来源：http://hz.yuanzhike.top/gtushhbqmn.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.jyoumei.cn/gtbnuolghu.html

[Q06] 删除列
来源：http://hz.kuanghao11.cn/gttmikpgle.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.xuanzx.com/gtfqiqilnw.html

[Q07] 删除表
来源：http://hz.xuanzx.com/gtdehthhmz.html

DROP TABLE IF EXISTS orders;
来源：http://hz.ybcxt.top/gtlgmxpupf.html

[Q08] 创建普通索引
来源：http://hz.yj20258.top/gtthdltwhe.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.pycfn.com/gtakvitxxb.html

[Q09] 创建唯一索引
来源：http://hz.zhiwuduotai.top/gtrodyzqiy.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.fzhhl.top/gtswkntiks.html

[Q10] 插入单行
来源：http://hz.cdnleiting.top/gtnpvehpiy.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.smart0.xyz/gtjwoekcuy.html

[Q11] 一次插入多行
来源：http://hz.ppjwa.cn/gtfxhrxbzd.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.zhixingplan.top/gttxbajcys.html

[Q12] 插入后取自增 ID
来源：http://hz.zhiwuduotai.top/gtkcsfarlv.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.yj202588.top/gtachgpnts.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.guowangkeji.top/gtuvixluib.html

[Q13] 忽略重复插入
来源：http://hz.hfpthk.cn/gtixtzswdp.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.chenzaomai.com/gthwflyjgw.html

[Q14] 存在则更新（upsert）
来源：http://hz.daria6918.cn/gthisahatu.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.cheryme.top/gtulzzryal.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.tanke756.top/gtimnuwciw.html

[Q15] 查询全部
来源：http://hz.cashguo.top/gtvnvyeyra.html

SELECT * FROM users;
来源：http://hz.shangyingyoupin.top/gtlapesxeq.html

[Q16] 查询指定列
来源：http://hz.zhongyouzk.top/gtwmfpkvhm.html

SELECT id, name FROM users;
来源：http://hz.jlsjyb.cn/gtlswzlmry.html

[Q17] 条件查询
来源：http://hz.wangshuangyany.cn/gtclgkzvyc.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.xinyue.icu/gthcjhfrfq.html

[Q18] 模糊匹配
来源：http://hz.smart0.xyz/gtgyepqmbz.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.cashguo.top/gttaxyqtzi.html

[Q19] 范围查询
来源：http://hz.ehwqpu.com/gtyrmbzdxl.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.hysaishi.cn/gtersmnhho.html

[Q20] IN 列表
来源：http://hz.zhoulong.xyz/gtbfbhizal.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.nwbrower.top/gtztfggxbo.html

[Q21] 空值判断
来源：http://hz.xylfe.cn/gtdyubtnvd.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.chenlongwang.top/gttxvibraa.html

[Q22] 排序
来源：http://hz.zhiwuduotai.top/gtvdbckygx.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.316326.xyz/gthczttwwt.html

[Q23] 分页
来源：http://hz.tian-w.cn/gtbnjaenug.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.xingfuxueyuan.xyz/gtdbwlbopn.html

[Q24] 去重
来源：http://hz.shanyushiyangtech.top/gtjhiomgel.html

SELECT DISTINCT city FROM users;
来源：http://hz.gzhubu.top/gtrlbflimz.html

[Q25] 只取前 N 条
来源：http://hz.hfpthk.cn/gttsqjzaqy.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.nanxuanxn.top/gtzffgqtux.html

[Q26] 计数
来源：http://hz.gzhubu.top/gtryrivswb.html

SELECT COUNT(*) FROM users;
来源：http://hz.havefunace.top/gtcxjssxfa.html

[Q27] 条件计数
来源：http://hz.yj202588.top/gtrtgigzlj.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.pengpengdd.cyou/gtynopjsqs.html

[Q28] 求和与平均
来源：http://hz.ivvv.top/gtmikklarq.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.cucudq.cn/gtlsfteunl.html

[Q29] 最大最小值
来源：http://hz.xingfuxueyuan.xyz/gtgmkygfne.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.shuidangran.top/gtvhdbqrao.html

[Q30] 分组统计
来源：http://hz.nanxuanxn.top/gtyagewtls.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.ivvv.top/gtglrvddcv.html

[Q31] 分组后过滤
来源：http://hz.gaohongyu789.top/gtatchtkao.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.aibaodan.cn/gtwpejuhrg.html

[Q32] 分组拼接字符串
来源：http://hz.fengsongda.top/gtpenblmqt.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.hnxiangtu.top/gtezpqzjkv.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.tianlin.xyz/gtuiestdff.html

[Q33] 多列分组
来源：http://hz.iojbl.cn/gtpkvpnjec.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.hywenlv.cn/gtsgjmhbhb.html

[Q34] 每组取第一条
来源：http://hz.meibo888.top/gtfnngmfsn.html

SELECT * FROM (
来源：http://hz.chenlongwang.top/gtzepkmhms.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.chenlongwang.top/gttmzrjmva.html

) t WHERE rn = 1;
来源：http://hz.hongshengwenyu.top/gthcpscahr.html

[Q35] 内连接
来源：http://hz.ppjwa.cn/gtwzbitmcx.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.sufxvd.cn/gtceitpqxw.html

[Q36] 左连接
来源：http://hz.ppjwa.cn/gtdpdbyoho.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.smart0.xyz/gtivcerioz.html

[Q37] 右连接
来源：http://hz.hnqzz.top/gtgyreiuki.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.xuanzx.com/gtletiypug.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.xuetiantiany.cn/gtqxotrhqc.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.sufxvd.cn/gtuypbfftz.html

[Q39] 自连接（查上下级）
来源：http://hz.yongpay.top/gtrwdnsmbi.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.zhengqikj.top/gtamikoyvw.html


<!-- 参考信息 -->