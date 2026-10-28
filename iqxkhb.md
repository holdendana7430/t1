代发 wailian999

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.zhiwuduotai.top/gtzspixyyw.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.birdmap.top/gtynkzvyfe.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.fzhhl.top/gtrjoarmzp.html

Go:   slices.Sort(arr)
来源：http://hz.zdqjudy.top/gtffwpzbjd.html

Ruby: arr.sort
来源：http://hz.hywenlv.cn/gtgwihiykk.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.sweek.top/gtqybxtgzj.html

[N03] 快速排序（分治示例）
来源：http://hz.kuanghao11.cn/gtflnoptrp.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.haohaochexian.top/gtecrwdahj.html

PHP:  // 递归实现，或用 usort
来源：http://hz.aibaodan.cn/gtxumpzbvw.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.0kj1m.cn/gtusocmeyf.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.zycfv.cn/gtwujtjtky.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.pycfn.com/gtnlvrlgzs.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.svipenyu.cn/gtozkmjacp.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.aibaodan.cn/gtwypvvcxl.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.hnxiangtu.top/gtqilbvcaz.html

[N04] 斐波那契数列
来源：http://hz.tianlin.xyz/gtnjrvprym.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.daria6918.cn/gtemqjurqr.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.shangyingyoupin.top/gtnocqjemf.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.jinghuilouyu.cn/gtofypcgwq.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.zhijiandao.cn/gtfcdsnwij.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.andypj.xyz/gthhqhyzct.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.redwolf501.top/gthkjqezav.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.ydzc1.top/gtgispsbxe.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.sxryk.cn/gtbdvtfaau.html

[N05] 最大公约数
来源：http://hz.snrcjt.cn/gtrxvdolee.html

Py:   math.gcd(a, b)
来源：http://hz.jinqigufen.top/gtbsayvdnd.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.sxryk.cn/gtetauiddt.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.jqgufenzy.top/gtjhfzazqa.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.chenzaomai.com/gtzimzfeki.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.xylfe.cn/gtkrudoron.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.ywan-chungtsiang.top/gtvtvsrrey.html

Ruby: a.gcd(b)
来源：http://hz.hywenlv.cn/gtyfllrekk.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.aizwys.cn/gtgjivcxpc.html

[N06] 判断回文字符串
来源：http://hz.hysaishi.cn/gtcvgqheew.html

Py:   s == s[::-1]
来源：http://hz.gzhubu.top/gtlfdioewz.html

PHP:  $s === strrev($s);
来源：http://hz.shzxlz.cn/gtnhgdhzxl.html

JS:   s === [...s].reverse().join("")
来源：http://hz.yueranfly.top/gtblvuoelb.html

TS:   s === [...s].reverse().join("")
来源：http://hz.hnqzz.top/gtmxdekujw.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.ywan-chungtsiang.top/gtigwoedmc.html

Go:   // 双指针从两端比较
来源：http://hz.jiagoushi.top/gtxaryexea.html

Ruby: s == s.reverse
来源：http://hz.yj20258888.top/gtftswxswl.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.ivvv.top/gtunjqiycr.html

[N07] 两数之和（返回下标）
来源：http://hz.zycfv.cn/gtbllbussx.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.hnqzz.top/gtjxelgxma.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.yj20258.top/gttjpeainq.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.zhoulong.xyz/gtxfdgenpq.html

TS:   // 手写 Map<string, number>
来源：http://hz.shzxlz.cn/gtdmhmxrgu.html

Java: // 手写 HashMap
来源：http://hz.52xcode.cn/gtmqsgxvrm.html

Go:   // 手写 map[int]int
来源：http://hz.hfpthk.cn/gtoopsrphl.html

Ruby: // 手写 Hash
来源：http://hz.xylfe.cn/gtbgeupddd.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.guannengcc.top/gthrzliltp.html

[N08] 生成全排列
来源：http://hz.nanxinkj.top/gtdwafdzzo.html

Py:   itertools.permutations(arr)
来源：http://hz.jinyuanbaomall.cn/gtybbdeilr.html

PHP:  // 手写递归交换
来源：http://hz.ppjwa.cn/gtwvtlyeff.html

JS:   // 手写回溯递归
来源：http://hz.hongshengwenyu.top/gtvscuajxy.html

TS:   // 手写回溯递归
来源：http://hz.sufxvd.cn/gtsxglomtv.html

Java: // 手写回溯递归
来源：http://hz.sxryk.cn/gtrfqptywi.html

Go:   // 手写回溯递归
来源：http://hz.sweek.top/gtgpdcpbwj.html

Ruby: arr.permutation.to_a
来源：http://hz.tanke756.top/gtpvencwpq.html

C#:   // 手写回溯递归
来源：http://hz.jlsjyb.cn/gtxknhgpot.html

[N09] 栈与队列
来源：http://hz.cucudq.cn/gtreayvgms.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.kuanghao11.cn/gtwrrrmjeo.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.havefunace.top/gtdfjzyhuh.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.zycfv.cn/gtterxiknd.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.redwolf501.top/gtsgitecia.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.ydzc1.top/gtyfzuhpvl.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.zdqjudy.top/gthanlcois.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.gogol.net.cn/gtwjycmxco.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.ehwqpu.com/gtrvuryzaw.html

[N10] 链表节点定义
来源：http://hz.zhixingplan.top/gtsktnddwc.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.dianchejie.cn/gtsskyttsv.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.jianghu66.top/gteoczzjqh.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.gotoacloud.top/gtntyzptve.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.ydjk.org.cn/gtlplhztse.html

Java: class Node { int v; Node next; }
来源：http://hz.dashuyun.cn/gtazpkrviw.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.gaohongyu789.top/gtufxjfjpy.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.andypj.xyz/gtewdcquer.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.yangfankeji.com/gtjuywnefo.html

[N11] 二叉树中序遍历
来源：http://hz.aizwys.cn/gtsugibren.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.ehwqpu.com/gtdprzcqrn.html

PHP:  // 手写递归函数
来源：http://hz.zhengqikj.top/gtqsqptnnv.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.shangyingyoupin.top/gtnlqdsxpo.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.ehwqpu.com/gtkwzrbzax.html

Java: // 手写递归
来源：http://hz.meibo888.top/gtrqfahcxg.html

Go:   // 手写递归
来源：http://hz.meibo888.top/gtmoxyimnn.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.c1oappe.top/gthnworvls.html

C#:   // 手写递归
来源：http://hz.cdnleiting.top/gtususnots.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.xylfe.cn/gtrcwywccz.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.zhixingplan.top/gtoeekwevv.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.wangshuangyany.cn/gtfcreywkz.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.dashuyun.cn/gteivlromc.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.sysykeji.top/gtsqxneqsd.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.smart0.xyz/gtgyqssnhb.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.dianchejie.cn/gtorcrcbvp.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.jinghuilouyu.cn/gtqpgbieyl.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.jinghuilouyu.cn/gtuiheeqsn.html

================================================================================
来源：http://hz.yuanzhike.top/gtgxtxryvj.html

O. 并发与异步
来源：http://hz.shangyingyoupin.top/gtuckwveof.html

================================================================================
来源：http://hz.mhx1999.top/gtccpozgya.html

[O01] 启动一个线程
来源：http://hz.yvedp.cn/gtnjaefwow.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.cqqwz.cn/gtnlbqaquv.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.xziqi.cn/gtdcrjejwb.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.feifeiyinyue.top/gtubxlrvuo.html

TS:   // 同 JS
来源：http://hz.iojbl.cn/gtplwfzkot.html

Java: new Thread(() -> f()).start()
来源：http://hz.sufxvd.cn/gtmrhvkrcl.html

Go:   go f()
来源：http://hz.nwbrower.top/gtxqhoacxj.html

Ruby: Thread.new { f }
来源：http://hz.haohaochexian.top/gtcsnepbly.html

C#:   Task.Run(() => F());
来源：http://hz.jlsjyb.cn/gtvadymtxh.html

[O02] 使用线程池
来源：http://hz.0kj1m.cn/gtqpigbjlw.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.zhoulong.xyz/gtoxevhqce.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.haohaochexian.top/gtlphmmhdg.html

JS:   // worker_threads 线程池
来源：http://hz.zhaomingkeji.xyz/gtuaxufozo.html

TS:   // worker_threads 线程池
来源：http://hz.shanyushiyangtech.top/gtreighnax.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.svipenyu.cn/gtjzioscqd.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.dianchejie.cn/gtaenyvkbd.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.xziqi.cn/gtjihhnchz.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.xingfuxueyuan.xyz/gtbxtwjjvj.html

[O03] 加锁保护共享数据
来源：http://hz.jinyuanbaomall.cn/gtouhosbud.html

Py:   with lock: shared += 1
来源：http://hz.sxryk.cn/gtfpeprldi.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.zhoulong.xyz/gtfgckshml.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.ywan-chungtsiang.top/gthyxtxcse.html

TS:   // 同 JS
来源：http://hz.yonumen.top/gtmnsqivct.html

Java: synchronized (this) { shared++; }
来源：http://hz.yueranfly.top/gtvijxnmjd.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.haohaochexian.top/gtlmuecmkg.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.guannengcc.top/gtxkptndos.html

C#:   lock (gate) { shared++; }
来源：http://hz.jiagoushi.top/gtsebpuzbx.html

[O04] 定义异步函数并等待
来源：http://hz.quarkkingdee.top/gtkqmxfgvl.html

Py:   async def f():⏎    await g()
来源：http://hz.shuidangran.top/gtghelyvra.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.hfpthk.cn/gtwwekrncw.html

JS:   async function f() { await g(); }
来源：http://hz.zhixingplan.top/gtzsfepyhr.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.zhiwuduotai.top/gtytiwvvwe.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.zhoulong.xyz/gtgjmfqjsy.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.iojbl.cn/gtqtqjtreu.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.pycfn.com/gthrxcrqyf.html

C#:   async Task F() { await G(); }
来源：http://hz.wangshuangyany.cn/gtqywiyccc.html

[O05] 并发执行并等待全部完成
来源：http://hz.havefunace.top/gtgrfauamr.html

Py:   asyncio.gather(*tasks)
来源：http://hz.yuanzhike.top/gthrfequzr.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.shangyingyoupin.top/gtkywctaaw.html

JS:   await Promise.all(tasks)
来源：http://hz.dashuyun.cn/gtinxyhnrd.html

TS:   await Promise.all(tasks)
来源：http://hz.yj20258.top/gtnlkwddcs.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.jinyuanbaomall.cn/gtimbdfvgk.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.wangshuangyany.cn/gtqzrjfxzu.html

Ruby: threads.map(&:join)
来源：http://hz.yuanzhike.top/gtodchapob.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.snrcjt.cn/gtwlpgkqby.html

[O06] 使用进程池
来源：http://hz.mhx1999.top/gtlrtvbdox.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.0kj1m.cn/gthbrzoybx.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.xuanzx.com/gtxwrgxmoi.html

JS:   // child_process / cluster 模块
来源：http://hz.hongshengwenyu.top/gtvusxdmfa.html

TS:   // child_process / cluster 模块
来源：http://hz.guannengcc.top/gtthwxclnj.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.andypj.xyz/gtkxtkxocb.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.daxiang520.top/gtungsfsmz.html

Ruby: // fork 块
来源：http://hz.jiagoushi.top/gtxdnmlmgc.html

C#:   Parallel.For
来源：http://hz.meibo888.top/gtmmjqlqsp.html

================================================================================
来源：http://hz.haohaochexian.top/gtlqofqewk.html

P. 常用工具函数
来源：http://hz.jinqigfzy.top/gtvdfzsbyv.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gtjsdloepe.html

[P01] 生成 UUID
来源：http://hz.sysykeji.top/gtbaovdqkf.html

Py:   str(uuid.uuid4())
来源：http://hz.birdmap.top/gthwutidol.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.jiagoushi.top/gtkckpqotx.html

JS:   crypto.randomUUID()
来源：http://hz.jianghu66.top/gtfzsrqxst.html

TS:   crypto.randomUUID()
来源：http://hz.shuidangran.top/gtjbixdxyn.html

Java: UUID.randomUUID().toString()
来源：http://hz.zhixingplan.top/gtfanreygj.html

Go:   // 用 github.com/google/uuid
来源：http://hz.zdqjudy.top/gtkrnbltex.html

Ruby: SecureRandom.uuid
来源：http://hz.cheryme.top/gtpmmscpig.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.nanxuanxn.top/gtispgvfql.html

[P02] MD5 / SHA256 摘要
来源：http://hz.jinyuanbaomall.cn/gtyqbaonji.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.yuxming.cn/gtifkdthbp.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.yuxming.cn/gtecxbtjwr.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.hnqzz.top/gtzvqgggrk.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.pycfn.com/gtbpcpkipv.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.daxiang520.top/gtwykxjcoe.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.nanxinkj.top/gtlaiezmta.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.yuanzhike.top/gtcqjnaaej.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.ybcxt.top/gtalsblvcc.html

[P03] 生成短随机字符串
来源：http://hz.yanxiufei.cn/gtzdytfmsq.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.ywan-chungtsiang.top/gtjohufgjz.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.yj20258888.top/gtbzuvjvmd.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.xuanzx.com/gtkvuomlas.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.yj202588.top/gtepdkqnfc.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.sysykeji.top/gtrehxwyry.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.guannengcc.top/gtcdaevhsb.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.jyoumei.cn/gtctwbdylp.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.hfpthk.cn/gtftiksola.html

[P04] 求长度
来源：http://hz.birdmap.top/gtxztgihkl.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.kuanghao11.cn/gtanetrugf.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.guannengcc.top/gtqsaljodh.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.tian-w.cn/gtdvczzofw.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.mhx1999.top/gtvixcntrk.html

Java: list.size();  map.size();  s.length()
来源：http://hz.bjfxy.top/gtbbqtgxgo.html

Go:   len(arr);  len(m)
来源：http://hz.yuxming.cn/gtcrsmsabl.html

Ruby: x.length;  x.size
来源：http://hz.zhengqikj.top/gtrqayjeib.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.chenjidiqi.icu/gtdoynnxtc.html

[P05] 判断两个对象内容是否相等
来源：http://hz.sxryk.cn/gtgtgqyugd.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.yanxiufei.cn/gtgqratwvn.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.shangyingyoupin.top/gtmtykzsiz.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.nwbrower.top/gtvvpysylc.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.316326.xyz/gtseizblyt.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.birdmap.top/gtiglougti.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.9152youxi.cn/gtmtlzrhdf.html

Ruby: a == b
来源：http://hz.9152youxi.cn/gtoohrwkqd.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.bjfxy.top/gtysrsaofj.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.cucudq.cn/gtfhluleyu.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.svipenyu.cn/gtffajglit.html

PHP:  if (empty($x)) {}
来源：http://hz.iojbl.cn/gtltrryacm.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.hnxiangtu.top/gtdwpqdujo.html

TS:   if (x == null) {}
来源：http://hz.yonumen.top/gtkzlqbguo.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.shzxlz.cn/gtfcoeovuk.html

Go:   if x == nil {}
来源：http://hz.zhaomingkeji.xyz/gtlrgwmosp.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.wangshuangyany.cn/gtgnawefjn.html

C#:   if (x is null) {}
来源：http://hz.iojbl.cn/gtfkffuthr.html

[P07] 防抖与节流
来源：http://hz.jyoumei.cn/gtkcvegyqw.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.kuanghao11.cn/gtkffgsdjv.html

PHP:  // 手写时间戳比较
来源：http://hz.dianchejie.cn/gthyxehikd.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.nwbrower.top/gtcyxjlwss.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.cqqwz.cn/gtkqjfjyat.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.tian-w.cn/gtptlvoqic.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.guannengcc.top/gtzbonibeb.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.yanxiufei.cn/gtcsnepdru.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.wangshuangyany.cn/gtugjqecuy.html

[P08] 处理浮点精度问题
来源：http://hz.ywan-chungtsiang.top/gtaccjfxrq.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.zhaomingkeji.xyz/gtsqwdgthl.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.shanyushiyangtech.top/gtbfuosaej.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.hnxiangtu.top/gtrrnyxktx.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.tianlin.xyz/gtwkavrxxu.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.yuxming.cn/gtggesetgs.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.nanxinkj.top/gtcjikwfav.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.bjfxy.top/gtmgilndhv.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.yj20258.top/gtbgppdjak.html

================================================================================
来源：http://hz.daria6918.cn/gtzaojidti.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.haohaochexian.top/gtidgpjbnx.html

================================================================================
来源：http://hz.zhijiandao.cn/gtfhshwqbx.html

[Q01] 创建表
来源：http://hz.aibaodan.cn/gtmokxjtpn.html

CREATE TABLE users (
来源：http://hz.smart0.xyz/gtvyrruwqz.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.cqqwz.cn/gtckgdcbwi.html

name VARCHAR(50) NOT NULL,
来源：http://hz.hongshengwenyu.top/gtggrrodbi.html

email VARCHAR(100) UNIQUE,
来源：http://hz.xingfuxueyuan.xyz/gttnujvgah.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.yanxiufei.cn/gtnnkqjnmq.html

);
来源：http://hz.chenjidiqi.icu/gtcyaxjkwl.html

[Q02] 创建带外键的表
来源：http://hz.tianlin.xyz/gtfnlbggob.html

CREATE TABLE orders (
来源：http://hz.pycfn.com/gtqajpysvw.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.hfpthk.cn/gthieuacup.html

user_id INT NOT NULL,
来源：http://hz.c1oappe.top/gtujjqkeyb.html

amount DECIMAL(10, 2),
来源：http://hz.yuanzhike.top/gtdidwhxck.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.xinyue.icu/gtvmuefglm.html

);
来源：http://hz.gzhubu.top/gtzcqgegkk.html

[Q03] 增加列
来源：http://hz.shzxlz.cn/gtvreuaovf.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.yonumen.top/gtnfyjkuyc.html

[Q04] 修改列类型
来源：http://hz.vqdsnc.cn/gtcbpszbuf.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.gaohongyu789.top/gtiacsalln.html

[Q05] 重命名列
来源：http://hz.sysykeji.top/gtrlwkzwep.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.cucudq.cn/gtifppjkmd.html

[Q06] 删除列
来源：http://hz.ehwqpu.com/gtemhglvsp.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.yuanzhike.top/gtvhuufloz.html

[Q07] 删除表
来源：http://hz.wangshuangyany.cn/gtljgymqth.html

DROP TABLE IF EXISTS orders;
来源：http://hz.daria6918.cn/gtrpkjgcag.html

[Q08] 创建普通索引
来源：http://hz.hfpthk.cn/gtuacnvgta.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.sufxvd.cn/gtlsfofnnk.html

[Q09] 创建唯一索引
来源：http://hz.daria6918.cn/gtbodfjhhx.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.zdqjudy.top/gthaeclmuc.html

[Q10] 插入单行
来源：http://hz.zhengqikj.top/gtjcteachs.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.ppjwa.cn/gttrtvvyhw.html

[Q11] 一次插入多行
来源：http://hz.birdmap.top/gtghmbndnq.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.yvedp.cn/gtnpkbrpij.html

[Q12] 插入后取自增 ID
来源：http://hz.zhongyouzk.top/gtwuufidso.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.cashguo.top/gtvnnelveu.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.jinyuanbaomall.cn/gtlmepvleh.html

[Q13] 忽略重复插入
来源：http://hz.zdqjudy.top/gtbmkhzemd.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.9152youxi.cn/gtgcfehboc.html

[Q14] 存在则更新（upsert）
来源：http://hz.sweek.top/gtvuuvwhiz.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.feifeiyinyue.top/gtwdbucubd.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.ehwqpu.com/gtsjrosrgc.html

[Q15] 查询全部
来源：http://hz.cqqwz.cn/gtcdepnuhh.html

SELECT * FROM users;
来源：http://hz.fzhhl.top/gtjpjeeval.html

[Q16] 查询指定列
来源：http://hz.fzhhl.top/gtaewemfdf.html

SELECT id, name FROM users;
来源：http://hz.svipenyu.cn/gtvwlgubvd.html

[Q17] 条件查询
来源：http://hz.cdnleiting.top/gtyrvvexio.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.jinghuilouyu.cn/gtjsmwbnjt.html

[Q18] 模糊匹配
来源：http://hz.ehwqpu.com/gtuhdzvgqi.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.guannengcc.top/gtvsgbrjun.html

[Q19] 范围查询
来源：http://hz.chenzaomai.com/gtnyiruiow.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.cqqwz.cn/gtobmypeko.html

[Q20] IN 列表
来源：http://hz.zycfv.cn/gtffkxxxtw.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.ydjk.org.cn/gttnqlwiwl.html

[Q21] 空值判断
来源：http://hz.ywan-chungtsiang.top/gtouczvzgj.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.vqdsnc.cn/gtenrcknys.html

[Q22] 排序
来源：http://hz.pycfn.com/gtflnlotwh.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.hnxiangtu.top/gtlkmdsczx.html

[Q23] 分页
来源：http://hz.yueranfly.top/gtquyfjcvb.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.bjfxy.top/gtrpwyebfo.html

[Q24] 去重
来源：http://hz.jinghuilouyu.cn/gtgxltwwlo.html

SELECT DISTINCT city FROM users;
来源：http://hz.vqdsnc.cn/gtidytzpxu.html

[Q25] 只取前 N 条
来源：http://hz.xylfe.cn/gtzmzgmzjc.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.tanke756.top/gtmtlianlr.html

[Q26] 计数
来源：http://hz.zhengqikj.top/gteekfhyht.html

SELECT COUNT(*) FROM users;
来源：http://hz.ydzc1.top/gtzsuzouby.html

[Q27] 条件计数
来源：http://hz.havefunace.top/gtsrbjaubq.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.9152youxi.cn/gtahicncdg.html

[Q28] 求和与平均
来源：http://hz.svipenyu.cn/gtcukpgsjy.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.0kj1m.cn/gtpyxzlfpj.html

[Q29] 最大最小值
来源：http://hz.zhixingplan.top/gttpftgaja.html


<!-- 参考信息 -->