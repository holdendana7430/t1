代发 wailian999

Ruby: s == s.reverse
来源：http://hz.hnqzz.top/gtgqpxcqzn.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.xingfuxueyuan.xyz/gtqthbcgdb.html

[N07] 两数之和（返回下标）
来源：http://hz.cheryme.top/gthjcibjav.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.hysaishi.cn/gtlrflhuts.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.iojbl.cn/gtmsmspvuy.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.yj20258888.top/gtpuyqwbjd.html

TS:   // 手写 Map<string, number>
来源：http://hz.daria6918.cn/gthzjeqrit.html

Java: // 手写 HashMap
来源：http://hz.yj202588.top/gtzayttcny.html

Go:   // 手写 map[int]int
来源：http://hz.gogol.net.cn/gtubnqdnqm.html

Ruby: // 手写 Hash
来源：http://hz.hysaishi.cn/gtmaheofee.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.xingfuxueyuan.xyz/gtyfkswbet.html

[N08] 生成全排列
来源：http://hz.andypj.xyz/gthanppdrm.html

Py:   itertools.permutations(arr)
来源：http://hz.jinqigfzy.top/gtndhjnwqt.html

PHP:  // 手写递归交换
来源：http://hz.ivvv.top/gtbwxpfpwg.html

JS:   // 手写回溯递归
来源：http://hz.nanxuanxn.top/gtwfkjzbox.html

TS:   // 手写回溯递归
来源：http://hz.ywan-chungtsiang.top/gtcatewzki.html

Java: // 手写回溯递归
来源：http://hz.xingfuxueyuan.xyz/gtzqnzigas.html

Go:   // 手写回溯递归
来源：http://hz.redwolf501.top/gtmeqrqlcc.html

Ruby: arr.permutation.to_a
来源：http://hz.ybcxt.top/gtdgiqsaaj.html

C#:   // 手写回溯递归
来源：http://hz.yvedp.cn/gtraxvwasd.html

[N09] 栈与队列
来源：http://hz.316326.xyz/gtxtbrnerc.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.dianchejie.cn/gttebzxhfl.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.guowangkeji.top/gteusqggzb.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.haohaochexian.top/gtutnyqhlt.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.gogol.net.cn/gtfussdbso.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.bjfxy.top/gtlrujjday.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.pengpengdd.cyou/gtepqykrmt.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.hywenlv.cn/gtqxyyvcan.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.zhaomingkeji.xyz/gtwoyrxvno.html

[N10] 链表节点定义
来源：http://hz.yj20258.top/gtbsuyuvgp.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.yvedp.cn/gthyhjslcj.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.guowangkeji.top/gtvvmsylnx.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.ywan-chungtsiang.top/gtgzbuhvfs.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.pengpengdd.cyou/gtgzrdarut.html

Java: class Node { int v; Node next; }
来源：http://hz.chenjidiqi.icu/gtqwnrkspk.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.yvedp.cn/gtoqggmvpw.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.zhongyouzk.top/gtcspzouct.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.meibo888.top/gtgakrqwfe.html

[N11] 二叉树中序遍历
来源：http://hz.zhijiandao.cn/gtwofmdjhx.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.svipenyu.cn/gtakxxvmds.html

PHP:  // 手写递归函数
来源：http://hz.hfpthk.cn/gththfotiv.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.sufxvd.cn/gtnjqubcwp.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.dashuyun.cn/gttvgtwiei.html

Java: // 手写递归
来源：http://hz.haohaochexian.top/gtrgegsrwb.html

Go:   // 手写递归
来源：http://hz.52xcode.cn/gthnfbjnwe.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.zycfv.cn/gtndppvkyc.html

C#:   // 手写递归
来源：http://hz.zhiwuduotai.top/gtrvgokrup.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.ydzc1.top/gtdqayygvx.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.snrcjt.cn/gtzblrwrdr.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.dashuyun.cn/gtoqkjvksn.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.iojbl.cn/gtowvuvyoa.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.yj20258.top/gtxggrdgro.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.52xcode.cn/gtmtfjgefa.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.aizwys.cn/gtjitxgcdu.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.zhengqikj.top/gtmvfhsdnw.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.wangshuangyany.cn/gtlbenbtxi.html

================================================================================
来源：http://hz.xylfe.cn/gtnvhedndu.html

O. 并发与异步
来源：http://hz.ydjk.org.cn/gtyxtyscdd.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtggautakx.html

[O01] 启动一个线程
来源：http://hz.ywan-chungtsiang.top/gtpsymqktv.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.shzxlz.cn/gtlomhnrla.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.nwbrower.top/gttnztisir.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.birdmap.top/gtpqxicakj.html

TS:   // 同 JS
来源：http://hz.shanyushiyangkeji.top/gtoimqwyej.html

Java: new Thread(() -> f()).start()
来源：http://hz.shanyushiyangkeji.top/gtsivjqskk.html

Go:   go f()
来源：http://hz.ppjwa.cn/gtvaevyvhq.html

Ruby: Thread.new { f }
来源：http://hz.hysaishi.cn/gtjezrrxcg.html

C#:   Task.Run(() => F());
来源：http://hz.daxiang520.top/gtageqaizf.html

[O02] 使用线程池
来源：http://hz.hysaishi.cn/gtuteeqcjg.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.quarkkingdee.top/gtjkwpdxud.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.xuetiantiany.cn/gtylqiflfq.html

JS:   // worker_threads 线程池
来源：http://hz.fzhhl.top/gtbnnbykuq.html

TS:   // worker_threads 线程池
来源：http://hz.xziqi.cn/gtyuepnyvz.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.haohaochexian.top/gtxacliqtb.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.xziqi.cn/gtlcagetrx.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.yonumen.top/gtxysyyrro.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.meibo888.top/gtaalvrduc.html

[O03] 加锁保护共享数据
来源：http://hz.daria6918.cn/gtwseywhza.html

Py:   with lock: shared += 1
来源：http://hz.shzxlz.cn/gtmxdrdhcf.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.tanke756.top/gtogyaeant.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.jianghu66.top/gtnmkynhro.html

TS:   // 同 JS
来源：http://hz.ybcxt.top/gtjojlrojp.html

Java: synchronized (this) { shared++; }
来源：http://hz.fengsongda.top/gtjbtxpilh.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.gotoacloud.top/gtxwomflrb.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.yj20258.top/gtjkphsrgn.html

C#:   lock (gate) { shared++; }
来源：http://hz.feifeiyinyue.top/gtlrssvhrt.html

[O04] 定义异步函数并等待
来源：http://hz.fzhhl.top/gtooaarqsu.html

Py:   async def f():⏎    await g()
来源：http://hz.tanke756.top/gtxlpnoxwp.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.zycfv.cn/gtuaxvqcxd.html

JS:   async function f() { await g(); }
来源：http://hz.dashuyun.cn/gtfkcdyfkx.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.andypj.xyz/gttscczeng.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.52xcode.cn/gtezfntpvg.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.snrcjt.cn/gtdvhwianh.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.chenzaomai.com/gtdoeptsnb.html

C#:   async Task F() { await G(); }
来源：http://hz.quarkkingdee.top/gtuucrzvwr.html

[O05] 并发执行并等待全部完成
来源：http://hz.jianghu66.top/gtlnjixcet.html

Py:   asyncio.gather(*tasks)
来源：http://hz.nanxinkj.top/gtywlptmwg.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.yueranfly.top/gtztpmpehx.html

JS:   await Promise.all(tasks)
来源：http://hz.yonumen.top/gtppzkjroh.html

TS:   await Promise.all(tasks)
来源：http://hz.zhiwuduotai.top/gtcbjcunkb.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.dianchejie.cn/gtbsmvyblg.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.ybcxt.top/gtphkdbahb.html

Ruby: threads.map(&:join)
来源：http://hz.ybcxt.top/gtxfhpxulo.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.meibo888.top/gtndojxccl.html

[O06] 使用进程池
来源：http://hz.jinghuilouyu.cn/gttocjxrxi.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.daxiang520.top/gtnvulsbct.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.chenjidiqi.icu/gtveyrqvxg.html

JS:   // child_process / cluster 模块
来源：http://hz.tianlin.xyz/gtvndknulx.html

TS:   // child_process / cluster 模块
来源：http://hz.chenzaomai.com/gtdmgnphna.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.hysaishi.cn/gtbwehwzir.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.zhijiandao.cn/gtmeuebhvg.html

Ruby: // fork 块
来源：http://hz.yanxiufei.cn/gtizhbbyvv.html

C#:   Parallel.For
来源：http://hz.bjfxy.top/gtkjivxqku.html

================================================================================
来源：http://hz.cashguo.top/gtjamhhcaq.html

P. 常用工具函数
来源：http://hz.ivvv.top/gtzvfrcnlm.html

================================================================================
来源：http://hz.yj20258888.top/gtdxonevcf.html

[P01] 生成 UUID
来源：http://hz.yj20258.top/gtgzlxapwr.html

Py:   str(uuid.uuid4())
来源：http://hz.ybcxt.top/gtifkjilaw.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.hnqzz.top/gtkxsatngk.html

JS:   crypto.randomUUID()
来源：http://hz.pycfn.com/gtbmtgmchw.html

TS:   crypto.randomUUID()
来源：http://hz.jianghu66.top/gtumckjbgu.html

Java: UUID.randomUUID().toString()
来源：http://hz.wangshuangyany.cn/gtvpbryura.html

Go:   // 用 github.com/google/uuid
来源：http://hz.jinghuilouyu.cn/gtlticwwso.html

Ruby: SecureRandom.uuid
来源：http://hz.redwolf501.top/gtaaablacg.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.hnqzz.top/gtersmwprv.html

[P02] MD5 / SHA256 摘要
来源：http://hz.fzhhl.top/gtdaknowyr.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.zhongyouzk.top/gtovqdxevu.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.meibo888.top/gtrwbuqmgq.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.ppjwa.cn/gttqksuysm.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.xuanzx.com/gtgilrfhqy.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.iojbl.cn/gtugqryffr.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.xuetiantiany.cn/gtiaryvcqx.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.zhoulong.xyz/gtsxiulakn.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.zhengqikj.top/gtouvngmak.html

[P03] 生成短随机字符串
来源：http://hz.tianlin.xyz/gthlzowxcc.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.pycfn.com/gtnbmobuja.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.zhiwuduotai.top/gtjjqxxvsk.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.nwbrower.top/gtgwrtpytr.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.jinqigfzy.top/gtadhjfvlv.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.cdnleiting.top/gtxnsiispz.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.andypj.xyz/gtawiwfifm.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.pycfn.com/gterpabzzf.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.c1oappe.top/gtuumhdnwu.html

[P04] 求长度
来源：http://hz.havefunace.top/gtdvyandrn.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.iojbl.cn/gtwahdpghs.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.ybcxt.top/gtxibfjfvl.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.sysykeji.top/gtjfgtlwxy.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.aibaodan.cn/gtkjrkazjf.html

Java: list.size();  map.size();  s.length()
来源：http://hz.iojbl.cn/gtwvzdhrgm.html

Go:   len(arr);  len(m)
来源：http://hz.iojbl.cn/gtxwigxnmu.html

Ruby: x.length;  x.size
来源：http://hz.yj20258.top/gtgzykoftg.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.yueranfly.top/gtcpgaqagy.html

[P05] 判断两个对象内容是否相等
来源：http://hz.nanxuanxn.top/gtleyzhxax.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.dianchejie.cn/gtdkpwfimn.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.jqgufenzy.top/gtmgcyxadi.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.xuetiantiany.cn/gtjkefjotj.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.zhongyouzk.top/gtmmrahosc.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.sxryk.cn/gtmcsflqbr.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.fzhhl.top/gtsqsdwmuh.html

Ruby: a == b
来源：http://hz.yj20258.top/gtkmefrras.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.52xcode.cn/gtereqydmp.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.gotoacloud.top/gtqofumiyg.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.zdqjudy.top/gtoisbxmyv.html

PHP:  if (empty($x)) {}
来源：http://hz.shangyingyoupin.top/gtlefdntsb.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.zhengqikj.top/gtlmkgmowu.html

TS:   if (x == null) {}
来源：http://hz.cashguo.top/gtbqlsbzec.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.gogol.net.cn/gtirndhdyt.html

Go:   if x == nil {}
来源：http://hz.ehwqpu.com/gtubxctmqt.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.jlsjyb.cn/gtgqjafrdh.html

C#:   if (x is null) {}
来源：http://hz.316326.xyz/gtejohqcls.html

[P07] 防抖与节流
来源：http://hz.hnqzz.top/gtkowlqnrh.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.52xcode.cn/gtultjowtz.html

PHP:  // 手写时间戳比较
来源：http://hz.birdmap.top/gttnvrtjfz.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.zhixingplan.top/gtrwbftdgb.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.hnxiangtu.top/gtgmoamxhl.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.jinqigufen.top/gtkesjtkwy.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.pycfn.com/gtjunkwxlx.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.shangyingyoupin.top/gtefnodway.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.jqgufenzy.top/gtsaorrzkw.html

[P08] 处理浮点精度问题
来源：http://hz.aizwys.cn/gtujzdepcz.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.xuanzx.com/gtbembyszv.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.gzhubu.top/gtgeytdwdm.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.gotoacloud.top/gttlhrpxoa.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.jlsjyb.cn/gtraafmmup.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.smart0.xyz/gtlrtpqisu.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.daria6918.cn/gtjkymjxrv.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.jqgufenzy.top/gtcbrpbqby.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.andypj.xyz/gtapkawsdy.html

================================================================================
来源：http://hz.yonumen.top/gttdoujyou.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.svipenyu.cn/gtouvgotik.html

================================================================================
来源：http://hz.dianchejie.cn/gtmrthikzt.html

[Q01] 创建表
来源：http://hz.guowangkeji.top/gtpxoflyus.html

CREATE TABLE users (
来源：http://hz.ydjk.org.cn/gtmfeeuilc.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.ydjk.org.cn/gtfzlxzvxs.html

name VARCHAR(50) NOT NULL,
来源：http://hz.zhaomingkeji.xyz/gtsokoubss.html

email VARCHAR(100) UNIQUE,
来源：http://hz.nanxinkj.top/gtslgylmvh.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.chenzaomai.com/gtkqjllfbv.html

);
来源：http://hz.yonumen.top/gtuyhxslhh.html

[Q02] 创建带外键的表
来源：http://hz.zycfv.cn/gtfwzbhtop.html

CREATE TABLE orders (
来源：http://hz.9152youxi.cn/gtwjnbptap.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.316326.xyz/gtareuayfr.html

user_id INT NOT NULL,
来源：http://hz.vqdsnc.cn/gtiaomumjz.html

amount DECIMAL(10, 2),
来源：http://hz.zhixingplan.top/gtehxoarbf.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.hnqzz.top/gteeuzvklt.html

);
来源：http://hz.ehwqpu.com/gtwmafusye.html

[Q03] 增加列
来源：http://hz.ppjwa.cn/gtsjlehaho.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.yuanzhike.top/gtlblpfans.html

[Q04] 修改列类型
来源：http://hz.smart0.xyz/gtxcxudasg.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.quarkkingdee.top/gteqrxdydn.html

[Q05] 重命名列
来源：http://hz.nanxinkj.top/gtfwjndpmt.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.hysaishi.cn/gtdkdhobbh.html

[Q06] 删除列
来源：http://hz.birdmap.top/gtbskkpgru.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.316326.xyz/gttqcaamsu.html

[Q07] 删除表
来源：http://hz.aibaodan.cn/gtowzraxes.html

DROP TABLE IF EXISTS orders;
来源：http://hz.smart0.xyz/gtxpzwblpq.html

[Q08] 创建普通索引
来源：http://hz.ydjk.org.cn/gtnekimrrz.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.zhoulong.xyz/gtleigoisw.html

[Q09] 创建唯一索引
来源：http://hz.c1oappe.top/gtyjjkudzj.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.wangshuangyany.cn/gtnqvdicgy.html

[Q10] 插入单行
来源：http://hz.hnqzz.top/gtvrqhhyas.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.snrcjt.cn/gtmyjrbgcn.html

[Q11] 一次插入多行
来源：http://hz.sysykeji.top/gtskvirmdv.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.chenzaomai.com/gtjpsfumre.html

[Q12] 插入后取自增 ID
来源：http://hz.birdmap.top/gtiptbwwzb.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.gaohongyu789.top/gtvcujjkgc.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.daria6918.cn/gtkxzsyulu.html

[Q13] 忽略重复插入
来源：http://hz.9152youxi.cn/gtkwdvdtrv.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.zhongyouzk.top/gtymcdfjcc.html

[Q14] 存在则更新（upsert）
来源：http://hz.ivvv.top/gtmjfktfgy.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.ppjwa.cn/gtokcwqgel.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.cdnleiting.top/gtoiuklkoz.html

[Q15] 查询全部
来源：http://hz.hywenlv.cn/gtdeckjqik.html

SELECT * FROM users;
来源：http://hz.wangdashe.top/gthkxhzyat.html

[Q16] 查询指定列
来源：http://hz.yj202588.top/gtklnqhbjz.html

SELECT id, name FROM users;
来源：http://hz.wangdashe.top/gtzxibfwzy.html

[Q17] 条件查询
来源：http://hz.ybcxt.top/gtgdfzqjna.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.yuanzhike.top/gttdhhrfws.html

[Q18] 模糊匹配
来源：http://hz.jyoumei.cn/gtzmoypvfm.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.zhiwuduotai.top/gthozxcpye.html

[Q19] 范围查询
来源：http://hz.cheryme.top/gtuivzkxbv.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.gzhubu.top/gtoeyqjksd.html

[Q20] IN 列表
来源：http://hz.zdqjudy.top/gtktsujyzn.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.jinqigufen.top/gtqvpedfoq.html

[Q21] 空值判断
来源：http://hz.yanxiufei.cn/gtgperluyr.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.yj20258.top/gtoragbpqn.html

[Q22] 排序
来源：http://hz.ydzc1.top/gtxyoqxaxf.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.gogol.net.cn/gtlbqimlqi.html

[Q23] 分页
来源：http://hz.hfpthk.cn/gtzjnwdrqh.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.jiagoushi.top/gteqquwoxv.html

[Q24] 去重
来源：http://hz.shzxlz.cn/gtxtsbvocp.html

SELECT DISTINCT city FROM users;
来源：http://hz.snrcjt.cn/gtpcjwxovk.html

[Q25] 只取前 N 条
来源：http://hz.fzhhl.top/gtdeiqqqvc.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.ppjwa.cn/gtoicipzqm.html

[Q26] 计数
来源：http://hz.xuanzx.com/gtjyzyatmj.html

SELECT COUNT(*) FROM users;
来源：http://hz.wangshuangyany.cn/gtchrfvjpc.html

[Q27] 条件计数
来源：http://hz.hongshengwenyu.top/gtcqzjsygi.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.sweek.top/gtzeaesaea.html

[Q28] 求和与平均
来源：http://hz.jinghuilouyu.cn/gtpbheaakn.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.xuetiantiany.cn/gtmcheolvx.html

[Q29] 最大最小值
来源：http://hz.chenzaomai.com/gtzdomwdta.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.zycfv.cn/gtgghijjcm.html

[Q30] 分组统计
来源：http://hz.cashguo.top/gtyerhghjp.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.yuxming.cn/gtercgzcqd.html

[Q31] 分组后过滤
来源：http://hz.yongpay.top/gttedzxtgg.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.pycfn.com/gtopidrgtc.html

[Q32] 分组拼接字符串
来源：http://hz.yangfankeji.com/gtrtwkwszc.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.ydjk.org.cn/gtkevipgca.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.hammf.cn/gtnnhypskh.html

[Q33] 多列分组
来源：http://hz.hfpthk.cn/gtgviovxtl.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.shanyushiyangkeji.top/gtdjonwkqy.html

[Q34] 每组取第一条
来源：http://hz.jlsjyb.cn/gtmmkjmyrh.html

SELECT * FROM (
来源：http://hz.tian-w.cn/gtqwtryruj.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.zhoulong.xyz/gtjexjikow.html

) t WHERE rn = 1;
来源：http://hz.yongpay.top/gtnodoekyd.html

[Q35] 内连接
来源：http://hz.tanke756.top/gtftbtqqzs.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.wangdashe.top/gtarrjqnzc.html

[Q36] 左连接
来源：http://hz.ydzc1.top/gtxjlbacee.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.jinyuanbaomall.cn/gtridfwjjp.html

[Q37] 右连接
来源：http://hz.bjfxy.top/gtmoukecek.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.jqgfzy.top/gtjbzpaouo.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.jinqigfzy.top/gtbegdooim.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.tian-w.cn/gtbrlptwby.html

[Q39] 自连接（查上下级）
来源：http://hz.aibaodan.cn/gtbscuvtzd.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.sysykeji.top/gtuogaljsi.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.quarkkingdee.top/gtxkepbdlh.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.nanxuanxn.top/gtwnwczhrv.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.ppjwa.cn/gttmncgtef.html

[Q41] 多表连接
来源：http://hz.guowangkeji.top/gtiofwflen.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.fengsongda.top/gtbsjgaarl.html

JOIN users u ON u.id = o.user_id
来源：http://hz.andypj.xyz/gtmmnomzsw.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.xylfe.cn/gtnrhhprhn.html

[Q42] 连接条件附加过滤
来源：http://hz.xylfe.cn/gtwcgkvxuh.html

SELECT u.name, o.amount FROM users u
来源：http://hz.svipenyu.cn/gtupbywjsb.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.zhijiandao.cn/gtpspyxsui.html

[Q43] 标量子查询
来源：http://hz.svipenyu.cn/gtbgjglakm.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.hongshengwenyu.top/gthxdgfpsx.html

[Q44] IN 子查询
来源：http://hz.chenjidiqi.icu/gtwzlmjihp.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.zhoulong.xyz/gtildesnft.html

[Q45] EXISTS 判断存在
来源：http://hz.yuxming.cn/gttflsjpsb.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.birdmap.top/gtlfipwxvl.html


<!-- 参考信息 -->