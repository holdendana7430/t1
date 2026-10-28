代发 wailian999

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.smart0.xyz/gthitxqeob.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.xinyue.icu/gtxiwyfgeg.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.zhoulong.xyz/gtdakgjzal.html

[N04] 斐波那契数列
来源：http://hz.daxiang520.top/gtufpjcxtb.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.xinyue.icu/gtbzieikdg.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.dashuyun.cn/gtwnpwyorx.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.hnqzz.top/gtasuadgit.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.c1oappe.top/gttiipcpqk.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.zdqjudy.top/gtmddqbieu.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.svipenyu.cn/gtztchlbea.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.jlsjyb.cn/gttmeggxpj.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.smart0.xyz/gtyqqadtsj.html

[N05] 最大公约数
来源：http://hz.sweek.top/gtqklhsars.html

Py:   math.gcd(a, b)
来源：http://hz.quarkkingdee.top/gtcnouuabc.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.hammf.cn/gtnffdmsdf.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.hnqzz.top/gtakfvxcxh.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.sysykeji.top/gtbsiwcvrx.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.zhixingplan.top/gtqsctytnx.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.shanyushiyangtech.top/gtsijwkevf.html

Ruby: a.gcd(b)
来源：http://hz.316326.xyz/gtvwndpotq.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.svipenyu.cn/gtiimzcbtp.html

[N06] 判断回文字符串
来源：http://hz.316326.xyz/gthlswoxzs.html

Py:   s == s[::-1]
来源：http://hz.shzxlz.cn/gtgzokuxmw.html

PHP:  $s === strrev($s);
来源：http://hz.aibaodan.cn/gttyhsljgx.html

JS:   s === [...s].reverse().join("")
来源：http://hz.feifeiyinyue.top/gtltaptcpu.html

TS:   s === [...s].reverse().join("")
来源：http://hz.hnxiangtu.top/gtqajoarav.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.sxryk.cn/gtsrtklizm.html

Go:   // 双指针从两端比较
来源：http://hz.hfpthk.cn/gtkhgvpyuk.html

Ruby: s == s.reverse
来源：http://hz.hnxiangtu.top/gtuvcyjckz.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.yvedp.cn/gtsjvacvtk.html

[N07] 两数之和（返回下标）
来源：http://hz.chenzaomai.com/gtnwblzgdg.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.fengsongda.top/gttkjjqijl.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.vqdsnc.cn/gtsizixaqi.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.guannengcc.top/gtidpprwls.html

TS:   // 手写 Map<string, number>
来源：http://hz.cucudq.cn/gtwisbdtrr.html

Java: // 手写 HashMap
来源：http://hz.hfpthk.cn/gtvmbntpyn.html

Go:   // 手写 map[int]int
来源：http://hz.chenlongwang.top/gtrzlnlmzw.html

Ruby: // 手写 Hash
来源：http://hz.daria6918.cn/gtazdnrkxf.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.guowangkeji.top/gtrwpgokyc.html

[N08] 生成全排列
来源：http://hz.shanyushiyangkeji.top/gthypxsado.html

Py:   itertools.permutations(arr)
来源：http://hz.daxiang520.top/gtchxhlwjv.html

PHP:  // 手写递归交换
来源：http://hz.kuanghao11.cn/gtpjktuyod.html

JS:   // 手写回溯递归
来源：http://hz.pengpengdd.cyou/gtoqvcscrj.html

TS:   // 手写回溯递归
来源：http://hz.cashguo.top/gtzodsrqjo.html

Java: // 手写回溯递归
来源：http://hz.hammf.cn/gtjoffmmgt.html

Go:   // 手写回溯递归
来源：http://hz.cqqwz.cn/gtztpumyje.html

Ruby: arr.permutation.to_a
来源：http://hz.ydjk.org.cn/gtjjdwgvuz.html

C#:   // 手写回溯递归
来源：http://hz.9152youxi.cn/gtxcwhyeds.html

[N09] 栈与队列
来源：http://hz.hywenlv.cn/gttezbgpsf.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.ppjwa.cn/gtlywdxtqg.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.ywan-chungtsiang.top/gtzzsnjyuz.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.hnqzz.top/gtwazkcdxh.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.smart0.xyz/gtkpnwsxdh.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.sxryk.cn/gtedouhcuc.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.yvedp.cn/gtquyghheh.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.cqqwz.cn/gtyipwwlie.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.chenzaomai.com/gtjzurkcev.html

[N10] 链表节点定义
来源：http://hz.zhengqikj.top/gtewakdeit.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.hnqzz.top/gtzlutipar.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.shanyushiyangtech.top/gtyzlkqekc.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.ehwqpu.com/gtdyatzkcs.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.yj202588.top/gtldrxmidt.html

Java: class Node { int v; Node next; }
来源：http://hz.yuxming.cn/gtjldtbklg.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.hongshengwenyu.top/gthqvlemws.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.gogol.net.cn/gtugivdfeb.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.wangdashe.top/gtcnwrghzd.html

[N11] 二叉树中序遍历
来源：http://hz.hammf.cn/gtcdtnhamq.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.vqdsnc.cn/gttyspkwew.html

PHP:  // 手写递归函数
来源：http://hz.xingfuxueyuan.xyz/gtarvfymih.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.zhaomingkeji.xyz/gtqctmlzzr.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.chenjidiqi.icu/gtuemcunkb.html

Java: // 手写递归
来源：http://hz.daria6918.cn/gtbxmjnylm.html

Go:   // 手写递归
来源：http://hz.gogol.net.cn/gtmojnpnpx.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.yvedp.cn/gtyzdavbie.html

C#:   // 手写递归
来源：http://hz.jiagoushi.top/gtnegzmomz.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.yuanzhike.top/gtfaroxcfb.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.cdnleiting.top/gtiprebhxs.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.zhijiandao.cn/gtqfwivyus.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.yuxming.cn/gtyvypozwu.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.fengsongda.top/gtcsdpvjua.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.hammf.cn/gtrawbihlj.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.kuanghao11.cn/gtghzryxwl.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.jlsjyb.cn/gtzinqcklq.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.wangshuangyany.cn/gtprlvcgyu.html

================================================================================
来源：http://hz.jinqigufen.top/gtbldahoyl.html

O. 并发与异步
来源：http://hz.vqdsnc.cn/gtcqgsuqlr.html

================================================================================
来源：http://hz.ppjwa.cn/gttutaslve.html

[O01] 启动一个线程
来源：http://hz.sweek.top/gtzucgdica.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.cheryme.top/gtsirptwpn.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.yangfankeji.com/gtxgtvxhtx.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.guowangkeji.top/gtzhuwvabk.html

TS:   // 同 JS
来源：http://hz.dianchejie.cn/gtxlmzzbvj.html

Java: new Thread(() -> f()).start()
来源：http://hz.zhoulong.xyz/gtzxtkmnni.html

Go:   go f()
来源：http://hz.feifeiyinyue.top/gtdtsuitsu.html

Ruby: Thread.new { f }
来源：http://hz.jqgufenzy.top/gtwdnbptwn.html

C#:   Task.Run(() => F());
来源：http://hz.sweek.top/gtyxhoxpme.html

[O02] 使用线程池
来源：http://hz.quarkkingdee.top/gtejsbzgbp.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.jinyuanbaomall.cn/gtjilbbfoy.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.zhaomingkeji.xyz/gtgfcezppa.html

JS:   // worker_threads 线程池
来源：http://hz.nanxuanxn.top/gtzqfbzlca.html

TS:   // worker_threads 线程池
来源：http://hz.tian-w.cn/gttycqqdpw.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.sufxvd.cn/gtjkoywxti.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.pengpengdd.cyou/gtkqjbmvox.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.9152youxi.cn/gttfsotsmb.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.ydzc1.top/gtfdrcezhd.html

[O03] 加锁保护共享数据
来源：http://hz.aibaodan.cn/gtrlnhkzmh.html

Py:   with lock: shared += 1
来源：http://hz.chenzaomai.com/gthvwkkkdz.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.sufxvd.cn/gtvuwkoimq.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.nanxuanxn.top/gtquyovlxp.html

TS:   // 同 JS
来源：http://hz.jinqigfzy.top/gtrowiwahh.html

Java: synchronized (this) { shared++; }
来源：http://hz.guowangkeji.top/gtxfledavi.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.cdnleiting.top/gtwjjpowyz.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.vqdsnc.cn/gtpdvxwuas.html

C#:   lock (gate) { shared++; }
来源：http://hz.xziqi.cn/gtlbfewuwt.html

[O04] 定义异步函数并等待
来源：http://hz.cucudq.cn/gtpcczezgc.html

Py:   async def f():⏎    await g()
来源：http://hz.yonumen.top/gtjidtnfki.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.tianlin.xyz/gtgqacjwms.html

JS:   async function f() { await g(); }
来源：http://hz.shanyushiyangtech.top/gtnoatmuge.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.xuetiantiany.cn/gttblqlsnx.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.yanxiufei.cn/gtziiosulq.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.cashguo.top/gtbljqoiwc.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.xuanzx.com/gtdrsrjcsb.html

C#:   async Task F() { await G(); }
来源：http://hz.tanke756.top/gtxtsjbsyz.html

[O05] 并发执行并等待全部完成
来源：http://hz.yuanzhike.top/gtzmindjbo.html

Py:   asyncio.gather(*tasks)
来源：http://hz.iojbl.cn/gtvhvkxurd.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.zhijiandao.cn/gtkckwvrkq.html

JS:   await Promise.all(tasks)
来源：http://hz.yangfankeji.com/gthlracgux.html

TS:   await Promise.all(tasks)
来源：http://hz.xylfe.cn/gtybslzzgg.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.nwbrower.top/gtksrwpkzg.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.chenjidiqi.icu/gtntfencvj.html

Ruby: threads.map(&:join)
来源：http://hz.chenjidiqi.icu/gtzrzfgnik.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.jyoumei.cn/gtosnuohlh.html

[O06] 使用进程池
来源：http://hz.jinqigufen.top/gthqhkszkx.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.havefunace.top/gtmzwpimfn.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.xuetiantiany.cn/gtdoxlouvx.html

JS:   // child_process / cluster 模块
来源：http://hz.shzxlz.cn/gtmicagste.html

TS:   // child_process / cluster 模块
来源：http://hz.yueranfly.top/gtwlyygoaz.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.gaohongyu789.top/gtuobgmyaf.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.smart0.xyz/gtugnyujgw.html

Ruby: // fork 块
来源：http://hz.yj202588.top/gtrqvzxtoi.html

C#:   Parallel.For
来源：http://hz.mhx1999.top/gtslpqnmgd.html

================================================================================
来源：http://hz.tianlin.xyz/gtklaketmx.html

P. 常用工具函数
来源：http://hz.gaohongyu789.top/gtrtmkldwb.html

================================================================================
来源：http://hz.ydzc1.top/gtxtjxyobf.html

[P01] 生成 UUID
来源：http://hz.nwbrower.top/gtdpucekkb.html

Py:   str(uuid.uuid4())
来源：http://hz.yj20258888.top/gtenqgtqmw.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.daria6918.cn/gtvoxgzoov.html

JS:   crypto.randomUUID()
来源：http://hz.hywenlv.cn/gtigaewhrv.html

TS:   crypto.randomUUID()
来源：http://hz.sysykeji.top/gtwrtatbtx.html

Java: UUID.randomUUID().toString()
来源：http://hz.yuanzhike.top/gtdanxeqhb.html

Go:   // 用 github.com/google/uuid
来源：http://hz.fzhhl.top/gtjjydumsf.html

Ruby: SecureRandom.uuid
来源：http://hz.redwolf501.top/gteehpafjh.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.yj20258888.top/gtomnbrwcd.html

[P02] MD5 / SHA256 摘要
来源：http://hz.vqdsnc.cn/gtejubhbgz.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.wangshuangyany.cn/gtsxblbjiu.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.svipenyu.cn/gthkwiqqir.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.svipenyu.cn/gtdfbmzntf.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.svipenyu.cn/gtpncvkrgg.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.xuanzx.com/gtwxbmtcvs.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.guannengcc.top/gtpnlcyceq.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.fzhhl.top/gtvmbnztrp.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.chenjidiqi.icu/gtjumvwkil.html

[P03] 生成短随机字符串
来源：http://hz.cheryme.top/gtxitiquav.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.zhoulong.xyz/gtpjfbesgr.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.hnxiangtu.top/gtyorhopdh.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.yuanzhike.top/gtyxpakuxi.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.yuxming.cn/gtidsjfvge.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.gzhubu.top/gtzljscygw.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.gotoacloud.top/gtajjxpyux.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.iojbl.cn/gtjxmpldfh.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.tianlin.xyz/gtgdbwzhal.html

[P04] 求长度
来源：http://hz.ydjk.org.cn/gtagjtrvhl.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.smart0.xyz/gtxgfnllgm.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.vqdsnc.cn/gtveimxtbz.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.daxiang520.top/gtrauivher.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.jiagoushi.top/gtaehvqogy.html

Java: list.size();  map.size();  s.length()
来源：http://hz.hongshengwenyu.top/gtcpaeraio.html

Go:   len(arr);  len(m)
来源：http://hz.jyoumei.cn/gtnabsxdht.html

Ruby: x.length;  x.size
来源：http://hz.52xcode.cn/gtomrferkv.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.zhoulong.xyz/gtwrlqhzfv.html

[P05] 判断两个对象内容是否相等
来源：http://hz.zhiwuduotai.top/gtiogazscm.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.guowangkeji.top/gtndvvwvrc.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.9152youxi.cn/gtgxkexwvb.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.ivvv.top/gtnkuawqan.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.jinqigufen.top/gtatgjzjgo.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.zhijiandao.cn/gtnuxdjwly.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.c1oappe.top/gtoemhrhfd.html

Ruby: a == b
来源：http://hz.bjfxy.top/gtnptnscqq.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.hammf.cn/gtgxygafat.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.ywan-chungtsiang.top/gtewjxclje.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.nanxinkj.top/gtbzqoekpz.html

PHP:  if (empty($x)) {}
来源：http://hz.fzhhl.top/gtksiwzufe.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.ehwqpu.com/gtpqwsprvj.html

TS:   if (x == null) {}
来源：http://hz.wangdashe.top/gtwqljdhpk.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.yuanzhike.top/gtuzcgevwb.html

Go:   if x == nil {}
来源：http://hz.aizwys.cn/gtfdzecxad.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.316326.xyz/gtmngtmzfp.html

C#:   if (x is null) {}
来源：http://hz.ywan-chungtsiang.top/gtvafxtfve.html

[P07] 防抖与节流
来源：http://hz.shuidangran.top/gtyhbubdbk.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.daxiang520.top/gttqktmauv.html

PHP:  // 手写时间戳比较
来源：http://hz.zhaomingkeji.xyz/gtzrpcgkjw.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.sxryk.cn/gtmnudastu.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.ehwqpu.com/gtnyvlzxso.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.sxryk.cn/gtewmhpwgs.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.hnqzz.top/gtysetzccz.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.fzhhl.top/gtjkhsnpvy.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.sysykeji.top/gtmhhgqbxn.html

[P08] 处理浮点精度问题
来源：http://hz.redwolf501.top/gtabbklacj.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.gotoacloud.top/gteqengcom.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.daxiang520.top/gtvptxpzlm.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.shangyingyoupin.top/gtvrpgxglv.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.hysaishi.cn/gttuomvpok.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.ehwqpu.com/gtafvktulf.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.shanyushiyangtech.top/gtrcqknaik.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.jinyuanbaomall.cn/gtkgiylgcg.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.cdnleiting.top/gtdqdcfowe.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtqgkaeata.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.xylfe.cn/gtoerlgxzf.html

================================================================================
来源：http://hz.feifeiyinyue.top/gthcpalkwi.html

[Q01] 创建表
来源：http://hz.jinqigufen.top/gtdjfamjli.html

CREATE TABLE users (
来源：http://hz.gaohongyu789.top/gttqwzcenu.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.sufxvd.cn/gtoqnorcml.html

name VARCHAR(50) NOT NULL,
来源：http://hz.jqgufenzy.top/gteaevyxzx.html

email VARCHAR(100) UNIQUE,
来源：http://hz.sufxvd.cn/gtmqnbnxnx.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.aizwys.cn/gtcivgfusy.html

);
来源：http://hz.birdmap.top/gtnpvgajpg.html

[Q02] 创建带外键的表
来源：http://hz.jiagoushi.top/gtryaxzztb.html

CREATE TABLE orders (
来源：http://hz.yangfankeji.com/gtkpwrhyai.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.316326.xyz/gtupspudet.html

user_id INT NOT NULL,
来源：http://hz.nanxinkj.top/gtzrbuqxdt.html

amount DECIMAL(10, 2),
来源：http://hz.ivvv.top/gtbtauazgq.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.yonumen.top/gtrerfxvuq.html

);
来源：http://hz.yongpay.top/gtfqxuvifq.html

[Q03] 增加列
来源：http://hz.yangfankeji.com/gtrpfjjznj.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.jiagoushi.top/gtbtnrktqk.html

[Q04] 修改列类型
来源：http://hz.xuetiantiany.cn/gtanvvoleu.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.yueranfly.top/gtahwjuvyl.html

[Q05] 重命名列
来源：http://hz.hnxiangtu.top/gtwzsxcsgt.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.fzhhl.top/gthomsufiu.html

[Q06] 删除列
来源：http://hz.c1oappe.top/gtgwaprcat.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.wangshuangyany.cn/gtlillnprl.html

[Q07] 删除表
来源：http://hz.shzxlz.cn/gtwecpafqh.html

DROP TABLE IF EXISTS orders;
来源：http://hz.haohaochexian.top/gtuwbkzlly.html

[Q08] 创建普通索引
来源：http://hz.yuxming.cn/gtnailhwds.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.jqgufenzy.top/gtxrwucmsi.html

[Q09] 创建唯一索引
来源：http://hz.yj202588.top/gtzokimqay.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.nanxinkj.top/gtpmwmcmgk.html

[Q10] 插入单行
来源：http://hz.yuanzhike.top/gtwftwopux.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.jinqigufen.top/gtuuvoejeh.html

[Q11] 一次插入多行
来源：http://hz.shuidangran.top/gtyrckjqld.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.aizwys.cn/gthullxawr.html

[Q12] 插入后取自增 ID
来源：http://hz.c1oappe.top/gtmnpafmay.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.sweek.top/gtobgdvppe.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.jinqigufen.top/gtcnhxuxdn.html

[Q13] 忽略重复插入
来源：http://hz.jinqigufen.top/gtyczutvzn.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.sweek.top/gtdtktglsn.html

[Q14] 存在则更新（upsert）
来源：http://hz.shanyushiyangtech.top/gtuxyrvwqa.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.sufxvd.cn/gtubugeyfv.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.jianghu66.top/gtkhjsdxcn.html

[Q15] 查询全部
来源：http://hz.hongshengwenyu.top/gtxxbpvinm.html

SELECT * FROM users;
来源：http://hz.havefunace.top/gtcyguvyuw.html

[Q16] 查询指定列
来源：http://hz.redwolf501.top/gtjheidcjy.html

SELECT id, name FROM users;
来源：http://hz.vqdsnc.cn/gtgnfqouuh.html

[Q17] 条件查询
来源：http://hz.vqdsnc.cn/gttpywdfsi.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.andypj.xyz/gtsbtyfkny.html

[Q18] 模糊匹配
来源：http://hz.aibaodan.cn/gtynvuqrzr.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.guowangkeji.top/gtexaxrhsg.html

[Q19] 范围查询
来源：http://hz.cdnleiting.top/gtrxrcouyo.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.feifeiyinyue.top/gtvecfidre.html

[Q20] IN 列表
来源：http://hz.shangyingyoupin.top/gttudrarff.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.tianlin.xyz/gtpvisjwjb.html

[Q21] 空值判断
来源：http://hz.nanxinkj.top/gtknsbjgls.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.redwolf501.top/gtajtgasgi.html

[Q22] 排序
来源：http://hz.zycfv.cn/gtxzrenanb.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.pengpengdd.cyou/gtzcmnxkvl.html

[Q23] 分页
来源：http://hz.chenlongwang.top/gtmjsfreub.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.jianghu66.top/gtfayzdweq.html

[Q24] 去重
来源：http://hz.meibo888.top/gtbhbwngqq.html

SELECT DISTINCT city FROM users;
来源：http://hz.hnqzz.top/gtysvvqcym.html

[Q25] 只取前 N 条
来源：http://hz.jinghuilouyu.cn/gttcifcxbq.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.ywan-chungtsiang.top/gtldkjhoul.html

[Q26] 计数
来源：http://hz.smart0.xyz/gtkkqxdagc.html

SELECT COUNT(*) FROM users;
来源：http://hz.hywenlv.cn/gtpdsrxmbx.html

[Q27] 条件计数
来源：http://hz.zdqjudy.top/gtussbuhrm.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.zhaomingkeji.xyz/gtlxewwcsm.html

[Q28] 求和与平均
来源：http://hz.jlsjyb.cn/gtanmdpnus.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.pycfn.com/gtdutvuika.html

[Q29] 最大最小值
来源：http://hz.sufxvd.cn/gttyjeqrcj.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.yongpay.top/gtrufegzyi.html

[Q30] 分组统计
来源：http://hz.tian-w.cn/gtcegqfqsk.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.yangfankeji.com/gtqefcgurp.html

[Q31] 分组后过滤
来源：http://hz.dashuyun.cn/gtkixykqmx.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.jinghuilouyu.cn/gthxepqefm.html

[Q32] 分组拼接字符串
来源：http://hz.gaohongyu789.top/gtxcslsbgx.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.xylfe.cn/gtwmvjucjh.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.bjfxy.top/gtnxcosyrg.html

[Q33] 多列分组
来源：http://hz.dashuyun.cn/gtnvwsxsyc.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.52xcode.cn/gttgbexcfk.html

[Q34] 每组取第一条
来源：http://hz.daxiang520.top/gtafnduqwu.html

SELECT * FROM (
来源：http://hz.jiagoushi.top/gtltgqlnas.html


<!-- 参考信息 -->