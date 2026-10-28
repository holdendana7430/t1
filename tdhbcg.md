代发 wailian999

Ruby: s == s.reverse
来源：http://hz.chenjidiqi.icu/gtdzimmilk.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.nwbrower.top/gtauikoqtu.html

[N07] 两数之和（返回下标）
来源：http://hz.zhixingplan.top/gttibdzwrd.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.smart0.xyz/gtvvvyvkzh.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.hammf.cn/gtihkfjmqd.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.yuanzhike.top/gtcodlgbdf.html

TS:   // 手写 Map<string, number>
来源：http://hz.tianlin.xyz/gtniahbqvj.html

Java: // 手写 HashMap
来源：http://hz.zhaomingkeji.xyz/gtxcaonfkv.html

Go:   // 手写 map[int]int
来源：http://hz.jinqigufen.top/gtihwqayet.html

Ruby: // 手写 Hash
来源：http://hz.yj20258888.top/gtqtiresgp.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.guowangkeji.top/gtsxxmzuyi.html

[N08] 生成全排列
来源：http://hz.iojbl.cn/gtymlzgegg.html

Py:   itertools.permutations(arr)
来源：http://hz.jqgufenzy.top/gtcgzwknlr.html

PHP:  // 手写递归交换
来源：http://hz.hongshengwenyu.top/gthowazoco.html

JS:   // 手写回溯递归
来源：http://hz.yj20258.top/gtzxmpjmrd.html

TS:   // 手写回溯递归
来源：http://hz.vqdsnc.cn/gtwogiglxs.html

Java: // 手写回溯递归
来源：http://hz.yueranfly.top/gtuoeqffzy.html

Go:   // 手写回溯递归
来源：http://hz.xylfe.cn/gtdtvyfjyw.html

Ruby: arr.permutation.to_a
来源：http://hz.hywenlv.cn/gtxhbqnetl.html

C#:   // 手写回溯递归
来源：http://hz.nanxuanxn.top/gtdvfgzuxv.html

[N09] 栈与队列
来源：http://hz.yonumen.top/gtytihiziu.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.9152youxi.cn/gtxvuyhjqz.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.sweek.top/gtfnlbdqdi.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.kuanghao11.cn/gtcvippapz.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.ybcxt.top/gtggwkinfz.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.jinyuanbaomall.cn/gtjuqezafj.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.dashuyun.cn/gtujighikc.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.ybcxt.top/gtseomlllx.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.cqqwz.cn/gtyicpqwbw.html

[N10] 链表节点定义
来源：http://hz.shanyushiyangkeji.top/gtadybnzto.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.ydzc1.top/gtpigoofrq.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.zdqjudy.top/gtarwfougy.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.vqdsnc.cn/gtsbbscqxi.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.ehwqpu.com/gtwghfqwjg.html

Java: class Node { int v; Node next; }
来源：http://hz.zhongyouzk.top/gtzzufnlnn.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.chenlongwang.top/gtequvhctv.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.ehwqpu.com/gtkmjrmcai.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.zhengqikj.top/gtcpazadhl.html

[N11] 二叉树中序遍历
来源：http://hz.guannengcc.top/gtsjyzcdku.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.jinyuanbaomall.cn/gtwybgjwvl.html

PHP:  // 手写递归函数
来源：http://hz.chenzaomai.com/gtiuhfnsom.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.daxiang520.top/gtuvfizofg.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.aizwys.cn/gtnfnyzsaj.html

Java: // 手写递归
来源：http://hz.yuxming.cn/gtbtlwoaii.html

Go:   // 手写递归
来源：http://hz.hnqzz.top/gtyiauckex.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.hongshengwenyu.top/gtxuhavdtl.html

C#:   // 手写递归
来源：http://hz.52xcode.cn/gtfiswzcmw.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.zhengqikj.top/gtmykthdtq.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.pengpengdd.cyou/gttcwprrld.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.xingfuxueyuan.xyz/gtqcrnrydz.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.fzhhl.top/gtmlmzfddd.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.iojbl.cn/gtvliovqgk.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.snrcjt.cn/gtlddfnjgt.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.hammf.cn/gtmjrgvhpl.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.shuidangran.top/gtcgunwzie.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.pycfn.com/gtuqkdkcqz.html

================================================================================
来源：http://hz.zhoulong.xyz/gtkpzjqvgt.html

O. 并发与异步
来源：http://hz.ydjk.org.cn/gtgoqpjhho.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gtnbagxxit.html

[O01] 启动一个线程
来源：http://hz.gzhubu.top/gtlorvxecf.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.hongshengwenyu.top/gtsgtxyanz.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.xuetiantiany.cn/gtwmigempj.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.nanxinkj.top/gthfmfhcvq.html

TS:   // 同 JS
来源：http://hz.yangfankeji.com/gtgnafleuh.html

Java: new Thread(() -> f()).start()
来源：http://hz.kuanghao11.cn/gtlfqumgyr.html

Go:   go f()
来源：http://hz.xuetiantiany.cn/gtibzxrgsc.html

Ruby: Thread.new { f }
来源：http://hz.cqqwz.cn/gtllqgxvqd.html

C#:   Task.Run(() => F());
来源：http://hz.hnxiangtu.top/gtewhlxykx.html

[O02] 使用线程池
来源：http://hz.aibaodan.cn/gtuckqcfoa.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.yvedp.cn/gtjmohnqyg.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.guannengcc.top/gtpyxafmgr.html

JS:   // worker_threads 线程池
来源：http://hz.fengsongda.top/gtkisqozdk.html

TS:   // worker_threads 线程池
来源：http://hz.redwolf501.top/gtqfwixhjc.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.0kj1m.cn/gtqacbgbws.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.cucudq.cn/gtshwijvqt.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.tian-w.cn/gtzwsaaaoc.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.daxiang520.top/gtybypstch.html

[O03] 加锁保护共享数据
来源：http://hz.haohaochexian.top/gtroootycn.html

Py:   with lock: shared += 1
来源：http://hz.zhijiandao.cn/gtbaakazdd.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.fzhhl.top/gtchfnpxxu.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.sufxvd.cn/gtjzqfosqy.html

TS:   // 同 JS
来源：http://hz.hysaishi.cn/gtkexvkugl.html

Java: synchronized (this) { shared++; }
来源：http://hz.zhijiandao.cn/gtoihalrsu.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.shangyingyoupin.top/gtdswknvvh.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.yanxiufei.cn/gtjttrvbhu.html

C#:   lock (gate) { shared++; }
来源：http://hz.zhijiandao.cn/gtrajutmet.html

[O04] 定义异步函数并等待
来源：http://hz.ydjk.org.cn/gtbntcnyhv.html

Py:   async def f():⏎    await g()
来源：http://hz.yj20258.top/gtlkabpmyn.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.ppjwa.cn/gtusokudgr.html

JS:   async function f() { await g(); }
来源：http://hz.ehwqpu.com/gtllilkyrf.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.yueranfly.top/gtqzexlfzo.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.cashguo.top/gtowhikkhj.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.yanxiufei.cn/gtwbgycugs.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.yangfankeji.com/gttbowingl.html

C#:   async Task F() { await G(); }
来源：http://hz.meibo888.top/gthljipogm.html

[O05] 并发执行并等待全部完成
来源：http://hz.hywenlv.cn/gthuykibuw.html

Py:   asyncio.gather(*tasks)
来源：http://hz.redwolf501.top/gtdfhazlgy.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.gzhubu.top/gtvhgudsak.html

JS:   await Promise.all(tasks)
来源：http://hz.jinghuilouyu.cn/gtfufjllqd.html

TS:   await Promise.all(tasks)
来源：http://hz.yj202588.top/gtzhwfmovm.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.zycfv.cn/gtzticpslr.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.ppjwa.cn/gtpromjhhc.html

Ruby: threads.map(&:join)
来源：http://hz.xylfe.cn/gtuejkwfja.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.ivvv.top/gtjvpljuwz.html

[O06] 使用进程池
来源：http://hz.fzhhl.top/gtaqnqtvub.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.xingfuxueyuan.xyz/gtejesxprv.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.nanxinkj.top/gtugpmstbq.html

JS:   // child_process / cluster 模块
来源：http://hz.cqqwz.cn/gtvevwwupl.html

TS:   // child_process / cluster 模块
来源：http://hz.zhiwuduotai.top/gtnuvikias.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.ydzc1.top/gtqbodifcn.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.iojbl.cn/gtrvvkxhij.html

Ruby: // fork 块
来源：http://hz.zhijiandao.cn/gtkyihbqkh.html

C#:   Parallel.For
来源：http://hz.xinyue.icu/gtsefqyhji.html

================================================================================
来源：http://hz.svipenyu.cn/gtunthxeum.html

P. 常用工具函数
来源：http://hz.ivvv.top/gtktoolwmy.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gtpdtzgkog.html

[P01] 生成 UUID
来源：http://hz.shanyushiyangkeji.top/gtrplipkch.html

Py:   str(uuid.uuid4())
来源：http://hz.yj202588.top/gtzkwlpucg.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.daxiang520.top/gttgxllisq.html

JS:   crypto.randomUUID()
来源：http://hz.kuanghao11.cn/gtdiapkjkc.html

TS:   crypto.randomUUID()
来源：http://hz.ehwqpu.com/gtikortcko.html

Java: UUID.randomUUID().toString()
来源：http://hz.guowangkeji.top/gttfipymqs.html

Go:   // 用 github.com/google/uuid
来源：http://hz.zycfv.cn/gtqqbdocbg.html

Ruby: SecureRandom.uuid
来源：http://hz.cashguo.top/gtrumrtryx.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.hammf.cn/gtddcrmiqb.html

[P02] MD5 / SHA256 摘要
来源：http://hz.fzhhl.top/gtactulkbc.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.pengpengdd.cyou/gtcqhpklyx.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.xylfe.cn/gtzzhrtaer.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.xziqi.cn/gtggjjryoe.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.hnqzz.top/gtotggplqa.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.hongshengwenyu.top/gtkuxfyysm.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.yangfankeji.com/gtgtlaxgii.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.nanxuanxn.top/gtymthkdik.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.guannengcc.top/gtskfejpdk.html

[P03] 生成短随机字符串
来源：http://hz.gogol.net.cn/gtzsfnjunf.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.redwolf501.top/gtzsmxwzqm.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.cucudq.cn/gtwjmorgwe.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.316326.xyz/gtykdpgyjc.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.havefunace.top/gttelvadep.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.gotoacloud.top/gtusetqdpo.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.9152youxi.cn/gtordnrhrb.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.jinyuanbaomall.cn/gtnfldvocj.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.aizwys.cn/gtutagtiiq.html

[P04] 求长度
来源：http://hz.jlsjyb.cn/gtcjlffjnd.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.tian-w.cn/gtpnpzfzjb.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.guowangkeji.top/gtsbrcruyq.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.zhongyouzk.top/gtkvipgbav.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.9152youxi.cn/gtcxcisfzo.html

Java: list.size();  map.size();  s.length()
来源：http://hz.jinghuilouyu.cn/gttbjboaqv.html

Go:   len(arr);  len(m)
来源：http://hz.chenzaomai.com/gtwedbatjc.html

Ruby: x.length;  x.size
来源：http://hz.nanxinkj.top/gtqotdxbjj.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.0kj1m.cn/gtnlezxrux.html

[P05] 判断两个对象内容是否相等
来源：http://hz.havefunace.top/gtxzfrxrgp.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.sufxvd.cn/gtgjafuttr.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.shzxlz.cn/gtzhydnxon.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.xuetiantiany.cn/gthudeuyzw.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.havefunace.top/gttunknqsw.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.hongshengwenyu.top/gtaifejqes.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.xziqi.cn/gteidzxshv.html

Ruby: a == b
来源：http://hz.ydzc1.top/gtcnagighf.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.jianghu66.top/gtnvmfxwlv.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.xingfuxueyuan.xyz/gtxqrockab.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.snrcjt.cn/gtnqamsslq.html

PHP:  if (empty($x)) {}
来源：http://hz.hnxiangtu.top/gtlilxupzl.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.jlsjyb.cn/gtmezwxkhb.html

TS:   if (x == null) {}
来源：http://hz.cdnleiting.top/gtdwuegpmj.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.ydzc1.top/gtfikiveid.html

Go:   if x == nil {}
来源：http://hz.pengpengdd.cyou/gtioshxthc.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.ydjk.org.cn/gttzthkcfz.html

C#:   if (x is null) {}
来源：http://hz.hfpthk.cn/gttdwkooif.html

[P07] 防抖与节流
来源：http://hz.pycfn.com/gtifppnjdz.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.meibo888.top/gtitetazru.html

PHP:  // 手写时间戳比较
来源：http://hz.zdqjudy.top/gtdmhhcvnx.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.aizwys.cn/gtewyaxbeb.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.jqgfzy.top/gtecssgfrj.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.daxiang520.top/gtvaeacwql.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.jqgufenzy.top/gtrrvazkzq.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.zhoulong.xyz/gtbddaaixq.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.cashguo.top/gtappytman.html

[P08] 处理浮点精度问题
来源：http://hz.sysykeji.top/gteofcrzma.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.zhaomingkeji.xyz/gtvdlagwiy.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.jinqigufen.top/gtpxkvqhud.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.vqdsnc.cn/gtpimgnton.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.hnqzz.top/gtjltengjo.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.zdqjudy.top/gtuoiaykev.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.guannengcc.top/gtlpkwkrfo.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.vqdsnc.cn/gtpvearuxf.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.zhixingplan.top/gtkuaelebk.html

================================================================================
来源：http://hz.chenzaomai.com/gtyxplbpfv.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.cucudq.cn/gtdvhgogjs.html

================================================================================
来源：http://hz.pycfn.com/gtgdjcpoua.html

[Q01] 创建表
来源：http://hz.xziqi.cn/gtbehfpccy.html

CREATE TABLE users (
来源：http://hz.ehwqpu.com/gtpxfinknu.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.xylfe.cn/gthmvaidgx.html

name VARCHAR(50) NOT NULL,
来源：http://hz.nanxinkj.top/gthtfiunwr.html

email VARCHAR(100) UNIQUE,
来源：http://hz.guannengcc.top/gtyfhxyesw.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.wangshuangyany.cn/gtiieifcjp.html

);
来源：http://hz.guannengcc.top/gtwxzhzvgb.html

[Q02] 创建带外键的表
来源：http://hz.zdqjudy.top/gtcsqkkimj.html

CREATE TABLE orders (
来源：http://hz.hongshengwenyu.top/gtrenbtlqk.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.cashguo.top/gtgmbsccle.html

user_id INT NOT NULL,
来源：http://hz.chenlongwang.top/gtsfevbreh.html

amount DECIMAL(10, 2),
来源：http://hz.yuanzhike.top/gteqljixvv.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.xylfe.cn/gtpolizycx.html

);
来源：http://hz.ydjk.org.cn/gtthretfym.html

[Q03] 增加列
来源：http://hz.wangshuangyany.cn/gtzfalickc.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.cheryme.top/gtexjjorky.html

[Q04] 修改列类型
来源：http://hz.shanyushiyangtech.top/gtvcplkjve.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.c1oappe.top/gtbdzpazzg.html

[Q05] 重命名列
来源：http://hz.xuanzx.com/gthtenjqyv.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.zhengqikj.top/gtsjqkxhdm.html

[Q06] 删除列
来源：http://hz.mhx1999.top/gtcripvqph.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.zdqjudy.top/gthifgpkdr.html

[Q07] 删除表
来源：http://hz.yueranfly.top/gtysssxjms.html

DROP TABLE IF EXISTS orders;
来源：http://hz.c1oappe.top/gtpwjsigqq.html

[Q08] 创建普通索引
来源：http://hz.tian-w.cn/gtaoaefzkw.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.kuanghao11.cn/gtnblgruhn.html

[Q09] 创建唯一索引
来源：http://hz.xuetiantiany.cn/gtwwtcqlft.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.gogol.net.cn/gtjunbtqts.html

[Q10] 插入单行
来源：http://hz.yuanzhike.top/gtgzijzlfn.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.jinqigfzy.top/gtiaxgwczb.html

[Q11] 一次插入多行
来源：http://hz.ehwqpu.com/gtjimigbsi.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.shzxlz.cn/gtnhvanofi.html

[Q12] 插入后取自增 ID
来源：http://hz.cashguo.top/gtfntriwsi.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.shanyushiyangtech.top/gtjmjbzawb.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.ydjk.org.cn/gtjadajkqo.html

[Q13] 忽略重复插入
来源：http://hz.gzhubu.top/gthqraqqyb.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.yj20258.top/gtkdfkyslw.html

[Q14] 存在则更新（upsert）
来源：http://hz.yanxiufei.cn/gtgnwpdauj.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.ydzc1.top/gtmibnhvaz.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.yvedp.cn/gtfimubiir.html

[Q15] 查询全部
来源：http://hz.cashguo.top/gtjvyonhyz.html

SELECT * FROM users;
来源：http://hz.cashguo.top/gtsgjxuywc.html

[Q16] 查询指定列
来源：http://hz.yueranfly.top/gtszvlkovb.html

SELECT id, name FROM users;
来源：http://hz.xinyue.icu/gtwjwbzvxk.html

[Q17] 条件查询
来源：http://hz.ydzc1.top/gtdyubstzs.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.hammf.cn/gtlkhgnudo.html

[Q18] 模糊匹配
来源：http://hz.birdmap.top/gtttmbocyh.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.tianlin.xyz/gtwltqqzpr.html

[Q19] 范围查询
来源：http://hz.hnqzz.top/gtlyuqdqns.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.havefunace.top/gtytpaypuj.html

[Q20] IN 列表
来源：http://hz.0kj1m.cn/gtgzmqrmty.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.andypj.xyz/gtbokppjhr.html

[Q21] 空值判断
来源：http://hz.hnxiangtu.top/gtkhsjvkdz.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.hongshengwenyu.top/gtyzfljick.html

[Q22] 排序
来源：http://hz.jinghuilouyu.cn/gtwnncwkda.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.cashguo.top/gtccywqerp.html

[Q23] 分页
来源：http://hz.cucudq.cn/gtkwpbyppt.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.jlsjyb.cn/gteqooqnza.html

[Q24] 去重
来源：http://hz.mhx1999.top/gtsyrwehzy.html

SELECT DISTINCT city FROM users;
来源：http://hz.wangshuangyany.cn/gtukkcorte.html

[Q25] 只取前 N 条
来源：http://hz.zhiwuduotai.top/gtxuonpzux.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.0kj1m.cn/gthypoxyra.html

[Q26] 计数
来源：http://hz.ydjk.org.cn/gtupgzqlwp.html

SELECT COUNT(*) FROM users;
来源：http://hz.yuanzhike.top/gtlregltdm.html

[Q27] 条件计数
来源：http://hz.ydjk.org.cn/gtnyhwxtmd.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.sufxvd.cn/gtofyfxebk.html

[Q28] 求和与平均
来源：http://hz.guannengcc.top/gtudegugsi.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.hnqzz.top/gtmvyzndtc.html

[Q29] 最大最小值
来源：http://hz.nanxinkj.top/gtpsyyxdtl.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.jinyuanbaomall.cn/gtvjucqsto.html

[Q30] 分组统计
来源：http://hz.cashguo.top/gtfsdwvcec.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.cucudq.cn/gtafotilhs.html

[Q31] 分组后过滤
来源：http://hz.9152youxi.cn/gtmzbtfsxw.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.ppjwa.cn/gtlbxdwoac.html

[Q32] 分组拼接字符串
来源：http://hz.zhaomingkeji.xyz/gtqlkzvzmu.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.ppjwa.cn/gtvopgzosa.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.kuanghao11.cn/gtnrlnyphp.html

[Q33] 多列分组
来源：http://hz.cqqwz.cn/gtbpuzkjif.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.zdqjudy.top/gtvgzzabim.html

[Q34] 每组取第一条
来源：http://hz.hywenlv.cn/gtrdozrdsv.html

SELECT * FROM (
来源：http://hz.jinyuanbaomall.cn/gttoszyqve.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.zhaomingkeji.xyz/gthviumwec.html

) t WHERE rn = 1;
来源：http://hz.guannengcc.top/gtnhhqippe.html

[Q35] 内连接
来源：http://hz.chenjidiqi.icu/gtetajafmb.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.daxiang520.top/gtqzijechd.html

[Q36] 左连接
来源：http://hz.zhoulong.xyz/gtobialrek.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.tianlin.xyz/gtebmehkbp.html

[Q37] 右连接
来源：http://hz.pycfn.com/gtqlqgldwh.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.yongpay.top/gtyqogcnez.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.nanxinkj.top/gthyqtdqby.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.jqgufenzy.top/gtubzyzmol.html

[Q39] 自连接（查上下级）
来源：http://hz.wangshuangyany.cn/gtvrjhrzsj.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.9152youxi.cn/gtpsshgrks.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.jiagoushi.top/gtbqxvesul.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.cqqwz.cn/gtwgnhydln.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.nanxinkj.top/gtxgehhjwy.html

[Q41] 多表连接
来源：http://hz.mhx1999.top/gtlmkrxdtb.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.yvedp.cn/gtggpljkab.html

JOIN users u ON u.id = o.user_id
来源：http://hz.ydjk.org.cn/gtsjdqbrkr.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.gogol.net.cn/gthcpolzkh.html

[Q42] 连接条件附加过滤
来源：http://hz.9152youxi.cn/gtejlvuzdl.html

SELECT u.name, o.amount FROM users u
来源：http://hz.svipenyu.cn/gtieowblec.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.gaohongyu789.top/gtdttntkan.html

[Q43] 标量子查询
来源：http://hz.yuanzhike.top/gthqgsapqu.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.kuanghao11.cn/gtzhwdhkss.html

[Q44] IN 子查询
来源：http://hz.jiagoushi.top/gtfmouqcjw.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.ehwqpu.com/gtchwgezsj.html

[Q45] EXISTS 判断存在
来源：http://hz.nwbrower.top/gtpttufpev.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.bjfxy.top/gttjbfgfif.html


<!-- 参考信息 -->