代发 wailian999

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://m.share.fehbvm.com/Article/details/glsuyaawc.sHtML

[N06] 判断回文字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gfmlznonj.sHtML

Py:   s == s[::-1]
来源：http://www.m.share.hesvh.cn/Article/details/gnvpgfoun.sHtML

PHP:  $s === strrev($s);
来源：http://3g.zdbjq.cn/Article/details/gadjnftnx.sHtML

JS:   s === [...s].reverse().join("")
来源：http://m.share.fehbvm.com/Article/details/ghjvrrizx.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.hesvh.cn/Article/details/gjgqenifq.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.blog.zdbjq.cn/Article/details/givwiiiff.sHtML

Go:   // 双指针从两端比较
来源：http://www.blog.zdbjq.cn/Article/details/ghnvgudtm.sHtML

Ruby: s == s.reverse
来源：http://blog.zdbjq.cn/Article/details/gtbnschko.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.share.hesvh.cn/Article/details/godkpecsa.sHtML

[N07] 两数之和（返回下标）
来源：http://read.share.fehbvm.com/Article/details/gtmksgpbc.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.fehbvm.com/Article/details/grjgujrou.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://blog.fehbvm.com/Article/details/gvdvgdkyi.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://baike.zdbjq.cn/Article/details/ggyewbfhr.sHtML

TS:   // 手写 Map<string, number>
来源：http://baike.zdbjq.cn/Article/details/gipdnbgno.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.hesvh.cn/Article/details/gdplzeojp.sHtML

Go:   // 手写 map[int]int
来源：http://www.m.share.fehbvm.com/Article/details/gpfsyngoo.sHtML

Ruby: // 手写 Hash
来源：http://3g.fehbvm.com/Article/details/gywdnzjgm.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://m.share.hesvh.cn/Article/details/gwhskjmmo.sHtML

[N08] 生成全排列
来源：http://3g.hesvh.cn/Article/details/gxtdhqcxv.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.fehbvm.com/Article/details/ggfxehohs.sHtML

PHP:  // 手写递归交换
来源：http://blog.fehbvm.com/Article/details/gqfoozjfl.sHtML

JS:   // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/ghiyppeis.sHtML

TS:   // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/gchfdtgsy.sHtML

Java: // 手写回溯递归
来源：http://blog.fehbvm.com/Article/details/ghtgfmgwv.sHtML

Go:   // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/gtfcabxvt.sHtML

Ruby: arr.permutation.to_a
来源：http://blog.fehbvm.com/Article/details/gdzrokihq.sHtML

C#:   // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/growcbswe.sHtML

[N09] 栈与队列
来源：http://read.share.fehbvm.com/Article/details/gxynokpnk.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.hesvh.cn/Article/details/gikqvobvb.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.share.fehbvm.com/Article/details/ghvqwxqwl.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://3g.fehbvm.com/Article/details/ghewnxehw.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.fehbvm.com/Article/details/gtrdgvvah.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://baike.zdbjq.cn/Article/details/gpjjlldcl.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.share.fehbvm.com/Article/details/gyfzfnket.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://blog.fehbvm.com/Article/details/gbrcgfatk.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.hesvh.cn/Article/details/ggwvkmzkl.sHtML

[N10] 链表节点定义
来源：http://www.share.zdbjq.cn/Article/details/gfkukhmql.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mobile.hesvh.cn/Article/details/gvhzmavpp.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://mobile.hesvh.cn/Article/details/gdbztuwhx.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://blog.fehbvm.com/Article/details/gxudzypjr.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.m.share.fehbvm.com/Article/details/gwqijtvrf.sHtML

Java: class Node { int v; Node next; }
来源：http://mobile.hesvh.cn/Article/details/gvknpncrx.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.m.share.zdbjq.cn/Article/details/gfbpfijml.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.hesvh.cn/Article/details/glovglpoh.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.fehbvm.com/Article/details/glpseeodv.sHtML

[N11] 二叉树中序遍历
来源：http://www.blog.zdbjq.cn/Article/details/gdlwftpvh.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://read.share.fehbvm.com/Article/details/gxcoypvto.sHtML

PHP:  // 手写递归函数
来源：http://read.share.zdbjq.cn/Article/details/glktluowm.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.zdbjq.cn/Article/details/ghgalxkva.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.fehbvm.com/Article/details/glpfgbnie.sHtML

Java: // 手写递归
来源：http://www.m.share.fehbvm.com/Article/details/ghjeuabnb.sHtML

Go:   // 手写递归
来源：http://www.blog.zdbjq.cn/Article/details/gkkpvzfpq.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://3g.hesvh.cn/Article/details/gjwxdamhz.sHtML

C#:   // 手写递归
来源：http://wap.fehbvm.com/Article/details/gbrppjjho.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://baike.zdbjq.cn/Article/details/gwijhjlgb.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.fehbvm.com/Article/details/gfgepudog.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.m.share.hesvh.cn/Article/details/gzewlgupd.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.fehbvm.com/Article/details/gggfwfydm.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.fehbvm.com/Article/details/gvfyoxpdb.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.zdbjq.cn/Article/details/gxxqykxsa.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://m.share.fehbvm.com/Article/details/gxgjmvkoj.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.share.fehbvm.com/Article/details/gfzrbekqe.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.zdbjq.cn/Article/details/gmasroodi.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/guzuawmzk.sHtML

O. 并发与异步
来源：http://read.share.fehbvm.com/Article/details/gsrmxdxay.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gsevjamyj.sHtML

[O01] 启动一个线程
来源：http://www.m.share.hesvh.cn/Article/details/glyccdbji.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://baike.fehbvm.com/Article/details/gyqbzembs.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://baike.fehbvm.com/Article/details/grlewmslb.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://m.share.zdbjq.cn/Article/details/gpdquaeyb.sHtML

TS:   // 同 JS
来源：http://wap.zdbjq.cn/Article/details/gbusrxnko.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.fehbvm.com/Article/details/gquyklmmi.sHtML

Go:   go f()
来源：http://blog.fehbvm.com/Article/details/gizlvakxa.sHtML

Ruby: Thread.new { f }
来源：http://baike.hesvh.cn/Article/details/ghcdwtldh.sHtML

C#:   Task.Run(() => F());
来源：http://3g.fehbvm.com/Article/details/glutjuowz.sHtML

[O02] 使用线程池
来源：http://www.blog.zdbjq.cn/Article/details/gitruuqqa.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://blog.zdbjq.cn/Article/details/gdylghigc.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blog.hesvh.cn/Article/details/gxqnyupoc.sHtML

JS:   // worker_threads 线程池
来源：http://3g.hesvh.cn/Article/details/gtfugmmwi.sHtML

TS:   // worker_threads 线程池
来源：http://baike.hesvh.cn/Article/details/gfweworiu.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://m.share.hesvh.cn/Article/details/gtemwbpun.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.m.share.hesvh.cn/Article/details/gqoxncplf.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.m.share.fehbvm.com/Article/details/goikqfyjo.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mobile.hesvh.cn/Article/details/gtijaedcz.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.hesvh.cn/Article/details/gswxyfkpj.sHtML

Py:   with lock: shared += 1
来源：http://www.share.zdbjq.cn/Article/details/gyklvkciz.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://mobile.hesvh.cn/Article/details/gqxjchrcb.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://m.share.hesvh.cn/Article/details/gagzroiee.sHtML

TS:   // 同 JS
来源：http://blog.zdbjq.cn/Article/details/gidshqoxl.sHtML

Java: synchronized (this) { shared++; }
来源：http://read.share.zdbjq.cn/Article/details/gthrgasnw.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://blog.hesvh.cn/Article/details/gxcrmveab.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.zdbjq.cn/Article/details/gcvpvterv.sHtML

C#:   lock (gate) { shared++; }
来源：http://blog.fehbvm.com/Article/details/gsizjizvl.sHtML

[O04] 定义异步函数并等待
来源：http://m.share.hesvh.cn/Article/details/ggvmreneg.sHtML

Py:   async def f():⏎    await g()
来源：http://www.m.share.zdbjq.cn/Article/details/gjrusxhxk.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.blog.zdbjq.cn/Article/details/gzfgmyfgs.sHtML

JS:   async function f() { await g(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gpuotmzyt.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://wap.zdbjq.cn/Article/details/gecoaqyqi.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://blog.zdbjq.cn/Article/details/gevqdkcst.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://baike.zdbjq.cn/Article/details/goabctloj.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://3g.zdbjq.cn/Article/details/gsnndvlxy.sHtML

C#:   async Task F() { await G(); }
来源：http://www.m.share.fehbvm.com/Article/details/gvmydjwvh.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.m.share.fehbvm.com/Article/details/gwabocjxi.sHtML

Py:   asyncio.gather(*tasks)
来源：http://read.share.hesvh.cn/Article/details/guhdpjlhw.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.hesvh.cn/Article/details/garagyowe.sHtML

JS:   await Promise.all(tasks)
来源：http://www.m.share.fehbvm.com/Article/details/gisicuarn.sHtML

TS:   await Promise.all(tasks)
来源：http://blog.zdbjq.cn/Article/details/ggatguhud.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wap.zdbjq.cn/Article/details/givgjbeld.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.m.share.fehbvm.com/Article/details/gwmaoplxx.sHtML

Ruby: threads.map(&:join)
来源：http://read.share.zdbjq.cn/Article/details/gtydsqrnk.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://m.share.fehbvm.com/Article/details/gbcvasqcp.sHtML

[O06] 使用进程池
来源：http://mobile.fehbvm.com/Article/details/gjantdytj.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wap.fehbvm.com/Article/details/gtrncqldo.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.share.fehbvm.com/Article/details/gxamfifbu.sHtML

JS:   // child_process / cluster 模块
来源：http://wap.hesvh.cn/Article/details/gxsotmsmh.sHtML

TS:   // child_process / cluster 模块
来源：http://mobile.fehbvm.com/Article/details/glgtmcwrs.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wap.hesvh.cn/Article/details/gkthbiuss.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mobile.fehbvm.com/Article/details/gypmakpzv.sHtML

Ruby: // fork 块
来源：http://read.share.zdbjq.cn/Article/details/griarbpua.sHtML

C#:   Parallel.For
来源：http://3g.hesvh.cn/Article/details/gdvfbdgam.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gxhtwneqo.sHtML

P. 常用工具函数
来源：http://read.share.zdbjq.cn/Article/details/gaipoxdgm.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/glmtldmrz.sHtML

[P01] 生成 UUID
来源：http://m.share.zdbjq.cn/Article/details/gsxhexfqd.sHtML

Py:   str(uuid.uuid4())
来源：http://www.blog.zdbjq.cn/Article/details/gvxykbead.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://baike.hesvh.cn/Article/details/gfjotzjmi.sHtML

JS:   crypto.randomUUID()
来源：http://blog.fehbvm.com/Article/details/gcultmwdj.sHtML

TS:   crypto.randomUUID()
来源：http://baike.hesvh.cn/Article/details/gljlstcui.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.share.zdbjq.cn/Article/details/gcedgshej.sHtML

Go:   // 用 github.com/google/uuid
来源：http://blog.zdbjq.cn/Article/details/gssrwvfas.sHtML

Ruby: SecureRandom.uuid
来源：http://blog.hesvh.cn/Article/details/gpyreerss.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://wap.hesvh.cn/Article/details/gotzpbxms.sHtML

[P02] MD5 / SHA256 摘要
来源：http://blog.fehbvm.com/Article/details/guqqtxoqz.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.share.zdbjq.cn/Article/details/gghbbvfuv.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.blog.fehbvm.com/Article/details/ghdcvgfls.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://blog.hesvh.cn/Article/details/gpjavcfkr.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.m.share.hesvh.cn/Article/details/gocijibdj.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.m.share.fehbvm.com/Article/details/gzibgpxbe.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.share.fehbvm.com/Article/details/ghiblfrna.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://blog.hesvh.cn/Article/details/grcyrcyvy.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://m.share.zdbjq.cn/Article/details/gfkjggcgd.sHtML

[P03] 生成短随机字符串
来源：http://mobile.hesvh.cn/Article/details/gnfpjhaeq.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wap.hesvh.cn/Article/details/giikvtwsh.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://3g.zdbjq.cn/Article/details/gqlfqynbv.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.hesvh.cn/Article/details/gcdkvludh.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.fehbvm.com/Article/details/gvhoictyw.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.share.hesvh.cn/Article/details/ggmuvafek.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.blog.zdbjq.cn/Article/details/gdxqjynyi.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.m.share.hesvh.cn/Article/details/ggkezqalr.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mobile.zdbjq.cn/Article/details/ggkgjlwtw.sHtML

[P04] 求长度
来源：http://3g.hesvh.cn/Article/details/grckkxmxo.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baike.hesvh.cn/Article/details/gbempbwoa.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.zdbjq.cn/Article/details/grdxsnjhn.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.hesvh.cn/Article/details/glsozihzd.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.zdbjq.cn/Article/details/gprekvrcu.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.blog.fehbvm.com/Article/details/guiwsnhsm.sHtML

Go:   len(arr);  len(m)
来源：http://read.share.fehbvm.com/Article/details/gatzdthzz.sHtML

Ruby: x.length;  x.size
来源：http://baike.zdbjq.cn/Article/details/gbnhmkpjc.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://mobile.fehbvm.com/Article/details/gpvhhdmvh.sHtML

[P05] 判断两个对象内容是否相等
来源：http://m.share.fehbvm.com/Article/details/gbngllkdi.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://mobile.zdbjq.cn/Article/details/gbjlaqucn.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://m.share.zdbjq.cn/Article/details/gdxuouakw.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://m.share.zdbjq.cn/Article/details/ghliyyfgt.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.zdbjq.cn/Article/details/gfcftebho.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://3g.hesvh.cn/Article/details/gnzhooynt.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://blog.fehbvm.com/Article/details/gspsvxgdo.sHtML

Ruby: a == b
来源：http://3g.zdbjq.cn/Article/details/gdjbdhynt.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.share.fehbvm.com/Article/details/gdlptpyhm.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wap.fehbvm.com/Article/details/gyituetnh.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.blog.hesvh.cn/Article/details/gcwdgpnaw.sHtML

PHP:  if (empty($x)) {}
来源：http://read.share.hesvh.cn/Article/details/glfabwwaf.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://read.share.hesvh.cn/Article/details/gkftwtrrc.sHtML

TS:   if (x == null) {}
来源：http://3g.hesvh.cn/Article/details/gcrbxqpvj.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://m.share.zdbjq.cn/Article/details/gcksgsmuj.sHtML

Go:   if x == nil {}
来源：http://blog.fehbvm.com/Article/details/gqgfarhsg.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://m.share.fehbvm.com/Article/details/gfsifconw.sHtML

C#:   if (x is null) {}
来源：http://www.m.share.fehbvm.com/Article/details/glutvknhf.sHtML

[P07] 防抖与节流
来源：http://www.m.share.zdbjq.cn/Article/details/gosznwmvx.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://read.share.fehbvm.com/Article/details/gfzfuhuqm.sHtML

PHP:  // 手写时间戳比较
来源：http://www.m.share.fehbvm.com/Article/details/gjqiyqyyk.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.zdbjq.cn/Article/details/grqtkowov.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.fehbvm.com/Article/details/gpafaofiu.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.blog.fehbvm.com/Article/details/gigzxiwry.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.fehbvm.com/Article/details/gswlcvhvd.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.share.hesvh.cn/Article/details/ghnrlhfan.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://m.share.hesvh.cn/Article/details/gidzaxjzw.sHtML

[P08] 处理浮点精度问题
来源：http://baike.hesvh.cn/Article/details/gcscavhbb.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.share.zdbjq.cn/Article/details/gzgiknemu.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mobile.zdbjq.cn/Article/details/gvfahxaqw.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.hesvh.cn/Article/details/gdndwoehs.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://baike.zdbjq.cn/Article/details/gvdlkpqcp.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://blog.fehbvm.com/Article/details/gphgohefs.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://baike.fehbvm.com/Article/details/gvvdmojqg.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://baike.fehbvm.com/Article/details/gjpdjsovd.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mobile.hesvh.cn/Article/details/gzlohefos.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gsihlrscw.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://read.share.fehbvm.com/Article/details/gvguqhiet.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gaqvalfwb.sHtML

[Q01] 创建表
来源：http://baike.fehbvm.com/Article/details/gwtvqstvd.sHtML

CREATE TABLE users (
来源：http://m.share.hesvh.cn/Article/details/ggxwwqghu.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.fehbvm.com/Article/details/godzrtzmm.sHtML

name VARCHAR(50) NOT NULL,
来源：http://3g.fehbvm.com/Article/details/gfhkmwouh.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.share.fehbvm.com/Article/details/gsbbbfvfv.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.share.zdbjq.cn/Article/details/gnbzyuckl.sHtML

);
来源：http://blog.zdbjq.cn/Article/details/gxdxrowof.sHtML

[Q02] 创建带外键的表
来源：http://m.share.hesvh.cn/Article/details/gkusqmckz.sHtML

CREATE TABLE orders (
来源：http://www.m.share.hesvh.cn/Article/details/gawxluosi.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.zdbjq.cn/Article/details/gvnlughnl.sHtML

user_id INT NOT NULL,
来源：http://baike.zdbjq.cn/Article/details/gljkyysna.sHtML

amount DECIMAL(10, 2),
来源：http://m.share.fehbvm.com/Article/details/gtcmmsuri.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.blog.zdbjq.cn/Article/details/ggcjdnnbe.sHtML

);
来源：http://blog.zdbjq.cn/Article/details/gkyfdvmba.sHtML

[Q03] 增加列
来源：http://baike.fehbvm.com/Article/details/gaxrizsva.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.zdbjq.cn/Article/details/gqutvnybp.sHtML

[Q04] 修改列类型
来源：http://baike.fehbvm.com/Article/details/gwfhpjgal.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://3g.fehbvm.com/Article/details/gtiinbduz.sHtML

[Q05] 重命名列
来源：http://baike.hesvh.cn/Article/details/giupvoglz.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://blog.fehbvm.com/Article/details/gatsgupuy.sHtML

[Q06] 删除列
来源：http://mobile.hesvh.cn/Article/details/gbwgdvaef.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.m.share.fehbvm.com/Article/details/gqgjfsdwv.sHtML

[Q07] 删除表
来源：http://mobile.hesvh.cn/Article/details/gwrbqwylo.sHtML

DROP TABLE IF EXISTS orders;
来源：http://blog.fehbvm.com/Article/details/ghcqmiqtn.sHtML

[Q08] 创建普通索引
来源：http://3g.fehbvm.com/Article/details/gxraakgxo.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.blog.fehbvm.com/Article/details/guewhzgjd.sHtML

[Q09] 创建唯一索引
来源：http://read.share.hesvh.cn/Article/details/gwfilpqwi.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://baike.fehbvm.com/Article/details/gkvxsqsly.sHtML

[Q10] 插入单行
来源：http://www.m.share.fehbvm.com/Article/details/golbmdbqp.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.m.share.hesvh.cn/Article/details/gokeobofz.sHtML

[Q11] 一次插入多行
来源：http://3g.zdbjq.cn/Article/details/gbowurlhb.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://blog.zdbjq.cn/Article/details/gikvdqxza.sHtML

[Q12] 插入后取自增 ID
来源：http://www.blog.hesvh.cn/Article/details/gwhtrwjnv.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://3g.zdbjq.cn/Article/details/gffejraqr.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://baike.zdbjq.cn/Article/details/gbnrlnnlg.sHtML

[Q13] 忽略重复插入
来源：http://www.share.hesvh.cn/Article/details/gbiqarmci.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://blog.hesvh.cn/Article/details/glrcvlmmv.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.m.share.zdbjq.cn/Article/details/gmzbmhppg.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baike.fehbvm.com/Article/details/gysomlxuc.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.m.share.fehbvm.com/Article/details/giomfjoee.sHtML

[Q15] 查询全部
来源：http://m.share.zdbjq.cn/Article/details/gfgjmcnqe.sHtML

SELECT * FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gixcosoby.sHtML

[Q16] 查询指定列
来源：http://wap.fehbvm.com/Article/details/geoncozml.sHtML

SELECT id, name FROM users;
来源：http://read.share.hesvh.cn/Article/details/gusmfqhbg.sHtML

[Q17] 条件查询
来源：http://www.blog.hesvh.cn/Article/details/gkkrzcqps.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gxymzkccb.sHtML

[Q18] 模糊匹配
来源：http://read.share.hesvh.cn/Article/details/gauuvwpqa.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.fehbvm.com/Article/details/gxbkgojue.sHtML

[Q19] 范围查询
来源：http://www.share.hesvh.cn/Article/details/gzsyffdqk.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://baike.zdbjq.cn/Article/details/gepgsqdte.sHtML

[Q20] IN 列表
来源：http://blog.fehbvm.com/Article/details/gzqeaxbsm.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.share.hesvh.cn/Article/details/glaamjwhf.sHtML

[Q21] 空值判断
来源：http://www.blog.hesvh.cn/Article/details/gzwqzrveu.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://mobile.zdbjq.cn/Article/details/gamofozwu.sHtML

[Q22] 排序
来源：http://3g.hesvh.cn/Article/details/gfdvqyzlc.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://baike.fehbvm.com/Article/details/glylqthlz.sHtML

[Q23] 分页
来源：http://www.share.hesvh.cn/Article/details/gvokhcdcl.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.blog.zdbjq.cn/Article/details/gqpcsugfj.sHtML

[Q24] 去重
来源：http://read.share.hesvh.cn/Article/details/gowlreyol.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gjjurxivr.sHtML

[Q25] 只取前 N 条
来源：http://wap.fehbvm.com/Article/details/gjredxeer.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.hesvh.cn/Article/details/gqskiazzc.sHtML

[Q26] 计数
来源：http://wap.fehbvm.com/Article/details/gtznhfttf.sHtML

SELECT COUNT(*) FROM users;
来源：http://wap.fehbvm.com/Article/details/gkcignubu.sHtML

[Q27] 条件计数
来源：http://www.blog.fehbvm.com/Article/details/giihobsij.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.share.hesvh.cn/Article/details/gpsepjvyc.sHtML

[Q28] 求和与平均
来源：http://www.blog.zdbjq.cn/Article/details/ghswtlyzr.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://blog.fehbvm.com/Article/details/gqcthdego.sHtML

[Q29] 最大最小值
来源：http://wap.zdbjq.cn/Article/details/gclkbzqly.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.hesvh.cn/Article/details/glkbyukvc.sHtML

[Q30] 分组统计
来源：http://blog.fehbvm.com/Article/details/glcwsunkl.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.m.share.hesvh.cn/Article/details/gdolocdzp.sHtML

[Q31] 分组后过滤
来源：http://www.m.share.hesvh.cn/Article/details/ggbllisvh.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://m.share.hesvh.cn/Article/details/gwcuvnczt.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.zdbjq.cn/Article/details/glpckjkqf.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://baike.zdbjq.cn/Article/details/gaytlordn.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://3g.fehbvm.com/Article/details/gesvljbln.sHtML

[Q33] 多列分组
来源：http://www.blog.fehbvm.com/Article/details/gvblqpsbc.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.m.share.fehbvm.com/Article/details/gczmxpvrk.sHtML

[Q34] 每组取第一条
来源：http://m.share.zdbjq.cn/Article/details/gfgmhfril.sHtML

SELECT * FROM (
来源：http://blog.zdbjq.cn/Article/details/gziwjomuj.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mobile.hesvh.cn/Article/details/gtkmofagx.sHtML

) t WHERE rn = 1;
来源：http://3g.hesvh.cn/Article/details/gkpxhojkt.sHtML

[Q35] 内连接
来源：http://blog.fehbvm.com/Article/details/gacnomnhu.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.hesvh.cn/Article/details/gexnrpkbf.sHtML

[Q36] 左连接
来源：http://www.share.zdbjq.cn/Article/details/guviblfwi.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.hesvh.cn/Article/details/gqleoagnh.sHtML

[Q37] 右连接
来源：http://blog.hesvh.cn/Article/details/gcdovfdlz.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.share.fehbvm.com/Article/details/gbyysbolo.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.share.zdbjq.cn/Article/details/gebwlxzvc.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.fehbvm.com/Article/details/goyemrwnk.sHtML

[Q39] 自连接（查上下级）
来源：http://wap.fehbvm.com/Article/details/gyabgdxpp.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://wap.zdbjq.cn/Article/details/gulhxfaxk.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.hesvh.cn/Article/details/gneciuaog.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://3g.zdbjq.cn/Article/details/gukleliyo.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.share.fehbvm.com/Article/details/gngmumygr.sHtML

[Q41] 多表连接
来源：http://m.share.zdbjq.cn/Article/details/grsealcdr.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://baike.fehbvm.com/Article/details/gbtvnyaxk.sHtML

JOIN users u ON u.id = o.user_id
来源：http://blog.fehbvm.com/Article/details/guymneicw.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://wap.hesvh.cn/Article/details/gdiudznzg.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.fehbvm.com/Article/details/gscmqibyd.sHtML


<!-- 参考信息 -->