代发 wailian999

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.shangyingyoupin.top/gtxytqfqzo.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.sxryk.cn/gtdokbqkxb.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.daria6918.cn/gtvgkvemch.html

Ruby: a.gcd(b)
来源：http://hz.c1oappe.top/gttygjikoe.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.ydzc1.top/gtmbixpkqf.html

[N06] 判断回文字符串
来源：http://hz.nanxuanxn.top/gtqtpqayvj.html

Py:   s == s[::-1]
来源：http://hz.cheryme.top/gthwqcxrym.html

PHP:  $s === strrev($s);
来源：http://hz.ehwqpu.com/gtgdqhlred.html

JS:   s === [...s].reverse().join("")
来源：http://hz.shzxlz.cn/gtdmqtepxk.html

TS:   s === [...s].reverse().join("")
来源：http://hz.sxryk.cn/gttnauzadi.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.quarkkingdee.top/gtdymaxflu.html

Go:   // 双指针从两端比较
来源：http://hz.gogol.net.cn/gtaopavimh.html

Ruby: s == s.reverse
来源：http://hz.jinyuanbaomall.cn/gtmopyrekg.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.snrcjt.cn/gtoarrkjta.html

[N07] 两数之和（返回下标）
来源：http://hz.birdmap.top/gtyjasefxj.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.chenzaomai.com/gtufgivlmz.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.hnxiangtu.top/gttcrxspcf.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.hfpthk.cn/gttrxzbfqf.html

TS:   // 手写 Map<string, number>
来源：http://hz.gotoacloud.top/gtbmjjyyas.html

Java: // 手写 HashMap
来源：http://hz.tian-w.cn/gtxjqjfpdn.html

Go:   // 手写 map[int]int
来源：http://hz.cdnleiting.top/gtjeoajzug.html

Ruby: // 手写 Hash
来源：http://hz.feifeiyinyue.top/gtfzocawam.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.zhaomingkeji.xyz/gtrdohpjhi.html

[N08] 生成全排列
来源：http://hz.zhixingplan.top/gtjhozfhvy.html

Py:   itertools.permutations(arr)
来源：http://hz.dashuyun.cn/gtioopmzuy.html

PHP:  // 手写递归交换
来源：http://hz.fzhhl.top/gtqejfzohu.html

JS:   // 手写回溯递归
来源：http://hz.yanxiufei.cn/gtvbakycwi.html

TS:   // 手写回溯递归
来源：http://hz.jiagoushi.top/gtcstskoqb.html

Java: // 手写回溯递归
来源：http://hz.gotoacloud.top/gtuukggeur.html

Go:   // 手写回溯递归
来源：http://hz.hongshengwenyu.top/gtmufnlakr.html

Ruby: arr.permutation.to_a
来源：http://hz.hfpthk.cn/gtrqwbxdum.html

C#:   // 手写回溯递归
来源：http://hz.cucudq.cn/gtnxsmnrne.html

[N09] 栈与队列
来源：http://hz.nanxinkj.top/gtqsammxlr.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.yj20258888.top/gtszpubtqn.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.zhiwuduotai.top/gtnasbuxho.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.shuidangran.top/gtxxrjgvdu.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.shanyushiyangkeji.top/gtatwuyrqn.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.pycfn.com/gtspqedpxc.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.sxryk.cn/gtupclqxjd.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.fengsongda.top/gtpcmjwacz.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.pycfn.com/gtroannlhj.html

[N10] 链表节点定义
来源：http://hz.jqgfzy.top/gtztjywtby.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.shanyushiyangkeji.top/gttvqnitgk.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.havefunace.top/gtmobhohfw.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.yongpay.top/gtaohrfiug.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.feifeiyinyue.top/gtpalehppz.html

Java: class Node { int v; Node next; }
来源：http://hz.yonumen.top/gtxcppuawu.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.fengsongda.top/gtougerubi.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.yj20258.top/gtvpuwvqfa.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.quarkkingdee.top/gtpxqaxont.html

[N11] 二叉树中序遍历
来源：http://hz.yonumen.top/gteiymgeiw.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.zhongyouzk.top/gtjqkufjdn.html

PHP:  // 手写递归函数
来源：http://hz.tianlin.xyz/gtptinlmtt.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.guowangkeji.top/gthpzkzucq.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.meibo888.top/gtknavwurz.html

Java: // 手写递归
来源：http://hz.aibaodan.cn/gtfxbifemu.html

Go:   // 手写递归
来源：http://hz.wangshuangyany.cn/gtzjbsewqm.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.ehwqpu.com/gthqodkpaf.html

C#:   // 手写递归
来源：http://hz.daxiang520.top/gtcjxwljhn.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.snrcjt.cn/gtlktkcwli.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.cashguo.top/gtwnrqkbje.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.jlsjyb.cn/gtafvgkzrv.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.xingfuxueyuan.xyz/gtypauxusr.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.xinyue.icu/gtnfphebve.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.zhijiandao.cn/gtnutbugsp.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.shangyingyoupin.top/gtrjuzbgio.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.9152youxi.cn/gtwgcjhoha.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.wangshuangyany.cn/gtphgixjnb.html

================================================================================
来源：http://hz.zycfv.cn/gtagncidlf.html

O. 并发与异步
来源：http://hz.jyoumei.cn/gtcotswmbd.html

================================================================================
来源：http://hz.yj20258.top/gtgwvmwmwj.html

[O01] 启动一个线程
来源：http://hz.ybcxt.top/gtkjosxuyr.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.gotoacloud.top/gtzraaalks.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.redwolf501.top/gtodryysgz.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.zhijiandao.cn/gtqhqrdvsa.html

TS:   // 同 JS
来源：http://hz.jyoumei.cn/gtaivasthx.html

Java: new Thread(() -> f()).start()
来源：http://hz.redwolf501.top/gtlcvivvxy.html

Go:   go f()
来源：http://hz.chenjidiqi.icu/gtpfbmtnql.html

Ruby: Thread.new { f }
来源：http://hz.gotoacloud.top/gtnqsvsmar.html

C#:   Task.Run(() => F());
来源：http://hz.aibaodan.cn/gtoipxrzsf.html

[O02] 使用线程池
来源：http://hz.yueranfly.top/gtfiddenzk.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.zhijiandao.cn/gtcssgdtez.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.shanyushiyangkeji.top/gtnnnsmrfc.html

JS:   // worker_threads 线程池
来源：http://hz.dianchejie.cn/gtpqdojblx.html

TS:   // worker_threads 线程池
来源：http://hz.jqgufenzy.top/gtytgtzpbj.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.9152youxi.cn/gtefcplqik.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.hfpthk.cn/gtfjekrzhx.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.zhaomingkeji.xyz/gtgfsffbnb.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.yvedp.cn/gtrfpmifkt.html

[O03] 加锁保护共享数据
来源：http://hz.cdnleiting.top/gtxmlzsgic.html

Py:   with lock: shared += 1
来源：http://hz.zhengqikj.top/gtjeiewrln.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.hammf.cn/gthtfncxuh.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.tanke756.top/gtohzwhfoy.html

TS:   // 同 JS
来源：http://hz.tian-w.cn/gtwtaduakc.html

Java: synchronized (this) { shared++; }
来源：http://hz.9152youxi.cn/gtwezxflyi.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.iojbl.cn/gtfoqjvpuz.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.sweek.top/gtruczdwph.html

C#:   lock (gate) { shared++; }
来源：http://hz.jinqigufen.top/gtvdvaijxb.html

[O04] 定义异步函数并等待
来源：http://hz.bjfxy.top/gtixjrejzm.html

Py:   async def f():⏎    await g()
来源：http://hz.tanke756.top/gtzloimzvf.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.aibaodan.cn/gthfdjnhvz.html

JS:   async function f() { await g(); }
来源：http://hz.jinqigufen.top/gtuakhyoki.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.yanxiufei.cn/gtmpealkyx.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.yvedp.cn/gtzqbeecos.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.hongshengwenyu.top/gtndysxwoi.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.cdnleiting.top/gtrjhbchwk.html

C#:   async Task F() { await G(); }
来源：http://hz.zhiwuduotai.top/gtxkqnhqmw.html

[O05] 并发执行并等待全部完成
来源：http://hz.ywan-chungtsiang.top/gtxzndoeky.html

Py:   asyncio.gather(*tasks)
来源：http://hz.yueranfly.top/gtgvnhsapx.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.pengpengdd.cyou/gtiritgtoc.html

JS:   await Promise.all(tasks)
来源：http://hz.gogol.net.cn/gtgjujeyfy.html

TS:   await Promise.all(tasks)
来源：http://hz.chenjidiqi.icu/gtnprbgeih.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.yj20258.top/gtxdhgsmvs.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.quarkkingdee.top/gtpjokngip.html

Ruby: threads.map(&:join)
来源：http://hz.pengpengdd.cyou/gtbcslxpru.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.ybcxt.top/gtppczwaef.html

[O06] 使用进程池
来源：http://hz.jqgfzy.top/gtnamzzxtl.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.chenjidiqi.icu/gtpbvgubdc.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.zdqjudy.top/gtoitwiyan.html

JS:   // child_process / cluster 模块
来源：http://hz.chenlongwang.top/gtitnjrtnl.html

TS:   // child_process / cluster 模块
来源：http://hz.gzhubu.top/gtdjdksese.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.ydzc1.top/gtikoeedkx.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.sxryk.cn/gtchqentle.html

Ruby: // fork 块
来源：http://hz.bjfxy.top/gtjosfukhi.html

C#:   Parallel.For
来源：http://hz.zhongyouzk.top/gtcdjdtpia.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gtptezgwau.html

P. 常用工具函数
来源：http://hz.redwolf501.top/gtrzaeiltk.html

================================================================================
来源：http://hz.tianlin.xyz/gtetbvmyhu.html

[P01] 生成 UUID
来源：http://hz.jinyuanbaomall.cn/gttjhtydfc.html

Py:   str(uuid.uuid4())
来源：http://hz.9152youxi.cn/gtiqjwylzs.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.xuanzx.com/gtovzaqumm.html

JS:   crypto.randomUUID()
来源：http://hz.tanke756.top/gtmvfdzhse.html

TS:   crypto.randomUUID()
来源：http://hz.andypj.xyz/gthnvohqll.html

Java: UUID.randomUUID().toString()
来源：http://hz.snrcjt.cn/gtncdsjsuu.html

Go:   // 用 github.com/google/uuid
来源：http://hz.chenlongwang.top/gtkcjnlxrt.html

Ruby: SecureRandom.uuid
来源：http://hz.sweek.top/gtxjtpresq.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.wangdashe.top/gtmjnszhen.html

[P02] MD5 / SHA256 摘要
来源：http://hz.cashguo.top/gtsidypvob.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.yanxiufei.cn/gtpdzirgbz.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.dashuyun.cn/gtnehlgjfq.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.cqqwz.cn/gtxvlwqnze.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.aibaodan.cn/gtnzyegtkv.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.haohaochexian.top/gtobfsrhwb.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.ydjk.org.cn/gtrfjyerur.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.0kj1m.cn/gtggkqbugd.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.jinghuilouyu.cn/gterkayhps.html

[P03] 生成短随机字符串
来源：http://hz.shanyushiyangkeji.top/gtmelfbvre.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.hnxiangtu.top/gtvyylzouo.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.52xcode.cn/gtakiogzzw.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.jqgfzy.top/gtuztmdaab.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.ydzc1.top/gtbspkijon.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.zhongyouzk.top/gthymgitpf.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.gaohongyu789.top/gtcfxlqbuf.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.mhx1999.top/gtqdnkbqzo.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.nwbrower.top/gtuvcbwark.html

[P04] 求长度
来源：http://hz.zhiwuduotai.top/gthgrrtntd.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.shzxlz.cn/gthphophwg.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.shangyingyoupin.top/gtatvrvckt.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.chenzaomai.com/gttdzaksgg.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.yvedp.cn/gtfgzwjwdx.html

Java: list.size();  map.size();  s.length()
来源：http://hz.yonumen.top/gtpbveurqe.html

Go:   len(arr);  len(m)
来源：http://hz.hongshengwenyu.top/gtkhfezgkd.html

Ruby: x.length;  x.size
来源：http://hz.yonumen.top/gtadnjseek.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.hysaishi.cn/gtsxxjpjhu.html

[P05] 判断两个对象内容是否相等
来源：http://hz.yongpay.top/gtzcvhmini.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.xuetiantiany.cn/gtrviunzuw.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.ppjwa.cn/gtxzrygwey.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.xinyue.icu/gtrwvjcgfv.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.xuetiantiany.cn/gtrbodzpvw.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.shzxlz.cn/gtxxkwhayk.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.c1oappe.top/gtvyfddewd.html

Ruby: a == b
来源：http://hz.wangdashe.top/gtgevqdtzg.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.shzxlz.cn/gtjjcjkhvy.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.c1oappe.top/gtmthjanwl.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.nwbrower.top/gtuazmtpbl.html

PHP:  if (empty($x)) {}
来源：http://hz.wangdashe.top/gttrvlppro.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.havefunace.top/gtlyflkyxt.html

TS:   if (x == null) {}
来源：http://hz.zycfv.cn/gtxvemhyge.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.ydzc1.top/gtsqqvmtyk.html

Go:   if x == nil {}
来源：http://hz.nanxuanxn.top/gtfgghxsmm.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.havefunace.top/gtqojjdkef.html

C#:   if (x is null) {}
来源：http://hz.shanyushiyangtech.top/gtmyhtfphs.html

[P07] 防抖与节流
来源：http://hz.nanxinkj.top/gtuklemoog.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.gaohongyu789.top/gtpdwgwogi.html

PHP:  // 手写时间戳比较
来源：http://hz.wangshuangyany.cn/gtgqlwxnrp.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.shanyushiyangkeji.top/gttcyincbs.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.jinyuanbaomall.cn/gtbykahamb.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.hnxiangtu.top/gtjexskmna.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.ivvv.top/gtadlagibf.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.quarkkingdee.top/gtppbphquj.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.tanke756.top/gtatkzdsmf.html

[P08] 处理浮点精度问题
来源：http://hz.zhiwuduotai.top/gtmiabtkmg.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.fengsongda.top/gtrmzjiuse.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.jqgfzy.top/gtdlywviyw.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.ydjk.org.cn/gtfxitrawq.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.316326.xyz/gtnjhhyutr.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.yvedp.cn/gtlkabtowm.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.zycfv.cn/gtyqnlvraf.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.yueranfly.top/gtzzzwvbad.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.wangshuangyany.cn/gtkeiurdmy.html

================================================================================
来源：http://hz.nwbrower.top/gtrpytfvxk.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.guannengcc.top/gtkgwcnxff.html

================================================================================
来源：http://hz.sysykeji.top/gtkhvvurew.html

[Q01] 创建表
来源：http://hz.jinqigufen.top/gtntzaypws.html

CREATE TABLE users (
来源：http://hz.yonumen.top/gtelhvglqc.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.svipenyu.cn/gtkcpjnbmw.html

name VARCHAR(50) NOT NULL,
来源：http://hz.wangdashe.top/gtzddisgff.html

email VARCHAR(100) UNIQUE,
来源：http://hz.316326.xyz/gtrfujeiqs.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.nanxuanxn.top/gtxzkgoghx.html

);
来源：http://hz.svipenyu.cn/gtziwwldhl.html

[Q02] 创建带外键的表
来源：http://hz.xingfuxueyuan.xyz/gtohyllolc.html

CREATE TABLE orders (
来源：http://hz.dianchejie.cn/gtltwjspgp.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.fzhhl.top/gtcwevwira.html

user_id INT NOT NULL,
来源：http://hz.316326.xyz/gtqcbbflhd.html

amount DECIMAL(10, 2),
来源：http://hz.birdmap.top/gtfhberivx.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.pengpengdd.cyou/gtygravsvv.html

);
来源：http://hz.feifeiyinyue.top/gtdfdqnvwf.html

[Q03] 增加列
来源：http://hz.cdnleiting.top/gtjszituxl.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.ywan-chungtsiang.top/gtdcfjrnxh.html

[Q04] 修改列类型
来源：http://hz.ywan-chungtsiang.top/gtyndgsayx.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.havefunace.top/gthzairdow.html

[Q05] 重命名列
来源：http://hz.sysykeji.top/gtbiecmmcn.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.sufxvd.cn/gtcamczchk.html

[Q06] 删除列
来源：http://hz.jinqigfzy.top/gthcovhvjt.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.sxryk.cn/gtswemsxtd.html

[Q07] 删除表
来源：http://hz.xylfe.cn/gtxotmzyni.html

DROP TABLE IF EXISTS orders;
来源：http://hz.jinghuilouyu.cn/gtjzlwnyrt.html

[Q08] 创建普通索引
来源：http://hz.cashguo.top/gtxuwdcebv.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.9152youxi.cn/gtriabadhh.html

[Q09] 创建唯一索引
来源：http://hz.yuanzhike.top/gtsofgeiqk.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.dianchejie.cn/gtcbkqittd.html

[Q10] 插入单行
来源：http://hz.kuanghao11.cn/gthnynvznn.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.andypj.xyz/gthsgmhicz.html

[Q11] 一次插入多行
来源：http://hz.jinqigufen.top/gtufbnxoba.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.0kj1m.cn/gtxihzqnpc.html

[Q12] 插入后取自增 ID
来源：http://hz.redwolf501.top/gttmjozywv.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.wangdashe.top/gtkwgmahfo.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.gogol.net.cn/gtbbltpzsc.html

[Q13] 忽略重复插入
来源：http://hz.feifeiyinyue.top/gtldxzysyh.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.pengpengdd.cyou/gtovoigtgb.html

[Q14] 存在则更新（upsert）
来源：http://hz.ydjk.org.cn/gtsgsdnadj.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.jinyuanbaomall.cn/gtgtbnaogz.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.bjfxy.top/gtmedjnhmy.html

[Q15] 查询全部
来源：http://hz.smart0.xyz/gtqwbsqesi.html

SELECT * FROM users;
来源：http://hz.gogol.net.cn/gtufvnrovs.html

[Q16] 查询指定列
来源：http://hz.hfpthk.cn/gtenzeullq.html

SELECT id, name FROM users;
来源：http://hz.zycfv.cn/gtqwirgpon.html

[Q17] 条件查询
来源：http://hz.fengsongda.top/gtlhacwfcc.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.cucudq.cn/gtccdggrme.html

[Q18] 模糊匹配
来源：http://hz.tian-w.cn/gtgoxigzxj.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.gzhubu.top/gtdjjhlwqg.html

[Q19] 范围查询
来源：http://hz.yanxiufei.cn/gtulwdgtoz.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.wangdashe.top/gtpfxycugo.html

[Q20] IN 列表
来源：http://hz.xylfe.cn/gtbamgcpfo.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.chenzaomai.com/gtrxsrwahe.html

[Q21] 空值判断
来源：http://hz.jyoumei.cn/gtbgdfbust.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.xuetiantiany.cn/gtcvyuusjz.html

[Q22] 排序
来源：http://hz.birdmap.top/gtsaffvreo.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.daria6918.cn/gtzrauanqw.html

[Q23] 分页
来源：http://hz.jinghuilouyu.cn/gtnsnbqpwb.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.hysaishi.cn/gtkicexatk.html

[Q24] 去重
来源：http://hz.gaohongyu789.top/gtkxcsrwya.html

SELECT DISTINCT city FROM users;
来源：http://hz.zycfv.cn/gtimmjnzwt.html

[Q25] 只取前 N 条
来源：http://hz.ybcxt.top/gthvqwvrrg.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.0kj1m.cn/gtudgzpzug.html

[Q26] 计数
来源：http://hz.zhixingplan.top/gthcfswaiv.html

SELECT COUNT(*) FROM users;
来源：http://hz.sxryk.cn/gtvvaaabjr.html

[Q27] 条件计数
来源：http://hz.iojbl.cn/gtuabbksyn.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.xylfe.cn/gtgaxejlvp.html

[Q28] 求和与平均
来源：http://hz.xuetiantiany.cn/gtufmbhmlr.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.yuxming.cn/gtdxlujyof.html

[Q29] 最大最小值
来源：http://hz.ywan-chungtsiang.top/gthmjxplaa.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.guowangkeji.top/gtaytqoljn.html

[Q30] 分组统计
来源：http://hz.yonumen.top/gtsooajjco.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.zhiwuduotai.top/gtbwvdfxpl.html

[Q31] 分组后过滤
来源：http://hz.yueranfly.top/gtwfjysdab.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.yonumen.top/gtvwbyghru.html

[Q32] 分组拼接字符串
来源：http://hz.jqgfzy.top/gtpxgeptni.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.9152youxi.cn/gtzlqlkzlc.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.meibo888.top/gtnsjgadpg.html

[Q33] 多列分组
来源：http://hz.jinghuilouyu.cn/gttqykqqto.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.yj20258888.top/gtwpemhbdp.html

[Q34] 每组取第一条
来源：http://hz.xinyue.icu/gtyfjvnpgt.html

SELECT * FROM (
来源：http://hz.iojbl.cn/gtcivzvjox.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.chenlongwang.top/gtklbuulmg.html

) t WHERE rn = 1;
来源：http://hz.pengpengdd.cyou/gtzwcfaald.html

[Q35] 内连接
来源：http://hz.shuidangran.top/gtcbbxyqcx.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.tanke756.top/gtcevfeolp.html

[Q36] 左连接
来源：http://hz.tianlin.xyz/gtpyifpidn.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.ehwqpu.com/gtibkwlomu.html

[Q37] 右连接
来源：http://hz.hnxiangtu.top/gttpxfqqld.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.wangshuangyany.cn/gtzonkicvo.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.zhoulong.xyz/gtsebdmfph.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.yangfankeji.com/gtteczexqa.html

[Q39] 自连接（查上下级）
来源：http://hz.ydzc1.top/gtuylytgve.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.zhongyouzk.top/gtnxyzvlya.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.shanyushiyangtech.top/gtnacfcbeu.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.aizwys.cn/gtbqqiyvic.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.sufxvd.cn/gtiaspwuvp.html

[Q41] 多表连接
来源：http://hz.xziqi.cn/gtamxsghie.html


<!-- 参考信息 -->