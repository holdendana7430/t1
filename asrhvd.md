代发 wailian999

[N05] 最大公约数
来源：http://hz.yvedp.cn/gtvgdtfkji.html

Py:   math.gcd(a, b)
来源：http://hz.pycfn.com/gtubpcmwpn.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.ydjk.org.cn/gtnospcxcv.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.cheryme.top/gtezphybuf.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.jyoumei.cn/gtzknsdhqr.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.0kj1m.cn/gtjoluyyas.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.quarkkingdee.top/gtwudrfzos.html

Ruby: a.gcd(b)
来源：http://hz.9152youxi.cn/gtcgywazjn.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.daxiang520.top/gtdmjutkxa.html

[N06] 判断回文字符串
来源：http://hz.jinqigufen.top/gtttxhlbez.html

Py:   s == s[::-1]
来源：http://hz.yueranfly.top/gtiqertypd.html

PHP:  $s === strrev($s);
来源：http://hz.xziqi.cn/gtkytdmjfy.html

JS:   s === [...s].reverse().join("")
来源：http://hz.xziqi.cn/gtykxseczh.html

TS:   s === [...s].reverse().join("")
来源：http://hz.daria6918.cn/gteyzlaant.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.aizwys.cn/gtuptbuffr.html

Go:   // 双指针从两端比较
来源：http://hz.gaohongyu789.top/gtoqbsweuo.html

Ruby: s == s.reverse
来源：http://hz.iojbl.cn/gtwqwsvbdh.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.birdmap.top/gtjobtudil.html

[N07] 两数之和（返回下标）
来源：http://hz.zhoulong.xyz/gtesjjwyrb.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.yuxming.cn/gtckdrchhd.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.haohaochexian.top/gtrqitlsop.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.yanxiufei.cn/gtyxrfoqlf.html

TS:   // 手写 Map<string, number>
来源：http://hz.snrcjt.cn/gtfjhdzdly.html

Java: // 手写 HashMap
来源：http://hz.andypj.xyz/gtstsekxqk.html

Go:   // 手写 map[int]int
来源：http://hz.jinghuilouyu.cn/gtenregdfu.html

Ruby: // 手写 Hash
来源：http://hz.nanxuanxn.top/gtofjxvfaj.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.gaohongyu789.top/gtchuseonv.html

[N08] 生成全排列
来源：http://hz.ydzc1.top/gtedgncwmx.html

Py:   itertools.permutations(arr)
来源：http://hz.shzxlz.cn/gtntyqnxwf.html

PHP:  // 手写递归交换
来源：http://hz.tianlin.xyz/gtrwrsvsvk.html

JS:   // 手写回溯递归
来源：http://hz.jinqigfzy.top/gtovlvylkw.html

TS:   // 手写回溯递归
来源：http://hz.tianlin.xyz/gtevqfoieu.html

Java: // 手写回溯递归
来源：http://hz.c1oappe.top/gtzmssolyv.html

Go:   // 手写回溯递归
来源：http://hz.ydjk.org.cn/gtxxxfrozb.html

Ruby: arr.permutation.to_a
来源：http://hz.cdnleiting.top/gtpkgzyvqu.html

C#:   // 手写回溯递归
来源：http://hz.ivvv.top/gtnxdqciwd.html

[N09] 栈与队列
来源：http://hz.guannengcc.top/gteuovrgrd.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.hywenlv.cn/gthdsybndi.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.ehwqpu.com/gtolxbjkpp.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.redwolf501.top/gtaltxrpmj.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.andypj.xyz/gtnwiwoply.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.nanxinkj.top/gtrzkazzza.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.316326.xyz/gtnuwmyrmn.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.hysaishi.cn/gtoctpebgs.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.pycfn.com/gtrmakkfzd.html

[N10] 链表节点定义
来源：http://hz.gogol.net.cn/gtcdfobvle.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.yueranfly.top/gtngatqmvd.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.smart0.xyz/gtjhlixfun.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.gogol.net.cn/gtszjnjbzg.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.jinqigufen.top/gtrghmhxyf.html

Java: class Node { int v; Node next; }
来源：http://hz.quarkkingdee.top/gtivoerqtf.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.quarkkingdee.top/gtbupmpayl.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.jianghu66.top/gtmpkoteig.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.zhixingplan.top/gtohweoeqs.html

[N11] 二叉树中序遍历
来源：http://hz.ydjk.org.cn/gtwrxjjbco.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.zycfv.cn/gtftjjwndk.html

PHP:  // 手写递归函数
来源：http://hz.zhiwuduotai.top/gthlpkvigo.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.jqgufenzy.top/gtbpkhwull.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.zhoulong.xyz/gtajlmodbe.html

Java: // 手写递归
来源：http://hz.zhijiandao.cn/gtcijpwuye.html

Go:   // 手写递归
来源：http://hz.yj20258888.top/gtaiumcrsu.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.ywan-chungtsiang.top/gtmgkbwnyu.html

C#:   // 手写递归
来源：http://hz.pycfn.com/gtlrzsjfnx.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.sxryk.cn/gtjhdrfykw.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.pengpengdd.cyou/gtelbovvci.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.yueranfly.top/gtpdydleav.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.yvedp.cn/gtyppwdkhh.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.jianghu66.top/gtdhajadbt.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.iojbl.cn/gttexiryva.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.9152youxi.cn/gtbxmwsney.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.ybcxt.top/gtfapxhkxn.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.ppjwa.cn/gtmwgjxtvt.html

================================================================================
来源：http://hz.hywenlv.cn/gtleakhoih.html

O. 并发与异步
来源：http://hz.daxiang520.top/gtfingvsyq.html

================================================================================
来源：http://hz.jyoumei.cn/gtlomjebur.html

[O01] 启动一个线程
来源：http://hz.wangshuangyany.cn/gtucnyvobk.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.ehwqpu.com/gtvyueqido.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.ydzc1.top/gtwgowxthk.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.cqqwz.cn/gtdsjougyy.html

TS:   // 同 JS
来源：http://hz.zhaomingkeji.xyz/gtmxbczxgw.html

Java: new Thread(() -> f()).start()
来源：http://hz.tanke756.top/gtuceepjwd.html

Go:   go f()
来源：http://hz.ehwqpu.com/gtisrdhuix.html

Ruby: Thread.new { f }
来源：http://hz.pengpengdd.cyou/gtvtnghbkq.html

C#:   Task.Run(() => F());
来源：http://hz.yangfankeji.com/gtpewadqpi.html

[O02] 使用线程池
来源：http://hz.iojbl.cn/gtuglpmepz.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.smart0.xyz/gtrpjrkfwx.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.daria6918.cn/gttwfrlgvi.html

JS:   // worker_threads 线程池
来源：http://hz.wangshuangyany.cn/gtuvinnkxc.html

TS:   // worker_threads 线程池
来源：http://hz.jlsjyb.cn/gtpsyivktz.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.nanxuanxn.top/gtrmpivkpg.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.nanxinkj.top/gtbqbribyt.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.redwolf501.top/gtlasnjfqa.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.jinyuanbaomall.cn/gtglxqxdra.html

[O03] 加锁保护共享数据
来源：http://hz.52xcode.cn/gtijjsggjd.html

Py:   with lock: shared += 1
来源：http://hz.chenjidiqi.icu/gtnhikoscx.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.hnxiangtu.top/gtmjnrcebk.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.shanyushiyangkeji.top/gtgbcepobt.html

TS:   // 同 JS
来源：http://hz.daria6918.cn/gtqzmklppp.html

Java: synchronized (this) { shared++; }
来源：http://hz.wangshuangyany.cn/gtbecyuwcn.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.feifeiyinyue.top/gtxlriqeqm.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.zhengqikj.top/gtexblzycq.html

C#:   lock (gate) { shared++; }
来源：http://hz.tanke756.top/gtnobajbno.html

[O04] 定义异步函数并等待
来源：http://hz.ywan-chungtsiang.top/gtcbznnrlq.html

Py:   async def f():⏎    await g()
来源：http://hz.zhiwuduotai.top/gtbckhioes.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.jyoumei.cn/gtcqrkssno.html

JS:   async function f() { await g(); }
来源：http://hz.wangshuangyany.cn/gtmtiiyrrk.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.ivvv.top/gtqperkjkx.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.kuanghao11.cn/gtmyrwkvvo.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.yvedp.cn/gtabuwafge.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.shuidangran.top/gtfervaymh.html

C#:   async Task F() { await G(); }
来源：http://hz.yj20258888.top/gtzaghpnac.html

[O05] 并发执行并等待全部完成
来源：http://hz.ywan-chungtsiang.top/gtnhacivfv.html

Py:   asyncio.gather(*tasks)
来源：http://hz.yangfankeji.com/gtbmjnpdvi.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.zhiwuduotai.top/gtxethivoe.html

JS:   await Promise.all(tasks)
来源：http://hz.sweek.top/gtmfcksyfn.html

TS:   await Promise.all(tasks)
来源：http://hz.hammf.cn/gtipmpthgz.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.gzhubu.top/gtfsutcdwq.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.gotoacloud.top/gtjvtbwkkj.html

Ruby: threads.map(&:join)
来源：http://hz.shangyingyoupin.top/gtdlrmbfvz.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.birdmap.top/gtrmjusrae.html

[O06] 使用进程池
来源：http://hz.jianghu66.top/gtsobpdfbk.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.cheryme.top/gtopiplhnz.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.jyoumei.cn/gttkhjvhuj.html

JS:   // child_process / cluster 模块
来源：http://hz.haohaochexian.top/gtbezmrhya.html

TS:   // child_process / cluster 模块
来源：http://hz.shzxlz.cn/gtnwpdkjcm.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.daxiang520.top/gtxxddurqq.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.shanyushiyangkeji.top/gtonjlvtei.html

Ruby: // fork 块
来源：http://hz.c1oappe.top/gtvstgawxo.html

C#:   Parallel.For
来源：http://hz.gzhubu.top/gtpljzgncg.html

================================================================================
来源：http://hz.iojbl.cn/gtasingtru.html

P. 常用工具函数
来源：http://hz.jqgufenzy.top/gtirtgpvee.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtvtktsnfj.html

[P01] 生成 UUID
来源：http://hz.tanke756.top/gtdzicgdyx.html

Py:   str(uuid.uuid4())
来源：http://hz.fengsongda.top/gtzaxpnlyi.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.yuxming.cn/gtjfudcgru.html

JS:   crypto.randomUUID()
来源：http://hz.wangdashe.top/gtexjcuxdv.html

TS:   crypto.randomUUID()
来源：http://hz.andypj.xyz/gtdqwhlttn.html

Java: UUID.randomUUID().toString()
来源：http://hz.yj20258.top/gtocttgjyx.html

Go:   // 用 github.com/google/uuid
来源：http://hz.xuetiantiany.cn/gtroauuxjn.html

Ruby: SecureRandom.uuid
来源：http://hz.0kj1m.cn/gtdaclnkij.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.zhoulong.xyz/gtohounajl.html

[P02] MD5 / SHA256 摘要
来源：http://hz.wangdashe.top/gtzggyjnsd.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.guowangkeji.top/gtwfdfnolp.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.nanxuanxn.top/gtizykitzr.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.shuidangran.top/gtyfvfncav.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.hywenlv.cn/gtfcdhagfy.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.hammf.cn/gtggqhrdzc.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.wangshuangyany.cn/gtoxezounq.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.ydjk.org.cn/gtycgnbqbt.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.ywan-chungtsiang.top/gtvweoavpr.html

[P03] 生成短随机字符串
来源：http://hz.shangyingyoupin.top/gtfmxrqgyg.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.9152youxi.cn/gtassqfbvr.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.zhengqikj.top/gtvhknzeob.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.nanxuanxn.top/gtugpvnbbo.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.yj20258.top/gtbxtfypdc.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.tanke756.top/gtalcnzykv.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.nanxuanxn.top/gtvawmoatq.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.andypj.xyz/gtaosfqzfj.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.hysaishi.cn/gtrorwmfap.html

[P04] 求长度
来源：http://hz.snrcjt.cn/gtiefltmyk.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.jinqigufen.top/gtdudcwmfp.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.guannengcc.top/gtuiotmeza.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.jqgufenzy.top/gtsmfoymst.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.kuanghao11.cn/gtzvvlfpuv.html

Java: list.size();  map.size();  s.length()
来源：http://hz.shangyingyoupin.top/gtxwokiafh.html

Go:   len(arr);  len(m)
来源：http://hz.hongshengwenyu.top/gtxmrzxqdx.html

Ruby: x.length;  x.size
来源：http://hz.gogol.net.cn/gtjyigukoe.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.shanyushiyangkeji.top/gtnixddcbp.html

[P05] 判断两个对象内容是否相等
来源：http://hz.nanxuanxn.top/gtugqamfwc.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.ydzc1.top/gtsrioxujb.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.shanyushiyangtech.top/gtntsejfgl.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.ybcxt.top/gtmujwwuhw.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.meibo888.top/gtetuzktsf.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.ehwqpu.com/gtweaijuyf.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.zhiwuduotai.top/gtpfztknnf.html

Ruby: a == b
来源：http://hz.jiagoushi.top/gtprirwwuv.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.chenzaomai.com/gtsjenunub.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.jinyuanbaomall.cn/gtgjdvrxgy.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.zhaomingkeji.xyz/gtmnpjehnu.html

PHP:  if (empty($x)) {}
来源：http://hz.c1oappe.top/gttgctpiza.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.vqdsnc.cn/gtcitaueez.html

TS:   if (x == null) {}
来源：http://hz.yuxming.cn/gtuwbtelvm.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.bjfxy.top/gtlthxknls.html

Go:   if x == nil {}
来源：http://hz.ydzc1.top/gtrcqwdjpz.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.hywenlv.cn/gtbcubdcoj.html

C#:   if (x is null) {}
来源：http://hz.sufxvd.cn/gtzcxmnodm.html

[P07] 防抖与节流
来源：http://hz.dianchejie.cn/gtkrrehdgr.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.yuxming.cn/gtzsgmrzvo.html

PHP:  // 手写时间戳比较
来源：http://hz.zycfv.cn/gtkjzjgfxa.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.zdqjudy.top/gtiqzfjria.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.fengsongda.top/gtoczkcehc.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.c1oappe.top/gtrjuuirqg.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.aizwys.cn/gttsruozco.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.tianlin.xyz/gtwfcttwxs.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.mhx1999.top/gtuencudcu.html

[P08] 处理浮点精度问题
来源：http://hz.xylfe.cn/gtfbxxyush.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.52xcode.cn/gtgvpaicaq.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.ybcxt.top/gtdlpbhmhw.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.yonumen.top/gtrnjqkhkh.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.zhengqikj.top/gtsgvkjvaf.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.xuetiantiany.cn/gtamuavwcv.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.52xcode.cn/gtkqkhxbxl.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.gzhubu.top/gtgaouxmuf.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.yvedp.cn/gtqmfwphdx.html

================================================================================
来源：http://hz.dashuyun.cn/gtcgjjgmis.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.daxiang520.top/gtmyrbpugm.html

================================================================================
来源：http://hz.yj20258.top/gtkbarejbd.html

[Q01] 创建表
来源：http://hz.fzhhl.top/gtxoejccgv.html

CREATE TABLE users (
来源：http://hz.zhongyouzk.top/gtjqgukwmi.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.shuidangran.top/gtnfhmixdz.html

name VARCHAR(50) NOT NULL,
来源：http://hz.nanxuanxn.top/gtnetlxuoo.html

email VARCHAR(100) UNIQUE,
来源：http://hz.redwolf501.top/gtfgnppfsj.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.xinyue.icu/gtrylhmlzu.html

);
来源：http://hz.daria6918.cn/gtweoqtjwp.html

[Q02] 创建带外键的表
来源：http://hz.yj202588.top/gtavlrxngv.html

CREATE TABLE orders (
来源：http://hz.havefunace.top/gthpuuwcze.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.ppjwa.cn/gtqlxtqdsk.html

user_id INT NOT NULL,
来源：http://hz.mhx1999.top/gtggwmyith.html

amount DECIMAL(10, 2),
来源：http://hz.bjfxy.top/gtgguiycbc.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.zhoulong.xyz/gtwjzyzumh.html

);
来源：http://hz.kuanghao11.cn/gtawllbfub.html

[Q03] 增加列
来源：http://hz.jinghuilouyu.cn/gtwzjwsrxv.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.shangyingyoupin.top/gtiwlmpbml.html

[Q04] 修改列类型
来源：http://hz.gogol.net.cn/gtedqhwlno.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.nwbrower.top/gtarsucqdv.html

[Q05] 重命名列
来源：http://hz.tian-w.cn/gtzmsvhqgh.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.yuanzhike.top/gtrfqggprg.html

[Q06] 删除列
来源：http://hz.gogol.net.cn/gtgjgavfym.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.jlsjyb.cn/gtyuihytoh.html

[Q07] 删除表
来源：http://hz.yj20258.top/gtseynjyyn.html

DROP TABLE IF EXISTS orders;
来源：http://hz.shanyushiyangkeji.top/gtsvpihwhk.html

[Q08] 创建普通索引
来源：http://hz.dianchejie.cn/gtedzkijoa.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.tianlin.xyz/gtdlhptetj.html

[Q09] 创建唯一索引
来源：http://hz.birdmap.top/gteddtmfvc.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.hongshengwenyu.top/gtnctfeifv.html

[Q10] 插入单行
来源：http://hz.yj20258888.top/gtkduzpwbv.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.c1oappe.top/gtsgiomrct.html

[Q11] 一次插入多行
来源：http://hz.daria6918.cn/gtienibvss.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.quarkkingdee.top/gtjllcvkwu.html

[Q12] 插入后取自增 ID
来源：http://hz.gaohongyu789.top/gtixubdjip.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.jinqigufen.top/gthanlxmec.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.xinyue.icu/gtnkbilego.html

[Q13] 忽略重复插入
来源：http://hz.yangfankeji.com/gtonrmvwrt.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.hfpthk.cn/gtkwznidtu.html

[Q14] 存在则更新（upsert）
来源：http://hz.aibaodan.cn/gtiovesuco.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.zhixingplan.top/gtkcsifysx.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.wangdashe.top/gtysstgizu.html

[Q15] 查询全部
来源：http://hz.wangshuangyany.cn/gtwqpoeubo.html

SELECT * FROM users;
来源：http://hz.pycfn.com/gtcyhuvodi.html

[Q16] 查询指定列
来源：http://hz.yongpay.top/gtnltastru.html

SELECT id, name FROM users;
来源：http://hz.0kj1m.cn/gtqfbpktkk.html

[Q17] 条件查询
来源：http://hz.guannengcc.top/gteuzlpgcu.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.wangshuangyany.cn/gtrnpqhttf.html

[Q18] 模糊匹配
来源：http://hz.yuxming.cn/gtnxmjtpjb.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.redwolf501.top/gtvnqxyjqu.html

[Q19] 范围查询
来源：http://hz.c1oappe.top/gtvlmezexs.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.dianchejie.cn/gtzuvndiaq.html

[Q20] IN 列表
来源：http://hz.316326.xyz/gtmkucducf.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.hnqzz.top/gtxmsnazji.html

[Q21] 空值判断
来源：http://hz.mhx1999.top/gtigdgzpep.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.quarkkingdee.top/gtkuzjspeh.html

[Q22] 排序
来源：http://hz.gaohongyu789.top/gtvkghrwvd.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.smart0.xyz/gtppzenebj.html

[Q23] 分页
来源：http://hz.shangyingyoupin.top/gtqlfzxoiz.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.chenlongwang.top/gtamvvhevm.html

[Q24] 去重
来源：http://hz.yuxming.cn/gtjqaochwa.html

SELECT DISTINCT city FROM users;
来源：http://hz.pengpengdd.cyou/gtmmtupqso.html

[Q25] 只取前 N 条
来源：http://hz.tanke756.top/gtuvqtjaxf.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.yonumen.top/gtxmgihqtd.html

[Q26] 计数
来源：http://hz.tanke756.top/gtjapoynzd.html

SELECT COUNT(*) FROM users;
来源：http://hz.jianghu66.top/gtjfpnqybe.html

[Q27] 条件计数
来源：http://hz.hnxiangtu.top/gtucptkjtk.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.ivvv.top/gtlgwyholc.html

[Q28] 求和与平均
来源：http://hz.hnxiangtu.top/gtyeyddqzu.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.gzhubu.top/gtxpnlzlgh.html

[Q29] 最大最小值
来源：http://hz.tian-w.cn/gtpzkqdoxe.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.andypj.xyz/gtizrdoxtr.html

[Q30] 分组统计
来源：http://hz.yj20258.top/gtpohcuckv.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.sufxvd.cn/gtaxjvtjmf.html

[Q31] 分组后过滤
来源：http://hz.9152youxi.cn/gthiotdhsi.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.yuanzhike.top/gtfawpeskb.html

[Q32] 分组拼接字符串
来源：http://hz.cashguo.top/gtrqngispo.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.ehwqpu.com/gtzfausksb.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.yongpay.top/gtnzkmnciy.html

[Q33] 多列分组
来源：http://hz.dashuyun.cn/gtjfwxisxg.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.jiagoushi.top/gtzembnimn.html

[Q34] 每组取第一条
来源：http://hz.tanke756.top/gtfllgvcry.html

SELECT * FROM (
来源：http://hz.c1oappe.top/gtolxuyxqd.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.hongshengwenyu.top/gtcbgnizds.html

) t WHERE rn = 1;
来源：http://hz.zhixingplan.top/gtlbwizqmq.html

[Q35] 内连接
来源：http://hz.zhaomingkeji.xyz/gtdbwhkkfk.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.shangyingyoupin.top/gtkxzmwcsm.html

[Q36] 左连接
来源：http://hz.ppjwa.cn/gtpkfnbgsd.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.zhijiandao.cn/gtfqakbnrp.html

[Q37] 右连接
来源：http://hz.hnqzz.top/gtdkkmgqwp.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.c1oappe.top/gtndunwmmc.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.chenzaomai.com/gtuwzivici.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.shuidangran.top/gtvefizqov.html

[Q39] 自连接（查上下级）
来源：http://hz.snrcjt.cn/gtxdgbyryr.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.dashuyun.cn/gtitiblify.html


<!-- 参考信息 -->