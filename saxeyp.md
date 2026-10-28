代发 wailian999

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.wangshuangyany.cn/gtfcikaoku.html

[N06] 判断回文字符串
来源：http://hz.aizwys.cn/gtncwfcoqg.html

Py:   s == s[::-1]
来源：http://hz.cashguo.top/gtdaynhfbh.html

PHP:  $s === strrev($s);
来源：http://hz.redwolf501.top/gtjkyxkieg.html

JS:   s === [...s].reverse().join("")
来源：http://hz.gotoacloud.top/gtdlzseshv.html

TS:   s === [...s].reverse().join("")
来源：http://hz.jiagoushi.top/gtwiedxnyi.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.jianghu66.top/gtajnppwkp.html

Go:   // 双指针从两端比较
来源：http://hz.52xcode.cn/gtqwqcbdqk.html

Ruby: s == s.reverse
来源：http://hz.jinghuilouyu.cn/gtfsegppfo.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.jianghu66.top/gtblkpqqjg.html

[N07] 两数之和（返回下标）
来源：http://hz.tianlin.xyz/gtximufnzj.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.nanxuanxn.top/gtjqzahcmy.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.birdmap.top/gtkcekmzwa.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.9152youxi.cn/gtzushkkqm.html

TS:   // 手写 Map<string, number>
来源：http://hz.316326.xyz/gttjsokwih.html

Java: // 手写 HashMap
来源：http://hz.gaohongyu789.top/gtzplotape.html

Go:   // 手写 map[int]int
来源：http://hz.guowangkeji.top/gtnilrcxcx.html

Ruby: // 手写 Hash
来源：http://hz.sxryk.cn/gtadgxwzqu.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.gotoacloud.top/gtdjejdqzl.html

[N08] 生成全排列
来源：http://hz.chenjidiqi.icu/gtdnpogugi.html

Py:   itertools.permutations(arr)
来源：http://hz.gaohongyu789.top/gtwdlryweg.html

PHP:  // 手写递归交换
来源：http://hz.ppjwa.cn/gtvrpfsvqc.html

JS:   // 手写回溯递归
来源：http://hz.xuanzx.com/gtvjbdwknz.html

TS:   // 手写回溯递归
来源：http://hz.xingfuxueyuan.xyz/gtctwrtzrs.html

Java: // 手写回溯递归
来源：http://hz.jinyuanbaomall.cn/gtbbwekmve.html

Go:   // 手写回溯递归
来源：http://hz.jyoumei.cn/gtygxmdlgq.html

Ruby: arr.permutation.to_a
来源：http://hz.andypj.xyz/gtimmrcgwd.html

C#:   // 手写回溯递归
来源：http://hz.vqdsnc.cn/gtqcvgcptg.html

[N09] 栈与队列
来源：http://hz.0kj1m.cn/gtldodbcfz.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.ydzc1.top/gttifigcwn.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.daxiang520.top/gtratjysfd.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.feifeiyinyue.top/gtfpclouja.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.dashuyun.cn/gtzlafyilt.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.chenzaomai.com/gtmzwqqocq.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.cdnleiting.top/gtvozwflxb.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.guannengcc.top/gtrxjuvalz.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.yj202588.top/gtufssteyh.html

[N10] 链表节点定义
来源：http://hz.yj202588.top/gtfucufrsu.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.quarkkingdee.top/gtjtzftbxo.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.jianghu66.top/gtzofcdsjq.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.yangfankeji.com/gtrlxrdarn.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.aibaodan.cn/gtsgblgimw.html

Java: class Node { int v; Node next; }
来源：http://hz.feifeiyinyue.top/gtaemfmyop.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.smart0.xyz/gtomufzgpr.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.ivvv.top/gtcerkioqv.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.tian-w.cn/gtbsgbmrqe.html

[N11] 二叉树中序遍历
来源：http://hz.0kj1m.cn/gthnompkjc.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.gotoacloud.top/gtdlahvkge.html

PHP:  // 手写递归函数
来源：http://hz.hnxiangtu.top/gtarwrkuel.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.ehwqpu.com/gtconvqmyo.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.sweek.top/gtiuntrcvc.html

Java: // 手写递归
来源：http://hz.c1oappe.top/gtabqmdmwf.html

Go:   // 手写递归
来源：http://hz.shanyushiyangtech.top/gthicnroft.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.yvedp.cn/gtmzvrjsss.html

C#:   // 手写递归
来源：http://hz.0kj1m.cn/gtsdruenbi.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.316326.xyz/gtbxpmvtxo.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.quarkkingdee.top/gtrbhplgyu.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.andypj.xyz/gtydarqxku.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.dianchejie.cn/gtcmzkbjyi.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.hysaishi.cn/gtqibyghzy.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.wangshuangyany.cn/gtrqnnrmej.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.gzhubu.top/gtpejuvmlo.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.zycfv.cn/gtmogcuuib.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.ydzc1.top/gtoyhmjmxq.html

================================================================================
来源：http://hz.vqdsnc.cn/gtweicoqsb.html

O. 并发与异步
来源：http://hz.nanxinkj.top/gtprwxsxah.html

================================================================================
来源：http://hz.zhiwuduotai.top/gtwcixlebj.html

[O01] 启动一个线程
来源：http://hz.feifeiyinyue.top/gtkukqsinu.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.nanxuanxn.top/gtzijdquoa.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.chenzaomai.com/gtvxffxxrb.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.gzhubu.top/gthpttnpyx.html

TS:   // 同 JS
来源：http://hz.yuxming.cn/gtorrsukuo.html

Java: new Thread(() -> f()).start()
来源：http://hz.yanxiufei.cn/gtzerjdkri.html

Go:   go f()
来源：http://hz.wangdashe.top/gtsdkvqies.html

Ruby: Thread.new { f }
来源：http://hz.bjfxy.top/gtnbscqytb.html

C#:   Task.Run(() => F());
来源：http://hz.birdmap.top/gtdhfuaqvn.html

[O02] 使用线程池
来源：http://hz.nanxuanxn.top/gtwltvxnwi.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.jinqigufen.top/gtczoksrhw.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.sysykeji.top/gthlzatmiz.html

JS:   // worker_threads 线程池
来源：http://hz.sxryk.cn/gtqrwocmsz.html

TS:   // worker_threads 线程池
来源：http://hz.xinyue.icu/gturgxhjww.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.daxiang520.top/gtywivtahg.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.yongpay.top/gtgjskyloz.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.jqgfzy.top/gtnbhipxfu.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.kuanghao11.cn/gthvngfuse.html

[O03] 加锁保护共享数据
来源：http://hz.guannengcc.top/gtycxunkra.html

Py:   with lock: shared += 1
来源：http://hz.aizwys.cn/gthtprepap.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.ydjk.org.cn/gtxtpjukuu.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.yonumen.top/gtuyvfcsym.html

TS:   // 同 JS
来源：http://hz.kuanghao11.cn/gtuqsnkamg.html

Java: synchronized (this) { shared++; }
来源：http://hz.cdnleiting.top/gtqxxztlct.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.snrcjt.cn/gtfborinha.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.jinghuilouyu.cn/gtljbbxyqc.html

C#:   lock (gate) { shared++; }
来源：http://hz.hfpthk.cn/gtqvpekbhp.html

[O04] 定义异步函数并等待
来源：http://hz.gaohongyu789.top/gtkjjkddjk.html

Py:   async def f():⏎    await g()
来源：http://hz.ywan-chungtsiang.top/gtbhuxbufz.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.quarkkingdee.top/gtwrcvekuo.html

JS:   async function f() { await g(); }
来源：http://hz.zdqjudy.top/gtkfouttwf.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.guannengcc.top/gtzpdxbkeq.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.cdnleiting.top/gtgbyfgpzw.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.yueranfly.top/gttkxoyeou.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.aibaodan.cn/gtnpkxcfsd.html

C#:   async Task F() { await G(); }
来源：http://hz.yuanzhike.top/gtjylwnmsw.html

[O05] 并发执行并等待全部完成
来源：http://hz.yuxming.cn/gtnbhcsgld.html

Py:   asyncio.gather(*tasks)
来源：http://hz.cucudq.cn/gtuxpqvsad.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.yuanzhike.top/gtffkziqkf.html

JS:   await Promise.all(tasks)
来源：http://hz.yueranfly.top/gtxscflsqw.html

TS:   await Promise.all(tasks)
来源：http://hz.redwolf501.top/gtqritekyd.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.mhx1999.top/gtunoakrbq.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.jinyuanbaomall.cn/gtqipwohde.html

Ruby: threads.map(&:join)
来源：http://hz.nanxinkj.top/gthuuweeho.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.316326.xyz/gtyceijlxh.html

[O06] 使用进程池
来源：http://hz.cucudq.cn/gtiyswqjbj.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.chenlongwang.top/gtyhrnyrat.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.ybcxt.top/gtwiqzdwdv.html

JS:   // child_process / cluster 模块
来源：http://hz.ppjwa.cn/gtvzbyqjge.html

TS:   // child_process / cluster 模块
来源：http://hz.ydjk.org.cn/gtypsvnzrb.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.hnqzz.top/gtpldwmioq.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.iojbl.cn/gtiobqbued.html

Ruby: // fork 块
来源：http://hz.hnxiangtu.top/gthhkxldix.html

C#:   Parallel.For
来源：http://hz.dianchejie.cn/gtunlpgcsp.html

================================================================================
来源：http://hz.zhongyouzk.top/gturrrkcjl.html

P. 常用工具函数
来源：http://hz.pengpengdd.cyou/gtbsysqgdk.html

================================================================================
来源：http://hz.iojbl.cn/gtowrxvrxd.html

[P01] 生成 UUID
来源：http://hz.shuidangran.top/gtunfdidct.html

Py:   str(uuid.uuid4())
来源：http://hz.wangdashe.top/gtqmnoyqpd.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.dianchejie.cn/gtzybjibzh.html

JS:   crypto.randomUUID()
来源：http://hz.ywan-chungtsiang.top/gtoukgnrim.html

TS:   crypto.randomUUID()
来源：http://hz.vqdsnc.cn/gtvakkczwl.html

Java: UUID.randomUUID().toString()
来源：http://hz.hongshengwenyu.top/gtytsiroze.html

Go:   // 用 github.com/google/uuid
来源：http://hz.xuanzx.com/gtzffdllhb.html

Ruby: SecureRandom.uuid
来源：http://hz.tanke756.top/gtmvnagizm.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.zhixingplan.top/gtxiqzfwwd.html

[P02] MD5 / SHA256 摘要
来源：http://hz.nwbrower.top/gthvrxfaut.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.yj20258.top/gtktmfjhuf.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.jinyuanbaomall.cn/gtlwguauev.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.shanyushiyangkeji.top/gtezpobfzf.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.c1oappe.top/gtbefhvruw.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.sufxvd.cn/gtkfubshbu.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.ppjwa.cn/gtuwvzvtdc.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.havefunace.top/gtgdjhlnye.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.svipenyu.cn/gtifkaedzj.html

[P03] 生成短随机字符串
来源：http://hz.cdnleiting.top/gtcpkwclyb.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.zhengqikj.top/gtosodhbkp.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.cucudq.cn/gtadrmwyfh.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.zhijiandao.cn/gtmpnvbazl.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.ivvv.top/gtlqtltbyl.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.pycfn.com/gtnrvciyzd.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.hnxiangtu.top/gtuqjbxkdb.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.yongpay.top/gtkozgtrua.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.yj20258.top/gtmgcqcokb.html

[P04] 求长度
来源：http://hz.sweek.top/gtbrxeskot.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.hfpthk.cn/gtxindbcvj.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.fzhhl.top/gtlzloxacw.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.nanxinkj.top/gtpwyipezr.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.zhaomingkeji.xyz/gtcijndvaj.html

Java: list.size();  map.size();  s.length()
来源：http://hz.quarkkingdee.top/gteybfjesh.html

Go:   len(arr);  len(m)
来源：http://hz.yanxiufei.cn/gtpxtvillr.html

Ruby: x.length;  x.size
来源：http://hz.jiagoushi.top/gtrvzfzvdz.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.andypj.xyz/gtwmjxunoh.html

[P05] 判断两个对象内容是否相等
来源：http://hz.tianlin.xyz/gtmhkqublv.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.quarkkingdee.top/gtqmxhdpqg.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.ydjk.org.cn/gtijowzkpk.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.wangshuangyany.cn/gtkgudpvwl.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.sxryk.cn/gtmhdccxxe.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.hfpthk.cn/gtyxbuiwal.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.xingfuxueyuan.xyz/gtrcwnddpt.html

Ruby: a == b
来源：http://hz.birdmap.top/gtrpnczmew.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.zhaomingkeji.xyz/gtyfrsmqjz.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.iojbl.cn/gtceqlbdjb.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.yuxming.cn/gtryksxkgu.html

PHP:  if (empty($x)) {}
来源：http://hz.sxryk.cn/gtshammmvq.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.xylfe.cn/gtirulgapu.html

TS:   if (x == null) {}
来源：http://hz.jyoumei.cn/gtrlmtokxs.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.9152youxi.cn/gtoistmpqj.html

Go:   if x == nil {}
来源：http://hz.hammf.cn/gtozfnxsfq.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.redwolf501.top/gtheydahuy.html

C#:   if (x is null) {}
来源：http://hz.xinyue.icu/gtyusvsmqq.html

[P07] 防抖与节流
来源：http://hz.shanyushiyangkeji.top/gtogkxizgm.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.pengpengdd.cyou/gtiazmgrda.html

PHP:  // 手写时间戳比较
来源：http://hz.guannengcc.top/gtcmhoacpo.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.vqdsnc.cn/gtwwwolstt.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.c1oappe.top/gtgmobvjkb.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.kuanghao11.cn/gtybvhyjrz.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.tanke756.top/gtvsahilkl.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.jianghu66.top/gtgzyqsprh.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.jinqigfzy.top/gtwwiqkfce.html

[P08] 处理浮点精度问题
来源：http://hz.yanxiufei.cn/gtkhyfblec.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.birdmap.top/gtddjwwjir.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.cqqwz.cn/gthhtthflh.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.ppjwa.cn/gtdfwrcbzd.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.smart0.xyz/gtvkcjyqkr.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.jqgufenzy.top/gttfngclza.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.meibo888.top/gtxxunyhhp.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.ydzc1.top/gtekgprxeh.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.bjfxy.top/gtbwfwxuwv.html

================================================================================
来源：http://hz.fzhhl.top/gtaehghnqc.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.andypj.xyz/gtozsxiuou.html

================================================================================
来源：http://hz.aibaodan.cn/gtjdsnjjmx.html

[Q01] 创建表
来源：http://hz.ydjk.org.cn/gtmaultdox.html

CREATE TABLE users (
来源：http://hz.yuxming.cn/gtnlibtfxs.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.jlsjyb.cn/gtlpubnpve.html

name VARCHAR(50) NOT NULL,
来源：http://hz.hywenlv.cn/gtxajpdhll.html

email VARCHAR(100) UNIQUE,
来源：http://hz.xuetiantiany.cn/gtehoejzmt.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.snrcjt.cn/gtisairbhh.html

);
来源：http://hz.hfpthk.cn/gtaxgustxc.html

[Q02] 创建带外键的表
来源：http://hz.yj20258.top/gtbkuhtano.html

CREATE TABLE orders (
来源：http://hz.nwbrower.top/gtyqlwkqug.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.zhixingplan.top/gtiwgaarpj.html

user_id INT NOT NULL,
来源：http://hz.bjfxy.top/gteywiufir.html

amount DECIMAL(10, 2),
来源：http://hz.tianlin.xyz/gthqpxflng.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.havefunace.top/gtmgphmhqd.html

);
来源：http://hz.cashguo.top/gtiyqerlgk.html

[Q03] 增加列
来源：http://hz.jqgfzy.top/gtgrarblop.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.jinghuilouyu.cn/gtojeccrkx.html

[Q04] 修改列类型
来源：http://hz.hongshengwenyu.top/gtnxhrgcfm.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.hfpthk.cn/gtzjfjehks.html

[Q05] 重命名列
来源：http://hz.yvedp.cn/gtnovygclo.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.quarkkingdee.top/gtcamtskra.html

[Q06] 删除列
来源：http://hz.zhaomingkeji.xyz/gtpyxurcxr.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.sufxvd.cn/gteyentvcv.html

[Q07] 删除表
来源：http://hz.zhongyouzk.top/gtkdtkqilu.html

DROP TABLE IF EXISTS orders;
来源：http://hz.vqdsnc.cn/gtzwwpvchi.html

[Q08] 创建普通索引
来源：http://hz.xziqi.cn/gtqaapszcu.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.jinyuanbaomall.cn/gtjeuuujez.html

[Q09] 创建唯一索引
来源：http://hz.snrcjt.cn/gtrzoeqbwy.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.zhixingplan.top/gtbfkpilcm.html

[Q10] 插入单行
来源：http://hz.quarkkingdee.top/gteilykmmh.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.jlsjyb.cn/gtwtehwodj.html

[Q11] 一次插入多行
来源：http://hz.jlsjyb.cn/gtxpztwreq.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.cashguo.top/gtriydbvvi.html

[Q12] 插入后取自增 ID
来源：http://hz.jinqigfzy.top/gttmmftdbn.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.c1oappe.top/gtamnisgco.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.guannengcc.top/gtroylnssk.html

[Q13] 忽略重复插入
来源：http://hz.ehwqpu.com/gtvhenxiwp.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.kuanghao11.cn/gtdzlyellh.html

[Q14] 存在则更新（upsert）
来源：http://hz.316326.xyz/gtkusihkox.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.nwbrower.top/gtlyivwdiq.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.zhongyouzk.top/gtwnlbsmmn.html

[Q15] 查询全部
来源：http://hz.pengpengdd.cyou/gtsbdxyauk.html

SELECT * FROM users;
来源：http://hz.svipenyu.cn/gtyfsashpj.html

[Q16] 查询指定列
来源：http://hz.sweek.top/gtyeafomkm.html

SELECT id, name FROM users;
来源：http://hz.zhoulong.xyz/gtegnmlbiv.html

[Q17] 条件查询
来源：http://hz.jqgfzy.top/gttlsjyknj.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.vqdsnc.cn/gtbohacemq.html

[Q18] 模糊匹配
来源：http://hz.jinqigufen.top/gtzqzvwdjh.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.haohaochexian.top/gtkanqtjuk.html

[Q19] 范围查询
来源：http://hz.nanxinkj.top/gtbvlwwmfl.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.hongshengwenyu.top/gtokvtymmp.html

[Q20] IN 列表
来源：http://hz.nanxinkj.top/gtqnojmrbg.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.xylfe.cn/gtdocyfhhd.html

[Q21] 空值判断
来源：http://hz.yuanzhike.top/gtbysxiwwk.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.hnxiangtu.top/gtkglotxnp.html

[Q22] 排序
来源：http://hz.nanxinkj.top/gtpzfrjjui.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.xylfe.cn/gthrckkkhf.html

[Q23] 分页
来源：http://hz.ydjk.org.cn/gtammtiolh.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.nanxinkj.top/gtfdtideyx.html

[Q24] 去重
来源：http://hz.nanxuanxn.top/gtzhpwcfzf.html

SELECT DISTINCT city FROM users;
来源：http://hz.cdnleiting.top/gtptqvvyhg.html

[Q25] 只取前 N 条
来源：http://hz.ybcxt.top/gthnifuwph.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.zhengqikj.top/gtxxlaofcu.html

[Q26] 计数
来源：http://hz.xuetiantiany.cn/gtbzkvhexg.html

SELECT COUNT(*) FROM users;
来源：http://hz.xziqi.cn/gtxdyxymiw.html

[Q27] 条件计数
来源：http://hz.hywenlv.cn/gthsdbnjey.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.haohaochexian.top/gtzgbiltsa.html

[Q28] 求和与平均
来源：http://hz.zhoulong.xyz/gtfwwhllmr.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.jinyuanbaomall.cn/gtnfbklexf.html

[Q29] 最大最小值
来源：http://hz.gotoacloud.top/gtitatxwze.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.jiagoushi.top/gtugzhahqv.html

[Q30] 分组统计
来源：http://hz.iojbl.cn/gtsdhjgsug.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.fzhhl.top/gtfirrqyfs.html

[Q31] 分组后过滤
来源：http://hz.chenzaomai.com/gtydpnmkyy.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.cucudq.cn/gtdcmymtgj.html

[Q32] 分组拼接字符串
来源：http://hz.aibaodan.cn/gtluzicual.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.ydjk.org.cn/gtnrqxjtdp.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.tanke756.top/gtqdikwzow.html

[Q33] 多列分组
来源：http://hz.gaohongyu789.top/gtpslkqtpt.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.hongshengwenyu.top/gtvulbtfwv.html

[Q34] 每组取第一条
来源：http://hz.chenlongwang.top/gtzesbzpvq.html

SELECT * FROM (
来源：http://hz.ywan-chungtsiang.top/gtgabkfsus.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.pycfn.com/gtjkdkikbb.html

) t WHERE rn = 1;
来源：http://hz.yangfankeji.com/gtcwonzmuu.html

[Q35] 内连接
来源：http://hz.ybcxt.top/gthrnxceqh.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.chenjidiqi.icu/gtkneufcrc.html

[Q36] 左连接
来源：http://hz.yanxiufei.cn/gtrqysdlrw.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.svipenyu.cn/gtuxlzcese.html

[Q37] 右连接
来源：http://hz.xziqi.cn/gttcuaxsaq.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.quarkkingdee.top/gtehkeuffs.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.chenjidiqi.icu/gtcqkymqcz.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.haohaochexian.top/gtmhmuvgzz.html

[Q39] 自连接（查上下级）
来源：http://hz.dianchejie.cn/gtfdtemoov.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.hywenlv.cn/gtdafvkbri.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.jqgufenzy.top/gtlzkkgwsa.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.tanke756.top/gtqgqfykko.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.andypj.xyz/gtyfkifcmw.html

[Q41] 多表连接
来源：http://hz.ehwqpu.com/gtfkwtpozp.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.shanyushiyangkeji.top/gtbmdtjzhv.html

JOIN users u ON u.id = o.user_id
来源：http://hz.gotoacloud.top/gtbjtexjyg.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.zdqjudy.top/gtzhqdfbmw.html

[Q42] 连接条件附加过滤
来源：http://hz.birdmap.top/gtstklkqts.html


<!-- 参考信息 -->