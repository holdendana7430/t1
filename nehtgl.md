代发 wailian999

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.wangshuangyany.cn/gtnwmsokjl.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.ydjk.org.cn/gtazhdqraw.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.hnqzz.top/gtubqnyulp.html

Ruby: a.gcd(b)
来源：http://hz.ehwqpu.com/gtzmsolsxi.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.shanyushiyangkeji.top/gtajdqecex.html

[N06] 判断回文字符串
来源：http://hz.sweek.top/gtakdlaoqk.html

Py:   s == s[::-1]
来源：http://hz.sufxvd.cn/gtqhxpnlrl.html

PHP:  $s === strrev($s);
来源：http://hz.jianghu66.top/gteavqcfqp.html

JS:   s === [...s].reverse().join("")
来源：http://hz.iojbl.cn/gtqjxrahka.html

TS:   s === [...s].reverse().join("")
来源：http://hz.dianchejie.cn/gtyugfgnyu.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.cqqwz.cn/gtwxtnohfp.html

Go:   // 双指针从两端比较
来源：http://hz.shangyingyoupin.top/gtxvmtczah.html

Ruby: s == s.reverse
来源：http://hz.ivvv.top/gtsflifmyt.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.vqdsnc.cn/gtonisojvg.html

[N07] 两数之和（返回下标）
来源：http://hz.jinqigfzy.top/gtmkuzarod.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.nwbrower.top/gtcaybltwf.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.daria6918.cn/gtwivwpboz.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.guannengcc.top/gttiuenhuh.html

TS:   // 手写 Map<string, number>
来源：http://hz.yj202588.top/gtxjpephhw.html

Java: // 手写 HashMap
来源：http://hz.yongpay.top/gtnvsuvbgc.html

Go:   // 手写 map[int]int
来源：http://hz.jinghuilouyu.cn/gttuuipgjv.html

Ruby: // 手写 Hash
来源：http://hz.zdqjudy.top/gtnkbyxdfl.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.316326.xyz/gtpeegzppi.html

[N08] 生成全排列
来源：http://hz.cucudq.cn/gtcwcmhmel.html

Py:   itertools.permutations(arr)
来源：http://hz.yanxiufei.cn/gtpqyvckzf.html

PHP:  // 手写递归交换
来源：http://hz.jqgfzy.top/gtaxsnouxg.html

JS:   // 手写回溯递归
来源：http://hz.shangyingyoupin.top/gtjaswzbna.html

TS:   // 手写回溯递归
来源：http://hz.xinyue.icu/gtygayvqai.html

Java: // 手写回溯递归
来源：http://hz.ehwqpu.com/gtotpgldwe.html

Go:   // 手写回溯递归
来源：http://hz.yanxiufei.cn/gtxfjhqqll.html

Ruby: arr.permutation.to_a
来源：http://hz.cheryme.top/gtiuhmxzvr.html

C#:   // 手写回溯递归
来源：http://hz.hongshengwenyu.top/gtqdmmycxg.html

[N09] 栈与队列
来源：http://hz.jyoumei.cn/gtrovklqwc.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.cucudq.cn/gtvlrptmbn.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.birdmap.top/gtzfmaybqo.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.zhongyouzk.top/gtkuahsswt.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.birdmap.top/gtjlzulzvz.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.feifeiyinyue.top/gtiefslvcg.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.feifeiyinyue.top/gtthuyivmc.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.shuidangran.top/gtwfmbabyd.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.gaohongyu789.top/gtavgzjlcc.html

[N10] 链表节点定义
来源：http://hz.jiagoushi.top/gthwjrdrua.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.wangdashe.top/gtfxdzokrw.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.chenzaomai.com/gtzvuazdur.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.shanyushiyangkeji.top/gthczxmekl.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.andypj.xyz/gtwqypgfsb.html

Java: class Node { int v; Node next; }
来源：http://hz.yanxiufei.cn/gtxmnffukp.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.yj202588.top/gtkqebvdft.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.zhoulong.xyz/gthxmdezxv.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.yonumen.top/gtapqhyqmg.html

[N11] 二叉树中序遍历
来源：http://hz.xuanzx.com/gtfurihlxz.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.52xcode.cn/gtqkjzavvz.html

PHP:  // 手写递归函数
来源：http://hz.pengpengdd.cyou/gtpmnrmdun.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.pycfn.com/gtptenqrul.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.hywenlv.cn/gtsdmraxxm.html

Java: // 手写递归
来源：http://hz.316326.xyz/gtbyeeazxr.html

Go:   // 手写递归
来源：http://hz.xuetiantiany.cn/gtzapkysgi.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.shangyingyoupin.top/gtwshymddw.html

C#:   // 手写递归
来源：http://hz.shangyingyoupin.top/gtxmyhhjxy.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.cucudq.cn/gtcvuemboi.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.gogol.net.cn/gtbovdlmux.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.yj20258.top/gtrdwghhsn.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.jiagoushi.top/gtpdvcobwe.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.zhoulong.xyz/gtzkucewzx.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.xuetiantiany.cn/gtzomkotfo.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.shanyushiyangtech.top/gtaddmomyi.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.aizwys.cn/gthethxhhw.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.guannengcc.top/gtaeeorvgx.html

================================================================================
来源：http://hz.gaohongyu789.top/gtuqynsvsx.html

O. 并发与异步
来源：http://hz.quarkkingdee.top/gtcjunljoi.html

================================================================================
来源：http://hz.yuxming.cn/gtwsfyonxa.html

[O01] 启动一个线程
来源：http://hz.jinghuilouyu.cn/gtegfyeosg.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.xinyue.icu/gtltqfyiyu.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.0kj1m.cn/gtmdgzoxxk.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.hywenlv.cn/gtcmgkxjbm.html

TS:   // 同 JS
来源：http://hz.mhx1999.top/gtbkpvykhc.html

Java: new Thread(() -> f()).start()
来源：http://hz.jinghuilouyu.cn/gtzeltpfkd.html

Go:   go f()
来源：http://hz.chenlongwang.top/gtkistxpxj.html

Ruby: Thread.new { f }
来源：http://hz.hfpthk.cn/gtdwrpvjkk.html

C#:   Task.Run(() => F());
来源：http://hz.zhaomingkeji.xyz/gtnqdzhxqv.html

[O02] 使用线程池
来源：http://hz.hysaishi.cn/gtrfvuvqyh.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.ivvv.top/gtjwiwywxr.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.yvedp.cn/gtzsgxpqxi.html

JS:   // worker_threads 线程池
来源：http://hz.snrcjt.cn/gtnxedsbxr.html

TS:   // worker_threads 线程池
来源：http://hz.haohaochexian.top/gtwywfkmmr.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.yuanzhike.top/gtlddivlwh.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.pengpengdd.cyou/gtqojajmvd.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.meibo888.top/gtetobnzca.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.ehwqpu.com/gtalzuxvon.html

[O03] 加锁保护共享数据
来源：http://hz.yangfankeji.com/gtmrnrbxwz.html

Py:   with lock: shared += 1
来源：http://hz.hywenlv.cn/gtpdmnetij.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.zhengqikj.top/gtyztmtgzu.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.hongshengwenyu.top/gthuiabbhs.html

TS:   // 同 JS
来源：http://hz.ivvv.top/gtchcutqxn.html

Java: synchronized (this) { shared++; }
来源：http://hz.gogol.net.cn/gtqgyhtcys.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.wangdashe.top/gtorozzmvt.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.hnxiangtu.top/gtvntvxkby.html

C#:   lock (gate) { shared++; }
来源：http://hz.chenlongwang.top/gtdcahfmeh.html

[O04] 定义异步函数并等待
来源：http://hz.gogol.net.cn/gtxkcvboyu.html

Py:   async def f():⏎    await g()
来源：http://hz.hammf.cn/gtxwbgopth.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.bjfxy.top/gtxaiipdph.html

JS:   async function f() { await g(); }
来源：http://hz.daria6918.cn/gtvejzzsmo.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.yj20258888.top/gtidyiprbo.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.guannengcc.top/gtlfnjqple.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.hammf.cn/gtpsszxbos.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.gotoacloud.top/gtvniohnfo.html

C#:   async Task F() { await G(); }
来源：http://hz.yongpay.top/gtomitnhfn.html

[O05] 并发执行并等待全部完成
来源：http://hz.dashuyun.cn/gtakmxuwmc.html

Py:   asyncio.gather(*tasks)
来源：http://hz.svipenyu.cn/gtsmkvzsym.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.tianlin.xyz/gtmdrslrfq.html

JS:   await Promise.all(tasks)
来源：http://hz.wangshuangyany.cn/gtphxvunjj.html

TS:   await Promise.all(tasks)
来源：http://hz.xinyue.icu/gtugrmyykb.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.hammf.cn/gtddnbcmnw.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.mhx1999.top/gtjhrrsgfa.html

Ruby: threads.map(&:join)
来源：http://hz.tian-w.cn/gtpcnclbqz.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.redwolf501.top/gtnimjwklq.html

[O06] 使用进程池
来源：http://hz.chenzaomai.com/gtzligapny.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.fengsongda.top/gtxhkeeeld.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.xziqi.cn/gtmbwokzur.html

JS:   // child_process / cluster 模块
来源：http://hz.guannengcc.top/gtrhkjxbbe.html

TS:   // child_process / cluster 模块
来源：http://hz.aizwys.cn/gtdrnitfoj.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.daxiang520.top/gtbfshvxim.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.kuanghao11.cn/gtvdmizhom.html

Ruby: // fork 块
来源：http://hz.daxiang520.top/gtiusyjaty.html

C#:   Parallel.For
来源：http://hz.tian-w.cn/gtxevegcux.html

================================================================================
来源：http://hz.gaohongyu789.top/gtwmmqilbt.html

P. 常用工具函数
来源：http://hz.aibaodan.cn/gtroselpzn.html

================================================================================
来源：http://hz.havefunace.top/gtunttegyj.html

[P01] 生成 UUID
来源：http://hz.jinyuanbaomall.cn/gttvlbjsaz.html

Py:   str(uuid.uuid4())
来源：http://hz.jyoumei.cn/gtauumtvie.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.birdmap.top/gtqfmhoghk.html

JS:   crypto.randomUUID()
来源：http://hz.ywan-chungtsiang.top/gtkphtsqgf.html

TS:   crypto.randomUUID()
来源：http://hz.zhoulong.xyz/gtcpjcaaqa.html

Java: UUID.randomUUID().toString()
来源：http://hz.dianchejie.cn/gtumwjblef.html

Go:   // 用 github.com/google/uuid
来源：http://hz.shangyingyoupin.top/gtgrmyuibt.html

Ruby: SecureRandom.uuid
来源：http://hz.jianghu66.top/gtqzwpasqt.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.hammf.cn/gtklckfzen.html

[P02] MD5 / SHA256 摘要
来源：http://hz.haohaochexian.top/gtuktoeeps.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.sweek.top/gtnyuypltc.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.9152youxi.cn/gtjgffhysw.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.xziqi.cn/gtservxvvg.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.daxiang520.top/gttzgiiawf.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.zdqjudy.top/gtaqhjizjj.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.chenzaomai.com/gtpvbpstya.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.shuidangran.top/gtxifaawrd.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.jlsjyb.cn/gthkhqjhgs.html

[P03] 生成短随机字符串
来源：http://hz.zycfv.cn/gtfczqysxg.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.52xcode.cn/gttxotppoh.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.zhixingplan.top/gtitrzdrmz.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.cucudq.cn/gtgaymtxid.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.cqqwz.cn/gtatzszmab.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.shangyingyoupin.top/gtxfjolnhg.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.daria6918.cn/gtvoislmut.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.svipenyu.cn/gthnqjmclg.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.yueranfly.top/gtragmjghe.html

[P04] 求长度
来源：http://hz.ppjwa.cn/gtajvgqwfz.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.cheryme.top/gtcqcuimip.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.cqqwz.cn/gtfeyoabyo.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.hfpthk.cn/gtwzrwnfbf.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.sufxvd.cn/gtozpjgulf.html

Java: list.size();  map.size();  s.length()
来源：http://hz.tianlin.xyz/gtuybzkhqq.html

Go:   len(arr);  len(m)
来源：http://hz.sweek.top/gtaomvzbha.html

Ruby: x.length;  x.size
来源：http://hz.tanke756.top/gtdaghizzm.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.yonumen.top/gtharowpac.html

[P05] 判断两个对象内容是否相等
来源：http://hz.yvedp.cn/gtjowftefx.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.yuxming.cn/gtrljycbtl.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.chenjidiqi.icu/gtbvfhymky.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.feifeiyinyue.top/gtqdazuwby.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.0kj1m.cn/gtwfvdbiai.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.andypj.xyz/gtswolsyxw.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.cucudq.cn/gtriwyzrzy.html

Ruby: a == b
来源：http://hz.c1oappe.top/gtwmbqvqlr.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.xylfe.cn/gtuywhfstj.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.kuanghao11.cn/gtxdnfcnrx.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.ppjwa.cn/gtvmzbtbjx.html

PHP:  if (empty($x)) {}
来源：http://hz.c1oappe.top/gteebmrokm.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.zycfv.cn/gtalemytbo.html

TS:   if (x == null) {}
来源：http://hz.havefunace.top/gtgvrpodqn.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.birdmap.top/gtjloefouj.html

Go:   if x == nil {}
来源：http://hz.guowangkeji.top/gtnqluvznc.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.yj20258.top/gtlyqtonca.html

C#:   if (x is null) {}
来源：http://hz.xinyue.icu/gtfhbpdezy.html

[P07] 防抖与节流
来源：http://hz.hnxiangtu.top/gttyvcvwbi.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.yj20258.top/gtjliqpmvy.html

PHP:  // 手写时间戳比较
来源：http://hz.jinqigufen.top/gtxfuesiym.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.sufxvd.cn/gtmtqyecpu.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.yj202588.top/gtsbohkfwv.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.yuxming.cn/gtknenmudo.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.aizwys.cn/gthiktlybw.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.xinyue.icu/gtjjtyeddj.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.zhiwuduotai.top/gtapspeymh.html

[P08] 处理浮点精度问题
来源：http://hz.yangfankeji.com/gtkzjhdnna.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.0kj1m.cn/gtpglhsulm.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.pengpengdd.cyou/gtcmhzyjzg.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.zhongyouzk.top/gtnwxqurhx.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.fzhhl.top/gtmhyvzfky.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.hnxiangtu.top/gtewzruzpk.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.zhoulong.xyz/gtemdmqwzs.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.pycfn.com/gtmazdndjz.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.jianghu66.top/gtpkhvhopk.html

================================================================================
来源：http://hz.yueranfly.top/gtkslbqbdp.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.shanyushiyangtech.top/gtpynbflhu.html

================================================================================
来源：http://hz.yangfankeji.com/gtdcahkvbq.html

[Q01] 创建表
来源：http://hz.sysykeji.top/gthakoyfhr.html

CREATE TABLE users (
来源：http://hz.dashuyun.cn/gtomxgifcw.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.sysykeji.top/gtypkpufgc.html

name VARCHAR(50) NOT NULL,
来源：http://hz.hysaishi.cn/gtcfzcrwnw.html

email VARCHAR(100) UNIQUE,
来源：http://hz.svipenyu.cn/gtmwjyndua.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.yuanzhike.top/gtdpthdrbe.html

);
来源：http://hz.tanke756.top/gtexbcqwqs.html

[Q02] 创建带外键的表
来源：http://hz.shanyushiyangtech.top/gtukasbsyc.html

CREATE TABLE orders (
来源：http://hz.zhixingplan.top/gtnjllybzz.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.yuxming.cn/gthgvpacfp.html

user_id INT NOT NULL,
来源：http://hz.yj20258888.top/gtvgolbooc.html

amount DECIMAL(10, 2),
来源：http://hz.smart0.xyz/gtjpayklab.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.52xcode.cn/gtrxbonwza.html

);
来源：http://hz.wangdashe.top/gtzbwcdewn.html

[Q03] 增加列
来源：http://hz.wangshuangyany.cn/gtrvewutso.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.wangshuangyany.cn/gthgsmvcew.html

[Q04] 修改列类型
来源：http://hz.zdqjudy.top/gtfyapyfki.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.gogol.net.cn/gtzrinvsrv.html

[Q05] 重命名列
来源：http://hz.kuanghao11.cn/gtnyqbqjwq.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.shanyushiyangkeji.top/gttawhaggt.html

[Q06] 删除列
来源：http://hz.wangdashe.top/gtpebdkkqv.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.ywan-chungtsiang.top/gtvwylykcr.html

[Q07] 删除表
来源：http://hz.jqgufenzy.top/gtmuqbjaks.html

DROP TABLE IF EXISTS orders;
来源：http://hz.ydjk.org.cn/gtcwuorslj.html

[Q08] 创建普通索引
来源：http://hz.zhoulong.xyz/gtnplydxrb.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.ydjk.org.cn/gtzsljzkgg.html

[Q09] 创建唯一索引
来源：http://hz.c1oappe.top/gtxzksqooj.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.hywenlv.cn/gtrwxoxqru.html

[Q10] 插入单行
来源：http://hz.hysaishi.cn/gtcmxjugln.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.xuanzx.com/gteldwluah.html

[Q11] 一次插入多行
来源：http://hz.xuanzx.com/gtvckrqffa.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.ybcxt.top/gtnldkygat.html

[Q12] 插入后取自增 ID
来源：http://hz.jinghuilouyu.cn/gtvhsvvjbk.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.zhengqikj.top/gtiulovuaq.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.jinyuanbaomall.cn/gtcsaamqvu.html

[Q13] 忽略重复插入
来源：http://hz.yvedp.cn/gtlikwkpgl.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.nanxinkj.top/gtazbuyohy.html

[Q14] 存在则更新（upsert）
来源：http://hz.yanxiufei.cn/gtxksxmgco.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.chenzaomai.com/gtnvyefuue.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.ydjk.org.cn/gthntjbbpy.html

[Q15] 查询全部
来源：http://hz.jiagoushi.top/gthpehsive.html

SELECT * FROM users;
来源：http://hz.aibaodan.cn/gtaeqxzgoq.html

[Q16] 查询指定列
来源：http://hz.snrcjt.cn/gtnzxojjms.html

SELECT id, name FROM users;
来源：http://hz.snrcjt.cn/gtqszngubq.html

[Q17] 条件查询
来源：http://hz.tanke756.top/gtmniyhfxi.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.gzhubu.top/gtdpxcykrx.html

[Q18] 模糊匹配
来源：http://hz.hywenlv.cn/gtfaepyorq.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.daxiang520.top/gtgbzfjcho.html

[Q19] 范围查询
来源：http://hz.svipenyu.cn/gttxtlatpu.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.9152youxi.cn/gtmbnuracp.html

[Q20] IN 列表
来源：http://hz.nwbrower.top/gtjmdczewz.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.hnxiangtu.top/gtzmatewea.html

[Q21] 空值判断
来源：http://hz.sxryk.cn/gtzvbjbbmg.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.shzxlz.cn/gtsgnsxkmm.html

[Q22] 排序
来源：http://hz.shanyushiyangkeji.top/gtdxbunpmu.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.svipenyu.cn/gtnusfzstn.html

[Q23] 分页
来源：http://hz.daxiang520.top/gtybezzlfs.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.yangfankeji.com/gtzmivlhxy.html

[Q24] 去重
来源：http://hz.yueranfly.top/gtrtynbray.html

SELECT DISTINCT city FROM users;
来源：http://hz.jinqigfzy.top/gtzjaluwcl.html

[Q25] 只取前 N 条
来源：http://hz.dashuyun.cn/gtacpxdgvr.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.vqdsnc.cn/gttaptorlv.html

[Q26] 计数
来源：http://hz.xingfuxueyuan.xyz/gtisgjptlz.html

SELECT COUNT(*) FROM users;
来源：http://hz.havefunace.top/gtbwcfjfyy.html

[Q27] 条件计数
来源：http://hz.zhijiandao.cn/gtumwkcgie.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.birdmap.top/gtagoqojbj.html

[Q28] 求和与平均
来源：http://hz.snrcjt.cn/gtpkumbwgo.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.sysykeji.top/gtjcaafdyn.html

[Q29] 最大最小值
来源：http://hz.zhijiandao.cn/gtpjwopocf.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.jinqigufen.top/gttirvsrwe.html

[Q30] 分组统计
来源：http://hz.sxryk.cn/gttvbfuomx.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.guowangkeji.top/gtidvumxft.html

[Q31] 分组后过滤
来源：http://hz.andypj.xyz/gtalnwyvtd.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.zhiwuduotai.top/gtdluytqtw.html

[Q32] 分组拼接字符串
来源：http://hz.guowangkeji.top/gtdgxrtgze.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.sysykeji.top/gthaggywza.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.gogol.net.cn/gtwcggbtun.html

[Q33] 多列分组
来源：http://hz.zhengqikj.top/gtfcblhctn.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.jinyuanbaomall.cn/gtwdxevqki.html

[Q34] 每组取第一条
来源：http://hz.cdnleiting.top/gtnahwytww.html

SELECT * FROM (
来源：http://hz.zhoulong.xyz/gtsgwbfxum.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.mhx1999.top/gthvveqdjn.html

) t WHERE rn = 1;
来源：http://hz.zdqjudy.top/gtnykkaarp.html

[Q35] 内连接
来源：http://hz.0kj1m.cn/gtzzltupzk.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.svipenyu.cn/gtopqsazgq.html

[Q36] 左连接
来源：http://hz.andypj.xyz/gtunnnstsp.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.zhiwuduotai.top/gtzuifapan.html

[Q37] 右连接
来源：http://hz.xuetiantiany.cn/gtyxkcmyzd.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.nanxuanxn.top/gtawwpwimn.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.yj20258.top/gtcufmuhcs.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.jinghuilouyu.cn/gtimllwvwe.html

[Q39] 自连接（查上下级）
来源：http://hz.daxiang520.top/gtxnqkqymi.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.jqgfzy.top/gtumxreuib.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.hongshengwenyu.top/gtowwdftef.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.cucudq.cn/gtvoehwceu.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.zycfv.cn/gtrhzbnlbm.html

[Q41] 多表连接
来源：http://hz.bjfxy.top/gtudjpdtxq.html


<!-- 参考信息 -->