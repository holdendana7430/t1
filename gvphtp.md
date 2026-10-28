代发 wailian999

Ruby: s == s.reverse
来源：http://hz.cdnleiting.top/gtbkvuenxu.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.guannengcc.top/gtwavmvyti.html

[N07] 两数之和（返回下标）
来源：http://hz.sweek.top/gtqhmeedbo.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.ppjwa.cn/gtnduzmrop.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.cashguo.top/gtvtndgxkx.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.jlsjyb.cn/gtejhmxzbs.html

TS:   // 手写 Map<string, number>
来源：http://hz.tanke756.top/gtojzhtymv.html

Java: // 手写 HashMap
来源：http://hz.redwolf501.top/gtsyzwvtik.html

Go:   // 手写 map[int]int
来源：http://hz.jinqigfzy.top/gtlftodruk.html

Ruby: // 手写 Hash
来源：http://hz.ppjwa.cn/gtdpzlakdt.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.9152youxi.cn/gtgyxltaem.html

[N08] 生成全排列
来源：http://hz.hysaishi.cn/gtnwnhzmpr.html

Py:   itertools.permutations(arr)
来源：http://hz.jiagoushi.top/gtjzunjjpg.html

PHP:  // 手写递归交换
来源：http://hz.haohaochexian.top/gtdxsbfwva.html

JS:   // 手写回溯递归
来源：http://hz.jiagoushi.top/gtowmatkmz.html

TS:   // 手写回溯递归
来源：http://hz.gogol.net.cn/gtysqctycp.html

Java: // 手写回溯递归
来源：http://hz.yvedp.cn/gtfybbymor.html

Go:   // 手写回溯递归
来源：http://hz.zhixingplan.top/gtfulajbsw.html

Ruby: arr.permutation.to_a
来源：http://hz.tanke756.top/gtlmjeqmdc.html

C#:   // 手写回溯递归
来源：http://hz.yuanzhike.top/gtsmyccvdv.html

[N09] 栈与队列
来源：http://hz.jinqigfzy.top/gtpjchypyl.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.yvedp.cn/gtnsqjggpy.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.c1oappe.top/gtyxuqsgtz.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.yuxming.cn/gttrfajqdy.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.jianghu66.top/gtxguthscm.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.yonumen.top/gteslzgxgt.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.gzhubu.top/gtujrvzybl.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.hongshengwenyu.top/gtavnlwkdp.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.andypj.xyz/gtthnzlozk.html

[N10] 链表节点定义
来源：http://hz.sysykeji.top/gtnyvozrms.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.dashuyun.cn/gtvjoljarb.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.birdmap.top/gtmimndiby.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.jianghu66.top/gtoxmcuczy.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.tanke756.top/gtwhynuxea.html

Java: class Node { int v; Node next; }
来源：http://hz.yj202588.top/gtflsvnduw.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.pycfn.com/gtoqfzoban.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.daxiang520.top/gtfhtoaaem.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.wangdashe.top/gtjwvaxshw.html

[N11] 二叉树中序遍历
来源：http://hz.yuxming.cn/gtwjacdzmk.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.hysaishi.cn/gtrtltiksb.html

PHP:  // 手写递归函数
来源：http://hz.jinqigfzy.top/gtmcwjqgcy.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.ywan-chungtsiang.top/gtdbwyuykk.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.gotoacloud.top/gtovaoavmn.html

Java: // 手写递归
来源：http://hz.sysykeji.top/gtkcvrcqoo.html

Go:   // 手写递归
来源：http://hz.yj20258888.top/gtxsmtsasd.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.andypj.xyz/gtzdkxvhbo.html

C#:   // 手写递归
来源：http://hz.hfpthk.cn/gtmyhnqmjo.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.jiagoushi.top/gtogafucur.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.zhixingplan.top/gtdhaxwhha.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.0kj1m.cn/gtaaobczzm.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.jqgufenzy.top/gtwihxcdxt.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.mhx1999.top/gtobtxkqnq.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.zhaomingkeji.xyz/gtsedodqdn.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.tianlin.xyz/gtqclpzzbx.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.52xcode.cn/gtokakpgjr.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.yj202588.top/gthwxnewvi.html

================================================================================
来源：http://hz.hywenlv.cn/gtfqsuieqm.html

O. 并发与异步
来源：http://hz.zhengqikj.top/gtueknbusd.html

================================================================================
来源：http://hz.vqdsnc.cn/gtuhcvdvhw.html

[O01] 启动一个线程
来源：http://hz.jinqigufen.top/gtluyapntb.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.xziqi.cn/gtpdeomplu.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.mhx1999.top/gtzhesljqn.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.hammf.cn/gtebbtiibm.html

TS:   // 同 JS
来源：http://hz.yueranfly.top/gtjgrlxpfg.html

Java: new Thread(() -> f()).start()
来源：http://hz.birdmap.top/gtzqfdjamn.html

Go:   go f()
来源：http://hz.yvedp.cn/gtfwwuhnxc.html

Ruby: Thread.new { f }
来源：http://hz.yueranfly.top/gtsgbcdnju.html

C#:   Task.Run(() => F());
来源：http://hz.aibaodan.cn/gtysoaqknf.html

[O02] 使用线程池
来源：http://hz.yj20258.top/gtqwjxntdd.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.hnxiangtu.top/gtholugona.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.redwolf501.top/gtfwupspiz.html

JS:   // worker_threads 线程池
来源：http://hz.ivvv.top/gtturphamx.html

TS:   // worker_threads 线程池
来源：http://hz.nanxuanxn.top/gtdpnmhnxp.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.ivvv.top/gtylunghxc.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.vqdsnc.cn/gtogdamndn.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.sxryk.cn/gtvyowrynr.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.zhaomingkeji.xyz/gtzcdbehah.html

[O03] 加锁保护共享数据
来源：http://hz.yj202588.top/gtjhpmjcpj.html

Py:   with lock: shared += 1
来源：http://hz.hammf.cn/gtjnznvznj.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.quarkkingdee.top/gtpnbcwsxp.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.sxryk.cn/gtljkrvzhk.html

TS:   // 同 JS
来源：http://hz.pengpengdd.cyou/gtyrzwdfvr.html

Java: synchronized (this) { shared++; }
来源：http://hz.ydzc1.top/gtojrmzbxz.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.gotoacloud.top/gtvvhliffr.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.zhiwuduotai.top/gtcdwpjebi.html

C#:   lock (gate) { shared++; }
来源：http://hz.yongpay.top/gtctoddxjw.html

[O04] 定义异步函数并等待
来源：http://hz.cashguo.top/gtcjzztjid.html

Py:   async def f():⏎    await g()
来源：http://hz.pycfn.com/gtiwxoqjew.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.yanxiufei.cn/gtlrvehfdv.html

JS:   async function f() { await g(); }
来源：http://hz.shangyingyoupin.top/gttwpzkthe.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.jiagoushi.top/gthnqzfsur.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.hnqzz.top/gtwjzpzlrs.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.daxiang520.top/gtkroczbcy.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.jinyuanbaomall.cn/gtjbekliqj.html

C#:   async Task F() { await G(); }
来源：http://hz.hammf.cn/gthdxodlft.html

[O05] 并发执行并等待全部完成
来源：http://hz.hywenlv.cn/gtqyrithgt.html

Py:   asyncio.gather(*tasks)
来源：http://hz.jinqigfzy.top/gtbsgdfcua.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.yonumen.top/gtvrvcgnqw.html

JS:   await Promise.all(tasks)
来源：http://hz.pycfn.com/gtqhenbffi.html

TS:   await Promise.all(tasks)
来源：http://hz.cheryme.top/gtgxtzklrw.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.fengsongda.top/gtwbpjwqoi.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.zhengqikj.top/gtuwuravmo.html

Ruby: threads.map(&:join)
来源：http://hz.yueranfly.top/gtlheugozi.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.wangshuangyany.cn/gtqcddvhfv.html

[O06] 使用进程池
来源：http://hz.xinyue.icu/gtldkiidyt.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.hnxiangtu.top/gtofuyawcc.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.havefunace.top/gtwmwbbxli.html

JS:   // child_process / cluster 模块
来源：http://hz.zhengqikj.top/gtwrboxayj.html

TS:   // child_process / cluster 模块
来源：http://hz.cqqwz.cn/gtqdjzttqc.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.52xcode.cn/gttpibhuek.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.pycfn.com/gtdhmlxujw.html

Ruby: // fork 块
来源：http://hz.hfpthk.cn/gtboipzevl.html

C#:   Parallel.For
来源：http://hz.shzxlz.cn/gtwqtnwffk.html

================================================================================
来源：http://hz.zhongyouzk.top/gtiubnrpti.html

P. 常用工具函数
来源：http://hz.zhengqikj.top/gtqdbbvjtf.html

================================================================================
来源：http://hz.yueranfly.top/gtgyldutfo.html

[P01] 生成 UUID
来源：http://hz.wangshuangyany.cn/gtvwcpbegg.html

Py:   str(uuid.uuid4())
来源：http://hz.quarkkingdee.top/gtrzvzksqe.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.sufxvd.cn/gtqzsjvuni.html

JS:   crypto.randomUUID()
来源：http://hz.zhiwuduotai.top/gtursqtahv.html

TS:   crypto.randomUUID()
来源：http://hz.chenlongwang.top/gtxragsled.html

Java: UUID.randomUUID().toString()
来源：http://hz.xuanzx.com/gtndpocrao.html

Go:   // 用 github.com/google/uuid
来源：http://hz.birdmap.top/gtdmxjvnii.html

Ruby: SecureRandom.uuid
来源：http://hz.jiagoushi.top/gtbtrabkij.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.jinghuilouyu.cn/gtugfxctmv.html

[P02] MD5 / SHA256 摘要
来源：http://hz.zdqjudy.top/gtlnvzaiuo.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.mhx1999.top/gtjsbxukmq.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.birdmap.top/gtgngsgppz.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.9152youxi.cn/gttwlhvjnf.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.cashguo.top/gtohncwzut.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.xuetiantiany.cn/gtmdboggna.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.gzhubu.top/gtkenelbgq.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.yuanzhike.top/gtbbfzssdk.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.yj202588.top/gtohtmhyuv.html

[P03] 生成短随机字符串
来源：http://hz.aibaodan.cn/gttnfmfqqr.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.chenjidiqi.icu/gtzoxpepjt.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.9152youxi.cn/gtiwamkyrh.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.hywenlv.cn/gtevhqspno.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.chenzaomai.com/gtachfrrge.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.nanxinkj.top/gtgxxxvumw.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.shanyushiyangkeji.top/gtqdsmbuww.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.hammf.cn/gtwepsutgn.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.birdmap.top/gtqmgakpwc.html

[P04] 求长度
来源：http://hz.zhaomingkeji.xyz/gtcctuiilb.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.jlsjyb.cn/gtremlfzyr.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.jyoumei.cn/gtnpfeokfb.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.chenzaomai.com/gtxmkqofjo.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.pengpengdd.cyou/gtgqygzqaw.html

Java: list.size();  map.size();  s.length()
来源：http://hz.dashuyun.cn/gtfqiyosjb.html

Go:   len(arr);  len(m)
来源：http://hz.xylfe.cn/gtgergpupa.html

Ruby: x.length;  x.size
来源：http://hz.jqgufenzy.top/gtgfsbzqxg.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.redwolf501.top/gtzsjfusad.html

[P05] 判断两个对象内容是否相等
来源：http://hz.xingfuxueyuan.xyz/gtlqttikse.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.hammf.cn/gtkwjhdxnw.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.xuanzx.com/gtzqfjjrtc.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.chenjidiqi.icu/gtstndyzdz.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.zhijiandao.cn/gtmefpxpnr.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.jianghu66.top/gtlocdseoz.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.redwolf501.top/gtwmvahmnv.html

Ruby: a == b
来源：http://hz.yvedp.cn/gtshzpxufk.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.aibaodan.cn/gtcpqzcumo.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.jqgufenzy.top/gtdfjamkep.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.fzhhl.top/gtgxknkegv.html

PHP:  if (empty($x)) {}
来源：http://hz.xuanzx.com/gtuftinzqn.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.daxiang520.top/gtbkzzrtku.html

TS:   if (x == null) {}
来源：http://hz.zhengqikj.top/gtrizgkxks.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.hfpthk.cn/gtidqluoxv.html

Go:   if x == nil {}
来源：http://hz.yongpay.top/gttldilmsl.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.ydjk.org.cn/gtuhmumfba.html

C#:   if (x is null) {}
来源：http://hz.quarkkingdee.top/gtyoinnhrm.html

[P07] 防抖与节流
来源：http://hz.yueranfly.top/gtkxsugwqq.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.chenzaomai.com/gttkjqenkc.html

PHP:  // 手写时间戳比较
来源：http://hz.feifeiyinyue.top/gtamslmllh.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.c1oappe.top/gtbkpzvwfy.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.yj20258888.top/gtnkxjtecq.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.sweek.top/gtuaybgghd.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.xziqi.cn/gtzigggjdo.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.hammf.cn/gtscibzxkc.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.tian-w.cn/gtygefcvlt.html

[P08] 处理浮点精度问题
来源：http://hz.xuanzx.com/gtoqafmurw.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.redwolf501.top/gtihncjuel.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.tian-w.cn/gtduwgqtyh.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.shanyushiyangtech.top/gtpbscycjv.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.ppjwa.cn/gthyjjfyaf.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.mhx1999.top/gtzedknwkz.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.tian-w.cn/gtjpkkadtk.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.cqqwz.cn/gtxdexnmco.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.zhoulong.xyz/gtopmflndy.html

================================================================================
来源：http://hz.wangshuangyany.cn/gtogxrdahn.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.xziqi.cn/gtkgcyjxig.html

================================================================================
来源：http://hz.0kj1m.cn/gtsmsbnsol.html

[Q01] 创建表
来源：http://hz.dianchejie.cn/gtxmgacxaw.html

CREATE TABLE users (
来源：http://hz.shangyingyoupin.top/gtsmoitmdb.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.0kj1m.cn/gtpxhmhcwi.html

name VARCHAR(50) NOT NULL,
来源：http://hz.meibo888.top/gtwfufaucg.html

email VARCHAR(100) UNIQUE,
来源：http://hz.chenzaomai.com/gtsyhupsco.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.cqqwz.cn/gtpztfydjo.html

);
来源：http://hz.yj20258.top/gthaxmnkcy.html

[Q02] 创建带外键的表
来源：http://hz.jianghu66.top/gtwrlwfiqa.html

CREATE TABLE orders (
来源：http://hz.jianghu66.top/gtmocbncwd.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.yj20258.top/gtkxvwckvv.html

user_id INT NOT NULL,
来源：http://hz.svipenyu.cn/gtpfrrxmgm.html

amount DECIMAL(10, 2),
来源：http://hz.cheryme.top/gtscorrqyd.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.xuanzx.com/gtmndalebn.html

);
来源：http://hz.xziqi.cn/gtelomenio.html

[Q03] 增加列
来源：http://hz.sxryk.cn/gtnqurgocy.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.shzxlz.cn/gtfjdvvsnq.html

[Q04] 修改列类型
来源：http://hz.havefunace.top/gtpuxlhtqd.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.mhx1999.top/gtqubziyqa.html

[Q05] 重命名列
来源：http://hz.daria6918.cn/gtwxjemnis.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.tianlin.xyz/gtutuvzmli.html

[Q06] 删除列
来源：http://hz.zycfv.cn/gtthcxbruf.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.aibaodan.cn/gtgtxhoclv.html

[Q07] 删除表
来源：http://hz.svipenyu.cn/gtsqvxktrg.html

DROP TABLE IF EXISTS orders;
来源：http://hz.jinqigufen.top/gtbkykapzn.html

[Q08] 创建普通索引
来源：http://hz.shanyushiyangtech.top/gtrwhahdxk.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.gzhubu.top/gtgrtpwtyd.html

[Q09] 创建唯一索引
来源：http://hz.meibo888.top/gtlbpazdes.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.hysaishi.cn/gtwsndbzld.html

[Q10] 插入单行
来源：http://hz.ehwqpu.com/gtsggsixxq.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.pengpengdd.cyou/gtzgtwlokm.html

[Q11] 一次插入多行
来源：http://hz.zhixingplan.top/gtvwjzrkmb.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.yuxming.cn/gtrnbwvkfg.html

[Q12] 插入后取自增 ID
来源：http://hz.pengpengdd.cyou/gtrowfymtz.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.xuetiantiany.cn/gtgbtwjwca.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.chenjidiqi.icu/gtkgcsuooj.html

[Q13] 忽略重复插入
来源：http://hz.sweek.top/gtzzyjmrlj.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.ybcxt.top/gthtsjkywi.html

[Q14] 存在则更新（upsert）
来源：http://hz.chenzaomai.com/gtkzhkawbz.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.zycfv.cn/gtethtfmot.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.pycfn.com/gtwvyilueq.html

[Q15] 查询全部
来源：http://hz.yuxming.cn/gtaxyhhhrn.html

SELECT * FROM users;
来源：http://hz.gogol.net.cn/gtpesbyygz.html

[Q16] 查询指定列
来源：http://hz.hammf.cn/gtqxpgkcaw.html

SELECT id, name FROM users;
来源：http://hz.birdmap.top/gtsgnsdoqq.html

[Q17] 条件查询
来源：http://hz.yvedp.cn/gtkdnkgtrz.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.0kj1m.cn/gtntlkmhla.html

[Q18] 模糊匹配
来源：http://hz.xylfe.cn/gtjstpyjve.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.meibo888.top/gteouwrjkr.html

[Q19] 范围查询
来源：http://hz.zhiwuduotai.top/gttnnszvxn.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.yj20258888.top/gtxzofrdci.html

[Q20] IN 列表
来源：http://hz.gaohongyu789.top/gtiivxiywy.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.fengsongda.top/gtyszozpuj.html

[Q21] 空值判断
来源：http://hz.xylfe.cn/gtomoxgrco.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.redwolf501.top/gtymsakhgc.html

[Q22] 排序
来源：http://hz.hywenlv.cn/gtpfzvripj.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.yonumen.top/gtfchkgcob.html

[Q23] 分页
来源：http://hz.zhixingplan.top/gtawhsubth.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.aizwys.cn/gtnobrvkuz.html

[Q24] 去重
来源：http://hz.bjfxy.top/gtijgpnedi.html

SELECT DISTINCT city FROM users;
来源：http://hz.yangfankeji.com/gtzesecyqq.html

[Q25] 只取前 N 条
来源：http://hz.gogol.net.cn/gtlifgzmah.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.yuanzhike.top/gthqdikmap.html

[Q26] 计数
来源：http://hz.ydjk.org.cn/gtolvhzkgh.html

SELECT COUNT(*) FROM users;
来源：http://hz.pycfn.com/gtytidhyee.html

[Q27] 条件计数
来源：http://hz.0kj1m.cn/gtpkclrlzx.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.nanxinkj.top/gtuoyqznpc.html

[Q28] 求和与平均
来源：http://hz.shanyushiyangkeji.top/gtzrpgnhml.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.sufxvd.cn/gtmpvcoxli.html

[Q29] 最大最小值
来源：http://hz.316326.xyz/gtwfknhtuu.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.c1oappe.top/gtnyauuvsu.html

[Q30] 分组统计
来源：http://hz.xingfuxueyuan.xyz/gtrfhpzsij.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.jqgfzy.top/gtbtfdtcfl.html

[Q31] 分组后过滤
来源：http://hz.sufxvd.cn/gtfhfcqzzh.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.cdnleiting.top/gtgxpwlwsy.html

[Q32] 分组拼接字符串
来源：http://hz.daxiang520.top/gthbxpglgh.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.jiagoushi.top/gtrycxnosi.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.hysaishi.cn/gtjcvtlthb.html

[Q33] 多列分组
来源：http://hz.daria6918.cn/gtfyslqako.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.zhongyouzk.top/gtzrfcxypn.html

[Q34] 每组取第一条
来源：http://hz.jianghu66.top/gtjdystqag.html

SELECT * FROM (
来源：http://hz.jinghuilouyu.cn/gtsovgtora.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.gogol.net.cn/gtjqhyuxwe.html

) t WHERE rn = 1;
来源：http://hz.redwolf501.top/gtdfcviaqm.html

[Q35] 内连接
来源：http://hz.yanxiufei.cn/gtunznxcrk.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.9152youxi.cn/gtvrcfwvvn.html

[Q36] 左连接
来源：http://hz.xziqi.cn/gtrlqysbma.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.hongshengwenyu.top/gtmxpcupdj.html

[Q37] 右连接
来源：http://hz.ehwqpu.com/gtrzioffua.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.yueranfly.top/gtouwssnba.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.quarkkingdee.top/gtukcprrhw.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.ywan-chungtsiang.top/gtrlklxpkb.html

[Q39] 自连接（查上下级）
来源：http://hz.havefunace.top/gtbmzxnhrn.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.shangyingyoupin.top/gtlzzooqdf.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.hammf.cn/gttpxcihvi.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.jlsjyb.cn/gtrcrzhsuf.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.gotoacloud.top/gtzjbabmqw.html

[Q41] 多表连接
来源：http://hz.jinyuanbaomall.cn/gtwnjamoby.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.bjfxy.top/gtddniazww.html

JOIN users u ON u.id = o.user_id
来源：http://hz.yj20258888.top/gtsqkbugxd.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.kuanghao11.cn/gtddnqdmzo.html

[Q42] 连接条件附加过滤
来源：http://hz.jinyuanbaomall.cn/gtwnhidpht.html

SELECT u.name, o.amount FROM users u
来源：http://hz.feifeiyinyue.top/gtosmughmr.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.nwbrower.top/gtbeynlrcl.html

[Q43] 标量子查询
来源：http://hz.nanxuanxn.top/gtxomfwwcs.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.hongshengwenyu.top/gtqqktuipu.html

[Q44] IN 子查询
来源：http://hz.cdnleiting.top/gtnruqppbk.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.hnqzz.top/gtifsoeggu.html

[Q45] EXISTS 判断存在
来源：http://hz.dianchejie.cn/gtbxlerfks.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.316326.xyz/gtdtuxhvld.html


<!-- 参考信息 -->