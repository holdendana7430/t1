代发 wailian999

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.gogol.net.cn/gtmudmuunt.html

[N06] 判断回文字符串
来源：http://hz.xinyue.icu/gtbpnwaauv.html

Py:   s == s[::-1]
来源：http://hz.dianchejie.cn/gtnwnjugnb.html

PHP:  $s === strrev($s);
来源：http://hz.daria6918.cn/gtpycrmtbo.html

JS:   s === [...s].reverse().join("")
来源：http://hz.shanyushiyangkeji.top/gtsypsiacd.html

TS:   s === [...s].reverse().join("")
来源：http://hz.yj20258.top/gtsygezlgs.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.jyoumei.cn/gtmnbzdzkv.html

Go:   // 双指针从两端比较
来源：http://hz.yonumen.top/gtgydlzevw.html

Ruby: s == s.reverse
来源：http://hz.quarkkingdee.top/gtjhpklmmi.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.zycfv.cn/gtgbkvdbyu.html

[N07] 两数之和（返回下标）
来源：http://hz.jinyuanbaomall.cn/gtbcjxwcvc.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.kuanghao11.cn/gtkefpnhba.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.gaohongyu789.top/gtbvctfoxe.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.hnqzz.top/gtabfvdjlw.html

TS:   // 手写 Map<string, number>
来源：http://hz.nwbrower.top/gtdnpccgsa.html

Java: // 手写 HashMap
来源：http://hz.zdqjudy.top/gtlqfdmdbs.html

Go:   // 手写 map[int]int
来源：http://hz.ywan-chungtsiang.top/gtscxppruf.html

Ruby: // 手写 Hash
来源：http://hz.c1oappe.top/gtydvydyjw.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.bjfxy.top/gtuizxvocy.html

[N08] 生成全排列
来源：http://hz.0kj1m.cn/gtfgpwbyrb.html

Py:   itertools.permutations(arr)
来源：http://hz.zdqjudy.top/gtqvxklihq.html

PHP:  // 手写递归交换
来源：http://hz.shangyingyoupin.top/gtpivxksub.html

JS:   // 手写回溯递归
来源：http://hz.chenzaomai.com/gtjlavgski.html

TS:   // 手写回溯递归
来源：http://hz.quarkkingdee.top/gtzwuzsuel.html

Java: // 手写回溯递归
来源：http://hz.yj20258.top/gttuhidgqr.html

Go:   // 手写回溯递归
来源：http://hz.smart0.xyz/gtcvmpshza.html

Ruby: arr.permutation.to_a
来源：http://hz.cucudq.cn/gticuqkavi.html

C#:   // 手写回溯递归
来源：http://hz.jinghuilouyu.cn/gtcpitwazs.html

[N09] 栈与队列
来源：http://hz.tianlin.xyz/gtpcqirwrm.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.iojbl.cn/gtsncmmwnf.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.jianghu66.top/gtqoyinels.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.52xcode.cn/gtqeeovfzm.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.yueranfly.top/gtiqaayhnh.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.zhijiandao.cn/gtmaoodrpo.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.sweek.top/gteyluiyqd.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.pycfn.com/gtwheuofyt.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.52xcode.cn/gtuyhaxixb.html

[N10] 链表节点定义
来源：http://hz.yuxming.cn/gtsbnwastq.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.zhaomingkeji.xyz/gtseubuxwj.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.sweek.top/gtjyolxads.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.ybcxt.top/gtqsmsaolq.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.gogol.net.cn/gthgikwmcl.html

Java: class Node { int v; Node next; }
来源：http://hz.xuetiantiany.cn/gthyckqswu.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.gogol.net.cn/gtkabjgycc.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.yuanzhike.top/gtvfchzhdl.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.kuanghao11.cn/gtoihdesdu.html

[N11] 二叉树中序遍历
来源：http://hz.yuanzhike.top/gtvbwtwpqr.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.yuxming.cn/gtvsstirjs.html

PHP:  // 手写递归函数
来源：http://hz.ydjk.org.cn/gtqfbidnyc.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.yangfankeji.com/gtfkhqtajq.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.yongpay.top/gterdujgvz.html

Java: // 手写递归
来源：http://hz.birdmap.top/gtyblrvbqj.html

Go:   // 手写递归
来源：http://hz.wangdashe.top/gtcngdtrvk.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.gaohongyu789.top/gtzdblmyld.html

C#:   // 手写递归
来源：http://hz.guannengcc.top/gtyeqoztgm.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.gogol.net.cn/gtuerlqjbe.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.sysykeji.top/gtnbjucrox.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.jianghu66.top/gtjbougyky.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.sweek.top/gtxhenpddl.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.xziqi.cn/gtahucqzpp.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.tianlin.xyz/gtzjbswuxq.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.ydzc1.top/gtqxqmdkci.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.316326.xyz/gtxmevdztb.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.snrcjt.cn/gtrnahehbw.html

================================================================================
来源：http://hz.gzhubu.top/gtojfnyinp.html

O. 并发与异步
来源：http://hz.jinqigufen.top/gtibogxfrh.html

================================================================================
来源：http://hz.tian-w.cn/gttetndluf.html

[O01] 启动一个线程
来源：http://hz.yueranfly.top/gtckogzvqt.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.sysykeji.top/gtojtcjeqa.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.aizwys.cn/gtlwidkiep.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.vqdsnc.cn/gtlyjmrnfq.html

TS:   // 同 JS
来源：http://hz.cashguo.top/gthzaxgfqj.html

Java: new Thread(() -> f()).start()
来源：http://hz.shanyushiyangkeji.top/gtkiwryaab.html

Go:   go f()
来源：http://hz.xziqi.cn/gteaxyqotl.html

Ruby: Thread.new { f }
来源：http://hz.cucudq.cn/gtlpglsits.html

C#:   Task.Run(() => F());
来源：http://hz.jiagoushi.top/gtymyuokbv.html

[O02] 使用线程池
来源：http://hz.gotoacloud.top/gtibfdeius.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.jqgfzy.top/gtdlqujdkc.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.gogol.net.cn/gtkyavuyuc.html

JS:   // worker_threads 线程池
来源：http://hz.c1oappe.top/gtuwuldqag.html

TS:   // worker_threads 线程池
来源：http://hz.hfpthk.cn/gtpqvhaomf.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.dashuyun.cn/gtsodrppdk.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.9152youxi.cn/gtyjdtytci.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.zhiwuduotai.top/gtfuzdxfob.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.hysaishi.cn/gtlikfnlwf.html

[O03] 加锁保护共享数据
来源：http://hz.shuidangran.top/gtibaxolvt.html

Py:   with lock: shared += 1
来源：http://hz.yongpay.top/gtapaikpcx.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.zhongyouzk.top/gtarexmcsx.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.pycfn.com/gtrdmqbbau.html

TS:   // 同 JS
来源：http://hz.nwbrower.top/gthtvavedx.html

Java: synchronized (this) { shared++; }
来源：http://hz.ydzc1.top/gtgxqahsgu.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.bjfxy.top/gtzxsxgrdx.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.hfpthk.cn/gtpeyoerna.html

C#:   lock (gate) { shared++; }
来源：http://hz.jyoumei.cn/gtlhkumezv.html

[O04] 定义异步函数并等待
来源：http://hz.yj20258.top/gtyeyocbrr.html

Py:   async def f():⏎    await g()
来源：http://hz.jqgufenzy.top/gtvtsgrgsy.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.svipenyu.cn/gtijqoxdsk.html

JS:   async function f() { await g(); }
来源：http://hz.ybcxt.top/gtkitplgfk.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.aizwys.cn/gtckqgjazs.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.yuanzhike.top/gtxkuzvmil.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.hnqzz.top/gtuuhqmmlm.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.wangdashe.top/gttrhardyi.html

C#:   async Task F() { await G(); }
来源：http://hz.cucudq.cn/gtwhqjhyay.html

[O05] 并发执行并等待全部完成
来源：http://hz.yj20258888.top/gtjmbvkkds.html

Py:   asyncio.gather(*tasks)
来源：http://hz.nwbrower.top/gtnshiobpv.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.hnxiangtu.top/gtvclnpeig.html

JS:   await Promise.all(tasks)
来源：http://hz.snrcjt.cn/gtowmjfakf.html

TS:   await Promise.all(tasks)
来源：http://hz.shzxlz.cn/gtuvqfgnwa.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.wangdashe.top/gtcbpwvmex.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.zdqjudy.top/gtmukpujda.html

Ruby: threads.map(&:join)
来源：http://hz.jinghuilouyu.cn/gtjzmomcgw.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.kuanghao11.cn/gtglowkpez.html

[O06] 使用进程池
来源：http://hz.zhengqikj.top/gtsmdjefnn.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.kuanghao11.cn/gtfqqeczml.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.yueranfly.top/gtgjrhmstn.html

JS:   // child_process / cluster 模块
来源：http://hz.guannengcc.top/gtmtgtxjel.html

TS:   // child_process / cluster 模块
来源：http://hz.yangfankeji.com/gtymbsghpx.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.jqgfzy.top/gttaytdsul.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.bjfxy.top/gthnlbgjrx.html

Ruby: // fork 块
来源：http://hz.fzhhl.top/gtvpwowlca.html

C#:   Parallel.For
来源：http://hz.vqdsnc.cn/gtyavuwlai.html

================================================================================
来源：http://hz.zycfv.cn/gtocyknjav.html

P. 常用工具函数
来源：http://hz.sweek.top/gtpjtiynrg.html

================================================================================
来源：http://hz.cucudq.cn/gtbtzybvxe.html

[P01] 生成 UUID
来源：http://hz.ydjk.org.cn/gtbvkuxity.html

Py:   str(uuid.uuid4())
来源：http://hz.9152youxi.cn/gthuytxxcz.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.ybcxt.top/gtfrggjkkg.html

JS:   crypto.randomUUID()
来源：http://hz.aibaodan.cn/gtghaybyiy.html

TS:   crypto.randomUUID()
来源：http://hz.jyoumei.cn/gtmqjdaghl.html

Java: UUID.randomUUID().toString()
来源：http://hz.guannengcc.top/gtkzpvzmez.html

Go:   // 用 github.com/google/uuid
来源：http://hz.shangyingyoupin.top/gtcjljgzat.html

Ruby: SecureRandom.uuid
来源：http://hz.nanxinkj.top/gtrnaevgbq.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.tianlin.xyz/gtsjbzptcz.html

[P02] MD5 / SHA256 摘要
来源：http://hz.wangdashe.top/gtxrnchndh.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.gogol.net.cn/gtfakyzrxu.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.yj20258.top/gtmmakzptw.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.pycfn.com/gtppuhzmea.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.9152youxi.cn/gtgoordbhp.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.smart0.xyz/gtjotouxmg.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.yj20258.top/gtanloupaj.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.ehwqpu.com/gtfurvchkz.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.hongshengwenyu.top/gtlileuhck.html

[P03] 生成短随机字符串
来源：http://hz.redwolf501.top/gtfnyyvtye.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.hnqzz.top/gteyekzhoe.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.daxiang520.top/gtyxuadrgy.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.shangyingyoupin.top/gtxtrjvsky.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.hammf.cn/gttibkqmua.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.cucudq.cn/gtomssjyaz.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.shangyingyoupin.top/gtpsnmtmed.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.tianlin.xyz/gtoncwasny.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.9152youxi.cn/gtnygnxxgl.html

[P04] 求长度
来源：http://hz.zhongyouzk.top/gtjgihsdek.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.hnqzz.top/gtkhkaotzy.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.hfpthk.cn/gtzuwnulnw.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.bjfxy.top/gtheceovev.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.cdnleiting.top/gtkgpizafq.html

Java: list.size();  map.size();  s.length()
来源：http://hz.yongpay.top/gtzeqdjteg.html

Go:   len(arr);  len(m)
来源：http://hz.ywan-chungtsiang.top/gtfdtzdrjy.html

Ruby: x.length;  x.size
来源：http://hz.52xcode.cn/gtyxnhrogb.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.haohaochexian.top/gtqipbzqpf.html

[P05] 判断两个对象内容是否相等
来源：http://hz.xingfuxueyuan.xyz/gtoqcxxhcj.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.wangdashe.top/gtswqiwfxh.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.fengsongda.top/gtghfupaxd.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.yuxming.cn/gtgiehfyfp.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.feifeiyinyue.top/gthmvantsp.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.yvedp.cn/gtdgcafegi.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.ivvv.top/gtezmgvynh.html

Ruby: a == b
来源：http://hz.meibo888.top/gtdbgdsijx.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.gaohongyu789.top/gtalrmiixu.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.wangshuangyany.cn/gtbqknyyyl.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.xingfuxueyuan.xyz/gtmmukotkl.html

PHP:  if (empty($x)) {}
来源：http://hz.9152youxi.cn/gtrldrswpg.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.iojbl.cn/gtggrryjwq.html

TS:   if (x == null) {}
来源：http://hz.ehwqpu.com/gtvujtybbj.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.jqgufenzy.top/gtcprisggq.html

Go:   if x == nil {}
来源：http://hz.hnqzz.top/gtflecimvf.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.hammf.cn/gtfnxojchj.html

C#:   if (x is null) {}
来源：http://hz.cucudq.cn/gtjwiyqgzh.html

[P07] 防抖与节流
来源：http://hz.dashuyun.cn/gtbweadkdr.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.gotoacloud.top/gtivelfljb.html

PHP:  // 手写时间戳比较
来源：http://hz.yvedp.cn/gtctcdwccf.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.sysykeji.top/gtkexpwvts.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.shangyingyoupin.top/gtaeugcmbx.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.daxiang520.top/gtoazamrjs.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.yj202588.top/gtxehsnknz.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.zhixingplan.top/gttamhqmxt.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.chenzaomai.com/gtmeutilfe.html

[P08] 处理浮点精度问题
来源：http://hz.aizwys.cn/gtovdrwoqt.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.pengpengdd.cyou/gtoirmnatl.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.meibo888.top/gttbjsktuc.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.guannengcc.top/gtstitjvhs.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.zhaomingkeji.xyz/gtfgbjsvom.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.feifeiyinyue.top/gtfwgxaztg.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.svipenyu.cn/gtlaavjjyn.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.shanyushiyangkeji.top/gtykaowyzq.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.iojbl.cn/gtsziyjgpk.html

================================================================================
来源：http://hz.gaohongyu789.top/gtsqlnaznq.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.hnxiangtu.top/gtzyuawqrs.html

================================================================================
来源：http://hz.sufxvd.cn/gtwnlaceii.html

[Q01] 创建表
来源：http://hz.yongpay.top/gtbfqvigtu.html

CREATE TABLE users (
来源：http://hz.redwolf501.top/gtdjwzzviq.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.yueranfly.top/gtcsjsgvsc.html

name VARCHAR(50) NOT NULL,
来源：http://hz.c1oappe.top/gtsauzhjih.html

email VARCHAR(100) UNIQUE,
来源：http://hz.jyoumei.cn/gtiqsjrsid.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.hnxiangtu.top/gtwotqjvlt.html

);
来源：http://hz.gogol.net.cn/gtsgqabfyh.html

[Q02] 创建带外键的表
来源：http://hz.cdnleiting.top/gtjxqgtcld.html

CREATE TABLE orders (
来源：http://hz.chenlongwang.top/gtxhtefsun.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.tianlin.xyz/gtmnkirwba.html

user_id INT NOT NULL,
来源：http://hz.fengsongda.top/gttrmmppkw.html

amount DECIMAL(10, 2),
来源：http://hz.cashguo.top/gtmbssrirx.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.fzhhl.top/gtphvdcwra.html

);
来源：http://hz.shzxlz.cn/gtdktbgsoq.html

[Q03] 增加列
来源：http://hz.pengpengdd.cyou/gtpdbnyzeg.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.hammf.cn/gtckbqbzoy.html

[Q04] 修改列类型
来源：http://hz.meibo888.top/gtmmxvuuvb.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.cheryme.top/gtkbukscti.html

[Q05] 重命名列
来源：http://hz.redwolf501.top/gtemsbsujt.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.tanke756.top/gtkkvqupgw.html

[Q06] 删除列
来源：http://hz.fzhhl.top/gturardrbj.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.xingfuxueyuan.xyz/gtocjarcos.html

[Q07] 删除表
来源：http://hz.yj20258888.top/gthanyoqkk.html

DROP TABLE IF EXISTS orders;
来源：http://hz.tianlin.xyz/gtejqznzba.html

[Q08] 创建普通索引
来源：http://hz.xuanzx.com/gtzjwfibtw.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.dashuyun.cn/gtbjhdxaai.html

[Q09] 创建唯一索引
来源：http://hz.tian-w.cn/gtamcyxyse.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.wangdashe.top/gtaeuuxoge.html

[Q10] 插入单行
来源：http://hz.yueranfly.top/gticqpxllw.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.dashuyun.cn/gtisednsbc.html

[Q11] 一次插入多行
来源：http://hz.316326.xyz/gtkumdcmtg.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.sxryk.cn/gtzvohrisb.html

[Q12] 插入后取自增 ID
来源：http://hz.wangdashe.top/gtphmmbmrp.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.yj202588.top/gtwhabhklq.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.fengsongda.top/gttyiqojim.html

[Q13] 忽略重复插入
来源：http://hz.redwolf501.top/gthqjlltkm.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.zhengqikj.top/gtztsjvbmc.html

[Q14] 存在则更新（upsert）
来源：http://hz.yj20258888.top/gtitltoxeb.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.52xcode.cn/gtvxwdmpeu.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.nanxuanxn.top/gtwdubikcw.html

[Q15] 查询全部
来源：http://hz.jqgufenzy.top/gtqlmjxzlk.html

SELECT * FROM users;
来源：http://hz.ppjwa.cn/gtmmxuehut.html

[Q16] 查询指定列
来源：http://hz.zhongyouzk.top/gtgwzajgoz.html

SELECT id, name FROM users;
来源：http://hz.zhixingplan.top/gtizfpczzp.html

[Q17] 条件查询
来源：http://hz.yueranfly.top/gtmbqwdpjz.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.tianlin.xyz/gtbstdbquk.html

[Q18] 模糊匹配
来源：http://hz.daxiang520.top/gtovwgkfmt.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.shuidangran.top/gtlbqzcidf.html

[Q19] 范围查询
来源：http://hz.quarkkingdee.top/gthktuqbtg.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.yj20258888.top/gtxcaaspzn.html

[Q20] IN 列表
来源：http://hz.wangshuangyany.cn/gtabvsltjn.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.tianlin.xyz/gtjxfttlur.html

[Q21] 空值判断
来源：http://hz.hnqzz.top/gtcvqncctz.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.ppjwa.cn/gtpruxosbg.html

[Q22] 排序
来源：http://hz.ydjk.org.cn/gtglxfrsks.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.meibo888.top/gtqjnvfsoz.html

[Q23] 分页
来源：http://hz.jiagoushi.top/gtjeosavag.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.snrcjt.cn/gtvohymisx.html

[Q24] 去重
来源：http://hz.yvedp.cn/gtwkrojltb.html

SELECT DISTINCT city FROM users;
来源：http://hz.jqgufenzy.top/gtygnaplho.html

[Q25] 只取前 N 条
来源：http://hz.hnqzz.top/gtrpapskep.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.chenzaomai.com/gtnorbmebb.html

[Q26] 计数
来源：http://hz.yuanzhike.top/gtxupaqyis.html

SELECT COUNT(*) FROM users;
来源：http://hz.jiagoushi.top/gtiardrhfs.html

[Q27] 条件计数
来源：http://hz.sysykeji.top/gtcirxdyhf.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.pycfn.com/gtbdxjixqu.html

[Q28] 求和与平均
来源：http://hz.tianlin.xyz/gtabfbverx.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.jinqigufen.top/gtgubjvevn.html

[Q29] 最大最小值
来源：http://hz.fzhhl.top/gtbufezkym.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.shuidangran.top/gtbdkrcyap.html

[Q30] 分组统计
来源：http://hz.ydjk.org.cn/gtnpgbwxgu.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.xinyue.icu/gtxapnsavi.html

[Q31] 分组后过滤
来源：http://hz.nanxinkj.top/gtcnrsbewr.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.yuxming.cn/gtkigyspkd.html

[Q32] 分组拼接字符串
来源：http://hz.jianghu66.top/gtromsvczr.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.52xcode.cn/gttslehxfk.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.fzhhl.top/gtykajroig.html

[Q33] 多列分组
来源：http://hz.sysykeji.top/gtsihweixd.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.hnxiangtu.top/gtxdvzwskl.html

[Q34] 每组取第一条
来源：http://hz.iojbl.cn/gtvetnywse.html

SELECT * FROM (
来源：http://hz.vqdsnc.cn/gttqwoogrh.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.ppjwa.cn/gtytkokbez.html

) t WHERE rn = 1;
来源：http://hz.guowangkeji.top/gtfseeildg.html

[Q35] 内连接
来源：http://hz.zhixingplan.top/gtvkgsighl.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.feifeiyinyue.top/gtlehehzkk.html

[Q36] 左连接
来源：http://hz.jianghu66.top/gtpjedbnfi.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.daxiang520.top/gtfyffunur.html

[Q37] 右连接
来源：http://hz.yj202588.top/gtrxagiqgu.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.mhx1999.top/gtdfbyujqd.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.havefunace.top/gtdnjkuaow.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.cucudq.cn/gtbknbdsjc.html

[Q39] 自连接（查上下级）
来源：http://hz.kuanghao11.cn/gtijkmnkjx.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.ivvv.top/gtrhvylryw.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.gotoacloud.top/gtphztpnnj.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.haohaochexian.top/gtztcqeszz.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.iojbl.cn/gtraikujdl.html

[Q41] 多表连接
来源：http://hz.aizwys.cn/gtmvgwssui.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.nanxuanxn.top/gtggprolli.html

JOIN users u ON u.id = o.user_id
来源：http://hz.daxiang520.top/gtdpgqoyaw.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.xuetiantiany.cn/gteyyfetbs.html

[Q42] 连接条件附加过滤
来源：http://hz.yj20258.top/gtxmhidrko.html


<!-- 参考信息 -->