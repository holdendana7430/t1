代发 wailian999

[N05] 最大公约数
来源：http://hz.hysaishi.cn/gtnshaceqp.html

Py:   math.gcd(a, b)
来源：http://hz.meibo888.top/gtlybywsqb.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.meibo888.top/gtbwjztfeu.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.tianlin.xyz/gtxmhvvdry.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.yj202588.top/gtasynsdbm.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.jinghuilouyu.cn/gtpptfkmot.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.kuanghao11.cn/gtohhpzmum.html

Ruby: a.gcd(b)
来源：http://hz.chenzaomai.com/gtxgliauvs.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.yuanzhike.top/gtkizbjqnk.html

[N06] 判断回文字符串
来源：http://hz.snrcjt.cn/gtlquldxgk.html

Py:   s == s[::-1]
来源：http://hz.jlsjyb.cn/gtzctpzgpp.html

PHP:  $s === strrev($s);
来源：http://hz.snrcjt.cn/gtnjywdmca.html

JS:   s === [...s].reverse().join("")
来源：http://hz.dianchejie.cn/gtvpvjqhiy.html

TS:   s === [...s].reverse().join("")
来源：http://hz.chenjidiqi.icu/gtcwxmbxgc.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.quarkkingdee.top/gtajwzdwhc.html

Go:   // 双指针从两端比较
来源：http://hz.dashuyun.cn/gtswhtgrfl.html

Ruby: s == s.reverse
来源：http://hz.yj20258.top/gtgrlyyvuy.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.c1oappe.top/gtackmqifb.html

[N07] 两数之和（返回下标）
来源：http://hz.yanxiufei.cn/gtokschusd.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.zhaomingkeji.xyz/gtrgycqwam.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.dashuyun.cn/gtoixudoty.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.ydzc1.top/gteucfccsz.html

TS:   // 手写 Map<string, number>
来源：http://hz.meibo888.top/gtxekxqwhc.html

Java: // 手写 HashMap
来源：http://hz.hongshengwenyu.top/gtrouvqxpq.html

Go:   // 手写 map[int]int
来源：http://hz.pengpengdd.cyou/gtqtuttehz.html

Ruby: // 手写 Hash
来源：http://hz.kuanghao11.cn/gtntbwrgee.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.hnxiangtu.top/gtfimlupuq.html

[N08] 生成全排列
来源：http://hz.zhaomingkeji.xyz/gttobbdtas.html

Py:   itertools.permutations(arr)
来源：http://hz.ydzc1.top/gtsnnucyhv.html

PHP:  // 手写递归交换
来源：http://hz.dashuyun.cn/gtepwijtoc.html

JS:   // 手写回溯递归
来源：http://hz.ppjwa.cn/gtwlmavsyr.html

TS:   // 手写回溯递归
来源：http://hz.iojbl.cn/gtzkwtbqpn.html

Java: // 手写回溯递归
来源：http://hz.wangdashe.top/gtovqztpck.html

Go:   // 手写回溯递归
来源：http://hz.316326.xyz/gtbncbbgch.html

Ruby: arr.permutation.to_a
来源：http://hz.nanxinkj.top/gtpwwrysiz.html

C#:   // 手写回溯递归
来源：http://hz.aibaodan.cn/gtwfmstcio.html

[N09] 栈与队列
来源：http://hz.yuxming.cn/gtzlcdzagh.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.ywan-chungtsiang.top/gtyadbuasx.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.sweek.top/gtuketbnjc.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.52xcode.cn/gtgylsddqy.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.haohaochexian.top/gtghujvtac.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.zhengqikj.top/gtbafuztyq.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.daria6918.cn/gtduthwcxf.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.kuanghao11.cn/gtrrzqdfdh.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.gogol.net.cn/gtrksydpfp.html

[N10] 链表节点定义
来源：http://hz.yonumen.top/gtubblfxiv.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.zycfv.cn/gtxutfnlxh.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.jyoumei.cn/gttgnzbhba.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.ywan-chungtsiang.top/gtuqjdiaro.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.cheryme.top/gtjxqztpux.html

Java: class Node { int v; Node next; }
来源：http://hz.haohaochexian.top/gtikvelvrk.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.meibo888.top/gtpsbnbfag.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.jinqigufen.top/gthookywqf.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.yj20258.top/gtvafmmydn.html

[N11] 二叉树中序遍历
来源：http://hz.nanxinkj.top/gtaqgwrgeu.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.shangyingyoupin.top/gtqiapucdn.html

PHP:  // 手写递归函数
来源：http://hz.ivvv.top/gtymwprvmv.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.gzhubu.top/gthaimmkon.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.jiagoushi.top/gtdmmchovw.html

Java: // 手写递归
来源：http://hz.zhiwuduotai.top/gtyeebxblu.html

Go:   // 手写递归
来源：http://hz.ydjk.org.cn/gtethriptf.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.jiagoushi.top/gttfqqfgcr.html

C#:   // 手写递归
来源：http://hz.ehwqpu.com/gtwcjulfmi.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.yonumen.top/gtzcsfrssw.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.9152youxi.cn/gtcvaixrzt.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.quarkkingdee.top/gtmjhanyxm.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.yj20258.top/gtobdbhawk.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.mhx1999.top/gtzgnerfrk.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.jinghuilouyu.cn/gtqvlsatuc.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.gzhubu.top/gttlwkhehe.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.zhoulong.xyz/gtlfgypyyv.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.sweek.top/gtmtqyaeis.html

================================================================================
来源：http://hz.jinqigfzy.top/gtivacolwj.html

O. 并发与异步
来源：http://hz.zhongyouzk.top/gtxtlknxyj.html

================================================================================
来源：http://hz.cdnleiting.top/gthcecvpfc.html

[O01] 启动一个线程
来源：http://hz.jinqigfzy.top/gthsibxsnr.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.sweek.top/gttradtuhx.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.vqdsnc.cn/gticaeeehy.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.cdnleiting.top/gtnecejmqp.html

TS:   // 同 JS
来源：http://hz.ivvv.top/gteupczsyv.html

Java: new Thread(() -> f()).start()
来源：http://hz.zhaomingkeji.xyz/gtitiaokbb.html

Go:   go f()
来源：http://hz.zhiwuduotai.top/gtoygutfbm.html

Ruby: Thread.new { f }
来源：http://hz.yonumen.top/gtizsxdmwz.html

C#:   Task.Run(() => F());
来源：http://hz.cucudq.cn/gtbyozrluv.html

[O02] 使用线程池
来源：http://hz.nanxuanxn.top/gtncgtkuye.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.jinyuanbaomall.cn/gtvbvvxaww.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.tanke756.top/gtglqrxwuz.html

JS:   // worker_threads 线程池
来源：http://hz.sufxvd.cn/gtrkfhksar.html

TS:   // worker_threads 线程池
来源：http://hz.ydjk.org.cn/gtvaoeoltw.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.iojbl.cn/gteksarvlh.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.cucudq.cn/gtfilfnhyz.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.daria6918.cn/gtubziaxmg.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.yvedp.cn/gtguvqslvz.html

[O03] 加锁保护共享数据
来源：http://hz.meibo888.top/gtkquqixdv.html

Py:   with lock: shared += 1
来源：http://hz.gzhubu.top/gtrmxhzgqz.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.jinyuanbaomall.cn/gtbdjwtcvl.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.cashguo.top/gticeesjnv.html

TS:   // 同 JS
来源：http://hz.jqgfzy.top/gtmtiktthz.html

Java: synchronized (this) { shared++; }
来源：http://hz.chenjidiqi.icu/gtnrfgvihf.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.jqgfzy.top/gtfewxygkw.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.shzxlz.cn/gtkwkuuixi.html

C#:   lock (gate) { shared++; }
来源：http://hz.sweek.top/gtfhxhyyvw.html

[O04] 定义异步函数并等待
来源：http://hz.aizwys.cn/gtpvqjrxlb.html

Py:   async def f():⏎    await g()
来源：http://hz.jinghuilouyu.cn/gtbhkwwzxh.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.jianghu66.top/gtbgrkzolp.html

JS:   async function f() { await g(); }
来源：http://hz.xziqi.cn/gtuftieija.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.xuanzx.com/gtzrrzcnsf.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.havefunace.top/gtrstjrphd.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.0kj1m.cn/gtspnhrtcw.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.cqqwz.cn/gtvyrnknzu.html

C#:   async Task F() { await G(); }
来源：http://hz.gzhubu.top/gtsnbnlhyi.html

[O05] 并发执行并等待全部完成
来源：http://hz.jyoumei.cn/gtferrwkej.html

Py:   asyncio.gather(*tasks)
来源：http://hz.jqgufenzy.top/gtjncpzowt.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.sweek.top/gtqsdydrpg.html

JS:   await Promise.all(tasks)
来源：http://hz.yj20258888.top/gtywqbxhyd.html

TS:   await Promise.all(tasks)
来源：http://hz.zhiwuduotai.top/gtcbmlbixk.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.zhaomingkeji.xyz/gtyvarskwu.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.zhoulong.xyz/gtdgznngwc.html

Ruby: threads.map(&:join)
来源：http://hz.daxiang520.top/gtmzltfjwv.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.52xcode.cn/gteoakkvij.html

[O06] 使用进程池
来源：http://hz.yueranfly.top/gtzwdipoid.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.jinghuilouyu.cn/gttasusstb.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.hysaishi.cn/gtfcahwtdu.html

JS:   // child_process / cluster 模块
来源：http://hz.smart0.xyz/gtmejwegap.html

TS:   // child_process / cluster 模块
来源：http://hz.jqgufenzy.top/gtpofuxwxk.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.gogol.net.cn/gtzwrdqzfy.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.mhx1999.top/gtkjfdugqo.html

Ruby: // fork 块
来源：http://hz.nanxuanxn.top/gtkcujnnxm.html

C#:   Parallel.For
来源：http://hz.yuanzhike.top/gtuivetdil.html

================================================================================
来源：http://hz.redwolf501.top/gtijpctsro.html

P. 常用工具函数
来源：http://hz.mhx1999.top/gtrpvgduhd.html

================================================================================
来源：http://hz.cqqwz.cn/gtrpcnkbvn.html

[P01] 生成 UUID
来源：http://hz.xuetiantiany.cn/gtfknnsnol.html

Py:   str(uuid.uuid4())
来源：http://hz.shanyushiyangtech.top/gtengdynwv.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.havefunace.top/gtkbsnrrld.html

JS:   crypto.randomUUID()
来源：http://hz.cqqwz.cn/gtzdflshop.html

TS:   crypto.randomUUID()
来源：http://hz.zhiwuduotai.top/gtikuwapsv.html

Java: UUID.randomUUID().toString()
来源：http://hz.jqgufenzy.top/gtwqbrsyne.html

Go:   // 用 github.com/google/uuid
来源：http://hz.cheryme.top/gtaysldtzh.html

Ruby: SecureRandom.uuid
来源：http://hz.hysaishi.cn/gtpcuefysj.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.nanxuanxn.top/gtcgccllvw.html

[P02] MD5 / SHA256 摘要
来源：http://hz.316326.xyz/gtphdjalzy.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.yvedp.cn/gtibcuoeoo.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.cucudq.cn/gtxfuzjwwc.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.jqgfzy.top/gtunnbpdes.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.yj20258888.top/gtdqkobmrd.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.zhijiandao.cn/gtmvduwgud.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.xylfe.cn/gthopgzlno.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.mhx1999.top/gtvimdttrb.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.hnqzz.top/gtljdtlvcb.html

[P03] 生成短随机字符串
来源：http://hz.chenlongwang.top/gtzowswjkn.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.316326.xyz/gtkjdpisvw.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.zdqjudy.top/gtwwhgnwfv.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.mhx1999.top/gtiavbvwpt.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.shangyingyoupin.top/gtcggtfmkd.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.guowangkeji.top/gtkllqgykw.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.shanyushiyangtech.top/gtcfvrphlk.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.hysaishi.cn/gtnhzxpjii.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.yonumen.top/gtvvqvbnvu.html

[P04] 求长度
来源：http://hz.tanke756.top/gtqszqyeln.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.chenlongwang.top/gtatlkfirh.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.guowangkeji.top/gtwbyjlvrg.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.yj202588.top/gtegnztpkw.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.zhoulong.xyz/gtajwiugwl.html

Java: list.size();  map.size();  s.length()
来源：http://hz.meibo888.top/gtcaeucqhj.html

Go:   len(arr);  len(m)
来源：http://hz.jyoumei.cn/gtngsrthmb.html

Ruby: x.length;  x.size
来源：http://hz.dianchejie.cn/gtmuxossqe.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.ppjwa.cn/gtkxdynllg.html

[P05] 判断两个对象内容是否相等
来源：http://hz.jqgufenzy.top/gtdnkmgwdn.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.52xcode.cn/gtcfmhpsdf.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.chenzaomai.com/gtxwzipanu.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.chenlongwang.top/gtwjoardjw.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.jinqigfzy.top/gtljscleox.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.zdqjudy.top/gtkpwetxch.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.ywan-chungtsiang.top/gtjvbnjryc.html

Ruby: a == b
来源：http://hz.pycfn.com/gtfmwapiqr.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.zhijiandao.cn/gtjywnvngw.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.xuanzx.com/gtpiqvojcu.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.hywenlv.cn/gtsevuuhzf.html

PHP:  if (empty($x)) {}
来源：http://hz.tanke756.top/gtamjurdmz.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.iojbl.cn/gtqmlylrnc.html

TS:   if (x == null) {}
来源：http://hz.shzxlz.cn/gtglasuarl.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.ydjk.org.cn/gtrjajwquy.html

Go:   if x == nil {}
来源：http://hz.ydzc1.top/gttexyzacs.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.redwolf501.top/gttzukgcev.html

C#:   if (x is null) {}
来源：http://hz.cucudq.cn/gtdccsneyb.html

[P07] 防抖与节流
来源：http://hz.hammf.cn/gtopsbtoyj.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.zhijiandao.cn/gtbmyscndh.html

PHP:  // 手写时间戳比较
来源：http://hz.hammf.cn/gtfhwpepad.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.zhixingplan.top/gtvvucsjlp.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.guowangkeji.top/gtqcxjmgxi.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.nanxuanxn.top/gtisdzuyqo.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.hnqzz.top/gtdxgcyzhd.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.hysaishi.cn/gtdksdvfdn.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.xingfuxueyuan.xyz/gtruqfbbva.html

[P08] 处理浮点精度问题
来源：http://hz.pengpengdd.cyou/gtjshqpggq.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.jiagoushi.top/gttxuogxcj.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.ppjwa.cn/gtbouofvks.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.havefunace.top/gtezknjltm.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.dashuyun.cn/gtbimjootn.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.jinyuanbaomall.cn/gtqcmmyzvf.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.cucudq.cn/gtafahxgem.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.0kj1m.cn/gtqybyqyvo.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.zycfv.cn/gtavbgzjvs.html

================================================================================
来源：http://hz.cheryme.top/gtmfawdkga.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.gzhubu.top/gtyakhlfvx.html

================================================================================
来源：http://hz.andypj.xyz/gtcyatmthu.html

[Q01] 创建表
来源：http://hz.chenjidiqi.icu/gtbhiwlaeq.html

CREATE TABLE users (
来源：http://hz.hfpthk.cn/gtxmtqoepv.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.zycfv.cn/gttmjefswg.html

name VARCHAR(50) NOT NULL,
来源：http://hz.hywenlv.cn/gtyzprtiac.html

email VARCHAR(100) UNIQUE,
来源：http://hz.zhaomingkeji.xyz/gtyalytauw.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.aibaodan.cn/gtdkeaqcgl.html

);
来源：http://hz.jqgfzy.top/gtbqppntkd.html

[Q02] 创建带外键的表
来源：http://hz.kuanghao11.cn/gtiyylwmzx.html

CREATE TABLE orders (
来源：http://hz.hammf.cn/gthkdsykya.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.cucudq.cn/gthrfumaoe.html

user_id INT NOT NULL,
来源：http://hz.ivvv.top/gtkuhvxqmr.html

amount DECIMAL(10, 2),
来源：http://hz.316326.xyz/gtunfpoyjg.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.yueranfly.top/gtxqyjsgzw.html

);
来源：http://hz.xinyue.icu/gtslvbtwyn.html

[Q03] 增加列
来源：http://hz.gzhubu.top/gtsdjkrnuq.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.yuxming.cn/gtgjqkevqi.html

[Q04] 修改列类型
来源：http://hz.gotoacloud.top/gtenizqfwq.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.cheryme.top/gtbajjxoip.html

[Q05] 重命名列
来源：http://hz.redwolf501.top/gtpuhkbdxk.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.52xcode.cn/gtuuinysht.html

[Q06] 删除列
来源：http://hz.yj20258.top/gtovuvuqgo.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.daria6918.cn/gtqkcqejmd.html

[Q07] 删除表
来源：http://hz.zhixingplan.top/gtkndxztxw.html

DROP TABLE IF EXISTS orders;
来源：http://hz.pycfn.com/gtwjkyqtca.html

[Q08] 创建普通索引
来源：http://hz.cheryme.top/gtttapwxqn.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.pengpengdd.cyou/gtxmeofgul.html

[Q09] 创建唯一索引
来源：http://hz.haohaochexian.top/gtfkdvefvr.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.zhiwuduotai.top/gtozraozpd.html

[Q10] 插入单行
来源：http://hz.yueranfly.top/gtkqdgfhnp.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.jinyuanbaomall.cn/gtgewzpuzd.html

[Q11] 一次插入多行
来源：http://hz.jyoumei.cn/gtyuarubap.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.feifeiyinyue.top/gtyyctcdnf.html

[Q12] 插入后取自增 ID
来源：http://hz.daria6918.cn/gttgqqrhnh.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.zycfv.cn/gtmukvfujm.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.jiagoushi.top/gtqsigpoup.html

[Q13] 忽略重复插入
来源：http://hz.cheryme.top/gtzzvctquy.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.ppjwa.cn/gtldwjtgqn.html

[Q14] 存在则更新（upsert）
来源：http://hz.zhijiandao.cn/gtjdvfrqmj.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.jiagoushi.top/gtizldsxxs.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.ehwqpu.com/gtbdyberww.html

[Q15] 查询全部
来源：http://hz.cdnleiting.top/gtxxathodg.html

SELECT * FROM users;
来源：http://hz.gzhubu.top/gtzfhxqlqd.html

[Q16] 查询指定列
来源：http://hz.iojbl.cn/gtirubbgsc.html

SELECT id, name FROM users;
来源：http://hz.aizwys.cn/gthjvixyft.html

[Q17] 条件查询
来源：http://hz.hammf.cn/gttqgduzik.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.wangshuangyany.cn/gtaftbnjlf.html

[Q18] 模糊匹配
来源：http://hz.tian-w.cn/gtzzwxrnbd.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.fzhhl.top/gtwggcxzvv.html

[Q19] 范围查询
来源：http://hz.52xcode.cn/gtjnagrjkf.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.zhoulong.xyz/gtbskgvzxw.html

[Q20] IN 列表
来源：http://hz.zdqjudy.top/gtjawltytc.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.aizwys.cn/gtukjbzkoo.html

[Q21] 空值判断
来源：http://hz.yongpay.top/gttwvsnixp.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.shuidangran.top/gtcfhajcgs.html

[Q22] 排序
来源：http://hz.zycfv.cn/gtygbfvcof.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.dianchejie.cn/gtrjrdzgup.html

[Q23] 分页
来源：http://hz.pycfn.com/gteddepxym.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.nanxuanxn.top/gtxktwphcp.html

[Q24] 去重
来源：http://hz.yangfankeji.com/gtohkrrxtt.html

SELECT DISTINCT city FROM users;
来源：http://hz.zhongyouzk.top/gtjlvfzhdy.html

[Q25] 只取前 N 条
来源：http://hz.xziqi.cn/gtwjesmmgw.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.9152youxi.cn/gtsykkogrz.html

[Q26] 计数
来源：http://hz.zhijiandao.cn/gtxgnhndeu.html

SELECT COUNT(*) FROM users;
来源：http://hz.c1oappe.top/gtvpvjlqty.html

[Q27] 条件计数
来源：http://hz.zhijiandao.cn/gtgqnraduw.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.hongshengwenyu.top/gtldfrsxaz.html

[Q28] 求和与平均
来源：http://hz.quarkkingdee.top/gtmyjkrnvi.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.aizwys.cn/gtmgeglmjk.html

[Q29] 最大最小值
来源：http://hz.shzxlz.cn/gtdouoxxmm.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.vqdsnc.cn/gtamjjvslh.html

[Q30] 分组统计
来源：http://hz.shzxlz.cn/gtbjjewmsp.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.xziqi.cn/gthdxovoug.html

[Q31] 分组后过滤
来源：http://hz.daxiang520.top/gtokrqaxzo.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.ivvv.top/gttwdheemx.html

[Q32] 分组拼接字符串
来源：http://hz.yonumen.top/gtpzpjtdri.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.guannengcc.top/gtcguinyeh.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.kuanghao11.cn/gtckitcnqf.html

[Q33] 多列分组
来源：http://hz.zycfv.cn/gtoyiarhic.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.svipenyu.cn/gthnouxoir.html

[Q34] 每组取第一条
来源：http://hz.cqqwz.cn/gtcsplhkeq.html

SELECT * FROM (
来源：http://hz.hongshengwenyu.top/gteyvjaxhf.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.jyoumei.cn/gtxuqflpaf.html

) t WHERE rn = 1;
来源：http://hz.feifeiyinyue.top/gtgjbnbapt.html

[Q35] 内连接
来源：http://hz.aizwys.cn/gtaafhhnsb.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.redwolf501.top/gtjiqumbgc.html

[Q36] 左连接
来源：http://hz.ydjk.org.cn/gtkvxxjrqk.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.jlsjyb.cn/gtefhcqbgv.html

[Q37] 右连接
来源：http://hz.feifeiyinyue.top/gtqbnuseyv.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.xylfe.cn/gtjavsgnxg.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.meibo888.top/gtmqbivfod.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.jiagoushi.top/gtpyvjujgi.html

[Q39] 自连接（查上下级）
来源：http://hz.fengsongda.top/gtefjeodjb.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.zhixingplan.top/gtlshawxom.html


<!-- 参考信息 -->