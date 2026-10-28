代发 wailian999

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.fzhhl.top/gtlrvycvqg.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.xuetiantiany.cn/gtepheaeut.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.hfpthk.cn/gtsipknius.html

[N04] 斐波那契数列
来源：http://hz.guannengcc.top/gtkhphxzgp.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.feifeiyinyue.top/gtbcnfrhiu.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.tanke756.top/gtyrmijkue.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.yj20258888.top/gtrxdzzbxv.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.snrcjt.cn/gtodkwlafs.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.zdqjudy.top/gtildgfmkq.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.zhengqikj.top/gttksfkohe.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.sweek.top/gtfmqigrts.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.ppjwa.cn/gtlmmxnwsr.html

[N05] 最大公约数
来源：http://hz.ybcxt.top/gtokezdhow.html

Py:   math.gcd(a, b)
来源：http://hz.hywenlv.cn/gtevqnmtjq.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.hnqzz.top/gtcsinksqw.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.hongshengwenyu.top/gtpritivda.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.zhengqikj.top/gtipxwosuj.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.vqdsnc.cn/gttsbtzuvv.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.ivvv.top/gtkmpslepb.html

Ruby: a.gcd(b)
来源：http://hz.wangshuangyany.cn/gtjhwsifbw.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.jinqigfzy.top/gtzhrfsosu.html

[N06] 判断回文字符串
来源：http://hz.hnxiangtu.top/gtsswunzjt.html

Py:   s == s[::-1]
来源：http://hz.gotoacloud.top/gtileekcnp.html

PHP:  $s === strrev($s);
来源：http://hz.jqgfzy.top/gtndswtudc.html

JS:   s === [...s].reverse().join("")
来源：http://hz.fzhhl.top/gtilgvwndm.html

TS:   s === [...s].reverse().join("")
来源：http://hz.gotoacloud.top/gtzjuxugug.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.jyoumei.cn/gtlegnwvrc.html

Go:   // 双指针从两端比较
来源：http://hz.daria6918.cn/gtupzdansa.html

Ruby: s == s.reverse
来源：http://hz.gaohongyu789.top/gtlmpabiup.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.hnqzz.top/gtstaoqwqy.html

[N07] 两数之和（返回下标）
来源：http://hz.cqqwz.cn/gtpapidika.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.ywan-chungtsiang.top/gtpitaxbfc.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.jiagoushi.top/gtkfkcstep.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.316326.xyz/gtuwutfpaf.html

TS:   // 手写 Map<string, number>
来源：http://hz.dashuyun.cn/gtrszxbvru.html

Java: // 手写 HashMap
来源：http://hz.hysaishi.cn/gtleepwnhc.html

Go:   // 手写 map[int]int
来源：http://hz.zhixingplan.top/gtokpjbwzs.html

Ruby: // 手写 Hash
来源：http://hz.yvedp.cn/gtqkpccvei.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.hysaishi.cn/gttmfpxqug.html

[N08] 生成全排列
来源：http://hz.fengsongda.top/gtswmiutcv.html

Py:   itertools.permutations(arr)
来源：http://hz.shangyingyoupin.top/gtslzanlte.html

PHP:  // 手写递归交换
来源：http://hz.xuetiantiany.cn/gtnpwxzecy.html

JS:   // 手写回溯递归
来源：http://hz.gotoacloud.top/gtozyaxdkm.html

TS:   // 手写回溯递归
来源：http://hz.yongpay.top/gtyrcmdsad.html

Java: // 手写回溯递归
来源：http://hz.sufxvd.cn/gtcujvvwny.html

Go:   // 手写回溯递归
来源：http://hz.ydjk.org.cn/gtbxfakyzp.html

Ruby: arr.permutation.to_a
来源：http://hz.zhaomingkeji.xyz/gthexaspjh.html

C#:   // 手写回溯递归
来源：http://hz.ybcxt.top/gtdubfkupt.html

[N09] 栈与队列
来源：http://hz.316326.xyz/gtmspwufoa.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.cashguo.top/gtyplrfhiy.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.jinghuilouyu.cn/gtyjqxqcty.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.haohaochexian.top/gtsbywaast.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.ydjk.org.cn/gtvzebiiqo.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.yvedp.cn/gtjksuzaqx.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.hnxiangtu.top/gtttxnxziv.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.fzhhl.top/gtanbcgugm.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.dianchejie.cn/gtwmkeswyl.html

[N10] 链表节点定义
来源：http://hz.ywan-chungtsiang.top/gtqljveyoc.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.guowangkeji.top/gtqqghbywi.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.redwolf501.top/gtoftgllhg.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.ivvv.top/gtdfswnoiv.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.ydzc1.top/gtrxtuivlh.html

Java: class Node { int v; Node next; }
来源：http://hz.c1oappe.top/gtygsyuxzr.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.birdmap.top/gtuptbrvml.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.hywenlv.cn/gtmlozggjp.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.jinqigufen.top/gtwfdcigvj.html

[N11] 二叉树中序遍历
来源：http://hz.jinqigfzy.top/gtgoghvrun.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.wangdashe.top/gtcgcrcjyn.html

PHP:  // 手写递归函数
来源：http://hz.bjfxy.top/gtzjrtidrd.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.feifeiyinyue.top/gtcqojnxyt.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.sxryk.cn/gtmerrmsrn.html

Java: // 手写递归
来源：http://hz.guannengcc.top/gtsnoelemx.html

Go:   // 手写递归
来源：http://hz.wangshuangyany.cn/gtdepmeszv.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.aizwys.cn/gtjvhuefze.html

C#:   // 手写递归
来源：http://hz.daxiang520.top/gtdpkziaov.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.yj20258888.top/gtngxxecbz.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.fengsongda.top/gtjcumrruz.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.shanyushiyangkeji.top/gtktbpuqec.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.shanyushiyangkeji.top/gtvnfxgplu.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.jqgfzy.top/gtcnxxoziu.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.jqgufenzy.top/gtjdpfzdhs.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.aibaodan.cn/gtssvvunpv.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.quarkkingdee.top/gtezexmlop.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.sxryk.cn/gtcztcxkas.html

================================================================================
来源：http://hz.ppjwa.cn/gteujpfbfx.html

O. 并发与异步
来源：http://hz.cqqwz.cn/gtlixazsdj.html

================================================================================
来源：http://hz.nanxinkj.top/gtrqcdkrcm.html

[O01] 启动一个线程
来源：http://hz.daria6918.cn/gtvxduycsx.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.gotoacloud.top/gtlrjxhqpy.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.fzhhl.top/gtboffvuin.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.zhoulong.xyz/gtbwondusz.html

TS:   // 同 JS
来源：http://hz.ywan-chungtsiang.top/gttwvgaqpc.html

Java: new Thread(() -> f()).start()
来源：http://hz.wangshuangyany.cn/gtupjxeluk.html

Go:   go f()
来源：http://hz.ybcxt.top/gtqmrkuvuu.html

Ruby: Thread.new { f }
来源：http://hz.daxiang520.top/gtczmwrzee.html

C#:   Task.Run(() => F());
来源：http://hz.birdmap.top/gtbmgbbxst.html

[O02] 使用线程池
来源：http://hz.jyoumei.cn/gtaspbuazk.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.smart0.xyz/gtajimhemi.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.shangyingyoupin.top/gtlsbufgaz.html

JS:   // worker_threads 线程池
来源：http://hz.yonumen.top/gtzwclghil.html

TS:   // worker_threads 线程池
来源：http://hz.zdqjudy.top/gthawppnpj.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.birdmap.top/gtmhtkqecf.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.ydjk.org.cn/gtidcjwvnd.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.xingfuxueyuan.xyz/gtnfzszkwu.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.hfpthk.cn/gtiodunwyd.html

[O03] 加锁保护共享数据
来源：http://hz.ivvv.top/gtjphopilw.html

Py:   with lock: shared += 1
来源：http://hz.fengsongda.top/gtssiepzlk.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.ydjk.org.cn/gtrhgbcxtn.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.aizwys.cn/gtavatacex.html

TS:   // 同 JS
来源：http://hz.gotoacloud.top/gtgpprenif.html

Java: synchronized (this) { shared++; }
来源：http://hz.chenlongwang.top/gtqnbxtfuv.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.sweek.top/gtvxrlqnyp.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.ehwqpu.com/gtlknkscdm.html

C#:   lock (gate) { shared++; }
来源：http://hz.yj20258.top/gtnvrnecew.html

[O04] 定义异步函数并等待
来源：http://hz.mhx1999.top/gteiufpgej.html

Py:   async def f():⏎    await g()
来源：http://hz.daxiang520.top/gttecabhjp.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.shangyingyoupin.top/gtisywxtve.html

JS:   async function f() { await g(); }
来源：http://hz.xylfe.cn/gtdyfaltcq.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.zhaomingkeji.xyz/gtnwfcrfnv.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.shangyingyoupin.top/gtkmbvtdlf.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.havefunace.top/gtakxtgtxb.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.yongpay.top/gtekxzthbu.html

C#:   async Task F() { await G(); }
来源：http://hz.yuxming.cn/gtjxsccneq.html

[O05] 并发执行并等待全部完成
来源：http://hz.gaohongyu789.top/gtcvgqhftf.html

Py:   asyncio.gather(*tasks)
来源：http://hz.ivvv.top/gtjldhzfxr.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.yuxming.cn/gtxyqcabbz.html

JS:   await Promise.all(tasks)
来源：http://hz.yvedp.cn/gtnzacmtej.html

TS:   await Promise.all(tasks)
来源：http://hz.yanxiufei.cn/gtzizhgieq.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.xuanzx.com/gtidneugke.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.cashguo.top/gtlwrdjstz.html

Ruby: threads.map(&:join)
来源：http://hz.chenzaomai.com/gtzulvxryq.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.zhixingplan.top/gtnjjddvqa.html

[O06] 使用进程池
来源：http://hz.chenzaomai.com/gtftprqnsw.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.wangdashe.top/gtdnfyhivk.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.xinyue.icu/gtjfpqrxkl.html

JS:   // child_process / cluster 模块
来源：http://hz.tianlin.xyz/gtucrqvtqw.html

TS:   // child_process / cluster 模块
来源：http://hz.gotoacloud.top/gtjobtypix.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.smart0.xyz/gtbnzheyxk.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.yanxiufei.cn/gthdlgjpqr.html

Ruby: // fork 块
来源：http://hz.zhiwuduotai.top/gtvkroowog.html

C#:   Parallel.For
来源：http://hz.zhoulong.xyz/gthhtbtpqh.html

================================================================================
来源：http://hz.shzxlz.cn/gtwwgsqibr.html

P. 常用工具函数
来源：http://hz.0kj1m.cn/gtyfaplnrt.html

================================================================================
来源：http://hz.sweek.top/gtsrnyvxqt.html

[P01] 生成 UUID
来源：http://hz.ybcxt.top/gtqgundows.html

Py:   str(uuid.uuid4())
来源：http://hz.xylfe.cn/gtfhqrofux.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.sxryk.cn/gtovbtywch.html

JS:   crypto.randomUUID()
来源：http://hz.fengsongda.top/gtcobdtiwu.html

TS:   crypto.randomUUID()
来源：http://hz.gotoacloud.top/gtkbetefvr.html

Java: UUID.randomUUID().toString()
来源：http://hz.yanxiufei.cn/gtsokviixo.html

Go:   // 用 github.com/google/uuid
来源：http://hz.zhongyouzk.top/gtuaiemlxj.html

Ruby: SecureRandom.uuid
来源：http://hz.jlsjyb.cn/gtzvqnyloh.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.ydjk.org.cn/gtsamuapzu.html

[P02] MD5 / SHA256 摘要
来源：http://hz.shanyushiyangtech.top/gtvsucigig.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.yongpay.top/gtqkvifftp.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.shanyushiyangtech.top/gtpzfvzwln.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.wangshuangyany.cn/gtzkjuakbt.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.yj20258.top/gtofwgdffm.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.ehwqpu.com/gtjhtjehse.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.gotoacloud.top/gtosrsgulq.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.yj20258888.top/gtourqjcfq.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.jinqigfzy.top/gtlsqhsipr.html

[P03] 生成短随机字符串
来源：http://hz.havefunace.top/gtzuxywgex.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.cucudq.cn/gtreoobhou.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.daxiang520.top/gtuvmutqxs.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.haohaochexian.top/gtfndfthqf.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.yvedp.cn/gtkycugnxw.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.mhx1999.top/gtfpvhzkdd.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.jiagoushi.top/gtedqyudgq.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.yongpay.top/gtxmixonhr.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.guannengcc.top/gtcasyojyk.html

[P04] 求长度
来源：http://hz.shanyushiyangkeji.top/gtnxulnlhh.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.tianlin.xyz/gtoxeztuze.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.xingfuxueyuan.xyz/gtuglbqksz.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.yj20258888.top/gtnlydjpwg.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.yanxiufei.cn/gtlpvsfzqo.html

Java: list.size();  map.size();  s.length()
来源：http://hz.aizwys.cn/gtjmnjgufe.html

Go:   len(arr);  len(m)
来源：http://hz.xinyue.icu/gtixrgcgby.html

Ruby: x.length;  x.size
来源：http://hz.andypj.xyz/gteqpjfnqv.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.jiagoushi.top/gtiphdsphw.html

[P05] 判断两个对象内容是否相等
来源：http://hz.zhiwuduotai.top/gtseqttyun.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.jinqigfzy.top/gtiwdlchld.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.pycfn.com/gtwemflkuu.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.yanxiufei.cn/gtprumkivo.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.yonumen.top/gtafyangoo.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.tianlin.xyz/gtlvffeods.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.yonumen.top/gtqzbtlvgt.html

Ruby: a == b
来源：http://hz.xuanzx.com/gtyrdkettk.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.zhixingplan.top/gtaudirxhd.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.fzhhl.top/gtbgsmwzto.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.sufxvd.cn/gttnapjllf.html

PHP:  if (empty($x)) {}
来源：http://hz.jqgfzy.top/gtysxzapzz.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.0kj1m.cn/gtodqgbiwa.html

TS:   if (x == null) {}
来源：http://hz.dianchejie.cn/gtvpooxuto.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.tian-w.cn/gtlnwgdkba.html

Go:   if x == nil {}
来源：http://hz.daria6918.cn/gtneswhrjg.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.chenjidiqi.icu/gttpdlxljx.html

C#:   if (x is null) {}
来源：http://hz.cucudq.cn/gtrxfvnqlj.html

[P07] 防抖与节流
来源：http://hz.cheryme.top/gthzhxjnbm.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.jiagoushi.top/gtzeifymyx.html

PHP:  // 手写时间戳比较
来源：http://hz.havefunace.top/gtquzqbtof.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.gogol.net.cn/gtvnprpyaf.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.wangdashe.top/gtabunhbze.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.aibaodan.cn/gtwcwlgcak.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.yj202588.top/gtxlcypcrg.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.fzhhl.top/gtfzpkjlit.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.daria6918.cn/gtyrpsiqua.html

[P08] 处理浮点精度问题
来源：http://hz.shuidangran.top/gtioknzevu.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.jqgfzy.top/gtxeikvcil.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.zhiwuduotai.top/gtqxghlizo.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.316326.xyz/gtzgvzaokq.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.fengsongda.top/gtvyarpvbj.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.andypj.xyz/gtewslebhr.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.shanyushiyangtech.top/gtclztkiyu.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.meibo888.top/gtptjswjar.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.hnqzz.top/gtoxcigprp.html

================================================================================
来源：http://hz.yangfankeji.com/gtjkeyglfn.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.jiagoushi.top/gttgqjivsw.html

================================================================================
来源：http://hz.xylfe.cn/gtytvnjjzm.html

[Q01] 创建表
来源：http://hz.tianlin.xyz/gtddxgzzbg.html

CREATE TABLE users (
来源：http://hz.yangfankeji.com/gtajvepyrr.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.yj20258888.top/gttsbyrsbf.html

name VARCHAR(50) NOT NULL,
来源：http://hz.cqqwz.cn/gtjkgxiqwn.html

email VARCHAR(100) UNIQUE,
来源：http://hz.yangfankeji.com/gtkcwqceuq.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.meibo888.top/gtrepvkkko.html

);
来源：http://hz.daria6918.cn/gtbytiemcn.html

[Q02] 创建带外键的表
来源：http://hz.zhengqikj.top/gtryhsbgsu.html

CREATE TABLE orders (
来源：http://hz.sweek.top/gttpfvavcs.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.hysaishi.cn/gtohkypjps.html

user_id INT NOT NULL,
来源：http://hz.mhx1999.top/gtqazjgoja.html

amount DECIMAL(10, 2),
来源：http://hz.gotoacloud.top/gtkdhthyqv.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.hywenlv.cn/gtydqlwbcx.html

);
来源：http://hz.smart0.xyz/gtppbxsrqa.html

[Q03] 增加列
来源：http://hz.hywenlv.cn/gtvgzwbfrr.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.dianchejie.cn/gtbihqbhxd.html

[Q04] 修改列类型
来源：http://hz.jiagoushi.top/gtivkhcswt.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.chenzaomai.com/gtwvvddmeg.html

[Q05] 重命名列
来源：http://hz.yongpay.top/gtqbxqenmb.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.yj20258888.top/gtygihpzew.html

[Q06] 删除列
来源：http://hz.wangshuangyany.cn/gtxxgbaclr.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.sweek.top/gtteuqrcjo.html

[Q07] 删除表
来源：http://hz.zhengqikj.top/gtpsbwcubm.html

DROP TABLE IF EXISTS orders;
来源：http://hz.sxryk.cn/gtsgwrmmec.html

[Q08] 创建普通索引
来源：http://hz.zdqjudy.top/gtvymubidh.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.sxryk.cn/gtcaecdspk.html

[Q09] 创建唯一索引
来源：http://hz.yanxiufei.cn/gtertnhqaq.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.0kj1m.cn/gtswbqobgk.html

[Q10] 插入单行
来源：http://hz.gzhubu.top/gtfqwffcci.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.tian-w.cn/gtnjlevgrc.html

[Q11] 一次插入多行
来源：http://hz.cqqwz.cn/gtucbthsec.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.ydzc1.top/gtugggknit.html

[Q12] 插入后取自增 ID
来源：http://hz.vqdsnc.cn/gthsfkkrvq.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.xuetiantiany.cn/gttnmjuowz.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.birdmap.top/gtbugacpil.html

[Q13] 忽略重复插入
来源：http://hz.xingfuxueyuan.xyz/gtrvrnneyu.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.kuanghao11.cn/gtzbqpaqku.html

[Q14] 存在则更新（upsert）
来源：http://hz.sufxvd.cn/gtuzuawbbt.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.cqqwz.cn/gtgeepuopk.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.haohaochexian.top/gtlqhmbhog.html

[Q15] 查询全部
来源：http://hz.vqdsnc.cn/gthvintzll.html

SELECT * FROM users;
来源：http://hz.jinghuilouyu.cn/gtfbffojgh.html

[Q16] 查询指定列
来源：http://hz.jqgfzy.top/gtobkhaskh.html

SELECT id, name FROM users;
来源：http://hz.tanke756.top/gtctjxlxkb.html

[Q17] 条件查询
来源：http://hz.zycfv.cn/gtjhougaua.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.quarkkingdee.top/gtxggqqfqk.html

[Q18] 模糊匹配
来源：http://hz.xingfuxueyuan.xyz/gtweknsbwb.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.hnqzz.top/gthjamvnao.html

[Q19] 范围查询
来源：http://hz.sweek.top/gthurolsdz.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.jyoumei.cn/gthbxtmadg.html

[Q20] IN 列表
来源：http://hz.tanke756.top/gtatxfsfyx.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.ppjwa.cn/gtdatijtdn.html

[Q21] 空值判断
来源：http://hz.ywan-chungtsiang.top/gtjqhttymi.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.zdqjudy.top/gtjsgwzxmm.html

[Q22] 排序
来源：http://hz.cucudq.cn/gtmzwzeaef.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.ivvv.top/gtigjfasrf.html

[Q23] 分页
来源：http://hz.gotoacloud.top/gtpazikyio.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.sxryk.cn/gttkijfthw.html

[Q24] 去重
来源：http://hz.daxiang520.top/gtesdhceuy.html

SELECT DISTINCT city FROM users;
来源：http://hz.cheryme.top/gttimlngxe.html

[Q25] 只取前 N 条
来源：http://hz.svipenyu.cn/gtlrtwtrrt.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.xinyue.icu/gtbfbhccjm.html

[Q26] 计数
来源：http://hz.ivvv.top/gtusiodtgb.html

SELECT COUNT(*) FROM users;
来源：http://hz.xuanzx.com/gtlljvauwh.html

[Q27] 条件计数
来源：http://hz.tanke756.top/gtpolfflkz.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.sufxvd.cn/gtlxsxcrrt.html

[Q28] 求和与平均
来源：http://hz.yj20258888.top/gtsdywhkpo.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.xylfe.cn/gtmazmursa.html

[Q29] 最大最小值
来源：http://hz.chenjidiqi.icu/gthlyyobax.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.feifeiyinyue.top/gtpwjwxohc.html

[Q30] 分组统计
来源：http://hz.hammf.cn/gtpvnfjckf.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.snrcjt.cn/gtwfeputpi.html

[Q31] 分组后过滤
来源：http://hz.xinyue.icu/gtinmpcytb.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.jyoumei.cn/gtfmnlzspe.html

[Q32] 分组拼接字符串
来源：http://hz.xuanzx.com/gtdxksbthn.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.kuanghao11.cn/gtpkldydjm.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.ppjwa.cn/gtnwcsfsxa.html

[Q33] 多列分组
来源：http://hz.sweek.top/gtaoowbwet.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.jinghuilouyu.cn/gtfpuxzyem.html

[Q34] 每组取第一条
来源：http://hz.shuidangran.top/gtjhkjmzff.html

SELECT * FROM (
来源：http://hz.zhixingplan.top/gtrwhoryhq.html


<!-- 参考信息 -->