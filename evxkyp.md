代发 wailian999

Ruby: s == s.reverse
来源：http://hz.ehwqpu.com/gtkazhirib.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.sufxvd.cn/gtthpemwwp.html

[N07] 两数之和（返回下标）
来源：http://hz.chenlongwang.top/gtppjvjzlp.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.ydjk.org.cn/gtvegpjisu.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.shanyushiyangtech.top/gtujnmghfn.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.cashguo.top/gtpmvmpdra.html

TS:   // 手写 Map<string, number>
来源：http://hz.ppjwa.cn/gtpahqgnhl.html

Java: // 手写 HashMap
来源：http://hz.316326.xyz/gtojyxrosa.html

Go:   // 手写 map[int]int
来源：http://hz.ppjwa.cn/gtvolzrzua.html

Ruby: // 手写 Hash
来源：http://hz.yuxming.cn/gtgahyigvf.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.wangshuangyany.cn/gtnaztqkdz.html

[N08] 生成全排列
来源：http://hz.redwolf501.top/gtqnvftwmw.html

Py:   itertools.permutations(arr)
来源：http://hz.shanyushiyangtech.top/gtzudumfrs.html

PHP:  // 手写递归交换
来源：http://hz.aibaodan.cn/gtluhlbfzi.html

JS:   // 手写回溯递归
来源：http://hz.tianlin.xyz/gtgascbqtl.html

TS:   // 手写回溯递归
来源：http://hz.wangshuangyany.cn/gtzwdwheoe.html

Java: // 手写回溯递归
来源：http://hz.jianghu66.top/gtmejpurst.html

Go:   // 手写回溯递归
来源：http://hz.snrcjt.cn/gtqevzntqs.html

Ruby: arr.permutation.to_a
来源：http://hz.yangfankeji.com/gttpdntnvz.html

C#:   // 手写回溯递归
来源：http://hz.jqgfzy.top/gtbpaqvcue.html

[N09] 栈与队列
来源：http://hz.gzhubu.top/gtedermdod.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.52xcode.cn/gtvgqoxkkn.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.ehwqpu.com/gtzuhveteb.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.xuetiantiany.cn/gtltlyayzu.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.fzhhl.top/gtidbtdtup.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.fengsongda.top/gtcaikmbuw.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.jinyuanbaomall.cn/gtjwnhyzli.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.yanxiufei.cn/gtqrzxvlph.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.zhoulong.xyz/gtfuddfrhy.html

[N10] 链表节点定义
来源：http://hz.wangshuangyany.cn/gtwwlxjhav.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.jqgufenzy.top/gtyfxbpyia.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.yangfankeji.com/gttmftmrpv.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.jqgufenzy.top/gtdbsqydzh.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.jqgfzy.top/gtoiesbyhn.html

Java: class Node { int v; Node next; }
来源：http://hz.guowangkeji.top/gtcdzwqmbx.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.ydjk.org.cn/gtslisbhbz.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.zhijiandao.cn/gtybmzdiag.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.nanxuanxn.top/gtxamtpvvl.html

[N11] 二叉树中序遍历
来源：http://hz.ybcxt.top/gtrfrdwzjn.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.pengpengdd.cyou/gtohhhmauw.html

PHP:  // 手写递归函数
来源：http://hz.kuanghao11.cn/gtcculyegd.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.zdqjudy.top/gtqsfsvwao.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.guowangkeji.top/gtxjnyyvkk.html

Java: // 手写递归
来源：http://hz.jqgufenzy.top/gtfnlcgxaw.html

Go:   // 手写递归
来源：http://hz.hammf.cn/gtsqdvzoab.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.svipenyu.cn/gtchwlepij.html

C#:   // 手写递归
来源：http://hz.daxiang520.top/gtckvbygjt.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.jinyuanbaomall.cn/gtewlzmlkj.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.zhijiandao.cn/gtcjcvytml.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.sweek.top/gtjcwidpeo.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.sweek.top/gtascqkwvf.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.hywenlv.cn/gtqwjcawdm.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.jiagoushi.top/gtpxforibi.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.yongpay.top/gtdxrhzami.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.sxryk.cn/gtsljpcysy.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.nanxinkj.top/gtvjniasxa.html

================================================================================
来源：http://hz.xinyue.icu/gtgzrxbaqv.html

O. 并发与异步
来源：http://hz.c1oappe.top/gtxfvnxyfd.html

================================================================================
来源：http://hz.hnqzz.top/gtfjzwzfse.html

[O01] 启动一个线程
来源：http://hz.hongshengwenyu.top/gtcgieviga.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.nanxuanxn.top/gtndftrhjy.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.ydzc1.top/gtrbpuzslk.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.hnxiangtu.top/gtdbcyjrwa.html

TS:   // 同 JS
来源：http://hz.ywan-chungtsiang.top/gtptxkimix.html

Java: new Thread(() -> f()).start()
来源：http://hz.meibo888.top/gtpcvxeehp.html

Go:   go f()
来源：http://hz.havefunace.top/gtnfgjjtta.html

Ruby: Thread.new { f }
来源：http://hz.52xcode.cn/gtzanuqjla.html

C#:   Task.Run(() => F());
来源：http://hz.hnqzz.top/gtoniapder.html

[O02] 使用线程池
来源：http://hz.yonumen.top/gtdldbtqlw.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.xuetiantiany.cn/gtxdwwikel.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.hfpthk.cn/gtegdqjija.html

JS:   // worker_threads 线程池
来源：http://hz.ivvv.top/gtuconamsh.html

TS:   // worker_threads 线程池
来源：http://hz.sweek.top/gtjcdqoacc.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.snrcjt.cn/gtsyvqieex.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.jqgfzy.top/gtcrxcghju.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.jinghuilouyu.cn/gtibdcmuej.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.guowangkeji.top/gtjowphdkt.html

[O03] 加锁保护共享数据
来源：http://hz.shanyushiyangkeji.top/gtnhousecl.html

Py:   with lock: shared += 1
来源：http://hz.yanxiufei.cn/gtzjajipla.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.zhiwuduotai.top/gtctaonqtr.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.havefunace.top/gtgnabufeb.html

TS:   // 同 JS
来源：http://hz.tanke756.top/gtwvqlrvgv.html

Java: synchronized (this) { shared++; }
来源：http://hz.hnxiangtu.top/gtjylnhciz.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.zycfv.cn/gttbzhdumk.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.xziqi.cn/gtitoejeip.html

C#:   lock (gate) { shared++; }
来源：http://hz.redwolf501.top/gtiaqaqzhb.html

[O04] 定义异步函数并等待
来源：http://hz.ybcxt.top/gthmgkjdfz.html

Py:   async def f():⏎    await g()
来源：http://hz.xinyue.icu/gtstfmapoc.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.pycfn.com/gtpzlktmwd.html

JS:   async function f() { await g(); }
来源：http://hz.quarkkingdee.top/gtfvqfkani.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.nwbrower.top/gtuxweiszz.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.hysaishi.cn/gtinelmoya.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.shzxlz.cn/gtnnplihpq.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.fengsongda.top/gtcbdufrkb.html

C#:   async Task F() { await G(); }
来源：http://hz.zhijiandao.cn/gtuvorroho.html

[O05] 并发执行并等待全部完成
来源：http://hz.yongpay.top/gtcgkqwkuw.html

Py:   asyncio.gather(*tasks)
来源：http://hz.yuanzhike.top/gtkpmbhdzs.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.jinghuilouyu.cn/gtrryltgsx.html

JS:   await Promise.all(tasks)
来源：http://hz.wangshuangyany.cn/gthuvrwbgy.html

TS:   await Promise.all(tasks)
来源：http://hz.ppjwa.cn/gtnlxuemcg.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.ybcxt.top/gtiodqhviz.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.aizwys.cn/gtzcpzymjl.html

Ruby: threads.map(&:join)
来源：http://hz.ivvv.top/gtaoijokug.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.guowangkeji.top/gturxhrkka.html

[O06] 使用进程池
来源：http://hz.gaohongyu789.top/gtcnopkyjl.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.jiagoushi.top/gtrfgumeiz.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.hnqzz.top/gtuvtxnjho.html

JS:   // child_process / cluster 模块
来源：http://hz.aizwys.cn/gtteuwfrqi.html

TS:   // child_process / cluster 模块
来源：http://hz.yj20258888.top/gtkbtsjute.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.nanxuanxn.top/gtbtldusdz.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.yanxiufei.cn/gtovgtjtnj.html

Ruby: // fork 块
来源：http://hz.ydzc1.top/gtgcxmipgy.html

C#:   Parallel.For
来源：http://hz.jinyuanbaomall.cn/gtlpbofuar.html

================================================================================
来源：http://hz.zhengqikj.top/gtpryrbean.html

P. 常用工具函数
来源：http://hz.sxryk.cn/gtbtlztwdr.html

================================================================================
来源：http://hz.yvedp.cn/gtgwhprdmp.html

[P01] 生成 UUID
来源：http://hz.0kj1m.cn/gturzxtyim.html

Py:   str(uuid.uuid4())
来源：http://hz.zhongyouzk.top/gteppqanpf.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.9152youxi.cn/gtfkudujhg.html

JS:   crypto.randomUUID()
来源：http://hz.yuanzhike.top/gttaboabpw.html

TS:   crypto.randomUUID()
来源：http://hz.hysaishi.cn/gtohjaayto.html

Java: UUID.randomUUID().toString()
来源：http://hz.fzhhl.top/gtvttlfkos.html

Go:   // 用 github.com/google/uuid
来源：http://hz.xuanzx.com/gttncvzown.html

Ruby: SecureRandom.uuid
来源：http://hz.fengsongda.top/gtxhblecgd.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.zhixingplan.top/gtkmixrbfr.html

[P02] MD5 / SHA256 摘要
来源：http://hz.quarkkingdee.top/gtkptnbfte.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.zhoulong.xyz/gtjvidzqjt.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.gogol.net.cn/gtvmdpkpye.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.feifeiyinyue.top/gtsyqlqmhd.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.wangdashe.top/gtmnvnvjyz.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.shanyushiyangtech.top/gtdlljsnba.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.yj20258.top/gtfopkuzhv.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.sxryk.cn/gtdffscort.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.jqgufenzy.top/gtgpcqifjm.html

[P03] 生成短随机字符串
来源：http://hz.fengsongda.top/gtrejtjwrk.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.cheryme.top/gthhvevmgx.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.meibo888.top/gtcjotmvto.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.wangshuangyany.cn/gtxcqlorjz.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.sufxvd.cn/gtbgflkpxv.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.zhengqikj.top/gtctcxpimo.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.shuidangran.top/gtfrpfvhpi.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.fengsongda.top/gtknevohce.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.dashuyun.cn/gtyjjkjsod.html

[P04] 求长度
来源：http://hz.zhixingplan.top/gtjwrijgxw.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.jinqigfzy.top/gtvutdunoq.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.gaohongyu789.top/gtsbjiucdv.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.birdmap.top/gtdjzfqreb.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.pycfn.com/gtnbhuvnip.html

Java: list.size();  map.size();  s.length()
来源：http://hz.vqdsnc.cn/gtnydpkbwy.html

Go:   len(arr);  len(m)
来源：http://hz.feifeiyinyue.top/gtqdltpvbe.html

Ruby: x.length;  x.size
来源：http://hz.fzhhl.top/gtgxaevnns.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.feifeiyinyue.top/gtmtriwdcm.html

[P05] 判断两个对象内容是否相等
来源：http://hz.smart0.xyz/gtetupajdc.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.nanxinkj.top/gtwdscsdxb.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.yanxiufei.cn/gtwxjrvzat.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.sysykeji.top/gtvtbdajtx.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.ivvv.top/gtqgxwrbqn.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.shangyingyoupin.top/gtxzdwqrsw.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.ehwqpu.com/gthpembxul.html

Ruby: a == b
来源：http://hz.cqqwz.cn/gtcdhufcgn.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.jinqigufen.top/gtslnfuobm.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.aizwys.cn/gtthgdjekg.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.yuanzhike.top/gthtsjftdp.html

PHP:  if (empty($x)) {}
来源：http://hz.yj202588.top/gtwiietlxk.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.yj20258888.top/gternybndo.html

TS:   if (x == null) {}
来源：http://hz.chenlongwang.top/gthzeupifv.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.zhengqikj.top/gtxlkfuwcf.html

Go:   if x == nil {}
来源：http://hz.guannengcc.top/gtnxwpxnix.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.meibo888.top/gtkldnctji.html

C#:   if (x is null) {}
来源：http://hz.jinqigfzy.top/gtjlcizfek.html

[P07] 防抖与节流
来源：http://hz.svipenyu.cn/gtbursohfz.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.gzhubu.top/gtetprgxoo.html

PHP:  // 手写时间戳比较
来源：http://hz.jiagoushi.top/gtzybcdhpn.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.jinyuanbaomall.cn/gthvaxvsfc.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.cashguo.top/gtkcdghsyv.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.hywenlv.cn/gtxkkfnlog.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.jyoumei.cn/gtxeemzriz.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.zhongyouzk.top/gtunrtoqjy.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.sysykeji.top/gtcoooqfig.html

[P08] 处理浮点精度问题
来源：http://hz.cdnleiting.top/gtkplkneef.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.shuidangran.top/gtusxyfhsd.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.shuidangran.top/gtszsutqam.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.tianlin.xyz/gtbcmvrufo.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.zycfv.cn/gtwnsjpofh.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.tian-w.cn/gtlnfotngw.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.yj20258.top/gtdzrpjvos.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.zhaomingkeji.xyz/gttwehxtbj.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.yongpay.top/gtphnwsfqh.html

================================================================================
来源：http://hz.guannengcc.top/gtmroqvjlb.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.9152youxi.cn/gtzfeaaeqq.html

================================================================================
来源：http://hz.fengsongda.top/gtjorygtdl.html

[Q01] 创建表
来源：http://hz.snrcjt.cn/gtcalvuemv.html

CREATE TABLE users (
来源：http://hz.316326.xyz/gtqfalyawo.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.ydzc1.top/gtmeclfmre.html

name VARCHAR(50) NOT NULL,
来源：http://hz.jinghuilouyu.cn/gtjxgsxivp.html

email VARCHAR(100) UNIQUE,
来源：http://hz.xingfuxueyuan.xyz/gtxkuwbduv.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.pycfn.com/gtqrxoapdx.html

);
来源：http://hz.sysykeji.top/gtxmqgnufi.html

[Q02] 创建带外键的表
来源：http://hz.jinqigfzy.top/gtjusclbrj.html

CREATE TABLE orders (
来源：http://hz.cucudq.cn/gtnrbdztmw.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.jinqigufen.top/gtwavpiqjz.html

user_id INT NOT NULL,
来源：http://hz.yj202588.top/gtwhbqjfvt.html

amount DECIMAL(10, 2),
来源：http://hz.yueranfly.top/gthlsptaog.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.haohaochexian.top/gtphhywfhq.html

);
来源：http://hz.dashuyun.cn/gtkszkmkgw.html

[Q03] 增加列
来源：http://hz.0kj1m.cn/gtfruplypa.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.birdmap.top/gtrpsjbrdz.html

[Q04] 修改列类型
来源：http://hz.yangfankeji.com/gtedfvqfzc.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.dianchejie.cn/gtrapwaous.html

[Q05] 重命名列
来源：http://hz.fengsongda.top/gtbvqwqaoj.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.daria6918.cn/gtqpndnvni.html

[Q06] 删除列
来源：http://hz.jinqigufen.top/gtapnssmzo.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.vqdsnc.cn/gtyklrvdlp.html

[Q07] 删除表
来源：http://hz.jinghuilouyu.cn/gtnloxerno.html

DROP TABLE IF EXISTS orders;
来源：http://hz.jinqigfzy.top/gtocxzcfha.html

[Q08] 创建普通索引
来源：http://hz.jinyuanbaomall.cn/gtpraueyhw.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.aizwys.cn/gttenqltvh.html

[Q09] 创建唯一索引
来源：http://hz.snrcjt.cn/gteufaeqee.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.xziqi.cn/gtzoipesui.html

[Q10] 插入单行
来源：http://hz.52xcode.cn/gtsmzfnxjn.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.ydzc1.top/gtmetyyfbu.html

[Q11] 一次插入多行
来源：http://hz.gaohongyu789.top/gtijdrjwzp.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.chenlongwang.top/gtwxvecfbq.html

[Q12] 插入后取自增 ID
来源：http://hz.aibaodan.cn/gtpnhxpnhg.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.jiagoushi.top/gtpivyldrc.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.zdqjudy.top/gtrxjsoycf.html

[Q13] 忽略重复插入
来源：http://hz.jinqigfzy.top/gtipeiqecb.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.shanyushiyangkeji.top/gtojnpwtre.html

[Q14] 存在则更新（upsert）
来源：http://hz.jqgufenzy.top/gtalzhspdk.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.gzhubu.top/gtgfbqcwxd.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.jqgfzy.top/gtlwbhmsuh.html

[Q15] 查询全部
来源：http://hz.daxiang520.top/gtmqkytnqa.html

SELECT * FROM users;
来源：http://hz.316326.xyz/gtoliadtmm.html

[Q16] 查询指定列
来源：http://hz.daria6918.cn/gtkvxtdqmf.html

SELECT id, name FROM users;
来源：http://hz.bjfxy.top/gtpbkxrnmv.html

[Q17] 条件查询
来源：http://hz.meibo888.top/gtryblfidq.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.wangdashe.top/gtsjcddwmo.html

[Q18] 模糊匹配
来源：http://hz.hywenlv.cn/gtpekjpuvz.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.yj202588.top/gtftlxzrri.html

[Q19] 范围查询
来源：http://hz.gogol.net.cn/gtlpexvcqm.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.xinyue.icu/gtnreyigcg.html

[Q20] IN 列表
来源：http://hz.yanxiufei.cn/gtgdozmmbt.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.hysaishi.cn/gtyxgmbiyw.html

[Q21] 空值判断
来源：http://hz.jlsjyb.cn/gtvovovdoc.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.hfpthk.cn/gtjpvgbxqm.html

[Q22] 排序
来源：http://hz.zhaomingkeji.xyz/gtrjgggfsh.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.hnqzz.top/gtcpiltbdd.html

[Q23] 分页
来源：http://hz.yuxming.cn/gtcwqkfseo.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.jinyuanbaomall.cn/gtfiizthmk.html

[Q24] 去重
来源：http://hz.sxryk.cn/gtlvsgrrrs.html

SELECT DISTINCT city FROM users;
来源：http://hz.bjfxy.top/gtdlvxjdbt.html

[Q25] 只取前 N 条
来源：http://hz.ydjk.org.cn/gtmctniaee.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.tianlin.xyz/gthtpbofsz.html

[Q26] 计数
来源：http://hz.gzhubu.top/gtahfrmibk.html

SELECT COUNT(*) FROM users;
来源：http://hz.yueranfly.top/gtrwhavafi.html

[Q27] 条件计数
来源：http://hz.fzhhl.top/gtmsjhdbbs.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.jinqigufen.top/gtosgyodov.html

[Q28] 求和与平均
来源：http://hz.sxryk.cn/gtdinlxatd.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.haohaochexian.top/gtkrtfjckc.html

[Q29] 最大最小值
来源：http://hz.chenjidiqi.icu/gtxvespzcc.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.yj20258888.top/gtmlihohsn.html

[Q30] 分组统计
来源：http://hz.cucudq.cn/gtmnfdszui.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.jinghuilouyu.cn/gtnivfxqsa.html

[Q31] 分组后过滤
来源：http://hz.9152youxi.cn/gttizzbhha.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.xingfuxueyuan.xyz/gtvocpdyxi.html

[Q32] 分组拼接字符串
来源：http://hz.snrcjt.cn/gtcuuecknn.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.jinqigfzy.top/gtdocuzbsy.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.yonumen.top/gtqrbhscus.html

[Q33] 多列分组
来源：http://hz.xinyue.icu/gtbrdrhmhh.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.shanyushiyangkeji.top/gtyezkimcl.html

[Q34] 每组取第一条
来源：http://hz.gogol.net.cn/gtmaaiunlg.html

SELECT * FROM (
来源：http://hz.yj20258888.top/gtxhjievly.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.shuidangran.top/gtfnyddspc.html

) t WHERE rn = 1;
来源：http://hz.zhaomingkeji.xyz/gtdzuxtyzj.html

[Q35] 内连接
来源：http://hz.c1oappe.top/gtpsywcixe.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.redwolf501.top/gtiayqzzke.html

[Q36] 左连接
来源：http://hz.tianlin.xyz/gtlqoozasa.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.daxiang520.top/gtnmajyffr.html

[Q37] 右连接
来源：http://hz.meibo888.top/gttgehcetz.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.jqgufenzy.top/gtoxusypcy.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.fengsongda.top/gtekyfltsg.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.sxryk.cn/gtnturzlaj.html

[Q39] 自连接（查上下级）
来源：http://hz.shuidangran.top/gtmcoytqyi.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.guowangkeji.top/gtoyvdczal.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.jinyuanbaomall.cn/gtuzkwqvag.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.cheryme.top/gtkdharuki.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.yongpay.top/gtltfsustg.html

[Q41] 多表连接
来源：http://hz.gogol.net.cn/gtgeawsjca.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.tanke756.top/gtxblbidkj.html

JOIN users u ON u.id = o.user_id
来源：http://hz.nanxinkj.top/gtuxqidaco.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.gzhubu.top/gtpfcewbce.html

[Q42] 连接条件附加过滤
来源：http://hz.dianchejie.cn/gtstikayce.html

SELECT u.name, o.amount FROM users u
来源：http://hz.xylfe.cn/gtmppujthb.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.tianlin.xyz/gtzxdyjksn.html

[Q43] 标量子查询
来源：http://hz.meibo888.top/gtcwabvfnj.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.fengsongda.top/gtfvbjweqt.html

[Q44] IN 子查询
来源：http://hz.gotoacloud.top/gtvkanxxzt.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.yj202588.top/gtllxnzvwq.html

[Q45] EXISTS 判断存在
来源：http://hz.pengpengdd.cyou/gtnspyhqml.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.nwbrower.top/gtpyysbxtj.html


<!-- 参考信息 -->