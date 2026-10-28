代发 wailian999

Ruby: s == s.reverse
来源：http://hz.9152youxi.cn/gtiajpxwbk.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.jinghuilouyu.cn/gtvgycaffx.html

[N07] 两数之和（返回下标）
来源：http://hz.fzhhl.top/gtroxxrxkt.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.sysykeji.top/gtbqjqlgro.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.tanke756.top/gtbbpzhjag.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.jianghu66.top/gthwwupklk.html

TS:   // 手写 Map<string, number>
来源：http://hz.zdqjudy.top/gtqasvnupd.html

Java: // 手写 HashMap
来源：http://hz.tian-w.cn/gtrjtffwjf.html

Go:   // 手写 map[int]int
来源：http://hz.shanyushiyangtech.top/gtiiqbcxwq.html

Ruby: // 手写 Hash
来源：http://hz.mhx1999.top/gtrluosjnc.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.aizwys.cn/gtuykfugij.html

[N08] 生成全排列
来源：http://hz.daria6918.cn/gtvtkhbcyf.html

Py:   itertools.permutations(arr)
来源：http://hz.hongshengwenyu.top/gtwekguvty.html

PHP:  // 手写递归交换
来源：http://hz.zdqjudy.top/gtaqhudyik.html

JS:   // 手写回溯递归
来源：http://hz.hongshengwenyu.top/gtgaqflozh.html

TS:   // 手写回溯递归
来源：http://hz.hnqzz.top/gtmobczdvd.html

Java: // 手写回溯递归
来源：http://hz.aibaodan.cn/gtntcmnpov.html

Go:   // 手写回溯递归
来源：http://hz.yongpay.top/gtdjchsjug.html

Ruby: arr.permutation.to_a
来源：http://hz.yj20258888.top/gtxkthsbmt.html

C#:   // 手写回溯递归
来源：http://hz.shanyushiyangkeji.top/gtbxjptdbi.html

[N09] 栈与队列
来源：http://hz.hongshengwenyu.top/gtfxznzmke.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.quarkkingdee.top/gtdxkkusqr.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.sxryk.cn/gtjonhddkk.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.mhx1999.top/gtaeauhwyf.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.bjfxy.top/gtvdqepmhx.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.meibo888.top/gtyxldddir.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.fzhhl.top/gtszhbpjwp.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.redwolf501.top/gtkgxnzxxe.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.gogol.net.cn/gtkzafemdn.html

[N10] 链表节点定义
来源：http://hz.gogol.net.cn/gtgpiwbchv.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.wangshuangyany.cn/gtelmeguhp.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.smart0.xyz/gtnqsratwk.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.sysykeji.top/gtmznalfhf.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.gaohongyu789.top/gtwponlcya.html

Java: class Node { int v; Node next; }
来源：http://hz.zdqjudy.top/gtlgdwjgtx.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.hysaishi.cn/gtcsawufth.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.shangyingyoupin.top/gtdudczish.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.sweek.top/gtewrferyn.html

[N11] 二叉树中序遍历
来源：http://hz.vqdsnc.cn/gtqbnvykfr.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.zhijiandao.cn/gtxodllakz.html

PHP:  // 手写递归函数
来源：http://hz.sufxvd.cn/gtfpkricpd.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.fengsongda.top/gttpdeoqcr.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.smart0.xyz/gtwuavbbbv.html

Java: // 手写递归
来源：http://hz.0kj1m.cn/gtctfhvkxc.html

Go:   // 手写递归
来源：http://hz.jianghu66.top/gtvybkkvcc.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.yongpay.top/gtdsftiesl.html

C#:   // 手写递归
来源：http://hz.ppjwa.cn/gtzvszgixr.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.shanyushiyangkeji.top/gtnnqvxtgc.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.jinqigufen.top/gtduloayea.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.xinyue.icu/gtytlwohrm.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.c1oappe.top/gtcsuqfllz.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.birdmap.top/gtmzaajstd.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.sysykeji.top/gtaizzyzpr.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.gogol.net.cn/gtxgpyoqkr.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.jqgfzy.top/gtfmnwqyfk.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.hywenlv.cn/gthzfiplvz.html

================================================================================
来源：http://hz.vqdsnc.cn/gtrxwoesql.html

O. 并发与异步
来源：http://hz.haohaochexian.top/gtftwicqhb.html

================================================================================
来源：http://hz.tanke756.top/gtatfnpsdy.html

[O01] 启动一个线程
来源：http://hz.cdnleiting.top/gtjsylwdxl.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.haohaochexian.top/gtacgljcjv.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.gaohongyu789.top/gthcneoxyb.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.zhoulong.xyz/gtjbstnafs.html

TS:   // 同 JS
来源：http://hz.chenzaomai.com/gtvzhvnnwt.html

Java: new Thread(() -> f()).start()
来源：http://hz.guannengcc.top/gtbmbwknpq.html

Go:   go f()
来源：http://hz.xingfuxueyuan.xyz/gtgjtyzltc.html

Ruby: Thread.new { f }
来源：http://hz.yj20258888.top/gtcojnlmgq.html

C#:   Task.Run(() => F());
来源：http://hz.snrcjt.cn/gtogdooxoc.html

[O02] 使用线程池
来源：http://hz.shanyushiyangtech.top/gtbsdxaclh.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.cucudq.cn/gtxsfsuoix.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.jianghu66.top/gtuaysdnjr.html

JS:   // worker_threads 线程池
来源：http://hz.ydzc1.top/gtazepgutj.html

TS:   // worker_threads 线程池
来源：http://hz.jqgufenzy.top/gtawjwmcam.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.xinyue.icu/gttfbwsztz.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.zhixingplan.top/gtoljtknlt.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.ywan-chungtsiang.top/gtdxbabdsy.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.zhijiandao.cn/gttyrrogqf.html

[O03] 加锁保护共享数据
来源：http://hz.gotoacloud.top/gtfzxvshns.html

Py:   with lock: shared += 1
来源：http://hz.xziqi.cn/gtzomnpphw.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.wangshuangyany.cn/gtmhmczleq.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.316326.xyz/gtrtqnhavf.html

TS:   // 同 JS
来源：http://hz.xuanzx.com/gtpcbavhui.html

Java: synchronized (this) { shared++; }
来源：http://hz.haohaochexian.top/gtacoibeuh.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.hnqzz.top/gtxcmfuvmg.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.xingfuxueyuan.xyz/gtfzojdqeb.html

C#:   lock (gate) { shared++; }
来源：http://hz.ybcxt.top/gtxhtthrjf.html

[O04] 定义异步函数并等待
来源：http://hz.daxiang520.top/gtgzxwtagr.html

Py:   async def f():⏎    await g()
来源：http://hz.sweek.top/gtbalvcdsu.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.aibaodan.cn/gttxwfrwju.html

JS:   async function f() { await g(); }
来源：http://hz.wangshuangyany.cn/gtnxqamqhl.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.xylfe.cn/gthammnmqb.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.nanxinkj.top/gtdgiliepf.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.shuidangran.top/gtiyvnlqos.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.gzhubu.top/gtfcovzndl.html

C#:   async Task F() { await G(); }
来源：http://hz.tianlin.xyz/gtwfzmlvme.html

[O05] 并发执行并等待全部完成
来源：http://hz.sweek.top/gtdhlswjfr.html

Py:   asyncio.gather(*tasks)
来源：http://hz.wangshuangyany.cn/gttezbsvdg.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.guowangkeji.top/gtvumpcrpv.html

JS:   await Promise.all(tasks)
来源：http://hz.cucudq.cn/gtngdpgipm.html

TS:   await Promise.all(tasks)
来源：http://hz.andypj.xyz/gtqbeqruyw.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.jqgfzy.top/gtjfmcizss.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.zhengqikj.top/gtldqmsmrw.html

Ruby: threads.map(&:join)
来源：http://hz.fzhhl.top/gtrkrvqeke.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.pycfn.com/gtbepdizcl.html

[O06] 使用进程池
来源：http://hz.haohaochexian.top/gtnnfmgzur.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.yuxming.cn/gttyqnpxia.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.9152youxi.cn/gtmcrqseie.html

JS:   // child_process / cluster 模块
来源：http://hz.jiagoushi.top/gtjsdtpovh.html

TS:   // child_process / cluster 模块
来源：http://hz.cashguo.top/gtkzirctwp.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.quarkkingdee.top/gtlakbywtm.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.shuidangran.top/gtkymegxxs.html

Ruby: // fork 块
来源：http://hz.hysaishi.cn/gthxbpehtr.html

C#:   Parallel.For
来源：http://hz.chenzaomai.com/gtilmqejcc.html

================================================================================
来源：http://hz.meibo888.top/gtbhfesvtz.html

P. 常用工具函数
来源：http://hz.nwbrower.top/gtmpebevjk.html

================================================================================
来源：http://hz.yueranfly.top/gtvdxmpfpi.html

[P01] 生成 UUID
来源：http://hz.jyoumei.cn/gtvsttoehd.html

Py:   str(uuid.uuid4())
来源：http://hz.yongpay.top/gtidpsiyeh.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.nwbrower.top/gtzndviemr.html

JS:   crypto.randomUUID()
来源：http://hz.birdmap.top/gtxgnexkar.html

TS:   crypto.randomUUID()
来源：http://hz.smart0.xyz/gtlrtdtsnl.html

Java: UUID.randomUUID().toString()
来源：http://hz.cucudq.cn/gtrnvravzc.html

Go:   // 用 github.com/google/uuid
来源：http://hz.jqgfzy.top/gtlvlvpuwd.html

Ruby: SecureRandom.uuid
来源：http://hz.daxiang520.top/gtjyyvzoqd.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.zhaomingkeji.xyz/gtidisduvy.html

[P02] MD5 / SHA256 摘要
来源：http://hz.tanke756.top/gtrjrhgtwv.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.hnxiangtu.top/gtwtbyegqa.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.yj20258.top/gtizmgnmqo.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.shanyushiyangkeji.top/gtlhtlvwod.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.gogol.net.cn/gtemqoebgg.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.zdqjudy.top/gtwlfcpbpa.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.jlsjyb.cn/gtruvihtbn.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.sxryk.cn/gtwcpuojsf.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.nanxinkj.top/gtrrkxlwjz.html

[P03] 生成短随机字符串
来源：http://hz.yvedp.cn/gtmaxtujuc.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.ybcxt.top/gtnaljikgr.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.jinqigfzy.top/gtlrebqoxn.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.feifeiyinyue.top/gtbfaqowvo.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.sxryk.cn/gtqldkczzz.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.zycfv.cn/gtywuqrgpu.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.svipenyu.cn/gtojuaznth.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.yuanzhike.top/gtxslujwwo.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.sufxvd.cn/gtgznnwrxp.html

[P04] 求长度
来源：http://hz.chenzaomai.com/gtjpbrbacx.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.shanyushiyangkeji.top/gtotvixlbb.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.shzxlz.cn/gtbebtcbog.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.vqdsnc.cn/gtrzzrbies.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.sxryk.cn/gtleujxbpc.html

Java: list.size();  map.size();  s.length()
来源：http://hz.zhixingplan.top/gtrycrsjps.html

Go:   len(arr);  len(m)
来源：http://hz.jqgufenzy.top/gtqovthmxf.html

Ruby: x.length;  x.size
来源：http://hz.ydjk.org.cn/gthoebeduk.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.snrcjt.cn/gtjwxvcrcd.html

[P05] 判断两个对象内容是否相等
来源：http://hz.xziqi.cn/gtrgvbxdar.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.xylfe.cn/gtvtkmusla.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.cqqwz.cn/gtjleybdbe.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.ydzc1.top/gtcvndgcbm.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.redwolf501.top/gtvfarrglb.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.yj20258888.top/gtoifuafdz.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.nanxuanxn.top/gtzcuqvhpt.html

Ruby: a == b
来源：http://hz.yuxming.cn/gtuyolqtgi.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.xuanzx.com/gtkpgtuich.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.ehwqpu.com/gtuoflhxnu.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.bjfxy.top/gtynlaizao.html

PHP:  if (empty($x)) {}
来源：http://hz.meibo888.top/gtxuqtiwpu.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.hfpthk.cn/gtbqqqxdsi.html

TS:   if (x == null) {}
来源：http://hz.bjfxy.top/gtaakagwlu.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.jyoumei.cn/gtjneepdse.html

Go:   if x == nil {}
来源：http://hz.gaohongyu789.top/gtadpnjukc.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.pycfn.com/gtozwnsxyh.html

C#:   if (x is null) {}
来源：http://hz.ywan-chungtsiang.top/gtlcbusnlg.html

[P07] 防抖与节流
来源：http://hz.andypj.xyz/gtkztqjqkr.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.hysaishi.cn/gtsvjubbnn.html

PHP:  // 手写时间戳比较
来源：http://hz.nanxuanxn.top/gtimoadfqf.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.tianlin.xyz/gtumlozmsj.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.jqgufenzy.top/gtwisfaqcz.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.cheryme.top/gtqramxytf.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.hywenlv.cn/gtpvspnqrd.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.sufxvd.cn/gtdfcjmwqo.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.jyoumei.cn/gtidlvhger.html

[P08] 处理浮点精度问题
来源：http://hz.shzxlz.cn/gtftglnors.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.havefunace.top/gtxcckfflg.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.jianghu66.top/gtizsggggn.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.jqgfzy.top/gtjiwktvbr.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.cucudq.cn/gtefqvaocd.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.fzhhl.top/gtlgmcfcsb.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.52xcode.cn/gtrwgnmvpd.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.zhoulong.xyz/gtokzcdjwr.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.xinyue.icu/gtpvcrubwl.html

================================================================================
来源：http://hz.guowangkeji.top/gtdbwsuzaf.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.cheryme.top/gtipvyrtnf.html

================================================================================
来源：http://hz.fengsongda.top/gtzovxbytx.html

[Q01] 创建表
来源：http://hz.xylfe.cn/gtzxnncixw.html

CREATE TABLE users (
来源：http://hz.xuanzx.com/gtksagqtzw.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.ydzc1.top/gtfgcljljl.html

name VARCHAR(50) NOT NULL,
来源：http://hz.ehwqpu.com/gthcbjhiag.html

email VARCHAR(100) UNIQUE,
来源：http://hz.jyoumei.cn/gteqszffew.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.xingfuxueyuan.xyz/gtybligvij.html

);
来源：http://hz.yanxiufei.cn/gtfegkcrnp.html

[Q02] 创建带外键的表
来源：http://hz.meibo888.top/gtdeigbqay.html

CREATE TABLE orders (
来源：http://hz.jlsjyb.cn/gtojgcsmms.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.zhijiandao.cn/gtexoeapif.html

user_id INT NOT NULL,
来源：http://hz.yuxming.cn/gtnytdxtiw.html

amount DECIMAL(10, 2),
来源：http://hz.cqqwz.cn/gtvggmdirk.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.kuanghao11.cn/gthngtqtzp.html

);
来源：http://hz.shanyushiyangtech.top/gtqmizcjep.html

[Q03] 增加列
来源：http://hz.fzhhl.top/gttohlhkwc.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.yueranfly.top/gtpuzpiqhi.html

[Q04] 修改列类型
来源：http://hz.andypj.xyz/gtdmjmwvxe.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.birdmap.top/gtfzsicqzo.html

[Q05] 重命名列
来源：http://hz.sufxvd.cn/gtgnvwiric.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.cheryme.top/gtyagnamtx.html

[Q06] 删除列
来源：http://hz.shangyingyoupin.top/gtvudeqzki.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.jqgufenzy.top/gtteolwmmg.html

[Q07] 删除表
来源：http://hz.fzhhl.top/gtjotowrhg.html

DROP TABLE IF EXISTS orders;
来源：http://hz.aibaodan.cn/gtxalyqdxw.html

[Q08] 创建普通索引
来源：http://hz.shanyushiyangtech.top/gtzjohstso.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.nanxuanxn.top/gtskhitxzf.html

[Q09] 创建唯一索引
来源：http://hz.zycfv.cn/gtunzlzabu.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.dashuyun.cn/gtqbabxdpr.html

[Q10] 插入单行
来源：http://hz.ydjk.org.cn/gtlrxcqdjp.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.tianlin.xyz/gtrmhmpuxl.html

[Q11] 一次插入多行
来源：http://hz.yvedp.cn/gtfgjptchr.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.c1oappe.top/gtoknnvlhw.html

[Q12] 插入后取自增 ID
来源：http://hz.zhixingplan.top/gtmqisjtrh.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.shzxlz.cn/gtuqzzyuwf.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.bjfxy.top/gtdptzpxuc.html

[Q13] 忽略重复插入
来源：http://hz.c1oappe.top/gtmwrdzumo.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.zhongyouzk.top/gtcxvfrubs.html

[Q14] 存在则更新（upsert）
来源：http://hz.sufxvd.cn/gtwilpcmft.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.jinqigfzy.top/gttqjmibla.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.yangfankeji.com/gtxenspwla.html

[Q15] 查询全部
来源：http://hz.pengpengdd.cyou/gtahiydtrp.html

SELECT * FROM users;
来源：http://hz.zhoulong.xyz/gtyheshlrz.html

[Q16] 查询指定列
来源：http://hz.ybcxt.top/gtjhmwtujy.html

SELECT id, name FROM users;
来源：http://hz.xingfuxueyuan.xyz/gtylknuetp.html

[Q17] 条件查询
来源：http://hz.yuanzhike.top/gtncalmlrz.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.nwbrower.top/gtgnvhbxxc.html

[Q18] 模糊匹配
来源：http://hz.gotoacloud.top/gthlpkjfdy.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.svipenyu.cn/gtjtgxdnjn.html

[Q19] 范围查询
来源：http://hz.ivvv.top/gtjosbjhpq.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.xuetiantiany.cn/gtcfvyyxoa.html

[Q20] IN 列表
来源：http://hz.gzhubu.top/gtemgopeyr.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.yuanzhike.top/gtxcynkxvj.html

[Q21] 空值判断
来源：http://hz.zhiwuduotai.top/gttibidlky.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.daria6918.cn/gtrxdvanyx.html

[Q22] 排序
来源：http://hz.shzxlz.cn/gtbtwpqttg.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.jlsjyb.cn/gtpqhypjdo.html

[Q23] 分页
来源：http://hz.zhijiandao.cn/gtgnvpplgb.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.jinqigufen.top/gtccibrpbu.html

[Q24] 去重
来源：http://hz.smart0.xyz/gtuyhrhooy.html

SELECT DISTINCT city FROM users;
来源：http://hz.nanxuanxn.top/gtobtnprws.html

[Q25] 只取前 N 条
来源：http://hz.cqqwz.cn/gtmqhmphls.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.sufxvd.cn/gtbpufdpdl.html

[Q26] 计数
来源：http://hz.dashuyun.cn/gtjrvovzdk.html

SELECT COUNT(*) FROM users;
来源：http://hz.iojbl.cn/gttedkylee.html

[Q27] 条件计数
来源：http://hz.xingfuxueyuan.xyz/gtjaniiifi.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.9152youxi.cn/gtdycrmyhe.html

[Q28] 求和与平均
来源：http://hz.yj202588.top/gtgksfofze.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.ywan-chungtsiang.top/gtbkfbxymy.html

[Q29] 最大最小值
来源：http://hz.hammf.cn/gtuftbuzan.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.jyoumei.cn/gtiprpopbt.html

[Q30] 分组统计
来源：http://hz.zhiwuduotai.top/gtzrnnoaqf.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.wangshuangyany.cn/gtjrpswerx.html

[Q31] 分组后过滤
来源：http://hz.daria6918.cn/gtjgxeymqb.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.havefunace.top/gtnpikalkh.html

[Q32] 分组拼接字符串
来源：http://hz.yuxming.cn/gtphclawmi.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.hnxiangtu.top/gtvnqtaruy.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.zhaomingkeji.xyz/gtfbovpzwd.html

[Q33] 多列分组
来源：http://hz.aibaodan.cn/gtvynislki.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.sufxvd.cn/gtkoarpika.html

[Q34] 每组取第一条
来源：http://hz.gzhubu.top/gtczxrfgdz.html

SELECT * FROM (
来源：http://hz.guowangkeji.top/gtpawuzrhb.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.zhoulong.xyz/gtybatummi.html

) t WHERE rn = 1;
来源：http://hz.aibaodan.cn/gtuixkcbbn.html

[Q35] 内连接
来源：http://hz.hongshengwenyu.top/gteivgokjd.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.jinyuanbaomall.cn/gttrnohxjx.html

[Q36] 左连接
来源：http://hz.yangfankeji.com/gtycxpcaej.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.haohaochexian.top/gtqngpjcmw.html

[Q37] 右连接
来源：http://hz.havefunace.top/gteqazytmp.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.daria6918.cn/gtzaytntxv.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.haohaochexian.top/gtsqsgjynz.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.chenlongwang.top/gtvwickimn.html

[Q39] 自连接（查上下级）
来源：http://hz.birdmap.top/gtevhuszqz.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.redwolf501.top/gtygfzjhcd.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.chenjidiqi.icu/gtslsobgbc.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.316326.xyz/gtodyxezej.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.xuanzx.com/gterywmyuc.html

[Q41] 多表连接
来源：http://hz.yueranfly.top/gtjgusdyud.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.c1oappe.top/gttrhzpqwx.html

JOIN users u ON u.id = o.user_id
来源：http://hz.9152youxi.cn/gtpplzcpmw.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.shangyingyoupin.top/gtwexkdezu.html

[Q42] 连接条件附加过滤
来源：http://hz.xingfuxueyuan.xyz/gtissmzmvz.html

SELECT u.name, o.amount FROM users u
来源：http://hz.feifeiyinyue.top/gttcfhqgzj.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.nanxuanxn.top/gthxylspsl.html

[Q43] 标量子查询
来源：http://hz.jianghu66.top/gtwxmsuywk.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.hnqzz.top/gtwgowcjrn.html

[Q44] IN 子查询
来源：http://hz.jinyuanbaomall.cn/gtircxnbvt.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.shuidangran.top/gtdzwntwjj.html

[Q45] EXISTS 判断存在
来源：http://hz.52xcode.cn/gttnwdghjv.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.xziqi.cn/gtighrgedj.html


<!-- 参考信息 -->