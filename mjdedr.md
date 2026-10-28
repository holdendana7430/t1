代发 wailian999

[N05] 最大公约数
来源：http://hz.yueranfly.top/gtsciqjclz.html

Py:   math.gcd(a, b)
来源：http://hz.sxryk.cn/gtpesvdavd.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.ydzc1.top/gtrrvskrsb.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.ybcxt.top/gtjiuakzkk.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.ppjwa.cn/gtxzoignxb.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.haohaochexian.top/gtsagpnbvl.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.yueranfly.top/gttlcmufst.html

Ruby: a.gcd(b)
来源：http://hz.sysykeji.top/gtvnkpmjvl.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.redwolf501.top/gtlrlpkbvo.html

[N06] 判断回文字符串
来源：http://hz.svipenyu.cn/gtsfxsvzcz.html

Py:   s == s[::-1]
来源：http://hz.gzhubu.top/gtkstefcdx.html

PHP:  $s === strrev($s);
来源：http://hz.redwolf501.top/gthwckhzfx.html

JS:   s === [...s].reverse().join("")
来源：http://hz.birdmap.top/gtlpfvxzmn.html

TS:   s === [...s].reverse().join("")
来源：http://hz.xuanzx.com/gtdfwbuczu.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.cdnleiting.top/gtlfbopsuu.html

Go:   // 双指针从两端比较
来源：http://hz.dianchejie.cn/gttzrfvkzg.html

Ruby: s == s.reverse
来源：http://hz.yueranfly.top/gtcsnotdxr.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.xziqi.cn/gtnrsrtots.html

[N07] 两数之和（返回下标）
来源：http://hz.shanyushiyangkeji.top/gtzgyvdvre.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.chenjidiqi.icu/gtcgiikefw.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.xingfuxueyuan.xyz/gtcobxabvp.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.zhengqikj.top/gtmbzscklt.html

TS:   // 手写 Map<string, number>
来源：http://hz.jinghuilouyu.cn/gtprpmgqqi.html

Java: // 手写 HashMap
来源：http://hz.jinyuanbaomall.cn/gtvdypcvys.html

Go:   // 手写 map[int]int
来源：http://hz.sysykeji.top/gtrzwgaboq.html

Ruby: // 手写 Hash
来源：http://hz.ivvv.top/gtbpvefmua.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.jinghuilouyu.cn/gtrzxiocgm.html

[N08] 生成全排列
来源：http://hz.snrcjt.cn/gtofzgacbv.html

Py:   itertools.permutations(arr)
来源：http://hz.nwbrower.top/gtbbtltbfo.html

PHP:  // 手写递归交换
来源：http://hz.hongshengwenyu.top/gtbnbcxlpj.html

JS:   // 手写回溯递归
来源：http://hz.zhengqikj.top/gtuwbcyzvh.html

TS:   // 手写回溯递归
来源：http://hz.kuanghao11.cn/gtbyznhqsh.html

Java: // 手写回溯递归
来源：http://hz.sysykeji.top/gtvrxrrlhe.html

Go:   // 手写回溯递归
来源：http://hz.bjfxy.top/gtpojukyll.html

Ruby: arr.permutation.to_a
来源：http://hz.zhaomingkeji.xyz/gtzexcyiel.html

C#:   // 手写回溯递归
来源：http://hz.jinghuilouyu.cn/gtfjgqlczw.html

[N09] 栈与队列
来源：http://hz.xziqi.cn/gtswahbkdt.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.zhijiandao.cn/gtnmtvzjsm.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.sweek.top/gtrcznbnku.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.zhengqikj.top/gtpwtsrkag.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.zhengqikj.top/gtllsevtxu.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.zhijiandao.cn/gtvibjigpe.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.xylfe.cn/gtnwsyxqze.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.yangfankeji.com/gteyzyvzml.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.sweek.top/gtcztymlfu.html

[N10] 链表节点定义
来源：http://hz.shanyushiyangtech.top/gtaokuelhr.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.jinqigufen.top/gtbhrigmjx.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.shzxlz.cn/gtihjaflly.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.gzhubu.top/gtyachorlz.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.shanyushiyangkeji.top/gtdohorhuw.html

Java: class Node { int v; Node next; }
来源：http://hz.havefunace.top/gtjblfycqb.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.cqqwz.cn/gtnmjgmeol.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.daria6918.cn/gtyzxgucrs.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.cqqwz.cn/gtbrfclblm.html

[N11] 二叉树中序遍历
来源：http://hz.jiagoushi.top/gtcjhmqyes.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.snrcjt.cn/gtikpcsywh.html

PHP:  // 手写递归函数
来源：http://hz.yanxiufei.cn/gtfvmdcgcy.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.guowangkeji.top/gtxevcwbuq.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.zhoulong.xyz/gtgsfedome.html

Java: // 手写递归
来源：http://hz.yangfankeji.com/gtbbybbkob.html

Go:   // 手写递归
来源：http://hz.dashuyun.cn/gtdhwcmjem.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.sweek.top/gtrkxicuvx.html

C#:   // 手写递归
来源：http://hz.yuanzhike.top/gtstirgjjy.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.havefunace.top/gtegwqjwdn.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.daria6918.cn/gtafhgrvup.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.jyoumei.cn/gtnlurskxt.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.jianghu66.top/gtcjbsqyto.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.xingfuxueyuan.xyz/gtrbkikoys.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.gzhubu.top/gtavxihqkf.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.zhixingplan.top/gtmjdkkxcw.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.andypj.xyz/gtnewpmozj.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.zhoulong.xyz/gtjsxbciej.html

================================================================================
来源：http://hz.feifeiyinyue.top/gteumzbqjo.html

O. 并发与异步
来源：http://hz.wangdashe.top/gtntjamznh.html

================================================================================
来源：http://hz.tianlin.xyz/gtiiiebzif.html

[O01] 启动一个线程
来源：http://hz.feifeiyinyue.top/gtiltugamj.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.birdmap.top/gtvsvybkiu.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.zhaomingkeji.xyz/gtxdicrrzn.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.aibaodan.cn/gtewkpsaos.html

TS:   // 同 JS
来源：http://hz.yuanzhike.top/gtocwemzzx.html

Java: new Thread(() -> f()).start()
来源：http://hz.redwolf501.top/gtudlqiysb.html

Go:   go f()
来源：http://hz.hnqzz.top/gtsjugecvd.html

Ruby: Thread.new { f }
来源：http://hz.yueranfly.top/gtutgjovww.html

C#:   Task.Run(() => F());
来源：http://hz.yuxming.cn/gttrlydlaz.html

[O02] 使用线程池
来源：http://hz.jqgufenzy.top/gtsdidbiom.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.jinqigufen.top/gtljbsxnvc.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.hywenlv.cn/gtwkygnoeq.html

JS:   // worker_threads 线程池
来源：http://hz.vqdsnc.cn/gtcebtksaq.html

TS:   // worker_threads 线程池
来源：http://hz.daxiang520.top/gtqmlbcciz.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.aibaodan.cn/gtjxpinhwx.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.xuetiantiany.cn/gtozfgnzge.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.yvedp.cn/gtcowxcoxa.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.316326.xyz/gtzscnspaa.html

[O03] 加锁保护共享数据
来源：http://hz.havefunace.top/gtknglruey.html

Py:   with lock: shared += 1
来源：http://hz.xinyue.icu/gtwvjzwwwh.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.jinyuanbaomall.cn/gtgbnhnvne.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.yanxiufei.cn/gtozatzzio.html

TS:   // 同 JS
来源：http://hz.0kj1m.cn/gtpsvjozgj.html

Java: synchronized (this) { shared++; }
来源：http://hz.redwolf501.top/gtltqadcyr.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.nanxuanxn.top/gttrizrltt.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.dianchejie.cn/gtxheqsxxy.html

C#:   lock (gate) { shared++; }
来源：http://hz.hammf.cn/gtihbtfnpp.html

[O04] 定义异步函数并等待
来源：http://hz.zhijiandao.cn/gttetbapyu.html

Py:   async def f():⏎    await g()
来源：http://hz.shanyushiyangtech.top/gtvjyfxokh.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.ehwqpu.com/gtioycrxbu.html

JS:   async function f() { await g(); }
来源：http://hz.gotoacloud.top/gtstdpteet.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.xuetiantiany.cn/gtbdmysybr.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.yonumen.top/gtzsmscdmz.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.zdqjudy.top/gtsihbwpnm.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.9152youxi.cn/gtnqnaxzyv.html

C#:   async Task F() { await G(); }
来源：http://hz.smart0.xyz/gtbliwwoht.html

[O05] 并发执行并等待全部完成
来源：http://hz.nanxinkj.top/gtabyxrwzu.html

Py:   asyncio.gather(*tasks)
来源：http://hz.havefunace.top/gtbzaersqk.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.cashguo.top/gtplqdomjv.html

JS:   await Promise.all(tasks)
来源：http://hz.shuidangran.top/gtumaurkdj.html

TS:   await Promise.all(tasks)
来源：http://hz.jianghu66.top/gtdpwpikle.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.yuxming.cn/gtbesldxtg.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.jinqigfzy.top/gtotdtpydg.html

Ruby: threads.map(&:join)
来源：http://hz.yanxiufei.cn/gthxhsfnro.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.svipenyu.cn/gtdqvjgmns.html

[O06] 使用进程池
来源：http://hz.xuetiantiany.cn/gtzivyisio.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.daria6918.cn/gtastsfziz.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.yangfankeji.com/gtxjxabdxf.html

JS:   // child_process / cluster 模块
来源：http://hz.zhaomingkeji.xyz/gtozntoybl.html

TS:   // child_process / cluster 模块
来源：http://hz.sxryk.cn/gtenlyhpzi.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.tian-w.cn/gtqfnzsvdr.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.wangdashe.top/gtqqkluqgq.html

Ruby: // fork 块
来源：http://hz.hnxiangtu.top/gtrcmpoevo.html

C#:   Parallel.For
来源：http://hz.hongshengwenyu.top/gtdibdjoun.html

================================================================================
来源：http://hz.yvedp.cn/gtijlagbvi.html

P. 常用工具函数
来源：http://hz.cqqwz.cn/gtmxtdwwyj.html

================================================================================
来源：http://hz.ydzc1.top/gtcvmhmpzp.html

[P01] 生成 UUID
来源：http://hz.zhiwuduotai.top/gtaasreoqv.html

Py:   str(uuid.uuid4())
来源：http://hz.tanke756.top/gtmppaxicv.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.yj20258.top/gtusypzccb.html

JS:   crypto.randomUUID()
来源：http://hz.chenjidiqi.icu/gtensztdck.html

TS:   crypto.randomUUID()
来源：http://hz.zhijiandao.cn/gtmojpbtqi.html

Java: UUID.randomUUID().toString()
来源：http://hz.cqqwz.cn/gtuqryrjlv.html

Go:   // 用 github.com/google/uuid
来源：http://hz.yuanzhike.top/gtwkgqglil.html

Ruby: SecureRandom.uuid
来源：http://hz.hysaishi.cn/gtyhwzrwja.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.gogol.net.cn/gtpknfkjuf.html

[P02] MD5 / SHA256 摘要
来源：http://hz.0kj1m.cn/gtbcvebevh.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.jiagoushi.top/gtoiwrtoan.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.dianchejie.cn/gtddevvpkg.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.nanxinkj.top/gtdiffpolw.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.jinyuanbaomall.cn/gtsiavhela.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.shangyingyoupin.top/gtaeelqspz.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.birdmap.top/gtbpibagbj.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.316326.xyz/gtacyehaxc.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.pengpengdd.cyou/gtxyswyils.html

[P03] 生成短随机字符串
来源：http://hz.hnxiangtu.top/gtsedgnfya.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.ydjk.org.cn/gttrcmrsqm.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.hnqzz.top/gtyjcumdij.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.ydjk.org.cn/gtagkkwucg.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.fzhhl.top/gtljvbaghu.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.xuanzx.com/gtdcqnrhjf.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.smart0.xyz/gthvuzcudf.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.quarkkingdee.top/gtgfpevzud.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.chenlongwang.top/gtucbswjhb.html

[P04] 求长度
来源：http://hz.jinqigfzy.top/gtjqqiwkgw.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.jlsjyb.cn/gtuynkjgoh.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.zycfv.cn/gtiwlmkyls.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.aizwys.cn/gtnczxhshu.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.chenjidiqi.icu/gtfgkrmoyj.html

Java: list.size();  map.size();  s.length()
来源：http://hz.fengsongda.top/gtjthirmrp.html

Go:   len(arr);  len(m)
来源：http://hz.gotoacloud.top/gtzcviwvhn.html

Ruby: x.length;  x.size
来源：http://hz.gaohongyu789.top/gtyaxpxaur.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.cucudq.cn/gtdnbzdpow.html

[P05] 判断两个对象内容是否相等
来源：http://hz.ivvv.top/gtugxyqlee.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.yj20258.top/gtiwvkshpd.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.ivvv.top/gttiisoyvf.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.aizwys.cn/gtqoxsxuvi.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.xylfe.cn/gtlxrquxit.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.zhengqikj.top/gtpiclsypv.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.guowangkeji.top/gtggwqztts.html

Ruby: a == b
来源：http://hz.xylfe.cn/gtydjzrhxz.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.quarkkingdee.top/gtlxfrcgjm.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.hnxiangtu.top/gtokqyqjro.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.ppjwa.cn/gtkelhualn.html

PHP:  if (empty($x)) {}
来源：http://hz.meibo888.top/gtgygpivlh.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.jinqigfzy.top/gthclgksvu.html

TS:   if (x == null) {}
来源：http://hz.zhixingplan.top/gtrvaxbdxk.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.cqqwz.cn/gtnahmcwbv.html

Go:   if x == nil {}
来源：http://hz.quarkkingdee.top/gtmeccfqms.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.zhijiandao.cn/gtvyxmehtu.html

C#:   if (x is null) {}
来源：http://hz.andypj.xyz/gtkrkdsmqt.html

[P07] 防抖与节流
来源：http://hz.yj20258.top/gtrjljvkor.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.sweek.top/gthfzgcuer.html

PHP:  // 手写时间戳比较
来源：http://hz.ivvv.top/gtpkzdnzwb.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.chenlongwang.top/gtpkjnzpmn.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.yvedp.cn/gtxwiurgdv.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.meibo888.top/gticzzdrxd.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.shanyushiyangkeji.top/gtljedgpfj.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.yonumen.top/gtgeknzsbl.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.vqdsnc.cn/gtgwxxdqxb.html

[P08] 处理浮点精度问题
来源：http://hz.snrcjt.cn/gtoeydxzul.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.vqdsnc.cn/gtbtbunpbc.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.ehwqpu.com/gtfjoktzmb.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.shangyingyoupin.top/gtntcjdcvf.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.ydzc1.top/gtmxuymtmu.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.zhijiandao.cn/gtiymvlsdc.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.chenlongwang.top/gtemwpljvh.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.xinyue.icu/gtorxrzeic.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.nwbrower.top/gtxofyuduf.html

================================================================================
来源：http://hz.snrcjt.cn/gtjbkiicck.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.yongpay.top/gtlgybnejz.html

================================================================================
来源：http://hz.shanyushiyangkeji.top/gtskxxsqxy.html

[Q01] 创建表
来源：http://hz.jinqigfzy.top/gtngueomsy.html

CREATE TABLE users (
来源：http://hz.havefunace.top/gtlccfzcrv.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.chenzaomai.com/gtxcydximt.html

name VARCHAR(50) NOT NULL,
来源：http://hz.ybcxt.top/gtlpdkopex.html

email VARCHAR(100) UNIQUE,
来源：http://hz.cheryme.top/gtjtbbijju.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.iojbl.cn/gtsngowjot.html

);
来源：http://hz.shanyushiyangtech.top/gtadzaqjno.html

[Q02] 创建带外键的表
来源：http://hz.meibo888.top/gtdkmetsgv.html

CREATE TABLE orders (
来源：http://hz.jinyuanbaomall.cn/gtjzvwwujg.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.nanxuanxn.top/gtflercxjo.html

user_id INT NOT NULL,
来源：http://hz.guowangkeji.top/gtgarptxfa.html

amount DECIMAL(10, 2),
来源：http://hz.316326.xyz/gtdhovhjeq.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.hywenlv.cn/gtqglodzxw.html

);
来源：http://hz.sufxvd.cn/gtqcrkpxeo.html

[Q03] 增加列
来源：http://hz.chenjidiqi.icu/gtsjvaayas.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.daxiang520.top/gtxjudglbk.html

[Q04] 修改列类型
来源：http://hz.xziqi.cn/gtnybpyvkc.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.dashuyun.cn/gtjlvkrhax.html

[Q05] 重命名列
来源：http://hz.chenlongwang.top/gtjsirqpuo.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.jqgufenzy.top/gtkibdanvf.html

[Q06] 删除列
来源：http://hz.jiagoushi.top/gtgqsxkgsw.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.ehwqpu.com/gtjgnetuzx.html

[Q07] 删除表
来源：http://hz.pengpengdd.cyou/gtxfeokbqc.html

DROP TABLE IF EXISTS orders;
来源：http://hz.yj20258888.top/gtoxseldvx.html

[Q08] 创建普通索引
来源：http://hz.bjfxy.top/gtxeggzdur.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.meibo888.top/gtyilnsyny.html

[Q09] 创建唯一索引
来源：http://hz.ivvv.top/gtmqtfelro.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.jlsjyb.cn/gtapgtzofo.html

[Q10] 插入单行
来源：http://hz.jiagoushi.top/gtnygwcrtw.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.jqgfzy.top/gtwmakqver.html

[Q11] 一次插入多行
来源：http://hz.dashuyun.cn/gtnwrqjxbi.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.yongpay.top/gttjztdyqi.html

[Q12] 插入后取自增 ID
来源：http://hz.9152youxi.cn/gtgltvhkos.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.daxiang520.top/gtdehlljyo.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.jinyuanbaomall.cn/gtoagyqshh.html

[Q13] 忽略重复插入
来源：http://hz.zdqjudy.top/gtndkdpmfj.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.zhengqikj.top/gtbijflsyj.html

[Q14] 存在则更新（upsert）
来源：http://hz.tanke756.top/gtllbpzrmh.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.shzxlz.cn/gtygomcgqx.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.yvedp.cn/gtjkmgxbsz.html

[Q15] 查询全部
来源：http://hz.kuanghao11.cn/gtvtxwcksr.html

SELECT * FROM users;
来源：http://hz.c1oappe.top/gtkqbtfiwm.html

[Q16] 查询指定列
来源：http://hz.dashuyun.cn/gttivbdncl.html

SELECT id, name FROM users;
来源：http://hz.ppjwa.cn/gtbqyyfzks.html

[Q17] 条件查询
来源：http://hz.jinghuilouyu.cn/gtevotgvpd.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.sysykeji.top/gttwhtdpgs.html

[Q18] 模糊匹配
来源：http://hz.ehwqpu.com/gtaspxrteu.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.yuxming.cn/gtosikffid.html

[Q19] 范围查询
来源：http://hz.shzxlz.cn/gtudlltebv.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.zhoulong.xyz/gtwziiqerc.html

[Q20] IN 列表
来源：http://hz.gaohongyu789.top/gtvejoecka.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.sxryk.cn/gtgmzvcjsu.html

[Q21] 空值判断
来源：http://hz.zhixingplan.top/gtycxhjyga.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.pengpengdd.cyou/gtceblxojj.html

[Q22] 排序
来源：http://hz.havefunace.top/gtyvujbwlk.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.c1oappe.top/gtxrsewrdn.html

[Q23] 分页
来源：http://hz.hysaishi.cn/gtbnepodrn.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.jlsjyb.cn/gtruuwppei.html

[Q24] 去重
来源：http://hz.cqqwz.cn/gtfwctqlhf.html

SELECT DISTINCT city FROM users;
来源：http://hz.zhijiandao.cn/gtebkmarov.html

[Q25] 只取前 N 条
来源：http://hz.smart0.xyz/gtniyurgoc.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.0kj1m.cn/gtuhocdszm.html

[Q26] 计数
来源：http://hz.yuanzhike.top/gthctlaxxr.html

SELECT COUNT(*) FROM users;
来源：http://hz.dianchejie.cn/gtygxjiscu.html

[Q27] 条件计数
来源：http://hz.jianghu66.top/gtorwjsrmc.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.shuidangran.top/gtujdykucs.html

[Q28] 求和与平均
来源：http://hz.fengsongda.top/gtlkmuckfv.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.cqqwz.cn/gtdcexcwlb.html

[Q29] 最大最小值
来源：http://hz.guowangkeji.top/gtzhzmaksy.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.52xcode.cn/gtkncxpcyn.html

[Q30] 分组统计
来源：http://hz.shanyushiyangtech.top/gtjolzrgog.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.xuetiantiany.cn/gtttxyecpu.html

[Q31] 分组后过滤
来源：http://hz.kuanghao11.cn/gtnitpxsbw.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.hnqzz.top/gtsjsbkfqa.html

[Q32] 分组拼接字符串
来源：http://hz.cashguo.top/gtugijyadq.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.zycfv.cn/gtgthemarl.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.iojbl.cn/gtvxqfgfwl.html

[Q33] 多列分组
来源：http://hz.tanke756.top/gtufymulkv.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.iojbl.cn/gtctglequz.html

[Q34] 每组取第一条
来源：http://hz.tianlin.xyz/gtndcsashu.html

SELECT * FROM (
来源：http://hz.52xcode.cn/gtjzpugnan.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.aibaodan.cn/gtjgjyuxfr.html

) t WHERE rn = 1;
来源：http://hz.zhongyouzk.top/gtdgppgqpm.html

[Q35] 内连接
来源：http://hz.iojbl.cn/gtzdpelvwt.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.gotoacloud.top/gtysfruvnx.html

[Q36] 左连接
来源：http://hz.xuetiantiany.cn/gtrcpkeojs.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.ywan-chungtsiang.top/gtamksjevw.html

[Q37] 右连接
来源：http://hz.sweek.top/gtwwsawkuw.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.feifeiyinyue.top/gtbqtvmezi.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.zhengqikj.top/gtocxinidt.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.hysaishi.cn/gtztpsnyhn.html

[Q39] 自连接（查上下级）
来源：http://hz.gzhubu.top/gtiecvfizp.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.wangdashe.top/gtwwuknlib.html


<!-- 参考信息 -->