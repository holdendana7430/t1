代发 wailian999

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.daria6918.cn/gttejiwnbn.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.hnxiangtu.top/gttfbstkho.html

TS:   // 手写 Map<string, number>
来源：http://hz.zhaomingkeji.xyz/gtantefzni.html

Java: // 手写 HashMap
来源：http://hz.zhiwuduotai.top/gtcwqpslue.html

Go:   // 手写 map[int]int
来源：http://hz.shzxlz.cn/gtrgykqezz.html

Ruby: // 手写 Hash
来源：http://hz.tian-w.cn/gtakshathy.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.jyoumei.cn/gtygegpwwc.html

[N08] 生成全排列
来源：http://hz.tianlin.xyz/gtywtxovpk.html

Py:   itertools.permutations(arr)
来源：http://hz.dashuyun.cn/gtgldcqyxw.html

PHP:  // 手写递归交换
来源：http://hz.wangshuangyany.cn/gtlohzulwj.html

JS:   // 手写回溯递归
来源：http://hz.yueranfly.top/gtxiftsyfc.html

TS:   // 手写回溯递归
来源：http://hz.gaohongyu789.top/gtzpapetnf.html

Java: // 手写回溯递归
来源：http://hz.ppjwa.cn/gtbuhlhboa.html

Go:   // 手写回溯递归
来源：http://hz.daria6918.cn/gtlgxkznrp.html

Ruby: arr.permutation.to_a
来源：http://hz.hywenlv.cn/gtagmqwpbd.html

C#:   // 手写回溯递归
来源：http://hz.zhengqikj.top/gtzsoirxpc.html

[N09] 栈与队列
来源：http://hz.zdqjudy.top/gtiywfpjpo.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.xziqi.cn/gtfcnwosal.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.andypj.xyz/gtxffuoywd.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.jlsjyb.cn/gtnwjazrtk.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.jqgufenzy.top/gtapndgcpa.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.hysaishi.cn/gtsarzeghf.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.0kj1m.cn/gtejkmmnsa.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.wangshuangyany.cn/gtibrnwevr.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.meibo888.top/gtntwglevh.html

[N10] 链表节点定义
来源：http://hz.cucudq.cn/gtwjxtkfdt.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.shuidangran.top/gtkrwwgxkl.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.cheryme.top/gtbachfikv.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.tian-w.cn/gtsgowrpvg.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.jqgfzy.top/gtyyuvkvjy.html

Java: class Node { int v; Node next; }
来源：http://hz.yj20258.top/gtpfrylubj.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.cheryme.top/gtjhbnxevv.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.smart0.xyz/gtlfhimudi.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.aizwys.cn/gtdxicobop.html

[N11] 二叉树中序遍历
来源：http://hz.aizwys.cn/gtvntmumjp.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.tian-w.cn/gtabxcigtu.html

PHP:  // 手写递归函数
来源：http://hz.yvedp.cn/gtslssuoln.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.0kj1m.cn/gtlncaixgo.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.yj20258888.top/gtducxunws.html

Java: // 手写递归
来源：http://hz.quarkkingdee.top/gtplqdybae.html

Go:   // 手写递归
来源：http://hz.vqdsnc.cn/gtkdlycytm.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.jinqigufen.top/gtbukixpob.html

C#:   // 手写递归
来源：http://hz.zhengqikj.top/gtkjyraofz.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.52xcode.cn/gtltcmpghy.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.haohaochexian.top/gtvexpakdk.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.yangfankeji.com/gtndkhwfas.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.fengsongda.top/gtkfxfszkx.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.xylfe.cn/gttwhcczpp.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.tianlin.xyz/gtmiybtnno.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.ydjk.org.cn/gtfkohnfmg.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.zycfv.cn/gtzndxomda.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.shanyushiyangkeji.top/gteyjtyatv.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gtupoallts.html

O. 并发与异步
来源：http://hz.guowangkeji.top/gtgktbsven.html

================================================================================
来源：http://hz.0kj1m.cn/gtpwcahnhh.html

[O01] 启动一个线程
来源：http://hz.yueranfly.top/gtukxifszz.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.shanyushiyangtech.top/gtqjpnlhcz.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.chenjidiqi.icu/gtzpruopfb.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.cashguo.top/gtwjfjwlba.html

TS:   // 同 JS
来源：http://hz.gogol.net.cn/gttewxkypf.html

Java: new Thread(() -> f()).start()
来源：http://hz.316326.xyz/gtjeweffag.html

Go:   go f()
来源：http://hz.mhx1999.top/gtiyydxctd.html

Ruby: Thread.new { f }
来源：http://hz.zycfv.cn/gtcwspuvnz.html

C#:   Task.Run(() => F());
来源：http://hz.redwolf501.top/gtxuzzcfyg.html

[O02] 使用线程池
来源：http://hz.yangfankeji.com/gtnjvtcwsx.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.yj202588.top/gtmjjtddcg.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.yonumen.top/gtjqyqmmob.html

JS:   // worker_threads 线程池
来源：http://hz.shuidangran.top/gtvdvvjpbh.html

TS:   // worker_threads 线程池
来源：http://hz.ehwqpu.com/gtbybqoqip.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.ydjk.org.cn/gtmkrfcotf.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.316326.xyz/gtctzvbjlq.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.yongpay.top/gtrcryuedg.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.kuanghao11.cn/gtngdslung.html

[O03] 加锁保护共享数据
来源：http://hz.jqgufenzy.top/gtbqlwybbz.html

Py:   with lock: shared += 1
来源：http://hz.yonumen.top/gtbuckituq.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.ydjk.org.cn/gtycrxcjyh.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.zhixingplan.top/gtbdqtvetr.html

TS:   // 同 JS
来源：http://hz.feifeiyinyue.top/gtakdzqkqp.html

Java: synchronized (this) { shared++; }
来源：http://hz.xuetiantiany.cn/gtajkesuvr.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.xziqi.cn/gteiavllai.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.yuanzhike.top/gtvtwvknyn.html

C#:   lock (gate) { shared++; }
来源：http://hz.xinyue.icu/gtdicxoqeu.html

[O04] 定义异步函数并等待
来源：http://hz.zhiwuduotai.top/gtswynpfte.html

Py:   async def f():⏎    await g()
来源：http://hz.9152youxi.cn/gthfusklfc.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.yj20258888.top/gtndavolql.html

JS:   async function f() { await g(); }
来源：http://hz.feifeiyinyue.top/gtadjucgzi.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.wangdashe.top/gtoqsqcjqy.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.yuxming.cn/gtrscbclbz.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.ywan-chungtsiang.top/gtfdfppgte.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.daria6918.cn/gtwyqzxyhb.html

C#:   async Task F() { await G(); }
来源：http://hz.yuxming.cn/gtkuybftps.html

[O05] 并发执行并等待全部完成
来源：http://hz.gzhubu.top/gtwizhrtbt.html

Py:   asyncio.gather(*tasks)
来源：http://hz.aizwys.cn/gtgpxvtngb.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.9152youxi.cn/gtdnpcfzpl.html

JS:   await Promise.all(tasks)
来源：http://hz.bjfxy.top/gthxqkjwuq.html

TS:   await Promise.all(tasks)
来源：http://hz.redwolf501.top/gtmejbeumw.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.svipenyu.cn/gtvhjnfccp.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.meibo888.top/gtatdmvoys.html

Ruby: threads.map(&:join)
来源：http://hz.hysaishi.cn/gtesgzpfkw.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.guannengcc.top/gtcuavatas.html

[O06] 使用进程池
来源：http://hz.cashguo.top/gtlimnqyfg.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.zhoulong.xyz/gthqardkxn.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.wangdashe.top/gthakeewmz.html

JS:   // child_process / cluster 模块
来源：http://hz.wangdashe.top/gtvmnfarzr.html

TS:   // child_process / cluster 模块
来源：http://hz.jianghu66.top/gtfthuuoih.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.pycfn.com/gttjaifvcq.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.andypj.xyz/gthstmbjxh.html

Ruby: // fork 块
来源：http://hz.andypj.xyz/gtbjnlkobj.html

C#:   Parallel.For
来源：http://hz.wangdashe.top/gtscqueohc.html

================================================================================
来源：http://hz.gogol.net.cn/gtaqigefdx.html

P. 常用工具函数
来源：http://hz.zhongyouzk.top/gtjpeyisrx.html

================================================================================
来源：http://hz.aizwys.cn/gtcxuwjmzc.html

[P01] 生成 UUID
来源：http://hz.andypj.xyz/gtdurnudcb.html

Py:   str(uuid.uuid4())
来源：http://hz.tian-w.cn/gtiziuwbsi.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.0kj1m.cn/gtkxxfdqbp.html

JS:   crypto.randomUUID()
来源：http://hz.sweek.top/gtygonldpy.html

TS:   crypto.randomUUID()
来源：http://hz.zhiwuduotai.top/gtfmjurdon.html

Java: UUID.randomUUID().toString()
来源：http://hz.gzhubu.top/gthgwlpael.html

Go:   // 用 github.com/google/uuid
来源：http://hz.yj20258888.top/gtfnadczjv.html

Ruby: SecureRandom.uuid
来源：http://hz.xingfuxueyuan.xyz/gtyerujplc.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.jianghu66.top/gtdditmzyz.html

[P02] MD5 / SHA256 摘要
来源：http://hz.9152youxi.cn/gtqpgfcfvd.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.yanxiufei.cn/gtwngvxaad.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.svipenyu.cn/gtvryredqm.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.wangshuangyany.cn/gtlthqwzub.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.jlsjyb.cn/gtntixvbce.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.dianchejie.cn/gtfrbvjqse.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.jyoumei.cn/gtjmumivkk.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.tanke756.top/gtgkopdbmc.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.aibaodan.cn/gtdqaxwnft.html

[P03] 生成短随机字符串
来源：http://hz.daria6918.cn/gtjqgspthj.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.hysaishi.cn/gtffbryihw.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.haohaochexian.top/gtxwnbngez.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.yueranfly.top/gtdjxvuftz.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.tanke756.top/gtzmwkitzk.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.guannengcc.top/gtleahxizq.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.wangdashe.top/gtnjklwtyv.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.zhixingplan.top/gtwpwwswng.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.havefunace.top/gtnejmrbny.html

[P04] 求长度
来源：http://hz.shuidangran.top/gtuxelplyu.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.zycfv.cn/gtvvenylmv.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.chenlongwang.top/gtovcbacwx.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.jinqigufen.top/gtlkfovvyo.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.zhoulong.xyz/gttedxjwfm.html

Java: list.size();  map.size();  s.length()
来源：http://hz.0kj1m.cn/gtbiaksaul.html

Go:   len(arr);  len(m)
来源：http://hz.zhoulong.xyz/gtjqlotvmz.html

Ruby: x.length;  x.size
来源：http://hz.dianchejie.cn/gtkdqlhxre.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.gaohongyu789.top/gtwedjwzoe.html

[P05] 判断两个对象内容是否相等
来源：http://hz.daxiang520.top/gtjpupldhb.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.ywan-chungtsiang.top/gtwckacjib.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.meibo888.top/gtxjoeymmf.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.cucudq.cn/gtlttwopdk.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.ppjwa.cn/gtinduqawf.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.shanyushiyangkeji.top/gtvpefusah.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.cdnleiting.top/gtxfynlnzs.html

Ruby: a == b
来源：http://hz.meibo888.top/gtxultbudd.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.yvedp.cn/gtuajxdagy.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.andypj.xyz/gtfzajggpw.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.52xcode.cn/gtbtakzybe.html

PHP:  if (empty($x)) {}
来源：http://hz.nanxinkj.top/gtswkqhddx.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.yj20258888.top/gtutdvirjl.html

TS:   if (x == null) {}
来源：http://hz.c1oappe.top/gtedrptjlm.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.zhengqikj.top/gtrogttegb.html

Go:   if x == nil {}
来源：http://hz.xylfe.cn/gtckoqoequ.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.shzxlz.cn/gtctwcoztj.html

C#:   if (x is null) {}
来源：http://hz.chenzaomai.com/gtzqlrppfw.html

[P07] 防抖与节流
来源：http://hz.hnqzz.top/gtomubttat.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.ybcxt.top/gtwsakyjhh.html

PHP:  // 手写时间戳比较
来源：http://hz.birdmap.top/gtdhkqfkpt.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.havefunace.top/gtywnzkmnm.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.jinghuilouyu.cn/gtnvnhbkyi.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.yvedp.cn/gtwyvqmgyf.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.jqgfzy.top/gtyivkkurh.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.cqqwz.cn/gtyixrqzan.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.aizwys.cn/gteeffiret.html

[P08] 处理浮点精度问题
来源：http://hz.daxiang520.top/gtzphujupv.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.zhijiandao.cn/gtyofdinkb.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.jinghuilouyu.cn/gtdksdmyia.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.chenjidiqi.icu/gthhznhjkl.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.kuanghao11.cn/gtpcdaqcox.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.birdmap.top/gtvztlatvo.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.vqdsnc.cn/gtrhivgtjb.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.cdnleiting.top/gtuaccacdm.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.fzhhl.top/gttqltwmjf.html

================================================================================
来源：http://hz.jyoumei.cn/gtelojwvzt.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.mhx1999.top/gtimddlggb.html

================================================================================
来源：http://hz.xuetiantiany.cn/gtwcdzaygu.html

[Q01] 创建表
来源：http://hz.sweek.top/gtvijnnfny.html

CREATE TABLE users (
来源：http://hz.ywan-chungtsiang.top/gtojlisjbk.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.dianchejie.cn/gtdcswambv.html

name VARCHAR(50) NOT NULL,
来源：http://hz.xziqi.cn/gtacqauapo.html

email VARCHAR(100) UNIQUE,
来源：http://hz.vqdsnc.cn/gtxunenlky.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.gaohongyu789.top/gtvqqyhxfp.html

);
来源：http://hz.vqdsnc.cn/gtkpugrjtg.html

[Q02] 创建带外键的表
来源：http://hz.smart0.xyz/gtdnhngjmd.html

CREATE TABLE orders (
来源：http://hz.9152youxi.cn/gtudxabczi.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.xingfuxueyuan.xyz/gtudvepcid.html

user_id INT NOT NULL,
来源：http://hz.52xcode.cn/gtjredqbdu.html

amount DECIMAL(10, 2),
来源：http://hz.daria6918.cn/gtghyhugwy.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.yanxiufei.cn/gthgnnoiwo.html

);
来源：http://hz.fengsongda.top/gtganqaxii.html

[Q03] 增加列
来源：http://hz.sxryk.cn/gtusnhkjyj.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.chenlongwang.top/gtnziibplk.html

[Q04] 修改列类型
来源：http://hz.cashguo.top/gttshhecou.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.yongpay.top/gtnokjgekt.html

[Q05] 重命名列
来源：http://hz.ydjk.org.cn/gtasvmxkcv.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.nanxinkj.top/gtmlhipyke.html

[Q06] 删除列
来源：http://hz.yangfankeji.com/gtehhrjkbl.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.zdqjudy.top/gtvluzowbp.html

[Q07] 删除表
来源：http://hz.sysykeji.top/gtxzuychxs.html

DROP TABLE IF EXISTS orders;
来源：http://hz.jqgufenzy.top/gtggwggnvk.html

[Q08] 创建普通索引
来源：http://hz.yueranfly.top/gttzwxzsog.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.shanyushiyangtech.top/gtuteuuwdp.html

[Q09] 创建唯一索引
来源：http://hz.xuanzx.com/gtjcttjgrz.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.zhengqikj.top/gtjmytfxpt.html

[Q10] 插入单行
来源：http://hz.dianchejie.cn/gtmxwuoqkk.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.zhengqikj.top/gtikgxvjwx.html

[Q11] 一次插入多行
来源：http://hz.yvedp.cn/gtwkucsbdq.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.fzhhl.top/gtvbkrucll.html

[Q12] 插入后取自增 ID
来源：http://hz.yanxiufei.cn/gtqhiyysry.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.cdnleiting.top/gtkslupatt.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.yvedp.cn/gtveojdxdx.html

[Q13] 忽略重复插入
来源：http://hz.chenzaomai.com/gtlhsejwux.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.yj20258888.top/gtppdssvxy.html

[Q14] 存在则更新（upsert）
来源：http://hz.shuidangran.top/gtzozksjgw.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.quarkkingdee.top/gtcbeifhtq.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.0kj1m.cn/gtlhgxpvvd.html

[Q15] 查询全部
来源：http://hz.haohaochexian.top/gtfkhaolcr.html

SELECT * FROM users;
来源：http://hz.sxryk.cn/gtjtqkskps.html

[Q16] 查询指定列
来源：http://hz.hfpthk.cn/gtbiqjxxmk.html

SELECT id, name FROM users;
来源：http://hz.redwolf501.top/gtjfreicbu.html

[Q17] 条件查询
来源：http://hz.ydzc1.top/gtifgpztas.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.havefunace.top/gticzslwby.html

[Q18] 模糊匹配
来源：http://hz.hongshengwenyu.top/gtjfsefqzk.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.snrcjt.cn/gtmqvqzcwy.html

[Q19] 范围查询
来源：http://hz.kuanghao11.cn/gtgjnydhgl.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.zhengqikj.top/gtokvxjldr.html

[Q20] IN 列表
来源：http://hz.quarkkingdee.top/gtleieslkl.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.dianchejie.cn/gtojllsdke.html

[Q21] 空值判断
来源：http://hz.ybcxt.top/gtzxgequjj.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.mhx1999.top/gtvsduixzh.html

[Q22] 排序
来源：http://hz.zhaomingkeji.xyz/gtgnurzift.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.yj202588.top/gttteifabs.html

[Q23] 分页
来源：http://hz.chenzaomai.com/gtsbtprkyu.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.shuidangran.top/gtzkdqvqvq.html

[Q24] 去重
来源：http://hz.snrcjt.cn/gtsfzjlocy.html

SELECT DISTINCT city FROM users;
来源：http://hz.chenjidiqi.icu/gtnlfvuipj.html

[Q25] 只取前 N 条
来源：http://hz.pengpengdd.cyou/gtrfqubbju.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.jqgufenzy.top/gttbobcfhs.html

[Q26] 计数
来源：http://hz.316326.xyz/gtfuypgdbr.html

SELECT COUNT(*) FROM users;
来源：http://hz.hongshengwenyu.top/gtujkewykf.html

[Q27] 条件计数
来源：http://hz.nwbrower.top/gtwiumxpar.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.gzhubu.top/gteklliroq.html

[Q28] 求和与平均
来源：http://hz.xylfe.cn/gtzbggiqnj.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.havefunace.top/gtjfohweym.html

[Q29] 最大最小值
来源：http://hz.shangyingyoupin.top/gtjjlypbjp.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.andypj.xyz/gtpeskkoii.html

[Q30] 分组统计
来源：http://hz.hammf.cn/gtranrmtig.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.yj202588.top/gtjhysotib.html

[Q31] 分组后过滤
来源：http://hz.nwbrower.top/gtekqjnagj.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.316326.xyz/gtxqkisyqy.html

[Q32] 分组拼接字符串
来源：http://hz.tian-w.cn/gtekwwfkfh.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.shangyingyoupin.top/gtrjeodoum.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.ybcxt.top/gttrmhssoz.html

[Q33] 多列分组
来源：http://hz.tian-w.cn/gtfijxykls.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.0kj1m.cn/gtdbifbfxl.html

[Q34] 每组取第一条
来源：http://hz.yj202588.top/gttltqbpxb.html

SELECT * FROM (
来源：http://hz.yj20258.top/gtxipfhhmq.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.ydzc1.top/gtnrvyceso.html

) t WHERE rn = 1;
来源：http://hz.daxiang520.top/gtreazyqnh.html

[Q35] 内连接
来源：http://hz.sysykeji.top/gtcvawcprs.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.yj20258.top/gttdbhmbxy.html

[Q36] 左连接
来源：http://hz.jiagoushi.top/gttqyoywoh.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.zhoulong.xyz/gtqnevjpsg.html

[Q37] 右连接
来源：http://hz.zhongyouzk.top/gtucnesrzj.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.jianghu66.top/gtzmnytclj.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.ybcxt.top/gtguakzjhe.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.nanxuanxn.top/gtgdcvqcbr.html

[Q39] 自连接（查上下级）
来源：http://hz.meibo888.top/gtkbgnpjtx.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.wangshuangyany.cn/gtswbynczs.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.shanyushiyangtech.top/gtseourvzi.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.jqgfzy.top/gtslzfdcra.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.shangyingyoupin.top/gthkfotclw.html

[Q41] 多表连接
来源：http://hz.zhixingplan.top/gtkrpoyvqa.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.iojbl.cn/gtmcozwkbf.html

JOIN users u ON u.id = o.user_id
来源：http://hz.yuxming.cn/gtexhwafzt.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.chenjidiqi.icu/gtsjypwmpe.html

[Q42] 连接条件附加过滤
来源：http://hz.yuxming.cn/gtihmgiyrj.html

SELECT u.name, o.amount FROM users u
来源：http://hz.sysykeji.top/gtebodxylz.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.zhiwuduotai.top/gtsxicvzxr.html

[Q43] 标量子查询
来源：http://hz.vqdsnc.cn/gthblcrhwm.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.wangshuangyany.cn/gtovjdidzd.html

[Q44] IN 子查询
来源：http://hz.jinyuanbaomall.cn/gtiaioaqvw.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.meibo888.top/gtrxqskxge.html

[Q45] EXISTS 判断存在
来源：http://hz.nwbrower.top/gtlqodlaef.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.chenjidiqi.icu/gtsejoliur.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.yuxming.cn/gtdpfhccsu.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.xingfuxueyuan.xyz/gtckmthzzc.html

[Q47] 与平均值比较
来源：http://hz.jianghu66.top/gtcsyhvioa.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.ivvv.top/gtdabsohko.html


<!-- 参考信息 -->