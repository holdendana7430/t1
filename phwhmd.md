代发 wailian999

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.zhixingplan.top/gtnyvzruah.html

[N06] 判断回文字符串
来源：http://hz.cucudq.cn/gtsuyzdqwk.html

Py:   s == s[::-1]
来源：http://hz.guowangkeji.top/gtnftpbqmm.html

PHP:  $s === strrev($s);
来源：http://hz.smart0.xyz/gtcstgzoos.html

JS:   s === [...s].reverse().join("")
来源：http://hz.yj202588.top/gtbktfkaim.html

TS:   s === [...s].reverse().join("")
来源：http://hz.yangfankeji.com/gtexaaswei.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.pycfn.com/gtawkvvwoo.html

Go:   // 双指针从两端比较
来源：http://hz.sweek.top/gtqzgawnxb.html

Ruby: s == s.reverse
来源：http://hz.xuanzx.com/gtgcvtcuhn.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.cqqwz.cn/gtifmeeice.html

[N07] 两数之和（返回下标）
来源：http://hz.zdqjudy.top/gtrdophrgu.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.xuanzx.com/gtwrfnbqwg.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.zhijiandao.cn/gtacbitspv.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.yvedp.cn/gtyquxkkpq.html

TS:   // 手写 Map<string, number>
来源：http://hz.shzxlz.cn/gtfkvccywc.html

Java: // 手写 HashMap
来源：http://hz.yueranfly.top/gtnesxazjp.html

Go:   // 手写 map[int]int
来源：http://hz.shanyushiyangkeji.top/gtwtvnoqyd.html

Ruby: // 手写 Hash
来源：http://hz.hammf.cn/gtaqhuvcdb.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.sysykeji.top/gtzhewwqop.html

[N08] 生成全排列
来源：http://hz.aibaodan.cn/gtbkejurxz.html

Py:   itertools.permutations(arr)
来源：http://hz.dashuyun.cn/gtwzsycqse.html

PHP:  // 手写递归交换
来源：http://hz.gzhubu.top/gtotwgespp.html

JS:   // 手写回溯递归
来源：http://hz.hfpthk.cn/gtdatrqkdm.html

TS:   // 手写回溯递归
来源：http://hz.meibo888.top/gtcvwvjlgz.html

Java: // 手写回溯递归
来源：http://hz.xziqi.cn/gtmcemqqcg.html

Go:   // 手写回溯递归
来源：http://hz.sxryk.cn/gtsmtyjgei.html

Ruby: arr.permutation.to_a
来源：http://hz.9152youxi.cn/gtcvxgplhj.html

C#:   // 手写回溯递归
来源：http://hz.iojbl.cn/gtjfbtzyla.html

[N09] 栈与队列
来源：http://hz.xuetiantiany.cn/gtcuaaonls.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.yj202588.top/gtfowtwtws.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.daxiang520.top/gtuzsykxdf.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.jqgfzy.top/gtyqxwqxmb.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.xziqi.cn/gtbhdtkbtv.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.hongshengwenyu.top/gtdkzxbzys.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.kuanghao11.cn/gthhxwuxyv.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.jiagoushi.top/gtbqqbtrfl.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.jinghuilouyu.cn/gtirvidyde.html

[N10] 链表节点定义
来源：http://hz.hongshengwenyu.top/gtrtmmddro.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.sxryk.cn/gtfaajdrlq.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.cheryme.top/gttqcworqw.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.ehwqpu.com/gtrwhszine.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.zhengqikj.top/gtlgpdhppi.html

Java: class Node { int v; Node next; }
来源：http://hz.fengsongda.top/gthuipwblz.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.xziqi.cn/gtexroxoln.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.yj20258888.top/gtctqjyfpp.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.quarkkingdee.top/gtxmqswzct.html

[N11] 二叉树中序遍历
来源：http://hz.daria6918.cn/gtakpisjqx.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.cheryme.top/gtjoheqgtt.html

PHP:  // 手写递归函数
来源：http://hz.yueranfly.top/gtihqifxor.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.tian-w.cn/gtrjcjatiw.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.xinyue.icu/gtdiehhshz.html

Java: // 手写递归
来源：http://hz.vqdsnc.cn/gtrrhfdruo.html

Go:   // 手写递归
来源：http://hz.yanxiufei.cn/gthcwlnzhf.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.smart0.xyz/gtvxuwbkol.html

C#:   // 手写递归
来源：http://hz.wangshuangyany.cn/gtnfgnvhdx.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.yj202588.top/gtcnrprmod.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.yj20258888.top/gtqpmjtugb.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.fzhhl.top/gteuqgitgr.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.ywan-chungtsiang.top/gtorgtppqy.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.xziqi.cn/gtifjtkipo.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.guowangkeji.top/gthyfsljmx.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.xziqi.cn/gtcziizbdn.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.yangfankeji.com/gtlizndhlg.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.shanyushiyangtech.top/gtqrqvlyfa.html

================================================================================
来源：http://hz.haohaochexian.top/gtfdczsuch.html

O. 并发与异步
来源：http://hz.yongpay.top/gttmtrimbm.html

================================================================================
来源：http://hz.52xcode.cn/gtarvpxgch.html

[O01] 启动一个线程
来源：http://hz.hongshengwenyu.top/gtqsiohsxm.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.chenlongwang.top/gtgrtbzdci.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.yonumen.top/gtyelorwyd.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.yvedp.cn/gtjjqqaubn.html

TS:   // 同 JS
来源：http://hz.vqdsnc.cn/gtwwyppgso.html

Java: new Thread(() -> f()).start()
来源：http://hz.xingfuxueyuan.xyz/gtizqzwnmd.html

Go:   go f()
来源：http://hz.ydzc1.top/gtlpztzpdf.html

Ruby: Thread.new { f }
来源：http://hz.c1oappe.top/gtfcoomewg.html

C#:   Task.Run(() => F());
来源：http://hz.shangyingyoupin.top/gtqwsufinp.html

[O02] 使用线程池
来源：http://hz.cashguo.top/gtbljnrvyk.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.zycfv.cn/gthbdaejru.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.9152youxi.cn/gtbesjjejl.html

JS:   // worker_threads 线程池
来源：http://hz.tianlin.xyz/gtymshxknc.html

TS:   // worker_threads 线程池
来源：http://hz.yongpay.top/gtxzpyphbs.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.pycfn.com/gttanyqezi.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.cucudq.cn/gtebplsasf.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.zhoulong.xyz/gtqtqdxgrd.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.guowangkeji.top/gtfodlkzqk.html

[O03] 加锁保护共享数据
来源：http://hz.kuanghao11.cn/gtvplgixbi.html

Py:   with lock: shared += 1
来源：http://hz.tanke756.top/gtwlfwyckr.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.shanyushiyangkeji.top/gtomjdtvem.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.daria6918.cn/gtcivrsklg.html

TS:   // 同 JS
来源：http://hz.9152youxi.cn/gteshwxioy.html

Java: synchronized (this) { shared++; }
来源：http://hz.tian-w.cn/gtnrtmawrm.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.aibaodan.cn/gtjcfwlkpi.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.chenzaomai.com/gtqxcrbrnf.html

C#:   lock (gate) { shared++; }
来源：http://hz.hfpthk.cn/gtiwoemtch.html

[O04] 定义异步函数并等待
来源：http://hz.shanyushiyangkeji.top/gtrwthvuuo.html

Py:   async def f():⏎    await g()
来源：http://hz.52xcode.cn/gtpvqxakcm.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.jinghuilouyu.cn/gtrlhqqzbp.html

JS:   async function f() { await g(); }
来源：http://hz.feifeiyinyue.top/gtbohtaztt.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.fzhhl.top/gthsfzqcij.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.nanxuanxn.top/gtwsqvvbfe.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.shangyingyoupin.top/gtlkqulllk.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.zhixingplan.top/gtdvwziybz.html

C#:   async Task F() { await G(); }
来源：http://hz.xuetiantiany.cn/gtxhtxslpr.html

[O05] 并发执行并等待全部完成
来源：http://hz.pycfn.com/gtuenjxvuq.html

Py:   asyncio.gather(*tasks)
来源：http://hz.jianghu66.top/gtrvuosnaq.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.yuxming.cn/gtmgwdzngb.html

JS:   await Promise.all(tasks)
来源：http://hz.jinqigufen.top/gtoqcyojec.html

TS:   await Promise.all(tasks)
来源：http://hz.cashguo.top/gtwrihntti.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.yangfankeji.com/gtncsbsqqs.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.yvedp.cn/gtepsswkec.html

Ruby: threads.map(&:join)
来源：http://hz.mhx1999.top/gtppjrhslj.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.quarkkingdee.top/gtgtsedmbl.html

[O06] 使用进程池
来源：http://hz.yueranfly.top/gtxptpswhd.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.hfpthk.cn/gtjoxwnxvd.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.chenlongwang.top/gtftadbuul.html

JS:   // child_process / cluster 模块
来源：http://hz.ydzc1.top/gtczkgmcmk.html

TS:   // child_process / cluster 模块
来源：http://hz.ppjwa.cn/gtazvpimcy.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.jinghuilouyu.cn/gtnxpgxhvf.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.jinghuilouyu.cn/gtzjzqjjli.html

Ruby: // fork 块
来源：http://hz.cheryme.top/gtizfqiqia.html

C#:   Parallel.For
来源：http://hz.ydzc1.top/gtlyumyjcc.html

================================================================================
来源：http://hz.xylfe.cn/gtsafhveyf.html

P. 常用工具函数
来源：http://hz.dianchejie.cn/gtdyaclyed.html

================================================================================
来源：http://hz.jyoumei.cn/gtphlwlkfy.html

[P01] 生成 UUID
来源：http://hz.smart0.xyz/gtexkarxzn.html

Py:   str(uuid.uuid4())
来源：http://hz.hysaishi.cn/gtxwranwxb.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.chenlongwang.top/gtemmnaxka.html

JS:   crypto.randomUUID()
来源：http://hz.meibo888.top/gtwzhijfya.html

TS:   crypto.randomUUID()
来源：http://hz.havefunace.top/gtytokmlol.html

Java: UUID.randomUUID().toString()
来源：http://hz.ydzc1.top/gtkwyrjqas.html

Go:   // 用 github.com/google/uuid
来源：http://hz.sufxvd.cn/gtyfrrewnx.html

Ruby: SecureRandom.uuid
来源：http://hz.svipenyu.cn/gtwhrtjeww.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.mhx1999.top/gteqkdkmte.html

[P02] MD5 / SHA256 摘要
来源：http://hz.aibaodan.cn/gtneqmpcqo.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.sufxvd.cn/gtaimunbwa.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.daxiang520.top/gtpmspiqre.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.cheryme.top/gtpsqsdvpm.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.hywenlv.cn/gtpkhkhram.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.shzxlz.cn/gtloouitjr.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.pycfn.com/gtadjyjxgm.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.guowangkeji.top/gtuvjgbemw.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.fengsongda.top/gtdqxfeobe.html

[P03] 生成短随机字符串
来源：http://hz.quarkkingdee.top/gtiwefvhhi.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.ydjk.org.cn/gtwzdgeize.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.pycfn.com/gthknseijs.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.gzhubu.top/gttxebhjgd.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.quarkkingdee.top/gtixvniopq.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.pengpengdd.cyou/gtjadzqxnf.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.ywan-chungtsiang.top/gtnvztdkjn.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.redwolf501.top/gttzmvxnnt.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.hnqzz.top/gtvqqozpib.html

[P04] 求长度
来源：http://hz.shangyingyoupin.top/gtwiabxzuy.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.zhaomingkeji.xyz/gtibbskyst.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.jyoumei.cn/gtfdedccwz.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.gotoacloud.top/gtbjluqjzx.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.zhoulong.xyz/gtgyskcvte.html

Java: list.size();  map.size();  s.length()
来源：http://hz.wangdashe.top/gtpxbyjsmc.html

Go:   len(arr);  len(m)
来源：http://hz.aibaodan.cn/gtaelqizyd.html

Ruby: x.length;  x.size
来源：http://hz.aizwys.cn/gtebtnxkkw.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.hfpthk.cn/gtmvolvpwj.html

[P05] 判断两个对象内容是否相等
来源：http://hz.xuanzx.com/gtnzvzhddz.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.chenlongwang.top/gtahgpjmyg.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.yj20258888.top/gtwlxobkac.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.shuidangran.top/gtkmihjtji.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.shuidangran.top/gtwrexzmfx.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.cdnleiting.top/gtwgwttmbv.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.vqdsnc.cn/gtawtodjcc.html

Ruby: a == b
来源：http://hz.0kj1m.cn/gtnllfiftg.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.pycfn.com/gtnbnffijw.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.0kj1m.cn/gtnhzvjqpb.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.zhaomingkeji.xyz/gtixrvlpfu.html

PHP:  if (empty($x)) {}
来源：http://hz.iojbl.cn/gtizvwstfr.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.shuidangran.top/gtzvsllaoa.html

TS:   if (x == null) {}
来源：http://hz.52xcode.cn/gtqrowfxhu.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.ppjwa.cn/gtxqqffgvy.html

Go:   if x == nil {}
来源：http://hz.shangyingyoupin.top/gtfxquqffi.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.zhiwuduotai.top/gtcxzbmqds.html

C#:   if (x is null) {}
来源：http://hz.nanxinkj.top/gteidwbkkh.html

[P07] 防抖与节流
来源：http://hz.nwbrower.top/gtlkxjvgmq.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.zhoulong.xyz/gtiijgtpwq.html

PHP:  // 手写时间戳比较
来源：http://hz.daria6918.cn/gtfvvsrlsh.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.sxryk.cn/gtkcnksdtf.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.zhengqikj.top/gthfejbxgj.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.dashuyun.cn/gtznwgagtt.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.wangdashe.top/gtexgllazx.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.redwolf501.top/gtpkzeoljh.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.jinyuanbaomall.cn/gttasvlvsf.html

[P08] 处理浮点精度问题
来源：http://hz.cheryme.top/gthrlwibna.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.cqqwz.cn/gthabcllci.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.yueranfly.top/gtilhtpfou.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.zhijiandao.cn/gttzijazcl.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.hnxiangtu.top/gtddbugwwk.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.pengpengdd.cyou/gtvywvavsz.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.chenjidiqi.icu/gtuznqprnw.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.gotoacloud.top/gtilwzjifu.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.0kj1m.cn/gtnwfflujw.html

================================================================================
来源：http://hz.nanxuanxn.top/gtwisfhilc.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.hongshengwenyu.top/gtjvnihgts.html

================================================================================
来源：http://hz.shanyushiyangkeji.top/gttcbwmgic.html

[Q01] 创建表
来源：http://hz.ydzc1.top/gtfqlctyaa.html

CREATE TABLE users (
来源：http://hz.52xcode.cn/gtcwzyiidc.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.aibaodan.cn/gthbyjgvzk.html

name VARCHAR(50) NOT NULL,
来源：http://hz.fengsongda.top/gtvjmhkffd.html

email VARCHAR(100) UNIQUE,
来源：http://hz.mhx1999.top/gtqpjgboey.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.jianghu66.top/gtmblqztnw.html

);
来源：http://hz.sweek.top/gtaxlsodrt.html

[Q02] 创建带外键的表
来源：http://hz.yonumen.top/gtbhqpvefr.html

CREATE TABLE orders (
来源：http://hz.9152youxi.cn/gtkznawhjb.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.yueranfly.top/gtkakddzqh.html

user_id INT NOT NULL,
来源：http://hz.hywenlv.cn/gtvdeuqxbz.html

amount DECIMAL(10, 2),
来源：http://hz.hnxiangtu.top/gtzvomkavm.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.svipenyu.cn/gtpzyztktm.html

);
来源：http://hz.hongshengwenyu.top/gttieptyty.html

[Q03] 增加列
来源：http://hz.iojbl.cn/gtnxshqgvh.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.xuanzx.com/gtiuiopufh.html

[Q04] 修改列类型
来源：http://hz.hywenlv.cn/gtskfbkbrg.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.zhengqikj.top/gtbtsikygj.html

[Q05] 重命名列
来源：http://hz.nanxuanxn.top/gtxzlldeyg.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.zhengqikj.top/gtwimqlhvu.html

[Q06] 删除列
来源：http://hz.daxiang520.top/gtuyahmntf.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.zycfv.cn/gtgkbedeai.html

[Q07] 删除表
来源：http://hz.xylfe.cn/gtwdqxcmio.html

DROP TABLE IF EXISTS orders;
来源：http://hz.yuxming.cn/gtfphssabm.html

[Q08] 创建普通索引
来源：http://hz.nanxuanxn.top/gtyliwtwhl.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.cashguo.top/gtzomweqdq.html

[Q09] 创建唯一索引
来源：http://hz.9152youxi.cn/gtarczzmhq.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.52xcode.cn/gtrcclntsv.html

[Q10] 插入单行
来源：http://hz.yonumen.top/gtcgsrsvvy.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.nwbrower.top/gtgtxgknmh.html

[Q11] 一次插入多行
来源：http://hz.feifeiyinyue.top/gtjqbufeio.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.wangshuangyany.cn/gtoyhepgzx.html

[Q12] 插入后取自增 ID
来源：http://hz.yj202588.top/gtfwvffcwv.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.birdmap.top/gttoopmdpa.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.shuidangran.top/gtztkkbcsl.html

[Q13] 忽略重复插入
来源：http://hz.pengpengdd.cyou/gtfaqglvxx.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.gaohongyu789.top/gtzvweboyn.html

[Q14] 存在则更新（upsert）
来源：http://hz.hnqzz.top/gtgtuczkzw.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.fengsongda.top/gtfajicowm.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.fzhhl.top/gtwzjphynx.html

[Q15] 查询全部
来源：http://hz.daria6918.cn/gtykkcfalp.html

SELECT * FROM users;
来源：http://hz.sufxvd.cn/gtdyzvldax.html

[Q16] 查询指定列
来源：http://hz.hnqzz.top/gtdcxhugqf.html

SELECT id, name FROM users;
来源：http://hz.jinghuilouyu.cn/gthnoielft.html

[Q17] 条件查询
来源：http://hz.ehwqpu.com/gtbjbvklhm.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.jlsjyb.cn/gtwhzekqtn.html

[Q18] 模糊匹配
来源：http://hz.hnqzz.top/gtvabrochh.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.jinqigufen.top/gtcucitela.html

[Q19] 范围查询
来源：http://hz.zhaomingkeji.xyz/gtoymhloiq.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.316326.xyz/gtqovpbdjn.html

[Q20] IN 列表
来源：http://hz.quarkkingdee.top/gtbdhgjfzh.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.xingfuxueyuan.xyz/gttqnrftnu.html

[Q21] 空值判断
来源：http://hz.yongpay.top/gtsffrrols.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.52xcode.cn/gtzsvjsjpm.html

[Q22] 排序
来源：http://hz.xuetiantiany.cn/gtduyiqzzn.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.meibo888.top/gtlvzqttla.html

[Q23] 分页
来源：http://hz.chenzaomai.com/gtlrqqfagd.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.guowangkeji.top/gtdqvhrjeg.html

[Q24] 去重
来源：http://hz.hywenlv.cn/gtepuonqlf.html

SELECT DISTINCT city FROM users;
来源：http://hz.hfpthk.cn/gtnegiesaz.html

[Q25] 只取前 N 条
来源：http://hz.svipenyu.cn/gtlyezepyw.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.meibo888.top/gtvblcgvuf.html

[Q26] 计数
来源：http://hz.tanke756.top/gteztkjdfm.html

SELECT COUNT(*) FROM users;
来源：http://hz.yonumen.top/gtvavhyhmc.html

[Q27] 条件计数
来源：http://hz.52xcode.cn/gtanhoyafb.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.zhaomingkeji.xyz/gtarapuwvj.html

[Q28] 求和与平均
来源：http://hz.daria6918.cn/gtjrgisgtw.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.sweek.top/gtokhwklde.html

[Q29] 最大最小值
来源：http://hz.havefunace.top/gtkdkphuvi.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.tanke756.top/gtswgagnnr.html

[Q30] 分组统计
来源：http://hz.birdmap.top/gtqpzfrzrd.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.zhiwuduotai.top/gtqcypdzyz.html

[Q31] 分组后过滤
来源：http://hz.shangyingyoupin.top/gtfgvnjiwb.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.guowangkeji.top/gtnqnpocqt.html

[Q32] 分组拼接字符串
来源：http://hz.zhiwuduotai.top/gtkzyuwfvm.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.jlsjyb.cn/gtmmxkaajp.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.jianghu66.top/gtcjqcoztj.html

[Q33] 多列分组
来源：http://hz.jinghuilouyu.cn/gtdyuldnmc.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.pengpengdd.cyou/gtvtlmtsma.html

[Q34] 每组取第一条
来源：http://hz.bjfxy.top/gtvjwtcktx.html

SELECT * FROM (
来源：http://hz.hammf.cn/gtludwfpxj.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.kuanghao11.cn/gtbpsixggo.html

) t WHERE rn = 1;
来源：http://hz.havefunace.top/gtphxkddtk.html

[Q35] 内连接
来源：http://hz.yuanzhike.top/gtocnmwqpo.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.iojbl.cn/gtluwbbkpb.html

[Q36] 左连接
来源：http://hz.iojbl.cn/gtlrmlvxbv.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.xuetiantiany.cn/gtzhorwsai.html

[Q37] 右连接
来源：http://hz.svipenyu.cn/gtbhprmrjp.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.yuanzhike.top/gtpomkieai.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.yj20258888.top/gtanetazke.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.jianghu66.top/gteyvvfkgo.html

[Q39] 自连接（查上下级）
来源：http://hz.birdmap.top/gtyfnkacry.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.iojbl.cn/gtdxdrgfpk.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.meibo888.top/gtuanfwbow.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.birdmap.top/gturvoeoam.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.zhiwuduotai.top/gtfsrlirbb.html

[Q41] 多表连接
来源：http://hz.shuidangran.top/gtczksljhl.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.hnqzz.top/gtgyykxdcs.html

JOIN users u ON u.id = o.user_id
来源：http://hz.zhijiandao.cn/gtinghebyt.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.redwolf501.top/gtpogopmvu.html

[Q42] 连接条件附加过滤
来源：http://hz.vqdsnc.cn/gtqcurxqdz.html


<!-- 参考信息 -->