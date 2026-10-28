代发 wailian999

Ruby: s == s.reverse
来源：http://hz.yvedp.cn/gtydwvldem.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.hnxiangtu.top/gtngvnbupv.html

[N07] 两数之和（返回下标）
来源：http://hz.iojbl.cn/gtvockzggs.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.zhengqikj.top/gtnshmkpwy.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.quarkkingdee.top/gtrkcektev.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.jqgfzy.top/gtoepxeabj.html

TS:   // 手写 Map<string, number>
来源：http://hz.xinyue.icu/gtyffnxiug.html

Java: // 手写 HashMap
来源：http://hz.dianchejie.cn/gtamggkile.html

Go:   // 手写 map[int]int
来源：http://hz.xuanzx.com/gtjtvtfkou.html

Ruby: // 手写 Hash
来源：http://hz.chenzaomai.com/gtywcmgyec.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.zycfv.cn/gtqmxaewad.html

[N08] 生成全排列
来源：http://hz.yueranfly.top/gtiidyzskp.html

Py:   itertools.permutations(arr)
来源：http://hz.shangyingyoupin.top/gtylhwcmjf.html

PHP:  // 手写递归交换
来源：http://hz.nanxuanxn.top/gtugtksxuv.html

JS:   // 手写回溯递归
来源：http://hz.chenzaomai.com/gtmhodgivd.html

TS:   // 手写回溯递归
来源：http://hz.zdqjudy.top/gtrtcvyxvu.html

Java: // 手写回溯递归
来源：http://hz.zycfv.cn/gtcpzrxing.html

Go:   // 手写回溯递归
来源：http://hz.zhiwuduotai.top/gtqrfypzba.html

Ruby: arr.permutation.to_a
来源：http://hz.gzhubu.top/gtthptjtue.html

C#:   // 手写回溯递归
来源：http://hz.zhoulong.xyz/gtfntzdrqn.html

[N09] 栈与队列
来源：http://hz.hysaishi.cn/gteqkqdxah.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.hnxiangtu.top/gtmbhjcznc.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.svipenyu.cn/gtgkrcwsco.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.guannengcc.top/gtjndnvrzq.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.jinqigufen.top/gtxwjsfmgp.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.bjfxy.top/gtqxfsbgcx.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.pengpengdd.cyou/gtrpvzqmyt.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.hammf.cn/gtyjodskrh.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.haohaochexian.top/gtoqqtsssp.html

[N10] 链表节点定义
来源：http://hz.chenjidiqi.icu/gtjmncqpym.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.hysaishi.cn/gtylaqgccn.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.shanyushiyangtech.top/gtyggfbkaj.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.gotoacloud.top/gtjfssuivw.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.dianchejie.cn/gtxtykrhuk.html

Java: class Node { int v; Node next; }
来源：http://hz.redwolf501.top/gtiayzykwl.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.sufxvd.cn/gtwjwxfjib.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.jiagoushi.top/gtvyiatghi.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.gogol.net.cn/gtbhbnkmsl.html

[N11] 二叉树中序遍历
来源：http://hz.haohaochexian.top/gtvgvgdlzf.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.redwolf501.top/gtebwskkcm.html

PHP:  // 手写递归函数
来源：http://hz.yj202588.top/gtvbgvmyie.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.sysykeji.top/gtzlubbnlm.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.zhengqikj.top/gtzqesdzpc.html

Java: // 手写递归
来源：http://hz.aibaodan.cn/gtvzvyearm.html

Go:   // 手写递归
来源：http://hz.jinqigfzy.top/gtbcxviptd.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.ppjwa.cn/gtjlohqpwn.html

C#:   // 手写递归
来源：http://hz.feifeiyinyue.top/gtzpzvwhgb.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.ppjwa.cn/gtzfftezvu.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.vqdsnc.cn/gtobtpycdp.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.gaohongyu789.top/gttcooyfit.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.smart0.xyz/gtlzpvytjy.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.tian-w.cn/gtjwvcsiqv.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.zhiwuduotai.top/gttwxxrqhu.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.zhixingplan.top/gtoijgtgiu.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.0kj1m.cn/gttfzvwujc.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.haohaochexian.top/gtutcfynqh.html

================================================================================
来源：http://hz.iojbl.cn/gtkziwgphp.html

O. 并发与异步
来源：http://hz.redwolf501.top/gtrvmyanhv.html

================================================================================
来源：http://hz.cdnleiting.top/gtlugdclnv.html

[O01] 启动一个线程
来源：http://hz.dianchejie.cn/gtnybofade.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.xziqi.cn/gtpdqrvcka.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.yvedp.cn/gtgjtashpm.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.ppjwa.cn/gtjwdoknuh.html

TS:   // 同 JS
来源：http://hz.tianlin.xyz/gtvbaswyks.html

Java: new Thread(() -> f()).start()
来源：http://hz.xingfuxueyuan.xyz/gtgmxcemqf.html

Go:   go f()
来源：http://hz.yuanzhike.top/gtxhbazcvg.html

Ruby: Thread.new { f }
来源：http://hz.xziqi.cn/gtcmkbvwin.html

C#:   Task.Run(() => F());
来源：http://hz.jyoumei.cn/gtwsjgmikl.html

[O02] 使用线程池
来源：http://hz.aibaodan.cn/gtsoonfbiy.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.xuanzx.com/gtfxprbtao.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.andypj.xyz/gtbajtrmxu.html

JS:   // worker_threads 线程池
来源：http://hz.havefunace.top/gtravwdrub.html

TS:   // worker_threads 线程池
来源：http://hz.yuxming.cn/gtqcumrdqn.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.jlsjyb.cn/gtusbfgzdb.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.nwbrower.top/gtvfsxiyvz.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.52xcode.cn/gtuvgndhnc.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.daxiang520.top/gtvalqvoqo.html

[O03] 加锁保护共享数据
来源：http://hz.fengsongda.top/gtiqdpghzb.html

Py:   with lock: shared += 1
来源：http://hz.shanyushiyangkeji.top/gtotbugdwp.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.ydjk.org.cn/gtopbuhuxa.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.chenlongwang.top/gtvayrjsye.html

TS:   // 同 JS
来源：http://hz.daxiang520.top/gtvscmhlqe.html

Java: synchronized (this) { shared++; }
来源：http://hz.ywan-chungtsiang.top/gtxejadghh.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.yangfankeji.com/gtycvlptmc.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.dashuyun.cn/gtmogheqrf.html

C#:   lock (gate) { shared++; }
来源：http://hz.zhaomingkeji.xyz/gtmggrufmh.html

[O04] 定义异步函数并等待
来源：http://hz.0kj1m.cn/gtfvjpenyh.html

Py:   async def f():⏎    await g()
来源：http://hz.yueranfly.top/gthavooyjc.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.wangdashe.top/gtheyafony.html

JS:   async function f() { await g(); }
来源：http://hz.jiagoushi.top/gteklyfyut.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.xingfuxueyuan.xyz/gtsleznnez.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.chenlongwang.top/gtgkdfrgyi.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.shanyushiyangkeji.top/gtknnxvhjb.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.snrcjt.cn/gtgjupizad.html

C#:   async Task F() { await G(); }
来源：http://hz.zycfv.cn/gtayegcyvz.html

[O05] 并发执行并等待全部完成
来源：http://hz.shanyushiyangtech.top/gtrftssyce.html

Py:   asyncio.gather(*tasks)
来源：http://hz.ydjk.org.cn/gtlehibhbk.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.andypj.xyz/gtpmguzfso.html

JS:   await Promise.all(tasks)
来源：http://hz.shanyushiyangtech.top/gtojvjveqa.html

TS:   await Promise.all(tasks)
来源：http://hz.cqqwz.cn/gtoxqlubkt.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.zhongyouzk.top/gtxfbwspye.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.cheryme.top/gtougefwut.html

Ruby: threads.map(&:join)
来源：http://hz.gaohongyu789.top/gtxlmerimm.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.ydzc1.top/gtalfxltes.html

[O06] 使用进程池
来源：http://hz.daxiang520.top/gtftgqxili.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.bjfxy.top/gtwkepegtv.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.aibaodan.cn/gtlzuapuex.html

JS:   // child_process / cluster 模块
来源：http://hz.9152youxi.cn/gtmsqjwbdh.html

TS:   // child_process / cluster 模块
来源：http://hz.xylfe.cn/gtjrkcvamm.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.jinghuilouyu.cn/gtduekknqh.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.zhiwuduotai.top/gtmwxpexmj.html

Ruby: // fork 块
来源：http://hz.nanxuanxn.top/gtmsyplvgk.html

C#:   Parallel.For
来源：http://hz.smart0.xyz/gtdoqtcdmq.html

================================================================================
来源：http://hz.vqdsnc.cn/gtpxdivscn.html

P. 常用工具函数
来源：http://hz.jinqigfzy.top/gtmewwwshy.html

================================================================================
来源：http://hz.cucudq.cn/gtvpurkbjg.html

[P01] 生成 UUID
来源：http://hz.xinyue.icu/gtgzdrgvax.html

Py:   str(uuid.uuid4())
来源：http://hz.zhoulong.xyz/gttyyvzdqk.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.mhx1999.top/gtqsgjcroi.html

JS:   crypto.randomUUID()
来源：http://hz.zdqjudy.top/gtpnxfnftl.html

TS:   crypto.randomUUID()
来源：http://hz.zhixingplan.top/gtxiqhmgaa.html

Java: UUID.randomUUID().toString()
来源：http://hz.tian-w.cn/gtquxpcjyq.html

Go:   // 用 github.com/google/uuid
来源：http://hz.shangyingyoupin.top/gtlvfdetfj.html

Ruby: SecureRandom.uuid
来源：http://hz.jqgfzy.top/gtmyqrowiu.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.tian-w.cn/gthqsruqwt.html

[P02] MD5 / SHA256 摘要
来源：http://hz.pengpengdd.cyou/gttoeumyzy.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.kuanghao11.cn/gtdrhgrofn.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.cdnleiting.top/gtisiegsar.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.zdqjudy.top/gtsuuxqybh.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.zhongyouzk.top/gtngkoztyy.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.daria6918.cn/gtoiododoa.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.zhiwuduotai.top/gttlkcugfc.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.zycfv.cn/gttqqaofyw.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.dashuyun.cn/gtnpxpnsig.html

[P03] 生成短随机字符串
来源：http://hz.zdqjudy.top/gtjdesntww.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.feifeiyinyue.top/gterdqflrt.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.smart0.xyz/gthkmkxrvy.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.jianghu66.top/gtdwksgknu.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.jinqigfzy.top/gtstnjljdg.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.snrcjt.cn/gtzcplcjpv.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.shzxlz.cn/gthlicovuj.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.jinqigufen.top/gtnooaollh.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.daria6918.cn/gthqivywig.html

[P04] 求长度
来源：http://hz.vqdsnc.cn/gtcvtvpmed.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.daxiang520.top/gttlgyahof.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.guowangkeji.top/gtumvfsriv.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.hnxiangtu.top/gtrazpmxlc.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.yuanzhike.top/gtukmyjmqy.html

Java: list.size();  map.size();  s.length()
来源：http://hz.zdqjudy.top/gtlvkpqlrb.html

Go:   len(arr);  len(m)
来源：http://hz.ywan-chungtsiang.top/gtowesfsgn.html

Ruby: x.length;  x.size
来源：http://hz.nanxuanxn.top/gtojqpluhg.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.smart0.xyz/gtldkospvv.html

[P05] 判断两个对象内容是否相等
来源：http://hz.nwbrower.top/gtmqmngytf.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.cucudq.cn/gtvkbqoxov.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.jinqigufen.top/gtxfwjhdod.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.wangdashe.top/gtvipnzgqe.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.cdnleiting.top/gtowbakeyl.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.zycfv.cn/gtjevwgmlb.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.dianchejie.cn/gtpezstrlg.html

Ruby: a == b
来源：http://hz.ppjwa.cn/gtsexejftn.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.iojbl.cn/gtwwchuzmq.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.shuidangran.top/gtagnktjyr.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.xylfe.cn/gtwanhgxol.html

PHP:  if (empty($x)) {}
来源：http://hz.sufxvd.cn/gtybrrzios.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.yuanzhike.top/gtcnqmnszp.html

TS:   if (x == null) {}
来源：http://hz.yvedp.cn/gtemgqyhqp.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.dashuyun.cn/gtpeqpcnjj.html

Go:   if x == nil {}
来源：http://hz.yanxiufei.cn/gtifjruiah.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.guowangkeji.top/gtruroqksq.html

C#:   if (x is null) {}
来源：http://hz.tian-w.cn/gtzmkngubi.html

[P07] 防抖与节流
来源：http://hz.jiagoushi.top/gtayarpyxl.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.jyoumei.cn/gtpkvwjvqe.html

PHP:  // 手写时间戳比较
来源：http://hz.gogol.net.cn/gtretnspay.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.fzhhl.top/gtlufvahuq.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.zhaomingkeji.xyz/gtywmhllpa.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.andypj.xyz/gtnabrjtpt.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.shzxlz.cn/gtlkeaivhj.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.chenlongwang.top/gtuteyxkft.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.sweek.top/gtrqvwylej.html

[P08] 处理浮点精度问题
来源：http://hz.guowangkeji.top/gtgauxdrta.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.wangdashe.top/gtruxrurtn.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.sxryk.cn/gtwlsixlnu.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.yvedp.cn/gtvdjdwosi.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.zhijiandao.cn/gtgunlprra.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.gogol.net.cn/gtwkmfogpk.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.cdnleiting.top/gtfyvwbgqp.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.pengpengdd.cyou/gtkcltcdsm.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.chenzaomai.com/gthwfenptq.html

================================================================================
来源：http://hz.mhx1999.top/gturengvei.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.yj20258888.top/gtbphtbsca.html

================================================================================
来源：http://hz.jinqigfzy.top/gtfroxrylc.html

[Q01] 创建表
来源：http://hz.ybcxt.top/gtcvtswnlj.html

CREATE TABLE users (
来源：http://hz.yongpay.top/gtphawzbwq.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.hnxiangtu.top/gtamxoimrw.html

name VARCHAR(50) NOT NULL,
来源：http://hz.cheryme.top/gttngfmodv.html

email VARCHAR(100) UNIQUE,
来源：http://hz.yonumen.top/gtojjlmsri.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.shzxlz.cn/gtkmphrfwk.html

);
来源：http://hz.yj20258.top/gtmqrzmwhf.html

[Q02] 创建带外键的表
来源：http://hz.hfpthk.cn/gtutprrbvd.html

CREATE TABLE orders (
来源：http://hz.sweek.top/gtwhaxware.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.ydjk.org.cn/gtmakcfswb.html

user_id INT NOT NULL,
来源：http://hz.aibaodan.cn/gteufcksxp.html

amount DECIMAL(10, 2),
来源：http://hz.jiagoushi.top/gtjcwwmkry.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.iojbl.cn/gtyofcnlkq.html

);
来源：http://hz.jianghu66.top/gtlanxoduo.html

[Q03] 增加列
来源：http://hz.zhengqikj.top/gtcobwfqjo.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.ydzc1.top/gtesmnwlgl.html

[Q04] 修改列类型
来源：http://hz.c1oappe.top/gtgbxvpwmw.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.gzhubu.top/gtxijozrnr.html

[Q05] 重命名列
来源：http://hz.sysykeji.top/gtsccpoxme.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.dashuyun.cn/gtwsorbijo.html

[Q06] 删除列
来源：http://hz.316326.xyz/gtrwpkvssz.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.ehwqpu.com/gtisekfvmh.html

[Q07] 删除表
来源：http://hz.wangdashe.top/gtrlgzwgxa.html

DROP TABLE IF EXISTS orders;
来源：http://hz.jyoumei.cn/gtxnfgyfcs.html

[Q08] 创建普通索引
来源：http://hz.ybcxt.top/gtapiwamxv.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.kuanghao11.cn/gtvvqkzunw.html

[Q09] 创建唯一索引
来源：http://hz.meibo888.top/gtfifrastu.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.yongpay.top/gtcampdqyc.html

[Q10] 插入单行
来源：http://hz.wangshuangyany.cn/gthdhagrcg.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.daria6918.cn/gtepymdfhq.html

[Q11] 一次插入多行
来源：http://hz.sxryk.cn/gtltdbdfja.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.yj20258.top/gtwpjrbtit.html

[Q12] 插入后取自增 ID
来源：http://hz.snrcjt.cn/gtifxaujoz.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.pycfn.com/gtcqnjztyq.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.cheryme.top/gtnfrdtghu.html

[Q13] 忽略重复插入
来源：http://hz.jianghu66.top/gttsaxzedb.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.aibaodan.cn/gthkbyqjnl.html

[Q14] 存在则更新（upsert）
来源：http://hz.hywenlv.cn/gtqztdgukz.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.chenzaomai.com/gtmojzsawk.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.ppjwa.cn/gtccxthwjq.html

[Q15] 查询全部
来源：http://hz.hywenlv.cn/gtcljteera.html

SELECT * FROM users;
来源：http://hz.ppjwa.cn/gtwigabulr.html

[Q16] 查询指定列
来源：http://hz.tianlin.xyz/gtuobdowwt.html

SELECT id, name FROM users;
来源：http://hz.xinyue.icu/gtgrqqjxwf.html

[Q17] 条件查询
来源：http://hz.zhaomingkeji.xyz/gtbiniaprs.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.sufxvd.cn/gtcrarpofd.html

[Q18] 模糊匹配
来源：http://hz.havefunace.top/gtowdbyaye.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.hongshengwenyu.top/gtqztivylq.html

[Q19] 范围查询
来源：http://hz.sysykeji.top/gtvgsxozgj.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.xuetiantiany.cn/gtjmonhtqy.html

[Q20] IN 列表
来源：http://hz.redwolf501.top/gtjlzahqov.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.pycfn.com/gtchvllyhz.html

[Q21] 空值判断
来源：http://hz.yanxiufei.cn/gtruebhqbk.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.aibaodan.cn/gtkbgmovyq.html

[Q22] 排序
来源：http://hz.yongpay.top/gtfmzebglo.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.yonumen.top/gtyfwfkgip.html

[Q23] 分页
来源：http://hz.kuanghao11.cn/gtasexvonb.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.kuanghao11.cn/gtpyhlfqly.html

[Q24] 去重
来源：http://hz.zhongyouzk.top/gtkbytbokp.html

SELECT DISTINCT city FROM users;
来源：http://hz.pengpengdd.cyou/gtouxykhqe.html

[Q25] 只取前 N 条
来源：http://hz.cheryme.top/gtxnhitfjd.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.dashuyun.cn/gtienkspat.html

[Q26] 计数
来源：http://hz.jiagoushi.top/gtsekjrlcw.html

SELECT COUNT(*) FROM users;
来源：http://hz.tian-w.cn/gtagylccke.html

[Q27] 条件计数
来源：http://hz.0kj1m.cn/gtzqifyxwc.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.yj20258888.top/gtvlbkxmkh.html

[Q28] 求和与平均
来源：http://hz.jinghuilouyu.cn/gtjnfphcng.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.nanxuanxn.top/gtuelphzxy.html

[Q29] 最大最小值
来源：http://hz.pengpengdd.cyou/gteovdgjfg.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.gogol.net.cn/gthilgitoc.html

[Q30] 分组统计
来源：http://hz.cqqwz.cn/gtcvykfdwk.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.ydjk.org.cn/gtrlzjrnca.html

[Q31] 分组后过滤
来源：http://hz.guowangkeji.top/gtmwptegyg.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.hnqzz.top/gtnjuvthhj.html

[Q32] 分组拼接字符串
来源：http://hz.xinyue.icu/gtlxapebaf.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.yj202588.top/gtzafwxeiy.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.bjfxy.top/gthadnrajv.html

[Q33] 多列分组
来源：http://hz.ydjk.org.cn/gtgxiwxiba.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.shanyushiyangkeji.top/gtgnjxuiyv.html

[Q34] 每组取第一条
来源：http://hz.shangyingyoupin.top/gtzbrfnsxl.html

SELECT * FROM (
来源：http://hz.tianlin.xyz/gtpncbibcg.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.mhx1999.top/gtysmeolzs.html

) t WHERE rn = 1;
来源：http://hz.daria6918.cn/gtqusbkkrz.html

[Q35] 内连接
来源：http://hz.sweek.top/gtcoqujxme.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.nwbrower.top/gtemdndsyz.html

[Q36] 左连接
来源：http://hz.fengsongda.top/gthwawdvac.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.wangshuangyany.cn/gtjojdqfcl.html

[Q37] 右连接
来源：http://hz.jyoumei.cn/gtjjygyauo.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.nanxinkj.top/gtzmgyxddu.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.chenjidiqi.icu/gtyuydybpu.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.chenlongwang.top/gtorkjndlp.html

[Q39] 自连接（查上下级）
来源：http://hz.cdnleiting.top/gtfqxwpjhe.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.jqgufenzy.top/gtdczhqliu.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.yongpay.top/gtewgpfrze.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.jinqigufen.top/gtlwrpwmvi.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.fengsongda.top/gtojcjdxfu.html

[Q41] 多表连接
来源：http://hz.tian-w.cn/gtpofairje.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.sysykeji.top/gtzbdtumii.html

JOIN users u ON u.id = o.user_id
来源：http://hz.redwolf501.top/gtookmldjp.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.bjfxy.top/gtlvtxvqoo.html

[Q42] 连接条件附加过滤
来源：http://hz.zhiwuduotai.top/gtmxgaistb.html

SELECT u.name, o.amount FROM users u
来源：http://hz.sweek.top/gtboqxwlvh.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.aibaodan.cn/gtntazypvo.html

[Q43] 标量子查询
来源：http://hz.tianlin.xyz/gtsbijuxgd.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.yvedp.cn/gtxjeonyiw.html

[Q44] IN 子查询
来源：http://hz.sufxvd.cn/gtwygndujs.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.dashuyun.cn/gtxpgdnhog.html

[Q45] EXISTS 判断存在
来源：http://hz.shanyushiyangtech.top/gtxftrquxr.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.hnxiangtu.top/gtnqglssyi.html


<!-- 参考信息 -->