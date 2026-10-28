代发 wailian999

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.sysykeji.top/gtoxppamso.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.quarkkingdee.top/gtvzvorddo.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.xziqi.cn/gtqhtibyxf.html

Ruby: a.gcd(b)
来源：http://hz.haohaochexian.top/gtbfveqgmi.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.fengsongda.top/gtvntendsf.html

[N06] 判断回文字符串
来源：http://hz.haohaochexian.top/gtdptxurpl.html

Py:   s == s[::-1]
来源：http://hz.gzhubu.top/gtzfparcbc.html

PHP:  $s === strrev($s);
来源：http://hz.ivvv.top/gtkkbmvhfh.html

JS:   s === [...s].reverse().join("")
来源：http://hz.daria6918.cn/gtxgynjoik.html

TS:   s === [...s].reverse().join("")
来源：http://hz.vqdsnc.cn/gtlckoyjkz.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.jqgufenzy.top/gtwoyvzpro.html

Go:   // 双指针从两端比较
来源：http://hz.yvedp.cn/gtqjtxxrpv.html

Ruby: s == s.reverse
来源：http://hz.tanke756.top/gtzmpwtbyf.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.snrcjt.cn/gtoybykojm.html

[N07] 两数之和（返回下标）
来源：http://hz.birdmap.top/gtowxmiuji.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.yongpay.top/gtixvqlytt.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.hywenlv.cn/gtsoqxzots.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.shuidangran.top/gtafogcitj.html

TS:   // 手写 Map<string, number>
来源：http://hz.dashuyun.cn/gtrmbleuxt.html

Java: // 手写 HashMap
来源：http://hz.sweek.top/gtqegacaah.html

Go:   // 手写 map[int]int
来源：http://hz.redwolf501.top/gthbzimnjo.html

Ruby: // 手写 Hash
来源：http://hz.yvedp.cn/gtjckpgtxk.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.shanyushiyangtech.top/gtpjyfzcll.html

[N08] 生成全排列
来源：http://hz.mhx1999.top/gtkczbxgin.html

Py:   itertools.permutations(arr)
来源：http://hz.aizwys.cn/gtgbjvjtfc.html

PHP:  // 手写递归交换
来源：http://hz.yueranfly.top/gtsfdhhogv.html

JS:   // 手写回溯递归
来源：http://hz.nanxinkj.top/gtmrprmtsa.html

TS:   // 手写回溯递归
来源：http://hz.vqdsnc.cn/gtlqbhlrwc.html

Java: // 手写回溯递归
来源：http://hz.yj20258888.top/gtbqephxxf.html

Go:   // 手写回溯递归
来源：http://hz.hongshengwenyu.top/gtnlhvrvou.html

Ruby: arr.permutation.to_a
来源：http://hz.yj20258.top/gtecmktvur.html

C#:   // 手写回溯递归
来源：http://hz.shuidangran.top/gtdibpbdqx.html

[N09] 栈与队列
来源：http://hz.zdqjudy.top/gtlfjgdxua.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.shzxlz.cn/gtkiztdkyp.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.andypj.xyz/gtvvmqpxjs.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.ivvv.top/gthqdxnipz.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.daria6918.cn/gtucajghbl.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.shanyushiyangtech.top/gtbuhdtuzo.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.xziqi.cn/gtjcqkqpbc.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.ppjwa.cn/gteecmrdgv.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.daria6918.cn/gteilkoomj.html

[N10] 链表节点定义
来源：http://hz.gogol.net.cn/gtxsklmxov.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.chenjidiqi.icu/gtjkqcvwga.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.jinyuanbaomall.cn/gtebmiqfkv.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.yangfankeji.com/gtdvruvszd.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.guowangkeji.top/gtxdxdofgw.html

Java: class Node { int v; Node next; }
来源：http://hz.jinyuanbaomall.cn/gtekxcjdur.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.zycfv.cn/gtojosbobr.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.aibaodan.cn/gtfdfklpxl.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.pycfn.com/gtsbihpckj.html

[N11] 二叉树中序遍历
来源：http://hz.xylfe.cn/gtxhbsbslh.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.gzhubu.top/gtdgvnlxgk.html

PHP:  // 手写递归函数
来源：http://hz.vqdsnc.cn/gttguuxuor.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.guowangkeji.top/gtogxdwwzv.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.shuidangran.top/gtikarzxel.html

Java: // 手写递归
来源：http://hz.zhixingplan.top/gthtaxcsmq.html

Go:   // 手写递归
来源：http://hz.cucudq.cn/gtasavkznx.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.sysykeji.top/gturveidxe.html

C#:   // 手写递归
来源：http://hz.yuxming.cn/gtlaqcclyc.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.0kj1m.cn/gtngpcjghp.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.hnqzz.top/gtclyphevk.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.kuanghao11.cn/gtdjsyocpf.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.ybcxt.top/gtdirovfgz.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.shangyingyoupin.top/gtdgqtxfkn.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.gotoacloud.top/gtxocglzkg.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.sufxvd.cn/gtbgcgqxjk.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.ehwqpu.com/gtlnmqhoog.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.hongshengwenyu.top/gtkktgzwls.html

================================================================================
来源：http://hz.snrcjt.cn/gtujzxsbje.html

O. 并发与异步
来源：http://hz.gzhubu.top/gtolrtwaga.html

================================================================================
来源：http://hz.aizwys.cn/gtqpflyfzl.html

[O01] 启动一个线程
来源：http://hz.tianlin.xyz/gtfizxkxhi.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.kuanghao11.cn/gtvrlesgbf.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.jlsjyb.cn/gtcsjrgjrf.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.hongshengwenyu.top/gtlzujcjvw.html

TS:   // 同 JS
来源：http://hz.316326.xyz/gtrpxsicvh.html

Java: new Thread(() -> f()).start()
来源：http://hz.zycfv.cn/gtxxmnyfzx.html

Go:   go f()
来源：http://hz.yuxming.cn/gtdlqpybnc.html

Ruby: Thread.new { f }
来源：http://hz.chenlongwang.top/gtdblulivl.html

C#:   Task.Run(() => F());
来源：http://hz.ydjk.org.cn/gtjcicbxtj.html

[O02] 使用线程池
来源：http://hz.gaohongyu789.top/gtemgfnsds.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.hnqzz.top/gtctadpibm.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.zhijiandao.cn/gtdxuhzabw.html

JS:   // worker_threads 线程池
来源：http://hz.jinyuanbaomall.cn/gtflhqpcvi.html

TS:   // worker_threads 线程池
来源：http://hz.jinyuanbaomall.cn/gtwrmqcksn.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.jyoumei.cn/gtsohssrei.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.bjfxy.top/gtpupdobni.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.xziqi.cn/gtpvvrfgsf.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.vqdsnc.cn/gtknegvmxk.html

[O03] 加锁保护共享数据
来源：http://hz.gogol.net.cn/gtgsvkxkja.html

Py:   with lock: shared += 1
来源：http://hz.jqgufenzy.top/gtyzxgjkwd.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.jinqigufen.top/gtlltqfyks.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.hfpthk.cn/gthmbmmvzl.html

TS:   // 同 JS
来源：http://hz.zycfv.cn/gtntjprxob.html

Java: synchronized (this) { shared++; }
来源：http://hz.yanxiufei.cn/gtlbnghszf.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.xziqi.cn/gtxvltzske.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.jinghuilouyu.cn/gtfrocwcqr.html

C#:   lock (gate) { shared++; }
来源：http://hz.shanyushiyangkeji.top/gtxctmubci.html

[O04] 定义异步函数并等待
来源：http://hz.aizwys.cn/gtxspzijpr.html

Py:   async def f():⏎    await g()
来源：http://hz.tianlin.xyz/gtbytydepn.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.zhongyouzk.top/gtvkosaywr.html

JS:   async function f() { await g(); }
来源：http://hz.vqdsnc.cn/gtrrjzgtky.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.52xcode.cn/gtclmenear.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.ehwqpu.com/gtautntegn.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.xinyue.icu/gtkagmdvpn.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.jinyuanbaomall.cn/gtipdtfvsv.html

C#:   async Task F() { await G(); }
来源：http://hz.hongshengwenyu.top/gtflpwfyzq.html

[O05] 并发执行并等待全部完成
来源：http://hz.fengsongda.top/gtcqfhfzgn.html

Py:   asyncio.gather(*tasks)
来源：http://hz.zhongyouzk.top/gttxmxnxqk.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.zhijiandao.cn/gtjeezkkcx.html

JS:   await Promise.all(tasks)
来源：http://hz.fengsongda.top/gtduqfruqd.html

TS:   await Promise.all(tasks)
来源：http://hz.aizwys.cn/gtbeidxswp.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.wangdashe.top/gtreonziwx.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.yonumen.top/gtsayceehs.html

Ruby: threads.map(&:join)
来源：http://hz.yj20258888.top/gtitoukenf.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.xinyue.icu/gtmqbgxbaa.html

[O06] 使用进程池
来源：http://hz.zhijiandao.cn/gtqmtjgzlp.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.vqdsnc.cn/gtnyihxuws.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.yj202588.top/gtyyeajxwp.html

JS:   // child_process / cluster 模块
来源：http://hz.nanxinkj.top/gttwofhimf.html

TS:   // child_process / cluster 模块
来源：http://hz.yvedp.cn/gtxmhfjwgs.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.meibo888.top/gtwmretlij.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.yj20258.top/gttvpzmhwb.html

Ruby: // fork 块
来源：http://hz.gaohongyu789.top/gtoarolobk.html

C#:   Parallel.For
来源：http://hz.kuanghao11.cn/gthehhfbhc.html

================================================================================
来源：http://hz.xinyue.icu/gtzysybeeq.html

P. 常用工具函数
来源：http://hz.chenlongwang.top/gtkfdkzgca.html

================================================================================
来源：http://hz.tian-w.cn/gttlreisbm.html

[P01] 生成 UUID
来源：http://hz.shuidangran.top/gtsvitccni.html

Py:   str(uuid.uuid4())
来源：http://hz.xziqi.cn/gtzkkwowna.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.316326.xyz/gtccukvbfy.html

JS:   crypto.randomUUID()
来源：http://hz.ybcxt.top/gtbvddkidd.html

TS:   crypto.randomUUID()
来源：http://hz.xuetiantiany.cn/gtyeejhmud.html

Java: UUID.randomUUID().toString()
来源：http://hz.hammf.cn/gtqkmgyeon.html

Go:   // 用 github.com/google/uuid
来源：http://hz.mhx1999.top/gtzckzwhrf.html

Ruby: SecureRandom.uuid
来源：http://hz.zhiwuduotai.top/gtifxdjvuu.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.xuanzx.com/gtbdhmvayi.html

[P02] MD5 / SHA256 摘要
来源：http://hz.chenjidiqi.icu/gtjylydsoi.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.hnqzz.top/gtzfxjlbme.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.fengsongda.top/gtvghposrx.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.cheryme.top/gttcziijin.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.zhoulong.xyz/gtujlflqtt.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.ybcxt.top/gtkrobhlaf.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.zhoulong.xyz/gtenlsmmhn.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.gzhubu.top/gtydhlicch.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.tian-w.cn/gtykcbdllt.html

[P03] 生成短随机字符串
来源：http://hz.jinqigfzy.top/gtcizgumlq.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.yvedp.cn/gtanglpecn.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.aibaodan.cn/gtpxgxdkmq.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.kuanghao11.cn/gttgqyqlsz.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.redwolf501.top/gtflyignfj.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.zhoulong.xyz/gtkpcejjwr.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.fengsongda.top/gthmwmzngl.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.shanyushiyangkeji.top/gtzbmnympq.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.xuanzx.com/gtqpeqcckg.html

[P04] 求长度
来源：http://hz.gzhubu.top/gtcwtlhwfb.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.yueranfly.top/gtxxwzucjy.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.cqqwz.cn/gtypugydnp.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.nanxinkj.top/gtcfexzrus.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.jyoumei.cn/gtgnlpiunj.html

Java: list.size();  map.size();  s.length()
来源：http://hz.c1oappe.top/gttfjxoxjq.html

Go:   len(arr);  len(m)
来源：http://hz.jinyuanbaomall.cn/gtpmwsiltq.html

Ruby: x.length;  x.size
来源：http://hz.gogol.net.cn/gtqndnafjh.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.yj20258.top/gtusscqsae.html

[P05] 判断两个对象内容是否相等
来源：http://hz.smart0.xyz/gtqsfeboeo.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.gogol.net.cn/gtiyqtoyot.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.gaohongyu789.top/gttrmrstvn.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.yongpay.top/gtkaabirsx.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.meibo888.top/gtlmiahhne.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.havefunace.top/gtsnfaykbm.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.yanxiufei.cn/gtmzlaavml.html

Ruby: a == b
来源：http://hz.xinyue.icu/gtbdftxlfs.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.yongpay.top/gtdvesnsxz.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.sxryk.cn/gtjcxokrwv.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.yanxiufei.cn/gtnmnnejcf.html

PHP:  if (empty($x)) {}
来源：http://hz.jianghu66.top/gtwxukdbdu.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.nanxinkj.top/gtxvwxlouk.html

TS:   if (x == null) {}
来源：http://hz.snrcjt.cn/gtjfgiuthj.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.svipenyu.cn/gtttaqhmqs.html

Go:   if x == nil {}
来源：http://hz.yvedp.cn/gtalgoynen.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.wangshuangyany.cn/gtetbskuub.html

C#:   if (x is null) {}
来源：http://hz.ppjwa.cn/gtkhvbsqmk.html

[P07] 防抖与节流
来源：http://hz.shanyushiyangkeji.top/gtndxzizlj.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.xziqi.cn/gtrncrxtmu.html

PHP:  // 手写时间戳比较
来源：http://hz.mhx1999.top/gtkrcqbmwj.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.snrcjt.cn/gtfsapceih.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.jqgfzy.top/gtjvqyurrj.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.iojbl.cn/gtfhshphjb.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.xylfe.cn/gtcjgwbiaf.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.cdnleiting.top/gtmhhkgdlb.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.yvedp.cn/gtqyecwpby.html

[P08] 处理浮点精度问题
来源：http://hz.mhx1999.top/gtjyjitwnd.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.meibo888.top/gtubpcvgzk.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.gotoacloud.top/gtgdfpydox.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.zdqjudy.top/gtfxpxefgr.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.pycfn.com/gtomzzhgwz.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.ybcxt.top/gtntxdbmrm.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.pengpengdd.cyou/gtfllykzsd.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.sysykeji.top/gtccjhldsk.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.wangdashe.top/gtznnoggdf.html

================================================================================
来源：http://hz.shzxlz.cn/gttwbokdqi.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.tian-w.cn/gtpoucjldv.html

================================================================================
来源：http://hz.gogol.net.cn/gtezufflru.html

[Q01] 创建表
来源：http://hz.aibaodan.cn/gthhulqcku.html

CREATE TABLE users (
来源：http://hz.hfpthk.cn/gtivdlegoo.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.chenzaomai.com/gticppnozu.html

name VARCHAR(50) NOT NULL,
来源：http://hz.pycfn.com/gtxxavrybc.html

email VARCHAR(100) UNIQUE,
来源：http://hz.snrcjt.cn/gtvreypkam.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.daria6918.cn/gtwuajrcog.html

);
来源：http://hz.yuanzhike.top/gtpptunwhr.html

[Q02] 创建带外键的表
来源：http://hz.xinyue.icu/gtqllzlxgy.html

CREATE TABLE orders (
来源：http://hz.hongshengwenyu.top/gtkmdeshud.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.zhaomingkeji.xyz/gtsrgfnoif.html

user_id INT NOT NULL,
来源：http://hz.daxiang520.top/gtgvrzlfqd.html

amount DECIMAL(10, 2),
来源：http://hz.zycfv.cn/gtncefsjmh.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.shanyushiyangkeji.top/gtlroflnbp.html

);
来源：http://hz.shanyushiyangkeji.top/gtqhvgxpiw.html

[Q03] 增加列
来源：http://hz.vqdsnc.cn/gtxebqcawp.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.shanyushiyangtech.top/gtqdxrnphd.html

[Q04] 修改列类型
来源：http://hz.xuetiantiany.cn/gtzfjbfxhn.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.fengsongda.top/gtkmaadwlj.html

[Q05] 重命名列
来源：http://hz.gzhubu.top/gtphwxeaii.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.yj202588.top/gtlhrjejgi.html

[Q06] 删除列
来源：http://hz.tanke756.top/gtnomgwqcn.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.cucudq.cn/gtpsgxwwlx.html

[Q07] 删除表
来源：http://hz.aibaodan.cn/gtalchuyom.html

DROP TABLE IF EXISTS orders;
来源：http://hz.sxryk.cn/gtnvnbbsjj.html

[Q08] 创建普通索引
来源：http://hz.cashguo.top/gtkgeicmkr.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.yj202588.top/gtkohdbfnu.html

[Q09] 创建唯一索引
来源：http://hz.zdqjudy.top/gtdncvzryy.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.shanyushiyangtech.top/gtkblexuwv.html

[Q10] 插入单行
来源：http://hz.yonumen.top/gtklqmozxw.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.jianghu66.top/gtwdkehxvy.html

[Q11] 一次插入多行
来源：http://hz.jqgfzy.top/gtupgxhort.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.zhaomingkeji.xyz/gtpilvvnpz.html

[Q12] 插入后取自增 ID
来源：http://hz.xziqi.cn/gtzfuweyyd.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.yj202588.top/gtqpgjxrfq.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.cucudq.cn/gttndlqxru.html

[Q13] 忽略重复插入
来源：http://hz.gotoacloud.top/gtonumkcxk.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.xziqi.cn/gtrpbkvozr.html

[Q14] 存在则更新（upsert）
来源：http://hz.mhx1999.top/gtuhzzhtmn.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.daria6918.cn/gtfenhwckc.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.hnxiangtu.top/gtrremvmul.html

[Q15] 查询全部
来源：http://hz.guowangkeji.top/gtkykeraty.html

SELECT * FROM users;
来源：http://hz.yueranfly.top/gtecnymgtl.html

[Q16] 查询指定列
来源：http://hz.gzhubu.top/gtkunucfyb.html

SELECT id, name FROM users;
来源：http://hz.jianghu66.top/gthugjdulq.html

[Q17] 条件查询
来源：http://hz.yvedp.cn/gtriajpjms.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.xingfuxueyuan.xyz/gtxuynrcmf.html

[Q18] 模糊匹配
来源：http://hz.jinqigufen.top/gtknokapgw.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.yj202588.top/gtfjqwryeg.html

[Q19] 范围查询
来源：http://hz.jqgfzy.top/gthwyymsvj.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.fzhhl.top/gtetejzibr.html

[Q20] IN 列表
来源：http://hz.cheryme.top/gtdurwldce.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.jinqigfzy.top/gtyfssjjhv.html

[Q21] 空值判断
来源：http://hz.shzxlz.cn/gtbbpzfpuu.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.ybcxt.top/gtzguovfbl.html

[Q22] 排序
来源：http://hz.yongpay.top/gtgrxsdcqr.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.wangshuangyany.cn/gthtciwzvl.html

[Q23] 分页
来源：http://hz.hysaishi.cn/gtulotzfls.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.fzhhl.top/gtougpdxdf.html

[Q24] 去重
来源：http://hz.zhixingplan.top/gtcumyyvhw.html

SELECT DISTINCT city FROM users;
来源：http://hz.yj20258.top/gtuegvvpbw.html

[Q25] 只取前 N 条
来源：http://hz.jinqigfzy.top/gtkvsnvphl.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.ivvv.top/gthlpholvs.html

[Q26] 计数
来源：http://hz.dashuyun.cn/gtgxqedyoo.html

SELECT COUNT(*) FROM users;
来源：http://hz.zycfv.cn/gtxfpwfxaq.html

[Q27] 条件计数
来源：http://hz.yj20258888.top/gtsiwvsjfi.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.ybcxt.top/gtszzhjqzc.html

[Q28] 求和与平均
来源：http://hz.meibo888.top/gtmnefblan.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.jlsjyb.cn/gtkfobjvjo.html

[Q29] 最大最小值
来源：http://hz.yueranfly.top/gtnopwgqao.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.hysaishi.cn/gtircqerag.html

[Q30] 分组统计
来源：http://hz.zhijiandao.cn/gtxevzksiq.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.kuanghao11.cn/gtzgizmjnw.html

[Q31] 分组后过滤
来源：http://hz.wangshuangyany.cn/gtjmcbozuv.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.jinqigfzy.top/gtfotuimvd.html

[Q32] 分组拼接字符串
来源：http://hz.hammf.cn/gtsorumwqy.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.daria6918.cn/gtkvizunlh.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.yongpay.top/gtbmnkmplq.html

[Q33] 多列分组
来源：http://hz.yvedp.cn/gtbskgizzw.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.gogol.net.cn/gtpqabucoc.html

[Q34] 每组取第一条
来源：http://hz.gaohongyu789.top/gtnqlsdcap.html

SELECT * FROM (
来源：http://hz.xylfe.cn/gtcoqliulg.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.haohaochexian.top/gtqymyzysn.html

) t WHERE rn = 1;
来源：http://hz.kuanghao11.cn/gtituvcvjp.html

[Q35] 内连接
来源：http://hz.hnxiangtu.top/gtmfmmdzbd.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.yangfankeji.com/gtblrzblys.html

[Q36] 左连接
来源：http://hz.aizwys.cn/gtvdhssjed.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.chenjidiqi.icu/gtrjlcthps.html

[Q37] 右连接
来源：http://hz.smart0.xyz/gtkijiafke.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.aizwys.cn/gthdbwrlyq.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.nanxuanxn.top/gttgfnkklr.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.316326.xyz/gtfxmjlejp.html

[Q39] 自连接（查上下级）
来源：http://hz.vqdsnc.cn/gtgeasgvga.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.cucudq.cn/gtotdvdqwe.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.xinyue.icu/gtbdhojwuj.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.svipenyu.cn/gtcgcudjhk.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.chenlongwang.top/gteequjcdi.html

[Q41] 多表连接
来源：http://hz.zhoulong.xyz/gthmmekiun.html


<!-- 参考信息 -->