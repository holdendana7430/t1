代发 wailian999

[N05] 最大公约数
来源：http://read.share.zdbjq.cn/Article/details/gfiqygfaz.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.fehbvm.com/Article/details/gimoxmncc.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://baike.hesvh.cn/Article/details/gtlhsaido.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.zdbjq.cn/Article/details/gypjbmeot.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.zdbjq.cn/Article/details/gysxwptdv.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wap.hesvh.cn/Article/details/gycnhdbzr.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mobile.fehbvm.com/Article/details/gushznzoh.sHtML

Ruby: a.gcd(b)
来源：http://blog.fehbvm.com/Article/details/gmxmfpssf.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wap.zdbjq.cn/Article/details/glsyzwfhv.sHtML

[N06] 判断回文字符串
来源：http://3g.hesvh.cn/Article/details/gwaamniwf.sHtML

Py:   s == s[::-1]
来源：http://m.share.fehbvm.com/Article/details/gofxwvnfe.sHtML

PHP:  $s === strrev($s);
来源：http://wap.hesvh.cn/Article/details/grdrzkgox.sHtML

JS:   s === [...s].reverse().join("")
来源：http://m.share.fehbvm.com/Article/details/gtwixrmyp.sHtML

TS:   s === [...s].reverse().join("")
来源：http://3g.fehbvm.com/Article/details/gxuewrwry.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.blog.fehbvm.com/Article/details/gblxrvyiv.sHtML

Go:   // 双指针从两端比较
来源：http://3g.fehbvm.com/Article/details/gapcaufzv.sHtML

Ruby: s == s.reverse
来源：http://www.blog.hesvh.cn/Article/details/gfdiihbdf.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.zdbjq.cn/Article/details/ggwloztls.sHtML

[N07] 两数之和（返回下标）
来源：http://read.share.fehbvm.com/Article/details/gwziacfnf.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.share.fehbvm.com/Article/details/goolhzaii.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mobile.zdbjq.cn/Article/details/ghzbhlnzx.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://baike.hesvh.cn/Article/details/gypfdojgb.sHtML

TS:   // 手写 Map<string, number>
来源：http://m.share.zdbjq.cn/Article/details/gqaqbyiig.sHtML

Java: // 手写 HashMap
来源：http://blog.zdbjq.cn/Article/details/gojuaqgdx.sHtML

Go:   // 手写 map[int]int
来源：http://baike.zdbjq.cn/Article/details/ggrcjyyum.sHtML

Ruby: // 手写 Hash
来源：http://wap.zdbjq.cn/Article/details/gjzssgkqv.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://blog.hesvh.cn/Article/details/gjmmdrmcb.sHtML

[N08] 生成全排列
来源：http://baike.fehbvm.com/Article/details/grhdjqblo.sHtML

Py:   itertools.permutations(arr)
来源：http://3g.hesvh.cn/Article/details/ggsgvszit.sHtML

PHP:  // 手写递归交换
来源：http://baike.fehbvm.com/Article/details/gensjlbhz.sHtML

JS:   // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/gvfemejmt.sHtML

TS:   // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/grvbhqiqa.sHtML

Java: // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/gaxgzfqrz.sHtML

Go:   // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/gbwxtglzo.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.fehbvm.com/Article/details/gqqohtwnx.sHtML

C#:   // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/ganfiwfoj.sHtML

[N09] 栈与队列
来源：http://mobile.hesvh.cn/Article/details/gjyghsvzl.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.hesvh.cn/Article/details/gujsxcoxo.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://baike.zdbjq.cn/Article/details/gttvtghbx.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://baike.fehbvm.com/Article/details/gnmpjbzfx.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://baike.hesvh.cn/Article/details/gjhqtuqrc.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.share.hesvh.cn/Article/details/gyezangud.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wap.hesvh.cn/Article/details/golbfsnmj.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.zdbjq.cn/Article/details/gqzjnfdox.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.fehbvm.com/Article/details/gigrbuknu.sHtML

[N10] 链表节点定义
来源：http://3g.fehbvm.com/Article/details/gykvhgzqn.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.blog.fehbvm.com/Article/details/gdqiyfgvz.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://baike.hesvh.cn/Article/details/grvilgqhg.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.blog.zdbjq.cn/Article/details/gzwxcnvvp.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://m.share.zdbjq.cn/Article/details/gykbgqhak.sHtML

Java: class Node { int v; Node next; }
来源：http://www.share.fehbvm.com/Article/details/gkfoozkdk.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://m.share.fehbvm.com/Article/details/goyangwod.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.zdbjq.cn/Article/details/gnqqtenpv.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://mobile.zdbjq.cn/Article/details/gispqmiub.sHtML

[N11] 二叉树中序遍历
来源：http://read.share.fehbvm.com/Article/details/gfrfkpbnn.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.m.share.zdbjq.cn/Article/details/grvuolshz.sHtML

PHP:  // 手写递归函数
来源：http://www.blog.hesvh.cn/Article/details/gbvubpzlh.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.hesvh.cn/Article/details/gfzaryfnq.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.hesvh.cn/Article/details/gagxpvvpq.sHtML

Java: // 手写递归
来源：http://www.blog.zdbjq.cn/Article/details/gumerevrx.sHtML

Go:   // 手写递归
来源：http://blog.zdbjq.cn/Article/details/gxfafinpl.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.zdbjq.cn/Article/details/gzdotovmq.sHtML

C#:   // 手写递归
来源：http://blog.fehbvm.com/Article/details/guyaqolil.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://baike.hesvh.cn/Article/details/gbnaptpbm.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.m.share.fehbvm.com/Article/details/gsjtkysgh.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.zdbjq.cn/Article/details/gzollgdew.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.fehbvm.com/Article/details/gnkuftjfn.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.fehbvm.com/Article/details/gfgwczzzb.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.zdbjq.cn/Article/details/gnhidvpxp.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://read.share.fehbvm.com/Article/details/gqgnayger.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.share.zdbjq.cn/Article/details/gxnxlhuri.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.hesvh.cn/Article/details/gqlfatbui.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gcswgrktc.sHtML

O. 并发与异步
来源：http://baike.fehbvm.com/Article/details/gujakohdu.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gvhhaixdx.sHtML

[O01] 启动一个线程
来源：http://www.m.share.hesvh.cn/Article/details/gwmojsdvy.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mobile.hesvh.cn/Article/details/gbcskzpre.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wap.hesvh.cn/Article/details/ghlaawtuw.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.zdbjq.cn/Article/details/grqnrdkhs.sHtML

TS:   // 同 JS
来源：http://www.m.share.zdbjq.cn/Article/details/gcnbchdvq.sHtML

Java: new Thread(() -> f()).start()
来源：http://baike.zdbjq.cn/Article/details/gxahuhdva.sHtML

Go:   go f()
来源：http://wap.fehbvm.com/Article/details/gbzihsprx.sHtML

Ruby: Thread.new { f }
来源：http://www.share.fehbvm.com/Article/details/gjeszzqdx.sHtML

C#:   Task.Run(() => F());
来源：http://baike.zdbjq.cn/Article/details/gjfdsxpoo.sHtML

[O02] 使用线程池
来源：http://baike.zdbjq.cn/Article/details/gbmwgbfms.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://m.share.hesvh.cn/Article/details/gxxaqgggl.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://m.share.fehbvm.com/Article/details/gnavoaczu.sHtML

JS:   // worker_threads 线程池
来源：http://blog.fehbvm.com/Article/details/gwrcwjsyv.sHtML

TS:   // worker_threads 线程池
来源：http://3g.zdbjq.cn/Article/details/gipwyelth.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.hesvh.cn/Article/details/gcqtedsxe.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://3g.fehbvm.com/Article/details/gagcdofqe.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.blog.hesvh.cn/Article/details/grlmvjbua.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.share.zdbjq.cn/Article/details/gxviuqdtx.sHtML

[O03] 加锁保护共享数据
来源：http://m.share.hesvh.cn/Article/details/grdhkphpn.sHtML

Py:   with lock: shared += 1
来源：http://www.share.fehbvm.com/Article/details/glckncgjz.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.blog.zdbjq.cn/Article/details/gectaqmvo.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.share.hesvh.cn/Article/details/gbdwbcaky.sHtML

TS:   // 同 JS
来源：http://read.share.hesvh.cn/Article/details/gmdqycswz.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.m.share.hesvh.cn/Article/details/gaqemqbba.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://3g.zdbjq.cn/Article/details/gyicztarg.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://read.share.zdbjq.cn/Article/details/gpankxxqi.sHtML

C#:   lock (gate) { shared++; }
来源：http://m.share.fehbvm.com/Article/details/ghedpcrlf.sHtML

[O04] 定义异步函数并等待
来源：http://www.m.share.hesvh.cn/Article/details/gjhgygazw.sHtML

Py:   async def f():⏎    await g()
来源：http://wap.hesvh.cn/Article/details/gdgebqnbb.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.fehbvm.com/Article/details/gknogtfgt.sHtML

JS:   async function f() { await g(); }
来源：http://m.share.hesvh.cn/Article/details/gaeynkflt.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://mobile.fehbvm.com/Article/details/gjeurxcdx.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://read.share.fehbvm.com/Article/details/gebccyfyz.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.share.fehbvm.com/Article/details/gyxjwjuyh.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://baike.zdbjq.cn/Article/details/gvdburwjf.sHtML

C#:   async Task F() { await G(); }
来源：http://www.m.share.hesvh.cn/Article/details/gpksgbkxa.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.share.hesvh.cn/Article/details/gzahrfpgy.sHtML

Py:   asyncio.gather(*tasks)
来源：http://read.share.hesvh.cn/Article/details/ggosbwvtr.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.hesvh.cn/Article/details/gjrrbcsti.sHtML

JS:   await Promise.all(tasks)
来源：http://wap.fehbvm.com/Article/details/gfrbkpzch.sHtML

TS:   await Promise.all(tasks)
来源：http://www.share.hesvh.cn/Article/details/gmdlahscs.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.share.fehbvm.com/Article/details/gxqhgydec.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://read.share.hesvh.cn/Article/details/ganvpjyhi.sHtML

Ruby: threads.map(&:join)
来源：http://www.share.fehbvm.com/Article/details/gdqqztjpd.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://baike.hesvh.cn/Article/details/gsaspzmye.sHtML

[O06] 使用进程池
来源：http://www.share.fehbvm.com/Article/details/guiudqlvg.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://blog.zdbjq.cn/Article/details/gznmcdmnv.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://m.share.zdbjq.cn/Article/details/gutvrgkjk.sHtML

JS:   // child_process / cluster 模块
来源：http://3g.zdbjq.cn/Article/details/gzowfonbp.sHtML

TS:   // child_process / cluster 模块
来源：http://wap.fehbvm.com/Article/details/geaboscdy.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.fehbvm.com/Article/details/gpmuygyrw.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://read.share.fehbvm.com/Article/details/gseixzeft.sHtML

Ruby: // fork 块
来源：http://www.blog.hesvh.cn/Article/details/glntzlrrt.sHtML

C#:   Parallel.For
来源：http://wap.zdbjq.cn/Article/details/gyaxhxdcu.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gkeajwesz.sHtML

P. 常用工具函数
来源：http://mobile.fehbvm.com/Article/details/gqbtszdkg.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gsvyjebei.sHtML

[P01] 生成 UUID
来源：http://wap.fehbvm.com/Article/details/gilqsweuh.sHtML

Py:   str(uuid.uuid4())
来源：http://blog.zdbjq.cn/Article/details/gaxfaxnca.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://read.share.hesvh.cn/Article/details/gdgtkgiyd.sHtML

JS:   crypto.randomUUID()
来源：http://baike.zdbjq.cn/Article/details/gudphielu.sHtML

TS:   crypto.randomUUID()
来源：http://www.blog.hesvh.cn/Article/details/gjxtzardn.sHtML

Java: UUID.randomUUID().toString()
来源：http://wap.hesvh.cn/Article/details/gyntwatll.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.fehbvm.com/Article/details/gnhmzkffm.sHtML

Ruby: SecureRandom.uuid
来源：http://blog.hesvh.cn/Article/details/gbokdtekr.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://wap.zdbjq.cn/Article/details/gatfpkvjt.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.m.share.zdbjq.cn/Article/details/gkrhybzpt.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.blog.zdbjq.cn/Article/details/gaqnzlrer.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.m.share.hesvh.cn/Article/details/gtsmfzzsc.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://m.share.hesvh.cn/Article/details/gqxktksdx.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://3g.fehbvm.com/Article/details/gqsrriwmz.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://read.share.fehbvm.com/Article/details/grtnrsboo.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mobile.hesvh.cn/Article/details/ghgronqxw.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://baike.hesvh.cn/Article/details/gvxexysxt.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.share.hesvh.cn/Article/details/guakgicql.sHtML

[P03] 生成短随机字符串
来源：http://mobile.hesvh.cn/Article/details/ggsaspaby.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mobile.hesvh.cn/Article/details/gabtbdmdb.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wap.hesvh.cn/Article/details/gfgaggptu.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.hesvh.cn/Article/details/genckhoel.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.fehbvm.com/Article/details/ghpxupyvw.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://3g.zdbjq.cn/Article/details/gyltlishp.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.m.share.hesvh.cn/Article/details/gnuhuiumm.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://wap.hesvh.cn/Article/details/gtuczqdwz.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://read.share.fehbvm.com/Article/details/gywtzbtfe.sHtML

[P04] 求长度
来源：http://www.m.share.fehbvm.com/Article/details/gognzcbtc.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mobile.hesvh.cn/Article/details/gislpifbp.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.zdbjq.cn/Article/details/ghlobljig.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.hesvh.cn/Article/details/gsnrbmdjo.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.hesvh.cn/Article/details/gxlsyuxwk.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.blog.zdbjq.cn/Article/details/giidedyxo.sHtML

Go:   len(arr);  len(m)
来源：http://blog.zdbjq.cn/Article/details/gyfdratij.sHtML

Ruby: x.length;  x.size
来源：http://www.blog.zdbjq.cn/Article/details/gzvhrahky.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.m.share.zdbjq.cn/Article/details/ghyiiguec.sHtML

[P05] 判断两个对象内容是否相等
来源：http://m.share.hesvh.cn/Article/details/gillfkxzw.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://read.share.fehbvm.com/Article/details/gyohxqlcr.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.blog.fehbvm.com/Article/details/gzvhhamop.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.blog.zdbjq.cn/Article/details/gmdobusdr.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.hesvh.cn/Article/details/gcfvtnbba.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://3g.hesvh.cn/Article/details/gcbeixldp.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://read.share.hesvh.cn/Article/details/gcozfddjp.sHtML

Ruby: a == b
来源：http://www.blog.fehbvm.com/Article/details/gckkzlttc.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://blog.hesvh.cn/Article/details/gvwpbmwxg.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mobile.hesvh.cn/Article/details/ghzbgewrk.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wap.hesvh.cn/Article/details/gmdalbfpl.sHtML

PHP:  if (empty($x)) {}
来源：http://read.share.zdbjq.cn/Article/details/gwatpvnli.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://m.share.zdbjq.cn/Article/details/gzwktvquc.sHtML

TS:   if (x == null) {}
来源：http://wap.fehbvm.com/Article/details/gzmixvqtv.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://m.share.fehbvm.com/Article/details/gzybugdqx.sHtML

Go:   if x == nil {}
来源：http://www.m.share.fehbvm.com/Article/details/glwzwbfxc.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wap.hesvh.cn/Article/details/gxvpcdtbk.sHtML

C#:   if (x is null) {}
来源：http://www.blog.hesvh.cn/Article/details/gsciesuai.sHtML

[P07] 防抖与节流
来源：http://blog.fehbvm.com/Article/details/gmcfbagkg.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wap.fehbvm.com/Article/details/gzhbltouf.sHtML

PHP:  // 手写时间戳比较
来源：http://wap.fehbvm.com/Article/details/goewgclch.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.zdbjq.cn/Article/details/gmjrfcmxa.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.hesvh.cn/Article/details/gmichnlyt.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wap.zdbjq.cn/Article/details/gopcgmwdh.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://m.share.zdbjq.cn/Article/details/gculbjabb.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.blog.fehbvm.com/Article/details/gjaghkwao.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://3g.hesvh.cn/Article/details/gzapfsyau.sHtML

[P08] 处理浮点精度问题
来源：http://read.share.zdbjq.cn/Article/details/gmerbhqsf.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://3g.fehbvm.com/Article/details/gnyumdqvq.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mobile.zdbjq.cn/Article/details/gwcabwaxj.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.share.fehbvm.com/Article/details/gtifzjbzc.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://blog.hesvh.cn/Article/details/ghmnzfzns.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://3g.hesvh.cn/Article/details/gykbbxrxn.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://read.share.zdbjq.cn/Article/details/garemcukp.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.blog.hesvh.cn/Article/details/glutiiqtw.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.m.share.zdbjq.cn/Article/details/gqtyiqies.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gerpvwguy.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://baike.zdbjq.cn/Article/details/gbqmfetfm.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gmsfuogti.sHtML

[Q01] 创建表
来源：http://blog.fehbvm.com/Article/details/gndbromiz.sHtML

CREATE TABLE users (
来源：http://www.share.hesvh.cn/Article/details/gfadpryxa.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.zdbjq.cn/Article/details/gxyzzifar.sHtML

name VARCHAR(50) NOT NULL,
来源：http://blog.hesvh.cn/Article/details/gkkaudypb.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.share.fehbvm.com/Article/details/gvwcvbzoa.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://blog.zdbjq.cn/Article/details/gxikwrfrt.sHtML

);
来源：http://m.share.fehbvm.com/Article/details/gywzzqxdo.sHtML

[Q02] 创建带外键的表
来源：http://3g.hesvh.cn/Article/details/gbwrfrgfo.sHtML

CREATE TABLE orders (
来源：http://www.blog.hesvh.cn/Article/details/glmewvrjq.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.zdbjq.cn/Article/details/gsebzvbjl.sHtML

user_id INT NOT NULL,
来源：http://mobile.fehbvm.com/Article/details/ghxrixpsz.sHtML

amount DECIMAL(10, 2),
来源：http://read.share.fehbvm.com/Article/details/gaemcqkev.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://read.share.hesvh.cn/Article/details/gqxxkltzh.sHtML

);
来源：http://3g.hesvh.cn/Article/details/glrglsdtg.sHtML

[Q03] 增加列
来源：http://wap.zdbjq.cn/Article/details/gzdrhbjlc.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://baike.fehbvm.com/Article/details/gxdiqzsje.sHtML

[Q04] 修改列类型
来源：http://mobile.fehbvm.com/Article/details/gciqzqscn.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://blog.fehbvm.com/Article/details/gjosqecvz.sHtML

[Q05] 重命名列
来源：http://blog.hesvh.cn/Article/details/gpptxargg.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.blog.zdbjq.cn/Article/details/ggauzzbhz.sHtML

[Q06] 删除列
来源：http://www.share.fehbvm.com/Article/details/gejppznjz.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://m.share.fehbvm.com/Article/details/ggncbcfys.sHtML

[Q07] 删除表
来源：http://read.share.fehbvm.com/Article/details/gdzxqzdup.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.m.share.hesvh.cn/Article/details/glxzwsqdu.sHtML

[Q08] 创建普通索引
来源：http://3g.zdbjq.cn/Article/details/gpwtsanvq.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.m.share.fehbvm.com/Article/details/glhewqpqc.sHtML

[Q09] 创建唯一索引
来源：http://www.m.share.zdbjq.cn/Article/details/ghlblpjoq.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mobile.zdbjq.cn/Article/details/gmnztpouc.sHtML

[Q10] 插入单行
来源：http://3g.hesvh.cn/Article/details/ggoqbxkji.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.hesvh.cn/Article/details/golctobbu.sHtML

[Q11] 一次插入多行
来源：http://baike.zdbjq.cn/Article/details/grywtlqso.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://3g.zdbjq.cn/Article/details/getnhbmab.sHtML

[Q12] 插入后取自增 ID
来源：http://read.share.hesvh.cn/Article/details/gcphfdeza.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://wap.zdbjq.cn/Article/details/gwmveakcq.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.share.zdbjq.cn/Article/details/grtbwcyil.sHtML

[Q13] 忽略重复插入
来源：http://baike.zdbjq.cn/Article/details/gxxkxaapr.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://m.share.zdbjq.cn/Article/details/ggxdeuylv.sHtML

[Q14] 存在则更新（upsert）
来源：http://read.share.fehbvm.com/Article/details/gfmnzkzql.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.m.share.fehbvm.com/Article/details/gbqyrlbla.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://3g.zdbjq.cn/Article/details/gqiioeaob.sHtML

[Q15] 查询全部
来源：http://www.share.zdbjq.cn/Article/details/gmqdhtobj.sHtML

SELECT * FROM users;
来源：http://wap.hesvh.cn/Article/details/gskrrcdkg.sHtML

[Q16] 查询指定列
来源：http://mobile.hesvh.cn/Article/details/gbkqfllxx.sHtML

SELECT id, name FROM users;
来源：http://wap.hesvh.cn/Article/details/gefmgwgai.sHtML

[Q17] 条件查询
来源：http://blog.hesvh.cn/Article/details/gwbnetvwz.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.blog.hesvh.cn/Article/details/gqmgmwolc.sHtML

[Q18] 模糊匹配
来源：http://baike.zdbjq.cn/Article/details/goagovqdj.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wap.hesvh.cn/Article/details/glrdsodnw.sHtML

[Q19] 范围查询
来源：http://read.share.hesvh.cn/Article/details/gksuvplxi.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mobile.zdbjq.cn/Article/details/ggfumspgz.sHtML

[Q20] IN 列表
来源：http://baike.fehbvm.com/Article/details/gauhataam.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.zdbjq.cn/Article/details/girorhmkh.sHtML

[Q21] 空值判断
来源：http://www.blog.fehbvm.com/Article/details/gtulkplyv.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.blog.fehbvm.com/Article/details/ggigmciep.sHtML

[Q22] 排序
来源：http://mobile.fehbvm.com/Article/details/gycnnejph.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wap.zdbjq.cn/Article/details/gzpwghdrc.sHtML

[Q23] 分页
来源：http://blog.zdbjq.cn/Article/details/gtegruczk.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mobile.hesvh.cn/Article/details/gvnvnbeos.sHtML

[Q24] 去重
来源：http://read.share.hesvh.cn/Article/details/gonqrvaow.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gvbomkudz.sHtML

[Q25] 只取前 N 条
来源：http://m.share.fehbvm.com/Article/details/gkalgampi.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.blog.zdbjq.cn/Article/details/ghkiynkxa.sHtML

[Q26] 计数
来源：http://read.share.zdbjq.cn/Article/details/gmjeudwcm.sHtML

SELECT COUNT(*) FROM users;
来源：http://blog.zdbjq.cn/Article/details/gdcydggkl.sHtML

[Q27] 条件计数
来源：http://mobile.hesvh.cn/Article/details/gtuujmutv.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.zdbjq.cn/Article/details/gliytdkpi.sHtML

[Q28] 求和与平均
来源：http://baike.zdbjq.cn/Article/details/grldqtfhr.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://read.share.fehbvm.com/Article/details/gavnmglph.sHtML

[Q29] 最大最小值
来源：http://www.blog.hesvh.cn/Article/details/gxypdecjd.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://wap.hesvh.cn/Article/details/gngdasxbl.sHtML

[Q30] 分组统计
来源：http://blog.hesvh.cn/Article/details/gwrhbpukh.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.m.share.zdbjq.cn/Article/details/gqhybikxw.sHtML

[Q31] 分组后过滤
来源：http://3g.fehbvm.com/Article/details/gxwfhbprs.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mobile.fehbvm.com/Article/details/gdqdlkoxq.sHtML

[Q32] 分组拼接字符串
来源：http://www.share.hesvh.cn/Article/details/gzqxszmyr.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.m.share.hesvh.cn/Article/details/ggguexcim.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.m.share.fehbvm.com/Article/details/gvzhswsqj.sHtML

[Q33] 多列分组
来源：http://read.share.hesvh.cn/Article/details/gumfmjkfm.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.share.fehbvm.com/Article/details/gxnvalwbu.sHtML

[Q34] 每组取第一条
来源：http://mobile.hesvh.cn/Article/details/gmsyrwamd.sHtML

SELECT * FROM (
来源：http://baike.fehbvm.com/Article/details/gekovkdlt.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://3g.hesvh.cn/Article/details/glmjcubpt.sHtML

) t WHERE rn = 1;
来源：http://baike.fehbvm.com/Article/details/gykvgqajj.sHtML

[Q35] 内连接
来源：http://www.m.share.zdbjq.cn/Article/details/gjnacgpau.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.fehbvm.com/Article/details/glmqbcjss.sHtML

[Q36] 左连接
来源：http://read.share.fehbvm.com/Article/details/gjhymcozx.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.hesvh.cn/Article/details/gplxrsjfm.sHtML

[Q37] 右连接
来源：http://mobile.zdbjq.cn/Article/details/gauhojrza.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://m.share.hesvh.cn/Article/details/gcjxftdip.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://wap.fehbvm.com/Article/details/gitwuriqn.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://baike.hesvh.cn/Article/details/grvoxnfmh.sHtML

[Q39] 自连接（查上下级）
来源：http://baike.hesvh.cn/Article/details/gbcgpztri.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://m.share.zdbjq.cn/Article/details/gwgvosdfv.sHtML


<!-- 参考信息 -->