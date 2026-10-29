代发 wailian999

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://3g.hesvh.cn/Article/details/gaabqzfhm.sHtML

[N06] 判断回文字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gukytzgpt.sHtML

Py:   s == s[::-1]
来源：http://mobile.hesvh.cn/Article/details/gvvcyuvpk.sHtML

PHP:  $s === strrev($s);
来源：http://read.share.fehbvm.com/Article/details/gakwiorlg.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.share.zdbjq.cn/Article/details/gtyjixaqf.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.hesvh.cn/Article/details/ghaeebnue.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.m.share.zdbjq.cn/Article/details/gjgcdpnhz.sHtML

Go:   // 双指针从两端比较
来源：http://wap.zdbjq.cn/Article/details/gpalcuqoh.sHtML

Ruby: s == s.reverse
来源：http://mobile.hesvh.cn/Article/details/gtevztaav.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.share.zdbjq.cn/Article/details/gwkntrwtq.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.hesvh.cn/Article/details/ggzrzswnu.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://blog.fehbvm.com/Article/details/gcyeunzgc.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.fehbvm.com/Article/details/gitwasneb.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://m.share.hesvh.cn/Article/details/ghdmqhady.sHtML

TS:   // 手写 Map<string, number>
来源：http://m.share.zdbjq.cn/Article/details/gwkqjgpwx.sHtML

Java: // 手写 HashMap
来源：http://www.blog.zdbjq.cn/Article/details/gfozzrwli.sHtML

Go:   // 手写 map[int]int
来源：http://wap.fehbvm.com/Article/details/gikeirzrr.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.fehbvm.com/Article/details/gefuwmvqx.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://3g.zdbjq.cn/Article/details/gfhassvsx.sHtML

[N08] 生成全排列
来源：http://www.m.share.fehbvm.com/Article/details/gikxxnkzc.sHtML

Py:   itertools.permutations(arr)
来源：http://blog.fehbvm.com/Article/details/gthgozhgh.sHtML

PHP:  // 手写递归交换
来源：http://mobile.zdbjq.cn/Article/details/gcofbaggt.sHtML

JS:   // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/ggwygpogu.sHtML

TS:   // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/gqfmoxjyd.sHtML

Java: // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/gklxgkavp.sHtML

Go:   // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/gbaszrgck.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.hesvh.cn/Article/details/gifnmlmkx.sHtML

C#:   // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/glmevuggx.sHtML

[N09] 栈与队列
来源：http://www.share.zdbjq.cn/Article/details/glivejmzv.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://baike.hesvh.cn/Article/details/gmfogqldm.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://blog.hesvh.cn/Article/details/guxqqecjg.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://read.share.fehbvm.com/Article/details/grodshdtn.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://blog.zdbjq.cn/Article/details/geecnexfj.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.fehbvm.com/Article/details/gfhygbjql.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.zdbjq.cn/Article/details/gexcbtfwk.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://baike.hesvh.cn/Article/details/gbwxzqulj.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.fehbvm.com/Article/details/gbhwwvdxd.sHtML

[N10] 链表节点定义
来源：http://www.share.hesvh.cn/Article/details/geapldcky.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mobile.hesvh.cn/Article/details/gqjycqghs.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://m.share.hesvh.cn/Article/details/gosokgbrc.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://3g.fehbvm.com/Article/details/gpywpnsap.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.blog.fehbvm.com/Article/details/gpxlcsbyo.sHtML

Java: class Node { int v; Node next; }
来源：http://wap.zdbjq.cn/Article/details/ghnzopyed.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://blog.fehbvm.com/Article/details/gojfloeon.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://mobile.hesvh.cn/Article/details/gnorhikce.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.blog.fehbvm.com/Article/details/gponhbbap.sHtML

[N11] 二叉树中序遍历
来源：http://www.share.zdbjq.cn/Article/details/gfyfrfega.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.zdbjq.cn/Article/details/gjjafbufh.sHtML

PHP:  // 手写递归函数
来源：http://mobile.hesvh.cn/Article/details/giavnxdva.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.fehbvm.com/Article/details/gfgjdfxbb.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.hesvh.cn/Article/details/gssblnrlo.sHtML

Java: // 手写递归
来源：http://mobile.hesvh.cn/Article/details/gljapcdct.sHtML

Go:   // 手写递归
来源：http://wap.hesvh.cn/Article/details/guohaftcm.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.hesvh.cn/Article/details/givboqykr.sHtML

C#:   // 手写递归
来源：http://www.m.share.fehbvm.com/Article/details/gdfnzplrp.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.fehbvm.com/Article/details/gawizhkcq.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://baike.hesvh.cn/Article/details/gfhflvhxr.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.hesvh.cn/Article/details/gjplkhsjx.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.zdbjq.cn/Article/details/gozsaghcx.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.hesvh.cn/Article/details/gppgkzknu.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.fehbvm.com/Article/details/guyxtsbip.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.blog.hesvh.cn/Article/details/gjyxsoxvp.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://baike.zdbjq.cn/Article/details/ghlplnmtw.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.zdbjq.cn/Article/details/gymvzeekp.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gxlivokle.sHtML

O. 并发与异步
来源：http://3g.fehbvm.com/Article/details/gowruevro.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gbnbgfpmi.sHtML

[O01] 启动一个线程
来源：http://3g.fehbvm.com/Article/details/grtumcnrh.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://m.share.zdbjq.cn/Article/details/ghwjgpckq.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.fehbvm.com/Article/details/glibhmkyx.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://baike.fehbvm.com/Article/details/gxsnuucgy.sHtML

TS:   // 同 JS
来源：http://3g.fehbvm.com/Article/details/gcitqfkgj.sHtML

Java: new Thread(() -> f()).start()
来源：http://m.share.fehbvm.com/Article/details/gjssgbbbx.sHtML

Go:   go f()
来源：http://read.share.fehbvm.com/Article/details/gnoarvfbb.sHtML

Ruby: Thread.new { f }
来源：http://www.blog.zdbjq.cn/Article/details/gmtekoooj.sHtML

C#:   Task.Run(() => F());
来源：http://read.share.fehbvm.com/Article/details/grznotars.sHtML

[O02] 使用线程池
来源：http://3g.fehbvm.com/Article/details/gvbnzhupx.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.hesvh.cn/Article/details/gutsdggtc.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blog.hesvh.cn/Article/details/gatlecjsk.sHtML

JS:   // worker_threads 线程池
来源：http://www.m.share.hesvh.cn/Article/details/gcvahxnfm.sHtML

TS:   // worker_threads 线程池
来源：http://blog.zdbjq.cn/Article/details/gqmsgfrvu.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://read.share.hesvh.cn/Article/details/gerhlefdp.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wap.zdbjq.cn/Article/details/grretovmd.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://m.share.fehbvm.com/Article/details/gffuknrny.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mobile.hesvh.cn/Article/details/gjknpjjgm.sHtML

[O03] 加锁保护共享数据
来源：http://mobile.zdbjq.cn/Article/details/gwptjnxge.sHtML

Py:   with lock: shared += 1
来源：http://3g.hesvh.cn/Article/details/gkzsrrioz.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://wap.zdbjq.cn/Article/details/gsvywixti.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://3g.zdbjq.cn/Article/details/gznzdsjjk.sHtML

TS:   // 同 JS
来源：http://www.share.zdbjq.cn/Article/details/gmqscixwh.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.fehbvm.com/Article/details/grikegpvz.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://m.share.hesvh.cn/Article/details/grkebvmsy.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://3g.hesvh.cn/Article/details/gktaycisy.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.blog.hesvh.cn/Article/details/gufxrgxtg.sHtML

[O04] 定义异步函数并等待
来源：http://baike.hesvh.cn/Article/details/gvwznnifh.sHtML

Py:   async def f():⏎    await g()
来源：http://m.share.hesvh.cn/Article/details/gtirwagst.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://m.share.zdbjq.cn/Article/details/grgsfghum.sHtML

JS:   async function f() { await g(); }
来源：http://3g.hesvh.cn/Article/details/gcflbflhz.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://wap.fehbvm.com/Article/details/ghrzrmavu.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://baike.hesvh.cn/Article/details/gpgmbgovn.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.m.share.zdbjq.cn/Article/details/glmqpndkp.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://wap.fehbvm.com/Article/details/gkdqfswts.sHtML

C#:   async Task F() { await G(); }
来源：http://www.m.share.zdbjq.cn/Article/details/grametwpp.sHtML

[O05] 并发执行并等待全部完成
来源：http://blog.fehbvm.com/Article/details/gimqpjjrz.sHtML

Py:   asyncio.gather(*tasks)
来源：http://3g.fehbvm.com/Article/details/gkekurunb.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://3g.hesvh.cn/Article/details/gezqwpjys.sHtML

JS:   await Promise.all(tasks)
来源：http://read.share.fehbvm.com/Article/details/gulfngfts.sHtML

TS:   await Promise.all(tasks)
来源：http://www.share.fehbvm.com/Article/details/gcymcdeok.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://read.share.fehbvm.com/Article/details/golzhwhvn.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://3g.zdbjq.cn/Article/details/guwxxamrx.sHtML

Ruby: threads.map(&:join)
来源：http://3g.zdbjq.cn/Article/details/gpmxrirqu.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.m.share.fehbvm.com/Article/details/glpntmngk.sHtML

[O06] 使用进程池
来源：http://www.blog.zdbjq.cn/Article/details/govtykhgm.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://m.share.fehbvm.com/Article/details/gdkcqvqdb.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.m.share.fehbvm.com/Article/details/gdmlktsyb.sHtML

JS:   // child_process / cluster 模块
来源：http://www.blog.zdbjq.cn/Article/details/gbzwhwekf.sHtML

TS:   // child_process / cluster 模块
来源：http://baike.zdbjq.cn/Article/details/ggfjitidk.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.hesvh.cn/Article/details/gbizgkrpp.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.blog.zdbjq.cn/Article/details/gaygiwodt.sHtML

Ruby: // fork 块
来源：http://baike.hesvh.cn/Article/details/gmkihmcvi.sHtML

C#:   Parallel.For
来源：http://blog.hesvh.cn/Article/details/gpvpzzrvx.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gfpbwxbnb.sHtML

P. 常用工具函数
来源：http://wap.hesvh.cn/Article/details/gpaakyvkp.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gjneweijw.sHtML

[P01] 生成 UUID
来源：http://www.blog.fehbvm.com/Article/details/gfxammiuz.sHtML

Py:   str(uuid.uuid4())
来源：http://baike.fehbvm.com/Article/details/gkuoibudg.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.m.share.fehbvm.com/Article/details/ggffetfrr.sHtML

JS:   crypto.randomUUID()
来源：http://3g.zdbjq.cn/Article/details/gfotlwsul.sHtML

TS:   crypto.randomUUID()
来源：http://3g.hesvh.cn/Article/details/gukhurgdb.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.blog.fehbvm.com/Article/details/guhjohbka.sHtML

Go:   // 用 github.com/google/uuid
来源：http://read.share.zdbjq.cn/Article/details/gyzplgilr.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.hesvh.cn/Article/details/gwqcplflr.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.share.fehbvm.com/Article/details/guvfzqcxh.sHtML

[P02] MD5 / SHA256 摘要
来源：http://mobile.hesvh.cn/Article/details/gmsfbvztu.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.blog.hesvh.cn/Article/details/gjfotkoju.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.fehbvm.com/Article/details/glejdcjfz.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://m.share.fehbvm.com/Article/details/gmjogkxqx.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mobile.hesvh.cn/Article/details/gsgjseqtj.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://3g.hesvh.cn/Article/details/gyhhovaff.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.share.hesvh.cn/Article/details/gtydyvxcd.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://baike.zdbjq.cn/Article/details/gtuyxyywp.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://3g.zdbjq.cn/Article/details/gsbryzhwx.sHtML

[P03] 生成短随机字符串
来源：http://wap.hesvh.cn/Article/details/gncuaibsn.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://3g.zdbjq.cn/Article/details/gxhuutftt.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://read.share.zdbjq.cn/Article/details/gheilwfft.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.zdbjq.cn/Article/details/gqplzuapj.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.fehbvm.com/Article/details/gsevkhmen.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.fehbvm.com/Article/details/gpmrwihxt.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.blog.fehbvm.com/Article/details/gskdkafzd.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://m.share.hesvh.cn/Article/details/gtbozcljt.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mobile.hesvh.cn/Article/details/gxxvlrdto.sHtML

[P04] 求长度
来源：http://baike.zdbjq.cn/Article/details/getzbhtpm.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://3g.hesvh.cn/Article/details/glmtlfebq.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.zdbjq.cn/Article/details/gbuvnlgik.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.zdbjq.cn/Article/details/gnlqddtjn.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.zdbjq.cn/Article/details/gtdlbsixw.sHtML

Java: list.size();  map.size();  s.length()
来源：http://mobile.zdbjq.cn/Article/details/gdovgmduh.sHtML

Go:   len(arr);  len(m)
来源：http://www.blog.hesvh.cn/Article/details/garnywoml.sHtML

Ruby: x.length;  x.size
来源：http://read.share.hesvh.cn/Article/details/guursspxk.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.blog.hesvh.cn/Article/details/ggkwpkgca.sHtML

[P05] 判断两个对象内容是否相等
来源：http://m.share.zdbjq.cn/Article/details/gezswsavo.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://read.share.zdbjq.cn/Article/details/gzygidnqh.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://m.share.fehbvm.com/Article/details/grtzqynfu.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.share.fehbvm.com/Article/details/giwacnznq.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.zdbjq.cn/Article/details/gwtqmrjhv.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.m.share.hesvh.cn/Article/details/gzxedvmaz.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.m.share.hesvh.cn/Article/details/geyybhbuo.sHtML

Ruby: a == b
来源：http://www.share.zdbjq.cn/Article/details/gtjnvtuym.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://m.share.fehbvm.com/Article/details/gduzyhhcf.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wap.zdbjq.cn/Article/details/gflauxiju.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wap.fehbvm.com/Article/details/gmhyaiaey.sHtML

PHP:  if (empty($x)) {}
来源：http://www.m.share.fehbvm.com/Article/details/gawvhuttd.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://blog.hesvh.cn/Article/details/gxuikmfxx.sHtML

TS:   if (x == null) {}
来源：http://baike.fehbvm.com/Article/details/gjymfbvyi.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://3g.zdbjq.cn/Article/details/gyssdrywr.sHtML

Go:   if x == nil {}
来源：http://www.share.zdbjq.cn/Article/details/gmkepphcm.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.m.share.fehbvm.com/Article/details/gerlpsxih.sHtML

C#:   if (x is null) {}
来源：http://read.share.fehbvm.com/Article/details/gbggameha.sHtML

[P07] 防抖与节流
来源：http://baike.zdbjq.cn/Article/details/gcamvnzlf.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://m.share.zdbjq.cn/Article/details/gbspimieq.sHtML

PHP:  // 手写时间戳比较
来源：http://www.blog.fehbvm.com/Article/details/gscaadgdn.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.zdbjq.cn/Article/details/gbxdwzvcg.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.fehbvm.com/Article/details/gvgjkfdej.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://baike.zdbjq.cn/Article/details/gwqgfaquk.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://baike.fehbvm.com/Article/details/gksbxcxnq.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://m.share.hesvh.cn/Article/details/gebrzjgnz.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://read.share.fehbvm.com/Article/details/gxofjauej.sHtML

[P08] 处理浮点精度问题
来源：http://baike.fehbvm.com/Article/details/gspiwzztp.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.blog.fehbvm.com/Article/details/gfaisblkv.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://read.share.hesvh.cn/Article/details/gmkmaxwdo.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://read.share.zdbjq.cn/Article/details/gurlstlqg.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.blog.fehbvm.com/Article/details/gdieutgbf.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wap.fehbvm.com/Article/details/gbrylgktb.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.share.fehbvm.com/Article/details/gjmlfgkwj.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://read.share.zdbjq.cn/Article/details/glmsbdhfx.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mobile.zdbjq.cn/Article/details/gisltuvhn.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gwfivyoqy.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://3g.fehbvm.com/Article/details/gycixjuro.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gumyipiqh.sHtML

[Q01] 创建表
来源：http://www.blog.fehbvm.com/Article/details/gipjvvvth.sHtML

CREATE TABLE users (
来源：http://mobile.fehbvm.com/Article/details/gxueaqlqb.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.fehbvm.com/Article/details/gqbulqhyv.sHtML

name VARCHAR(50) NOT NULL,
来源：http://mobile.hesvh.cn/Article/details/gebcyqqby.sHtML

email VARCHAR(100) UNIQUE,
来源：http://blog.hesvh.cn/Article/details/gytcuuosu.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://read.share.zdbjq.cn/Article/details/gvhobyrzo.sHtML

);
来源：http://read.share.fehbvm.com/Article/details/gfdkwwiwn.sHtML

[Q02] 创建带外键的表
来源：http://mobile.fehbvm.com/Article/details/gaphybjob.sHtML

CREATE TABLE orders (
来源：http://www.blog.hesvh.cn/Article/details/ggfgmltoz.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.zdbjq.cn/Article/details/gdvgqqqiz.sHtML

user_id INT NOT NULL,
来源：http://www.blog.hesvh.cn/Article/details/gezpogcxh.sHtML

amount DECIMAL(10, 2),
来源：http://www.share.hesvh.cn/Article/details/grgamkuly.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.share.fehbvm.com/Article/details/gagfxzwhz.sHtML

);
来源：http://www.blog.fehbvm.com/Article/details/ggjwilyev.sHtML

[Q03] 增加列
来源：http://blog.fehbvm.com/Article/details/gntfnpiow.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://3g.hesvh.cn/Article/details/gzytzdqbo.sHtML

[Q04] 修改列类型
来源：http://read.share.hesvh.cn/Article/details/grntejvef.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://blog.fehbvm.com/Article/details/gllewztqp.sHtML

[Q05] 重命名列
来源：http://baike.hesvh.cn/Article/details/gxohwmdrk.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wap.fehbvm.com/Article/details/gpxtqxiks.sHtML

[Q06] 删除列
来源：http://m.share.zdbjq.cn/Article/details/grjtifeqw.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://read.share.hesvh.cn/Article/details/grieeomed.sHtML

[Q07] 删除表
来源：http://blog.zdbjq.cn/Article/details/gzjkfnirv.sHtML

DROP TABLE IF EXISTS orders;
来源：http://3g.fehbvm.com/Article/details/gwemorkae.sHtML

[Q08] 创建普通索引
来源：http://m.share.hesvh.cn/Article/details/gpgvqvjjb.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://wap.hesvh.cn/Article/details/gnrqnmsob.sHtML

[Q09] 创建唯一索引
来源：http://wap.zdbjq.cn/Article/details/gsedsonpc.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.share.fehbvm.com/Article/details/grwcjffdn.sHtML

[Q10] 插入单行
来源：http://read.share.fehbvm.com/Article/details/gtiwcobye.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.blog.hesvh.cn/Article/details/gqrssayaf.sHtML

[Q11] 一次插入多行
来源：http://m.share.zdbjq.cn/Article/details/gthmcuvnc.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mobile.zdbjq.cn/Article/details/gdiytzrjq.sHtML

[Q12] 插入后取自增 ID
来源：http://www.share.hesvh.cn/Article/details/ghxrseysr.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://3g.hesvh.cn/Article/details/gaypkzlzu.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://m.share.fehbvm.com/Article/details/glejlhgqh.sHtML

[Q13] 忽略重复插入
来源：http://baike.zdbjq.cn/Article/details/gnlkpibir.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://3g.zdbjq.cn/Article/details/gcfekiono.sHtML

[Q14] 存在则更新（upsert）
来源：http://baike.fehbvm.com/Article/details/ggeqapoha.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wap.hesvh.cn/Article/details/gxwoopseb.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://baike.hesvh.cn/Article/details/gnfzvuqdb.sHtML

[Q15] 查询全部
来源：http://mobile.fehbvm.com/Article/details/gkrcuggdn.sHtML

SELECT * FROM users;
来源：http://www.share.fehbvm.com/Article/details/gyhoswefb.sHtML

[Q16] 查询指定列
来源：http://m.share.fehbvm.com/Article/details/ggepfohil.sHtML

SELECT id, name FROM users;
来源：http://read.share.hesvh.cn/Article/details/gwzmvxvrz.sHtML

[Q17] 条件查询
来源：http://blog.zdbjq.cn/Article/details/gryzznsce.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://blog.hesvh.cn/Article/details/gpwirlgdl.sHtML

[Q18] 模糊匹配
来源：http://blog.zdbjq.cn/Article/details/gestywfby.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.m.share.hesvh.cn/Article/details/goagcsbsr.sHtML

[Q19] 范围查询
来源：http://3g.fehbvm.com/Article/details/gcnshppfw.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://3g.zdbjq.cn/Article/details/gmsvpiwad.sHtML

[Q20] IN 列表
来源：http://mobile.fehbvm.com/Article/details/gccxxvnqw.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gtkojzdjh.sHtML

[Q21] 空值判断
来源：http://www.blog.hesvh.cn/Article/details/gnsgaahwb.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.blog.fehbvm.com/Article/details/gvbiownnm.sHtML

[Q22] 排序
来源：http://read.share.hesvh.cn/Article/details/gwczfhkue.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.fehbvm.com/Article/details/gciwdsdxa.sHtML

[Q23] 分页
来源：http://blog.hesvh.cn/Article/details/goixrytkq.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://baike.zdbjq.cn/Article/details/gsogjcwmi.sHtML

[Q24] 去重
来源：http://3g.fehbvm.com/Article/details/gpwrrjfix.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gjvjvuosl.sHtML

[Q25] 只取前 N 条
来源：http://www.blog.hesvh.cn/Article/details/gksnlplqx.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.hesvh.cn/Article/details/giwceybpv.sHtML

[Q26] 计数
来源：http://m.share.hesvh.cn/Article/details/gszodabrp.sHtML

SELECT COUNT(*) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gqyeqfpvj.sHtML

[Q27] 条件计数
来源：http://3g.zdbjq.cn/Article/details/gjgwipcxz.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gykeidzad.sHtML

[Q28] 求和与平均
来源：http://baike.zdbjq.cn/Article/details/gtuypklyc.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.share.fehbvm.com/Article/details/guugnmtam.sHtML

[Q29] 最大最小值
来源：http://www.share.zdbjq.cn/Article/details/gymzpnpdh.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.fehbvm.com/Article/details/gqdhpebmw.sHtML

[Q30] 分组统计
来源：http://wap.hesvh.cn/Article/details/gbjhejqhe.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.m.share.zdbjq.cn/Article/details/gntzklnag.sHtML

[Q31] 分组后过滤
来源：http://read.share.hesvh.cn/Article/details/gksmefvyt.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.m.share.hesvh.cn/Article/details/gvrobxyjw.sHtML

[Q32] 分组拼接字符串
来源：http://3g.hesvh.cn/Article/details/gwimhutrs.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.blog.zdbjq.cn/Article/details/ghxyjadto.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.share.hesvh.cn/Article/details/gpeqqeism.sHtML

[Q33] 多列分组
来源：http://blog.hesvh.cn/Article/details/grtecguzx.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://baike.fehbvm.com/Article/details/gwstzytvr.sHtML

[Q34] 每组取第一条
来源：http://wap.fehbvm.com/Article/details/gcvbimuvj.sHtML

SELECT * FROM (
来源：http://wap.fehbvm.com/Article/details/gpmdyvssl.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.m.share.zdbjq.cn/Article/details/gcyvlzdnu.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gvkbyskam.sHtML

[Q35] 内连接
来源：http://www.share.zdbjq.cn/Article/details/goixwugqb.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wap.zdbjq.cn/Article/details/ghnqpmwqy.sHtML

[Q36] 左连接
来源：http://read.share.zdbjq.cn/Article/details/grliexnxq.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.share.fehbvm.com/Article/details/grizaigcn.sHtML

[Q37] 右连接
来源：http://3g.zdbjq.cn/Article/details/guelvxpyr.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://blog.hesvh.cn/Article/details/grtmcrkml.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://blog.zdbjq.cn/Article/details/gtcdeberj.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.blog.fehbvm.com/Article/details/gstwfgnuq.sHtML

[Q39] 自连接（查上下级）
来源：http://wap.fehbvm.com/Article/details/gasyidory.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://wap.hesvh.cn/Article/details/gsphyirwf.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.zdbjq.cn/Article/details/gdoulzvof.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.blog.fehbvm.com/Article/details/gwhiempbr.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://m.share.fehbvm.com/Article/details/glacxsfhx.sHtML

[Q41] 多表连接
来源：http://mobile.zdbjq.cn/Article/details/gaeagplwy.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://read.share.fehbvm.com/Article/details/gochpfkjn.sHtML

JOIN users u ON u.id = o.user_id
来源：http://wap.zdbjq.cn/Article/details/gegdigtrv.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.fehbvm.com/Article/details/gkfudiqag.sHtML

[Q42] 连接条件附加过滤
来源：http://wap.fehbvm.com/Article/details/gvimkddyx.sHtML


<!-- 参考信息 -->