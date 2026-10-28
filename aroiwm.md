代发 wailian999

JS:   s === [...s].reverse().join("")
来源：http://hz.yj20258.top/gtftekvkdj.html

TS:   s === [...s].reverse().join("")
来源：http://hz.hysaishi.cn/gtgsyzqiyy.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.yangfankeji.com/gtpysdgdjr.html

Go:   // 双指针从两端比较
来源：http://hz.sysykeji.top/gtvktqvffw.html

Ruby: s == s.reverse
来源：http://hz.jinqigufen.top/gtesgbqpeb.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.wangshuangyany.cn/gthcizpjne.html

[N07] 两数之和（返回下标）
来源：http://hz.xylfe.cn/gtuemdeylv.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.hnxiangtu.top/gtgykujwuj.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.yangfankeji.com/gtfgmrntij.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.yueranfly.top/gtjzlouyfj.html

TS:   // 手写 Map<string, number>
来源：http://hz.zhaomingkeji.xyz/gthjzydyaa.html

Java: // 手写 HashMap
来源：http://hz.ywan-chungtsiang.top/gtfconhlql.html

Go:   // 手写 map[int]int
来源：http://hz.hfpthk.cn/gtojznceam.html

Ruby: // 手写 Hash
来源：http://hz.gogol.net.cn/gtlhxqceyv.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.shanyushiyangtech.top/gttxubmslu.html

[N08] 生成全排列
来源：http://hz.xinyue.icu/gtuqnepgln.html

Py:   itertools.permutations(arr)
来源：http://hz.yongpay.top/gtpemmvotn.html

PHP:  // 手写递归交换
来源：http://hz.jinqigfzy.top/gtgopkkual.html

JS:   // 手写回溯递归
来源：http://hz.hnqzz.top/gtkszicjxe.html

TS:   // 手写回溯递归
来源：http://hz.zhiwuduotai.top/gtomaesgaw.html

Java: // 手写回溯递归
来源：http://hz.sxryk.cn/gtwpwgbvyc.html

Go:   // 手写回溯递归
来源：http://hz.zhiwuduotai.top/gtyfdabzjv.html

Ruby: arr.permutation.to_a
来源：http://hz.gogol.net.cn/gtnokkupie.html

C#:   // 手写回溯递归
来源：http://hz.zhixingplan.top/gtmdcghnyd.html

[N09] 栈与队列
来源：http://hz.gotoacloud.top/gttqzlyken.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.zhongyouzk.top/gtsyhlwgoz.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.haohaochexian.top/gtdluppjtb.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.birdmap.top/gtikgfzwfs.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.shangyingyoupin.top/gtejnutqbb.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.yuxming.cn/gtmgfhembz.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.aizwys.cn/gthhykmtet.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.yongpay.top/gteqprcxwv.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.yvedp.cn/gtlyhshozo.html

[N10] 链表节点定义
来源：http://hz.yanxiufei.cn/gtmpzzprtk.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.xingfuxueyuan.xyz/gtgcomtmqc.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.jqgfzy.top/gtpabluhly.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.zhixingplan.top/gteczmzzdn.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.zhiwuduotai.top/gtctdeqisw.html

Java: class Node { int v; Node next; }
来源：http://hz.yangfankeji.com/gtzfosiicr.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.cucudq.cn/gtkprjsjlf.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.0kj1m.cn/gttfgglvya.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.jlsjyb.cn/gtbscbsgjs.html

[N11] 二叉树中序遍历
来源：http://hz.cqqwz.cn/gtmmdoalet.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.svipenyu.cn/gtaefofesf.html

PHP:  // 手写递归函数
来源：http://hz.haohaochexian.top/gtepkbbzug.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.tian-w.cn/gtptulmlyc.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.ivvv.top/gtiscjoxpb.html

Java: // 手写递归
来源：http://hz.9152youxi.cn/gtohhpccoo.html

Go:   // 手写递归
来源：http://hz.aizwys.cn/gthbviwqpr.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.hongshengwenyu.top/gtxyfruhcm.html

C#:   // 手写递归
来源：http://hz.cucudq.cn/gtixifuwkt.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.zycfv.cn/gttaydafjd.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.ivvv.top/gtljqkbzeb.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.vqdsnc.cn/gtkseelvnr.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.yonumen.top/gtvigsseqj.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.jinqigufen.top/gtebddfbxp.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.yj20258888.top/gtnfcvepqb.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.zhixingplan.top/gtzseezlgz.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.pengpengdd.cyou/gttsfqjzsj.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.jqgfzy.top/gtdrbhdvun.html

================================================================================
来源：http://hz.0kj1m.cn/gtbhhkgnfz.html

O. 并发与异步
来源：http://hz.pengpengdd.cyou/gtachdgypj.html

================================================================================
来源：http://hz.wangdashe.top/gtiihcbxph.html

[O01] 启动一个线程
来源：http://hz.jyoumei.cn/gtxmvehvmu.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.pengpengdd.cyou/gttfgynnbr.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.birdmap.top/gtctdivkfo.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.hnxiangtu.top/gtbrumqgtf.html

TS:   // 同 JS
来源：http://hz.jinyuanbaomall.cn/gteiilbwli.html

Java: new Thread(() -> f()).start()
来源：http://hz.snrcjt.cn/gtsbglayjm.html

Go:   go f()
来源：http://hz.quarkkingdee.top/gtgwmqdrzw.html

Ruby: Thread.new { f }
来源：http://hz.shanyushiyangkeji.top/gtgiezunec.html

C#:   Task.Run(() => F());
来源：http://hz.ydzc1.top/gtjiyjioae.html

[O02] 使用线程池
来源：http://hz.zhengqikj.top/gtgpijhutj.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.hnxiangtu.top/gtcpgrhmix.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.ydjk.org.cn/gtxdhnlktr.html

JS:   // worker_threads 线程池
来源：http://hz.meibo888.top/gtolgaoydg.html

TS:   // worker_threads 线程池
来源：http://hz.smart0.xyz/gtgrwodadb.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.jinqigufen.top/gtjnpryxix.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.jinghuilouyu.cn/gtvqvoiadv.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.yuxming.cn/gtevcckpvm.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.tian-w.cn/gtgvkmwofk.html

[O03] 加锁保护共享数据
来源：http://hz.daxiang520.top/gtltidjjbq.html

Py:   with lock: shared += 1
来源：http://hz.hysaishi.cn/gtudukyxza.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.zhaomingkeji.xyz/gttsqelipg.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.jqgfzy.top/gtcroktish.html

TS:   // 同 JS
来源：http://hz.hammf.cn/gterlnkhwx.html

Java: synchronized (this) { shared++; }
来源：http://hz.fengsongda.top/gtedkvycng.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.guowangkeji.top/gtspwrhjal.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.nanxinkj.top/gtklvxmhsy.html

C#:   lock (gate) { shared++; }
来源：http://hz.zhijiandao.cn/gtjpxxcqjd.html

[O04] 定义异步函数并等待
来源：http://hz.daxiang520.top/gtaibrwsje.html

Py:   async def f():⏎    await g()
来源：http://hz.nanxinkj.top/gtlgyntihu.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.shzxlz.cn/gtbuyqdiua.html

JS:   async function f() { await g(); }
来源：http://hz.sweek.top/gtmphfjxut.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.chenjidiqi.icu/gtehzbzbyc.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.ppjwa.cn/gtjtlonivl.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.ywan-chungtsiang.top/gtcqesttqz.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.shzxlz.cn/gtcbppgbhb.html

C#:   async Task F() { await G(); }
来源：http://hz.wangdashe.top/gtpuhmrmpg.html

[O05] 并发执行并等待全部完成
来源：http://hz.pycfn.com/gtnsymkyzo.html

Py:   asyncio.gather(*tasks)
来源：http://hz.yongpay.top/gtrcszkimg.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.chenlongwang.top/gtpcxpbgdv.html

JS:   await Promise.all(tasks)
来源：http://hz.52xcode.cn/gttxlxfdyc.html

TS:   await Promise.all(tasks)
来源：http://hz.mhx1999.top/gtbxoimabp.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.shangyingyoupin.top/gtpnaiepxn.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.c1oappe.top/gtndmslkyr.html

Ruby: threads.map(&:join)
来源：http://hz.gzhubu.top/gtjehdmknu.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.quarkkingdee.top/gthosummym.html

[O06] 使用进程池
来源：http://hz.nanxuanxn.top/gtykmuqocr.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.c1oappe.top/gtrwikjbst.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.hfpthk.cn/gtxvtnupdo.html

JS:   // child_process / cluster 模块
来源：http://hz.cqqwz.cn/gtncwrgvvy.html

TS:   // child_process / cluster 模块
来源：http://hz.birdmap.top/gthzejmfyd.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.zhongyouzk.top/gtnxetynpc.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.sufxvd.cn/gtxdpuharz.html

Ruby: // fork 块
来源：http://hz.havefunace.top/gtrxqlkptb.html

C#:   Parallel.For
来源：http://hz.yonumen.top/gtdiiswxvg.html

================================================================================
来源：http://hz.yj20258888.top/gtnjeppkij.html

P. 常用工具函数
来源：http://hz.sweek.top/gtfsbkzbqr.html

================================================================================
来源：http://hz.c1oappe.top/gtoryiwuqe.html

[P01] 生成 UUID
来源：http://hz.c1oappe.top/gtilzpcoyl.html

Py:   str(uuid.uuid4())
来源：http://hz.zhixingplan.top/gtkdfrfqha.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.andypj.xyz/gtxatbwxub.html

JS:   crypto.randomUUID()
来源：http://hz.chenjidiqi.icu/gtsfmtrpfg.html

TS:   crypto.randomUUID()
来源：http://hz.zdqjudy.top/gtggjjhjfj.html

Java: UUID.randomUUID().toString()
来源：http://hz.sufxvd.cn/gtwyushmxk.html

Go:   // 用 github.com/google/uuid
来源：http://hz.mhx1999.top/gtjuogflun.html

Ruby: SecureRandom.uuid
来源：http://hz.sufxvd.cn/gtmawwzhhh.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.hysaishi.cn/gtrwtgbpjd.html

[P02] MD5 / SHA256 摘要
来源：http://hz.hywenlv.cn/gtgqwqsxcr.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.yongpay.top/gtgquhsqfc.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.ivvv.top/gtoecubwji.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.sysykeji.top/gtdbrygles.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.yj20258.top/gtwzcdzxxe.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.iojbl.cn/gtxvhlukag.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.yanxiufei.cn/gtbimldjhz.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.zhongyouzk.top/gtrdaqizrx.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.jiagoushi.top/gtlmdbgnpc.html

[P03] 生成短随机字符串
来源：http://hz.cheryme.top/gtswcancvm.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.gzhubu.top/gtavywrmqn.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.guannengcc.top/gtgqaylnlp.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.iojbl.cn/gtnluorjuu.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.cheryme.top/gtmfnxsfde.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.xuetiantiany.cn/gtrdhvsont.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.sysykeji.top/gtpbncpyhe.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.wangshuangyany.cn/gtsvpkorqg.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.316326.xyz/gtwokwjzge.html

[P04] 求长度
来源：http://hz.ydjk.org.cn/gtoqyssucz.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.guowangkeji.top/gtndcwjpze.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.jinyuanbaomall.cn/gtuvlbnklo.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.zhijiandao.cn/gtvlpdqedr.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.52xcode.cn/gtrppuzhjy.html

Java: list.size();  map.size();  s.length()
来源：http://hz.chenlongwang.top/gtevtgczpe.html

Go:   len(arr);  len(m)
来源：http://hz.yueranfly.top/gtivjigemj.html

Ruby: x.length;  x.size
来源：http://hz.cqqwz.cn/gtjrwkzwuu.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.nanxuanxn.top/gtjvexerfp.html

[P05] 判断两个对象内容是否相等
来源：http://hz.ywan-chungtsiang.top/gtbcoaknim.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.gzhubu.top/gthhvgxkdj.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.redwolf501.top/gtdmtibdcq.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.nanxinkj.top/gtqynnjbnt.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.zhaomingkeji.xyz/gtfuycpxcc.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.zhiwuduotai.top/gtnxfcktrm.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.yuanzhike.top/gtiooyygkh.html

Ruby: a == b
来源：http://hz.redwolf501.top/gtbbhqzpdl.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.guowangkeji.top/gtvpjgjxou.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.haohaochexian.top/gtcurqacmk.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.chenlongwang.top/gtyfqrkxyl.html

PHP:  if (empty($x)) {}
来源：http://hz.jinyuanbaomall.cn/gtvqtunrth.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.bjfxy.top/gtjoaqbwly.html

TS:   if (x == null) {}
来源：http://hz.ydzc1.top/gtkfhdlpbg.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.nanxuanxn.top/gtnbrrzolm.html

Go:   if x == nil {}
来源：http://hz.bjfxy.top/gtrdkfusut.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.cdnleiting.top/gtgsiapnmh.html

C#:   if (x is null) {}
来源：http://hz.jianghu66.top/gtvpewbgoh.html

[P07] 防抖与节流
来源：http://hz.svipenyu.cn/gtxcxladcg.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.jiagoushi.top/gtxupalann.html

PHP:  // 手写时间戳比较
来源：http://hz.ppjwa.cn/gtysqvknxw.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.aizwys.cn/gtrrcupndq.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.zdqjudy.top/gtutdleqez.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.ivvv.top/gtihrfxsce.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.jyoumei.cn/gtvgvnrfes.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.daria6918.cn/gtenpaezzj.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.yj202588.top/gtpsqaoepf.html

[P08] 处理浮点精度问题
来源：http://hz.jqgufenzy.top/gtsujmjlvv.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.jianghu66.top/gtxpwrsjdo.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.guannengcc.top/gtykrywcpr.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.ybcxt.top/gtjjrtgkpn.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.birdmap.top/gtvvmznhub.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.daxiang520.top/gtdvxcjgvv.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.wangdashe.top/gtirqoupac.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.hywenlv.cn/gthyetkevp.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.xuetiantiany.cn/gtuclkdxbq.html

================================================================================
来源：http://hz.yj202588.top/gtpifgxymj.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.xingfuxueyuan.xyz/gtkrgnzdgg.html

================================================================================
来源：http://hz.sysykeji.top/gtjkhuitvg.html

[Q01] 创建表
来源：http://hz.aizwys.cn/gtizcjbfys.html

CREATE TABLE users (
来源：http://hz.dianchejie.cn/gtkewvpuds.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.zhijiandao.cn/gtuqykarht.html

name VARCHAR(50) NOT NULL,
来源：http://hz.meibo888.top/gtwyodinuy.html

email VARCHAR(100) UNIQUE,
来源：http://hz.sxryk.cn/gtbzpmcrnj.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.ydjk.org.cn/gtdfakgwkd.html

);
来源：http://hz.52xcode.cn/gtcqidwnlp.html

[Q02] 创建带外键的表
来源：http://hz.zhiwuduotai.top/gtajvkhgjf.html

CREATE TABLE orders (
来源：http://hz.zdqjudy.top/gtsoyimawa.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.nanxinkj.top/gtubxhfxfn.html

user_id INT NOT NULL,
来源：http://hz.ydzc1.top/gtrzjhqhan.html

amount DECIMAL(10, 2),
来源：http://hz.c1oappe.top/gtuyvhgqjx.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.sxryk.cn/gtuyjfqsxq.html

);
来源：http://hz.jyoumei.cn/gtmaueokxu.html

[Q03] 增加列
来源：http://hz.yuxming.cn/gtinntpgng.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.fengsongda.top/gtcosxyqvv.html

[Q04] 修改列类型
来源：http://hz.xuanzx.com/gtmfdhwref.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.316326.xyz/gtzpaxzbnp.html

[Q05] 重命名列
来源：http://hz.cashguo.top/gtaysitpqh.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.pengpengdd.cyou/gtbrejlmec.html

[Q06] 删除列
来源：http://hz.meibo888.top/gtfitqsxgy.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.chenjidiqi.icu/gthpzxitmf.html

[Q07] 删除表
来源：http://hz.bjfxy.top/gtrlxxhzov.html

DROP TABLE IF EXISTS orders;
来源：http://hz.zhixingplan.top/gtdherqbkf.html

[Q08] 创建普通索引
来源：http://hz.guannengcc.top/gtzoskldoq.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.zhijiandao.cn/gtxjfxtbjf.html

[Q09] 创建唯一索引
来源：http://hz.c1oappe.top/gtlepgvvtd.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.yangfankeji.com/gtztbxhdwy.html

[Q10] 插入单行
来源：http://hz.ivvv.top/gtgyepytzu.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.jlsjyb.cn/gtdsjjdrzk.html

[Q11] 一次插入多行
来源：http://hz.yangfankeji.com/gtpndvgwyt.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.bjfxy.top/gtgtuocrmn.html

[Q12] 插入后取自增 ID
来源：http://hz.smart0.xyz/gtzffhsbkx.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.vqdsnc.cn/gtzwsssjif.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.ydzc1.top/gtpejbsqlv.html

[Q13] 忽略重复插入
来源：http://hz.xinyue.icu/gthrxundoe.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.xuanzx.com/gtvyyusvmy.html

[Q14] 存在则更新（upsert）
来源：http://hz.zhoulong.xyz/gtswazbztn.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.daxiang520.top/gtkbmdmebs.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.svipenyu.cn/gtcaiuscpd.html

[Q15] 查询全部
来源：http://hz.yanxiufei.cn/gtemkbrwsi.html

SELECT * FROM users;
来源：http://hz.sweek.top/gttftrvgqk.html

[Q16] 查询指定列
来源：http://hz.zycfv.cn/gtjcbemvue.html

SELECT id, name FROM users;
来源：http://hz.xziqi.cn/gtqziwkwkl.html

[Q17] 条件查询
来源：http://hz.dashuyun.cn/gthdestjtr.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.nanxuanxn.top/gtwpmapwih.html

[Q18] 模糊匹配
来源：http://hz.mhx1999.top/gtjcjhwpdk.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.daxiang520.top/gtysgwjztu.html

[Q19] 范围查询
来源：http://hz.ybcxt.top/gtnisqgojt.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.wangdashe.top/gtiwoxasno.html

[Q20] IN 列表
来源：http://hz.quarkkingdee.top/gtpotntkdv.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.ehwqpu.com/gtcjqxiskn.html

[Q21] 空值判断
来源：http://hz.fengsongda.top/gtsvdyauxz.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.fzhhl.top/gtxsyqsbpo.html

[Q22] 排序
来源：http://hz.yueranfly.top/gtidxxvfml.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.chenjidiqi.icu/gtrgenrwqc.html

[Q23] 分页
来源：http://hz.zhengqikj.top/gtmpgzlnmm.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.nwbrower.top/gtotvlefvq.html

[Q24] 去重
来源：http://hz.daria6918.cn/gtyzppyqna.html

SELECT DISTINCT city FROM users;
来源：http://hz.xingfuxueyuan.xyz/gtfvrunkge.html

[Q25] 只取前 N 条
来源：http://hz.fengsongda.top/gtwbdlznrc.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.hysaishi.cn/gtiiapbykn.html

[Q26] 计数
来源：http://hz.zdqjudy.top/gtzloxwjjb.html

SELECT COUNT(*) FROM users;
来源：http://hz.316326.xyz/gttyfzwphp.html

[Q27] 条件计数
来源：http://hz.aibaodan.cn/gtbcdtfvny.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.kuanghao11.cn/gtpqhrbvaa.html

[Q28] 求和与平均
来源：http://hz.aibaodan.cn/gtqftmseki.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.ivvv.top/gtntybjrbu.html

[Q29] 最大最小值
来源：http://hz.redwolf501.top/gteihqpgur.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.pengpengdd.cyou/gtquoirdoz.html

[Q30] 分组统计
来源：http://hz.c1oappe.top/gtznvscujm.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.ydjk.org.cn/gtpdgjfheb.html

[Q31] 分组后过滤
来源：http://hz.yj20258888.top/gtkqnhytne.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.sweek.top/gtccoyvgnm.html

[Q32] 分组拼接字符串
来源：http://hz.yj20258.top/gtuxgmeson.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.pengpengdd.cyou/gtvjpphnix.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.nanxuanxn.top/gtbgqknjsp.html

[Q33] 多列分组
来源：http://hz.zhaomingkeji.xyz/gtdrnwodwr.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.ywan-chungtsiang.top/gtecdiibox.html

[Q34] 每组取第一条
来源：http://hz.gogol.net.cn/gthjazbdwu.html

SELECT * FROM (
来源：http://hz.fengsongda.top/gtvvllfodq.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.jiagoushi.top/gtxcyticxq.html

) t WHERE rn = 1;
来源：http://hz.tanke756.top/gtfworopct.html

[Q35] 内连接
来源：http://hz.chenzaomai.com/gtbitauztj.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.jianghu66.top/gtpglnohzr.html

[Q36] 左连接
来源：http://hz.iojbl.cn/gtjhzhhzij.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.aibaodan.cn/gtyfdotuld.html

[Q37] 右连接
来源：http://hz.hongshengwenyu.top/gtqrvfhjnp.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.hnqzz.top/gtadljlkzn.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.ehwqpu.com/gtersftibh.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.jyoumei.cn/gtbdbrmbja.html

[Q39] 自连接（查上下级）
来源：http://hz.gotoacloud.top/gtoufqouyi.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.jyoumei.cn/gtojghwzhy.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.xuanzx.com/gtmliubyrk.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.sweek.top/gtswjjzmax.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.sxryk.cn/gtdglsorhp.html

[Q41] 多表连接
来源：http://hz.wangdashe.top/gtvzsgxhia.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.c1oappe.top/gtlpqiausk.html

JOIN users u ON u.id = o.user_id
来源：http://hz.sxryk.cn/gtbyfzntrr.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.yanxiufei.cn/gtonogqric.html

[Q42] 连接条件附加过滤
来源：http://hz.cdnleiting.top/gtcwvpetng.html

SELECT u.name, o.amount FROM users u
来源：http://hz.52xcode.cn/gtyelyeglf.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.smart0.xyz/gttoxicmjy.html

[Q43] 标量子查询
来源：http://hz.yuanzhike.top/gtqcdeddik.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.wangdashe.top/gtjraculwo.html


<!-- 参考信息 -->