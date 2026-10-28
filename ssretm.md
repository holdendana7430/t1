代发 wailian999

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.nanxuanxn.top/gtrrejpvul.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.ivvv.top/gtskvxonnl.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.ehwqpu.com/gtfpoxpemt.html

Ruby: a.gcd(b)
来源：http://hz.fzhhl.top/gtxonvqcqe.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.bjfxy.top/gtqfevihhs.html

[N06] 判断回文字符串
来源：http://hz.aizwys.cn/gtludkmnxc.html

Py:   s == s[::-1]
来源：http://hz.cqqwz.cn/gtflvvqked.html

PHP:  $s === strrev($s);
来源：http://hz.xinyue.icu/gtpywsefkl.html

JS:   s === [...s].reverse().join("")
来源：http://hz.bjfxy.top/gtmubyuwst.html

TS:   s === [...s].reverse().join("")
来源：http://hz.meibo888.top/gtqvajuiwr.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.quarkkingdee.top/gtnoklroan.html

Go:   // 双指针从两端比较
来源：http://hz.yuxming.cn/gtiylvclzq.html

Ruby: s == s.reverse
来源：http://hz.chenzaomai.com/gtgtpncdpv.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.yonumen.top/gtrvmvpkif.html

[N07] 两数之和（返回下标）
来源：http://hz.shuidangran.top/gtkubvpjcm.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.yonumen.top/gtlvcyxhte.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.hnxiangtu.top/gtialwhhtc.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.meibo888.top/gtakvmtwzo.html

TS:   // 手写 Map<string, number>
来源：http://hz.yj20258.top/gtuhiyxlfp.html

Java: // 手写 HashMap
来源：http://hz.hammf.cn/gtissyasyo.html

Go:   // 手写 map[int]int
来源：http://hz.ppjwa.cn/gtjzgjqgoj.html

Ruby: // 手写 Hash
来源：http://hz.hywenlv.cn/gtnjtjkgid.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.hfpthk.cn/gtimfelrdj.html

[N08] 生成全排列
来源：http://hz.ywan-chungtsiang.top/gtpbeemztm.html

Py:   itertools.permutations(arr)
来源：http://hz.jinqigfzy.top/gtadadbffm.html

PHP:  // 手写递归交换
来源：http://hz.yj20258.top/gtbphswqyw.html

JS:   // 手写回溯递归
来源：http://hz.guannengcc.top/gtgszmhrxt.html

TS:   // 手写回溯递归
来源：http://hz.zhaomingkeji.xyz/gtrdnhvggc.html

Java: // 手写回溯递归
来源：http://hz.yj202588.top/gtvwgizxwq.html

Go:   // 手写回溯递归
来源：http://hz.daria6918.cn/gtwbylotou.html

Ruby: arr.permutation.to_a
来源：http://hz.gaohongyu789.top/gtxoijqhih.html

C#:   // 手写回溯递归
来源：http://hz.c1oappe.top/gtcrmitxoi.html

[N09] 栈与队列
来源：http://hz.vqdsnc.cn/gtxzfcxzdz.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.kuanghao11.cn/gtjnhksbsx.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.bjfxy.top/gtvqdxsbmz.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.zhengqikj.top/gtoktivegi.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.zhengqikj.top/gtimsxomld.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.yueranfly.top/gtsyohafbu.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.shanyushiyangkeji.top/gtkhynkwxm.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.mhx1999.top/gtddirogzo.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.shzxlz.cn/gtsmlntxlt.html

[N10] 链表节点定义
来源：http://hz.yj20258888.top/gtnrbbeowt.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.fengsongda.top/gtiokjzawh.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.yuanzhike.top/gtygkdjiib.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.guannengcc.top/gtmofinciv.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.jqgfzy.top/gtbfrbnyfv.html

Java: class Node { int v; Node next; }
来源：http://hz.redwolf501.top/gtklmgitca.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.cashguo.top/gtyieiogll.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.xingfuxueyuan.xyz/gtdlslgcjq.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.jiagoushi.top/gtuplcnykh.html

[N11] 二叉树中序遍历
来源：http://hz.nanxuanxn.top/gtbydmapwx.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.snrcjt.cn/gtvhqakobn.html

PHP:  // 手写递归函数
来源：http://hz.hnxiangtu.top/gthdfjvrqr.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.hammf.cn/gtyaqnfcgw.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.birdmap.top/gtjrfjbnff.html

Java: // 手写递归
来源：http://hz.gogol.net.cn/gtjhcjavrv.html

Go:   // 手写递归
来源：http://hz.xuanzx.com/gtgfjrlhcp.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.daxiang520.top/gtzfegspec.html

C#:   // 手写递归
来源：http://hz.meibo888.top/gtpqimtige.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.zycfv.cn/gtbzhunooj.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.shanyushiyangtech.top/gtgrngcfpa.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.feifeiyinyue.top/gtpbfhoxqa.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.nanxinkj.top/gtnotozfmq.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.andypj.xyz/gtndrmaaii.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.yj202588.top/gtyctqjoug.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.redwolf501.top/gtikozanah.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.yuanzhike.top/gthgpsebyt.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.gzhubu.top/gtwpdcpemo.html

================================================================================
来源：http://hz.vqdsnc.cn/gtncxumkge.html

O. 并发与异步
来源：http://hz.nanxinkj.top/gtykqwnedm.html

================================================================================
来源：http://hz.gotoacloud.top/gtupyeztwf.html

[O01] 启动一个线程
来源：http://hz.andypj.xyz/gtaqjjsbat.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.dashuyun.cn/gtikdgtrgn.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.dashuyun.cn/gtshirzscw.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.jinqigufen.top/gtcspvvgrp.html

TS:   // 同 JS
来源：http://hz.yanxiufei.cn/gtavevzdfk.html

Java: new Thread(() -> f()).start()
来源：http://hz.guowangkeji.top/gtqkyolyeg.html

Go:   go f()
来源：http://hz.jinqigufen.top/gtebtiesqv.html

Ruby: Thread.new { f }
来源：http://hz.hywenlv.cn/gtzattgrcl.html

C#:   Task.Run(() => F());
来源：http://hz.aizwys.cn/gtryytcwtn.html

[O02] 使用线程池
来源：http://hz.jinyuanbaomall.cn/gtbuntvybb.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.9152youxi.cn/gttodqemgn.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.svipenyu.cn/gtwhuoruzn.html

JS:   // worker_threads 线程池
来源：http://hz.meibo888.top/gtxnfpqzaj.html

TS:   // worker_threads 线程池
来源：http://hz.jinqigfzy.top/gtnfidsiau.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.0kj1m.cn/gtoqsxinoa.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.kuanghao11.cn/gtpomyuzaw.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.yanxiufei.cn/gtwiiiwaiu.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.daria6918.cn/gtjrjdsdum.html

[O03] 加锁保护共享数据
来源：http://hz.9152youxi.cn/gtkrurufep.html

Py:   with lock: shared += 1
来源：http://hz.yj202588.top/gtebrfnrgm.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.xylfe.cn/gtfzoftehs.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.hnqzz.top/gtdsasivmn.html

TS:   // 同 JS
来源：http://hz.cdnleiting.top/gtninwhdli.html

Java: synchronized (this) { shared++; }
来源：http://hz.xingfuxueyuan.xyz/gtgtelqjto.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.c1oappe.top/gtacjaxdup.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.jlsjyb.cn/gtnlgjvzax.html

C#:   lock (gate) { shared++; }
来源：http://hz.shanyushiyangkeji.top/gtffwxsqpa.html

[O04] 定义异步函数并等待
来源：http://hz.sweek.top/gtrvzkquee.html

Py:   async def f():⏎    await g()
来源：http://hz.gzhubu.top/gttgraadic.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.yangfankeji.com/gtjcaojwkt.html

JS:   async function f() { await g(); }
来源：http://hz.hammf.cn/gtjstlvvcb.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.cqqwz.cn/gtfkgvfnwg.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.aibaodan.cn/gthicklfat.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.smart0.xyz/gtwnnzfhjg.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.xuanzx.com/gtjeinqeur.html

C#:   async Task F() { await G(); }
来源：http://hz.zhijiandao.cn/gtttfeicdk.html

[O05] 并发执行并等待全部完成
来源：http://hz.ybcxt.top/gtaahicizy.html

Py:   asyncio.gather(*tasks)
来源：http://hz.xziqi.cn/gtudbxpydi.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.ydjk.org.cn/gtkaeekrtf.html

JS:   await Promise.all(tasks)
来源：http://hz.tian-w.cn/gtqiefptql.html

TS:   await Promise.all(tasks)
来源：http://hz.ywan-chungtsiang.top/gtfimpwztr.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.hnqzz.top/gtqmjcfcbl.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.wangdashe.top/gtfxuzcecj.html

Ruby: threads.map(&:join)
来源：http://hz.zhongyouzk.top/gtskofqlpm.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.c1oappe.top/gteotgpdpb.html

[O06] 使用进程池
来源：http://hz.yueranfly.top/gtdxblyoad.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.cheryme.top/gtaccaxmrx.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.xinyue.icu/gttrosmwoa.html

JS:   // child_process / cluster 模块
来源：http://hz.hnqzz.top/gticgnkind.html

TS:   // child_process / cluster 模块
来源：http://hz.c1oappe.top/gtsmjtxxvj.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.guannengcc.top/gtrfpfkmoy.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.hywenlv.cn/gtqepoiwrq.html

Ruby: // fork 块
来源：http://hz.nanxinkj.top/gtzsydiqqs.html

C#:   Parallel.For
来源：http://hz.jqgufenzy.top/gtrzrtrder.html

================================================================================
来源：http://hz.zhoulong.xyz/gtbqqvzsym.html

P. 常用工具函数
来源：http://hz.cheryme.top/gtbokqhqlk.html

================================================================================
来源：http://hz.52xcode.cn/gtogelbgdz.html

[P01] 生成 UUID
来源：http://hz.shangyingyoupin.top/gtbzpalqda.html

Py:   str(uuid.uuid4())
来源：http://hz.zhixingplan.top/gtglrwjxfd.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.jinghuilouyu.cn/gtfunntogz.html

JS:   crypto.randomUUID()
来源：http://hz.yanxiufei.cn/gtlyceaugs.html

TS:   crypto.randomUUID()
来源：http://hz.jinghuilouyu.cn/gtwydqtxhy.html

Java: UUID.randomUUID().toString()
来源：http://hz.aibaodan.cn/gtmtepjrqt.html

Go:   // 用 github.com/google/uuid
来源：http://hz.feifeiyinyue.top/gtbazmecau.html

Ruby: SecureRandom.uuid
来源：http://hz.yonumen.top/gtfyzwkhyi.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.havefunace.top/gtckakgzcb.html

[P02] MD5 / SHA256 摘要
来源：http://hz.ydjk.org.cn/gttpqxfmtu.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.hywenlv.cn/gtwyrvifqw.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.hywenlv.cn/gtzjdkligh.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.tanke756.top/gtnjwfqbrq.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.jinqigufen.top/gtzlmuyskv.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.zhengqikj.top/gtsvouyxdf.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.316326.xyz/gtgnrzakqk.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.redwolf501.top/gtjumtgdhl.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.fengsongda.top/gtgkestjwm.html

[P03] 生成短随机字符串
来源：http://hz.havefunace.top/gtgkmedpsw.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.sweek.top/gtrrkcrgpq.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.xingfuxueyuan.xyz/gttalnhiuh.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.yangfankeji.com/gtnzaamlrb.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.yanxiufei.cn/gtdtnzjupt.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.yuanzhike.top/gtpqoxjfna.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.xziqi.cn/gteqnzzikh.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.ppjwa.cn/gtqszycvhl.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.fzhhl.top/gtnznipzxk.html

[P04] 求长度
来源：http://hz.cashguo.top/gtuoshrpof.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.guannengcc.top/gtkoyeusen.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.yongpay.top/gtczfbohhq.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.cqqwz.cn/gtkutnskjs.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.nanxuanxn.top/gtwredvpvg.html

Java: list.size();  map.size();  s.length()
来源：http://hz.cucudq.cn/gttzdcdndx.html

Go:   len(arr);  len(m)
来源：http://hz.hysaishi.cn/gtfufugtyt.html

Ruby: x.length;  x.size
来源：http://hz.nwbrower.top/gtynyqnfsg.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.zhongyouzk.top/gtjbfadgfc.html

[P05] 判断两个对象内容是否相等
来源：http://hz.gogol.net.cn/gttzgqfooe.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.gaohongyu789.top/gtmlqnxrin.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.daria6918.cn/gtlqizlflg.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.ivvv.top/gturhwuhlh.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.52xcode.cn/gtfmponubw.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.zhongyouzk.top/gtbhfbsyjz.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.sufxvd.cn/gtqgowrlry.html

Ruby: a == b
来源：http://hz.jlsjyb.cn/gtkyvevdta.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.zhiwuduotai.top/gtkllfdbdf.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.yongpay.top/gtyeeckhym.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.xuetiantiany.cn/gtbpurbgud.html

PHP:  if (empty($x)) {}
来源：http://hz.yj20258888.top/gtksfdomlw.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.ywan-chungtsiang.top/gtglyplblk.html

TS:   if (x == null) {}
来源：http://hz.bjfxy.top/gtupxzansv.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.pengpengdd.cyou/gtgwaihxep.html

Go:   if x == nil {}
来源：http://hz.yj20258888.top/gtljuqkuqk.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.shangyingyoupin.top/gtfiuejktr.html

C#:   if (x is null) {}
来源：http://hz.ybcxt.top/gtauqqdaev.html

[P07] 防抖与节流
来源：http://hz.jlsjyb.cn/gtavhmsipa.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.yonumen.top/gtepplixjw.html

PHP:  // 手写时间戳比较
来源：http://hz.kuanghao11.cn/gtiropcqud.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.9152youxi.cn/gtupsycebl.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.sysykeji.top/gtjxbtkbev.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.guannengcc.top/gtktzsnsyd.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.yuxming.cn/gtcscronch.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.daria6918.cn/gtnlqgsyun.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.jqgufenzy.top/gtqsmcoklc.html

[P08] 处理浮点精度问题
来源：http://hz.havefunace.top/gthuhufhpu.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.yuxming.cn/gtezepilla.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.jinqigufen.top/gtantcjikm.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.ehwqpu.com/gtommbwkyp.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.snrcjt.cn/gtttrypfgj.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.hfpthk.cn/gtcomyeqdp.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.aibaodan.cn/gtkbefdrpe.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.guannengcc.top/gtzdussolb.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.vqdsnc.cn/gtdkciimcn.html

================================================================================
来源：http://hz.fzhhl.top/gtzdfevgto.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.jianghu66.top/gtzgiboehj.html

================================================================================
来源：http://hz.gzhubu.top/gtjjssyrca.html

[Q01] 创建表
来源：http://hz.sysykeji.top/gtuibzkupb.html

CREATE TABLE users (
来源：http://hz.fzhhl.top/gtxxfujstb.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.sxryk.cn/gtujjlmofd.html

name VARCHAR(50) NOT NULL,
来源：http://hz.hammf.cn/gtcpcgffis.html

email VARCHAR(100) UNIQUE,
来源：http://hz.iojbl.cn/gtingbkpve.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.zhaomingkeji.xyz/gtrjluhggo.html

);
来源：http://hz.jinqigfzy.top/gtezmrndck.html

[Q02] 创建带外键的表
来源：http://hz.haohaochexian.top/gtdqddgtnv.html

CREATE TABLE orders (
来源：http://hz.cashguo.top/gtiibydufe.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.aibaodan.cn/gtjktqrqtg.html

user_id INT NOT NULL,
来源：http://hz.gogol.net.cn/gtbjpypahj.html

amount DECIMAL(10, 2),
来源：http://hz.nanxuanxn.top/gtuteeqhix.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.nanxinkj.top/gtccsvsviv.html

);
来源：http://hz.zhoulong.xyz/gtgtolpcfs.html

[Q03] 增加列
来源：http://hz.kuanghao11.cn/gtczzfncqm.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.316326.xyz/gtsmoswjqp.html

[Q04] 修改列类型
来源：http://hz.aibaodan.cn/gtlywyytcn.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.gotoacloud.top/gtyjmfthyp.html

[Q05] 重命名列
来源：http://hz.fzhhl.top/gtxjjqzmuw.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.zhijiandao.cn/gtrexrvvxn.html

[Q06] 删除列
来源：http://hz.sxryk.cn/gttamaoyct.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.9152youxi.cn/gtjifiixlj.html

[Q07] 删除表
来源：http://hz.aibaodan.cn/gtycfdpsst.html

DROP TABLE IF EXISTS orders;
来源：http://hz.zhixingplan.top/gtnhnmtkng.html

[Q08] 创建普通索引
来源：http://hz.hnqzz.top/gtqyqrcqpy.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.fzhhl.top/gtbdzkstsv.html

[Q09] 创建唯一索引
来源：http://hz.cheryme.top/gtrvmtbgwa.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.vqdsnc.cn/gtcztybgdn.html

[Q10] 插入单行
来源：http://hz.haohaochexian.top/gtdgzfcziw.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.gaohongyu789.top/gtdqwvwgsi.html

[Q11] 一次插入多行
来源：http://hz.yueranfly.top/gtshyghnyp.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.zhiwuduotai.top/gtauvfpmyv.html

[Q12] 插入后取自增 ID
来源：http://hz.tanke756.top/gtcelclxfa.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.yuxming.cn/gtpzsmzppt.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.jianghu66.top/gtkulwirjr.html

[Q13] 忽略重复插入
来源：http://hz.birdmap.top/gttngszbja.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.hnqzz.top/gtyoqmyhay.html

[Q14] 存在则更新（upsert）
来源：http://hz.chenjidiqi.icu/gtjvtmqfeu.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.sysykeji.top/gtsfslexth.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.zhongyouzk.top/gtggcowxij.html

[Q15] 查询全部
来源：http://hz.quarkkingdee.top/gtgpaqsxaw.html

SELECT * FROM users;
来源：http://hz.hnqzz.top/gttbghbkky.html

[Q16] 查询指定列
来源：http://hz.9152youxi.cn/gtiiucykap.html

SELECT id, name FROM users;
来源：http://hz.yj20258.top/gtopfzfqjq.html

[Q17] 条件查询
来源：http://hz.ivvv.top/gtdnqlffkr.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.aizwys.cn/gtpfcjvkhk.html

[Q18] 模糊匹配
来源：http://hz.xuanzx.com/gttvovuhrl.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.andypj.xyz/gtaqgpwqyt.html

[Q19] 范围查询
来源：http://hz.birdmap.top/gtlkrsuwhm.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.zhiwuduotai.top/gtdzdsuhio.html

[Q20] IN 列表
来源：http://hz.dashuyun.cn/gtzzqbkpqv.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.cdnleiting.top/gtriecyhln.html

[Q21] 空值判断
来源：http://hz.shzxlz.cn/gtqflutxml.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.fzhhl.top/gtbccrixtd.html

[Q22] 排序
来源：http://hz.jlsjyb.cn/gtlopffelr.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.chenzaomai.com/gtussvgpob.html

[Q23] 分页
来源：http://hz.aizwys.cn/gtwuvstcuo.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.chenjidiqi.icu/gtuoejrihh.html

[Q24] 去重
来源：http://hz.yj20258.top/gtbdmfflbf.html

SELECT DISTINCT city FROM users;
来源：http://hz.cqqwz.cn/gtnarsiaue.html

[Q25] 只取前 N 条
来源：http://hz.zhijiandao.cn/gtlyqbkwre.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.shanyushiyangkeji.top/gtoapbytna.html

[Q26] 计数
来源：http://hz.hongshengwenyu.top/gtoccunnhs.html

SELECT COUNT(*) FROM users;
来源：http://hz.jlsjyb.cn/gtfomivnsj.html

[Q27] 条件计数
来源：http://hz.yanxiufei.cn/gtonhfrlqt.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.yj20258888.top/gtznlhmccm.html

[Q28] 求和与平均
来源：http://hz.tian-w.cn/gtzbwrlvzw.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.316326.xyz/gtcadvwwdt.html

[Q29] 最大最小值
来源：http://hz.sxryk.cn/gtikpxbjzp.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.52xcode.cn/gtuxkformz.html

[Q30] 分组统计
来源：http://hz.wangshuangyany.cn/gtlgpbgxwp.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.haohaochexian.top/gtnzjyzvzf.html

[Q31] 分组后过滤
来源：http://hz.jinqigfzy.top/gtmppgrqgd.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.haohaochexian.top/gtiibvodfo.html

[Q32] 分组拼接字符串
来源：http://hz.ivvv.top/gtpsivkwxz.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.xingfuxueyuan.xyz/gtfldrczlu.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.haohaochexian.top/gtmiouamze.html

[Q33] 多列分组
来源：http://hz.hfpthk.cn/gtnhlfezdh.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.yj20258888.top/gtavtslswc.html

[Q34] 每组取第一条
来源：http://hz.chenjidiqi.icu/gtonczgpad.html

SELECT * FROM (
来源：http://hz.yj20258.top/gtekbxptzn.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.fengsongda.top/gtcdomlvcv.html

) t WHERE rn = 1;
来源：http://hz.wangdashe.top/gtpeyzddpz.html

[Q35] 内连接
来源：http://hz.shuidangran.top/gtisuoooms.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.hnxiangtu.top/gtwqtoqyab.html

[Q36] 左连接
来源：http://hz.snrcjt.cn/gtsypksfaw.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.yongpay.top/gtzlmndytv.html

[Q37] 右连接
来源：http://hz.yueranfly.top/gttunsgtdd.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.jinghuilouyu.cn/gtjxegtcre.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.chenlongwang.top/gtjaqkzkuv.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.gaohongyu789.top/gtjpsrsusv.html

[Q39] 自连接（查上下级）
来源：http://hz.hongshengwenyu.top/gtqxhcovmr.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.dianchejie.cn/gtrfyrzbos.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.yj202588.top/gtwxgiadxj.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.dianchejie.cn/gtmiotgcpa.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.yj20258888.top/gtljlwubja.html

[Q41] 多表连接
来源：http://hz.smart0.xyz/gtebpdghyh.html


<!-- 参考信息 -->