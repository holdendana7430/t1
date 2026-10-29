代发 wailian999

[N05] 最大公约数
来源：http://www.m.share.fehbvm.com/Article/details/gappehgzu.sHtML

Py:   math.gcd(a, b)
来源：http://blog.fehbvm.com/Article/details/ganamrkcu.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.hesvh.cn/Article/details/gwnxfcdez.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.zdbjq.cn/Article/details/gklhgvmog.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.fehbvm.com/Article/details/gpvlrwabo.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://read.share.zdbjq.cn/Article/details/gojijpkbe.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://baike.hesvh.cn/Article/details/gcidtpwsf.sHtML

Ruby: a.gcd(b)
来源：http://blog.fehbvm.com/Article/details/gfxwfagem.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mobile.zdbjq.cn/Article/details/gcvpycutl.sHtML

[N06] 判断回文字符串
来源：http://m.share.fehbvm.com/Article/details/gfgiiaehu.sHtML

Py:   s == s[::-1]
来源：http://blog.fehbvm.com/Article/details/gpukyxffa.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.zdbjq.cn/Article/details/gyomlnhzm.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.zdbjq.cn/Article/details/gcgcypucd.sHtML

TS:   s === [...s].reverse().join("")
来源：http://baike.zdbjq.cn/Article/details/gqqnrhrqq.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.blog.hesvh.cn/Article/details/gtodxbjyp.sHtML

Go:   // 双指针从两端比较
来源：http://mobile.hesvh.cn/Article/details/gxuluezmr.sHtML

Ruby: s == s.reverse
来源：http://3g.fehbvm.com/Article/details/gedhoejxz.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.m.share.zdbjq.cn/Article/details/gqgplvghs.sHtML

[N07] 两数之和（返回下标）
来源：http://m.share.fehbvm.com/Article/details/gbtnqnijh.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://baike.zdbjq.cn/Article/details/ganvxpjqf.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wap.hesvh.cn/Article/details/gjdcvlaxq.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.share.zdbjq.cn/Article/details/gfrfvrctz.sHtML

TS:   // 手写 Map<string, number>
来源：http://baike.hesvh.cn/Article/details/gngdnszfl.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.hesvh.cn/Article/details/gjikxeist.sHtML

Go:   // 手写 map[int]int
来源：http://m.share.fehbvm.com/Article/details/gwotuqhiq.sHtML

Ruby: // 手写 Hash
来源：http://mobile.zdbjq.cn/Article/details/gpqlyarea.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.zdbjq.cn/Article/details/gkwcmfsfq.sHtML

[N08] 生成全排列
来源：http://www.m.share.hesvh.cn/Article/details/gyxboltfj.sHtML

Py:   itertools.permutations(arr)
来源：http://read.share.zdbjq.cn/Article/details/ggyjmtqjd.sHtML

PHP:  // 手写递归交换
来源：http://www.share.fehbvm.com/Article/details/gayolfesr.sHtML

JS:   // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/geoblyngc.sHtML

TS:   // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/gthlkgdun.sHtML

Java: // 手写回溯递归
来源：http://read.share.hesvh.cn/Article/details/gjybpkutt.sHtML

Go:   // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/grrhbwiyl.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.hesvh.cn/Article/details/gpmysxyib.sHtML

C#:   // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/gqwlcosfa.sHtML

[N09] 栈与队列
来源：http://blog.fehbvm.com/Article/details/gwtxtdcvm.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.fehbvm.com/Article/details/gwckvdkhi.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.zdbjq.cn/Article/details/gresknbfu.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://baike.zdbjq.cn/Article/details/gggpxdwqp.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://baike.hesvh.cn/Article/details/gsbhsgkpl.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://3g.zdbjq.cn/Article/details/gttwpcafa.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mobile.fehbvm.com/Article/details/gzdyhsroc.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mobile.fehbvm.com/Article/details/glzhiuvqw.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://3g.fehbvm.com/Article/details/gxmvnxtmt.sHtML

[N10] 链表节点定义
来源：http://m.share.zdbjq.cn/Article/details/gsyxxrhzv.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.zdbjq.cn/Article/details/gnoqtrepe.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.fehbvm.com/Article/details/galphtlko.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mobile.zdbjq.cn/Article/details/gpczheciv.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wap.zdbjq.cn/Article/details/gdgrkzjvg.sHtML

Java: class Node { int v; Node next; }
来源：http://m.share.hesvh.cn/Article/details/gdlxxxliz.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://m.share.fehbvm.com/Article/details/gwdvaxbtw.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.hesvh.cn/Article/details/gggiguipn.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://mobile.zdbjq.cn/Article/details/gnwsqtcou.sHtML

[N11] 二叉树中序遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gtuukpxgm.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.zdbjq.cn/Article/details/gxuubzahb.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.hesvh.cn/Article/details/gnkofjqug.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.zdbjq.cn/Article/details/gbnuhdbfg.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.fehbvm.com/Article/details/glextksat.sHtML

Java: // 手写递归
来源：http://blog.hesvh.cn/Article/details/gbdcgphlr.sHtML

Go:   // 手写递归
来源：http://3g.fehbvm.com/Article/details/gemzqhzco.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.m.share.hesvh.cn/Article/details/gktpwceku.sHtML

C#:   // 手写递归
来源：http://baike.zdbjq.cn/Article/details/gytmdjftp.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.share.zdbjq.cn/Article/details/geuljvggs.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blog.fehbvm.com/Article/details/gibazsclk.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://m.share.zdbjq.cn/Article/details/gojkithpy.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.zdbjq.cn/Article/details/gxelmqkna.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.zdbjq.cn/Article/details/guljneflk.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.fehbvm.com/Article/details/grckbdasc.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mobile.zdbjq.cn/Article/details/guzpemuok.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://baike.hesvh.cn/Article/details/gthxllwif.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.hesvh.cn/Article/details/gtxnrcczg.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gksdjezqi.sHtML

O. 并发与异步
来源：http://read.share.fehbvm.com/Article/details/gytlgazbh.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/glnyedfvv.sHtML

[O01] 启动一个线程
来源：http://read.share.zdbjq.cn/Article/details/gthdibayh.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wap.zdbjq.cn/Article/details/gvodtuzdn.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mobile.fehbvm.com/Article/details/givyddnbo.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://m.share.hesvh.cn/Article/details/gemgvttut.sHtML

TS:   // 同 JS
来源：http://www.share.hesvh.cn/Article/details/gaplrewzx.sHtML

Java: new Thread(() -> f()).start()
来源：http://wap.hesvh.cn/Article/details/gteerlpeo.sHtML

Go:   go f()
来源：http://read.share.fehbvm.com/Article/details/grsivhtuf.sHtML

Ruby: Thread.new { f }
来源：http://www.blog.hesvh.cn/Article/details/gzogldpou.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.hesvh.cn/Article/details/gowzcvjao.sHtML

[O02] 使用线程池
来源：http://www.blog.zdbjq.cn/Article/details/gzoqwethy.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://3g.hesvh.cn/Article/details/gxzwuiezs.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.zdbjq.cn/Article/details/gyabroars.sHtML

JS:   // worker_threads 线程池
来源：http://read.share.hesvh.cn/Article/details/ggeawlelu.sHtML

TS:   // worker_threads 线程池
来源：http://m.share.zdbjq.cn/Article/details/gleixlxiu.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://m.share.hesvh.cn/Article/details/grcmkzvxy.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://3g.hesvh.cn/Article/details/ggetzqqbd.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.m.share.hesvh.cn/Article/details/glrwwfbja.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://read.share.fehbvm.com/Article/details/guqkaddxa.sHtML

[O03] 加锁保护共享数据
来源：http://wap.hesvh.cn/Article/details/gxofojugx.sHtML

Py:   with lock: shared += 1
来源：http://blog.hesvh.cn/Article/details/gxgrjuymz.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.share.hesvh.cn/Article/details/gfohknuem.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://3g.zdbjq.cn/Article/details/grvydlpte.sHtML

TS:   // 同 JS
来源：http://read.share.hesvh.cn/Article/details/grfzrkbyb.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.blog.hesvh.cn/Article/details/gewyodvrl.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.zdbjq.cn/Article/details/grlxyswnv.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://wap.hesvh.cn/Article/details/gpisijyig.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.hesvh.cn/Article/details/gxqbunzdk.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.fehbvm.com/Article/details/goghyrbsl.sHtML

Py:   async def f():⏎    await g()
来源：http://read.share.zdbjq.cn/Article/details/gufvsraws.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://3g.hesvh.cn/Article/details/gevnrrglh.sHtML

JS:   async function f() { await g(); }
来源：http://blog.hesvh.cn/Article/details/gtthsheks.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://mobile.hesvh.cn/Article/details/gwymrntuw.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.zdbjq.cn/Article/details/gmrjfyhtx.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mobile.fehbvm.com/Article/details/gcgbvjlon.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.zdbjq.cn/Article/details/gxktlrgtc.sHtML

C#:   async Task F() { await G(); }
来源：http://m.share.hesvh.cn/Article/details/gxzwqovlo.sHtML

[O05] 并发执行并等待全部完成
来源：http://mobile.hesvh.cn/Article/details/goqhxsnee.sHtML

Py:   asyncio.gather(*tasks)
来源：http://blog.fehbvm.com/Article/details/gpusgyctp.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.m.share.fehbvm.com/Article/details/gyugxesbg.sHtML

JS:   await Promise.all(tasks)
来源：http://mobile.hesvh.cn/Article/details/gscduxjfz.sHtML

TS:   await Promise.all(tasks)
来源：http://3g.fehbvm.com/Article/details/gauyfdcgd.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.m.share.hesvh.cn/Article/details/gxkiwtyrf.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wap.hesvh.cn/Article/details/glhvysumn.sHtML

Ruby: threads.map(&:join)
来源：http://m.share.hesvh.cn/Article/details/geerwpsgs.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://3g.hesvh.cn/Article/details/gtkxvungk.sHtML

[O06] 使用进程池
来源：http://www.blog.hesvh.cn/Article/details/gcccotdin.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.m.share.zdbjq.cn/Article/details/goskaekgy.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://wap.fehbvm.com/Article/details/godcinzww.sHtML

JS:   // child_process / cluster 模块
来源：http://wap.zdbjq.cn/Article/details/gwtkcfvaa.sHtML

TS:   // child_process / cluster 模块
来源：http://read.share.fehbvm.com/Article/details/gxzptazsp.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.fehbvm.com/Article/details/gclzahomi.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://baike.zdbjq.cn/Article/details/gzvqimtit.sHtML

Ruby: // fork 块
来源：http://blog.zdbjq.cn/Article/details/gluutfomu.sHtML

C#:   Parallel.For
来源：http://baike.fehbvm.com/Article/details/gevxutwuv.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gecwaleak.sHtML

P. 常用工具函数
来源：http://mobile.hesvh.cn/Article/details/ghucsevja.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gsqujdydq.sHtML

[P01] 生成 UUID
来源：http://baike.hesvh.cn/Article/details/genhppkvn.sHtML

Py:   str(uuid.uuid4())
来源：http://read.share.fehbvm.com/Article/details/giqctfjuv.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wap.zdbjq.cn/Article/details/gmuccysxn.sHtML

JS:   crypto.randomUUID()
来源：http://blog.hesvh.cn/Article/details/gbsgrgmfr.sHtML

TS:   crypto.randomUUID()
来源：http://3g.fehbvm.com/Article/details/gxbebfxof.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.share.fehbvm.com/Article/details/gjymiqmjv.sHtML

Go:   // 用 github.com/google/uuid
来源：http://blog.fehbvm.com/Article/details/gytzmtzxq.sHtML

Ruby: SecureRandom.uuid
来源：http://read.share.hesvh.cn/Article/details/guazczvol.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.blog.hesvh.cn/Article/details/gqlycrwgf.sHtML

[P02] MD5 / SHA256 摘要
来源：http://m.share.fehbvm.com/Article/details/gbhilbqpk.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wap.zdbjq.cn/Article/details/ghhzznsno.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://mobile.fehbvm.com/Article/details/gfiixkoil.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.m.share.fehbvm.com/Article/details/gcuaorprc.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.hesvh.cn/Article/details/gdzescokh.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://baike.hesvh.cn/Article/details/gorhylxdd.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://blog.zdbjq.cn/Article/details/gesunwyde.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://m.share.zdbjq.cn/Article/details/gaiwgblnf.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://3g.fehbvm.com/Article/details/gmpfcourz.sHtML

[P03] 生成短随机字符串
来源：http://read.share.hesvh.cn/Article/details/givejwvyb.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mobile.hesvh.cn/Article/details/gvtdxwpkt.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mobile.zdbjq.cn/Article/details/gsihxsnfx.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.zdbjq.cn/Article/details/gxotbjgqo.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.fehbvm.com/Article/details/gyzbjoajo.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mobile.hesvh.cn/Article/details/gdbxghshq.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mobile.hesvh.cn/Article/details/gwsmbhhvh.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://3g.fehbvm.com/Article/details/gdvchogpr.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.m.share.hesvh.cn/Article/details/gwdrhitbw.sHtML

[P04] 求长度
来源：http://read.share.zdbjq.cn/Article/details/glracijxs.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://m.share.fehbvm.com/Article/details/gezxhagoi.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.fehbvm.com/Article/details/ghybimxvb.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.hesvh.cn/Article/details/gubmyzimg.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.hesvh.cn/Article/details/gpczxxdea.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.share.hesvh.cn/Article/details/glwvdirte.sHtML

Go:   len(arr);  len(m)
来源：http://mobile.fehbvm.com/Article/details/gjiewwvql.sHtML

Ruby: x.length;  x.size
来源：http://mobile.zdbjq.cn/Article/details/gmklqkuwi.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://3g.zdbjq.cn/Article/details/gaoatzhpo.sHtML

[P05] 判断两个对象内容是否相等
来源：http://wap.fehbvm.com/Article/details/gxzesxtlk.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.m.share.zdbjq.cn/Article/details/gwqnrnqis.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.m.share.zdbjq.cn/Article/details/gzbbevetl.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://baike.zdbjq.cn/Article/details/gzfgxcjem.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.zdbjq.cn/Article/details/gdbucopjt.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.blog.fehbvm.com/Article/details/gnugacmau.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.fehbvm.com/Article/details/godesvuas.sHtML

Ruby: a == b
来源：http://baike.hesvh.cn/Article/details/gddwpgisn.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://3g.hesvh.cn/Article/details/grferlidj.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://3g.hesvh.cn/Article/details/gnirmteno.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://m.share.zdbjq.cn/Article/details/grslhcyte.sHtML

PHP:  if (empty($x)) {}
来源：http://www.share.hesvh.cn/Article/details/gjoulpfxo.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wap.zdbjq.cn/Article/details/gcmnhpatb.sHtML

TS:   if (x == null) {}
来源：http://www.m.share.fehbvm.com/Article/details/gpknieuey.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://3g.fehbvm.com/Article/details/gwshmtlur.sHtML

Go:   if x == nil {}
来源：http://read.share.fehbvm.com/Article/details/gvxuhajem.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.m.share.hesvh.cn/Article/details/galbijmew.sHtML

C#:   if (x is null) {}
来源：http://m.share.fehbvm.com/Article/details/gwegoozyt.sHtML

[P07] 防抖与节流
来源：http://baike.zdbjq.cn/Article/details/gzimrjors.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.share.fehbvm.com/Article/details/grwfgsxwv.sHtML

PHP:  // 手写时间戳比较
来源：http://blog.zdbjq.cn/Article/details/ggbvmgwob.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.zdbjq.cn/Article/details/gagarxqqc.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.fehbvm.com/Article/details/gwialkktv.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://blog.zdbjq.cn/Article/details/gmdtldbiz.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.share.fehbvm.com/Article/details/grzgafjym.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.share.zdbjq.cn/Article/details/gxvhemdif.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.share.hesvh.cn/Article/details/gffrjjyfp.sHtML

[P08] 处理浮点精度问题
来源：http://mobile.fehbvm.com/Article/details/gioyuvhzk.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://3g.hesvh.cn/Article/details/gcafuaakq.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://read.share.zdbjq.cn/Article/details/gelkmfhro.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://read.share.hesvh.cn/Article/details/gtmvfvusx.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.m.share.zdbjq.cn/Article/details/gtpcyrpgz.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.blog.fehbvm.com/Article/details/gteasopyh.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://read.share.fehbvm.com/Article/details/gibbsuxek.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://baike.zdbjq.cn/Article/details/gpkiiphdx.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://m.share.fehbvm.com/Article/details/gdzzcksmu.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gqiowwnmc.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.share.hesvh.cn/Article/details/gkoncsfnb.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gegabbdeh.sHtML

[Q01] 创建表
来源：http://read.share.fehbvm.com/Article/details/gpogjzhil.sHtML

CREATE TABLE users (
来源：http://mobile.zdbjq.cn/Article/details/gdtuogvlf.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.fehbvm.com/Article/details/gnbvtjofq.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.blog.hesvh.cn/Article/details/gxtezcsph.sHtML

email VARCHAR(100) UNIQUE,
来源：http://mobile.hesvh.cn/Article/details/grwugoach.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.blog.hesvh.cn/Article/details/gnxeyywxh.sHtML

);
来源：http://www.m.share.zdbjq.cn/Article/details/gnxxlwjgn.sHtML

[Q02] 创建带外键的表
来源：http://baike.zdbjq.cn/Article/details/gvngxflwt.sHtML

CREATE TABLE orders (
来源：http://3g.hesvh.cn/Article/details/gmndljfob.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.hesvh.cn/Article/details/gtnapvdjq.sHtML

user_id INT NOT NULL,
来源：http://mobile.fehbvm.com/Article/details/gqydwplll.sHtML

amount DECIMAL(10, 2),
来源：http://www.blog.hesvh.cn/Article/details/gvjqkckri.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wap.hesvh.cn/Article/details/grmsrikoc.sHtML

);
来源：http://www.blog.hesvh.cn/Article/details/gnboqkgpy.sHtML

[Q03] 增加列
来源：http://www.share.zdbjq.cn/Article/details/glpmosczg.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://3g.zdbjq.cn/Article/details/gcvrhanzb.sHtML

[Q04] 修改列类型
来源：http://wap.hesvh.cn/Article/details/gqwefhzbg.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.share.zdbjq.cn/Article/details/gctuvcawe.sHtML

[Q05] 重命名列
来源：http://www.share.hesvh.cn/Article/details/gmojqpscw.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.blog.fehbvm.com/Article/details/ggfvkyuko.sHtML

[Q06] 删除列
来源：http://www.share.hesvh.cn/Article/details/gwmhykqga.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.share.fehbvm.com/Article/details/gctamdgpf.sHtML

[Q07] 删除表
来源：http://blog.zdbjq.cn/Article/details/gkjceawrl.sHtML

DROP TABLE IF EXISTS orders;
来源：http://read.share.fehbvm.com/Article/details/gzovdvexb.sHtML

[Q08] 创建普通索引
来源：http://mobile.zdbjq.cn/Article/details/grkntwaiu.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://wap.fehbvm.com/Article/details/gyqfnzonx.sHtML

[Q09] 创建唯一索引
来源：http://mobile.fehbvm.com/Article/details/gfstndqpn.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://3g.fehbvm.com/Article/details/gthoytrfh.sHtML

[Q10] 插入单行
来源：http://www.blog.fehbvm.com/Article/details/gufmfaumr.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mobile.zdbjq.cn/Article/details/gwdwlkdct.sHtML

[Q11] 一次插入多行
来源：http://read.share.hesvh.cn/Article/details/gyvufzxyd.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.fehbvm.com/Article/details/gywsvfifa.sHtML

[Q12] 插入后取自增 ID
来源：http://www.share.fehbvm.com/Article/details/ghszqnzit.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.share.zdbjq.cn/Article/details/gbxjekvte.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mobile.hesvh.cn/Article/details/gfixyuock.sHtML

[Q13] 忽略重复插入
来源：http://www.blog.zdbjq.cn/Article/details/gvdekkcmh.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mobile.hesvh.cn/Article/details/gaxzelsix.sHtML

[Q14] 存在则更新（upsert）
来源：http://baike.fehbvm.com/Article/details/gokwesfks.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baike.hesvh.cn/Article/details/gprgovevr.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://m.share.hesvh.cn/Article/details/gwyserwyp.sHtML

[Q15] 查询全部
来源：http://3g.zdbjq.cn/Article/details/gvlweeazm.sHtML

SELECT * FROM users;
来源：http://wap.hesvh.cn/Article/details/gxhjtpgsm.sHtML

[Q16] 查询指定列
来源：http://wap.zdbjq.cn/Article/details/gtiijdmyt.sHtML

SELECT id, name FROM users;
来源：http://www.share.hesvh.cn/Article/details/gdssxbnlo.sHtML

[Q17] 条件查询
来源：http://www.m.share.fehbvm.com/Article/details/geucaoumn.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mobile.fehbvm.com/Article/details/gzspugcmi.sHtML

[Q18] 模糊匹配
来源：http://3g.zdbjq.cn/Article/details/gmydvxpbz.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wap.fehbvm.com/Article/details/gpufvrzms.sHtML

[Q19] 范围查询
来源：http://read.share.fehbvm.com/Article/details/gjrivrwoq.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wap.fehbvm.com/Article/details/ginpssfuj.sHtML

[Q20] IN 列表
来源：http://m.share.fehbvm.com/Article/details/gawgcccpc.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.zdbjq.cn/Article/details/gvuqsjbfe.sHtML

[Q21] 空值判断
来源：http://m.share.hesvh.cn/Article/details/gbbbjkcrk.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://m.share.hesvh.cn/Article/details/gkwoskogy.sHtML

[Q22] 排序
来源：http://3g.fehbvm.com/Article/details/goukupqwm.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.blog.hesvh.cn/Article/details/gibcvvlth.sHtML

[Q23] 分页
来源：http://m.share.hesvh.cn/Article/details/gingxoswc.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://m.share.zdbjq.cn/Article/details/gbdfcrgvj.sHtML

[Q24] 去重
来源：http://www.blog.fehbvm.com/Article/details/ghyurtbby.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gxbuucdxc.sHtML

[Q25] 只取前 N 条
来源：http://3g.fehbvm.com/Article/details/gbhqkndzi.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://baike.fehbvm.com/Article/details/gxqpkwosr.sHtML

[Q26] 计数
来源：http://wap.fehbvm.com/Article/details/gjpevqivt.sHtML

SELECT COUNT(*) FROM users;
来源：http://m.share.hesvh.cn/Article/details/gejpvxrpd.sHtML

[Q27] 条件计数
来源：http://www.m.share.zdbjq.cn/Article/details/gagnidrgv.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gzwzyepht.sHtML

[Q28] 求和与平均
来源：http://m.share.fehbvm.com/Article/details/gsylvxlsq.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gmfhmnbsh.sHtML

[Q29] 最大最小值
来源：http://www.share.hesvh.cn/Article/details/gdcqnnuib.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gkeszputb.sHtML

[Q30] 分组统计
来源：http://m.share.zdbjq.cn/Article/details/gvyddnjtn.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.fehbvm.com/Article/details/gdllglfcc.sHtML

[Q31] 分组后过滤
来源：http://m.share.zdbjq.cn/Article/details/gnzysdjii.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.m.share.hesvh.cn/Article/details/gzzwoahgm.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.hesvh.cn/Article/details/gyghaizqh.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://baike.hesvh.cn/Article/details/gpkwwecal.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://blog.fehbvm.com/Article/details/gindkxnra.sHtML

[Q33] 多列分组
来源：http://m.share.zdbjq.cn/Article/details/goljtyskn.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.zdbjq.cn/Article/details/gsltsaybo.sHtML

[Q34] 每组取第一条
来源：http://wap.hesvh.cn/Article/details/gvamfpcga.sHtML

SELECT * FROM (
来源：http://www.m.share.zdbjq.cn/Article/details/gcpwlkewu.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.blog.hesvh.cn/Article/details/gwpbieuhz.sHtML

) t WHERE rn = 1;
来源：http://m.share.hesvh.cn/Article/details/gifnmyyjs.sHtML

[Q35] 内连接
来源：http://m.share.zdbjq.cn/Article/details/gsumfsyad.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.zdbjq.cn/Article/details/gtomchpqf.sHtML

[Q36] 左连接
来源：http://www.blog.fehbvm.com/Article/details/gjzyrfwly.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.fehbvm.com/Article/details/gtpceiysw.sHtML

[Q37] 右连接
来源：http://read.share.fehbvm.com/Article/details/gicngfxlc.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://baike.hesvh.cn/Article/details/gnriwmtpv.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://baike.fehbvm.com/Article/details/gilseagtq.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wap.hesvh.cn/Article/details/gepmpqfhq.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.fehbvm.com/Article/details/glhkitxfh.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.m.share.zdbjq.cn/Article/details/gpyicenfr.sHtML


<!-- 参考信息 -->