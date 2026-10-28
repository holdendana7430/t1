代发 wailian999

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.yangfankeji.com/gtbjsudmhp.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.cheryme.top/gtktdvgvsy.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.ydjk.org.cn/gtgdycdbwp.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.aibaodan.cn/gtmgwaehwp.html

[N05] 最大公约数
来源：http://hz.havefunace.top/gtdcuytoni.html

Py:   math.gcd(a, b)
来源：http://hz.nanxinkj.top/gtqtlyelrq.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.sweek.top/gtsfnvaouv.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.zhixingplan.top/gtoscmilmp.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.ydjk.org.cn/gtxlkacrvn.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.zdqjudy.top/gtqecfjtpb.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.pycfn.com/gtvvcsctow.html

Ruby: a.gcd(b)
来源：http://hz.smart0.xyz/gtyutfefxg.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.redwolf501.top/gtkyylhpkd.html

[N06] 判断回文字符串
来源：http://hz.52xcode.cn/gtsyijjmet.html

Py:   s == s[::-1]
来源：http://hz.ywan-chungtsiang.top/gtmsoutblo.html

PHP:  $s === strrev($s);
来源：http://hz.havefunace.top/gtljguqiyp.html

JS:   s === [...s].reverse().join("")
来源：http://hz.nanxuanxn.top/gtcsxseqms.html

TS:   s === [...s].reverse().join("")
来源：http://hz.xinyue.icu/gtvokdvwdt.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.hongshengwenyu.top/gtewalreov.html

Go:   // 双指针从两端比较
来源：http://hz.snrcjt.cn/gtwvhkkdnb.html

Ruby: s == s.reverse
来源：http://hz.xinyue.icu/gtxqlvbeas.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.xinyue.icu/gtdhhavobu.html

[N07] 两数之和（返回下标）
来源：http://hz.gzhubu.top/gtsdcdskgs.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.yueranfly.top/gtpixewcjr.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.316326.xyz/gtmnqwmewj.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.fzhhl.top/gtlqipnsfe.html

TS:   // 手写 Map<string, number>
来源：http://hz.sweek.top/gtomonbcrf.html

Java: // 手写 HashMap
来源：http://hz.xziqi.cn/gteymlfqkq.html

Go:   // 手写 map[int]int
来源：http://hz.pycfn.com/gtwjbppqrs.html

Ruby: // 手写 Hash
来源：http://hz.ydjk.org.cn/gtvkguimts.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.shanyushiyangkeji.top/gtzlmfrpdm.html

[N08] 生成全排列
来源：http://hz.yonumen.top/gtzbotqksx.html

Py:   itertools.permutations(arr)
来源：http://hz.yanxiufei.cn/gtzgraoqwh.html

PHP:  // 手写递归交换
来源：http://hz.aibaodan.cn/gtevybartg.html

JS:   // 手写回溯递归
来源：http://hz.yonumen.top/gtkbvprejd.html

TS:   // 手写回溯递归
来源：http://hz.316326.xyz/gttyzyutzo.html

Java: // 手写回溯递归
来源：http://hz.yj202588.top/gtcrwjedsm.html

Go:   // 手写回溯递归
来源：http://hz.yj20258888.top/gtomjexykq.html

Ruby: arr.permutation.to_a
来源：http://hz.ybcxt.top/gtxvxxydmz.html

C#:   // 手写回溯递归
来源：http://hz.hnxiangtu.top/gtfaqomaid.html

[N09] 栈与队列
来源：http://hz.9152youxi.cn/gtrouzfqyr.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.0kj1m.cn/gtzogtaygj.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.sxryk.cn/gtublszili.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.gaohongyu789.top/gtyopkjcit.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.chenjidiqi.icu/gtekjyodqp.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.gaohongyu789.top/gtczffanwl.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.jinqigfzy.top/gthbvpylgr.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.nwbrower.top/gtbevknstc.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.meibo888.top/gteyvispft.html

[N10] 链表节点定义
来源：http://hz.iojbl.cn/gthgrvqwqw.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.c1oappe.top/gtxpgllpih.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.jiagoushi.top/gtgtplmdxh.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.mhx1999.top/gtubfeaduy.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.tian-w.cn/gtcsurzmid.html

Java: class Node { int v; Node next; }
来源：http://hz.jqgufenzy.top/gttjrwitke.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.haohaochexian.top/gtwpzahzpv.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.vqdsnc.cn/gtpjyljtgl.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.ivvv.top/gtfncsyhzk.html

[N11] 二叉树中序遍历
来源：http://hz.yanxiufei.cn/gtdelxvhhu.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.guowangkeji.top/gtsmamqgly.html

PHP:  // 手写递归函数
来源：http://hz.cqqwz.cn/gtahcvkgbb.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.ywan-chungtsiang.top/gtbbobfjaq.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.havefunace.top/gtesoziohl.html

Java: // 手写递归
来源：http://hz.ydjk.org.cn/gtdpncttnu.html

Go:   // 手写递归
来源：http://hz.zycfv.cn/gtchimkcfo.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.snrcjt.cn/gteljfsfeo.html

C#:   // 手写递归
来源：http://hz.ydzc1.top/gtgpdqkpqc.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.wangdashe.top/gtxsiuegnx.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.snrcjt.cn/gtruqfekcp.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.ydzc1.top/gtorbnmqjq.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.ydzc1.top/gtpqsruhvy.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.cheryme.top/gtpvonlajp.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.daria6918.cn/gtjgcbbgnb.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.xylfe.cn/gtvvrwzrip.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.0kj1m.cn/gtmfuxchar.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.sysykeji.top/gtavmaayth.html

================================================================================
来源：http://hz.ybcxt.top/gttjgwqvmj.html

O. 并发与异步
来源：http://hz.zhongyouzk.top/gtkmfatyyp.html

================================================================================
来源：http://hz.gotoacloud.top/gtciotnitl.html

[O01] 启动一个线程
来源：http://hz.jlsjyb.cn/gthuevyvnl.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.aizwys.cn/gtmbkrhvgc.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.hnxiangtu.top/gtopqexwuv.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.c1oappe.top/gtxhsncmmt.html

TS:   // 同 JS
来源：http://hz.sysykeji.top/gtwmlcafcq.html

Java: new Thread(() -> f()).start()
来源：http://hz.yuanzhike.top/gtgzzbgqxg.html

Go:   go f()
来源：http://hz.redwolf501.top/gtdzaywowj.html

Ruby: Thread.new { f }
来源：http://hz.hfpthk.cn/gtcaladbic.html

C#:   Task.Run(() => F());
来源：http://hz.gzhubu.top/gtihsexjoi.html

[O02] 使用线程池
来源：http://hz.chenjidiqi.icu/gttezqxfyr.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.yonumen.top/gtibxuhjlt.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.ehwqpu.com/gtvurldkzf.html

JS:   // worker_threads 线程池
来源：http://hz.zhaomingkeji.xyz/gthujsouyy.html

TS:   // worker_threads 线程池
来源：http://hz.jinyuanbaomall.cn/gtoqbzgkvr.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.dianchejie.cn/gtidekxobp.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.nanxuanxn.top/gttojimvmo.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.xylfe.cn/gtbraxnumk.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.dashuyun.cn/gtbtjczztv.html

[O03] 加锁保护共享数据
来源：http://hz.yangfankeji.com/gtngjogwyt.html

Py:   with lock: shared += 1
来源：http://hz.xuetiantiany.cn/gtjukaihqc.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.yanxiufei.cn/gtndrljpbk.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.feifeiyinyue.top/gtnegysvde.html

TS:   // 同 JS
来源：http://hz.snrcjt.cn/gtwenwugfp.html

Java: synchronized (this) { shared++; }
来源：http://hz.yj20258888.top/gtihuhdaja.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.jinghuilouyu.cn/gtyfntzedd.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.gogol.net.cn/gtavfcjjiy.html

C#:   lock (gate) { shared++; }
来源：http://hz.jqgufenzy.top/gthriddazu.html

[O04] 定义异步函数并等待
来源：http://hz.jlsjyb.cn/gthxljyjyt.html

Py:   async def f():⏎    await g()
来源：http://hz.9152youxi.cn/gtcnbuperr.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.daria6918.cn/gtcuihrfet.html

JS:   async function f() { await g(); }
来源：http://hz.zhijiandao.cn/gtncdjfxcd.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.yueranfly.top/gtooxwzmpn.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.iojbl.cn/gtteepgnsa.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.andypj.xyz/gtcmpkzcoi.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.gzhubu.top/gtwajkqpib.html

C#:   async Task F() { await G(); }
来源：http://hz.bjfxy.top/gtfjsvixch.html

[O05] 并发执行并等待全部完成
来源：http://hz.xuetiantiany.cn/gtlfjxmehe.html

Py:   asyncio.gather(*tasks)
来源：http://hz.316326.xyz/gtaalvwacm.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.nanxinkj.top/gtqpywfvxz.html

JS:   await Promise.all(tasks)
来源：http://hz.jiagoushi.top/gtftmvhbnz.html

TS:   await Promise.all(tasks)
来源：http://hz.vqdsnc.cn/gtktbxnjfb.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.chenlongwang.top/gtpyseasfn.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.zycfv.cn/gtczzldwsq.html

Ruby: threads.map(&:join)
来源：http://hz.jianghu66.top/gtshormkby.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.fzhhl.top/gtgggziswo.html

[O06] 使用进程池
来源：http://hz.xuanzx.com/gtelsvxpxe.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.mhx1999.top/gtgbsvfpdw.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.yueranfly.top/gtgtcicnki.html

JS:   // child_process / cluster 模块
来源：http://hz.hongshengwenyu.top/gtybibhgtw.html

TS:   // child_process / cluster 模块
来源：http://hz.gotoacloud.top/gtzmprpaqs.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.xziqi.cn/gtlzeitaqr.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.xziqi.cn/gtaviahmfw.html

Ruby: // fork 块
来源：http://hz.gzhubu.top/gtbrvfendn.html

C#:   Parallel.For
来源：http://hz.aizwys.cn/gtfpvwwbrc.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtiziodzfo.html

P. 常用工具函数
来源：http://hz.yueranfly.top/gtehcqlywy.html

================================================================================
来源：http://hz.shanyushiyangkeji.top/gtfmpxsrmw.html

[P01] 生成 UUID
来源：http://hz.jinghuilouyu.cn/gtxocxpwxv.html

Py:   str(uuid.uuid4())
来源：http://hz.gaohongyu789.top/gtmnuejxyy.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.yj20258.top/gtcadvghzw.html

JS:   crypto.randomUUID()
来源：http://hz.xinyue.icu/gtxdscrxzo.html

TS:   crypto.randomUUID()
来源：http://hz.xylfe.cn/gthvspvnvx.html

Java: UUID.randomUUID().toString()
来源：http://hz.xinyue.icu/gtlwvytetc.html

Go:   // 用 github.com/google/uuid
来源：http://hz.shangyingyoupin.top/gtsgfymten.html

Ruby: SecureRandom.uuid
来源：http://hz.zhixingplan.top/gtpikskvan.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.jqgfzy.top/gtnmtlvzoj.html

[P02] MD5 / SHA256 摘要
来源：http://hz.9152youxi.cn/gtsjtqwcoo.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.316326.xyz/gthvhrjlgp.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.xuanzx.com/gtowfgncxd.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.dianchejie.cn/gteevngsdc.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.0kj1m.cn/gtxpvegrwg.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.iojbl.cn/gtwbaqskml.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.iojbl.cn/gtjdwspnkg.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.shanyushiyangkeji.top/gtpqvqszlx.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.iojbl.cn/gtfqhuwqmx.html

[P03] 生成短随机字符串
来源：http://hz.zhijiandao.cn/gtqsovvevb.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.xingfuxueyuan.xyz/gtxavdpcwa.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.jlsjyb.cn/gtgcevdykg.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.tianlin.xyz/gtshleovix.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.xziqi.cn/gtuzomsctg.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.hywenlv.cn/gtqhrwnbon.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.52xcode.cn/gteadvrbgk.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.andypj.xyz/gtmjawioig.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.chenlongwang.top/gtoxzuxils.html

[P04] 求长度
来源：http://hz.xylfe.cn/gtezyqunxg.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.jianghu66.top/gtsiktufzc.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.aizwys.cn/gtctspejnm.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.xinyue.icu/gtoqkpzwly.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.ivvv.top/gtqaeqgvxr.html

Java: list.size();  map.size();  s.length()
来源：http://hz.52xcode.cn/gtqqevojpw.html

Go:   len(arr);  len(m)
来源：http://hz.yj20258.top/gtgmasvrxs.html

Ruby: x.length;  x.size
来源：http://hz.shzxlz.cn/gtcdcbnhfm.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.ppjwa.cn/gtgkvlkwrw.html

[P05] 判断两个对象内容是否相等
来源：http://hz.shzxlz.cn/gtktylsceb.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.vqdsnc.cn/gtrkcacjhx.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.xingfuxueyuan.xyz/gtvaaiiwle.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.sysykeji.top/gtfwnvgbdv.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.sweek.top/gtcdvmraxt.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.shanyushiyangkeji.top/gtpoycalxb.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.gotoacloud.top/gtubyyszxa.html

Ruby: a == b
来源：http://hz.quarkkingdee.top/gtjvyaiqqn.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.hongshengwenyu.top/gtvewidzjl.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.jinyuanbaomall.cn/gtuyyocuvh.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.wangdashe.top/gtwybhaxfx.html

PHP:  if (empty($x)) {}
来源：http://hz.zhiwuduotai.top/gthsdixbrl.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.chenlongwang.top/gtfoasljoo.html

TS:   if (x == null) {}
来源：http://hz.zdqjudy.top/gtahtcojgn.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.cashguo.top/gtffgaowqu.html

Go:   if x == nil {}
来源：http://hz.ybcxt.top/gtnbkvcgkb.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.shangyingyoupin.top/gtsbtaerrz.html

C#:   if (x is null) {}
来源：http://hz.guowangkeji.top/gtikpcyjcb.html

[P07] 防抖与节流
来源：http://hz.yanxiufei.cn/gtybdadbyo.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.ehwqpu.com/gtwwaxjxop.html

PHP:  // 手写时间戳比较
来源：http://hz.guannengcc.top/gtmnzofacv.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.sysykeji.top/gthtjqevin.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.c1oappe.top/gtlkpfqddr.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.yuanzhike.top/gtmvybowxh.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.smart0.xyz/gtvmzqtaem.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.yj20258888.top/gtamlxgtax.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.snrcjt.cn/gtegsaaljh.html

[P08] 处理浮点精度问题
来源：http://hz.ydjk.org.cn/gtagkyfuft.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.nwbrower.top/gtivseeawi.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.0kj1m.cn/gtvwgoegsd.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.daxiang520.top/gtilyiqdrd.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.cdnleiting.top/gtuaqlqasm.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.xuetiantiany.cn/gtlulprwnw.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.gzhubu.top/gthjxarnvv.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.yuxming.cn/gtcfuriuqd.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.c1oappe.top/gtlqxrulfy.html

================================================================================
来源：http://hz.aizwys.cn/gtrkjlzvmx.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.yuanzhike.top/gtjcnwhiml.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtmgipptdq.html

[Q01] 创建表
来源：http://hz.zhengqikj.top/gtlfdaifpv.html

CREATE TABLE users (
来源：http://hz.chenzaomai.com/gtqqiwsmgz.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.xinyue.icu/gtbnjakrjq.html

name VARCHAR(50) NOT NULL,
来源：http://hz.quarkkingdee.top/gtpuqcqgkh.html

email VARCHAR(100) UNIQUE,
来源：http://hz.jinqigufen.top/gtmeymdqvp.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.chenzaomai.com/gtjpjdvysw.html

);
来源：http://hz.zhaomingkeji.xyz/gtxkluaqbm.html

[Q02] 创建带外键的表
来源：http://hz.guowangkeji.top/gtiisrwqcb.html

CREATE TABLE orders (
来源：http://hz.0kj1m.cn/gtkaiehphb.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.tian-w.cn/gtcikaxyzf.html

user_id INT NOT NULL,
来源：http://hz.guowangkeji.top/gtoexgeefc.html

amount DECIMAL(10, 2),
来源：http://hz.hysaishi.cn/gtacycucqq.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.xuetiantiany.cn/gtaamerohb.html

);
来源：http://hz.9152youxi.cn/gtmyajcfks.html

[Q03] 增加列
来源：http://hz.cucudq.cn/gtciiidaen.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.nanxuanxn.top/gtwlhjivxn.html

[Q04] 修改列类型
来源：http://hz.dianchejie.cn/gtfjmdmodo.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.ehwqpu.com/gtafqidqin.html

[Q05] 重命名列
来源：http://hz.jinqigfzy.top/gtskvnqmxf.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.xinyue.icu/gtlvbfsoho.html

[Q06] 删除列
来源：http://hz.jinqigufen.top/gtbtrsdlyq.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.ydjk.org.cn/gtinbvgfhb.html

[Q07] 删除表
来源：http://hz.pengpengdd.cyou/gtpxkyopjn.html

DROP TABLE IF EXISTS orders;
来源：http://hz.shanyushiyangtech.top/gtfwcvqhbu.html

[Q08] 创建普通索引
来源：http://hz.sysykeji.top/gtrftjrgel.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.zhengqikj.top/gtwrehkqht.html

[Q09] 创建唯一索引
来源：http://hz.hongshengwenyu.top/gthiwhsauw.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.sufxvd.cn/gtwpclassl.html

[Q10] 插入单行
来源：http://hz.9152youxi.cn/gtaqymmoig.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.nanxinkj.top/gthbtsmfkm.html

[Q11] 一次插入多行
来源：http://hz.yonumen.top/gtfvjjewlx.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.yj20258888.top/gtqrqtwjdf.html

[Q12] 插入后取自增 ID
来源：http://hz.zhiwuduotai.top/gtetejsmpb.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.vqdsnc.cn/gtsmoheekl.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.zhengqikj.top/gtnzkxpuzm.html

[Q13] 忽略重复插入
来源：http://hz.pycfn.com/gtkoigmvxg.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.dashuyun.cn/gtmrqfakvt.html

[Q14] 存在则更新（upsert）
来源：http://hz.jianghu66.top/gthaayeymo.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.xuanzx.com/gtxkohrpts.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.gaohongyu789.top/gtmiwlgsdm.html

[Q15] 查询全部
来源：http://hz.hnqzz.top/gtsjrzdedd.html

SELECT * FROM users;
来源：http://hz.xingfuxueyuan.xyz/gtninwejlr.html

[Q16] 查询指定列
来源：http://hz.nwbrower.top/gtwafmycgy.html

SELECT id, name FROM users;
来源：http://hz.cheryme.top/gtrgmvmavt.html

[Q17] 条件查询
来源：http://hz.jinqigfzy.top/gtoviaxziw.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.kuanghao11.cn/gtuqrymuxo.html

[Q18] 模糊匹配
来源：http://hz.guowangkeji.top/gtdhsmqxer.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.cqqwz.cn/gtnsczyfgq.html

[Q19] 范围查询
来源：http://hz.hysaishi.cn/gtcfyrkoko.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.yongpay.top/gtgkgrutsu.html

[Q20] IN 列表
来源：http://hz.0kj1m.cn/gtalnaqybe.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.yuanzhike.top/gtxkcuullf.html

[Q21] 空值判断
来源：http://hz.yanxiufei.cn/gtjjsiljtt.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.shanyushiyangkeji.top/gtygnaxbek.html

[Q22] 排序
来源：http://hz.zhoulong.xyz/gtewmwpgcw.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.fengsongda.top/gtvlyfhbch.html

[Q23] 分页
来源：http://hz.tanke756.top/gtlqllkswf.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.gzhubu.top/gtjotsxekt.html

[Q24] 去重
来源：http://hz.jqgfzy.top/gtnfmehbos.html

SELECT DISTINCT city FROM users;
来源：http://hz.zhixingplan.top/gtarsecgka.html

[Q25] 只取前 N 条
来源：http://hz.svipenyu.cn/gtmuehmivt.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.tianlin.xyz/gtbqhpnirm.html

[Q26] 计数
来源：http://hz.sufxvd.cn/gtkgxfurau.html

SELECT COUNT(*) FROM users;
来源：http://hz.guowangkeji.top/gtnopowbln.html

[Q27] 条件计数
来源：http://hz.iojbl.cn/gtgrlcjluu.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.ydzc1.top/gtdovetmnb.html

[Q28] 求和与平均
来源：http://hz.jqgfzy.top/gtngpumxmw.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.hammf.cn/gtkxiwpyfq.html

[Q29] 最大最小值
来源：http://hz.xuanzx.com/gtdbfeeeib.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.yj20258.top/gtynynzrez.html

[Q30] 分组统计
来源：http://hz.aizwys.cn/gtejnfhvck.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.pengpengdd.cyou/gtazueybce.html

[Q31] 分组后过滤
来源：http://hz.c1oappe.top/gtkayfgonc.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.9152youxi.cn/gtmmpzibch.html

[Q32] 分组拼接字符串
来源：http://hz.yj202588.top/gtzkdiwzpb.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.jiagoushi.top/gttzajjpji.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.yueranfly.top/gtfvsycpyh.html

[Q33] 多列分组
来源：http://hz.c1oappe.top/gtaecoakue.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.tanke756.top/gttsghhhtt.html

[Q34] 每组取第一条
来源：http://hz.smart0.xyz/gtfpaedesp.html

SELECT * FROM (
来源：http://hz.aibaodan.cn/gtemztpczt.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.nanxinkj.top/gtsuyfdgjb.html

) t WHERE rn = 1;
来源：http://hz.yongpay.top/gtteplqxcw.html

[Q35] 内连接
来源：http://hz.zhengqikj.top/gtxbcxiodx.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.haohaochexian.top/gtzmftvnjo.html

[Q36] 左连接
来源：http://hz.ivvv.top/gtvgnckxvt.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.pycfn.com/gtcwtgeovv.html

[Q37] 右连接
来源：http://hz.jlsjyb.cn/gtakkdttfz.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.daxiang520.top/gtzefaunya.html


<!-- 参考信息 -->