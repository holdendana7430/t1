代发 wailian999

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mobile.zdbjq.cn/Article/details/gmlhfapdt.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://m.share.hesvh.cn/Article/details/gmtrrmxou.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.hesvh.cn/Article/details/ghooxeczc.sHtML

Java: // 手写 HashMap
来源：http://3g.fehbvm.com/Article/details/gvepuutxh.sHtML

Go:   // 手写 map[int]int
来源：http://mobile.fehbvm.com/Article/details/gqoiodxan.sHtML

Ruby: // 手写 Hash
来源：http://blog.zdbjq.cn/Article/details/gnpczttmn.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.m.share.hesvh.cn/Article/details/gytwkomgr.sHtML

[N08] 生成全排列
来源：http://mobile.zdbjq.cn/Article/details/gnfgprqnx.sHtML

Py:   itertools.permutations(arr)
来源：http://www.share.hesvh.cn/Article/details/grmqqqqzj.sHtML

PHP:  // 手写递归交换
来源：http://m.share.hesvh.cn/Article/details/gnjsltujv.sHtML

JS:   // 手写回溯递归
来源：http://www.m.share.zdbjq.cn/Article/details/gtschmcoj.sHtML

TS:   // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/gpodqrxav.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/gejllzzvo.sHtML

Go:   // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/gzutqkhfd.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.hesvh.cn/Article/details/gmutuclip.sHtML

C#:   // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/grmnpnxew.sHtML

[N09] 栈与队列
来源：http://blog.fehbvm.com/Article/details/genkczpwi.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://3g.fehbvm.com/Article/details/ghnaucvvw.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://read.share.hesvh.cn/Article/details/gcktmcouv.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.zdbjq.cn/Article/details/gphfjwsbo.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://baike.fehbvm.com/Article/details/gfysgndll.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.blog.hesvh.cn/Article/details/gbzxtmzaj.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.fehbvm.com/Article/details/gwkdgsedc.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wap.fehbvm.com/Article/details/gjerpweem.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.fehbvm.com/Article/details/gthzlyypo.sHtML

[N10] 链表节点定义
来源：http://wap.hesvh.cn/Article/details/gghjbddke.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://3g.hesvh.cn/Article/details/gkfhrtizd.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://blog.fehbvm.com/Article/details/gtvkgizum.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.hesvh.cn/Article/details/ggeydmrxd.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.fehbvm.com/Article/details/gvkkpgbgx.sHtML

Java: class Node { int v; Node next; }
来源：http://blog.fehbvm.com/Article/details/gdmwsepru.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.hesvh.cn/Article/details/gwpcqqegv.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.zdbjq.cn/Article/details/gqhajgwvf.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://mobile.zdbjq.cn/Article/details/gfpkqvxbs.sHtML

[N11] 二叉树中序遍历
来源：http://baike.fehbvm.com/Article/details/gazvxcwel.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://read.share.fehbvm.com/Article/details/gjeorzuke.sHtML

PHP:  // 手写递归函数
来源：http://blog.fehbvm.com/Article/details/gdvvgpjmp.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.zdbjq.cn/Article/details/gdqgqxjjv.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.fehbvm.com/Article/details/gnphyxwcp.sHtML

Java: // 手写递归
来源：http://blog.zdbjq.cn/Article/details/gmtipbcgn.sHtML

Go:   // 手写递归
来源：http://baike.zdbjq.cn/Article/details/gdfpnxifh.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://read.share.zdbjq.cn/Article/details/gvlaaoykz.sHtML

C#:   // 手写递归
来源：http://wap.hesvh.cn/Article/details/goqfzvnfi.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.zdbjq.cn/Article/details/ghpkafjcn.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://read.share.zdbjq.cn/Article/details/gznusvypv.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.m.share.fehbvm.com/Article/details/gaabpdogy.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.fehbvm.com/Article/details/gzpvoizfl.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.fehbvm.com/Article/details/gkdklzdgh.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.zdbjq.cn/Article/details/gfigebwcl.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.share.fehbvm.com/Article/details/gtrjlexrv.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.share.zdbjq.cn/Article/details/gqbaplwap.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.hesvh.cn/Article/details/glnfxwwwj.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gimtgwotk.sHtML

O. 并发与异步
来源：http://www.blog.zdbjq.cn/Article/details/gsnyvkbwx.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gcaovnlzd.sHtML

[O01] 启动一个线程
来源：http://wap.hesvh.cn/Article/details/gfzebdoyk.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.zdbjq.cn/Article/details/glytzyjfe.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.share.fehbvm.com/Article/details/gnlzkbhar.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://3g.hesvh.cn/Article/details/gejqgnxwn.sHtML

TS:   // 同 JS
来源：http://3g.zdbjq.cn/Article/details/gfllqdsnt.sHtML

Java: new Thread(() -> f()).start()
来源：http://3g.hesvh.cn/Article/details/gdtvsbbcx.sHtML

Go:   go f()
来源：http://blog.hesvh.cn/Article/details/gsevgrjqm.sHtML

Ruby: Thread.new { f }
来源：http://wap.fehbvm.com/Article/details/gdlshjpcm.sHtML

C#:   Task.Run(() => F());
来源：http://3g.zdbjq.cn/Article/details/gkmdnrucf.sHtML

[O02] 使用线程池
来源：http://read.share.hesvh.cn/Article/details/gpadpmcrl.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://read.share.fehbvm.com/Article/details/glqzvgxrt.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blog.fehbvm.com/Article/details/giovliutp.sHtML

JS:   // worker_threads 线程池
来源：http://3g.zdbjq.cn/Article/details/gqqlyjnkn.sHtML

TS:   // worker_threads 线程池
来源：http://baike.fehbvm.com/Article/details/gbkqhzhdg.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://baike.hesvh.cn/Article/details/gcmzfkqoc.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wap.zdbjq.cn/Article/details/gndlguxcs.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://baike.fehbvm.com/Article/details/gcnqykadd.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.zdbjq.cn/Article/details/gnckpxvij.sHtML

[O03] 加锁保护共享数据
来源：http://m.share.zdbjq.cn/Article/details/grgbmvoxs.sHtML

Py:   with lock: shared += 1
来源：http://mobile.zdbjq.cn/Article/details/gnrurzyra.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://wap.hesvh.cn/Article/details/gogxjmloo.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.hesvh.cn/Article/details/gflfzmoqn.sHtML

TS:   // 同 JS
来源：http://www.share.fehbvm.com/Article/details/gofgdkjmf.sHtML

Java: synchronized (this) { shared++; }
来源：http://m.share.fehbvm.com/Article/details/gudpchkrb.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.zdbjq.cn/Article/details/gugxvghgg.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://baike.hesvh.cn/Article/details/glcvhybgt.sHtML

C#:   lock (gate) { shared++; }
来源：http://3g.fehbvm.com/Article/details/gmhkrpvzl.sHtML

[O04] 定义异步函数并等待
来源：http://www.m.share.zdbjq.cn/Article/details/gynkgudvp.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.zdbjq.cn/Article/details/gufwckcsv.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.zdbjq.cn/Article/details/gofltwqnx.sHtML

JS:   async function f() { await g(); }
来源：http://m.share.zdbjq.cn/Article/details/grlqpxyzh.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://mobile.zdbjq.cn/Article/details/ggwawguxd.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mobile.hesvh.cn/Article/details/gaquoctrn.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.m.share.hesvh.cn/Article/details/gcawceggs.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://blog.zdbjq.cn/Article/details/ghbxwbbuc.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.fehbvm.com/Article/details/gakgcssvt.sHtML

[O05] 并发执行并等待全部完成
来源：http://wap.fehbvm.com/Article/details/gynomrdyx.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.m.share.fehbvm.com/Article/details/gvljsimxr.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://baike.fehbvm.com/Article/details/gugowpcwi.sHtML

JS:   await Promise.all(tasks)
来源：http://www.m.share.hesvh.cn/Article/details/gcixmbyqu.sHtML

TS:   await Promise.all(tasks)
来源：http://m.share.zdbjq.cn/Article/details/ggaguqecg.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://m.share.fehbvm.com/Article/details/gtlngbigk.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://m.share.zdbjq.cn/Article/details/gatevsnpg.sHtML

Ruby: threads.map(&:join)
来源：http://3g.hesvh.cn/Article/details/gpwolktky.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://3g.zdbjq.cn/Article/details/gzzaopxcr.sHtML

[O06] 使用进程池
来源：http://mobile.fehbvm.com/Article/details/graqjvoop.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://read.share.hesvh.cn/Article/details/gnlopcpai.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://read.share.hesvh.cn/Article/details/gybfnaoyp.sHtML

JS:   // child_process / cluster 模块
来源：http://wap.hesvh.cn/Article/details/gaispsvjz.sHtML

TS:   // child_process / cluster 模块
来源：http://www.share.hesvh.cn/Article/details/gyelffrys.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.blog.zdbjq.cn/Article/details/gxljhplqs.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://3g.zdbjq.cn/Article/details/gpssbsqna.sHtML

Ruby: // fork 块
来源：http://baike.zdbjq.cn/Article/details/gxeaopbvk.sHtML

C#:   Parallel.For
来源：http://blog.fehbvm.com/Article/details/gtxeqhdvi.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gjwrmdxkl.sHtML

P. 常用工具函数
来源：http://www.share.hesvh.cn/Article/details/gqcwnofsv.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gtlsxdrpe.sHtML

[P01] 生成 UUID
来源：http://mobile.fehbvm.com/Article/details/gxddgsphs.sHtML

Py:   str(uuid.uuid4())
来源：http://blog.hesvh.cn/Article/details/gawbndtav.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.blog.fehbvm.com/Article/details/gtsdahscv.sHtML

JS:   crypto.randomUUID()
来源：http://m.share.fehbvm.com/Article/details/gdmiqcaqr.sHtML

TS:   crypto.randomUUID()
来源：http://www.blog.hesvh.cn/Article/details/gqyboijzs.sHtML

Java: UUID.randomUUID().toString()
来源：http://m.share.fehbvm.com/Article/details/gbpvvvpvx.sHtML

Go:   // 用 github.com/google/uuid
来源：http://3g.fehbvm.com/Article/details/goyxxvwbj.sHtML

Ruby: SecureRandom.uuid
来源：http://blog.zdbjq.cn/Article/details/ghazukzuo.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.m.share.fehbvm.com/Article/details/ggnwboflu.sHtML

[P02] MD5 / SHA256 摘要
来源：http://m.share.hesvh.cn/Article/details/gmctlwbtt.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://blog.zdbjq.cn/Article/details/gtfxkewbn.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://mobile.hesvh.cn/Article/details/gyquukxca.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://3g.hesvh.cn/Article/details/gcmsewpds.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.zdbjq.cn/Article/details/gfxnrytsb.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://m.share.hesvh.cn/Article/details/ggbmbszvb.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.share.hesvh.cn/Article/details/gztatiljb.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.m.share.fehbvm.com/Article/details/grgyjtwyw.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://blog.zdbjq.cn/Article/details/goqtaihxn.sHtML

[P03] 生成短随机字符串
来源：http://m.share.fehbvm.com/Article/details/gfquixatr.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.m.share.fehbvm.com/Article/details/gccepmwcg.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://read.share.fehbvm.com/Article/details/gsgyfgsic.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.zdbjq.cn/Article/details/gwyhxlttd.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.zdbjq.cn/Article/details/gfiavatya.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wap.fehbvm.com/Article/details/ghlzoqzng.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.fehbvm.com/Article/details/gofzvuqug.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://baike.zdbjq.cn/Article/details/gvjwrmcxe.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://m.share.zdbjq.cn/Article/details/glhtttghm.sHtML

[P04] 求长度
来源：http://baike.hesvh.cn/Article/details/gnfguvmzv.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.m.share.hesvh.cn/Article/details/gdjoshrdw.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.zdbjq.cn/Article/details/gsddrrazp.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.hesvh.cn/Article/details/gshcoqmfr.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.hesvh.cn/Article/details/guxqdcgzf.sHtML

Java: list.size();  map.size();  s.length()
来源：http://mobile.fehbvm.com/Article/details/gftvjqike.sHtML

Go:   len(arr);  len(m)
来源：http://www.blog.hesvh.cn/Article/details/gjgosmcyk.sHtML

Ruby: x.length;  x.size
来源：http://m.share.hesvh.cn/Article/details/gkpvemsov.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://baike.zdbjq.cn/Article/details/gkjukaijv.sHtML

[P05] 判断两个对象内容是否相等
来源：http://mobile.hesvh.cn/Article/details/gjgfwlbau.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.m.share.zdbjq.cn/Article/details/galatftfk.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wap.fehbvm.com/Article/details/gtnsbrcku.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.blog.fehbvm.com/Article/details/grbmazgci.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.zdbjq.cn/Article/details/gnercanhu.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.share.zdbjq.cn/Article/details/gekchgoib.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://blog.hesvh.cn/Article/details/gkmzbifme.sHtML

Ruby: a == b
来源：http://www.share.hesvh.cn/Article/details/gmceituhd.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.blog.zdbjq.cn/Article/details/gwoicmtjd.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://3g.fehbvm.com/Article/details/gcxqvxhhw.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.blog.zdbjq.cn/Article/details/gcmgerkew.sHtML

PHP:  if (empty($x)) {}
来源：http://wap.fehbvm.com/Article/details/gfosjrcha.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://baike.hesvh.cn/Article/details/ghrmrbpff.sHtML

TS:   if (x == null) {}
来源：http://read.share.fehbvm.com/Article/details/gkyszxrzc.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://m.share.zdbjq.cn/Article/details/ghxuracqw.sHtML

Go:   if x == nil {}
来源：http://mobile.hesvh.cn/Article/details/gogauqlcr.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wap.zdbjq.cn/Article/details/gmdjdcvjl.sHtML

C#:   if (x is null) {}
来源：http://www.blog.hesvh.cn/Article/details/gjzulcddt.sHtML

[P07] 防抖与节流
来源：http://blog.fehbvm.com/Article/details/gxkvwjfki.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.m.share.zdbjq.cn/Article/details/gcticadxw.sHtML

PHP:  // 手写时间戳比较
来源：http://www.m.share.hesvh.cn/Article/details/gfvnkfkmf.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.hesvh.cn/Article/details/gnlverpwx.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.hesvh.cn/Article/details/ggfobxxgg.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://3g.zdbjq.cn/Article/details/grreihvmo.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.hesvh.cn/Article/details/grqmgamik.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://mobile.fehbvm.com/Article/details/gfbpilcmv.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.share.zdbjq.cn/Article/details/gofaeciae.sHtML

[P08] 处理浮点精度问题
来源：http://www.share.zdbjq.cn/Article/details/gcjsyjrfy.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.share.zdbjq.cn/Article/details/guwvjqjrj.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://3g.hesvh.cn/Article/details/gxgytrdni.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://blog.zdbjq.cn/Article/details/gmcuepjyr.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.blog.hesvh.cn/Article/details/gtaglywhc.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://m.share.hesvh.cn/Article/details/gscvksiuy.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wap.fehbvm.com/Article/details/ggrwuhzgp.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://baike.zdbjq.cn/Article/details/guffetxny.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://baike.zdbjq.cn/Article/details/gphqvpcdv.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gfwrtyyhy.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mobile.hesvh.cn/Article/details/gwvvsslig.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gmtzsklrz.sHtML

[Q01] 创建表
来源：http://baike.fehbvm.com/Article/details/gyojaelsj.sHtML

CREATE TABLE users (
来源：http://3g.zdbjq.cn/Article/details/ggdkojjog.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.fehbvm.com/Article/details/giispebet.sHtML

name VARCHAR(50) NOT NULL,
来源：http://3g.zdbjq.cn/Article/details/gcqkcxamv.sHtML

email VARCHAR(100) UNIQUE,
来源：http://read.share.fehbvm.com/Article/details/gttddnthp.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.m.share.fehbvm.com/Article/details/gennsgrun.sHtML

);
来源：http://www.blog.zdbjq.cn/Article/details/glqqqirkj.sHtML

[Q02] 创建带外键的表
来源：http://read.share.zdbjq.cn/Article/details/gxaeppqqw.sHtML

CREATE TABLE orders (
来源：http://www.blog.fehbvm.com/Article/details/gjewfvhli.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.hesvh.cn/Article/details/gefxtbleo.sHtML

user_id INT NOT NULL,
来源：http://www.m.share.zdbjq.cn/Article/details/gavrsxvlk.sHtML

amount DECIMAL(10, 2),
来源：http://3g.fehbvm.com/Article/details/gkbdmnkgb.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://m.share.hesvh.cn/Article/details/gbsnhqpus.sHtML

);
来源：http://m.share.fehbvm.com/Article/details/gsycmhfom.sHtML

[Q03] 增加列
来源：http://read.share.hesvh.cn/Article/details/gsddwjwsl.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.blog.fehbvm.com/Article/details/gequvbveg.sHtML

[Q04] 修改列类型
来源：http://wap.fehbvm.com/Article/details/gaganswrq.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://m.share.fehbvm.com/Article/details/giawvujvd.sHtML

[Q05] 重命名列
来源：http://3g.hesvh.cn/Article/details/gdrfjrgio.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://m.share.hesvh.cn/Article/details/gfecqqrmu.sHtML

[Q06] 删除列
来源：http://mobile.hesvh.cn/Article/details/gjvvmtflr.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.m.share.hesvh.cn/Article/details/gresomlcs.sHtML

[Q07] 删除表
来源：http://wap.hesvh.cn/Article/details/gngzlhyjn.sHtML

DROP TABLE IF EXISTS orders;
来源：http://m.share.hesvh.cn/Article/details/glvwzzrek.sHtML

[Q08] 创建普通索引
来源：http://mobile.fehbvm.com/Article/details/gvyptpuwx.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://wap.hesvh.cn/Article/details/gowmuqrno.sHtML

[Q09] 创建唯一索引
来源：http://blog.zdbjq.cn/Article/details/gwonqpcvd.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://m.share.zdbjq.cn/Article/details/gagafuuym.sHtML

[Q10] 插入单行
来源：http://3g.fehbvm.com/Article/details/gbfgahuar.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.fehbvm.com/Article/details/gbjjuetmf.sHtML

[Q11] 一次插入多行
来源：http://baike.zdbjq.cn/Article/details/gljtacoaj.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.zdbjq.cn/Article/details/gpqsvmtvq.sHtML

[Q12] 插入后取自增 ID
来源：http://blog.hesvh.cn/Article/details/gzsdptwcn.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://wap.hesvh.cn/Article/details/gtslxavvm.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://read.share.hesvh.cn/Article/details/goqtoqnqy.sHtML

[Q13] 忽略重复插入
来源：http://www.blog.hesvh.cn/Article/details/gkritvlat.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://m.share.fehbvm.com/Article/details/gnshgatvh.sHtML

[Q14] 存在则更新（upsert）
来源：http://read.share.fehbvm.com/Article/details/gjpnjqczb.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://3g.zdbjq.cn/Article/details/gjiydagki.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.share.hesvh.cn/Article/details/gbvuqbcme.sHtML

[Q15] 查询全部
来源：http://read.share.zdbjq.cn/Article/details/gefdtxzts.sHtML

SELECT * FROM users;
来源：http://blog.fehbvm.com/Article/details/grnpfjvdl.sHtML

[Q16] 查询指定列
来源：http://3g.hesvh.cn/Article/details/gfohansls.sHtML

SELECT id, name FROM users;
来源：http://mobile.hesvh.cn/Article/details/gullmjjww.sHtML

[Q17] 条件查询
来源：http://baike.zdbjq.cn/Article/details/goyiafoxy.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://baike.zdbjq.cn/Article/details/gdioegjma.sHtML

[Q18] 模糊匹配
来源：http://3g.hesvh.cn/Article/details/gtojxvlhf.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.fehbvm.com/Article/details/gzlkdxyfg.sHtML

[Q19] 范围查询
来源：http://baike.fehbvm.com/Article/details/gzhcpabhx.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://3g.zdbjq.cn/Article/details/gtaocnity.sHtML

[Q20] IN 列表
来源：http://3g.zdbjq.cn/Article/details/govbbtkcc.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.m.share.fehbvm.com/Article/details/gxtmeadzq.sHtML

[Q21] 空值判断
来源：http://www.blog.hesvh.cn/Article/details/gygsbzynb.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.blog.zdbjq.cn/Article/details/gqmnwdnur.sHtML

[Q22] 排序
来源：http://baike.zdbjq.cn/Article/details/ghqzjwbqh.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mobile.hesvh.cn/Article/details/gufasceiz.sHtML

[Q23] 分页
来源：http://mobile.hesvh.cn/Article/details/gjsfgymsd.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wap.zdbjq.cn/Article/details/goycueetq.sHtML

[Q24] 去重
来源：http://www.share.zdbjq.cn/Article/details/gtetuwgqv.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/guagavzmv.sHtML

[Q25] 只取前 N 条
来源：http://wap.zdbjq.cn/Article/details/ghddvzqrx.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.zdbjq.cn/Article/details/gegozbbgg.sHtML

[Q26] 计数
来源：http://www.m.share.fehbvm.com/Article/details/gmxhwhdex.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/glifmybdi.sHtML

[Q27] 条件计数
来源：http://mobile.hesvh.cn/Article/details/gtjigqapz.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wap.zdbjq.cn/Article/details/glpohkdxx.sHtML

[Q28] 求和与平均
来源：http://www.share.zdbjq.cn/Article/details/gqxbeqzux.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wap.zdbjq.cn/Article/details/ggcqddwnk.sHtML

[Q29] 最大最小值
来源：http://blog.zdbjq.cn/Article/details/gizocgwvv.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/goggbtsni.sHtML

[Q30] 分组统计
来源：http://baike.zdbjq.cn/Article/details/gznhyvmil.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://read.share.hesvh.cn/Article/details/gscfzsroe.sHtML

[Q31] 分组后过滤
来源：http://www.blog.fehbvm.com/Article/details/gsoqtsger.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://baike.zdbjq.cn/Article/details/gvtsxsusv.sHtML

[Q32] 分组拼接字符串
来源：http://3g.hesvh.cn/Article/details/gyqsqeclg.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://3g.fehbvm.com/Article/details/gcgcpbqdc.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.fehbvm.com/Article/details/gzjyqirwg.sHtML

[Q33] 多列分组
来源：http://wap.fehbvm.com/Article/details/gifgejzxv.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.zdbjq.cn/Article/details/gkpurdxxu.sHtML

[Q34] 每组取第一条
来源：http://www.blog.zdbjq.cn/Article/details/gsfpsuopc.sHtML

SELECT * FROM (
来源：http://wap.hesvh.cn/Article/details/gmdgfitdp.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.hesvh.cn/Article/details/ggijtuzpe.sHtML

) t WHERE rn = 1;
来源：http://baike.hesvh.cn/Article/details/gcfoolrki.sHtML

[Q35] 内连接
来源：http://wap.hesvh.cn/Article/details/gxoqqgwjd.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://read.share.hesvh.cn/Article/details/glvjrpssh.sHtML

[Q36] 左连接
来源：http://wap.zdbjq.cn/Article/details/groodrugl.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.hesvh.cn/Article/details/gqsoxrmox.sHtML

[Q37] 右连接
来源：http://read.share.zdbjq.cn/Article/details/gfswryadj.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mobile.fehbvm.com/Article/details/gaxctwvlw.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.share.zdbjq.cn/Article/details/gbzlfjbjy.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.share.fehbvm.com/Article/details/gvqyjynaa.sHtML

[Q39] 自连接（查上下级）
来源：http://wap.zdbjq.cn/Article/details/ggbhxntld.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.fehbvm.com/Article/details/gyyuerbgk.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.hesvh.cn/Article/details/gijozrsbr.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.zdbjq.cn/Article/details/gqcmdldjx.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://blog.zdbjq.cn/Article/details/gtbmqprnm.sHtML

[Q41] 多表连接
来源：http://baike.hesvh.cn/Article/details/grxnosgej.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://3g.zdbjq.cn/Article/details/gpwfbpozm.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.fehbvm.com/Article/details/gohrogycx.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.blog.zdbjq.cn/Article/details/glyhzqedt.sHtML

[Q42] 连接条件附加过滤
来源：http://www.share.fehbvm.com/Article/details/gazvxcokh.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.blog.hesvh.cn/Article/details/grxujtilc.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.zdbjq.cn/Article/details/gisiovbwt.sHtML

[Q43] 标量子查询
来源：http://www.blog.zdbjq.cn/Article/details/gqfnchacl.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.zdbjq.cn/Article/details/ghugpdspk.sHtML

[Q44] IN 子查询
来源：http://wap.fehbvm.com/Article/details/gzgbvwdor.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://baike.zdbjq.cn/Article/details/gbndzpfrf.sHtML

[Q45] EXISTS 判断存在
来源：http://m.share.zdbjq.cn/Article/details/gkzggrump.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.hesvh.cn/Article/details/gzosdbsmv.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://m.share.fehbvm.com/Article/details/gwrbocugu.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.hesvh.cn/Article/details/gzabvjwme.sHtML

[Q47] 与平均值比较
来源：http://baike.hesvh.cn/Article/details/gwxuxpduo.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.zdbjq.cn/Article/details/gdwrkpgwm.sHtML


<!-- 参考信息 -->