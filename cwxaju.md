代发 wailian999

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.hysaishi.cn/gtuqvhkvpa.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.pycfn.com/gtxkhlepzb.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.shanyushiyangkeji.top/gtqikerbzl.html

Ruby: a.gcd(b)
来源：http://hz.gzhubu.top/gteqgujvne.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.birdmap.top/gtfowbutwe.html

[N06] 判断回文字符串
来源：http://hz.zhaomingkeji.xyz/gtmydgvvgg.html

Py:   s == s[::-1]
来源：http://hz.daxiang520.top/gtyqafxali.html

PHP:  $s === strrev($s);
来源：http://hz.xylfe.cn/gtwfkdjrdp.html

JS:   s === [...s].reverse().join("")
来源：http://hz.smart0.xyz/gtnygscysf.html

TS:   s === [...s].reverse().join("")
来源：http://hz.svipenyu.cn/gtdjhhkrov.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.zhixingplan.top/gtpqwcpgcl.html

Go:   // 双指针从两端比较
来源：http://hz.tianlin.xyz/gtoxlepkzi.html

Ruby: s == s.reverse
来源：http://hz.andypj.xyz/gtomjorxzy.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.jiagoushi.top/gtkfipiboc.html

[N07] 两数之和（返回下标）
来源：http://hz.mhx1999.top/gtplnxmdso.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.hnqzz.top/gttwsbpuvj.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.nanxinkj.top/gtigynfsqc.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.mhx1999.top/gtypkbmirx.html

TS:   // 手写 Map<string, number>
来源：http://hz.yueranfly.top/gtcffjbviu.html

Java: // 手写 HashMap
来源：http://hz.snrcjt.cn/gtzdhbzuwh.html

Go:   // 手写 map[int]int
来源：http://hz.xylfe.cn/gtyvidgfvt.html

Ruby: // 手写 Hash
来源：http://hz.gotoacloud.top/gtxtelhkgi.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.yanxiufei.cn/gtinfxcckt.html

[N08] 生成全排列
来源：http://hz.zdqjudy.top/gtwzhaddcy.html

Py:   itertools.permutations(arr)
来源：http://hz.jlsjyb.cn/gticlltapa.html

PHP:  // 手写递归交换
来源：http://hz.shanyushiyangtech.top/gtabsfnaov.html

JS:   // 手写回溯递归
来源：http://hz.zhoulong.xyz/gtauqbklek.html

TS:   // 手写回溯递归
来源：http://hz.sufxvd.cn/gtrbldtooj.html

Java: // 手写回溯递归
来源：http://hz.zhiwuduotai.top/gtsamszbwg.html

Go:   // 手写回溯递归
来源：http://hz.dianchejie.cn/gtumwjilxj.html

Ruby: arr.permutation.to_a
来源：http://hz.cashguo.top/gtaumuzvrn.html

C#:   // 手写回溯递归
来源：http://hz.gzhubu.top/gtnligjozy.html

[N09] 栈与队列
来源：http://hz.shanyushiyangtech.top/gtlpwtcpgw.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.jiagoushi.top/gtqelzpqgm.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.cdnleiting.top/gtvbbbiirv.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.c1oappe.top/gtnydmmsir.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.hfpthk.cn/gtkuuvqbrp.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.pycfn.com/gtzkycjdoo.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.hysaishi.cn/gtnrapyyqk.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.daria6918.cn/gtrutvxlhg.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.shuidangran.top/gtiklhxlcp.html

[N10] 链表节点定义
来源：http://hz.yuanzhike.top/gtarxplbyg.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.jyoumei.cn/gtsspcdubj.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.hnqzz.top/gtubattrtt.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.smart0.xyz/gtrbyfzueq.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.cdnleiting.top/gtlzlptavs.html

Java: class Node { int v; Node next; }
来源：http://hz.jlsjyb.cn/gtcyexcmrf.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.nanxuanxn.top/gtxekfxpch.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.tanke756.top/gtlgophigx.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.ywan-chungtsiang.top/gtupcbmexh.html

[N11] 二叉树中序遍历
来源：http://hz.dashuyun.cn/gtfkornfca.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.birdmap.top/gtbixzbskq.html

PHP:  // 手写递归函数
来源：http://hz.jinqigufen.top/gtrrijnvsx.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.jinghuilouyu.cn/gtlwtgsxrq.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.gogol.net.cn/gtgxlrphwg.html

Java: // 手写递归
来源：http://hz.haohaochexian.top/gtboolvnck.html

Go:   // 手写递归
来源：http://hz.ybcxt.top/gtpzycvuqc.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.yonumen.top/gtptjcsfnz.html

C#:   // 手写递归
来源：http://hz.snrcjt.cn/gtuuaeroia.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.cashguo.top/gtuojbqtpt.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.wangshuangyany.cn/gtarkxosck.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.nwbrower.top/gtewitzcgy.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.andypj.xyz/gtxffworsb.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.xuetiantiany.cn/gtkvazgjvg.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.guowangkeji.top/gtjgvfpprt.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.xuanzx.com/gtibnodmlj.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.cashguo.top/gtrcozhtlb.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.dashuyun.cn/gtrtmggelb.html

================================================================================
来源：http://hz.hammf.cn/gtxehnbuaw.html

O. 并发与异步
来源：http://hz.sxryk.cn/gtkeftwypl.html

================================================================================
来源：http://hz.guannengcc.top/gtpeilagvy.html

[O01] 启动一个线程
来源：http://hz.xylfe.cn/gtkyvpnedg.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.jinqigufen.top/gteyoewerq.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.yj20258888.top/gtxrplvnws.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.zycfv.cn/gtcjkayosk.html

TS:   // 同 JS
来源：http://hz.gotoacloud.top/gtmmbqlyfh.html

Java: new Thread(() -> f()).start()
来源：http://hz.hywenlv.cn/gtaufnynxh.html

Go:   go f()
来源：http://hz.sufxvd.cn/gtpgjlfyak.html

Ruby: Thread.new { f }
来源：http://hz.redwolf501.top/gtnhmpxsww.html

C#:   Task.Run(() => F());
来源：http://hz.pengpengdd.cyou/gtqyatndyx.html

[O02] 使用线程池
来源：http://hz.dianchejie.cn/gtxgsmpsqd.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.9152youxi.cn/gtexlkzfuh.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.zycfv.cn/gtnautuqbq.html

JS:   // worker_threads 线程池
来源：http://hz.smart0.xyz/gtrpvkwsnv.html

TS:   // worker_threads 线程池
来源：http://hz.jinqigfzy.top/gtnovmqydq.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.daxiang520.top/gtntssytgc.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.hnqzz.top/gtxthitkhb.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.pengpengdd.cyou/gtwlhunyba.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.vqdsnc.cn/gtmptoinah.html

[O03] 加锁保护共享数据
来源：http://hz.yj20258888.top/gthzricwxr.html

Py:   with lock: shared += 1
来源：http://hz.ybcxt.top/gtawzlzlyj.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.gotoacloud.top/gtumelefob.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.sxryk.cn/gtwwlefggr.html

TS:   // 同 JS
来源：http://hz.shanyushiyangkeji.top/gtwsamwdtx.html

Java: synchronized (this) { shared++; }
来源：http://hz.yj20258.top/gtjhrjhccw.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.cheryme.top/gtwmyirboi.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.feifeiyinyue.top/gtorktiulm.html

C#:   lock (gate) { shared++; }
来源：http://hz.smart0.xyz/gtwrrsaear.html

[O04] 定义异步函数并等待
来源：http://hz.pengpengdd.cyou/gtyrwydtcs.html

Py:   async def f():⏎    await g()
来源：http://hz.yonumen.top/gtqohyoygg.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.52xcode.cn/gtsaiktoai.html

JS:   async function f() { await g(); }
来源：http://hz.yj202588.top/gtvpondroi.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.sweek.top/gtwpvgaonq.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.cheryme.top/gtkgakmasf.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.hfpthk.cn/gthnsdhzwz.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.nanxinkj.top/gthjxgcncb.html

C#:   async Task F() { await G(); }
来源：http://hz.hongshengwenyu.top/gtvcpgwemc.html

[O05] 并发执行并等待全部完成
来源：http://hz.meibo888.top/gtmolsicvq.html

Py:   asyncio.gather(*tasks)
来源：http://hz.xinyue.icu/gtblhkqxwe.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.jyoumei.cn/gtfdhpcmct.html

JS:   await Promise.all(tasks)
来源：http://hz.gzhubu.top/gtrrzcahtp.html

TS:   await Promise.all(tasks)
来源：http://hz.shuidangran.top/gtpgfwenac.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.svipenyu.cn/gtzxsmovxu.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.pycfn.com/gtomfiwbww.html

Ruby: threads.map(&:join)
来源：http://hz.jianghu66.top/gtldlyhfsr.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.zhiwuduotai.top/gtringncsg.html

[O06] 使用进程池
来源：http://hz.nanxuanxn.top/gtkajhbvxx.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.cheryme.top/gtbssthvyg.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.nwbrower.top/gtahhizpcf.html

JS:   // child_process / cluster 模块
来源：http://hz.nanxinkj.top/gtsmshkdqo.html

TS:   // child_process / cluster 模块
来源：http://hz.daria6918.cn/gtjjvdbtym.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.yanxiufei.cn/gtkvzvzvri.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.chenlongwang.top/gtjbhuaipb.html

Ruby: // fork 块
来源：http://hz.shzxlz.cn/gtzktzkrur.html

C#:   Parallel.For
来源：http://hz.zycfv.cn/gtwwlrhlkh.html

================================================================================
来源：http://hz.zhongyouzk.top/gtwcywhxnh.html

P. 常用工具函数
来源：http://hz.aibaodan.cn/gtjygkjyko.html

================================================================================
来源：http://hz.jinqigfzy.top/gtpvnslmrx.html

[P01] 生成 UUID
来源：http://hz.jyoumei.cn/gtehmslojn.html

Py:   str(uuid.uuid4())
来源：http://hz.bjfxy.top/gtjobuuqzi.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.yueranfly.top/gtnpyacesb.html

JS:   crypto.randomUUID()
来源：http://hz.zhaomingkeji.xyz/gtyovtggix.html

TS:   crypto.randomUUID()
来源：http://hz.316326.xyz/gtjyopogqg.html

Java: UUID.randomUUID().toString()
来源：http://hz.jyoumei.cn/gtfusqgxsq.html

Go:   // 用 github.com/google/uuid
来源：http://hz.tian-w.cn/gtzsjuqtrn.html

Ruby: SecureRandom.uuid
来源：http://hz.hnqzz.top/gtudnpsoob.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.jinyuanbaomall.cn/gtzndypvxd.html

[P02] MD5 / SHA256 摘要
来源：http://hz.jinghuilouyu.cn/gterczgslc.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.ydzc1.top/gtdocbogry.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.sysykeji.top/gtwhorqqvh.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.yuxming.cn/gtyzpprwui.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.zhiwuduotai.top/gtfkzncxjh.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.vqdsnc.cn/gtydrbrhxk.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.yongpay.top/gtembnobru.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.yvedp.cn/gtjkyycmip.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.cucudq.cn/gteknxosty.html

[P03] 生成短随机字符串
来源：http://hz.jiagoushi.top/gtjorfzend.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.zhixingplan.top/gtcisbzfmx.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.yueranfly.top/gtzcimlphx.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.kuanghao11.cn/gtqvprjeth.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.0kj1m.cn/gtnongzyry.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.c1oappe.top/gtvrvoifhz.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.guowangkeji.top/gtpgsnivfm.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.fengsongda.top/gtouymbfbj.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.feifeiyinyue.top/gtfmlnbysg.html

[P04] 求长度
来源：http://hz.sxryk.cn/gtysfydyxx.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.ivvv.top/gtgzvvofet.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.shuidangran.top/gtvtsezcyv.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.yuanzhike.top/gtinzymnow.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.sxryk.cn/gtqbeaqimk.html

Java: list.size();  map.size();  s.length()
来源：http://hz.ybcxt.top/gtiszpaqkd.html

Go:   len(arr);  len(m)
来源：http://hz.zhiwuduotai.top/gtuzynjkws.html

Ruby: x.length;  x.size
来源：http://hz.havefunace.top/gttsicfhma.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.yvedp.cn/gtktmhzldw.html

[P05] 判断两个对象内容是否相等
来源：http://hz.zhiwuduotai.top/gtgphgtmob.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.wangshuangyany.cn/gtvazhsxru.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.hysaishi.cn/gtewlejpmc.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.gaohongyu789.top/gtebpnjnua.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.zhijiandao.cn/gtssfzvgko.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.bjfxy.top/gtgbiimgtk.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.daxiang520.top/gtazglvzhk.html

Ruby: a == b
来源：http://hz.tanke756.top/gtmkwlqpgx.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.sysykeji.top/gtwisoqkvb.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.hnxiangtu.top/gtvzxxkyoo.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.birdmap.top/gtcwfyrdvs.html

PHP:  if (empty($x)) {}
来源：http://hz.zhengqikj.top/gthkugyeeu.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.zycfv.cn/gtluyiuucm.html

TS:   if (x == null) {}
来源：http://hz.jqgfzy.top/gtctpkryzh.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.feifeiyinyue.top/gtdykzdbcr.html

Go:   if x == nil {}
来源：http://hz.jinghuilouyu.cn/gtesrbvxok.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.daria6918.cn/gtguktnrdr.html

C#:   if (x is null) {}
来源：http://hz.chenzaomai.com/gtthwmlidj.html

[P07] 防抖与节流
来源：http://hz.hywenlv.cn/gtlepelbrp.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.pengpengdd.cyou/gtnthabtsm.html

PHP:  // 手写时间戳比较
来源：http://hz.316326.xyz/gtnnxtuoln.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.bjfxy.top/gtevpbglst.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.fzhhl.top/gtdwayozoq.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.bjfxy.top/gtiqhryqfg.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.shanyushiyangkeji.top/gtowpvggfu.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.ppjwa.cn/gtkvlfytuf.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.sufxvd.cn/gtwnymchpr.html

[P08] 处理浮点精度问题
来源：http://hz.hongshengwenyu.top/gtzreuiavv.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.guannengcc.top/gttqbbjpzq.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.chenlongwang.top/gtgmqswmxh.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.dianchejie.cn/gtnhiupesy.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.zhaomingkeji.xyz/gtlzxoyqkf.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.ppjwa.cn/gtjnmhtadp.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.vqdsnc.cn/gtstyazuye.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.guannengcc.top/gtvallmlqx.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.cheryme.top/gtmzjijjzp.html

================================================================================
来源：http://hz.ydjk.org.cn/gteqecasfs.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.quarkkingdee.top/gtysjqulgi.html

================================================================================
来源：http://hz.yangfankeji.com/gtsnqxfwrk.html

[Q01] 创建表
来源：http://hz.hnxiangtu.top/gtsxkmmlim.html

CREATE TABLE users (
来源：http://hz.snrcjt.cn/gtthqdtbvp.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.guowangkeji.top/gtaofrnete.html

name VARCHAR(50) NOT NULL,
来源：http://hz.smart0.xyz/gtolmrzhea.html

email VARCHAR(100) UNIQUE,
来源：http://hz.smart0.xyz/gteeonpbdy.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.svipenyu.cn/gteqrskzen.html

);
来源：http://hz.yj20258.top/gtxzewecoc.html

[Q02] 创建带外键的表
来源：http://hz.xziqi.cn/gtgvhjfyhy.html

CREATE TABLE orders (
来源：http://hz.zhengqikj.top/gthvbwroum.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.yj20258.top/gtsxjqxxjl.html

user_id INT NOT NULL,
来源：http://hz.sxryk.cn/gtobqyfpzm.html

amount DECIMAL(10, 2),
来源：http://hz.zhoulong.xyz/gtaesikofk.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.ywan-chungtsiang.top/gttccekrvw.html

);
来源：http://hz.ydzc1.top/gtahwfkwmv.html

[Q03] 增加列
来源：http://hz.gzhubu.top/gtusloiwqi.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.shanyushiyangtech.top/gthacwqicz.html

[Q04] 修改列类型
来源：http://hz.shanyushiyangkeji.top/gtotdanixg.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.shanyushiyangtech.top/gtrrpsdpzi.html

[Q05] 重命名列
来源：http://hz.gogol.net.cn/gtxsyhomnd.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.zycfv.cn/gtqzovnkoe.html

[Q06] 删除列
来源：http://hz.xylfe.cn/gtqlmjprdc.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.yangfankeji.com/gtlezibjqn.html

[Q07] 删除表
来源：http://hz.smart0.xyz/gtbgqaaafg.html

DROP TABLE IF EXISTS orders;
来源：http://hz.feifeiyinyue.top/gtzuhtchzv.html

[Q08] 创建普通索引
来源：http://hz.yj202588.top/gtantopvaf.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.yvedp.cn/gtdyxqfcra.html

[Q09] 创建唯一索引
来源：http://hz.svipenyu.cn/gtvcaptjtl.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.ybcxt.top/gttpcgjrjp.html

[Q10] 插入单行
来源：http://hz.chenjidiqi.icu/gtnqlsflvx.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.hfpthk.cn/gtnnvogukm.html

[Q11] 一次插入多行
来源：http://hz.jiagoushi.top/gtyghzxzvw.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.bjfxy.top/gthxwppetw.html

[Q12] 插入后取自增 ID
来源：http://hz.ivvv.top/gttdeypllx.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.hongshengwenyu.top/gtqyhxtpip.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.nanxuanxn.top/gtsuzodlle.html

[Q13] 忽略重复插入
来源：http://hz.zhoulong.xyz/gtlyqzoapl.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.nanxuanxn.top/gtcjbqbjug.html

[Q14] 存在则更新（upsert）
来源：http://hz.kuanghao11.cn/gtzjxyrxpi.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.xinyue.icu/gtaypusgew.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.haohaochexian.top/gtdqbnmeux.html

[Q15] 查询全部
来源：http://hz.guannengcc.top/gtidtswpnz.html

SELECT * FROM users;
来源：http://hz.quarkkingdee.top/gtbjukiskc.html

[Q16] 查询指定列
来源：http://hz.jinyuanbaomall.cn/gtyizwpwdf.html

SELECT id, name FROM users;
来源：http://hz.cashguo.top/gtlawksqie.html

[Q17] 条件查询
来源：http://hz.gogol.net.cn/gtbhtooexg.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.ywan-chungtsiang.top/gtpxpsqxvy.html

[Q18] 模糊匹配
来源：http://hz.zhengqikj.top/gthjqtmibp.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.svipenyu.cn/gtqgkseezx.html

[Q19] 范围查询
来源：http://hz.sweek.top/gtxmtxwqrm.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.daxiang520.top/gtfmxlbicd.html

[Q20] IN 列表
来源：http://hz.xuanzx.com/gtvxwbqxqe.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.zhoulong.xyz/gtjkrhwfwq.html

[Q21] 空值判断
来源：http://hz.daxiang520.top/gtdmuewltp.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.ivvv.top/gtdlrnwyym.html

[Q22] 排序
来源：http://hz.iojbl.cn/gtqtuksdek.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.xuanzx.com/gtehsakgrv.html

[Q23] 分页
来源：http://hz.cucudq.cn/gthpacggsl.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.zycfv.cn/gtuhjaiyfm.html

[Q24] 去重
来源：http://hz.yonumen.top/gtbbpkfafg.html

SELECT DISTINCT city FROM users;
来源：http://hz.hnqzz.top/gtmiyqyfuw.html

[Q25] 只取前 N 条
来源：http://hz.zhengqikj.top/gtrheessto.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.ydzc1.top/gteydvgidy.html

[Q26] 计数
来源：http://hz.vqdsnc.cn/gtbltsnkoz.html

SELECT COUNT(*) FROM users;
来源：http://hz.hnqzz.top/gtlrqncuqo.html

[Q27] 条件计数
来源：http://hz.zhengqikj.top/gthcizuqyc.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.jinyuanbaomall.cn/gtwougnetw.html

[Q28] 求和与平均
来源：http://hz.jianghu66.top/gtvggabrnt.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.yueranfly.top/gtogikwdkd.html

[Q29] 最大最小值
来源：http://hz.ydzc1.top/gtwjjknbie.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.smart0.xyz/gtxjtimfhw.html

[Q30] 分组统计
来源：http://hz.cdnleiting.top/gtvtkwyykd.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.fengsongda.top/gtgntibhju.html

[Q31] 分组后过滤
来源：http://hz.ydzc1.top/gthaqymtrx.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.yvedp.cn/gtgcmdlmcz.html

[Q32] 分组拼接字符串
来源：http://hz.shzxlz.cn/gtjzicrkzq.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.tianlin.xyz/gtlmhyxots.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.daxiang520.top/gtjqvwznoh.html

[Q33] 多列分组
来源：http://hz.quarkkingdee.top/gtafhnasco.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.52xcode.cn/gtinhzjzug.html

[Q34] 每组取第一条
来源：http://hz.ivvv.top/gthridgpvo.html

SELECT * FROM (
来源：http://hz.xuetiantiany.cn/gtyvquoouq.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.havefunace.top/gtioayzkaf.html

) t WHERE rn = 1;
来源：http://hz.sufxvd.cn/gtoyedyjol.html

[Q35] 内连接
来源：http://hz.xylfe.cn/gtzgueqmig.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.haohaochexian.top/gtekzgzzxc.html

[Q36] 左连接
来源：http://hz.aibaodan.cn/gtzrgykzzu.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.zhongyouzk.top/gthucoevja.html

[Q37] 右连接
来源：http://hz.smart0.xyz/gtgbkcjrml.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.snrcjt.cn/gtcpeajjyy.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.birdmap.top/gtjsxlkehr.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.xylfe.cn/gtgvgimkqx.html

[Q39] 自连接（查上下级）
来源：http://hz.xylfe.cn/gtajizvmqe.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.shangyingyoupin.top/gtqfzytepe.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.chenjidiqi.icu/gtkxfccjov.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.cdnleiting.top/gtjsyhpifw.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.hongshengwenyu.top/gtywaupiqa.html

[Q41] 多表连接
来源：http://hz.xylfe.cn/gtmlwgwmby.html


<!-- 参考信息 -->