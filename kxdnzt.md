代发 wailian999

[N05] 最大公约数
来源：http://hz.guannengcc.top/gtirarulvd.html

Py:   math.gcd(a, b)
来源：http://hz.shzxlz.cn/gtmbnepbsg.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.xziqi.cn/gtwuhahtdq.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.316326.xyz/gtxmnzhvto.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.aibaodan.cn/gtmpjrusgb.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.yuanzhike.top/gtnozvbndm.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.c1oappe.top/gtksmbagcj.html

Ruby: a.gcd(b)
来源：http://hz.nanxinkj.top/gtozzvalhb.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.jlsjyb.cn/gtljxvddhy.html

[N06] 判断回文字符串
来源：http://hz.guowangkeji.top/gtlqiykqoi.html

Py:   s == s[::-1]
来源：http://hz.52xcode.cn/gtvkaumltf.html

PHP:  $s === strrev($s);
来源：http://hz.zycfv.cn/gtvojojuws.html

JS:   s === [...s].reverse().join("")
来源：http://hz.ppjwa.cn/gtratexbrm.html

TS:   s === [...s].reverse().join("")
来源：http://hz.ivvv.top/gtpmwsrotb.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.zycfv.cn/gtpljfatld.html

Go:   // 双指针从两端比较
来源：http://hz.iojbl.cn/gtkjilxwzj.html

Ruby: s == s.reverse
来源：http://hz.snrcjt.cn/gtihcdsrdt.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.guannengcc.top/gtctllpqtq.html

[N07] 两数之和（返回下标）
来源：http://hz.aibaodan.cn/gtvchnrqph.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.shangyingyoupin.top/gtdhafzbgr.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.zhijiandao.cn/gtktzzgvti.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.gaohongyu789.top/gtltxbsdec.html

TS:   // 手写 Map<string, number>
来源：http://hz.chenlongwang.top/gtsxnyxbhj.html

Java: // 手写 HashMap
来源：http://hz.yvedp.cn/gtncpbgykw.html

Go:   // 手写 map[int]int
来源：http://hz.ppjwa.cn/gtjficnpjz.html

Ruby: // 手写 Hash
来源：http://hz.zdqjudy.top/gtmnoryrjw.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.jqgufenzy.top/gtbyxziiqd.html

[N08] 生成全排列
来源：http://hz.hammf.cn/gteovkzcpb.html

Py:   itertools.permutations(arr)
来源：http://hz.hfpthk.cn/gtdjcdkxfl.html

PHP:  // 手写递归交换
来源：http://hz.meibo888.top/gtkfurpnyd.html

JS:   // 手写回溯递归
来源：http://hz.yj20258888.top/gtcmbmjdpp.html

TS:   // 手写回溯递归
来源：http://hz.shuidangran.top/gtkffirbfq.html

Java: // 手写回溯递归
来源：http://hz.andypj.xyz/gtvpldqrac.html

Go:   // 手写回溯递归
来源：http://hz.jiagoushi.top/gtdlbdaaiy.html

Ruby: arr.permutation.to_a
来源：http://hz.pengpengdd.cyou/gtxdvrjzbk.html

C#:   // 手写回溯递归
来源：http://hz.zhijiandao.cn/gthawfjurd.html

[N09] 栈与队列
来源：http://hz.316326.xyz/gtnazvlooi.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.nwbrower.top/gtxudxdkbs.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.cqqwz.cn/gtbplgffqd.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.fengsongda.top/gtgvckclxc.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.gaohongyu789.top/gtkycqeind.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.fengsongda.top/gtgkwmowvd.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.zhongyouzk.top/gtdoybxpfo.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.daxiang520.top/gtwlrciftq.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.guannengcc.top/gtbuwmszru.html

[N10] 链表节点定义
来源：http://hz.52xcode.cn/gtvnugoiei.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.aibaodan.cn/gtxxlrhdkr.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.xuetiantiany.cn/gtaqtvauhm.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.yj20258.top/gtvllsvooi.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.jqgfzy.top/gtnblkccfn.html

Java: class Node { int v; Node next; }
来源：http://hz.hysaishi.cn/gtepyatzdp.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.tanke756.top/gtlplniuqy.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.yueranfly.top/gtkpcnjbtc.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.ivvv.top/gtzwhxcwti.html

[N11] 二叉树中序遍历
来源：http://hz.52xcode.cn/gtclturthg.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.jqgufenzy.top/gtvzqtkhuy.html

PHP:  // 手写递归函数
来源：http://hz.iojbl.cn/gtscpbcxxs.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.hywenlv.cn/gthqqbftub.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.zhixingplan.top/gtpxuhmtiw.html

Java: // 手写递归
来源：http://hz.hammf.cn/gtjdzrmgqs.html

Go:   // 手写递归
来源：http://hz.redwolf501.top/gtcamhwvwe.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.hongshengwenyu.top/gtpdgzwiuj.html

C#:   // 手写递归
来源：http://hz.cucudq.cn/gtuornqhxv.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.jinqigfzy.top/gtqixpsgac.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.jlsjyb.cn/gtwxyuhoro.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.andypj.xyz/gteihzzfme.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.hnxiangtu.top/gtmulikdnb.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.jlsjyb.cn/gttdyrzxts.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.haohaochexian.top/gtuxjailze.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.pengpengdd.cyou/gtvwgedqrp.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.yvedp.cn/gtcczoyypl.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.meibo888.top/gtcnrjnmhs.html

================================================================================
来源：http://hz.shangyingyoupin.top/gtjhaummet.html

O. 并发与异步
来源：http://hz.ybcxt.top/gtnavhcocw.html

================================================================================
来源：http://hz.daxiang520.top/gthyxbycdb.html

[O01] 启动一个线程
来源：http://hz.nanxuanxn.top/gtklxoqtvq.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.yonumen.top/gtcuktkzzj.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.yongpay.top/gtmwzkzyjh.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.jlsjyb.cn/gtbcucdvnf.html

TS:   // 同 JS
来源：http://hz.ydzc1.top/gtdhbdjceb.html

Java: new Thread(() -> f()).start()
来源：http://hz.nwbrower.top/gtxdkgalhe.html

Go:   go f()
来源：http://hz.jinqigfzy.top/gtxwxbhgow.html

Ruby: Thread.new { f }
来源：http://hz.ehwqpu.com/gtvdrhohjx.html

C#:   Task.Run(() => F());
来源：http://hz.nwbrower.top/gtufkoqhum.html

[O02] 使用线程池
来源：http://hz.zhoulong.xyz/gtjtlqotyi.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.yonumen.top/gtxiyifgnn.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.xuanzx.com/gtegbnfgyj.html

JS:   // worker_threads 线程池
来源：http://hz.zdqjudy.top/gtrwuytgss.html

TS:   // worker_threads 线程池
来源：http://hz.svipenyu.cn/gttqwfivps.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.daria6918.cn/gtmdankkog.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.hnxiangtu.top/gtuwunraae.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.cucudq.cn/gtrfmxyocj.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.jyoumei.cn/gtajeujzxv.html

[O03] 加锁保护共享数据
来源：http://hz.jianghu66.top/gtpuemnxmw.html

Py:   with lock: shared += 1
来源：http://hz.yvedp.cn/gtieivtbbl.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.gzhubu.top/gtprxiiirq.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.hnxiangtu.top/gtgccfnaab.html

TS:   // 同 JS
来源：http://hz.zhaomingkeji.xyz/gtogpyadpn.html

Java: synchronized (this) { shared++; }
来源：http://hz.cqqwz.cn/gtzwufwhrf.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.gotoacloud.top/gtogmuceaq.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.yonumen.top/gtylygylba.html

C#:   lock (gate) { shared++; }
来源：http://hz.dashuyun.cn/gtusbutcoh.html

[O04] 定义异步函数并等待
来源：http://hz.zhaomingkeji.xyz/gttpnchozb.html

Py:   async def f():⏎    await g()
来源：http://hz.jqgfzy.top/gtgjrthepx.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.bjfxy.top/gtspkodpag.html

JS:   async function f() { await g(); }
来源：http://hz.shanyushiyangtech.top/gtyrwvwawi.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.sweek.top/gtcrfdnixh.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.yuxming.cn/gtnvmicbbk.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.feifeiyinyue.top/gtinumbybs.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.daxiang520.top/gtcrgxgrej.html

C#:   async Task F() { await G(); }
来源：http://hz.ivvv.top/gtmoxmutuq.html

[O05] 并发执行并等待全部完成
来源：http://hz.bjfxy.top/gteoyeaxkz.html

Py:   asyncio.gather(*tasks)
来源：http://hz.mhx1999.top/gtjwkqbvtc.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.vqdsnc.cn/gtbpsfpxqe.html

JS:   await Promise.all(tasks)
来源：http://hz.52xcode.cn/gtthfvipfu.html

TS:   await Promise.all(tasks)
来源：http://hz.pycfn.com/gtgmhierze.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.zycfv.cn/gtngzmcifx.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.cdnleiting.top/gtyizegvnp.html

Ruby: threads.map(&:join)
来源：http://hz.hfpthk.cn/gtirvhsxfk.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.sysykeji.top/gtpvcgqqbu.html

[O06] 使用进程池
来源：http://hz.zhiwuduotai.top/gtpvrihoxr.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.nanxinkj.top/gtqfgbaokm.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.nwbrower.top/gtwkeozmfb.html

JS:   // child_process / cluster 模块
来源：http://hz.daxiang520.top/gtxvvdzeuc.html

TS:   // child_process / cluster 模块
来源：http://hz.hammf.cn/gtwnyqdloj.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.hfpthk.cn/gtpbdsschc.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.zhengqikj.top/gtpberkekm.html

Ruby: // fork 块
来源：http://hz.c1oappe.top/gtafhsfcyt.html

C#:   Parallel.For
来源：http://hz.dashuyun.cn/gtthcreliz.html

================================================================================
来源：http://hz.havefunace.top/gtycxxvxsp.html

P. 常用工具函数
来源：http://hz.zycfv.cn/gtunyqmbol.html

================================================================================
来源：http://hz.yvedp.cn/gtnlnvnvpk.html

[P01] 生成 UUID
来源：http://hz.ppjwa.cn/gtlrebjzrr.html

Py:   str(uuid.uuid4())
来源：http://hz.nwbrower.top/gtjhbpfgyc.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.smart0.xyz/gtkjioyfvs.html

JS:   crypto.randomUUID()
来源：http://hz.guowangkeji.top/gtghnwvvko.html

TS:   crypto.randomUUID()
来源：http://hz.nanxinkj.top/gtrsquwjsl.html

Java: UUID.randomUUID().toString()
来源：http://hz.hywenlv.cn/gtbmtbphnm.html

Go:   // 用 github.com/google/uuid
来源：http://hz.nwbrower.top/gtqmzmgmtp.html

Ruby: SecureRandom.uuid
来源：http://hz.jinyuanbaomall.cn/gttnqvrnug.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.cheryme.top/gtwwakicpm.html

[P02] MD5 / SHA256 摘要
来源：http://hz.zhongyouzk.top/gtxhajdcoo.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.snrcjt.cn/gtenvwjwjk.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.0kj1m.cn/gtdfppvflb.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.shuidangran.top/gtelirxilj.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.shanyushiyangkeji.top/gtukxpxoag.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.nwbrower.top/gtnzncrvgj.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.daria6918.cn/gtuzerthua.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.52xcode.cn/gtjnfbtjbx.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.chenzaomai.com/gtfbezjooo.html

[P03] 生成短随机字符串
来源：http://hz.hysaishi.cn/gtnrmxxwid.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.chenlongwang.top/gtwtzwwirq.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.yj202588.top/gtlfenyejx.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.yj20258.top/gtnddartoa.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.xziqi.cn/gttvvmvsaw.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.hfpthk.cn/gtzlsvqnvi.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.ivvv.top/gtspqsobxp.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.yj202588.top/gtiytscvoo.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.yuxming.cn/gtohjyajjs.html

[P04] 求长度
来源：http://hz.andypj.xyz/gtccfimold.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.316326.xyz/gtewctctqe.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.316326.xyz/gtkkhylirj.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.jyoumei.cn/gtxjkpdcxp.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.dashuyun.cn/gtqnttjdac.html

Java: list.size();  map.size();  s.length()
来源：http://hz.vqdsnc.cn/gthtemsipm.html

Go:   len(arr);  len(m)
来源：http://hz.jiagoushi.top/gtgarcphsj.html

Ruby: x.length;  x.size
来源：http://hz.jinqigufen.top/gtlgvyaqky.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.kuanghao11.cn/gtcnzboytv.html

[P05] 判断两个对象内容是否相等
来源：http://hz.zycfv.cn/gtnochkrby.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.nanxuanxn.top/gtikxbomid.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.chenlongwang.top/gtyvkkkwun.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.vqdsnc.cn/gtmbooslnl.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.yj20258.top/gtetsilmln.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.snrcjt.cn/gtaxiatgts.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.gaohongyu789.top/gtedybxgdt.html

Ruby: a == b
来源：http://hz.gogol.net.cn/gtgabvivvg.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.tian-w.cn/gttdfvcbfl.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.yonumen.top/gtabdfukqn.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.feifeiyinyue.top/gtoezmcgwc.html

PHP:  if (empty($x)) {}
来源：http://hz.chenjidiqi.icu/gtgpcorriy.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.fzhhl.top/gtadygtvub.html

TS:   if (x == null) {}
来源：http://hz.havefunace.top/gtjmgzamcw.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.hongshengwenyu.top/gtljjpldby.html

Go:   if x == nil {}
来源：http://hz.yanxiufei.cn/gtnsrilviw.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.yj202588.top/gtfpfjqtfc.html

C#:   if (x is null) {}
来源：http://hz.hfpthk.cn/gtbqxptzkw.html

[P07] 防抖与节流
来源：http://hz.cheryme.top/gtjczjakqu.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.ydzc1.top/gtocugyusp.html

PHP:  // 手写时间戳比较
来源：http://hz.birdmap.top/gtreayfksw.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.fzhhl.top/gtfgqyqqkr.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.mhx1999.top/gtrbbrxnvj.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.ybcxt.top/gtkcgeiied.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.redwolf501.top/gtzftxfqhh.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.gogol.net.cn/gtiqyfkwmo.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.hammf.cn/gtgjycjvod.html

[P08] 处理浮点精度问题
来源：http://hz.mhx1999.top/gtyozmixin.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.pengpengdd.cyou/gtnekxbnhs.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.jinqigufen.top/gtxypfyyes.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.sweek.top/gtfjcvbrib.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.xziqi.cn/gtebpcrsex.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.52xcode.cn/gtlfojblgc.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.jqgfzy.top/gtovubcaiw.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.hysaishi.cn/gtwconzgee.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.jinqigufen.top/gtzeugjloz.html

================================================================================
来源：http://hz.jiagoushi.top/gtsmpyetnp.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.xingfuxueyuan.xyz/gtdpfmllka.html

================================================================================
来源：http://hz.hfpthk.cn/gtlymcdpif.html

[Q01] 创建表
来源：http://hz.chenjidiqi.icu/gtphvejhej.html

CREATE TABLE users (
来源：http://hz.9152youxi.cn/gttpovtsvw.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.cqqwz.cn/gttzwvyuse.html

name VARCHAR(50) NOT NULL,
来源：http://hz.meibo888.top/gtizrmxhxk.html

email VARCHAR(100) UNIQUE,
来源：http://hz.xuanzx.com/gtmujdthit.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.zhijiandao.cn/gtmruszrls.html

);
来源：http://hz.9152youxi.cn/gtsucfrwdu.html

[Q02] 创建带外键的表
来源：http://hz.zhijiandao.cn/gtapmscoke.html

CREATE TABLE orders (
来源：http://hz.ydzc1.top/gtebwwrzne.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.yj202588.top/gtdkxbpdas.html

user_id INT NOT NULL,
来源：http://hz.guannengcc.top/gtqqeserwi.html

amount DECIMAL(10, 2),
来源：http://hz.daria6918.cn/gtubcmlbpv.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.ppjwa.cn/gttgwpuzam.html

);
来源：http://hz.guowangkeji.top/gtzkyjnkbl.html

[Q03] 增加列
来源：http://hz.sufxvd.cn/gtdpstnrai.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.hongshengwenyu.top/gtorxwxvyr.html

[Q04] 修改列类型
来源：http://hz.yueranfly.top/gtwuvzpnzm.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.svipenyu.cn/gtivgicmki.html

[Q05] 重命名列
来源：http://hz.ydzc1.top/gtvnvnnrsa.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.xinyue.icu/gtflzfadgp.html

[Q06] 删除列
来源：http://hz.andypj.xyz/gteslzzkwg.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.c1oappe.top/gtejiolxjz.html

[Q07] 删除表
来源：http://hz.jianghu66.top/gtgqbaaltr.html

DROP TABLE IF EXISTS orders;
来源：http://hz.havefunace.top/gtukqtchcf.html

[Q08] 创建普通索引
来源：http://hz.feifeiyinyue.top/gtypmdfezq.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.guannengcc.top/gtytkdlcwu.html

[Q09] 创建唯一索引
来源：http://hz.ehwqpu.com/gtuaerihay.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.zhixingplan.top/gtubjnrepm.html

[Q10] 插入单行
来源：http://hz.fengsongda.top/gtywzfalge.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.kuanghao11.cn/gtxycnxsjx.html

[Q11] 一次插入多行
来源：http://hz.jqgufenzy.top/gthvkykenl.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.yvedp.cn/gtbgntjpyy.html

[Q12] 插入后取自增 ID
来源：http://hz.vqdsnc.cn/gtdnzuilec.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.chenzaomai.com/gtprhckrsk.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.c1oappe.top/gtwekppqrr.html

[Q13] 忽略重复插入
来源：http://hz.xylfe.cn/gtrfopqgfl.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.52xcode.cn/gtnpcybxoy.html

[Q14] 存在则更新（upsert）
来源：http://hz.gzhubu.top/gthhwnxskb.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.zhaomingkeji.xyz/gttfdsedkj.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.wangdashe.top/gtsqgjkvih.html

[Q15] 查询全部
来源：http://hz.chenlongwang.top/gtckrnetde.html

SELECT * FROM users;
来源：http://hz.nwbrower.top/gtxcshtjjs.html

[Q16] 查询指定列
来源：http://hz.xingfuxueyuan.xyz/gthafhzrko.html

SELECT id, name FROM users;
来源：http://hz.nwbrower.top/gtifispbhe.html

[Q17] 条件查询
来源：http://hz.cashguo.top/gttqtzwgqq.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.zhongyouzk.top/gtkatfyxvs.html

[Q18] 模糊匹配
来源：http://hz.birdmap.top/gtdiokfgme.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.xziqi.cn/gtkkxivuod.html

[Q19] 范围查询
来源：http://hz.daria6918.cn/gtkptiaazr.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.tianlin.xyz/gtuoijgqrd.html

[Q20] IN 列表
来源：http://hz.fengsongda.top/gtcjthwiwb.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.hysaishi.cn/gtmncweaui.html

[Q21] 空值判断
来源：http://hz.fzhhl.top/gtkyeobzox.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.kuanghao11.cn/gtcrihwlxz.html

[Q22] 排序
来源：http://hz.tianlin.xyz/gtfalbgukx.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.c1oappe.top/gtzfbqrawk.html

[Q23] 分页
来源：http://hz.dianchejie.cn/gtynhgokps.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.fengsongda.top/gtcngagbsh.html

[Q24] 去重
来源：http://hz.shangyingyoupin.top/gtcvujhwsi.html

SELECT DISTINCT city FROM users;
来源：http://hz.jlsjyb.cn/gtnuntsgzp.html

[Q25] 只取前 N 条
来源：http://hz.hysaishi.cn/gtyqmtkinp.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.dianchejie.cn/gtflrxxxor.html

[Q26] 计数
来源：http://hz.quarkkingdee.top/gtlkvjmqok.html

SELECT COUNT(*) FROM users;
来源：http://hz.yvedp.cn/gtkplwlyvx.html

[Q27] 条件计数
来源：http://hz.iojbl.cn/gtkocpurix.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.guowangkeji.top/gtmzhgbzte.html

[Q28] 求和与平均
来源：http://hz.c1oappe.top/gtuchygdcf.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.smart0.xyz/gtfllummme.html

[Q29] 最大最小值
来源：http://hz.pycfn.com/gtkcjmqjqj.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.hongshengwenyu.top/gtbskqneit.html

[Q30] 分组统计
来源：http://hz.andypj.xyz/gtjycyiihn.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.jyoumei.cn/gtmkqssyii.html

[Q31] 分组后过滤
来源：http://hz.iojbl.cn/gthehcovre.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.cqqwz.cn/gtejdmjsqv.html

[Q32] 分组拼接字符串
来源：http://hz.dianchejie.cn/gtzduuspad.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.jqgufenzy.top/gtdbjsqnwk.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.jinqigufen.top/gtxcdqqkml.html

[Q33] 多列分组
来源：http://hz.guannengcc.top/gtmpwlvdul.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.ydzc1.top/gtbubuibjp.html

[Q34] 每组取第一条
来源：http://hz.yueranfly.top/gtxyxkqbdj.html

SELECT * FROM (
来源：http://hz.xziqi.cn/gtqojotyhs.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.gogol.net.cn/gttnirktal.html

) t WHERE rn = 1;
来源：http://hz.kuanghao11.cn/gtodxrarne.html

[Q35] 内连接
来源：http://hz.zycfv.cn/gtudbqmbrh.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.sysykeji.top/gtzkeqfbnc.html

[Q36] 左连接
来源：http://hz.fengsongda.top/gttzyzzfou.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.jinqigfzy.top/gtacxqaunv.html

[Q37] 右连接
来源：http://hz.zhongyouzk.top/gtwvnjhkqs.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.gogol.net.cn/gtlgpsqbbv.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.pengpengdd.cyou/gtxuebcbiw.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.fengsongda.top/gtgwxnxiyb.html

[Q39] 自连接（查上下级）
来源：http://hz.zhaomingkeji.xyz/gtqgmreemr.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.fengsongda.top/gthrgednrm.html


<!-- 参考信息 -->