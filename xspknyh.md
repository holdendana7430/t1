代发 wailian999

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mobile.fanxiaobao.xyz/Article/details/gphtulbpb.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://wap.fanxiaobao.xyz/Article/details/gaxndegao.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.share.fanxiaobao.xyz/Article/details/gyrnoqtgw.sHtML

Java: // 手写 HashMap
来源：http://baike.fanxiaobao.xyz/Article/details/giazyftxn.sHtML

Go:   // 手写 map[int]int
来源：http://m.share.fanxiaobao.xyz/Article/details/gsjtvmmin.sHtML

Ruby: // 手写 Hash
来源：http://blog.fanxiaobao.xyz/Article/details/gpmorsred.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://m.share.fanxiaobao.xyz/Article/details/gkuvpiaro.sHtML

[N08] 生成全排列
来源：http://3g.fanxiaobao.xyz/Article/details/gfztidpha.sHtML

Py:   itertools.permutations(arr)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkwbjcdsn.sHtML

PHP:  // 手写递归交换
来源：http://m.share.fanxiaobao.xyz/Article/details/giadmnvtk.sHtML

JS:   // 手写回溯递归
来源：http://3g.fanxiaobao.xyz/Article/details/gyejyzzuc.sHtML

TS:   // 手写回溯递归
来源：http://www.share.fanxiaobao.xyz/Article/details/geqdklgsq.sHtML

Java: // 手写回溯递归
来源：http://m.share.fanxiaobao.xyz/Article/details/gbsoqodfd.sHtML

Go:   // 手写回溯递归
来源：http://3g.fanxiaobao.xyz/Article/details/govynewcd.sHtML

Ruby: arr.permutation.to_a
来源：http://www.blog.fanxiaobao.xyz/Article/details/gulgzhaxd.sHtML

C#:   // 手写回溯递归
来源：http://mobile.fanxiaobao.xyz/Article/details/gvjuzlwif.sHtML

[N09] 栈与队列
来源：http://baike.fanxiaobao.xyz/Article/details/gmohfeecm.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.fanxiaobao.xyz/Article/details/gwergymde.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.share.fanxiaobao.xyz/Article/details/gycdbptbl.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.share.fanxiaobao.xyz/Article/details/gfratuedj.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.share.fanxiaobao.xyz/Article/details/gwzehwqdh.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://blog.fanxiaobao.xyz/Article/details/gtjxewete.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://baike.fanxiaobao.xyz/Article/details/ggilsznwh.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wap.fanxiaobao.xyz/Article/details/gjlwrityg.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.fanxiaobao.xyz/Article/details/gftatmeul.sHtML

[N10] 链表节点定义
来源：http://mobile.fanxiaobao.xyz/Article/details/gsuwgfccr.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://baike.fanxiaobao.xyz/Article/details/gjnnwotnu.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gdsuzerzm.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://read.share.fanxiaobao.xyz/Article/details/gehpawlem.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.fanxiaobao.xyz/Article/details/gtbymhadx.sHtML

Java: class Node { int v; Node next; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gecuqyanh.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://wap.fanxiaobao.xyz/Article/details/gmnwakpou.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.fanxiaobao.xyz/Article/details/gycgkvucz.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gkhnfhjaz.sHtML

[N11] 二叉树中序遍历
来源：http://3g.fanxiaobao.xyz/Article/details/gwiuuzcba.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.share.fanxiaobao.xyz/Article/details/glkoiukmh.sHtML

PHP:  // 手写递归函数
来源：http://mobile.fanxiaobao.xyz/Article/details/ghjcnqzzd.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.fanxiaobao.xyz/Article/details/gcnyrmmoy.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.fanxiaobao.xyz/Article/details/gpdtddpgg.sHtML

Java: // 手写递归
来源：http://www.share.fanxiaobao.xyz/Article/details/gycwztpco.sHtML

Go:   // 手写递归
来源：http://www.share.fanxiaobao.xyz/Article/details/ggxxtqrbf.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mobile.fanxiaobao.xyz/Article/details/ghbguqupy.sHtML

C#:   // 手写递归
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggqlctgnh.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://baike.fanxiaobao.xyz/Article/details/grwtglvry.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mobile.fanxiaobao.xyz/Article/details/gehozgsuf.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcpdhsbhg.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.fanxiaobao.xyz/Article/details/gjsuuwklt.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.fanxiaobao.xyz/Article/details/gbueprufq.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.fanxiaobao.xyz/Article/details/gutqqlmzw.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxjbqgled.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxxszhlqq.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.fanxiaobao.xyz/Article/details/gnkjlwanv.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqoxudonj.sHtML

O. 并发与异步
来源：http://baike.fanxiaobao.xyz/Article/details/gyhjnswct.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gocuujqdt.sHtML

[O01] 启动一个线程
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwmtmabth.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wap.fanxiaobao.xyz/Article/details/gqoravthd.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.share.fanxiaobao.xyz/Article/details/ghqoluxuu.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mobile.fanxiaobao.xyz/Article/details/gliebdosu.sHtML

TS:   // 同 JS
来源：http://www.blog.fanxiaobao.xyz/Article/details/goljyocki.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gscmmnvhm.sHtML

Go:   go f()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gojlebsbw.sHtML

Ruby: Thread.new { f }
来源：http://3g.fanxiaobao.xyz/Article/details/gxjntxevp.sHtML

C#:   Task.Run(() => F());
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwpqvbxnu.sHtML

[O02] 使用线程池
来源：http://m.share.fanxiaobao.xyz/Article/details/ghbaihapm.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.fanxiaobao.xyz/Article/details/gdhejczyu.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blog.fanxiaobao.xyz/Article/details/gimyfbprz.sHtML

JS:   // worker_threads 线程池
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcwiqgvnf.sHtML

TS:   // worker_threads 线程池
来源：http://m.share.fanxiaobao.xyz/Article/details/gmidvmvul.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwwttoeae.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gagevhumg.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.fanxiaobao.xyz/Article/details/gjfcrwtil.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://m.share.fanxiaobao.xyz/Article/details/gsvupiirb.sHtML

[O03] 加锁保护共享数据
来源：http://wap.fanxiaobao.xyz/Article/details/gagkrflhx.sHtML

Py:   with lock: shared += 1
来源：http://3g.fanxiaobao.xyz/Article/details/gitlkdnxl.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.share.fanxiaobao.xyz/Article/details/gpnvzdpty.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grzfwbzqs.sHtML

TS:   // 同 JS
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjisxkzyc.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.fanxiaobao.xyz/Article/details/gnujgrofm.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://3g.fanxiaobao.xyz/Article/details/gsvnqzigf.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpstetirn.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guiqrnjpu.sHtML

[O04] 定义异步函数并等待
来源：http://mobile.fanxiaobao.xyz/Article/details/glkoupeeh.sHtML

Py:   async def f():⏎    await g()
来源：http://blog.fanxiaobao.xyz/Article/details/gaiytesof.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://read.share.fanxiaobao.xyz/Article/details/gbipuiqqa.sHtML

JS:   async function f() { await g(); }
来源：http://mobile.fanxiaobao.xyz/Article/details/grdbbszdl.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://wap.fanxiaobao.xyz/Article/details/giskxioiv.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbvocsbwk.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.share.fanxiaobao.xyz/Article/details/ghpuljtbj.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://3g.fanxiaobao.xyz/Article/details/gjzbdwjup.sHtML

C#:   async Task F() { await G(); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwhxbcwff.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsnefodck.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.fanxiaobao.xyz/Article/details/gptuvtmoq.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wap.fanxiaobao.xyz/Article/details/gukjseiwp.sHtML

JS:   await Promise.all(tasks)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grckcahrj.sHtML

TS:   await Promise.all(tasks)
来源：http://baike.fanxiaobao.xyz/Article/details/ghjqbcxgv.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmpapqper.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://3g.fanxiaobao.xyz/Article/details/grgmyqyxm.sHtML

Ruby: threads.map(&:join)
来源：http://blog.fanxiaobao.xyz/Article/details/gokjgiwen.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://baike.fanxiaobao.xyz/Article/details/gbkfnolpj.sHtML

[O06] 使用进程池
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glhhjfckb.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://3g.fanxiaobao.xyz/Article/details/glmfyafdx.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.share.fanxiaobao.xyz/Article/details/gpqdgzwnt.sHtML

JS:   // child_process / cluster 模块
来源：http://baike.fanxiaobao.xyz/Article/details/gubewbvdn.sHtML

TS:   // child_process / cluster 模块
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcvqgkzct.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.share.fanxiaobao.xyz/Article/details/ggadfnoql.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mobile.fanxiaobao.xyz/Article/details/gjlyjucni.sHtML

Ruby: // fork 块
来源：http://read.share.fanxiaobao.xyz/Article/details/gkohuwdxr.sHtML

C#:   Parallel.For
来源：http://mobile.fanxiaobao.xyz/Article/details/gseigdzpv.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gqfgfjdqe.sHtML

P. 常用工具函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmrvscjcq.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gjyoysecv.sHtML

[P01] 生成 UUID
来源：http://mobile.fanxiaobao.xyz/Article/details/gqnovsgql.sHtML

Py:   str(uuid.uuid4())
来源：http://blog.fanxiaobao.xyz/Article/details/gdlvzcdtn.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mobile.fanxiaobao.xyz/Article/details/glvvnpqls.sHtML

JS:   crypto.randomUUID()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ginfiaacn.sHtML

TS:   crypto.randomUUID()
来源：http://baike.fanxiaobao.xyz/Article/details/gpscvzlea.sHtML

Java: UUID.randomUUID().toString()
来源：http://mobile.fanxiaobao.xyz/Article/details/gdmltrtds.sHtML

Go:   // 用 github.com/google/uuid
来源：http://mobile.fanxiaobao.xyz/Article/details/gtldrsxdx.sHtML

Ruby: SecureRandom.uuid
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzpbirocr.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://read.share.fanxiaobao.xyz/Article/details/gmsaxrwmy.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqdviroag.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://read.share.fanxiaobao.xyz/Article/details/gbhpgzoej.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://read.share.fanxiaobao.xyz/Article/details/gkuwwugxa.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wap.fanxiaobao.xyz/Article/details/gjuqqimhq.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mobile.fanxiaobao.xyz/Article/details/gnemkhhsd.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://m.share.fanxiaobao.xyz/Article/details/gqipholme.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wap.fanxiaobao.xyz/Article/details/gkkdxxygr.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://baike.fanxiaobao.xyz/Article/details/gakhiomry.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://blog.fanxiaobao.xyz/Article/details/ggzrvvowu.sHtML

[P03] 生成短随机字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvtewdzcc.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.blog.fanxiaobao.xyz/Article/details/glquomtgc.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gauqydmhg.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.fanxiaobao.xyz/Article/details/gtufijypq.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.fanxiaobao.xyz/Article/details/gmotzbfga.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://m.share.fanxiaobao.xyz/Article/details/gebrfhbxz.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://baike.fanxiaobao.xyz/Article/details/gejepbtaa.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://read.share.fanxiaobao.xyz/Article/details/glwgpekdd.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wap.fanxiaobao.xyz/Article/details/ghjovtpky.sHtML

[P04] 求长度
来源：http://3g.fanxiaobao.xyz/Article/details/ghjxgudun.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmxykodcl.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.fanxiaobao.xyz/Article/details/gbwkmruyo.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.fanxiaobao.xyz/Article/details/gaffgytsl.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.fanxiaobao.xyz/Article/details/gtkwvljgi.sHtML

Java: list.size();  map.size();  s.length()
来源：http://baike.fanxiaobao.xyz/Article/details/ghpfslgrz.sHtML

Go:   len(arr);  len(m)
来源：http://m.share.fanxiaobao.xyz/Article/details/gspijdkqb.sHtML

Ruby: x.length;  x.size
来源：http://blog.fanxiaobao.xyz/Article/details/gjmdwgbuu.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.share.fanxiaobao.xyz/Article/details/gyqimtzmf.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcoazmwpz.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://baike.fanxiaobao.xyz/Article/details/gtcgaoenh.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpmrkwsub.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://read.share.fanxiaobao.xyz/Article/details/gqueudicf.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.fanxiaobao.xyz/Article/details/gkeyvkgcc.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://3g.fanxiaobao.xyz/Article/details/gghnxgtru.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://baike.fanxiaobao.xyz/Article/details/ghgouaulv.sHtML

Ruby: a == b
来源：http://wap.fanxiaobao.xyz/Article/details/gthkmxjeq.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.share.fanxiaobao.xyz/Article/details/gfqjnrrvt.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://3g.fanxiaobao.xyz/Article/details/ghooxypzg.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://blog.fanxiaobao.xyz/Article/details/gpghezgxx.sHtML

PHP:  if (empty($x)) {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gtasuzdum.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.blog.fanxiaobao.xyz/Article/details/gngwbeemt.sHtML

TS:   if (x == null) {}
来源：http://wap.fanxiaobao.xyz/Article/details/gwrlyhskp.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://baike.fanxiaobao.xyz/Article/details/gljrlinms.sHtML

Go:   if x == nil {}
来源：http://wap.fanxiaobao.xyz/Article/details/grhmuhwbu.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://baike.fanxiaobao.xyz/Article/details/gmiwdfsmx.sHtML

C#:   if (x is null) {}
来源：http://blog.fanxiaobao.xyz/Article/details/gvnvlgeot.sHtML

[P07] 防抖与节流
来源：http://wap.fanxiaobao.xyz/Article/details/gfleepnxg.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.blog.fanxiaobao.xyz/Article/details/gymbyuqpg.sHtML

PHP:  // 手写时间戳比较
来源：http://read.share.fanxiaobao.xyz/Article/details/giglyuibr.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.fanxiaobao.xyz/Article/details/gzmzctsbj.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdghvfrso.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wap.fanxiaobao.xyz/Article/details/gtwnxnnpx.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mobile.fanxiaobao.xyz/Article/details/ggcyekxwd.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://mobile.fanxiaobao.xyz/Article/details/gxdubsvgz.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://blog.fanxiaobao.xyz/Article/details/gfdwablzj.sHtML

[P08] 处理浮点精度问题
来源：http://mobile.fanxiaobao.xyz/Article/details/ggyszttlv.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfzithqrg.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://blog.fanxiaobao.xyz/Article/details/gfqjmohur.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://3g.fanxiaobao.xyz/Article/details/ggqnimfnj.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://blog.fanxiaobao.xyz/Article/details/gkutrnszt.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://read.share.fanxiaobao.xyz/Article/details/gwfcihhck.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wap.fanxiaobao.xyz/Article/details/grimafurd.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://3g.fanxiaobao.xyz/Article/details/ggiqdnhqu.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://3g.fanxiaobao.xyz/Article/details/gihxrxpjf.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gfapetlob.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mobile.fanxiaobao.xyz/Article/details/gpeqknxck.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gyoazcksa.sHtML

[Q01] 创建表
来源：http://mobile.fanxiaobao.xyz/Article/details/gxhtqqexd.sHtML

CREATE TABLE users (
来源：http://baike.fanxiaobao.xyz/Article/details/gvrybycim.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.fanxiaobao.xyz/Article/details/gdzkrektj.sHtML

name VARCHAR(50) NOT NULL,
来源：http://mobile.fanxiaobao.xyz/Article/details/gumaaiteh.sHtML

email VARCHAR(100) UNIQUE,
来源：http://m.share.fanxiaobao.xyz/Article/details/ghaqebbut.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://m.share.fanxiaobao.xyz/Article/details/gwrenzmpk.sHtML

);
来源：http://read.share.fanxiaobao.xyz/Article/details/gcvjagrwc.sHtML

[Q02] 创建带外键的表
来源：http://blog.fanxiaobao.xyz/Article/details/gslykarhp.sHtML

CREATE TABLE orders (
来源：http://3g.fanxiaobao.xyz/Article/details/ggmirbmjl.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxdvjaews.sHtML

user_id INT NOT NULL,
来源：http://wap.fanxiaobao.xyz/Article/details/gylmqhtfy.sHtML

amount DECIMAL(10, 2),
来源：http://mobile.fanxiaobao.xyz/Article/details/gvxrdzyaa.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wap.fanxiaobao.xyz/Article/details/giiwjmslv.sHtML

);
来源：http://read.share.fanxiaobao.xyz/Article/details/gsgqpjibh.sHtML

[Q03] 增加列
来源：http://www.share.fanxiaobao.xyz/Article/details/glyxnvzti.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://3g.fanxiaobao.xyz/Article/details/guqimslxe.sHtML

[Q04] 修改列类型
来源：http://m.share.fanxiaobao.xyz/Article/details/gsvevzutb.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://baike.fanxiaobao.xyz/Article/details/glrebuhis.sHtML

[Q05] 重命名列
来源：http://www.share.fanxiaobao.xyz/Article/details/geyibuydz.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mobile.fanxiaobao.xyz/Article/details/glnbhrkla.sHtML

[Q06] 删除列
来源：http://www.blog.fanxiaobao.xyz/Article/details/gplpnzikd.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://read.share.fanxiaobao.xyz/Article/details/gjcwjspvj.sHtML

[Q07] 删除表
来源：http://m.share.fanxiaobao.xyz/Article/details/gcelnkgbz.sHtML

DROP TABLE IF EXISTS orders;
来源：http://baike.fanxiaobao.xyz/Article/details/gchbshrqy.sHtML

[Q08] 创建普通索引
来源：http://mobile.fanxiaobao.xyz/Article/details/gegpmwkih.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://blog.fanxiaobao.xyz/Article/details/gafctneow.sHtML

[Q09] 创建唯一索引
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxmbstent.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.share.fanxiaobao.xyz/Article/details/gfdwecuiy.sHtML

[Q10] 插入单行
来源：http://wap.fanxiaobao.xyz/Article/details/gltemoodj.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.blog.fanxiaobao.xyz/Article/details/gebgmnsjs.sHtML

[Q11] 一次插入多行
来源：http://www.share.fanxiaobao.xyz/Article/details/gmawksfjl.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggstjtvxe.sHtML

[Q12] 插入后取自增 ID
来源：http://www.share.fanxiaobao.xyz/Article/details/grydmvhlc.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://read.share.fanxiaobao.xyz/Article/details/gxfsdiqkt.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mobile.fanxiaobao.xyz/Article/details/goywbwkcz.sHtML

[Q13] 忽略重复插入
来源：http://www.share.fanxiaobao.xyz/Article/details/gdxouabxm.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://baike.fanxiaobao.xyz/Article/details/gbszorrej.sHtML

[Q14] 存在则更新（upsert）
来源：http://mobile.fanxiaobao.xyz/Article/details/gugngmxpn.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wap.fanxiaobao.xyz/Article/details/gswdxdlvf.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://read.share.fanxiaobao.xyz/Article/details/ggjgaxowb.sHtML

[Q15] 查询全部
来源：http://3g.fanxiaobao.xyz/Article/details/giuadxbax.sHtML

SELECT * FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gdndvvhir.sHtML

[Q16] 查询指定列
来源：http://www.share.fanxiaobao.xyz/Article/details/gyavpxcew.sHtML

SELECT id, name FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gmfqiystv.sHtML

[Q17] 条件查询
来源：http://read.share.fanxiaobao.xyz/Article/details/gaoeazijw.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/guhtbgkmm.sHtML

[Q18] 模糊匹配
来源：http://m.share.fanxiaobao.xyz/Article/details/ggxknbqfw.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wap.fanxiaobao.xyz/Article/details/gryfrnlns.sHtML

[Q19] 范围查询
来源：http://mobile.fanxiaobao.xyz/Article/details/gpjlwgbfd.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gblacelqp.sHtML

[Q20] IN 列表
来源：http://read.share.fanxiaobao.xyz/Article/details/gvgioyetk.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdgfuzzgg.sHtML

[Q21] 空值判断
来源：http://blog.fanxiaobao.xyz/Article/details/gemrkysig.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://wap.fanxiaobao.xyz/Article/details/guscxuebm.sHtML

[Q22] 排序
来源：http://wap.fanxiaobao.xyz/Article/details/gptgdaqye.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://baike.fanxiaobao.xyz/Article/details/gjdpuwskq.sHtML

[Q23] 分页
来源：http://wap.fanxiaobao.xyz/Article/details/ggxnlopyw.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wap.fanxiaobao.xyz/Article/details/gkzdxkjtp.sHtML

[Q24] 去重
来源：http://blog.fanxiaobao.xyz/Article/details/gawmjfrak.sHtML

SELECT DISTINCT city FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gpdwqfmrd.sHtML

[Q25] 只取前 N 条
来源：http://3g.fanxiaobao.xyz/Article/details/gwrvklhie.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wap.fanxiaobao.xyz/Article/details/gmgnuzfcq.sHtML

[Q26] 计数
来源：http://m.share.fanxiaobao.xyz/Article/details/gzpncwptb.sHtML

SELECT COUNT(*) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/geqgdujvc.sHtML

[Q27] 条件计数
来源：http://wap.fanxiaobao.xyz/Article/details/gudjomnsu.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gstsmwxck.sHtML

[Q28] 求和与平均
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gntchoruu.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wap.fanxiaobao.xyz/Article/details/gtbqpghai.sHtML

[Q29] 最大最小值
来源：http://3g.fanxiaobao.xyz/Article/details/gzpehlviy.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/goqsdeqma.sHtML

[Q30] 分组统计
来源：http://read.share.fanxiaobao.xyz/Article/details/gofaoivac.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mobile.fanxiaobao.xyz/Article/details/glgiexffo.sHtML

[Q31] 分组后过滤
来源：http://mobile.fanxiaobao.xyz/Article/details/gortejlzh.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://3g.fanxiaobao.xyz/Article/details/gddlcxyyb.sHtML

[Q32] 分组拼接字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/gxkxcvfes.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glewuekts.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.fanxiaobao.xyz/Article/details/gmniqwkwi.sHtML

[Q33] 多列分组
来源：http://blog.fanxiaobao.xyz/Article/details/gmggavzsd.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://baike.fanxiaobao.xyz/Article/details/gvdcfhzxf.sHtML

[Q34] 每组取第一条
来源：http://wap.fanxiaobao.xyz/Article/details/gaarkmznb.sHtML

SELECT * FROM (
来源：http://m.share.fanxiaobao.xyz/Article/details/gpyfogkwn.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://m.share.fanxiaobao.xyz/Article/details/gagxujxkb.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkkyexzeh.sHtML

[Q35] 内连接
来源：http://www.share.fanxiaobao.xyz/Article/details/ggzxxkckm.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.fanxiaobao.xyz/Article/details/gicsjdquo.sHtML

[Q36] 左连接
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpeovqchl.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://blog.fanxiaobao.xyz/Article/details/ggvkpsoeo.sHtML

[Q37] 右连接
来源：http://www.share.fanxiaobao.xyz/Article/details/gxkdzvnpg.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.share.fanxiaobao.xyz/Article/details/gfkbyfyef.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://wap.fanxiaobao.xyz/Article/details/gtztoweaz.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://baike.fanxiaobao.xyz/Article/details/grgcxbmmn.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.fanxiaobao.xyz/Article/details/gbefxizuq.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://read.share.fanxiaobao.xyz/Article/details/gxwthpqjv.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mobile.fanxiaobao.xyz/Article/details/glqzvubpi.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.fanxiaobao.xyz/Article/details/gvlphcdrn.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mobile.fanxiaobao.xyz/Article/details/ggvbicrzz.sHtML

[Q41] 多表连接
来源：http://www.share.fanxiaobao.xyz/Article/details/gpuckxpyj.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://read.share.fanxiaobao.xyz/Article/details/ggjqbelga.sHtML

JOIN users u ON u.id = o.user_id
来源：http://3g.fanxiaobao.xyz/Article/details/gjdauyzhc.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://blog.fanxiaobao.xyz/Article/details/glgtjqgov.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.fanxiaobao.xyz/Article/details/gberkghgk.sHtML

SELECT u.name, o.amount FROM users u
来源：http://read.share.fanxiaobao.xyz/Article/details/gzxsbvzjc.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://read.share.fanxiaobao.xyz/Article/details/gynzlkbpl.sHtML

[Q43] 标量子查询
来源：http://www.share.fanxiaobao.xyz/Article/details/gjbbfyfuh.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.fanxiaobao.xyz/Article/details/glzzcbleh.sHtML

[Q44] IN 子查询
来源：http://www.share.fanxiaobao.xyz/Article/details/gpapybaiv.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gedazpyxv.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.fanxiaobao.xyz/Article/details/gxwauemcv.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfgdhwiwm.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.fanxiaobao.xyz/Article/details/gynepmhrc.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwcatqmti.sHtML

[Q47] 与平均值比较
来源：http://m.share.fanxiaobao.xyz/Article/details/gjaqzmino.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wap.fanxiaobao.xyz/Article/details/gfmfrwnxg.sHtML


<!-- 参考信息 -->