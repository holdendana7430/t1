代发 wailian999

Py:   itertools.permutations(arr)
来源：http://m.share.hesvh.cn/Article/details/gwwampyop.sHtML

PHP:  // 手写递归交换
来源：http://mobile.hesvh.cn/Article/details/gzhdifhgf.sHtML

JS:   // 手写回溯递归
来源：http://www.blog.fehbvm.com/Article/details/gfkdthdht.sHtML

TS:   // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/ggxofwbcg.sHtML

Java: // 手写回溯递归
来源：http://read.share.hesvh.cn/Article/details/gsvhjsblf.sHtML

Go:   // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/gcecnwxru.sHtML

Ruby: arr.permutation.to_a
来源：http://www.blog.hesvh.cn/Article/details/gucjztfbe.sHtML

C#:   // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/ghuvvpalk.sHtML

[N09] 栈与队列
来源：http://www.blog.hesvh.cn/Article/details/gzerxvyxp.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://read.share.zdbjq.cn/Article/details/gdkfmsxiw.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://m.share.zdbjq.cn/Article/details/grkllwvyz.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://3g.zdbjq.cn/Article/details/gxflqthqq.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://blog.zdbjq.cn/Article/details/gqqbxrfsl.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://3g.hesvh.cn/Article/details/gclqwcrpa.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://m.share.zdbjq.cn/Article/details/gfcgplabw.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.blog.hesvh.cn/Article/details/gmgkxzhtu.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.hesvh.cn/Article/details/gbmdpxtrk.sHtML

[N10] 链表节点定义
来源：http://baike.zdbjq.cn/Article/details/gpmuliqdq.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.zdbjq.cn/Article/details/gpuqpctxu.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://blog.hesvh.cn/Article/details/glokrdvsu.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mobile.hesvh.cn/Article/details/gchqyajzs.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.hesvh.cn/Article/details/gbdomuskz.sHtML

Java: class Node { int v; Node next; }
来源：http://3g.fehbvm.com/Article/details/gvoqshcgk.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://3g.zdbjq.cn/Article/details/gzlvpzwoq.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.m.share.zdbjq.cn/Article/details/gpnqtsjry.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://read.share.fehbvm.com/Article/details/getchwsas.sHtML

[N11] 二叉树中序遍历
来源：http://www.share.zdbjq.cn/Article/details/gjwzqpyqi.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.share.fehbvm.com/Article/details/gjlkrpfay.sHtML

PHP:  // 手写递归函数
来源：http://baike.zdbjq.cn/Article/details/gtmakxmja.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.fehbvm.com/Article/details/gztrftzcq.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.hesvh.cn/Article/details/gyvaezzfh.sHtML

Java: // 手写递归
来源：http://baike.fehbvm.com/Article/details/glafkwvjy.sHtML

Go:   // 手写递归
来源：http://m.share.fehbvm.com/Article/details/gddknkqml.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://m.share.hesvh.cn/Article/details/glcdrfmvp.sHtML

C#:   // 手写递归
来源：http://read.share.hesvh.cn/Article/details/ggxlpbscn.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://read.share.zdbjq.cn/Article/details/gwsscthxt.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.blog.zdbjq.cn/Article/details/gtavoltgq.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.m.share.hesvh.cn/Article/details/geamhplhl.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.zdbjq.cn/Article/details/ghpurcjfj.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.zdbjq.cn/Article/details/gvmgaocjd.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.zdbjq.cn/Article/details/gzeboweds.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.fehbvm.com/Article/details/gnbwwksgu.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.hesvh.cn/Article/details/gxstsgznu.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.zdbjq.cn/Article/details/gkxqoioam.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/ghvqlinpa.sHtML

O. 并发与异步
来源：http://read.share.zdbjq.cn/Article/details/gryuybkxv.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/ggniyhwgn.sHtML

[O01] 启动一个线程
来源：http://read.share.hesvh.cn/Article/details/gxrxqqobz.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://blog.zdbjq.cn/Article/details/gvriysbbk.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.blog.fehbvm.com/Article/details/gpvlkjgfp.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.zdbjq.cn/Article/details/gauiowkir.sHtML

TS:   // 同 JS
来源：http://m.share.fehbvm.com/Article/details/ggutlxova.sHtML

Java: new Thread(() -> f()).start()
来源：http://baike.fehbvm.com/Article/details/guodvepqn.sHtML

Go:   go f()
来源：http://baike.hesvh.cn/Article/details/gmshzgzqn.sHtML

Ruby: Thread.new { f }
来源：http://www.blog.fehbvm.com/Article/details/gtixlenkj.sHtML

C#:   Task.Run(() => F());
来源：http://www.m.share.hesvh.cn/Article/details/gjrjbbdsv.sHtML

[O02] 使用线程池
来源：http://m.share.fehbvm.com/Article/details/ghxkeyvyw.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://m.share.zdbjq.cn/Article/details/gfjspjkzl.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mobile.hesvh.cn/Article/details/gyltdbfai.sHtML

JS:   // worker_threads 线程池
来源：http://www.blog.hesvh.cn/Article/details/gwzdyugwg.sHtML

TS:   // worker_threads 线程池
来源：http://read.share.hesvh.cn/Article/details/gcutlntnh.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.m.share.hesvh.cn/Article/details/gkzrspkvl.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mobile.hesvh.cn/Article/details/gmwkdmdoo.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://read.share.hesvh.cn/Article/details/gynarydjx.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://baike.zdbjq.cn/Article/details/gawfmmjmb.sHtML

[O03] 加锁保护共享数据
来源：http://3g.zdbjq.cn/Article/details/gvorjhkak.sHtML

Py:   with lock: shared += 1
来源：http://read.share.hesvh.cn/Article/details/gmjxqzfrz.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://wap.hesvh.cn/Article/details/gduxftcmp.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wap.zdbjq.cn/Article/details/gegnfxnbi.sHtML

TS:   // 同 JS
来源：http://read.share.hesvh.cn/Article/details/gertoohwf.sHtML

Java: synchronized (this) { shared++; }
来源：http://read.share.hesvh.cn/Article/details/gdeiknrft.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wap.hesvh.cn/Article/details/ghwpgwtqh.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.zdbjq.cn/Article/details/gytlthmob.sHtML

C#:   lock (gate) { shared++; }
来源：http://wap.fehbvm.com/Article/details/gcxgegkdl.sHtML

[O04] 定义异步函数并等待
来源：http://m.share.fehbvm.com/Article/details/gqgxtwogp.sHtML

Py:   async def f():⏎    await g()
来源：http://read.share.zdbjq.cn/Article/details/gpjotxbro.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.zdbjq.cn/Article/details/gmpyiczms.sHtML

JS:   async function f() { await g(); }
来源：http://baike.fehbvm.com/Article/details/gpubgpwzf.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://m.share.hesvh.cn/Article/details/gscgdktkj.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.share.fehbvm.com/Article/details/grzogqozv.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://m.share.zdbjq.cn/Article/details/gfckarxum.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.hesvh.cn/Article/details/gxlyauhdl.sHtML

C#:   async Task F() { await G(); }
来源：http://www.share.hesvh.cn/Article/details/gypoxgmmd.sHtML

[O05] 并发执行并等待全部完成
来源：http://wap.hesvh.cn/Article/details/gnfxxwbzu.sHtML

Py:   asyncio.gather(*tasks)
来源：http://wap.zdbjq.cn/Article/details/gnrfsbyvx.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://baike.zdbjq.cn/Article/details/gbixkndni.sHtML

JS:   await Promise.all(tasks)
来源：http://baike.hesvh.cn/Article/details/gaedgqzxl.sHtML

TS:   await Promise.all(tasks)
来源：http://read.share.zdbjq.cn/Article/details/gmzllorrv.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://read.share.hesvh.cn/Article/details/gdorozoww.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://read.share.zdbjq.cn/Article/details/ghecwlnod.sHtML

Ruby: threads.map(&:join)
来源：http://blog.zdbjq.cn/Article/details/gitaijqjn.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://read.share.zdbjq.cn/Article/details/ggvjkpflg.sHtML

[O06] 使用进程池
来源：http://www.m.share.zdbjq.cn/Article/details/gdsvjoldu.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.share.fehbvm.com/Article/details/gtnnwyivy.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://blog.fehbvm.com/Article/details/givvomaan.sHtML

JS:   // child_process / cluster 模块
来源：http://www.blog.fehbvm.com/Article/details/gqamodydr.sHtML

TS:   // child_process / cluster 模块
来源：http://www.m.share.hesvh.cn/Article/details/gbwppqmio.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://blog.zdbjq.cn/Article/details/gboizejlc.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.hesvh.cn/Article/details/gdculyoql.sHtML

Ruby: // fork 块
来源：http://3g.hesvh.cn/Article/details/gvuzzaqik.sHtML

C#:   Parallel.For
来源：http://www.m.share.fehbvm.com/Article/details/gkaizuvyh.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gkwftfleg.sHtML

P. 常用工具函数
来源：http://baike.fehbvm.com/Article/details/ghbigqqhf.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gktfktwjo.sHtML

[P01] 生成 UUID
来源：http://baike.zdbjq.cn/Article/details/gmpgkqifj.sHtML

Py:   str(uuid.uuid4())
来源：http://www.blog.hesvh.cn/Article/details/gloixrfzq.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://m.share.fehbvm.com/Article/details/gimdfipfr.sHtML

JS:   crypto.randomUUID()
来源：http://baike.fehbvm.com/Article/details/grkyksgvz.sHtML

TS:   crypto.randomUUID()
来源：http://m.share.hesvh.cn/Article/details/gmgeejahq.sHtML

Java: UUID.randomUUID().toString()
来源：http://mobile.fehbvm.com/Article/details/gpiipydjk.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.m.share.hesvh.cn/Article/details/gvsylumpp.sHtML

Ruby: SecureRandom.uuid
来源：http://www.share.fehbvm.com/Article/details/gujbfaihp.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://baike.hesvh.cn/Article/details/gqihuojhm.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.hesvh.cn/Article/details/gxtnrixva.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.share.zdbjq.cn/Article/details/gbifttimy.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://read.share.zdbjq.cn/Article/details/gqskffrei.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.m.share.zdbjq.cn/Article/details/gtgjfwcmo.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.share.hesvh.cn/Article/details/gsgtjxgxx.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://read.share.fehbvm.com/Article/details/gcdbnirrk.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://baike.fehbvm.com/Article/details/guduymmvd.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://m.share.hesvh.cn/Article/details/glkdkdlkc.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://baike.zdbjq.cn/Article/details/ggyuvabno.sHtML

[P03] 生成短随机字符串
来源：http://wap.hesvh.cn/Article/details/gmvwmdnxd.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://m.share.hesvh.cn/Article/details/gmaeddcit.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://3g.hesvh.cn/Article/details/gvyswtirv.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.hesvh.cn/Article/details/gzaolcsim.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.zdbjq.cn/Article/details/gxbpayibx.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.blog.zdbjq.cn/Article/details/ghttvjlrn.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://3g.hesvh.cn/Article/details/gdfznsaby.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.m.share.hesvh.cn/Article/details/gvsywkzuk.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mobile.hesvh.cn/Article/details/gtkhqxxyl.sHtML

[P04] 求长度
来源：http://read.share.zdbjq.cn/Article/details/gokzfsjhb.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://read.share.fehbvm.com/Article/details/gariehhex.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.zdbjq.cn/Article/details/gxlutztqb.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.zdbjq.cn/Article/details/gcojeypfh.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.hesvh.cn/Article/details/gqtaiufyw.sHtML

Java: list.size();  map.size();  s.length()
来源：http://wap.zdbjq.cn/Article/details/gvqhhwwow.sHtML

Go:   len(arr);  len(m)
来源：http://baike.fehbvm.com/Article/details/goarmrdji.sHtML

Ruby: x.length;  x.size
来源：http://www.m.share.zdbjq.cn/Article/details/gnrgswpgb.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://3g.hesvh.cn/Article/details/gblbtwbkd.sHtML

[P05] 判断两个对象内容是否相等
来源：http://m.share.fehbvm.com/Article/details/gccecjflr.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://blog.fehbvm.com/Article/details/gexpbbtzs.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://read.share.fehbvm.com/Article/details/ggtmkppfv.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mobile.zdbjq.cn/Article/details/gobafzsza.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.fehbvm.com/Article/details/guabdshmc.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://m.share.zdbjq.cn/Article/details/gzadlyaiw.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://read.share.zdbjq.cn/Article/details/gjxpobzgb.sHtML

Ruby: a == b
来源：http://blog.hesvh.cn/Article/details/grwlljzms.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wap.hesvh.cn/Article/details/grjtxxccs.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.share.fehbvm.com/Article/details/gdsdobgws.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.blog.fehbvm.com/Article/details/gofrxiqaf.sHtML

PHP:  if (empty($x)) {}
来源：http://baike.zdbjq.cn/Article/details/gekricvda.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://blog.fehbvm.com/Article/details/giykjdcni.sHtML

TS:   if (x == null) {}
来源：http://www.share.zdbjq.cn/Article/details/gzuqighdo.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://3g.zdbjq.cn/Article/details/gsmhkhczi.sHtML

Go:   if x == nil {}
来源：http://blog.zdbjq.cn/Article/details/gkmfdzesh.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wap.fehbvm.com/Article/details/gjnnbhdsa.sHtML

C#:   if (x is null) {}
来源：http://read.share.fehbvm.com/Article/details/genhhmura.sHtML

[P07] 防抖与节流
来源：http://read.share.fehbvm.com/Article/details/glrvsmlci.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wap.fehbvm.com/Article/details/gdksogjym.sHtML

PHP:  // 手写时间戳比较
来源：http://www.share.zdbjq.cn/Article/details/gvxftfwui.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.hesvh.cn/Article/details/gqmlsusjw.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.zdbjq.cn/Article/details/ggujlynpu.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://blog.hesvh.cn/Article/details/gzmkagarr.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mobile.zdbjq.cn/Article/details/gsgmtshrv.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://wap.zdbjq.cn/Article/details/gqfhkhelk.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.blog.hesvh.cn/Article/details/gbgqtinfw.sHtML

[P08] 处理浮点精度问题
来源：http://www.share.hesvh.cn/Article/details/gldkapqty.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mobile.fehbvm.com/Article/details/gocyhhxtj.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.blog.fehbvm.com/Article/details/gxxsnhupq.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mobile.hesvh.cn/Article/details/gxdrakxob.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mobile.zdbjq.cn/Article/details/gwptdhfam.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wap.hesvh.cn/Article/details/gykyrryls.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://3g.hesvh.cn/Article/details/gvejswywj.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.m.share.zdbjq.cn/Article/details/gamkhjrac.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.blog.zdbjq.cn/Article/details/gphkmflkh.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gcbeqvvki.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://read.share.zdbjq.cn/Article/details/gtngyyyuo.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gjwanbkwf.sHtML

[Q01] 创建表
来源：http://wap.hesvh.cn/Article/details/gedmcjgoh.sHtML

CREATE TABLE users (
来源：http://read.share.zdbjq.cn/Article/details/ghoiutupm.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.fehbvm.com/Article/details/gvbntpyri.sHtML

name VARCHAR(50) NOT NULL,
来源：http://baike.hesvh.cn/Article/details/ghygqgyxx.sHtML

email VARCHAR(100) UNIQUE,
来源：http://read.share.fehbvm.com/Article/details/gbvlbibbl.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://m.share.hesvh.cn/Article/details/gcxqdworv.sHtML

);
来源：http://www.m.share.fehbvm.com/Article/details/geivgvrbw.sHtML

[Q02] 创建带外键的表
来源：http://3g.hesvh.cn/Article/details/grdxlyood.sHtML

CREATE TABLE orders (
来源：http://m.share.hesvh.cn/Article/details/gowavnxmi.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.zdbjq.cn/Article/details/gppkocfys.sHtML

user_id INT NOT NULL,
来源：http://read.share.zdbjq.cn/Article/details/gsmzmeoso.sHtML

amount DECIMAL(10, 2),
来源：http://www.share.fehbvm.com/Article/details/grygrshkf.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.share.zdbjq.cn/Article/details/gtgcljqko.sHtML

);
来源：http://www.blog.fehbvm.com/Article/details/gfnvyllpd.sHtML

[Q03] 增加列
来源：http://www.m.share.hesvh.cn/Article/details/geelimvvq.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.zdbjq.cn/Article/details/gsyirawxg.sHtML

[Q04] 修改列类型
来源：http://www.share.fehbvm.com/Article/details/giqkzpsii.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://blog.fehbvm.com/Article/details/gdswudswq.sHtML

[Q05] 重命名列
来源：http://www.blog.zdbjq.cn/Article/details/gtitngsyj.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.share.zdbjq.cn/Article/details/gjemsrqol.sHtML

[Q06] 删除列
来源：http://www.m.share.zdbjq.cn/Article/details/gortgsncl.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.share.hesvh.cn/Article/details/giyausaty.sHtML

[Q07] 删除表
来源：http://wap.zdbjq.cn/Article/details/gvvkyvina.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.blog.fehbvm.com/Article/details/gvugfwtrr.sHtML

[Q08] 创建普通索引
来源：http://www.blog.fehbvm.com/Article/details/gyfdxwisf.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://read.share.fehbvm.com/Article/details/gcsjmulor.sHtML

[Q09] 创建唯一索引
来源：http://www.m.share.zdbjq.cn/Article/details/gazlshtly.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.share.zdbjq.cn/Article/details/gfyyqxjxv.sHtML

[Q10] 插入单行
来源：http://baike.hesvh.cn/Article/details/gxzzigqzl.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wap.zdbjq.cn/Article/details/gftdflxwm.sHtML

[Q11] 一次插入多行
来源：http://m.share.hesvh.cn/Article/details/gfxslzfdr.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://m.share.zdbjq.cn/Article/details/gyqgafxzm.sHtML

[Q12] 插入后取自增 ID
来源：http://www.share.hesvh.cn/Article/details/gjnczsifd.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://read.share.hesvh.cn/Article/details/ggaiqaigp.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://baike.zdbjq.cn/Article/details/ggelckzmc.sHtML

[Q13] 忽略重复插入
来源：http://mobile.fehbvm.com/Article/details/gqzgqanju.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.zdbjq.cn/Article/details/gabsdnhyn.sHtML

[Q14] 存在则更新（upsert）
来源：http://read.share.hesvh.cn/Article/details/gxrrmcydz.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mobile.zdbjq.cn/Article/details/ghuhzryxo.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mobile.hesvh.cn/Article/details/gpoqompcx.sHtML

[Q15] 查询全部
来源：http://www.blog.hesvh.cn/Article/details/gnpqfrrll.sHtML

SELECT * FROM users;
来源：http://mobile.fehbvm.com/Article/details/gmbpgqpoy.sHtML

[Q16] 查询指定列
来源：http://mobile.hesvh.cn/Article/details/gskuvjaua.sHtML

SELECT id, name FROM users;
来源：http://3g.zdbjq.cn/Article/details/gsejajidj.sHtML

[Q17] 条件查询
来源：http://3g.zdbjq.cn/Article/details/grruhcpez.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.blog.fehbvm.com/Article/details/gmmgguwgm.sHtML

[Q18] 模糊匹配
来源：http://m.share.zdbjq.cn/Article/details/guihohwow.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wap.zdbjq.cn/Article/details/gxhyueegy.sHtML

[Q19] 范围查询
来源：http://blog.hesvh.cn/Article/details/gnpvdrxok.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://blog.zdbjq.cn/Article/details/gotdocdql.sHtML

[Q20] IN 列表
来源：http://baike.fehbvm.com/Article/details/gsgyqcyhm.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.fehbvm.com/Article/details/gypybilyi.sHtML

[Q21] 空值判断
来源：http://read.share.fehbvm.com/Article/details/gnvdzquxc.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.share.hesvh.cn/Article/details/gojuhuyfe.sHtML

[Q22] 排序
来源：http://3g.fehbvm.com/Article/details/gaiyyblns.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.fehbvm.com/Article/details/gjgutloxr.sHtML

[Q23] 分页
来源：http://blog.fehbvm.com/Article/details/gefintftm.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://blog.fehbvm.com/Article/details/gdodcdbrb.sHtML

[Q24] 去重
来源：http://m.share.hesvh.cn/Article/details/gbcyepuqe.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gduwfgprx.sHtML

[Q25] 只取前 N 条
来源：http://wap.hesvh.cn/Article/details/gjzbnspyi.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.fehbvm.com/Article/details/gzlivqabu.sHtML

[Q26] 计数
来源：http://baike.hesvh.cn/Article/details/gusqfjcwa.sHtML

SELECT COUNT(*) FROM users;
来源：http://mobile.fehbvm.com/Article/details/gihxnrofd.sHtML

[Q27] 条件计数
来源：http://www.share.fehbvm.com/Article/details/graketaxq.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gcpggnrbq.sHtML

[Q28] 求和与平均
来源：http://www.m.share.hesvh.cn/Article/details/gxwkmzzmt.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://3g.zdbjq.cn/Article/details/gscwfhftl.sHtML

[Q29] 最大最小值
来源：http://www.m.share.hesvh.cn/Article/details/gsfzjrcob.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://m.share.fehbvm.com/Article/details/gqjoelmfp.sHtML

[Q30] 分组统计
来源：http://baike.hesvh.cn/Article/details/gyzojoghp.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.hesvh.cn/Article/details/gfkkonagt.sHtML

[Q31] 分组后过滤
来源：http://mobile.fehbvm.com/Article/details/gwuiffyha.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.zdbjq.cn/Article/details/gqvhgmkxh.sHtML

[Q32] 分组拼接字符串
来源：http://mobile.fehbvm.com/Article/details/ggjeqyuvw.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.blog.zdbjq.cn/Article/details/gzvlzznxy.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wap.zdbjq.cn/Article/details/gzdswwmyl.sHtML

[Q33] 多列分组
来源：http://baike.fehbvm.com/Article/details/ggcyclfxv.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://baike.fehbvm.com/Article/details/gxrwuvkhl.sHtML

[Q34] 每组取第一条
来源：http://baike.zdbjq.cn/Article/details/grxmpjuko.sHtML

SELECT * FROM (
来源：http://mobile.zdbjq.cn/Article/details/gzzjlictm.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mobile.fehbvm.com/Article/details/grjfbhnhm.sHtML

) t WHERE rn = 1;
来源：http://www.share.hesvh.cn/Article/details/gnoqmjxqr.sHtML

[Q35] 内连接
来源：http://mobile.hesvh.cn/Article/details/gywfglbjw.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://m.share.zdbjq.cn/Article/details/gghuwqcrk.sHtML

[Q36] 左连接
来源：http://baike.fehbvm.com/Article/details/gioswyjgb.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.share.hesvh.cn/Article/details/gqlekvcvo.sHtML

[Q37] 右连接
来源：http://www.m.share.fehbvm.com/Article/details/gyezctiwc.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.share.fehbvm.com/Article/details/gmxuswkmp.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://wap.hesvh.cn/Article/details/gqagtyoiv.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://baike.zdbjq.cn/Article/details/gmkyhlpaq.sHtML

[Q39] 自连接（查上下级）
来源：http://www.blog.hesvh.cn/Article/details/gqmunqjxk.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://read.share.zdbjq.cn/Article/details/gwblnyruq.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.zdbjq.cn/Article/details/ganyvqwsg.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.hesvh.cn/Article/details/gxwxciscn.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.hesvh.cn/Article/details/gmhjibien.sHtML

[Q41] 多表连接
来源：http://www.share.zdbjq.cn/Article/details/glgmjuxlz.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.fehbvm.com/Article/details/gbaqsyyng.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.fehbvm.com/Article/details/gysddbebg.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.hesvh.cn/Article/details/giujtnexr.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.zdbjq.cn/Article/details/ggxtdrzua.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.share.hesvh.cn/Article/details/gjhwgclpt.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://read.share.fehbvm.com/Article/details/gazvzepzz.sHtML

[Q43] 标量子查询
来源：http://www.share.hesvh.cn/Article/details/gjtwpgpal.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.fehbvm.com/Article/details/gefnkjpsj.sHtML

[Q44] IN 子查询
来源：http://www.share.zdbjq.cn/Article/details/gdqdxbwvi.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://m.share.hesvh.cn/Article/details/gvymqzxjl.sHtML

[Q45] EXISTS 判断存在
来源：http://wap.fehbvm.com/Article/details/gmoxsvymm.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.fehbvm.com/Article/details/gbfcupyru.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://blog.hesvh.cn/Article/details/gwikvufhu.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.fehbvm.com/Article/details/gzkutjjyp.sHtML

[Q47] 与平均值比较
来源：http://blog.fehbvm.com/Article/details/gfpjmmiyf.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.share.hesvh.cn/Article/details/gliqevvuu.sHtML

[Q48] CTE 公用表表达式
来源：http://baike.fehbvm.com/Article/details/giqcofqna.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://baike.zdbjq.cn/Article/details/gbrfaknga.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://mobile.zdbjq.cn/Article/details/gggnxoefu.sHtML

[Q49] 更新单行
来源：http://www.share.hesvh.cn/Article/details/gzuvvvmch.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.share.zdbjq.cn/Article/details/gzeweccps.sHtML

[Q50] 批量更新
来源：http://baike.hesvh.cn/Article/details/gxpwzbqus.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.hesvh.cn/Article/details/gqjmwklib.sHtML

[Q51] 用子查询更新
来源：http://www.m.share.zdbjq.cn/Article/details/gwcnoudof.sHtML


<!-- 参考信息 -->