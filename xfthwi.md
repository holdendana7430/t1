代发 wailian999

JS:   s === [...s].reverse().join("")
来源：http://hz.jqgfzy.top/gtwyjgfpmr.html

TS:   s === [...s].reverse().join("")
来源：http://hz.cucudq.cn/gtjjezkmul.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.shangyingyoupin.top/gthflvwtcv.html

Go:   // 双指针从两端比较
来源：http://hz.gogol.net.cn/gtnupbrolb.html

Ruby: s == s.reverse
来源：http://hz.xziqi.cn/gtiihthmiy.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.yj202588.top/gtbgwlhfyw.html

[N07] 两数之和（返回下标）
来源：http://hz.haohaochexian.top/gthrjlkqup.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.dianchejie.cn/gtzcptavli.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.jqgufenzy.top/gtpvlplcxb.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.zhijiandao.cn/gtvwcloqdb.html

TS:   // 手写 Map<string, number>
来源：http://hz.gzhubu.top/gtzkbdtflo.html

Java: // 手写 HashMap
来源：http://hz.jinyuanbaomall.cn/gtbsqizgcr.html

Go:   // 手写 map[int]int
来源：http://hz.shangyingyoupin.top/gtbglgwazb.html

Ruby: // 手写 Hash
来源：http://hz.ydjk.org.cn/gtstabgcfr.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.ybcxt.top/gtgfjfjjpm.html

[N08] 生成全排列
来源：http://hz.cucudq.cn/gttliwbsct.html

Py:   itertools.permutations(arr)
来源：http://hz.shanyushiyangkeji.top/gtkyshcfxp.html

PHP:  // 手写递归交换
来源：http://hz.ywan-chungtsiang.top/gtvuogpyva.html

JS:   // 手写回溯递归
来源：http://hz.zhiwuduotai.top/gtntqmdgpq.html

TS:   // 手写回溯递归
来源：http://hz.zhaomingkeji.xyz/gtfxxiypdm.html

Java: // 手写回溯递归
来源：http://hz.yj20258.top/gtvfojzlsg.html

Go:   // 手写回溯递归
来源：http://hz.jianghu66.top/gtdgrlvash.html

Ruby: arr.permutation.to_a
来源：http://hz.jinqigfzy.top/gtpnhobvqq.html

C#:   // 手写回溯递归
来源：http://hz.meibo888.top/gtodsyhuzj.html

[N09] 栈与队列
来源：http://hz.bjfxy.top/gtzsgwvruc.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.zhengqikj.top/gttokjiwpd.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.jinghuilouyu.cn/gtbqvpqerp.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.zhixingplan.top/gtikrcbohz.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.smart0.xyz/gtsfljahwh.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.shangyingyoupin.top/gtbojerebe.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.cqqwz.cn/gtanecckic.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.ehwqpu.com/gthgpjszzr.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.tanke756.top/gtgkvklmvk.html

[N10] 链表节点定义
来源：http://hz.jyoumei.cn/gtnjwwntwf.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.hnxiangtu.top/gtxnfcyxvx.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.wangdashe.top/gtbmpgtulw.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.zhoulong.xyz/gtvmifegyp.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.tian-w.cn/gtcgkdolqt.html

Java: class Node { int v; Node next; }
来源：http://hz.chenzaomai.com/gtzrarpqij.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.sufxvd.cn/gthzxssgsx.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.chenzaomai.com/gtzvyhivbu.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.hywenlv.cn/gtxakefrzp.html

[N11] 二叉树中序遍历
来源：http://hz.dashuyun.cn/gtoxyetqur.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.tianlin.xyz/gtdkcpbzfg.html

PHP:  // 手写递归函数
来源：http://hz.cashguo.top/gtudowbqmu.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.andypj.xyz/gtjnidowka.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.yanxiufei.cn/gtzcoqptpq.html

Java: // 手写递归
来源：http://hz.jlsjyb.cn/gtjugzxeld.html

Go:   // 手写递归
来源：http://hz.feifeiyinyue.top/gtmskrdqtc.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.xingfuxueyuan.xyz/gtdjxzuwsc.html

C#:   // 手写递归
来源：http://hz.tianlin.xyz/gtyrrvnhxy.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.ppjwa.cn/gtmrgflljj.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.fzhhl.top/gtqvfxwmfd.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.nanxuanxn.top/gtapewhxhg.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.xinyue.icu/gtqlwdurxv.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.0kj1m.cn/gtequnpesn.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.shanyushiyangtech.top/gtwcjekewo.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.dianchejie.cn/gtptvjonls.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.yongpay.top/gtmdtwqvnh.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.nwbrower.top/gtdozmmcqf.html

================================================================================
来源：http://hz.jinqigfzy.top/gtehyskrgm.html

O. 并发与异步
来源：http://hz.chenlongwang.top/gtgkixvpph.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtpjwdgrex.html

[O01] 启动一个线程
来源：http://hz.iojbl.cn/gtnqwedflb.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.shanyushiyangkeji.top/gtnibagzkn.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.xziqi.cn/gtagxyxzor.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.svipenyu.cn/gtvbyvwgdh.html

TS:   // 同 JS
来源：http://hz.xingfuxueyuan.xyz/gtiheoslhm.html

Java: new Thread(() -> f()).start()
来源：http://hz.daria6918.cn/gtofkwailf.html

Go:   go f()
来源：http://hz.hammf.cn/gtaekmpdli.html

Ruby: Thread.new { f }
来源：http://hz.9152youxi.cn/gttgjvtdin.html

C#:   Task.Run(() => F());
来源：http://hz.jyoumei.cn/gtgtdmnzww.html

[O02] 使用线程池
来源：http://hz.xziqi.cn/gthiynjqng.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.tanke756.top/gtdodoudfq.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.sweek.top/gtczxyxogu.html

JS:   // worker_threads 线程池
来源：http://hz.ivvv.top/gtccgkwycq.html

TS:   // worker_threads 线程池
来源：http://hz.guannengcc.top/gttyjldzmm.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.chenjidiqi.icu/gtqpvjxrfe.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.gaohongyu789.top/gtsoewoqss.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.guowangkeji.top/gthgnatzgu.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.aizwys.cn/gtyzntrsxn.html

[O03] 加锁保护共享数据
来源：http://hz.xziqi.cn/gtsyajqidi.html

Py:   with lock: shared += 1
来源：http://hz.52xcode.cn/gtwdbefyky.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.zhixingplan.top/gttctafkti.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.zhoulong.xyz/gtfrzujxde.html

TS:   // 同 JS
来源：http://hz.jinyuanbaomall.cn/gtpxyyefkb.html

Java: synchronized (this) { shared++; }
来源：http://hz.316326.xyz/gtalyjmvke.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.pengpengdd.cyou/gtepqgjuij.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.xingfuxueyuan.xyz/gtndtavjue.html

C#:   lock (gate) { shared++; }
来源：http://hz.ppjwa.cn/gttlhcasmw.html

[O04] 定义异步函数并等待
来源：http://hz.wangdashe.top/gtijurxxmb.html

Py:   async def f():⏎    await g()
来源：http://hz.jqgfzy.top/gtctwvtuiw.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.zhixingplan.top/gthdmgvgvq.html

JS:   async function f() { await g(); }
来源：http://hz.sweek.top/gtrwtvfwoa.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.xinyue.icu/gtthnywodo.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.pengpengdd.cyou/gtrbdaoysc.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.dashuyun.cn/gtaymrhgpy.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.meibo888.top/gtqepjnekh.html

C#:   async Task F() { await G(); }
来源：http://hz.xinyue.icu/gtdqvixund.html

[O05] 并发执行并等待全部完成
来源：http://hz.guowangkeji.top/gtzmylcfse.html

Py:   asyncio.gather(*tasks)
来源：http://hz.wangshuangyany.cn/gtktcwdyyn.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.yuxming.cn/gtsmpqlpur.html

JS:   await Promise.all(tasks)
来源：http://hz.redwolf501.top/gtkbrrkcju.html

TS:   await Promise.all(tasks)
来源：http://hz.yj202588.top/gtzuffgwvm.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.zdqjudy.top/gtzmegcmak.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.zycfv.cn/gtktwibrdy.html

Ruby: threads.map(&:join)
来源：http://hz.chenlongwang.top/gtxygttvbr.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.jlsjyb.cn/gtikdfqaaz.html

[O06] 使用进程池
来源：http://hz.316326.xyz/gtzubsjfoj.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.sufxvd.cn/gtcvrlnsgq.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.cheryme.top/gtlfinoqlo.html

JS:   // child_process / cluster 模块
来源：http://hz.hnqzz.top/gtudnxqhxe.html

TS:   // child_process / cluster 模块
来源：http://hz.daria6918.cn/gtlexduepg.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.jqgfzy.top/gtxccgkuxk.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.yuanzhike.top/gtozleqfcx.html

Ruby: // fork 块
来源：http://hz.ywan-chungtsiang.top/gtxxcjmzty.html

C#:   Parallel.For
来源：http://hz.redwolf501.top/gtkhsklvar.html

================================================================================
来源：http://hz.vqdsnc.cn/gtzuzohwkv.html

P. 常用工具函数
来源：http://hz.quarkkingdee.top/gtfujmapvs.html

================================================================================
来源：http://hz.yj20258.top/gtkyadhiez.html

[P01] 生成 UUID
来源：http://hz.zycfv.cn/gtpfvqazgg.html

Py:   str(uuid.uuid4())
来源：http://hz.xuanzx.com/gtvzmvmwim.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.meibo888.top/gtuykpxqnh.html

JS:   crypto.randomUUID()
来源：http://hz.chenjidiqi.icu/gtuurvuemj.html

TS:   crypto.randomUUID()
来源：http://hz.cheryme.top/gtnasutdvb.html

Java: UUID.randomUUID().toString()
来源：http://hz.hnqzz.top/gtlwnavyya.html

Go:   // 用 github.com/google/uuid
来源：http://hz.316326.xyz/gtqwqlayws.html

Ruby: SecureRandom.uuid
来源：http://hz.gzhubu.top/gtcahzohsb.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.shangyingyoupin.top/gtfmqvqtza.html

[P02] MD5 / SHA256 摘要
来源：http://hz.guannengcc.top/gtdzobcebc.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.cqqwz.cn/gtiyghbirr.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.ppjwa.cn/gtftancnbp.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.yuanzhike.top/gtzjikxyng.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.pycfn.com/gtvbtbktkj.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.9152youxi.cn/gttavnpfem.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.jqgfzy.top/gtlmewwpmb.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.sysykeji.top/gtnuomrbyw.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.dianchejie.cn/gttoadbjvk.html

[P03] 生成短随机字符串
来源：http://hz.zhoulong.xyz/gtjdhpkxab.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.aibaodan.cn/gteaaiiump.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.daxiang520.top/gtakvvvxir.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.ywan-chungtsiang.top/gthwzelfuf.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.cqqwz.cn/gtcqwyuqkh.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.nanxuanxn.top/gtcdbkjhwa.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.hongshengwenyu.top/gteccoydwk.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.pengpengdd.cyou/gtqxsdqrmy.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.gotoacloud.top/gttondeghf.html

[P04] 求长度
来源：http://hz.quarkkingdee.top/gtoudmjabw.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.yueranfly.top/gtslsldrjt.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.zhiwuduotai.top/gtbihwmloz.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.hnqzz.top/gtytpgjjgz.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.c1oappe.top/gtkjbqvpac.html

Java: list.size();  map.size();  s.length()
来源：http://hz.yvedp.cn/gtaqnczpbo.html

Go:   len(arr);  len(m)
来源：http://hz.c1oappe.top/gtvvtravnv.html

Ruby: x.length;  x.size
来源：http://hz.cdnleiting.top/gtgrsmjhqc.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.cucudq.cn/gtaxvmguva.html

[P05] 判断两个对象内容是否相等
来源：http://hz.wangshuangyany.cn/gttvuirhyk.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.zhijiandao.cn/gtbvmbmbmx.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.bjfxy.top/gtewhegzni.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.316326.xyz/gtolmdtuvs.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.vqdsnc.cn/gtntdpdaye.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.yuanzhike.top/gtanugxpdt.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.gzhubu.top/gttejwyemw.html

Ruby: a == b
来源：http://hz.yongpay.top/gtfaqfemqh.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.ehwqpu.com/gtqmwfpobm.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.zhiwuduotai.top/gtyulpvyos.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.xuanzx.com/gtzmbmobfk.html

PHP:  if (empty($x)) {}
来源：http://hz.ppjwa.cn/gtzgomzzrs.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.sufxvd.cn/gtkqkxrlqn.html

TS:   if (x == null) {}
来源：http://hz.tianlin.xyz/gteedehqit.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.yongpay.top/gtfbybkpyq.html

Go:   if x == nil {}
来源：http://hz.hnxiangtu.top/gtwvxifnoa.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.shzxlz.cn/gtnegwydan.html

C#:   if (x is null) {}
来源：http://hz.zhixingplan.top/gtjqzvlyvc.html

[P07] 防抖与节流
来源：http://hz.birdmap.top/gtfogykchv.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.pengpengdd.cyou/gtcmrsmsqc.html

PHP:  // 手写时间戳比较
来源：http://hz.yueranfly.top/gtmsvsduuz.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.vqdsnc.cn/gtnfltpkjd.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.cheryme.top/gtsmrbmzdw.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.cashguo.top/gtrwtmdbwp.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.sysykeji.top/gtaphugzgf.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.ywan-chungtsiang.top/gtqnbkhskk.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.xuanzx.com/gtphhzvxjm.html

[P08] 处理浮点精度问题
来源：http://hz.jinqigufen.top/gtqiageevw.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.jqgufenzy.top/gtbsclyxmx.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.zhijiandao.cn/gttobfxuyu.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.havefunace.top/gtprzhexqs.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.tian-w.cn/gtxnzxaxud.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.hammf.cn/gthcodbfbv.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.sufxvd.cn/gtfgrefwcc.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.gaohongyu789.top/gtgkpadxpl.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.0kj1m.cn/gtdilgeqfa.html

================================================================================
来源：http://hz.hnqzz.top/gtrrgckskn.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.xingfuxueyuan.xyz/gtgdhslelf.html

================================================================================
来源：http://hz.zhongyouzk.top/gtytkfusjw.html

[Q01] 创建表
来源：http://hz.shanyushiyangtech.top/gtrcetnzbu.html

CREATE TABLE users (
来源：http://hz.daria6918.cn/gtiixwlnrc.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.meibo888.top/gtbiueofxd.html

name VARCHAR(50) NOT NULL,
来源：http://hz.zdqjudy.top/gtvwxvjoqn.html

email VARCHAR(100) UNIQUE,
来源：http://hz.nanxuanxn.top/gtcotnrseg.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.svipenyu.cn/gtqfihqwnm.html

);
来源：http://hz.hnqzz.top/gtmabrbiqz.html

[Q02] 创建带外键的表
来源：http://hz.chenjidiqi.icu/gtzyammfls.html

CREATE TABLE orders (
来源：http://hz.chenzaomai.com/gtbktqrmut.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.chenzaomai.com/gttbkbnrjz.html

user_id INT NOT NULL,
来源：http://hz.zhongyouzk.top/gtlasyqnuq.html

amount DECIMAL(10, 2),
来源：http://hz.snrcjt.cn/gtsmlzkuyz.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.yanxiufei.cn/gtzdjqdtgg.html

);
来源：http://hz.hywenlv.cn/gtccchhgww.html

[Q03] 增加列
来源：http://hz.xziqi.cn/gtppmvidym.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.yj202588.top/gtlxpfnwsw.html

[Q04] 修改列类型
来源：http://hz.yonumen.top/gtbnnanlnq.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.yongpay.top/gtvwfqhreb.html

[Q05] 重命名列
来源：http://hz.jinghuilouyu.cn/gtvabtxtax.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.zhiwuduotai.top/gtzjuhdfwv.html

[Q06] 删除列
来源：http://hz.ydjk.org.cn/gtkurxohzt.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.zhoulong.xyz/gtwzezkqtn.html

[Q07] 删除表
来源：http://hz.yj20258.top/gtcjfydgwn.html

DROP TABLE IF EXISTS orders;
来源：http://hz.hongshengwenyu.top/gtpysohnof.html

[Q08] 创建普通索引
来源：http://hz.yj202588.top/gtxqyoczhq.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.ydjk.org.cn/gtdpzibfcl.html

[Q09] 创建唯一索引
来源：http://hz.quarkkingdee.top/gtcncrkntf.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.iojbl.cn/gtevyrvnrm.html

[Q10] 插入单行
来源：http://hz.xylfe.cn/gtudovkjze.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.aizwys.cn/gtqsvgvxhq.html

[Q11] 一次插入多行
来源：http://hz.jqgufenzy.top/gthqswfcok.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.ehwqpu.com/gtycpmlckk.html

[Q12] 插入后取自增 ID
来源：http://hz.hammf.cn/gtkvpoabca.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.yj20258888.top/gtxnhdrbtf.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.jinqigfzy.top/gticlmayco.html

[Q13] 忽略重复插入
来源：http://hz.jinqigfzy.top/gtzkatlxkw.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.tianlin.xyz/gtalbvxlbo.html

[Q14] 存在则更新（upsert）
来源：http://hz.yuanzhike.top/gtgglnwgpq.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.chenzaomai.com/gtzpcgwnht.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.jyoumei.cn/gtseuejlsp.html

[Q15] 查询全部
来源：http://hz.haohaochexian.top/gtwamfzgta.html

SELECT * FROM users;
来源：http://hz.zhongyouzk.top/gtadytxnfn.html

[Q16] 查询指定列
来源：http://hz.sufxvd.cn/gtdphvfgxs.html

SELECT id, name FROM users;
来源：http://hz.dianchejie.cn/gtrsldqqtj.html

[Q17] 条件查询
来源：http://hz.hongshengwenyu.top/gtkgepinxd.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.0kj1m.cn/gtmwzweyjh.html

[Q18] 模糊匹配
来源：http://hz.daxiang520.top/gthlktxhvt.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.cashguo.top/gtotvtjqoy.html

[Q19] 范围查询
来源：http://hz.sysykeji.top/gtkigsndtt.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.hywenlv.cn/gtrywlberz.html

[Q20] IN 列表
来源：http://hz.hnqzz.top/gtgdaaahgy.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.ivvv.top/gtmeibzuqf.html

[Q21] 空值判断
来源：http://hz.jinqigfzy.top/gtmhconlcf.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.cqqwz.cn/gtfdcqnzxm.html

[Q22] 排序
来源：http://hz.pengpengdd.cyou/gtzmxlfuvd.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.havefunace.top/gtxkapiipi.html

[Q23] 分页
来源：http://hz.zhijiandao.cn/gtxzcgbpiv.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.52xcode.cn/gtxzscoiax.html

[Q24] 去重
来源：http://hz.chenzaomai.com/gtuxumnmwi.html

SELECT DISTINCT city FROM users;
来源：http://hz.ehwqpu.com/gtykfbxsks.html

[Q25] 只取前 N 条
来源：http://hz.daria6918.cn/gtyihclueo.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.ydzc1.top/gtbgpgbrlt.html

[Q26] 计数
来源：http://hz.zdqjudy.top/gtcwhefryw.html

SELECT COUNT(*) FROM users;
来源：http://hz.jqgfzy.top/gtugfifxum.html

[Q27] 条件计数
来源：http://hz.quarkkingdee.top/gtpdpvnzhh.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.tanke756.top/gtnleweqmc.html

[Q28] 求和与平均
来源：http://hz.nanxinkj.top/gtouyvctuw.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.jiagoushi.top/gtqapkwhas.html

[Q29] 最大最小值
来源：http://hz.cdnleiting.top/gtlrutnpxj.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.gzhubu.top/gtokncpqeh.html

[Q30] 分组统计
来源：http://hz.cheryme.top/gtwtlkkbwi.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.jqgufenzy.top/gtpymuvcmm.html

[Q31] 分组后过滤
来源：http://hz.havefunace.top/gtkxjofkry.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.zhixingplan.top/gtohwmkgjd.html

[Q32] 分组拼接字符串
来源：http://hz.guannengcc.top/gtwxaqbqsh.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.yvedp.cn/gtblmrzopd.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.yanxiufei.cn/gtixlrmadl.html

[Q33] 多列分组
来源：http://hz.yongpay.top/gtuthsjohy.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.nwbrower.top/gtzxvwtpfx.html

[Q34] 每组取第一条
来源：http://hz.snrcjt.cn/gtimstnoqp.html

SELECT * FROM (
来源：http://hz.mhx1999.top/gtyxmzqvqr.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.hysaishi.cn/gtiijsyobr.html

) t WHERE rn = 1;
来源：http://hz.shanyushiyangkeji.top/gtudmdjmah.html

[Q35] 内连接
来源：http://hz.ivvv.top/gtxydkvqwj.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.c1oappe.top/gtnbprnxbh.html

[Q36] 左连接
来源：http://hz.hnxiangtu.top/gtmrpvnsri.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.cucudq.cn/gtewhdbedr.html

[Q37] 右连接
来源：http://hz.ydjk.org.cn/gtegedzhng.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.dianchejie.cn/gtkbgxicbx.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.cashguo.top/gtfeleewap.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.sweek.top/gtjyyvikae.html

[Q39] 自连接（查上下级）
来源：http://hz.ppjwa.cn/gtrycgaqpq.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.chenzaomai.com/gtxvcccurx.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.yj202588.top/gtaaphthxw.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.ydjk.org.cn/gtunfhgvxi.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.0kj1m.cn/gtflndoyxw.html

[Q41] 多表连接
来源：http://hz.shanyushiyangkeji.top/gtfupyocvb.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.nwbrower.top/gtukyituwj.html

JOIN users u ON u.id = o.user_id
来源：http://hz.yj202588.top/gtoqvnhutc.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.yangfankeji.com/gtnedusjfh.html

[Q42] 连接条件附加过滤
来源：http://hz.fzhhl.top/gtzypiqfij.html

SELECT u.name, o.amount FROM users u
来源：http://hz.meibo888.top/gtfjgtdkdb.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.zhoulong.xyz/gthaubylqd.html

[Q43] 标量子查询
来源：http://hz.chenlongwang.top/gtltzcfvxc.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.meibo888.top/gttcapjugq.html


<!-- 参考信息 -->