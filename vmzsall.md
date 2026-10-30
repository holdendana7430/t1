代发 wailian999

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wap.fehbvm.com/Article/details/gctmoqwzl.sHtML

[N06] 判断回文字符串
来源：http://baike.fehbvm.com/Article/details/gslbehkiy.sHtML

Py:   s == s[::-1]
来源：http://www.m.share.hesvh.cn/Article/details/gfurvairl.sHtML

PHP:  $s === strrev($s);
来源：http://wap.fehbvm.com/Article/details/gbmoiqduq.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.hesvh.cn/Article/details/gxakxufta.sHtML

TS:   s === [...s].reverse().join("")
来源：http://blog.hesvh.cn/Article/details/gtfvkclml.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.share.hesvh.cn/Article/details/gmgzexzzk.sHtML

Go:   // 双指针从两端比较
来源：http://mobile.fehbvm.com/Article/details/gteghybpf.sHtML

Ruby: s == s.reverse
来源：http://read.share.hesvh.cn/Article/details/gnqgcayfc.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://mobile.zdbjq.cn/Article/details/gcsggnjfz.sHtML

[N07] 两数之和（返回下标）
来源：http://read.share.zdbjq.cn/Article/details/gjlkdrila.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.zdbjq.cn/Article/details/gzjhpjvsu.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://m.share.zdbjq.cn/Article/details/gnsngtjcf.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.blog.zdbjq.cn/Article/details/gpjvlldzc.sHtML

TS:   // 手写 Map<string, number>
来源：http://3g.fehbvm.com/Article/details/gptepkluh.sHtML

Java: // 手写 HashMap
来源：http://www.share.zdbjq.cn/Article/details/gcanitydk.sHtML

Go:   // 手写 map[int]int
来源：http://baike.zdbjq.cn/Article/details/gmtripvmn.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.fehbvm.com/Article/details/gybsqlgfo.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.share.fehbvm.com/Article/details/goszhndtb.sHtML

[N08] 生成全排列
来源：http://baike.hesvh.cn/Article/details/gfclbniyn.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.fehbvm.com/Article/details/gqeowqisz.sHtML

PHP:  // 手写递归交换
来源：http://www.m.share.hesvh.cn/Article/details/gtxnvgsdp.sHtML

JS:   // 手写回溯递归
来源：http://www.blog.fehbvm.com/Article/details/gtwiuqucp.sHtML

TS:   // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/gcbrwtaal.sHtML

Java: // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/gtgukxiwe.sHtML

Go:   // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/gjcnpvsjh.sHtML

Ruby: arr.permutation.to_a
来源：http://www.blog.fehbvm.com/Article/details/gtsmkprnf.sHtML

C#:   // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/gasgtobfb.sHtML

[N09] 栈与队列
来源：http://read.share.fehbvm.com/Article/details/ggdrrqnvk.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.fehbvm.com/Article/details/gdchuwwqg.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://blog.hesvh.cn/Article/details/gidpxssyv.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.share.hesvh.cn/Article/details/ggfzlrdnz.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.m.share.fehbvm.com/Article/details/gpqkpcxha.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://baike.zdbjq.cn/Article/details/gwbmzlpfc.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://m.share.hesvh.cn/Article/details/gkeqbqmpa.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.zdbjq.cn/Article/details/ghvjyhuwh.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://3g.hesvh.cn/Article/details/grzkgahxp.sHtML

[N10] 链表节点定义
来源：http://www.blog.zdbjq.cn/Article/details/gndmecucn.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mobile.hesvh.cn/Article/details/gthfaetio.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://wap.hesvh.cn/Article/details/gwwsupkce.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wap.fehbvm.com/Article/details/gldddrizz.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.hesvh.cn/Article/details/geqdhkute.sHtML

Java: class Node { int v; Node next; }
来源：http://mobile.hesvh.cn/Article/details/gjkcwlwhp.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://blog.zdbjq.cn/Article/details/ggzxvmyjm.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.zdbjq.cn/Article/details/gahdrhaiq.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://wap.fehbvm.com/Article/details/gewvcguma.sHtML

[N11] 二叉树中序遍历
来源：http://3g.hesvh.cn/Article/details/gydgdyzlh.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.share.hesvh.cn/Article/details/gqsgdoxoj.sHtML

PHP:  // 手写递归函数
来源：http://read.share.fehbvm.com/Article/details/gttqorsys.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.hesvh.cn/Article/details/gepbtvcla.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.hesvh.cn/Article/details/gxctvpfso.sHtML

Java: // 手写递归
来源：http://www.blog.hesvh.cn/Article/details/gxxcommps.sHtML

Go:   // 手写递归
来源：http://www.blog.hesvh.cn/Article/details/gxcskwuwm.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.m.share.hesvh.cn/Article/details/gcstnzewe.sHtML

C#:   // 手写递归
来源：http://wap.fehbvm.com/Article/details/gjmhybojq.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://read.share.hesvh.cn/Article/details/gidrkueqb.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://read.share.fehbvm.com/Article/details/guhtxevzb.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.m.share.fehbvm.com/Article/details/gaakvlabt.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.zdbjq.cn/Article/details/ghrhzaseh.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.zdbjq.cn/Article/details/glzefwpmt.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.zdbjq.cn/Article/details/gvzshjjfb.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mobile.fehbvm.com/Article/details/gheznoksq.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://baike.hesvh.cn/Article/details/gadbrilkn.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.hesvh.cn/Article/details/geetafont.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gdigrffld.sHtML

O. 并发与异步
来源：http://m.share.fehbvm.com/Article/details/ggarleeap.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gkfxezlqd.sHtML

[O01] 启动一个线程
来源：http://3g.fehbvm.com/Article/details/gdggjxfnz.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.zdbjq.cn/Article/details/gieaadevc.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.hesvh.cn/Article/details/gnxpulfgv.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://baike.zdbjq.cn/Article/details/gbzrvhohw.sHtML

TS:   // 同 JS
来源：http://m.share.fehbvm.com/Article/details/glmcyiizp.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.share.zdbjq.cn/Article/details/ggdjwzcid.sHtML

Go:   go f()
来源：http://www.m.share.zdbjq.cn/Article/details/gbesdtapb.sHtML

Ruby: Thread.new { f }
来源：http://www.m.share.zdbjq.cn/Article/details/gsktldtgc.sHtML

C#:   Task.Run(() => F());
来源：http://wap.fehbvm.com/Article/details/ggpfiyvpp.sHtML

[O02] 使用线程池
来源：http://baike.hesvh.cn/Article/details/gmkuixtxk.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://baike.zdbjq.cn/Article/details/guzjbhfqq.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.zdbjq.cn/Article/details/grujdqgro.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.zdbjq.cn/Article/details/gibwojbjm.sHtML

TS:   // worker_threads 线程池
来源：http://www.m.share.hesvh.cn/Article/details/gnfzziozy.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.m.share.hesvh.cn/Article/details/gnzfuylrd.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.m.share.fehbvm.com/Article/details/grvkwzsxm.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://3g.fehbvm.com/Article/details/gxhhubxfq.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://read.share.zdbjq.cn/Article/details/gdarlyxoe.sHtML

[O03] 加锁保护共享数据
来源：http://m.share.hesvh.cn/Article/details/glaxgersp.sHtML

Py:   with lock: shared += 1
来源：http://blog.hesvh.cn/Article/details/gujinrjlj.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://wap.zdbjq.cn/Article/details/ggbdqftfl.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.m.share.zdbjq.cn/Article/details/gyxhcfijd.sHtML

TS:   // 同 JS
来源：http://3g.zdbjq.cn/Article/details/ghbmyehkh.sHtML

Java: synchronized (this) { shared++; }
来源：http://read.share.fehbvm.com/Article/details/glgsnypzl.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://baike.zdbjq.cn/Article/details/gnsapxkfk.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://read.share.hesvh.cn/Article/details/gwdkjdpgd.sHtML

C#:   lock (gate) { shared++; }
来源：http://m.share.fehbvm.com/Article/details/ggnfesxtx.sHtML

[O04] 定义异步函数并等待
来源：http://3g.zdbjq.cn/Article/details/gwlltcnsc.sHtML

Py:   async def f():⏎    await g()
来源：http://www.share.hesvh.cn/Article/details/galgmgtpy.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mobile.fehbvm.com/Article/details/gmazranun.sHtML

JS:   async function f() { await g(); }
来源：http://wap.fehbvm.com/Article/details/gfpzcsylw.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gnubtrcoz.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.blog.hesvh.cn/Article/details/gzwepyqce.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://baike.fehbvm.com/Article/details/gnbfxauun.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.blog.hesvh.cn/Article/details/gopuyuvdg.sHtML

C#:   async Task F() { await G(); }
来源：http://wap.hesvh.cn/Article/details/gshrqtdsf.sHtML

[O05] 并发执行并等待全部完成
来源：http://mobile.hesvh.cn/Article/details/gkojgzvpx.sHtML

Py:   asyncio.gather(*tasks)
来源：http://read.share.hesvh.cn/Article/details/gmwkvgcse.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://m.share.hesvh.cn/Article/details/gfpbxgfyq.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.zdbjq.cn/Article/details/gmtahhkwa.sHtML

TS:   await Promise.all(tasks)
来源：http://baike.fehbvm.com/Article/details/ganuiagcg.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.m.share.zdbjq.cn/Article/details/gczyvfacs.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://3g.zdbjq.cn/Article/details/gnqfdzlti.sHtML

Ruby: threads.map(&:join)
来源：http://mobile.fehbvm.com/Article/details/gqethydfu.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://3g.hesvh.cn/Article/details/grvpwjhsz.sHtML

[O06] 使用进程池
来源：http://wap.fehbvm.com/Article/details/guzmiaxvd.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.share.hesvh.cn/Article/details/gmbxgdilj.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.blog.fehbvm.com/Article/details/gzxdkllop.sHtML

JS:   // child_process / cluster 模块
来源：http://baike.fehbvm.com/Article/details/gbzvrswea.sHtML

TS:   // child_process / cluster 模块
来源：http://read.share.hesvh.cn/Article/details/ggcczmzvd.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://read.share.hesvh.cn/Article/details/gadwrqajr.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.share.fehbvm.com/Article/details/gxiaeanru.sHtML

Ruby: // fork 块
来源：http://wap.zdbjq.cn/Article/details/gerztarxf.sHtML

C#:   Parallel.For
来源：http://blog.fehbvm.com/Article/details/gqaqgzlxp.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gixdjxigx.sHtML

P. 常用工具函数
来源：http://blog.hesvh.cn/Article/details/gigehvgeu.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gqsxrwlyc.sHtML

[P01] 生成 UUID
来源：http://baike.hesvh.cn/Article/details/gdyrtqcad.sHtML

Py:   str(uuid.uuid4())
来源：http://www.m.share.fehbvm.com/Article/details/gxkihommc.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.blog.zdbjq.cn/Article/details/gpnceseue.sHtML

JS:   crypto.randomUUID()
来源：http://www.share.fehbvm.com/Article/details/grofbymfm.sHtML

TS:   crypto.randomUUID()
来源：http://www.blog.fehbvm.com/Article/details/gvycmylrx.sHtML

Java: UUID.randomUUID().toString()
来源：http://3g.fehbvm.com/Article/details/gjkvreedd.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.share.fehbvm.com/Article/details/gwqtjnkrl.sHtML

Ruby: SecureRandom.uuid
来源：http://www.blog.fehbvm.com/Article/details/gqkcbhcti.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://wap.zdbjq.cn/Article/details/gxexbrkqs.sHtML

[P02] MD5 / SHA256 摘要
来源：http://baike.zdbjq.cn/Article/details/gaduxbsmo.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://m.share.zdbjq.cn/Article/details/gwrspdzfy.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://blog.zdbjq.cn/Article/details/gcufkejjp.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wap.zdbjq.cn/Article/details/gtujfcpyr.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.share.fehbvm.com/Article/details/gomnyjrid.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.blog.fehbvm.com/Article/details/grlgxzmoq.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://read.share.fehbvm.com/Article/details/gkgtkwcrj.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.blog.hesvh.cn/Article/details/grioaoetx.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.blog.hesvh.cn/Article/details/gimsgpvud.sHtML

[P03] 生成短随机字符串
来源：http://baike.fehbvm.com/Article/details/gmjzbsyxv.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://baike.hesvh.cn/Article/details/gwmhydbes.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.blog.hesvh.cn/Article/details/gzltvbuyq.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gvdzayegt.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.hesvh.cn/Article/details/gladqxitx.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.share.hesvh.cn/Article/details/gqyervoee.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://m.share.zdbjq.cn/Article/details/giuxgmlrf.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://mobile.fehbvm.com/Article/details/gowsxcqxs.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://baike.hesvh.cn/Article/details/gthtluuvi.sHtML

[P04] 求长度
来源：http://m.share.hesvh.cn/Article/details/gvjvgrgvk.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.blog.hesvh.cn/Article/details/ggdbjkjkk.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.zdbjq.cn/Article/details/gdfevdrbu.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.hesvh.cn/Article/details/gxjklbzca.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.fehbvm.com/Article/details/gezqxsrbp.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.blog.hesvh.cn/Article/details/gropajyrd.sHtML

Go:   len(arr);  len(m)
来源：http://www.blog.fehbvm.com/Article/details/gqassqqux.sHtML

Ruby: x.length;  x.size
来源：http://www.blog.zdbjq.cn/Article/details/gupzjxglq.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://wap.fehbvm.com/Article/details/gzpfjfmuj.sHtML

[P05] 判断两个对象内容是否相等
来源：http://wap.fehbvm.com/Article/details/gbyaywfom.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://blog.fehbvm.com/Article/details/gocmpopat.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://blog.fehbvm.com/Article/details/gblooytwa.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.share.zdbjq.cn/Article/details/gioitpgux.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.zdbjq.cn/Article/details/gwjkwdxgu.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wap.hesvh.cn/Article/details/gxfagebdh.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://wap.hesvh.cn/Article/details/gxngmgnvo.sHtML

Ruby: a == b
来源：http://blog.hesvh.cn/Article/details/gwzcjskjw.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://blog.fehbvm.com/Article/details/gsihdiihv.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.m.share.fehbvm.com/Article/details/gcamzutuf.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://3g.fehbvm.com/Article/details/glnmexvfl.sHtML

PHP:  if (empty($x)) {}
来源：http://wap.zdbjq.cn/Article/details/gnlnnwvkf.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://m.share.zdbjq.cn/Article/details/gjvgtjxry.sHtML

TS:   if (x == null) {}
来源：http://www.share.fehbvm.com/Article/details/gbkteytta.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://wap.fehbvm.com/Article/details/gqqzgxfgx.sHtML

Go:   if x == nil {}
来源：http://baike.zdbjq.cn/Article/details/gxdfiaiky.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.share.zdbjq.cn/Article/details/gmxviqphy.sHtML

C#:   if (x is null) {}
来源：http://www.m.share.hesvh.cn/Article/details/gnurvzblu.sHtML

[P07] 防抖与节流
来源：http://blog.zdbjq.cn/Article/details/gxkcdrkmw.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://3g.zdbjq.cn/Article/details/gkrjwwvmo.sHtML

PHP:  // 手写时间戳比较
来源：http://read.share.fehbvm.com/Article/details/gmjhjsdsx.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.hesvh.cn/Article/details/gjwymmlnt.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.hesvh.cn/Article/details/giitansuc.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://m.share.zdbjq.cn/Article/details/gkzrfxjnm.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://m.share.fehbvm.com/Article/details/gqdtklmss.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.blog.fehbvm.com/Article/details/gluvdhfqg.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://read.share.hesvh.cn/Article/details/guucwmonv.sHtML

[P08] 处理浮点精度问题
来源：http://read.share.fehbvm.com/Article/details/gsepwjjwz.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.blog.fehbvm.com/Article/details/gneazfgsn.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.share.zdbjq.cn/Article/details/gxwvpmbxc.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.fehbvm.com/Article/details/ghuxcdvym.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://baike.zdbjq.cn/Article/details/guaqvsatj.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://m.share.fehbvm.com/Article/details/gajkyzjxl.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://blog.zdbjq.cn/Article/details/gexyjapkc.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.m.share.fehbvm.com/Article/details/gzgreafus.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mobile.zdbjq.cn/Article/details/guxldxxim.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gxsgbocjz.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.share.hesvh.cn/Article/details/gjvxgnnoa.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gjlivyxst.sHtML

[Q01] 创建表
来源：http://www.share.hesvh.cn/Article/details/gkgrhcyin.sHtML

CREATE TABLE users (
来源：http://www.blog.fehbvm.com/Article/details/gvwjrlrbf.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.hesvh.cn/Article/details/gbvmwnpwf.sHtML

name VARCHAR(50) NOT NULL,
来源：http://read.share.hesvh.cn/Article/details/gogfkyzjf.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.m.share.zdbjq.cn/Article/details/galpcrucn.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.m.share.hesvh.cn/Article/details/gaxdzbyoy.sHtML

);
来源：http://blog.fehbvm.com/Article/details/gvdwvznhg.sHtML

[Q02] 创建带外键的表
来源：http://3g.zdbjq.cn/Article/details/gwyjpvtmb.sHtML

CREATE TABLE orders (
来源：http://3g.hesvh.cn/Article/details/gzxjtgfrk.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.hesvh.cn/Article/details/gccvjiali.sHtML

user_id INT NOT NULL,
来源：http://blog.fehbvm.com/Article/details/gpxtbzecw.sHtML

amount DECIMAL(10, 2),
来源：http://m.share.hesvh.cn/Article/details/gnxmzycvj.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.blog.zdbjq.cn/Article/details/gpvlczrux.sHtML

);
来源：http://mobile.hesvh.cn/Article/details/gmiglvfkz.sHtML

[Q03] 增加列
来源：http://read.share.fehbvm.com/Article/details/gnoeugtsz.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.fehbvm.com/Article/details/ghovmjhxn.sHtML

[Q04] 修改列类型
来源：http://m.share.hesvh.cn/Article/details/ggvrtufzz.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mobile.hesvh.cn/Article/details/gqbbudzzm.sHtML

[Q05] 重命名列
来源：http://blog.fehbvm.com/Article/details/gdtwdphuw.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.share.zdbjq.cn/Article/details/gpvfhtwmf.sHtML

[Q06] 删除列
来源：http://blog.fehbvm.com/Article/details/gcahyblma.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://read.share.zdbjq.cn/Article/details/gjsjglfmc.sHtML

[Q07] 删除表
来源：http://www.share.hesvh.cn/Article/details/gfkdhumpt.sHtML

DROP TABLE IF EXISTS orders;
来源：http://blog.zdbjq.cn/Article/details/ggbtwbcnn.sHtML

[Q08] 创建普通索引
来源：http://mobile.zdbjq.cn/Article/details/gkewpiyal.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://blog.zdbjq.cn/Article/details/gymvdjraq.sHtML

[Q09] 创建唯一索引
来源：http://m.share.fehbvm.com/Article/details/geebquaqc.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://blog.fehbvm.com/Article/details/gnkqyrwep.sHtML

[Q10] 插入单行
来源：http://m.share.hesvh.cn/Article/details/ggsubfktv.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.share.zdbjq.cn/Article/details/gkejlbwfn.sHtML

[Q11] 一次插入多行
来源：http://www.blog.fehbvm.com/Article/details/gaqffysky.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.m.share.fehbvm.com/Article/details/gvrmyvlgx.sHtML

[Q12] 插入后取自增 ID
来源：http://read.share.hesvh.cn/Article/details/gwprbwapc.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://3g.hesvh.cn/Article/details/gogykiznj.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.share.hesvh.cn/Article/details/gkzcojtal.sHtML

[Q13] 忽略重复插入
来源：http://wap.fehbvm.com/Article/details/ghrguxpnw.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mobile.zdbjq.cn/Article/details/grfobdcdk.sHtML

[Q14] 存在则更新（upsert）
来源：http://baike.zdbjq.cn/Article/details/gveevdiya.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.m.share.fehbvm.com/Article/details/gwxvbwsjl.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://baike.fehbvm.com/Article/details/gyxwfhcpx.sHtML

[Q15] 查询全部
来源：http://www.share.fehbvm.com/Article/details/gkthmvtbq.sHtML

SELECT * FROM users;
来源：http://read.share.fehbvm.com/Article/details/gyqewojrw.sHtML

[Q16] 查询指定列
来源：http://baike.hesvh.cn/Article/details/gelfsyipy.sHtML

SELECT id, name FROM users;
来源：http://wap.fehbvm.com/Article/details/glqumkyit.sHtML

[Q17] 条件查询
来源：http://www.blog.zdbjq.cn/Article/details/gyakhpkgs.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mobile.hesvh.cn/Article/details/ghlnbdybt.sHtML

[Q18] 模糊匹配
来源：http://read.share.hesvh.cn/Article/details/gwxxlftbf.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://baike.fehbvm.com/Article/details/gvblkwbgq.sHtML

[Q19] 范围查询
来源：http://baike.zdbjq.cn/Article/details/gmwdtenny.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://blog.fehbvm.com/Article/details/gxabnijfy.sHtML

[Q20] IN 列表
来源：http://m.share.hesvh.cn/Article/details/gdwzszxsl.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.zdbjq.cn/Article/details/gnisgnqhi.sHtML

[Q21] 空值判断
来源：http://mobile.zdbjq.cn/Article/details/gysgieeao.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://m.share.zdbjq.cn/Article/details/godyrfflz.sHtML

[Q22] 排序
来源：http://www.share.fehbvm.com/Article/details/gjgzrjjba.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://m.share.zdbjq.cn/Article/details/gxbhkoppm.sHtML

[Q23] 分页
来源：http://wap.hesvh.cn/Article/details/gxqqhpntf.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://blog.fehbvm.com/Article/details/gwyhewdjq.sHtML

[Q24] 去重
来源：http://blog.zdbjq.cn/Article/details/gvuqjexwl.sHtML

SELECT DISTINCT city FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gljyaqgfm.sHtML

[Q25] 只取前 N 条
来源：http://www.blog.hesvh.cn/Article/details/garihmahp.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.blog.fehbvm.com/Article/details/gtajrftsh.sHtML

[Q26] 计数
来源：http://www.m.share.hesvh.cn/Article/details/grsggojqz.sHtML

SELECT COUNT(*) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gzycqgpso.sHtML

[Q27] 条件计数
来源：http://m.share.zdbjq.cn/Article/details/gvnkkreej.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.share.hesvh.cn/Article/details/gkcvwyhkk.sHtML

[Q28] 求和与平均
来源：http://mobile.fehbvm.com/Article/details/ggytexbrq.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://read.share.hesvh.cn/Article/details/gybvvviod.sHtML

[Q29] 最大最小值
来源：http://read.share.zdbjq.cn/Article/details/gpfqqlzwv.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gsavjvrob.sHtML

[Q30] 分组统计
来源：http://wap.fehbvm.com/Article/details/ghmiczfaq.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://blog.hesvh.cn/Article/details/gfsrmsech.sHtML

[Q31] 分组后过滤
来源：http://www.blog.hesvh.cn/Article/details/gnummqpef.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.fehbvm.com/Article/details/ghwitqsff.sHtML

[Q32] 分组拼接字符串
来源：http://www.share.hesvh.cn/Article/details/gujzrrtel.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.m.share.fehbvm.com/Article/details/gofomailh.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.m.share.hesvh.cn/Article/details/ggxgobrxg.sHtML

[Q33] 多列分组
来源：http://www.share.hesvh.cn/Article/details/gddfzklix.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mobile.zdbjq.cn/Article/details/gnfjagood.sHtML

[Q34] 每组取第一条
来源：http://www.blog.fehbvm.com/Article/details/ggnnmcnya.sHtML

SELECT * FROM (
来源：http://blog.zdbjq.cn/Article/details/gxkvenggv.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.m.share.fehbvm.com/Article/details/gchnwziet.sHtML

) t WHERE rn = 1;
来源：http://mobile.zdbjq.cn/Article/details/gnqthkbqq.sHtML

[Q35] 内连接
来源：http://baike.fehbvm.com/Article/details/gdankphza.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://read.share.fehbvm.com/Article/details/grbsussas.sHtML

[Q36] 左连接
来源：http://www.m.share.zdbjq.cn/Article/details/gptmmzocq.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.zdbjq.cn/Article/details/gprejcvjv.sHtML

[Q37] 右连接
来源：http://read.share.fehbvm.com/Article/details/gzhommbit.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.hesvh.cn/Article/details/gdtdmyqnd.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.m.share.fehbvm.com/Article/details/gscpfytub.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mobile.fehbvm.com/Article/details/gyrqygjmf.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.zdbjq.cn/Article/details/gvoweoamm.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.fehbvm.com/Article/details/gnkjmoznm.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.blog.hesvh.cn/Article/details/gyqtfecei.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.fehbvm.com/Article/details/gltbptsry.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://3g.fehbvm.com/Article/details/gzmarjqmr.sHtML

[Q41] 多表连接
来源：http://read.share.zdbjq.cn/Article/details/gnrxsvgph.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.fehbvm.com/Article/details/gihkxicbg.sHtML

JOIN users u ON u.id = o.user_id
来源：http://read.share.zdbjq.cn/Article/details/gzbhchdoc.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://3g.fehbvm.com/Article/details/glahqinir.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.fehbvm.com/Article/details/gkwyqcrkp.sHtML


<!-- 参考信息 -->