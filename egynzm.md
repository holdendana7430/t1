代发 wailian999

Ruby: s == s.reverse
来源：http://hz.zhijiandao.cn/gtcpkawyex.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.xylfe.cn/gthjistuze.html

[N07] 两数之和（返回下标）
来源：http://hz.sufxvd.cn/gtnwpnvmcf.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.wangdashe.top/gtuuwiuncm.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.xuetiantiany.cn/gtrvtxomot.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.hnxiangtu.top/gtazzjwvgz.html

TS:   // 手写 Map<string, number>
来源：http://hz.zhixingplan.top/gtsckishea.html

Java: // 手写 HashMap
来源：http://hz.52xcode.cn/gtdleyjasm.html

Go:   // 手写 map[int]int
来源：http://hz.xuanzx.com/gtkbdhmtnw.html

Ruby: // 手写 Hash
来源：http://hz.guannengcc.top/gtohucvdxr.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.yj20258.top/gtcxqprcvm.html

[N08] 生成全排列
来源：http://hz.316326.xyz/gtwlnimehh.html

Py:   itertools.permutations(arr)
来源：http://hz.wangshuangyany.cn/gtebmjtsfg.html

PHP:  // 手写递归交换
来源：http://hz.ehwqpu.com/gtykvfhzru.html

JS:   // 手写回溯递归
来源：http://hz.shangyingyoupin.top/gtyjnnykbm.html

TS:   // 手写回溯递归
来源：http://hz.havefunace.top/gtdpxpvgmk.html

Java: // 手写回溯递归
来源：http://hz.wangdashe.top/gtcwpwbkot.html

Go:   // 手写回溯递归
来源：http://hz.dashuyun.cn/gtvgvaormv.html

Ruby: arr.permutation.to_a
来源：http://hz.hammf.cn/gtkffghnsb.html

C#:   // 手写回溯递归
来源：http://hz.tian-w.cn/gtxhullbej.html

[N09] 栈与队列
来源：http://hz.yonumen.top/gtrnsxjdky.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.shuidangran.top/gthjvwqbhb.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.dianchejie.cn/gteccbwyxq.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.yuxming.cn/gtpkevtoae.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.nanxuanxn.top/gttajddsyl.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.wangdashe.top/gteehfxrzd.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.tian-w.cn/gtppxhpsro.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.aizwys.cn/gtlsxdmyqs.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.zhiwuduotai.top/gttxousgaz.html

[N10] 链表节点定义
来源：http://hz.sweek.top/gtelmrzxpx.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.bjfxy.top/gtyfnckybb.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.ivvv.top/gtmtrdjiku.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.yj202588.top/gtcpsjqgxd.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.yuanzhike.top/gtjuyxyszw.html

Java: class Node { int v; Node next; }
来源：http://hz.andypj.xyz/gtizvftrtx.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.jiagoushi.top/gtyatfvnpk.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.bjfxy.top/gtgeybohxl.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.zhixingplan.top/gtituamhad.html

[N11] 二叉树中序遍历
来源：http://hz.ybcxt.top/gtosygdgnp.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.zhixingplan.top/gtfuysxuus.html

PHP:  // 手写递归函数
来源：http://hz.kuanghao11.cn/gtsjdpyoht.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.yvedp.cn/gtmahowpvf.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.fzhhl.top/gthewoaiem.html

Java: // 手写递归
来源：http://hz.yj20258.top/gtaoettkbw.html

Go:   // 手写递归
来源：http://hz.cdnleiting.top/gtpjrwqwtt.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.nanxinkj.top/gtchwwhrbe.html

C#:   // 手写递归
来源：http://hz.sxryk.cn/gtgqgoddix.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.shangyingyoupin.top/gtxmzpvlot.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.shangyingyoupin.top/gtxhotiqqh.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.zhijiandao.cn/gtsqmaewut.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.gzhubu.top/gtgfnwtojb.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.jyoumei.cn/gtuvqvunwd.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.yanxiufei.cn/gtgtjflrkt.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.9152youxi.cn/gttochmspp.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.zhaomingkeji.xyz/gtdoqmrktq.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.yonumen.top/gtfgaslref.html

================================================================================
来源：http://hz.tianlin.xyz/gtjljammir.html

O. 并发与异步
来源：http://hz.sxryk.cn/gtragajgkc.html

================================================================================
来源：http://hz.zhixingplan.top/gtpxomrwqy.html

[O01] 启动一个线程
来源：http://hz.xuetiantiany.cn/gtjrauemxp.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.cheryme.top/gtspywezvh.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.gaohongyu789.top/gtokimtjwy.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.jiagoushi.top/gtbriukncp.html

TS:   // 同 JS
来源：http://hz.cdnleiting.top/gtizycrsek.html

Java: new Thread(() -> f()).start()
来源：http://hz.yj202588.top/gtxlwszyzv.html

Go:   go f()
来源：http://hz.daria6918.cn/gtpvrwnisb.html

Ruby: Thread.new { f }
来源：http://hz.xylfe.cn/gtjhrtasbs.html

C#:   Task.Run(() => F());
来源：http://hz.cashguo.top/gtnctdstca.html

[O02] 使用线程池
来源：http://hz.zycfv.cn/gtkpmoifow.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.ywan-chungtsiang.top/gtxvgzxnev.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.ppjwa.cn/gtsdcznxcq.html

JS:   // worker_threads 线程池
来源：http://hz.xylfe.cn/gtquspuadr.html

TS:   // worker_threads 线程池
来源：http://hz.shangyingyoupin.top/gtjxhjyqcg.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.jinyuanbaomall.cn/gtjejtaepy.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.pycfn.com/gtjsubwnmv.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.gotoacloud.top/gtvbsesuor.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.jiagoushi.top/gtkyjzgpvy.html

[O03] 加锁保护共享数据
来源：http://hz.yj202588.top/gtkreubtku.html

Py:   with lock: shared += 1
来源：http://hz.tian-w.cn/gtiymdsdsw.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.xuetiantiany.cn/gtgcwwhjrk.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.tianlin.xyz/gtqbeaxqxf.html

TS:   // 同 JS
来源：http://hz.cheryme.top/gtwnttwpwl.html

Java: synchronized (this) { shared++; }
来源：http://hz.cqqwz.cn/gthzxhmutl.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.ybcxt.top/gtooaghlop.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.jinqigfzy.top/gtvvchxhys.html

C#:   lock (gate) { shared++; }
来源：http://hz.daria6918.cn/gtjzznuljx.html

[O04] 定义异步函数并等待
来源：http://hz.haohaochexian.top/gtarbicssf.html

Py:   async def f():⏎    await g()
来源：http://hz.yueranfly.top/gtgcisonni.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.svipenyu.cn/gtiojybudk.html

JS:   async function f() { await g(); }
来源：http://hz.iojbl.cn/gtvhonijvk.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.c1oappe.top/gtbuzmilwu.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.ppjwa.cn/gtkeqojlrz.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.andypj.xyz/gteimshuvo.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.jqgufenzy.top/gtyvtdskdv.html

C#:   async Task F() { await G(); }
来源：http://hz.zhoulong.xyz/gtqntgwfoj.html

[O05] 并发执行并等待全部完成
来源：http://hz.yuxming.cn/gtpyqrwdtf.html

Py:   asyncio.gather(*tasks)
来源：http://hz.guowangkeji.top/gtgmpudtxa.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.xylfe.cn/gtzigqfova.html

JS:   await Promise.all(tasks)
来源：http://hz.shzxlz.cn/gtxibtuxqi.html

TS:   await Promise.all(tasks)
来源：http://hz.guannengcc.top/gtlwwtcgvk.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.yvedp.cn/gtjxdjyrbn.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.316326.xyz/gtuwndutgl.html

Ruby: threads.map(&:join)
来源：http://hz.cdnleiting.top/gtieqgirrb.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.0kj1m.cn/gtkpyeyhvy.html

[O06] 使用进程池
来源：http://hz.jlsjyb.cn/gtatyjifmb.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.sufxvd.cn/gtczqzubvw.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.iojbl.cn/gtmxfcakip.html

JS:   // child_process / cluster 模块
来源：http://hz.chenlongwang.top/gtnxrdmfod.html

TS:   // child_process / cluster 模块
来源：http://hz.jianghu66.top/gtyixsrthk.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.meibo888.top/gteeyzrmhp.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.zhaomingkeji.xyz/gthmmetmgd.html

Ruby: // fork 块
来源：http://hz.9152youxi.cn/gtitruqwxz.html

C#:   Parallel.For
来源：http://hz.tanke756.top/gthckorpis.html

================================================================================
来源：http://hz.yvedp.cn/gtczsjlhwf.html

P. 常用工具函数
来源：http://hz.chenjidiqi.icu/gtesmhfrkz.html

================================================================================
来源：http://hz.hnqzz.top/gtsisdxsax.html

[P01] 生成 UUID
来源：http://hz.jinyuanbaomall.cn/gtocmrssno.html

Py:   str(uuid.uuid4())
来源：http://hz.cdnleiting.top/gtpnemknar.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.yvedp.cn/gtutislhji.html

JS:   crypto.randomUUID()
来源：http://hz.zhiwuduotai.top/gtkyzhhalg.html

TS:   crypto.randomUUID()
来源：http://hz.pengpengdd.cyou/gtxkyxcphm.html

Java: UUID.randomUUID().toString()
来源：http://hz.c1oappe.top/gtokwgzyke.html

Go:   // 用 github.com/google/uuid
来源：http://hz.hywenlv.cn/gtptnnhvcs.html

Ruby: SecureRandom.uuid
来源：http://hz.mhx1999.top/gtkqyxrjdu.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.hongshengwenyu.top/gtjtwwtear.html

[P02] MD5 / SHA256 摘要
来源：http://hz.pengpengdd.cyou/gtmibtrqjl.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.hfpthk.cn/gtrugtssnb.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.yueranfly.top/gtbsgfdftb.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.zhijiandao.cn/gttcsitgpb.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.dianchejie.cn/gtuzaufpuh.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.ybcxt.top/gtwwlmkqtg.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.cdnleiting.top/gtpcpznyfk.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.ywan-chungtsiang.top/gtescnklrn.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.havefunace.top/gtxalxjfoa.html

[P03] 生成短随机字符串
来源：http://hz.yuxming.cn/gtbebdviqp.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.yj20258.top/gtdlcgypzb.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.shanyushiyangkeji.top/gtpclehhyg.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.gaohongyu789.top/gtuenmgjzj.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.cheryme.top/gtbxoqnhnm.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.ywan-chungtsiang.top/gtwysxbpbw.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.xuetiantiany.cn/gtxpibvuba.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.xylfe.cn/gtxfrvpqrw.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.zycfv.cn/gtqzvfdroh.html

[P04] 求长度
来源：http://hz.zhengqikj.top/gtlsinygsx.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.iojbl.cn/gteckkrozi.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.kuanghao11.cn/gttgsuzsrj.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.ydzc1.top/gtztnltdty.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.yj202588.top/gtdiisftwk.html

Java: list.size();  map.size();  s.length()
来源：http://hz.guannengcc.top/gtfnhxuxiw.html

Go:   len(arr);  len(m)
来源：http://hz.sxryk.cn/gtmqtlkmxe.html

Ruby: x.length;  x.size
来源：http://hz.cucudq.cn/gtxddiatbo.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.yvedp.cn/gtwdfmlrmf.html

[P05] 判断两个对象内容是否相等
来源：http://hz.aizwys.cn/gtqbhkdfus.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.andypj.xyz/gtxjaglnfx.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.ydzc1.top/gtidpndilt.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.chenjidiqi.icu/gteziyqgrw.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.daxiang520.top/gtlhprywgj.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.vqdsnc.cn/gtfxafxilc.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.yueranfly.top/gtcfijgtll.html

Ruby: a == b
来源：http://hz.cqqwz.cn/gtilraucii.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.gotoacloud.top/gtkoifchqs.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.guowangkeji.top/gtamosllmb.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.ywan-chungtsiang.top/gtlugtpzfk.html

PHP:  if (empty($x)) {}
来源：http://hz.xingfuxueyuan.xyz/gtammmagnh.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.52xcode.cn/gtdzzamufv.html

TS:   if (x == null) {}
来源：http://hz.sufxvd.cn/gtqiwkobjp.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.redwolf501.top/gtfpraxjtm.html

Go:   if x == nil {}
来源：http://hz.xylfe.cn/gtxgskxaat.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.zhijiandao.cn/gtcgphszpj.html

C#:   if (x is null) {}
来源：http://hz.gaohongyu789.top/gtfezvedag.html

[P07] 防抖与节流
来源：http://hz.52xcode.cn/gthkyvlglv.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.yanxiufei.cn/gtblgpstgu.html

PHP:  // 手写时间戳比较
来源：http://hz.jqgfzy.top/gtuisesakp.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.zhijiandao.cn/gtcqhmbukj.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.zycfv.cn/gtbqcpbpiq.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.hywenlv.cn/gtkxdxjxzm.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.pengpengdd.cyou/gtntkvoqbd.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.cdnleiting.top/gtjldtwkmr.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.zycfv.cn/gtryveagjv.html

[P08] 处理浮点精度问题
来源：http://hz.yvedp.cn/gtlrnvhasz.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.gogol.net.cn/gtvndthsuu.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.kuanghao11.cn/gtxrotjouf.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.jqgfzy.top/gtpfgfcjho.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.ybcxt.top/gtpybmdqwu.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.xuetiantiany.cn/gtstqipjqk.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.zhixingplan.top/gtxfiuhjad.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.jyoumei.cn/gtvlrmuqds.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.sweek.top/gtkcjosmja.html

================================================================================
来源：http://hz.havefunace.top/gtgmxmcvdm.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.dashuyun.cn/gtcizltkhz.html

================================================================================
来源：http://hz.hywenlv.cn/gtgawslsps.html

[Q01] 创建表
来源：http://hz.smart0.xyz/gtvbxkkfjx.html

CREATE TABLE users (
来源：http://hz.zhaomingkeji.xyz/gtpwwrwrrl.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.guowangkeji.top/gtnbuhovjg.html

name VARCHAR(50) NOT NULL,
来源：http://hz.aibaodan.cn/gtvclytfcm.html

email VARCHAR(100) UNIQUE,
来源：http://hz.jlsjyb.cn/gtokyqapbe.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.zycfv.cn/gthuhvctdf.html

);
来源：http://hz.birdmap.top/gttomnhfws.html

[Q02] 创建带外键的表
来源：http://hz.xylfe.cn/gtapdsuqcb.html

CREATE TABLE orders (
来源：http://hz.9152youxi.cn/gtfedghjtp.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.wangshuangyany.cn/gtqbrvkyul.html

user_id INT NOT NULL,
来源：http://hz.ppjwa.cn/gtdukjbpib.html

amount DECIMAL(10, 2),
来源：http://hz.birdmap.top/gtkjwwgtvd.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.yongpay.top/gtrtqporsl.html

);
来源：http://hz.zhaomingkeji.xyz/gtkgaxfaxr.html

[Q03] 增加列
来源：http://hz.xuanzx.com/gtswvulopm.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.ydzc1.top/gtlzfbxkfc.html

[Q04] 修改列类型
来源：http://hz.gotoacloud.top/gthmfhpjyh.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.9152youxi.cn/gtwwdkbdhc.html

[Q05] 重命名列
来源：http://hz.jyoumei.cn/gtsoriedtw.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.svipenyu.cn/gtuhtdxwwh.html

[Q06] 删除列
来源：http://hz.jlsjyb.cn/gtvsrvfaoq.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.52xcode.cn/gtvidabxib.html

[Q07] 删除表
来源：http://hz.gaohongyu789.top/gtbmvcxuny.html

DROP TABLE IF EXISTS orders;
来源：http://hz.gzhubu.top/gtixxyqamd.html

[Q08] 创建普通索引
来源：http://hz.yvedp.cn/gtzmualyje.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.vqdsnc.cn/gtkrvgselp.html

[Q09] 创建唯一索引
来源：http://hz.nanxuanxn.top/gtofgfhskk.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.chenjidiqi.icu/gtxgorlinl.html

[Q10] 插入单行
来源：http://hz.quarkkingdee.top/gtvhqmegqu.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.tian-w.cn/gtiufamppf.html

[Q11] 一次插入多行
来源：http://hz.jiagoushi.top/gtcumboajf.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.feifeiyinyue.top/gtcsdgnzsr.html

[Q12] 插入后取自增 ID
来源：http://hz.52xcode.cn/gtcjgbbfer.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.zdqjudy.top/gtoleponau.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.cheryme.top/gtptpvgybx.html

[Q13] 忽略重复插入
来源：http://hz.xuanzx.com/gtexyfrtab.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.gaohongyu789.top/gtqjewrevw.html

[Q14] 存在则更新（upsert）
来源：http://hz.yanxiufei.cn/gtzfqdxwoj.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.mhx1999.top/gtvtzzhfau.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.316326.xyz/gtiynduznq.html

[Q15] 查询全部
来源：http://hz.pengpengdd.cyou/gtdxgrvepr.html

SELECT * FROM users;
来源：http://hz.jiagoushi.top/gtgysmbzil.html

[Q16] 查询指定列
来源：http://hz.mhx1999.top/gthxkvhgug.html

SELECT id, name FROM users;
来源：http://hz.hammf.cn/gtgjcuiqtz.html

[Q17] 条件查询
来源：http://hz.vqdsnc.cn/gtjixcghnv.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.jlsjyb.cn/gthtjezskj.html

[Q18] 模糊匹配
来源：http://hz.yonumen.top/gtzpujdepq.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.jinghuilouyu.cn/gtqxzqcxew.html

[Q19] 范围查询
来源：http://hz.cashguo.top/gtbwoumfry.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.pengpengdd.cyou/gtpijfrizs.html

[Q20] IN 列表
来源：http://hz.dianchejie.cn/gtlwdgqgkg.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.shuidangran.top/gtygceaiex.html

[Q21] 空值判断
来源：http://hz.jinghuilouyu.cn/gtckclzvvn.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.yanxiufei.cn/gtuzdmsfyr.html

[Q22] 排序
来源：http://hz.tian-w.cn/gttedxkdjn.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.yueranfly.top/gtqazgdkjz.html

[Q23] 分页
来源：http://hz.cqqwz.cn/gtezycswre.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.nwbrower.top/gtmkdhkdin.html

[Q24] 去重
来源：http://hz.bjfxy.top/gtancbemqm.html

SELECT DISTINCT city FROM users;
来源：http://hz.yongpay.top/gtxasqqibi.html

[Q25] 只取前 N 条
来源：http://hz.yueranfly.top/gtytmjvzoz.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.sysykeji.top/gtwdbgodib.html

[Q26] 计数
来源：http://hz.kuanghao11.cn/gtztheqlhr.html

SELECT COUNT(*) FROM users;
来源：http://hz.sweek.top/gtqyrcaxvj.html

[Q27] 条件计数
来源：http://hz.chenzaomai.com/gtllaocdwc.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.zhongyouzk.top/gthfgwxfax.html

[Q28] 求和与平均
来源：http://hz.gaohongyu789.top/gtutwqzmru.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.dianchejie.cn/gtyncsswrk.html

[Q29] 最大最小值
来源：http://hz.shangyingyoupin.top/gtsarqujtm.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.mhx1999.top/gtcatpfezs.html

[Q30] 分组统计
来源：http://hz.ivvv.top/gtyoedfdft.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.wangshuangyany.cn/gtrcbzyhxo.html

[Q31] 分组后过滤
来源：http://hz.yj20258.top/gtveqrohsh.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.jianghu66.top/gtnjnghzoh.html

[Q32] 分组拼接字符串
来源：http://hz.cqqwz.cn/gtkldpfvus.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.jlsjyb.cn/gtlnbgcflk.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.birdmap.top/gtpwbhlgji.html

[Q33] 多列分组
来源：http://hz.zhongyouzk.top/gtlrfznesw.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.wangdashe.top/gtelhblxbk.html

[Q34] 每组取第一条
来源：http://hz.jinyuanbaomall.cn/gtuamdvuro.html

SELECT * FROM (
来源：http://hz.haohaochexian.top/gtnctgaesp.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.yvedp.cn/gtpnxgnkha.html

) t WHERE rn = 1;
来源：http://hz.daxiang520.top/gthmpfbcjq.html

[Q35] 内连接
来源：http://hz.bjfxy.top/gtjwwojmlv.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.nanxinkj.top/gtunhpwlrq.html

[Q36] 左连接
来源：http://hz.birdmap.top/gtrgjtifxo.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.meibo888.top/gtwfmqrfos.html

[Q37] 右连接
来源：http://hz.9152youxi.cn/gtsoysuuvz.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.zhiwuduotai.top/gtydzzwgnv.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.wangshuangyany.cn/gtmwjfwggl.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.jianghu66.top/gtkxjazrvx.html

[Q39] 自连接（查上下级）
来源：http://hz.jinqigfzy.top/gthkkeduvx.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.smart0.xyz/gtjxwvpxeb.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.aizwys.cn/gtsjahusht.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.shanyushiyangtech.top/gtuwfqdvlj.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.jiagoushi.top/gtffkduyxe.html

[Q41] 多表连接
来源：http://hz.gogol.net.cn/gtwzhwghfn.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.zhengqikj.top/gtfkfwherr.html

JOIN users u ON u.id = o.user_id
来源：http://hz.daria6918.cn/gtyacyqkap.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.aizwys.cn/gtbcizahuo.html

[Q42] 连接条件附加过滤
来源：http://hz.shanyushiyangtech.top/gtjduthkmc.html

SELECT u.name, o.amount FROM users u
来源：http://hz.shanyushiyangkeji.top/gtptyavxqk.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.shangyingyoupin.top/gtqkdllwxm.html

[Q43] 标量子查询
来源：http://hz.yonumen.top/gttjmgpytu.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.kuanghao11.cn/gtptdglqdd.html

[Q44] IN 子查询
来源：http://hz.hfpthk.cn/gtdkbgrfjc.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.yongpay.top/gthvzfdqny.html

[Q45] EXISTS 判断存在
来源：http://hz.xuanzx.com/gtnscuwaof.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.nanxinkj.top/gthgwubczo.html


<!-- 参考信息 -->