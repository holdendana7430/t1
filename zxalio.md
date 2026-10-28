代发 wailian999

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.smart0.xyz/gtgavkjxzu.html

[N06] 判断回文字符串
来源：http://hz.ydjk.org.cn/gtixwocriy.html

Py:   s == s[::-1]
来源：http://hz.chenzaomai.com/gteoywwcsg.html

PHP:  $s === strrev($s);
来源：http://hz.kuanghao11.cn/gtkgtkpxvl.html

JS:   s === [...s].reverse().join("")
来源：http://hz.shangyingyoupin.top/gtbdtdaxcu.html

TS:   s === [...s].reverse().join("")
来源：http://hz.meibo888.top/gtjylcwwwd.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.guowangkeji.top/gtkeswfvwd.html

Go:   // 双指针从两端比较
来源：http://hz.jinyuanbaomall.cn/gtzlrgaubv.html

Ruby: s == s.reverse
来源：http://hz.shuidangran.top/gtmiixotef.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.snrcjt.cn/gtoaerzxpm.html

[N07] 两数之和（返回下标）
来源：http://hz.fengsongda.top/gttfgqgysz.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.gogol.net.cn/gtjqphuteb.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.hywenlv.cn/gtvjxssbup.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.zhongyouzk.top/gtyuwxdvml.html

TS:   // 手写 Map<string, number>
来源：http://hz.ppjwa.cn/gtitxmxexq.html

Java: // 手写 HashMap
来源：http://hz.zhiwuduotai.top/gtfqywucws.html

Go:   // 手写 map[int]int
来源：http://hz.tian-w.cn/gtssgnhdvt.html

Ruby: // 手写 Hash
来源：http://hz.zhongyouzk.top/gtslrmccei.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.wangshuangyany.cn/gtftmlfqtt.html

[N08] 生成全排列
来源：http://hz.gaohongyu789.top/gthfqaevbn.html

Py:   itertools.permutations(arr)
来源：http://hz.fengsongda.top/gtgylflesw.html

PHP:  // 手写递归交换
来源：http://hz.shzxlz.cn/gtijhvwqgu.html

JS:   // 手写回溯递归
来源：http://hz.jinghuilouyu.cn/gtppbvtfck.html

TS:   // 手写回溯递归
来源：http://hz.zhengqikj.top/gtsypbnkzk.html

Java: // 手写回溯递归
来源：http://hz.mhx1999.top/gtmyvssaua.html

Go:   // 手写回溯递归
来源：http://hz.yangfankeji.com/gtpeahfozz.html

Ruby: arr.permutation.to_a
来源：http://hz.cheryme.top/gtoidvuxfd.html

C#:   // 手写回溯递归
来源：http://hz.haohaochexian.top/gtbbfzskur.html

[N09] 栈与队列
来源：http://hz.zhoulong.xyz/gtmpamreom.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.yj20258.top/gtllanaqct.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.yanxiufei.cn/gtzotdcflb.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.jianghu66.top/gttzwdmrca.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.ywan-chungtsiang.top/gtmqkhmvbr.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.jyoumei.cn/gttdbazikj.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.xuanzx.com/gtzviwkmab.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.gogol.net.cn/gtlfwqtaqe.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.ydzc1.top/gtdgqccwpw.html

[N10] 链表节点定义
来源：http://hz.yj20258888.top/gtzgmopdim.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.yj20258888.top/gtkrqsejgf.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.yuxming.cn/gtemrmsfdp.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.jqgufenzy.top/gtxwxyncuw.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.shuidangran.top/gtlohaytbx.html

Java: class Node { int v; Node next; }
来源：http://hz.pengpengdd.cyou/gtdjbeemng.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.zdqjudy.top/gtrddzchut.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.nanxuanxn.top/gtoxutfutk.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.svipenyu.cn/gtcpvcpssr.html

[N11] 二叉树中序遍历
来源：http://hz.bjfxy.top/gtvbcfxzjb.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.shuidangran.top/gtihvjkbhu.html

PHP:  // 手写递归函数
来源：http://hz.ywan-chungtsiang.top/gtmakxtlcw.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.xziqi.cn/gtwavcovab.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.zhengqikj.top/gtefvqmyfh.html

Java: // 手写递归
来源：http://hz.vqdsnc.cn/gtbdnoyelh.html

Go:   // 手写递归
来源：http://hz.tanke756.top/gtkjzaehgt.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.dianchejie.cn/gtjbpdauxh.html

C#:   // 手写递归
来源：http://hz.yuanzhike.top/gtjyayfhhw.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.0kj1m.cn/gtuffzlozm.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.cdnleiting.top/gtlmoihdoy.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.xylfe.cn/gtspjarpds.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.zhongyouzk.top/gtadukghla.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.pycfn.com/gtqjxxoexd.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.gaohongyu789.top/gtovxqedfw.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.ydzc1.top/gtpihqjfph.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.ppjwa.cn/gtjxknzpvq.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.guannengcc.top/gttiiknbct.html

================================================================================
来源：http://hz.316326.xyz/gthloznqje.html

O. 并发与异步
来源：http://hz.gotoacloud.top/gtvboetnuy.html

================================================================================
来源：http://hz.birdmap.top/gthjeyucga.html

[O01] 启动一个线程
来源：http://hz.gaohongyu789.top/gtdxjscytz.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.hfpthk.cn/gtartsmaqz.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.redwolf501.top/gtzzuesuhz.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.jinghuilouyu.cn/gtakhuparh.html

TS:   // 同 JS
来源：http://hz.zhixingplan.top/gtjnkqsgxx.html

Java: new Thread(() -> f()).start()
来源：http://hz.pycfn.com/gtpkmhyieu.html

Go:   go f()
来源：http://hz.yj20258.top/gtdkxjktus.html

Ruby: Thread.new { f }
来源：http://hz.sxryk.cn/gtgcrwrbqi.html

C#:   Task.Run(() => F());
来源：http://hz.meibo888.top/gtsvpjyfzm.html

[O02] 使用线程池
来源：http://hz.hongshengwenyu.top/gtcuitybpe.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.cucudq.cn/gtouoewcds.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.daria6918.cn/gtzluwygnh.html

JS:   // worker_threads 线程池
来源：http://hz.316326.xyz/gtylylleqr.html

TS:   // worker_threads 线程池
来源：http://hz.dashuyun.cn/gtjdayemdi.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.yanxiufei.cn/gtdyngnfpf.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.zhoulong.xyz/gtxplwedcq.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.xuetiantiany.cn/gtmicvsgcm.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.zhaomingkeji.xyz/gtfuutzenf.html

[O03] 加锁保护共享数据
来源：http://hz.hammf.cn/gtvayjtedc.html

Py:   with lock: shared += 1
来源：http://hz.zhaomingkeji.xyz/gtumtyvjrp.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.ydzc1.top/gttwgyqjij.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.chenzaomai.com/gtmbawzzzx.html

TS:   // 同 JS
来源：http://hz.ybcxt.top/gtszanyalq.html

Java: synchronized (this) { shared++; }
来源：http://hz.316326.xyz/gtbusdzghe.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.tanke756.top/gtxcnvekde.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.zhongyouzk.top/gtjibtsmmw.html

C#:   lock (gate) { shared++; }
来源：http://hz.pycfn.com/gtqaldwusq.html

[O04] 定义异步函数并等待
来源：http://hz.nanxinkj.top/gtixpovcos.html

Py:   async def f():⏎    await g()
来源：http://hz.sweek.top/gtgtyhfcfx.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.jqgufenzy.top/gtkslfulpz.html

JS:   async function f() { await g(); }
来源：http://hz.yj202588.top/gtolskjywp.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.tianlin.xyz/gtmxqaycye.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.316326.xyz/gtaohxocgx.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.feifeiyinyue.top/gtbnpnkqry.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.xuanzx.com/gtdriliylo.html

C#:   async Task F() { await G(); }
来源：http://hz.xuanzx.com/gtjxzkkshb.html

[O05] 并发执行并等待全部完成
来源：http://hz.zhongyouzk.top/gtypbqhwcn.html

Py:   asyncio.gather(*tasks)
来源：http://hz.shzxlz.cn/gticicaxws.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.ydzc1.top/gtluvrhhir.html

JS:   await Promise.all(tasks)
来源：http://hz.shangyingyoupin.top/gtsehryloh.html

TS:   await Promise.all(tasks)
来源：http://hz.sxryk.cn/gtmnryjgcj.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.aibaodan.cn/gtchxsgzlt.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.guannengcc.top/gtoryvoloo.html

Ruby: threads.map(&:join)
来源：http://hz.zhijiandao.cn/gtyidyzgmo.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.tianlin.xyz/gtxnhmqftw.html

[O06] 使用进程池
来源：http://hz.wangshuangyany.cn/gtpcjpzdnq.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.yuxming.cn/gtycybcmlc.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.aizwys.cn/gtdcfqgetx.html

JS:   // child_process / cluster 模块
来源：http://hz.sxryk.cn/gtufonkjpb.html

TS:   // child_process / cluster 模块
来源：http://hz.yuanzhike.top/gtpupgkosq.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.fengsongda.top/gtysnxbmms.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.redwolf501.top/gtumzqfuiy.html

Ruby: // fork 块
来源：http://hz.xuetiantiany.cn/gtlautbddi.html

C#:   Parallel.For
来源：http://hz.jqgfzy.top/gtldbvyype.html

================================================================================
来源：http://hz.guowangkeji.top/gtbkhyekjk.html

P. 常用工具函数
来源：http://hz.yongpay.top/gtrylbxrvl.html

================================================================================
来源：http://hz.yueranfly.top/gtauahyccg.html

[P01] 生成 UUID
来源：http://hz.jianghu66.top/gtcdnjlevy.html

Py:   str(uuid.uuid4())
来源：http://hz.tanke756.top/gtqqfnytky.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.guannengcc.top/gttjnmovdm.html

JS:   crypto.randomUUID()
来源：http://hz.sysykeji.top/gtikctgiwl.html

TS:   crypto.randomUUID()
来源：http://hz.tian-w.cn/gtmznpynrv.html

Java: UUID.randomUUID().toString()
来源：http://hz.smart0.xyz/gtvrpafvah.html

Go:   // 用 github.com/google/uuid
来源：http://hz.zhaomingkeji.xyz/gtylzidisc.html

Ruby: SecureRandom.uuid
来源：http://hz.ppjwa.cn/gtxsxlehxu.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.cdnleiting.top/gtnqsbjkxc.html

[P02] MD5 / SHA256 摘要
来源：http://hz.xingfuxueyuan.xyz/gtvkhaxsnw.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.ydzc1.top/gtocuspgsa.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.yonumen.top/gteqfcuxcw.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.tanke756.top/gtopslnwxr.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.shanyushiyangkeji.top/gtdaejcdhr.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.vqdsnc.cn/gthecaxqqm.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.ydzc1.top/gtngnesinc.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.nanxuanxn.top/gtcwoiylwa.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.316326.xyz/gthfqyugbi.html

[P03] 生成短随机字符串
来源：http://hz.jyoumei.cn/gtopcyxpbz.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.cqqwz.cn/gtjdgwirpr.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.chenjidiqi.icu/gtiyoiulsp.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.jyoumei.cn/gthshpkimb.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.smart0.xyz/gtusyobplr.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.52xcode.cn/gtpalvjixa.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.sxryk.cn/gtoicjfwdn.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.quarkkingdee.top/gtrfgjuyho.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.zhoulong.xyz/gteyurshcb.html

[P04] 求长度
来源：http://hz.hfpthk.cn/gtsjelnlvm.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.shanyushiyangkeji.top/gthxqfkyuv.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.chenjidiqi.icu/gtkjfffvlo.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.guannengcc.top/gteerkqial.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.svipenyu.cn/gtjvsmcuur.html

Java: list.size();  map.size();  s.length()
来源：http://hz.jqgufenzy.top/gtpkwvjhrw.html

Go:   len(arr);  len(m)
来源：http://hz.shangyingyoupin.top/gtwhmrgpcd.html

Ruby: x.length;  x.size
来源：http://hz.meibo888.top/gtyuivhtue.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.yj202588.top/gtnnkxbrku.html

[P05] 判断两个对象内容是否相等
来源：http://hz.dianchejie.cn/gttqsmjbtn.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.vqdsnc.cn/gttbqzomqg.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.hfpthk.cn/gtwimsmgkz.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.quarkkingdee.top/gtqutejbwe.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.yj20258888.top/gtruzjccfq.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.hywenlv.cn/gtsyaozidl.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.cucudq.cn/gtufnsclyo.html

Ruby: a == b
来源：http://hz.sysykeji.top/gtyqbdqimf.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.yongpay.top/gtqnpyavrf.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.yangfankeji.com/gtawmjtydp.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.nanxinkj.top/gtkozpcuzt.html

PHP:  if (empty($x)) {}
来源：http://hz.daxiang520.top/gtzimhwifd.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.shzxlz.cn/gtisnnakyk.html

TS:   if (x == null) {}
来源：http://hz.birdmap.top/gtqipzqnht.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.ydjk.org.cn/gtloqikdim.html

Go:   if x == nil {}
来源：http://hz.gzhubu.top/gteejgxesc.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.dashuyun.cn/gtaecmubxf.html

C#:   if (x is null) {}
来源：http://hz.jianghu66.top/gtdafykjzc.html

[P07] 防抖与节流
来源：http://hz.jyoumei.cn/gtooyvsoyv.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.gotoacloud.top/gtmotmhgoj.html

PHP:  // 手写时间戳比较
来源：http://hz.chenzaomai.com/gtlktmbkvd.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.redwolf501.top/gtnddnxhut.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.nwbrower.top/gtyqcocmif.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.zhiwuduotai.top/gtfcnzupbd.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.jyoumei.cn/gtirkjzoia.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.feifeiyinyue.top/gtrkrgtevu.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.ybcxt.top/gtblsaapkh.html

[P08] 处理浮点精度问题
来源：http://hz.zdqjudy.top/gtptfgfhnq.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.daxiang520.top/gtmhwffqdg.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.xylfe.cn/gtozdfbnit.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.zycfv.cn/gtqsqlcqlc.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.sxryk.cn/gtiwwndjnz.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.gzhubu.top/gtqjnjxjvm.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.xuanzx.com/gtffprrguz.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.tanke756.top/gtpoyyrdzk.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.feifeiyinyue.top/gtvhjnuptt.html

================================================================================
来源：http://hz.zhiwuduotai.top/gtszgratuo.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.svipenyu.cn/gtulzecukk.html

================================================================================
来源：http://hz.aibaodan.cn/gtroeyzugc.html

[Q01] 创建表
来源：http://hz.xingfuxueyuan.xyz/gtfzbieltc.html

CREATE TABLE users (
来源：http://hz.zhoulong.xyz/gtzplpmtdr.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.tanke756.top/gtnnzjzhxc.html

name VARCHAR(50) NOT NULL,
来源：http://hz.chenlongwang.top/gtspaftnvs.html

email VARCHAR(100) UNIQUE,
来源：http://hz.sxryk.cn/gtrgxxuqqp.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.redwolf501.top/gtswshgsla.html

);
来源：http://hz.daria6918.cn/gtyavbcuss.html

[Q02] 创建带外键的表
来源：http://hz.zhongyouzk.top/gtukvstncm.html

CREATE TABLE orders (
来源：http://hz.feifeiyinyue.top/gtlbnvvoap.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.zdqjudy.top/gtuibiyyzd.html

user_id INT NOT NULL,
来源：http://hz.vqdsnc.cn/gtswwlbpyg.html

amount DECIMAL(10, 2),
来源：http://hz.sweek.top/gtbdjzrmdr.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.bjfxy.top/gtwntfllpw.html

);
来源：http://hz.9152youxi.cn/gtbrrwwckx.html

[Q03] 增加列
来源：http://hz.jiagoushi.top/gtxrxpupqb.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.hnqzz.top/gtxldtzdnc.html

[Q04] 修改列类型
来源：http://hz.haohaochexian.top/gtdxcxsujy.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.daria6918.cn/gtcxjjvove.html

[Q05] 重命名列
来源：http://hz.ppjwa.cn/gtekbzcyod.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.cucudq.cn/gtimrbonde.html

[Q06] 删除列
来源：http://hz.chenjidiqi.icu/gtzrgktyns.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.shangyingyoupin.top/gtfoynauai.html

[Q07] 删除表
来源：http://hz.shanyushiyangtech.top/gtmtdayhvn.html

DROP TABLE IF EXISTS orders;
来源：http://hz.xinyue.icu/gtovhvvgij.html

[Q08] 创建普通索引
来源：http://hz.wangshuangyany.cn/gtfurtaepb.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.cheryme.top/gtixpvsayq.html

[Q09] 创建唯一索引
来源：http://hz.xziqi.cn/gtsblwortx.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.jinyuanbaomall.cn/gtgnwvniwa.html

[Q10] 插入单行
来源：http://hz.ydjk.org.cn/gtdesedtbn.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.jianghu66.top/gtnxlhnqez.html

[Q11] 一次插入多行
来源：http://hz.meibo888.top/gtqfvdcvsm.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.vqdsnc.cn/gteuphrllw.html

[Q12] 插入后取自增 ID
来源：http://hz.sysykeji.top/gtskarwoxl.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.hnxiangtu.top/gthhqqbrul.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.yangfankeji.com/gtkydljqjk.html

[Q13] 忽略重复插入
来源：http://hz.hysaishi.cn/gtjuxyrybu.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.sufxvd.cn/gtlfwdnxns.html

[Q14] 存在则更新（upsert）
来源：http://hz.jiagoushi.top/gtkrgsrqjf.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.zhongyouzk.top/gtrpvabohx.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.zhijiandao.cn/gtepjgravc.html

[Q15] 查询全部
来源：http://hz.chenjidiqi.icu/gteolzeinu.html

SELECT * FROM users;
来源：http://hz.gzhubu.top/gtcdwlgluq.html

[Q16] 查询指定列
来源：http://hz.yongpay.top/gttugsszdw.html

SELECT id, name FROM users;
来源：http://hz.redwolf501.top/gthsdamfiy.html

[Q17] 条件查询
来源：http://hz.mhx1999.top/gtaqovtini.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.yj20258888.top/gteiisgqff.html

[Q18] 模糊匹配
来源：http://hz.52xcode.cn/gttfmbnfzp.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.aibaodan.cn/gtjktvmazp.html

[Q19] 范围查询
来源：http://hz.c1oappe.top/gtxaviybtm.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.wangshuangyany.cn/gtsbwbutaa.html

[Q20] IN 列表
来源：http://hz.hysaishi.cn/gtsbuglclq.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.yj20258888.top/gtukwaiczt.html

[Q21] 空值判断
来源：http://hz.yj20258.top/gtpifkzuix.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.gzhubu.top/gtjnnictpo.html

[Q22] 排序
来源：http://hz.xylfe.cn/gtmixqtyes.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.quarkkingdee.top/gtpjrdeqqe.html

[Q23] 分页
来源：http://hz.0kj1m.cn/gtxlzncchc.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.ppjwa.cn/gteplcllqi.html

[Q24] 去重
来源：http://hz.aizwys.cn/gtghtladft.html

SELECT DISTINCT city FROM users;
来源：http://hz.ydzc1.top/gtyfmldzgz.html

[Q25] 只取前 N 条
来源：http://hz.aizwys.cn/gtcjbelwug.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.wangdashe.top/gtrwnvtypz.html

[Q26] 计数
来源：http://hz.jqgufenzy.top/gtbwockmle.html

SELECT COUNT(*) FROM users;
来源：http://hz.shanyushiyangkeji.top/gttezlppux.html

[Q27] 条件计数
来源：http://hz.316326.xyz/gtsdpqulbi.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.sysykeji.top/gtigpahfxp.html

[Q28] 求和与平均
来源：http://hz.yongpay.top/gtywgovcyy.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.ydjk.org.cn/gtpzqayzqt.html

[Q29] 最大最小值
来源：http://hz.daria6918.cn/gtgtehmhin.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.feifeiyinyue.top/gtqtnzumjw.html

[Q30] 分组统计
来源：http://hz.feifeiyinyue.top/gtimpbeatx.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.yj20258888.top/gtjwiagfrh.html

[Q31] 分组后过滤
来源：http://hz.jiagoushi.top/gtmozdhtom.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.kuanghao11.cn/gtnqkwccpp.html

[Q32] 分组拼接字符串
来源：http://hz.yj20258888.top/gtcoyypubz.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.xingfuxueyuan.xyz/gtssnlnxfj.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.zhixingplan.top/gtvuvzkjgs.html

[Q33] 多列分组
来源：http://hz.wangdashe.top/gttybnftmx.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.jinqigfzy.top/gtbnyhvoii.html

[Q34] 每组取第一条
来源：http://hz.shangyingyoupin.top/gtrpyswlvk.html

SELECT * FROM (
来源：http://hz.dianchejie.cn/gtbgieyqzt.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.sxryk.cn/gttzbeymbn.html

) t WHERE rn = 1;
来源：http://hz.zhoulong.xyz/gttaiprvvo.html

[Q35] 内连接
来源：http://hz.hongshengwenyu.top/gtcvmsapen.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.tian-w.cn/gtiqebxgdh.html

[Q36] 左连接
来源：http://hz.fzhhl.top/gttamvgbyt.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.jianghu66.top/gtalvdvbra.html

[Q37] 右连接
来源：http://hz.tanke756.top/gtcpjgdbsn.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.aibaodan.cn/gtwcvwfxwn.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.xuetiantiany.cn/gtppqxnnob.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.xuanzx.com/gtfamqulya.html

[Q39] 自连接（查上下级）
来源：http://hz.havefunace.top/gtbozkhfuz.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.xylfe.cn/gtguaxxgkd.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.redwolf501.top/gttwlsvxlo.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.dashuyun.cn/gtzrcparxw.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.feifeiyinyue.top/gtnhrqtdbo.html

[Q41] 多表连接
来源：http://hz.havefunace.top/gtrvqyydsj.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.svipenyu.cn/gtaiexegop.html

JOIN users u ON u.id = o.user_id
来源：http://hz.vqdsnc.cn/gtgcouyfsl.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.gotoacloud.top/gtbljdmtst.html

[Q42] 连接条件附加过滤
来源：http://hz.fengsongda.top/gtfytrpkaf.html


<!-- 参考信息 -->