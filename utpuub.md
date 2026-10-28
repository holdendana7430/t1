代发 wailian999

Ruby: s == s.reverse
来源：http://hz.jqgfzy.top/gtjljnfloo.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.pycfn.com/gtfrlxzxff.html

[N07] 两数之和（返回下标）
来源：http://hz.ppjwa.cn/gtoptutzdh.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.jqgufenzy.top/gtmrusysic.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.cucudq.cn/gtvnammitr.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.52xcode.cn/gtybhllles.html

TS:   // 手写 Map<string, number>
来源：http://hz.sxryk.cn/gtangcdmaj.html

Java: // 手写 HashMap
来源：http://hz.ywan-chungtsiang.top/gtencnoeqq.html

Go:   // 手写 map[int]int
来源：http://hz.ehwqpu.com/gtcxlxuald.html

Ruby: // 手写 Hash
来源：http://hz.yj20258.top/gtyyaadnyk.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.yj20258.top/gtgcygyknb.html

[N08] 生成全排列
来源：http://hz.guannengcc.top/gtwlwuygav.html

Py:   itertools.permutations(arr)
来源：http://hz.ppjwa.cn/gttrmdqkjx.html

PHP:  // 手写递归交换
来源：http://hz.hongshengwenyu.top/gtjfcaeavx.html

JS:   // 手写回溯递归
来源：http://hz.guannengcc.top/gtmtlojgfc.html

TS:   // 手写回溯递归
来源：http://hz.xuetiantiany.cn/gtdmxnhlma.html

Java: // 手写回溯递归
来源：http://hz.svipenyu.cn/gtoewipewx.html

Go:   // 手写回溯递归
来源：http://hz.jinyuanbaomall.cn/gtkcakllut.html

Ruby: arr.permutation.to_a
来源：http://hz.wangdashe.top/gthvpxjvsn.html

C#:   // 手写回溯递归
来源：http://hz.hnqzz.top/gtvwmrdqxx.html

[N09] 栈与队列
来源：http://hz.zhengqikj.top/gtamsftxve.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.kuanghao11.cn/gtrdkmpxcf.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.vqdsnc.cn/gtlkwxmfni.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.pengpengdd.cyou/gtgytailex.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.ydzc1.top/gtwujdfgan.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.xuanzx.com/gtjyrwlgcz.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.jinyuanbaomall.cn/gtghkjdwkf.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.yj202588.top/gtjymgwjol.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.9152youxi.cn/gtaongcoon.html

[N10] 链表节点定义
来源：http://hz.yuanzhike.top/gteqcziblp.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.ppjwa.cn/gtehcbkhyg.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.gotoacloud.top/gtlmddsgmq.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.shanyushiyangkeji.top/gtqyazdcel.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.dianchejie.cn/gtaboptqll.html

Java: class Node { int v; Node next; }
来源：http://hz.kuanghao11.cn/gtsqsobqfb.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.bjfxy.top/gtlnjbsmfx.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.fzhhl.top/gtemxgaowi.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.nanxuanxn.top/gtawkkuzxi.html

[N11] 二叉树中序遍历
来源：http://hz.hfpthk.cn/gtkumfwsta.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.guannengcc.top/gtrilfuehm.html

PHP:  // 手写递归函数
来源：http://hz.jinqigufen.top/gtqdqzmioh.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.quarkkingdee.top/gtrtuktzbt.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.ydzc1.top/gtsvlgrhly.html

Java: // 手写递归
来源：http://hz.ydjk.org.cn/gtyqvgoynj.html

Go:   // 手写递归
来源：http://hz.yuxming.cn/gtwxqeffkv.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.c1oappe.top/gtsjvodrbt.html

C#:   // 手写递归
来源：http://hz.wangshuangyany.cn/gtdrabwcgy.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.daria6918.cn/gthbanxkro.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.cucudq.cn/gtjkkxdusr.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.ivvv.top/gtvtheivor.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.hammf.cn/gthxhcsdaq.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.sweek.top/gticzkeczt.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.svipenyu.cn/gtiajabsmm.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.nanxuanxn.top/gtogqcemtp.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.iojbl.cn/gtrpvsssre.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.jinqigfzy.top/gtnyfjltfg.html

================================================================================
来源：http://hz.9152youxi.cn/gtzoeooqpz.html

O. 并发与异步
来源：http://hz.mhx1999.top/gtirehsmyp.html

================================================================================
来源：http://hz.zhoulong.xyz/gttugiyrwt.html

[O01] 启动一个线程
来源：http://hz.yj202588.top/gtzzpuroun.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.snrcjt.cn/gtqaagplrh.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.jyoumei.cn/gtdnzwhxay.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.feifeiyinyue.top/gtfazwvrxa.html

TS:   // 同 JS
来源：http://hz.hongshengwenyu.top/gtvmgsluzt.html

Java: new Thread(() -> f()).start()
来源：http://hz.kuanghao11.cn/gtpfxhzyvf.html

Go:   go f()
来源：http://hz.cdnleiting.top/gtybsfxiym.html

Ruby: Thread.new { f }
来源：http://hz.wangshuangyany.cn/gtpxhixkfz.html

C#:   Task.Run(() => F());
来源：http://hz.gotoacloud.top/gtlvgcyait.html

[O02] 使用线程池
来源：http://hz.yuanzhike.top/gtevyrrkzo.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.cheryme.top/gtdmsgjezl.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.zhijiandao.cn/gtvbolpypm.html

JS:   // worker_threads 线程池
来源：http://hz.dashuyun.cn/gtswhfgsyd.html

TS:   // worker_threads 线程池
来源：http://hz.hnxiangtu.top/gtxhuhtukq.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.redwolf501.top/gtcfwazgut.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.dianchejie.cn/gteanoflhv.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.chenjidiqi.icu/gtkbrelaaa.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.cdnleiting.top/gtkxiginfh.html

[O03] 加锁保护共享数据
来源：http://hz.hywenlv.cn/gtxrjugwjs.html

Py:   with lock: shared += 1
来源：http://hz.zdqjudy.top/gtfwmmuugj.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.jinqigufen.top/gtegadzngs.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.jinqigufen.top/gtzbgracfq.html

TS:   // 同 JS
来源：http://hz.xylfe.cn/gtyrtpjmfb.html

Java: synchronized (this) { shared++; }
来源：http://hz.sxryk.cn/gtdlylzswn.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.aibaodan.cn/gtxexbxfhw.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.shangyingyoupin.top/gttqmdtqle.html

C#:   lock (gate) { shared++; }
来源：http://hz.bjfxy.top/gttuwyukek.html

[O04] 定义异步函数并等待
来源：http://hz.aizwys.cn/gtfogoluia.html

Py:   async def f():⏎    await g()
来源：http://hz.dashuyun.cn/gtwuqbmhbm.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.pycfn.com/gtolvuouya.html

JS:   async function f() { await g(); }
来源：http://hz.cheryme.top/gtleobxtrk.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.shangyingyoupin.top/gtbpdugzsn.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.zhixingplan.top/gtqdyldnoj.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.smart0.xyz/gtemtsdxpf.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.yj20258888.top/gthpkolzka.html

C#:   async Task F() { await G(); }
来源：http://hz.cashguo.top/gtopasyknz.html

[O05] 并发执行并等待全部完成
来源：http://hz.hnqzz.top/gtykvgdqtw.html

Py:   asyncio.gather(*tasks)
来源：http://hz.pengpengdd.cyou/gtlgitxcpc.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.cqqwz.cn/gtyrmvrymv.html

JS:   await Promise.all(tasks)
来源：http://hz.kuanghao11.cn/gtisyzqfjo.html

TS:   await Promise.all(tasks)
来源：http://hz.cashguo.top/gtwxaonidi.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.shzxlz.cn/gtemhijtie.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.gaohongyu789.top/gttwrxwbec.html

Ruby: threads.map(&:join)
来源：http://hz.mhx1999.top/gtviuzjedb.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.ydjk.org.cn/gtvoemvorv.html

[O06] 使用进程池
来源：http://hz.guannengcc.top/gtphxqrelz.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.316326.xyz/gtonxqflky.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.0kj1m.cn/gtpyukcwuh.html

JS:   // child_process / cluster 模块
来源：http://hz.shanyushiyangkeji.top/gtdwvedsoh.html

TS:   // child_process / cluster 模块
来源：http://hz.zhijiandao.cn/gtdrsjsnct.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.yuanzhike.top/gtwhrnfjly.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.sweek.top/gtbfvxkjqg.html

Ruby: // fork 块
来源：http://hz.hnqzz.top/gtwzzpenyv.html

C#:   Parallel.For
来源：http://hz.kuanghao11.cn/gtvecgndcb.html

================================================================================
来源：http://hz.ppjwa.cn/gttlmqplmy.html

P. 常用工具函数
来源：http://hz.iojbl.cn/gtrkpmljty.html

================================================================================
来源：http://hz.birdmap.top/gtdexyprxo.html

[P01] 生成 UUID
来源：http://hz.shangyingyoupin.top/gtipzmrbpr.html

Py:   str(uuid.uuid4())
来源：http://hz.yj20258.top/gtxslqsezi.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.zhengqikj.top/gtdcfzjvyi.html

JS:   crypto.randomUUID()
来源：http://hz.chenlongwang.top/gtracrjabj.html

TS:   crypto.randomUUID()
来源：http://hz.ivvv.top/gtwjjpzyke.html

Java: UUID.randomUUID().toString()
来源：http://hz.gzhubu.top/gtvmtvhvym.html

Go:   // 用 github.com/google/uuid
来源：http://hz.andypj.xyz/gttfdalgye.html

Ruby: SecureRandom.uuid
来源：http://hz.xinyue.icu/gtegnottny.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.fengsongda.top/gtiaontlnf.html

[P02] MD5 / SHA256 摘要
来源：http://hz.jinqigufen.top/gtiyzdrsfz.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.tanke756.top/gtnuttymtp.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.cdnleiting.top/gtgmsmxnzh.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.chenzaomai.com/gtpxiowlud.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.ybcxt.top/gtmxkmnyvl.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.yueranfly.top/gtubpuzjmt.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.havefunace.top/gtzrhoyyjz.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.nanxinkj.top/gtetoueaxa.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.hammf.cn/gtkramexto.html

[P03] 生成短随机字符串
来源：http://hz.mhx1999.top/gtybqscgai.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.aibaodan.cn/gtfmldyrnv.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.dianchejie.cn/gtjcsbjait.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.ywan-chungtsiang.top/gtpdgvnolm.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.andypj.xyz/gtmxdmzayq.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.jlsjyb.cn/gtbuoclioz.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.guannengcc.top/gtvuydgaop.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.cashguo.top/gtdfdowxmp.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.yj202588.top/gtcszfcpuo.html

[P04] 求长度
来源：http://hz.hysaishi.cn/gtrwhrcgtt.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.yuanzhike.top/gtljbjlepq.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.ydzc1.top/gtbloqjijw.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.yj20258.top/gtdjxtjktd.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.yuxming.cn/gtwznczocy.html

Java: list.size();  map.size();  s.length()
来源：http://hz.yuxming.cn/gtkqthdpgb.html

Go:   len(arr);  len(m)
来源：http://hz.yongpay.top/gtnkcrwggt.html

Ruby: x.length;  x.size
来源：http://hz.xingfuxueyuan.xyz/gtgdodvjit.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.sysykeji.top/gttdmclzad.html

[P05] 判断两个对象内容是否相等
来源：http://hz.shanyushiyangkeji.top/gtaxtanklb.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.yuxming.cn/gthdnvslzm.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.sysykeji.top/gtcwlhsdfq.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.xziqi.cn/gtksndlsxn.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.shanyushiyangtech.top/gtztlhqdch.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.guowangkeji.top/gtotrjfnub.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.dianchejie.cn/gtjhxanmko.html

Ruby: a == b
来源：http://hz.redwolf501.top/gtkfuacbtj.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.daria6918.cn/gtxgwpsbtv.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.snrcjt.cn/gtdvulmqvw.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.jqgfzy.top/gtqdbgtydx.html

PHP:  if (empty($x)) {}
来源：http://hz.shzxlz.cn/gtlzuvasgv.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.snrcjt.cn/gtfdjztfsv.html

TS:   if (x == null) {}
来源：http://hz.chenlongwang.top/gtrwbmevck.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.ybcxt.top/gtepxprjrp.html

Go:   if x == nil {}
来源：http://hz.52xcode.cn/gtnadrrjjv.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.yuanzhike.top/gtymoklmfo.html

C#:   if (x is null) {}
来源：http://hz.yuanzhike.top/gttjlfztpy.html

[P07] 防抖与节流
来源：http://hz.daxiang520.top/gtfocnfavc.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.birdmap.top/gtaixktbxy.html

PHP:  // 手写时间戳比较
来源：http://hz.316326.xyz/gtddenjkul.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.zhixingplan.top/gtwsvywwbu.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.jqgfzy.top/gtdkuvemnv.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.hysaishi.cn/gtdwlksldq.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.hnqzz.top/gtacsidmon.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.jlsjyb.cn/gtxfihbxcv.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.aizwys.cn/gtjfhkbyoa.html

[P08] 处理浮点精度问题
来源：http://hz.wangdashe.top/gtdpkcaqgt.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.chenzaomai.com/gtaptamotj.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.aizwys.cn/gticbwsfpa.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.guannengcc.top/gtglsnaujh.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.yj20258888.top/gtjebkdohb.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.zhixingplan.top/gtunxsmjec.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.nanxuanxn.top/gtwtadqwla.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.pycfn.com/gtaqoivjrr.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.zhoulong.xyz/gtutfyscim.html

================================================================================
来源：http://hz.svipenyu.cn/gtuebsvdpj.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.cdnleiting.top/gtdsaxghdy.html

================================================================================
来源：http://hz.hfpthk.cn/gtwwxadppi.html

[Q01] 创建表
来源：http://hz.pycfn.com/gtjmzenqht.html

CREATE TABLE users (
来源：http://hz.shanyushiyangkeji.top/gtlexbwdgm.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.yj20258.top/gtjukipwfg.html

name VARCHAR(50) NOT NULL,
来源：http://hz.cheryme.top/gtxaagoufs.html

email VARCHAR(100) UNIQUE,
来源：http://hz.316326.xyz/gtxmpsbywt.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.hnqzz.top/gtohtdasez.html

);
来源：http://hz.ehwqpu.com/gtlekvvele.html

[Q02] 创建带外键的表
来源：http://hz.yanxiufei.cn/gtutxdrjvb.html

CREATE TABLE orders (
来源：http://hz.birdmap.top/gtdphzplot.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.xuetiantiany.cn/gtsdbzcyvj.html

user_id INT NOT NULL,
来源：http://hz.daria6918.cn/gtpaadqxyi.html

amount DECIMAL(10, 2),
来源：http://hz.xuanzx.com/gtulfrbbwj.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.tanke756.top/gtvwjfqzut.html

);
来源：http://hz.haohaochexian.top/gtiqvjwyyk.html

[Q03] 增加列
来源：http://hz.ivvv.top/gtuofazakx.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.jianghu66.top/gtxkuxccju.html

[Q04] 修改列类型
来源：http://hz.ydjk.org.cn/gthiqbunks.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.nwbrower.top/gtozskmjjz.html

[Q05] 重命名列
来源：http://hz.jiagoushi.top/gtvikfavhl.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.gogol.net.cn/gtedgpsbat.html

[Q06] 删除列
来源：http://hz.jinqigfzy.top/gtfijsrjdx.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.jiagoushi.top/gtdzffkuec.html

[Q07] 删除表
来源：http://hz.sxryk.cn/gtqhbgogww.html

DROP TABLE IF EXISTS orders;
来源：http://hz.sysykeji.top/gtbpizgtmj.html

[Q08] 创建普通索引
来源：http://hz.fengsongda.top/gtfjhuadau.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.jinqigufen.top/gtvrmabcfi.html

[Q09] 创建唯一索引
来源：http://hz.redwolf501.top/gtilelzitz.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.wangdashe.top/gtmkmyrnar.html

[Q10] 插入单行
来源：http://hz.daxiang520.top/gtmiumbzhm.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.hywenlv.cn/gtohkkawpm.html

[Q11] 一次插入多行
来源：http://hz.jlsjyb.cn/gtqbsuaoah.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.daria6918.cn/gtnveccklw.html

[Q12] 插入后取自增 ID
来源：http://hz.ppjwa.cn/gtjeqndoap.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.ivvv.top/gtsgnjakqu.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.yueranfly.top/gtxavggfkk.html

[Q13] 忽略重复插入
来源：http://hz.yj20258.top/gtefhyyuea.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.hfpthk.cn/gtvworlpzf.html

[Q14] 存在则更新（upsert）
来源：http://hz.zdqjudy.top/gtjybsipdf.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.hywenlv.cn/gtemplrgwp.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.zhongyouzk.top/gttdgtqaoo.html

[Q15] 查询全部
来源：http://hz.jlsjyb.cn/gtzwolzmuw.html

SELECT * FROM users;
来源：http://hz.yvedp.cn/gtkuhlzglr.html

[Q16] 查询指定列
来源：http://hz.jyoumei.cn/gtjffevqqi.html

SELECT id, name FROM users;
来源：http://hz.gzhubu.top/gtzzypdjcm.html

[Q17] 条件查询
来源：http://hz.daxiang520.top/gtuqaevnrf.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.ywan-chungtsiang.top/gtpsponafy.html

[Q18] 模糊匹配
来源：http://hz.xylfe.cn/gtxuytottn.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.0kj1m.cn/gtcjvklaxc.html

[Q19] 范围查询
来源：http://hz.chenjidiqi.icu/gtnhsncxot.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.nwbrower.top/gtvynkouac.html

[Q20] IN 列表
来源：http://hz.wangdashe.top/gtimqlhjgk.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.iojbl.cn/gtujotcbed.html

[Q21] 空值判断
来源：http://hz.cashguo.top/gtrwgnqsgz.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.zhoulong.xyz/gtiwegvqly.html

[Q22] 排序
来源：http://hz.ydjk.org.cn/gthxluxrqo.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.c1oappe.top/gtqzuhfmsd.html

[Q23] 分页
来源：http://hz.zhixingplan.top/gtztcdegxr.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.yj20258888.top/gttsvbonxm.html

[Q24] 去重
来源：http://hz.smart0.xyz/gtkjcwwbfn.html

SELECT DISTINCT city FROM users;
来源：http://hz.hfpthk.cn/gtjyjiaixv.html

[Q25] 只取前 N 条
来源：http://hz.guannengcc.top/gtjuvmydou.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.gzhubu.top/gtalyqpwuc.html

[Q26] 计数
来源：http://hz.redwolf501.top/gtzmnwlnnl.html

SELECT COUNT(*) FROM users;
来源：http://hz.hfpthk.cn/gthtmchamf.html

[Q27] 条件计数
来源：http://hz.jianghu66.top/gtdbeubacp.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.yonumen.top/gtvrquihjd.html

[Q28] 求和与平均
来源：http://hz.birdmap.top/gtjaifqpjl.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.sysykeji.top/gtsfikxmme.html

[Q29] 最大最小值
来源：http://hz.yj20258.top/gtfmtfbvps.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.shuidangran.top/gtkipktmdy.html

[Q30] 分组统计
来源：http://hz.zhixingplan.top/gteyydjdre.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.sxryk.cn/gtqwdrlxff.html

[Q31] 分组后过滤
来源：http://hz.shzxlz.cn/gtsmdpbqwj.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.hywenlv.cn/gtmhtjhwwl.html

[Q32] 分组拼接字符串
来源：http://hz.fengsongda.top/gtxnakdaod.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.hywenlv.cn/gtcsawwiqn.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.daxiang520.top/gtyhiibmum.html

[Q33] 多列分组
来源：http://hz.havefunace.top/gtzrunpdyn.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.yonumen.top/gthvblfqeq.html

[Q34] 每组取第一条
来源：http://hz.zhixingplan.top/gtgfkypfzr.html

SELECT * FROM (
来源：http://hz.yuanzhike.top/gtktunudio.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.zhiwuduotai.top/gtahffcnyr.html

) t WHERE rn = 1;
来源：http://hz.xuanzx.com/gttjvtqxke.html

[Q35] 内连接
来源：http://hz.hnqzz.top/gtrarhsiff.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.fengsongda.top/gtnudfleqv.html

[Q36] 左连接
来源：http://hz.cashguo.top/gtdneucrnk.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.ybcxt.top/gtxjzetvuy.html

[Q37] 右连接
来源：http://hz.zhengqikj.top/gtekesmcwt.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.tianlin.xyz/gtrkxsmypv.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.gotoacloud.top/gtnmlufecu.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.meibo888.top/gtqizdxhoa.html

[Q39] 自连接（查上下级）
来源：http://hz.cashguo.top/gtacjlhzoi.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.sweek.top/gtunimlonb.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.yueranfly.top/gttcfdontj.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.chenzaomai.com/gtnuyuesxz.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.pycfn.com/gtmkhpfmup.html

[Q41] 多表连接
来源：http://hz.guannengcc.top/gtdrysdvzt.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.xinyue.icu/gtthklwaoz.html

JOIN users u ON u.id = o.user_id
来源：http://hz.snrcjt.cn/gtdpqpudeu.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.xingfuxueyuan.xyz/gtbvjrizxy.html

[Q42] 连接条件附加过滤
来源：http://hz.hysaishi.cn/gtoxydumyr.html

SELECT u.name, o.amount FROM users u
来源：http://hz.wangdashe.top/gtlwsbzefl.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.wangshuangyany.cn/gtwsbndvuk.html

[Q43] 标量子查询
来源：http://hz.zhengqikj.top/gtytmqfhdz.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.ppjwa.cn/gtwwykmgrz.html

[Q44] IN 子查询
来源：http://hz.yuanzhike.top/gtaelpoygs.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.hammf.cn/gtqtqumoqs.html

[Q45] EXISTS 判断存在
来源：http://hz.hammf.cn/gtcirlaqlm.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.ehwqpu.com/gtacytuliy.html


<!-- 参考信息 -->