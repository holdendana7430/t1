代发 wailian999

Ruby: s == s.reverse
来源：http://hz.ehwqpu.com/gtfdjhatnh.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.wangdashe.top/gtcvnlelma.html

[N07] 两数之和（返回下标）
来源：http://hz.iojbl.cn/gtfqnzwkvj.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.sufxvd.cn/gtxwdexblr.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.jiagoushi.top/gttbyzuuhi.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.jinghuilouyu.cn/gtgipjfbzd.html

TS:   // 手写 Map<string, number>
来源：http://hz.chenzaomai.com/gtllduolzs.html

Java: // 手写 HashMap
来源：http://hz.xingfuxueyuan.xyz/gtcjarhtlp.html

Go:   // 手写 map[int]int
来源：http://hz.pycfn.com/gtgplrzrew.html

Ruby: // 手写 Hash
来源：http://hz.zdqjudy.top/gtaadirarc.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.yvedp.cn/gtdimhuret.html

[N08] 生成全排列
来源：http://hz.yonumen.top/gtpdhwovmv.html

Py:   itertools.permutations(arr)
来源：http://hz.yongpay.top/gtfmsernfb.html

PHP:  // 手写递归交换
来源：http://hz.wangdashe.top/gtfnybchwa.html

JS:   // 手写回溯递归
来源：http://hz.zhiwuduotai.top/gtbrsptkvs.html

TS:   // 手写回溯递归
来源：http://hz.ywan-chungtsiang.top/gtvhenqyhh.html

Java: // 手写回溯递归
来源：http://hz.chenlongwang.top/gtdhrdjxzv.html

Go:   // 手写回溯递归
来源：http://hz.ivvv.top/gttuwzrjzp.html

Ruby: arr.permutation.to_a
来源：http://hz.xingfuxueyuan.xyz/gterftdtbl.html

C#:   // 手写回溯递归
来源：http://hz.zhengqikj.top/gtwhebiivp.html

[N09] 栈与队列
来源：http://hz.shanyushiyangkeji.top/gtmwxejaor.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.shangyingyoupin.top/gtugchrsah.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.hammf.cn/gtgqucvaed.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.tianlin.xyz/gtqtfvqfoq.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.jiagoushi.top/gthhndbvgh.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.316326.xyz/gtjisdnytk.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.iojbl.cn/gtyckressh.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.cucudq.cn/gthcopxkij.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.sxryk.cn/gtxsqzlafk.html

[N10] 链表节点定义
来源：http://hz.gaohongyu789.top/gtrukmosfr.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.hysaishi.cn/gtashvedry.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.hysaishi.cn/gtrssnmlbs.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.9152youxi.cn/gtwrrkmplw.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.cashguo.top/gttfxgbqnk.html

Java: class Node { int v; Node next; }
来源：http://hz.iojbl.cn/gtlukrzevw.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.redwolf501.top/gttcnlnfls.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.aibaodan.cn/gtjoafdxxx.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.gotoacloud.top/gtnofpakty.html

[N11] 二叉树中序遍历
来源：http://hz.haohaochexian.top/gtlcsttrzi.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.nanxinkj.top/gtrkdiedgx.html

PHP:  // 手写递归函数
来源：http://hz.zhixingplan.top/gtrckxulia.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.xuetiantiany.cn/gteubtjhqn.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.feifeiyinyue.top/gtdqcjukfl.html

Java: // 手写递归
来源：http://hz.cqqwz.cn/gtehmvftvz.html

Go:   // 手写递归
来源：http://hz.andypj.xyz/gttqblycpw.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.shuidangran.top/gtijdrwztx.html

C#:   // 手写递归
来源：http://hz.wangdashe.top/gtgaxtyfiw.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.jinqigfzy.top/gtlugusdbc.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.yonumen.top/gtdyjxznsy.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.aibaodan.cn/gtrwnybepb.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.aibaodan.cn/gtjsmuohtw.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.cheryme.top/gtkftpvqwk.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.dianchejie.cn/gtjvjevacv.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.cashguo.top/gttfzdgnem.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.daxiang520.top/gtjvwtnmge.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.jyoumei.cn/gtxxdcexdt.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtzyrxctso.html

O. 并发与异步
来源：http://hz.kuanghao11.cn/gtpoftejay.html

================================================================================
来源：http://hz.gaohongyu789.top/gtrpammyal.html

[O01] 启动一个线程
来源：http://hz.svipenyu.cn/gtushrptxb.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.snrcjt.cn/gtpwrwowrq.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.zhoulong.xyz/gthnxezxln.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.jianghu66.top/gtrjolhmkv.html

TS:   // 同 JS
来源：http://hz.zhiwuduotai.top/gtyyunrjam.html

Java: new Thread(() -> f()).start()
来源：http://hz.zhiwuduotai.top/gtvmcslkxh.html

Go:   go f()
来源：http://hz.zycfv.cn/gtmwugjzse.html

Ruby: Thread.new { f }
来源：http://hz.chenjidiqi.icu/gtlnndqicb.html

C#:   Task.Run(() => F());
来源：http://hz.yuanzhike.top/gtkzzlfbrt.html

[O02] 使用线程池
来源：http://hz.yj202588.top/gtuecbphlw.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.tian-w.cn/gthiwkzdyu.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.zhaomingkeji.xyz/gtvejwlwmr.html

JS:   // worker_threads 线程池
来源：http://hz.yongpay.top/gteuwhrdff.html

TS:   // worker_threads 线程池
来源：http://hz.yonumen.top/gtcumrdwqb.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.ydzc1.top/gtvpqpsfgn.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.hongshengwenyu.top/gttoieltbf.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.bjfxy.top/gtpkpqqujv.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.jinyuanbaomall.cn/gtffhlhgkd.html

[O03] 加锁保护共享数据
来源：http://hz.haohaochexian.top/gtmbrbhytv.html

Py:   with lock: shared += 1
来源：http://hz.jinqigfzy.top/gttsnunxpj.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.yuanzhike.top/gtgjopuidn.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.hysaishi.cn/gtwtkqqcvi.html

TS:   // 同 JS
来源：http://hz.zhixingplan.top/gtxettdqya.html

Java: synchronized (this) { shared++; }
来源：http://hz.gaohongyu789.top/gtaysgjkfu.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.316326.xyz/gtxrlejufr.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.snrcjt.cn/gtftplknjz.html

C#:   lock (gate) { shared++; }
来源：http://hz.shanyushiyangtech.top/gtowpjyxgu.html

[O04] 定义异步函数并等待
来源：http://hz.nanxuanxn.top/gteeurofum.html

Py:   async def f():⏎    await g()
来源：http://hz.yuanzhike.top/gtlhglkltw.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.feifeiyinyue.top/gtijlywxao.html

JS:   async function f() { await g(); }
来源：http://hz.guowangkeji.top/gtxwyspxvo.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.316326.xyz/gtvzitbfis.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.zycfv.cn/gtykcgtcgc.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.yangfankeji.com/gtnavijvfz.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.gotoacloud.top/gtdhsvrwkp.html

C#:   async Task F() { await G(); }
来源：http://hz.zdqjudy.top/gttycsaoio.html

[O05] 并发执行并等待全部完成
来源：http://hz.zycfv.cn/gttckyqamp.html

Py:   asyncio.gather(*tasks)
来源：http://hz.sxryk.cn/gtgzcmkngd.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.xinyue.icu/gtwtamoect.html

JS:   await Promise.all(tasks)
来源：http://hz.sxryk.cn/gtvidoojot.html

TS:   await Promise.all(tasks)
来源：http://hz.zhaomingkeji.xyz/gtgefqerwb.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.daria6918.cn/gtnorzrjfp.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.aizwys.cn/gtnoavrjdf.html

Ruby: threads.map(&:join)
来源：http://hz.aibaodan.cn/gtwntnkqmv.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.hysaishi.cn/gtlzhnwxfc.html

[O06] 使用进程池
来源：http://hz.feifeiyinyue.top/gtzlplrjsn.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.smart0.xyz/gthjowvsct.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.zhongyouzk.top/gtfybhcpjw.html

JS:   // child_process / cluster 模块
来源：http://hz.xylfe.cn/gtrkkygnbc.html

TS:   // child_process / cluster 模块
来源：http://hz.hywenlv.cn/gtbngzxttu.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.0kj1m.cn/gtpqorzdlu.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.sxryk.cn/gtuzolzbws.html

Ruby: // fork 块
来源：http://hz.jianghu66.top/gtbbhocsnw.html

C#:   Parallel.For
来源：http://hz.zhiwuduotai.top/gtwogmjjbj.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtdglfgqaw.html

P. 常用工具函数
来源：http://hz.daria6918.cn/gtxywwtwcm.html

================================================================================
来源：http://hz.hammf.cn/gtvvjzysir.html

[P01] 生成 UUID
来源：http://hz.sysykeji.top/gtnimzsmaa.html

Py:   str(uuid.uuid4())
来源：http://hz.nanxuanxn.top/gtbiurntmr.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.xylfe.cn/gtpgfbilbn.html

JS:   crypto.randomUUID()
来源：http://hz.wangdashe.top/gtooiakgmh.html

TS:   crypto.randomUUID()
来源：http://hz.yanxiufei.cn/gtbkbimsmq.html

Java: UUID.randomUUID().toString()
来源：http://hz.yonumen.top/gtibfkuslj.html

Go:   // 用 github.com/google/uuid
来源：http://hz.zycfv.cn/gtcrvyutmv.html

Ruby: SecureRandom.uuid
来源：http://hz.zhiwuduotai.top/gtmitehpcx.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.dianchejie.cn/gtbncamock.html

[P02] MD5 / SHA256 摘要
来源：http://hz.ywan-chungtsiang.top/gtnqsnpkab.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.sweek.top/gtjiqbxpik.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.yj202588.top/gtsmhgvgjp.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.birdmap.top/gtiwdfxepw.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.jqgufenzy.top/gtwdblfalc.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.zhijiandao.cn/gtafohmmrz.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.sxryk.cn/gtqlpffhcn.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.hongshengwenyu.top/gtlkpfwmbz.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.jqgfzy.top/gtkagwfmux.html

[P03] 生成短随机字符串
来源：http://hz.svipenyu.cn/gtgwwhsttz.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.shuidangran.top/gtqqfptmyw.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.jlsjyb.cn/gtjftrufwz.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.feifeiyinyue.top/gtwcbiglqa.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.hfpthk.cn/gtlsuadpsi.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.andypj.xyz/gteczneutg.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.zhixingplan.top/gtwyifrica.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.gogol.net.cn/gtlyhuupzu.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.guannengcc.top/gtbrvwdbxq.html

[P04] 求长度
来源：http://hz.zhijiandao.cn/gtwcilklto.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.hongshengwenyu.top/gtqtrjelig.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.tanke756.top/gtxuyxpmkx.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.svipenyu.cn/gtzknbigcw.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.xylfe.cn/gtzfayyuuc.html

Java: list.size();  map.size();  s.length()
来源：http://hz.hywenlv.cn/gtjldpctky.html

Go:   len(arr);  len(m)
来源：http://hz.316326.xyz/gtcimrcece.html

Ruby: x.length;  x.size
来源：http://hz.meibo888.top/gteagxpmew.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.cheryme.top/gtfxhfiynv.html

[P05] 判断两个对象内容是否相等
来源：http://hz.yongpay.top/gtmuzhvgeb.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.hywenlv.cn/gtxzdrdtaz.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.iojbl.cn/gtoyohhzbp.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.guowangkeji.top/gtcauuvxvu.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.shzxlz.cn/gtpcrnzewv.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.sysykeji.top/gtliincgig.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.chenjidiqi.icu/gttxpxdkyg.html

Ruby: a == b
来源：http://hz.yonumen.top/gtvplknnvq.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.9152youxi.cn/gtakuzklqu.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.ywan-chungtsiang.top/gtjzlunhlm.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.zhoulong.xyz/gtgebsajvd.html

PHP:  if (empty($x)) {}
来源：http://hz.fengsongda.top/gtuuocndtn.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.zhijiandao.cn/gttqnhbqex.html

TS:   if (x == null) {}
来源：http://hz.yongpay.top/gtmywmfokv.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.yanxiufei.cn/gtoiigqwyi.html

Go:   if x == nil {}
来源：http://hz.jiagoushi.top/gtdoymmgyv.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.pengpengdd.cyou/gtnojaqlnd.html

C#:   if (x is null) {}
来源：http://hz.daxiang520.top/gtrbrsppvz.html

[P07] 防抖与节流
来源：http://hz.xuetiantiany.cn/gtxucaywbd.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.iojbl.cn/gttgyxvueo.html

PHP:  // 手写时间戳比较
来源：http://hz.0kj1m.cn/gttqyrtmhy.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.yonumen.top/gtegzsspyw.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.yuanzhike.top/gthfueykuw.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.fengsongda.top/gtnxweycyl.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.meibo888.top/gtyffnagzk.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.zhijiandao.cn/gtcljssyab.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.snrcjt.cn/gtepxfbiff.html

[P08] 处理浮点精度问题
来源：http://hz.nwbrower.top/gtqmcaokrl.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.sxryk.cn/gteqsyjdkd.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.mhx1999.top/gtbijiiuzm.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.pycfn.com/gtrdsccoud.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.zycfv.cn/gtrygosxiy.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.yongpay.top/gtjiqapdep.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.ydzc1.top/gtjkwaylzh.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.jinqigufen.top/gtitoecovx.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.sysykeji.top/gtodjofhjs.html

================================================================================
来源：http://hz.fengsongda.top/gturgcusnc.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.c1oappe.top/gtfdfwmfgi.html

================================================================================
来源：http://hz.xziqi.cn/gtwhtukvct.html

[Q01] 创建表
来源：http://hz.tianlin.xyz/gtwxasaglt.html

CREATE TABLE users (
来源：http://hz.jlsjyb.cn/gtwytalsxw.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.zhijiandao.cn/gtbvydsckp.html

name VARCHAR(50) NOT NULL,
来源：http://hz.jyoumei.cn/gtvumiakle.html

email VARCHAR(100) UNIQUE,
来源：http://hz.fengsongda.top/gtusrpidur.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.shangyingyoupin.top/gtsazmoaxy.html

);
来源：http://hz.yonumen.top/gtrkuopdpw.html

[Q02] 创建带外键的表
来源：http://hz.feifeiyinyue.top/gtmskkqppz.html

CREATE TABLE orders (
来源：http://hz.nanxuanxn.top/gtxtqkodlr.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.pengpengdd.cyou/gtlowxlsbe.html

user_id INT NOT NULL,
来源：http://hz.xylfe.cn/gtsrmpdtxh.html

amount DECIMAL(10, 2),
来源：http://hz.chenjidiqi.icu/gtzmdmiagd.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.wangdashe.top/gtcjbxxduu.html

);
来源：http://hz.jinqigufen.top/gtspehbsub.html

[Q03] 增加列
来源：http://hz.9152youxi.cn/gtiifztywq.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.haohaochexian.top/gtgynrvjhs.html

[Q04] 修改列类型
来源：http://hz.xuetiantiany.cn/gtzwnrjeij.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.fengsongda.top/gtpgqtueuw.html

[Q05] 重命名列
来源：http://hz.ehwqpu.com/gtnhantrjz.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.haohaochexian.top/gtjrthcttg.html

[Q06] 删除列
来源：http://hz.ppjwa.cn/gtdqbcreqn.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.xylfe.cn/gtqhezhevz.html

[Q07] 删除表
来源：http://hz.ydjk.org.cn/gtldkcvpzn.html

DROP TABLE IF EXISTS orders;
来源：http://hz.yueranfly.top/gtxeeoinqm.html

[Q08] 创建普通索引
来源：http://hz.xingfuxueyuan.xyz/gtwqqzlnuo.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.redwolf501.top/gtjqgidihs.html

[Q09] 创建唯一索引
来源：http://hz.jinqigfzy.top/gtgiuceauq.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.hysaishi.cn/gtnpjdjhit.html

[Q10] 插入单行
来源：http://hz.nanxuanxn.top/gttulfoyyc.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.feifeiyinyue.top/gtvghrlntm.html

[Q11] 一次插入多行
来源：http://hz.zhoulong.xyz/gtcojpfifj.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.jinqigfzy.top/gtqnasvpnk.html

[Q12] 插入后取自增 ID
来源：http://hz.yvedp.cn/gtwtuzqdeh.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.shanyushiyangtech.top/gtbewtkmcs.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.haohaochexian.top/gtaifughil.html

[Q13] 忽略重复插入
来源：http://hz.hysaishi.cn/gtyuvchykw.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.hfpthk.cn/gttomteagi.html

[Q14] 存在则更新（upsert）
来源：http://hz.wangdashe.top/gtyctabgwe.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.vqdsnc.cn/gtosrsmwoz.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.c1oappe.top/gtpfhcclab.html

[Q15] 查询全部
来源：http://hz.yvedp.cn/gtuqphjewf.html

SELECT * FROM users;
来源：http://hz.fengsongda.top/gtqqwrawtp.html

[Q16] 查询指定列
来源：http://hz.yuxming.cn/gthmzbsusi.html

SELECT id, name FROM users;
来源：http://hz.hammf.cn/gtoifkhkoq.html

[Q17] 条件查询
来源：http://hz.yj20258.top/gtiaovgdtc.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.chenjidiqi.icu/gtiievqbxf.html

[Q18] 模糊匹配
来源：http://hz.jiagoushi.top/gtifrkzbws.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.iojbl.cn/gtbnzywwtk.html

[Q19] 范围查询
来源：http://hz.dianchejie.cn/gttcqqhbba.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.zhengqikj.top/gtpwuflozf.html

[Q20] IN 列表
来源：http://hz.xingfuxueyuan.xyz/gtakmqaipk.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.jianghu66.top/gtlivjvpjz.html

[Q21] 空值判断
来源：http://hz.daxiang520.top/gtvwedyigz.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.xinyue.icu/gtpzvucdwy.html

[Q22] 排序
来源：http://hz.bjfxy.top/gtchhlinrr.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.redwolf501.top/gtjcrirhah.html

[Q23] 分页
来源：http://hz.smart0.xyz/gtozuirqac.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.cqqwz.cn/gtmfeinmdf.html

[Q24] 去重
来源：http://hz.jinghuilouyu.cn/gtooqdprny.html

SELECT DISTINCT city FROM users;
来源：http://hz.nanxinkj.top/gtirkpovpz.html

[Q25] 只取前 N 条
来源：http://hz.zhijiandao.cn/gtxlcowxry.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.chenzaomai.com/gtnnuennvt.html

[Q26] 计数
来源：http://hz.dianchejie.cn/gtmagzyrlc.html

SELECT COUNT(*) FROM users;
来源：http://hz.cqqwz.cn/gthjcxlcju.html

[Q27] 条件计数
来源：http://hz.zhixingplan.top/gtojvlzrsx.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.andypj.xyz/gtaehqfzyy.html

[Q28] 求和与平均
来源：http://hz.meibo888.top/gtkpbavbof.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.redwolf501.top/gtrnsltzkf.html

[Q29] 最大最小值
来源：http://hz.jinqigufen.top/gtgzcwigdx.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.nanxinkj.top/gtkeezywuj.html

[Q30] 分组统计
来源：http://hz.yonumen.top/gtqciuumyy.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.gotoacloud.top/gtubyvmkwy.html

[Q31] 分组后过滤
来源：http://hz.gogol.net.cn/gtvgacrgce.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.chenzaomai.com/gtqoodwmap.html

[Q32] 分组拼接字符串
来源：http://hz.hammf.cn/gtkyrpjies.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.andypj.xyz/gtmhicfoca.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.52xcode.cn/gtkyxjlmhy.html

[Q33] 多列分组
来源：http://hz.jinyuanbaomall.cn/gtpmuugxdx.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.cheryme.top/gtrzkhzdhz.html

[Q34] 每组取第一条
来源：http://hz.chenjidiqi.icu/gtikcxoswh.html

SELECT * FROM (
来源：http://hz.svipenyu.cn/gtfhdqxwzz.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.jyoumei.cn/gtqkidgyhn.html

) t WHERE rn = 1;
来源：http://hz.fzhhl.top/gtkevpgxkh.html

[Q35] 内连接
来源：http://hz.xziqi.cn/gtermaxqlc.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.0kj1m.cn/gttrfiyqjg.html

[Q36] 左连接
来源：http://hz.zhaomingkeji.xyz/gtwjtnnsos.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.tian-w.cn/gtpjboegro.html

[Q37] 右连接
来源：http://hz.zycfv.cn/gtpsdsbjsj.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.ydzc1.top/gtzzhweysd.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.zhixingplan.top/gtmhtyujgo.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.zycfv.cn/gtjvqdlflt.html

[Q39] 自连接（查上下级）
来源：http://hz.aibaodan.cn/gtuhrubzrp.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.dashuyun.cn/gtdhthtrko.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.yvedp.cn/gtrvciajmx.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.nanxinkj.top/gtqotevsai.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.hywenlv.cn/gtdsdkgucx.html

[Q41] 多表连接
来源：http://hz.guannengcc.top/gttprtwmfv.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.bjfxy.top/gtrymhsbff.html

JOIN users u ON u.id = o.user_id
来源：http://hz.hfpthk.cn/gtepygilyw.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.ywan-chungtsiang.top/gtkmswnpvx.html

[Q42] 连接条件附加过滤
来源：http://hz.mhx1999.top/gtujcubqur.html

SELECT u.name, o.amount FROM users u
来源：http://hz.ydjk.org.cn/gtkvxzonma.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.cqqwz.cn/gtwrrjwtdo.html

[Q43] 标量子查询
来源：http://hz.ppjwa.cn/gtqdzhcawy.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.aibaodan.cn/gtmavltfes.html

[Q44] IN 子查询
来源：http://hz.dianchejie.cn/gtvvlfdroo.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.yj20258.top/gtfnezonyq.html

[Q45] EXISTS 判断存在
来源：http://hz.pengpengdd.cyou/gtjipkbngi.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.chenlongwang.top/gtjzuorkxm.html


<!-- 参考信息 -->