代发 wailian999

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.chenzaomai.com/gtzjpgkrdq.html

[N06] 判断回文字符串
来源：http://hz.dashuyun.cn/gtpfpzvdeq.html

Py:   s == s[::-1]
来源：http://hz.zhongyouzk.top/gtiomfghxx.html

PHP:  $s === strrev($s);
来源：http://hz.daria6918.cn/gtohufncql.html

JS:   s === [...s].reverse().join("")
来源：http://hz.jiagoushi.top/gtjkfmibtj.html

TS:   s === [...s].reverse().join("")
来源：http://hz.yangfankeji.com/gtmcsonnki.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.zhongyouzk.top/gtdehawuie.html

Go:   // 双指针从两端比较
来源：http://hz.daria6918.cn/gtchmvbymr.html

Ruby: s == s.reverse
来源：http://hz.snrcjt.cn/gtebmgovdz.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.pycfn.com/gtkqfsgyla.html

[N07] 两数之和（返回下标）
来源：http://hz.tanke756.top/gtwrainfix.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.jianghu66.top/gtgeiruivg.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.cheryme.top/gtekqcwfax.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.kuanghao11.cn/gtvtlosmcy.html

TS:   // 手写 Map<string, number>
来源：http://hz.jlsjyb.cn/gtfrbiqmzw.html

Java: // 手写 HashMap
来源：http://hz.wangshuangyany.cn/gtlbkvoyzh.html

Go:   // 手写 map[int]int
来源：http://hz.zhengqikj.top/gtfskrhemk.html

Ruby: // 手写 Hash
来源：http://hz.cheryme.top/gtcovzkhko.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.aizwys.cn/gtnssfccnh.html

[N08] 生成全排列
来源：http://hz.sufxvd.cn/gtwcmlizov.html

Py:   itertools.permutations(arr)
来源：http://hz.hnqzz.top/gtgxweiwtx.html

PHP:  // 手写递归交换
来源：http://hz.ydjk.org.cn/gtxljlmsra.html

JS:   // 手写回溯递归
来源：http://hz.hongshengwenyu.top/gtdktzvgao.html

TS:   // 手写回溯递归
来源：http://hz.cqqwz.cn/gtmlkufuky.html

Java: // 手写回溯递归
来源：http://hz.zhoulong.xyz/gtetzdezya.html

Go:   // 手写回溯递归
来源：http://hz.316326.xyz/gtmtharclf.html

Ruby: arr.permutation.to_a
来源：http://hz.cqqwz.cn/gtgccfsqye.html

C#:   // 手写回溯递归
来源：http://hz.pycfn.com/gtygrlrvzo.html

[N09] 栈与队列
来源：http://hz.shzxlz.cn/gtgpuqscfr.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.jlsjyb.cn/gtcildugjr.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.yj202588.top/gtavisddqc.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.jinqigufen.top/gtqeurgkaq.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.nanxuanxn.top/gtrctkqmyc.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.snrcjt.cn/gtqrwjhjga.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.cucudq.cn/gtzyytvvuw.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.0kj1m.cn/gtjcdzihrv.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.zhoulong.xyz/gtjrtidthv.html

[N10] 链表节点定义
来源：http://hz.smart0.xyz/gtjalttode.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.nanxinkj.top/gtpwoadcda.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.cdnleiting.top/gtqzavgtkq.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.tanke756.top/gtjewvnxep.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.jinghuilouyu.cn/gtqsbzvhji.html

Java: class Node { int v; Node next; }
来源：http://hz.nwbrower.top/gtoarabfmk.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.gogol.net.cn/gtriyagzop.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.hammf.cn/gtkkfcajhj.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.xziqi.cn/gtzzpxjztu.html

[N11] 二叉树中序遍历
来源：http://hz.zhengqikj.top/gtnvcyttpc.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.zhixingplan.top/gtdmusjwtq.html

PHP:  // 手写递归函数
来源：http://hz.gogol.net.cn/gtwdymyxdd.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.shzxlz.cn/gtjphauphx.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.aibaodan.cn/gtmryrclcq.html

Java: // 手写递归
来源：http://hz.tian-w.cn/gtgmvcxojn.html

Go:   // 手写递归
来源：http://hz.yanxiufei.cn/gtrdtldjrr.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.gotoacloud.top/gtelvshbla.html

C#:   // 手写递归
来源：http://hz.bjfxy.top/gtybbamcue.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.cashguo.top/gtobruqpob.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.daria6918.cn/gtralcttmk.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.snrcjt.cn/gtfmdkoikt.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.gogol.net.cn/gtojrxalce.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.haohaochexian.top/gtlsjkkdym.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.fzhhl.top/gtbvmpkyzi.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.fzhhl.top/gtzajnyxdi.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.jlsjyb.cn/gtpagpixde.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.haohaochexian.top/gtnfjoczal.html

================================================================================
来源：http://hz.zhengqikj.top/gtnthowfii.html

O. 并发与异步
来源：http://hz.sxryk.cn/gtfnbfhyxl.html

================================================================================
来源：http://hz.sufxvd.cn/gtwjivqfga.html

[O01] 启动一个线程
来源：http://hz.316326.xyz/gtbdbzomha.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.zhoulong.xyz/gtsyyuqnpv.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.cdnleiting.top/gtfncwureg.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.feifeiyinyue.top/gtysamirpt.html

TS:   // 同 JS
来源：http://hz.jqgufenzy.top/gtrfkkkyer.html

Java: new Thread(() -> f()).start()
来源：http://hz.yj20258.top/gtisvnxytf.html

Go:   go f()
来源：http://hz.havefunace.top/gtfydnaqha.html

Ruby: Thread.new { f }
来源：http://hz.yangfankeji.com/gtsdrhiznr.html

C#:   Task.Run(() => F());
来源：http://hz.zhaomingkeji.xyz/gtwhuhzqca.html

[O02] 使用线程池
来源：http://hz.xylfe.cn/gtkhmweiic.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.hammf.cn/gtjaslumdf.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.cheryme.top/gtvacqtiyr.html

JS:   // worker_threads 线程池
来源：http://hz.xziqi.cn/gteyrdqvvy.html

TS:   // worker_threads 线程池
来源：http://hz.zhaomingkeji.xyz/gtnlnwpciy.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.c1oappe.top/gtujpmdctn.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.xinyue.icu/gtnvgqnnuf.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.yongpay.top/gtfdfvxbwr.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.jyoumei.cn/gtnvquxeox.html

[O03] 加锁保护共享数据
来源：http://hz.zhengqikj.top/gtnljtprlg.html

Py:   with lock: shared += 1
来源：http://hz.ybcxt.top/gtkeptrmsw.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.zhengqikj.top/gtcswhiwpj.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.cashguo.top/gtbeeexlti.html

TS:   // 同 JS
来源：http://hz.mhx1999.top/gtcxnxeszb.html

Java: synchronized (this) { shared++; }
来源：http://hz.chenzaomai.com/gtcqvbcnll.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.zhijiandao.cn/gtlpivixpv.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.jinghuilouyu.cn/gtryggtovz.html

C#:   lock (gate) { shared++; }
来源：http://hz.jinqigfzy.top/gtqhhofdkt.html

[O04] 定义异步函数并等待
来源：http://hz.hywenlv.cn/gtmmbtcqmy.html

Py:   async def f():⏎    await g()
来源：http://hz.dianchejie.cn/gtymzlvqfe.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.pengpengdd.cyou/gtxpswolbh.html

JS:   async function f() { await g(); }
来源：http://hz.yangfankeji.com/gtbjzmxbcw.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.meibo888.top/gtmspndher.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.jiagoushi.top/gtevhhgkgv.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.yangfankeji.com/gtclqfyxvt.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.aibaodan.cn/gtjeerjnim.html

C#:   async Task F() { await G(); }
来源：http://hz.havefunace.top/gtyptftvwm.html

[O05] 并发执行并等待全部完成
来源：http://hz.tianlin.xyz/gtakhytawx.html

Py:   asyncio.gather(*tasks)
来源：http://hz.sweek.top/gtuedjvvng.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.yvedp.cn/gtwxukyijy.html

JS:   await Promise.all(tasks)
来源：http://hz.ppjwa.cn/gthusgidsh.html

TS:   await Promise.all(tasks)
来源：http://hz.andypj.xyz/gtyhajjlpg.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.shanyushiyangkeji.top/gtatytmtrh.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.quarkkingdee.top/gtikyyzgzx.html

Ruby: threads.map(&:join)
来源：http://hz.bjfxy.top/gtouvmzfuy.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.yonumen.top/gtvycrazos.html

[O06] 使用进程池
来源：http://hz.316326.xyz/gttwuuzwrq.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.zhijiandao.cn/gtchvuhaac.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.bjfxy.top/gtedbyujws.html

JS:   // child_process / cluster 模块
来源：http://hz.zhijiandao.cn/gtytzrfqzl.html

TS:   // child_process / cluster 模块
来源：http://hz.kuanghao11.cn/gtaadntumc.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.cdnleiting.top/gtenadcwua.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.cashguo.top/gtxnhcvzdi.html

Ruby: // fork 块
来源：http://hz.pycfn.com/gtjpmbsyhf.html

C#:   Parallel.For
来源：http://hz.jiagoushi.top/gtmbjcmcan.html

================================================================================
来源：http://hz.hammf.cn/gtymkmhrmq.html

P. 常用工具函数
来源：http://hz.pycfn.com/gtkmiemfst.html

================================================================================
来源：http://hz.cucudq.cn/gtumdwwjfm.html

[P01] 生成 UUID
来源：http://hz.havefunace.top/gtuipqcexz.html

Py:   str(uuid.uuid4())
来源：http://hz.yonumen.top/gtiwqwwscb.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.jyoumei.cn/gtlokzafvl.html

JS:   crypto.randomUUID()
来源：http://hz.vqdsnc.cn/gthgybnwyn.html

TS:   crypto.randomUUID()
来源：http://hz.vqdsnc.cn/gtdtvjtkvi.html

Java: UUID.randomUUID().toString()
来源：http://hz.redwolf501.top/gthsopfkfp.html

Go:   // 用 github.com/google/uuid
来源：http://hz.jqgufenzy.top/gtdyktnyvc.html

Ruby: SecureRandom.uuid
来源：http://hz.wangshuangyany.cn/gtjhgrmlve.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.jinyuanbaomall.cn/gtpzpsjbpu.html

[P02] MD5 / SHA256 摘要
来源：http://hz.shanyushiyangtech.top/gtmtkynbzd.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.jlsjyb.cn/gtgwpurhzy.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.aibaodan.cn/gtaprkhufo.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.sysykeji.top/gtbumbeync.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.yueranfly.top/gtllakwyka.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.chenjidiqi.icu/gtalbjvruo.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.shuidangran.top/gtekhigbtv.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.jyoumei.cn/gtrlexkfaj.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.meibo888.top/gtkufpnmoc.html

[P03] 生成短随机字符串
来源：http://hz.gotoacloud.top/gtugzdiwem.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.svipenyu.cn/gtnfqgwmvo.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.aibaodan.cn/gtmvkgbnls.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.tanke756.top/gtazleeorq.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.shzxlz.cn/gtfwrmqcea.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.ydzc1.top/gtebeahsot.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.zdqjudy.top/gtcwvjpnuw.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.gotoacloud.top/gtpxeyjwyu.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.sweek.top/gtosbgirvy.html

[P04] 求长度
来源：http://hz.pycfn.com/gtniqllvmg.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.ppjwa.cn/gtzkbxnnvx.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.zhoulong.xyz/gtspkbacss.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.fzhhl.top/gtldizudme.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.hnqzz.top/gtihfqrrkf.html

Java: list.size();  map.size();  s.length()
来源：http://hz.shanyushiyangtech.top/gtoshgshfp.html

Go:   len(arr);  len(m)
来源：http://hz.52xcode.cn/gtnacserej.html

Ruby: x.length;  x.size
来源：http://hz.yj202588.top/gtvovotpho.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.xylfe.cn/gtddadfidr.html

[P05] 判断两个对象内容是否相等
来源：http://hz.zhoulong.xyz/gtgtyiomti.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.jianghu66.top/gtbzhjlbig.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.0kj1m.cn/gtnwfopsas.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.wangdashe.top/gtxslqcwes.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.hnqzz.top/gtoyajayga.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.yueranfly.top/gtafxwblsv.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.shuidangran.top/gtgyzcwxaz.html

Ruby: a == b
来源：http://hz.sufxvd.cn/gttdnxyphs.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.cheryme.top/gtzcdfezpe.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.yangfankeji.com/gtlaxgktpf.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.andypj.xyz/gtmzymwxxn.html

PHP:  if (empty($x)) {}
来源：http://hz.hywenlv.cn/gttofoaqos.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.ydjk.org.cn/gtherubzei.html

TS:   if (x == null) {}
来源：http://hz.shzxlz.cn/gtmpghwhmt.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.zhoulong.xyz/gtegybrvul.html

Go:   if x == nil {}
来源：http://hz.zhengqikj.top/gtrsuwmwwf.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.zhiwuduotai.top/gtyjabzwhh.html

C#:   if (x is null) {}
来源：http://hz.bjfxy.top/gtjsevvail.html

[P07] 防抖与节流
来源：http://hz.316326.xyz/gtgfiheqnc.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.nanxinkj.top/gtvtlqtvkl.html

PHP:  // 手写时间戳比较
来源：http://hz.yangfankeji.com/gtueqqfkcg.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.chenjidiqi.icu/gtwtflnvsn.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.gogol.net.cn/gtqhbmikif.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.sweek.top/gtxheoogra.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.shanyushiyangkeji.top/gtqigirvea.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.fengsongda.top/gtmqeqromh.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.iojbl.cn/gtcoclwcoh.html

[P08] 处理浮点精度问题
来源：http://hz.xuetiantiany.cn/gtipxuyxvf.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.hnxiangtu.top/gtjoufuyvx.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.sxryk.cn/gtquqmlons.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.quarkkingdee.top/gtlthlbljt.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.shanyushiyangkeji.top/gtdiuahkxc.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.daria6918.cn/gtjletmzlc.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.guannengcc.top/gtpwfndibo.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.hammf.cn/gtlvqwahol.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.mhx1999.top/gtqtcabdfy.html

================================================================================
来源：http://hz.cashguo.top/gtvuqzvrke.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.bjfxy.top/gtmcclpheq.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gtkavokxpy.html

[Q01] 创建表
来源：http://hz.xuanzx.com/gtdhjbkrmx.html

CREATE TABLE users (
来源：http://hz.cheryme.top/gtzhgoxxfw.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.tianlin.xyz/gtixvelsds.html

name VARCHAR(50) NOT NULL,
来源：http://hz.shangyingyoupin.top/gteuhyprqu.html

email VARCHAR(100) UNIQUE,
来源：http://hz.hnxiangtu.top/gtgmdnxksd.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.zhaomingkeji.xyz/gtjaqebyts.html

);
来源：http://hz.ppjwa.cn/gtyasgjeff.html

[Q02] 创建带外键的表
来源：http://hz.vqdsnc.cn/gtrsbpowyk.html

CREATE TABLE orders (
来源：http://hz.yueranfly.top/gtfthpkgil.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.52xcode.cn/gtwzfolypv.html

user_id INT NOT NULL,
来源：http://hz.zhongyouzk.top/gtmrghglcz.html

amount DECIMAL(10, 2),
来源：http://hz.cashguo.top/gtjeddctap.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.hywenlv.cn/gtuzswdpqs.html

);
来源：http://hz.wangshuangyany.cn/gtokyeusad.html

[Q03] 增加列
来源：http://hz.shuidangran.top/gtuvfwyuis.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.pengpengdd.cyou/gtafqprlle.html

[Q04] 修改列类型
来源：http://hz.ybcxt.top/gthxkailmg.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.shzxlz.cn/gttkkzcuxi.html

[Q05] 重命名列
来源：http://hz.aibaodan.cn/gtjzcvfdrq.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.zdqjudy.top/gtpycghuuy.html

[Q06] 删除列
来源：http://hz.sysykeji.top/gtxxkdcklr.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.jlsjyb.cn/gtjsngvzte.html

[Q07] 删除表
来源：http://hz.0kj1m.cn/gtyjopkbrz.html

DROP TABLE IF EXISTS orders;
来源：http://hz.redwolf501.top/gtvcydiaea.html

[Q08] 创建普通索引
来源：http://hz.nanxuanxn.top/gtbrsavrag.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.yueranfly.top/gtmvzhisgr.html

[Q09] 创建唯一索引
来源：http://hz.pengpengdd.cyou/gtckvyaprp.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.vqdsnc.cn/gthsnrroyh.html

[Q10] 插入单行
来源：http://hz.sweek.top/gttgkwxatm.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.sufxvd.cn/gtlauruhwp.html

[Q11] 一次插入多行
来源：http://hz.ydjk.org.cn/gtajimurlc.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.mhx1999.top/gtdfytgytx.html

[Q12] 插入后取自增 ID
来源：http://hz.jiagoushi.top/gtoposejry.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.birdmap.top/gtzlebaswu.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.xziqi.cn/gtnjgmjdbp.html

[Q13] 忽略重复插入
来源：http://hz.vqdsnc.cn/gtpqdtiflx.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.ybcxt.top/gtffcyfftk.html

[Q14] 存在则更新（upsert）
来源：http://hz.jinghuilouyu.cn/gtueycdyta.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.chenjidiqi.icu/gtalygghuv.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.jinyuanbaomall.cn/gtladovnqx.html

[Q15] 查询全部
来源：http://hz.chenlongwang.top/gtukgaekxi.html

SELECT * FROM users;
来源：http://hz.zdqjudy.top/gtiafdiyxb.html

[Q16] 查询指定列
来源：http://hz.zhoulong.xyz/gtdmtlactr.html

SELECT id, name FROM users;
来源：http://hz.hfpthk.cn/gtxmddwytk.html

[Q17] 条件查询
来源：http://hz.xylfe.cn/gtdobqloqz.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.gzhubu.top/gtqtdhqwuv.html

[Q18] 模糊匹配
来源：http://hz.pycfn.com/gtiqrbxuxl.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.gzhubu.top/gtjqktuecd.html

[Q19] 范围查询
来源：http://hz.daxiang520.top/gtxescepto.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.xylfe.cn/gtcqdwdwuw.html

[Q20] IN 列表
来源：http://hz.iojbl.cn/gtcslmusdl.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.gogol.net.cn/gtuhqvhjui.html

[Q21] 空值判断
来源：http://hz.feifeiyinyue.top/gthgqaxhhb.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.cheryme.top/gtyngbkkfu.html

[Q22] 排序
来源：http://hz.tanke756.top/gtbcityerm.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.jinghuilouyu.cn/gtawfhhfet.html

[Q23] 分页
来源：http://hz.gogol.net.cn/gtjjjnjdge.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.shzxlz.cn/gtpeeckovv.html

[Q24] 去重
来源：http://hz.wangshuangyany.cn/gttxgqpjdg.html

SELECT DISTINCT city FROM users;
来源：http://hz.shanyushiyangtech.top/gtcbkfnmdg.html

[Q25] 只取前 N 条
来源：http://hz.jinyuanbaomall.cn/gtxhejgvxd.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.yvedp.cn/gtfxrkpoqf.html

[Q26] 计数
来源：http://hz.jianghu66.top/gtdbwzolev.html

SELECT COUNT(*) FROM users;
来源：http://hz.shzxlz.cn/gtrwqlgqag.html

[Q27] 条件计数
来源：http://hz.cheryme.top/gtggxepyjz.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.mhx1999.top/gtomumscvr.html

[Q28] 求和与平均
来源：http://hz.snrcjt.cn/gttoqlrdld.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.yj20258.top/gtvfiezvpo.html

[Q29] 最大最小值
来源：http://hz.hysaishi.cn/gtzgsagpcc.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.shanyushiyangtech.top/gthcbcaohy.html

[Q30] 分组统计
来源：http://hz.c1oappe.top/gtawozptsj.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.quarkkingdee.top/gtwlzpnvaj.html

[Q31] 分组后过滤
来源：http://hz.wangshuangyany.cn/gtarwvagvj.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.wangshuangyany.cn/gtdbthyonc.html

[Q32] 分组拼接字符串
来源：http://hz.shuidangran.top/gttwjjzypj.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.zdqjudy.top/gtgnzvwicg.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.chenjidiqi.icu/gtrdgjzvqr.html

[Q33] 多列分组
来源：http://hz.jinqigufen.top/gtumvahqhm.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.hammf.cn/gtgwtpiqzt.html

[Q34] 每组取第一条
来源：http://hz.tanke756.top/gtxczleljh.html

SELECT * FROM (
来源：http://hz.shzxlz.cn/gtlloyvpuh.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.ydjk.org.cn/gtcduejnjw.html

) t WHERE rn = 1;
来源：http://hz.jyoumei.cn/gtfgtyvmku.html

[Q35] 内连接
来源：http://hz.jinghuilouyu.cn/gtgjbewock.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.shanyushiyangtech.top/gtqislxtri.html

[Q36] 左连接
来源：http://hz.jinqigfzy.top/gtslqcuubl.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.guowangkeji.top/gtbhptrtbr.html

[Q37] 右连接
来源：http://hz.xylfe.cn/gtljgcvbux.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.sweek.top/gteltgpgab.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.yuanzhike.top/gtrwpwspxy.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.feifeiyinyue.top/gtmorgavsm.html

[Q39] 自连接（查上下级）
来源：http://hz.yj20258.top/gtpojosuvn.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.quarkkingdee.top/gtlyznvlne.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.tanke756.top/gthurqfkie.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.havefunace.top/gtjjbuwbrn.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.iojbl.cn/gttnlyrzxb.html

[Q41] 多表连接
来源：http://hz.dianchejie.cn/gtpfoymfit.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.0kj1m.cn/gtyubfncrp.html

JOIN users u ON u.id = o.user_id
来源：http://hz.hysaishi.cn/gtrynwxqgg.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.hywenlv.cn/gtgphcbrjt.html

[Q42] 连接条件附加过滤
来源：http://hz.zhengqikj.top/gtroxsfcyz.html


<!-- 参考信息 -->