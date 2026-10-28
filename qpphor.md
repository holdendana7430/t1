代发 wailian999

[N05] 最大公约数
来源：http://hz.meibo888.top/gtzzgnbpva.html

Py:   math.gcd(a, b)
来源：http://hz.wangshuangyany.cn/gtymujmflj.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.ydzc1.top/gtboxswuid.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.jyoumei.cn/gtaehbvlml.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.c1oappe.top/gtbkafzxcs.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.sweek.top/gteclhqgsr.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.pengpengdd.cyou/gtfpabfule.html

Ruby: a.gcd(b)
来源：http://hz.gogol.net.cn/gtncwzgtim.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.shanyushiyangkeji.top/gtfgickahi.html

[N06] 判断回文字符串
来源：http://hz.yuxming.cn/gthtzadufr.html

Py:   s == s[::-1]
来源：http://hz.cucudq.cn/gtyknthpkq.html

PHP:  $s === strrev($s);
来源：http://hz.ydzc1.top/gtwoyqouty.html

JS:   s === [...s].reverse().join("")
来源：http://hz.ehwqpu.com/gtqrzwqtnt.html

TS:   s === [...s].reverse().join("")
来源：http://hz.zhoulong.xyz/gtndoqwtbq.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.yangfankeji.com/gtidqngplh.html

Go:   // 双指针从两端比较
来源：http://hz.hywenlv.cn/gthxeoogei.html

Ruby: s == s.reverse
来源：http://hz.wangdashe.top/gtodrphlzh.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.c1oappe.top/gtlobamcyk.html

[N07] 两数之和（返回下标）
来源：http://hz.shanyushiyangtech.top/gtwfmzlasv.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.jqgfzy.top/gtprvtbluk.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.hnqzz.top/gtyayqsbnk.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.yangfankeji.com/gtcwrbghcv.html

TS:   // 手写 Map<string, number>
来源：http://hz.jlsjyb.cn/gtvmfktoii.html

Java: // 手写 HashMap
来源：http://hz.yangfankeji.com/gtajdlblzm.html

Go:   // 手写 map[int]int
来源：http://hz.yj202588.top/gtkemeqwzs.html

Ruby: // 手写 Hash
来源：http://hz.tanke756.top/gtrbeaoxpv.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.haohaochexian.top/gtftppojdp.html

[N08] 生成全排列
来源：http://hz.yvedp.cn/gtmbnebujp.html

Py:   itertools.permutations(arr)
来源：http://hz.hongshengwenyu.top/gtajbxpduk.html

PHP:  // 手写递归交换
来源：http://hz.xinyue.icu/gtroevcusm.html

JS:   // 手写回溯递归
来源：http://hz.xuetiantiany.cn/gtkecyajdr.html

TS:   // 手写回溯递归
来源：http://hz.aibaodan.cn/gtppnujtuk.html

Java: // 手写回溯递归
来源：http://hz.yuxming.cn/gtozbexdmh.html

Go:   // 手写回溯递归
来源：http://hz.shangyingyoupin.top/gtfhyttgez.html

Ruby: arr.permutation.to_a
来源：http://hz.gogol.net.cn/gtaebipdww.html

C#:   // 手写回溯递归
来源：http://hz.9152youxi.cn/gtrsvrbdjt.html

[N09] 栈与队列
来源：http://hz.ydzc1.top/gtzrrkyjms.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.tian-w.cn/gtbwepzgyh.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.9152youxi.cn/gtqgxkzedq.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.aizwys.cn/gtxbmbjjfs.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.cqqwz.cn/gtksatxdiy.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.iojbl.cn/gthpsgqvqd.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.ehwqpu.com/gtcvbrnpep.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.yanxiufei.cn/gtrpyeaiyu.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.haohaochexian.top/gtfyzeqpnk.html

[N10] 链表节点定义
来源：http://hz.iojbl.cn/gtwmoweusm.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.nwbrower.top/gtoeacakdt.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.bjfxy.top/gtjuexvtkt.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.sweek.top/gtzrzanihx.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.nwbrower.top/gtlseahksr.html

Java: class Node { int v; Node next; }
来源：http://hz.yuxming.cn/gtedxhtllk.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.jlsjyb.cn/gtzldrxjzw.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.jlsjyb.cn/gtlvofdgos.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.aibaodan.cn/gthjbaxttw.html

[N11] 二叉树中序遍历
来源：http://hz.zhaomingkeji.xyz/gtrljqbnix.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.gaohongyu789.top/gtlheavlyw.html

PHP:  // 手写递归函数
来源：http://hz.yanxiufei.cn/gttrcewaod.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.hysaishi.cn/gtzcxieweo.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.hysaishi.cn/gttvqzcvtk.html

Java: // 手写递归
来源：http://hz.hnxiangtu.top/gtzzpiokzl.html

Go:   // 手写递归
来源：http://hz.chenjidiqi.icu/gthokjftes.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.svipenyu.cn/gtrrttnnkc.html

C#:   // 手写递归
来源：http://hz.sweek.top/gtybfhelhl.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.andypj.xyz/gtmkgppwys.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.zhongyouzk.top/gtdyyrkwll.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.svipenyu.cn/gtqzkdaezh.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.aizwys.cn/gttjfvixrd.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.gaohongyu789.top/gtkjzsrddj.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.wangshuangyany.cn/gtffomkypu.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.jinqigfzy.top/gtqatgmsln.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.ivvv.top/gtrvbelvyc.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.pycfn.com/gtbatohect.html

================================================================================
来源：http://hz.meibo888.top/gtsfldhdrv.html

O. 并发与异步
来源：http://hz.yj202588.top/gtzksaizrr.html

================================================================================
来源：http://hz.zhoulong.xyz/gtgozsbokd.html

[O01] 启动一个线程
来源：http://hz.sufxvd.cn/gtqlxirbbw.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.cheryme.top/gtrizdwpgt.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.cheryme.top/gtzyqojukh.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.vqdsnc.cn/gtrzbjtzpj.html

TS:   // 同 JS
来源：http://hz.ehwqpu.com/gtskrzrqip.html

Java: new Thread(() -> f()).start()
来源：http://hz.shangyingyoupin.top/gtvdhujwhw.html

Go:   go f()
来源：http://hz.guowangkeji.top/gtymsakkli.html

Ruby: Thread.new { f }
来源：http://hz.aibaodan.cn/gtytholxlv.html

C#:   Task.Run(() => F());
来源：http://hz.cqqwz.cn/gtdmgvqkft.html

[O02] 使用线程池
来源：http://hz.fzhhl.top/gtuiodsxar.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.jianghu66.top/gtnveyfadt.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.quarkkingdee.top/gtfpfzzfvw.html

JS:   // worker_threads 线程池
来源：http://hz.jlsjyb.cn/gtqxxdgpbw.html

TS:   // worker_threads 线程池
来源：http://hz.gzhubu.top/gtgqxipajh.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.andypj.xyz/gtedpikegu.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.hnqzz.top/gtrpxacnji.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.sxryk.cn/gtgoqkdyig.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.c1oappe.top/gtujoadnpb.html

[O03] 加锁保护共享数据
来源：http://hz.smart0.xyz/gtmqbydcyo.html

Py:   with lock: shared += 1
来源：http://hz.snrcjt.cn/gthomvkzar.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.xuanzx.com/gttremlkiu.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.jinqigufen.top/gtmuzukyho.html

TS:   // 同 JS
来源：http://hz.jqgufenzy.top/gthuaiormv.html

Java: synchronized (this) { shared++; }
来源：http://hz.aizwys.cn/gtpwkzxvli.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.sxryk.cn/gtfqrajtyi.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.daxiang520.top/gtbvbxyvde.html

C#:   lock (gate) { shared++; }
来源：http://hz.nanxuanxn.top/gtrgkpsoto.html

[O04] 定义异步函数并等待
来源：http://hz.aizwys.cn/gttqkherdv.html

Py:   async def f():⏎    await g()
来源：http://hz.yj202588.top/gtwutllfmy.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.ppjwa.cn/gtjybjtusn.html

JS:   async function f() { await g(); }
来源：http://hz.zhijiandao.cn/gtseajkuii.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.yanxiufei.cn/gtiriwocfl.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.zhaomingkeji.xyz/gtspnqphdv.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.tian-w.cn/gtiyzabhcd.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.zhiwuduotai.top/gtqxdfgrpa.html

C#:   async Task F() { await G(); }
来源：http://hz.0kj1m.cn/gtcsjwchwd.html

[O05] 并发执行并等待全部完成
来源：http://hz.hammf.cn/gtygeyzipj.html

Py:   asyncio.gather(*tasks)
来源：http://hz.smart0.xyz/gtvdkitujy.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.yj20258888.top/gtmfdrmrlx.html

JS:   await Promise.all(tasks)
来源：http://hz.sufxvd.cn/gttbmobwsu.html

TS:   await Promise.all(tasks)
来源：http://hz.fzhhl.top/gtvzllpael.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.xziqi.cn/gtjkbgahnm.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.yj20258.top/gtilseltzl.html

Ruby: threads.map(&:join)
来源：http://hz.ppjwa.cn/gttxezkgpf.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.yongpay.top/gtfgpmkvbb.html

[O06] 使用进程池
来源：http://hz.birdmap.top/gtnmmxhzir.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.yvedp.cn/gtdkjgrgbh.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.hammf.cn/gtvcaplggo.html

JS:   // child_process / cluster 模块
来源：http://hz.nanxuanxn.top/gtmbpphakn.html

TS:   // child_process / cluster 模块
来源：http://hz.vqdsnc.cn/gtwexdyscy.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.bjfxy.top/gtmzifkeby.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.chenzaomai.com/gtsakimtra.html

Ruby: // fork 块
来源：http://hz.yj20258.top/gtozkongxv.html

C#:   Parallel.For
来源：http://hz.cucudq.cn/gtvrufnrko.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gtsiexxyim.html

P. 常用工具函数
来源：http://hz.jiagoushi.top/gtwpozeovx.html

================================================================================
来源：http://hz.daxiang520.top/gtotpugjrd.html

[P01] 生成 UUID
来源：http://hz.zhiwuduotai.top/gtoulovdau.html

Py:   str(uuid.uuid4())
来源：http://hz.chenlongwang.top/gtggvqfajp.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.ivvv.top/gtlnnkwxku.html

JS:   crypto.randomUUID()
来源：http://hz.xingfuxueyuan.xyz/gtutrrflzs.html

TS:   crypto.randomUUID()
来源：http://hz.ehwqpu.com/gtmhjompxo.html

Java: UUID.randomUUID().toString()
来源：http://hz.iojbl.cn/gtvcwxtqgn.html

Go:   // 用 github.com/google/uuid
来源：http://hz.cucudq.cn/gtwzpaokoi.html

Ruby: SecureRandom.uuid
来源：http://hz.nanxinkj.top/gthfqlqfjl.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.nwbrower.top/gthjapxkrt.html

[P02] MD5 / SHA256 摘要
来源：http://hz.yvedp.cn/gtfyauolkg.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.hammf.cn/gtwtzwbdot.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.iojbl.cn/gtzbftkcbt.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.ehwqpu.com/gtshqrvwsh.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.yvedp.cn/gtfprvluxx.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.tianlin.xyz/gtdeuoqwgj.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.zhengqikj.top/gtocljadok.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.smart0.xyz/gtyxqawgcj.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.snrcjt.cn/gtyfdqqupc.html

[P03] 生成短随机字符串
来源：http://hz.jinqigufen.top/gtnkchcwmj.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.gzhubu.top/gtjtcdngdo.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.redwolf501.top/gtjaghpxjh.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.iojbl.cn/gtkizffopn.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.yueranfly.top/gtiwfdmwzn.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.zhoulong.xyz/gtjriymtnu.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.0kj1m.cn/gtwcmdhuqq.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.zhaomingkeji.xyz/gtaxaexcdk.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.cqqwz.cn/gtmhttwpkg.html

[P04] 求长度
来源：http://hz.9152youxi.cn/gtwohsgmot.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.jinqigfzy.top/gtakezbtrf.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.snrcjt.cn/gtpaxnpdpm.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.havefunace.top/gtnpzpemsk.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.chenlongwang.top/gtwpnkoeyi.html

Java: list.size();  map.size();  s.length()
来源：http://hz.tianlin.xyz/gtouujowil.html

Go:   len(arr);  len(m)
来源：http://hz.gogol.net.cn/gtutamqvgg.html

Ruby: x.length;  x.size
来源：http://hz.ehwqpu.com/gtumqzyqhl.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.ydzc1.top/gtwvxabbvr.html

[P05] 判断两个对象内容是否相等
来源：http://hz.birdmap.top/gtkpmaxucm.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.gotoacloud.top/gtmorgcizu.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.hongshengwenyu.top/gtwmjimhvl.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.shanyushiyangtech.top/gtddocilnn.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.xuanzx.com/gthjcrcehi.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.hnxiangtu.top/gtikoaladz.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.chenlongwang.top/gtrigntaxv.html

Ruby: a == b
来源：http://hz.cheryme.top/gtnjowzqmq.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.tanke756.top/gtwqjczdvx.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.iojbl.cn/gtluxzzphn.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.nanxuanxn.top/gtfieaqffo.html

PHP:  if (empty($x)) {}
来源：http://hz.jinghuilouyu.cn/gttmzbwdul.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.nanxuanxn.top/gttkkpkapq.html

TS:   if (x == null) {}
来源：http://hz.zhixingplan.top/gtatpdxjlv.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.svipenyu.cn/gtnuahosqf.html

Go:   if x == nil {}
来源：http://hz.ivvv.top/gtyqheofrl.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.0kj1m.cn/gtxxwgigbf.html

C#:   if (x is null) {}
来源：http://hz.wangshuangyany.cn/gtyhuxfenf.html

[P07] 防抖与节流
来源：http://hz.zycfv.cn/gtwvirziqi.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.hfpthk.cn/gtjedhlytz.html

PHP:  // 手写时间戳比较
来源：http://hz.aizwys.cn/gtwggjpzzb.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.chenlongwang.top/gtysnwfcbu.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.jyoumei.cn/gtsfdvsanu.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.jianghu66.top/gtzjuthffe.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.dianchejie.cn/gtvfdsiwao.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.xuetiantiany.cn/gtimtzckgp.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.jqgfzy.top/gtrdeifaxc.html

[P08] 处理浮点精度问题
来源：http://hz.xingfuxueyuan.xyz/gtqvpghczq.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.jinqigfzy.top/gtyvgwiwae.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.cdnleiting.top/gtkmajbcpx.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.jlsjyb.cn/gtxohfaeap.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.yj20258888.top/gtvhckxteb.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.snrcjt.cn/gttggqrxyi.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.zhiwuduotai.top/gtltwzxobq.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.gogol.net.cn/gtipqwzdbx.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.jinyuanbaomall.cn/gtvszqigcr.html

================================================================================
来源：http://hz.dashuyun.cn/gtqunzbxgd.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.ehwqpu.com/gtclfaoacn.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtysiirpbd.html

[Q01] 创建表
来源：http://hz.sufxvd.cn/gtfvqlciai.html

CREATE TABLE users (
来源：http://hz.chenzaomai.com/gtnoxxcdpe.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.yueranfly.top/gtirjejgcv.html

name VARCHAR(50) NOT NULL,
来源：http://hz.yvedp.cn/gtpxczdnxx.html

email VARCHAR(100) UNIQUE,
来源：http://hz.ppjwa.cn/gtflrlxsnm.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.jinqigufen.top/gtgubxtkmm.html

);
来源：http://hz.jqgfzy.top/gtjmupsmhh.html

[Q02] 创建带外键的表
来源：http://hz.fzhhl.top/gtnmoyfclh.html

CREATE TABLE orders (
来源：http://hz.zdqjudy.top/gtzvwogtsa.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.jlsjyb.cn/gtwkfuowfv.html

user_id INT NOT NULL,
来源：http://hz.jinyuanbaomall.cn/gtrknyxcvr.html

amount DECIMAL(10, 2),
来源：http://hz.yonumen.top/gtqjjfimnc.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.dianchejie.cn/gtwdgfrpwr.html

);
来源：http://hz.zhijiandao.cn/gtfvaqgswa.html

[Q03] 增加列
来源：http://hz.cqqwz.cn/gtlpqqsfcw.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.gzhubu.top/gtzmcmiewt.html

[Q04] 修改列类型
来源：http://hz.yanxiufei.cn/gtppgiqzuz.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.hammf.cn/gtexwrtbgh.html

[Q05] 重命名列
来源：http://hz.havefunace.top/gttktnrrux.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.chenjidiqi.icu/gtotczswke.html

[Q06] 删除列
来源：http://hz.jinyuanbaomall.cn/gtvececwzc.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.jinqigfzy.top/gtsibxmlox.html

[Q07] 删除表
来源：http://hz.haohaochexian.top/gtevamawby.html

DROP TABLE IF EXISTS orders;
来源：http://hz.fzhhl.top/gtjpzxcmmf.html

[Q08] 创建普通索引
来源：http://hz.ywan-chungtsiang.top/gtvfamhvyj.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.sufxvd.cn/gtfdjfjkeh.html

[Q09] 创建唯一索引
来源：http://hz.tanke756.top/gttrrookfp.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.cashguo.top/gtwgckrgcs.html

[Q10] 插入单行
来源：http://hz.yvedp.cn/gtfgqvwefg.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.wangshuangyany.cn/gtjqmzjexk.html

[Q11] 一次插入多行
来源：http://hz.xylfe.cn/gtubxjgatd.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.mhx1999.top/gtbajskmzy.html

[Q12] 插入后取自增 ID
来源：http://hz.0kj1m.cn/gtddycxqdh.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.yuxming.cn/gtwpnmtuts.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.bjfxy.top/gtwqumjznn.html

[Q13] 忽略重复插入
来源：http://hz.meibo888.top/gtigvluqys.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.yj20258.top/gtqrhxmwyu.html

[Q14] 存在则更新（upsert）
来源：http://hz.pycfn.com/gtbkflkbiv.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.dashuyun.cn/gtgjpcwiyj.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.zhaomingkeji.xyz/gtzhihpdau.html

[Q15] 查询全部
来源：http://hz.yvedp.cn/gtsktsbiun.html

SELECT * FROM users;
来源：http://hz.meibo888.top/gtivqelbkc.html

[Q16] 查询指定列
来源：http://hz.9152youxi.cn/gteicjpaxa.html

SELECT id, name FROM users;
来源：http://hz.ydzc1.top/gtxhjznrxn.html

[Q17] 条件查询
来源：http://hz.ywan-chungtsiang.top/gtwgnwanom.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.cucudq.cn/gtjrmhrvgv.html

[Q18] 模糊匹配
来源：http://hz.xingfuxueyuan.xyz/gtmgoypuyo.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.jinqigufen.top/gtfohhbzht.html

[Q19] 范围查询
来源：http://hz.ppjwa.cn/gtmmuookhg.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.snrcjt.cn/gtyauxubki.html

[Q20] IN 列表
来源：http://hz.cashguo.top/gtxoehltag.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.zhijiandao.cn/gtfsbapraq.html

[Q21] 空值判断
来源：http://hz.c1oappe.top/gtonjqvedv.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.guowangkeji.top/gtxiymbgad.html

[Q22] 排序
来源：http://hz.tian-w.cn/gtqtjgcyjh.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.9152youxi.cn/gtajqiorch.html

[Q23] 分页
来源：http://hz.cqqwz.cn/gtqnjkuwew.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.daria6918.cn/gtirvvnvac.html

[Q24] 去重
来源：http://hz.hywenlv.cn/gteewujjaq.html

SELECT DISTINCT city FROM users;
来源：http://hz.sxryk.cn/gtttdxtevi.html

[Q25] 只取前 N 条
来源：http://hz.shzxlz.cn/gtfwjonjij.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.jinqigufen.top/gtmikcugca.html

[Q26] 计数
来源：http://hz.chenlongwang.top/gtduwbmpji.html

SELECT COUNT(*) FROM users;
来源：http://hz.cdnleiting.top/gtqrzmdrps.html

[Q27] 条件计数
来源：http://hz.yueranfly.top/gtsupnlqmr.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.hammf.cn/gtcoggloqx.html

[Q28] 求和与平均
来源：http://hz.daxiang520.top/gtidntohot.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.haohaochexian.top/gtfymzdqcp.html

[Q29] 最大最小值
来源：http://hz.shzxlz.cn/gttscodoms.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.iojbl.cn/gtscrxymfd.html

[Q30] 分组统计
来源：http://hz.jlsjyb.cn/gtfyxwyocw.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.zhijiandao.cn/gtzpwldhly.html

[Q31] 分组后过滤
来源：http://hz.zycfv.cn/gtufwwqpxl.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.cqqwz.cn/gtzjnprzab.html

[Q32] 分组拼接字符串
来源：http://hz.iojbl.cn/gtxquvubmw.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.zhaomingkeji.xyz/gtdbbbuhdj.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.0kj1m.cn/gtixbowhgw.html

[Q33] 多列分组
来源：http://hz.xuanzx.com/gtudjudiyp.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.daxiang520.top/gtbljjecme.html

[Q34] 每组取第一条
来源：http://hz.guowangkeji.top/gtsmafzbtr.html

SELECT * FROM (
来源：http://hz.bjfxy.top/gtoqcsixsv.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.guannengcc.top/gtyhoketdi.html

) t WHERE rn = 1;
来源：http://hz.zhengqikj.top/gtrxkodgjm.html

[Q35] 内连接
来源：http://hz.cheryme.top/gtlqialfxi.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.xingfuxueyuan.xyz/gtjcckfkfo.html

[Q36] 左连接
来源：http://hz.yanxiufei.cn/gtyejzbacg.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.tian-w.cn/gtxzsypfqf.html

[Q37] 右连接
来源：http://hz.fengsongda.top/gtrmyvkytd.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.nanxinkj.top/gtqujfblha.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.jqgfzy.top/gttkfxvtub.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.iojbl.cn/gtbmaaqoam.html

[Q39] 自连接（查上下级）
来源：http://hz.gzhubu.top/gtssrkphrv.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.zhixingplan.top/gtqxyhpaei.html


<!-- 参考信息 -->