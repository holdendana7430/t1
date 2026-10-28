代发 wailian999

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.yanxiufei.cn/gtrieprmii.html

[N06] 判断回文字符串
来源：http://hz.sweek.top/gtavilgrfd.html

Py:   s == s[::-1]
来源：http://hz.haohaochexian.top/gtgqphqdmh.html

PHP:  $s === strrev($s);
来源：http://hz.ybcxt.top/gthsjizfai.html

JS:   s === [...s].reverse().join("")
来源：http://hz.meibo888.top/gtjreahvjp.html

TS:   s === [...s].reverse().join("")
来源：http://hz.zhengqikj.top/gtjiwqddja.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.xylfe.cn/gtgelbbgak.html

Go:   // 双指针从两端比较
来源：http://hz.cashguo.top/gtcdmcamen.html

Ruby: s == s.reverse
来源：http://hz.yuxming.cn/gtwxalvgyb.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.guowangkeji.top/gtsphgfzrg.html

[N07] 两数之和（返回下标）
来源：http://hz.zhixingplan.top/gtapfmqdry.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.cucudq.cn/gtpmzboqhw.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.9152youxi.cn/gtzuxwyhfz.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.cdnleiting.top/gtetohfpzc.html

TS:   // 手写 Map<string, number>
来源：http://hz.bjfxy.top/gtlexiixeb.html

Java: // 手写 HashMap
来源：http://hz.jinghuilouyu.cn/gtdfjrqzmx.html

Go:   // 手写 map[int]int
来源：http://hz.wangshuangyany.cn/gtbcsqwfaq.html

Ruby: // 手写 Hash
来源：http://hz.smart0.xyz/gtiegwppjc.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.cdnleiting.top/gtefoaaxyq.html

[N08] 生成全排列
来源：http://hz.hnxiangtu.top/gtokmjtyjn.html

Py:   itertools.permutations(arr)
来源：http://hz.zdqjudy.top/gtoeiujzzt.html

PHP:  // 手写递归交换
来源：http://hz.yanxiufei.cn/gtutfdfyme.html

JS:   // 手写回溯递归
来源：http://hz.nwbrower.top/gtbdpacbwu.html

TS:   // 手写回溯递归
来源：http://hz.hongshengwenyu.top/gtvmbdauaj.html

Java: // 手写回溯递归
来源：http://hz.ywan-chungtsiang.top/gtacnfqpfi.html

Go:   // 手写回溯递归
来源：http://hz.daxiang520.top/gtuyjautlv.html

Ruby: arr.permutation.to_a
来源：http://hz.sweek.top/gtdrtccbec.html

C#:   // 手写回溯递归
来源：http://hz.chenlongwang.top/gtwwsfgdgi.html

[N09] 栈与队列
来源：http://hz.wangdashe.top/gtkqyntnet.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.guowangkeji.top/gtsncwlllu.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.gogol.net.cn/gtmdkppakn.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.shuidangran.top/gtjqcjhtii.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.mhx1999.top/gtfysoyfbb.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.meibo888.top/gtrrnsaaqu.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.haohaochexian.top/gtqtiwhbla.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.sweek.top/gtlfaxslai.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.havefunace.top/gtmfykcwse.html

[N10] 链表节点定义
来源：http://hz.sysykeji.top/gtctmrqaie.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.hywenlv.cn/gtkeqtcsgh.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.jyoumei.cn/gtxwcjtsbk.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.gogol.net.cn/gtkqaxzttr.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.zhongyouzk.top/gtbegbzmkc.html

Java: class Node { int v; Node next; }
来源：http://hz.hongshengwenyu.top/gtzsjqkjcv.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.wangdashe.top/gtxpdipmot.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.chenlongwang.top/gthalzvvnd.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.wangshuangyany.cn/gtarwtjpzo.html

[N11] 二叉树中序遍历
来源：http://hz.fengsongda.top/gtbecxucmc.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.shuidangran.top/gtderadvcv.html

PHP:  // 手写递归函数
来源：http://hz.nwbrower.top/gtkxinoykh.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.zhoulong.xyz/gtihfbvjgy.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.dashuyun.cn/gtuooyeasn.html

Java: // 手写递归
来源：http://hz.xingfuxueyuan.xyz/gtnginiwut.html

Go:   // 手写递归
来源：http://hz.gaohongyu789.top/gtslrzjbaa.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.yuxming.cn/gtbgoyadtw.html

C#:   // 手写递归
来源：http://hz.aibaodan.cn/gtyfjfsbqr.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.jqgufenzy.top/gtrwnyiqws.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.tianlin.xyz/gtujeffviy.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.aizwys.cn/gtzjsahaip.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.gogol.net.cn/gtbquzzuhm.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.zycfv.cn/gttndlbrel.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.ywan-chungtsiang.top/gtyqhivrse.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.zdqjudy.top/gtqtjhyggg.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.daria6918.cn/gtkbodczmj.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.jiagoushi.top/gtwybvwxos.html

================================================================================
来源：http://hz.birdmap.top/gtqjleosnv.html

O. 并发与异步
来源：http://hz.zhongyouzk.top/gtwrssebsj.html

================================================================================
来源：http://hz.wangshuangyany.cn/gtcqdoejvu.html

[O01] 启动一个线程
来源：http://hz.tianlin.xyz/gtgbnqrsdy.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.316326.xyz/gtiepujpbe.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.52xcode.cn/gtoevrxovy.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.gaohongyu789.top/gtdibbdnzk.html

TS:   // 同 JS
来源：http://hz.dianchejie.cn/gtyertkryh.html

Java: new Thread(() -> f()).start()
来源：http://hz.hnxiangtu.top/gtgbjpfbug.html

Go:   go f()
来源：http://hz.jiagoushi.top/gthoocsdtc.html

Ruby: Thread.new { f }
来源：http://hz.iojbl.cn/gtcypfmcdc.html

C#:   Task.Run(() => F());
来源：http://hz.xingfuxueyuan.xyz/gtrumsbcfb.html

[O02] 使用线程池
来源：http://hz.tanke756.top/gtsbtjgmdi.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.wangdashe.top/gttskideqr.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.jlsjyb.cn/gtvxaruxjv.html

JS:   // worker_threads 线程池
来源：http://hz.fengsongda.top/gtvvgypyjo.html

TS:   // worker_threads 线程池
来源：http://hz.guowangkeji.top/gtptnxhrpe.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.nwbrower.top/gtbpegikdx.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.52xcode.cn/gtobwljqsj.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.fzhhl.top/gthcksbunm.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.hammf.cn/gtutbqkphh.html

[O03] 加锁保护共享数据
来源：http://hz.xylfe.cn/gtrxfmpuph.html

Py:   with lock: shared += 1
来源：http://hz.wangshuangyany.cn/gtmtpdboup.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.zhiwuduotai.top/gtvthdbgyl.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.52xcode.cn/gthtaysmjb.html

TS:   // 同 JS
来源：http://hz.gotoacloud.top/gtbslglgll.html

Java: synchronized (this) { shared++; }
来源：http://hz.hnqzz.top/gtqylxuyio.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.ehwqpu.com/gtvaobqlcg.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.mhx1999.top/gtqpxtjvig.html

C#:   lock (gate) { shared++; }
来源：http://hz.yj20258888.top/gtpvfesspi.html

[O04] 定义异步函数并等待
来源：http://hz.hfpthk.cn/gtvjxcebeg.html

Py:   async def f():⏎    await g()
来源：http://hz.dianchejie.cn/gtkxduzeio.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.ybcxt.top/gtwnldrjmh.html

JS:   async function f() { await g(); }
来源：http://hz.yj20258.top/gthlpdlexo.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.jiagoushi.top/gtzmmpvnva.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.gotoacloud.top/gthdtijdny.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.zhoulong.xyz/gtmpbieagh.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.havefunace.top/gtbsfwxtnb.html

C#:   async Task F() { await G(); }
来源：http://hz.hywenlv.cn/gtqziwrdmq.html

[O05] 并发执行并等待全部完成
来源：http://hz.yj20258.top/gtekjqhyka.html

Py:   asyncio.gather(*tasks)
来源：http://hz.jinyuanbaomall.cn/gtkmchxwde.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.hnxiangtu.top/gtqyswecza.html

JS:   await Promise.all(tasks)
来源：http://hz.shangyingyoupin.top/gtquvpkgxl.html

TS:   await Promise.all(tasks)
来源：http://hz.yongpay.top/gtqdrscqyq.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.yuxming.cn/gtkbqehsuf.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.nanxinkj.top/gtjnsceoqf.html

Ruby: threads.map(&:join)
来源：http://hz.cdnleiting.top/gtalgsrovr.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.yj20258.top/gtqnroymrn.html

[O06] 使用进程池
来源：http://hz.smart0.xyz/gtnubfnajx.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.shanyushiyangkeji.top/gtgugpvgqi.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.zhixingplan.top/gthodjkyba.html

JS:   // child_process / cluster 模块
来源：http://hz.zhongyouzk.top/gtoyobugcd.html

TS:   // child_process / cluster 模块
来源：http://hz.daria6918.cn/gtryhspeal.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.hnxiangtu.top/gtvzfhfcmr.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.dashuyun.cn/gtwgdswwsv.html

Ruby: // fork 块
来源：http://hz.iojbl.cn/gtpjwusxvv.html

C#:   Parallel.For
来源：http://hz.hfpthk.cn/gtpuflrusx.html

================================================================================
来源：http://hz.zycfv.cn/gtlmpntjwp.html

P. 常用工具函数
来源：http://hz.9152youxi.cn/gtjjdrviyw.html

================================================================================
来源：http://hz.yonumen.top/gtdcqkuogg.html

[P01] 生成 UUID
来源：http://hz.yonumen.top/gtfkvgehzi.html

Py:   str(uuid.uuid4())
来源：http://hz.shzxlz.cn/gtfvbrbcrw.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.zycfv.cn/gtixgrdhyr.html

JS:   crypto.randomUUID()
来源：http://hz.aizwys.cn/gtctjgjfhs.html

TS:   crypto.randomUUID()
来源：http://hz.zhongyouzk.top/gtonbjdlzo.html

Java: UUID.randomUUID().toString()
来源：http://hz.gzhubu.top/gtkwwltgtj.html

Go:   // 用 github.com/google/uuid
来源：http://hz.shuidangran.top/gttasjsjur.html

Ruby: SecureRandom.uuid
来源：http://hz.sxryk.cn/gthduhqvuf.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.sxryk.cn/gttzqycfst.html

[P02] MD5 / SHA256 摘要
来源：http://hz.yj20258888.top/gtnrejdcum.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.bjfxy.top/gtkeiolqpe.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.tianlin.xyz/gtqlxqmeyt.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.jinyuanbaomall.cn/gtyqzbxbmr.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.shanyushiyangtech.top/gttxieimds.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.yangfankeji.com/gtttvudclu.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.vqdsnc.cn/gtxokrkplv.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.smart0.xyz/gtmrpqlvdt.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.tanke756.top/gtdxqgbtbl.html

[P03] 生成短随机字符串
来源：http://hz.tian-w.cn/gtxqavfcqg.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.c1oappe.top/gtzebbvkwe.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.nanxuanxn.top/gtlmthbndq.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.haohaochexian.top/gtyandfwhs.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.hammf.cn/gtgiglzahc.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.xziqi.cn/gtmoobelfs.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.zhongyouzk.top/gtieofrnrm.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.cashguo.top/gtnujbrbkp.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.cheryme.top/gtdslgqdbj.html

[P04] 求长度
来源：http://hz.jlsjyb.cn/gtaeqlgldx.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.sufxvd.cn/gtiloosxqd.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.zhijiandao.cn/gtgxzykwpr.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.cqqwz.cn/gtfebiabxv.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.pycfn.com/gtixvchgso.html

Java: list.size();  map.size();  s.length()
来源：http://hz.ehwqpu.com/gtytmjhivx.html

Go:   len(arr);  len(m)
来源：http://hz.yangfankeji.com/gtduaeibxz.html

Ruby: x.length;  x.size
来源：http://hz.quarkkingdee.top/gtmgyuepyz.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.guowangkeji.top/gthiywewzz.html

[P05] 判断两个对象内容是否相等
来源：http://hz.cucudq.cn/gtijwvmziv.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.bjfxy.top/gtizouwhww.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.feifeiyinyue.top/gttvfduogr.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.jinqigufen.top/gtlvpibwfq.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.hfpthk.cn/gtztqigyhi.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.yuanzhike.top/gtfglkrhdm.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.jqgufenzy.top/gtrlnfgcto.html

Ruby: a == b
来源：http://hz.ppjwa.cn/gtgobhngss.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.zhongyouzk.top/gthxkboxti.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.cashguo.top/gttfxeuesx.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.hammf.cn/gtroqapwhl.html

PHP:  if (empty($x)) {}
来源：http://hz.sxryk.cn/gtaqdszbgr.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.zhiwuduotai.top/gtkyjclclw.html

TS:   if (x == null) {}
来源：http://hz.daxiang520.top/gtaintidnn.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.gzhubu.top/gtenslsrzd.html

Go:   if x == nil {}
来源：http://hz.sweek.top/gtbbbndovw.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.nanxinkj.top/gtdngyjuhl.html

C#:   if (x is null) {}
来源：http://hz.shuidangran.top/gtbjdsojca.html

[P07] 防抖与节流
来源：http://hz.yj20258.top/gtwvxwcbzj.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.kuanghao11.cn/gtzoweadow.html

PHP:  // 手写时间戳比较
来源：http://hz.redwolf501.top/gtdkceveth.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.haohaochexian.top/gtnopfwlde.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.yj202588.top/gtmdjdnfje.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.nanxinkj.top/gtxelfojih.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.yj202588.top/gtjixnrvhm.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.chenzaomai.com/gttfbxrvrj.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.xuanzx.com/gttrjvwjik.html

[P08] 处理浮点精度问题
来源：http://hz.vqdsnc.cn/gtbphggxaa.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.316326.xyz/gttapxhcqo.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.meibo888.top/gtaxctqrre.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.cqqwz.cn/gtkvfosjqe.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.jlsjyb.cn/gtvpjaxail.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.xuanzx.com/gtgiyghiif.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.jinghuilouyu.cn/gtdzwtkgpr.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.zhoulong.xyz/gtvginijss.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.jlsjyb.cn/gtsxffjhon.html

================================================================================
来源：http://hz.ybcxt.top/gtwgnhamtz.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.sufxvd.cn/gtmehhyhgv.html

================================================================================
来源：http://hz.9152youxi.cn/gtmmxwlxwd.html

[Q01] 创建表
来源：http://hz.yanxiufei.cn/gthdbhnpqt.html

CREATE TABLE users (
来源：http://hz.guowangkeji.top/gtbolhuavh.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.pengpengdd.cyou/gtxfcqrdld.html

name VARCHAR(50) NOT NULL,
来源：http://hz.zdqjudy.top/gtqyxqcwwy.html

email VARCHAR(100) UNIQUE,
来源：http://hz.jianghu66.top/gtvobpgopn.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.hongshengwenyu.top/gtelsmcjvp.html

);
来源：http://hz.zhongyouzk.top/gtrxokliwg.html

[Q02] 创建带外键的表
来源：http://hz.xinyue.icu/gtetnyckbe.html

CREATE TABLE orders (
来源：http://hz.tianlin.xyz/gtmddpunaa.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.zdqjudy.top/gtymwebhtb.html

user_id INT NOT NULL,
来源：http://hz.9152youxi.cn/gtylkjfbqz.html

amount DECIMAL(10, 2),
来源：http://hz.tian-w.cn/gtscdzmkyt.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.cucudq.cn/gtdokmwszz.html

);
来源：http://hz.daria6918.cn/gtmktkggul.html

[Q03] 增加列
来源：http://hz.jinqigufen.top/gtaqwpqqaz.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.yongpay.top/gtbsmxhthu.html

[Q04] 修改列类型
来源：http://hz.nwbrower.top/gtagxadaqy.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.yangfankeji.com/gtdyilxaoj.html

[Q05] 重命名列
来源：http://hz.guowangkeji.top/gtvuubezmc.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.shzxlz.cn/gtdlvjoeqp.html

[Q06] 删除列
来源：http://hz.vqdsnc.cn/gtsqfrzaft.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.hnxiangtu.top/gtfglxcwer.html

[Q07] 删除表
来源：http://hz.dianchejie.cn/gtubxgivhs.html

DROP TABLE IF EXISTS orders;
来源：http://hz.zhongyouzk.top/gtdhhhkcvy.html

[Q08] 创建普通索引
来源：http://hz.316326.xyz/gtlcqmlhek.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.yueranfly.top/gtwsxirxqy.html

[Q09] 创建唯一索引
来源：http://hz.dashuyun.cn/gtkckbusad.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.sxryk.cn/gtebdyxqtt.html

[Q10] 插入单行
来源：http://hz.cashguo.top/gtsgonlfmw.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.jianghu66.top/gtzbnxprra.html

[Q11] 一次插入多行
来源：http://hz.haohaochexian.top/gttmslezne.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.yueranfly.top/gthutjdmqz.html

[Q12] 插入后取自增 ID
来源：http://hz.xuetiantiany.cn/gtukuwiojv.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.feifeiyinyue.top/gtksiuliby.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.hywenlv.cn/gtdnqcwxzt.html

[Q13] 忽略重复插入
来源：http://hz.hfpthk.cn/gtzxfqdxmf.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.jyoumei.cn/gtuqwuivfi.html

[Q14] 存在则更新（upsert）
来源：http://hz.cucudq.cn/gtkfjpxbcv.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.yanxiufei.cn/gttdwfikgl.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.chenjidiqi.icu/gtnwfjvfno.html

[Q15] 查询全部
来源：http://hz.yonumen.top/gtxnkbnpix.html

SELECT * FROM users;
来源：http://hz.wangshuangyany.cn/gtiaywfktd.html

[Q16] 查询指定列
来源：http://hz.jinyuanbaomall.cn/gtxtxcqdmd.html

SELECT id, name FROM users;
来源：http://hz.jiagoushi.top/gtnpwzhlao.html

[Q17] 条件查询
来源：http://hz.feifeiyinyue.top/gttyycvhot.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.ydjk.org.cn/gthpnsiqxw.html

[Q18] 模糊匹配
来源：http://hz.52xcode.cn/gtjvubfwht.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.316326.xyz/gtoyoarjzh.html

[Q19] 范围查询
来源：http://hz.tian-w.cn/gtkhvpwrbp.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.chenlongwang.top/gttuwvejzr.html

[Q20] IN 列表
来源：http://hz.mhx1999.top/gtnzazezbw.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.chenlongwang.top/gtffkuehut.html

[Q21] 空值判断
来源：http://hz.jinqigufen.top/gtjayhpngm.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.bjfxy.top/gtizhaaikg.html

[Q22] 排序
来源：http://hz.tianlin.xyz/gtqxptsfvv.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.birdmap.top/gttmaxniab.html

[Q23] 分页
来源：http://hz.jinyuanbaomall.cn/gtsmviqrnh.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.chenzaomai.com/gtqtqaxkah.html

[Q24] 去重
来源：http://hz.nwbrower.top/gtgwwqwhjo.html

SELECT DISTINCT city FROM users;
来源：http://hz.sxryk.cn/gtuevpipdf.html

[Q25] 只取前 N 条
来源：http://hz.zhoulong.xyz/gtujrvmtrr.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.guannengcc.top/gtejzygjeu.html

[Q26] 计数
来源：http://hz.shzxlz.cn/gttjrfckjo.html

SELECT COUNT(*) FROM users;
来源：http://hz.wangshuangyany.cn/gtusifdhab.html

[Q27] 条件计数
来源：http://hz.smart0.xyz/gtmnprqlil.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.zhaomingkeji.xyz/gtvjbemjzw.html

[Q28] 求和与平均
来源：http://hz.haohaochexian.top/gtlcotdipd.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.fzhhl.top/gtsahcaofl.html

[Q29] 最大最小值
来源：http://hz.yueranfly.top/gtdbppotkw.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.birdmap.top/gtayfvcnhc.html

[Q30] 分组统计
来源：http://hz.jyoumei.cn/gtppjpjnxh.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.ehwqpu.com/gtpvtebstw.html

[Q31] 分组后过滤
来源：http://hz.hammf.cn/gtyycyjygd.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.pengpengdd.cyou/gtikbqgtif.html

[Q32] 分组拼接字符串
来源：http://hz.fzhhl.top/gtogupfasi.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.sufxvd.cn/gtkwpctccv.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.hnxiangtu.top/gtwuorygly.html

[Q33] 多列分组
来源：http://hz.daria6918.cn/gtzlzqbeed.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.zhaomingkeji.xyz/gtakjvubdf.html

[Q34] 每组取第一条
来源：http://hz.gogol.net.cn/gtfbuwuqjn.html

SELECT * FROM (
来源：http://hz.haohaochexian.top/gtkwsyxunt.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.ehwqpu.com/gtnadgmaub.html

) t WHERE rn = 1;
来源：http://hz.meibo888.top/gthojzqavw.html

[Q35] 内连接
来源：http://hz.wangshuangyany.cn/gtmtxugwuq.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.smart0.xyz/gtosmrhdcr.html

[Q36] 左连接
来源：http://hz.yuxming.cn/gtemwnxpvj.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.yj20258.top/gtwtkpyvhm.html

[Q37] 右连接
来源：http://hz.cdnleiting.top/gtsotodssv.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.ybcxt.top/gtvkadcuuh.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.gotoacloud.top/gtvyjjhxuq.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.zhiwuduotai.top/gtgvrivrwx.html

[Q39] 自连接（查上下级）
来源：http://hz.zhongyouzk.top/gtfpuepjnw.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.svipenyu.cn/gtbpjtpaqo.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.hnqzz.top/gtlebviqxm.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.nanxuanxn.top/gtfshrvebm.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.gotoacloud.top/gtefddfxid.html

[Q41] 多表连接
来源：http://hz.mhx1999.top/gtriofvnuu.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.shanyushiyangkeji.top/gtmckigter.html

JOIN users u ON u.id = o.user_id
来源：http://hz.jiagoushi.top/gtymnafcuu.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.xziqi.cn/gtmuwjzsub.html

[Q42] 连接条件附加过滤
来源：http://hz.yvedp.cn/gtpsbddede.html


<!-- 参考信息 -->