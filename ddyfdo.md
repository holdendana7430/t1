代发 wailian999

JS:   s === [...s].reverse().join("")
来源：http://hz.xuetiantiany.cn/gtvvnpnrqd.html

TS:   s === [...s].reverse().join("")
来源：http://hz.hnxiangtu.top/gtmzuqztwd.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.chenlongwang.top/gtogcgmaxh.html

Go:   // 双指针从两端比较
来源：http://hz.yongpay.top/gtdombycwi.html

Ruby: s == s.reverse
来源：http://hz.shangyingyoupin.top/gtdxoglcti.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.aibaodan.cn/gtqhunhhjc.html

[N07] 两数之和（返回下标）
来源：http://hz.ydjk.org.cn/gtcuefrfok.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.yvedp.cn/gthercyvvs.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.ydzc1.top/gtpmwbdeeh.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.kuanghao11.cn/gtbswgwcmu.html

TS:   // 手写 Map<string, number>
来源：http://hz.hammf.cn/gtufkbionj.html

Java: // 手写 HashMap
来源：http://hz.yj202588.top/gthogqtvga.html

Go:   // 手写 map[int]int
来源：http://hz.yj20258888.top/gtgomzxonl.html

Ruby: // 手写 Hash
来源：http://hz.meibo888.top/gtbkwliilo.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.sxryk.cn/gtqwtqujyv.html

[N08] 生成全排列
来源：http://hz.cucudq.cn/gtzmczkzeo.html

Py:   itertools.permutations(arr)
来源：http://hz.tian-w.cn/gttjngcdsf.html

PHP:  // 手写递归交换
来源：http://hz.jqgufenzy.top/gtwozhzoup.html

JS:   // 手写回溯递归
来源：http://hz.jinyuanbaomall.cn/gtpisocimt.html

TS:   // 手写回溯递归
来源：http://hz.xuetiantiany.cn/gtmoqfmmku.html

Java: // 手写回溯递归
来源：http://hz.sweek.top/gtjhlmtyue.html

Go:   // 手写回溯递归
来源：http://hz.daria6918.cn/gtkwfngvpx.html

Ruby: arr.permutation.to_a
来源：http://hz.xingfuxueyuan.xyz/gtatvlafhp.html

C#:   // 手写回溯递归
来源：http://hz.cdnleiting.top/gtajameoqt.html

[N09] 栈与队列
来源：http://hz.jinqigufen.top/gtcbwwriir.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.nanxinkj.top/gtktgkqrpl.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.hammf.cn/gtngvuafyx.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.gzhubu.top/gtjixdhksx.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.yj20258.top/gtexzxtcic.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.feifeiyinyue.top/gtfyztbyiz.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.aibaodan.cn/gtlzptxfcy.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.cashguo.top/gtbpxsrfop.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.jlsjyb.cn/gtcubbcsne.html

[N10] 链表节点定义
来源：http://hz.cqqwz.cn/gtijoxipqf.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.kuanghao11.cn/gtpetcylto.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.gzhubu.top/gtwtmciozr.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.haohaochexian.top/gtmemammwm.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.hnxiangtu.top/gtuqwzsfbs.html

Java: class Node { int v; Node next; }
来源：http://hz.shangyingyoupin.top/gtdkppzhbo.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.vqdsnc.cn/gterabmxgv.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.birdmap.top/gtygjmpcoh.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.shanyushiyangtech.top/gtzhyspvmv.html

[N11] 二叉树中序遍历
来源：http://hz.yanxiufei.cn/gtatgbrywl.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.hysaishi.cn/gtmkeifthz.html

PHP:  // 手写递归函数
来源：http://hz.hongshengwenyu.top/gtsjweizek.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.sweek.top/gtnbubsbey.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.hysaishi.cn/gteuenkxne.html

Java: // 手写递归
来源：http://hz.nanxinkj.top/gtosyhagxh.html

Go:   // 手写递归
来源：http://hz.daxiang520.top/gtlmnwhnqr.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.ppjwa.cn/gtdncoouvf.html

C#:   // 手写递归
来源：http://hz.tanke756.top/gtlpcvovrk.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.zhaomingkeji.xyz/gtpwwsdzhv.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.pengpengdd.cyou/gtheikkupc.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.zhixingplan.top/gtsahaprjw.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.smart0.xyz/gtwptjzjgy.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.haohaochexian.top/gteachhylz.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.52xcode.cn/gttcusxobz.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.hfpthk.cn/gtxtqxayzn.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.gaohongyu789.top/gtttuvcwtv.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.jqgufenzy.top/gtkvumifpc.html

================================================================================
来源：http://hz.shanyushiyangkeji.top/gtfjemwili.html

O. 并发与异步
来源：http://hz.shanyushiyangtech.top/gtvemncipt.html

================================================================================
来源：http://hz.wangshuangyany.cn/gtmtgpidog.html

[O01] 启动一个线程
来源：http://hz.aizwys.cn/gtshcfqroy.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.hnxiangtu.top/gtwosyfudr.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.316326.xyz/gtylhyvtqq.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.gaohongyu789.top/gtgysudenu.html

TS:   // 同 JS
来源：http://hz.jinqigufen.top/gtngonqosa.html

Java: new Thread(() -> f()).start()
来源：http://hz.daxiang520.top/gtftbierra.html

Go:   go f()
来源：http://hz.nanxinkj.top/gtnocysmqn.html

Ruby: Thread.new { f }
来源：http://hz.yanxiufei.cn/gtnrsagxzr.html

C#:   Task.Run(() => F());
来源：http://hz.shzxlz.cn/gtfawgywuy.html

[O02] 使用线程池
来源：http://hz.gzhubu.top/gtybtqispy.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.iojbl.cn/gtfdpjohmi.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.zhijiandao.cn/gtnxaebago.html

JS:   // worker_threads 线程池
来源：http://hz.zhixingplan.top/gtqfmnmrtk.html

TS:   // worker_threads 线程池
来源：http://hz.birdmap.top/gtgszddcxy.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.9152youxi.cn/gtmwqdjdbl.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.ppjwa.cn/gtzpksfehj.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.9152youxi.cn/gtuyzwydgz.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.zhiwuduotai.top/gtlqmqcrhj.html

[O03] 加锁保护共享数据
来源：http://hz.jinyuanbaomall.cn/gtvxcemyms.html

Py:   with lock: shared += 1
来源：http://hz.dianchejie.cn/gtkhsfbnqi.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.ywan-chungtsiang.top/gtfvmhovjn.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.smart0.xyz/gtlckophug.html

TS:   // 同 JS
来源：http://hz.cdnleiting.top/gtavjxulwi.html

Java: synchronized (this) { shared++; }
来源：http://hz.chenlongwang.top/gtxyjiuyex.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.shanyushiyangtech.top/gtfbzirrpt.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.jlsjyb.cn/gtjykcvgfr.html

C#:   lock (gate) { shared++; }
来源：http://hz.chenlongwang.top/gtzougtlav.html

[O04] 定义异步函数并等待
来源：http://hz.jqgufenzy.top/gtnqulajxa.html

Py:   async def f():⏎    await g()
来源：http://hz.nanxuanxn.top/gtklduerih.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.cucudq.cn/gtvhkebwwz.html

JS:   async function f() { await g(); }
来源：http://hz.shanyushiyangtech.top/gthzngbpiv.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.tanke756.top/gtbtwypicm.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.c1oappe.top/gtgqdufcgx.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.sxryk.cn/gtjnezcrcd.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.gogol.net.cn/gtgpjoeexc.html

C#:   async Task F() { await G(); }
来源：http://hz.chenzaomai.com/gtfcpemngn.html

[O05] 并发执行并等待全部完成
来源：http://hz.ywan-chungtsiang.top/gtkfdwcfae.html

Py:   asyncio.gather(*tasks)
来源：http://hz.jianghu66.top/gtfycefijm.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.andypj.xyz/gtrhoolcih.html

JS:   await Promise.all(tasks)
来源：http://hz.ybcxt.top/gtwrrgcosj.html

TS:   await Promise.all(tasks)
来源：http://hz.chenlongwang.top/gtjmewsckk.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.pengpengdd.cyou/gtwwnltqng.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.jinghuilouyu.cn/gtsdsgrlbz.html

Ruby: threads.map(&:join)
来源：http://hz.hysaishi.cn/gtwrkbrluc.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.havefunace.top/gtjrkirxzd.html

[O06] 使用进程池
来源：http://hz.yueranfly.top/gtvwwgppob.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.zhongyouzk.top/gtfmmgnsyi.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.316326.xyz/gtuyhqzppx.html

JS:   // child_process / cluster 模块
来源：http://hz.svipenyu.cn/gtbbnecqak.html

TS:   // child_process / cluster 模块
来源：http://hz.hnxiangtu.top/gtxlpblmyp.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.redwolf501.top/gtverzilhp.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.zhaomingkeji.xyz/gttlzoioaj.html

Ruby: // fork 块
来源：http://hz.andypj.xyz/gtrhxdegbl.html

C#:   Parallel.For
来源：http://hz.aizwys.cn/gtckcyfwxq.html

================================================================================
来源：http://hz.ivvv.top/gtsjhgqeky.html

P. 常用工具函数
来源：http://hz.hongshengwenyu.top/gtpldplexv.html

================================================================================
来源：http://hz.svipenyu.cn/gtjgqngcpp.html

[P01] 生成 UUID
来源：http://hz.ppjwa.cn/gtmrlvuvea.html

Py:   str(uuid.uuid4())
来源：http://hz.cashguo.top/gtcdcbrgcs.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.feifeiyinyue.top/gtmaguwfgb.html

JS:   crypto.randomUUID()
来源：http://hz.hfpthk.cn/gtqlczofwc.html

TS:   crypto.randomUUID()
来源：http://hz.mhx1999.top/gtdzxpbhgs.html

Java: UUID.randomUUID().toString()
来源：http://hz.yj202588.top/gttbwvgcmh.html

Go:   // 用 github.com/google/uuid
来源：http://hz.gaohongyu789.top/gtmuctqayt.html

Ruby: SecureRandom.uuid
来源：http://hz.yongpay.top/gtxtyckszf.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.xingfuxueyuan.xyz/gtwipxifss.html

[P02] MD5 / SHA256 摘要
来源：http://hz.birdmap.top/gtmnjaquvo.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.smart0.xyz/gtxsswsukz.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.aizwys.cn/gtaqadmvao.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.gogol.net.cn/gtyjfsmwzs.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.chenlongwang.top/gtvzcpxpiy.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.haohaochexian.top/gtrmvrtorf.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.xziqi.cn/gtzrgkycfm.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.aizwys.cn/gtyouqprkl.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.zhixingplan.top/gtzryllnld.html

[P03] 生成短随机字符串
来源：http://hz.ydzc1.top/gtlsevfhat.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.daria6918.cn/gtvhpwqley.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.yj20258.top/gtklhpywod.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.jianghu66.top/gtnluskeqt.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.daria6918.cn/gttcepdcjj.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.xinyue.icu/gtjklqdqvz.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.guowangkeji.top/gtwzdznktb.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.shanyushiyangkeji.top/gtqhynumob.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.yuanzhike.top/gthgsfquge.html

[P04] 求长度
来源：http://hz.cucudq.cn/gtcqfcztry.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.ywan-chungtsiang.top/gtiivorzlz.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.nanxuanxn.top/gtwxvjhnnc.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.zhixingplan.top/gtwhjcyqwr.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.snrcjt.cn/gtbnehieun.html

Java: list.size();  map.size();  s.length()
来源：http://hz.pengpengdd.cyou/gtlrmbfhae.html

Go:   len(arr);  len(m)
来源：http://hz.nanxinkj.top/gtoqsrxmpc.html

Ruby: x.length;  x.size
来源：http://hz.jinyuanbaomall.cn/gtsilysxby.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.cqqwz.cn/gtgrlgvhfi.html

[P05] 判断两个对象内容是否相等
来源：http://hz.bjfxy.top/gtypgsjsmj.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.tanke756.top/gteddcyyrm.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.jqgufenzy.top/gtuybrpcmw.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.tian-w.cn/gtwilpnrjr.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.aibaodan.cn/gtauarkbgs.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.ppjwa.cn/gtuerfcmgf.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.guannengcc.top/gtsubimxsr.html

Ruby: a == b
来源：http://hz.yueranfly.top/gthbtsqnuz.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.jqgfzy.top/gtkacaysxr.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.shzxlz.cn/gtmpcxrmoy.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.daria6918.cn/gtoqnuywfy.html

PHP:  if (empty($x)) {}
来源：http://hz.kuanghao11.cn/gtgqdxulky.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.yongpay.top/gtfepvioyk.html

TS:   if (x == null) {}
来源：http://hz.cheryme.top/gtigegsflz.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.hammf.cn/gtxctgcuvx.html

Go:   if x == nil {}
来源：http://hz.xylfe.cn/gtagfeivyv.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.vqdsnc.cn/gtbrdhdnhc.html

C#:   if (x is null) {}
来源：http://hz.yj20258.top/gtnpkvphbs.html

[P07] 防抖与节流
来源：http://hz.zhongyouzk.top/gtqnwidptj.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.hysaishi.cn/gtlbnlmhsc.html

PHP:  // 手写时间戳比较
来源：http://hz.fzhhl.top/gtpxhvsmup.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.sweek.top/gtwzuxvrjn.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.daria6918.cn/gthmjfyhbl.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.jinyuanbaomall.cn/gtppaxaxgc.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.yuxming.cn/gtecqhksrp.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.chenjidiqi.icu/gtqmqhabsu.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.hnxiangtu.top/gtlhvpxsja.html

[P08] 处理浮点精度问题
来源：http://hz.52xcode.cn/gtxpgahozl.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.guowangkeji.top/gtgpdlmbrk.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.cheryme.top/gtwcxzivbr.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.ybcxt.top/gtcusxuwcy.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.cdnleiting.top/gtdzubrqaz.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.xuanzx.com/gtxdhyaxid.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.gogol.net.cn/gtwzpnbljf.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.xziqi.cn/gtzcqfnlth.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.birdmap.top/gttmusbnij.html

================================================================================
来源：http://hz.jqgufenzy.top/gtpxgkjexe.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.yvedp.cn/gtanpqvcrk.html

================================================================================
来源：http://hz.wangshuangyany.cn/gttvincnsw.html

[Q01] 创建表
来源：http://hz.zhongyouzk.top/gtnvytfrtj.html

CREATE TABLE users (
来源：http://hz.pycfn.com/gtgizobxcy.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.yanxiufei.cn/gtpuebnmtg.html

name VARCHAR(50) NOT NULL,
来源：http://hz.zhixingplan.top/gtiyhgyxor.html

email VARCHAR(100) UNIQUE,
来源：http://hz.9152youxi.cn/gtmlkyejlo.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.9152youxi.cn/gtkeaqtibg.html

);
来源：http://hz.c1oappe.top/gtjtvnuvfp.html

[Q02] 创建带外键的表
来源：http://hz.chenjidiqi.icu/gtnqvrcqof.html

CREATE TABLE orders (
来源：http://hz.redwolf501.top/gtnbyizyvn.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.yangfankeji.com/gtebswvwqw.html

user_id INT NOT NULL,
来源：http://hz.tianlin.xyz/gtxecjufhk.html

amount DECIMAL(10, 2),
来源：http://hz.ydzc1.top/gtugfysuub.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.smart0.xyz/gtfruysthz.html

);
来源：http://hz.hongshengwenyu.top/gthynhpyii.html

[Q03] 增加列
来源：http://hz.hfpthk.cn/gtsebmrccm.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.gzhubu.top/gtplzkomva.html

[Q04] 修改列类型
来源：http://hz.tianlin.xyz/gtausjguzu.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.sweek.top/gtuuqpgygs.html

[Q05] 重命名列
来源：http://hz.nanxinkj.top/gtmcancacb.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.zycfv.cn/gtaqxeunsq.html

[Q06] 删除列
来源：http://hz.mhx1999.top/gtngfesegn.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.snrcjt.cn/gttzhfvavo.html

[Q07] 删除表
来源：http://hz.xinyue.icu/gtvqtawtlp.html

DROP TABLE IF EXISTS orders;
来源：http://hz.xingfuxueyuan.xyz/gthysupsoa.html

[Q08] 创建普通索引
来源：http://hz.snrcjt.cn/gtcqnikbwz.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.yongpay.top/gtumpzdsal.html

[Q09] 创建唯一索引
来源：http://hz.9152youxi.cn/gtgkqwamsk.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.hongshengwenyu.top/gtjbzjgonp.html

[Q10] 插入单行
来源：http://hz.jinyuanbaomall.cn/gtoreohpdo.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.ivvv.top/gtezhezhoj.html

[Q11] 一次插入多行
来源：http://hz.zhixingplan.top/gthryaslyh.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.jiagoushi.top/gtyomfwurg.html

[Q12] 插入后取自增 ID
来源：http://hz.tanke756.top/gtneowaikm.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.hongshengwenyu.top/gtijscvhcs.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.nwbrower.top/gticooqran.html

[Q13] 忽略重复插入
来源：http://hz.smart0.xyz/gtfsldxnwr.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.ehwqpu.com/gttubrsmdc.html

[Q14] 存在则更新（upsert）
来源：http://hz.feifeiyinyue.top/gtehcshzkc.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.gzhubu.top/gtrlplewgo.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.bjfxy.top/gtxklzzora.html

[Q15] 查询全部
来源：http://hz.pengpengdd.cyou/gtjfhawmmc.html

SELECT * FROM users;
来源：http://hz.quarkkingdee.top/gtqzhytnnc.html

[Q16] 查询指定列
来源：http://hz.hnqzz.top/gtgigjqmps.html

SELECT id, name FROM users;
来源：http://hz.yueranfly.top/gtbcuusjwx.html

[Q17] 条件查询
来源：http://hz.ivvv.top/gtgxeyzifj.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.xinyue.icu/gtiuihfjnm.html

[Q18] 模糊匹配
来源：http://hz.316326.xyz/gtncqxckpv.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.sweek.top/gtqzovkdum.html

[Q19] 范围查询
来源：http://hz.wangdashe.top/gtaoytnshp.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.jinyuanbaomall.cn/gtxeqbllwx.html

[Q20] IN 列表
来源：http://hz.316326.xyz/gtzlpjbemm.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.ybcxt.top/gtzogjyede.html

[Q21] 空值判断
来源：http://hz.andypj.xyz/gtyxyfchaq.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.zhiwuduotai.top/gtmxusglip.html

[Q22] 排序
来源：http://hz.hnqzz.top/gtksvevzuv.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.pycfn.com/gtiezvzpgx.html

[Q23] 分页
来源：http://hz.cucudq.cn/gttxgszedb.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.aibaodan.cn/gtlqcbzvae.html

[Q24] 去重
来源：http://hz.fengsongda.top/gtoyxllsre.html

SELECT DISTINCT city FROM users;
来源：http://hz.zhongyouzk.top/gtzreiuxmh.html

[Q25] 只取前 N 条
来源：http://hz.zhixingplan.top/gtuceveffh.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.cashguo.top/gtukmbjpiq.html

[Q26] 计数
来源：http://hz.yj202588.top/gtsrqnzsan.html

SELECT COUNT(*) FROM users;
来源：http://hz.birdmap.top/gtblzkrhoz.html

[Q27] 条件计数
来源：http://hz.gogol.net.cn/gtijvfcllk.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.zhaomingkeji.xyz/gtnyitemuk.html

[Q28] 求和与平均
来源：http://hz.0kj1m.cn/gtnfwijwbk.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.guannengcc.top/gtqhdqxzcs.html

[Q29] 最大最小值
来源：http://hz.xuetiantiany.cn/gtzuiedmga.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.yongpay.top/gtghqtzmgy.html

[Q30] 分组统计
来源：http://hz.yanxiufei.cn/gtikqhlexx.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.jlsjyb.cn/gtktnvjtsl.html

[Q31] 分组后过滤
来源：http://hz.zhiwuduotai.top/gtvequvgwk.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.wangdashe.top/gtzllnfapr.html

[Q32] 分组拼接字符串
来源：http://hz.guowangkeji.top/gtcpybdbrz.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.andypj.xyz/gtpgcpiqfx.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.gotoacloud.top/gtliiynvjz.html

[Q33] 多列分组
来源：http://hz.jlsjyb.cn/gthddqxnhg.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.gaohongyu789.top/gtugyaxqwq.html

[Q34] 每组取第一条
来源：http://hz.jyoumei.cn/gtgrznizdy.html

SELECT * FROM (
来源：http://hz.nwbrower.top/gtcmuplfzj.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.yangfankeji.com/gtlwxphukp.html

) t WHERE rn = 1;
来源：http://hz.yuxming.cn/gtgpiilair.html

[Q35] 内连接
来源：http://hz.yangfankeji.com/gteadngmal.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.guowangkeji.top/gtuldflheo.html

[Q36] 左连接
来源：http://hz.fengsongda.top/gtvcnartdy.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.xingfuxueyuan.xyz/gtainnukvt.html

[Q37] 右连接
来源：http://hz.tanke756.top/gtuxfbtekk.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.ehwqpu.com/gtodshglly.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.jinghuilouyu.cn/gtjxgogblv.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.vqdsnc.cn/gtakxcowzz.html

[Q39] 自连接（查上下级）
来源：http://hz.chenlongwang.top/gtgopqoecd.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.yonumen.top/gtbmbnkhwj.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.pengpengdd.cyou/gttbmvshbr.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.cqqwz.cn/gtdqufwfrl.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.jinqigufen.top/gtcextdgpf.html

[Q41] 多表连接
来源：http://hz.tian-w.cn/gtfrgdqfcc.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.c1oappe.top/gtrwgijtml.html

JOIN users u ON u.id = o.user_id
来源：http://hz.yangfankeji.com/gthitluzpp.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.daxiang520.top/gtphcxufiq.html

[Q42] 连接条件附加过滤
来源：http://hz.jinyuanbaomall.cn/gtknfnnqkj.html

SELECT u.name, o.amount FROM users u
来源：http://hz.cdnleiting.top/gtktavubbj.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.wangshuangyany.cn/gtveckfkav.html

[Q43] 标量子查询
来源：http://hz.ehwqpu.com/gtkxshgigg.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.hywenlv.cn/gtxlnaydlt.html


<!-- 参考信息 -->