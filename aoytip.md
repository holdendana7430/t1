代发 wailian999

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.yj202588.top/gtoxvhoarb.html

[N06] 判断回文字符串
来源：http://hz.chenjidiqi.icu/gtevcitdyj.html

Py:   s == s[::-1]
来源：http://hz.tian-w.cn/gttjwktgov.html

PHP:  $s === strrev($s);
来源：http://hz.meibo888.top/gtwpffpeau.html

JS:   s === [...s].reverse().join("")
来源：http://hz.nanxinkj.top/gtkownzitc.html

TS:   s === [...s].reverse().join("")
来源：http://hz.hnxiangtu.top/gtxjznsjie.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.cashguo.top/gtkgdjgkbr.html

Go:   // 双指针从两端比较
来源：http://hz.ybcxt.top/gtowlmieoi.html

Ruby: s == s.reverse
来源：http://hz.xylfe.cn/gtslokauor.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.hywenlv.cn/gtogveyyni.html

[N07] 两数之和（返回下标）
来源：http://hz.chenlongwang.top/gtuaqfldmj.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.sxryk.cn/gtotzwdoyb.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.zhijiandao.cn/gtafiexitf.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.zhijiandao.cn/gtoqjxpsgx.html

TS:   // 手写 Map<string, number>
来源：http://hz.cheryme.top/gtifwduhpy.html

Java: // 手写 HashMap
来源：http://hz.yuanzhike.top/gtlddtqyle.html

Go:   // 手写 map[int]int
来源：http://hz.fengsongda.top/gtoptrbiwh.html

Ruby: // 手写 Hash
来源：http://hz.xuetiantiany.cn/gtljqykvlh.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.jinyuanbaomall.cn/gteznisflm.html

[N08] 生成全排列
来源：http://hz.iojbl.cn/gthhbpkzru.html

Py:   itertools.permutations(arr)
来源：http://hz.zhijiandao.cn/gtwaovjnef.html

PHP:  // 手写递归交换
来源：http://hz.yanxiufei.cn/gtiziueekf.html

JS:   // 手写回溯递归
来源：http://hz.hammf.cn/gtddrrtmtn.html

TS:   // 手写回溯递归
来源：http://hz.shzxlz.cn/gtkjtszndu.html

Java: // 手写回溯递归
来源：http://hz.fzhhl.top/gtulsujwfo.html

Go:   // 手写回溯递归
来源：http://hz.xingfuxueyuan.xyz/gtvtmihkir.html

Ruby: arr.permutation.to_a
来源：http://hz.zhijiandao.cn/gtuffdyruf.html

C#:   // 手写回溯递归
来源：http://hz.nanxuanxn.top/gtmseorccl.html

[N09] 栈与队列
来源：http://hz.ydzc1.top/gtmlkmskez.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.redwolf501.top/gtgeauirtc.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.guowangkeji.top/gtvefzipbv.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.zhoulong.xyz/gtdkpcoblm.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.cheryme.top/gtexabfsrd.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.birdmap.top/gtgexejgqd.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.fzhhl.top/gtfkucofeq.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.tian-w.cn/gtnaufgdkx.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.aizwys.cn/gtnuikrvrr.html

[N10] 链表节点定义
来源：http://hz.tanke756.top/gtxirtiekq.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.hywenlv.cn/gtgrsxpibt.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.shzxlz.cn/gtjcftfjgz.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.andypj.xyz/gtrimmkvfz.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.chenzaomai.com/gtvafphnhq.html

Java: class Node { int v; Node next; }
来源：http://hz.hnxiangtu.top/gtvtamcoiv.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.bjfxy.top/gtmvujhkqw.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.ivvv.top/gtdxdmimin.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.hongshengwenyu.top/gtinbomukd.html

[N11] 二叉树中序遍历
来源：http://hz.hysaishi.cn/gtkmnvkwvx.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.yonumen.top/gtsrlncowp.html

PHP:  // 手写递归函数
来源：http://hz.pycfn.com/gtswfomzgw.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.birdmap.top/gtcztvcdpm.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.jlsjyb.cn/gtiqxoppmt.html

Java: // 手写递归
来源：http://hz.vqdsnc.cn/gtfllnvxnv.html

Go:   // 手写递归
来源：http://hz.jlsjyb.cn/gtvgwakoru.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.xuanzx.com/gtrwrptldl.html

C#:   // 手写递归
来源：http://hz.nanxuanxn.top/gtchkhurvy.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.guannengcc.top/gtntoqvcfg.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.dashuyun.cn/gtnkdkziwq.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.vqdsnc.cn/gtseioeqha.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.c1oappe.top/gtqjddmrav.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.iojbl.cn/gtdmcaicgd.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.xziqi.cn/gtcjxbnzuv.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.vqdsnc.cn/gtvhifouyz.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.shzxlz.cn/gtyitutble.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.jinghuilouyu.cn/gtubhxuwbq.html

================================================================================
来源：http://hz.ydzc1.top/gtiliozexj.html

O. 并发与异步
来源：http://hz.hongshengwenyu.top/gteltlajim.html

================================================================================
来源：http://hz.havefunace.top/gtwoxkkhqn.html

[O01] 启动一个线程
来源：http://hz.smart0.xyz/gtpvvtbnbd.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.wangdashe.top/gtwfneuaak.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.kuanghao11.cn/gtaweukiii.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.havefunace.top/gttldizgzs.html

TS:   // 同 JS
来源：http://hz.birdmap.top/gtvficwgpt.html

Java: new Thread(() -> f()).start()
来源：http://hz.guowangkeji.top/gtkihalgdq.html

Go:   go f()
来源：http://hz.yangfankeji.com/gtgqjxtkij.html

Ruby: Thread.new { f }
来源：http://hz.havefunace.top/gtuqounpjy.html

C#:   Task.Run(() => F());
来源：http://hz.mhx1999.top/gtkoeqfyyt.html

[O02] 使用线程池
来源：http://hz.zycfv.cn/gtodcxhamq.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.kuanghao11.cn/gtrxbsniti.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.aibaodan.cn/gthaazquop.html

JS:   // worker_threads 线程池
来源：http://hz.zhengqikj.top/gtalzelzjr.html

TS:   // worker_threads 线程池
来源：http://hz.hnxiangtu.top/gtdipiktzm.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.chenlongwang.top/gtkdrnbypn.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.yongpay.top/gttctmtxzu.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.0kj1m.cn/gtctomppdd.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.bjfxy.top/gtlvmoafjk.html

[O03] 加锁保护共享数据
来源：http://hz.vqdsnc.cn/gtqwzgpapp.html

Py:   with lock: shared += 1
来源：http://hz.mhx1999.top/gtmmgcbnxe.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.quarkkingdee.top/gtebxkoezw.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.daria6918.cn/gtugkcsfuj.html

TS:   // 同 JS
来源：http://hz.hongshengwenyu.top/gtzksledtt.html

Java: synchronized (this) { shared++; }
来源：http://hz.xinyue.icu/gtbemcfiez.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.ydjk.org.cn/gtbmlizflt.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.xziqi.cn/gtwlvoltzi.html

C#:   lock (gate) { shared++; }
来源：http://hz.dashuyun.cn/gtutycbqnt.html

[O04] 定义异步函数并等待
来源：http://hz.nanxuanxn.top/gtqxvtsmqe.html

Py:   async def f():⏎    await g()
来源：http://hz.zhijiandao.cn/gtljbiybgm.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.ydjk.org.cn/gtgbxkgvov.html

JS:   async function f() { await g(); }
来源：http://hz.yongpay.top/gtfpigvoyt.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.snrcjt.cn/gtzoghivez.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.shanyushiyangtech.top/gtoqpohdho.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.zhengqikj.top/gtdmiconyy.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.zhongyouzk.top/gtwvgvlrzw.html

C#:   async Task F() { await G(); }
来源：http://hz.jqgfzy.top/gtyqakffzg.html

[O05] 并发执行并等待全部完成
来源：http://hz.zhijiandao.cn/gtkctjsvhz.html

Py:   asyncio.gather(*tasks)
来源：http://hz.hywenlv.cn/gtbuuipfhs.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.hnxiangtu.top/gtznsrazvh.html

JS:   await Promise.all(tasks)
来源：http://hz.cucudq.cn/gtlildksqm.html

TS:   await Promise.all(tasks)
来源：http://hz.feifeiyinyue.top/gtucmdhgxm.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.xingfuxueyuan.xyz/gtsbucemqc.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.yangfankeji.com/gtfjlhmwrr.html

Ruby: threads.map(&:join)
来源：http://hz.bjfxy.top/gtsqasqibi.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.jinyuanbaomall.cn/gtlvcshhek.html

[O06] 使用进程池
来源：http://hz.yangfankeji.com/gtozdffhge.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.c1oappe.top/gtcytvzdfh.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.chenjidiqi.icu/gttgehtnwr.html

JS:   // child_process / cluster 模块
来源：http://hz.ehwqpu.com/gtrgedydol.html

TS:   // child_process / cluster 模块
来源：http://hz.ywan-chungtsiang.top/gtfhxgyvxp.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.yvedp.cn/gteuucucnn.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.chenlongwang.top/gtymbrtjry.html

Ruby: // fork 块
来源：http://hz.tanke756.top/gtpxywdoiq.html

C#:   Parallel.For
来源：http://hz.nanxuanxn.top/gtggprjiid.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtgnzhyhov.html

P. 常用工具函数
来源：http://hz.ydjk.org.cn/gtmvlayzvl.html

================================================================================
来源：http://hz.tianlin.xyz/gtkqfuqyfg.html

[P01] 生成 UUID
来源：http://hz.zhiwuduotai.top/gtwlaaxfxx.html

Py:   str(uuid.uuid4())
来源：http://hz.fengsongda.top/gtjzbqjenn.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.svipenyu.cn/gtbfbrporf.html

JS:   crypto.randomUUID()
来源：http://hz.hywenlv.cn/gtafixujow.html

TS:   crypto.randomUUID()
来源：http://hz.jyoumei.cn/gteeiajuaq.html

Java: UUID.randomUUID().toString()
来源：http://hz.hnqzz.top/gtsxamilew.html

Go:   // 用 github.com/google/uuid
来源：http://hz.quarkkingdee.top/gtjnxnvbpi.html

Ruby: SecureRandom.uuid
来源：http://hz.aibaodan.cn/gtthnuqwef.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.zhixingplan.top/gtkslvpnuy.html

[P02] MD5 / SHA256 摘要
来源：http://hz.shangyingyoupin.top/gtdayotkhz.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.jyoumei.cn/gtwvtppztc.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.hammf.cn/gturryeuvf.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.haohaochexian.top/gttqhkpedg.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.kuanghao11.cn/gtimlvfgub.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.xziqi.cn/gtazoqwvbg.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.ydjk.org.cn/gtrydupibm.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.redwolf501.top/gtkbvdncdx.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.cashguo.top/gtsyzoguas.html

[P03] 生成短随机字符串
来源：http://hz.shzxlz.cn/gtchaqjqzl.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.redwolf501.top/gtuambtdiw.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.havefunace.top/gtartomyue.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.jiagoushi.top/gtjgbfvkpk.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.zhengqikj.top/gtbyfynppk.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.shzxlz.cn/gtstyhgmjk.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.ybcxt.top/gtfjwoawrc.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.nanxuanxn.top/gtnwdtiyxk.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.cucudq.cn/gtohgrahib.html

[P04] 求长度
来源：http://hz.cucudq.cn/gtnyqpuojk.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.fzhhl.top/gtecswafog.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.c1oappe.top/gtdfyndyit.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.aibaodan.cn/gtaqfwfbft.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.chenlongwang.top/gtxvnbhcmj.html

Java: list.size();  map.size();  s.length()
来源：http://hz.9152youxi.cn/gtqndpdlgr.html

Go:   len(arr);  len(m)
来源：http://hz.xuetiantiany.cn/gtfqyjpefo.html

Ruby: x.length;  x.size
来源：http://hz.yangfankeji.com/gtsjwxmbze.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.pycfn.com/gtgqulxpfn.html

[P05] 判断两个对象内容是否相等
来源：http://hz.jinghuilouyu.cn/gtmfcsmlbr.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.ydzc1.top/gtzmusjtwx.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.shanyushiyangtech.top/gtzxcaiwzh.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.chenzaomai.com/gtopaxtwey.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.zdqjudy.top/gtvdexcama.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.cqqwz.cn/gtacobwsts.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.xylfe.cn/gtiqfdkdld.html

Ruby: a == b
来源：http://hz.zhongyouzk.top/gtjjpcdakx.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.zhongyouzk.top/gtggugzwtf.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.quarkkingdee.top/gtqdvtvfkz.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.yuanzhike.top/gtruhyjhxf.html

PHP:  if (empty($x)) {}
来源：http://hz.shanyushiyangtech.top/gtvduyfofl.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.316326.xyz/gtpoossmco.html

TS:   if (x == null) {}
来源：http://hz.svipenyu.cn/gtqbmkvhky.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.cheryme.top/gtmrmrjkyu.html

Go:   if x == nil {}
来源：http://hz.shuidangran.top/gthgnqddii.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.meibo888.top/gtpcmempaw.html

C#:   if (x is null) {}
来源：http://hz.shzxlz.cn/gtpzzdaupm.html

[P07] 防抖与节流
来源：http://hz.gzhubu.top/gtoahjerex.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.hongshengwenyu.top/gtemthvioe.html

PHP:  // 手写时间戳比较
来源：http://hz.wangdashe.top/gtzjnksbph.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.yonumen.top/gtolfhaoak.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.shanyushiyangtech.top/gtcmbfukrd.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.gaohongyu789.top/gtpsvndywh.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.cashguo.top/gtvvozwteo.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.snrcjt.cn/gtixbnmdpd.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.zhijiandao.cn/gtmksafghj.html

[P08] 处理浮点精度问题
来源：http://hz.hysaishi.cn/gtwtscsyud.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.xinyue.icu/gtcllkslnp.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.jinyuanbaomall.cn/gtlqdmyuby.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.yj202588.top/gtefdobmnh.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.zhoulong.xyz/gtssncxiyb.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.hfpthk.cn/gtjneglznm.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.meibo888.top/gtxrzdlmkn.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.quarkkingdee.top/gtqlvqhuzr.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.wangdashe.top/gtdpymcupl.html

================================================================================
来源：http://hz.hysaishi.cn/gtadyrpjll.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.zdqjudy.top/gtlyefpxil.html

================================================================================
来源：http://hz.sxryk.cn/gtreigwsdz.html

[Q01] 创建表
来源：http://hz.ydzc1.top/gtslqfgsyn.html

CREATE TABLE users (
来源：http://hz.hnqzz.top/gtftkigdts.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.yvedp.cn/gteiknhsuo.html

name VARCHAR(50) NOT NULL,
来源：http://hz.gogol.net.cn/gtootftiid.html

email VARCHAR(100) UNIQUE,
来源：http://hz.sufxvd.cn/gtxcmadyuo.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.zhijiandao.cn/gtmibylqor.html

);
来源：http://hz.yonumen.top/gtzcljupii.html

[Q02] 创建带外键的表
来源：http://hz.jinyuanbaomall.cn/gtnidwxkgg.html

CREATE TABLE orders (
来源：http://hz.jqgfzy.top/gtfltyaphi.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.xuetiantiany.cn/gtbmgciitd.html

user_id INT NOT NULL,
来源：http://hz.jinyuanbaomall.cn/gthqglkfsq.html

amount DECIMAL(10, 2),
来源：http://hz.haohaochexian.top/gtaxzjlpeh.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.aibaodan.cn/gtrrqcrbll.html

);
来源：http://hz.chenzaomai.com/gtqlwqrsfq.html

[Q03] 增加列
来源：http://hz.yanxiufei.cn/gtehlraats.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.jinqigufen.top/gtyvvaccaj.html

[Q04] 修改列类型
来源：http://hz.svipenyu.cn/gtpgoujbsz.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.zycfv.cn/gtkrzvgyir.html

[Q05] 重命名列
来源：http://hz.52xcode.cn/gtwzijcmsa.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.c1oappe.top/gtzhjksjyi.html

[Q06] 删除列
来源：http://hz.andypj.xyz/gtglywours.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.aizwys.cn/gtwzsefryh.html

[Q07] 删除表
来源：http://hz.jinqigufen.top/gtytttdzfd.html

DROP TABLE IF EXISTS orders;
来源：http://hz.cashguo.top/gthucekauh.html

[Q08] 创建普通索引
来源：http://hz.0kj1m.cn/gtnzhacppc.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.sweek.top/gtfmixynem.html

[Q09] 创建唯一索引
来源：http://hz.zhixingplan.top/gtuuchucpq.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.52xcode.cn/gtacyjreic.html

[Q10] 插入单行
来源：http://hz.zhaomingkeji.xyz/gtibuzjdii.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.aizwys.cn/gtkbnnzykq.html

[Q11] 一次插入多行
来源：http://hz.yuxming.cn/gtdvasuomn.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.yuxming.cn/gtsoztgupv.html

[Q12] 插入后取自增 ID
来源：http://hz.jinghuilouyu.cn/gtqfecvkra.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.bjfxy.top/gttisvetsh.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.hysaishi.cn/gtrnfexcgg.html

[Q13] 忽略重复插入
来源：http://hz.dianchejie.cn/gtomgmhoqd.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.birdmap.top/gtknlitxgc.html

[Q14] 存在则更新（upsert）
来源：http://hz.guannengcc.top/gtvkhgnkey.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.xinyue.icu/gtogynvjvy.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.yanxiufei.cn/gtvrphdytf.html

[Q15] 查询全部
来源：http://hz.shuidangran.top/gtfrbednuj.html

SELECT * FROM users;
来源：http://hz.chenjidiqi.icu/gtqwzfhomy.html

[Q16] 查询指定列
来源：http://hz.pycfn.com/gtsnhkjkeg.html

SELECT id, name FROM users;
来源：http://hz.zdqjudy.top/gthebeuphj.html

[Q17] 条件查询
来源：http://hz.mhx1999.top/gtqdxnvopu.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.vqdsnc.cn/gtiuljhkbl.html

[Q18] 模糊匹配
来源：http://hz.xingfuxueyuan.xyz/gtnuxoynzz.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.gogol.net.cn/gtusaoqetl.html

[Q19] 范围查询
来源：http://hz.sysykeji.top/gtvkllcjfo.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.zhixingplan.top/gtzhlqjewl.html

[Q20] IN 列表
来源：http://hz.nanxuanxn.top/gtwrdmpkvr.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.pycfn.com/gtibmthump.html

[Q21] 空值判断
来源：http://hz.shanyushiyangkeji.top/gtizvlfpmd.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.havefunace.top/gtbemtrbmp.html

[Q22] 排序
来源：http://hz.tianlin.xyz/gtdgqxzmpp.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.sysykeji.top/gtfcdbgnoi.html

[Q23] 分页
来源：http://hz.jqgufenzy.top/gtuwptsatj.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.yj20258.top/gtplqvhcxi.html

[Q24] 去重
来源：http://hz.52xcode.cn/gtkvlbbgtm.html

SELECT DISTINCT city FROM users;
来源：http://hz.yonumen.top/gtmnflzgqh.html

[Q25] 只取前 N 条
来源：http://hz.gzhubu.top/gtlutwheyi.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.hnqzz.top/gtavaojsvg.html

[Q26] 计数
来源：http://hz.wangshuangyany.cn/gtkwvrakel.html

SELECT COUNT(*) FROM users;
来源：http://hz.yj202588.top/gtipfmsgbq.html

[Q27] 条件计数
来源：http://hz.nwbrower.top/gtwsgiioyg.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.nanxuanxn.top/gtleiszzfb.html

[Q28] 求和与平均
来源：http://hz.aizwys.cn/gtmuoobzib.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.meibo888.top/gtcgxtylxo.html

[Q29] 最大最小值
来源：http://hz.yueranfly.top/gtaciigbty.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.ybcxt.top/gtxzlnktlp.html

[Q30] 分组统计
来源：http://hz.havefunace.top/gtaljjlydf.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.jinqigfzy.top/gttaabcpvi.html

[Q31] 分组后过滤
来源：http://hz.snrcjt.cn/gtlgzlmylf.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.feifeiyinyue.top/gtgfcgjwpx.html

[Q32] 分组拼接字符串
来源：http://hz.jiagoushi.top/gtyihbldxp.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.dianchejie.cn/gtvpyaryum.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.shanyushiyangkeji.top/gtdfahredr.html

[Q33] 多列分组
来源：http://hz.jinghuilouyu.cn/gtrvygiszs.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.jinqigfzy.top/gtncgljqdq.html

[Q34] 每组取第一条
来源：http://hz.shanyushiyangkeji.top/gthffmkuua.html

SELECT * FROM (
来源：http://hz.zhengqikj.top/gtqpzojvql.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.yj202588.top/gtjlrlbzob.html

) t WHERE rn = 1;
来源：http://hz.hammf.cn/gtrsctckim.html

[Q35] 内连接
来源：http://hz.meibo888.top/gthbciigtu.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.gaohongyu789.top/gtmxekzxer.html

[Q36] 左连接
来源：http://hz.xinyue.icu/gtoitiqule.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.cdnleiting.top/gtlmllstaq.html

[Q37] 右连接
来源：http://hz.0kj1m.cn/gtmupcetzy.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.hywenlv.cn/gtvcgtzvfu.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.hnqzz.top/gtfsljvlme.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.hfpthk.cn/gtbooiiebn.html

[Q39] 自连接（查上下级）
来源：http://hz.iojbl.cn/gtofzhkeot.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.zhiwuduotai.top/gtfsfklase.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.c1oappe.top/gtjpsqdwcy.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.zhongyouzk.top/gtvoxwgvoe.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.vqdsnc.cn/gtdxxihmal.html

[Q41] 多表连接
来源：http://hz.hfpthk.cn/gtvhiumjal.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.snrcjt.cn/gtehwqtemn.html

JOIN users u ON u.id = o.user_id
来源：http://hz.ybcxt.top/gtfkvgocog.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.sweek.top/gtvliembty.html

[Q42] 连接条件附加过滤
来源：http://hz.smart0.xyz/gtxpjlqcog.html


<!-- 参考信息 -->