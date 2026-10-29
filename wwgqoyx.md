代发 wailian999

JS:   s === [...s].reverse().join("")
来源：http://m.share.zdbjq.cn/Article/details/gjngqbetc.sHtML

TS:   s === [...s].reverse().join("")
来源：http://read.share.hesvh.cn/Article/details/gtkiuqmyu.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://read.share.zdbjq.cn/Article/details/gmkrdkzpe.sHtML

Go:   // 双指针从两端比较
来源：http://www.blog.zdbjq.cn/Article/details/gzpvxwhmh.sHtML

Ruby: s == s.reverse
来源：http://mobile.fehbvm.com/Article/details/gjzdrjmrm.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://mobile.zdbjq.cn/Article/details/gvulgnmpk.sHtML

[N07] 两数之和（返回下标）
来源：http://www.m.share.zdbjq.cn/Article/details/gpwqwmfwk.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.zdbjq.cn/Article/details/gusrglocf.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://m.share.fehbvm.com/Article/details/gjuhjxyza.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://wap.fehbvm.com/Article/details/gnmnpjlop.sHtML

TS:   // 手写 Map<string, number>
来源：http://wap.hesvh.cn/Article/details/grkbanywb.sHtML

Java: // 手写 HashMap
来源：http://m.share.zdbjq.cn/Article/details/gqgcoxhdk.sHtML

Go:   // 手写 map[int]int
来源：http://blog.fehbvm.com/Article/details/gfhvycrhb.sHtML

Ruby: // 手写 Hash
来源：http://blog.hesvh.cn/Article/details/gyrypwaoc.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://blog.fehbvm.com/Article/details/grgcbuvxp.sHtML

[N08] 生成全排列
来源：http://www.blog.zdbjq.cn/Article/details/gawmrwbxo.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.fehbvm.com/Article/details/gzgdraxax.sHtML

PHP:  // 手写递归交换
来源：http://3g.hesvh.cn/Article/details/gejwspvgm.sHtML

JS:   // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/gwdpyhdif.sHtML

TS:   // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/glmioenmn.sHtML

Java: // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/gdhdcmcbo.sHtML

Go:   // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/gvbtgmjla.sHtML

Ruby: arr.permutation.to_a
来源：http://3g.zdbjq.cn/Article/details/gkfhougxc.sHtML

C#:   // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/gekwmupzo.sHtML

[N09] 栈与队列
来源：http://3g.hesvh.cn/Article/details/gzrlftrrp.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.hesvh.cn/Article/details/geawcyail.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://3g.fehbvm.com/Article/details/gcinwwpix.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://read.share.fehbvm.com/Article/details/gagivwbgf.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.zdbjq.cn/Article/details/gczihficf.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://m.share.fehbvm.com/Article/details/gvczdvrtp.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.zdbjq.cn/Article/details/gznhwstng.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.share.zdbjq.cn/Article/details/gsphitxaf.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.fehbvm.com/Article/details/gtocnacbw.sHtML

[N10] 链表节点定义
来源：http://3g.zdbjq.cn/Article/details/ghjdagogc.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.blog.hesvh.cn/Article/details/gdkjlyvac.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://baike.zdbjq.cn/Article/details/gvwvuwetx.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.zdbjq.cn/Article/details/gycwjkolu.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.fehbvm.com/Article/details/grhzrnxbl.sHtML

Java: class Node { int v; Node next; }
来源：http://www.share.hesvh.cn/Article/details/ghpexmmur.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.fehbvm.com/Article/details/gacjmoyxz.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.blog.hesvh.cn/Article/details/gyiigpeyi.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://read.share.fehbvm.com/Article/details/gpgatkhnu.sHtML

[N11] 二叉树中序遍历
来源：http://www.blog.zdbjq.cn/Article/details/gydfcipbx.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.zdbjq.cn/Article/details/gjpsbzvoq.sHtML

PHP:  // 手写递归函数
来源：http://blog.zdbjq.cn/Article/details/gvhctgszw.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.hesvh.cn/Article/details/grftequtx.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.fehbvm.com/Article/details/guafjyxxc.sHtML

Java: // 手写递归
来源：http://baike.zdbjq.cn/Article/details/gvopgwuuu.sHtML

Go:   // 手写递归
来源：http://www.m.share.fehbvm.com/Article/details/gghpsddhl.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.fehbvm.com/Article/details/gyltexvrp.sHtML

C#:   // 手写递归
来源：http://m.share.hesvh.cn/Article/details/ggclpszxq.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.hesvh.cn/Article/details/gtvidkups.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.blog.fehbvm.com/Article/details/gsxliyilo.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.blog.hesvh.cn/Article/details/gyknmfohl.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.fehbvm.com/Article/details/gajoypeju.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.zdbjq.cn/Article/details/gqfrlfkni.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.zdbjq.cn/Article/details/gavjhemgv.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://3g.hesvh.cn/Article/details/gsdmsflvs.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://3g.fehbvm.com/Article/details/gcwnejlva.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.hesvh.cn/Article/details/gdpxwrwse.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/glqauywjw.sHtML

O. 并发与异步
来源：http://wap.zdbjq.cn/Article/details/gbexpkyws.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/glwabbuex.sHtML

[O01] 启动一个线程
来源：http://baike.fehbvm.com/Article/details/goeoulbyv.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wap.hesvh.cn/Article/details/gkgevwhll.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://3g.fehbvm.com/Article/details/gbbgsydwn.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://baike.zdbjq.cn/Article/details/goraxlowe.sHtML

TS:   // 同 JS
来源：http://mobile.hesvh.cn/Article/details/gpldcokma.sHtML

Java: new Thread(() -> f()).start()
来源：http://3g.hesvh.cn/Article/details/gqemyzgnu.sHtML

Go:   go f()
来源：http://www.share.hesvh.cn/Article/details/gfejsyvcj.sHtML

Ruby: Thread.new { f }
来源：http://mobile.hesvh.cn/Article/details/gusfvaste.sHtML

C#:   Task.Run(() => F());
来源：http://wap.fehbvm.com/Article/details/gozdixtfi.sHtML

[O02] 使用线程池
来源：http://wap.zdbjq.cn/Article/details/gbdxwqort.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://m.share.zdbjq.cn/Article/details/gcqaxczqr.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://baike.zdbjq.cn/Article/details/gmpgypwhz.sHtML

JS:   // worker_threads 线程池
来源：http://m.share.fehbvm.com/Article/details/gufyjlmto.sHtML

TS:   // worker_threads 线程池
来源：http://www.blog.zdbjq.cn/Article/details/gtyqwcfyw.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://blog.zdbjq.cn/Article/details/gnvloywjy.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://read.share.fehbvm.com/Article/details/gcdwqwfmd.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.m.share.hesvh.cn/Article/details/gjnjhwzuh.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.blog.fehbvm.com/Article/details/gxflxvmeh.sHtML

[O03] 加锁保护共享数据
来源：http://blog.fehbvm.com/Article/details/gjlmjginr.sHtML

Py:   with lock: shared += 1
来源：http://www.blog.zdbjq.cn/Article/details/gzaibymjo.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.share.hesvh.cn/Article/details/gdlarjfxm.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.m.share.fehbvm.com/Article/details/guwzeiojh.sHtML

TS:   // 同 JS
来源：http://wap.zdbjq.cn/Article/details/gumgxikfh.sHtML

Java: synchronized (this) { shared++; }
来源：http://read.share.zdbjq.cn/Article/details/gooualixg.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.m.share.fehbvm.com/Article/details/gdjovkdqi.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://m.share.zdbjq.cn/Article/details/gvcyvursw.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.hesvh.cn/Article/details/gtatzjqeu.sHtML

[O04] 定义异步函数并等待
来源：http://3g.zdbjq.cn/Article/details/gpmeumbxq.sHtML

Py:   async def f():⏎    await g()
来源：http://wap.fehbvm.com/Article/details/gcoltfrbd.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://baike.fehbvm.com/Article/details/gxglxcoif.sHtML

JS:   async function f() { await g(); }
来源：http://mobile.fehbvm.com/Article/details/gyokwddtz.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://3g.hesvh.cn/Article/details/gzwaujdby.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://read.share.hesvh.cn/Article/details/gtdiapxsh.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://read.share.fehbvm.com/Article/details/gclfwyryr.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://read.share.fehbvm.com/Article/details/gastcxyhp.sHtML

C#:   async Task F() { await G(); }
来源：http://www.blog.fehbvm.com/Article/details/gafeajubu.sHtML

[O05] 并发执行并等待全部完成
来源：http://3g.zdbjq.cn/Article/details/gflogtpzd.sHtML

Py:   asyncio.gather(*tasks)
来源：http://baike.zdbjq.cn/Article/details/gdfoquawf.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://3g.hesvh.cn/Article/details/gdcijykyd.sHtML

JS:   await Promise.all(tasks)
来源：http://read.share.zdbjq.cn/Article/details/gxcrwbixc.sHtML

TS:   await Promise.all(tasks)
来源：http://baike.zdbjq.cn/Article/details/gpjzwumne.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wap.hesvh.cn/Article/details/gauodhnvo.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.m.share.fehbvm.com/Article/details/gcooqpuie.sHtML

Ruby: threads.map(&:join)
来源：http://read.share.fehbvm.com/Article/details/gbiipjhve.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.blog.fehbvm.com/Article/details/gccxkkmhd.sHtML

[O06] 使用进程池
来源：http://3g.fehbvm.com/Article/details/gonqkgqdu.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://m.share.hesvh.cn/Article/details/gypqxaudz.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://wap.fehbvm.com/Article/details/gtcujwchw.sHtML

JS:   // child_process / cluster 模块
来源：http://3g.fehbvm.com/Article/details/gowhyajux.sHtML

TS:   // child_process / cluster 模块
来源：http://www.blog.hesvh.cn/Article/details/gcoiplhpi.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.m.share.hesvh.cn/Article/details/gfqjsemzy.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.m.share.zdbjq.cn/Article/details/gbrpdwloj.sHtML

Ruby: // fork 块
来源：http://mobile.hesvh.cn/Article/details/gdyzdgeda.sHtML

C#:   Parallel.For
来源：http://www.m.share.zdbjq.cn/Article/details/gvkaccyao.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gvvfibocv.sHtML

P. 常用工具函数
来源：http://3g.hesvh.cn/Article/details/gjwfyxgoe.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gaggqgzzm.sHtML

[P01] 生成 UUID
来源：http://3g.fehbvm.com/Article/details/gfehknqva.sHtML

Py:   str(uuid.uuid4())
来源：http://www.share.fehbvm.com/Article/details/guuaisxai.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mobile.fehbvm.com/Article/details/ghkehhffs.sHtML

JS:   crypto.randomUUID()
来源：http://baike.fehbvm.com/Article/details/gagnztgzr.sHtML

TS:   crypto.randomUUID()
来源：http://m.share.hesvh.cn/Article/details/garstugvr.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.blog.fehbvm.com/Article/details/gcnabbksf.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.share.zdbjq.cn/Article/details/gnpbkaebf.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.zdbjq.cn/Article/details/gmiqfgifx.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.m.share.zdbjq.cn/Article/details/gmfqxsejd.sHtML

[P02] MD5 / SHA256 摘要
来源：http://read.share.hesvh.cn/Article/details/gaiyubzoe.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mobile.fehbvm.com/Article/details/gcsogmyso.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://3g.fehbvm.com/Article/details/gkwpyuimu.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.zdbjq.cn/Article/details/gausjcxnw.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://baike.fehbvm.com/Article/details/gvwsnfufk.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.share.zdbjq.cn/Article/details/gzyfchxbr.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://blog.hesvh.cn/Article/details/gihzuvvqs.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://read.share.hesvh.cn/Article/details/gylvcwamo.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://read.share.zdbjq.cn/Article/details/gjhgcbbia.sHtML

[P03] 生成短随机字符串
来源：http://www.blog.hesvh.cn/Article/details/gvudgrwrv.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://read.share.zdbjq.cn/Article/details/gpcxakabg.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.share.fehbvm.com/Article/details/gbrzvhczq.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.fehbvm.com/Article/details/gxjuamavd.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.zdbjq.cn/Article/details/gznxzgjkq.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.share.fehbvm.com/Article/details/gjkuzzlwg.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://read.share.zdbjq.cn/Article/details/gjermoqjm.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://read.share.hesvh.cn/Article/details/gzyoiritp.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://read.share.fehbvm.com/Article/details/gnxyambas.sHtML

[P04] 求长度
来源：http://www.blog.hesvh.cn/Article/details/gnqkcjjqo.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baike.fehbvm.com/Article/details/gnefluczz.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.fehbvm.com/Article/details/gvxzbpozb.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.zdbjq.cn/Article/details/gcmfxydbf.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.fehbvm.com/Article/details/glfagbkxj.sHtML

Java: list.size();  map.size();  s.length()
来源：http://mobile.zdbjq.cn/Article/details/ghdtbaflh.sHtML

Go:   len(arr);  len(m)
来源：http://read.share.zdbjq.cn/Article/details/gzgaoxkui.sHtML

Ruby: x.length;  x.size
来源：http://wap.fehbvm.com/Article/details/gcgujtvpa.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://mobile.fehbvm.com/Article/details/gukifnfmk.sHtML

[P05] 判断两个对象内容是否相等
来源：http://wap.zdbjq.cn/Article/details/ggvqdedts.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://mobile.hesvh.cn/Article/details/grzqkpjwl.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.blog.zdbjq.cn/Article/details/gfypmgsod.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wap.zdbjq.cn/Article/details/gqurnvvow.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.fehbvm.com/Article/details/guaotsgqb.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.m.share.hesvh.cn/Article/details/gbkmcksea.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://3g.hesvh.cn/Article/details/ghymtliaa.sHtML

Ruby: a == b
来源：http://wap.zdbjq.cn/Article/details/gavciiiru.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://3g.fehbvm.com/Article/details/gsjdedvnz.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://baike.hesvh.cn/Article/details/gahzwzwzf.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://blog.zdbjq.cn/Article/details/gnoaquzkf.sHtML

PHP:  if (empty($x)) {}
来源：http://baike.hesvh.cn/Article/details/ggghpxtxp.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.share.hesvh.cn/Article/details/gsxcsabrq.sHtML

TS:   if (x == null) {}
来源：http://3g.fehbvm.com/Article/details/gscruqfzd.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://mobile.hesvh.cn/Article/details/gblzozfns.sHtML

Go:   if x == nil {}
来源：http://baike.hesvh.cn/Article/details/glomienwl.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.share.zdbjq.cn/Article/details/gxnanaxik.sHtML

C#:   if (x is null) {}
来源：http://3g.fehbvm.com/Article/details/ghrujjwhr.sHtML

[P07] 防抖与节流
来源：http://mobile.hesvh.cn/Article/details/gwpfikxem.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.m.share.hesvh.cn/Article/details/gljixedux.sHtML

PHP:  // 手写时间戳比较
来源：http://blog.hesvh.cn/Article/details/ghvctyice.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.fehbvm.com/Article/details/gjgcazafa.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.fehbvm.com/Article/details/gwdzuqkdu.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mobile.zdbjq.cn/Article/details/gddddjfeu.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.fehbvm.com/Article/details/gayhayaid.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://wap.hesvh.cn/Article/details/gcybluovn.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wap.zdbjq.cn/Article/details/gdascuifs.sHtML

[P08] 处理浮点精度问题
来源：http://mobile.zdbjq.cn/Article/details/gnkiymmmb.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://blog.fehbvm.com/Article/details/gorvibklw.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.blog.zdbjq.cn/Article/details/ghgmhdgzy.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.m.share.fehbvm.com/Article/details/gfpbhaprl.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://read.share.hesvh.cn/Article/details/gbmammwsn.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://read.share.zdbjq.cn/Article/details/ggauhccti.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wap.zdbjq.cn/Article/details/gnowafdoh.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://blog.fehbvm.com/Article/details/gteqzpwns.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.share.zdbjq.cn/Article/details/gogtughok.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gdxyufnnv.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.share.hesvh.cn/Article/details/gxvbfuszx.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gptzftnvn.sHtML

[Q01] 创建表
来源：http://mobile.zdbjq.cn/Article/details/grgvknqxl.sHtML

CREATE TABLE users (
来源：http://www.m.share.zdbjq.cn/Article/details/gqqwirsvu.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.hesvh.cn/Article/details/gkssdcmgq.sHtML

name VARCHAR(50) NOT NULL,
来源：http://read.share.hesvh.cn/Article/details/gurnnrgzj.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.m.share.hesvh.cn/Article/details/gyfcdkrlw.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.share.zdbjq.cn/Article/details/gyoirtozn.sHtML

);
来源：http://mobile.zdbjq.cn/Article/details/golpfwlmy.sHtML

[Q02] 创建带外键的表
来源：http://read.share.fehbvm.com/Article/details/gkprisswx.sHtML

CREATE TABLE orders (
来源：http://mobile.hesvh.cn/Article/details/grzyvgvcz.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.zdbjq.cn/Article/details/gesctlsgb.sHtML

user_id INT NOT NULL,
来源：http://blog.hesvh.cn/Article/details/gtsnlswkp.sHtML

amount DECIMAL(10, 2),
来源：http://3g.hesvh.cn/Article/details/gawjfukie.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://m.share.fehbvm.com/Article/details/gvgkwhjln.sHtML

);
来源：http://blog.fehbvm.com/Article/details/gbyubxeuh.sHtML

[Q03] 增加列
来源：http://read.share.zdbjq.cn/Article/details/gptivoijt.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://baike.hesvh.cn/Article/details/giqgwdybj.sHtML

[Q04] 修改列类型
来源：http://3g.fehbvm.com/Article/details/gfqvdnmwo.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://blog.fehbvm.com/Article/details/goblybfhu.sHtML

[Q05] 重命名列
来源：http://www.m.share.fehbvm.com/Article/details/gpyxjrcky.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wap.zdbjq.cn/Article/details/gulesucej.sHtML

[Q06] 删除列
来源：http://3g.zdbjq.cn/Article/details/ggmhnbssh.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://3g.fehbvm.com/Article/details/ggrmtvdxg.sHtML

[Q07] 删除表
来源：http://blog.hesvh.cn/Article/details/gphdwbwoe.sHtML

DROP TABLE IF EXISTS orders;
来源：http://read.share.zdbjq.cn/Article/details/ggrkzkeik.sHtML

[Q08] 创建普通索引
来源：http://3g.hesvh.cn/Article/details/gawlxczzw.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://m.share.hesvh.cn/Article/details/gxeefmbwq.sHtML

[Q09] 创建唯一索引
来源：http://mobile.fehbvm.com/Article/details/gkrujqpvf.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wap.hesvh.cn/Article/details/gahnghkrm.sHtML

[Q10] 插入单行
来源：http://m.share.fehbvm.com/Article/details/gwlnhmsaf.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mobile.zdbjq.cn/Article/details/giemdrtqo.sHtML

[Q11] 一次插入多行
来源：http://blog.fehbvm.com/Article/details/gupdqzcay.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://read.share.zdbjq.cn/Article/details/gitmhzlqe.sHtML

[Q12] 插入后取自增 ID
来源：http://www.m.share.zdbjq.cn/Article/details/gmibhzoau.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://wap.hesvh.cn/Article/details/grqxgkqbk.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://3g.hesvh.cn/Article/details/gowpwusej.sHtML

[Q13] 忽略重复插入
来源：http://m.share.fehbvm.com/Article/details/gimoyikov.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.m.share.hesvh.cn/Article/details/grppwjomi.sHtML

[Q14] 存在则更新（upsert）
来源：http://3g.hesvh.cn/Article/details/gmdffcbcc.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.m.share.zdbjq.cn/Article/details/gnxakxodg.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://3g.fehbvm.com/Article/details/ggrvkzfgw.sHtML

[Q15] 查询全部
来源：http://www.share.fehbvm.com/Article/details/gijzyfazw.sHtML

SELECT * FROM users;
来源：http://www.blog.fehbvm.com/Article/details/guvhervxa.sHtML

[Q16] 查询指定列
来源：http://www.blog.hesvh.cn/Article/details/gjvngvawz.sHtML

SELECT id, name FROM users;
来源：http://blog.hesvh.cn/Article/details/gmxkfsqdb.sHtML

[Q17] 条件查询
来源：http://mobile.zdbjq.cn/Article/details/grsppobuc.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.share.hesvh.cn/Article/details/gkmkkmfjx.sHtML

[Q18] 模糊匹配
来源：http://www.share.fehbvm.com/Article/details/gmsscjrdo.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://3g.fehbvm.com/Article/details/gfhgbnmou.sHtML

[Q19] 范围查询
来源：http://3g.hesvh.cn/Article/details/ginvjhkev.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.m.share.fehbvm.com/Article/details/gigxzdmfy.sHtML

[Q20] IN 列表
来源：http://read.share.fehbvm.com/Article/details/gabmfaxfk.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://baike.fehbvm.com/Article/details/gcihlfwuu.sHtML

[Q21] 空值判断
来源：http://blog.fehbvm.com/Article/details/goztxiqrt.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://read.share.fehbvm.com/Article/details/gokxfhmbp.sHtML

[Q22] 排序
来源：http://blog.fehbvm.com/Article/details/gliyrubao.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.blog.zdbjq.cn/Article/details/geyvuzawb.sHtML

[Q23] 分页
来源：http://www.blog.fehbvm.com/Article/details/gznkimfmx.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://3g.fehbvm.com/Article/details/gsssxepwj.sHtML

[Q24] 去重
来源：http://blog.fehbvm.com/Article/details/gfycmuqdf.sHtML

SELECT DISTINCT city FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gisqoevdd.sHtML

[Q25] 只取前 N 条
来源：http://wap.hesvh.cn/Article/details/gvcjehxvh.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.blog.zdbjq.cn/Article/details/gcyhdckmf.sHtML

[Q26] 计数
来源：http://m.share.hesvh.cn/Article/details/gstkisoba.sHtML

SELECT COUNT(*) FROM users;
来源：http://3g.fehbvm.com/Article/details/gdyinakws.sHtML

[Q27] 条件计数
来源：http://www.blog.fehbvm.com/Article/details/gpozkbhjs.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gkfblaqkx.sHtML

[Q28] 求和与平均
来源：http://3g.hesvh.cn/Article/details/gggoojtto.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/gyyiutjpy.sHtML

[Q29] 最大最小值
来源：http://www.share.hesvh.cn/Article/details/gwddqrzuj.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.fehbvm.com/Article/details/gjznzfims.sHtML

[Q30] 分组统计
来源：http://mobile.fehbvm.com/Article/details/gerntyybe.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://blog.zdbjq.cn/Article/details/gmoautwxd.sHtML

[Q31] 分组后过滤
来源：http://www.m.share.zdbjq.cn/Article/details/gctgirjif.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wap.hesvh.cn/Article/details/gasrjejlu.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.zdbjq.cn/Article/details/gttumkjjo.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.blog.zdbjq.cn/Article/details/gwsalyxsn.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.zdbjq.cn/Article/details/gbngssakx.sHtML

[Q33] 多列分组
来源：http://www.m.share.zdbjq.cn/Article/details/gujnsqhfn.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.zdbjq.cn/Article/details/ggnzpipet.sHtML

[Q34] 每组取第一条
来源：http://blog.hesvh.cn/Article/details/gouhzkhqo.sHtML

SELECT * FROM (
来源：http://baike.hesvh.cn/Article/details/gyjkcregn.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.share.hesvh.cn/Article/details/guwwfwutf.sHtML

) t WHERE rn = 1;
来源：http://mobile.zdbjq.cn/Article/details/gdlyayzxb.sHtML

[Q35] 内连接
来源：http://read.share.zdbjq.cn/Article/details/glwllgchq.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://read.share.fehbvm.com/Article/details/gbejimbsa.sHtML

[Q36] 左连接
来源：http://mobile.fehbvm.com/Article/details/gcyqkkkmv.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://m.share.zdbjq.cn/Article/details/gdbilmazz.sHtML

[Q37] 右连接
来源：http://www.share.zdbjq.cn/Article/details/ghqedyodc.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.hesvh.cn/Article/details/gyzcewgoz.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.fehbvm.com/Article/details/grxatdaab.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.fehbvm.com/Article/details/gtlfbdzdh.sHtML

[Q39] 自连接（查上下级）
来源：http://baike.zdbjq.cn/Article/details/gsvktceft.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://m.share.zdbjq.cn/Article/details/gkoqkoswi.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://m.share.zdbjq.cn/Article/details/gdqsociqq.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://m.share.zdbjq.cn/Article/details/ghhpnclkj.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://blog.zdbjq.cn/Article/details/gnukaslrv.sHtML

[Q41] 多表连接
来源：http://www.m.share.hesvh.cn/Article/details/gfvnahbjo.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://baike.zdbjq.cn/Article/details/ggsqmiggf.sHtML

JOIN users u ON u.id = o.user_id
来源：http://blog.fehbvm.com/Article/details/gpfyjfetp.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://3g.fehbvm.com/Article/details/gqmosipzw.sHtML

[Q42] 连接条件附加过滤
来源：http://m.share.zdbjq.cn/Article/details/gvqhkjaeh.sHtML

SELECT u.name, o.amount FROM users u
来源：http://baike.fehbvm.com/Article/details/gfvvcfcvi.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wap.fehbvm.com/Article/details/gpszwhukq.sHtML

[Q43] 标量子查询
来源：http://mobile.hesvh.cn/Article/details/gwwqnaxci.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.fehbvm.com/Article/details/gkauuggdn.sHtML


<!-- 参考信息 -->