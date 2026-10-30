代发 wailian999

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://read.share.hesvh.cn/Article/details/ghrcxmlua.sHtML

[N06] 判断回文字符串
来源：http://read.share.zdbjq.cn/Article/details/gfuymylrg.sHtML

Py:   s == s[::-1]
来源：http://baike.fehbvm.com/Article/details/gpkjlvxul.sHtML

PHP:  $s === strrev($s);
来源：http://3g.hesvh.cn/Article/details/gcbfbjkcb.sHtML

JS:   s === [...s].reverse().join("")
来源：http://wap.zdbjq.cn/Article/details/ghcmkgswe.sHtML

TS:   s === [...s].reverse().join("")
来源：http://3g.fehbvm.com/Article/details/gdzcwjyuw.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.m.share.fehbvm.com/Article/details/gmfujdqia.sHtML

Go:   // 双指针从两端比较
来源：http://www.m.share.fehbvm.com/Article/details/gyriaymjt.sHtML

Ruby: s == s.reverse
来源：http://www.m.share.fehbvm.com/Article/details/gmqdxghxg.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://blog.hesvh.cn/Article/details/gdsesziex.sHtML

[N07] 两数之和（返回下标）
来源：http://read.share.zdbjq.cn/Article/details/gjcivrsyh.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.blog.zdbjq.cn/Article/details/gmlloaqrx.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://read.share.fehbvm.com/Article/details/ghyfwytfg.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://blog.fehbvm.com/Article/details/gsyysijpn.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.fehbvm.com/Article/details/gputqsfmy.sHtML

Java: // 手写 HashMap
来源：http://3g.hesvh.cn/Article/details/gqkonckrf.sHtML

Go:   // 手写 map[int]int
来源：http://baike.hesvh.cn/Article/details/gldzqhuoh.sHtML

Ruby: // 手写 Hash
来源：http://wap.fehbvm.com/Article/details/gewgarhce.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://3g.hesvh.cn/Article/details/gunpmoctn.sHtML

[N08] 生成全排列
来源：http://www.blog.fehbvm.com/Article/details/gvpcsmjap.sHtML

Py:   itertools.permutations(arr)
来源：http://read.share.zdbjq.cn/Article/details/ghcbtzrje.sHtML

PHP:  // 手写递归交换
来源：http://www.share.zdbjq.cn/Article/details/gdtortoxq.sHtML

JS:   // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/gwpmwxmhb.sHtML

TS:   // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/gzfjffbdg.sHtML

Java: // 手写回溯递归
来源：http://www.blog.fehbvm.com/Article/details/gpzhqdfls.sHtML

Go:   // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/gnuaalqql.sHtML

Ruby: arr.permutation.to_a
来源：http://blog.fehbvm.com/Article/details/ghgcyphqv.sHtML

C#:   // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/gmskvdxka.sHtML

[N09] 栈与队列
来源：http://m.share.hesvh.cn/Article/details/ghoholdvw.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.fehbvm.com/Article/details/gzboyxqhg.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://3g.hesvh.cn/Article/details/ghuqfucbp.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://3g.hesvh.cn/Article/details/gfjsmxkxz.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.fehbvm.com/Article/details/gviqfkoxv.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.fehbvm.com/Article/details/gtxfdjhwt.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.fehbvm.com/Article/details/gnwmwrlmm.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mobile.fehbvm.com/Article/details/gseuckyln.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.hesvh.cn/Article/details/glvgybzlz.sHtML

[N10] 链表节点定义
来源：http://read.share.hesvh.cn/Article/details/guviaojab.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.blog.zdbjq.cn/Article/details/gneccyjkw.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.blog.hesvh.cn/Article/details/gmnkkikdi.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://blog.zdbjq.cn/Article/details/gpyssuxbc.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.hesvh.cn/Article/details/gzjarlyvn.sHtML

Java: class Node { int v; Node next; }
来源：http://www.share.zdbjq.cn/Article/details/gxyvpuojg.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://wap.zdbjq.cn/Article/details/gxlggdfin.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.zdbjq.cn/Article/details/gdvyesnib.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://read.share.fehbvm.com/Article/details/gazwphviu.sHtML

[N11] 二叉树中序遍历
来源：http://www.share.fehbvm.com/Article/details/ggjcvdpvv.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.blog.hesvh.cn/Article/details/ghsqpduab.sHtML

PHP:  // 手写递归函数
来源：http://baike.hesvh.cn/Article/details/gtmwsfwis.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.hesvh.cn/Article/details/glffbuxsq.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.fehbvm.com/Article/details/gjhxxxrrw.sHtML

Java: // 手写递归
来源：http://m.share.hesvh.cn/Article/details/gxntmodbj.sHtML

Go:   // 手写递归
来源：http://m.share.zdbjq.cn/Article/details/gwfndqevd.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.m.share.fehbvm.com/Article/details/gabkhpmjd.sHtML

C#:   // 手写递归
来源：http://mobile.fehbvm.com/Article/details/gvlkzofqp.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.share.zdbjq.cn/Article/details/gelqoqsfp.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mobile.zdbjq.cn/Article/details/gqjomzcur.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.m.share.zdbjq.cn/Article/details/gohfobnzw.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.zdbjq.cn/Article/details/gmlfihmpl.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.zdbjq.cn/Article/details/gojmabqjy.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.zdbjq.cn/Article/details/gmzsczaze.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.m.share.hesvh.cn/Article/details/gbtbcwsvw.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://m.share.fehbvm.com/Article/details/gphrovcxc.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.fehbvm.com/Article/details/gdlqyzpwr.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/ggzgvduzx.sHtML

O. 并发与异步
来源：http://wap.zdbjq.cn/Article/details/gjyxhknyy.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/grfpdasew.sHtML

[O01] 启动一个线程
来源：http://www.share.fehbvm.com/Article/details/gfsidwltm.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mobile.fehbvm.com/Article/details/gwdkrvzjb.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://blog.fehbvm.com/Article/details/gyeacmqpf.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://3g.zdbjq.cn/Article/details/gybrrrais.sHtML

TS:   // 同 JS
来源：http://www.share.hesvh.cn/Article/details/gzdefidpb.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.fehbvm.com/Article/details/gbvvywwer.sHtML

Go:   go f()
来源：http://m.share.hesvh.cn/Article/details/guzhwhaqn.sHtML

Ruby: Thread.new { f }
来源：http://www.share.zdbjq.cn/Article/details/gpgwtdkwr.sHtML

C#:   Task.Run(() => F());
来源：http://www.blog.zdbjq.cn/Article/details/gqshfnkrz.sHtML

[O02] 使用线程池
来源：http://blog.fehbvm.com/Article/details/ggqbtmmnv.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://baike.zdbjq.cn/Article/details/gelqrcmzd.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://m.share.hesvh.cn/Article/details/ghvkhacce.sHtML

JS:   // worker_threads 线程池
来源：http://www.m.share.zdbjq.cn/Article/details/ghgphvfcr.sHtML

TS:   // worker_threads 线程池
来源：http://baike.hesvh.cn/Article/details/gscsfetlo.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://mobile.fehbvm.com/Article/details/gqaszfith.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://read.share.zdbjq.cn/Article/details/grvzwhdur.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://3g.hesvh.cn/Article/details/guhkpicnr.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://3g.fehbvm.com/Article/details/gnyviicst.sHtML

[O03] 加锁保护共享数据
来源：http://blog.zdbjq.cn/Article/details/gvkhvpqsr.sHtML

Py:   with lock: shared += 1
来源：http://www.m.share.zdbjq.cn/Article/details/gmyqudppc.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.m.share.zdbjq.cn/Article/details/golcptpjg.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.hesvh.cn/Article/details/gbutdclku.sHtML

TS:   // 同 JS
来源：http://www.m.share.fehbvm.com/Article/details/glkkfgayj.sHtML

Java: synchronized (this) { shared++; }
来源：http://baike.hesvh.cn/Article/details/ghhofyxuo.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://3g.zdbjq.cn/Article/details/gvcmhzvro.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://wap.zdbjq.cn/Article/details/gidxdyili.sHtML

C#:   lock (gate) { shared++; }
来源：http://wap.zdbjq.cn/Article/details/gihbrmdfn.sHtML

[O04] 定义异步函数并等待
来源：http://www.m.share.fehbvm.com/Article/details/gohsursbv.sHtML

Py:   async def f():⏎    await g()
来源：http://baike.zdbjq.cn/Article/details/gjoduffwk.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.blog.fehbvm.com/Article/details/gyxpfkilb.sHtML

JS:   async function f() { await g(); }
来源：http://m.share.hesvh.cn/Article/details/gmcdqmmiv.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.share.zdbjq.cn/Article/details/gjhzuasql.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://blog.fehbvm.com/Article/details/ggumygbje.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://m.share.fehbvm.com/Article/details/gbhausvyp.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://read.share.hesvh.cn/Article/details/gdugqllnj.sHtML

C#:   async Task F() { await G(); }
来源：http://www.m.share.zdbjq.cn/Article/details/ghacmndcb.sHtML

[O05] 并发执行并等待全部完成
来源：http://wap.hesvh.cn/Article/details/gwlfccdpb.sHtML

Py:   asyncio.gather(*tasks)
来源：http://read.share.hesvh.cn/Article/details/gfjivmemc.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.blog.fehbvm.com/Article/details/gtbymttjf.sHtML

JS:   await Promise.all(tasks)
来源：http://www.m.share.fehbvm.com/Article/details/ghpcxxudp.sHtML

TS:   await Promise.all(tasks)
来源：http://wap.fehbvm.com/Article/details/gsaqhfvgh.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://read.share.fehbvm.com/Article/details/geimcgvkv.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://baike.zdbjq.cn/Article/details/gcpzpnrgg.sHtML

Ruby: threads.map(&:join)
来源：http://3g.hesvh.cn/Article/details/grjflkorj.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://3g.zdbjq.cn/Article/details/gfqfmamkq.sHtML

[O06] 使用进程池
来源：http://baike.hesvh.cn/Article/details/gcjldqukv.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.blog.fehbvm.com/Article/details/glosjsist.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://baike.hesvh.cn/Article/details/gpbxzarhf.sHtML

JS:   // child_process / cluster 模块
来源：http://m.share.fehbvm.com/Article/details/gdbdajslt.sHtML

TS:   // child_process / cluster 模块
来源：http://wap.zdbjq.cn/Article/details/grrpuavww.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://read.share.hesvh.cn/Article/details/gtbmaggxn.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mobile.zdbjq.cn/Article/details/gxrqtzbbg.sHtML

Ruby: // fork 块
来源：http://3g.fehbvm.com/Article/details/grbtnplhl.sHtML

C#:   Parallel.For
来源：http://read.share.fehbvm.com/Article/details/gddjfuvbj.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gjvxkzbbk.sHtML

P. 常用工具函数
来源：http://www.m.share.zdbjq.cn/Article/details/gmpzgewgs.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gwctehfzl.sHtML

[P01] 生成 UUID
来源：http://www.blog.fehbvm.com/Article/details/gvhuiabyk.sHtML

Py:   str(uuid.uuid4())
来源：http://m.share.zdbjq.cn/Article/details/geqhrifrg.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mobile.hesvh.cn/Article/details/gtqfqebqi.sHtML

JS:   crypto.randomUUID()
来源：http://mobile.hesvh.cn/Article/details/ghahzjrwr.sHtML

TS:   crypto.randomUUID()
来源：http://3g.fehbvm.com/Article/details/gfgpetmhz.sHtML

Java: UUID.randomUUID().toString()
来源：http://blog.fehbvm.com/Article/details/gphoanowp.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.m.share.hesvh.cn/Article/details/gqqyssuyo.sHtML

Ruby: SecureRandom.uuid
来源：http://blog.zdbjq.cn/Article/details/gxalwqplp.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://3g.hesvh.cn/Article/details/gozthdcck.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.m.share.fehbvm.com/Article/details/gyjwsylvr.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.share.hesvh.cn/Article/details/gobpnikql.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://blog.fehbvm.com/Article/details/gjfyemhge.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://m.share.fehbvm.com/Article/details/gnqplulse.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mobile.hesvh.cn/Article/details/gkckqbduf.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://blog.zdbjq.cn/Article/details/gzmmpldnm.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://read.share.zdbjq.cn/Article/details/gtsnksvjf.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wap.hesvh.cn/Article/details/gprjvgkor.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.blog.zdbjq.cn/Article/details/gatmngfkv.sHtML

[P03] 生成短随机字符串
来源：http://blog.zdbjq.cn/Article/details/gbcfxljjc.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.blog.hesvh.cn/Article/details/gxjhwliam.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://m.share.fehbvm.com/Article/details/gfhvivmjz.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.hesvh.cn/Article/details/gnqdlelpi.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.zdbjq.cn/Article/details/ghloerjnz.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.share.fehbvm.com/Article/details/guepymwfe.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://blog.zdbjq.cn/Article/details/gpbreautf.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.blog.fehbvm.com/Article/details/gumeflvwo.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://m.share.fehbvm.com/Article/details/gcgrzkeyo.sHtML

[P04] 求长度
来源：http://mobile.hesvh.cn/Article/details/ghbbjoeca.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.m.share.hesvh.cn/Article/details/gqvaudbca.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.zdbjq.cn/Article/details/gaynsanoo.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.hesvh.cn/Article/details/gginulfvs.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.hesvh.cn/Article/details/gosppcqff.sHtML

Java: list.size();  map.size();  s.length()
来源：http://m.share.hesvh.cn/Article/details/gsgptyhol.sHtML

Go:   len(arr);  len(m)
来源：http://mobile.fehbvm.com/Article/details/gftwjorvo.sHtML

Ruby: x.length;  x.size
来源：http://m.share.zdbjq.cn/Article/details/gkwnbngpu.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://wap.fehbvm.com/Article/details/gxlnaffmw.sHtML

[P05] 判断两个对象内容是否相等
来源：http://mobile.hesvh.cn/Article/details/gxuaextqy.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://read.share.zdbjq.cn/Article/details/gadqwnuwp.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://read.share.zdbjq.cn/Article/details/gsyicuzfi.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://m.share.fehbvm.com/Article/details/gaqvqgthc.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.zdbjq.cn/Article/details/gbxtoglgm.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.share.zdbjq.cn/Article/details/gpmvgtyid.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://wap.zdbjq.cn/Article/details/goxkuvjha.sHtML

Ruby: a == b
来源：http://read.share.fehbvm.com/Article/details/grqcclmao.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://blog.zdbjq.cn/Article/details/gpodadkto.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wap.fehbvm.com/Article/details/gvkapjytr.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://blog.fehbvm.com/Article/details/gndejjaqh.sHtML

PHP:  if (empty($x)) {}
来源：http://baike.fehbvm.com/Article/details/ghtjvpvzf.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mobile.fehbvm.com/Article/details/gdugdthoi.sHtML

TS:   if (x == null) {}
来源：http://www.blog.hesvh.cn/Article/details/ghszzxpal.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://m.share.fehbvm.com/Article/details/gqkoumsit.sHtML

Go:   if x == nil {}
来源：http://3g.hesvh.cn/Article/details/guyprwhbp.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.m.share.fehbvm.com/Article/details/gzxiaxyvi.sHtML

C#:   if (x is null) {}
来源：http://www.share.fehbvm.com/Article/details/ghpajstnt.sHtML

[P07] 防抖与节流
来源：http://m.share.hesvh.cn/Article/details/gpbcmbjrc.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://m.share.fehbvm.com/Article/details/gloiiykus.sHtML

PHP:  // 手写时间戳比较
来源：http://www.blog.fehbvm.com/Article/details/gpqzbswah.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.hesvh.cn/Article/details/gmiexstwp.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.hesvh.cn/Article/details/grolsskyr.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mobile.zdbjq.cn/Article/details/gtoqywyyc.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.m.share.hesvh.cn/Article/details/gvyeaavik.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.zdbjq.cn/Article/details/gfqyykhql.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://m.share.hesvh.cn/Article/details/gqqejydfd.sHtML

[P08] 处理浮点精度问题
来源：http://www.share.hesvh.cn/Article/details/gjsjjbhkk.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://blog.hesvh.cn/Article/details/gqsazsqeq.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mobile.hesvh.cn/Article/details/glitjwnis.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.m.share.hesvh.cn/Article/details/ggcoklkwz.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wap.zdbjq.cn/Article/details/gxwrgwgle.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.share.fehbvm.com/Article/details/gslzusyeq.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.blog.zdbjq.cn/Article/details/gbpaucjqc.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://baike.hesvh.cn/Article/details/gfjzvpafn.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mobile.fehbvm.com/Article/details/gipmeibvu.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gvehwdxmk.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://m.share.fehbvm.com/Article/details/ghjszgpyt.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gglqaoztb.sHtML

[Q01] 创建表
来源：http://baike.zdbjq.cn/Article/details/grzcwagkd.sHtML

CREATE TABLE users (
来源：http://mobile.fehbvm.com/Article/details/ggifzvybw.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.fehbvm.com/Article/details/gthlqpuyn.sHtML

name VARCHAR(50) NOT NULL,
来源：http://3g.hesvh.cn/Article/details/gczduifho.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.blog.hesvh.cn/Article/details/gqnaridcz.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wap.zdbjq.cn/Article/details/gkmhymyhb.sHtML

);
来源：http://m.share.zdbjq.cn/Article/details/gfxfuxbyy.sHtML

[Q02] 创建带外键的表
来源：http://mobile.zdbjq.cn/Article/details/ggftsuhkz.sHtML

CREATE TABLE orders (
来源：http://baike.fehbvm.com/Article/details/gcknvdgjj.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.hesvh.cn/Article/details/garwdgyxd.sHtML

user_id INT NOT NULL,
来源：http://m.share.zdbjq.cn/Article/details/gludlupqd.sHtML

amount DECIMAL(10, 2),
来源：http://3g.hesvh.cn/Article/details/gfomqmtai.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://m.share.zdbjq.cn/Article/details/gcsygazpt.sHtML

);
来源：http://mobile.zdbjq.cn/Article/details/goyqmcumi.sHtML

[Q03] 增加列
来源：http://www.m.share.hesvh.cn/Article/details/gkxudmeca.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.blog.hesvh.cn/Article/details/gctagbukw.sHtML

[Q04] 修改列类型
来源：http://mobile.zdbjq.cn/Article/details/glmihgnnm.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.share.fehbvm.com/Article/details/gvuswzaay.sHtML

[Q05] 重命名列
来源：http://www.share.fehbvm.com/Article/details/gpezjgnft.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://read.share.hesvh.cn/Article/details/gexoaqgtu.sHtML

[Q06] 删除列
来源：http://3g.hesvh.cn/Article/details/gdjpyilya.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.m.share.hesvh.cn/Article/details/ghhksudqy.sHtML

[Q07] 删除表
来源：http://wap.hesvh.cn/Article/details/grbhyhpud.sHtML

DROP TABLE IF EXISTS orders;
来源：http://wap.hesvh.cn/Article/details/ggsuktnqd.sHtML

[Q08] 创建普通索引
来源：http://wap.hesvh.cn/Article/details/gnksiqtwx.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.blog.fehbvm.com/Article/details/gcxprozpn.sHtML

[Q09] 创建唯一索引
来源：http://www.m.share.zdbjq.cn/Article/details/ghbmlgupn.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://3g.fehbvm.com/Article/details/gpepxzbtu.sHtML

[Q10] 插入单行
来源：http://www.share.fehbvm.com/Article/details/gbeupimku.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.m.share.hesvh.cn/Article/details/grxibmuxs.sHtML

[Q11] 一次插入多行
来源：http://blog.hesvh.cn/Article/details/gfskldlim.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://3g.hesvh.cn/Article/details/gqajfgeta.sHtML

[Q12] 插入后取自增 ID
来源：http://blog.zdbjq.cn/Article/details/gyecqnhez.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://mobile.fehbvm.com/Article/details/ghoxsobga.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mobile.zdbjq.cn/Article/details/gotknqhpc.sHtML

[Q13] 忽略重复插入
来源：http://www.share.fehbvm.com/Article/details/grtvfopxm.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://3g.fehbvm.com/Article/details/gielxhure.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.share.hesvh.cn/Article/details/gvolzqxan.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.m.share.fehbvm.com/Article/details/gwqfdiusq.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mobile.hesvh.cn/Article/details/gwwotigll.sHtML

[Q15] 查询全部
来源：http://mobile.zdbjq.cn/Article/details/gjmgpconm.sHtML

SELECT * FROM users;
来源：http://blog.zdbjq.cn/Article/details/gimyetxsv.sHtML

[Q16] 查询指定列
来源：http://read.share.fehbvm.com/Article/details/gsbpukqyu.sHtML

SELECT id, name FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gvpicsiiy.sHtML

[Q17] 条件查询
来源：http://www.share.zdbjq.cn/Article/details/gdidmkibj.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://baike.zdbjq.cn/Article/details/gdftxvtif.sHtML

[Q18] 模糊匹配
来源：http://wap.fehbvm.com/Article/details/gvjgrllgj.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mobile.zdbjq.cn/Article/details/gzyzltzzl.sHtML

[Q19] 范围查询
来源：http://www.m.share.hesvh.cn/Article/details/gkyvofvei.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://blog.zdbjq.cn/Article/details/gdbmxvjbl.sHtML

[Q20] IN 列表
来源：http://baike.fehbvm.com/Article/details/glcpanafj.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.fehbvm.com/Article/details/gbrgncgpn.sHtML

[Q21] 空值判断
来源：http://blog.zdbjq.cn/Article/details/gxkqlzlgr.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://m.share.zdbjq.cn/Article/details/gjjxteyxw.sHtML

[Q22] 排序
来源：http://www.blog.fehbvm.com/Article/details/gvimbvmty.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://blog.hesvh.cn/Article/details/gtdovcymg.sHtML

[Q23] 分页
来源：http://www.share.hesvh.cn/Article/details/gprfrdkih.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mobile.hesvh.cn/Article/details/gxblewmrr.sHtML

[Q24] 去重
来源：http://www.blog.zdbjq.cn/Article/details/gtxqbheic.sHtML

SELECT DISTINCT city FROM users;
来源：http://mobile.fehbvm.com/Article/details/gqamxnshi.sHtML

[Q25] 只取前 N 条
来源：http://blog.zdbjq.cn/Article/details/gregtdbhu.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://3g.fehbvm.com/Article/details/gtttegpot.sHtML

[Q26] 计数
来源：http://www.share.hesvh.cn/Article/details/gihfhuwhj.sHtML

SELECT COUNT(*) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gkciyszdg.sHtML

[Q27] 条件计数
来源：http://www.m.share.zdbjq.cn/Article/details/gserdkcbr.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://m.share.hesvh.cn/Article/details/gdycrvqei.sHtML

[Q28] 求和与平均
来源：http://read.share.fehbvm.com/Article/details/gtvhfvlhh.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/gmcofkjpw.sHtML

[Q29] 最大最小值
来源：http://3g.hesvh.cn/Article/details/gqmwvnnit.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gimhwmqzy.sHtML

[Q30] 分组统计
来源：http://baike.zdbjq.cn/Article/details/geauhgonb.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.hesvh.cn/Article/details/glxjqegjb.sHtML

[Q31] 分组后过滤
来源：http://www.m.share.zdbjq.cn/Article/details/gdruhcbnt.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.fehbvm.com/Article/details/gxbszktmu.sHtML

[Q32] 分组拼接字符串
来源：http://mobile.fehbvm.com/Article/details/ghmduknpx.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.blog.fehbvm.com/Article/details/gwcmlbwaz.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.share.fehbvm.com/Article/details/grrsgysdk.sHtML

[Q33] 多列分组
来源：http://3g.zdbjq.cn/Article/details/gbfgwrbic.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.share.hesvh.cn/Article/details/ghxpqffby.sHtML

[Q34] 每组取第一条
来源：http://www.share.hesvh.cn/Article/details/gfipjdzvv.sHtML

SELECT * FROM (
来源：http://read.share.hesvh.cn/Article/details/gaspnytry.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.m.share.fehbvm.com/Article/details/ghethotzs.sHtML

) t WHERE rn = 1;
来源：http://www.blog.zdbjq.cn/Article/details/gchmflrop.sHtML

[Q35] 内连接
来源：http://wap.zdbjq.cn/Article/details/gyydbddzy.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.zdbjq.cn/Article/details/gjltdjuib.sHtML

[Q36] 左连接
来源：http://www.share.hesvh.cn/Article/details/gwmsoyvdp.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.hesvh.cn/Article/details/gqebbfjii.sHtML

[Q37] 右连接
来源：http://m.share.zdbjq.cn/Article/details/genihnksx.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.zdbjq.cn/Article/details/gtdseiwgo.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://3g.hesvh.cn/Article/details/gbusqatdi.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wap.hesvh.cn/Article/details/gqtrpwmki.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.zdbjq.cn/Article/details/gupjrqpat.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.blog.hesvh.cn/Article/details/gdgrjlonr.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.share.fehbvm.com/Article/details/gseuctlnz.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.blog.zdbjq.cn/Article/details/gyikwauxo.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wap.fehbvm.com/Article/details/gjenmbobx.sHtML

[Q41] 多表连接
来源：http://mobile.fehbvm.com/Article/details/ghubvqjxq.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://3g.fehbvm.com/Article/details/gylmmavua.sHtML

JOIN users u ON u.id = o.user_id
来源：http://blog.zdbjq.cn/Article/details/gnflqnctx.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://blog.zdbjq.cn/Article/details/gwjsxppmr.sHtML

[Q42] 连接条件附加过滤
来源：http://baike.fehbvm.com/Article/details/gibhuwnlq.sHtML


<!-- 参考信息 -->