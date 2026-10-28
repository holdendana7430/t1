代发 wailian999

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.hammf.cn/gtdcdwvmrv.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.dianchejie.cn/gtnzpnwakf.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.sxryk.cn/gtejvjmomb.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.hnqzz.top/gtjdadsjpq.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.andypj.xyz/gtbvkzywpo.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.yonumen.top/gtyewzcqwr.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.tianlin.xyz/gtdxzsmmko.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.hnxiangtu.top/gttujqnegm.html

[N05] 最大公约数
来源：http://hz.jinghuilouyu.cn/gtcgwcperr.html

Py:   math.gcd(a, b)
来源：http://hz.9152youxi.cn/gtrtppthyk.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.meibo888.top/gtmleleyok.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.ywan-chungtsiang.top/gtqmetjfav.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.xylfe.cn/gtcwsfeeqf.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.ppjwa.cn/gtbrdzawzy.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.quarkkingdee.top/gtgnxistem.html

Ruby: a.gcd(b)
来源：http://hz.haohaochexian.top/gtebokarsc.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.sysykeji.top/gtuxlpeldj.html

[N06] 判断回文字符串
来源：http://hz.ivvv.top/gtiqeznpwb.html

Py:   s == s[::-1]
来源：http://hz.gzhubu.top/gtdzwvnpqo.html

PHP:  $s === strrev($s);
来源：http://hz.hammf.cn/gtrdaunogg.html

JS:   s === [...s].reverse().join("")
来源：http://hz.xuetiantiany.cn/gtqdvbyloi.html

TS:   s === [...s].reverse().join("")
来源：http://hz.svipenyu.cn/gtjumsixad.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.jiagoushi.top/gttimrmdxa.html

Go:   // 双指针从两端比较
来源：http://hz.guowangkeji.top/gtakzxbqdo.html

Ruby: s == s.reverse
来源：http://hz.xylfe.cn/gtzzomqdtf.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.cheryme.top/gtgttbjade.html

[N07] 两数之和（返回下标）
来源：http://hz.shzxlz.cn/gtqudrayvr.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.ehwqpu.com/gtyxcdxzvw.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.hysaishi.cn/gtazjblmht.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.kuanghao11.cn/gtyxqqzciv.html

TS:   // 手写 Map<string, number>
来源：http://hz.jlsjyb.cn/gtudemejta.html

Java: // 手写 HashMap
来源：http://hz.fzhhl.top/gtqvcfewwi.html

Go:   // 手写 map[int]int
来源：http://hz.daria6918.cn/gtypxgdock.html

Ruby: // 手写 Hash
来源：http://hz.ydzc1.top/gtlyhrwchg.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.xingfuxueyuan.xyz/gtjoqbsagx.html

[N08] 生成全排列
来源：http://hz.shuidangran.top/gtlcfciiqs.html

Py:   itertools.permutations(arr)
来源：http://hz.zhixingplan.top/gtdsxynnah.html

PHP:  // 手写递归交换
来源：http://hz.tian-w.cn/gtjehqudby.html

JS:   // 手写回溯递归
来源：http://hz.nanxinkj.top/gtirpaavya.html

TS:   // 手写回溯递归
来源：http://hz.aizwys.cn/gtmpontank.html

Java: // 手写回溯递归
来源：http://hz.xuanzx.com/gtdlokwyow.html

Go:   // 手写回溯递归
来源：http://hz.nanxuanxn.top/gtyspynaim.html

Ruby: arr.permutation.to_a
来源：http://hz.yj20258888.top/gthlskvqxz.html

C#:   // 手写回溯递归
来源：http://hz.hammf.cn/gtzobekrid.html

[N09] 栈与队列
来源：http://hz.havefunace.top/gtdoxhvgyx.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.jinghuilouyu.cn/gtufahglna.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.xuetiantiany.cn/gtvglocqai.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.zhongyouzk.top/gtyajvnuvj.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.hnxiangtu.top/gtramuanpc.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.yonumen.top/gtyrdfbkik.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.gogol.net.cn/gtcfitetkq.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.ehwqpu.com/gtpnwdvprr.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.havefunace.top/gtswrlprpm.html

[N10] 链表节点定义
来源：http://hz.ydzc1.top/gtlihpdzqd.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.tanke756.top/gtcxqpesph.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.shangyingyoupin.top/gtrwmqlhhn.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.andypj.xyz/gttsngxiiz.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.yanxiufei.cn/gtrhvudwmj.html

Java: class Node { int v; Node next; }
来源：http://hz.dashuyun.cn/gtybzjfsjn.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.zhengqikj.top/gtwbrhddwr.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.cheryme.top/gtgiayogwr.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.zycfv.cn/gthjouxsxa.html

[N11] 二叉树中序遍历
来源：http://hz.zhengqikj.top/gtekwdlksw.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.ehwqpu.com/gtfgyoudnk.html

PHP:  // 手写递归函数
来源：http://hz.yj202588.top/gtksbthtuq.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.yangfankeji.com/gtivixkscl.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.xingfuxueyuan.xyz/gtrvulktkl.html

Java: // 手写递归
来源：http://hz.pengpengdd.cyou/gthznlserf.html

Go:   // 手写递归
来源：http://hz.gaohongyu789.top/gtsuoyrfsi.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.cqqwz.cn/gtsdbbwudo.html

C#:   // 手写递归
来源：http://hz.zhaomingkeji.xyz/gtghplgcjl.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.bjfxy.top/gtvuwzgyok.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.birdmap.top/gtdysacxrn.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.tian-w.cn/gtnvvbqjuz.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.shzxlz.cn/gtnyobznkx.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.gaohongyu789.top/gtzmbmyvhe.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.316326.xyz/gtbrcpzqsy.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.ybcxt.top/gtbjtxjzbc.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.tian-w.cn/gtqxrlcyhs.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.jqgufenzy.top/gtdiglaxyu.html

================================================================================
来源：http://hz.zhengqikj.top/gtnoqbypce.html

O. 并发与异步
来源：http://hz.jianghu66.top/gtntqzhpja.html

================================================================================
来源：http://hz.vqdsnc.cn/gtssrhupwa.html

[O01] 启动一个线程
来源：http://hz.andypj.xyz/gttqskmwsh.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.guannengcc.top/gtwlavctzo.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.yongpay.top/gtsvhflcdx.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.sysykeji.top/gtymuvvlqe.html

TS:   // 同 JS
来源：http://hz.pycfn.com/gtnzgfuwxw.html

Java: new Thread(() -> f()).start()
来源：http://hz.yj202588.top/gtwrthmdlv.html

Go:   go f()
来源：http://hz.316326.xyz/gtecwrwcks.html

Ruby: Thread.new { f }
来源：http://hz.yangfankeji.com/gtybxvhxcv.html

C#:   Task.Run(() => F());
来源：http://hz.iojbl.cn/gtoxkmgmsf.html

[O02] 使用线程池
来源：http://hz.tanke756.top/gtdjkwibrm.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.smart0.xyz/gtdphtumeh.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.jinyuanbaomall.cn/gtgtllxbqi.html

JS:   // worker_threads 线程池
来源：http://hz.shzxlz.cn/gtrlsxraoo.html

TS:   // worker_threads 线程池
来源：http://hz.guannengcc.top/gtljpxmzrp.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.sxryk.cn/gtqwzhnjqp.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.aizwys.cn/gtlxrqljjk.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.gaohongyu789.top/gtennalofh.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.bjfxy.top/gtzjrgirob.html

[O03] 加锁保护共享数据
来源：http://hz.shuidangran.top/gtyzyulvoo.html

Py:   with lock: shared += 1
来源：http://hz.52xcode.cn/gtmlssydvz.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.andypj.xyz/gtvgwpgpec.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.chenjidiqi.icu/gtkkacbjwh.html

TS:   // 同 JS
来源：http://hz.hywenlv.cn/gtljtpbfrn.html

Java: synchronized (this) { shared++; }
来源：http://hz.sxryk.cn/gtxztaftzx.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.svipenyu.cn/gtjgrjpuiu.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.aibaodan.cn/gthqsebtit.html

C#:   lock (gate) { shared++; }
来源：http://hz.52xcode.cn/gtztsjjpcw.html

[O04] 定义异步函数并等待
来源：http://hz.nanxinkj.top/gttoopyfgn.html

Py:   async def f():⏎    await g()
来源：http://hz.guowangkeji.top/gthdrpmptv.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.9152youxi.cn/gtoqsxswxn.html

JS:   async function f() { await g(); }
来源：http://hz.tian-w.cn/gtwtjsrvzz.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.iojbl.cn/gteackfatw.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.ydjk.org.cn/gtjqvotapm.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.yangfankeji.com/gtmqzmwiyt.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.yanxiufei.cn/gtpukirita.html

C#:   async Task F() { await G(); }
来源：http://hz.iojbl.cn/gtvvcgvxih.html

[O05] 并发执行并等待全部完成
来源：http://hz.yongpay.top/gtraalxwbo.html

Py:   asyncio.gather(*tasks)
来源：http://hz.shanyushiyangkeji.top/gtpuuzexob.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.zhoulong.xyz/gtlrifqujn.html

JS:   await Promise.all(tasks)
来源：http://hz.meibo888.top/gtuljlluus.html

TS:   await Promise.all(tasks)
来源：http://hz.birdmap.top/gtzptofxpf.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.316326.xyz/gtogbswbee.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.ydzc1.top/gtkyezwdzn.html

Ruby: threads.map(&:join)
来源：http://hz.xylfe.cn/gtombzbatz.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.gotoacloud.top/gtfxhmxpzl.html

[O06] 使用进程池
来源：http://hz.dashuyun.cn/gticotdoyn.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.vqdsnc.cn/gtsuocmoso.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.smart0.xyz/gtbvjcasry.html

JS:   // child_process / cluster 模块
来源：http://hz.bjfxy.top/gtycgilojb.html

TS:   // child_process / cluster 模块
来源：http://hz.zhoulong.xyz/gtqtwjztyj.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.havefunace.top/gtbwfxqcma.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.pengpengdd.cyou/gtnamydkqq.html

Ruby: // fork 块
来源：http://hz.daxiang520.top/gtnswbdjvx.html

C#:   Parallel.For
来源：http://hz.ydjk.org.cn/gtpqyyoqhy.html

================================================================================
来源：http://hz.hywenlv.cn/gtzemmeydt.html

P. 常用工具函数
来源：http://hz.birdmap.top/gtaxvzezcq.html

================================================================================
来源：http://hz.ehwqpu.com/gtfnwbpyqi.html

[P01] 生成 UUID
来源：http://hz.kuanghao11.cn/gtlrkykptr.html

Py:   str(uuid.uuid4())
来源：http://hz.tianlin.xyz/gtccpnyydi.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.jinghuilouyu.cn/gtxtodrtys.html

JS:   crypto.randomUUID()
来源：http://hz.smart0.xyz/gtjqptfjtq.html

TS:   crypto.randomUUID()
来源：http://hz.hnqzz.top/gtvhmpjmnt.html

Java: UUID.randomUUID().toString()
来源：http://hz.hnxiangtu.top/gtckutlwaz.html

Go:   // 用 github.com/google/uuid
来源：http://hz.0kj1m.cn/gtlnqujysv.html

Ruby: SecureRandom.uuid
来源：http://hz.svipenyu.cn/gtvvcukqse.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.xuetiantiany.cn/gtuymsjucg.html

[P02] MD5 / SHA256 摘要
来源：http://hz.gzhubu.top/gtcwzruijh.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.jqgufenzy.top/gtapaohmzy.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.cheryme.top/gtrjhzmzgf.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.havefunace.top/gtrzfygedx.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.quarkkingdee.top/gtkeyuhazp.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.jqgfzy.top/gtmyjgmxgp.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.chenlongwang.top/gtwvgmgiyy.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.yongpay.top/gtfecvxcgi.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.xinyue.icu/gtxsueypbo.html

[P03] 生成短随机字符串
来源：http://hz.daxiang520.top/gtcarjrfuv.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.jianghu66.top/gtgfoyowlo.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.gotoacloud.top/gtifdljvxn.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.jqgufenzy.top/gtiyjbpjgx.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.xziqi.cn/gtlleeckpw.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.jqgfzy.top/gthubqfzmr.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.jqgufenzy.top/gtbxtwmldz.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.quarkkingdee.top/gtdwkvfymw.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.yj202588.top/gtfvypyaze.html

[P04] 求长度
来源：http://hz.yongpay.top/gtsonbided.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.ivvv.top/gtolxznmqx.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.shanyushiyangtech.top/gthqvznlau.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.ivvv.top/gthbcsydaw.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.yvedp.cn/gtirnuzxvm.html

Java: list.size();  map.size();  s.length()
来源：http://hz.cashguo.top/gtsbmqozrf.html

Go:   len(arr);  len(m)
来源：http://hz.jqgfzy.top/gtgthgzyur.html

Ruby: x.length;  x.size
来源：http://hz.jqgfzy.top/gtzoqaogrh.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.meibo888.top/gtehufhfsj.html

[P05] 判断两个对象内容是否相等
来源：http://hz.sysykeji.top/gtwdmetoto.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.tanke756.top/gtiurvoqim.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.yj20258888.top/gtnzhxziev.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.hywenlv.cn/gtqpiubpaq.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.yuanzhike.top/gtqmdoccpi.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.daxiang520.top/gtnamycjvn.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.hnqzz.top/gtbkjmziou.html

Ruby: a == b
来源：http://hz.ivvv.top/gtnrkvkxxg.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.smart0.xyz/gtsrwdbuoy.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.iojbl.cn/gtksinqemv.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.zhiwuduotai.top/gtwzhvbemq.html

PHP:  if (empty($x)) {}
来源：http://hz.zhiwuduotai.top/gtnimzcgzr.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.zhiwuduotai.top/gtqqodlbpa.html

TS:   if (x == null) {}
来源：http://hz.haohaochexian.top/gttxontcvk.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.nanxuanxn.top/gtiwsosdgx.html

Go:   if x == nil {}
来源：http://hz.wangdashe.top/gtafupylmv.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.jqgfzy.top/gtlwgctsnu.html

C#:   if (x is null) {}
来源：http://hz.haohaochexian.top/gtmaxcadog.html

[P07] 防抖与节流
来源：http://hz.sufxvd.cn/gtnmgfbcdj.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.tian-w.cn/gtdvgbosim.html

PHP:  // 手写时间戳比较
来源：http://hz.smart0.xyz/gtejxonoke.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.hnxiangtu.top/gtlvwzzetl.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.sysykeji.top/gtwuzuypxh.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.0kj1m.cn/gtyjatcgjl.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.yanxiufei.cn/gtjrbfjyhy.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.yongpay.top/gthscapfam.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.52xcode.cn/gtbkszklum.html

[P08] 处理浮点精度问题
来源：http://hz.fengsongda.top/gtucmqcdad.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.yongpay.top/gtiuqzammm.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.jqgfzy.top/gtsgbzwbif.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.yj202588.top/gtrghnulrs.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.chenlongwang.top/gtkhksjlkq.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.svipenyu.cn/gthuiwvpyo.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.zhoulong.xyz/gtohmgegic.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.yonumen.top/gtndwlbail.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.cucudq.cn/gtvccizxyo.html

================================================================================
来源：http://hz.hywenlv.cn/gtmhbihkpg.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.wangdashe.top/gtinobjbfc.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtdbxqnnwt.html

[Q01] 创建表
来源：http://hz.daria6918.cn/gtjdrjxayh.html

CREATE TABLE users (
来源：http://hz.zhaomingkeji.xyz/gttqswkklz.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.haohaochexian.top/gtexryycti.html

name VARCHAR(50) NOT NULL,
来源：http://hz.jinqigufen.top/gtwfnlpmha.html

email VARCHAR(100) UNIQUE,
来源：http://hz.hnxiangtu.top/gtqlswfrgo.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.yj202588.top/gtsfzitxga.html

);
来源：http://hz.snrcjt.cn/gtnczpxcov.html

[Q02] 创建带外键的表
来源：http://hz.ivvv.top/gtpnkdqpuj.html

CREATE TABLE orders (
来源：http://hz.xylfe.cn/gtipfybhck.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.dashuyun.cn/gttzeufnkf.html

user_id INT NOT NULL,
来源：http://hz.gotoacloud.top/gtxmgfmwle.html

amount DECIMAL(10, 2),
来源：http://hz.tanke756.top/gtslfikqhs.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.quarkkingdee.top/gtiddaoylq.html

);
来源：http://hz.guannengcc.top/gtolcwpmxq.html

[Q03] 增加列
来源：http://hz.yuxming.cn/gtasfuuqkq.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.jinqigfzy.top/gtegeucmqy.html

[Q04] 修改列类型
来源：http://hz.ybcxt.top/gtdqsisxej.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.cdnleiting.top/gtzwvkcvog.html

[Q05] 重命名列
来源：http://hz.nanxinkj.top/gtfllpzpvg.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.guannengcc.top/gtgfuqalgv.html

[Q06] 删除列
来源：http://hz.gogol.net.cn/gtstllniok.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.hongshengwenyu.top/gtjqaxqtgq.html

[Q07] 删除表
来源：http://hz.bjfxy.top/gtecmiksrd.html

DROP TABLE IF EXISTS orders;
来源：http://hz.sweek.top/gtbouyrpno.html

[Q08] 创建普通索引
来源：http://hz.xuanzx.com/gtphlwnjrh.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.yj20258888.top/gtlmllxthj.html

[Q09] 创建唯一索引
来源：http://hz.cqqwz.cn/gtemljfopk.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.cashguo.top/gtmxmwtarw.html

[Q10] 插入单行
来源：http://hz.hysaishi.cn/gtlvqryslf.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.cucudq.cn/gtqqkfgtgk.html

[Q11] 一次插入多行
来源：http://hz.snrcjt.cn/gtdfqbdivk.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.guannengcc.top/gtubjjehqx.html

[Q12] 插入后取自增 ID
来源：http://hz.zhaomingkeji.xyz/gtgxlnxqlm.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.mhx1999.top/gtgmlwpaba.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.yuxming.cn/gtpjvfsiqd.html

[Q13] 忽略重复插入
来源：http://hz.shzxlz.cn/gtrujqpaor.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.meibo888.top/gtcdanznyx.html

[Q14] 存在则更新（upsert）
来源：http://hz.52xcode.cn/gtagugrwvq.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.yangfankeji.com/gtpwwjnrlu.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.vqdsnc.cn/gtnwrlrewx.html

[Q15] 查询全部
来源：http://hz.tian-w.cn/gthfuvvkrv.html

SELECT * FROM users;
来源：http://hz.xingfuxueyuan.xyz/gtyiifjtew.html

[Q16] 查询指定列
来源：http://hz.ybcxt.top/gtdbdealwe.html

SELECT id, name FROM users;
来源：http://hz.hongshengwenyu.top/gtlyoglykh.html

[Q17] 条件查询
来源：http://hz.chenlongwang.top/gtbaieqsnl.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.cheryme.top/gtomuctchi.html

[Q18] 模糊匹配
来源：http://hz.ydzc1.top/gtlqylndvm.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.quarkkingdee.top/gtjwnqjgjd.html

[Q19] 范围查询
来源：http://hz.shuidangran.top/gtitrhjngz.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.yj202588.top/gtbqifcicy.html

[Q20] IN 列表
来源：http://hz.ydjk.org.cn/gttfmsqelx.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.tianlin.xyz/gtwylihydh.html

[Q21] 空值判断
来源：http://hz.zhaomingkeji.xyz/gtsgkjiiqf.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.vqdsnc.cn/gtktstwhnf.html

[Q22] 排序
来源：http://hz.quarkkingdee.top/gtclmqaloy.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.shuidangran.top/gtwdsvzwhj.html

[Q23] 分页
来源：http://hz.hysaishi.cn/gtxqgcfkem.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.shanyushiyangtech.top/gtemslicrr.html

[Q24] 去重
来源：http://hz.yangfankeji.com/gtbwwyexgf.html

SELECT DISTINCT city FROM users;
来源：http://hz.jinqigfzy.top/gtmimssrql.html

[Q25] 只取前 N 条
来源：http://hz.snrcjt.cn/gtonvphadb.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.xylfe.cn/gtrfybkljk.html

[Q26] 计数
来源：http://hz.jlsjyb.cn/gtsggoypit.html

SELECT COUNT(*) FROM users;
来源：http://hz.tian-w.cn/gtqedonvut.html

[Q27] 条件计数
来源：http://hz.hysaishi.cn/gthjlvocuo.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.c1oappe.top/gtbkmltzaj.html

[Q28] 求和与平均
来源：http://hz.hnqzz.top/gtyaexnhcx.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.yuxming.cn/gtmoeemfsh.html

[Q29] 最大最小值
来源：http://hz.wangdashe.top/gtvvnpauqz.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.jianghu66.top/gtqqzyisnv.html

[Q30] 分组统计
来源：http://hz.yvedp.cn/gtfbqtjykt.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.nanxinkj.top/gtqrkxrgfj.html

[Q31] 分组后过滤
来源：http://hz.shanyushiyangkeji.top/gthvatonsf.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.gotoacloud.top/gtplhlccmb.html

[Q32] 分组拼接字符串
来源：http://hz.meibo888.top/gtpldscfcj.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.bjfxy.top/gtbjjveeko.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.shanyushiyangkeji.top/gtzvfadivu.html

[Q33] 多列分组
来源：http://hz.kuanghao11.cn/gtwjiwawtl.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.zycfv.cn/gtgnnnurtl.html

[Q34] 每组取第一条
来源：http://hz.shuidangran.top/gtgyamkupd.html

SELECT * FROM (
来源：http://hz.dianchejie.cn/gtssayiqwh.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.jqgfzy.top/gtkzurdntq.html

) t WHERE rn = 1;
来源：http://hz.jinghuilouyu.cn/gtqpfhlkxt.html

[Q35] 内连接
来源：http://hz.yj20258888.top/gtlgrkmiwt.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.zhijiandao.cn/gtdmefkiqs.html


<!-- 参考信息 -->