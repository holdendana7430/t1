代发 wailian999

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.hfpthk.cn/gtyntjabrp.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.316326.xyz/gtmcvdckzy.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.c1oappe.top/gtpziqyqhr.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.xinyue.icu/gtsjfbzqvu.html

[N05] 最大公约数
来源：http://hz.xingfuxueyuan.xyz/gtzbevzjit.html

Py:   math.gcd(a, b)
来源：http://hz.andypj.xyz/gtuyiirhjr.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.guannengcc.top/gtupqlvrvh.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.shanyushiyangtech.top/gtaapbuirp.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.cucudq.cn/gthojwyxap.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.jinghuilouyu.cn/gtowqphnir.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.zdqjudy.top/gtzwurpnld.html

Ruby: a.gcd(b)
来源：http://hz.daria6918.cn/gtqtmkrzfz.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.aibaodan.cn/gtsklgimtu.html

[N06] 判断回文字符串
来源：http://hz.jqgufenzy.top/gtxhedfqiu.html

Py:   s == s[::-1]
来源：http://hz.yj20258.top/gtqtoukudd.html

PHP:  $s === strrev($s);
来源：http://hz.tanke756.top/gtkloezcxg.html

JS:   s === [...s].reverse().join("")
来源：http://hz.tanke756.top/gtmaejdswk.html

TS:   s === [...s].reverse().join("")
来源：http://hz.havefunace.top/gtjlioylqh.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.havefunace.top/gtdoguoxzy.html

Go:   // 双指针从两端比较
来源：http://hz.ybcxt.top/gtlvuoeawo.html

Ruby: s == s.reverse
来源：http://hz.jinqigufen.top/gtzvozyyrk.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.xinyue.icu/gthddegdtx.html

[N07] 两数之和（返回下标）
来源：http://hz.zhongyouzk.top/gtijtscrwn.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.shanyushiyangtech.top/gtjfgrimsa.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.xingfuxueyuan.xyz/gtfudfbhzu.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.ybcxt.top/gtbbbjgavb.html

TS:   // 手写 Map<string, number>
来源：http://hz.52xcode.cn/gtrtmhoebo.html

Java: // 手写 HashMap
来源：http://hz.jlsjyb.cn/gtqpexmhiv.html

Go:   // 手写 map[int]int
来源：http://hz.pengpengdd.cyou/gttrhoyjuf.html

Ruby: // 手写 Hash
来源：http://hz.yueranfly.top/gtyieleelv.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.dianchejie.cn/gtogxmfyvj.html

[N08] 生成全排列
来源：http://hz.0kj1m.cn/gtdpttsxxe.html

Py:   itertools.permutations(arr)
来源：http://hz.zhoulong.xyz/gtepdpzjim.html

PHP:  // 手写递归交换
来源：http://hz.hnqzz.top/gtuypscxgp.html

JS:   // 手写回溯递归
来源：http://hz.guannengcc.top/gtetdtpbgk.html

TS:   // 手写回溯递归
来源：http://hz.yuxming.cn/gtfbfkjvrw.html

Java: // 手写回溯递归
来源：http://hz.jyoumei.cn/gtuotsqjzn.html

Go:   // 手写回溯递归
来源：http://hz.jlsjyb.cn/gtfcmglkde.html

Ruby: arr.permutation.to_a
来源：http://hz.yanxiufei.cn/gtyahgpgql.html

C#:   // 手写回溯递归
来源：http://hz.smart0.xyz/gttxszoxer.html

[N09] 栈与队列
来源：http://hz.jinghuilouyu.cn/gtrnryxxex.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.redwolf501.top/gtzqkqnwgq.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.tian-w.cn/gtbmzntytr.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.snrcjt.cn/gtepabvpon.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.feifeiyinyue.top/gtvwveprsz.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.bjfxy.top/gtblnufcan.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.svipenyu.cn/gtkhhrvlgp.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.xinyue.icu/gtrgijwghl.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.jinqigufen.top/gtxmmfzeec.html

[N10] 链表节点定义
来源：http://hz.ydzc1.top/gtltqrjboe.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.sxryk.cn/gtzaurhhhc.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.shanyushiyangtech.top/gtynrwmgzu.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.dashuyun.cn/gtfkqraqll.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.sxryk.cn/gtlsmxmjyr.html

Java: class Node { int v; Node next; }
来源：http://hz.chenlongwang.top/gtnbonlhqt.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.kuanghao11.cn/gtamrvjndi.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.hysaishi.cn/gtdodobepl.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.shangyingyoupin.top/gtfpdpwhyf.html

[N11] 二叉树中序遍历
来源：http://hz.yangfankeji.com/gtpzmkwsna.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.hongshengwenyu.top/gtltkiieyl.html

PHP:  // 手写递归函数
来源：http://hz.jqgfzy.top/gtmvwknkma.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.andypj.xyz/gtkapdycth.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.chenjidiqi.icu/gtccfggrzr.html

Java: // 手写递归
来源：http://hz.shzxlz.cn/gtefyxnuhg.html

Go:   // 手写递归
来源：http://hz.feifeiyinyue.top/gtmlotigpb.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.hnqzz.top/gtcjokmvcx.html

C#:   // 手写递归
来源：http://hz.tianlin.xyz/gtkbyqsgjj.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.kuanghao11.cn/gtaerdlesv.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.cucudq.cn/gtmuwbtqfy.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.zhiwuduotai.top/gtxuhdjhnj.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.gogol.net.cn/gtnuotdlxh.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.jinqigfzy.top/gtvphqjeot.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.nanxuanxn.top/gtwholaivr.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.aibaodan.cn/gtumdnyseg.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.yangfankeji.com/gtqmzqxypv.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.jlsjyb.cn/gtrmaggyug.html

================================================================================
来源：http://hz.andypj.xyz/gttrqvlmak.html

O. 并发与异步
来源：http://hz.yangfankeji.com/gtknfaffbs.html

================================================================================
来源：http://hz.jlsjyb.cn/gtiluesjtl.html

[O01] 启动一个线程
来源：http://hz.hnxiangtu.top/gtzdjptdso.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.ehwqpu.com/gteomileva.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.jqgfzy.top/gtjfkcxmsl.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.bjfxy.top/gtgbzihjhp.html

TS:   // 同 JS
来源：http://hz.xinyue.icu/gtkhpfayqm.html

Java: new Thread(() -> f()).start()
来源：http://hz.shanyushiyangtech.top/gtqsgymfcu.html

Go:   go f()
来源：http://hz.fzhhl.top/gtivadjeht.html

Ruby: Thread.new { f }
来源：http://hz.yongpay.top/gtuwewkfty.html

C#:   Task.Run(() => F());
来源：http://hz.yangfankeji.com/gtkyufvglb.html

[O02] 使用线程池
来源：http://hz.jinqigufen.top/gthykeruru.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.gzhubu.top/gtqboydbtw.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.shuidangran.top/gthaswtceg.html

JS:   // worker_threads 线程池
来源：http://hz.ehwqpu.com/gttbjfzelm.html

TS:   // worker_threads 线程池
来源：http://hz.xziqi.cn/gtzzevgrlw.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.tanke756.top/gtedeusfxc.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.hywenlv.cn/gtttugnjld.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.yj20258.top/gtbllmmlrf.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.zdqjudy.top/gtdoaxkeul.html

[O03] 加锁保护共享数据
来源：http://hz.ehwqpu.com/gtokmynuea.html

Py:   with lock: shared += 1
来源：http://hz.cheryme.top/gtczrhdfsn.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.svipenyu.cn/gtcozumndo.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.hywenlv.cn/gtyxdgkhiv.html

TS:   // 同 JS
来源：http://hz.xinyue.icu/gtemkgxqnr.html

Java: synchronized (this) { shared++; }
来源：http://hz.jinyuanbaomall.cn/gtogewrnca.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.fengsongda.top/gtbdupkmdv.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.hammf.cn/gtnpqimypi.html

C#:   lock (gate) { shared++; }
来源：http://hz.bjfxy.top/gteepwpqpv.html

[O04] 定义异步函数并等待
来源：http://hz.pengpengdd.cyou/gtgpdsyrbm.html

Py:   async def f():⏎    await g()
来源：http://hz.zhaomingkeji.xyz/gtbpwfbane.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.cheryme.top/gtontdmjsr.html

JS:   async function f() { await g(); }
来源：http://hz.gogol.net.cn/gtycmirdmd.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.yueranfly.top/gtomdcjvtf.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.sysykeji.top/gtvocgoeol.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.yueranfly.top/gtioxijeeb.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.guannengcc.top/gtxwvqyinn.html

C#:   async Task F() { await G(); }
来源：http://hz.shzxlz.cn/gtvyumzshj.html

[O05] 并发执行并等待全部完成
来源：http://hz.jyoumei.cn/gtbecreesw.html

Py:   asyncio.gather(*tasks)
来源：http://hz.fzhhl.top/gtmdydqnrw.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.xinyue.icu/gtvyichjby.html

JS:   await Promise.all(tasks)
来源：http://hz.yj20258888.top/gtjbwuvonl.html

TS:   await Promise.all(tasks)
来源：http://hz.zhaomingkeji.xyz/gtdngijbiv.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.hfpthk.cn/gtwvygnbdm.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.tanke756.top/gtuxygjuno.html

Ruby: threads.map(&:join)
来源：http://hz.aizwys.cn/gttdminxdw.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.sysykeji.top/gthcnrnsag.html

[O06] 使用进程池
来源：http://hz.yueranfly.top/gtnuelgngk.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.yonumen.top/gtnpeevjnk.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.havefunace.top/gtjtmvcvpl.html

JS:   // child_process / cluster 模块
来源：http://hz.yuanzhike.top/gtpdcgcdwt.html

TS:   // child_process / cluster 模块
来源：http://hz.hammf.cn/gtwqtleswo.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.pycfn.com/gttigtepmw.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.shangyingyoupin.top/gtcuexeqes.html

Ruby: // fork 块
来源：http://hz.zycfv.cn/gtyjocdgfq.html

C#:   Parallel.For
来源：http://hz.nwbrower.top/gtebjxuwlr.html

================================================================================
来源：http://hz.shzxlz.cn/gtbzdmmzyi.html

P. 常用工具函数
来源：http://hz.jlsjyb.cn/gtultgmone.html

================================================================================
来源：http://hz.fengsongda.top/gtwpvwnkrt.html

[P01] 生成 UUID
来源：http://hz.xuetiantiany.cn/gtulqsmftr.html

Py:   str(uuid.uuid4())
来源：http://hz.hfpthk.cn/gtakrdtgow.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.hongshengwenyu.top/gtprfueakb.html

JS:   crypto.randomUUID()
来源：http://hz.vqdsnc.cn/gthfwdvqkt.html

TS:   crypto.randomUUID()
来源：http://hz.shuidangran.top/gtxwgerdui.html

Java: UUID.randomUUID().toString()
来源：http://hz.xingfuxueyuan.xyz/gtytvgkcrj.html

Go:   // 用 github.com/google/uuid
来源：http://hz.shanyushiyangkeji.top/gtpvwbhkkj.html

Ruby: SecureRandom.uuid
来源：http://hz.yuxming.cn/gtqahwuvdj.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.ydzc1.top/gtjalokfun.html

[P02] MD5 / SHA256 摘要
来源：http://hz.aibaodan.cn/gtcjdnrzkf.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.yj20258.top/gtgspejwzv.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.gogol.net.cn/gtqdamuezy.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.yuxming.cn/gtgsslezwp.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.bjfxy.top/gteqegyner.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.316326.xyz/gtajicmzzw.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.xinyue.icu/gtbigcoesw.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.jiagoushi.top/gtifafykkn.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.zhaomingkeji.xyz/gtzsmkmcyx.html

[P03] 生成短随机字符串
来源：http://hz.ivvv.top/gtvfqxvcbv.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.xuetiantiany.cn/gtsrigglbx.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.xingfuxueyuan.xyz/gtaszdqmnz.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.9152youxi.cn/gtmjaxxpbm.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.xylfe.cn/gtgbaobqqp.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.jianghu66.top/gtbcrnnsnz.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.hywenlv.cn/gtcqsiwvtf.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.nanxinkj.top/gtxyqhxlkx.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.feifeiyinyue.top/gtjpxmfjfs.html

[P04] 求长度
来源：http://hz.jiagoushi.top/gtsikphvuy.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.xziqi.cn/gtnxvguphy.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.cqqwz.cn/gtmlxvkhkj.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.yangfankeji.com/gticnpfeia.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.zdqjudy.top/gtikqrnnuq.html

Java: list.size();  map.size();  s.length()
来源：http://hz.pengpengdd.cyou/gtgmvbcbfl.html

Go:   len(arr);  len(m)
来源：http://hz.hnxiangtu.top/gtvruksfzv.html

Ruby: x.length;  x.size
来源：http://hz.haohaochexian.top/gtikwupyiu.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.xinyue.icu/gtizdwjjzl.html

[P05] 判断两个对象内容是否相等
来源：http://hz.nwbrower.top/gtikhoueaf.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.gotoacloud.top/gtbtqfnodn.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.birdmap.top/gtnpvxpyha.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.tianlin.xyz/gthubcgxjq.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.zhaomingkeji.xyz/gtpqzlhyvq.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.redwolf501.top/gtdkwfspni.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.tianlin.xyz/gteqjxfqti.html

Ruby: a == b
来源：http://hz.jinghuilouyu.cn/gtypvtrurk.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.hfpthk.cn/gtmnhmebze.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.xinyue.icu/gtgkfursci.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.zdqjudy.top/gtujytddrt.html

PHP:  if (empty($x)) {}
来源：http://hz.zhixingplan.top/gtvlonnvkm.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.jiagoushi.top/gtmddgfcyl.html

TS:   if (x == null) {}
来源：http://hz.yuxming.cn/gtxmdofofh.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.andypj.xyz/gtwcdoiycb.html

Go:   if x == nil {}
来源：http://hz.chenzaomai.com/gtxglorjin.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.jinqigufen.top/gtuvukdfza.html

C#:   if (x is null) {}
来源：http://hz.shangyingyoupin.top/gteztocvkt.html

[P07] 防抖与节流
来源：http://hz.jyoumei.cn/gtekvpuifw.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.gogol.net.cn/gtxvdomkda.html

PHP:  // 手写时间戳比较
来源：http://hz.hysaishi.cn/gtpkigrbda.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.hfpthk.cn/gtuytfchil.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.fzhhl.top/gtrbhxygqh.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.yonumen.top/gtfoxeyffa.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.yvedp.cn/gtrwdfhhdj.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.zhengqikj.top/gtxviucczj.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.sweek.top/gtoxtuinpi.html

[P08] 处理浮点精度问题
来源：http://hz.mhx1999.top/gtzttdlett.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.zdqjudy.top/gtygcyhzzo.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.hnxiangtu.top/gtawhmustf.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.ydzc1.top/gtphhjwxka.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.hammf.cn/gtgbvgvloc.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.kuanghao11.cn/gtljsdnlgv.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.kuanghao11.cn/gtosbwgzmk.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.guannengcc.top/gtpdkacksb.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.vqdsnc.cn/gtyajgbysk.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtbsniyxsh.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.fengsongda.top/gtjhpyxlkw.html

================================================================================
来源：http://hz.ehwqpu.com/gtplocqgjj.html

[Q01] 创建表
来源：http://hz.xylfe.cn/gtcakldxob.html

CREATE TABLE users (
来源：http://hz.316326.xyz/gtupqnbxff.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.zhixingplan.top/gtygglandn.html

name VARCHAR(50) NOT NULL,
来源：http://hz.ydzc1.top/gtdrxbuliv.html

email VARCHAR(100) UNIQUE,
来源：http://hz.jinqigufen.top/gtiiuqlldb.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.yj202588.top/gtxwaasnfl.html

);
来源：http://hz.hfpthk.cn/gtgzdtwmtr.html

[Q02] 创建带外键的表
来源：http://hz.yueranfly.top/gtktedbiqb.html

CREATE TABLE orders (
来源：http://hz.zhoulong.xyz/gtxgwfjcmu.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.fengsongda.top/gtiicrtgsg.html

user_id INT NOT NULL,
来源：http://hz.jqgufenzy.top/gtvydzunvb.html

amount DECIMAL(10, 2),
来源：http://hz.wangdashe.top/gtkhizjvyc.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.svipenyu.cn/gtweecpiji.html

);
来源：http://hz.fzhhl.top/gtsdchktjt.html

[Q03] 增加列
来源：http://hz.shangyingyoupin.top/gtbwjkrqap.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.chenlongwang.top/gtnxpyrzqw.html

[Q04] 修改列类型
来源：http://hz.gotoacloud.top/gtyskrpbqw.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.yonumen.top/gtuaezfzli.html

[Q05] 重命名列
来源：http://hz.fengsongda.top/gttaxmrmmf.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.zhixingplan.top/gteznzwnyt.html

[Q06] 删除列
来源：http://hz.fzhhl.top/gtarkcnyrs.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.ppjwa.cn/gtovoywpma.html

[Q07] 删除表
来源：http://hz.yj202588.top/gtzxqeuzxv.html

DROP TABLE IF EXISTS orders;
来源：http://hz.sufxvd.cn/gtlcmtamce.html

[Q08] 创建普通索引
来源：http://hz.zhongyouzk.top/gtmcloodlb.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.birdmap.top/gtshpaylui.html

[Q09] 创建唯一索引
来源：http://hz.yvedp.cn/gtkwhuvyoq.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.kuanghao11.cn/gtouyfdcsk.html

[Q10] 插入单行
来源：http://hz.hammf.cn/gtsewkfdww.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.yj20258.top/gtmwywmmre.html

[Q11] 一次插入多行
来源：http://hz.yueranfly.top/gtapykdcyc.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.ydzc1.top/gtjjqjmuvw.html

[Q12] 插入后取自增 ID
来源：http://hz.andypj.xyz/gtxwiovuis.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.daria6918.cn/gtrkpjdlzt.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.fengsongda.top/gtvbjsdafb.html

[Q13] 忽略重复插入
来源：http://hz.shzxlz.cn/gteaegoxvn.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.cashguo.top/gtjyfchibc.html

[Q14] 存在则更新（upsert）
来源：http://hz.dianchejie.cn/gtbmahsywg.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.iojbl.cn/gtwxjydueh.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.guowangkeji.top/gtxfupnmxp.html

[Q15] 查询全部
来源：http://hz.cheryme.top/gtffxwlyal.html

SELECT * FROM users;
来源：http://hz.cucudq.cn/gtxjolwcbd.html

[Q16] 查询指定列
来源：http://hz.ydjk.org.cn/gtucljdimw.html

SELECT id, name FROM users;
来源：http://hz.andypj.xyz/gtxoptojvm.html

[Q17] 条件查询
来源：http://hz.shangyingyoupin.top/gtipsaqjet.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.ppjwa.cn/gtpfhpgxyh.html

[Q18] 模糊匹配
来源：http://hz.dashuyun.cn/gtidogxilo.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.ydzc1.top/gtpqpusbyg.html

[Q19] 范围查询
来源：http://hz.chenjidiqi.icu/gtbzsagpql.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.0kj1m.cn/gtnprcerxj.html

[Q20] IN 列表
来源：http://hz.kuanghao11.cn/gtrxceogzx.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.andypj.xyz/gtzsabygzj.html

[Q21] 空值判断
来源：http://hz.jqgufenzy.top/gtdsuonzpb.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.jiagoushi.top/gttfgwlsnp.html

[Q22] 排序
来源：http://hz.zhongyouzk.top/gtkuuxphfq.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.zhijiandao.cn/gtvyknnzhm.html

[Q23] 分页
来源：http://hz.kuanghao11.cn/gtpusznlmk.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.yongpay.top/gtwwjyxqfn.html

[Q24] 去重
来源：http://hz.jianghu66.top/gtxisauelo.html

SELECT DISTINCT city FROM users;
来源：http://hz.c1oappe.top/gtczosazax.html

[Q25] 只取前 N 条
来源：http://hz.cheryme.top/gtvgkfcfsc.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.gotoacloud.top/gthhrjtbdw.html

[Q26] 计数
来源：http://hz.yanxiufei.cn/gtoziimuuc.html

SELECT COUNT(*) FROM users;
来源：http://hz.shzxlz.cn/gtwtctkeej.html

[Q27] 条件计数
来源：http://hz.0kj1m.cn/gtufvyyiwt.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.tianlin.xyz/gtmrtcgszx.html

[Q28] 求和与平均
来源：http://hz.daxiang520.top/gthowqnqln.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.daria6918.cn/gtbtfejrqv.html

[Q29] 最大最小值
来源：http://hz.nwbrower.top/gtecbselnd.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.zdqjudy.top/gtokrdkukh.html

[Q30] 分组统计
来源：http://hz.haohaochexian.top/gtqqqfoozo.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.sysykeji.top/gtijwzzowr.html

[Q31] 分组后过滤
来源：http://hz.svipenyu.cn/gtltyfxkwe.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.cheryme.top/gtyonvqjgr.html

[Q32] 分组拼接字符串
来源：http://hz.hfpthk.cn/gtlwpsgrtf.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.hongshengwenyu.top/gtctbntpqs.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.xuanzx.com/gtbqrxzgmt.html

[Q33] 多列分组
来源：http://hz.xuanzx.com/gtdduqlolx.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.daria6918.cn/gthqbjbeng.html

[Q34] 每组取第一条
来源：http://hz.wangshuangyany.cn/gtmualrklc.html

SELECT * FROM (
来源：http://hz.sxryk.cn/gttfdapayk.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.guannengcc.top/gtkikrbohl.html

) t WHERE rn = 1;
来源：http://hz.kuanghao11.cn/gtbvudysji.html

[Q35] 内连接
来源：http://hz.yueranfly.top/gtgbpxalaw.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.pengpengdd.cyou/gtbzmnmdcz.html

[Q36] 左连接
来源：http://hz.chenlongwang.top/gtalvkcvtz.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.guannengcc.top/gtfadxvxpl.html

[Q37] 右连接
来源：http://hz.cdnleiting.top/gtsbmpnyeg.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.gogol.net.cn/gtrqbcmupi.html


<!-- 参考信息 -->